# Vibe Skills

Two ways to waste time vibecoding: build the wrong thing, or lose the thread building the right thing.

These skills fix both. `/idea` validates what you're building before you start. `/planning-setup` keeps your agent focused once you do.

## Install

```bash
npx skills add rohanpatriot/vibe-skills
```

Verify it worked: run `/idea` or `/planning-setup` in your AI coding agent.

## What's Inside

### idea

Transform raw ideas into validated, buildable MVPs.

**Use when** you have an idea but need to stress-test assumptions, identify your first customers, and define what to actually build.

**Run**: `/idea` or `/idea I want to build a tool that...`

**Creates**:
- `idea-brief.md` — Your idea with testable hypotheses
- `customer-profile.md` — Target customer with earlyvangelist criteria
- `mvp-spec.md` — MVP features mapped to problems solved
- `custdev-tasks.md` — Customer development research tasks

Guides you through five phases: idea intake, problem discovery, customer discovery, solution fit, and MVP definition. When you're ready to build, it hands off to `/planning-setup`.

---

### planning-setup

For projects that span multiple sessions with moving pieces.

**Use when** you're starting something complex—multiple features, days of work, decisions that need tracking.

**Run**: `/planning-setup`

**Creates**:
- `task_plan.md` — Goal, phases, decisions, errors
- `findings.md` — Research discoveries, technical decisions
- `progress.md` — Session logs, test results
- `.claude/rules/` — Rules that force your agent to use these files

No more starting from zero every session. No more repeating the same dead ends.

## How Skills Work

Skills give your agent persistent instructions. When you install this repo:
- Your agent gains new `/commands` you can invoke
- Skills create files that survive session restarts
- Rules enforce discipline (like "save findings after every research task")

This doesn't reinvent the wheel. It builds on your agent's built-in planning mode and task system—adding file-based persistence so your context survives across sessions.

## Why I Built This

Most people fail in two places: they build the wrong thing, or they lose the thread while building the right thing.

The first skill validates your idea before you write a line of code. The second keeps your agent focused once you start building. Both are about not wasting your time.

You focus on the outcome. Your agent handles the execution. These skills make sure you're building something worth building—and that nothing falls through the cracks once you start.

## License

MIT — Do what you want with it.
