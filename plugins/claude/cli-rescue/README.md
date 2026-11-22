# cli-rescue

Claude Code plugins that delegate substantial coding or investigation tasks to another coding CLI and return its output unchanged.

| Plugin | Delegates to | Commands |
|---|---|---|
| `qwen` | Qwen Code | `/qwen:rescue`, `/qwen:review`, `/qwen:setup` |
| `gemini` | Gemini CLI | `/gemini:rescue`, `/gemini:setup` |

Each plugin is a thin forwarding wrapper: one `Bash` call to its `*-companion.mjs` script, no paraphrasing. Run `/<plugin>:setup` first to check that the CLI is installed and authenticated.

## Install

Add this folder as a marketplace, then install a plugin:

```
/plugin marketplace add ./plugins/claude/cli-rescue
/plugin install qwen@cli-rescue
/plugin install gemini@cli-rescue
```

The plugins use only Claude Code's public plugin interface and the installed CLI's own command line.
