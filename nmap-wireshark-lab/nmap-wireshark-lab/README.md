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
   ```
4. Saved the `.pcapng` file and took screenshots of scan results and packet logs.

## 📁 Folder Structure

```
nmap-wireshark-lab/
├── README.md
├── setup.md
├── notes/
│   └── observations.md
├── screenshots/
│   ├── nmap-scan-kali.png
│   └── wireshark-capture-ubuntu.png
├── pcap-files/
│   └── nmap-attack.pcapng
```

## 📌 Key Learnings

- Visualized TCP SYN scan patterns in Wireshark.
- Identified how reconnaissance appears to a defender.
- Understood the basic attacker-victim model in a local lab.

## 🧠 Tools Used

- Nmap
- Wireshark
- VirtualBox
- Ubuntu Linux
- Kali Linux

## 📜 License

MIT
