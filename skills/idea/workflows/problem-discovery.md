# Phase 2: Problem Discovery

Research whether the problem actually exists, how painful it is, and what workarounds people use today.

## Goal

Validate (or invalidate) the problem hypothesis by gathering evidence:
- Does this problem actually exist?
- How painful is it (using the earlyvangelist scale)?
- What are people doing about it today?
- Is there market evidence of demand?

## Process

### Step 1: Define Research Questions

Based on the problem hypothesis from Phase 1, identify what we need to learn:

1. **Existence**: Is there evidence people experience this problem?
2. **Frequency**: How often does it occur?
3. **Severity**: What's the impact when it happens?
4. **Workarounds**: What do people do about it today?
5. **Spend**: Is anyone paying to solve this already?

### Step 2: Research the Problem Space

Use subagents to investigate. Spawn an Explore agent to:

**Search for problem evidence:**
- Forum discussions, Reddit threads, Stack Overflow questions
- Blog posts describing the pain
- Social media complaints
- Support tickets / public issue trackers

**Analyze existing solutions:**
- Direct competitors
- Adjacent tools people repurpose
- DIY solutions and workarounds
- Failed products in this space (and why they failed)

**Check market signals:**
- Search volume for related terms
- Funding in the space
- Job postings mentioning the problem
- Conference talks / content about the topic

Example research prompt for subagent:
> Research the problem space for [problem hypothesis]. Find evidence of: (1) people experiencing this problem, (2) existing solutions or workarounds, (3) market demand signals. Search forums, Reddit, product sites, and industry content.

### Step 3: Assess Problem Severity

Using the research findings, assess where potential customers fall on the earlyvangelist pain scale:

See [references/earlyvangelist-scale.md](../references/earlyvangelist-scale.md)

| Level | Description | Evidence |
|-------|-------------|----------|
| 1 | Latent problem - don't know they have it | No searches, no complaints |
| 2 | Passive problem - know it, live with it | Occasional mentions, no action |
| 3 | Active problem - seeking solutions | Searching, asking questions |
| 4 | Urgent problem - built workarounds | DIY solutions, scripts, hacks |
| 5 | Critical problem - allocated budget | Paying for imperfect solutions |

**You need level 4-5 customers for an MVP to work.** Levels 1-3 require education before sales.

### Step 4: Document Findings

Ask the user to review findings and discuss:

> Here's what I found about the problem space:
>
> **Evidence the problem exists:** [summary]
>
> **Current workarounds:** [summary]
>
> **Pain level assessment:** [1-5 with reasoning]
>
> **Market signals:** [summary]
>
> Does this match your understanding? Anything surprising?

### Step 5: Decision Point

Based on evidence, one of three paths:

**A. Problem validated (Level 4-5 pain found)**
> The problem is real and painful. People are building workarounds and/or spending money. Let's move to customer discovery to define exactly who we're building for.

Proceed to [customer-discovery.md](customer-discovery.md).

**B. Problem exists but weak (Level 2-3 pain)**
> The problem exists, but the pain isn't acute. We have options:
> 1. Find a more specific segment where pain is higher
> 2. Pivot to an adjacent, more painful problem
> 3. Continue knowing we'll need to educate the market

Use `AskUserQuestion` to decide direction.

**C. Problem not validated (Level 1 or no evidence)**
> I couldn't find strong evidence this problem exists or matters. This is valuable learning! Options:
> 1. Refine the problem hypothesis and research again
> 2. Pivot to a different problem you've observed
> 3. Continue based on your direct experience (higher risk)

Use `AskUserQuestion` to decide direction.

## Tips

- **Look for workarounds, not complaints.** Complaining is cheap. Building a hacky solution means real pain.
- **Failed products are gold.** They prove the problem existed; learn why the solution didn't work.
- **Absence of evidence isn't proof of absence.** Maybe you're searching wrong, or the market is nascent.
- **Trust direct observation.** If you've personally experienced the problem, that's data too—but one data point isn't a market.
