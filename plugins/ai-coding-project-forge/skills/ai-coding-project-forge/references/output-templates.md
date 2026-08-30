# Project document templates / 專案文件模板

Write every heading and field in the user's selected language. The English and Traditional Chinese labels below are semantic equivalents, not a requirement to duplicate both languages.

## PRODUCT.md

Include: project name / 專案名稱, one-sentence goal / 一句話目標, users / 使用者, current pain / 現況痛點, scenarios / 使用情境, inputs and outputs / 輸入輸出, workflow / 操作流程, screens / 主要畫面, MVP modules / MVP 模組, later phase / 第二階段, explicitly excluded / 明確不做, business rules / 商業規則, assumptions to confirm / 假設待確認, success measures / 成功指標.

## ARCHITECTURE.md

Include: architecture goals and principles / 架構目標與原則, system boundary / 系統邊界, frontend, backend, modules, data model / 資料模型, file storage / 檔案保存, accounts and roles / 帳號角色, workspace isolation / 工作空間隔離, AI versus deterministic responsibilities / AI 與非 AI 分工, model routing / 模型路由, secrets / 密鑰, privacy / 隱私, logs / 日誌, deployment / 部署, backup and rollback / 備份回滾, rationale / 技術選擇理由, risks and open decisions / 風險與待決定.

## ACCEPTANCE.md

Include scope, environment, test data, and functional/error/boundary cases. Add authorization, privacy, performance, cost, backup, and rollback when applicable. Use the selected-language equivalent of:

```markdown
### AC-001 Case name / 案例名稱
- Related module / 對應模組：
- Given / 給定：
- When / 當：
- Then / 那麼：
- Must not / 不允許：
- Test data / 測試資料：
- Evidence / 驗收證據：
- Result / 結果：Not tested / 未測試
```

## AGENTS.md

Keep it concise. Include required reading, project purpose and scope, project map, build and test commands, engineering and safety rules, smallest vertical slice, definition of done, and mandatory stop conditions. Mark unverified commands as `To confirm` / `待確認`; never invent them.

## START_CODEX.md

Use the user's selected language. The meaning must remain:

```markdown
# Start Codex implementation / 啟動 Codex 施工

Read PRODUCT.md, ARCHITECTURE.md, ACCEPTANCE.md, AGENTS.md, and the existing project completely.

In the first turn only:
1. Restate the goal, MVP, and excluded scope.
2. List open questions, assumptions, and major risks.
3. Inspect existing files, runtime, and available commands.
4. Propose the smallest vertical-slice plan.
5. List planned file changes and acceptance cases.

Do not modify code in this turn. Wait for approval of the plan before implementation.
```
