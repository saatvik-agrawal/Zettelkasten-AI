# *This is currently a WIP repo. Not ready for deployment or use just yet!*

### What is this?

> **Zettelkasten AI** — An Obsidian plugin that respects your note structure, reasons through your links, and helps you build a truly atomic, intelligent Zettelkasten.

---

### Project Summary

> **Zettelkasten AI** is a plugin for Obsidian that enhances your knowledge workflow with GPT-powered link suggestions, atomic note splitting, and intentional note graph building. Unlike existing semantic plugins, Zettelkasten AI doesn't just find similar notes — it explains *why* links make sense based on your vault’s structure and note content. It integrates seamlessly with tools like Smart Connections and Rocketnotes while preserving the manual, mindful nature of Zettelkasten through explainable AI blocks, YAML metadata, and vault-respecting logic.

---

## ❓ Why This Plugin?

While tools like **Smart Connections** and **Rocketnotes** help surface similar notes and enable AI-driven conversations, they often overlook the **core philosophy of Zettelkasten**:

> **Intentional linking, atomic thinking, and transparent reasoning.**

**Zettelkasten AI** is built specifically to support that philosophy. It doesn’t just connect notes — it helps you understand, shape, and evolve your note network intentionally.

### 🧩 What Makes It Different?

- 🔗 **Link Suggestions with Contextual Reasoning**Suggests connections and explains why — using your note content, tags, and existing links.
- 🧠 **GPT-Powered Atomic Note Splitting**Detects multiple ideas and helps split long notes into atomic ones, keeping backlinks intact.
- 🧭 **Vault-Aware Semantics**Respects your existing Obsidian link graph (incoming/outgoing links), tag clusters, and folder structure.
- 📝 **Transparent Metadata Layer**Adds suggested links and rationale as editable `%%AI_LINKS%%` or YAML blocks — you stay in control.
- 🤝 **Interoperable with Smart Connections & Rocketnotes**
  Reuses embeddings, leverages FAISS indexes, or replaces parts with your own pipeline.

---

## 🔧 Roadmap

- [X] Plugin scaffold from Obsidian Sample Plugin
- [X] Integrate OpenAI API for GPT-based tasks
- [X] Add `Suggest Zettelkasten Links` command
- [ ] Add editable `%%AI_LINKS%%` metadata block
- [ ] Add `Split into Atomic Notes` command using GPT
- [ ] Smart Chat: Ask questions with Zettelkasten-style context
- [ ] Use Smart Connections' embeddings if present
- [ ] Fallback to Rocketnotes-style FAISS + SentenceTransformer pipeline
- [ ] Plugin settings tab with model and feature controls
- [ ] Visual summary of note graph updates (link suggestions, splits)

---

## 🎖️ Plugin Highlights (Badge Block)

