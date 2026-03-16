```
██╗   ██╗███╗   ███╗██████╗ ██████╗  █████╗     ███╗   ██╗██╗   ██╗██╗     ██╗     
██║   ██║████╗ ████║██╔══██╗██╔══██╗██╔══██╗    ████╗  ██║██║   ██║██║     ██║     
██║   ██║██╔████╔██║██████╔╝██████╔╝███████║    ██╔██╗ ██║██║   ██║██║     ██║     
██║   ██║██║╚██╔╝██║██╔══██╗██╔══██╗██╔══██║    ██║╚██╗██║██║   ██║██║     ██║     
╚██████╔╝██║ ╚═╝ ██║██████╔╝██║  ██║██║  ██║    ██║ ╚████║╚██████╔╝███████╗███████╗
 ╚═════╝ ╚═╝     ╚═╝╚═════╝ ╚═╝  ╚═╝╚═╝  ╚═╝    ╚═╝  ╚═══╝ ╚═════╝ ╚══════╝╚══════╝
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
            [ OFFENSIVE SECURITY OPERATOR  |  SYSTEM ARCHITECT ]
       "4e6f7450657479612e5761726e696e673a4578706c6f6974496e50726f6772657373"
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
```

<div align="center">

### `>>> import reality; reality.exploit()`

*In systems we trust. In vulnerabilities we thrive.*

</div>

---

## SIGINT INTERCEPT // CLEARANCE LEVEL: PUBLIC

```python
# Entity Classification: UMBRANULL
# Threat Level: [REDACTED]
# Operational Status: ACTIVE
# Last Known Activity: 14 days continuous engagement
# Primary Objective: Vg6JtB9mK2xQ (ROT13: Flfgrz Pbzcebzvfr)
```

**Who am I?**

A **systems architect** by day, **shadow operator** by night. I don't just write code — I **dissect it, weaponize it, and rebuild it bulletproof**.

My background in **public procurement** (licitações) gave me something most pentesters lack: **understanding of business logic exploits**, compliance loopholes, and how systems **actually** break.

