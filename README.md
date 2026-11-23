# App Store Answer Check — an Agent Skill by The Ask Why Company

Verify App Store / Google Play / Galaxy Store privacy, age-rating and listing answers against the code before submitting.

**When it's used:** use before submitting a mobile app to the Apple App Store, Google Play or Samsung Galaxy Store — to verify privacy labels, data safety, age rating answers and listing claims against what the code actually does.

Read the skill: [skills/app-store-answer-check/SKILL.md](skills/app-store-answer-check/SKILL.md)

Works with Claude (Claude Code, Claude.ai) and any tool that reads the open [Agent Skills](https://agentskills.io) `SKILL.md` format.

## Install in Claude
**Claude Code:**
```
/plugin marketplace add theaskwhy/app-store-answer-check
/plugin install app-store-answer-check@app-store-answer-check
```
Or from the full catalogue: `/plugin marketplace add theaskwhy/skills` then `/plugin install app-store-answer-check@theaskwhy`.

**Manual:** copy `skills/app-store-answer-check/` into `~/.claude/skills/` (personal) or `.claude/skills/` (project).

**Claude.ai:** zip the `skills/app-store-answer-check` folder and upload it under Settings → Capabilities → Skills.

## Use it with any AI agent
This skill uses the open **Agent Skills** standard (`SKILL.md`), so the same file works in Claude Code, OpenAI Codex, Cursor, Gemini CLI, GitHub Copilot, Windsurf, Antigravity, OpenCode, Goose and many more.

**Quickest (any supported agent):** the open-source `skills` installer detects your tools and installs for them:
```
npx skills add theaskwhy/app-store-answer-check
```

**Manual:** copy `skills/app-store-answer-check/` into your tool's skills folder:

| Tool | Personal (all projects) | One project |
|---|---|---|
| Claude Code | `~/.claude/skills/` | `.claude/skills/` |
| OpenAI Codex | `~/.codex/skills/` | `.agents/skills/` |
| Cursor | `~/.cursor/skills/` | `.cursor/skills/` |
| Gemini CLI / Antigravity | `~/.gemini/skills/` | `.gemini/skills/` |
| GitHub Copilot | `~/.copilot/skills/` | `.github/skills/` |
| Windsurf | — | `.windsurf/skills/` |
| Any spec-compliant agent | — | `.agents/skills/` |

Folder names change between tool versions — if a tool doesn't pick it up, check its current skills documentation. Tools without skills support can still use it: paste `SKILL.md` into the tool's rules/instructions file (e.g. `AGENTS.md`, Cursor rules).

## More skills
Full catalogue: [github.com/theaskwhy/skills](https://github.com/theaskwhy/skills)

## Licence
MIT © The Ask Why Company LLC. If you use or adapt this skill, a credit to The Ask Why Company is appreciated.