![Powered by OpenAI](https://img.shields.io/badge/AI-OpenAI-green?logo=openai)
![Zettelkasten Core](https://img.shields.io/badge/Philosophy-Zettelkasten-blueviolet)
![Vault-Aware](https://img.shields.io/badge/Context-Vault%20Links%20%26%20Tags-informational)
![Atomic Notes](https://img.shields.io/badge/Notes-Atomic-yellow)
![Respects Your Links](https://img.shields.io/badge/Manual%20Links-First-priority)
![Obsidian Plugin](https://img.shields.io/badge/Built%20for-Obsidian-black?logo=obsidian)

---

## 🤝 Contributors & Supporters

Zettelkasten AI builds on the amazing work of others in the open-source knowledge management ecosystem:

- 🧠 [Rocketnotes](https://github.com/fynnfluegge/rocketnotes) for modular vector search and RAG workflows
- 🔗 [Smart Connections](https://github.com/brianpetro/obsidian-smart-connections) for semantic note discovery and AI chat
- ⚙️ [Obsidian Sample Plugin](https://github.com/obsidianmd/obsidian-sample-plugin) for the development foundation

### ❤️ Special thanks to:

- The Obsidian community on [Discord](https://discord.gg/obsidianmd) and [GitHub Discussions](https://github.com/obsidianmd/obsidian-api)
- Brian Petro and Fynn Fluegge for making their ideas and architectures open and adaptable
- Everyone exploring the frontier of **intentional AI in personal knowledge**

If you'd like to support the project, feel free to:

- ⭐ Star the repo
- 🗣 Share feedback and ideas
- ☕ [Buy me a coffee](https://buymeacoffee.com/yourpage)





<h1 align="center">🧠 Zettelkasten AI for Obsidian</h1>

<p align="center">
  <strong>An Obsidian plugin that respects your notes, reasons through your links, and helps you build an atomic, intelligent Zettelkasten system.</strong>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/AI-OpenAI-green?logo=openai">
  <img src="https://img.shields.io/badge/Philosophy-Zettelkasten-blueviolet">
  <img src="https://img.shields.io/badge/Context-Vault%20Links%20%26%20Tags-informational">
  <img src="https://img.shields.io/badge/Notes-Atomic-yellow">
  <img src="https://img.shields.io/badge/Manual%20Links-First-priority">
  <img src="https://img.shields.io/badge/Built%20for-Obsidian-black?logo=obsidian">
</p>

---

## 🧭 Overview

Zettelkasten AI enhances your Obsidian vault by helping you think and link more intentionally. It adds GPT-powered tools that suggest meaningful note connections, split large notes into atomic Zettels, and let you chat with your own ideas — all while preserving and leveraging your existing backlinks and structure.

This plugin was created by drawing inspiration from amazing tools like [Smart Connections](https://github.com/brianpetro/obsidian-smart-connections) and [Rocketnotes](https://github.com/fynnfluegge/rocketnotes), but with a sharp focus on the needs of Zettelkasten-style note-taking: atomicity, traceable reasoning, and user control.

---

## 🔍 Features

| Feature                                                | Description                                                                                |
| ------------------------------------------------------ | ------------------------------------------------------------------------------------------ |
| 🔗**Suggest Zettelkasten Links**                 | Finds and suggests new links with explanations based on your vault's content and structure |
| ✂️**Split into Atomic Notes**                  | Uses GPT to split compound notes into clean atomic Zettels with backlinks                  |
| 💬**Chat With Your Vault**                       | Ask questions across your vault using GPT, powered by retrieved relevant notes             |
| 🧠**Intent-Aware Suggestions**                   | Uses your manual links and tags to guide GPT toward meaningful, non-random connections     |
| 📝**Transparent Metadata**                       | AI suggestions are saved in editable `%%AI_LINKS%%` blocks or YAML for full user control |
| 🤝**Integrates Smart Connections & Rocketnotes** | Reuses existing embeddings and tools where available to reduce duplication and cost        |

---

## ✨ Why This Plugin?

While Smart Connections and Rocketnotes offer powerful semantic tooling, Zettelkasten AI is designed for people who want their second brain to be **intentional**, **explainable**, and **structurally coherent**.

- 🧠 **Not just “what’s similar” — but “why should this be linked?”**
- ✍️ **AI doesn't overwrite your thinking — it supports it**
- 🗃 **Makes your link network smarter, not noisier**

---

## 📦 Installation

> Coming soon to the [Obsidian Community Plugins](https://obsidian.md/plugins)

For now, manual install:

```bash
git clone https://github.com/yourusername/obsidian-zk-ai-plugin.git
cd obsidian-zk-ai-plugin
npm install
npm run build
```

Copy the `main.js`, `manifest.json`, and `styles.css` to:

```
.your-vault/.obsidian/plugins/zettelkasten-ai/
```

Then enable the plugin in Obsidian → Settings → Community Plugins.

---

## 🧪 Roadmap

```markdown
- [x] Plugin scaffold with command registration
- [x] Command: Suggest Zettelkasten Links
- [ ] Add editable `%%AI_LINKS%%` block or YAML metadata
- [x] Command: Split into Atomic Notes (stub)
- [ ] GPT-powered splitting with backlink preservation
- [ ] Command: Chat With Vault (RAG-style)
- [ ] Integrate with Smart Connections’ embeddings
- [ ] Fallback to Rocketnotes-style FAISS + chunking
- [ ] Settings tab for OpenAI API keys & customization
- [ ] Visual indicator of proposed vs. accepted links
```

---

## 🙏 Credits & Inspirations

This plugin is made possible by the foundational work of:

- 🧠 [Rocketnotes](https://github.com/fynnfluegge/rocketnotes): For FAISS-based search, markdown chunking, and RAG pipelines
- 🔗 [Smart Connections](https://github.com/brianpetro/obsidian-smart-connections): For embeddings, smart chat, and note-level context awareness
- 🧪 [Obsidian Sample Plugin](https://github.com/obsidianmd/obsidian-sample-plugin): For the starter template and dev tools

Some components are adapted under the MIT license — see code headers for inline attribution.

---

## 💡 Contribute

Contributions are welcome! Whether you're improving the logic, suggesting UI enhancements, or submitting issues — this plugin grows with the community.

```bash
git clone https://github.com/yourusername/obsidian-zk-ai-plugin.git
npm install
npm run dev
```

---

## ☕ Support

If this plugin helps you think better, write more clearly, or reclaim your ideas:

> 💖 [Buy me a coffee](https://buymeacoffee.com/yourpage)

Your support fuels development and lets this stay free, open-source, and made for thinkers.

---

## 📜 License

MIT — do what you want, just give credit.
See [LICENSE](./LICENSE) for details.
