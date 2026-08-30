# Conditional interview flow / 條件式訪談流程

Use labels in the user's selected language. The bilingual labels below define equivalent meaning; do not show both languages unless the user asks for bilingual output.

## Progress / 進度顯示

Start each turn with `Project Forge: Card N/8 | Current: card name` or `專案鍛造進度：第 N/8 卡｜目前：卡片名稱`.

## Card 1: Problem / 卡1：問題

Collect the target user, current method, most painful step, and desired improvement. Complete this sentence:

> Improve [painful work] for [user] from [current method] to [desired outcome].
>
> 為【使用者】把【麻煩工作】從【目前做法】改善成【期望結果】。

## Card 2: Inputs and outputs / 卡2：輸入輸出

Request at least one de-identified real input, the ideal output, a normal case, and an error case. If no example exists, help define a mock-data format and clearly mark it as unvalidated.

## Card 3: User story / 卡3：操作故事

Describe the main path: enter tool → input/upload → process → review → save/export. Keep only one primary success path in the first version.

## Card 4: Screens / 卡4：畫面

Design three to five low-fidelity screens. For each, list purpose, fields, primary actions, and loading/empty/error/success states. Do not choose a framework yet.

## Card 5: Scope / 卡5：範圍

Classify items as MVP, later phase, explicitly excluded, or undecided. Keep the MVP near three to six modules; propose a smaller version if it grows beyond that.

## Card 6: Acceptance / 卡6：驗收

Create Given–When–Then cases for each module. Cover normal, error, and boundary behavior. For multiple users or sensitive data, also cover authorization, isolation, privacy, and recovery.

## Card 7: Architecture / 卡7：架構

Ask only required decisions about delivery surface, frontend/backend, login, data, AI, deployment, and backup. Enable questions appropriate to personal, team, or public/sensitive use. Every technical component must solve a real requirement.

## Card 8: Implementation handoff / 卡8：施工

Confirm the project directory, smallest vertical slice, development phases, candidate test commands, definition of done, and Codex stop conditions.

## Card confirmation / 每卡確認格式

```markdown
### Card summary / 本卡摘要
- Confirmed / 已確認：
- Reasonable inference / 合理推論：
- To confirm / 待確認：
- Not in this phase / 暫不實作：
- Conflicts / 衝突：None / 無，或列出

Choose / 請選擇：Confirm / 確認本卡｜Edit / 修改答案｜Previous / 回到上一卡
```
