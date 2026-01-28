# Phase 4: Solution Fit

Test whether your proposed solution actually solves the validated problem for your target customer.

## Goal

Before defining features, validate that your solution approach fits:
- Does the solution address the core problem?
- Does it work for your specific customer segment?
- Is the approach differentiated enough?

## Process

### Step 1: Revisit the Solution Hypothesis

Pull the solution hypothesis from the idea brief:

> Your original solution hypothesis was:
>
> "[Solution hypothesis from idea-brief.md]"
>
> Now that we've validated the problem and defined the customer, let's test if this still makes sense.

### Step 2: Map Solution to Problem

Create an explicit mapping:

| Validated Problem | How Solution Addresses It | Gap? |
|-------------------|---------------------------|------|
| [Problem aspect 1] | [How solution helps] | [Yes/No + notes] |
| [Problem aspect 2] | [How solution helps] | [Yes/No + notes] |
| [Problem aspect 3] | [How solution helps] | [Yes/No + notes] |

Discuss with the user:

> Here's how your solution maps to the validated problem:
>
> [Show table]
>
> I see [X] gaps. Should we address these, or are they out of scope for MVP?

### Step 3: Check Customer Fit

Evaluate solution against earlyvangelist characteristics:

**Workflow Fit**
- Does it integrate with how they work today?
- What would they need to change?
- Is the change worth the benefit?

**Technical Fit**
- Does it work in their environment?
- Any blockers (security, compliance, integration)?
- Do they have the skills to adopt it?

**Economic Fit**
- Can they afford it?
- Does the value justify the cost?
- How does ROI compare to alternatives?

Ask the user about any concerns:

> A few fit questions:
>
> 1. How does this fit into your customer's existing workflow?
> 2. Any technical constraints to consider?
> 3. What would they pay for this (roughly)?

### Step 4: Competitive Differentiation

If existing or resegmented market, validate differentiation:

> Your competitors include [from research]. Here's how your solution differs:
>
> | Factor | Competitors | Your Solution |
> |--------|------------|---------------|
> | [Factor 1] | [How they do it] | [Your approach] |
> | [Factor 2] | [How they do it] | [Your approach] |
>
> Is this differentiation meaningful to your target customer?

For new markets, differentiation is less relevant—validation is about whether the approach resonates at all.

### Step 5: Identify Solution Risks

Surface assumptions that could kill the solution:

**Technical Risks**
- Can this actually be built?
- Are there dependencies outside your control?
- What's the hardest technical challenge?

**Market Risks**
- Will customers understand this?
- Is the behavior change too large?
- Is timing right (too early? too late?)?

**Execution Risks**
- Do you have the skills to build this?
- What resources are needed?
- What could delay or derail you?

Discuss the top 2-3 risks:

> The biggest risks I see for this solution are:
>
> 1. [Risk] - because [reason]
> 2. [Risk] - because [reason]
>
> How would you address these?

### Step 6: Decision Point

Based on fit analysis, one of three paths:

**A. Solution fits well**
> Your solution addresses the core problem for your target customer with meaningful differentiation. Let's move to MVP definition to scope what to build first.

Proceed to [mvp-definition.md](mvp-definition.md).

**B. Solution fits with adjustments**
> The core approach is sound, but we should adjust:
>
> [List recommended adjustments]
>
> Should we update the solution hypothesis and continue, or explore alternatives?

Use `AskUserQuestion` to decide direction.

**C. Solution doesn't fit**
> There's a significant gap between your solution and the validated problem/customer. Options:
>
> 1. Pivot the solution to better address the problem
> 2. Revisit customer discovery to find a better-fit segment
> 3. Go back to problem discovery with a new angle

Use `AskUserQuestion` to decide direction.

## Tips

- **Fit isn't about perfection.** It's about whether the core value proposition works. Edge cases are for later.
- **Listen to the gaps.** Where solution doesn't map to problem is where pivots hide.
- **Differentiation must matter.** Being different isn't enough; it must be different in a way customers value.
- **Risks are hypotheses.** Just like the idea itself, they need testing—but acknowledge them now.
