# unityctl CLI

- Version: generated from source
- OpenCLI: `0.1-draft`

Command-line reference for `unityctl CLI`. Available command areas include play, config, package, script, skill, bridge, and more.

UnityCtl - CLI tool for controlling Unity Editor

<a id="overview"></a>
## Overview

### CLI Scope

- Top-level command groups: `25`
- Documented commands: `75`
- Leaf commands: `55`

### Available Commands

- [assets](assets/index.md) — Asset management operations
- [bridge](bridge/index.md) — Bridge management operations
- [config](config/index.md) — Configuration management
- [dialog](dialog/index.md) — Detect and dismiss Unity Editor popup dialogs
- [editor](editor/index.md) — Unity Editor operations
- [logs](logs/index.md) — View Unity console logs
- [menu](menu/index.md) — Unity menu operations
- [package](package/index.md) — Unity package management
- [play](play/index.md) — Play mode operations
- [plugin](plugin/index.md) — Plugin management
- [prefab](prefab/index.md) — Prefab stage navigation
- [record](record/index.md) — Video recording operations (requires Unity Recorder package)
- [sample-exec](#command-sample-exec) — Executable plugin: sample-exec
- [sample-script](sample-script/index.md) — Sample script plugin demonstrating the plugin system
- [scene](scene/index.md) — Scene management operations
- [screenshot](screenshot/index.md) — Screenshot operations
- [script](script/index.md) — C# script execution operations
- [setup](#command-setup) — Set up unityctl for a Unity project (config + package + skill)
- [skill](skill/index.md) — Claude Code skill management
- [snapshot](snapshot/index.md) — Snapshot the scene hierarchy as a compact, LLM-friendly tree with instance IDs
- [status](#command-status) — Show project status including Unity Editor and bridge state
- [test](test/index.md) — Unity test runner operations
- [ui](ui/index.md) — UI interaction commands (play mode)
- [update](#command-update) — Update UnityCtl CLI, bridge, and Unity package
- [wait](#command-wait) — Wait until Unity Editor is connected and ready to accept commands


## Root Options

| Name | Aliases | Value | Required | Recursive | Scope | Group | Description | Arguments |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| --project | — | <PROJECT> | No | No | Declared | — | Path to Unity project root (optional, will auto-detect if not specified) | PROJECT · required · arity 1 |
| --agent-id | — | <AGENT_ID> | No | No | Declared | — | Agent ID for distinguishing multiple agents | AGENT_ID · required · arity 1 |
| --json | — | flag | No | No | Declared | — | Output JSON responses instead of human-readable text | — |
| --timeout | -t | <TIMEOUT> | No | No | Declared | — | Timeout in seconds for commands sent to Unity (overrides the per-command default) | TIMEOUT · required · arity 1 |
| --version | — | flag | No | No | Declared | — | Show version information | — |
| --help | -?, -h | flag | No | No | Declared | — | Show help and usage information | — |


## Commands

<a id="command-sample-exec"></a>
### `sample-exec`

Executable plugin: sample-exec

#### Arguments

| Name | Required | Arity | Accepted Values | Group | Description |
| --- | --- | --- | --- | --- | --- |
| ARGS | No | 0..1 | — | — | Arguments to pass to the plugin executable |

#### Options

| Name | Aliases | Value | Required | Recursive | Scope | Group | Description | Arguments |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| --project | — | <PROJECT> | No | No | Declared | — | Path to Unity project root (optional, will auto-detect if not specified) | PROJECT · required · arity 1 |
| --agent-id | — | <AGENT_ID> | No | No | Declared | — | Agent ID for distinguishing multiple agents | AGENT_ID · required · arity 1 |
| --json | — | flag | No | No | Declared | — | Output JSON responses instead of human-readable text | — |
| --timeout | -t | <TIMEOUT> | No | No | Declared | — | Timeout in seconds for commands sent to Unity (overrides the per-command default) | TIMEOUT · required · arity 1 |
| --help | -?, -h | flag | No | No | Declared | — | Show help and usage information | — |

<a id="command-setup"></a>
### `setup`

Set up unityctl for a Unity project (config + package + skill)

#### Options

| Name | Aliases | Value | Required | Recursive | Scope | Group | Description | Arguments |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| --method | -m | <METHOD> | No | No | Declared | — | Package installation method: upm (git URL) or local (file path) [default: upm] | METHOD · required · arity 1 |
| --skip-package | — | flag | No | No | Declared | — | Skip Unity package installation | — |
| --skip-skill | — | flag | No | No | Declared | — | Skip Claude Code skill installation | — |
| --global-skill | — | flag | No | No | Declared | — | Install skill globally (~/.claude/skills/) instead of locally | — |
| --yes | -y | flag | No | No | Declared | — | Skip confirmation prompts (non-interactive mode) | — |
| --project | — | <PROJECT> | No | No | Declared | — | Path to Unity project root (optional, will auto-detect if not specified) | PROJECT · required · arity 1 |
| --agent-id | — | <AGENT_ID> | No | No | Declared | — | Agent ID for distinguishing multiple agents | AGENT_ID · required · arity 1 |
| --json | — | flag | No | No | Declared | — | Output JSON responses instead of human-readable text | — |
| --timeout | -t | <TIMEOUT> | No | No | Declared | — | Timeout in seconds for commands sent to Unity (overrides the per-command default) | TIMEOUT · required · arity 1 |
| --help | -?, -h | flag | No | No | Declared | — | Show help and usage information | — |

<a id="command-status"></a>
### `status`

Show project status including Unity Editor and bridge state

#### Options

| Name | Aliases | Value | Required | Recursive | Scope | Group | Description | Arguments |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| --project | — | <PROJECT> | No | No | Declared | — | Path to Unity project root (optional, will auto-detect if not specified) | PROJECT · required · arity 1 |
| --agent-id | — | <AGENT_ID> | No | No | Declared | — | Agent ID for distinguishing multiple agents | AGENT_ID · required · arity 1 |
| --json | — | flag | No | No | Declared | — | Output JSON responses instead of human-readable text | — |
| --timeout | -t | <TIMEOUT> | No | No | Declared | — | Timeout in seconds for commands sent to Unity (overrides the per-command default) | TIMEOUT · required · arity 1 |
| --help | -?, -h | flag | No | No | Declared | — | Show help and usage information | — |

<a id="command-update"></a>
### `update`

Update UnityCtl CLI, bridge, and Unity package

#### Options

| Name | Aliases | Value | Required | Recursive | Scope | Group | Description | Arguments |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| --check | — | flag | No | No | Declared | — | Check for updates without installing | — |
| --tools-only | — | <TOOLS_ONLY> | No | No | Declared | — | Only update CLI and Bridge tools (skip Unity package and skill) | TOOLS_ONLY · optional · arity 0..1 |
| --package-only | — | <PACKAGE_ONLY> | No | No | Declared | — | Only update Unity package (skip CLI and Bridge tools) | PACKAGE_ONLY · optional · arity 0..1 |
| --version | -v | <VERSION> | No | No | Declared | — | Specific version to update to (default: latest) | VERSION · optional · arity 0..1 |
| --yes | -y | flag | No | No | Declared | — | Skip confirmation prompts | — |
| --skip-skill | — | flag | No | No | Declared | — | Skip Claude Code skill update | — |
| --project | — | <PROJECT> | No | No | Declared | — | Path to Unity project root (optional, will auto-detect if not specified) | PROJECT · required · arity 1 |
| --agent-id | — | <AGENT_ID> | No | No | Declared | — | Agent ID for distinguishing multiple agents | AGENT_ID · required · arity 1 |
| --json | — | flag | No | No | Declared | — | Output JSON responses instead of human-readable text | — |
| --timeout | -t | <TIMEOUT> | No | No | Declared | — | Timeout in seconds for commands sent to Unity (overrides the per-command default) | TIMEOUT · required · arity 1 |
| --help | -?, -h | flag | No | No | Declared | — | Show help and usage information | — |

<a id="command-wait"></a>
### `wait`

Wait until Unity Editor is connected and ready to accept commands

#### Options

| Name | Aliases | Value | Required | Recursive | Scope | Group | Description | Arguments |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| --poll-timeout | — | <POLL_TIMEOUT> | No | No | Declared | — | Maximum seconds to wait for Unity to be ready (default: 120, or wait-timeout from config) | POLL_TIMEOUT · optional · arity 0..1 |
| --project | — | <PROJECT> | No | No | Declared | — | Path to Unity project root (optional, will auto-detect if not specified) | PROJECT · required · arity 1 |
| --agent-id | — | <AGENT_ID> | No | No | Declared | — | Agent ID for distinguishing multiple agents | AGENT_ID · required · arity 1 |
| --json | — | flag | No | No | Declared | — | Output JSON responses instead of human-readable text | — |
| --timeout | -t | <TIMEOUT> | No | No | Declared | — | Timeout in seconds for commands sent to Unity (overrides the per-command default) | TIMEOUT · required · arity 1 |
| --help | -?, -h | flag | No | No | Declared | — | Show help and usage information | — |
