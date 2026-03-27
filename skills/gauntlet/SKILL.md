---
name: gauntlet
description: "Run a business idea through a 5-stage evaluation gauntlet — idea validation, market sizing, pricing architecture, team blueprint, and exit lens. The 'run everything' skill. Use when someone says 'evaluate this business,' 'run the gauntlet,' 'full business evaluation,' or brings an idea they want pressure-tested from every angle."
---

# The Gauntlet

Five stages. Each one kills bad ideas and sharpens good ones. You bring a business idea or opportunity — we run it through the full battery of frameworks from 793 episodes of My First Million.

This is the "run everything" skill. Each stage produces a clear pass/fail. After each stage, the user decides: move forward or go deeper.

## How It Works

Run stages sequentially. Do NOT skip ahead. Present each stage's result before moving to the next. After each stage, ask: **"Ready for the next stage, or want to go deeper on this one?"**

If they want to go deeper on any stage, point them to the full skill:
- Stage 1 → `/ask-sam:idea-vetter`
- Stage 2 → (built into idea-vetter filter 3)
- Stage 3 → `/ask-sam:pricing-optimizer`
- Stage 4 → `/ask-sam:hiring-framework`
- Stage 5 → `/ask-sam:exit-coach` and `/ask-sam:acquisition-evaluator`

---

## Stage 1: Idea Check

Three frameworks, run in order.

### The Thiel Test

From Imad Rahimi (Mercury, $3.5B) — "I Built A $1B Company... Here's 7 Business Ideas I Would Start This Year":

> "The best ideas come disguised as bad ideas. You're looking for the overlap between 'sounds like a bad idea' and 'actually a good idea.'"

Three sub-tests:
1. **Does it sound bad to most people?** If everyone loves it, the market is already crowded. Ask: "When you tell people this idea, do they get excited or confused?" Excitement is a yellow flag.
2. **Is there an inflection point?** Something changed — technology, regulation, culture — that makes this possible NOW but wasn't before. No inflection point = you're late.
3. **Does it scare people off?** Difficulty, weirdness, or stigma creates a natural moat. Easy ideas attract competition.

**Source:** `transcripts/mfm/2025-03-27-i-built-a-1b-company-heres-7-business-ideas-i-would-start-this-year.md`

### The Value Equation (Hormozi)

```
Value = (Dream Outcome x Perceived Likelihood) / (Time Delay x Effort Required)
```

Score each variable 1-5:
- **Dream Outcome (1-5):** How life-changing is the result for the customer?
- **Perceived Likelihood (1-5):** Does the customer believe it will work? What proof exists?
- **Time Delay (1-5, where 5 = instant):** How fast do they see results? Lipo scores 5. Personal training scores 2.
- **Effort Required (1-5, where 5 = zero effort):** How much work does the customer do?

Calculate: (Dream x Likelihood) / (Time x Effort). Above 4 is strong. Below 2 is a problem.

**Source:** `transcripts/mfm/2024-08-17-how-to-craft-a-100m-offer-in-6-minutes.md`

### The North Star Formula (Shaan)

> "I like when you can boil a plan down to a very simple equation. With Hampton: 'Ten thousand times ten thousand.' You just need 10,000 CEOs who will pay you $10,000 a year and you have a $100 million business."

Ask: "Can you express your entire business model in one multiplication?"

Examples:
- `1,000 customers x $500/month = $6M ARR`
- `50,000 units x $30 margin = $1.5M/year`
- `200 clients x $10,000/project = $2M/year`

If they can't compress it to one equation, the model is too complex. Push until they can.

**Source:** `transcripts/mfm/2023-04-04-how-to-buy-a-d2c-startup-for-cheap-and-sell-it-for-millions.md`

### Stage 1 Pass Criteria

Passes Thiel test (at least 2 of 3 sub-tests) **OR** scores 4+ on Value Equation **AND** has a clean North Star formula.

If it fails all three: stop here. The idea needs rethinking before the other stages matter.

---

## Stage 2: Market Sizing

One framework. Cold math.

### Unit Economics Check (Sam)

> "The math is basically: how valuable is the purchase price of the product, multiplied by the frequency one person buys it, multiplied by the number of people who have that need."

Have the user fill in:
- **Price per unit/transaction:** $___
- **Purchase frequency:** ___ times per [year/month/lifetime]
- **Total addressable buyers:** ___
- **Realistic capture rate:** ___% (be conservative — 1-5% of TAM is common for startups)

Calculate: **Price x Frequency x TAM x Capture Rate = Revenue Ceiling**

Then the reality check:
- **Ceiling < $100K/year:** That's a hobby, not a business. Fine if you know that going in.
- **Ceiling $100K-$1M/year:** Lifestyle business. Can be great — but it won't attract investors or top talent. Know what you're building.
- **Ceiling > $1M/year:** Real business territory.
- **Ceiling > $10M/year:** Venture-scale if the capture rate holds.

Then ask: **"What does it cost you to acquire one customer?"**

