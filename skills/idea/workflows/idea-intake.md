# Phase 1: Idea Intake

Capture the raw idea and expand it into structured, testable hypotheses.

## Goal

Transform a vague idea into a clear statement with explicit assumptions about:
- The **problem** you think exists
- The **customer** you think has it
- The **solution** you think will work

## Process

### Step 1: Capture the Raw Idea

If the user provided their idea, acknowledge it. If not, ask:

> What's your idea? Don't worry about making it perfect—just describe what you're thinking about building and why.

### Step 2: Expand with "What If" Prompts

Ask follow-up questions to flesh out the idea:

**About the problem:**
- What specific pain does this solve?
- What happens if people don't solve this problem?
- How do people deal with this today?

**About the customer:**
- Who specifically has this problem?
- What's their role/context when they feel this pain?
- How often do they encounter this problem?

**About the solution:**
- Why this approach vs. alternatives?
- What's the core thing it does (in one sentence)?
- What makes this different from existing solutions?

Use `AskUserQuestion` to gather these answers conversationally—don't dump all questions at once.

### Step 3: State Initial Hypotheses

Based on the conversation, help the user articulate three core hypotheses:

**Problem Hypothesis**
> We believe [specific customer] experiences [specific problem] when [specific context], causing [specific negative outcome].

**Customer Hypothesis**
> We believe our target customer is [description] who currently [workaround/behavior] because [reason].

**Solution Hypothesis**
> We believe [our solution] will solve [the problem] by [mechanism], which is better than alternatives because [differentiation].

See [references/hypothesis-templates.md](../references/hypothesis-templates.md) for more examples.

### Step 4: Generate Idea Brief

Create `idea-brief.md` in the project directory using the template at [templates/idea-brief.md](../templates/idea-brief.md).

Fill it with:
- The raw idea as stated
- Expanded context from the conversation
- The three stated hypotheses
- Initial assumptions to test

### Step 5: Transition to Problem Discovery

Summarize what we captured and preview the next phase:

> I've captured your idea in `idea-brief.md`. You're betting that [problem hypothesis summary].
>
> Next, let's research whether this problem actually exists and how painful it is. Ready to dig into problem discovery?

Proceed to [problem-discovery.md](problem-discovery.md) when the user confirms.

## Tips

- **Don't judge the idea.** Your job is to capture and structure it, not evaluate it. Validation comes later.
- **Push for specificity.** "People" becomes "engineering managers at Series A startups." "Sometimes" becomes "every Monday during sprint planning."
- **Hypotheses should be falsifiable.** If you can't imagine evidence that would disprove it, it's not specific enough.
