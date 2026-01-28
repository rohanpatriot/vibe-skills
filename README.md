# Vibe Skills

You don't need to be a developer. You need to ship.

I'm not here to teach you to code. I'm here to make sure you don't have to. Vibecoding is simple: you say what you want, Claude builds it. But Claude has a memory problem. Context slips. Mistakes repeat. Projects go sideways.

These skills fix that.

## Install

```bash
npx skills add rohanpatriot/vibe-skills
```

Verify it worked: run `/planning-setup` in Claude Code.

## What's Inside

### planning-setup

For projects that span multiple sessions with moving pieces.

**Use when** you're starting something complex—multiple features, days of work, decisions that need tracking.

**Run**: `/planning-setup`

**Creates**:
- `task_plan.md` — Goal, phases, decisions, errors
- `findings.md` — Research discoveries, technical decisions
- `progress.md` — Session logs, test results
- `.claude/rules/` — Rules that force Claude to use these files

No more starting from zero every session. No more repeating the same dead ends.

## How Skills Work

Skills give Claude persistent instructions. When you install this repo:
- Claude gains new `/commands` you can invoke
- Skills create files that survive session restarts
- Rules enforce discipline (like "save findings after every research task")

This doesn't reinvent the wheel. It builds on Claude's built-in planning mode and task system—adding file-based persistence so your context survives across sessions.

## Why I Built This

Most people quit when projects get complicated. Not because they lack vision—because their tools lose the thread.

Claude is good. But Claude forgets. These skills give it a system so it doesn't.

You focus on the outcome. Claude handles the execution. This makes sure nothing falls through the cracks.

## License

MIT — Do what you want with it.
