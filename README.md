
# Week 1 - Simple LAN Topology Lab

**Student:** Aftab Alam
**Internship:** IT-SIMPLERA Solutions - Network Administration
**Date:** Nov 20, 2026

## 1. Objective
To design a basic LAN topology with 2 PCs and a Switch, configure static IPv4, and verify end-to-end connectivity using ICMP ping in both Cisco Packet Tracer and GNS3 (PuTTY).

## 2. Networking Concepts Learned
- **LAN & Switch:** How devices form a single broadcast domain via Layer 2 switch
- **IPv4:** Use of Class C private IP 192.168.1.0/24 and mask 255.255.255.0
- **ICMP:** Ping test for reachability check

## 3. IP Scheme
| Device | IP Address | Subnet |
| :--- | :--- | :--- |
| PC1 | 192.168.1.1 | 255.255.255.0 |
| PC2 | 192.168.1.2 | 255.255.255.0 |
| Switch1 | Layer 2 | N/A |

## 4. Packet Tracer Implementation
Connected PC1 & PC2 to Switch1 via Copper Straight-Through cable. Configured IPs via IP Configuration tab. Result: Ping `192.168.1.2` from PC1 -> 4 Replies, 0% Loss - SUCCESS.

## 5. GNS3 & PuTTY Implementation
Created same topology with 2 VPCS nodes in GNS3. Used PuTTY commands:
- `ip 192.168.1.1/24` on PC1
- `ip 192.168.1.2/24` on PC2
Result: Ping from PC1 -> 5 Replies, ttl=64 - SUCCESS.

## 6. Challenges
- GNS3 nodes needed to be started manually (red to green).
- VPCS uses CLI `ip` command, not GUI like Packet Tracer.

## 7. Conclusion
Week 01 completed successfully. Learned fundamentals and hands-on with both simulators. Ready for routing tasks.
