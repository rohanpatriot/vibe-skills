# Phase 5: MVP Definition

Define the minimum feature set for earlyvangelists, map features to problems, and generate customer development tasks.

## Goal

Create a concrete MVP specification that:
- Targets earlyvangelists specifically (not mainstream)
- Maps every feature to a validated problem
- Excludes everything that isn't essential for learning
- Includes tasks for continued customer development

## Process

### Step 1: Review What We Know

Summarize the journey:

> Here's what we've validated:
>
> **Problem:** [Problem statement]
> **Customer:** [Earlyvangelist profile summary]
> **Solution:** [Solution approach]
> **Market Type:** [Existing/New/Resegmented]
>
> Now let's scope the MVP.

### Step 2: Define MVP Principles

Remind the user of MVP philosophy:

**For Earlyvangelists, Not Mainstream**
- Earlyvangelists tolerate rough edges
- They want the core value, not polish
- They'll give you feedback; mainstream users won't

**Minimum = Just Enough to Learn**
- What's the smallest thing that tests our hypotheses?
- What would we learn from putting this in front of customers?
- What can we skip and add later based on feedback?

**Features Map to Problems**
- Every feature should address a validated problem
- If a feature doesn't map, cut it or justify why it's essential

### Step 3: Brainstorm Feature Candidates

Generate potential features with the user:

> What features come to mind for the MVP? Let's list them all first, then prioritize.

Capture their list, then probe for missing essentials:

> What about [obvious capability]? Is that needed for the core value?

### Step 4: Map Features to Problems

Create explicit mapping for each candidate feature:

| Feature | Problem It Solves | Essential for MVP? | Notes |
|---------|-------------------|-------------------|-------|
| [Feature 1] | [Problem] | Yes/No | [Reasoning] |
| [Feature 2] | [Problem] | Yes/No | [Reasoning] |
| [Feature 3] | [Problem] | Yes/No | [Reasoning] |
| [Feature 4] | None - nice to have | No | Cut |

Discuss with user:

> Here's the feature mapping:
>
> [Show table]
>
> Features without clear problem mapping are candidates for cutting. Features marked "No" can wait for v2.
>
> Does this prioritization feel right?

Use `AskUserQuestion` to finalize the feature set.

### Step 5: Define Success Criteria

For the MVP, what signals success?

**Learning Goals**
- What hypotheses does this MVP test?
- What would make us confident to proceed?
- What would make us pivot?

**Metrics** (if applicable)
- Usage signals (signups, activation, retention)
- Feedback signals (NPS, qualitative themes)
- Business signals (willingness to pay, conversion)

Ask the user:

> What would success look like for this MVP? What would tell you it's working vs. not?

### Step 6: Generate Customer Development Tasks

The MVP isn't just code—it's learning. Generate tasks for continued validation:

**Before Building**
- [ ] Interview [N] potential earlyvangelists about the problem
- [ ] Show mockups/prototypes to [N] people for feedback
- [ ] Validate pricing/willingness to pay with [approach]

**During Building**
- [ ] Share progress with [N] earlyvangelists for input
- [ ] Test [specific assumption] with [method]
- [ ] Recruit beta users from [channel]

**After Launching MVP**
- [ ] Collect feedback from first [N] users
- [ ] Track [specific metrics]
- [ ] Run [type of test] to validate [hypothesis]

Customize based on the specific idea and customer profile.

### Step 7: Generate Output Files

Create two files in the project directory:

**`mvp-spec.md`** using template at [templates/mvp-spec.md](../templates/mvp-spec.md):
- MVP features with problem mapping
- What's explicitly out of scope
- Success criteria
- Key assumptions being tested

**`custdev-tasks.md`** using template at [templates/custdev-tasks.md](../templates/custdev-tasks.md):
- Pre-build tasks
- During-build tasks
- Post-launch tasks
- Interview questions and scripts

### Step 8: Transition to Build Planning

Summarize and offer handoff:

> Your MVP is defined in `mvp-spec.md` with [N] core features targeting earlyvangelists.
>
> Customer development tasks are in `custdev-tasks.md`—I recommend starting these before (or while) you build.
>
> **Ready to plan the build?** I can run `/planning-setup` to create a task plan, findings log, and progress tracker for implementation.
>
> Or you can:
> 1. Start customer development first (recommended!)
> 2. Review the outputs and come back when ready
> 3. Jump into building on your own

Use `AskUserQuestion` with these options.

> **Note:** For complex implementation work, Claude will use plan mode to design the technical approach before coding.

If they choose planning-setup, invoke the skill:

> Great! Running `/planning-setup` to set up build planning...

## Tips

- **Cut aggressively.** The hardest part of MVP definition is saying no. Less is more.
- **Features aren't value.** A feature is code; value is a problem solved. Always trace back to the problem.
- **Earlyvangelists want speed, not polish.** Ship something ugly that solves their problem over something beautiful that doesn't.
- **Customer development is ongoing.** The MVP is a tool for learning, not a product launch. Keep talking to customers.