If they don't know (most don't), prescribe Sam's test: run $500 in ads or 100 cold outreach messages. Measure cost per sign-up. That's your real CAC — not the theoretical one.

**CAC sanity check:** If CAC > 30% of first-year revenue per customer, the unit economics don't work without significant retention.

**Source:** `transcripts/mfm/2022-06-03-follow-these-3-steps-to-start-a-1000000-lead-generation-business.md`

### Stage 2 Pass Criteria

Revenue ceiling > $1M/year with a capture rate you can defend. If ceiling is $100K-$1M, flag it as a lifestyle business (not a kill — just a label). Below $100K, this stage fails.

---

## Stage 3: Pricing Architecture

Three frameworks for getting the price right.

### The Three Levers (Patrick Campbell / ProfitWell)

From hundreds of thousands of willingness-to-pay data points:

> "Revenue per customer should be going up and to the right. The average time between price increases is three years. I've seen so many companies leave money on the table because they're scared."

Most founders underwork monetization. Acquisition gets all the attention. The three levers:

1. **Add-Ons:** "Add-ons boost lifetime value by 20-50%. Most high-growth subscription companies have 12 or more add-ons." Ask: What could you sell alongside the core product? Priority support, white-glove onboarding, custom reporting, done-for-you services.
2. **Localization:** "The Nordics are willing to pay ~30% higher than the US for the exact same product." If selling internationally, geo-based pricing (even just 3-4 tiers) captures 15-20% more revenue.
3. **Tiering:** Create Good/Better/Best where the middle tier is the one you want most people to buy. The top tier exists to make the middle feel reasonable (anchoring).

**Source:** `transcripts/mfm/2023-11-16-brainstorming-ideas-with-the-200m-man-ft-patrick-campbell-519.md`

### Price Sensitivity Test

Two questions to ask 10-20 potential customers:
1. "At what price would this be so cheap you'd question the quality?"
2. "At what price would this be so expensive you'd never buy it?"

The sweet spot is between those two numbers, biased toward the upper end. From Shaan: "Unless half the people are saying no, you're priced way too low."

**Source:** `transcripts/mfm/2022-01-25-coaching-our-producer-to-make-5000hour-with-consulting.md`

### The Add-On Strategy

Map it out:
- **Core product:** What's the base offering? Price: $___
- **Premium add-ons:** What 2-3 things could you charge extra for? Price each.
- **Enterprise/VIP tier:** What does the "I want everything" package look like? Price: $___

Rule of thumb: if your product has fewer than 3 upsell options, you're leaving 20-50% of LTV on the table.

### Stage 3 Pass Criteria

Clear pricing model with at least one add-on path identified. If the user says "I'll just charge one price for one thing" — that's a warning, not a pass.

---

## Stage 4: Team Blueprint

Three frameworks for the people side.

### First 3 Hires (Hormozi)

> Hire for the role you're worst at first.

Ask the user:
1. "What are you best at — product, sales, or operations?"
2. "What do you hate doing or constantly avoid?"

The first hire covers the founder's weakness. The second hire scales the founder's strength (so the founder can focus on strategy). The third hire is the one that makes the business run without the founder being in every meeting.

Map it:
- **Hire #1:** ___ (covers founder weakness) — Role: ___, Est. cost: $___/year
- **Hire #2:** ___ (scales founder strength) — Role: ___, Est. cost: $___/year
- **Hire #3:** ___ (operations/independence) — Role: ___, Est. cost: $___/year

**Source:** `transcripts/mfm/2025-11-14-alex-hormozis-best-frameworks-for-business-and-beyond.md`

### Cost Model

Simple math:
- **Total annual salary burden:** Hire 1 + Hire 2 + Hire 3 = $___/year
- **Revenue needed to cover team:** At target margin, that's $___/year in revenue
- **Timeline to self-sustaining:** Based on Stage 2 growth assumptions, the team pays for itself by month ___

If the team costs more than projected Year 1 revenue, the user is either hiring too fast or needs to bootstrap with contractors first.

### Contractor vs. FTE Decision

Use Blake's "teach me something" test for critical hires:

> "My favorite interview question is 'teach me something.' You do that two or three times — push back, say 'I don't understand, walk me through it' — and you undress people that way."

**Rule:** If the role requires deep domain expertise (the person needs to teach YOU things about the business), hire FTE. If the role is execution of a known playbook (you could teach THEM), use a contractor.

**Source:** `transcripts/mfm/2025-05-07-how-i-got-5-billion-in-preorders-for-a-supersonic-jet-company.md`

### Stage 4 Pass Criteria

First 3 hires identified with a funding path that doesn't require the business to be profitable on day one but doesn't require 3 years of runway either. If the user can't name who they'd hire first, this stage needs work.

---

## Stage 5: Exit Lens

Two frameworks. You should know the ending before you start.

### Buyer Profile

Who buys this business? Three categories:

