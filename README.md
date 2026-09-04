# agent-skills

AI agent skills, one repo per skill. Each installs with one command.

## Skills

| Skill | What it does | Install |
|---|---|---|
| [atomic-commits](https://github.com/saurav-codes/atomic-commits) | Splits uncommitted changes into granular, conventional atomic commits in dependency order | `npx skills add saurav-codes/atomic-commits -g` |
| [sd-generate](https://github.com/saurav-codes/sd-generate) | Generates images with Stable Diffusion 3.5 Large on DigitalOcean Inference | `npx skills add saurav-codes/sd-generate -g` |
| [htmx-expert](https://github.com/saurav-codes/htmx-expert) | Enforces production-grade htmx patterns and the htmx web security golden rules | `npx skills add saurav-codes/htmx-expert -g` |
| [hindsight-memory](https://github.com/saurav-codes/hindsight-memory) | Routes memory requests to a self-hosted Hindsight MCP bank: retain, recall, reflect, invalidate | `npx skills add saurav-codes/hindsight-memory -g` |
| [avoid-ai-writing](https://github.com/saurav-codes/avoid-ai-writing) | Audits and rewrites text to remove AI writing patterns, with detect, rewrite, and edit modes | `npx skills add saurav-codes/avoid-ai-writing -g` |
| [use-modern-go](https://github.com/JetBrains/go-modern-guidelines) | Applies the Modern Go Guidelines version-specific guidance when writing, modifying, fixing, or refactoring Go code | `npx skills add JetBrains/go-modern-guidelines -g` |

## Adding a skill

One repo per skill, named after the skill. The repo root holds `SKILL.md` plus a `reference/` folder for disclosed docs. Add the new repo as a row in the table above.
