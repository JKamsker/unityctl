# `snapshot`

[README](../README.md) › `snapshot`

Snapshot the scene hierarchy as a compact, LLM-friendly tree with instance IDs

## Subcommands

- [query](#command-snapshot-query) — Hit-test at screen coordinates — what's at this pixel?

## Options

| Name | Aliases | Value | Required | Recursive | Scope | Group | Description | Arguments |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| --id | — | <ID> | No | No | Declared | — | Drill into a specific object by instance ID | ID · required · arity 1 |
| --depth | — | <DEPTH> | No | No | Declared | — | Max hierarchy depth (default: 2) | DEPTH · optional · arity 0..1 |
| --components | — | flag | No | No | Declared | — | Include all serialized property values | — |
| --screen | — | flag | No | No | Declared | — | Include screen-space bounds, visibility, and hittability | — |
| --filter | — | <FILTER> | No | No | Declared | — | Filter by type:T, name:N*, or tag:T | FILTER · required · arity 1 |
| --scene | — | <SCENE> | No | No | Declared | — | Snapshot a specific scene (opens additively if not loaded) | SCENE · required · arity 1 |
| --prefab | — | <PREFAB> | No | No | Declared | — | Snapshot a prefab asset | PREFAB · required · arity 1 |
| --project | — | <PROJECT> | No | No | Declared | — | Path to Unity project root (optional, will auto-detect if not specified) | PROJECT · required · arity 1 |
| --agent-id | — | <AGENT_ID> | No | No | Declared | — | Agent ID for distinguishing multiple agents | AGENT_ID · required · arity 1 |
| --json | — | flag | No | No | Declared | — | Output JSON responses instead of human-readable text | — |
| --timeout | -t | <TIMEOUT> | No | No | Declared | — | Timeout in seconds for commands sent to Unity (overrides the per-command default) | TIMEOUT · required · arity 1 |
| --help | -?, -h | flag | No | No | Declared | — | Show help and usage information | — |

<a id="command-snapshot-query"></a>
## `snapshot query`

Hit-test at screen coordinates — what's at this pixel?

### Arguments

| Name | Required | Arity | Accepted Values | Group | Description |
| --- | --- | --- | --- | --- | --- |
| X | Yes | 1 | — | — | Screen X coordinate |
| Y | Yes | 1 | — | — | Screen Y coordinate |

### Options

| Name | Aliases | Value | Required | Recursive | Scope | Group | Description | Arguments |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| --project | — | <PROJECT> | No | No | Declared | — | Path to Unity project root (optional, will auto-detect if not specified) | PROJECT · required · arity 1 |
| --agent-id | — | <AGENT_ID> | No | No | Declared | — | Agent ID for distinguishing multiple agents | AGENT_ID · required · arity 1 |
| --json | — | flag | No | No | Declared | — | Output JSON responses instead of human-readable text | — |
| --timeout | -t | <TIMEOUT> | No | No | Declared | — | Timeout in seconds for commands sent to Unity (overrides the per-command default) | TIMEOUT · required · arity 1 |
| --help | -?, -h | flag | No | No | Declared | — | Show help and usage information | — |
