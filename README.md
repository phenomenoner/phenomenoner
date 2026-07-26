# 嗨，我是 phenomenoner 👋

**Quant / Algo Trading / AI Harness Engineering** — Taipei (25°N, 121°E)

> 我做 AI agent 的基礎建設，上線之後睡得著覺的那種。
>
> I build AI agent infrastructure — the kind that lets you sleep at night.

量化交易出身。錢在線上跑的系統會逼你養成一些好習慣：動手前先留紀錄、權限預設關閉、模型只負責思考、方向盤永遠在人手上。這些習慣，我每個專案都照做。

---

## 🧭 從這裡開始 Start Here

| 你想看的是… | 去這裡 |
|---|---|
| 🦀 一個 agent 框架可以多「無聊」而可靠（Rust、6 個依賴、1,200+ 測試不用呼叫模型） | [agent-harness-core](https://github.com/phenomenoner/agent-harness-core) |
| 🧠 AI 的記憶怎麼做到每筆有出處、改壞了退得回去 | [openclaw-mem](https://github.com/phenomenoner/openclaw-mem) |
| 🔗 不同家的 agents 怎麼合作，離線了還能自己補課 | [a2a-superhub](https://github.com/phenomenoner/a2a-superhub) |
| 📈 AI 出主意、人做決定的台股當沖架構 | [steamer-card-engine](https://github.com/phenomenoner/steamer-card-engine) |
| 🤝 怎麼把一整套領域知識整理成 AI 能照著做的 skill | [neoapi-skill](https://github.com/phenomenoner/neoapi-skill) |

## 🚀 What I Build

| 專案 | 在做什麼 | 招牌亮點 |
|---|---|---|
| [**agent-harness-core**](https://github.com/phenomenoner/agent-harness-core) | 大多數 agent 框架只管「怎麼想」，這個專門管「怎麼上線」：進線、權限、佇列、投遞、稽核、跨重啟接續，一手包 | Rust 寫的，6 個依賴、沒有 async runtime；1,200+ 測試全程不用呼叫模型，Telegram / Discord 直接接 |
| [**openclaw-mem**](https://github.com/phenomenoner/openclaw-mem) | AI 記憶的治理層：每筆記憶有出處、被排除有理由，改壞了退得回去 | 不跟人比 recall 分數，比「說得出為什麼」——同一份記憶、同一個查詢，換個信任政策就給出不同的受控結果，全程有紀錄可查 |
| [**a2a-superhub**](https://github.com/phenomenoner/a2a-superhub) | 不同框架的 agents 一起做事的協調中樞：任務生命週期、artifacts、共享記憶 | 週一早上你跟 agent A 講的事，週四凌晨 agent B 醒來自己讀到，出處齊全——記憶用 Markdown 存，Obsidian 打得開、git 管得住 |
| [**hermes-agent-harness-plus**](https://github.com/phenomenoner/hermes-agent-harness-plus) | 長時間 AI 工作的隨身筆記本：任務畫布、證據自動摘要、本地語意搜尋 | 跟 AI 工作一整天，早上查到的重點常被下午的對話淹沒——它幫你隨手記下來，之後用問的就找得回來。資料全存在自己電腦，不外傳 |
| [**neoapi-skill**](https://github.com/phenomenoner/neoapi-skill) | 把富邦 Neo API 的官方文件跟實戰經驗，做成 AI 能照著做的交易工作流程 | 13 條防呆守則、測試/正式環境嚴格分離、附離線文件快照；Codex / Claude / Gemini 都能直接用 |
| [**steamer-card-engine**](https://github.com/phenomenoner/steamer-card-engine) | 台股當沖策略 runtime：策略卡只表達「想做什麼」，不直接碰券商下單 | 停損、強制平倉、緊急煞車是架構內建不是選配；回放驗證是一級需求，策略改了可以回頭對答案 |

## ⚙️ 我寫系統的五個習慣 How I Build

Demo 誰都會做，我比較在意出事之後，查不查得到原因。用大白話講：

1. **Receipts over trust｜先記帳，再動手** — 系統要做任何會留下影響的事，先寫下「我要做什麼」，做完再記「發生了什麼」。哪天出包，翻本子就知道來龍去脈。
2. **Deterministic first｜該規矩的地方就規矩** — 開門、排隊、看時鐘這種事，交給一板一眼的程式來做，AI 只負責出腦力。
3. **Fail-closed｜門禁預設是關的** — 名單上沒有你，門就不會開。不是先放進來、出事再想辦法擋。
4. **Local-first, boring tech｜資料放家裡，工具挑耐用的** — SQLite、JSONL、Markdown、同步 Rust。無聊的技術出問題好追，也活得比較久。
5. **Humans hold the breaker｜方向盤在人手上** — AI 可以提案、試算、複盤，但真正按下去的那一下，永遠是人。

## 🛠️ Stack

![Rust](https://img.shields.io/badge/Rust-000000?style=flat&logo=rust&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-003B57?style=flat&logo=sqlite&logoColor=white)
![Qdrant](https://img.shields.io/badge/Qdrant-DC244C?style=flat&logo=qdrant&logoColor=white)
![MCP](https://img.shields.io/badge/MCP-Model_Context_Protocol-5A67D8?style=flat)
![Markdown](https://img.shields.io/badge/Markdown-000000?style=flat&logo=markdown&logoColor=white)

**領域 Domains:** AI Agent Infrastructure · Memory Governance · Multi-Agent Coordination · Quant / 台股演算法交易

## 📫 Connect

- 🌐 個人網站 Website: [phenomenoner.github.io](https://phenomenoner.github.io)
- 💻 GitHub: [@phenomenoner](https://github.com/phenomenoner)
- ✉️ Email: phenomenoner@gmail.com

*對 agent 基礎設施、記憶治理或交易系統有興趣，歡迎來聊聊。*
*Into agent infrastructure, memory governance, or trading systems? Come say hi.*
