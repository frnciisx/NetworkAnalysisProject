# Network Analysis Project – Wireshark & tcpdump (Ubuntu VM)

## Overview
Applied my skills from previous training projects on [TryHackMe](https://tryhackme.com/) and [LetsDefend](https://letsdefend.io/) to complete a hands-on network analysis project using Ubuntu, Wireshark.  
This project strengthened my understanding of Linux environments, network protocols, and packet-level traffic analysis.

---

## 🛠 Tools & Environment
- Ubuntu VM  
- Wireshark  
- Linux Terminal  

---
## 📋 Process
- Downloaded and installed [UTM](https://mac.getutm.app/) on my Mac and set up an Ubuntu VM using an Ubuntu ISO file  
- Used the Ubuntu terminal to install and configure tools like Wireshark and tcpdump  
- Captured approximately **30,000 packets** from websites like:  
  - `testudo.umd.edu`  
  - `youtube.com`  
  - `linkedin.com`  
- Filtered HTTP and DNS traffic using Wireshark display filters  
- Followed HTTP streams to understand traffic flow and verify website legitimacy  
- Explored common ports like:
  - `tcp.port == 80` (HTTP)
  - `tcp.port == 443` (HTTPS)
  - `udp.port == 53` (DNS)
---

## 🚨 Redirect Website Curiosity
I've always been annoyed by redirect-heavy websites and use an adblocker to avoid them.  
With Wireshark, I wanted to see what was really happening behind those redirects.

While analyzing traffic from a redirect website, I filtered DNS traffic using `udp.port == 53` and noticed logs for `www.storygize.net` — a site I hadn’t actively opened.  
At first this confused me, but after inspecting the packet details, I realized it was just a DNS query and that my system never actually connected to the site.

This experience helped me better understand how redirects work and how many background requests they attempt to trigger.

---

## 📸 Screenshots
[Ubuntu VM and Wireshark capture](Screenshots)

---

## 💡 Key Learnings
- Understanding of **TCP/IP, DNS, HTTP/HTTPS protocols**  
- Packet analysis and **network security monitoring**  
- Linux terminal navigation and **network troubleshooting**  
- Learned to distinguish between **DNS lookups** and **actual connections**  
- Gained insight into how **redirects and ad domains** appear in network traffic  

---

## 🚀 Future Goals
I want to use this new skill to help others stay safe online by recognizing suspicious network behavior,  
and to become personally smarter and more cautious about the sites and links I click on.
