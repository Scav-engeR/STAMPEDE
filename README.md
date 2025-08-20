# 🎯 STAMPEDE - Educational Vulnerability Scanner

<div align="center">

```
███████╗████████╗ █████╗ ███╗   ███╗██████╗ ███████╗██████╗ ███████╗
██╔════╝╚══██╔══╝██╔══██╗████╗ ████║██╔══██╗██╔════╝██╔══██╗██╔════╝
███████╗   ██║   ███████║██╔████╔██║██████╔╝█████╗  ██║  ██║█████╗  
╚════██║   ██║   ██╔══██║██║╚██╔╝██║██╔═══╝ ██╔══╝  ██║  ██║██╔══╝  
███████║   ██║   ██║  ██║██║ ╚═╝ ██║██║     ███████╗██████╔╝███████╗
╚══════╝   ╚═╝   ╚═╝  ╚═╝╚═╝     ╚═╝╚═╝     ╚══════╝╚═════╝ ╚══════╝
```

### 🎓 **STRICTLY FOR EDUCATIONAL PURPOSES** 🎓
*A comprehensive vulnerability scanner designed for cybersecurity education and authorized security assessments*

[![Python](https://img.shields.io/badge/Python-3.9+-blue.svg)](https://python.org)
[![License](https://img.shields.io/badge/License-Educational%20Use%20Only-red.svg)](#license)
[![Security](https://img.shields.io/badge/Purpose-Educational%20Security%20Research-green.svg)](#educational-purpose)

**Created by:** [@scav-enger](https://github.com/Scav-engeR) | **Telegram:** @Ghiddra

</div>

---

## 🚨 **CRITICAL EDUCATIONAL DISCLAIMER**

> **⚠️ THIS TOOL IS EXCLUSIVELY FOR EDUCATIONAL PURPOSES ⚠️**

### 📚 **Educational Objectives**
- Learn about common web application vulnerabilities
- Understand security assessment methodologies  
- Practice ethical hacking techniques in controlled environments
- Develop defensive security skills and awareness

### ✅ **Authorized Use Cases**
- **Educational Labs:** Cybersecurity courses and training environments
- **Personal Learning:** Testing on your own systems and applications
- **Authorized Research:** Security research with proper permissions
- **Professional Training:** Corporate security training programs
- **Capture The Flag (CTF):** Educational CTF competitions

### 🚫 **STRICTLY PROHIBITED**
- Testing websites or systems without explicit written authorization
- Any malicious, illegal, or unethical activities
- Unauthorized penetration testing or security assessments
- Any activity that violates local, state, federal, or international laws

---

## 🎯 **What is STAMPEDE?**

STAMPEDE is an educational vulnerability scanner designed to help cybersecurity students, professionals, and researchers understand common web application security flaws. It tests for **40+ different vulnerability types** commonly found in web applications, providing hands-on learning opportunities for those studying cybersecurity.

### 🧠 **Learning Focus Areas**
- **OWASP Top 10 Vulnerabilities**
- **Injection Attacks** (SQL, Command, LDAP, etc.)
- **Cross-Site Scripting (XSS)**
- **Security Misconfigurations**
- **Authentication & Session Management Flaws**
- **HTTP Security Headers**
- **File Upload Vulnerabilities**

---

## 🔍 **Vulnerability Detection Capabilities**

<details>
<summary><b>📋 Complete Vulnerability List (40+ Types)</b></summary>

### **Injection Vulnerabilities**
- ✅ SQL Injection (Basic & Blind)
- ✅ Command Injection  
- ✅ LDAP Injection
- ✅ Server-Side Template Injection (SSTI)
- ✅ Client-Side Template Injection (CSTI)
- ✅ XXE (XML External Entity)
- ✅ XXE via SVG File Upload
- ✅ SSI (Server-Side Includes) Injection

### **Cross-Site Scripting (XSS)**
- ✅ Reflected XSS
- ✅ Stored XSS Detection
- ✅ DOM-based XSS Patterns

### **File System Vulnerabilities**
- ✅ Local File Inclusion (LFI)
- ✅ Remote File Inclusion (RFI)
- ✅ Path Traversal
- ✅ Directory Listing
- ✅ Unrestricted File Upload

### **Authentication & Session Management**
- ✅ Cross-Site Request Forgery (CSRF)
- ✅ Session Fixation
- ✅ Insecure Authentication

### **HTTP Security Issues**
- ✅ HTTP Header Injection
- ✅ Host Header Injection
- ✅ HTTP Parameter Pollution (HPP)
- ✅ HTTP Verb Tampering
- ✅ HTTP Method Override
- ✅ HTTP Response Splitting
- ✅ CRLF Injection

### **Advanced Attack Vectors**
- ✅ Server-Side Request Forgery (SSRF)
- ✅ Open Redirect
- ✅ Clickjacking
- ✅ Insecure CORS Configuration
- ✅ Cache Poisoning
- ✅ HTTP Smuggling
- ✅ HTTP Desync Attacks
- ✅ Web Cache Deception

### **Information Disclosure**
- ✅ Sensitive Data Exposure
- ✅ Subdomain Takeover
- ✅ Email Header Injection

### **Deserialization & Data Processing**
- ✅ Insecure Deserialization
- ✅ HPP in Headers

</details>

---

## 🛠 **Installation & Setup**

### **Prerequisites**
```bash
# Preferably Python 3.9 or higher
python3 --version

# Required Python packages
python3.x -m pip install -r requirements.txt
```

### **Optional: Rainbow Colors with Lolcat**
```bash
# Ubuntu/Debian
sudo apt-get update && sudo apt-get install lolcat

# macOS
brew install lolcat

# Arch Linux
sudo pacman -S lolcat

# CentOS/RHEL/Fedora
sudo yum install ruby
gem install lolcat
```

### **Quick Start**
```bash
# Clone the repository
git clone https://github.com/Scav-engeR/STAMPEDE.git
cd STAMPEDE

# Make executable
chmod +x STAMPEDE.py

# Create a target list file
echo "http://testphp.vulnweb.com" > targets.txt
echo "http://demo.testfire.net" >> targets.txt

# Run the scanner (EDUCATIONAL USE ONLY!)
python3 STAMPEDE.py
or
python3 STAMPEDE.py -f targets.txt
```

---

## 📖 **Usage Guide**

### **Command Line Options**
```bash
python3 STAMPEDE.py
or
python3 STAMPEDE.py -f <target_file>
```

### **Educational Testing Environments**
For hands-on learning, use these legal testing platforms:

#### **Free Vulnerable Applications**
- **DVWA** (Damn Vulnerable Web Application)
- **WebGoat** by OWASP
- **Mutillidae II**
- **bWAPP** (buggy Web Application)
- **VulnHub VMs**

#### **Online Testing Platforms**
- **TryHackMe** - Cybersecurity training platform
- **HackTheBox** - Penetration testing labs
- **PortSwigger Web Security Academy**
- **OverTheWire** - Security wargames

---

## 📊 **Output & Results**

### **Console Output**
```
[INFO] Testing http://example.com
[VULNERABLE] SQL Injection Vulnerable: http://example.com
[INFO] XSS Not Vulnerable: http://example.com
[SUCCESS] Scanning complete.
```

### **Log Files**
- `logs/log.txt` - Detailed scan logs
- `logs/success.txt` - Vulnerability findings only

---

## 🔧 **Configuration**

### **Threading (Default: 1 thread)**
```python
# In main() function, adjust thread count (MAX: 10)
for _ in range(5):  # Change from 1 to desired number
    t = threading.Thread(target=worker, args=(url_queue,))
```

### **Timeout Settings**
```python
# Adjust request timeouts in make_request() function
response = requests.get(url, verify=False, timeout=10)  # 10 seconds
```

---

## 🎓 **Educational Resources**

### **Learning Materials**
- [OWASP Web Security Testing Guide](https://owasp.org/www-project-web-security-testing-guide/)
- [PortSwigger Web Security Academy](https://portswigger.net/web-security)
- [SANS Web Application Security](https://www.sans.org/cyber-security-courses/web-app-penetration-testing-ethical-hacking/)

### **Responsible Disclosure**
Learn about responsible disclosure practices:
- [HackerOne Disclosure Guidelines](https://www.hackerone.com/disclosure-guidelines)
- [CERT Vulnerability Disclosure Policy](https://vuls.cert.org/confluence/display/CVD)

### **Legal Resources**
- [Computer Fraud and Abuse Act (CFAA)](https://www.justice.gov/criminal-ccips/computer-fraud-and-abuse-act)
- [Ethical Hacking Guidelines](https://www.sans.org/white-papers/34720/)

---

## ⚖️ **Legal & Ethical Guidelines**

### **🔒 Authorization Requirements**
- **Always obtain explicit written permission** before testing any system
- **Document your authorization** before beginning any security assessment
- **Respect scope limitations** defined in your authorization
- **Follow responsible disclosure** practices for any findings

### **📋 Pre-Testing Checklist**
- [ ] I have written authorization to test this system
- [ ] I understand the scope and limitations of my authorization
- [ ] I will not access, modify, or destroy data beyond what's necessary
- [ ] I will report findings through proper channels
- [ ] I understand the legal implications of my actions

### **🌟 Ethical Principles**
1. **Do No Harm** - Never damage systems or compromise data
2. **Respect Privacy** - Protect any sensitive information encountered
3. **Professional Conduct** - Maintain the highest ethical standards
4. **Continuous Learning** - Use knowledge to improve security posture

---

## 🤝 **Contributing to Security Education**

### **How to Contribute**
- Report bugs and suggest improvements
- Add new educational vulnerability checks
- Improve documentation and learning resources
- Share educational use cases and scenarios

### **Development Guidelines**
- All contributions must maintain educational focus
- Include proper error handling and logging
- Add educational comments explaining vulnerability concepts
- Follow responsible disclosure for any real vulnerabilities found

---

## 📞 **Support & Community**

### **Educational Support**
- **GitHub Issues:** Report bugs or request educational features
- **Discussions:** Share learning experiences and ask questions
- **Documentation:** Contribute to educational resources

### **Security Community**
- **OWASP Local Chapters:** Join your local cybersecurity community
- **Security Conferences:** DEF CON, BSides, OWASP events
- **Online Forums:** Reddit r/netsec, Information Security Stack Exchange

---

## ⭐ **Acknowledgments**

### **Educational Inspiration**
- **OWASP Foundation** - For web security education resources
- **Cybersecurity Community** - For sharing knowledge and best practices
- **Vulnerable Applications** - DVWA, WebGoat, and other educational platforms

### **Security Researchers**
Thanks to the cybersecurity community for advancing security education and making the internet safer for everyone.

---

## 📄 **License**

```
EDUCATIONAL USE ONLY LICENSE

This software is provided strictly for educational purposes only.

PERMITTED USES:
✅ Educational and learning purposes
✅ Authorized security research
✅ Personal systems and applications you own
✅ Systems with explicit written permission

PROHIBITED USES:
❌ Unauthorized access to any system
❌ Malicious or illegal activities
❌ Commercial use without proper licensing
❌ Any activity violating applicable laws

By using this software, you agree to use it responsibly and ethically.
The author assumes no responsibility for misuse or illegal activities.
```

---

## 🔗 **Important Links**

- **🏠 Repository:** [github.com/Scav-engeR/STAMPEDE](https://github.com/Scav-engeR/STAMPEDE)
- **📚 OWASP:** [owasp.org](https://owasp.org)
- **🎯 PortSwigger Academy:** [portswigger.net/web-security](https://portswigger.net/web-security)
- **🛡️ SANS Security:** [sans.org](https://sans.org)

---

<div align="center">

### 🎓 **Remember: With Great Power Comes Great Responsibility** 🎓

*Use your cybersecurity knowledge to protect and defend, not to harm or exploit.*

**Happy Learning! 🚀**

---

**Created with ❤️ for the cybersecurity education community**

**© 2024 @scav-enger - Educational Use Only**

</div>
