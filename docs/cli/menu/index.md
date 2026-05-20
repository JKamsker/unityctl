# `menu`

[README](../README.md) › `menu`

Unity menu operations

## Subcommands

- [execute](#command-menu-execute) — Execute a Unity menu item
- [list](#command-menu-list) — List all available Unity menu items

## Options

| Name | Aliases | Value | Required | Recursive | Scope | Group | Description | Arguments |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| --project | — | <PROJECT> | No | No | Declared | — | Path to Unity project root (optional, will auto-detect if not specified) | PROJECT · required · arity 1 |
| --agent-id | — | <AGENT_ID> | No | No | Declared | — | Agent ID for distinguishing multiple agents | AGENT_ID · required · arity 1 |
| --json | — | flag | No | No | Declared | — | Output JSON responses instead of human-readable text | — |
| --timeout | -t | <TIMEOUT> | No | No | Declared | — | Timeout in seconds for commands sent to Unity (overrides the per-command default) | TIMEOUT · required · arity 1 |
| --help | -?, -h | flag | No | No | Declared | — | Show help and usage information | — |

<a id="command-menu-execute"></a>
## `menu execute`

Execute a Unity menu item

### Arguments

| Name | Required | Arity | Accepted Values | Group | Description |
| --- | --- | --- | --- | --- | --- |
| PATH | Yes | 1 | — | — | Menu item path (e.g., "File/Save" or "Assets/Refresh") |

### Options

| Name | Aliases | Value | Required | Recursive | Scope | Group | Description | Arguments |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| --project | — | <PROJECT> | No | No | Declared | — | Path to Unity project root (optional, will auto-detect if not specified) | PROJECT · required · arity 1 |
| --agent-id | — | <AGENT_ID> | No | No | Declared | — | Agent ID for distinguishing multiple agents | AGENT_ID · required · arity 1 |
| --json | — | flag | No | No | Declared | — | Output JSON responses instead of human-readable text | — |
| --timeout | -t | <TIMEOUT> | No | No | Declared | — | Timeout in seconds for commands sent to Unity (overrides the per-command default) | TIMEOUT · required · arity 1 |
| --help | -?, -h | flag | No | No | Declared | — | Show help and usage information | — |

<a id="command-menu-list"></a>
## `menu list`

List all available Unity menu items

### Options

| Name | Aliases | Value | Required | Recursive | Scope | Group | Description | Arguments |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| --project | — | <PROJECT> | No | No | Declared | — | Path to Unity project root (optional, will auto-detect if not specified) | PROJECT · required · arity 1 |
| --agent-id | — | <AGENT_ID> | No | No | Declared | — | Agent ID for distinguishing multiple agents | AGENT_ID · required · arity 1 |
| --json | — | flag | No | No | Declared | — | Output JSON responses instead of human-readable text | — |
| --timeout | -t | <TIMEOUT> | No | No | Declared | — | Timeout in seconds for commands sent to Unity (overrides the per-command default) | TIMEOUT · required · arity 1 |
| --help | -?, -h | flag | No | No | Declared | — | Show help and usage information | — |
