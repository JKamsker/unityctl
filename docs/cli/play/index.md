# `play`

[README](../README.md) › `play`

Play mode operations

## Subcommands

- [enter](#command-play-enter) — Enter play mode
- [exit](#command-play-exit) — Exit play mode
- [pause](#command-play-pause) — Pause or unpause play mode (toggle)
- [status](#command-play-status) — Get play mode status
- [step](#command-play-step) — Advance one frame (while paused)

## Options

| Name | Aliases | Value | Required | Recursive | Scope | Group | Description | Arguments |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| --project | — | <PROJECT> | No | No | Declared | — | Path to Unity project root (optional, will auto-detect if not specified) | PROJECT · required · arity 1 |
| --agent-id | — | <AGENT_ID> | No | No | Declared | — | Agent ID for distinguishing multiple agents | AGENT_ID · required · arity 1 |
| --json | — | flag | No | No | Declared | — | Output JSON responses instead of human-readable text | — |
| --timeout | -t | <TIMEOUT> | No | No | Declared | — | Timeout in seconds for commands sent to Unity (overrides the per-command default) | TIMEOUT · required · arity 1 |
| --help | -?, -h | flag | No | No | Declared | — | Show help and usage information | — |

<a id="command-play-enter"></a>
## `play enter`

Enter play mode

### Options

| Name | Aliases | Value | Required | Recursive | Scope | Group | Description | Arguments |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| --project | — | <PROJECT> | No | No | Declared | — | Path to Unity project root (optional, will auto-detect if not specified) | PROJECT · required · arity 1 |
| --agent-id | — | <AGENT_ID> | No | No | Declared | — | Agent ID for distinguishing multiple agents | AGENT_ID · required · arity 1 |
| --json | — | flag | No | No | Declared | — | Output JSON responses instead of human-readable text | — |
| --timeout | -t | <TIMEOUT> | No | No | Declared | — | Timeout in seconds for commands sent to Unity (overrides the per-command default) | TIMEOUT · required · arity 1 |
| --help | -?, -h | flag | No | No | Declared | — | Show help and usage information | — |

<a id="command-play-exit"></a>
## `play exit`

Exit play mode

### Options

| Name | Aliases | Value | Required | Recursive | Scope | Group | Description | Arguments |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| --project | — | <PROJECT> | No | No | Declared | — | Path to Unity project root (optional, will auto-detect if not specified) | PROJECT · required · arity 1 |
| --agent-id | — | <AGENT_ID> | No | No | Declared | — | Agent ID for distinguishing multiple agents | AGENT_ID · required · arity 1 |
| --json | — | flag | No | No | Declared | — | Output JSON responses instead of human-readable text | — |
| --timeout | -t | <TIMEOUT> | No | No | Declared | — | Timeout in seconds for commands sent to Unity (overrides the per-command default) | TIMEOUT · required · arity 1 |
| --help | -?, -h | flag | No | No | Declared | — | Show help and usage information | — |

<a id="command-play-pause"></a>
## `play pause`

Pause or unpause play mode (toggle)

### Options

| Name | Aliases | Value | Required | Recursive | Scope | Group | Description | Arguments |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| --project | — | <PROJECT> | No | No | Declared | — | Path to Unity project root (optional, will auto-detect if not specified) | PROJECT · required · arity 1 |
| --agent-id | — | <AGENT_ID> | No | No | Declared | — | Agent ID for distinguishing multiple agents | AGENT_ID · required · arity 1 |
| --json | — | flag | No | No | Declared | — | Output JSON responses instead of human-readable text | — |
| --timeout | -t | <TIMEOUT> | No | No | Declared | — | Timeout in seconds for commands sent to Unity (overrides the per-command default) | TIMEOUT · required · arity 1 |
| --help | -?, -h | flag | No | No | Declared | — | Show help and usage information | — |

<a id="command-play-status"></a>
## `play status`

Get play mode status

### Options

| Name | Aliases | Value | Required | Recursive | Scope | Group | Description | Arguments |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| --project | — | <PROJECT> | No | No | Declared | — | Path to Unity project root (optional, will auto-detect if not specified) | PROJECT · required · arity 1 |
| --agent-id | — | <AGENT_ID> | No | No | Declared | — | Agent ID for distinguishing multiple agents | AGENT_ID · required · arity 1 |
| --json | — | flag | No | No | Declared | — | Output JSON responses instead of human-readable text | — |
| --timeout | -t | <TIMEOUT> | No | No | Declared | — | Timeout in seconds for commands sent to Unity (overrides the per-command default) | TIMEOUT · required · arity 1 |
| --help | -?, -h | flag | No | No | Declared | — | Show help and usage information | — |

<a id="command-play-step"></a>
## `play step`

Advance one frame (while paused)

### Options

| Name | Aliases | Value | Required | Recursive | Scope | Group | Description | Arguments |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| --project | — | <PROJECT> | No | No | Declared | — | Path to Unity project root (optional, will auto-detect if not specified) | PROJECT · required · arity 1 |
| --agent-id | — | <AGENT_ID> | No | No | Declared | — | Agent ID for distinguishing multiple agents | AGENT_ID · required · arity 1 |
| --json | — | flag | No | No | Declared | — | Output JSON responses instead of human-readable text | — |
| --timeout | -t | <TIMEOUT> | No | No | Declared | — | Timeout in seconds for commands sent to Unity (overrides the per-command default) | TIMEOUT · required · arity 1 |
| --help | -?, -h | flag | No | No | Declared | — | Show help and usage information | — |
