# 🌿 Serenity — Mental Health Companion

A calm, browser-based mental health companion app that provides mood tracking, guided journaling, breathing exercises, and AI-powered emotional support — all without requiring a backend.

![Serenity App Screenshot](docs/screenshot.png)

---

## ✨ Features

- **Mood Check-in** — Log your current emotional state with one click
- **AI Chat** — Compassionate conversational support powered by a configurable LLM backend
- **Guided Journal** — Write freely with optional AI-driven mood analysis
- **Breathing Exercises** — Interactive 4-7-8 breathing technique with visual guidance
- **Insights Dashboard** — Mood trends and pattern recognition over time
- **Model Configurator** — Plug in any OpenAI-compatible or Ollama endpoint

---

## 🚀 Getting Started

### Option 1: Open Directly

No build step required. Simply open `index.html` in any modern browser:

```bash
open index.html
# or just double-click the file
```

### Option 2: Serve Locally

For the AI features to work properly (due to browser CORS restrictions), serve the file over HTTP:

```bash
# Python
python3 -m http.server 8080

# Node.js (npx)
npx serve .
```

Then visit `http://localhost:8080`.

---

## 🤖 Connecting an AI Model

Serenity supports any OpenAI-compatible API or a local [Ollama](https://ollama.ai) instance.

1. Click the **⚙ Configure** button in the top bar
2. Enter your model endpoint (e.g. `http://localhost:11434/api/generate` for Ollama)
3. Set your model name and API type
4. Click **Connect**

### Supported Backends

| Backend | API Type | Example Endpoint |
|---|---|---|
| Ollama (local) | `ollama` | `http://localhost:11434/api/generate` |
| OpenAI | `openai` | `https://api.openai.com/v1/chat/completions` |
| LM Studio | `openai` | `http://localhost:1234/v1/chat/completions` |
| Any OpenAI-compatible | `openai` | Your custom URL |

> **Privacy note:** When using a local model (Ollama, LM Studio), all data stays on your device.

---

## 🗂 Project Structure

```
serenity-mental-health/
├── index.html          # Main application (self-contained)
├── docs/               # Documentation assets
│   └── screenshot.png
├── .github/
│   └── ISSUE_TEMPLATE/ # Bug report & feature request templates
├── CONTRIBUTING.md     # Contribution guidelines
├── LICENSE             # MIT License
└── README.md
```

---

## 🛡 Mental Health Disclaimer

Serenity is a **wellness tool**, not a medical application. It is not a substitute for professional mental health care.

- In a crisis, please contact a crisis helpline in your country
- **India:** iCall — 9152987821 | Vandrevala Foundation — 1860-2662-345 (24/7)
- **International:** [findahelpline.com](https://findahelpline.com)

---

## 🤝 Contributing

Contributions are welcome! Please read [CONTRIBUTING.md](CONTRIBUTING.md) before opening a PR.

---

## 📄 License

MIT © 2025 — See [LICENSE](LICENSE)
