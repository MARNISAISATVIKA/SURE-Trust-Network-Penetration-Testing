Network Penetration Testing Report

Project Title: Black Box Approach for Multiple IPs
Domain: Cybersecurity & Ethical Hacking (VAPT)
Duration: January 2025 - February 2025
Mentor: Mr. Nishchay Gaba (Cybersecurity Researcher at Hacking Articles)

Overview
Conducted black box penetration testing on 30 public IP addresses to identify security vulnerabilities from an external attacker's perspective. Combined automated scanning with manual validation to assess network security posture.

Key Findings

Critical Vulnerabilities (4)
- Unpatched RDP (CVE-2019-0708): Allows remote code execution
- SSLv2/SSLv3 exposure (CVE-2016-0800): Vulnerable to DROWN attacks
- Default credentials on Telnet services
- Outdated TLS configurations

High Risk Vulnerabilities (5)
- OpenSSH user enumeration (CVE-2018-15473)
- Weak TLS configurations (Logjam, BEAST, ROBOT)
- Unencrypted credential transmission

Medium Risk Vulnerabilities (4)
- SSH command injection (CVE-2020-15778)
- Weak ciphers (SWEET32, RC4)

Low Risk Vulnerabilities (1)
- Anonymous FTP access

Methodology
1. Reconnaissance: WHOIS lookups, DNS analysis, port scanning
2. Vulnerability Assessment: Automated scanning with OpenVAS
3. Manual Validation: Exploit verification using Metasploit
4. Reporting: Documented findings with PoC evidence

Tools Used
- Scanning: Nmap, OpenVAS, Masscan
- Exploitation: Metasploit, Burp Suite
- Analysis: Wireshark, SSLScan
- Reporting: Dradis, LaTeX

Recommendations
1. Immediate Actions:
   - Patch critical vulnerabilities (RDP, SSLv2/SSLv3)
   - Disable Telnet and outdated protocols
   - Enforce TLS 1.2/1.3 across all services

2. Long-term Improvements:
   - Implement continuous vulnerability scanning
   - Conduct regular penetration testing
   - Provide security training for staff

License
MIT License - See LICENSE file for details. 
