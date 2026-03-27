---
name: Three-Method Company Valuation
description: Walk someone through how to value any company using all three standard methods — industry earnings multiple, formula-based strategic value, and comparable sales. Use when someone asks how much their company is worth, how buyers value businesses, what multiple they should expect, or how to prepare for an acquisition conversation.
type: framework
domain: frameworks
status: published
episodes:
  - GkNJbj5qbXM
date_created: 2026-03-04
source_guests:
  - James Altucher
---

# Three-Method Company Valuation

Walk someone through how to value any company using James Altucher's three-method framework — drawn from his experience selling multiple companies and investing in dozens more, discussed on My First Million.

## When to Use

The user needs to value a company — either their own before a sale, or a target before an acquisition. They might say:
- "How much is my company worth?"
- "A buyer asked me my number — what do I say?"
- "What multiple should I expect when I sell?"
- "How do acquirers think about company valuation?"
- "We're about to enter acquisition conversations — how do I think about what we're worth?"
- "I'm trying to buy a company — how do I value it?"

## The Core Principle

From James Altucher (`GkNJbj5qbXM.md`):

> "There are three ways to value a company. One is a standard industry multiple on your earnings... The second way is what you just described — if we put ads all over here and you're driving this amount of traffic, and we monetize those ads, this is what we're worth... The third way is comparable deals in the space."

No single method gives you the answer. Each method tells you something different about how a specific buyer is likely to think about your business. The goal is to run all three, understand which one favors you most, and lead with that framing in negotiations — while anticipating which method the buyer will use.

## Method 1: Industry Earnings Multiple

The most common valuation method for profitable businesses. Buyers apply a standard multiple to your EBITDA or net income.

James Altucher:

> "One is a standard industry multiple on your earnings — and cut it in half, by the way, because no one's going to pay the maximum. So if you have a profitable company in an industry that trades on the stock market at 20 times earnings, your company is probably last year's profits times 10. That's a basic formula."

**The haircut rule:** Take the public market multiple for comparable public companies in your sector. Cut it roughly in half. That's the realistic private company multiple.

Why the haircut? Public companies are liquid, audited, institutionally traded. Private companies are illiquid, less transparent, harder to exit. Buyers discount for that.

**How to find the public multiple:**
- Look at P/E ratios for public companies in your sector
- Look at EV/EBITDA multiples for acquisitions in your sector (S&P Capital IQ, PitchBook if you have access, or press releases)
- Ask your banker or accountant — they track this

**Formula:**
```
Private Company Value (Method 1) ≈ Last Year's EBITDA × (Public Multiple / 2)
```

**Ask the user:** What is your trailing twelve-month EBITDA? What do comparable public companies trade at in your sector? Run the math together.

**Limitation:** This method only works if your business is profitable. Pre-revenue or breakeven businesses need Method 2 or 3.

## Method 2: Strategic Value Formula

For businesses where the value to the buyer is not primarily about current earnings — it's about what the buyer can do with what you have (traffic, audience, data, distribution).

James Altucher:

> "The second way is what you just described — if we put ads all over here and you're driving this amount of traffic, and we monetize those ads, this is what we're worth. Cut that in half."

And his warning:

> "On my second company, I made the mistake of not controlling the variables in that formula. They knew the variables better than I did, so I had to make sure when negotiating the formula that I understood the variables enough that it worked out to what I wanted. I didn't do that properly on my second negotiation."

This method is a collaborative financial model: you and the buyer agree on the inputs (traffic, conversion rates, CPMs, retention, etc.) and build a formula together. The danger is that the buyer controls the assumptions. Your job is to:

1. Know your own numbers cold — don't let them assert variables you can't verify
2. Build the model yourself before the negotiation so you can push back on buyer assumptions
3. Insist on conservative-but-defensible inputs (if they lowball your traffic, you push back with your analytics)

**Ask the user:** If a buyer's strategic value from your business is based on metrics like traffic, users, data, or distribution — do you know those numbers precisely? Build the model together: what's the buyer getting, what's it worth to them at standard monetization rates, and what's a fair share of that value for you?

**Formula (example):**
```
Strategic Value = (Monthly Visitors × Monetization Rate × 12 months × Retention)
                ÷ 2 (buyer discount)
```
The specific formula depends on the business and buyer type.

## Method 3: Comparable Sales

The most commonly used method in tech, where earnings-based multiples are hard to apply to unprofitable or pre-revenue businesses.

James Altucher:

> "The third way is comparable deals in the space. They sold for this, we're bigger, so we should be this. That's kind of a BS way to value a company, but it's how people value companies, particularly in tech. Like Giphy — they weren't valuing off earnings."

He elaborated on why this matters in practice:

> "And then Tenor, their competitor, just sold to Google the year before for a little less. By the way, is it true that Giphy was the second-largest search engine in the world?"

Comp-based valuation logic:
- Find the closest recent deal in your space (similar revenue, similar user base, similar growth rate)
- Adjust up or down based on how you compare
- The more recent the comp, the more weight it carries

**Ask the user:** What are the most comparable recent acquisitions in your space? Walk through: who sold, for how much, at what revenue/user scale, and how does your business compare? If comps are available, they become your anchor in the negotiation.

**Limitation:** Altucher calls this "kind of a BS way" because it's highly gameable — buyers can always find a comp that supports a lower valuation. Know the comps better than the buyer does.

## Step: Run All Three and Pick Your Lead

After running all three methods, you'll have a range. Compare them:

| Method | Your Valuation | Notes |
|--------|---------------|-------|
| Earnings multiple | $X | Applies if profitable |
| Strategic value | $X | Applies if buyer has clear use case |
| Comparable sales | $X | Applies if good comps exist |

Lead with whichever method produces the highest defensible number for your specific buyer. If you're selling to a strategic acquirer, Method 2 likely wins. If you're selling to a financial buyer (PE), Method 1. If you're in a hot sector with recent high-value exits, Method 3.

James Altucher on the overall challenge:

> "When they come to you and say, how much do you want for your company — that's a very hard question to answer. You don't want to sound greedy. You don't want to sound desperate. You don't want to underprice yourself. So there are all sorts of negotiating techniques to help them answer that question in a way that works for both sides."

## Quick Reference

| Method | Best For | Key Metric | Haircut |
|--------|----------|-----------|---------|
| Earnings multiple | Profitable businesses | EBITDA × sector multiple | ~50% off public multiple |
| Strategic value formula | Traffic, audience, data plays | Buyer's monetization model | ~50% off theoretical value |
| Comparable sales | Tech, high-growth, pre-profit | Recent deals in your sector | Adjust for size/growth |

## Search the Archive

```
grep -ri "valuation\|EBITDA.*multiple\|how much.*company.*worth" transcripts/
grep -ri "comparable.*deal\|comp.*transaction\|strategic.*value" transcripts/
grep -ri "James Altucher\|selling.*company.*method" transcripts/
```

## Output

After working through this framework, deliver:
1. **Method 1 result** — EBITDA × (sector public multiple / 2)
2. **Method 2 result** — strategic value model built with buyer assumptions, with your pushback on key inputs
3. **Method 3 result** — best available comp transactions, adjusted for your company's profile
4. **Recommended lead method** — which method to present first to this specific buyer type
5. **Negotiation prep** — what number to anchor on and why

## Source

[Entrepreneur Who Lost Millions Breaks Down How To Come Back Financially](https://www.youtube.com/watch?v=GkNJbj5qbXM) — Sam Parr and Shaan Puri interview James Altucher, May 2020.
