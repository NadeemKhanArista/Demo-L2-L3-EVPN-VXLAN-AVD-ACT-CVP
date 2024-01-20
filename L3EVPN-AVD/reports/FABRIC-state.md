# Validate State Report

**Table of Contents:**

- [Validate State Report](validate-state-report)
  - [Test Results Summary](#test-results-summary)
  - [Failed Test Results Summary](#failed-test-results-summary)
  - [All Test Results](#all-test-results)

## Test Results Summary

### Summary Totals

| Total Tests | Total Tests Passed | Total Tests Failed |
| ----------- | ------------------ | ------------------ |
| 484 | 440 | 44 |

### Summary Totals Devices Under Tests

| DUT | Total Tests | Tests Passed | Tests Failed | Categories Failed |
| --- | ----------- | ------------ | ------------ | ----------------- |
| MCI-CTFSTL-BLF03a |  68 | 55 | 13 | NTP, Interface State, LLDP Topology, MLAG, BGP, Routing Table, Loopback0 Reachability |
| MCI-CTFSTL-BLF03b |  68 | 55 | 13 | NTP, Interface State, LLDP Topology, MLAG, BGP, Routing Table, Loopback0 Reachability |
| MCI-CTFSTL-LF01a |  64 | 61 | 3 | NTP, Interface State, LLDP Topology |
| MCI-CTFSTL-LF01b |  64 | 61 | 3 | NTP, Interface State, LLDP Topology |
| MCI-CTFSTL-LF02a |  64 | 63 | 1 | NTP |
| MCI-CTFSTL-LF02b |  64 | 59 | 5 | NTP, Interface State, LLDP Topology, IP Reachability, BGP |
| MCI-CTFSTL-SP01 |  46 | 45 | 1 | NTP |
| MCI-CTFSTL-SP02 |  46 | 41 | 5 | NTP, Interface State, LLDP Topology, IP Reachability, BGP |

### Summary Totals Per Category

| Test Category | Total Tests | Tests Passed | Tests Failed |
| ------------- | ----------- | ------------ | ------------ |
| Hardware |  112 | 112 | 0 |
| NTP |  8 | 0 | 8 |
| Interface State |  122 | 106 | 16 |
| LLDP Topology |  36 | 28 | 8 |
| MLAG |  6 | 4 | 2 |
| IP Reachability |  24 | 22 | 2 |
| BGP |  62 | 58 | 4 |
| Routing Table |  66 | 64 | 2 |
| Loopback0 Reachability |  48 | 46 | 2 |

## Failed Test Results Summary

| Test ID | Node | Test Category | Test Description | Test | Test Result | Failure Reason |
| ------- | ---- | ------------- | ---------------- | ---- | ----------- | -------------- |
| 113 | MCI-CTFSTL-BLF03a | NTP | Synchronised with NTP server | NTP | FAIL | Not synchronised to NTP server |
| 114 | MCI-CTFSTL-BLF03b | NTP | Synchronised with NTP server | NTP | FAIL | Not synchronised to NTP server |
| 115 | MCI-CTFSTL-LF01a | NTP | Synchronised with NTP server | NTP | FAIL | Not synchronised to NTP server |
| 116 | MCI-CTFSTL-LF01b | NTP | Synchronised with NTP server | NTP | FAIL | Not synchronised to NTP server |
| 117 | MCI-CTFSTL-LF02a | NTP | Synchronised with NTP server | NTP | FAIL | Not synchronised to NTP server |
| 118 | MCI-CTFSTL-LF02b | NTP | Synchronised with NTP server | NTP | FAIL | Not synchronised to NTP server |
| 119 | MCI-CTFSTL-SP01 | NTP | Synchronised with NTP server | NTP | FAIL | Not synchronised to NTP server |
| 120 | MCI-CTFSTL-SP02 | NTP | Synchronised with NTP server | NTP | FAIL | Not synchronised to NTP server |
| 121 | MCI-CTFSTL-BLF03a | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet51/1 - MLAG_PEER_MCI-CTFSTL-BLF03b_Ethernet51/1 | FAIL | Interface shutdown: False - interface status: down - line protocol status: down |
| 122 | MCI-CTFSTL-BLF03a | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet52/1 - MLAG_PEER_MCI-CTFSTL-BLF03b_Ethernet52/1 | FAIL | Interface shutdown: False - interface status: down - line protocol status: down |
| 125 | MCI-CTFSTL-BLF03b | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet51/1 - MLAG_PEER_MCI-CTFSTL-BLF03a_Ethernet51/1 | FAIL | Interface shutdown: False - interface status: down - line protocol status: down |
| 126 | MCI-CTFSTL-BLF03b | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet52/1 - MLAG_PEER_MCI-CTFSTL-BLF03a_Ethernet52/1 | FAIL | Interface shutdown: False - interface status: down - line protocol status: down |
| 130 | MCI-CTFSTL-LF01a | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet52/1 - MLAG_PEER_MCI-CTFSTL-LF01b_Ethernet52/1 | FAIL | Interface shutdown: False - interface status: down - line protocol status: down |
| 134 | MCI-CTFSTL-LF01b | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet52/1 - MLAG_PEER_MCI-CTFSTL-LF01a_Ethernet52/1 | FAIL | Interface shutdown: False - interface status: down - line protocol status: down |
| 144 | MCI-CTFSTL-LF02b | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet50/1 - P2P_LINK_TO_MCI-CTFSTL-SP02_Ethernet52/1 | FAIL | Interface shutdown: False - interface status: down - line protocol status: down |
| 154 | MCI-CTFSTL-SP02 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet52/1 - P2P_LINK_TO_MCI-CTFSTL-LF02B_Ethernet50/1 | FAIL | Interface shutdown: False - interface status: down - line protocol status: down |
| 157 | MCI-CTFSTL-BLF03a | Interface State | Port-Channel Interface & Line Protocol == "up" | Port-Channel511 - MLAG_PEER_MCI-CTFSTL-BLF03b_Po511 | FAIL | Interface shutdown: False - interface status: down - line protocol status: lowerLayerDown |
| 158 | MCI-CTFSTL-BLF03b | Interface State | Port-Channel Interface & Line Protocol == "up" | Port-Channel511 - MLAG_PEER_MCI-CTFSTL-BLF03a_Po511 | FAIL | Interface shutdown: False - interface status: down - line protocol status: lowerLayerDown |
| 163 | MCI-CTFSTL-BLF03a | Interface State | Vlan Interface & Line Protocol == "up" | Vlan4093 - MLAG_PEER_L3_PEERING | FAIL | Interface shutdown: False - interface status: down - line protocol status: lowerLayerDown |
| 167 | MCI-CTFSTL-BLF03a | Interface State | Vlan Interface & Line Protocol == "up" | Vlan3009 - MLAG_PEER_L3_iBGP: vrf VRF10 | FAIL | Interface shutdown: False - interface status: down - line protocol status: lowerLayerDown |
| 170 | MCI-CTFSTL-BLF03a | Interface State | Vlan Interface & Line Protocol == "up" | Vlan3010 - MLAG_PEER_L3_iBGP: vrf VRF11 | FAIL | Interface shutdown: False - interface status: down - line protocol status: lowerLayerDown |
| 171 | MCI-CTFSTL-BLF03b | Interface State | Vlan Interface & Line Protocol == "up" | Vlan4093 - MLAG_PEER_L3_PEERING | FAIL | Interface shutdown: False - interface status: down - line protocol status: lowerLayerDown |
| 175 | MCI-CTFSTL-BLF03b | Interface State | Vlan Interface & Line Protocol == "up" | Vlan3009 - MLAG_PEER_L3_iBGP: vrf VRF10 | FAIL | Interface shutdown: False - interface status: down - line protocol status: lowerLayerDown |
| 178 | MCI-CTFSTL-BLF03b | Interface State | Vlan Interface & Line Protocol == "up" | Vlan3010 - MLAG_PEER_L3_iBGP: vrf VRF11 | FAIL | Interface shutdown: False - interface status: down - line protocol status: lowerLayerDown |
| 243 | MCI-CTFSTL-BLF03a | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet51/1 - remote: MCI-CTFSTL-BLF03b_Ethernet51/1 | FAIL | Interface Down - N/A |
| 244 | MCI-CTFSTL-BLF03a | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet52/1 - remote: MCI-CTFSTL-BLF03b_Ethernet52/1 | FAIL | Interface Down - N/A |
| 247 | MCI-CTFSTL-BLF03b | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet51/1 - remote: MCI-CTFSTL-BLF03a_Ethernet51/1 | FAIL | Interface Down - N/A |
| 248 | MCI-CTFSTL-BLF03b | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet52/1 - remote: MCI-CTFSTL-BLF03a_Ethernet52/1 | FAIL | Interface Down - N/A |
| 252 | MCI-CTFSTL-LF01a | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet52/1 - remote: MCI-CTFSTL-LF01b_Ethernet52/1 | FAIL | Interface Down - N/A |
| 256 | MCI-CTFSTL-LF01b | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet52/1 - remote: MCI-CTFSTL-LF01a_Ethernet52/1 | FAIL | Interface Down - N/A |
| 266 | MCI-CTFSTL-LF02b | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet50/1 - remote: MCI-CTFSTL-SP02_Ethernet52/1 | FAIL | Interface Down - N/A |
| 276 | MCI-CTFSTL-SP02 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet52/1 - remote: MCI-CTFSTL-LF02b_Ethernet50/1 | FAIL | Interface Down - N/A |
| 279 | MCI-CTFSTL-BLF03a | MLAG | MLAG State active & Status connected | MLAG | FAIL | State: inactive - Negotiation_status: connecting |
| 280 | MCI-CTFSTL-BLF03b | MLAG | MLAG State active & Status connected | MLAG | FAIL | State: inactive - Negotiation_status: connecting |
| 296 | MCI-CTFSTL-LF02b | IP Reachability | ip reachability test p2p links | Source: MCI-CTFSTL-LF02b_Ethernet50/1 - Destination: MCI-CTFSTL-SP02_Ethernet52/1 | FAIL | 100% packet loss |
| 306 | MCI-CTFSTL-SP02 | IP Reachability | ip reachability test p2p links | Source: MCI-CTFSTL-SP02_Ethernet52/1 - Destination: MCI-CTFSTL-LF02b_Ethernet50/1 | FAIL | 100% packet loss |
| 317 | MCI-CTFSTL-BLF03a | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 10.255.1.105 | FAIL | Session state Active |
| 320 | MCI-CTFSTL-BLF03b | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 10.255.1.104 | FAIL | Session state Active |
| 334 | MCI-CTFSTL-LF02b | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 10.255.255.14 | FAIL | Session state Idle |
| 344 | MCI-CTFSTL-SP02 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 10.255.255.15 | FAIL | Session state Idle |
| 390 | MCI-CTFSTL-BLF03a | Routing Table | Remote Lo0 address | 10.255.0.8 | FAIL | Lo0 10.255.0.8 is not in the routing table |
| 397 | MCI-CTFSTL-BLF03b | Routing Table | Remote Lo0 address | 10.255.0.7 | FAIL | Lo0 10.255.0.7 is not in the routing table |
| 438 | MCI-CTFSTL-BLF03a | Loopback0 Reachability | Loopback0 Reachability | Source: MCI-CTFSTL-BLF03a - 10.255.0.7 Destination: 10.255.0.8 | FAIL | 100% packet loss |
| 445 | MCI-CTFSTL-BLF03b | Loopback0 Reachability | Loopback0 Reachability | Source: MCI-CTFSTL-BLF03b - 10.255.0.8 Destination: 10.255.0.7 | FAIL | 100% packet loss |

## All Test Results

| Test ID | Node | Test Category | Test Description | Test | Test Result | Failure Reason |
| ------- | ---- | ------------- | ---------------- | ---- | ----------- | -------------- |
| 1 | MCI-CTFSTL-BLF03a | Hardware | Power supply status | Power supply 1 | PASS | - |
| 2 | MCI-CTFSTL-BLF03a | Hardware | Power supply status | Power supply 2 | PASS | - |
| 3 | MCI-CTFSTL-BLF03b | Hardware | Power supply status | Power supply 1 | PASS | - |
| 4 | MCI-CTFSTL-BLF03b | Hardware | Power supply status | Power supply 2 | PASS | - |
| 5 | MCI-CTFSTL-LF01a | Hardware | Power supply status | Power supply 1 | PASS | - |
| 6 | MCI-CTFSTL-LF01a | Hardware | Power supply status | Power supply 2 | PASS | - |
| 7 | MCI-CTFSTL-LF01b | Hardware | Power supply status | Power supply 1 | PASS | - |
| 8 | MCI-CTFSTL-LF01b | Hardware | Power supply status | Power supply 2 | PASS | - |
| 9 | MCI-CTFSTL-LF02a | Hardware | Power supply status | Power supply 1 | PASS | - |
| 10 | MCI-CTFSTL-LF02a | Hardware | Power supply status | Power supply 2 | PASS | - |
| 11 | MCI-CTFSTL-LF02b | Hardware | Power supply status | Power supply 1 | PASS | - |
| 12 | MCI-CTFSTL-LF02b | Hardware | Power supply status | Power supply 2 | PASS | - |
| 13 | MCI-CTFSTL-SP01 | Hardware | Power supply status | Power supply 1 | PASS | - |
| 14 | MCI-CTFSTL-SP01 | Hardware | Power supply status | Power supply 2 | PASS | - |
| 15 | MCI-CTFSTL-SP02 | Hardware | Power supply status | Power supply 1 | PASS | - |
| 16 | MCI-CTFSTL-SP02 | Hardware | Power supply status | Power supply 2 | PASS | - |
| 17 | MCI-CTFSTL-BLF03a | Hardware | Fan status (power supplies) | Power supply fan PowerSupply1 | PASS | - |
| 18 | MCI-CTFSTL-BLF03a | Hardware | Fan status (power supplies) | Power supply fan PowerSupply2 | PASS | - |
| 19 | MCI-CTFSTL-BLF03b | Hardware | Fan status (power supplies) | Power supply fan PowerSupply1 | PASS | - |
| 20 | MCI-CTFSTL-BLF03b | Hardware | Fan status (power supplies) | Power supply fan PowerSupply2 | PASS | - |
| 21 | MCI-CTFSTL-LF01a | Hardware | Fan status (power supplies) | Power supply fan PowerSupply1 | PASS | - |
| 22 | MCI-CTFSTL-LF01a | Hardware | Fan status (power supplies) | Power supply fan PowerSupply2 | PASS | - |
| 23 | MCI-CTFSTL-LF01b | Hardware | Fan status (power supplies) | Power supply fan PowerSupply1 | PASS | - |
| 24 | MCI-CTFSTL-LF01b | Hardware | Fan status (power supplies) | Power supply fan PowerSupply2 | PASS | - |
| 25 | MCI-CTFSTL-LF02a | Hardware | Fan status (power supplies) | Power supply fan PowerSupply1 | PASS | - |
| 26 | MCI-CTFSTL-LF02a | Hardware | Fan status (power supplies) | Power supply fan PowerSupply2 | PASS | - |
| 27 | MCI-CTFSTL-LF02b | Hardware | Fan status (power supplies) | Power supply fan PowerSupply1 | PASS | - |
| 28 | MCI-CTFSTL-LF02b | Hardware | Fan status (power supplies) | Power supply fan PowerSupply2 | PASS | - |
| 29 | MCI-CTFSTL-SP01 | Hardware | Fan status (power supplies) | Power supply fan PowerSupply1 | PASS | - |
| 30 | MCI-CTFSTL-SP01 | Hardware | Fan status (power supplies) | Power supply fan PowerSupply2 | PASS | - |
| 31 | MCI-CTFSTL-SP02 | Hardware | Fan status (power supplies) | Power supply fan PowerSupply1 | PASS | - |
| 32 | MCI-CTFSTL-SP02 | Hardware | Fan status (power supplies) | Power supply fan PowerSupply2 | PASS | - |
| 33 | MCI-CTFSTL-BLF03a | Hardware | Fan status (fan tray) | Tray 1 | PASS | - |
| 34 | MCI-CTFSTL-BLF03a | Hardware | Fan status (fan tray) | Tray 2 | PASS | - |
| 35 | MCI-CTFSTL-BLF03b | Hardware | Fan status (fan tray) | Tray 1 | PASS | - |
| 36 | MCI-CTFSTL-BLF03b | Hardware | Fan status (fan tray) | Tray 2 | PASS | - |
| 37 | MCI-CTFSTL-LF01a | Hardware | Fan status (fan tray) | Tray 1 | PASS | - |
| 38 | MCI-CTFSTL-LF01a | Hardware | Fan status (fan tray) | Tray 2 | PASS | - |
| 39 | MCI-CTFSTL-LF01b | Hardware | Fan status (fan tray) | Tray 1 | PASS | - |
| 40 | MCI-CTFSTL-LF01b | Hardware | Fan status (fan tray) | Tray 2 | PASS | - |
| 41 | MCI-CTFSTL-LF02a | Hardware | Fan status (fan tray) | Tray 1 | PASS | - |
| 42 | MCI-CTFSTL-LF02a | Hardware | Fan status (fan tray) | Tray 2 | PASS | - |
| 43 | MCI-CTFSTL-LF02b | Hardware | Fan status (fan tray) | Tray 1 | PASS | - |
| 44 | MCI-CTFSTL-LF02b | Hardware | Fan status (fan tray) | Tray 2 | PASS | - |
| 45 | MCI-CTFSTL-SP01 | Hardware | Fan status (fan tray) | Tray 1 | PASS | - |
| 46 | MCI-CTFSTL-SP01 | Hardware | Fan status (fan tray) | Tray 2 | PASS | - |
| 47 | MCI-CTFSTL-SP02 | Hardware | Fan status (fan tray) | Tray 1 | PASS | - |
| 48 | MCI-CTFSTL-SP02 | Hardware | Fan status (fan tray) | Tray 2 | PASS | - |
| 49 | MCI-CTFSTL-BLF03a | Hardware | Temperature | System temperature | PASS | - |
| 50 | MCI-CTFSTL-BLF03b | Hardware | Temperature | System temperature | PASS | - |
| 51 | MCI-CTFSTL-LF01a | Hardware | Temperature | System temperature | PASS | - |
| 52 | MCI-CTFSTL-LF01b | Hardware | Temperature | System temperature | PASS | - |
| 53 | MCI-CTFSTL-LF02a | Hardware | Temperature | System temperature | PASS | - |
| 54 | MCI-CTFSTL-LF02b | Hardware | Temperature | System temperature | PASS | - |
| 55 | MCI-CTFSTL-SP01 | Hardware | Temperature | System temperature | PASS | - |
| 56 | MCI-CTFSTL-SP02 | Hardware | Temperature | System temperature | PASS | - |
| 57 | MCI-CTFSTL-BLF03a | Hardware | Transceivers manufacturers | Port 7 | PASS | - |
| 58 | MCI-CTFSTL-BLF03a | Hardware | Transceivers manufacturers | Port 9 | PASS | - |
| 59 | MCI-CTFSTL-BLF03a | Hardware | Transceivers manufacturers | Port 8 | PASS | - |
| 60 | MCI-CTFSTL-BLF03a | Hardware | Transceivers manufacturers | Port 10 | PASS | - |
| 61 | MCI-CTFSTL-BLF03a | Hardware | Transceivers manufacturers | Port 54 | PASS | - |
| 62 | MCI-CTFSTL-BLF03a | Hardware | Transceivers manufacturers | Port 49 | PASS | - |
| 63 | MCI-CTFSTL-BLF03a | Hardware | Transceivers manufacturers | Port 51 | PASS | - |
| 64 | MCI-CTFSTL-BLF03a | Hardware | Transceivers manufacturers | Port 53 | PASS | - |
| 65 | MCI-CTFSTL-BLF03a | Hardware | Transceivers manufacturers | Port 52 | PASS | - |
| 66 | MCI-CTFSTL-BLF03a | Hardware | Transceivers manufacturers | Port 50 | PASS | - |
| 67 | MCI-CTFSTL-BLF03b | Hardware | Transceivers manufacturers | Port 7 | PASS | - |
| 68 | MCI-CTFSTL-BLF03b | Hardware | Transceivers manufacturers | Port 9 | PASS | - |
| 69 | MCI-CTFSTL-BLF03b | Hardware | Transceivers manufacturers | Port 8 | PASS | - |
| 70 | MCI-CTFSTL-BLF03b | Hardware | Transceivers manufacturers | Port 10 | PASS | - |
| 71 | MCI-CTFSTL-BLF03b | Hardware | Transceivers manufacturers | Port 54 | PASS | - |
| 72 | MCI-CTFSTL-BLF03b | Hardware | Transceivers manufacturers | Port 49 | PASS | - |
| 73 | MCI-CTFSTL-BLF03b | Hardware | Transceivers manufacturers | Port 51 | PASS | - |
| 74 | MCI-CTFSTL-BLF03b | Hardware | Transceivers manufacturers | Port 53 | PASS | - |
| 75 | MCI-CTFSTL-BLF03b | Hardware | Transceivers manufacturers | Port 52 | PASS | - |
| 76 | MCI-CTFSTL-BLF03b | Hardware | Transceivers manufacturers | Port 50 | PASS | - |
| 77 | MCI-CTFSTL-LF01a | Hardware | Transceivers manufacturers | Port 54 | PASS | - |
| 78 | MCI-CTFSTL-LF01a | Hardware | Transceivers manufacturers | Port 49 | PASS | - |
| 79 | MCI-CTFSTL-LF01a | Hardware | Transceivers manufacturers | Port 51 | PASS | - |
| 80 | MCI-CTFSTL-LF01a | Hardware | Transceivers manufacturers | Port 53 | PASS | - |
| 81 | MCI-CTFSTL-LF01a | Hardware | Transceivers manufacturers | Port 52 | PASS | - |
| 82 | MCI-CTFSTL-LF01a | Hardware | Transceivers manufacturers | Port 50 | PASS | - |
| 83 | MCI-CTFSTL-LF01b | Hardware | Transceivers manufacturers | Port 54 | PASS | - |
| 84 | MCI-CTFSTL-LF01b | Hardware | Transceivers manufacturers | Port 49 | PASS | - |
| 85 | MCI-CTFSTL-LF01b | Hardware | Transceivers manufacturers | Port 51 | PASS | - |
| 86 | MCI-CTFSTL-LF01b | Hardware | Transceivers manufacturers | Port 53 | PASS | - |
| 87 | MCI-CTFSTL-LF01b | Hardware | Transceivers manufacturers | Port 52 | PASS | - |
| 88 | MCI-CTFSTL-LF01b | Hardware | Transceivers manufacturers | Port 50 | PASS | - |
| 89 | MCI-CTFSTL-LF02a | Hardware | Transceivers manufacturers | Port 54 | PASS | - |
| 90 | MCI-CTFSTL-LF02a | Hardware | Transceivers manufacturers | Port 49 | PASS | - |
| 91 | MCI-CTFSTL-LF02a | Hardware | Transceivers manufacturers | Port 51 | PASS | - |
| 92 | MCI-CTFSTL-LF02a | Hardware | Transceivers manufacturers | Port 53 | PASS | - |
| 93 | MCI-CTFSTL-LF02a | Hardware | Transceivers manufacturers | Port 52 | PASS | - |
| 94 | MCI-CTFSTL-LF02a | Hardware | Transceivers manufacturers | Port 50 | PASS | - |
| 95 | MCI-CTFSTL-LF02b | Hardware | Transceivers manufacturers | Port 54 | PASS | - |
| 96 | MCI-CTFSTL-LF02b | Hardware | Transceivers manufacturers | Port 49 | PASS | - |
| 97 | MCI-CTFSTL-LF02b | Hardware | Transceivers manufacturers | Port 51 | PASS | - |
| 98 | MCI-CTFSTL-LF02b | Hardware | Transceivers manufacturers | Port 53 | PASS | - |
| 99 | MCI-CTFSTL-LF02b | Hardware | Transceivers manufacturers | Port 52 | PASS | - |
| 100 | MCI-CTFSTL-LF02b | Hardware | Transceivers manufacturers | Port 50 | PASS | - |
| 101 | MCI-CTFSTL-SP01 | Hardware | Transceivers manufacturers | Port 54 | PASS | - |
| 102 | MCI-CTFSTL-SP01 | Hardware | Transceivers manufacturers | Port 49 | PASS | - |
| 103 | MCI-CTFSTL-SP01 | Hardware | Transceivers manufacturers | Port 51 | PASS | - |
| 104 | MCI-CTFSTL-SP01 | Hardware | Transceivers manufacturers | Port 53 | PASS | - |
| 105 | MCI-CTFSTL-SP01 | Hardware | Transceivers manufacturers | Port 52 | PASS | - |
| 106 | MCI-CTFSTL-SP01 | Hardware | Transceivers manufacturers | Port 50 | PASS | - |
| 107 | MCI-CTFSTL-SP02 | Hardware | Transceivers manufacturers | Port 54 | PASS | - |
| 108 | MCI-CTFSTL-SP02 | Hardware | Transceivers manufacturers | Port 49 | PASS | - |
| 109 | MCI-CTFSTL-SP02 | Hardware | Transceivers manufacturers | Port 51 | PASS | - |
| 110 | MCI-CTFSTL-SP02 | Hardware | Transceivers manufacturers | Port 53 | PASS | - |
| 111 | MCI-CTFSTL-SP02 | Hardware | Transceivers manufacturers | Port 52 | PASS | - |
| 112 | MCI-CTFSTL-SP02 | Hardware | Transceivers manufacturers | Port 50 | PASS | - |
| 113 | MCI-CTFSTL-BLF03a | NTP | Synchronised with NTP server | NTP | FAIL | Not synchronised to NTP server |
| 114 | MCI-CTFSTL-BLF03b | NTP | Synchronised with NTP server | NTP | FAIL | Not synchronised to NTP server |
| 115 | MCI-CTFSTL-LF01a | NTP | Synchronised with NTP server | NTP | FAIL | Not synchronised to NTP server |
| 116 | MCI-CTFSTL-LF01b | NTP | Synchronised with NTP server | NTP | FAIL | Not synchronised to NTP server |
| 117 | MCI-CTFSTL-LF02a | NTP | Synchronised with NTP server | NTP | FAIL | Not synchronised to NTP server |
| 118 | MCI-CTFSTL-LF02b | NTP | Synchronised with NTP server | NTP | FAIL | Not synchronised to NTP server |
| 119 | MCI-CTFSTL-SP01 | NTP | Synchronised with NTP server | NTP | FAIL | Not synchronised to NTP server |
| 120 | MCI-CTFSTL-SP02 | NTP | Synchronised with NTP server | NTP | FAIL | Not synchronised to NTP server |
| 121 | MCI-CTFSTL-BLF03a | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet51/1 - MLAG_PEER_MCI-CTFSTL-BLF03b_Ethernet51/1 | FAIL | Interface shutdown: False - interface status: down - line protocol status: down |
| 122 | MCI-CTFSTL-BLF03a | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet52/1 - MLAG_PEER_MCI-CTFSTL-BLF03b_Ethernet52/1 | FAIL | Interface shutdown: False - interface status: down - line protocol status: down |
| 123 | MCI-CTFSTL-BLF03a | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet49/1 - P2P_LINK_TO_MCI-CTFSTL-SP01_Ethernet53/1 | PASS | - |
| 124 | MCI-CTFSTL-BLF03a | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet50/1 - P2P_LINK_TO_MCI-CTFSTL-SP02_Ethernet53/1 | PASS | - |
| 125 | MCI-CTFSTL-BLF03b | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet51/1 - MLAG_PEER_MCI-CTFSTL-BLF03a_Ethernet51/1 | FAIL | Interface shutdown: False - interface status: down - line protocol status: down |
| 126 | MCI-CTFSTL-BLF03b | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet52/1 - MLAG_PEER_MCI-CTFSTL-BLF03a_Ethernet52/1 | FAIL | Interface shutdown: False - interface status: down - line protocol status: down |
| 127 | MCI-CTFSTL-BLF03b | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet49/1 - P2P_LINK_TO_MCI-CTFSTL-SP01_Ethernet54/1 | PASS | - |
| 128 | MCI-CTFSTL-BLF03b | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet50/1 - P2P_LINK_TO_MCI-CTFSTL-SP02_Ethernet54/1 | PASS | - |
| 129 | MCI-CTFSTL-LF01a | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet51/1 - MLAG_PEER_MCI-CTFSTL-LF01b_Ethernet51/1 | PASS | - |
| 130 | MCI-CTFSTL-LF01a | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet52/1 - MLAG_PEER_MCI-CTFSTL-LF01b_Ethernet52/1 | FAIL | Interface shutdown: False - interface status: down - line protocol status: down |
| 131 | MCI-CTFSTL-LF01a | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet49/1 - P2P_LINK_TO_MCI-CTFSTL-SP01_Ethernet49/1 | PASS | - |
| 132 | MCI-CTFSTL-LF01a | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet50/1 - P2P_LINK_TO_MCI-CTFSTL-SP02_Ethernet49/1 | PASS | - |
| 133 | MCI-CTFSTL-LF01b | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet51/1 - MLAG_PEER_MCI-CTFSTL-LF01a_Ethernet51/1 | PASS | - |
| 134 | MCI-CTFSTL-LF01b | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet52/1 - MLAG_PEER_MCI-CTFSTL-LF01a_Ethernet52/1 | FAIL | Interface shutdown: False - interface status: down - line protocol status: down |
| 135 | MCI-CTFSTL-LF01b | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet49/1 - P2P_LINK_TO_MCI-CTFSTL-SP01_Ethernet50/1 | PASS | - |
| 136 | MCI-CTFSTL-LF01b | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet50/1 - P2P_LINK_TO_MCI-CTFSTL-SP02_Ethernet50/1 | PASS | - |
| 137 | MCI-CTFSTL-LF02a | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet51/1 - MLAG_PEER_MCI-CTFSTL-LF02b_Ethernet51/1 | PASS | - |
| 138 | MCI-CTFSTL-LF02a | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet52/1 - MLAG_PEER_MCI-CTFSTL-LF02b_Ethernet52/1 | PASS | - |
| 139 | MCI-CTFSTL-LF02a | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet49/1 - P2P_LINK_TO_MCI-CTFSTL-SP01_Ethernet51/1 | PASS | - |
| 140 | MCI-CTFSTL-LF02a | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet50/1 - P2P_LINK_TO_MCI-CTFSTL-SP02_Ethernet51/1 | PASS | - |
| 141 | MCI-CTFSTL-LF02b | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet51/1 - MLAG_PEER_MCI-CTFSTL-LF02a_Ethernet51/1 | PASS | - |
| 142 | MCI-CTFSTL-LF02b | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet52/1 - MLAG_PEER_MCI-CTFSTL-LF02a_Ethernet52/1 | PASS | - |
| 143 | MCI-CTFSTL-LF02b | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet49/1 - P2P_LINK_TO_MCI-CTFSTL-SP01_Ethernet52/1 | PASS | - |
| 144 | MCI-CTFSTL-LF02b | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet50/1 - P2P_LINK_TO_MCI-CTFSTL-SP02_Ethernet52/1 | FAIL | Interface shutdown: False - interface status: down - line protocol status: down |
| 145 | MCI-CTFSTL-SP01 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet49/1 - P2P_LINK_TO_MCI-CTFSTL-LF01A_Ethernet49/1 | PASS | - |
| 146 | MCI-CTFSTL-SP01 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet50/1 - P2P_LINK_TO_MCI-CTFSTL-LF01B_Ethernet49/1 | PASS | - |
| 147 | MCI-CTFSTL-SP01 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet51/1 - P2P_LINK_TO_MCI-CTFSTL-LF02A_Ethernet49/1 | PASS | - |
| 148 | MCI-CTFSTL-SP01 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet52/1 - P2P_LINK_TO_MCI-CTFSTL-LF02B_Ethernet49/1 | PASS | - |
| 149 | MCI-CTFSTL-SP01 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet53/1 - P2P_LINK_TO_MCI-CTFSTL-BLF03A_Ethernet49/1 | PASS | - |
| 150 | MCI-CTFSTL-SP01 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet54/1 - P2P_LINK_TO_MCI-CTFSTL-BLF03B_Ethernet49/1 | PASS | - |
| 151 | MCI-CTFSTL-SP02 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet49/1 - P2P_LINK_TO_MCI-CTFSTL-LF01A_Ethernet50/1 | PASS | - |
| 152 | MCI-CTFSTL-SP02 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet50/1 - P2P_LINK_TO_MCI-CTFSTL-LF01B_Ethernet50/1 | PASS | - |
| 153 | MCI-CTFSTL-SP02 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet51/1 - P2P_LINK_TO_MCI-CTFSTL-LF02A_Ethernet50/1 | PASS | - |
| 154 | MCI-CTFSTL-SP02 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet52/1 - P2P_LINK_TO_MCI-CTFSTL-LF02B_Ethernet50/1 | FAIL | Interface shutdown: False - interface status: down - line protocol status: down |
| 155 | MCI-CTFSTL-SP02 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet53/1 - P2P_LINK_TO_MCI-CTFSTL-BLF03A_Ethernet50/1 | PASS | - |
| 156 | MCI-CTFSTL-SP02 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet54/1 - P2P_LINK_TO_MCI-CTFSTL-BLF03B_Ethernet50/1 | PASS | - |
| 157 | MCI-CTFSTL-BLF03a | Interface State | Port-Channel Interface & Line Protocol == "up" | Port-Channel511 - MLAG_PEER_MCI-CTFSTL-BLF03b_Po511 | FAIL | Interface shutdown: False - interface status: down - line protocol status: lowerLayerDown |
| 158 | MCI-CTFSTL-BLF03b | Interface State | Port-Channel Interface & Line Protocol == "up" | Port-Channel511 - MLAG_PEER_MCI-CTFSTL-BLF03a_Po511 | FAIL | Interface shutdown: False - interface status: down - line protocol status: lowerLayerDown |
| 159 | MCI-CTFSTL-LF01a | Interface State | Port-Channel Interface & Line Protocol == "up" | Port-Channel511 - MLAG_PEER_MCI-CTFSTL-LF01b_Po511 | PASS | - |
| 160 | MCI-CTFSTL-LF01b | Interface State | Port-Channel Interface & Line Protocol == "up" | Port-Channel511 - MLAG_PEER_MCI-CTFSTL-LF01a_Po511 | PASS | - |
| 161 | MCI-CTFSTL-LF02a | Interface State | Port-Channel Interface & Line Protocol == "up" | Port-Channel511 - MLAG_PEER_MCI-CTFSTL-LF02b_Po511 | PASS | - |
| 162 | MCI-CTFSTL-LF02b | Interface State | Port-Channel Interface & Line Protocol == "up" | Port-Channel511 - MLAG_PEER_MCI-CTFSTL-LF02a_Po511 | PASS | - |
| 163 | MCI-CTFSTL-BLF03a | Interface State | Vlan Interface & Line Protocol == "up" | Vlan4093 - MLAG_PEER_L3_PEERING | FAIL | Interface shutdown: False - interface status: down - line protocol status: lowerLayerDown |
| 164 | MCI-CTFSTL-BLF03a | Interface State | Vlan Interface & Line Protocol == "up" | Vlan4094 - MLAG_PEER | PASS | - |
| 165 | MCI-CTFSTL-BLF03a | Interface State | Vlan Interface & Line Protocol == "up" | Vlan11 - VRF10_VLAN11 | PASS | - |
| 166 | MCI-CTFSTL-BLF03a | Interface State | Vlan Interface & Line Protocol == "up" | Vlan12 - VRF10_VLAN12 | PASS | - |
| 167 | MCI-CTFSTL-BLF03a | Interface State | Vlan Interface & Line Protocol == "up" | Vlan3009 - MLAG_PEER_L3_iBGP: vrf VRF10 | FAIL | Interface shutdown: False - interface status: down - line protocol status: lowerLayerDown |
| 168 | MCI-CTFSTL-BLF03a | Interface State | Vlan Interface & Line Protocol == "up" | Vlan21 - VRF11_VLAN21 | PASS | - |
| 169 | MCI-CTFSTL-BLF03a | Interface State | Vlan Interface & Line Protocol == "up" | Vlan22 - VRF11_VLAN22 | PASS | - |
| 170 | MCI-CTFSTL-BLF03a | Interface State | Vlan Interface & Line Protocol == "up" | Vlan3010 - MLAG_PEER_L3_iBGP: vrf VRF11 | FAIL | Interface shutdown: False - interface status: down - line protocol status: lowerLayerDown |
| 171 | MCI-CTFSTL-BLF03b | Interface State | Vlan Interface & Line Protocol == "up" | Vlan4093 - MLAG_PEER_L3_PEERING | FAIL | Interface shutdown: False - interface status: down - line protocol status: lowerLayerDown |
| 172 | MCI-CTFSTL-BLF03b | Interface State | Vlan Interface & Line Protocol == "up" | Vlan4094 - MLAG_PEER | PASS | - |
| 173 | MCI-CTFSTL-BLF03b | Interface State | Vlan Interface & Line Protocol == "up" | Vlan11 - VRF10_VLAN11 | PASS | - |
| 174 | MCI-CTFSTL-BLF03b | Interface State | Vlan Interface & Line Protocol == "up" | Vlan12 - VRF10_VLAN12 | PASS | - |
| 175 | MCI-CTFSTL-BLF03b | Interface State | Vlan Interface & Line Protocol == "up" | Vlan3009 - MLAG_PEER_L3_iBGP: vrf VRF10 | FAIL | Interface shutdown: False - interface status: down - line protocol status: lowerLayerDown |
| 176 | MCI-CTFSTL-BLF03b | Interface State | Vlan Interface & Line Protocol == "up" | Vlan21 - VRF11_VLAN21 | PASS | - |
| 177 | MCI-CTFSTL-BLF03b | Interface State | Vlan Interface & Line Protocol == "up" | Vlan22 - VRF11_VLAN22 | PASS | - |
| 178 | MCI-CTFSTL-BLF03b | Interface State | Vlan Interface & Line Protocol == "up" | Vlan3010 - MLAG_PEER_L3_iBGP: vrf VRF11 | FAIL | Interface shutdown: False - interface status: down - line protocol status: lowerLayerDown |
| 179 | MCI-CTFSTL-LF01a | Interface State | Vlan Interface & Line Protocol == "up" | Vlan4093 - MLAG_PEER_L3_PEERING | PASS | - |
| 180 | MCI-CTFSTL-LF01a | Interface State | Vlan Interface & Line Protocol == "up" | Vlan4094 - MLAG_PEER | PASS | - |
| 181 | MCI-CTFSTL-LF01a | Interface State | Vlan Interface & Line Protocol == "up" | Vlan11 - VRF10_VLAN11 | PASS | - |
| 182 | MCI-CTFSTL-LF01a | Interface State | Vlan Interface & Line Protocol == "up" | Vlan12 - VRF10_VLAN12 | PASS | - |
| 183 | MCI-CTFSTL-LF01a | Interface State | Vlan Interface & Line Protocol == "up" | Vlan3009 - MLAG_PEER_L3_iBGP: vrf VRF10 | PASS | - |
| 184 | MCI-CTFSTL-LF01a | Interface State | Vlan Interface & Line Protocol == "up" | Vlan21 - VRF11_VLAN21 | PASS | - |
| 185 | MCI-CTFSTL-LF01a | Interface State | Vlan Interface & Line Protocol == "up" | Vlan22 - VRF11_VLAN22 | PASS | - |
| 186 | MCI-CTFSTL-LF01a | Interface State | Vlan Interface & Line Protocol == "up" | Vlan3010 - MLAG_PEER_L3_iBGP: vrf VRF11 | PASS | - |
| 187 | MCI-CTFSTL-LF01b | Interface State | Vlan Interface & Line Protocol == "up" | Vlan4093 - MLAG_PEER_L3_PEERING | PASS | - |
| 188 | MCI-CTFSTL-LF01b | Interface State | Vlan Interface & Line Protocol == "up" | Vlan4094 - MLAG_PEER | PASS | - |
| 189 | MCI-CTFSTL-LF01b | Interface State | Vlan Interface & Line Protocol == "up" | Vlan11 - VRF10_VLAN11 | PASS | - |
| 190 | MCI-CTFSTL-LF01b | Interface State | Vlan Interface & Line Protocol == "up" | Vlan12 - VRF10_VLAN12 | PASS | - |
| 191 | MCI-CTFSTL-LF01b | Interface State | Vlan Interface & Line Protocol == "up" | Vlan3009 - MLAG_PEER_L3_iBGP: vrf VRF10 | PASS | - |
| 192 | MCI-CTFSTL-LF01b | Interface State | Vlan Interface & Line Protocol == "up" | Vlan21 - VRF11_VLAN21 | PASS | - |
| 193 | MCI-CTFSTL-LF01b | Interface State | Vlan Interface & Line Protocol == "up" | Vlan22 - VRF11_VLAN22 | PASS | - |
| 194 | MCI-CTFSTL-LF01b | Interface State | Vlan Interface & Line Protocol == "up" | Vlan3010 - MLAG_PEER_L3_iBGP: vrf VRF11 | PASS | - |
| 195 | MCI-CTFSTL-LF02a | Interface State | Vlan Interface & Line Protocol == "up" | Vlan4093 - MLAG_PEER_L3_PEERING | PASS | - |
| 196 | MCI-CTFSTL-LF02a | Interface State | Vlan Interface & Line Protocol == "up" | Vlan4094 - MLAG_PEER | PASS | - |
| 197 | MCI-CTFSTL-LF02a | Interface State | Vlan Interface & Line Protocol == "up" | Vlan11 - VRF10_VLAN11 | PASS | - |
| 198 | MCI-CTFSTL-LF02a | Interface State | Vlan Interface & Line Protocol == "up" | Vlan12 - VRF10_VLAN12 | PASS | - |
| 199 | MCI-CTFSTL-LF02a | Interface State | Vlan Interface & Line Protocol == "up" | Vlan3009 - MLAG_PEER_L3_iBGP: vrf VRF10 | PASS | - |
| 200 | MCI-CTFSTL-LF02a | Interface State | Vlan Interface & Line Protocol == "up" | Vlan21 - VRF11_VLAN21 | PASS | - |
| 201 | MCI-CTFSTL-LF02a | Interface State | Vlan Interface & Line Protocol == "up" | Vlan22 - VRF11_VLAN22 | PASS | - |
| 202 | MCI-CTFSTL-LF02a | Interface State | Vlan Interface & Line Protocol == "up" | Vlan3010 - MLAG_PEER_L3_iBGP: vrf VRF11 | PASS | - |
| 203 | MCI-CTFSTL-LF02b | Interface State | Vlan Interface & Line Protocol == "up" | Vlan4093 - MLAG_PEER_L3_PEERING | PASS | - |
| 204 | MCI-CTFSTL-LF02b | Interface State | Vlan Interface & Line Protocol == "up" | Vlan4094 - MLAG_PEER | PASS | - |
| 205 | MCI-CTFSTL-LF02b | Interface State | Vlan Interface & Line Protocol == "up" | Vlan11 - VRF10_VLAN11 | PASS | - |
| 206 | MCI-CTFSTL-LF02b | Interface State | Vlan Interface & Line Protocol == "up" | Vlan12 - VRF10_VLAN12 | PASS | - |
| 207 | MCI-CTFSTL-LF02b | Interface State | Vlan Interface & Line Protocol == "up" | Vlan3009 - MLAG_PEER_L3_iBGP: vrf VRF10 | PASS | - |
| 208 | MCI-CTFSTL-LF02b | Interface State | Vlan Interface & Line Protocol == "up" | Vlan21 - VRF11_VLAN21 | PASS | - |
| 209 | MCI-CTFSTL-LF02b | Interface State | Vlan Interface & Line Protocol == "up" | Vlan22 - VRF11_VLAN22 | PASS | - |
| 210 | MCI-CTFSTL-LF02b | Interface State | Vlan Interface & Line Protocol == "up" | Vlan3010 - MLAG_PEER_L3_iBGP: vrf VRF11 | PASS | - |
| 211 | MCI-CTFSTL-BLF03a | Interface State | Vxlan Interface Status & Line Protocol == "up" | Vxlan1 | PASS | - |
| 212 | MCI-CTFSTL-BLF03b | Interface State | Vxlan Interface Status & Line Protocol == "up" | Vxlan1 | PASS | - |
| 213 | MCI-CTFSTL-LF01a | Interface State | Vxlan Interface Status & Line Protocol == "up" | Vxlan1 | PASS | - |
| 214 | MCI-CTFSTL-LF01b | Interface State | Vxlan Interface Status & Line Protocol == "up" | Vxlan1 | PASS | - |
| 215 | MCI-CTFSTL-LF02a | Interface State | Vxlan Interface Status & Line Protocol == "up" | Vxlan1 | PASS | - |
| 216 | MCI-CTFSTL-LF02b | Interface State | Vxlan Interface Status & Line Protocol == "up" | Vxlan1 | PASS | - |
| 217 | MCI-CTFSTL-BLF03a | Interface State | Loopback Interface Status & Line Protocol == "up" | Loopback0 - EVPN_Overlay_Peering | PASS | - |
| 218 | MCI-CTFSTL-BLF03a | Interface State | Loopback Interface Status & Line Protocol == "up" | Loopback1 - VTEP_VXLAN_Tunnel_Source | PASS | - |
| 219 | MCI-CTFSTL-BLF03a | Interface State | Loopback Interface Status & Line Protocol == "up" | Loopback10 - VRF10_VTEP_DIAGNOSTICS | PASS | - |
| 220 | MCI-CTFSTL-BLF03a | Interface State | Loopback Interface Status & Line Protocol == "up" | Loopback11 - VRF11_VTEP_DIAGNOSTICS | PASS | - |
| 221 | MCI-CTFSTL-BLF03b | Interface State | Loopback Interface Status & Line Protocol == "up" | Loopback0 - EVPN_Overlay_Peering | PASS | - |
| 222 | MCI-CTFSTL-BLF03b | Interface State | Loopback Interface Status & Line Protocol == "up" | Loopback1 - VTEP_VXLAN_Tunnel_Source | PASS | - |
| 223 | MCI-CTFSTL-BLF03b | Interface State | Loopback Interface Status & Line Protocol == "up" | Loopback10 - VRF10_VTEP_DIAGNOSTICS | PASS | - |
| 224 | MCI-CTFSTL-BLF03b | Interface State | Loopback Interface Status & Line Protocol == "up" | Loopback11 - VRF11_VTEP_DIAGNOSTICS | PASS | - |
| 225 | MCI-CTFSTL-LF01a | Interface State | Loopback Interface Status & Line Protocol == "up" | Loopback0 - EVPN_Overlay_Peering | PASS | - |
| 226 | MCI-CTFSTL-LF01a | Interface State | Loopback Interface Status & Line Protocol == "up" | Loopback1 - VTEP_VXLAN_Tunnel_Source | PASS | - |
| 227 | MCI-CTFSTL-LF01a | Interface State | Loopback Interface Status & Line Protocol == "up" | Loopback10 - VRF10_VTEP_DIAGNOSTICS | PASS | - |
| 228 | MCI-CTFSTL-LF01a | Interface State | Loopback Interface Status & Line Protocol == "up" | Loopback11 - VRF11_VTEP_DIAGNOSTICS | PASS | - |
| 229 | MCI-CTFSTL-LF01b | Interface State | Loopback Interface Status & Line Protocol == "up" | Loopback0 - EVPN_Overlay_Peering | PASS | - |
| 230 | MCI-CTFSTL-LF01b | Interface State | Loopback Interface Status & Line Protocol == "up" | Loopback1 - VTEP_VXLAN_Tunnel_Source | PASS | - |
| 231 | MCI-CTFSTL-LF01b | Interface State | Loopback Interface Status & Line Protocol == "up" | Loopback10 - VRF10_VTEP_DIAGNOSTICS | PASS | - |
| 232 | MCI-CTFSTL-LF01b | Interface State | Loopback Interface Status & Line Protocol == "up" | Loopback11 - VRF11_VTEP_DIAGNOSTICS | PASS | - |
| 233 | MCI-CTFSTL-LF02a | Interface State | Loopback Interface Status & Line Protocol == "up" | Loopback0 - EVPN_Overlay_Peering | PASS | - |
| 234 | MCI-CTFSTL-LF02a | Interface State | Loopback Interface Status & Line Protocol == "up" | Loopback1 - VTEP_VXLAN_Tunnel_Source | PASS | - |
| 235 | MCI-CTFSTL-LF02a | Interface State | Loopback Interface Status & Line Protocol == "up" | Loopback10 - VRF10_VTEP_DIAGNOSTICS | PASS | - |
| 236 | MCI-CTFSTL-LF02a | Interface State | Loopback Interface Status & Line Protocol == "up" | Loopback11 - VRF11_VTEP_DIAGNOSTICS | PASS | - |
| 237 | MCI-CTFSTL-LF02b | Interface State | Loopback Interface Status & Line Protocol == "up" | Loopback0 - EVPN_Overlay_Peering | PASS | - |
| 238 | MCI-CTFSTL-LF02b | Interface State | Loopback Interface Status & Line Protocol == "up" | Loopback1 - VTEP_VXLAN_Tunnel_Source | PASS | - |
| 239 | MCI-CTFSTL-LF02b | Interface State | Loopback Interface Status & Line Protocol == "up" | Loopback10 - VRF10_VTEP_DIAGNOSTICS | PASS | - |
| 240 | MCI-CTFSTL-LF02b | Interface State | Loopback Interface Status & Line Protocol == "up" | Loopback11 - VRF11_VTEP_DIAGNOSTICS | PASS | - |
| 241 | MCI-CTFSTL-SP01 | Interface State | Loopback Interface Status & Line Protocol == "up" | Loopback0 - EVPN_Overlay_Peering | PASS | - |
| 242 | MCI-CTFSTL-SP02 | Interface State | Loopback Interface Status & Line Protocol == "up" | Loopback0 - EVPN_Overlay_Peering | PASS | - |
| 243 | MCI-CTFSTL-BLF03a | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet51/1 - remote: MCI-CTFSTL-BLF03b_Ethernet51/1 | FAIL | Interface Down - N/A |
| 244 | MCI-CTFSTL-BLF03a | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet52/1 - remote: MCI-CTFSTL-BLF03b_Ethernet52/1 | FAIL | Interface Down - N/A |
| 245 | MCI-CTFSTL-BLF03a | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet49/1 - remote: MCI-CTFSTL-SP01_Ethernet53/1 | PASS | - |
| 246 | MCI-CTFSTL-BLF03a | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet50/1 - remote: MCI-CTFSTL-SP02_Ethernet53/1 | PASS | - |
| 247 | MCI-CTFSTL-BLF03b | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet51/1 - remote: MCI-CTFSTL-BLF03a_Ethernet51/1 | FAIL | Interface Down - N/A |
| 248 | MCI-CTFSTL-BLF03b | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet52/1 - remote: MCI-CTFSTL-BLF03a_Ethernet52/1 | FAIL | Interface Down - N/A |
| 249 | MCI-CTFSTL-BLF03b | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet49/1 - remote: MCI-CTFSTL-SP01_Ethernet54/1 | PASS | - |
| 250 | MCI-CTFSTL-BLF03b | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet50/1 - remote: MCI-CTFSTL-SP02_Ethernet54/1 | PASS | - |
| 251 | MCI-CTFSTL-LF01a | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet51/1 - remote: MCI-CTFSTL-LF01b_Ethernet51/1 | PASS | - |
| 252 | MCI-CTFSTL-LF01a | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet52/1 - remote: MCI-CTFSTL-LF01b_Ethernet52/1 | FAIL | Interface Down - N/A |
| 253 | MCI-CTFSTL-LF01a | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet49/1 - remote: MCI-CTFSTL-SP01_Ethernet49/1 | PASS | - |
| 254 | MCI-CTFSTL-LF01a | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet50/1 - remote: MCI-CTFSTL-SP02_Ethernet49/1 | PASS | - |
| 255 | MCI-CTFSTL-LF01b | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet51/1 - remote: MCI-CTFSTL-LF01a_Ethernet51/1 | PASS | - |
| 256 | MCI-CTFSTL-LF01b | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet52/1 - remote: MCI-CTFSTL-LF01a_Ethernet52/1 | FAIL | Interface Down - N/A |
| 257 | MCI-CTFSTL-LF01b | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet49/1 - remote: MCI-CTFSTL-SP01_Ethernet50/1 | PASS | - |
| 258 | MCI-CTFSTL-LF01b | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet50/1 - remote: MCI-CTFSTL-SP02_Ethernet50/1 | PASS | - |
| 259 | MCI-CTFSTL-LF02a | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet51/1 - remote: MCI-CTFSTL-LF02b_Ethernet51/1 | PASS | - |
| 260 | MCI-CTFSTL-LF02a | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet52/1 - remote: MCI-CTFSTL-LF02b_Ethernet52/1 | PASS | - |
| 261 | MCI-CTFSTL-LF02a | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet49/1 - remote: MCI-CTFSTL-SP01_Ethernet51/1 | PASS | - |
| 262 | MCI-CTFSTL-LF02a | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet50/1 - remote: MCI-CTFSTL-SP02_Ethernet51/1 | PASS | - |
| 263 | MCI-CTFSTL-LF02b | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet51/1 - remote: MCI-CTFSTL-LF02a_Ethernet51/1 | PASS | - |
| 264 | MCI-CTFSTL-LF02b | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet52/1 - remote: MCI-CTFSTL-LF02a_Ethernet52/1 | PASS | - |
| 265 | MCI-CTFSTL-LF02b | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet49/1 - remote: MCI-CTFSTL-SP01_Ethernet52/1 | PASS | - |
| 266 | MCI-CTFSTL-LF02b | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet50/1 - remote: MCI-CTFSTL-SP02_Ethernet52/1 | FAIL | Interface Down - N/A |
| 267 | MCI-CTFSTL-SP01 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet49/1 - remote: MCI-CTFSTL-LF01a_Ethernet49/1 | PASS | - |
| 268 | MCI-CTFSTL-SP01 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet50/1 - remote: MCI-CTFSTL-LF01b_Ethernet49/1 | PASS | - |
| 269 | MCI-CTFSTL-SP01 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet51/1 - remote: MCI-CTFSTL-LF02a_Ethernet49/1 | PASS | - |
| 270 | MCI-CTFSTL-SP01 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet52/1 - remote: MCI-CTFSTL-LF02b_Ethernet49/1 | PASS | - |
| 271 | MCI-CTFSTL-SP01 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet53/1 - remote: MCI-CTFSTL-BLF03a_Ethernet49/1 | PASS | - |
| 272 | MCI-CTFSTL-SP01 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet54/1 - remote: MCI-CTFSTL-BLF03b_Ethernet49/1 | PASS | - |
| 273 | MCI-CTFSTL-SP02 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet49/1 - remote: MCI-CTFSTL-LF01a_Ethernet50/1 | PASS | - |
| 274 | MCI-CTFSTL-SP02 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet50/1 - remote: MCI-CTFSTL-LF01b_Ethernet50/1 | PASS | - |
| 275 | MCI-CTFSTL-SP02 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet51/1 - remote: MCI-CTFSTL-LF02a_Ethernet50/1 | PASS | - |
| 276 | MCI-CTFSTL-SP02 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet52/1 - remote: MCI-CTFSTL-LF02b_Ethernet50/1 | FAIL | Interface Down - N/A |
| 277 | MCI-CTFSTL-SP02 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet53/1 - remote: MCI-CTFSTL-BLF03a_Ethernet50/1 | PASS | - |
| 278 | MCI-CTFSTL-SP02 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet54/1 - remote: MCI-CTFSTL-BLF03b_Ethernet50/1 | PASS | - |
| 279 | MCI-CTFSTL-BLF03a | MLAG | MLAG State active & Status connected | MLAG | FAIL | State: inactive - Negotiation_status: connecting |
| 280 | MCI-CTFSTL-BLF03b | MLAG | MLAG State active & Status connected | MLAG | FAIL | State: inactive - Negotiation_status: connecting |
| 281 | MCI-CTFSTL-LF01a | MLAG | MLAG State active & Status connected | MLAG | PASS | - |
| 282 | MCI-CTFSTL-LF01b | MLAG | MLAG State active & Status connected | MLAG | PASS | - |
| 283 | MCI-CTFSTL-LF02a | MLAG | MLAG State active & Status connected | MLAG | PASS | - |
| 284 | MCI-CTFSTL-LF02b | MLAG | MLAG State active & Status connected | MLAG | PASS | - |
| 285 | MCI-CTFSTL-BLF03a | IP Reachability | ip reachability test p2p links | Source: MCI-CTFSTL-BLF03a_Ethernet49/1 - Destination: MCI-CTFSTL-SP01_Ethernet53/1 | PASS | - |
| 286 | MCI-CTFSTL-BLF03a | IP Reachability | ip reachability test p2p links | Source: MCI-CTFSTL-BLF03a_Ethernet50/1 - Destination: MCI-CTFSTL-SP02_Ethernet53/1 | PASS | - |
| 287 | MCI-CTFSTL-BLF03b | IP Reachability | ip reachability test p2p links | Source: MCI-CTFSTL-BLF03b_Ethernet49/1 - Destination: MCI-CTFSTL-SP01_Ethernet54/1 | PASS | - |
| 288 | MCI-CTFSTL-BLF03b | IP Reachability | ip reachability test p2p links | Source: MCI-CTFSTL-BLF03b_Ethernet50/1 - Destination: MCI-CTFSTL-SP02_Ethernet54/1 | PASS | - |
| 289 | MCI-CTFSTL-LF01a | IP Reachability | ip reachability test p2p links | Source: MCI-CTFSTL-LF01a_Ethernet49/1 - Destination: MCI-CTFSTL-SP01_Ethernet49/1 | PASS | - |
| 290 | MCI-CTFSTL-LF01a | IP Reachability | ip reachability test p2p links | Source: MCI-CTFSTL-LF01a_Ethernet50/1 - Destination: MCI-CTFSTL-SP02_Ethernet49/1 | PASS | - |
| 291 | MCI-CTFSTL-LF01b | IP Reachability | ip reachability test p2p links | Source: MCI-CTFSTL-LF01b_Ethernet49/1 - Destination: MCI-CTFSTL-SP01_Ethernet50/1 | PASS | - |
| 292 | MCI-CTFSTL-LF01b | IP Reachability | ip reachability test p2p links | Source: MCI-CTFSTL-LF01b_Ethernet50/1 - Destination: MCI-CTFSTL-SP02_Ethernet50/1 | PASS | - |
| 293 | MCI-CTFSTL-LF02a | IP Reachability | ip reachability test p2p links | Source: MCI-CTFSTL-LF02a_Ethernet49/1 - Destination: MCI-CTFSTL-SP01_Ethernet51/1 | PASS | - |
| 294 | MCI-CTFSTL-LF02a | IP Reachability | ip reachability test p2p links | Source: MCI-CTFSTL-LF02a_Ethernet50/1 - Destination: MCI-CTFSTL-SP02_Ethernet51/1 | PASS | - |
| 295 | MCI-CTFSTL-LF02b | IP Reachability | ip reachability test p2p links | Source: MCI-CTFSTL-LF02b_Ethernet49/1 - Destination: MCI-CTFSTL-SP01_Ethernet52/1 | PASS | - |
| 296 | MCI-CTFSTL-LF02b | IP Reachability | ip reachability test p2p links | Source: MCI-CTFSTL-LF02b_Ethernet50/1 - Destination: MCI-CTFSTL-SP02_Ethernet52/1 | FAIL | 100% packet loss |
| 297 | MCI-CTFSTL-SP01 | IP Reachability | ip reachability test p2p links | Source: MCI-CTFSTL-SP01_Ethernet49/1 - Destination: MCI-CTFSTL-LF01a_Ethernet49/1 | PASS | - |
| 298 | MCI-CTFSTL-SP01 | IP Reachability | ip reachability test p2p links | Source: MCI-CTFSTL-SP01_Ethernet50/1 - Destination: MCI-CTFSTL-LF01b_Ethernet49/1 | PASS | - |
| 299 | MCI-CTFSTL-SP01 | IP Reachability | ip reachability test p2p links | Source: MCI-CTFSTL-SP01_Ethernet51/1 - Destination: MCI-CTFSTL-LF02a_Ethernet49/1 | PASS | - |
| 300 | MCI-CTFSTL-SP01 | IP Reachability | ip reachability test p2p links | Source: MCI-CTFSTL-SP01_Ethernet52/1 - Destination: MCI-CTFSTL-LF02b_Ethernet49/1 | PASS | - |
| 301 | MCI-CTFSTL-SP01 | IP Reachability | ip reachability test p2p links | Source: MCI-CTFSTL-SP01_Ethernet53/1 - Destination: MCI-CTFSTL-BLF03a_Ethernet49/1 | PASS | - |
| 302 | MCI-CTFSTL-SP01 | IP Reachability | ip reachability test p2p links | Source: MCI-CTFSTL-SP01_Ethernet54/1 - Destination: MCI-CTFSTL-BLF03b_Ethernet49/1 | PASS | - |
| 303 | MCI-CTFSTL-SP02 | IP Reachability | ip reachability test p2p links | Source: MCI-CTFSTL-SP02_Ethernet49/1 - Destination: MCI-CTFSTL-LF01a_Ethernet50/1 | PASS | - |
| 304 | MCI-CTFSTL-SP02 | IP Reachability | ip reachability test p2p links | Source: MCI-CTFSTL-SP02_Ethernet50/1 - Destination: MCI-CTFSTL-LF01b_Ethernet50/1 | PASS | - |
| 305 | MCI-CTFSTL-SP02 | IP Reachability | ip reachability test p2p links | Source: MCI-CTFSTL-SP02_Ethernet51/1 - Destination: MCI-CTFSTL-LF02a_Ethernet50/1 | PASS | - |
| 306 | MCI-CTFSTL-SP02 | IP Reachability | ip reachability test p2p links | Source: MCI-CTFSTL-SP02_Ethernet52/1 - Destination: MCI-CTFSTL-LF02b_Ethernet50/1 | FAIL | 100% packet loss |
| 307 | MCI-CTFSTL-SP02 | IP Reachability | ip reachability test p2p links | Source: MCI-CTFSTL-SP02_Ethernet53/1 - Destination: MCI-CTFSTL-BLF03a_Ethernet50/1 | PASS | - |
| 308 | MCI-CTFSTL-SP02 | IP Reachability | ip reachability test p2p links | Source: MCI-CTFSTL-SP02_Ethernet54/1 - Destination: MCI-CTFSTL-BLF03b_Ethernet50/1 | PASS | - |
| 309 | MCI-CTFSTL-BLF03a | BGP | ArBGP is configured and operating | ArBGP | PASS | - |
| 310 | MCI-CTFSTL-BLF03b | BGP | ArBGP is configured and operating | ArBGP | PASS | - |
| 311 | MCI-CTFSTL-LF01a | BGP | ArBGP is configured and operating | ArBGP | PASS | - |
| 312 | MCI-CTFSTL-LF01b | BGP | ArBGP is configured and operating | ArBGP | PASS | - |
| 313 | MCI-CTFSTL-LF02a | BGP | ArBGP is configured and operating | ArBGP | PASS | - |
| 314 | MCI-CTFSTL-LF02b | BGP | ArBGP is configured and operating | ArBGP | PASS | - |
| 315 | MCI-CTFSTL-SP01 | BGP | ArBGP is configured and operating | ArBGP | PASS | - |
| 316 | MCI-CTFSTL-SP02 | BGP | ArBGP is configured and operating | ArBGP | PASS | - |
| 317 | MCI-CTFSTL-BLF03a | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 10.255.1.105 | FAIL | Session state Active |
| 318 | MCI-CTFSTL-BLF03a | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 10.255.255.16 | PASS | - |
| 319 | MCI-CTFSTL-BLF03a | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 10.255.255.18 | PASS | - |
| 320 | MCI-CTFSTL-BLF03b | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 10.255.1.104 | FAIL | Session state Active |
| 321 | MCI-CTFSTL-BLF03b | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 10.255.255.20 | PASS | - |
| 322 | MCI-CTFSTL-BLF03b | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 10.255.255.22 | PASS | - |
| 323 | MCI-CTFSTL-LF01a | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 10.255.1.97 | PASS | - |
| 324 | MCI-CTFSTL-LF01a | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 10.255.255.0 | PASS | - |
| 325 | MCI-CTFSTL-LF01a | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 10.255.255.2 | PASS | - |
| 326 | MCI-CTFSTL-LF01b | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 10.255.1.96 | PASS | - |
| 327 | MCI-CTFSTL-LF01b | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 10.255.255.4 | PASS | - |
| 328 | MCI-CTFSTL-LF01b | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 10.255.255.6 | PASS | - |
| 329 | MCI-CTFSTL-LF02a | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 10.255.1.101 | PASS | - |
| 330 | MCI-CTFSTL-LF02a | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 10.255.255.8 | PASS | - |
| 331 | MCI-CTFSTL-LF02a | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 10.255.255.10 | PASS | - |
| 332 | MCI-CTFSTL-LF02b | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 10.255.1.100 | PASS | - |
| 333 | MCI-CTFSTL-LF02b | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 10.255.255.12 | PASS | - |
| 334 | MCI-CTFSTL-LF02b | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 10.255.255.14 | FAIL | Session state Idle |
| 335 | MCI-CTFSTL-SP01 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 10.255.255.1 | PASS | - |
| 336 | MCI-CTFSTL-SP01 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 10.255.255.5 | PASS | - |
| 337 | MCI-CTFSTL-SP01 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 10.255.255.9 | PASS | - |
| 338 | MCI-CTFSTL-SP01 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 10.255.255.13 | PASS | - |
| 339 | MCI-CTFSTL-SP01 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 10.255.255.17 | PASS | - |
| 340 | MCI-CTFSTL-SP01 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 10.255.255.21 | PASS | - |
| 341 | MCI-CTFSTL-SP02 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 10.255.255.3 | PASS | - |
| 342 | MCI-CTFSTL-SP02 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 10.255.255.7 | PASS | - |
| 343 | MCI-CTFSTL-SP02 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 10.255.255.11 | PASS | - |
| 344 | MCI-CTFSTL-SP02 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 10.255.255.15 | FAIL | Session state Idle |
| 345 | MCI-CTFSTL-SP02 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 10.255.255.19 | PASS | - |
| 346 | MCI-CTFSTL-SP02 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 10.255.255.23 | PASS | - |
| 347 | MCI-CTFSTL-BLF03a | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 10.255.0.1 | PASS | - |
| 348 | MCI-CTFSTL-BLF03a | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 10.255.0.2 | PASS | - |
| 349 | MCI-CTFSTL-BLF03b | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 10.255.0.1 | PASS | - |
| 350 | MCI-CTFSTL-BLF03b | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 10.255.0.2 | PASS | - |
| 351 | MCI-CTFSTL-LF01a | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 10.255.0.1 | PASS | - |
| 352 | MCI-CTFSTL-LF01a | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 10.255.0.2 | PASS | - |
| 353 | MCI-CTFSTL-LF01b | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 10.255.0.1 | PASS | - |
| 354 | MCI-CTFSTL-LF01b | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 10.255.0.2 | PASS | - |
| 355 | MCI-CTFSTL-LF02a | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 10.255.0.1 | PASS | - |
| 356 | MCI-CTFSTL-LF02a | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 10.255.0.2 | PASS | - |
| 357 | MCI-CTFSTL-LF02b | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 10.255.0.1 | PASS | - |
| 358 | MCI-CTFSTL-LF02b | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 10.255.0.2 | PASS | - |
| 359 | MCI-CTFSTL-SP01 | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 10.255.0.7 | PASS | - |
| 360 | MCI-CTFSTL-SP01 | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 10.255.0.8 | PASS | - |
| 361 | MCI-CTFSTL-SP01 | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 10.255.0.3 | PASS | - |
| 362 | MCI-CTFSTL-SP01 | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 10.255.0.4 | PASS | - |
| 363 | MCI-CTFSTL-SP01 | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 10.255.0.5 | PASS | - |
| 364 | MCI-CTFSTL-SP01 | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 10.255.0.6 | PASS | - |
| 365 | MCI-CTFSTL-SP02 | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 10.255.0.7 | PASS | - |
| 366 | MCI-CTFSTL-SP02 | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 10.255.0.8 | PASS | - |
| 367 | MCI-CTFSTL-SP02 | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 10.255.0.3 | PASS | - |
| 368 | MCI-CTFSTL-SP02 | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 10.255.0.4 | PASS | - |
| 369 | MCI-CTFSTL-SP02 | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 10.255.0.5 | PASS | - |
| 370 | MCI-CTFSTL-SP02 | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 10.255.0.6 | PASS | - |
| 371 | MCI-CTFSTL-BLF03a | Routing Table | Remote VTEP address | 10.255.1.7 | PASS | - |
| 372 | MCI-CTFSTL-BLF03a | Routing Table | Remote VTEP address | 10.255.1.3 | PASS | - |
| 373 | MCI-CTFSTL-BLF03a | Routing Table | Remote VTEP address | 10.255.1.5 | PASS | - |
| 374 | MCI-CTFSTL-BLF03b | Routing Table | Remote VTEP address | 10.255.1.7 | PASS | - |
| 375 | MCI-CTFSTL-BLF03b | Routing Table | Remote VTEP address | 10.255.1.3 | PASS | - |
| 376 | MCI-CTFSTL-BLF03b | Routing Table | Remote VTEP address | 10.255.1.5 | PASS | - |
| 377 | MCI-CTFSTL-LF01a | Routing Table | Remote VTEP address | 10.255.1.7 | PASS | - |
| 378 | MCI-CTFSTL-LF01a | Routing Table | Remote VTEP address | 10.255.1.3 | PASS | - |
| 379 | MCI-CTFSTL-LF01a | Routing Table | Remote VTEP address | 10.255.1.5 | PASS | - |
| 380 | MCI-CTFSTL-LF01b | Routing Table | Remote VTEP address | 10.255.1.7 | PASS | - |
| 381 | MCI-CTFSTL-LF01b | Routing Table | Remote VTEP address | 10.255.1.3 | PASS | - |
| 382 | MCI-CTFSTL-LF01b | Routing Table | Remote VTEP address | 10.255.1.5 | PASS | - |
| 383 | MCI-CTFSTL-LF02a | Routing Table | Remote VTEP address | 10.255.1.7 | PASS | - |
| 384 | MCI-CTFSTL-LF02a | Routing Table | Remote VTEP address | 10.255.1.3 | PASS | - |
| 385 | MCI-CTFSTL-LF02a | Routing Table | Remote VTEP address | 10.255.1.5 | PASS | - |
| 386 | MCI-CTFSTL-LF02b | Routing Table | Remote VTEP address | 10.255.1.7 | PASS | - |
| 387 | MCI-CTFSTL-LF02b | Routing Table | Remote VTEP address | 10.255.1.3 | PASS | - |
| 388 | MCI-CTFSTL-LF02b | Routing Table | Remote VTEP address | 10.255.1.5 | PASS | - |
| 389 | MCI-CTFSTL-BLF03a | Routing Table | Remote Lo0 address | 10.255.0.7 | PASS | - |
| 390 | MCI-CTFSTL-BLF03a | Routing Table | Remote Lo0 address | 10.255.0.8 | FAIL | Lo0 10.255.0.8 is not in the routing table |
| 391 | MCI-CTFSTL-BLF03a | Routing Table | Remote Lo0 address | 10.255.0.3 | PASS | - |
| 392 | MCI-CTFSTL-BLF03a | Routing Table | Remote Lo0 address | 10.255.0.4 | PASS | - |
| 393 | MCI-CTFSTL-BLF03a | Routing Table | Remote Lo0 address | 10.255.0.5 | PASS | - |
| 394 | MCI-CTFSTL-BLF03a | Routing Table | Remote Lo0 address | 10.255.0.6 | PASS | - |
| 395 | MCI-CTFSTL-BLF03a | Routing Table | Remote Lo0 address | 10.255.0.1 | PASS | - |
| 396 | MCI-CTFSTL-BLF03a | Routing Table | Remote Lo0 address | 10.255.0.2 | PASS | - |
| 397 | MCI-CTFSTL-BLF03b | Routing Table | Remote Lo0 address | 10.255.0.7 | FAIL | Lo0 10.255.0.7 is not in the routing table |
| 398 | MCI-CTFSTL-BLF03b | Routing Table | Remote Lo0 address | 10.255.0.8 | PASS | - |
| 399 | MCI-CTFSTL-BLF03b | Routing Table | Remote Lo0 address | 10.255.0.3 | PASS | - |
| 400 | MCI-CTFSTL-BLF03b | Routing Table | Remote Lo0 address | 10.255.0.4 | PASS | - |
| 401 | MCI-CTFSTL-BLF03b | Routing Table | Remote Lo0 address | 10.255.0.5 | PASS | - |
| 402 | MCI-CTFSTL-BLF03b | Routing Table | Remote Lo0 address | 10.255.0.6 | PASS | - |
| 403 | MCI-CTFSTL-BLF03b | Routing Table | Remote Lo0 address | 10.255.0.1 | PASS | - |
| 404 | MCI-CTFSTL-BLF03b | Routing Table | Remote Lo0 address | 10.255.0.2 | PASS | - |
| 405 | MCI-CTFSTL-LF01a | Routing Table | Remote Lo0 address | 10.255.0.7 | PASS | - |
| 406 | MCI-CTFSTL-LF01a | Routing Table | Remote Lo0 address | 10.255.0.8 | PASS | - |
| 407 | MCI-CTFSTL-LF01a | Routing Table | Remote Lo0 address | 10.255.0.3 | PASS | - |
| 408 | MCI-CTFSTL-LF01a | Routing Table | Remote Lo0 address | 10.255.0.4 | PASS | - |
| 409 | MCI-CTFSTL-LF01a | Routing Table | Remote Lo0 address | 10.255.0.5 | PASS | - |
| 410 | MCI-CTFSTL-LF01a | Routing Table | Remote Lo0 address | 10.255.0.6 | PASS | - |
| 411 | MCI-CTFSTL-LF01a | Routing Table | Remote Lo0 address | 10.255.0.1 | PASS | - |
| 412 | MCI-CTFSTL-LF01a | Routing Table | Remote Lo0 address | 10.255.0.2 | PASS | - |
| 413 | MCI-CTFSTL-LF01b | Routing Table | Remote Lo0 address | 10.255.0.7 | PASS | - |
| 414 | MCI-CTFSTL-LF01b | Routing Table | Remote Lo0 address | 10.255.0.8 | PASS | - |
| 415 | MCI-CTFSTL-LF01b | Routing Table | Remote Lo0 address | 10.255.0.3 | PASS | - |
| 416 | MCI-CTFSTL-LF01b | Routing Table | Remote Lo0 address | 10.255.0.4 | PASS | - |
| 417 | MCI-CTFSTL-LF01b | Routing Table | Remote Lo0 address | 10.255.0.5 | PASS | - |
| 418 | MCI-CTFSTL-LF01b | Routing Table | Remote Lo0 address | 10.255.0.6 | PASS | - |
| 419 | MCI-CTFSTL-LF01b | Routing Table | Remote Lo0 address | 10.255.0.1 | PASS | - |
| 420 | MCI-CTFSTL-LF01b | Routing Table | Remote Lo0 address | 10.255.0.2 | PASS | - |
| 421 | MCI-CTFSTL-LF02a | Routing Table | Remote Lo0 address | 10.255.0.7 | PASS | - |
| 422 | MCI-CTFSTL-LF02a | Routing Table | Remote Lo0 address | 10.255.0.8 | PASS | - |
| 423 | MCI-CTFSTL-LF02a | Routing Table | Remote Lo0 address | 10.255.0.3 | PASS | - |
| 424 | MCI-CTFSTL-LF02a | Routing Table | Remote Lo0 address | 10.255.0.4 | PASS | - |
| 425 | MCI-CTFSTL-LF02a | Routing Table | Remote Lo0 address | 10.255.0.5 | PASS | - |
| 426 | MCI-CTFSTL-LF02a | Routing Table | Remote Lo0 address | 10.255.0.6 | PASS | - |
| 427 | MCI-CTFSTL-LF02a | Routing Table | Remote Lo0 address | 10.255.0.1 | PASS | - |
| 428 | MCI-CTFSTL-LF02a | Routing Table | Remote Lo0 address | 10.255.0.2 | PASS | - |
| 429 | MCI-CTFSTL-LF02b | Routing Table | Remote Lo0 address | 10.255.0.7 | PASS | - |
| 430 | MCI-CTFSTL-LF02b | Routing Table | Remote Lo0 address | 10.255.0.8 | PASS | - |
| 431 | MCI-CTFSTL-LF02b | Routing Table | Remote Lo0 address | 10.255.0.3 | PASS | - |
| 432 | MCI-CTFSTL-LF02b | Routing Table | Remote Lo0 address | 10.255.0.4 | PASS | - |
| 433 | MCI-CTFSTL-LF02b | Routing Table | Remote Lo0 address | 10.255.0.5 | PASS | - |
| 434 | MCI-CTFSTL-LF02b | Routing Table | Remote Lo0 address | 10.255.0.6 | PASS | - |
| 435 | MCI-CTFSTL-LF02b | Routing Table | Remote Lo0 address | 10.255.0.1 | PASS | - |
| 436 | MCI-CTFSTL-LF02b | Routing Table | Remote Lo0 address | 10.255.0.2 | PASS | - |
| 437 | MCI-CTFSTL-BLF03a | Loopback0 Reachability | Loopback0 Reachability | Source: MCI-CTFSTL-BLF03a - 10.255.0.7 Destination: 10.255.0.7 | PASS | - |
| 438 | MCI-CTFSTL-BLF03a | Loopback0 Reachability | Loopback0 Reachability | Source: MCI-CTFSTL-BLF03a - 10.255.0.7 Destination: 10.255.0.8 | FAIL | 100% packet loss |
| 439 | MCI-CTFSTL-BLF03a | Loopback0 Reachability | Loopback0 Reachability | Source: MCI-CTFSTL-BLF03a - 10.255.0.7 Destination: 10.255.0.3 | PASS | - |
| 440 | MCI-CTFSTL-BLF03a | Loopback0 Reachability | Loopback0 Reachability | Source: MCI-CTFSTL-BLF03a - 10.255.0.7 Destination: 10.255.0.4 | PASS | - |
| 441 | MCI-CTFSTL-BLF03a | Loopback0 Reachability | Loopback0 Reachability | Source: MCI-CTFSTL-BLF03a - 10.255.0.7 Destination: 10.255.0.5 | PASS | - |
| 442 | MCI-CTFSTL-BLF03a | Loopback0 Reachability | Loopback0 Reachability | Source: MCI-CTFSTL-BLF03a - 10.255.0.7 Destination: 10.255.0.6 | PASS | - |
| 443 | MCI-CTFSTL-BLF03a | Loopback0 Reachability | Loopback0 Reachability | Source: MCI-CTFSTL-BLF03a - 10.255.0.7 Destination: 10.255.0.1 | PASS | - |
| 444 | MCI-CTFSTL-BLF03a | Loopback0 Reachability | Loopback0 Reachability | Source: MCI-CTFSTL-BLF03a - 10.255.0.7 Destination: 10.255.0.2 | PASS | - |
| 445 | MCI-CTFSTL-BLF03b | Loopback0 Reachability | Loopback0 Reachability | Source: MCI-CTFSTL-BLF03b - 10.255.0.8 Destination: 10.255.0.7 | FAIL | 100% packet loss |
| 446 | MCI-CTFSTL-BLF03b | Loopback0 Reachability | Loopback0 Reachability | Source: MCI-CTFSTL-BLF03b - 10.255.0.8 Destination: 10.255.0.8 | PASS | - |
| 447 | MCI-CTFSTL-BLF03b | Loopback0 Reachability | Loopback0 Reachability | Source: MCI-CTFSTL-BLF03b - 10.255.0.8 Destination: 10.255.0.3 | PASS | - |
| 448 | MCI-CTFSTL-BLF03b | Loopback0 Reachability | Loopback0 Reachability | Source: MCI-CTFSTL-BLF03b - 10.255.0.8 Destination: 10.255.0.4 | PASS | - |
| 449 | MCI-CTFSTL-BLF03b | Loopback0 Reachability | Loopback0 Reachability | Source: MCI-CTFSTL-BLF03b - 10.255.0.8 Destination: 10.255.0.5 | PASS | - |
| 450 | MCI-CTFSTL-BLF03b | Loopback0 Reachability | Loopback0 Reachability | Source: MCI-CTFSTL-BLF03b - 10.255.0.8 Destination: 10.255.0.6 | PASS | - |
| 451 | MCI-CTFSTL-BLF03b | Loopback0 Reachability | Loopback0 Reachability | Source: MCI-CTFSTL-BLF03b - 10.255.0.8 Destination: 10.255.0.1 | PASS | - |
| 452 | MCI-CTFSTL-BLF03b | Loopback0 Reachability | Loopback0 Reachability | Source: MCI-CTFSTL-BLF03b - 10.255.0.8 Destination: 10.255.0.2 | PASS | - |
| 453 | MCI-CTFSTL-LF01a | Loopback0 Reachability | Loopback0 Reachability | Source: MCI-CTFSTL-LF01a - 10.255.0.3 Destination: 10.255.0.7 | PASS | - |
| 454 | MCI-CTFSTL-LF01a | Loopback0 Reachability | Loopback0 Reachability | Source: MCI-CTFSTL-LF01a - 10.255.0.3 Destination: 10.255.0.8 | PASS | - |
| 455 | MCI-CTFSTL-LF01a | Loopback0 Reachability | Loopback0 Reachability | Source: MCI-CTFSTL-LF01a - 10.255.0.3 Destination: 10.255.0.3 | PASS | - |
| 456 | MCI-CTFSTL-LF01a | Loopback0 Reachability | Loopback0 Reachability | Source: MCI-CTFSTL-LF01a - 10.255.0.3 Destination: 10.255.0.4 | PASS | - |
| 457 | MCI-CTFSTL-LF01a | Loopback0 Reachability | Loopback0 Reachability | Source: MCI-CTFSTL-LF01a - 10.255.0.3 Destination: 10.255.0.5 | PASS | - |
| 458 | MCI-CTFSTL-LF01a | Loopback0 Reachability | Loopback0 Reachability | Source: MCI-CTFSTL-LF01a - 10.255.0.3 Destination: 10.255.0.6 | PASS | - |
| 459 | MCI-CTFSTL-LF01a | Loopback0 Reachability | Loopback0 Reachability | Source: MCI-CTFSTL-LF01a - 10.255.0.3 Destination: 10.255.0.1 | PASS | - |
| 460 | MCI-CTFSTL-LF01a | Loopback0 Reachability | Loopback0 Reachability | Source: MCI-CTFSTL-LF01a - 10.255.0.3 Destination: 10.255.0.2 | PASS | - |
| 461 | MCI-CTFSTL-LF01b | Loopback0 Reachability | Loopback0 Reachability | Source: MCI-CTFSTL-LF01b - 10.255.0.4 Destination: 10.255.0.7 | PASS | - |
| 462 | MCI-CTFSTL-LF01b | Loopback0 Reachability | Loopback0 Reachability | Source: MCI-CTFSTL-LF01b - 10.255.0.4 Destination: 10.255.0.8 | PASS | - |
| 463 | MCI-CTFSTL-LF01b | Loopback0 Reachability | Loopback0 Reachability | Source: MCI-CTFSTL-LF01b - 10.255.0.4 Destination: 10.255.0.3 | PASS | - |
| 464 | MCI-CTFSTL-LF01b | Loopback0 Reachability | Loopback0 Reachability | Source: MCI-CTFSTL-LF01b - 10.255.0.4 Destination: 10.255.0.4 | PASS | - |
| 465 | MCI-CTFSTL-LF01b | Loopback0 Reachability | Loopback0 Reachability | Source: MCI-CTFSTL-LF01b - 10.255.0.4 Destination: 10.255.0.5 | PASS | - |
| 466 | MCI-CTFSTL-LF01b | Loopback0 Reachability | Loopback0 Reachability | Source: MCI-CTFSTL-LF01b - 10.255.0.4 Destination: 10.255.0.6 | PASS | - |
| 467 | MCI-CTFSTL-LF01b | Loopback0 Reachability | Loopback0 Reachability | Source: MCI-CTFSTL-LF01b - 10.255.0.4 Destination: 10.255.0.1 | PASS | - |
| 468 | MCI-CTFSTL-LF01b | Loopback0 Reachability | Loopback0 Reachability | Source: MCI-CTFSTL-LF01b - 10.255.0.4 Destination: 10.255.0.2 | PASS | - |
| 469 | MCI-CTFSTL-LF02a | Loopback0 Reachability | Loopback0 Reachability | Source: MCI-CTFSTL-LF02a - 10.255.0.5 Destination: 10.255.0.7 | PASS | - |
| 470 | MCI-CTFSTL-LF02a | Loopback0 Reachability | Loopback0 Reachability | Source: MCI-CTFSTL-LF02a - 10.255.0.5 Destination: 10.255.0.8 | PASS | - |
| 471 | MCI-CTFSTL-LF02a | Loopback0 Reachability | Loopback0 Reachability | Source: MCI-CTFSTL-LF02a - 10.255.0.5 Destination: 10.255.0.3 | PASS | - |
| 472 | MCI-CTFSTL-LF02a | Loopback0 Reachability | Loopback0 Reachability | Source: MCI-CTFSTL-LF02a - 10.255.0.5 Destination: 10.255.0.4 | PASS | - |
| 473 | MCI-CTFSTL-LF02a | Loopback0 Reachability | Loopback0 Reachability | Source: MCI-CTFSTL-LF02a - 10.255.0.5 Destination: 10.255.0.5 | PASS | - |
| 474 | MCI-CTFSTL-LF02a | Loopback0 Reachability | Loopback0 Reachability | Source: MCI-CTFSTL-LF02a - 10.255.0.5 Destination: 10.255.0.6 | PASS | - |
| 475 | MCI-CTFSTL-LF02a | Loopback0 Reachability | Loopback0 Reachability | Source: MCI-CTFSTL-LF02a - 10.255.0.5 Destination: 10.255.0.1 | PASS | - |
| 476 | MCI-CTFSTL-LF02a | Loopback0 Reachability | Loopback0 Reachability | Source: MCI-CTFSTL-LF02a - 10.255.0.5 Destination: 10.255.0.2 | PASS | - |
| 477 | MCI-CTFSTL-LF02b | Loopback0 Reachability | Loopback0 Reachability | Source: MCI-CTFSTL-LF02b - 10.255.0.6 Destination: 10.255.0.7 | PASS | - |
| 478 | MCI-CTFSTL-LF02b | Loopback0 Reachability | Loopback0 Reachability | Source: MCI-CTFSTL-LF02b - 10.255.0.6 Destination: 10.255.0.8 | PASS | - |
| 479 | MCI-CTFSTL-LF02b | Loopback0 Reachability | Loopback0 Reachability | Source: MCI-CTFSTL-LF02b - 10.255.0.6 Destination: 10.255.0.3 | PASS | - |
| 480 | MCI-CTFSTL-LF02b | Loopback0 Reachability | Loopback0 Reachability | Source: MCI-CTFSTL-LF02b - 10.255.0.6 Destination: 10.255.0.4 | PASS | - |
| 481 | MCI-CTFSTL-LF02b | Loopback0 Reachability | Loopback0 Reachability | Source: MCI-CTFSTL-LF02b - 10.255.0.6 Destination: 10.255.0.5 | PASS | - |
| 482 | MCI-CTFSTL-LF02b | Loopback0 Reachability | Loopback0 Reachability | Source: MCI-CTFSTL-LF02b - 10.255.0.6 Destination: 10.255.0.6 | PASS | - |
| 483 | MCI-CTFSTL-LF02b | Loopback0 Reachability | Loopback0 Reachability | Source: MCI-CTFSTL-LF02b - 10.255.0.6 Destination: 10.255.0.1 | PASS | - |
| 484 | MCI-CTFSTL-LF02b | Loopback0 Reachability | Loopback0 Reachability | Source: MCI-CTFSTL-LF02b - 10.255.0.6 Destination: 10.255.0.2 | PASS | - |
