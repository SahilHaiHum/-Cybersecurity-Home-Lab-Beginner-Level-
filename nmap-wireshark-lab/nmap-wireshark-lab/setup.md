# 🛠️ Lab Setup Instructions

## Machines Used

- **Kali Linux** – Attacker VM
- **Ubuntu Linux** – Victim VM

## Network Setup

- VirtualBox > Host-Only Adapter (both VMs on same internal network)
- Confirmed both machines can ping each other

## Tools Installed

- Kali: Nmap (pre-installed)
- Ubuntu: Wireshark

## Steps

1. Launch both VMs.
2. Start Wireshark on Ubuntu and begin capturing on the correct interface (e.g., `eth0` or `enp0s3`).
3. On Kali, run:
   ```bash
   nmap -sS -T4 -v <Ubuntu-IP>
   ```
4. Stop capture on Ubuntu and save the `.pcapng` file.
5. Analyze packet types, flags (SYN), and connection attempts.
