# Bluemoon w2
Penetration Testing Lab: Methodology & Findings

1. **Network Discovery**: Initially, I used `netdiscover` to identify the active IP address of the target within the local network.
2. **Reconnaissance**: Once the IP was confirmed, I performed an `nmap` scan to identify open ports and running services.
3. **Web Enumeration**: I accessed the target via **Firefox** to inspect the web interface. To uncover hidden paths, I ran **Gobuster**, which successfully revealed a hidden directory containing a **QR code**.
4. **Exploitation**: The most challenging phase was cracking the **FTP password**. After identifying the necessary wordlists and tools (like Hydra), I successfully gained access to the server.

<img width="592" height="602" alt="image" src="https://github.com/user-attachments/assets/2e4e4d02-9f32-416a-84d7-02a66936c4f6" />

## Tool & Command Reference

| Phase | Tool | Purpose |
| :--- | :--- | :--- |
| **Scanning** | `netdiscover` | Host discovery and IP identification |
| **Enumeration** | `nmap` | Port scanning and service version detection |
| **Fuzzing** | `gobuster` | Directory brute-forcing for hidden assets |
| **Cracking** | `Hydra` | Brute-forcing FTP credentials |
