# Metasploitable 2 - VAPT Project

This repository documents a full Vulnerability Assessment and Penetration Testing (VAPT) process carried out against the intentionally vulnerable **Metasploitable 2** virtual machine.

## 🎯 Objective

To identify and exploit real-world vulnerabilities using professional penetration testing methodologies and tools such as **Nikto** and **Metasploit**, culminating in shell access and privilege escalation.

---

## 🛠️ Tools Used

- **Kali Linux (Attacker Machine)**
- **Nikto** – Web server vulnerability scanner
- **Metasploit Framework** – Exploitation and payload management

---

## 📋 Steps Performed

1. **Service Enumeration** (via Nmap & manual browsing)
2. **Nikto Scan** of the target web server
3. **Exploitation using Metasploit:**
   - `exploit/unix/ftp/vsftpd_234_backdoor`
   - `exploit/multi/http/php_cgi_arg_injection`
   - `exploit/multi/http/apache_mod_cgi_bash_env_exec`
4. **Obtained Shell Access** via Meterpreter
5. **Privilege Escalation** attempt from `www-data` to `root`

---

## 📂 Files Included

- `VAPT_Report.pdf`: Detailed step-by-step report
- `nikto_scan.txt`: Raw Nikto scan output
- `exploit_steps.md`: Manual breakdown of Metasploit module usage
- `metasploit_commands.txt`: Commands used during the session
- `/screenshots/`: Key visual proof of successful exploitation

---

## 📷 Screenshots

| Screenshot | Description |
|------------|-------------|
| `nikto_results.png` | Vulnerabilities detected by Nikto |
| `metasploit_shell_access.png` | Gaining shell using Apache exploit |
| `meterpreter_session.png` | Meterpreter session opened |
| `privilege_escalation_attempt.png` | Attempt to escalate from www-data to root |

---

## 📄 Final Report

See the PDF report: [`VAPT_Report.pdf`](./VAPT_Report.pdf) for a full write-up of the engagement.

---

## ⚠️ Disclaimer

> This project was performed in a **legal, controlled lab environment** using Metasploitable 2 for educational purposes only.  
> Do not attempt these techniques on any system without **explicit permission**.

---

## ⭐ Highlights

- Discovered multiple critical web and FTP vulnerabilities
- Gained low-privilege shell access on the target system
- Demonstrated hands-on Metasploit usage for real-world attack chains

---
