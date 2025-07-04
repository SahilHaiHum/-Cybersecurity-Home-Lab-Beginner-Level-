# 📋 Observations

- The Nmap scan uses SYN packets to detect open ports (TCP SYN scan).
- Wireshark on Ubuntu captured multiple SYN packets from the Kali IP.
- No full TCP handshake observed – only SYN, no ACK/FIN (since it's a stealth scan).
- Open ports responded with SYN-ACK; closed ports responded with RST.
- Good visualization of how simple reconnaissance looks at the packet level.
