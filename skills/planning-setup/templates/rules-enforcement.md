# Planning-with-Files Enforcement Rules

These rules ensure consistent use of the planning-with-files methodology for complex tasks.

## Rule 1: Create Plan First

**When**: Starting a complex task requiring >5 tool calls or multiple sessions

**Requirement**: Create or update task_plan.md before beginning work

**Why**: KV-cache optimization - establishing context early is cheaper than trying to recover it later

**Action**:
```
1. Read existing task_plan.md (if it exists)
2. Update or create with:
   - Clear goal
   - Defined phases
   - Key questions to answer
   - Initial constraints
3. Begin work
```

---

## Rule 2: 2-Action Rule

**When**: After browser navigation, search operations, or visual exploration

**Requirement**: Save findings to findings.md before taking additional actions

**Why**: Visual/browser context is expensive to re-load. Capture it while it's in memory.

**Action**:
```
1. Navigate/search/explore (Action 1)
2. Write findings to findings.md (Action 2)
3. Continue with next action
```

**Applies to**:
- Browser automation (mcp__claude-in-chrome__)
- Web searches (WebSearch)
- Screenshot analysis (Read on images)
- Documentation exploration (WebFetch)

---

## Rule 3: Read Before Decide

**When**: Before making major decisions or changing direction

**Requirement**: Reread relevant planning files to refresh context

**Why**: Filesystem as external memory - don't rely on KV-cache for critical decisions

**Action**:
```
Before major decisions:
1. Read task_plan.md (goal, current phase, decisions)
2. Read findings.md (what we've learned)
3. Read progress.md (what we've tried)
4. Make informed decision
5. Log decision in task_plan.md
```

**Major decisions include**:
- Changing approach or architecture
- Selecting between alternatives
- Moving to a new phase
- Deciding something doesn't work

---

## Rule 4: Log All Errors

**When**: Any error, failure, or unexpected outcome occurs

**Requirement**: Log to task_plan.md Errors table immediately

**Why**: Keep wrong stuff in - errors guide learning and prevent repeated mistakes

**Action**:
```
1. Log error to task_plan.md Errors table:
   - Error: What happened
   - Context: What you were trying to do
   - Resolution/Mutation: How you addressed it
   - Date: When it occurred
2. If resolved, add resolution (don't delete the error)
3. If it changes approach, update Current Phase or Decisions
```

**Don't**:
- Delete error entries
- Hide failed attempts
- Assume you'll remember it

---

## Integration with TaskCreate/TaskUpdate

Planning-with-files works alongside built-in task tools:

**Use task_plan.md for**:
- Project phases (high-level structure)
- Key decisions affecting the whole project
- Errors that change approach
- Cross-session context

**Use TaskCreate/TaskUpdate for**:
- Individual tasks within a phase
- Specific action items
- Task dependencies
- Current work tracking

**Hybrid workflow**:
```
1. task_plan.md shows: "Phase 2: Implementation ⏳"
2. TaskCreate individual tasks:
   - "Implement user authentication"
   - "Write tests for auth flow"
   - "Update API documentation"
3. As tasks complete, findings → findings.md
4. When phase completes, update task_plan.md
```

---

## Enforcement

Claude should proactively:
- Suggest creating task_plan.md for complex tasks
- Remind about the 2-Action Rule after browser/search ops
- Suggest rereading files before major decisions
- Prompt to log errors when they occur

These rules can be overridden by explicit user instruction, but should be the default behavior for complex multi-step work.
