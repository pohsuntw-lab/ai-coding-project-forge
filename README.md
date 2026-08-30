# 具象 AI Coding 專案鍛造師 / AI Coding Project Forge

把模糊的軟體想法整理成 Codex 能安全開工的完整規格。Turn an early software idea into a clear, testable, Codex-ready project package.

**繁體中文與 English 雙語支援｜Traditional Chinese and English**

[在 ChatGPT 安裝插件 / Install in ChatGPT](https://chatgpt.com/plugins/plugins_6a93c934664c8191baa12828cdb9cc58)

## 為什麼使用 / Why use it

許多 AI Coding 專案不是卡在寫程式，而是還沒說清楚使用者、流程、範圍、資料、風險與驗收方式。本插件以八張決策卡逐步訪談，讓初學者不必先懂軟體術語，也能得到一致、可檢查、可交付 Codex 的文件。

Many AI coding projects fail before implementation because users, workflows, scope, data, risks, and acceptance criteria are still unclear. This plugin uses eight guided decision cards so non-technical users can create consistent, reviewable specifications without learning software jargon first.

## 適合誰 / Who it is for

- 想做 App、網站、內部工具或 AI 工作流程，但不知道從哪開始的人。
- 需要把訪談筆記或零散構想整理成正式專案規格的團隊。
- 教師帶領學生從需求分析進入 Codex 實作的課程。
- 想在施工前檢查現有規格是否一致、可驗收的人。
- People planning an app, website, internal tool, or AI workflow.
- Teams turning notes and scattered ideas into an implementation brief.
- Educators teaching the path from requirements to Codex implementation.
- Builders reviewing whether existing specifications are consistent and testable.

## 八張決策卡 / Eight decision cards

| # | 繁體中文 | English | 主要成果 / Outcome |
|---|---|---|---|
| 1 | 問題 | Problem | 使用者、痛點與期望結果 |
| 2 | 輸入輸出 | Inputs & outputs | 真實範例、正常與異常情境 |
| 3 | 操作故事 | User story | 第一版主要成功路徑 |
| 4 | 畫面 | Screens | 3–5 個低保真畫面與狀態 |
| 5 | 範圍 | Scope | MVP、後續、不做與待決定 |
| 6 | 驗收 | Acceptance | Given–When–Then 驗收案例 |
| 7 | 架構 | Architecture | 與真實需求對應的技術設計 |
| 8 | 施工 | Handoff | 最小垂直切片與 Codex 開工計畫 |

## 五份交付文件 / Five deliverables

| 文件 | 用途 / Purpose |
|---|---|
| `PRODUCT.md` | 產品目標、使用者、流程、畫面、MVP 與成功指標 / Product goals, users, workflow, screens, MVP, and success measures |
| `ARCHITECTURE.md` | 系統邊界、模組、資料、AI 分工、安全、部署與回滾 / Boundaries, modules, data, AI responsibilities, security, deployment, and rollback |
| `ACCEPTANCE.md` | 正常、錯誤、邊界、權限與復原案例 / Normal, error, boundary, authorization, and recovery cases |
| `AGENTS.md` | Codex 每次施工都必須遵守的規則與完成定義 / Rules and definition of done for Codex |
| `START_CODEX.md` | 新 Codex 任務的第一則提示，先檢查與規劃、不立即修改 / First-task prompt that requires inspection and planning before edits |

## 雙語使用方式 / Bilingual behavior

- 插件會依你的訊息自動使用繁體中文或英文。
- 訪談、摘要與五份文件會保持同一語言。
- 對話中切換語言時，已確認的決策會保留。
- 只有你明確要求時，才會同時產生中英文兩套文件。
- The plugin automatically follows the language of your request.
- Interviews, summaries, and all five files stay in the selected language.
- Confirmed decisions are preserved if you switch languages mid-conversation.
- Two complete language versions are produced only when explicitly requested.

## 快速開始 / Quick start

安裝後，在新對話中提及插件並輸入其中一句：

- `我要建立新的 AI Coding 專案，請用繁體中文從問題訪談開始。`
- `I want to start a new AI coding project. Interview me in English.`
- `檢查我的專案規格是否足以交給 Codex 施工。`
- `Review whether my project specification is ready for Codex implementation.`

## 設計原則 / Design principles

- 規格核准前不寫程式 / No implementation before specification approval.
- 不捏造資料、法規、商業規則或技術環境 / Never invent data, laws, business rules, or environments.
- 優先採用最簡單可行方案 / Start with the simplest viable design.
- 高風險或不可逆行動保留人工核准 / Keep humans in control of high-risk or irreversible actions.
- 每個 MVP 模組都必須能追溯到架構責任與驗收案例 / Every MVP module must map to architecture ownership and acceptance cases.

## 安裝、支援與政策 / Installation, support, and policies

- [學生安裝與使用 / Student installation](STUDENT_INSTALLATION.md)
- [教師發佈指南 / Educator publishing guide](PUBLISHING_GUIDE.md)
- [支援 / Support](SUPPORT.md)
- [隱私權政策 / Privacy Policy](PRIVACY.md)
- [服務條款 / Terms of Service](TERMS.md)

## 版本 / Version

`v0.2.0` adds full Traditional Chinese and English interaction, bilingual documentation, and language-aware deliverables.

`v0.2.0` 新增完整繁中／英文互動、雙語文件與依使用者語言產出的能力。
