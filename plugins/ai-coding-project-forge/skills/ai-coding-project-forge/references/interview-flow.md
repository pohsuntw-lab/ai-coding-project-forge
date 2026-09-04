# Natural conditional interview flow / 自然條件式訪談流程

Use the user's selected language. The bilingual labels below define equivalent meaning; do not show both languages unless the user asks for bilingual output.

## Core principle / 核心原則

The user should feel that they are having a helpful conversation, not completing a software requirements form. Keep the nine decision areas as an internal completeness check, including the final delivery platform and packaging form. Expose only four simple planning stages and ask one main question at a time. After the five files are delivered, offer the continuation path through GitHub, Codex development, testing, preview, acceptance, authorized release, and value verification without forcing those stages into the initial interview.

## Stage 1: Say the idea / 階段一：說出想法

Start with:

> 你想做一個什麼工具？請像平常聊天一樣告訴我，不完整也沒關係，我會陪你一步一步整理。

> What tool would you like to make? Tell me as you normally would in a chat. It does not need to be complete; I will help you work it out step by step.

From the answer, identify internally:

- who has the problem;
- what is difficult today;
- how it is handled now;
- what better result the user wants.

Do not require all four facts in the first answer. Ask only for the most consequential missing fact next.

## Stage 2: Work it out together / 階段二：一起想清楚

Cover these internal decision areas gradually without naming them:

### Inputs and results / 輸入與結果

Ask what the person will provide first: answer questions, type text, upload a file, select an option, or use existing data. Then ask what useful result the tool should produce.

Request one de-identified real example when it will materially improve the specification. If none exists, offer to define a simple mock example and label it unvalidated. Ask about normal, error, and boundary behavior only when each becomes relevant; do not present them as a four-part form.

### Main use / 主要操作

Reconstruct one primary path internally: enter tool → provide input → process → review → save/export. Describe it back in everyday language and ask whether it matches real life.

### Suggested screens / 建議畫面

When a visual interface is needed, propose three to five simple screens. For each screen, define purpose, fields, actions, and loading/empty/error/success states internally. Show the user only a concise proposal, for example:

> 根據你的使用方式，我建議第一版只有四個畫面：開始頁、旅行問卷、三套方案比較、正式行程。你覺得還缺少哪個必要畫面？

Do not ask the user to choose a framework or design technical states.

### Delivery target / 交付平台

After the main use and intended users are clear, ask where the completed application must run and how the user wants to receive it. Use a short plain-language question such as:

> 這個工具最後要在哪裡使用？例如直接用瀏覽器開啟、Windows 安裝包、Mac App、Ubuntu/Linux、Android 手機或平板、iPhone/iPad，還是需要多平台？如果你不確定，我可以依使用情境建議。

Then confirm the expected artifact only when needed: hosted URL, installer, portable executable, app package, container/service, or source code. Ask about target OS version, device architecture, offline use, signing, store distribution, and installation permissions only when they change feasibility or acceptance.

Never assume Web is the answer. If the target remains undecided, explain that this changes the architecture and cannot be finalized silently.

### Scope / 第一版範圍

Classify requests internally as first version, later, explicitly excluded, or undecided. Keep the first version near three to six modules and one primary success path. If it grows beyond that, recommend a smaller version and explain what will still be useful when it is finished.

## Stage 3: Confirm the first version / 階段三：確認第一版

Present one plain-language blueprint containing:

1. What problem the tool solves and for whom.
2. What the user provides and receives.
3. The first complete end-to-end workflow.
4. The first-version modules.
5. The suggested screens, when applicable.
6. What will wait until later.
7. Where it will run and how it will be delivered or installed.
8. What observable result means the first version works.

Ask for one overall confirmation:

- 對，照這個第一版進行 / Yes, use this first version
- 有一點要修改 / I need to change something
- 我還不確定，請你建議 / I am not sure—please recommend

Do not show a fixed list of confirmed facts, inferences, exclusions, and conflicts when those categories are empty. If there is a real conflict, explain only the competing choices and their practical impact. If a public, sensitive, paid, or irreversible action is involved, ask the necessary human-approval and safety question in ordinary language before approval.

## Stage 4: Create the files / 階段四：產生文件

After the blueprint is approved, complete the following internal work without turning it into another user questionnaire:

### Acceptance / 驗收

Create Given–When–Then cases for every first-version module. Cover normal, error, and boundary behavior. Add authorization, isolation, privacy, recovery, performance, or cost cases only when the project requires them.

### Architecture / 架構

Choose the simplest architecture that satisfies the confirmed use. Infer technical design from user-facing decisions such as:

- only this user versus several people;
- one device versus access from anywhere;
- temporary versus retained data;
- ordinary versus sensitive information;
- suggestion versus automatic or irreversible action;
- target operating system, device type, application form, packaging, distribution, and offline requirements.

Every technical component must solve a confirmed requirement. Keep unsupported commands and environments marked as unconfirmed.

### Implementation handoff / Codex交接

Define the project directory, target platform, expected build artifact, packaging and release phases, smallest vertical slice, candidate build/test/package commands, definition of done, and Codex stop conditions. `START_CODEX.md` must require Codex to inspect and propose a plan before modifying code, then work in recoverable milestones, update `PROJECT_STATUS.md`, run tests, and return preview and acceptance evidence for the user's next EW AI Coding continuation.

### Package and compilation / 文件與一致性

Generate `PRODUCT.md`, `ARCHITECTURE.md`, `ACCEPTANCE.md`, `AGENTS.md`, and `START_CODEX.md` as one package. Run the consistency checks in `SKILL.md` internally. Pause only if a major conflict, missing core example, or product-changing decision prevents a reliable package.

## Conversation examples / 對話表達原則

Prefer:

> 這個工具只有你自己使用，還是也要讓其他人使用？

Avoid:

> 請定義帳號、角色、租戶隔離與驗證架構。

Prefer:

> 使用工具時，你最可能先做什麼：回答問題、輸入文字，還是上傳檔案？如果你不知道，我可以根據你的構想建議。

Avoid:

> 請一次提供輸入、輸出、正常案例、錯誤案例與邊界條件。

Prefer:

> 我目前理解的是：你想讓旅伴填寫需求，產生三套行程，再一起比較和確認。對嗎？

Avoid fixed card summaries and approval forms after every answer.
