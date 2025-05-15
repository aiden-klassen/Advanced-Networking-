# Advanced-Networking-

# IP Subnetting and Enterprise Network Design – Johannesburg & Luanda Offices

This project presents a comprehensive Packet Tracer network design for a growing company with offices in Johannesburg (Headquarters) and Luanda (Branch). The project involves efficient IP subnetting using Variable Length Subnet Masking (VLSM), VLAN implementation, inter-VLAN routing, OSPF configuration, DHCP server deployment, and secure wireless networking across both sites.

## Overview

- Assigned IPv4 network: 192.168.0.0/22
- VLSM used to allocate subnets for:
  - IT (50 hosts)
  - HR (30 hosts)
  - Sales (60 hosts)
  - Marketing (25 hosts)
  - Management (10 hosts)
- Two physical locations: Johannesburg (HQ) and Luanda (Branch)

## Key Features and Configurations

### 1. Subnet Planning
- Designed a subnet plan using VLSM for optimal IP address allocation.
- Each department was assigned a subnet with appropriate:
  - Network address
  - Subnet mask
  - Assignable IP range
  - Broadcast address
- Efficient use of the 192.168.0.0/22 space ensured minimal waste.

### 2. Network Topology in Packet Tracer
- Implemented the subnet plan using appropriate Cisco routers, switches, and end devices.
- Johannesburg and Luanda were interconnected via OSPF routing.
- VLANs were configured for departments at the Johannesburg office:
  - VLAN 10: IT (Fa0/1 – Fa0/10)
  - VLAN 20: HR (Fa0/11 – Fa0/15)
  - VLAN 30: Sales (Fa0/16 – Fa0/20)
  - VLAN 40: Marketing (Fa0/21 – Fa0/23)
  - VLAN 50: Management (Fa0/24)

### 3. Routing and VLAN Communication
- Implemented inter-VLAN routing using a router-on-a-stick configuration.
- Configured OSPF between both locations to enable dynamic routing.
- Verified end-to-end connectivity across VLANs and between Johannesburg and Luanda.

### 4. DHCP Server Configuration
- Configured the Johannesburg router to act as a central DHCP server.
- DHCP pools were created for each VLAN and for devices in Luanda.
- Verified successful IP assignment across all devices in both locations.

### 5. Wireless Network Setup
- Configured secure wireless routers for employees and guests in both Johannesburg and Luanda.
- Applied consistent SSIDs and wireless security protocols.
- Verified connectivity between wireless and wired devices across both offices.

## File

- `company_network_design.pkt` – Complete Cisco Packet Tracer simulation file

## Tools Used

- Cisco Packet Tracer
- Routers, Switches, Wireless Routers, PCs, Laptops, and Servers

---

This project demonstrates effective IP planning, VLAN segmentation, routing, and security best practices for a modern enterprise network spanning multiple locations.
