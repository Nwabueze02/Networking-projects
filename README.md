# Networking Projects
A collection of hands-on networking projects built in Cisco Packet Tracer, demonstrating core network engineering and security skills including VLAN segmentation, inter-VLAN routing, DHCP, VPN, ACLs, and network design.
 
---
 
## Project 1 — Small Office Network with VLAN Segmentation & Inter-VLAN Routing
 
### Overview
Designed and configured a small office network simulating a real business environment with two departments (Sales and IT) separated by VLANs, with a router handling traffic between them using the router-on-a-stick method.
 
### Technologies Used
- Cisco IOS (2911 Router, 2960 Switch)
- VLANs (VLAN 10 — Sales, VLAN 20 — IT)
- Router-on-a-Stick Inter-VLAN Routing
- DHCP (automatic IP assignment per VLAN)
- Cisco Packet Tracer
### Network Topology
<img width="1376" height="930" alt="Diagram" src="https://github.com/user-attachments/assets/a3637a5e-04a1-433f-8e29-f646c9d5d9b3" />

 
### IP Addressing Scheme
 
| Device | VLAN | Network | Gateway |
|---|---|---|---|
| PC-Sales-1 | VLAN 10 | 192.168.10.0/24 | 192.168.10.1 |
| PC-Sales-2 | VLAN 10 | 192.168.10.0/24 | 192.168.10.1 |
| PC-IT-1 | VLAN 20 | 192.168.20.0/24 | 192.168.20.1 |
| PC-IT-2 | VLAN 20 | 192.168.20.0/24 | 192.168.20.1 |
 
### What I Configured
- Created VLAN 10 (Sales) and VLAN 20 (IT) on the switch
- Assigned PC ports to their respective VLANs as access ports
- Configured the router uplink as a trunk port to carry both VLANs
- Created sub-interfaces on the router (Gi0/0.10 and Gi0/0.20) with 802.1Q encapsulation
- Configured DHCP pools on the router for each VLAN
- Verified full connectivity within and across VLANs
### Verification Screenshots
 
**VLAN Assignment — show vlan brief**
 
<img width="419" height="117" alt="Vlanbrief" src="https://github.com/user-attachments/assets/093ddd97-cfd0-4f3a-b5e1-8c5901e86359" />

 
**Routing Table — show ip route**
 
<img width="419" height="180" alt="Route" src="https://github.com/user-attachments/assets/3f6fd51c-a7a7-4f0f-affc-4b360f30a31e" />

 
**DHCP Leases — show ip dhcp binding**
 
<img width="362" height="76" alt="DHCPBinding" src="https://github.com/user-attachments/assets/bde5ffe4-0baf-420e-b74b-344383200442" />

 
**Cross-VLAN Ping Test (Sales → IT)**
 
<img width="419" height="465" alt="PingTest" src="https://github.com/user-attachments/assets/99919b45-7339-4511-80e6-bcea57e41579" />

 
### Key Concepts Demonstrated
- **VLAN segmentation** — logically separating departments on a shared physical switch improves security and reduces broadcast traffic
- **Router-on-a-stick** — a single physical router interface handles routing between multiple VLANs using sub-interfaces
- **DHCP** — devices receive IP addresses automatically based on which VLAN they belong to
- **Trunk links** — the switch-to-router link carries traffic for all VLANs tagged with 802.1Q
---
 
## Project 2 — Multi-Site Enterprise Network with VPN & Network Security
*Coming soon — In progress*
 
Two-site enterprise network featuring inter-VLAN routing, site-to-site and remote access VPN (IKE/IPsec), ACLs, NAT, DHCP, DNS, and a DMZ for isolated public-facing services.
 
---
 
## Tools & Technologies
- Cisco Packet Tracer
- Cisco IOS
- Python 
## Certifications
- CompTIA Network+ (active)
- CompTIA Security+ (in progress)
- CCNA (in progress)
## Connect
- LinkedIn: Nwabueze Onyemachi
- Email: nionyemachi44@gmail.com
 
