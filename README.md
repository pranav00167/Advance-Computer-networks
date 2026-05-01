🔹 Overview

This repository contains implementation and analysis of fundamental networking concepts using Wireshark and Cisco Packet Tracer.
The labs progress from basic packet analysis to advanced routing protocols like BGP.
*****************************************************************************************************************************************************
🧪 Lab 1: Packet Capture and Analysis (Wireshark)
Objective

To capture live network packets and analyze protocol behavior.

Description
Used Wireshark to capture packets.
Observed protocols such as:
ARP
ICMP
DNS
HTTP
Outcome
Understood packet structure and protocol layering.
Identified source/destination MAC and IP addresses.

*********************************************************************************************************************************************************
🧪 Lab 2: Protocol Analysis
Objective

To analyze different network protocols in detail.

Description
Filtered packets using:
arp, icmp, dns, tcp, http
Studied:
TCP handshake
DNS query/response
HTTP request/response
Outcome
Gained understanding of real-time protocol communication.
Learned how data flows across network layers.

*********************************************************************************************************************************************************

🧪 Lab 3: Network Topologies
Objective

To design and simulate different network topologies.

Description
Created star, bus, and mesh topologies in Cisco Packet Tracer.
Tested connectivity using ping.
Outcome
Understood how topology affects performance and reliability.

*********************************************************************************************************************************************************

🧪 Lab 4: DHCP Configuration
Objective

To configure dynamic IP addressing.

Description
Configured router as DHCP server.
Assigned IP addresses automatically to PCs.
Outcome
Learned automatic IP allocation.
Understood DHCP working mechanism.

*********************************************************************************************************************************************************

🧪 Lab 5: Static Routing
Objective

To configure manual routing between networks.

Description
Connected multiple networks using routers.
Configured routes using: ip route <network> <mask> <next-hop>
Outcome
Achieved communication between networks manually.
Understood routing table behavior.
*********************************************************************************************************************************************************

🧪 Lab 6: RIP (Routing Information Protocol)
Objective

To implement dynamic routing using RIP.

Description
Configured RIP v2:
router rip
version 2
network <network-id>

Outcome
Routers learned routes automatically.
Observed routing entries marked as R.

*********************************************************************************************************************************************************
🧪 Lab 7: OSPF (Open Shortest Path First)
Objective

To configure link-state routing protocol.

Description
Configured OSPF with Area 0:
router ospf 1
network <network> <wildcard-mask> area 0

Outcome
Observed shortest path calculation using SPF algorithm.
Verified routes marked as O.
*********************************************************************************************************************************************************
🧪 Lab 8: BGP (Border Gateway Protocol)
Objective

To configure inter-domain routing using BGP.

Description
Configured eBGP between different Autonomous Systems:
router bgp <AS-number>
neighbor <IP> remote-as <AS>
Advertised networks using:
network <network> mask <subnet-mask>

Outcome
Established communication between different AS.
Observed routing entries marked as B.
Understood path-vector routing.

*********************************************************************************************************************************************************
