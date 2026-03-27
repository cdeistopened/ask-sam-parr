# Idea Vetter

Walk a founder through evaluating a business idea using frameworks from Sam Parr, Shaan Puri, and guests on My First Million.

## When to Use

The user has a business idea and wants to pressure-test it. They might say:
- "I have an idea for X — is it worth pursuing?"
- "Help me evaluate this business concept"
- "Should I start this company?"

## The Framework Stack

Run the idea through these filters in order. Each builds on the previous. Stop and discuss at each stage — don't rush through.

### Filter 1: The Thiel Test (Disguised as Bad)

From Imad Rahimi (Mercury, $3.5B) in the episode "I Built A $1B Company... Here's 7 Business Ideas I Would Start This Year":

> "The best ideas come disguised as bad ideas. You're looking for the overlap between 'sounds like a bad idea' and 'actually a good idea.'"

Three sub-tests:
1. **Does it sound like a bad idea to most people?** If everyone thinks it's great, the market is probably already crowded.
2. **Is there an inflection point?** Something that recently changed (technology, regulation, culture) that makes this possible now but wasn't before.
3. **Does it scare people off?** The best ideas have a natural moat of difficulty, weirdness, or stigma that reduces competition.

Ask the user: "When you tell people about this idea, do they immediately get excited — or do they look confused or skeptical?" If the answer is "everyone loves it," that's actually a yellow flag.

**Source transcript:** `transcripts/mfm/2025-03-27-i-built-a-1b-company-heres-7-business-ideas-i-would-start-this-year.md`

### Filter 2: The Value Equation (Hormozi)

From Alex Hormozi across multiple episodes:

```
Value = (Dream Outcome × Perceived Likelihood) / (Time Delay × Effort Required)
```

Walk through each variable:
- **Dream Outcome:** What's the best possible result for the customer? How life-changing is it?
- **Perceived Likelihood:** Does the customer believe this will actually work? What proof exists?
- **Time Delay:** How long until the customer sees results? (Shorter = more valuable. Lipo vs. personal training.)
- **Effort Required:** How much work does the customer have to do? (Less = more valuable.)

The goal: maximize the numerator, minimize the denominator. If the idea scores poorly on time delay or effort, ask whether there's a way to restructure.

**Source transcript:** `transcripts/mfm/2024-08-17-how-to-craft-a-100m-offer-in-6-minutes.md`

### Filter 3: The Unit Economics Check (Sam's Math)

From Sam Parr's lead gen episode and multiple brainstorming sessions:

> "The math is basically: how valuable is the purchase price of the product, multiplied by the frequency one person buys it, multiplied by the number of people who have that need."

Have the user fill in:
- **Price per unit/transaction:** $___
- **Purchase frequency:** ___ times per [year/month/lifetime]
- **Total addressable buyers:** ___
- **Realistic capture rate:** ___% (be conservative — 1-5% of TAM is common)

Calculate: `Price × Frequency × TAM × Capture Rate = Revenue ceiling`

If the revenue ceiling is under $1M/year, the idea may work as a lifestyle business but won't be venture-scale. That's not necessarily bad — just know what you're building.

Then ask: "What does it cost you to acquire one customer?" If they don't know, walk them through Sam's method: run a small test (ads, cold outreach, content) to find the real CAC, not the theoretical one.

**Source transcript:** `transcripts/mfm/2022-06-03-follow-these-3-steps-to-start-a-1000000-lead-generation-business.md`

### Filter 4: The North Star Formula (Shaan's Compression)

From Shaan Puri across multiple episodes:

> "I like when you can boil a plan down to a very simple equation. With Hampton: 'Ten thousand times ten thousand.' You just need 10,000 CEOs who will pay you $10,000 a year and you have a $100 million business."

Ask: "Can you express your entire business model in one multiplication?" Examples:
- `1,000 customers × $500/month = $6M ARR`
- `50,000 units × $30 margin = $1.5M/year`
- `200 clients × $10,000/project = $2M/year`

If the user can't compress it to one equation, the business model might be too complex or unclear. Push them to simplify until they can.

**Source transcript:** `transcripts/mfm/2023-04-04-how-to-buy-a-d2c-startup-for-cheap-and-sell-it-for-millions.md`

### Filter 5: The Validation Plan (Sam's 100 Conversations)

From Sam Parr on customer discovery:

