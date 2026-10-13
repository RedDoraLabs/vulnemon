# 🦊 Vulnemon

**Learn Cybersecurity Like a Game.**

Vulnemon is an open-source, gamified cybersecurity training platform where you learn ethical hacking through browser-based vulnerability labs. Progress from absolute beginner to advanced security professional — level by level.

> Think **Duolingo meets TryHackMe** — but open-source and built for the Indian market.

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Status](https://img.shields.io/badge/status-active%20development-orange.svg)
![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)

---

## 🎯 What is Vulnemon?

Most cybersecurity training platforms are:
- ❌ Expensive (₹50,000+ per year)
- ❌ Theory-heavy and boring
- ❌ No structured progression path
- ❌ Not beginner-friendly

Vulnemon fixes all of this:
- ✅ **Free & Open Source** — learn without burning your wallet
- ✅ **Gamified** — XP, levels, badges, leaderboard
- ✅ **Hands-On Labs** — real vulnerable environments in your browser
- ✅ **Level-Based Progression** — start from zero, go all the way
- ✅ **AI-Powered Hints** — adaptive guidance based on your skill level

---

## 🏗️ Architecture

```
┌─────────────────────────────────────────────┐
│                   Frontend                   │
│            Next.js + React + Tailwind        │
├─────────────────────────────────────────────┤
│                   Backend                    │
│          Node.js + Express + REST API        │
├─────────────────────────────────────────────┤
│              Lab Engine                      │
│     Docker containers per user session       │
│     Isolated vulnerable environments         │
├─────────────────────────────────────────────┤
│              Database                        │
│         PostgreSQL + Redis (cache)           │
├─────────────────────────────────────────────┤
│           AI Hint Engine                     │
│     LLM-powered adaptive guidance            │
└─────────────────────────────────────────────┘
```

---

## 🧪 Lab Categories

| Category | Description | Labs |
|----------|-------------|------|
| 🌐 **Web Security** | OWASP Top 10 — SQLi, XSS, SSRF, IDOR, Auth Bypass | 30+ |
| 🔑 **Cryptography** | Classical ciphers, RSA, AES, hash cracking, JWT attacks | 15+ |
| 🔍 **OSINT** | Google dorking, metadata analysis, social media recon | 15+ |
| 🔬 **Digital Forensics** | Disk analysis, memory forensics, network pcap analysis | 15+ |
| ⚙️ **Reverse Engineering** | Binary analysis, disassembly, malware basics | 10+ |
| 🛡️ **Blue Team** | SOC operations, log analysis, incident response | 15+ |

---

## 🎮 Gamification System

```
Level 1-10:    Beginner      →  Basic concepts, simple labs
Level 11-25:   Intermediate  →  OWASP Top 10, real-world scenarios
Level 26-40:   Advanced      →  Chained exploits, complex attacks
Level 41-50:   Expert        →  CTF-style challenges, zero-day research
```

- 🏆 **XP Points** — Earn XP for every lab completed
- 🎖️ **Badges** — Unlock badges for milestones (First Blood, 10-Streak, Speed Run)
- 📊 **Leaderboard** — Compete with the community
- 🔥 **Streaks** — Daily streak tracking for consistency

---

## 🚀 Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) v20+
- [Docker](https://www.docker.com/) & Docker Compose
- [PostgreSQL](https://www.postgresql.org/) 15+
- [Git](https://git-scm.com/)

### Installation

```bash
# Clone the repository
git clone https://github.com/RedDoraLabs/vulnemon.git
cd vulnemon

# Install dependencies
npm install

# Set up environment variables
cp .env.example .env
# Edit .env with your database credentials

# Start the development server
npm run dev

# Start lab containers (requires Docker)
docker-compose up -d
```

Open [http://localhost:3000](http://localhost:3000) in your browser.

---

## 📁 Project Structure

```
vulnemon/
├── src/
│   ├── app/              # Next.js pages and routes
│   ├── components/       # Reusable React components
│   ├── lib/              # Utility functions and helpers
│   ├── api/              # Backend API routes
│   └── styles/           # Global styles
├── labs/
│   ├── web/              # Web security lab configs
│   ├── crypto/           # Cryptography challenges
│   ├── osint/            # OSINT challenges
│   ├── forensics/        # Forensics lab configs
│   ├── reversing/        # Reverse engineering labs
│   └── blueteam/         # Blue team scenarios
├── docker/
│   ├── labs/             # Dockerfiles for each lab
│   └── docker-compose.yml
├── docs/
│   ├── CONTRIBUTING.md
│   ├── LAB_CREATION.md
│   └── API.md
├── .env.example
├── package.json
├── LICENSE
└── README.md
```

---

## 🤝 Contributing

We welcome contributions from everyone! Here's how you can help:

### 🧪 Create Labs
The easiest way to contribute — design new vulnerability labs. See [LAB_CREATION.md](docs/LAB_CREATION.md) for the guide.

### 💻 Frontend Development
Help build the dashboard, lab interfaces, leaderboard, and user profiles. We use **Next.js, React, and Tailwind CSS**.

### 🐳 Docker Lab Environments
Build isolated Docker containers for new lab categories.

### 🎨 UI/UX Design
Help improve the user experience and visual design.

### 📝 Documentation
Improve docs, write tutorials, or create lab walkthroughs.

### How to Contribute

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-lab`)
3. Commit your changes (`git commit -m 'Add: SQL Injection Level 5 lab'`)
4. Push to the branch (`git push origin feature/amazing-lab`)
5. Open a Pull Request

Please read our [Contributing Guide](docs/CONTRIBUTING.md) before submitting.

---

## 🗺️ Roadmap

- [x] Project architecture and design
- [x] Lab challenge framework
- [ ] User authentication and profiles
- [ ] First 20 web security labs
- [ ] XP and leveling system
- [ ] Leaderboard
- [ ] AI-powered hint engine
- [ ] Browser-based terminal (no local setup)
- [ ] Mobile responsive design
- [ ] Community lab submissions
- [ ] API for third-party integrations

---

## 🛡️ Security

Found a security vulnerability in Vulnemon itself? Please report it responsibly:

- Email: prem@reddoralabs.com
- Do NOT open a public issue for security vulnerabilities

---

## 📄 License

This project is licensed under the MIT License — see the [LICENSE](LICENSE) file for details.

---

## 🦊 About RedDoraLabs

**Reddora Labs Private Limited** is an offensive security and AI company building tools and platforms to make cybersecurity accessible to everyone.

- 🌐 [reddoralabs.com](https://reddoralabs.com)
- 💼 [LinkedIn](https://linkedin.com/company/reddoralabs)
- 📸 [Instagram](https://instagram.com/reddoralabs)
- 🐙 [GitHub](https://github.com/RedDoraLabs)

---

<p align="center">
  <strong>Built with ❤️ by <a href="https://reddoralabs.com">RedDoraLabs</a></strong><br/>
  <em>Making cybersecurity education accessible, gamified, and fun.</em>
</p>
