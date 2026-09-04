# agent-skills

AI agent skills, one repo per skill. Each installs with one command.

## Skills

| Skill | What it does | Install |
|---|---|---|
| [atomic-commits](https://github.com/saurav-codes/atomic-commits) | Splits uncommitted changes into granular, conventional atomic commits in dependency order | `npx skills add saurav-codes/atomic-commits` |
| [sd-generate](https://github.com/saurav-codes/sd-generate) | Generates images with Stable Diffusion 3.5 Large on DigitalOcean Inference | `npx skills add saurav-codes/sd-generate` |
| [htmx-expert](https://github.com/saurav-codes/htmx-expert) | Enforces production-grade htmx patterns and the htmx web security golden rules | `npx skills add saurav-codes/htmx-expert` |

## Install

Run the install command for the skill you want, for example:

```bash
npx skills add saurav-codes/htmx-expert
```

`npx skills add` clones the repo into your agent's skills folder with the right layout.

Manual alternative for any skill in the table:

```bash
git clone https://github.com/saurav-codes/htmx-expert.git <skills-dir>/htmx-expert
```

Where `<skills-dir>` is your agent's skills folder, for example `~/.agents/skills` or `~/.claude/skills`.

## Adding a skill

One repo per skill, named after the skill. The repo root holds `SKILL.md` plus a `reference/` folder for disclosed docs. Add the new repo as a row in the table above.
