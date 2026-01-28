# Hypothesis Templates

Ideas are hypotheses, not facts. Stating them explicitly makes them testable. Here are templates for articulating your assumptions.

## The Three Core Hypotheses

Every idea rests on three fundamental bets:

### 1. Problem Hypothesis

> We believe **[specific customer]** experiences **[specific problem]** when **[specific context]**, causing **[specific negative outcome]**.

**Examples:**

> We believe **engineering managers at Series A startups** experience **difficulty tracking developer productivity** when **preparing for board meetings**, causing **hours of manual data collection and uncertainty in reporting**.

> We believe **freelance designers** experience **scope creep from clients** when **project requirements aren't documented upfront**, causing **unpaid work and damaged relationships**.

> We believe **parents of toddlers** experience **mealtime stress** when **children refuse to eat prepared food**, causing **wasted food, wasted time, and family tension**.

**What makes it testable:**
- Specific customer (not "people" or "users")
- Specific context (when does this happen?)
- Specific outcome (what's the cost of the problem?)

---

### 2. Customer Hypothesis

> We believe our target customer is **[description]** who currently **[workaround/behavior]** because **[reason]**.

**Examples:**

> We believe our target customer is **solo founders building their first SaaS** who currently **use spreadsheets to track metrics** because **existing analytics tools are too expensive or complex**.

> We believe our target customer is **senior developers at large companies** who currently **write custom scripts to enforce code standards** because **existing linters don't cover their team's specific conventions**.

> We believe our target customer is **small restaurant owners** who currently **manually reconcile delivery app orders** because **none of the apps integrate with their POS system**.

**What makes it testable:**
- Observable behavior (what they do today)
- Reason for behavior (why they do it that way)
- Segment specificity (who exactly)

---

### 3. Solution Hypothesis

> We believe **[our solution]** will solve **[the problem]** by **[mechanism]**, which is better than alternatives because **[differentiation]**.

**Examples:**

> We believe **an automated metrics dashboard** will solve **the productivity tracking problem** by **pulling data directly from GitHub, Jira, and Slack**, which is better than alternatives because **managers get real-time visibility without asking engineers to self-report**.

> We believe **a template-based scope document generator** will solve **the scope creep problem** by **creating client-facing contracts from intake questions**, which is better than alternatives because **designers don't need to learn contract law or spend hours on proposals**.

> We believe **a meal planning app with kid-friendly recipes** will solve **mealtime stress** by **suggesting nutritionally-balanced meals kids actually eat, based on preference data**, which is better than alternatives because **existing apps don't optimize for picky eaters**.

**What makes it testable:**
- Clear mechanism (how it works)
- Explicit differentiation (why this vs. alternatives)
- Connection to validated problem

---

## Secondary Hypotheses

Beyond the core three, you may need to test:

### Channel Hypothesis
> We believe we can reach **[target customers]** through **[channel]** because **[evidence/reasoning]**.

### Pricing Hypothesis
> We believe **[target customers]** will pay **[$X/model]** for **[solution]** because **[value justification]**.

### Retention Hypothesis
> We believe customers will continue using **[solution]** because **[ongoing value/switching cost]**.

### Viral/Growth Hypothesis
> We believe **[mechanism]** will cause existing users to bring **[N]** new users because **[reason]**.

---

## Hypothesis Quality Checklist

A good hypothesis is:

| Quality | Question | Fix If Not |
|---------|----------|------------|
| **Specific** | Can two people read this and have the same understanding? | Remove ambiguous words |
| **Falsifiable** | Can you imagine evidence that would disprove it? | Add measurable criteria |
| **Testable** | Could you run an experiment to validate this? | Make it more concrete |
| **Important** | If this is wrong, does it change your approach? | If not, don't test it |

---

## From Hypothesis to Test

Each hypothesis implies a test:

| Hypothesis Type | Test Approach |
|-----------------|---------------|
| Problem | Customer interviews, surveys, forum research |
| Customer | Segment analysis, earlyvangelist identification |
| Solution | Prototypes, landing page tests, pilot programs |
| Channel | Small-scale experiments in each channel |
| Pricing | Willingness-to-pay interviews, pricing page tests |

---

## Common Hypothesis Mistakes

**Too vague:**
> "We believe users have trouble managing their tasks."

**Better:**
> "We believe product managers at B2B SaaS companies experience dropped balls when managing feature requests across multiple channels (Slack, email, support tickets), causing delays and frustrated customers."

**Not falsifiable:**
> "We believe people want better tools."

**Better:**
> "We believe engineering teams with 10-50 developers will pay $500/month for a tool that reduces code review cycle time by 50%."

**Assumed conclusion:**
> "We believe our app is the best solution."

**Better:**
> "We believe our async-first approach will outperform competitors for remote teams because it doesn't require scheduling meetings across time zones."
