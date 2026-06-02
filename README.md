# superbereza.md

A public **Claude Code plugin marketplace** — small, cross-agent skills for AI coding agents. Each plugin is a standalone repo; this marketplace just aggregates them so you can install with one command.

## Use

```text
/plugin marketplace add superbereza/superbereza.md
/plugin install things@superbereza.md
/plugin install drop@superbereza.md
/plugin install claude-remote@superbereza.md
```

Non-interactive equivalent:

```bash
claude plugin marketplace add superbereza/superbereza.md
claude plugin install things@superbereza.md
```

## Plugins

| Plugin | What it does | Repo |
|---|---|---|
| `things` | Things 3 CLI + skill — read/write tasks, JSON output | [things-cli](https://github.com/superbereza/things-cli) |
| `drop` | Share any file, folder, or app via a password-protected HTTPS link | [agent-instant-drop](https://github.com/superbereza/agent-instant-drop) |
| `claude-remote` | Launch Claude Code Remote Control sessions in a detached tmux pane | [claude-remote-launcher](https://github.com/superbereza/claude-remote-launcher) |

Each plugin also works **standalone** (`git clone … && ./install.sh`) and as **its own marketplace** — see its repo. All are built to one skill-repo standard: the same `skills/` directory is consumed by **Claude Code, Cursor, Codex and Gemini**.
