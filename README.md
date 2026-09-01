# EW AI Coding

## Enterprise AI Application Pre-Deployment Forge

**Turn workplace knowledge into a buildable, testable, and governable AI application blueprint—before coding begins.**

EW AI Coding is a free bilingual skill that helps employees and teams describe a real workplace problem in ordinary language, focus the first useful version, separate software, model, data, and human responsibilities, and generate five consistent files ready for Codex.

**企業 AI 應用開發前置部署鍛造工具**

EW AI Coding 是免費的中英雙語技能，引導企業員工以自然語言說出工作問題，在正式開發前完成問題聚焦、流程梳理、資料條件、系統邊界、模型分工、人工核准與驗收標準，最後產生五份可交付 Codex 的一致文件。

[Install in ChatGPT / 在 ChatGPT 安裝](https://chatgpt.com/plugins/plugins_6a93c934664c8191baa12828cdb9cc58)

## Why it matters

Office made document, spreadsheet, and presentation creation a basic workplace capability. AI Coding is making small application creation accessible to the people who understand the work best.

EW AI Coding does not claim that every employee should become a software engineer. It helps the employee who understands the problem define what should be built, what data is required, what success means, and when a specialist must be involved.

## 為什麼企業需要

Office 讓文件、試算表與簡報成為員工的基礎能力；AI Coding 正在讓最瞭解工作的人，也能把經驗轉化為小型數位工具。

EW AI Coding 不是要求每位員工成為軟體工程師，而是協助員工定義應該開發什麼、需要哪些資料、如何驗收，以及何時必須引入模型、領域、資安或軟體專家。

## What “pre-deployment” means

Here, **pre-deployment** does not mean deploying code to a server. It means deploying the business problem, workflow, data conditions, responsibilities, system boundaries, and acceptance criteria into a reliable implementation blueprint before development starts.

這裡的「前置部署」不是把程式部署到伺服器，而是在開發前，先把企業問題、工作流程、資料條件、權責分工、系統邊界與驗收標準部署到可執行的開發藍圖中。

## Who it is for

- Employees who understand a recurring workplace problem but do not have a software background.
- Department AI application champions who want to build useful internal tools with Codex.
- Teams turning interviews, meeting notes, and operating experience into an implementation-ready blueprint.
- Builders reviewing whether an existing specification is consistent, safe, and testable.
- 了解現場痛點、但沒有軟體背景的企業員工。
- 希望用 Codex 建立部門工具的 AI 應用種子人員。
- 要把訪談、會議紀錄與工作經驗轉成可施工藍圖的團隊。
- 需要檢查既有規格是否一致、安全、可驗收的開發者。

## Four conversational stages

1. **Say the problem** — Describe the work in ordinary language.
2. **Work it out together** — Clarify inputs, results, workflow, data, exceptions, and responsibility.
3. **Confirm the first version** — Approve one small, complete, useful application blueprint.
4. **Create the files** — Generate one consistent Codex handoff package.

四段自然對話：說出問題、一起想清楚、確認第一版、產生文件。使用者不必先學會 PRD、架構、API 或程式語言。

## Five Codex-ready deliverables

| File | Purpose / 用途 |
|---|---|
| `PRODUCT.md` | Problem, users, workflow, screens, first-version scope, and success measures / 問題、使用者、流程、畫面、第一版與成功指標 |
| `ARCHITECTURE.md` | Software, model, data, human responsibility, security, deployment, and rollback / 程式、模型、資料、人工責任、安全、部署與回滾 |
| `ACCEPTANCE.md` | Measurable normal, error, boundary, authorization, and recovery cases / 可量測的正常、錯誤、邊界、權限與復原案例 |
| `AGENTS.md` | Rules, commands, stop conditions, and definition of done for Codex / Codex 必須遵守的規則、命令、停止條件與完成定義 |
| `START_CODEX.md` | The first Codex instruction: inspect and propose a plan before editing / 啟動 Codex 的第一則指令：先檢查與規劃，再開始修改 |

## Enterprise governance boundary

EW AI Coding classifies the application before handoff:

| Level | Typical scope | Required control |
|---|---|---|
| Personal tool | One user, non-sensitive data, reversible work | User testing |
| Department tool | Shared workflow or team data | Owner, permissions, versioning, and department review |
| Enterprise system | Sensitive data, cross-department use, or critical records | IT, security, architecture, and formal acceptance |
| High-risk system | Money, legal or medical action, safety, or device control | Qualified specialists and mandatory human approval |

企業可自行建立一般工具，但涉及敏感資料、跨部門、財務、安全、法律、醫療或設備控制時，必須升級治理與專業審查。AI Coding 能降低開發門檻，不會取消工程責任。

## Responsibility routing

- **Codex and deterministic software:** interfaces, workflows, databases, permissions, reports, sorting, and state transitions.
- **Model specialists:** computer vision, time-series detection, retrieval, multimodal models, fine-tuning, evaluation, and inference optimization.
- **Domain specialists:** CAD geometry, manufacturing, energy, finance, healthcare, or other professional rules.
- **Data specialists and infrastructure:** data quality, lineage, replay, integration, and reliable real-world data sources.
- **Humans:** approval of high-risk, irreversible, or professionally accountable decisions.

EW AI Coding 的目的不是把所有工作交給單一軟體商，而是先讓企業掌握問題、規格與驗收，再精準判斷真正需要哪一類專家。

## Language behavior

- English and Traditional Chinese are fully supported.
- The skill follows the language of the latest user request.
- The interview, blueprint, and five files remain in one selected language.
- Bilingual deliverables are created only when explicitly requested.
- 完整支援英文與繁體中文，並依使用者最新訊息選擇語言。
- 訪談、藍圖與五份文件保持同一語言；只有明確要求時才產生雙語文件。

## Quick start

- `Help me turn a workplace problem into a focused, testable AI application blueprint for Codex.`
- `請幫我把企業工作問題聚焦成可開發、可驗收的 AI 應用，再交給 Codex。`
- `Review my existing MD files for Codex readiness.｜請檢查既有 MD 文件是否一致且可交給 Codex 開發。`

## Design principles

- Simple for employees; rigorous for implementation.
- Define the problem before choosing a model or technical stack.
- No coding before the first-version blueprint is approved.
- Do not invent data, laws, business rules, users, departments, or environments.
- Build one complete useful workflow before expanding scope.
- Keep humans in control of high-risk or irreversible actions.
- Map every first-version module to architecture ownership and acceptance evidence.
- Preserve enterprise ownership of code, data, and knowledge.

## Installation, support, and policies

- [Student installation / 學員安裝](STUDENT_INSTALLATION.md)
- [Educator publishing guide / 教師發佈指南](PUBLISHING_GUIDE.md)
- [Support / 支援](SUPPORT.md)
- [Privacy Policy / 隱私權政策](PRIVACY.md)
- [Terms of Service / 服務條款](TERMS.md)

## Version

`v0.3.4` corrects the public Directory and ChatGPT composer icons so the new gold elephant brand asset is shown consistently. Functional behavior is unchanged from v0.3.3.

`v0.3.4` 修正外掛目錄與 ChatGPT 輸入框圖示，統一顯示新的金色大象商標；功能內容與 v0.3.3 相同。

`v0.3.3` establishes EW AI Coding as an **Enterprise AI Application Pre-Deployment Forge**, makes English the primary product language with Traditional Chinese support, adds enterprise application risk routing, and clarifies the boundary between AI Coding, model specialists, domain experts, data infrastructure, and human approval.

`v0.3.3` 將 EW AI Coding 正式定位為「企業 AI 應用開發前置部署鍛造工具」，以英文為主、繁體中文為輔，新增企業應用風險分流，並明確區分 AI Coding、模型專家、領域專家、資料基礎設施與人工核准的責任。

`v0.3.0` simplified the visible interview into four natural conversational stages and generated the five files as one consistent package.

`v0.2.0` added full Traditional Chinese and English interaction and language-aware deliverables.
