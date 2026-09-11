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
| [frontend-design](https://github.com/saurav-codes/frontend-design) | Enforces minimalist design taste for frontend UI and bans AI-slop patterns across color, typography, layout, motion, copy, and accessibility | `npx skills add saurav-codes/frontend-design -g` |
| [use-modern-go](https://github.com/JetBrains/go-modern-guidelines) | Applies the Modern Go Guidelines version-specific guidance when writing, modifying, fixing, or refactoring Go code | `npx skills add JetBrains/go-modern-guidelines -g` |
| [gstack-review](https://github.com/saurav-codes/gstack-review) | Infrastructure-first security audit: secrets archaeology, supply chain, CI/CD, LLM security, OWASP, STRIDE, with false-positive filtering | `npx skills add saurav-codes/gstack-review -g` |
| [ai-company-with-herdr](https://github.com/saurav-codes/ai-company-with-herdr) | Runs a hierarchical AI agent company over Herdr panes: a tech lead hands off to a senior engineer that executes with workers and a strongest-model reviewer, communicating via handoff and inbox files | `npx skills add saurav-codes/ai-company-with-herdr -g` |
| [hacker-audit](https://github.com/saurav-codes/hacker-audit) | Black-box security audit of a web app the owner verifies: recon, JS bundle extraction, scanners, manual business-logic attacks, PoC-backed findings | `npx skills add saurav-codes/hacker-audit -g` |
| [archify](https://github.com/tt-a1i/archify) | Creates polished, validated architecture, workflow, sequence, data-flow, and lifecycle diagrams as standalone HTML with inline SVG and export | `npx skills add tt-a1i/archify -g` |
| [i-have-adhd](https://github.com/ayghri/i-have-adhd) | Shapes agent output for an ADHD reader: next action first, numbered steps, restated state, concrete time estimates | `npx skills add ayghri/i-have-adhd -g` |
| [kun](https://github.com/kunchenguid/kun) | Summons Kun, a problem-solving persona for how Kun thinks, builds, and solves problems | `npx skills add kunchenguid/kun/skills/kun -g` |

## Install all

Installs every skill in the table above, globally (parses the table, so new rows are picked up automatically):

```bash
curl -fsSL https://raw.githubusercontent.com/saurav-codes/agent-skills/main/README.md | grep '^|' | grep -oE 'npx skills add [^`|]+' | sed -e 's/^npx /npx -y /' -e 's|$| --agent "*" -y </dev/null|' | sh
```

## Adding a skill

One repo per skill, named after the skill. The repo root holds `SKILL.md` plus a `reference/` folder for disclosed docs. Add the new repo as a row in the table above.
