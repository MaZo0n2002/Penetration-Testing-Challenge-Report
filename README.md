# 🔐 SecureTeam CTF Report – Cybersecurity Portfolio

This repository contains a detailed penetration testing report created as part of a university-level cybersecurity course project. The task involved identifying and exploiting vulnerabilities across three escalating flags, ultimately gaining root access to a vulnerable system.

> 🧑‍💻 **Author**: Mazen Mostafa Ahmed Abdelhafez  
> 🎓 **University**: German University in Cairo (GUC)  
> 📬 **Email**: mazen.mabdelhafez2002@gmail.com

---

## 🗂️ Project Overview

This Capture The Flag (CTF)-style challenge was completed collaboratively with my team, **SecureTeam**, to simulate real-world penetration testing. The report documents every step of the engagement, including scanning, exploitation, privilege escalation, and post-exploitation.

### 🔎 Contents
- `Team_19_Secure_Team.pdf`: Full technical report with screenshots, commands, and Q&A for each phase.

---

## 🚩 Flags Breakdown

### ✅ Flag 1 – Web Enumeration & Command Injection
- Aggressive Nmap scanning to identify open ports (80, 443, 5432)
- Directory enumeration using `dirb`
- SQL Injection on login form at `/index.php`
- Command injection to gain a reverse shell
- Extracted encoded data and decoded using CyberChef

### ✅ Flag 2 – Local Enumeration & Decoding
- File enumeration using `find` and user analysis
- Hex-encoded flag hidden among fake decoys
- Decoded using CyberChef to retrieve the flag

### ✅ Flag 3 – Privilege Escalation to Root
- Kernel version enumeration (`uname -a`)
- Identified known vulnerability in CentOS 4.5 (kernel 2.6.9)
- Used `searchsploit` to find exploit (9479.c)
- Hosted and transferred exploit to victim machine
- Compiled and executed to gain root access

---

## 🛠️ Tools & Techniques

| Tool        | Purpose                              |
|-------------|--------------------------------------|
| `nmap`      | Port scanning & service enumeration  |
| `dirb`      | Directory brute-forcing              |
| `sqlmap`    | SQL Injection (manually exploited)   |
| `netcat`    | Reverse shell setup                  |
| `CyberChef` | Decoding encoded strings             |
| `searchsploit` | Finding privilege escalation exploits |
| `wget`, `gcc`, `bash` | Exploit delivery and execution |

---

## 📌 Key Takeaways

- Demonstrated understanding of common vulnerabilities like SQL Injection and OS Command Injection
- Gained hands-on experience with Linux privilege escalation
- Strengthened teamwork and structured reporting in cybersecurity scenarios

---