Currently engineering **[SGL Enterprise](https://github.com/igorleite97/sgl_enterprise)** — a procurement ERP fortified with DDD, Event Sourcing, and zero-trust architecture.

**Inspirations from history:**
```
> NotPetya (2017)     → $10B damage. Lesson: Supply chain is everything.
> WannaCry (2017)     → 300K+ infections. Lesson: Patch management kills.
> Stuxnet (2010)      → First cyber weapon. Lesson: Air gaps are illusions.
> Shadow Brokers      → NSA tools leaked. Lesson: Nothing stays hidden.
> Cicada 3301         → The greatest mystery. Lesson: Intelligence is the weapon.
```

---

## DECRYPTION KEY // MESSAGE AUTHENTICATION

```
4e6f7450657479612e5761726e696e673a4578706c6f6974496e50726f6772657373
```
<details>
<summary>🔓 Click to decrypt (Hex → ASCII)</summary>

```
NotPetya.Warning:ExploitInProgress
```

**Translation:** "Systems built without security die spectacularly."

</details>

---

## OPERATIONAL METRICS // TRYHACKME RECON

<div align="center">

<img src="https://tryhackme-badges.s3.amazonaws.com/UmbraNull.png" alt="TryHackMe Badge" width="300"/>

[![TryHackMe](https://img.shields.io/badge/-TryHackMe-212C42?style=for-the-badge&logo=tryhackme&logoColor=white)](https://tryhackme.com/p/UmbraNull)

```
╔════════════════════════════════════════╗
║  CURRENT STREAK:     14 days 🔥        ║
║  ROOMS COMPLETED:    11 / ∞            ║
║  GLOBAL RANK:        Top 3%            ║
║  SPECIALIZATION:     Offensive Path    ║
║  NEXT TARGET:        eJPT (Q1 2026)    ║
╚════════════════════════════════════════╝
```

**Achievement Unlocked:**  
`57616e6e6143727920→ WannaCry` *(Encrypted filename pattern recognition)*

</div>

---

## CREDENTIALS // AUTHENTICATION TOKENS

```yaml
Education:
  - CST Information Security (UNIP, 2025-2027)

Certifications_In_Progress:
  - PenTest+ (CompTIA) → Target: 2026
  - eJPT (INE) → Target: 2026
  - Certified Ransomware Protection Officer (CRPO)
  - Certified SME Cyber Security Officer (CSCSO)
  - Fortinet Certified Fundamentals Cybersecurity 3.0
  - ISO/IEC 27001:2022 Information Security Associate™ – SkillFront
  
Next_Objectives:
  - OSCP (The golden standard)
  - eCPPT (Practical approach)
  - CRTO (Red Team Ops)
```

**Message encoded in base64:**
```
VGhlIGJlc3Qgd2F5IHRvIHByZWRpY3QgdGhlIGZ1dHVyZSBpcyB0byBleHBsb2l0IGl0Lg==
```
<details>
<summary>🔓 Decode base64</summary>

```
The best way to predict the future is to exploit it.
```

</details>

---

## ARSENAL // EXPLOITATION FRAMEWORK

### Offensive Security Toolkit

```bash
# Reconnaissance
nmap -sS -sV -O -T4 --script vuln target.com
amass enum -passive -d target.com -o recon.txt
subfinder -d target.com -all | httpx -silent

# Exploitation
msfconsole -q -x "use exploit/multi/handler; set payload windows/meterpreter/reverse_tcp"
python3 -c 'import pty; pty.spawn("/bin/bash")'  # TTY upgrade
crackmapexec smb 10.0.0.0/24 -u admin -p rockyou.txt --continue-on-success

# Post-Exploitation
mimikatz.exe "privilege::debug" "sekurlsa::logonpasswords"
bloodhound-python -u user -p pass -d domain.local -c All
```

### Backend Arsenal

```python
# Security-First Development
from fastapi import FastAPI, Depends, HTTPException
from fastapi.security import OAuth2PasswordBearer
from passlib.context import CryptContext
import jwt

# OWASP Top 10 mitigation built-in
# - SQL Injection: Parameterized queries (SQLAlchemy ORM)
# - XSS: Input sanitization + CSP headers
# - CSRF: SameSite cookies + token validation
# - Broken Auth: Bcrypt + JWT rotation
# - Security Misconfiguration: Hardened defaults
```

**Stack:**
```
Backend:      Python (FastAPI, asyncio, pytest)
Frontend:     TypeScript (React, Next.js)
Security:     JWT, RBAC, OWASP compliance
Architecture: DDD, Event Sourcing, CQRS
DevOps:       Docker, CI/CD, Zero-trust
```

---

## CLASSIFIED PROJECTS // ACCESS GRANTED

### Project Codename: "PROCUREMENT_SHIELD"

**Repository:** [SGL Enterprise](https://github.com/igorleite97/sgl_enterprise)

**Mission Brief:**  
Secure enterprise procurement system handling **government contracts** (high-value target). Built with security as **foundation**, not afterthought.

**Security Implementations:**
```python
# Event Sourcing = Complete audit trail (NotPetya lesson)
# RBAC = Principle of least privilege (Stuxnet lesson)
# Input validation = No SQLi surface (WannaCry lesson)
# Zero-trust architecture = Trust nothing (Shadow Brokers lesson)
```

**Tech Specs:**
- Python + FastAPI (async performance)
- PostgreSQL + Event Store (immutable logs)
- Domain-Driven Design (business logic isolation)
- Comprehensive test coverage (pytest)

**Why it matters:**  
Public procurement = **in taxpayer money**. Systems this critical **cannot** be insecure.

---

### Project Codename: "BREACH_DOCUMENTATION"

**Repository:** [Offensive Write-ups](https://github.com/igorleite97/offensive-writeups)

Professional-grade penetration testing reports from:
- TryHackMe offensive path
- HackTheBox machines
- Personal security research

**Documented Exploits:**
```
✅ Basic Pentesting  → SMB anonymous, SSH bruteforce, lateral movement
✅ Kenobi           → ProFTPD mod_copy, NFS misconfiguration, SUID exploitation
🔄 Brooklyn Nine Nine → [REDACTED - In Progress]
📋 Lazyadmin        → [QUEUED]
📋 Attacktive Directory → [QUEUED]
```

**Methodology:** PTES framework, OWASP guidelines, professional reporting standards.

---

## PATTERN RECOGNITION // CICADA PROTOCOL

```
4c 6f 6f 6b 20 64 65 65 70 65 72 2e 20 54 68 65 20 
61 6e 73 77 65 72 73 20 61 72 65 20 69 6e 20 74 68 
65 20 63 6f 64 65 2e
```

<details>
<summary>🔓 Decrypt (HEX)</summary>

```
Look deeper. The answers are in the code.
```

**Hidden Message:**  
Those who understand systems **own** them. Those who don't are **owned** by them.

</details>

---

## SURVEILLANCE DATA // GITHUB METRICS

<div align="center">

![UmbraNull's GitHub stats](https://github-readme-stats.vercel.app/api?username=igorleite97&show_icons=true&theme=tokyonight&hide_border=true&bg_color=0D1117&title_color=00FF41&icon_color=00FF41&text_color=C9D1D9&count_private=true)

![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=igorleite97&layout=compact&theme=tokyonight&hide_border=true&bg_color=0D1117&title_color=00FF41&text_color=C9D1D9)

![GitHub Streak](https://github-readme-streak-stats.herokuapp.com/?user=igorleite97&theme=tokyonight&hide_border=true&background=0D1117&ring=00FF41&fire=00FF41&currStreakLabel=00FF41)

</div>

---

## ACTIVE OPERATIONS // Q1 2026 OBJECTIVES

```python
class MissionBriefing:
    def __init__(self):
        self.primary_objective = "eJPT Certification (March 2026)"
        self.secondary_objectives = [
            "Complete TryHackMe Offensive Path (20+ rooms)",
            "SGL Enterprise v2.0 (Microservices migration)",
            "Active Directory attack chain research",
            "Build custom exploit toolkit (Python)"
        ]
        
    def execute(self):
        while not self.mission_complete():
            self.train()
            self.exploit()
            self.document()
            self.repeat()
```

**Current Learning Path:**
```
Phase 1: Foundation
├─ ✅ Basic Pentesting
├─ ✅ Kenobi
└─ 🔄 Brooklyn Nine Nine

Phase 2: Intermediate
├─ 📋 Lazyadmin
├─ 📋 Startup  
└─ 📋 Attacktive Directory

Phase 3: Advanced
└─ 📋 [ENCRYPTED: 53747578 6e6574]  → "Stuxnet"
```

---

## COMMUNICATION CHANNELS // SECURE LINKS

<div align="center">

[![TryHackMe](https://img.shields.io/badge/-TryHackMe-212C42?style=for-the-badge&logo=tryhackme&logoColor=white)](https://tryhackme.com/p/UmbraNull)
[![HackTheBox](https://img.shields.io/badge/-HackTheBox-9FEF00?style=for-the-badge&logo=hackthebox&logoColor=black)](https://app.hackthebox.com/profile/019c4c95-6170-73b2-b61c-c5741403d621)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/igor-leite-a9b839222)
[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:igor_leite_123@hotmail.com)

</div>

```
PGP Key Fingerprint: [REDACTED - Request via secure channel]
Signal: [Available upon verification]
ProtonMail: [Operational security maintained]
```

---

## 💭 OPERATIONAL PHILOSOPHY // CORE PRINCIPLES

```assembly
; Assembly of thought - compiled into action
.section .text
.global _philosophy

_philosophy:
    push    "Offense informs defense"
    push    "Break systems to build unbreakable ones"
    push    "Business logic > Technical exploits"
    push    "Documentation is force multiplication"
    call    execute_mission
    ret
```

### The UmbraNull Doctrine

1. **Learn from history's greatest breaches**  
   NotPetya taught us supply chains fail. WannaCry showed patch management matters. Stuxnet proved air gaps are myths.

2. **Exploit first, patch later**  
   You can't defend what you don't understand. I break systems to learn their true weaknesses.

3. **Code is law, bugs are exploits**  
   Every line of code is a potential vulnerability. Every system has a backdoor — intentional or not.

4. **Anonymity is power**  
   UmbraNull = Shadow + Void. I exist in the null space between detection and compromise.

---

## FINAL TRANSMISSION // CICADA SEQUENCE

```
01010111 01100101 00100000 01100001 01110010 
01100101 00100000 01110100 01101000 01100101 
00100000 01110011 01101000 01100001 01100100 
01101111 01110111 01110011 00100000 01110100 
01101000 01100001 01110100 00100000 01110011 
01111001 01110011 01110100 01100101 01101101 
01110011 00100000 01100011 01100001 01110011 
01110100 00101110
```

<details>
<summary>🔓 Binary Decode</summary>

```
We are the shadows that systems cast.
```

</details>

---

<div align="center">

```
┌───────────────────────────────────────────────────────────────┐
│                                                               │
│  [SYSTEM COMPROMISED]                                         │
│  [ROOT ACCESS GRANTED]                                        │
│  [PERSISTENCE ESTABLISHED]                                    │
│                                                               │
│  "In the void between bits, we find truth.                    │
│   In the null pointer exception, we find freedom.             │
│   In the shadow of every system, we operate."                 │
│                                                               │
│  — UmbraNull                                                  │
│                                                               │
│  Connection Status: ENCRYPTED                                 │
│  Threat Level: MAXIMUM                                        │
│  Next Breach: IMMINENT                                        │
│                                                               │
└───────────────────────────────────────────────────────────────┘
```

### `>>> exit()`

**Encrypted farewell:**  
`VGhlIGdhbWUgaXMgb24uIEZpbmQgbWUgaWYgeW91IGNhbi4=`

<details>
<summary>Final Message (Base64)</summary>

```
The game is on. Find me if you can.
```

</details>

---

⭐ **If you decoded this, you're worth recruiting. Star the repo to signal.**

**Last Transmission:** March 2026  
**Operator Status:** `[ACTIVE]`  
**Next Infiltration:** `[CLASSIFIED]`

</div>

---

## 🔍 EASTER EGGS HIDDEN IN THIS README

Can you find all **7 encrypted messages**?

1. Hex string in banner
2. ROT13 in SIGINT
3. Hex in Decryption Key
4. Base64 after credentials
5. Filename pattern (WannaCry)
6. Hex in Cicada Protocol
7. Binary in Final Transmission
8. **BONUS:** Base64 farewell

**Hint:** `echo "[encrypted_string]" | base64 -d`

**Prize for decoding all:** Nothing. But you proved you belong here.

---

```
     _____           _                
    |  ___|__   ___ | |_ _ __  _ __  
    | |_ / _ \ / _ \| __| '_ \| '_ \ 
    |  _| (_) | (_) | |_| |_) | | | |
    |_|  \___/ \___/ \__| .__/|_| |_|
                        |_|           
    
    Process terminated. Memory wiped.
    No logs. No trace. Only results.
```
