# FABRIC

## Table of Contents

- [Fabric Switches and Management IP](#fabric-switches-and-management-ip)
  - [Fabric Switches with inband Management IP](#fabric-switches-with-inband-management-ip)
- [Fabric Topology](#fabric-topology)
- [Fabric IP Allocation](#fabric-ip-allocation)
  - [Fabric Point-To-Point Links](#fabric-point-to-point-links)
  - [Point-To-Point Links Node Allocation](#point-to-point-links-node-allocation)
  - [Loopback Interfaces (BGP EVPN Peering)](#loopback-interfaces-bgp-evpn-peering)
  - [Loopback0 Interfaces Node Allocation](#loopback0-interfaces-node-allocation)
  - [VTEP Loopback VXLAN Tunnel Source Interfaces (VTEPs Only)](#vtep-loopback-vxlan-tunnel-source-interfaces-vteps-only)
  - [VTEP Loopback Node allocation](#vtep-loopback-node-allocation)

## Fabric Switches and Management IP

| POD | Type | Node | Management IP | Platform | Provisioned in CloudVision | Serial Number |
| --- | ---- | ---- | ------------- | -------- | -------------------------- | ------------- |
| FABRIC | l3leaf | MCI-CTFSTL-BLF03a | 172.18.102.26/24 | veos | Provisioned | - |
| FABRIC | l3leaf | MCI-CTFSTL-BLF03b | 172.18.102.27/24 | veos | Provisioned | - |
| FABRIC | l3leaf | MCI-CTFSTL-LF01a | 172.18.102.22/24 | veos | Provisioned | - |
| FABRIC | l3leaf | MCI-CTFSTL-LF01b | 172.18.102.23/24 | veos | Provisioned | - |
| FABRIC | l3leaf | MCI-CTFSTL-LF02a | 172.18.102.24/24 | veos | Provisioned | - |
| FABRIC | l3leaf | MCI-CTFSTL-LF02b | 172.18.102.25/24 | veos | Provisioned | - |
| FABRIC | spine | MCI-CTFSTL-SP01 | 172.18.102.20/24 | veos | Provisioned | - |
| FABRIC | spine | MCI-CTFSTL-SP02 | 172.18.102.21/24 | veos | Provisioned | - |

> Provision status is based on Ansible inventory declaration and do not represent real status from CloudVision.

### Fabric Switches with inband Management IP

| POD | Type | Node | Management IP | Inband Interface |
| --- | ---- | ---- | ------------- | ---------------- |

## Fabric Topology

| Type | Node | Node Interface | Peer Type | Peer Node | Peer Interface |
| ---- | ---- | -------------- | --------- | ----------| -------------- |
| l3leaf | MCI-CTFSTL-BLF03a | Ethernet49/1 | spine | MCI-CTFSTL-SP01 | Ethernet53/1 |
| l3leaf | MCI-CTFSTL-BLF03a | Ethernet50/1 | spine | MCI-CTFSTL-SP02 | Ethernet54/1 |
| l3leaf | MCI-CTFSTL-BLF03a | Ethernet51/1 | mlag_peer | MCI-CTFSTL-BLF03b | Ethernet51/1 |
| l3leaf | MCI-CTFSTL-BLF03a | Ethernet52/1 | mlag_peer | MCI-CTFSTL-BLF03b | Ethernet52/1 |
| l3leaf | MCI-CTFSTL-BLF03b | Ethernet49/1 | spine | MCI-CTFSTL-SP01 | Ethernet54/1 |
| l3leaf | MCI-CTFSTL-BLF03b | Ethernet50/1 | spine | MCI-CTFSTL-SP02 | Ethernet53/1 |
| l3leaf | MCI-CTFSTL-LF01a | Ethernet49/1 | spine | MCI-CTFSTL-SP01 | Ethernet49/1 |
| l3leaf | MCI-CTFSTL-LF01a | Ethernet50/1 | spine | MCI-CTFSTL-SP02 | Ethernet49/1 |
| l3leaf | MCI-CTFSTL-LF01a | Ethernet51/1 | mlag_peer | MCI-CTFSTL-LF01b | Ethernet51/1 |
| l3leaf | MCI-CTFSTL-LF01a | Ethernet52/1 | mlag_peer | MCI-CTFSTL-LF01b | Ethernet52/1 |
| l3leaf | MCI-CTFSTL-LF01b | Ethernet49/1 | spine | MCI-CTFSTL-SP01 | Ethernet50/1 |
| l3leaf | MCI-CTFSTL-LF01b | Ethernet50/1 | spine | MCI-CTFSTL-SP02 | Ethernet50/1 |
| l3leaf | MCI-CTFSTL-LF02a | Ethernet49/1 | spine | MCI-CTFSTL-SP01 | Ethernet51/1 |
| l3leaf | MCI-CTFSTL-LF02a | Ethernet50/1 | spine | MCI-CTFSTL-SP02 | Ethernet51/1 |
| l3leaf | MCI-CTFSTL-LF02a | Ethernet51/1 | mlag_peer | MCI-CTFSTL-LF02b | Ethernet51/1 |
| l3leaf | MCI-CTFSTL-LF02a | Ethernet52/1 | mlag_peer | MCI-CTFSTL-LF02b | Ethernet52/1 |
| l3leaf | MCI-CTFSTL-LF02b | Ethernet49/1 | spine | MCI-CTFSTL-SP01 | Ethernet52/1 |
| l3leaf | MCI-CTFSTL-LF02b | Ethernet50/1 | spine | MCI-CTFSTL-SP02 | Ethernet52/1 |

## Fabric IP Allocation

### Fabric Point-To-Point Links

| Uplink IPv4 Pool | Available Addresses | Assigned addresses | Assigned Address % |
| ---------------- | ------------------- | ------------------ | ------------------ |
| 10.255.255.0/26 | 64 | 24 | 37.5 % |

### Point-To-Point Links Node Allocation

| Node | Node Interface | Node IP Address | Peer Node | Peer Interface | Peer IP Address |
| ---- | -------------- | --------------- | --------- | -------------- | --------------- |
| MCI-CTFSTL-BLF03a | Ethernet49/1 | 10.255.255.17/31 | MCI-CTFSTL-SP01 | Ethernet53/1 | 10.255.255.16/31 |
| MCI-CTFSTL-BLF03a | Ethernet50/1 | 10.255.255.19/31 | MCI-CTFSTL-SP02 | Ethernet54/1 | 10.255.255.18/31 |
| MCI-CTFSTL-BLF03b | Ethernet49/1 | 10.255.255.21/31 | MCI-CTFSTL-SP01 | Ethernet54/1 | 10.255.255.20/31 |
| MCI-CTFSTL-BLF03b | Ethernet50/1 | 10.255.255.23/31 | MCI-CTFSTL-SP02 | Ethernet53/1 | 10.255.255.22/31 |
| MCI-CTFSTL-LF01a | Ethernet49/1 | 10.255.255.1/31 | MCI-CTFSTL-SP01 | Ethernet49/1 | 10.255.255.0/31 |
| MCI-CTFSTL-LF01a | Ethernet50/1 | 10.255.255.3/31 | MCI-CTFSTL-SP02 | Ethernet49/1 | 10.255.255.2/31 |
| MCI-CTFSTL-LF01b | Ethernet49/1 | 10.255.255.5/31 | MCI-CTFSTL-SP01 | Ethernet50/1 | 10.255.255.4/31 |
| MCI-CTFSTL-LF01b | Ethernet50/1 | 10.255.255.7/31 | MCI-CTFSTL-SP02 | Ethernet50/1 | 10.255.255.6/31 |
| MCI-CTFSTL-LF02a | Ethernet49/1 | 10.255.255.9/31 | MCI-CTFSTL-SP01 | Ethernet51/1 | 10.255.255.8/31 |
| MCI-CTFSTL-LF02a | Ethernet50/1 | 10.255.255.11/31 | MCI-CTFSTL-SP02 | Ethernet51/1 | 10.255.255.10/31 |
| MCI-CTFSTL-LF02b | Ethernet49/1 | 10.255.255.13/31 | MCI-CTFSTL-SP01 | Ethernet52/1 | 10.255.255.12/31 |
| MCI-CTFSTL-LF02b | Ethernet50/1 | 10.255.255.15/31 | MCI-CTFSTL-SP02 | Ethernet52/1 | 10.255.255.14/31 |

### Loopback Interfaces (BGP EVPN Peering)

| Loopback Pool | Available Addresses | Assigned addresses | Assigned Address % |
| ------------- | ------------------- | ------------------ | ------------------ |
| 10.255.0.0/27 | 32 | 8 | 25.0 % |

### Loopback0 Interfaces Node Allocation

| POD | Node | Loopback0 |
| --- | ---- | --------- |
| FABRIC | MCI-CTFSTL-BLF03a | 10.255.0.7/32 |
| FABRIC | MCI-CTFSTL-BLF03b | 10.255.0.8/32 |
| FABRIC | MCI-CTFSTL-LF01a | 10.255.0.3/32 |
| FABRIC | MCI-CTFSTL-LF01b | 10.255.0.4/32 |
| FABRIC | MCI-CTFSTL-LF02a | 10.255.0.5/32 |
| FABRIC | MCI-CTFSTL-LF02b | 10.255.0.6/32 |
| FABRIC | MCI-CTFSTL-SP01 | 10.255.0.1/32 |
| FABRIC | MCI-CTFSTL-SP02 | 10.255.0.2/32 |

### VTEP Loopback VXLAN Tunnel Source Interfaces (VTEPs Only)

| VTEP Loopback Pool | Available Addresses | Assigned addresses | Assigned Address % |
| --------------------- | ------------------- | ------------------ | ------------------ |
| 10.255.1.0/27 | 32 | 6 | 18.75 % |

### VTEP Loopback Node allocation

| POD | Node | Loopback1 |
| --- | ---- | --------- |
| FABRIC | MCI-CTFSTL-BLF03a | 10.255.1.7/32 |
| FABRIC | MCI-CTFSTL-BLF03b | 10.255.1.7/32 |
| FABRIC | MCI-CTFSTL-LF01a | 10.255.1.3/32 |
| FABRIC | MCI-CTFSTL-LF01b | 10.255.1.3/32 |
| FABRIC | MCI-CTFSTL-LF02a | 10.255.1.5/32 |
| FABRIC | MCI-CTFSTL-LF02b | 10.255.1.5/32 |
