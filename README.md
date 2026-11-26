# NorthStar Technologies
### Enterprise Campus Network Design & Implementation

A multi-VLAN enterprise campus network designed and simulated using Cisco Packet Tracer 9.x. This project demonstrates enterprise networking concepts, Layer 2 and Layer 3 infrastructure, network redundancy, dynamic routing, wireless infrastructure, and network security.

## Project Overview

NorthStar Technologies is a simulated enterprise network designed to support approximately 200 users across multiple departments.

The network was designed with an emphasis on scalability, availability, segmentation, and centralized network management.

The project incorporates redundant switching infrastructure, inter-VLAN routing, dynamic routing, wireless connectivity, and access control policies to simulate a realistic enterprise environment.

## Network Architecture

The network incorporates:

- Redundant Layer 3 core and distribution switching.
- Multiple access-layer switches supporting wired endpoints.
- Department-based VLAN segmentation.
- Centralized wireless management through a Wireless LAN Controller (WLC).
- Dedicated server infrastructure.
- Voice VLAN infrastructure for IP telephony.
- Redundant default gateway functionality.

## Technologies & Implementations

| Technology | Implementation |
|---|---|
| VLANs | Department-based network segmentation |
| Inter-VLAN Routing | Layer 3 switching |
| HSRP | Default gateway redundancy |
| STP | Loop prevention and load balancing |
| OSPF | Dynamic routing, Area 0 |
| DHCP | Automated IP address assignment |
| ACLs | Traffic filtering and network security |
| WLC | Centralized wireless management |
| Wireless | Enterprise and guest SSIDs |
| VoIP | Dedicated voice VLAN |
| Trunking | 802.1Q VLAN transport |

## VLAN Architecture

The network uses dedicated VLANs to separate departments, infrastructure, and endpoint types.

| VLAN | Name | Purpose |
|---|---|---|
| 10 | NET-MGMT | Network management |
| 20 | SALES | Sales department |
| 30 | OPERATIONS | Operations department |
| 40 | IT | IT department |
| 50 | HR | Human Resources |
| 60 | FINANCE | Finance department |
| 70 | CORP-MGMT | Corporate management |
| 80 | SERVERS | Server infrastructure |
| 90 | VOICE | IP telephony |
| 100 | CORP-WIFI | Corporate wireless |
| 110 | GUEST-WIFI | Guest wireless |
| 120 | PRINTERS | Network printers |
| 999 | NATIVE | Native VLAN |

## Routing & Redundancy

**HSRP (Hot Standby Router Protocol)**

Implemented between redundant distribution switches to provide highly available default gateways for network VLANs.

**OSPF (Open Shortest Path First)**

Configured as the dynamic routing protocol using Area 0 to provide routing between Layer 3 network devices.

**Spanning Tree Protocol**

Implemented to prevent Layer 2 switching loops while providing a load-balanced switching topology across redundant distribution switches.

## Wireless Infrastructure

A centralized Wireless LAN Controller manages the wireless access point infrastructure.

The wireless architecture includes:

- Corporate wireless SSID.
- Guest wireless SSID.
- Dedicated corporate and guest wireless VLANs.
- Guest network isolation through ACLs.
- Centralized access point management.

## Network Security

Security controls implemented throughout the network include:

- VLAN-based segmentation.
- Extended Access Control Lists (ACLs).
- Guest wireless network restrictions.
- Dedicated management and infrastructure VLANs.
- Outside-facing traffic filtering at the network edge.

## Project Objectives

The primary objectives of this project were to:

1. Design a scalable enterprise campus network.
2. Implement redundant switching and gateway infrastructure.
3. Configure dynamic routing between network segments.
4. Implement department-based VLAN segmentation.
5. Deploy centralized wireless management.
6. Establish network security policies using ACLs.
7. Integrate IP telephony and supporting infrastructure.
8. Troubleshoot and validate network connectivity through practical configuration and testing.

## Project Environment

- **Simulation Platform:** Cisco Packet Tracer 9.x
- **Network Design:** Enterprise campus LAN
- **Estimated Users:** 200
- **Access Layer:** 10 access switches
- **Routing Protocol:** OSPF
- **Redundancy:** HSRP and STP

## Project Files

The repository includes the Cisco Packet Tracer project file (`.pkt`), with supporting documentation and network topology images to be added.

## Disclaimer

This is an independent educational networking project created in a simulated environment using Cisco Packet Tracer. It is intended to demonstrate networking knowledge, configuration experience, and enterprise network design concepts.