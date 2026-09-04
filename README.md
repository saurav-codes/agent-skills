# agent-skills

AI agent skills, one repo per skill, plus one repo of bundled skills. Each installs with one command.

## Standalone skills

| Skill | What it does | Install |
|---|---|---|
| [atomic-commits](https://github.com/saurav-codes/atomic-commits) | Splits uncommitted changes into granular, conventional atomic commits in dependency order | `npx skills add saurav-codes/atomic-commits -g` |
| [sd-generate](https://github.com/saurav-codes/sd-generate) | Generates images with Stable Diffusion 3.5 Large on DigitalOcean Inference | `npx skills add saurav-codes/sd-generate -g` |
| [htmx-expert](https://github.com/saurav-codes/htmx-expert) | Enforces production-grade htmx patterns and the htmx web security golden rules | `npx skills add saurav-codes/htmx-expert -g` |
| [hindsight-memory](https://github.com/saurav-codes/hindsight-memory) | Routes memory requests to a self-hosted Hindsight MCP bank: retain, recall, reflect, invalidate | `npx skills add saurav-codes/hindsight-memory -g` |
| [avoid-ai-writing](https://github.com/saurav-codes/avoid-ai-writing) | Audits and rewrites text to remove AI writing patterns, with detect, rewrite, and edit modes | `npx skills add saurav-codes/avoid-ai-writing -g` |
| [email-best-practices](https://github.com/saurav-codes/email-best-practices) | Email deliverability (SPF, DKIM, DMARC), compliance, sending patterns, and accessibility | `npx skills add saurav-codes/email-best-practices -g` |
| [writing-for-agents](https://github.com/saurav-codes/writing-for-agents) | Writing documents agents consume: skills, AGENTS.md, context pointers, pruning | `npx skills add saurav-codes/writing-for-agents -g` |

## Bundled skills

[bundled-skills](https://github.com/saurav-codes/bundled-skills) merges 76 overlapping single-purpose skills into seven lean bundles. Each bundle holds one lean `SKILL.md` plus `reference/` files per subdomain.

| Bundle | Absorbs | Covers |
|---|---|---|
| growth-playbook | 19 marketing skills | Ads, SEO and AI-search, ASO, copywriting, pricing, launch, content, research, community, referrals, PR, free tools, onboarding, planning |
| firebase-stack | 10 Firebase skills | CLI, Auth, Firestore, Hosting, App Hosting, Data Connect, Crashlytics, Remote Config, AI Logic, rules audits |
| web-recon | 10 browser and research skills | Local browsers, Browser Use Cloud, the browser-use SDK, OpenCLI adapters, social research, 30-day opinions, cited research |
| build-pipeline | 10 developer workflow skills | TDD, subagent execution, diagnosis, code review, design, domain modeling, git safety, pre-commit |
| frontend-craft | 6 frontend skills | Visual design, UI polish, motion, view transitions, shadcn/ui, prototyping |
| email-stack | 3 email skills | Resend API, Resend CLI, agent inboxes |
| spec-workshop | 18 planning and writing skills | Grilling, handoff, specs, tickets, triage, wayfinder, writing pipeline, setup |

Install every bundle:
```bash
npx skills add saurav-codes/bundled-skills --all -g
```

Install one bundle:
```bash
npx skills add saurav-codes/bundled-skills -s growth-playbook -g
```

## Adding a skill

One repo per skill, named after the skill. The repo root holds `SKILL.md` plus a `reference/` folder for disclosed docs. Add the new repo as a row in the table above. Bundles live in bundled-skills, one folder per bundle.
