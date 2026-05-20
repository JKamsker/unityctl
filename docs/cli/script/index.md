# `script`

[README](../README.md) › `script`

C# script execution operations

## Subcommands

- [eval](#command-script-eval) — Evaluate a C# expression in the Unity Editor
- [execute](#command-script-execute) — Execute C# code in the Unity Editor
- [lookup-type](#command-script-lookup-type) — Find loaded types by short name (returns FullName, namespace, assembly)
- [members](#command-script-members) — List public members of a type (properties, methods, fields, events)

## Options

| Name | Aliases | Value | Required | Recursive | Scope | Group | Description | Arguments |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| --project | — | <PROJECT> | No | No | Declared | — | Path to Unity project root (optional, will auto-detect if not specified) | PROJECT · required · arity 1 |
| --agent-id | — | <AGENT_ID> | No | No | Declared | — | Agent ID for distinguishing multiple agents | AGENT_ID · required · arity 1 |
| --json | — | flag | No | No | Declared | — | Output JSON responses instead of human-readable text | — |
| --timeout | -t | <TIMEOUT> | No | No | Declared | — | Timeout in seconds for commands sent to Unity (overrides the per-command default) | TIMEOUT · required · arity 1 |
| --help | -?, -h | flag | No | No | Declared | — | Show help and usage information | — |

<a id="command-script-eval"></a>
## `script eval`

Evaluate a C# expression in the Unity Editor

### Arguments

| Name | Required | Arity | Accepted Values | Group | Description |
| --- | --- | --- | --- | --- | --- |
| EXPRESSION | No | 0..1 | — | — | C# expression or method body to evaluate [] |
| SCRIPT_ARGS | No | 0..1 | — | — | Arguments to pass to Main (after --) [] |

### Options

| Name | Aliases | Value | Required | Recursive | Scope | Group | Description | Arguments |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| --using | -u | <USING> | No | No | Declared | — | Additional using directives (e.g., UnityEngine.UI) [] | USING · required · arity 1 |
| --id | — | <ID> | No | No | Declared | — | Target object by instance ID (from snapshot). Injects 'target'. Comma-separated IDs inject 'targets[]' array. | ID · required · arity 1 |
| --project | — | <PROJECT> | No | No | Declared | — | Path to Unity project root (optional, will auto-detect if not specified) | PROJECT · required · arity 1 |
| --agent-id | — | <AGENT_ID> | No | No | Declared | — | Agent ID for distinguishing multiple agents | AGENT_ID · required · arity 1 |
| --json | — | flag | No | No | Declared | — | Output JSON responses instead of human-readable text | — |
| --timeout | -t | <TIMEOUT> | No | No | Declared | — | Timeout in seconds for commands sent to Unity (overrides the per-command default) | TIMEOUT · required · arity 1 |
| --help | -?, -h | flag | No | No | Declared | — | Show help and usage information | — |

<a id="command-script-execute"></a>
## `script execute`

Execute C# code in the Unity Editor

### Arguments

| Name | Required | Arity | Accepted Values | Group | Description |
| --- | --- | --- | --- | --- | --- |
| SCRIPT_ARGS | No | 0..1 | — | — | Arguments to pass to the script's Main method (after --) [] |

### Options

| Name | Aliases | Value | Required | Recursive | Scope | Group | Description | Arguments |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| --file | -f | <FILE> | No | No | Declared | — | Read C# code from a file | FILE · required · arity 1 |
| --class | — | <CLASS> | No | No | Declared | — | Name of the class containing the method to execute [default: Script] | CLASS · required · arity 1 |
| --method | — | <METHOD> | No | No | Declared | — | Name of the static method to execute [default: Main] | METHOD · required · arity 1 |
| --project | — | <PROJECT> | No | No | Declared | — | Path to Unity project root (optional, will auto-detect if not specified) | PROJECT · required · arity 1 |
| --agent-id | — | <AGENT_ID> | No | No | Declared | — | Agent ID for distinguishing multiple agents | AGENT_ID · required · arity 1 |
| --json | — | flag | No | No | Declared | — | Output JSON responses instead of human-readable text | — |
| --timeout | -t | <TIMEOUT> | No | No | Declared | — | Timeout in seconds for commands sent to Unity (overrides the per-command default) | TIMEOUT · required · arity 1 |
| --help | -?, -h | flag | No | No | Declared | — | Show help and usage information | — |

<a id="command-script-lookup-type"></a>
## `script lookup-type`

Find loaded types by short name (returns FullName, namespace, assembly)

### Arguments

| Name | Required | Arity | Accepted Values | Group | Description |
| --- | --- | --- | --- | --- | --- |
| NAME | No | 0..1 | — | — | Short or partial type name (e.g. 'Storage', 'ClanFeedOSA') |

### Options

| Name | Aliases | Value | Required | Recursive | Scope | Group | Description | Arguments |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| --limit | -n | <LIMIT> | No | No | Declared | — | Maximum matches to return (1–100) [default: 10] | LIMIT · required · arity 1 |
| --project | — | <PROJECT> | No | No | Declared | — | Path to Unity project root (optional, will auto-detect if not specified) | PROJECT · required · arity 1 |
| --agent-id | — | <AGENT_ID> | No | No | Declared | — | Agent ID for distinguishing multiple agents | AGENT_ID · required · arity 1 |
| --json | — | flag | No | No | Declared | — | Output JSON responses instead of human-readable text | — |
| --timeout | -t | <TIMEOUT> | No | No | Declared | — | Timeout in seconds for commands sent to Unity (overrides the per-command default) | TIMEOUT · required · arity 1 |
| --help | -?, -h | flag | No | No | Declared | — | Show help and usage information | — |

<a id="command-script-members"></a>
## `script members`

List public members of a type (properties, methods, fields, events)

### Arguments

| Name | Required | Arity | Accepted Values | Group | Description |
| --- | --- | --- | --- | --- | --- |
| TYPE | Yes | 1 | — | — | Type name — short (e.g. 'Transform') or fully-qualified ('UnityEngine.Transform') |

### Options

| Name | Aliases | Value | Required | Recursive | Scope | Group | Description | Arguments |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| --filter | -f | <FILTER> | No | No | Declared | — | Case-insensitive substring filter on member names | FILTER · required · arity 1 |
| --static | -s | flag | No | No | Declared | — | Only static members | — |
| --limit | -n | <LIMIT> | No | No | Declared | — | Maximum members to return (1–500) [default: 50] | LIMIT · required · arity 1 |
| --project | — | <PROJECT> | No | No | Declared | — | Path to Unity project root (optional, will auto-detect if not specified) | PROJECT · required · arity 1 |
| --agent-id | — | <AGENT_ID> | No | No | Declared | — | Agent ID for distinguishing multiple agents | AGENT_ID · required · arity 1 |
| --json | — | flag | No | No | Declared | — | Output JSON responses instead of human-readable text | — |
| --timeout | -t | <TIMEOUT> | No | No | Declared | — | Timeout in seconds for commands sent to Unity (overrides the per-command default) | TIMEOUT · required · arity 1 |
| --help | -?, -h | flag | No | No | Declared | — | Show help and usage information | — |
