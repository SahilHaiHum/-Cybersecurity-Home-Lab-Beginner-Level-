# 🧪 Nmap Scan & Wireshark Capture – Beginner Cybersecurity Homelab

This project demonstrates a simple cybersecurity lab where a Kali Linux machine scans a Ubuntu machine using Nmap, while the Ubuntu machine captures the attack live using Wireshark.

## 🎯 Objective

To visualize how a port scan looks from both the attacker and defender’s point of view.

## 🛠️ Lab Setup

| Machine  | OS     | Role     | Description             |
|----------|--------|----------|--------------------------|
| Kali     | Linux  | Attacker | Ran Nmap scan            |
| Ubuntu   | Linux  | Victim   | Captured traffic in Wireshark |

## 🔍 Steps Performed

1. Set up Kali and Ubuntu on VirtualBox using a Host-only network.
2. On Ubuntu, started Wireshark to capture all interface traffic.
3. From Kali, ran the following scan:
   ```bash
   nmap -sS -T4 -v 192.168.X.X
