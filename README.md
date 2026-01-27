# Vibe Skills

Skills for vibecoding. Ship great stuff without being a developer.

Vibecoding is about describing what you want and letting AI handle the technical details. These skills help Claude Code stay organized, remember context across sessions, and keep complex projects on track—so you can focus on the vision while Claude handles the execution.

## Installation

```bash
npx skills add rohanpatriot/vibe-skills
```

## Available Skills

### planning-setup

Stay organized on bigger projects. This skill sets up a simple planning system that helps Claude remember what you're building, what's been tried, and what's next.

**Use when:** Your project is getting complex—multiple features, lots of back-and-forth, or work that spans several sessions.

```bash
/planning-setup
```

**What it creates:**
- `task_plan.md` - Your goal, current phase, decisions made
- `findings.md` - What Claude discovers along the way
- `progress.md` - Session-by-session log of what happened
- Enforcement rules so Claude actually uses these files

No more "wait, what were we doing?" moments.

## Why This Exists

When you're vibecoding a complex project, context gets lost. Claude forgets what was tried, repeats mistakes, or loses track of the bigger picture.

These skills give Claude the structure to:
- Remember across sessions
- Learn from errors
- Stay focused on your actual goal

You describe what you want. Claude figures out how. These skills help Claude do that better.

## License

MIT License - See [LICENSE](LICENSE) for details.
