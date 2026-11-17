# AI Agents Lab

Ten free, open-source tools that finish a job — a ready-to-send WhatsApp message, a shoot-ready video script, a reply draft, a working WhatsApp automation — and run entirely in your browser.

**Live:** https://satyamkumar-builds.github.io/ai-agents-lab/

No sign-up. No server. The AI tools run on your own API key (BYOK), and that key is stored only in your browser's local storage — requests go straight from your browser to the provider. Two tools need no key at all.

## Why this exists

A general chatbot gives you a conversation. These tools are shaped around one job each — a fixed script format, platform-specific post rules, templates that follow WhatsApp's compliance rules — so the output is finished work you can copy, download and reuse.

## The tools

| # | Tool | What it does | Needs |
|---|------|--------------|-------|
| 1 | [StudyBuddy AI](https://satyamkumar-builds.github.io/ai-agents-lab/study-buddy/) | Explains any topic story-first, with an example, key points and a check question | Your API key |
| 2 | [CodeMentor AI](https://satyamkumar-builds.github.io/ai-agents-lab/code-mentor/) | Line-by-line code explanations, bug hunts with reasons, practice tasks | Your API key |
| 3 | [Salon & Business Assistant](https://satyamkumar-builds.github.io/ai-agents-lab/business-assistant/) | Demo customer-support agent configured with your own services and prices | Your API key |
| 4 | [ScriptWriter AI](https://satyamkumar-builds.github.io/ai-agents-lab/script-writer/) | Short-video scripts: hook, body, on-screen text, CTA — timed to duration | Your API key |
| 5 | [WhatsApp Message Studio](https://satyamkumar-builds.github.io/ai-agents-lab/whatsapp-studio/) | 45 ready business WhatsApp templates in 3 languages, plus optional AI polish | Nothing (key optional) |
| 6 | [FlowStudio](https://satyamkumar-builds.github.io/ai-agents-lab/flow-studio/) | Visual WhatsApp automation builder — trigger → message → delay blocks, run from your browser | Your Meta WhatsApp credentials |
| 7 | [Social Post Generator](https://satyamkumar-builds.github.io/ai-agents-lab/social-post-generator/) | Ready posts for Instagram, LinkedIn and X with platform rules built in | Your API key |
| 8 | [Email Replier](https://satyamkumar-builds.github.io/ai-agents-lab/email-replier/) | Professional reply drafts in five tones, without invented facts or promises | Your API key |
| 9 | [Profile Optimizer](https://satyamkumar-builds.github.io/ai-agents-lab/profile-optimizer/) | LinkedIn/Fiverr headline options and bio rewrites — honest improvements only | Your API key |
| 10 | [Prompt Library](https://satyamkumar-builds.github.io/ai-agents-lab/prompt-library/) | 23 copy-ready prompts for study, coding, exams and interviews | Nothing |

## Quick start

1. Open the [live site](https://satyamkumar-builds.github.io/ai-agents-lab/) — no install, no account.
2. For AI tools, get a free Google Gemini API key from [aistudio.google.com/apikey](https://aistudio.google.com/apikey) and paste it into the tool. OpenRouter and Groq keys also work — switch the provider inside any tool.
3. To run it locally: clone this repo and open `index.html`, or serve the folder with any static server, e.g. `python3 -m http.server`.

## Tech notes

- Plain HTML, CSS and JavaScript. No framework, no backend, and no build step to view or edit the site. (The shared `lab.css` is a precompiled Tailwind stylesheet — the pages link it directly instead of loading a CSS framework from a CDN at runtime.)
- AI requests are made directly from the browser to the provider's API (Gemini `generateContent`, or the OpenAI-compatible endpoints of OpenRouter and Groq). Keys live in `localStorage` under `byok_key_<provider>` and are never sent anywhere else.
- FlowStudio calls Meta's Graph API with credentials the user provides; they stay in the user's browser too. It enforces an opt-in warning and a 20-recipient cap per run.
- Recent outputs and chat history are kept in the visitor's own browser (`localStorage`) — nothing is uploaded or tracked.

## Honest limits

These are small, single-purpose tools, not a platform. FlowStudio runs only while its page is open. AI answer quality depends on the model behind your key.

## Contributing

Improvements are welcome — open an issue or a pull request. Please keep the same principles: no backend, no tracking, no invented claims in copy, and tools that finish a job rather than start a chat.

## Licence

MIT — see [LICENSE](LICENSE). Built by [Satyam Kumar](https://satyamkumar-builds.github.io/animated-portfolio/) (SatyamLabs).
