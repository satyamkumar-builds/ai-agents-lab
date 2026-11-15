# SatyamLabs AI Agents Lab

8 free AI agents and automations that run on **your own API key** (BYOK — Bring Your Own Key).

**Live site:** https://satyamkumar-builds.github.io/ai-agents-lab/

No sign-up. No backend. No server stores your key — every tool runs fully in your browser, and your key is saved only in your own browser's localStorage.

## The tools

### AI Agents (chat, with conversation memory)

| Tool | What it does | Live |
|---|---|---|
| StudyBuddy AI | Explains any topic simply — story first, then example — in Hindi / Hinglish / English, for students | [study-buddy](https://satyamkumar-builds.github.io/ai-agents-lab/study-buddy/) |
| CodeMentor AI | Explains code line by line, finds bugs, teaches the fix instead of just dumping a solution | [code-mentor](https://satyamkumar-builds.github.io/ai-agents-lab/code-mentor/) |
| Salon & Business Assistant | Demo customer-support agent for a small business — answers customer questions, suggests bookings; business name and services are editable | [business-assistant](https://satyamkumar-builds.github.io/ai-agents-lab/business-assistant/) |
| ScriptWriter AI | Writes short-form video scripts (hook, body, CTA) in Hindi / Hinglish / English from a topic | [script-writer](https://satyamkumar-builds.github.io/ai-agents-lab/script-writer/) |

### Automations (form → one-click output)

| Tool | What it does | Live |
|---|---|---|
| WhatsApp Message Studio | 3 ready-to-send business WhatsApp message variants + a wa.me link. Works template-only without a key; AI polish if you add one | [whatsapp-studio](https://satyamkumar-builds.github.io/ai-agents-lab/whatsapp-studio/) |
| Social Post Generator | Caption + hashtags + best-posting-time tip for Instagram / LinkedIn / X | [social-post-generator](https://satyamkumar-builds.github.io/ai-agents-lab/social-post-generator/) |
| Email Replier | Paste an incoming email, pick a tone, get a professional reply draft | [email-replier](https://satyamkumar-builds.github.io/ai-agents-lab/email-replier/) |
| Profile Optimizer | Paste a LinkedIn / Fiverr bio, get improved versions + headline options | [profile-optimizer](https://satyamkumar-builds.github.io/ai-agents-lab/profile-optimizer/) |

## Get a free API key (1 minute)

1. Go to [aistudio.google.com/apikey](https://aistudio.google.com/apikey) and sign in with Google.
2. Click **Create API key** and copy it.
3. Open any tool above, paste the key in the key box, and start.

OpenRouter and Groq keys also work — switch the provider inside any tool and (if you want) change the model name.

## How BYOK works here

- The key is stored **only in your browser** (localStorage), separately per provider.
- Requests go **directly from your browser** to the provider API (Google / OpenRouter / Groq). This site has no backend and never sees your key.
- You can delete the key any time by clearing it in the tool and pressing Save, or by clearing site data in your browser.

## Tech

Plain HTML + vanilla JavaScript + Tailwind CDN. No build step, no framework, hosted on GitHub Pages. Each tool is a single self-contained `index.html` — view source and copy the pattern freely.

## Author

Built by **Satyam Kumar** — founder of Line Free India, building SatyamLabs.
GitHub: [@satyamkumar-builds](https://github.com/satyamkumar-builds)

These tools are live demos for the **AI Agents & Automation** division of his portfolio. They are honest working demos — no fake users, no fake ratings.
