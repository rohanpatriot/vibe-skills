# Manus Principles: Why Planning-with-Files Works

These six principles explain why file-based planning is effective for LLMs working on complex tasks.

## 1. KV-Cache: Context Established Early is Cheap

**Principle**: Tokens processed early in a conversation cost less attention-wise than tokens added later.

**Implication**:
- Create task_plan.md at the start, not midway through
- Front-load the goal, phases, and constraints
- Don't try to recover context later - establish it upfront

**Example**:
- ❌ Work for 30 turns, then try to summarize what you're doing
- ✅ Write task_plan.md in turn 2, reference it throughout

---

## 2. Mask Don't Remove: Attention Manipulation

**Principle**: You can't delete tokens from KV-cache, but you can mask them with new content.

**Implication**:
- Append to files rather than editing them
- Use tables with new rows, not updated cells
- When things change, add a new entry explaining the change

**Example**:
- ❌ Edit the "Decisions Made" table to change a decision
- ✅ Add a new row: "Changed decision on X because Y"

---

## 3. Filesystem as External Memory

**Principle**: Files persist across sessions; KV-cache doesn't.

**Implication**:
- Critical context must live in files, not just in-memory
- Files are the source of truth for goals, decisions, errors
- Rereading files is cheaper than trying to remember

**Example**:
- ❌ "I remember we decided to use approach X"
- ✅ Read task_plan.md → "Decisions Made table shows we chose X because Y"

---

## 4. Manipulate Attention Through Recitation

**Principle**: Reading a file aloud (in reasoning) brings it into active attention.

**Implication**:
- Before major decisions, explicitly reread planning files
- Recite the goal, current phase, and key findings
- Use the 5-Question Reboot Check when resuming work

**Example**:
- ❌ Make a decision based on vague recollection
- ✅ "Let me read task_plan.md... the goal is X, we're in phase Y, we decided Z"

---

## 5. Keep Wrong Stuff In

**Principle**: Errors and failed attempts are valuable learning signals.

**Implication**:
- Log all errors to the Errors table
- Don't delete failed approaches
- Track what was tried and why it didn't work
- Add resolutions/mutations, don't erase mistakes

**Example**:
- ❌ Delete the row about the failed API attempt
- ✅ Add resolution: "Switched to OAuth because API key approach failed due to rate limits"

---

## 6. Don't Get Few-Shotted

**Principle**: Repeating the same pattern creates a strong prior that's hard to break.

**Implication**:
- Vary your language and structure
- Don't always use the same format for findings
- Mix up how you document things
- Avoid ritualistic patterns that stop you from adapting

**Example**:
- ❌ Every finding entry has the same 5 bullet points
- ✅ Adapt the format to what you learned (sometimes bullets, sometimes prose, sometimes tables)

---

## How These Principles Shape Planning-with-Files

| Principle | How It's Applied |
|-----------|------------------|
| KV-Cache | Create task_plan.md first, establish goal and phases early |
| Mask Don't Remove | Append to tables (Decisions, Errors), don't edit past entries |
| Filesystem = Memory | All critical context in files (task_plan, findings, progress) |
| Recitation | Read-before-decide rule, 5-Question Reboot Check |
| Keep Wrong In | Errors table tracks failures with resolutions |
| Don't Few-Shot | Vary documentation format, adapt to what you learn |

---

## Further Reading

These principles come from practical experience with LLM planning across many complex projects. They're not theoretical - they're patterns that consistently improve outcomes for multi-session, complex work.

For how to apply these principles day-to-day, see [usage-guide.md](usage-guide.md).
