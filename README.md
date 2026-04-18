# 🔥 RoastMyCode

> Paste your code. Get destroyed. Actually fix it.

An AI-powered code roaster that judges your code like a savage stand-up comedian — then gives you **real, actionable fixes**.

**Built at v0 India IRL Hackathon 🇮🇳**

---

## 🚀 Live Demo

**[roastmycode-two.vercel.app](https://roastmycode-two.vercel.app)**

---

## ✨ Features

| Feature | Description |
|---|---|
| 🎤 **Comedian Roast** | Brutal, hilarious roast of your code in stand-up comedian style |
| 🐛 **Issue Detection** | Identifies bugs, anti-patterns, and bad practices with severity levels |
| 🔧 **Concrete Fixes** | Actionable suggestions + improved code snippets, not just criticism |
| 💀 **Hall of Shame** | Live global leaderboard — lowest score = most shameful code |
| 🎴 **Shareable Roast Cards** | Generate and share your roast with a custom card |
| 📊 **Code Score** | Get a score out of 100 (lower = worse, obviously) |
| 🏷️ **Verdict Tags** | Instant labels like `DUMPSTER FIRE`, `CRIME SCENE`, `HELP ME` |

---

## 💻 Supported Languages

Python · JavaScript · TypeScript · Java · C++ · Go · Rust · Ruby · PHP · C#

---

## 🛠️ Stack

- **Vanilla React 18** via CDN — zero build step, zero dependencies to install
- **Anthropic Claude API** — for the actual roasting and fix generation
- **Firebase Firestore** — real-time Hall of Shame leaderboard
- **Vercel** — instant deployment
- **Single `index.html`** — deploys anywhere in seconds

---

## ⚡ Quick Deploy

### 1. Clone & configure

```bash
git clone https://github.com/YOUR_USERNAME/roastmycode.git
cd roastmycode
```

Open `index.html` and fill in your credentials:

```js
// Firebase config (for leaderboard)
const firebaseConfig = {
  apiKey: "YOUR_API_KEY",
  authDomain: "YOUR_PROJECT.firebaseapp.com",
  projectId: "YOUR_PROJECT_ID",
  ...
};
```

The Anthropic API key is handled via a proxy — no key exposed on the frontend.

### 2. Deploy to Vercel

```bash
# Install Vercel CLI (if not already)
npm i -g vercel

vercel
```

Or just push to GitHub and connect the repo on [vercel.com](https://vercel.com) — the `vercel.json` handles all routing automatically.

---

## 📁 Project Structure

```
roastmycode/
├── index.html      # Entire app — React + styles + logic
├── vercel.json     # SPA routing config for Vercel
└── README.md
```

---

## 🔧 Local Development

No build step needed. Just open `index.html` in a browser, or serve it with any static server:

```bash
npx serve .
# or
python -m http.server 3000
```

---

## 🏆 Hall of Shame

The leaderboard is **live and global** — powered by Firebase Firestore. Every roast you submit (with a nickname) gets ranked. The lower your score, the higher your shame. Compete with devs worldwide to write the worst code.

---

## 📸 Screenshots

| Roast It | Hall of Shame |
|---|---|
| ![Roast Tab](screenshots/roast.png) | ![Hall of Shame](screenshots/shame.png) |

---

## 🤝 Contributing

PRs welcome! Some ideas:
- Add more languages
- Dark/light theme toggle
- Roast history (local storage)
- Export roast as image

---

## 📄 License

MIT — roast freely.
