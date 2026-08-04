<div align="center">

# 嗨，我是 phenomenoner 👋

**台股量化交易 · Agent Infrastructure · Software Engineering**

做過交易系統，現在主要寫 agent runtime、記憶與協作工具，還有 Codex workflow。

📍 Taipei · 25°N, 121°E

[繁體中文](./README.md) · [English](./README.en.md) · [個人網站](https://phenomenoner.github.io) · [Email](mailto:phenomenoner@gmail.com)

</div>

---

## 我在做什麼

我原本做台股量化與演算法交易。交易系統不能只看回測漂不漂亮；真的上線之後，每一筆動作都要有紀錄，權限要收得住，行情或券商斷線時不能亂做事，出問題也要能重播還原。

後來一路做到 AI agent，習慣沒有差太多。我在意的不是 demo 看起來多聰明，而是系統跑久了之後還查得到、停得住，重啟後也接得回來。能用 deterministic code 處理的事情，我不會硬丟給模型猜。

> **該由程式守住的就寫清楚；該由人決定的，就不要偷偷自動化。**

## 🧭 Projects

### Agent runtime / developer tooling

- [**agent-harness-core**](https://github.com/phenomenoner/agent-harness-core) — 模型外圍那些不太適合拿來 demo、但上線後最容易出事的部分：ingress、權限、佇列、投遞、稽核，以及跨重啟續跑。目前以 Rust 實作，6 個依賴、沒有 async runtime；1,200+ 個測試不需要呼叫模型，Telegram / Discord 可以直接接。
- [**Chatgpt-Codex-App-Plus**](https://github.com/phenomenoner/Chatgpt-Codex-App-Plus) — 把平常累積的 Codex skills、review gate、長時間命令監督與分工規則，整理成可安裝、可檢查的公開版本。不是把整份個人設定直接打包上傳；同步只收 manifest 核准的檔案，碰到憑證、私有路徑、未知檔案或 hash 不一致就停。
- [**hermes-agent-harness-plus**](https://github.com/phenomenoner/hermes-agent-harness-plus) — 長時間跟 AI 工作時用的本地工作台，保存任務畫布、證據摘要與語意索引。早上查到的東西，不會到下午就被長對話洗掉；資料也留在自己的電腦。

### Memory / multi-agent coordination

- [**openclaw-mem**](https://github.com/phenomenoner/openclaw-mem) — 重點不是讓 AI 記得越多越好，而是每筆記憶都要知道從哪裡來、為什麼被採用或排除，改壞了也退得回去。查詢結果會受信任政策約束，不是單純做相似度搜尋。
- [**a2a-superhub**](https://github.com/phenomenoner/a2a-superhub) — 讓不同框架的 agents 共用任務、artifacts 與記憶。Agent A 先做到一半，Agent B 晚幾天再醒來，還是能沿著出處接手；底層內容用 Markdown 保存，Obsidian 和 git 都能直接處理。

### Taiwan trading / domain workflows

- [**steamer-card-engine**](https://github.com/phenomenoner/steamer-card-engine) — 台股當沖策略 runtime。策略卡只寫交易意圖，不直接碰券商下單；停損、強制平倉、緊急煞車與 replay 都放在架構層處理。
- [**neoapi-skill**](https://github.com/phenomenoner/neoapi-skill) — 把富邦 Neo API 的官方文件與實務防呆整理成 AI 能照著走的 workflow。測試與正式環境分開，附離線文件快照，也把常見下單風險寫進 13 條 guardrails；Codex、Claude、Gemini 都能使用。

## ⚙️ 做系統時，我通常這樣取捨

- 能用一般程式穩定解決的，就不要賭模型每次都猜對。
- 任何會留下外部影響的動作，先記 intent，做完再留 result；有問題才有帳可查。
- 權限預設關閉。沒有明確授權，就不送單、不發訊息、不改外部狀態。
- Replay、重啟恢復和緊急停止不是上線前才補的功能，設計時就要留位置。
- 資料能放本機就先放本機；SQLite、JSONL、Markdown 這類普通但耐用的工具通常很好用。
- AI 可以做研究、提案和複盤，最後會真的影響市場或外部系統的那一步，方向盤留給人。

## 🛠️ Stack

![Rust](https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![PowerShell](https://img.shields.io/badge/PowerShell-5391FE?style=flat-square&logo=powershell&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-003B57?style=flat-square&logo=sqlite&logoColor=white)
![Qdrant](https://img.shields.io/badge/Qdrant-DC244C?style=flat-square&logo=qdrant&logoColor=white)
![MCP](https://img.shields.io/badge/MCP-Model_Context_Protocol-5A67D8?style=flat-square)
![Markdown](https://img.shields.io/badge/Markdown-000000?style=flat-square&logo=markdown&logoColor=white)

**Domains:** AI Agent Infrastructure · Memory Governance · Multi-Agent Coordination · 台股量化／演算法交易

## 📫 聯絡

- Website: [phenomenoner.github.io](https://phenomenoner.github.io)
- GitHub: [@phenomenoner](https://github.com/phenomenoner)
- Email: [phenomenoner@gmail.com](mailto:phenomenoner@gmail.com)

如果你剛好也在做 agent runtime、memory 或交易系統，歡迎來信。比起 pitch，我比較喜歡直接聊設計、失敗案例和怎麼驗證。
