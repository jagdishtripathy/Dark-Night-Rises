<div align="center">

```
██████╗  █████╗ ██████╗ ██╗  ██╗    ███╗   ██╗██╗ ██████╗ ██╗  ██╗████████╗
██╔══██╗██╔══██╗██╔══██╗██║ ██╔╝    ████╗  ██║██║██╔════╝ ██║  ██║╚══██╔══╝
██║  ██║███████║██████╔╝█████╔╝     ██╔██╗ ██║██║██║  ███╗███████║   ██║   
██║  ██║██╔══██║██╔══██╗██╔═██╗     ██║╚██╗██║██║██║   ██║██╔══██║   ██║   
██████╔╝██║  ██║██║  ██║██║  ██╗    ██║ ╚████║██║╚██████╔╝██║  ██║   ██║   
╚═════╝ ╚═╝  ╚═╝╚═╝  ╚═╝╚═╝  ╚═╝   ╚═╝  ╚═══╝╚═╝ ╚═════╝ ╚═╝  ╚═╝   ╚═╝   
                         ██████╗ ██╗███████╗███████╗███████╗
                         ██╔══██╗██║██╔════╝██╔════╝██╔════╝
                         ██████╔╝██║███████╗█████╗  ███████╗
                         ██╔══██╗██║╚════██║██╔══╝  ╚════██║
                         ██║  ██║██║███████║███████╗███████║
                         ╚═╝  ╚═╝╚═╝╚══════╝╚══════╝╚══════╝
```

# 🌑 DARK NIGHT RISES CTF

### A fully-featured, browser-based Capture The Flag hacking platform

**Created by SOM** · 12 Challenges · 2375 Points · Zero Dependencies · Pure HTML/CSS/JS

---

