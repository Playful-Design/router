# Playful Design Router

Design skills for your coding agent, plus a router that picks the right one for each task.

```bash
npx skills add playful-design/router
```

Installs the `playful-design-router` skill and 42 skills it routes to. Works with Claude Code, Codex, Cursor and the other agents the [skills CLI](https://github.com/vercel-labs/skills) supports. More at [playfuldesign.app/skills](https://www.playfuldesign.app/skills).

## What's included

| Author | Skills | Original |
| --- | --- | --- |
| Emil Kowalski | 15 design-engineering and animation skills | [emilkowalski/skills](https://github.com/emilkowalski/skills) |
| Raphael Salaja | 25 interface principles and procedures | [raphaelsalaja/skills](https://github.com/raphaelsalaja/skills) |
| Benji Taylor | stageshow | [benjitaylor/skills](https://github.com/benjitaylor/skills) |
| Vercel | web-design-guidelines | [vercel-labs/agent-skills](https://github.com/vercel-labs/agent-skills) |

Each skill folder is an unmodified copy of its author's skill at a pinned commit, with that author's MIT license kept inside the folder. All credit belongs to them. Emil's `prototype` is left out because it shares a name with Raphael's `prototype` and the two would overwrite each other.

To install one author's skills on their own, use their repo directly, for example `npx skills add emilkowalski/skills`.

## The router

`skills/playful-design-router/SKILL.md` checks which design skills are installed, applies the standards skills on every change, and routes each task: stageshow for faux product UI, animate for new motion, match to recreate a reference, verify and viewports before work is called done. Skills that only run when called by name are suggested, not run.
