# 🛡️ Network Defense Lab using Security Onion & pfSense

This project demonstrates the implementation of a network defense lab using virtualization technologies. The objective was to simulate real-world cyberattacks and test detection and mitigation strategies using **Security Onion (IDS)** and **pfSense (Firewall)**.

## 🔧 Lab Setup
- **Attacker VM:** Kali Linux
- **Target VM:** Ubuntu (Web & FTP Server)
- **Firewall:** pfSense
- **IDS:** Security Onion (with Kibana)

## 🧪 Simulated Attacks
1. **Port Scanning & Service Detection** using `nmap`
2. **ProFTPD Remote Code Execution** using Metasploit
3. **Denial of Service (DoS)** using Slowloris

## 🔍 Detection & Response
- Lucene queries in **Kibana** were used to detect anomalous logs.
- Alerts were generated in Security Onion and correlated with attack timelines.
- **Firewall rules** were enforced via pfSense to block malicious traffic:
  - Block DoS patterns
  - Block HTTP for internal users
  - Block social media access
  - Block inbound FTP

## 📌 Key Takeaways
- Hands-on configuration of IDS and firewall rules.
- Realistic simulation of network attacks.
- Understanding log analysis and threat mitigation.
