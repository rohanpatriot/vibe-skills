# Vibe Skills

This repository contains Claude Code skills for planning, productivity, and vibe-coded development.

## Repository Structure

```
vibe-skills/
├── skills/                      # All skills go here
│   └── planning-setup/          # Planning infrastructure scaffolding
├── CLAUDE.md                    # This file
└── README.md                    # User documentation
```

## Skill Requirements

### YAML Frontmatter (REQUIRED)

Every `SKILL.md` file must begin with valid YAML frontmatter:

```yaml
---
name: skill-name
description: What this skill does and when to use it. Claude uses this to decide when to apply the skill automatically.
---
```

- `name` is **REQUIRED** - must match directory name, lowercase-with-hyphens
- `description` is **REQUIRED** - Claude uses this for automatic skill selection

### File Naming

- Skill directories: `lowercase-with-hyphens`
- Main file: `SKILL.md` (exact casing)
- Workflow files: `lowercase-with-hyphens.md`
- Reference files: `lowercase-with-hyphens.md`

## Skill Design Philosophy

**Skills are tools, not documentation.**

Write as an active collaborator:
- "I help you find..."
- "I'll audit this for..."
- "I check your code for..."

Create workflows that DO things:
- audit, test, check, analyze, decompose, verify

## File Reference Patterns

Always use relative markdown links:

```markdown
See [workflows/main-workflow.md](workflows/main-workflow.md)
See [references/concepts.md](references/concepts.md)
```