1. **Strategic Acquirer** (competitor or adjacent company): They're buying your customers, your technology, or your market position. Pays the highest multiples because the value to them exceeds the standalone value. Sam sold The Hustle to HubSpot — a strategic acquisition.
2. **PE Firm** (financial buyer / rollup): They're buying cash flow. They want stable, predictable revenue with room to optimize. Pays 3-7x EBITDA for small businesses. Good if you're building a boring, profitable machine.
3. **Individual Buyer** (operator/lifestyle): They're buying a job they own. Pays 2-4x SDE. Good for businesses under $5M revenue where the owner IS the business.

Ask: "Which of these three is most likely to want YOUR business? Why?"

If the answer is "nobody" — that's not necessarily fatal (some businesses are better as hold-forever cash machines), but the user should know that going in.

**Source:** `transcripts/mfm/2022-03-18-i-sold-my-company-for-millions-heres-what-i-got-wrong.md` (Sam/Shaan exit debrief)

### Valuation Method

From James Altucher and multiple acquisition episodes:

Three approaches to know:
1. **Earnings Multiple** (most common): Annual profit x industry multiple. SaaS: 5-15x ARR. Service businesses: 2-5x profit. E-commerce: 2-4x profit. Boring businesses: 2.5-4x SDE.
2. **Comparable Transactions:** What did similar businesses sell for? Search BizBuySell, Acquire.com, or MFM episodes for comps.
3. **Strategic Premium:** If a buyer NEEDS what you have (customer list, technology, team), the multiple goes up 2-3x over standard earnings.

Ask: "Based on your Stage 2 revenue ceiling and this valuation framework, what's this business worth in 3-5 years?"

### Exit Timeline

> "Know your exit before you start." — Sam Parr

Three options:
- **3-year flip:** Build fast, get to profitability, sell to PE or strategic. Optimize for growth rate and clean books.
- **5-year build:** Build a real brand, grow the team, create something defensible. Optimize for market position and recurring revenue.
- **Hold forever:** Never sell. Optimize for cash flow and lifestyle. This is a valid choice — most great businesses are never sold.

Ask: "Which timeline fits your life right now?"

**Source:** `transcripts/mfm/2022-03-18-i-sold-my-company-for-millions-heres-what-i-got-wrong.md`, `transcripts/mfm/2023-11-02-how-i-bought-a-multi-million-dollar-egg-carton-business-for-0-sarah-moore-interv.md`

### Stage 5 Pass Criteria

At least one plausible buyer category identified AND a valuation method that produces a number the user finds motivating. If they're building a hold-forever business, the "exit" is the annual cash flow — that's still a pass.

---

## The Gauntlet Report

After all 5 stages, produce this report:

```markdown
# Gauntlet Report: [Business Name/Idea]

## Stage Results
| Stage | Result | Key Finding |
|-------|--------|-------------|
| Idea Check | [pass]/[warn]/[fail] | [one line] |
| Market Sizing | [pass]/[warn]/[fail] | [one line] |
| Pricing | [pass]/[warn]/[fail] | [one line] |
| Team | [pass]/[warn]/[fail] | [one line] |
| Exit | [pass]/[warn]/[fail] | [one line] |

## Overall Assessment
[2-3 paragraphs. Be blunt. "Here's where this breaks" not "this might face challenges."
Use specific numbers from the stages. Reference the frameworks by name.
If it passed everything, say what makes it strong AND what could still kill it.
If it failed stages, say exactly which assumptions need to change for it to work.]

## Go Deeper
[List the full skills to run for the weakest 1-2 stages, e.g.:]
- Pricing was the weakest stage. Run `/ask-sam:pricing-optimizer` for the full Patrick Campbell framework and quarterly pricing calendar.
- Your first 3 hires are unclear. Run `/ask-sam:hiring-framework` for role-specific interview design.

## Source Episodes
[List every episode referenced across all 5 stages with titles]
```

Use these result markers:
- **pass** = solid, move forward with confidence
- **warn** = passable but has a known weakness — flag it
- **fail** = this stage broke — fix it before proceeding

## Deep-Dive References

When the gauntlet reveals a weak stage, point the user to these references in addition to the full skill:

- Read `references/frameworks/million-dollar-business-ideas.md` for proven idea patterns (Stage 1 remediation)
- Read `references/frameworks/saas-metrics.md` for SaaS market sizing benchmarks (Stage 2 remediation)
- Read `references/frameworks/customer-exclusion-policy.md` for narrowing the customer to improve pricing (Stage 3)
- Read `references/frameworks/co-founder-alignment.md` for co-founder fit before hiring (Stage 4)
- Read `references/frameworks/three-method-company-valuation.md` for valuation methodology (Stage 5)
- Read `references/frameworks/boring-businesses.md` for the boring business thesis if the idea is too exciting
- Read `references/frameworks/one-to-two-dollar-machine.md` for unit economics sanity check

## Voice

Write like Sam talks: blunt, specific numbers, no hedging. "Your revenue ceiling is $400K — that's a lifestyle business, not a venture play" beats "the market opportunity may be somewhat limited." Call things what they are.
