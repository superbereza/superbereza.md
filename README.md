# superbereza.md

> *The repository that will replace me. Patiently.*

A public **Claude Code plugin marketplace** — small, cross-agent skills for AI coding agents. Each plugin is a standalone repo; this marketplace just aggregates them so you can install with one command.

## Use

```text
/plugin marketplace add superbereza/superbereza.md

# everything at once (umbrella plugin):
/plugin install i-want-it-all@superbereza.md

# …or pick individually:
/plugin install things@superbereza.md
/plugin install drop@superbereza.md
/plugin install agent-sessions@superbereza.md
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
| `agent-sessions` | Spawn, message and close Claude Code / Codex / any-CLI sessions in herdr or tmux (+ tmux→herdr migration) | [agent-sessions](https://github.com/superbereza/agent-sessions) |
| `claude-session-keeper` | Persist Remote Control / tmux sessions across reboots and crashes | [claude-session-keeper](https://github.com/superbereza/claude-session-keeper) |
| `claude-session-teleport` | Move a live chat session between machines — clone/migrate + tmux respawn | [claude-session-teleport](https://github.com/superbereza/claude-session-teleport) |
| `browser` | Drive a real, headed web browser from the agent (persistent Playwright daemon) | [browser-skill](https://github.com/superbereza/browser-skill) |
| `i-want-it-all` | Umbrella — installs all of the above at once | — (lives here) |

Each plugin also works **standalone** (`git clone … && ./install.sh`) and as **its own marketplace** — see its repo. All are built to one skill-repo standard: the same `skills/` directory is consumed by **Claude Code, Cursor, Codex and Gemini**.
