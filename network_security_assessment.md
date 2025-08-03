Network Security Assessment Report

Submitted by: Kanya PerumalRaj  
Date: August 3, 2025  
Tools Used: Nmap, Wireshark  
Objective: To identify potential vulnerabilities in a test network using scanning and packet analysis techniques.



 1. Introduction

This report presents the findings of a network security assessment performed on a local test network. The purpose is to detect open ports, identify running services, and analyze network traffic to uncover vulnerabilities or misconfigurations. The assessment is conducted using two powerful tools: **Nmap** for network scanning and **Wireshark** for packet sniffing.



 2. Tools Overview

 Nmap:
- A network scanning tool used to discover hosts and services on a network.
- Used here to scan open ports, service versions, and possible OS.

Wireshark:
- A packet analyzer that captures network traffic in real time.
- Helps identify unsecured data transfers, unauthorized access, and suspicious patterns.



| Component       | Details                      |
|----------------|------------------------------|
| Target Machine | Ubuntu VM (192.168.0.105)    |
| Attacker System| Kali Linux (192.168.0.104)   |
| Network Type   | Local Wi-Fi / Virtual Network|


4. Nmap Scan Results

Command Used:
```bash
nmap -sV -O -A 192.168.0.105 -oN nmap_results.txt
