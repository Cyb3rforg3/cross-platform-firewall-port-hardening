# cross-platform-firewall-port-hardening
Cybersecurity Internship project -secure-port-contro-windows-linux  Task 4
# 🔐 Cross-Platform Firewall Port Hardening

This project demonstrates how to **block and allow specific ports** across both **Windows** and **Kali Linux** to secure systems from unauthorized access, exploits, and malware callbacks. It uses **Windows Defender Firewall (via GUI and PowerShell)** and **UFW/iptables on Kali Linux**.

---

## 📖 About the Project

The goal of this project is to implement **port-level security** by allowing only necessary ports (e.g., SSH) and blocking known vulnerable or unnecessary ports such as:

- 21 (FTP)
- 23 (Telnet)
- 135-139 (NetBIOS)
- 445 (SMB)
- 1433-1434 (SQL Server)
- 3389 (RDP, if unused)

It covers:
- Creating rules using GUI & CLI
- Validating open/closed ports
- Logging blocked attempts
- Cross-platform comparisons

---

## 🧰 Technologies Used

- 🔒 Windows Defender Firewall
- 💻 PowerShell
- 🐧 Kali Linux
- 🔥 UFW (`Uncomplicated Firewall`)
- 🧱 iptables
- 🧪 nmap, telnet, netcat

---

## 🚧 Firewall Rules Implemented

| OS           | Port | Protocol | Action |
|--------------|------|----------|--------|
| Windows      | 21, 23, 445 | TCP | Block |
| Kali Linux   | 21, 23, 445 | TCP | Block |
| Both         | 22          | TCP | Allow (SSH) |

---

## 📁 Folder Structure
cross-platform-firewall-port-hardening/
├── 
README.md
├── LICENSE
├── .gitignore
├── windows/
│   ├── Report.md
│   └── screenshots/
│       ├── After set up rule.png
|       ├── setting a  rule(1).png
|       ├── setting a  rule(2).png
|       ├── setting a  rule(3).png
|       ├── setting a  rule(4).png
|       ├── setting a  rule(5).png
│       └── Windows_logs.png
│   
├── kali-linux/
│   ├── Report.md
|
└─── test/
      └── nmap_test_results.md
