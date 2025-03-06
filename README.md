# 🔍 Cisco Configuration File Auditing Tool (CCFAT)

This executable analyzes a **Cisco IOS configuration file** and verifies compliance with **recommended security best practices**
## 📌 Key Compliance Checks

The tool ensures your configuration aligns with security best practices by checking for:

✅ **Basic Security Hardening**  
- Disabling **IP domain lookup**  
- Configuring an **enable secret** and **username secret**  
- Enabling **AAA new-model** and **AAA authentication** for login and enable  

✅ **User & Privilege Management**  
- Ensuring **local user privilege** is set to **1** (no high-privilege default accounts)  
- Configuring **VTY, console, and TTY exec-timeout** values (≤10 minutes)  

✅ **Network Services & Protocols**  
- Disabling **CDP, BOOTP, DHCP, IP identd, source routing, and PAD service**  
- Enabling **TCP keepalives** (in and out)  

✅ **SSH & Authentication Hardening**  
- Configuring **SSH timeout, authentication retries**, and enforcing **SSH version 2**  
- Setting a **domain name** and generating **RSA keys** (modulus ≥ 2048)  

✅ **Logging & Monitoring**  
- Configuring logging (**on, buffered, console, syslog host, trap level, timestamps, source-interface**)  
- Ensuring **NTP servers** are configured  

✅ **SNMP & Banner Security**  
- Checking **SNMP community strings** to avoid insecure default values  
- Setting **banner MOTD, login, and exec banners**  

✅ **Default & Insecure Accounts**  
- Identifying generic or default usernames (e.g., `admin`, `cisco`, `test`, `demo`, `guest`, `default`, `administrator`)  

---

⚡ **Ensure your Cisco IOS configurations meet industry security standards!**  
💡 Feel free to contribute, submit issues, or request features. 🚀

Building cool things in tech ☁️ | Open-source & security 🚀 | Fuel my work ☕ → https://www.buymeacoffee.com/alfie
