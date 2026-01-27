# Vibe Skills

A collection of Claude Code skills for planning, productivity, and vibe-coded development.

## Installation

```bash
npx skills add huntsyea/vibe-skills
```

## Available Skills

### planning-setup

Sets up planning-with-files infrastructure for complex projects. Creates task_plan.md, findings.md, progress.md, updates CLAUDE.md with methodology guidance, and adds .claude/rules enforcement.

**Use when:** Starting a project that will require >5 tool calls or complex multi-step work.

```bash
/planning-setup
```

## Repository Structure

```
vibe-skills/
├── skills/
│   └── planning-setup/          # Planning infrastructure scaffolding
│       ├── SKILL.md             # Main skill file
│       ├── references/          # Usage guide, Manus principles
│       ├── workflows/           # Setup workflows
│       └── templates/           # Planning file templates
├── CLAUDE.md                    # Project instructions
└── README.md                    # This file
```

## Testing Locally

```bash
npx skills add ./path/to/vibe-skills
```

## License

MIT License - See [LICENSE](LICENSE) for details.
