# Local Engineering / 本機工程

## Purpose / 目的

Use this workflow only when the requested application must interact with a local machine or edge device by installing software, generating local configuration, running services, creating adapters, integrating device data, or validating a local deployment.

Do not expose Local Engineering as a required mode to ordinary users. Detect it from the user's actual goal and route internally.

本流程只在應用需要操作本機、邊緣設備、安裝軟體、建立設定、執行服務、產生介接程式、整合設備資料或驗證本機部署時啟用。不要要求一般使用者先選「工程模式」。

## Entry conditions / 啟動條件

Route here when one or more are true:

- target runs on Windows, macOS, Ubuntu/Linux, IPC, edge computer, or on-premises server;
- implementation requires install, configure, start, stop, restart, or inspect a local service;
- implementation needs local files, logs, ports, environment variables, packages, daemons, containers, or device interfaces;
- implementation requires a protocol adapter, local API connector, data collector, or device integration;
- the user explicitly asks to deploy, install, connect, configure, test, repair, migrate, or verify a local system.

Do not route here merely because the final app is installable. Use this workflow only when local execution or environment-specific deployment materially affects correctness.

## User experience / 使用者體驗

Keep the visible interaction simple. The user should be able to say what they want in ordinary language.

Internally determine:

1. target machine and operating system;
2. existing software and project state;
3. required local capability;
4. dependencies and privileges;
5. reversible vs irreversible changes;
6. validation evidence;
7. rollback path.

Never assume a clean machine. Inspect or ask about existing state before proposing replacement.

## Workflow / 工作流程

### Phase A — Inspect and plan / 檢視與規劃

- Identify the target environment only to the level required.
- Reuse existing code, configuration, services, folders, and ports where possible.
- If the user provides an existing repository, project folder, ZIP, log, or screenshot, inspect it before proposing changes.
- Record unknown environment facts explicitly instead of inventing them.
- Separate application logic from machine-specific deployment logic.

### Phase B — Generate / 生成

Generate a structured Deployment Package rather than isolated commands whenever the task changes a local environment.

The package should include:
- manifest;
- human-readable README;
- install or apply steps;
- configuration;
- verification;
- rollback;
- evidence/result template.

Follow `deployment-package.md`.

### Phase C — Execute / 執行

If no local execution tool is available:
- clearly state that the package or commands are prepared but not executed;
- guide the user to run the smallest safe step;
- ask for the returned output or log only when it materially affects the next step;
- never claim installation, service start, file modification, or test success without evidence.

If an authorized local runtime or MCP tool becomes available in the future:
- use it only after the planned changes are explicit;
- prefer atomic, inspectable operations;
- require confirmation before destructive, privileged, irreversible, credential-related, network-exposure, or production-impacting actions;
- preserve evidence of what was changed and the result.

### Phase D — Verify / 驗證

Verification must test the intended outcome, not merely command completion.

Examples:
- process/service is actually running;
- required port is listening;
- expected file exists with expected structure;
- target API responds;
- device connection succeeds;
- expected data is arriving;
- timestamps and units are plausible;
- application survives restart when persistence is required.

Record failed checks rather than masking them.

### Phase E — Rollback / 回復

For any meaningful system change, define how to return to the previous known state.

Rollback should cover, when relevant:
- restore previous config;
- stop and remove newly added service;
- uninstall or disable newly added package;
- restore previous file;
- remove newly created scheduled job;
- revert environment variable or port exposure.

A rollback plan is not proof that rollback was executed.

## Protocol and device handoff / 協議與設備交接

EW AI Coding is not the authoritative protocol-document interpreter when a dedicated protocol mapping workflow is available.

When a structured protocol specification is supplied by a protocol-mapping tool, treat it as an input contract. Do not silently reinterpret addresses, data types, byte order, scale, unit, polling interval, or write permissions.

Recommended handoff artifact:

`protocol-spec.json`

Minimum useful fields may include:
- protocol;
- device identity;
- connection parameters;
- register or point mapping;
- data type;
- byte/word order;
- scale;
- unit;
- polling interval;
- read/write permission;
- source evidence or unresolved fields.

EW AI Coding then turns that specification into implementation and deployment artifacts.

## Boundary / 邊界

Local Engineering extends EW AI Coding; it does not redefine the product.

Ordinary users should still experience:
idea → clarification → specification → Codex → test → acceptance.

Only local/edge projects additionally use:
environment → deployment package → execute → verify → rollback.
