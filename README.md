# harness-support

Support code for coding-agent harnesses: mods, plugins, hooks and small runtimes that make a harness work well inside a long-running multi-agent system.

Each folder holds the support for one harness. Nothing here is a dependency of the main system; a harness that needs a capability gets it from its own folder.

| Folder | Harness |
|---|---|
| `claude/` | Claude Code |
| `codex/` | Codex CLI |
| `pi/` | Pi |
| `omp/` | Omp |
| `reasonix/` | Reasonix |
| `dsh/` | Dsh |

More folders are added when a harness needs support.

## Rules

- English only in code, comments, logs, issues and pull requests.
- Roles, not personal or agent names. No hosts, absolute paths, chat ids or keys in any file.
- No dependency on a third-party harness source tree: ideas and public interfaces only.
- Each change starts as an issue that states the problem, the desired outcome and how it is measured.
