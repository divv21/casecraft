# 🧠 CaseCraft — PM Case Study Simulator

> Practice real product management case studies, get AI-powered feedback, and track your growth — all in one open-source tool built for PM aspirants.

---

## 🚀 What is CaseCraft?

Preparing for PM interviews is hard. Most resources give you frameworks to memorize but no way to **practice applying them** to real scenarios and get feedback.

**CaseCraft** fixes that.

It gives you realistic product scenarios (just like real PM interviews), lets you write your answer, and uses AI to evaluate your response on structure, user empathy, metrics thinking, and more. Then it tracks your progress over time so you can see yourself improving.

Think of it as your **personal PM interview coach** — open source and free, forever.

---

## ✨ Features

- 🎯 **Curated Case Library** — Real-world PM scenarios across categories (Metrics, Product Design, Strategy, Estimation)
- 🤖 **AI Feedback Engine** — Get scored on PM frameworks: CIRCLES, HEART, RICE, and more
- 📈 **Progress Tracker** — See your scores improve over time with visual dashboards
- 🏷️ **Difficulty Levels** — Beginner → Intermediate → Advanced
- 🌐 **Company Filters** — Practice cases inspired by Google, Meta, Amazon, Spotify, and more
- 📝 **Framework Hints** — Optional hints so beginners aren't left stuck
- 🧩 **Contributor-Friendly** — Add new cases, improve scoring rubrics, build new features

---

## 🖼️ Screenshots

> Coming soon — contributions welcome!

---

## 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| Frontend | React + Tailwind CSS |
| Backend | Node.js + Express |
| Database | PostgreSQL |
| AI | OpenAI API / Gemini API |
| Auth | Clerk / Firebase Auth |
| Hosting | Vercel (frontend) + Render (backend) |

---

## 📁 Project Structure

```
casecraft/
├── client/          # React frontend
│   ├── components/
│   ├── pages/
│   └── utils/
├── server/          # Node.js backend
│   ├── routes/
│   ├── controllers/
│   └── models/
├── data/            # Case study JSON files
│   ├── metrics/
│   ├── design/
│   ├── strategy/
│   └── estimation/
└── docs/            # Documentation
```

---

## 🏁 Getting Started

### Prerequisites
- Node.js v18+
- PostgreSQL
- An OpenAI or Gemini API key

### Installation

```bash
# Clone the repo
git clone https://github.com/divv21/casecraft.git
cd casecraft

# Install dependencies
npm install

# Set up environment variables
cp .env.example .env
# Add your API keys to .env

# Run the development server
npm run dev
```

**Read the full guide → [CONTRIBUTING.md](CONTRIBUTING.md)**

---

## 📋 Roadmap

### v0.1 — MVP
- [ ] Case library with 20+ scenarios
- [ ] Text input + AI feedback
- [ ] Basic scoring (structure, metrics, user empathy)

### v0.2 — Progress Tracking
- [ ] User accounts
- [ ] Score history + charts
- [ ] Streaks and practice reminders

### v0.3 — Community
- [ ] Leaderboard
- [ ] Peer feedback
- [ ] Community-submitted cases

---

## 🧑‍💼 For PM Aspirants

CaseCraft covers all major PM interview question types:

| Category | Example Prompt |
|---|---|
| **Metrics** | "Spotify's daily active users dropped 15%. Walk me through your diagnosis." |
| **Product Design** | "Design a feature for Google Maps for blind users." |
| **Strategy** | "Should Amazon enter the grocery delivery market in India?" |
| **Estimation** | "How many Uber rides happen in Mumbai on a weekday?" |
| **Improvement** | "How would you improve Instagram Reels?" |

---

## 📜 License

MIT License — free to use, modify, and distribute.

---

## 📬 Contact

**Project Admin:** Divija (https://github.com/divv21)  
**Email:** divvdev21@email.com  
**Discord:** 

> ⭐ If you find this useful, please star the repo — it helps more contributors find the project!
