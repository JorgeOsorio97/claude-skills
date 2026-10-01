# claude-skills

Jorge Osorio's Claude Code plugins, published as a plugin marketplace.

## Install

```
/plugin marketplace add JorgeOsorio97/claude-skills
/plugin install roadmap@jorgeosorio97
```

Recommended companion (the "grill" step uses it if present):

```
/plugin marketplace add mattpocock/skills
/plugin install mattpocock-skills@mattpocock
```

## Update

```
/plugin marketplace update jorgeosorio97
```

Or turn on auto-update for the `jorgeosorio97` marketplace in `/plugin` → Marketplaces.

## Plugins

| Plugin | Skills | What it does |
|---|---|---|
| `roadmap` | `roadmap`, `continue-roadmap` | Build a roadmap for work that spans several sessions/PRs, then resume it stage by stage. Roadmaps live in `.claude/plans/<work>/ROADMAP.md` (gitignored). |

## Contributing

1. Edit the skill under `plugins/<plugin>/skills/<skill>/SKILL.md`.
2. Bump `version` in `plugins/<plugin>/.claude-plugin/plugin.json` — clients only
   pick up a change when the version moves.
3. `claude plugin validate .` before opening the PR.
4. Open a PR; no direct pushes to `main`.
