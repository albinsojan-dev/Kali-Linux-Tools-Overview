# Kali-Linux-Tools

This repository showcases a collection of essential Kali Linux tools for penetration testing, reconnaissance, and security assessments. Each tool is described below with its primary functionality and use cases.

## Featured Tools

### Reconnaissance Tools
| Tool | Description | Use Case | Supported Platforms |
|------|-------------|----------|---------------------|
| **SubBrute** | SubBrute is designed to discover subdomains of a target website by using a wordlist | Subdomain enumeration during reconnaissance | Kali, macOS, Windows |
| **sublist3r** | Sublist3r tool designed for enumerating subdomains of a target website | Passive subdomain discovery for security audits | Kali, macOS, Windows |
| **Assetfinder** | To discover domains and subdomains associated with a specific target domain | Asset discovery in bug bounty hunting | Kali, macOS, Windows |
| **subfinder** | Subdomain enumeration tool for discovering valid subdomains of a website | Fast and comprehensive subdomain enumeration | Kali, macOS, Windows |
| **recon-ng** | Supports tasks like domain enumeration, email harvesting, IP geolocation, and vulnerability assessment | Full-spectrum reconnaissance framework | Kali, macOS, Windows (with Python setup) |
| **nslookup** | Used to query DNS servers to obtain domain name or IP address mappings, or other DNS records | DNS query resolution and troubleshooting | Kali, macOS, Windows (native on Windows, available on Kali/macOS) |
| **theHarvester** | OSINT tool designed for gathering information about a target domain or organization during the reconnaissance phase | Open-source intelligence gathering | Kali, macOS, Windows |
| **Gobuster** | Designed for brute-force enumeration and discovery in web security testing, uncovering hidden resources on web servers | Directory-listing | Kali, macOS, Windows |

### Network & Web Tools
| Tool | Description | Use Case | Supported Platforms |
|------|-------------|----------|---------------------|
| **Ngrok** | A cross-platform tool that creates secure tunnels from a local machine to the internet | Exposing local web servers to the public internet for testing | Kali, macOS, Windows |
| **httpprobe** | Tests the availability and performance of web servers or APIs by sending HTTP requests and checking for expected responses | Web server health checks and probing | Kali, macOS, Windows |
| **bettercap** | A powerful, flexible tool for performing man-in-the-middle (MITM) attacks, network sniffing, and packet manipulation | Network attack simulation and traffic analysis | Kali, macOS, Windows (limited Windows support) |
| **netdiscover** | A network scanning tool designed to discover active devices on a network by analyzing ARP traffic | Local network mapping and device discovery | Kali, macOS (with compilation), Linux-focused (limited Windows support) |
| **wafw00f** | Identifies and fingerprints Web Application Firewalls (WAFs) protecting websites | WAF detection for web vulnerability testing | Kali, macOS, Windows |
| **whatweb** | A web scanner that identifies technologies, CMS, and other components of a website | Website fingerprinting and technology identification | Kali, macOS, Windows |
| **Nikto** | An open-source web server scanner designed to identify vulnerabilities and misconfigurations in web servers and applications | Web server vulnerability scanning | Kali, macOS, Windows |
| **python3 -m http.server 8000** | Starts a simple built-in HTTP server using Python's http.server module, serving files from the current working directory over HTTP on port 8000 | Quick file serving for testing web applications | Kali, macOS, Windows (requires Python3 installation) |
| **hydra** | A password-cracking tool that performs brute-force attacks on various protocols, including HTTP POST forms, using username and password wordlists | Brute-forcing login credentials for web applications or network services | Kali, macOS, Windows |

### Social Engineering & Exploitation Tools
| Tool | Description | Use Case | Supported Platforms |
|------|-------------|----------|---------------------|
| **Zphisher** | Automates the creation of phishing pages for websites like Facebook, Instagram, Google | Social engineering and phishing simulations for awareness training | Kali, macOS, Windows |
| **Evil-Droid** | Creates, generates, and embeds malicious APK payloads to penetrate Android devices | Android penetration testing and malware simulation | Kali, Linux-focused (limited macOS/Windows support with setup) |
| **cewl** | A custom wordlist generator that crawls a website to create tailored password lists for brute-force attacks | Custom dictionary creation for password cracking | Kali, macOS, Windows |

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
sudo apt install recon-ng theharvester nikto whatweb cewl
# For GitHub-based tools, clone repositories
git clone https://github.com/htr-tech/zphisher.git
git clone https://github.com/projectdiscovery/subfinder.git
# ... and so on
```

**Note:** Always run tools with appropriate permissions (e.g., `sudo` for network tools) and ensure you have authorization for testing.

## Ethical Guidelines

- Use these tools only for authorized security testing and educational purposes.
- Unauthorized access to systems is illegal and unethical.
- Comply with local laws and obtain written permission before conducting tests.

## Contributing

Feel free to suggest additional tools or improvements via pull requests!

## License

This documentation is licensed under MIT. Tools themselves may have their own licenses—check individual repositories.
</artifact>

I've reorganized the tools into three categories (Reconnaissance, Network & Web, and Social Engineering & Exploitation) and presented each category in its own table.
