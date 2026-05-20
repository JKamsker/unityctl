# `record`

[README](../README.md) › `record`

Video recording operations (requires Unity Recorder package)

## Subcommands

- [start](#command-record-start) — Start recording video of the game view
- [status](#command-record-status) — Get current recording status
- [stop](#command-record-stop) — Stop the current recording

## Options

| Name | Aliases | Value | Required | Recursive | Scope | Group | Description | Arguments |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| --project | — | <PROJECT> | No | No | Declared | — | Path to Unity project root (optional, will auto-detect if not specified) | PROJECT · required · arity 1 |
| --agent-id | — | <AGENT_ID> | No | No | Declared | — | Agent ID for distinguishing multiple agents | AGENT_ID · required · arity 1 |
| --json | — | flag | No | No | Declared | — | Output JSON responses instead of human-readable text | — |
| --timeout | -t | <TIMEOUT> | No | No | Declared | — | Timeout in seconds for commands sent to Unity (overrides the per-command default) | TIMEOUT · required · arity 1 |
| --help | -?, -h | flag | No | No | Declared | — | Show help and usage information | — |

<a id="command-record-start"></a>
## `record start`

Start recording video of the game view

<a id="command-record-status"></a>
## `record status`

Get current recording status

<a id="command-record-stop"></a>
## `record stop`

Stop the current recording
