# 🛡️ CyberShield — Ransomware Detection Dashboard

A **cyberpunk-themed, browser-based ransomware detection dashboard** built as a college project.  
No backend required — runs entirely in the browser using localStorage.

![CyberShield Preview](https://img.shields.io/badge/STATUS-ACTIVE-00ffe7?style=for-the-badge&labelColor=050508)
![HTML](https://img.shields.io/badge/HTML-5-ff1a1a?style=for-the-badge)
![CSS](https://img.shields.io/badge/CSS-3-00ffe7?style=for-the-badge)
![JS](https://img.shields.io/badge/JS-Vanilla-ffe600?style=for-the-badge)

---

## 🚀 Live Demo (GitHub Pages)

👉 **https://kellyyadav.github.io/cybershield/**

---

## ✨ Features

- 🔐 **User Auth** — Register / Login (stored in browser localStorage)
- 📂 **File Scanner** — Drag & drop any file for analysis
- 🧮 **Real Entropy Analysis** — Shannon entropy computed from actual file bytes
- 📊 **Threat Scoring** — 0–100 risk score with detailed reasons
- 📈 **Live Charts** — Score history trend chart (Canvas)
- 🎯 **Threat Gauge** — Animated semicircle risk meter
- 📋 **Detection Log** — Full scan history per user
- 🔔 **Toast Alerts** — Real-time status notifications

---

## 🧠 Detection Engine

| Signal | Weight |
|---|---|
| High entropy (>7.5 bits) | +40 pts |
| Risky extension (.exe/.bat/.vbs) | +30 pts |
| High byte randomness (>85%) | +25 pts |
| Large file size (>1MB) | +10 pts |

**Severity:**
- 🚨 **CRITICAL** — Score ≥ 75
- ⚠️ **SUSPICIOUS** — Score ≥ 45
- ✅ **SAFE** — Score < 45

---

## 📦 Deploy to GitHub Pages (Free Hosting)

### Step 1 — Create Repository
1. Go to [github.com](https://github.com) → **New Repository**
2. Name it `cybershield` (or anything you like)
3. Make it **Public**
4. Click **Create repository**

### Step 2 — Upload the File
```bash
# Option A: Drag & drop index.html in the GitHub UI

# Option B: Via Git
git init
git add index.html README.md
git commit -m "🛡️ Initial deploy — CyberShield Dashboard"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/cybershield.git
git push -u origin main
```

### Step 3 — Enable GitHub Pages
1. Go to repo **Settings** → **Pages**
2. Source: **Deploy from a branch**
3. Branch: `main` → folder: `/ (root)`
4. Click **Save**
5. Wait ~60 seconds → visit `https://YOUR_USERNAME.github.io/cybershield/`

---

## 🗂️ File Structure

```
cybershield/
├── index.html    ← Entire app (single file, no dependencies)
└── README.md
```

---

## 👨‍💻 Tech Stack

| Technology | Usage |
|---|---|
| HTML5 Canvas | Gauge + Chart rendering |
| CSS3 Animations | Cyberpunk UI, scanlines, glows |
| Vanilla JS | Engine + auth + localStorage |
| Google Fonts | Orbitron, Share Tech Mono, Rajdhani |

---

## 📌 Note

> This is a **simulated detection tool** for educational purposes.  
> It uses real entropy analysis but is NOT a replacement for production antivirus software.

---

*Made with ❤️ for college project — by Kellyyadav
