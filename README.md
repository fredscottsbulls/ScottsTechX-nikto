# 🔍 ScottsTechX Nikto

<p align="center">
  <img src="https://img.shields.io/badge/Nikto-Web-Scanner-00ff88?style=for-the-badge&logo=linux&logoColor=black" alt="Nikto"/>
  <img src="https://img.shields.io/badge/Web-Security-00ff88?style=for-the-badge&logo=shield&logoColor=black" alt="Web Security"/>
</p>

> **Web server vulnerability scanner — find misconfigs, outdated software, and known CVEs.**

---

## ⚡ What It Does

Nikto scans web servers for 7000+ known vulnerabilities, misconfigurations, dangerous files, and outdated software versions. Essential for initial web reconnaissance.

## 🚀 Quick Usage

```bash
# Basic scan
nikto -h target.com

# Full scan with tuning
nikto -h target.com -T 1-6

# Scan specific ports
nikto -h target.com -p 80,443,8080

# Save output
nikto -h target.com -o results.xml -Format xml

# Evade detection (slow)
nikto -h target.com -evasion +Tuning 1
```

## 🛡 Bug Bounty

```bash
nikto -h https://target.com -ssl -timeout 30
nikto -h target.com -plugins "+@ALL" -maxtime 2h
```

---

MIT © 2026