> "I talked to a hundred potential customers. Only two out of the hundred were like, 'Give it to me right now.' But if 2% of people want something and the market's big enough, that's probably enough for an early adopter base."

Key rules from *The Mom Test* (referenced by Sam):
- Never ask "would you pay for this?" — people lie.
- Instead ask about past behavior: "How do you currently solve this problem? What have you tried? How much have you spent?"
- The goal is to find the people who are already hacking together a solution — they're your early adopters.

Help the user build a validation plan:
1. List 100 potential customers (by name if possible)
2. Draft 3 discovery questions that avoid leading
3. Set a threshold: "If X out of 100 say 'give it to me now,' proceed"
4. Time-box: 2-4 weeks to complete the conversations

**Source transcripts:** `transcripts/mfm/2025-03-27-i-built-a-1b-company-heres-7-business-ideas-i-would-start-this-year.md`, `transcripts/mfm/2022-08-19-how-to-close-your-first-1000-customers-startup-sales-101.md`

### Filter 6: The Playbook Clone Check

From Sam and Shaan's recurring pattern:

> "I would just clone this business in a different category. That's really underrated and most people don't do it."

Before building from scratch, search the transcripts for whether someone has already described a working version of this idea — or something close. Use:
```
grep -r "relevant keyword" transcripts/
```

If a similar business exists:
- Who built it? What did they learn?
- What worked and what didn't?
- Can you take their playbook and apply it to a different market, geography, or customer segment?

The best version of the user's idea might be "X but for Y" — and the transcripts may contain the X.

**Source transcript:** `transcripts/mfm/2022-05-04-from-small-business-to-franchise-how-to-make-it-happen.md`

## Output

After running all six filters, summarize:
1. **Thiel Test:** Pass/Fail + reasoning
2. **Value Equation:** Score each variable 1-5
3. **Unit Economics:** Revenue ceiling + CAC estimate
4. **North Star Formula:** The one equation
5. **Validation Plan:** The 100-person list and discovery questions
6. **Playbook Clone:** Any existing models found in the archive

Then give an honest assessment: "Based on these frameworks, here's where this idea is strong and where it needs work." Don't just be encouraging — Sam and Shaan are blunt, and so should this assessment be.

## Deep-Dive References

Read these for additional frameworks when the user's idea falls into a specific category:

- Read `references/frameworks/million-dollar-business-ideas.md` for the MFM pattern library of ideas that actually worked
- Read `references/frameworks/online-business-ideas.md` for the MFM digital business playbook
- Read `references/frameworks/small-business-ideas.md` for opportunities hiding in plain sight
- Read `references/frameworks/side-hustle-ideas.md` for part-time and margin business models
- Read `references/frameworks/boring-businesses.md` for the full boring business thesis
- Read `references/frameworks/sweaty-startups.md` for service-based startup opportunities
- Read `references/frameworks/1000-true-fans.md` for the minimum viable audience model
- Read `references/frameworks/creator-economy.md` for creator-first business models
- Read `references/frameworks/content-to-commerce.md` for audience-to-product conversion patterns
- Read `references/frameworks/negative-cac-media-commerce.md` for businesses where content IS the acquisition channel
- Read `references/frameworks/newsletter-business.md` for newsletter-as-business economics
- Read `references/frameworks/community-building.md` for community-driven business models
- Read `references/frameworks/franchising.md` for franchise model evaluation
- Read `references/frameworks/saas-metrics.md` for SaaS-specific unit economics and benchmarks
- Read `references/frameworks/network-effects.md` for network effect types and defensibility
- Read `references/frameworks/personal-monopoly.md` for building a business only you can build
- Read `references/frameworks/productize-yourself.md` for the leverage and productization framework
- Read `references/frameworks/skill-stacking.md` for combining skills into unique market positions
- Read `references/frameworks/contrarian-thinking.md` for the contrarian thesis in business ideas
- Read `references/frameworks/one-to-two-dollar-machine.md` for the simple unit economics mental model
- Read `references/frameworks/ideabrowser-com.md` for Sam's idea validation tool

People profiles relevant to idea validation:
- Read `references/people/alex-hormozi.md` for the value equation and offer creation frameworks
- Read `references/people/greg-isenberg.md` for community-first business validation
- Read `references/people/james-currier.md` for network effects and defensibility analysis
