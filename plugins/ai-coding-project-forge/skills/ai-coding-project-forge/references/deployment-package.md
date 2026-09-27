# EW Deployment Package / EW 部署工作包

## Purpose / 目的

Use a Deployment Package when AI Coding produces changes that must be applied to a local machine, IPC, edge computer, server, or device-facing software environment.

The package is a stable handoff between planning and execution. It works today with manual execution and can later be consumed by an authorized local runtime or MCP server without changing the higher-level workflow.

## Recommended structure / 建議結構

```text
EW-DEPLOY-<task-id>/
├── manifest.json
├── README.md
├── install/
│   └── apply.*
├── config/
├── verify/
│   └── verify.*
├── rollback/
│   └── rollback.*
└── evidence/
    └── result.md
```

Use platform-appropriate extensions such as `.sh`, `.ps1`, `.py`, `.json`, `.yaml`, or service definitions.

Do not create empty folders merely to satisfy the structure. Include only what the deployment requires.

## manifest.json

The manifest is the machine-readable plan. It should describe intent, not hide logic.

Recommended fields:

```json
{
  "schema_version": "1.0",
  "task_id": "EW-DEPLOY-000001",
  "objective": "Describe the intended deployed capability",
  "target": {
    "os": "ubuntu",
    "architecture": "x86_64",
    "environment": "local"
  },
  "preconditions": [],
  "inputs": [],
  "changes": [],
  "verification": [],
  "rollback_available": true,
  "requires_privilege": false,
  "requires_network_exposure": false,
  "requires_secret": false,
  "status": "prepared"
}
```

Unknown values must remain unknown or omitted. Do not fabricate hostnames, ports, credentials, paths, versions, or device addresses.

## README.md

Explain in plain language:
- what this package changes;
- what it does not change;
- prerequisites;
- how to preview or inspect changes;
- how to apply;
- what successful verification looks like;
- how to rollback;
- which steps require confirmation.

A non-programmer should be able to understand the risk before execution.

## Apply / 安裝或套用

The apply step should:
- fail visibly on errors;
- avoid destructive defaults;
- be idempotent where practical;
- preserve or back up existing configuration before replacement;
- log meaningful actions;
- avoid embedding secrets;
- not expose services publicly unless explicitly required and authorized.

Prefer small, composable steps over a large opaque installer.

## Verification / 驗證

Verification is mandatory for any deployment that claims success.

Checks should be tied to acceptance evidence, for example:
- package installed;
- service active;
- endpoint reachable;
- configuration loaded;
- device connection established;
- expected record written;
- expected data observed;
- restart persistence confirmed.

Do not equate exit code 0 with business success.

## Rollback / 回復

Rollback should be included whenever the package changes a persistent system state.

A good rollback:
- restores the last known configuration;
- disables newly created services;
- removes only artifacts created by this deployment;
- avoids deleting user data;
- reports what was restored and what remains.

## Evidence / 證據

`evidence/result.md` should record:
- execution date/time if known;
- target environment;
- package/task ID;
- commands or actions actually executed;
- verification results;
- failures or warnings;
- rollback state;
- unresolved follow-up.

Prepared files are not evidence of execution.

## Status model / 狀態模型

Use explicit states:
- `prepared` — package generated, not executed;
- `approved` — user/authorized operator approved execution;
- `executing`;
- `verification_failed`;
- `verified`;
- `rollback_required`;
- `rolled_back`.

Never mark `verified` without real verification evidence.

## Future runtime compatibility / 未來 Runtime 相容性

A future EW Local Runtime or MCP server should consume the same package model instead of embedding domain-specific deployment knowledge into MCP tools.

Runtime responsibilities:
- inspect environment;
- receive package;
- request required authorization;
- execute approved package;
- stream logs/status;
- run verification;
- execute rollback when authorized.

Domain knowledge remains in Skills and generated artifacts; runtime remains a narrow execution layer.
