# `dialog`

[README](../README.md) › `dialog`

Detect and dismiss Unity Editor popup dialogs

## Subcommands

- [dismiss](#command-dialog-dismiss) — Dismiss a popup dialog by clicking a button
- [list](#command-dialog-list) — List detected popup dialogs

## Options

| Name | Aliases | Value | Required | Recursive | Scope | Group | Description | Arguments |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| --project | — | <PROJECT> | No | No | Declared | — | Path to Unity project root (optional, will auto-detect if not specified) | PROJECT · required · arity 1 |
| --agent-id | — | <AGENT_ID> | No | No | Declared | — | Agent ID for distinguishing multiple agents | AGENT_ID · required · arity 1 |
| --json | — | flag | No | No | Declared | — | Output JSON responses instead of human-readable text | — |
| --timeout | -t | <TIMEOUT> | No | No | Declared | — | Timeout in seconds for commands sent to Unity (overrides the per-command default) | TIMEOUT · required · arity 1 |
| --help | -?, -h | flag | No | No | Declared | — | Show help and usage information | — |

<a id="command-dialog-dismiss"></a>
## `dialog dismiss`

Dismiss a popup dialog by clicking a button

### Options

| Name | Aliases | Value | Required | Recursive | Scope | Group | Description | Arguments |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| --button | — | <BUTTON> | No | No | Declared | — | Button text to click (case-insensitive). If not specified, clicks the first button. | BUTTON · required · arity 1 |
| --project | — | <PROJECT> | No | No | Declared | — | Path to Unity project root (optional, will auto-detect if not specified) | PROJECT · required · arity 1 |
| --agent-id | — | <AGENT_ID> | No | No | Declared | — | Agent ID for distinguishing multiple agents | AGENT_ID · required · arity 1 |
| --json | — | flag | No | No | Declared | — | Output JSON responses instead of human-readable text | — |
| --timeout | -t | <TIMEOUT> | No | No | Declared | — | Timeout in seconds for commands sent to Unity (overrides the per-command default) | TIMEOUT · required · arity 1 |
| --help | -?, -h | flag | No | No | Declared | — | Show help and usage information | — |

<a id="command-dialog-list"></a>
## `dialog list`

List detected popup dialogs

### Options

| Name | Aliases | Value | Required | Recursive | Scope | Group | Description | Arguments |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| --project | — | <PROJECT> | No | No | Declared | — | Path to Unity project root (optional, will auto-detect if not specified) | PROJECT · required · arity 1 |
| --agent-id | — | <AGENT_ID> | No | No | Declared | — | Agent ID for distinguishing multiple agents | AGENT_ID · required · arity 1 |
| --json | — | flag | No | No | Declared | — | Output JSON responses instead of human-readable text | — |
| --timeout | -t | <TIMEOUT> | No | No | Declared | — | Timeout in seconds for commands sent to Unity (overrides the per-command default) | TIMEOUT · required · arity 1 |
| --help | -?, -h | flag | No | No | Declared | — | Show help and usage information | — |
