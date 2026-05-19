# 🤝 Contributing to CaseCraft

First off — **thank you for being here!** CaseCraft is a community-driven project and every contribution matters, whether it's adding a case study, fixing a typo, or building a full feature.

This guide will help you get started, no matter your experience level.

---

## 📌 Table of Contents

- [Code of Conduct](#code-of-conduct)
- [Who Can Contribute?](#who-can-contribute)
- [How to Contribute](#how-to-contribute)
- [Setting Up the Project](#setting-up-the-project)
- [Types of Contributions](#types-of-contributions)
- [Submitting a Pull Request](#submitting-a-pull-request)
- [Issue Labels Guide](#issue-labels-guide)
- [GSSoC Guidelines](#gssoc-guidelines)
- [Need Help?](#need-help)

---

## 📜 Code of Conduct

By participating in this project, you agree to be respectful, inclusive, and kind to all contributors. We do not tolerate harassment of any kind.

- Be welcoming to newcomers
- Accept constructive feedback gracefully
- Focus on what's best for the community
- Show empathy toward other contributors

Violations can be reported to the project admin.

---

## 👐 Who Can Contribute?

**Everyone.** Seriously.

- 🟢 **Complete beginners** — You can add case studies by editing a JSON file. No coding needed.
- 🟡 **Intermediate devs** — Pick up UI components, bug fixes, or new pages.
- 🔴 **Advanced devs** — Work on the AI scoring engine, backend APIs, or architecture improvements.

If you're a GSSoC participant, this project is designed with you in mind.

---

## 🛠️ How to Contribute

### Step 1 — Find an Issue

Browse the [Issues tab](https://github.com/divv21/casecraft/issues) and find one that matches your skill level. Look for these labels:

- `good-first-issue` → Perfect if this is your first open source contribution
- `beginner` → Requires basic HTML/CSS/JS knowledge
- `intermediate` → Requires React or Node.js knowledge
- `advanced` → Requires deeper system or AI knowledge
- `documentation` → Writing or improving docs
- `content` → Adding or editing case studies (no coding!)

> ⚠️ **Always comment on an issue before starting work.** This avoids two people working on the same thing. Wait for the admin to assign it to you.

---

### Step 2 — Fork & Clone

```bash
# Fork the repo from GitHub UI, then clone your fork
git clone https://github.com/divv21/casecraft.git
cd casecraft
```

---

### Step 3 — Create a Branch

Always work on a new branch. Never commit directly to `main`.

```bash
# Format: type/short-description
git checkout -b feat/add-spotify-case
git checkout -b fix/scoring-bug
git checkout -b docs/update-readme
```

Branch naming convention:
| Prefix | When to use |
|---|---|
| `feat/` | Adding a new feature |
| `fix/` | Fixing a bug |
| `docs/` | Documentation changes |
| `content/` | Adding case studies |
| `style/` | UI or styling changes |

---

### Step 4 — Set Up the Project Locally

```bash
# Install dependencies
npm install

# Copy environment file and fill in your API keys
cp .env.example .env

# Start the development server
npm run dev
```

The app will run at `http://localhost:3000`

---

### Step 5 — Make Your Changes

- Keep your changes focused — one issue per PR
- Follow the existing code style
- Add comments where the logic isn't obvious
- Test your changes before submitting

---

### Step 6 — Commit Your Changes

Write clear, meaningful commit messages:

```bash
# Good ✅
git commit -m "feat: add Spotify DAU drop case study"
git commit -m "fix: correct scoring for metrics category"
git commit -m "docs: add setup instructions for Windows"

# Bad ❌
git commit -m "changes"
git commit -m "fix stuff"
git commit -m "done"
```

We follow [Conventional Commits](https://www.conventionalcommits.org/) format:
`type: short description`

---

## 📝 Types of Contributions

### 1. Adding a Case Study (No coding needed!)

Case studies live in `/data/cases/` as JSON files. Copy an existing one and fill in your scenario.

```json
{
  "id": "spotify-dau-drop",
  "title": "Spotify DAU Drop",
  "company": "Spotify",
  "category": "metrics",
  "difficulty": "intermediate",
  "prompt": "You are a PM at Spotify. You notice that Daily Active Users dropped by 15% over the past two weeks. Walk me through how you would diagnose and respond to this.",
  "hint": "Consider using a structured diagnostic framework. Start by clarifying the metric, then look at internal vs external causes.",
  "framework_tags": ["metrics", "diagnosis", "root-cause-analysis"],
  "scoring_rubric": {
    "structure": "Does the answer follow a logical diagnostic flow?",
    "metrics": "Does the candidate identify the right metrics to investigate?",
    "user_empathy": "Does the candidate consider the user impact?",
    "action_plan": "Does the candidate propose clear next steps?"
  }
}
```

---

### 2. UI / Frontend Contributions

- Built with **React + Tailwind CSS**
- Components live in `/client/components/`
- Pages live in `/client/pages/`
- Follow existing component structure and naming

---

### 3. Backend Contributions

- Built with **Node.js + Express**
- Routes in `/server/routes/`
- Controllers in `/server/controllers/`
- Always validate inputs and handle errors

---

### 4. Documentation

- Fix typos, unclear instructions, or outdated info
- Add examples where things are confusing
- Translate docs (future goal)

---

## 🔃 Submitting a Pull Request

1. Push your branch to your fork:
```bash
git push origin feat/your-branch-name
```

2. Go to the original CaseCraft repo on GitHub

3. Click **"Compare & pull request"**

4. Fill in the PR template:
   - What does this PR do?
   - Which issue does it close? (e.g. `Closes #12`)
   - Screenshots (if UI change)
   - Any notes for the reviewer?

5. Wait for a review — we'll respond within **2-3 days**

> ✅ Make sure your PR passes all checks before requesting a review.

---

## 🏷️ Issue Labels Guide

| Label | Meaning |
|---|---|
| `good-first-issue` | Great for first-time contributors |
| `beginner` | Basic knowledge needed |
| `intermediate` | Mid-level skill needed |
| `advanced` | Complex task |
| `content` | Case study additions |
| `documentation` | Docs work |
| `bug` | Something is broken |
| `enhancement` | New feature or improvement |
| `help wanted` | Admin needs support |
| `under review` | Being reviewed by admin |
| `duplicate` | Already reported |
| `wontfix` | Will not be worked on |

---

## 🌟 GSSoC Guidelines

If you're contributing as part of **GSSoC 2026**, please read this carefully:

- ✅ Comment on an issue and wait to be **assigned** before starting
- ✅ One active issue per contributor at a time
- ✅ Follow the PR template completely
- ✅ Be responsive if the admin asks for changes
- ❌ Do not open PRs for issues not assigned to you
- ❌ Do not spam issues or PRs
- ❌ Do not copy-paste solutions from the internet without understanding them

**Points are awarded based on PR quality, not just quantity.** A well-thought-out PR is worth more than five rushed ones.

---

## ❓ Need Help?

Stuck? Don't worry — just ask!

- 💬 **Comment on the issue** you're working on
- 📢 **Join our Discord** — 
- 📧 **Email the admin** — divvdev21@gmail.com

We're here to help you succeed, not just merge code.

---

## 🙏 Thank You

Every contribution, big or small — makes CaseCraft better for every PM aspirant out there. We're glad you're here.

Happy contributing! 🚀
