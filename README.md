# Networking---Routing & Switching
This network planning was created and model using Huawei Devices.

The network follows a hybrid hierarchical topology, incorporating elements of star, mesh, and hierarchical (tree) structures.

The Headquarters (HQ) and Branch (BR) are connected through core and distribution layers.
The service provider (SP) network uses OSPF (Open Shortest Path First) routing for wide-area connectivity.
Redundant links between core switches and routers suggest high availability and fault tolerance.

Tools used : eNSP.

SSH & FTP client : MobaXterm

Devices Used :
The topology consists of the following network devices:

Routers (R): Used for inter-network communication, OSPF routing, and WAN connectivity.
Switches (CoreSW, ACSW, BR-CoreSW, BR-ACSW): Used for local LAN switching and VLAN segmentation.
End Devices (PCs): Workstations connected to access switches.
Service Provider (SP) Network: Connects the HQ and branch through multiple routers.
This also include firewalls USG6000V, Server and Six PC's.

Protocols Applied :
OSPF (Open Shortest Path First): Used as the routing protocol in the Service Provider Area (OSPF AREA 0).
VRRP (Virtual Router Redundancy Protocol): Provides router redundancy for HQ to ensure high availability.
VLANs (Virtual Local Area Networks): Implemented in HQ and Branch networks for segmentation and security (e.g., VLAN10, VLAN20, VLAN150, VLAN160).
This also include other protocols like HRP,HSB, BGP, IBGP, ISIS, DCHP,Authentication using aaa and MD5, STP, MSTP and also LSP, SFP and BFD.

Security Implementations :
VLAN segmentation to isolate network traffic.
VRRP for gateway redundancy, ensuring failover in case of primary router failure.
Service provider connection ensures secure OSPF routing.
External access control via internet-facing router (R-8) with DNS resolution to Google’s public DNS (8.8.8.8).

This network is designed for scalability, fault tolerance, and security by implementing a hybrid hierarchical topology with redundant routers, VLAN segmentation, OSPF routing, and VRRP redundancy for failover. The setup ensures an efficient and resilient enterprise network.







