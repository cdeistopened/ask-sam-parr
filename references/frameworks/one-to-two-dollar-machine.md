---
name: The $1 Into $2 Machine
description: Walk someone through evaluating whether their business has found a unit economics machine — a model that reliably turns $1 of investment into $2 of return — and help them decide whether to pour in capital or hold back. Use when someone is deciding whether to raise money, hire aggressively, or scale spending. Also use when someone says their business is growing but they're unsure whether to keep investing in growth. Trigger phrases include "should I raise?", "should I be spending more on marketing?", "how do I know if my unit economics work?", "is it time to scale?", or "I keep hiring but I don't know if it's paying off."
type: framework
domain: frameworks
status: published
episodes:
  - 0cLWUCE02KE
date_created: 2026-03-04
source_guests:
  - Kevin Ryan
---

# The $1 Into $2 Machine

Walk someone through Kevin Ryan's investment decision framework — the mental model that drove AlleyCorp's four billion-dollar companies out of a single studio. The question is never "should I spend money?" The question is: have you built a machine that reliably turns $1 into $2?

## When to Use

The user is trying to decide whether to invest more capital — in people, in marketing, in expansion — or is uncertain whether their unit economics justify scaling. They might say:

- "Should I raise money right now?"
- "I'm not sure if I should keep hiring"
- "How do I know when to pour it on?"
- "Is my marketing working well enough to scale?"
- "We're growing but I don't know if we're spending the right amount"
- "Should I be losing money to grow faster?"

## The Core Principle

From Sam Parr (`0cLWUCE02KE.md`), paraphrasing Kevin Ryan's framework:

> "If my idea is good enough, I'm going to build a machine that turns $1 into $2. And if I have that machine, what are you going to do? You're going to go get as much money as you can and back that truck up into that machine and dump it in there." — Sam Parr, paraphrasing Kevin Ryan

The machine test is binary: either you have it or you don't. If you do, the only rational move is to dump as much fuel into it as possible. If you don't, spending more money is just burning cash.

Ryan ran this logic at DoubleClick — expanding to 25 countries before a single country was profitable — and it swept the market. The machine worked. He backed the truck.

## Step 1: Find the Repeatable Unit

Before you can test the machine, you need to isolate the repeatable unit — the action that, when you spend money, produces a predictable return.

> "If you have a salesperson who costs $150,000 and they're selling $500,000 worth, you need to hire those people all day long. Because you have an opportunity." — Kevin Ryan

**Ask the user:**

- What is the repeatable unit in your business? (A salesperson, an ad campaign, a new market, a new product line)
- What does it cost to add one unit?
- What does one unit produce in revenue, on what timeline?

| Unit | Input Cost | Output Revenue | Timeline | Ratio |
|------|-----------|----------------|----------|-------|
| Salesperson | $150K/yr | $500K/yr | 12 months | 3.3x |
| Ad campaign | $10K/mo | $25K/mo | 30 days | 2.5x |
| New market | $500K | $1.2M | 18 months | 2.4x |

If the ratio is above 2x and the timeline is acceptable, you have a machine. Below 1.5x or unpredictable — you don't.

## Step 2: Test the Machine at Small Scale

Don't scale before you've confirmed the machine is real. The machine only works if the numbers hold as you add units.

**Ask the user:**

- Have you proven this unit economics model more than once? (One data point is not a machine.)
- Does the ratio hold when you add a second salesperson, a second campaign, a second market?
- Is your CAC (customer acquisition cost) stable, or does it creep up as you spend more?

The danger signal: the first unit looks great, but the second and third perform worse. This means you've skimmed the most efficient opportunity and the machine is market-constrained.

**Output:** A simple table showing the last 3-5 units deployed and their returns. If the ratio is consistent, the machine is real.

## Step 3: Run the Dilution Test

Before raising capital to pour into the machine, Ryan's framework demands one more calculation: does the dilution cost less than the machine produces?

> "Let's say you're going to raise $2 million at a $20 million valuation. You're going to dilute 10%. You just have to ask yourself: if I took that $2 million and invested it into growth over the next 18 months, is our company going to be worth more than 10% versus if we do not? And if it is, then I need to do that trade. And if it's not, I should not." — Kevin Ryan (paraphrased from Sam Parr's notes)

**Run this math with the user:**

| Item | Amount |
|------|--------|
| Capital being raised | $X |
| Equity being given up | Y% |
| Current implied valuation | $X / Y% |
| Machine return in 18 months | Z% increase in value |
| Net: is Z% > Y%? | Go / No-Go |

If the machine produces value faster than the dilution costs, the trade is correct. If not, don't raise — or raise less.

## Step 4: Know When to Stop Pumping

The machine test also tells you when to stop. Ryan has cut 30% of headcount at companies where the machine stopped working.

> "There are times in various companies where it doesn't make sense to invest a lot more money because we're not getting the return. You run out of market share, it's not as big a market as you think, something's not working as well. And so then the right thing to do is to not invest." — Kevin Ryan

Signs the machine has stopped working:

- CAC is rising faster than revenue per customer
- New markets or campaigns are underperforming earlier ones
- You're hiring salespeople but pipeline isn't growing proportionally
- Payback period is extending

**Ask the user:** Have you run the same unit test on your most recent hires / campaigns / markets as you ran on the first ones? What did the numbers show?

If the machine is slowing, hold. Don't keep pouring money into a machine that's broken.

## Step 5: Decide: Back the Truck or Hold

After the machine test, the answer should be clear:

| Condition | Decision |
|-----------|---------|
| Machine is real, dilution math works, units are consistent | Back the truck — raise and deploy aggressively |
| Machine is real, but dilution math doesn't work | Grow from cash flow, raise later at a better valuation |
| Machine is uncertain — too few data points | Prove it at small scale before raising |
| Machine is broken — CAC rising, returns falling | Cut spending, fix the model, then retest |
| Machine never existed — no repeatable unit | Stop scaling. Find the machine first. |

## Quick Reference

| Step | Question | Signal |
|------|---------|--------|
| 1. Find the unit | What repeatable thing produces $2 from $1? | A salesperson, campaign, or market with a >2x return |
| 2. Test it | Does the ratio hold across multiple instances? | Consistency = machine is real |
| 3. Dilution test | Is the raise worth the equity? | Machine return > dilution cost |
| 4. Know when to stop | Is the machine still working? | CAC rising = machine breaking |
| 5. Decide | Back the truck or hold? | Binary: all in or fix first |

## Search the Archive

```
grep -ri "unit economics\|CAC\|cost per acquisition\|back the truck" transcripts/
grep -ri "raise money\|when to scale\|hire fast\|losing money.*investing" transcripts/
grep -ri "Kevin Ryan\|AlleyCorp\|DoubleClick\|MongoDB" transcripts/
```

## Output

After the session, deliver:

1. **Unit table** — the repeatable unit identified, with input cost, output revenue, and ratio
2. **Machine verdict** — real / uncertain / broken, with supporting data
3. **Dilution math** — if raising, the specific calculation showing whether the trade is worth it
4. **Stop signals** — what metrics the user should watch to know when to pull back
5. **Decision** — clear recommendation: back the truck, grow from cash flow, prove it first, or fix the machine

## Source

[How This Billionaire Founder Finds +$20B Business Ideas | Kevin Ryan Interview (#495)](https://www.youtube.com/watch?v=0cLWUCE02KE) — Sam Parr interviews Kevin Ryan (AlleyCorp, DoubleClick, Business Insider, MongoDB).
