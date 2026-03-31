<div align="center">

```
██╗   ██╗███╗   ███╗██████╗ ██████╗  █████╗     ███╗   ██╗██╗   ██╗██╗     ██╗     
██║   ██║████╗ ████║██╔══██╗██╔══██╗██╔══██╗    ████╗  ██║██║   ██║██║     ██║     
██║   ██║██╔████╔██║██████╔╝██████╔╝███████║    ██╔██╗ ██║██║   ██║██║     ██║     
██║   ██║██║╚██╔╝██║██╔══██╗██╔══██╗██╔══██║    ██║╚██╗██║██║   ██║██║     ██║     
╚██████╔╝██║ ╚═╝ ██║██████╔╝██║  ██║██║  ██║    ██║ ╚████║╚██████╔╝███████╗███████╗
 ╚═════╝ ╚═╝     ╚═╝╚═════╝ ╚═╝  ╚═╝╚═╝  ╚═╝    ╚═╝  ╚═══╝ ╚═════╝ ╚══════╝╚══════╝
```

[![TryHackMe](https://img.shields.io/badge/TryHackMe-UmbraNull-212C42?style=flat-square&logo=tryhackme&logoColor=white)](https://tryhackme.com/p/UmbraNull)
[![HackTheBox](https://img.shields.io/badge/HackTheBox-UmbraNull-9FEF00?style=flat-square&logo=hackthebox&logoColor=black)](https://app.hackthebox.com/profile/019c4c95-6170-73b2-b61c-c5741403d621)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Igor_Leite-0077B5?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/igor-leite-a9b839222)

![Status](https://img.shields.io/badge/Status-Active-success?style=flat-square)
![Focus](https://img.shields.io/badge/Focus-Offensive_Security-red?style=flat-square)
![Target](https://img.shields.io/badge/Target-eJPT_2026-blue?style=flat-square)

</div>

---

## About

Backend developer transitioning into offensive security and Red Team operations. My background in public procurement systems gave me an unusual angle on business logic vulnerabilities — how complex workflows create attack surfaces that purely technical assessments miss.

Currently focused on practical exploitation in controlled environments, Python automation for offensive tasks, and building a portfolio that demonstrates methodology over tooling.

```python
profile = {
    "location":       "Brasília, DF — Brazil",
    "current_role":   "Analyst of Technology & Bids @ Croma Tecnologia",
    "education":      "CST Information Security — UNIP (2025–2027)",
    "certification":  "eJPT (INE Security) — Target: 2026",
    "thm_handle":     "UmbraNull",
}
```

---

## Offensive Security

Practical exploitation documented in controlled lab environments (TryHackMe, HackTheBox). Write-ups focus on attack chain reasoning — not just what worked, but why.

**Techniques applied:**

```
Reconnaissance      →  Nmap, Gobuster, enum4linux, custom Python scripts
Web Exploitation    →  File upload RCE, SQL injection, CMS exploitation
Credential Attacks  →  Hydra, John the Ripper, Hashcat, PCAP analysis
Steganography       →  binwalk (append), steghide (LSB), zip2john
Privilege Escalation →  SUID abuse, cron hijacking, sudo CVEs, PATH manipulation
Active Directory    →  Kerberos enum, AS-REP Roasting, DCSync
```

**Completed rooms:**

| Platform    | Room                 | Key Techniques                                        |
|-------------|----------------------|-------------------------------------------------------|
| TryHackMe   | Agent Sudo           | User-Agent bypass, steganography chain, CVE-2019-14287 |
| TryHackMe   | Startup              | FTP+webshell RCE, PCAP credential extraction, cron PrivEsc |
| TryHackMe   | Break Out The Cage   | Vigenère cipher, Python command injection, cron exploitation |
| TryHackMe   | Brooklyn Nine Nine   | SSH brute-force, SUID /bin/less (GTFOBins)            |
| TryHackMe   | Kenobi               | ProFTPD mod_copy (CVE-2015-3306), NFS, PATH hijacking |
| TryHackMe   | Mr. Robot CTF        | WordPress enumeration, hash cracking, SUID nmap       |
| TryHackMe   | Wonderland           | PATH manipulation, Linux capabilities                 |
| TryHackMe   | Attacktive Directory | AS-REP Roasting, DCSync                               |
| TryHackMe   | Simple CTF           | CMS Made Simple SQLi, VIM GTFOBins                    |
| TryHackMe   | Basic Pentesting     | SMB enumeration, SSH key cracking                     |

→ Full write-ups: [github.com/igorleite97/offensive-writeups](https://github.com/igorleite97/offensive-writeups)

---

## Backend Development

**SGL Enterprise** — Public procurement ERP built security-first.

```
Stack:        Python (FastAPI, asyncio, pytest) + TypeScript (React)
Architecture: DDD + Clean Architecture + Event Sourcing
Security:     JWT/RBAC, input validation, audit trail via event log
Database:     PostgreSQL + SQLAlchemy (async)
```

→ [github.com/igorleite97/sgl_enterprise](https://github.com/igorleite97/sgl_enterprise)

---

## Technical Stack

```bash
# Offensive
Kali Linux · Nmap · Burp Suite · Metasploit · Hydra · John the Ripper
Gobuster · binwalk · steghide · enum4linux · Wireshark

# Development
Python · FastAPI · SQLAlchemy · PostgreSQL · Docker
TypeScript · React · JWT · REST APIs

# Knowledge
OWASP Top 10 · DDD · Event Sourcing · Clean Architecture
```

---

## Learning Path

```
Phase 1 — Foundation         ✅ complete
├─ Basic Pentesting
├─ Kenobi
├─ Brooklyn Nine Nine
├─ Startup
├─ Break Out The Cage
└─ Agent Sudo

Phase 2 — Intermediate        ◉ current
├─ Lazy Admin
├─ Ignite
├─ Bolt
└─ HackPark

Phase 3 — Certification
└─ eJPT (INE Security)  →  Target: 2026

Phase 4 — Advanced
├─ Active Directory deep-dive
├─ Buffer overflow fundamentals
└─ OSCP (planned)
```

---

## Certifications

| Certification                               | Status           |
|---------------------------------------------|------------------|
| eJPT — INE Security                         | In progress      |
| ISO/IEC 27001:2022 Associate — SkillFront   | Completed 2026   |
| Getting Started in Cybersecurity — Fortinet | Completed 2026   |
| CRPO — EU Cyber Academy                     | Completed 2026   |
| OSCP                                        | Planned          |

---

## GitHub Stats

<div align="center">

![GitHub Stats](https://github-readme-stats.vercel.app/api?username=igorleite97&show_icons=true&theme=tokyonight&hide_border=true&bg_color=0D1117&title_color=79c0ff&icon_color=79c0ff&text_color=C9D1D9&count_private=true)

![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=igorleite97&layout=compact&theme=tokyonight&hide_border=true&bg_color=0D1117&title_color=79c0ff&text_color=C9D1D9)

<img src="https://tryhackme-badges.s3.amazonaws.com/UmbraNull.png" alt="TryHackMe Badge" width="280"/>

</div>

---

## Repositories

| Repository | Description |
|------------|-------------|
| [offensive-writeups](https://github.com/igorleite97/offensive-writeups) | Technical write-ups from TryHackMe and HackTheBox |
| [sgl_enterprise](https://github.com/igorleite97/sgl_enterprise) | Public procurement ERP — Python/FastAPI/DDD |

---

<div align="center">

*"Ferramentas ficam obsoletas. Entender os protocolos é o que diferencia quem opera de quem apenas executa."*

</div>
