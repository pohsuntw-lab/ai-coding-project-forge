# 具象 AI Coding 專案鍛造師 / AI Coding Project Forge

**不只和 AI 聊天，開始用 AI 創造自己的工具。**

把日常語言中的軟體想法，整理成 Codex 能安全開工的完整規格。Turn an everyday-language software idea into a clear, testable, Codex-ready project package.

**繁體中文與 English 雙語支援｜Traditional Chinese and English**

[在 ChatGPT 安裝插件 / Install in ChatGPT](https://chatgpt.com/plugins/plugins_6a93c934664c8191baa12828cdb9cc58)

## 為什麼使用 / Why use it

許多人已經會用 ChatGPT 聊天，卻不知道如何把生活、工作中的想法變成可以重複使用的工具。你不需要先學會 PRD、架構、API 或程式語言，只要像平常聊天一樣說出想法，插件就會一步一步協助你想清楚第一版，並在背後完成專業規格。

Many people already chat with AI but do not know how to turn an idea from daily life or work into a reusable tool. You do not need to learn PRDs, architecture, APIs, or programming first. Explain the idea in ordinary language; the plugin helps you define a realistic first version and prepares the professional specifications behind the scenes.

## 適合誰 / Who it is for

- 只會使用 ChatGPT 聊天，想嘗試開發第一款工具的人。
- 想做 App、網站、個人效率工具或 AI 工作流程，但沒有軟體背景的人。
- 需要把訪談筆記或零散構想整理成正式專案規格的團隊。
- 想接續既有程式，或在施工前檢查規格是否一致、可驗收的人。
- People who use ChatGPT and want to create their first tool.
- Non-technical users planning an app, website, personal productivity tool, or AI workflow.
- Teams turning notes and scattered ideas into an implementation brief.
- Builders continuing existing code or reviewing whether specifications are ready for Codex.

## 四段自然對話 / Four conversational stages

使用者不必選擇專案模式，也不必填寫八張需求表。插件會從一句自然的想法開始：

> 你想做一個什麼工具？請像平常聊天一樣告訴我，不完整也沒關係，我會陪你一步一步整理。

The user does not need to select a project mode or complete a requirements form. The plugin starts with one natural question:

> What tool would you like to make? Tell me as you normally would in a chat. It does not need to be complete; I will help you work it out step by step.

| 階段 | 使用者做什麼 | AI 在背後做什麼 |
|---|---|---|
| 1. 說出想法 | 用自己的話描述想做的工具 | 判斷問題、使用者與期望結果 |
| 2. 一起想清楚 | 每次回答一個簡單問題 | 整理輸入、輸出、流程與必要畫面 |
| 3. 確認第一版 | 確認或修改一頁專案藍圖 | 縮小範圍、規劃驗收與最簡單架構 |
| 4. 產生文件 | 取得五份文件並交給 Codex | 完成一致性檢查與施工交接 |

Eight professional decision areas remain inside the plugin as a completeness check, but users see only four simple conversational stages.

## 五份交付文件 / Five deliverables

| 文件 | 用途 / Purpose |
|---|---|
| `PRODUCT.md` | 產品目標、使用者、流程、畫面、第一版與成功指標 / Product goals, users, workflow, screens, first version, and success measures |
| `ARCHITECTURE.md` | 系統邊界、模組、資料、AI 分工、安全、部署與回滾 / Boundaries, modules, data, AI responsibilities, security, deployment, and rollback |
| `ACCEPTANCE.md` | 正常、錯誤、邊界、權限與復原案例 / Normal, error, boundary, authorization, and recovery cases |
| `AGENTS.md` | Codex 每次施工都必須遵守的規則與完成定義 / Rules and definition of done for Codex |
| `START_CODEX.md` | 新 Codex 任務的第一則提示，先檢查與規劃、不立即修改 / First-task prompt that requires inspection and planning before edits |

五份文件是給 Codex 施工使用。一般使用者只需確認一頁容易理解的第一版專案藍圖，不必逐份審查技術文件。

The five files are for Codex implementation. Ordinary users confirm one plain-language first-version blueprint rather than reviewing every technical file separately.

## 雙語使用方式 / Bilingual behavior

- 插件會依你的訊息自動使用繁體中文或英文。
- 訪談、藍圖與五份文件會保持同一語言。
- 對話中切換語言時，已確認的決策會保留。
- 只有你明確要求時，才會同時產生中英文兩套文件。
- The plugin automatically follows the language of your request.
- The conversation, blueprint, and all five files stay in the selected language.
- Confirmed decisions are preserved if you switch languages mid-conversation.
- Two complete language versions are produced only when explicitly requested.

## 快速開始 / Quick start

安裝後，在新對話中提及插件並輸入：

- `我想做一個自己的工具，但我不懂軟體開發，請陪我一步一步想清楚。`
- `I have an idea for a tool but no software background. Help me work it out step by step.`
- `檢查我的專案規格是否足以交給 Codex 施工。`
- `Review whether my project specification is ready for Codex implementation.`

## 設計原則 / Design principles

- 對使用者保持簡單，對 Codex 保持嚴謹 / Simple for the user, rigorous for Codex.
- 使用者用生活語言回答，AI 負責轉譯成軟體規格 / Users speak naturally; AI translates the answers into specifications.
- 規格核准前不寫程式 / No implementation before the first-version blueprint is approved.
- 不捏造資料、法規、商業規則或技術環境 / Never invent data, laws, business rules, or environments.
- 優先完成一條真正能運作的流程 / Start with one complete workflow that can produce a real result.
- 高風險或不可逆行動保留人工核准 / Keep humans in control of high-risk or irreversible actions.
- 每個第一版模組都能追溯到架構責任與驗收案例 / Every first-version module maps to architecture ownership and acceptance cases.

## 安裝、支援與政策 / Installation, support, and policies

- [學生安裝與使用 / Student installation](STUDENT_INSTALLATION.md)
- [教師發佈指南 / Educator publishing guide](PUBLISHING_GUIDE.md)
- [支援 / Support](SUPPORT.md)
- [隱私權政策 / Privacy Policy](PRIVACY.md)
- [服務條款 / Terms of Service](TERMS.md)

## 版本 / Version

`v0.3.0` replaces the visible eight-card interview with four natural conversational stages, lets the plugin infer the project mode, asks one main question at a time, proposes the simplest first version, and generates the five files as one coordinated package.

`v0.3.0` 將使用者可見的八張決策卡改為四段自然對話，由插件自動判斷專案模式、每次只問一個主要問題、主動提出最簡單第一版，並一次產生相互一致的五份文件。

`v0.2.0` added full Traditional Chinese and English interaction, bilingual documentation, and language-aware deliverables.
