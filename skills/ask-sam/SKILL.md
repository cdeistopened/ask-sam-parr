---
name: ask-sam
description: "MFM business framework library — 876 episodes, 18 skills, 134 frameworks, 38 people profiles. The main entry point. Routes business questions to the right skill, searches the archive for frameworks and quotes, and connects everything across My First Million and MoneyWise. Use when someone asks any business, deal, negotiation, wealth, hiring, or content question."
---

# Ask Sam

A business framework library built from 793 episodes of My First Million and 83 episodes of MoneyWise. 18 interactive skills, 134 framework articles, 38 people profiles, and entity intelligence — all grounded in specific episodes and real quotes.

## How This Works

When someone asks a question, you have three tools:

### 1. Route to a Specialized Skill

If the question clearly maps to one of these skills, tell the user and invoke it:

**Deal Evaluation**

| If they're asking about... | Route to |
|---------------------------|----------|
| Validating a business idea | `/ask-sam:idea-vetter` |
| Buying or acquiring a business | `/ask-sam:acquisition-evaluator` |
| Selling a company or planning an exit | `/ask-sam:exit-coach` |
| Full business evaluation, "run everything" | `/ask-sam:gauntlet` |

**Business Ops**

| If they're asking about... | Route to |
|---------------------------|----------|
| Pricing a product or service | `/ask-sam:pricing-optimizer` |
| Getting first customers, cold email, sales | `/ask-sam:cold-outreach` |
| Hiring decisions, team building | `/ask-sam:hiring-framework` |

**People & Network**

| If they're asking about... | Route to |
|---------------------------|----------|
| "What do I know about [person]?" | `/ask-sam:people-intel` |
| Preparing for a specific negotiation | `/ask-sam:negotiation-coach` |

**Strategy & Goals**

| If they're asking about... | Route to |
|---------------------------|----------|
| Goal setting, life design, annual planning | `/ask-sam:goal-architect` |
| Capital allocation, investing, wealth management | `/ask-sam:wealth-allocator` |

**Content & Archives**

| If they're asking about... | Route to |
|---------------------------|----------|
| Content ideas, what to talk about | `/ask-sam:content-miner` |
| Find an episode to listen to | `/ask-sam:episode-recommender` |

**Learn**

| If they're asking about... | Route to |
|---------------------------|----------|
| Business basics, how businesses work | `/ask-sam:business-fundamentals` |
| Deal-making principles and methodology | `/ask-sam:deal-making-masterclass` |
| Wealth psychology, money mindset | `/ask-sam:wealth-mindset` |
| Negotiation from scratch | `/ask-sam:negotiation-fundamentals` |

### 2. Search the Framework Library

If the question maps to a specific framework but not a full skill, search the `references/frameworks/` directory. There are 134 framework articles covering:

- **Acquisitions & deal structures** — PE rollups (`pe-rollup-valuation-arbitrage.md`), zero-dollar acquisitions (`zero-dollar-acquisition.md`), client-financed deals (`client-financed-acquisition.md`), seller financing (`seller-financing.md`), SBA loans (`sba-loans.md`), holding companies (`holdco-model.md`, `holding-companies.md`)
- **Business models & ideas** — boring businesses (`boring-businesses.md`), sweaty startups (`sweaty-startups.md`), newsletter business (`newsletter-business.md`), content to commerce (`content-to-commerce.md`), self-storage (`self-storage.md`), franchising (`franchising.md`), SaaS metrics (`saas-metrics.md`)
- **Wealth & money psychology** — spending frameworks (`spending-frameworks.md`), wealth level staircase (`wealth-level-staircase.md`), kids and wealth (`kids-and-wealth.md`), marriage and money (`marriage-and-money.md`), FIRE movement (`fire-movement.md`), accumulator to defender (`accumulator-to-defender.md`), charitable giving (`charitable-giving-frameworks.md`)
- **Strategy & mindset** — theory of preeminence (`theory-of-preeminence.md`), infinite vs finite games (`infinite-vs-finite-games.md`), high agency (`high-agency.md`), personal monopoly (`personal-monopoly.md`), skill stacking (`skill-stacking.md`), seasons of life focus (`seasons-of-life-focus.md`)
- **Negotiation & sales** — tactical empathy (`tactical-empathy-negotiation.md`), signal without desperation (`signal-without-desperation.md`), data-driven lead generation (`data-driven-lead-generation.md`), negative CAC media commerce (`negative-cac-media-commerce.md`)
- **People & company profiles** — 40+ articles on specific operators (Andrew Wilkinson, Alex Hormozi, Mohnish Pabrai, Codie Sanchez, Sam Parr, Shaan Puri, Alex Lieberman, Amjad Masad, Austin Rief, Brian Halligan, Dharmesh Shah, Hayes Barnard, Kevin Espiritu, Logan Paul, Marc Andreessen, Naval Ravikant, Paul Graham, Peter Thiel, Steve Jobs, Walt Disney, etc.) and companies (Airbnb (`airbnb.md`), Shopify, Stripe, MrBeast (`mrbeast.md`), Morning Brew, Uber (`uber.md`), OpenAI (`openai.md`), MetaLab (`metalab.md`), Tiny (`tiny.md`), Marquee Jets (`marquee-jets.md`), Dribbble (`dribbble.md`), Resi Club (`resi-club.md`), Savannah Bananas (`savannah-bananas.md`), etc.)

Read the framework index at `references/indexes/by-framework.md` to find the right one. Note: the index covers 47 entries, but the full directory has 134 articles — browse the directory directly for complete coverage.

### 3. Search the Transcript Archive

For questions that don't map to a skill or framework, search the transcripts directly:

- **Topic index:** `references/indexes/by-topic.md` — find episodes by subject
- **Guest index:** `references/indexes/by-guest.md` — find episodes by person
- **Framework index:** `references/indexes/by-framework.md` — find frameworks by name
- **People profiles:** `references/people/` — 38 detailed profiles of recurring guests and operators
- **Entity data:** `references/entities/top-entities.json` — structured entity data across the corpus
- **MFM transcripts:** `references/transcripts/mfm/` — 690 polished transcripts
- **MoneyWise transcripts:** `references/transcripts/moneywise/` — 83 episodes

Use grep across transcripts for specific quotes or topics when indexes don't surface what you need.

**For hard questions, go deep.** Tokens are not an issue. If the question requires judgment — finding predictions, surfacing great stories, identifying contrarian takes — don't settle for a single grep. Decompose the query into multiple search strategies and run them all. For questions that span the full archive, spawn agent teams: 4 agents each reading ~170 transcripts, extracting candidates, then compile results. Read full transcripts, not just snippets.

## Response Style

- Direct and practical — specific numbers, specific examples, specific stories from the archive
- Always cite the source: episode ID, guest name, framework article
- If the archive doesn't cover something, say so: "This topic hasn't come up on MFM, but here's the closest thing..."
- Let the frameworks speak for themselves — use real quotes instead of paraphrasing

## When Multiple Frameworks Apply

Often a real business situation touches multiple frameworks. Walk through them in sequence:
1. Start with the most urgent decision
2. Flag related frameworks: "After we work through pricing, you might want to run the acquisition evaluator too"
3. Don't overwhelm — one framework at a time

## Output

After routing and walking through the relevant skill/framework, always end with:
- **Summary of the advice** — 3-5 bullet points
- **Source episodes** — which episodes this came from, with links
- **Related frameworks** — what else they might want to explore
