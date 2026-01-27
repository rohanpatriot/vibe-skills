## Planning Methodology

This project uses **planning-with-files**, a file-based planning approach for complex multi-step work.

### Planning Context

These files are automatically loaded into Claude's memory at session start:

@{{PLANNING_DIR}}/task_plan.md
@{{PLANNING_DIR}}/findings.md
@{{PLANNING_DIR}}/progress.md

### Overview

Planning-with-files uses three interconnected files as external memory:
- **task_plan.md** - Phase tracking, decisions, errors
- **findings.md** - Research discoveries, visual findings
- **progress.md** - Session log, test results

These files work alongside Claude's built-in TaskCreate/TaskUpdate tools:
- Files track project phases and high-level progress
- Task tools manage individual tasks within each phase

### When to Use

Use planning-with-files for:
- Complex tasks requiring >5 tool calls
- Multi-session projects
- Work requiring research and exploration
- Projects with multiple phases or dependencies
- Situations where you need to maintain context across sessions

For simple, single-step tasks, use TaskCreate/TaskUpdate directly.

### Core Rules

See `.claude/rules/planning-with-files.md` for enforcement rules:
- Create plan first (for complex tasks)
- 2-Action Rule (save findings after browser/search)
- Read before decide (refresh goals before major decisions)
- Log all errors (track and mutate approach)

### Setup

To set up planning-with-files for a new project, use:
```
/huntsyea:planning-setup
```

This creates the planning files, updates this file, and adds enforcement rules.
