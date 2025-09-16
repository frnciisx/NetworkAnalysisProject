# Network Analysis Project – Wireshark (Ubuntu VM)

## Overview
Applied my skills from training projects to complete a hands-on network analysis project using Ubuntu and Wireshark. This project introduced and strengthened my understanding of Linux environments, network protocols, and packet-level traffic analysis.

---

## Tools & Environment
- Ubuntu VM  
- Wireshark   
- Linux Terminal  

---

## Process
1. Captured approximately **30,000 packets** from websites such as:  
   - `testudo.umd.edu`  
   - `youtube.com`  
   - `maps.umd.edu`  
   - `linkedin.com`  
2. Filtered HTTP and DNS traffic using Wireshark display filters to isolate relevant communication.  
3. Followed HTTP streams to understand traffic flow and verify website legitimacy.  
4. Analyzed traffic across **common network ports** to understand protocol behavior and security:

| Port | Protocol | Description |
|------|----------|-------------|
| 80   | TCP      | HTTP (unencrypted web traffic) |
| 443  | TCP      | HTTPS (encrypted web traffic) |
| 53   | TCP/UDP  | DNS queries and responses |

5. Used display filters in Wireshark such as:  
```text
tcp.port == 80
tcp.port == 443
udp.port == 53
http
dns
