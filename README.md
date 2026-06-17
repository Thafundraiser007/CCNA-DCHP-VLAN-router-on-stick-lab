# CCNA-DCHP-VLAN-router-on-stick-lab
This project demonstrates a Cisco network using VLAN segmentation with DHCP and inter-VLAN routing using a Router-on-a-Stick configuration.


## Topology
- 1 Router (Cisco 2911)
- 1 Switch (Cisco 2960)
- 4 PCs
- 2 VLANs:
  - VLAN 10 (DATA)
  - VLAN 20 (SALES)

## Features
- VLAN creation and port assignment
- 802.1Q trunk configuration
- Inter-VLAN routing via subinterfaces
- DHCP server configured on router
- Automatic IP assignment per VLAN

## IP Addressing Scheme
- VLAN 10: 192.168.10.0/24
- VLAN 20: 192.168.20.0/24

## Key Configurations
### Router
- Subinterfaces:
  - Fa0/0.10 → VLAN 10
  - Fa0/0.20 → VLAN 20
- DHCP pools for both VLANs

### Switch
- VLAN 10 and VLAN 20 configured
- Access ports assigned to correct VLANs
- Trunk link to router

## Verification
- PCs receive IP addresses via DHCP
- PCs can ping their default gateway
- Inter-VLAN routing is successful

## Skills Demonstrated
- VLAN configuration
- Trunking (802.1Q)
- DHCP configuration
- Router-on-a-stick
- Basic troubleshooting

## Author
Jamill Naipao
