<div align="center">

# Hi, I'm phenomenoner 👋

**Taiwan Quant Trading · Agent Infrastructure · Software Engineering**

I used to build trading systems. These days I work on agent runtimes, memory and coordination tools, and Codex workflows.

📍 Taipei · 25°N, 121°E

[繁體中文](./README.md) · [English](./README.en.md) · [Website](https://phenomenoner.github.io) · [Email](mailto:phenomenoner@gmail.com)

</div>

---

## What I work on

I started with quantitative and algorithmic trading in Taiwan equities. A backtest can look great while the live system still fails in very ordinary ways. Every action needs a record, authority has to stay narrow, market-data or broker outages must not trigger bad decisions, and failures need to be replayable.

Those habits carried over when I moved into AI agents. I care less about how clever a demo looks than whether the system remains understandable after it has been running for a while, stops when a boundary breaks, and recovers cleanly after a restart. If deterministic code can handle something reliably, I do not ask a model to guess.

> **If software should enforce it, make the rule explicit. If a human should decide it, do not quietly automate it.**

## 🧭 Projects

### Agent runtimes and developer tooling

- [**agent-harness-core**](https://github.com/phenomenoner/agent-harness-core) — The parts around a model that rarely make a good demo but tend to cause trouble in production: ingress, authority, queues, delivery, audit, and continuity across restarts. It is written in Rust with six dependencies and no async runtime; 1,200+ tests run without model calls, and Telegram and Discord connect directly.
- [**Chatgpt-Codex-App-Plus**](https://github.com/phenomenoner/Chatgpt-Codex-App-Plus) — A public, installable version of the Codex skills, review gate, long-run supervision, and delegation rules I use in day-to-day work. It does not dump an entire personal configuration into a repository: synchronization accepts only manifest-approved files and stops on credentials, private paths, unknown files, or hash mismatches.
- [**hermes-agent-harness-plus**](https://github.com/phenomenoner/hermes-agent-harness-plus) — A local workspace for long AI sessions, with a task canvas, evidence summaries, and semantic search. Useful findings from the morning do not disappear under the afternoon's conversation, and the data stays on your machine.

### Memory and multi-agent coordination

- [**openclaw-mem**](https://github.com/phenomenoner/openclaw-mem) — The goal is not to make an AI remember everything. Each memory keeps its source and the reason it was included or excluded, changes can be rolled back, and trust policy—not similarity alone—controls retrieval.
- [**a2a-superhub**](https://github.com/phenomenoner/a2a-superhub) — Shared tasks, artifacts, and memory for agents built with different frameworks. Agent A can stop halfway and Agent B can pick up days later with provenance intact. The underlying content is Markdown, so Obsidian and git can work with it directly.

### Taiwan trading and domain workflows

- [**steamer-card-engine**](https://github.com/phenomenoner/steamer-card-engine) — A Taiwan day-trading strategy runtime. Strategy cards describe trading intent without placing broker orders directly; stop-loss, forced liquidation, emergency braking, and replay live at the architecture layer.
- [**neoapi-skill**](https://github.com/phenomenoner/neoapi-skill) — Fubon Neo API documentation and practical safeguards organized into a workflow an AI can follow. Test and live environments stay separate, offline documentation snapshots are included, and 13 guardrails cover common order risks. It works with Codex, Claude, and Gemini.

## ⚙️ How I make trade-offs

- If ordinary code can solve a problem reliably, do not bet on a model guessing correctly every time.
- Before any external side effect, record the intent; afterward, record the result. Incidents are much easier to debug when there is a ledger.
- Authority starts closed. Without explicit permission, do not place an order, send a message, or change external state.
- Replay, restart recovery, and emergency stops need room in the design from the beginning, not as pre-launch patches.
- Keep data local when practical. SQLite, JSONL, and Markdown are ordinary tools, which is often exactly why they last.
- AI can research, propose, and review. A human keeps control of the final step that can affect a market or an external system.

## 🛠️ Stack

![Rust](https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![PowerShell](https://img.shields.io/badge/PowerShell-5391FE?style=flat-square&logo=powershell&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-003B57?style=flat-square&logo=sqlite&logoColor=white)
![Qdrant](https://img.shields.io/badge/Qdrant-DC244C?style=flat-square&logo=qdrant&logoColor=white)
![MCP](https://img.shields.io/badge/MCP-Model_Context_Protocol-5A67D8?style=flat-square)
![Markdown](https://img.shields.io/badge/Markdown-000000?style=flat-square&logo=markdown&logoColor=white)

**Domains:** AI Agent Infrastructure · Memory Governance · Multi-Agent Coordination · Taiwan Quant / Algorithmic Trading

## 📫 Contact

- Website: [phenomenoner.github.io](https://phenomenoner.github.io)
- GitHub: [@phenomenoner](https://github.com/phenomenoner)
- Email: [phenomenoner@gmail.com](mailto:phenomenoner@gmail.com)

If you also work on agent runtimes, memory, or trading systems, feel free to get in touch. I am more interested in design details, failure cases, and verification than polished pitches.
