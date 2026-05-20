# `logs`

[README](../README.md) › `logs`

View Unity console logs

## Subcommands

- [clear](#command-logs-clear) — Clear log history (set watermark)

## Options

| Name | Aliases | Value | Required | Recursive | Scope | Group | Description | Arguments |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| --follow | -f | flag | No | No | Declared | — | Follow log output (stream continuously) | — |
| --count | -n, --last, --lines | <LINES> | No | No | Declared | — | Limit to N most recent lines (default: all since last clear) | LINES · optional · arity 0..1 |
| --no-color | — | flag | No | No | Declared | — | Disable colored output | — |
| --verbose | — | flag | No | No | Declared | — | Show all fields including timestamps | — |
| --full | — | flag | No | No | Declared | — | Show full log history (ignore clear watermark) | — |
| --stack | — | flag | No | No | Declared | — | Show stack traces for log entries | — |
| --level | -l | <LEVEL> | No | No | Declared | — | Minimum log level: log, warning, error (default: all) | LEVEL · optional · arity 0..1 |
| --project | — | <PROJECT> | No | No | Declared | — | Path to Unity project root (optional, will auto-detect if not specified) | PROJECT · required · arity 1 |
| --agent-id | — | <AGENT_ID> | No | No | Declared | — | Agent ID for distinguishing multiple agents | AGENT_ID · required · arity 1 |
| --json | — | flag | No | No | Declared | — | Output JSON responses instead of human-readable text | — |
| --timeout | -t | <TIMEOUT> | No | No | Declared | — | Timeout in seconds for commands sent to Unity (overrides the per-command default) | TIMEOUT · required · arity 1 |
| --help | -?, -h | flag | No | No | Declared | — | Show help and usage information | — |

<a id="command-logs-clear"></a>
## `logs clear`

Clear log history (set watermark)

### Options

| Name | Aliases | Value | Required | Recursive | Scope | Group | Description | Arguments |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| --project | — | <PROJECT> | No | No | Declared | — | Path to Unity project root (optional, will auto-detect if not specified) | PROJECT · required · arity 1 |
| --agent-id | — | <AGENT_ID> | No | No | Declared | — | Agent ID for distinguishing multiple agents | AGENT_ID · required · arity 1 |
| --json | — | flag | No | No | Declared | — | Output JSON responses instead of human-readable text | — |
| --timeout | -t | <TIMEOUT> | No | No | Declared | — | Timeout in seconds for commands sent to Unity (overrides the per-command default) | TIMEOUT · required · arity 1 |
| --help | -?, -h | flag | No | No | Declared | — | Show help and usage information | — |
