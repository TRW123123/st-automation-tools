# agent-skill-starter

Two free `SKILL.md` files for AI coding agents: `house-rules` and `pre-publish-gate`. They are plain Markdown and set the ground rules an agent needs before it touches anything outside your machine: when to ask for approval, how to handle secrets, what counts as evidence, and what to check before text goes public.

They work with Claude Code, Codex, Cursor and any other agent that reads `SKILL.md` files. No code, no API keys, nothing to install.

## What's in this repo

| Skill | What it does |
|---|---|
| `skills/house-rules` | 11 base rules: language, approvals, secrets, evidence, logins, untrusted web content |
| `skills/pre-publish-gate` | 10 checks before any post, email or product page goes out: facts, proof, filler words, platform fit, privacy |

## How to use

1. Copy the folders from `skills/` into your agent's skills directory:
   - **Claude Code:** `.claude/skills/` in your project, or `~/.claude/skills/` for all projects
   - **Codex:** `.agents/skills/` in your repo, or `~/.agents/skills/` for all repos
   - **Cursor:** `.cursor/skills/` or `.agents/skills/` in your project (Cursor also reads `.claude/skills/`)
2. Fill in the values in square brackets, such as the owner name and language. Each file ends with a "Fill in" table that lists them.
3. Ask your agent to load `house-rules` at the start of a task. Run `pre-publish-gate` before you approve any outside text.

Rules 7 and 8 in `house-rules` point to two skills from the full kit (`one-bot-per-login`, `job-queue-worker`). Delete those lines if you only use this repo.

## The full kit

The **Agent Skill Starter Kit** has six skills. Besides the two here, it adds:

- `job-queue-worker`: claim, heartbeat, complete or fail for webhook and queue jobs, with fail classes
- `one-bot-per-login`: lease files so two agents never work in the same browser login or device
- `approval-first-outreach`: draft first, check duplicates and do-not-contact lists, ask once, then send exactly that
- `evidence-report`: research reports where every claim has a link and estimates are marked

Get it here: https://payhip.com/b/sxCKk

## License

MIT for the files in this repo. See `LICENSE`.
