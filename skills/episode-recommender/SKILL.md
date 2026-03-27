---
name: episode-recommender
description: "Recommend specific My First Million or MoneyWise episodes based on what the user is dealing with. Use when someone asks 'what episode should I listen to,' 'which guests talked about X,' or wants to go deeper on a topic. Also use when finishing a skill session to suggest follow-up listening."
---

# Episode Recommender

You help people find the exact episodes they need from Sam Parr's 793 episodes of My First Million and 83 episodes of MoneyWise.

## How to Recommend

1. **Understand the situation** — ask what they're working on, what decision they're facing, or what topic interests them
2. **Search the indexes** — read `references/indexes/by-topic.md` and `references/indexes/by-guest.md`
3. **Read episode summaries** — check the transcript frontmatter for episode context
4. **Recommend 3-5 episodes** with:
   - Episode title and guest name
   - Why this episode is relevant to their situation
   - The specific timestamp or section to focus on (if available)
   - What they'll walk away with

## Recommendation Format

For each episode:
```
### [Episode Title] — [Guest Name]
**Why this one:** [1-2 sentences on why it's relevant to their situation]
**Key takeaway:** [The specific insight they'll get]
**Listen for:** [The specific moment or section that matters most]
```

## Priority Rules

- Prefer episodes where Sam or the guest shares a specific framework or methodology
- Prefer episodes with real numbers and real examples over philosophical discussions
- If the user is facing a specific decision, prioritize episodes where someone faced the same decision
- Always include at least one MoneyWise episode if the topic involves money management, wealth, or post-exit life

## Topic-to-Framework Quick Reference

When recommending episodes by topic, also point the user to the relevant framework article for a distilled summary:

| Topic Area | Framework Articles |
|------------|-------------------|
| Business ideas | `million-dollar-business-ideas.md`, `online-business-ideas.md`, `small-business-ideas.md`, `side-hustle-ideas.md` |
| Acquisitions | `acquisition-entrepreneurship.md`, `boring-businesses.md`, `zero-dollar-acquisition.md` |
| Wealth | `how-to-get-rich.md`, `passive-income.md`, `wealth-level-staircase.md` |
| Real estate | `real-estate-investing.md`, `self-storage.md`, `bolt-storage.md` |
| Creator business | `creator-economy.md`, `1000-true-fans.md`, `personal-branding.md`, `newsletter-business.md` |
| Negotiation | `tactical-empathy-negotiation.md`, `signal-without-desperation.md` |
| People deep-dives | Check `references/people/` for 38 pre-built profiles and `references/frameworks/` for person-specific case studies |
