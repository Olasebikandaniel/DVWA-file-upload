# DVWA File Upload → Remote Code Execution Lab Exploits (2026 Kali Vibes)

Hands-on exploitation of **Damn Vulnerable Web Application (DVWA)** File Upload vulnerability across security levels.

What we dropped:
- Weevely stealth PHP backdoor generation + upload → agent connect-back
- Custom `exploit.php` webshell with Metasploit-style reverse shell handling
- Metasploit `msfvenom` polyglot.php payload + multi/handler setup for reverse_tcp
- Bypass techniques: double extensions, MIME spoofing, path traversal chaining
- Screenshots of every stage — from upload success → shell → whoami → full filesystem recon

All in a controlled VirtualBox Kali → DVWA localhost:4280 lab.  
For educational/red-team practice only. Never run this against anything you don't own.

Tools chain: Kali Linux • Weevely • Metasploit • DVWA (low/medium/high)

Learning outcome → Understand why unrestricted file upload = instant RCE gateway, and how modern WAFs/input validation still get slept on in 2026.

Star if it helped your OSCP prep or Sunday lab grind. PRs welcome for high-sec bypass variants. 🛡️→💀
