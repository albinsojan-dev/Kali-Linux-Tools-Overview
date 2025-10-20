# Kali-Linux-Tools

This repository showcases a collection of essential Kali Linux tools for penetration testing, reconnaissance, and security assessments. Each tool is described with its primary functionality and use cases.

## Table of Contents

- [Reconnaissance](#reconnaissance-tools)
- [Network & Web](#network--web-tools)
- [Vulnerability Analysis](#vulnerability-analysis)
- [Wireless Attacks](#wireless-attacks)
- [Password Attacks](#password-attacks)
- [Exploitation](#exploitation-tools)
- [Post-Exploitation](#post-exploitation)
- [Social Engineering & Exploitation Tools](#social-engineering--exploitation-tools)
- [Forensics & Analysis](#forensics--analysis)
- [Web Application Testing](#web-application-testing)
- [Specialized & Miscellaneous Tools](#specialized--miscellaneous-tools)
- [Notes on Platform Support](#notes-on-platform-support)

---

### Reconnaissance Tools
| Tool | Description | Use Case | Supported Platforms |
|------|-------------|----------|---------------------|
| **SubBrute** | Discovers subdomains of a target website using a wordlist | Subdomain enumeration during reconnaissance | Kali, macOS, Windows |
| **sublist3r** | Enumerates subdomains of a target website through multiple sources | Passive subdomain discovery for security audits | Kali, macOS, Windows |
| **Assetfinder** | Discovers domains and subdomains associated with a specific target domain | Asset discovery in bug bounty hunting | Kali, macOS, Windows |
| **subfinder** | Subdomain enumeration tool for discovering valid subdomains of a website | Fast and comprehensive subdomain enumeration | Kali, macOS, Windows |
| **recon-ng** | Full-spectrum reconnaissance framework supporting domain enumeration, email harvesting, IP geolocation, and vulnerability assessment | Full reconnaissance workflow automation | Kali, macOS, Windows (with Python setup) |
| **nslookup** | Queries DNS servers to obtain domain name or IP address mappings and other DNS records | DNS query resolution and troubleshooting | Kali, macOS, Windows (native on Windows) |
| **theHarvester** | OSINT tool for gathering information about target domains or organizations during reconnaissance | Open-source intelligence gathering | Kali, macOS, Windows |
| **Gobuster** | Brute-force enumeration and discovery tool uncovering hidden resources on web servers | Directory and file enumeration | Kali, macOS, Windows |
| **DNSRecon** | Enumerates DNS records including A, MX, PTR, SPF and other record types | Comprehensive DNS information gathering | Kali, macOS, Windows |
| **Amass** | Advanced DNS enumeration and network mapping tool for OSINT reconnaissance | Large-scale domain and subdomain discovery | Kali, macOS, Windows |
| **Enum4linux-ng** | Windows and Samba enumeration tool for gathering domain and user information | Active Directory and SMB enumeration | Kali, Linux, macOS |
| **Exiflooter** | Extracts geolocation and metadata from images on URLs or directories | OSINT through metadata extraction | Kali, macOS, Windows |
| **Httpx** | Fast HTTP probe for validating live hosts and gathering web server information | Web server validation and probing | Kali, macOS, Windows |
| **Shodan-cli** | CLI interface for Shodan, a search engine for internet-connected devices | Internet-wide device reconnaissance | Kali, macOS, Windows |
| **Masscan** | High-speed port scanner for large network ranges and rapid reconnaissance | Large-scale port scanning and discovery | Kali, Linux, macOS |
| **Blood Hound** | Open-source tool that uses graph theory to visualize relationships and attack paths in Active Directory environments | Identifying privilege escalation paths and misconfigurations in AD for penetration testing and defense | Kali, macOS, Windows (cross-platform with Neo4j backend) |

### Network & Web Tools
| Tool | Description | Use Case | Supported Platforms |
|------|-------------|----------|---------------------|
| **Ngrok** | Creates secure tunnels from a local machine to the internet | Exposing local services for testing and collaboration | Kali, macOS, Windows |
| **httpprobe** | Tests availability and performance of web servers by sending HTTP requests | Web server health checks and validation | Kali, macOS, Windows |
| **bettercap** | Powerful tool for performing MITM attacks, network sniffing, and packet manipulation | Network attack simulation and traffic analysis | Kali, macOS, Windows (limited) |
| **netdiscover** | Network scanning tool discovering active devices by analyzing ARP traffic | Local network mapping and device discovery | Kali, Linux-focused (limited Windows) |
| **wafw00f** | Identifies and fingerprints Web Application Firewalls protecting websites | WAF detection for vulnerability testing | Kali, macOS, Windows |
| **whatweb** | Web scanner identifying technologies, CMS, and components of websites | Website fingerprinting and technology identification | Kali, macOS, Windows |
| **Nikto** | Open-source web server scanner identifying vulnerabilities and misconfigurations | Web server vulnerability assessment | Kali, macOS, Windows |
| **python3 -m http.server 8000** | Starts a simple built-in HTTP server serving files from current directory on port 8000 | Quick file serving for testing web applications | Kali, macOS, Windows (requires Python3) |
| **hydra** | Password-cracking tool performing brute-force attacks on various protocols | Brute-forcing login credentials for web and network services | Kali, macOS, Windows |
| **Wireshark** | Packet analyzer for capturing and inspecting network traffic in real-time | Network traffic analysis and protocol inspection | Kali, macOS, Windows |
| **Tcpdump** | Command-line packet analyzer for capturing and filtering network traffic | Network monitoring and packet capture | Kali, macOS, Windows |
| **Ettercap** | Suite for man-in-the-middle attacks including ARP poisoning and sniffing | Network attack simulation and credential harvesting | Kali, macOS, Linux |
| **Responder** | LLMNR/NBT-NS poisoning tool for Windows network credential harvesting | Credential capture from Windows networks | Kali, Linux, macOS |
| **Arpspoof** | Performs ARP spoofing to intercept network traffic and manipulate routing | Network manipulation and traffic interception | Kali, macOS, Linux |

### Vulnerability Analysis
| Tool | Description | Use Case | Supported Platforms |
|------|-------------|----------|---------------------|
| **Burp Suite** | Web vulnerability scanner for comprehensive testing of web application security | Advanced web application security assessment | Kali, macOS, Windows |
| **OWASP ZAP** | Web application security scanner finding vulnerabilities like XSS and SQL injection | OWASP-focused web application testing | Kali, macOS, Windows |
| **Tinja** | CLI tool for testing web pages for template injection vulnerabilities | Template injection vulnerability detection | Kali, macOS, Windows |
| **CRLfuzz** | Fast tool to scan for CRLF injection vulnerabilities in web applications | CRLF vulnerability assessment | Kali, Linux, macOS |
| **Wpscan** | WordPress-specific vulnerability scanner for themes, plugins, and user enumeration | WordPress security assessment | Kali, macOS, Windows |
| **OpenVAS** | Open-source vulnerability scanner for comprehensive network assessments | Enterprise-level vulnerability scanning | Kali, Linux, Windows (limited) |
| **Lynis** | System auditing tool checking Linux and Unix security configurations | Linux/Unix security hardening assessment | Kali, Linux, macOS |
| **Nuclei** | Fast and customizable vulnerability scanner for web and network services | Template-based vulnerability scanning | Kali, macOS, Windows |
| **Legion** | Automated network penetration testing framework with graphical interface | Automated and coordinated penetration testing | Kali, Linux |
| **Nessus** | Commercial vulnerability scanner for comprehensive network assessments | Professional-grade vulnerability management | Kali, macOS, Windows |

### Wireless Attacks
| Tool | Description | Use Case | Supported Platforms |
|------|-------------|----------|---------------------|
| **Aircrack-ng** | Wi-Fi security auditing including packet capture and WEP/WPA key cracking | Wireless network penetration testing | Kali, macOS, Linux |
| **Kismet** | Wireless network detector, sniffer, and IDS for Wi-Fi and Bluetooth | Passive wireless network discovery and analysis | Kali, macOS, Linux |
| **Fern WiFi Cracker** | GUI-based tool for auditing and cracking Wi-Fi networks | User-friendly wireless network testing | Kali, Linux |
| **Wifite** | Automated Wi-Fi attack tool for cracking WEP and WPA passwords | Streamlined wireless penetration testing | Kali, Linux, macOS |
| **Reaver** | Attacks WPS-enabled Wi-Fi routers to recover WPA/WPA2 passphrases | WPS vulnerability exploitation | Kali, Linux, macOS |
| **Airgeddon** | Multi-tool for Wi-Fi auditing including deauthentication and password cracking | Comprehensive wireless testing framework | Kali, Linux, macOS |
| **Eaphammer** | Exploits EAP vulnerabilities in Wi-Fi networks through man-in-the-middle attacks | Enterprise Wi-Fi penetration testing | Kali, Linux |

### Password Attacks
| Tool | Description | Use Case | Supported Platforms |
|------|-------------|----------|---------------------|
| **Hydra** | Password cracking tool performing brute-force attacks on various protocols | Brute-forcing credentials for multiple services | Kali, macOS, Windows |
| **John the Ripper** | Offline password cracker using dictionary and brute-force methods | Fast offline password hash cracking | Kali, macOS, Windows |
| **Hashcat** | Advanced password recovery tool using GPU acceleration for multiple hash types | High-speed GPU-accelerated password cracking | Kali, macOS, Windows |
| **Bopscrk** | Generates smart and customizable wordlists for targeted password cracking | Intelligent wordlist generation for password attacks | Kali, Linux, macOS |
| **Crunch** | Generates custom wordlists for password cracking based on user-defined patterns | Pattern-based wordlist creation | Kali, macOS, Windows |
| **CeWL** | Creates custom wordlists by crawling websites for unique words and phrases | Targeted dictionary generation from target websites | Kali, macOS, Windows |
| **Patator** | Multi-purpose brute-forcing tool for various protocols including FTP and SSH | Multi-protocol brute force attacks | Kali, Linux |
| **Medusa** | Modular brute-forcing tool for network service logins like SSH and FTP | Flexible network service credential testing | Kali, Linux, macOS |
| **RainbowCrack** | Uses precomputed rainbow tables for fast password cracking from hashes | Time-optimized offline password recovery | Kali, Linux, Windows |

### Exploitation Tools
| Tool | Description | Use Case | Supported Platforms |
|------|-------------|----------|---------------------|
| **Metasploit** | Comprehensive penetration testing framework for exploiting known vulnerabilities | Professional-grade exploitation and post-exploitation | Kali, macOS, Windows |
| **Sqlmap** | Automated tool for SQL injection testing and database takeover | SQL injection vulnerability exploitation | Kali, macOS, Windows |
| **Netexec** | Network service exploitation tool for assessing large-scale network environments | Rapid multi-system exploitation and reconnaissance | Kali, Linux |
| **Donut-shellcode** | Generates position-independent shellcode from executable payloads | Advanced shellcode generation for exploitation | Kali, Linux, Windows |
| **searchsploit** | Searchable local copy of Exploit-DB for offline exploit research | Quick exploit lookup and research | Kali, Linux, macOS |
| **BeEF** | Browser Exploitation Framework for targeting and manipulating web browsers | Advanced browser-based exploitation campaigns | Kali, macOS, Windows |
| **Sickle** | Shellcode development and analysis tool for custom exploit creation | Shellcode development and optimization | Kali, Linux |
| **RouterSploit** | Framework for exploiting vulnerabilities in routers and IoT devices | Router and IoT device penetration testing | Kali, Linux |
| **Armitage** | GUI front-end for Metasploit providing visual attack management and collaboration | Visual penetration testing coordination | Kali, macOS, Windows |
| **SQLNinja** | Specialized tool for exploiting SQL injection vulnerabilities for database access | Advanced SQL injection exploitation | Kali, Linux, macOS |

### Post-Exploitation
| Tool | Description | Use Case | Supported Platforms |
|------|-------------|----------|---------------------|
| **Empire** | Post-exploitation and adversary emulation framework with extensive modules | Advanced post-exploitation and persistence | Kali, Windows, macOS |
| **Mimikatz** | Extracts credentials, Kerberos tickets, and sensitive data from memory | Windows credential extraction and manipulation | Kali, Windows |
| **PowerSploit** | PowerShell-based post-exploitation framework for Windows systems | Windows post-exploitation automation | Kali, Windows |
| **Rubeus** | Raw Kerberos interaction and abuse tool for Active Directory manipulation | Advanced Active Directory exploitation | Kali, Windows |
| **Sharphound** | BloodHound data collector for Active Directory enumeration and analysis | Active Directory mapping for privilege escalation | Kali, Windows |
| **Bloodhound-ce-python** | Python-based ingestor for BloodHound Community Edition data collection | AD relationship analysis and attack path planning | Kali, Linux, macOS |
| **Hoaxshell** | Windows reverse shell payload generator using HTTP/HTTPS protocols | Alternative reverse shell generation and control | Kali, Windows |
| **Meterpreter** | Advanced post-exploitation shell with extensive capabilities and extensibility | Interactive post-exploitation operations | Kali, macOS, Windows |
| **Netcat** | Versatile networking tool for creating connections, backdoors, and reverse shells | Lightweight network communication and backdoor creation | Kali, macOS, Windows |
| **Evil-WinRM** | Windows Remote Management shell for post-exploitation on Windows systems | WinRM-based remote shell access | Kali, Windows, Linux |

### Social Engineering & Exploitation Tools
| Tool | Description | Use Case | Supported Platforms |
|------|-------------|----------|---------------------|
| **Zphisher** | Automates phishing page creation for popular websites and services | Social engineering training and phishing simulations | Kali, macOS, Windows |
| **Evil-Droid** | Creates, generates, and embeds malicious APK payloads for Android penetration | Android malware simulation and testing | Kali, Linux-focused (limited macOS/Windows) |
| **SET (Social-Engineer Toolkit)** | Comprehensive framework for social engineering attacks including phishing | Full-spectrum social engineering campaigns | Kali, macOS, Linux |
| **Phishing Frenzy** | Framework for creating and managing phishing campaigns at scale | Organizational phishing awareness campaigns | Kali, Linux, Windows |
| **Gophish** | Open-source phishing framework for simulated attacks and campaign management | Professional phishing simulation platform | Kali, macOS, Windows |

### Forensics & Analysis
| Tool | Description | Use Case | Supported Platforms |
|------|-------------|----------|---------------------|
| **Binwalk3** | Firmware analysis tool for extracting embedded files from firmware images | Embedded device and firmware analysis | Kali, Linux, macOS |
| **Autopsy** | Graphical interface for digital forensics investigations and file recovery | GUI-based digital forensics platform | Kali, macOS, Windows |
| **Volatility** | Memory forensics framework for analyzing RAM dumps and volatile memory | Advanced memory analysis and incident response | Kali, macOS, Windows |
| **Foremost** | Recovers files from disk images based on headers and footers | File carving and data recovery | Kali, Linux, macOS |
| **Sleuth Kit** | Collection of tools for disk image analysis and file recovery | Command-line forensics and file system analysis | Kali, macOS, Windows |
| **Pdf-parser** | Parses PDF documents to identify fundamental elements and structures | PDF malware analysis and inspection | Kali, Linux, macOS |
| **Pdfid** | Scans PDF files for keywords indicating suspicious content like JavaScript | PDF threat detection and analysis | Kali, Linux, macOS |
| **Bulk Extractor** | Extracts structured data like emails and URLs from disk images | Large-scale data extraction from forensic images | Kali, Linux, macOS |

### Web Application Testing
| Tool | Description | Use Case | Supported Platforms |
|------|-------------|----------|---------------------|
| **Dirb** | Web directory scanner finding hidden directories and files on web servers | Directory and file enumeration on web servers | Kali, macOS, Windows |
| **Ffuf** | Fast web fuzzer for discovering hidden files, directories, and parameters | High-speed web content discovery and fuzzing | Kali, macOS, Windows |
| **Graudit** | Source code auditing tool for identifying security vulnerabilities in code | Static code analysis for vulnerability detection | Kali, Linux, macOS |
| **Sqlmc** | SQL injection testing and vulnerability assessment tool | SQL injection vulnerability validation | Kali, Linux, macOS |
| **Wfuzz** | Web application fuzzer for discovering hidden content and vulnerabilities | Comprehensive web application fuzzing | Kali, macOS, Windows |
| **Commix** | Automated tool for exploiting command injection vulnerabilities in web apps | Command injection vulnerability testing | Kali, macOS, Windows |
| **XSSer** | Automated XSS vulnerability scanner and exploitation tool | Cross-site scripting detection and exploitation | Kali, macOS, Windows |

### Specialized & Miscellaneous Tools
| Tool | Description | Use Case | Supported Platforms |
|------|-------------|----------|---------------------|
| **CARsenal** | Car hacking toolkit for interacting with CAN networks and automotive systems | Vehicle security testing and CAN bus analysis | Kali, Linux |
| **ICSim** | Simulator for testing CARsenal toolkit and automotive protocols without hardware | Virtual automotive security testing environment | Kali, Linux |
| **Chisel** | Fast TCP/UDP tunnel useful for network pivoting and traffic forwarding | Lightweight tunneling for network segmentation bypass | Kali, macOS, Windows |
| **Ligolo-ng** | Advanced tunneling tool designed specifically for network pivoting scenarios | Sophisticated network pivoting and tunnel management | Kali, Linux, macOS |
| **ImHex** | Hex editor designed for reverse engineers and security researchers | Binary analysis and reverse engineering | Kali, macOS, Windows |
| **Kustomize** | Customization tool for Kubernetes YAML configurations | Kubernetes security and configuration testing | Kali, Linux, macOS |
| **Rekono** | Automation platform combining multiple hacking tools for streamlined pentesting | Integrated pentesting workflow automation | Kali, Linux |
| **P0f** | Identifies operating systems via passive packet analysis without generating traffic | Stealthy OS fingerprinting and reconnaissance | Kali, Linux, macOS |
| **Dradis** | Collaborative reporting platform for organizing penetration testing results | Team-based penetration testing documentation | Kali, macOS, Windows |
| **Faraday** | Collaborative penetration testing and vulnerability management platform | Enterprise vulnerability and test management | Kali, macOS, Windows |
| **ZMap** | Fast internet-wide scanning tool for large-scale network discovery | Rapid internet-scale reconnaissance and scanning | Kali, Linux |

### Notes on Platform Support
- **Kali Linux**: All tools listed are natively supported or easily installable on Kali Linux, as it is a security-focused distribution designed for penetration testing and reconnaissance.
- **macOS**: Most tools are supported via package managers like Homebrew or by compiling from source. Some tools (e.g., netdiscover, Evil-Droid) may require additional setup or dependencies.
- **Windows**: Many tools work on Windows with proper setup (e.g., Python, Go, or WSL for Linux-based tools). However, some tools like netdiscover and Evil-Droid have limited or no native Windows support and may require a Linux environment (e.g., WSL or a virtual machine).
- Tools like `nslookup` and `python3 -m http.server` are available on Windows natively or with minimal setup (e.g., Python installation).
- Always verify tool compatibility with the specific version of your operating system and ensure you have the necessary dependencies installed.

## Installation & Usage

Most tools are pre-installed in Kali Linux. For others:

```bash
# Update your system
sudo apt update && sudo apt upgrade

# Install specific tools (examples)
sudo apt install recon-ng theharvester nikto whatweb cewl metasploit-framework

# For GitHub-based tools, clone repositories
git clone https://github.com/htr-tech/zphisher.git
git clone https://github.com/projectdiscovery/subfinder.git
# ... and so on
```

**Note:** Always run tools with appropriate permissions (e.g., `sudo` for network tools) and ensure you have written authorization for security testing.

## Ethical Guidelines

- Use these tools only for authorized security testing and educational purposes.
- Unauthorized access to computer systems is illegal and unethical.
- Comply with all applicable local laws and regulations.
- Obtain explicit written permission before conducting any security assessments.
- Document all testing activities and maintain confidentiality of findings.

## Contributing

Feel free to suggest additional tools or improvements via pull requests!

## License

This documentation is licensed under MIT. Tools themselves may have their own licenses—check individual repositories for specific licensing information.