![Challenges](https://img.shields.io/badge/Challenges-12-00ffe7?style=for-the-badge&logo=target&logoColor=black)
![Points](https://img.shields.io/badge/Total%20Points-2375-ff003c?style=for-the-badge)
![No Server](https://img.shields.io/badge/Server-Not%20Required-00ff41?style=for-the-badge&logo=html5&logoColor=black)
![License](https://img.shields.io/badge/License-MIT-ffb800?style=for-the-badge)
![Made With](https://img.shields.io/badge/Made%20With-HTML%20%2F%20CSS%20%2F%20JS-0d1520?style=for-the-badge)

</div>

---

## 🎯 What is this?

**Dark Night Rises** is a self-contained, educational Capture The Flag (CTF) cybersecurity platform. No backend, no database, no installation — just open a browser and hack.

It simulates **12 real-world web vulnerabilities** in a safe, legal, sandboxed environment. Each challenge teaches one exploitation technique, from beginner reconnaissance to advanced cryptographic attacks.

> ⚠️ **All vulnerabilities are simulated in-browser. This platform does not attack any real server.**

---

## 🚀 Quick Start

### Option 1 — Python (Recommended)
```bash
git clone https://github.com/YOUR-USERNAME/dark-night-rises-ctf.git
cd dark-night-rises-ctf
python3 -m http.server 8080
```
Open → **http://localhost:8080**

### Option 2 — Node.js
```bash
git clone https://github.com/YOUR-USERNAME/dark-night-rises-ctf.git
npx serve dark-night-rises-ctf -p 8080
```

### Option 3 — PHP
```bash
cd dark-night-rises-ctf
php -S localhost:8080
```

### Option 4 — Just open it
Double-click `index.html` — most challenges work directly from the filesystem too.

---

## 🗂️ Repository Structure

```
dark-night-rises-ctf/
│
├── index.html              ← Main landing page
├── login.html              ← Login page (contains Level 01 & 02 flags)
├── challenges.html         ← Challenge browser with filters
├── scoreboard.html         ← Live leaderboard with countdown timer
├── rules.html              ← Rules, scoring table, allowed tools
│
└── challenges/
    ├── level1.html         ← Hidden in Source Code       [Easy   · 50pts]
    ├── level2.html         ← Cookie Monster              [Easy   · 75pts]
    ├── level3.html         ← Robots.txt Exposed          [Easy   · 50pts]
    ├── level4.html         ← Base64 Maze                 [Easy   · 75pts]
    ├── level5.html         ← SQL Injection               [Medium · 150pts]
    ├── level6.html         ← XSS Injection               [Medium · 150pts]
    ├── level7.html         ← Directory Traversal         [Medium · 175pts]
    ├── level8.html         ← JWT Forgery                 [Medium · 200pts]
    ├── level9.html         ← Broken Auth Chain           [Hard   · 300pts]
    ├── level10.html        ← SSRF Attack                 [Hard   · 300pts]
    ├── level11.html        ← IDOR Escalation             [Hard   · 350pts]
    └── level12.html        ← The Final Cipher            [Hard   · 500pts]
```

---

## 🧩 Challenge Overview

| # | Challenge | Difficulty | Points | Technique |
|---|-----------|:----------:|:------:|-----------|
| 01 | Hidden in Source Code | 🟢 Easy | 50 | HTML comment inspection |
| 02 | Cookie Monster | 🟢 Easy | 75 | Browser cookie manipulation |
| 03 | Robots.txt Exposed | 🟢 Easy | 50 | Robots.txt recon |
| 04 | Base64 Maze | 🟢 Easy | 75 | Multi-layer Base64 decoding |
| 05 | SQL Injection | 🟡 Medium | 150 | Classic SQLi login bypass |
| 06 | XSS Injection | 🟡 Medium | 150 | DOM-based Cross-Site Scripting |
| 07 | Directory Traversal | 🟡 Medium | 175 | Path traversal (`../`) |
| 08 | JWT Forgery | 🟡 Medium | 200 | JWT `alg:none` bypass |
| 09 | Broken Auth Chain | 🔴 Hard | 300 | Multi-step auth logic flaw |
| 10 | SSRF Attack | 🔴 Hard | 300 | Server-Side Request Forgery |
| 11 | IDOR Escalation | 🔴 Hard | 350 | Insecure Direct Object Reference |
| 12 | The Final Cipher | 🔴 Hard | 500 | AES-ECB pattern exploitation |
| | **TOTAL** | | **2375** | |

---

## 🖥️ Platform Features

- **Matrix rain** background with animated canvas
- **12 interactive challenge pages** — each fully self-contained
- **Simulated terminals**, query panels, network logs, and API explorers
- **Flag submission with success overlays** on every challenge
- **Live scoreboard** with countdown timer and podium display
- **Challenge filter** by difficulty and category
- **Zero backend** — everything runs in the browser
- **Dark hacker aesthetic** — Orbitron + Share Tech Mono fonts, cyan/red/amber palette

---

## 🛡️ Vulnerability Categories Covered

```
Recon          →  HTML source inspection, robots.txt enumeration
Encoding       →  Base64 (encoding ≠ encryption)
Injection      →  SQL Injection, XSS (DOM-based)
Path Security  →  Directory / Path Traversal
Authentication →  Cookie auth, JWT algorithm confusion, broken auth chains
Access Control →  IDOR (Insecure Direct Object Reference)
Server-Side    →  SSRF (Server-Side Request Forgery)
Cryptography   →  AES-ECB block pattern analysis
```

---

## 📋 Rules Summary

- Flags follow the format: `FLAG{...}`
- Attack only the challenge pages — not external systems
- Do not share flags with other participants
- Tools like Burp Suite, browser DevTools, and CyberChef are allowed
- Maximum total score: **2375 points**

Full rules: [`rules.html`](rules.html)

---

## 🏆 Scoring

| Difficulty | Challenges | Points Each | Total |
|:----------:|:----------:|:-----------:|:-----:|
| 🟢 Easy | 4 | 50–75 | 250 |
| 🟡 Medium | 4 | 150–200 | 675 |
| 🔴 Hard | 4 | 300–500 | 1450 |
| | **12** | | **2375** |

---

## 🔧 Customisation

Want to fork and modify this for your own event?

1. **Change flags** — search for `FLAG{` in each challenge file and replace with your own values
2. **Change branding** — update `DARK NIGHT RISES` and `SOM` references in HTML/CSS
3. **Add challenges** — follow the existing page structure (header → panel → flag-submit pattern)
4. **Timer** — update the countdown initial value in `scoreboard.html`
5. **Leaderboard** — edit the `players` array in `scoreboard.html` with real participant data

---

## 📚 Learning Resources

Each challenge teaches a real OWASP vulnerability class. To learn more:

- [OWASP Top 10](https://owasp.org/www-project-top-ten/)
- [PortSwigger Web Security Academy](https://portswigger.net/web-security) — free labs
- [CyberChef](https://gchq.github.io/CyberChef/) — encoding/decoding tool
- [HackTheBox](https://www.hackthebox.com/) — advanced CTF practice
- [TryHackMe](https://tryhackme.com/) — beginner-friendly rooms

---

## ⚠️ Disclaimer

This platform is for **educational purposes only**. All vulnerabilities are simulated entirely in the browser. No real servers, databases, or networks are attacked. Use the techniques you learn here only on systems you own or have explicit permission to test.

---

## 📄 License

MIT License — free to use, fork, and modify. See [`LICENSE`](LICENSE) for details.

---

<div align="center">

**Built with ❤️ and lots of `FLAG{...}` by SOM**

*Dark Night Rises · CTF Platform · Educational Use Only*

⭐ Star this repo if it helped you learn!

</div>
