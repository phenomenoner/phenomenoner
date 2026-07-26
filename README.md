# 嗨，我是 phenomenoner 👋

**Quant / Algo Trading / AI Harness Engineering** — Taipei (25°N, 121°E)

> 我做 AI agent 的基礎建設：收據、權限、斷路器——讓自主系統上線之後，大家都睡得著覺。
>
> I build infrastructure for AI agents — receipts, permissions, and circuit breakers — so you can ship autonomy and still sleep at night.

我從量化交易圈過來。錢在線上跑的系統會逼你養成一些好習慣：副作用要留收據、權限預設關閉、模型只負責思考、人握著斷路器。這些習慣，我每個專案都照做。

---

## 🧭 從這裡開始 Start Here

| 你想看的是… | 去這裡 |
|---|---|
| 🦀 一個 agent 框架可以多「無聊」而可靠（Rust、6 個依賴、1,200+ 測試） | [agent-harness-core](https://github.com/phenomenoner/agent-harness-core) |
| 🧠 AI 記憶怎麼做到有出處、可還原 | [openclaw-mem](https://github.com/phenomenoner/openclaw-mem) |
| 🔗 不同框架的 agents 怎麼非同步共享知識 | [a2a-superhub](https://github.com/phenomenoner/a2a-superhub) |
| 📈 AI 出主意、人做決定的當沖交易架構 | [steamer-card-engine](https://github.com/phenomenoner/steamer-card-engine) |
| 🤝 怎麼把散落的領域知識整理成 AI 能照著做的 skill | [neoapi-skill](https://github.com/phenomenoner/neoapi-skill) |

## 🚀 What I Build

| 專案 | 一句話 | 核心想法 |
|---|---|---|
| [**agent-harness-core**](https://github.com/phenomenoner/agent-harness-core) ![stars](https://img.shields.io/github/stars/phenomenoner/agent-harness-core?style=flat&logo=github&label=%E2%98%85) | 自架 AI agent runtime（Rust）：佇列、權限、稽核、跨重啟的 session 接續 | 無聊是刻意的，可靠才是重點 |
| [**openclaw-mem**](https://github.com/phenomenoner/openclaw-mem) ![stars](https://img.shields.io/github/stars/phenomenoner/openclaw-mem?style=flat&logo=github&label=%E2%98%85) | AI 記憶治理層：出處、信任政策、trace 收據、可還原 | 記憶不用最大，但要說得出來源 |
| [**a2a-superhub**](https://github.com/phenomenoner/a2a-superhub) ![stars](https://img.shields.io/github/stars/phenomenoner/a2a-superhub?style=flat&logo=github&label=%E2%98%85) | Agent-to-agent 協調中樞：任務生命週期 + Markdown 為本的共享記憶 | 每個 agent 都是同事，不是下屬 |
| [**hermes-agent-harness-plus**](https://github.com/phenomenoner/hermes-agent-harness-plus) ![stars](https://img.shields.io/github/stars/phenomenoner/hermes-agent-harness-plus?style=flat&logo=github&label=%E2%98%85) | Agent 工具箱：任務畫布、證據追蹤、本地語意搜尋 | 結論要拿得出證據 |
| [**neoapi-skill**](https://github.com/phenomenoner/neoapi-skill) ![stars](https://img.shields.io/github/stars/phenomenoner/neoapi-skill?style=flat&logo=github&label=%E2%98%85) | 台股富邦 Neo API 的 AI skill：13 條防呆守則、測試/正式環境隔離 | 先讀文件，再下單 |
| [**steamer-card-engine**](https://github.com/phenomenoner/steamer-card-engine) ![stars](https://img.shields.io/github/stars/phenomenoner/steamer-card-engine?style=flat&logo=github&label=%E2%98%85) | 台股當沖策略 runtime：策略卡只表達意圖，不直接碰券商下單 | AI 出主意，人做決定 |

## ⚙️ 我寫系統的五個習慣 How I Build

Demo 誰都會做，我比較在意出事之後，查不查得到原因。這五個習慣，我每個專案都照做：

1. **Receipts over trust** — 有副作用的事，先把意圖跟結果寫進帳本再做。真的出事了，翻紀錄就能還原現場。
2. **Deterministic first** — 權限、排程、佇列交給普通程式碼就好，模型只負責思考。該確定的地方，不要有驚喜。
3. **Fail-closed** — 白名單沒設、身分沒綁、憑證不在，系統就什麼都不做。安全是預設值，不是之後才補的。
4. **Local-first, boring tech** — SQLite、JSONL、Markdown、同步 Rust、依賴越少越好。無聊的技術出問題好追，也活得比較久。
5. **Humans hold the breaker** — AI 可以寫策略、跑驗證、做回放分析，但按下 live 那顆按鈕的，永遠是人。

## 🛠️ Stack

![Rust](https://img.shields.io/badge/Rust-000000?style=flat&logo=rust&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-003B57?style=flat&logo=sqlite&logoColor=white)
![Qdrant](https://img.shields.io/badge/Qdrant-DC244C?style=flat&logo=qdrant&logoColor=white)
![MCP](https://img.shields.io/badge/MCP-Model_Context_Protocol-5A67D8?style=flat)
![Markdown](https://img.shields.io/badge/Markdown-000000?style=flat&logo=markdown&logoColor=white)

**領域 Domains:** AI Agent Infrastructure · Memory Governance · Multi-Agent Coordination · Quant / 台股演算法交易

## 📫 Connect

- GitHub: [@phenomenoner](https://github.com/phenomenoner)
- Email: phenomenoner@gmail.com

*Agent 基礎設施、記憶治理、交易系統，或任何想把 AI 做得更可靠的題目，都歡迎找我聊。*
*Open to collaboration on agent infrastructure, memory governance, and trading systems engineering.*
