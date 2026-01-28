# Phase 3: Customer Discovery

Define who has this problem using earlyvangelist criteria and identify your market type.

## Goal

Move from "people have this problem" to "these specific people have this problem severely enough to pay for a solution."

Define:
- Who exactly is your target customer?
- What makes them an earlyvangelist (early adopter who'll co-develop)?
- What market type are you entering?

## Process

### Step 1: Segment Potential Customers

From the problem discovery research, identify distinct customer segments:

> Based on our research, here are the segments that seem to experience this problem:
>
> 1. [Segment A] - [brief description, pain indicators]
> 2. [Segment B] - [brief description, pain indicators]
> 3. [Segment C] - [brief description, pain indicators]
>
> Which of these resonates most with who you want to build for?

Use `AskUserQuestion` with options for each segment plus "Other."

### Step 2: Apply Earlyvangelist Criteria

For the chosen segment, evaluate against the five earlyvangelist characteristics:

See [references/earlyvangelist-scale.md](../references/earlyvangelist-scale.md)

| Criterion | Question | Evidence |
|-----------|----------|----------|
| **Has the problem** | Do they actively experience this pain? | |
| **Knows they have it** | Are they aware and articulate about it? | |
| **Has been seeking solution** | Have they looked for alternatives? | |
| **Has budget** | Can they pay (or influence payment)? | |
| **Can cobble together workaround** | Have they built something themselves? | |

An earlyvangelist scores high on all five. If your segment doesn't, consider:
- Narrowing the segment further
- Looking at a different segment
- Redefining who within the segment meets criteria

### Step 3: Identify Market Type

Market type changes everything about how you compete and grow.

See [references/market-types.md](../references/market-types.md)

**Existing Market**
- Competitors exist with defined features
- Customers know what they want
- You compete on better/faster/cheaper
- Sales cycle is shorter but competition is fierce

**New Market**
- No direct competitors
- Customers don't know they need this
- You compete on vision and education
- Long sales cycle, but can own the market

**Resegmented Market**
- Take existing market, focus on niche or different value prop
- Either low-cost (underserve mainstream) or niche (overserve specific segment)
- Positioning is everything

Ask the user:

> Based on our research, where does this fit?
>
> 1. **Existing market** - There are competitors doing similar things
> 2. **New market** - Nothing like this exists yet
> 3. **Resegmented** - Competitors exist but you're targeting a specific niche or different value prop

Use `AskUserQuestion` and discuss implications of their choice.

### Step 4: Build Customer Profile

Synthesize everything into a detailed customer profile:

**Demographics/Firmographics**
- Role, seniority, team size
- Company type, size, industry
- Geography, technical environment

**Psychographics**
- Goals and motivations
- Fears and frustrations
- How they evaluate solutions

**Behavioral**
- Where they spend time (online/offline)
- How they buy (process, influencers)
- Current tools and workflows

**Earlyvangelist Signals**
- Specific behaviors that indicate level 4-5 pain
- Where to find them
- How to identify them quickly

### Step 5: Generate Customer Profile

Create `customer-profile.md` in the project directory using the template at [templates/customer-profile.md](../templates/customer-profile.md).

### Step 6: Transition to Solution Fit

Summarize and preview next phase:

> I've documented your target customer in `customer-profile.md`.
>
> You're targeting [customer summary] who experience [problem] at pain level [X]. This is a [market type] market, which means [key implication].
>
> Now let's test whether your proposed solution actually fits this validated problem. Ready?

Proceed to [solution-fit.md](solution-fit.md) when confirmed.

## Tips

- **Earlyvangelists aren't mainstream.** They're weird in a good way—more pain tolerant, more visionary. Don't try to make them normal.
- **Budget authority matters.** Someone who feels the pain but can't buy is a reference, not a customer.
- **Market type isn't a choice—it's a discovery.** Be honest about what the research shows, not what you wish.
- **One segment to start.** Even if multiple segments have the problem, pick ONE for your MVP. Expand later.
