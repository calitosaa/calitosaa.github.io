# calitossaa.github.io # 🧠 URBALUX — Unified AI Workspace for Developers

> A browser-native, single-file AI workspace that consolidates multiple AI capabilities into one interface — no backend, no build step, no lock-in.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![GitHub Stars](https://img.shields.io/github/stars/calitosaa/urbalux?style=social)](https://github.com/calitosaa/urbalux)
[![Live Demo](https://img.shields.io/badge/demo-live-brightgreen)](https://calitosaa.github.io/urbalux)

---

## ✨ What is URBALUX?

URBALUX is an open-source, **zero-backend AI workspace** that runs entirely in the browser. It gives developers, researchers, and power users a single interface to interact with multiple AI APIs — Anthropic Claude, Google Gemini, and image generation via Pollinations.ai — without installing anything, spinning up a server, or managing infrastructure.

Think of it as your personal Notion + NotebookLM + ChatGPT — but open source, self-hostable, and built for developers who want full control.

---

## 🚀 Features

### 🗒️ Notebook Studio (NotebookLM-inspired)
- Upload PDFs, images, audio, and URLs as sources
- AI-generated Audio Overviews with "join conversation" mode
- Slide Deck generation, Table of Contents, Custom Personas
- Multilingual output support
- 13 Studio tools including Video Overview and Image Analysis

### 💬 Multimodal Chat
- Three modes: **Chat Normal**, **Chat Código** (code-focused), **Generar Imágenes**
- Full file support: images, PDFs, videos, audio, URLs
- Image generation via Pollinations.ai / Flux
- Streaming responses with real-time rendering

### 🔍 SurfSense Engine (Client-side RAG)
- BM25 ranking algorithm — entirely in the browser
- PDF extraction, Wikipedia integration, CORS-proxied URL fetching
- Streaming AI responses with source citations
- localStorage persistence — no database needed

### 🤖 Automation & Agents *(in progress)*
- Visual workflow builder
- Multi-step AI pipelines

---

## 🏗️ Architecture

URBALUX is built on a **browser-native, single-file architecture**:

```
urbalux/
├── index.html          # Main entry point
├── notebook/           # NotebookLM replica module
├── chat/               # Multimodal chat interface
├── surfsense/          # Client-side RAG engine
├── automation/         # Agent workflow builder
└── assets/             # Shared styles and utilities
```

**Philosophy:**
- ✅ Zero backend — all API calls made directly from the browser
- ✅ CDN-only dependencies — no npm, no build tools required
- ✅ Single-file modules — fork any section independently
- ✅ API-key-in-browser pattern — ideal for personal use and prototyping

---

## 🌍 Why This Matters

URBALUX was built specifically to **lower the barrier for Spanish-speaking and Latin American developers** to build with AI APIs. The documentation, UI, and community are maintained in both Spanish and English.

There are thousands of developers in LATAM who want to build AI-powered tools but are blocked by:
- Complex backend requirements
- English-only documentation
- Expensive infrastructure

URBALUX removes all three barriers.

---

## ⚡ Quick Start

No installation required. Just open the HTML file in your browser.

```bash
# Clone the repo
git clone https://github.com/calitosaa/urbalux.git
cd urbalux

# Open in browser (no server needed for most features)
open index.html

# Or serve locally for full API functionality
npx serve .
```

Then add your API keys in the settings panel inside the app.

---

## 🔑 API Keys Required

| Feature | API Key |
|--------|---------|
| Claude Chat & Notebook | `ANTHROPIC_API_KEY` |
| Gemini features | `GOOGLE_AI_KEY` |
| Image generation | None (Pollinations.ai is free) |

Keys are stored in `localStorage` — they never leave your browser.

---

## 🗺️ Roadmap

- [x] NotebookLM replica (13 Studio tools)
- [x] Multimodal chat (3 modes)
- [x] SurfSense Engine (client-side RAG)
- [ ] Automation / Agent builder
- [ ] Programming section (code sandbox)
- [ ] Design tools section
- [ ] Media Creation (audio/video gen)
- [ ] Community section
- [ ] Firebase backend option for data persistence
- [ ] PWA support

---

## 🤝 Contributing

Contributions welcome! URBALUX is especially looking for:
- Spanish/English documentation improvements
- New AI provider integrations
- UI/UX improvements
- Additional RAG strategies for SurfSense

```bash
# Fork → Clone → Branch → PR
git checkout -b feature/your-feature
git commit -m "Add: your feature description"
git push origin feature/your-feature
```

---

## 📄 License

MIT — free to use, fork, and build on.

---

## 👤 Author

**Carlos** ([@calitosaa](https://github.com/calitosaa))  
Building open-source AI tools for the Spanish-speaking developer community.

---

*If URBALUX saved you time, consider giving it a ⭐ — it helps more developers find it.*
