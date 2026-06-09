# Nudge 🔔
### AI that turns meeting transcripts into tracked Notion tasks automatically.

[![Live Demo](https://img.shields.io/badge/Live-Demo-brightgreen)](https://nudge-s5sp.vercel.app)
[![Powered by Groq](https://img.shields.io/badge/Powered%20by-Groq%20LLaMA-blue)](https://groq.com)



## The Problem
Every meeting ends with action items nobody tracks. They live in someone's head, a messy notes doc, or nowhere at all. The next meeting starts with "wait, what were we supposed to do?"

**80% of meeting action items are never completed because nobody tracks them.**

## The Solution
Paste your meeting notes into Nudge. AI reads them, extracts every action item, identifies who owns it, and automatically creates individual tasks in Notion. No manual work. No forgotten follow-ups.


## How It Works

```
Meeting Notes → Tally Form → n8n Webhook → Groq LLaMA AI → Notion Tasks
```

1. **Input** — Paste your meeting transcript into the Nudge form
2. **AI Processing** — Groq LLaMA 3.3 reads the transcript and extracts every action item, owner, and deadline
3. **Auto-create** — n8n automatically creates individual Notion tasks for each action item
4. **Track** — Every task appears in your Notion database, ready to manage

---

## Demo

**Input:**
> "Amelia will build the landing page by Wednesday. John needs to send the investor update by Thursday. Sarah will schedule the demo calls by Friday."

**Output in Notion:**

| Task | Owner | Status |
|------|-------|--------|
| Build the landing page | Amelia | To Do |
| Send investor update | John | To Do |
| Schedule demo calls | Sarah | To Do |

---

## Tech Stack

| Tool | Purpose |
|------|---------|
| **n8n** | Workflow automation engine |
| **Groq LLaMA 3.3 70B** | AI action item extraction |
| **Notion API** | Task database |
| **Tally** | User input form |
| **Vercel** | Frontend deployment |

---

## What I Learned Building This

- Webhook architecture and real-time data triggers
- Calling external AI APIs (Groq) via HTTP Request nodes
- Parsing and transforming JSON data with JavaScript
- Connecting multiple tools into a single automated pipeline
- Deploying a live product accessible from anywhere

---

## Why This Is Different From ChatGPT

ChatGPT can't create Notion tasks. ChatGPT can't run automatically every time you have a meeting. ChatGPT can't send follow-up reminders. Nudge does all of this without any human triggering it.

---

## Built By

**Amelia Ann Pereria** — APM candidate passionate about building AI-powered products that solve real workflow problems.

[LinkedIn](https://linkedin.com/in/ameliaannpereria) · [Live Demo](https://nudge-s5sp.vercel.app)
