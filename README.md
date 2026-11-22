# harness-support

Support code for coding-agent harnesses: MCP servers, plugins and mods, and Agent Skills that make a harness work well inside a long-running multi-agent system.

Nothing here is a dependency of the main system; a harness that needs a capability takes it from the matching folder.

| Folder | Holds |
|---|---|
| `mcp/` | MCP servers and tools a harness can register. |
| `plugins/` | Plugins, mods, hooks and small runtimes that extend a harness. |
| `agent-skills/` | Agent Skills (a directory with a `SKILL.md`, following the agentskills.io format). |

Inside a folder, a subfolder is named for the harness it supports (for example `plugins/claude` or `plugins/codex`) when the code is specific to one harness; code that works with any harness sits directly in the folder.

Open work is tracked in the issues of this repository. Issues for a specific harness carry its label (`claude`, `codex`).

## Rules

- English only in code, comments, logs, issues and pull requests.
- Roles, not personal or agent names. No hosts, absolute paths, chat ids or keys in any file.
- No dependency on a third-party harness source tree: ideas and public interfaces only.
- Each change starts as an issue that states the problem, the desired outcome and how it is measured.
