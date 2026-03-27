---
name: content-miner
description: "Mine the MFM/MoneyWise archive for content opportunities — gap analysis, revisit-worthy takes, guest callbacks, and clip discovery. Use when someone says 'what should I talk about,' 'find me content ideas,' 'what's in my archive about X,' 'which guests should I bring back,' or wants to turn trending topics into content using existing material."
---

# Content Miner

Mine the 876-episode archive (793 MFM + 83 MoneyWise) for content opportunities backed by archive evidence. The user provides context — trending topics, audience questions, content gaps — and gets ranked ideas with specific episode references, quotes, and angles.

## When to Use

The user wants content ideas grounded in their existing archive. They might say:
- "What should I talk about next?"
- "What's in my archive about [topic]?"
- "Which guests should I bring back?"
- "This topic is trending — do I have anything on it?"
- "What topics have I mentioned but never really covered?"
- "Find me revisit-worthy takes from old episodes"

## How It Works

This skill has four mining modes. Ask the user which mode they want, or suggest one based on their question. If they say something general like "find me content ideas," run Gap Mining first, then offer the other modes.

**No external trend awareness.** The user provides the trend context. This skill's job is to search the archive, not the internet.

---

## Mode 1: Gap Mining

**Purpose:** Find topics mentioned across episodes but never deep-dived.

**Trigger phrases:** "What haven't I covered?" / "What topics am I missing?" / "Find gaps in my content"

### Workflow

1. Read `references/indexes/by-topic.md` — this maps topics to episode IDs
2. Read `references/indexes/by-framework.md` — this lists the 47 frameworks with dedicated articles
3. Cross-reference: which topics appear in **3+ episodes** in the topic index but have **no corresponding framework article** in the framework index?
4. For each gap found, grep `references/transcripts/` for the topic keyword to confirm it appears in multiple transcripts and isn't just an index artifact
5. Read 2-3 relevant transcript sections to find the best quotes and angles

### Output: Gap Analysis Table

For each gap (aim for 5-10):

| Topic | Episodes Mentioning It | Existing Coverage | Suggested Angle |
|-------|----------------------|-------------------|-----------------|
| [topic] | [count] episodes ([list top 3 IDs]) | [None / Brief mention in X article] | [Specific angle that would fill the gap] |

Include a representative quote from the strongest episode for each gap.

---

## Mode 2: Revisit Mining

**Purpose:** Find takes and predictions from 2+ years ago worth revisiting now.

**Trigger phrases:** "Was I right about X?" / "What did I say about [topic] years ago?" / "Find revisit-worthy takes"

### Workflow

1. User provides a topic (or ask them for one — e.g., "AI," "crypto," "remote work," "newsletters")
2. Grep `references/transcripts/` for the topic across the archive
3. Focus on older episodes — look at episode filenames/dates to identify content from 2+ years ago
4. Read the relevant transcript sections for strong, specific takes or predictions (not vague observations)
5. For each revisit candidate, note: what was the original take? What has changed since? What's the revisit angle?

### Output: Revisit Candidates

For each candidate (aim for 3-5):

**Episode:** [ID / title]
**Original Take:** "[Direct quote from transcript]"
**What's Changed:** [Brief description of what happened since — the user can fill in details since they know the current landscape better than the archive does]
**Revisit Angle:** [Specific framing for a new episode — "I was right about X," "I was wrong about Y," "This aged surprisingly well," "Here's what nobody saw coming"]

---

## Mode 3: Callback Mining

**Purpose:** Identify guests worth bringing back based on archive presence and time elapsed.

**Trigger phrases:** "Which guests should I bring back?" / "Who haven't I had on in a while?" / "Guest ideas"

### Workflow

1. Read `references/indexes/by-guest.md` — this lists guests with their episodes, frameworks, and key topics
2. Read `references/people/` profiles for guests with high archive presence (multiple episodes, associated frameworks, or skill references)
3. Identify guests who:
   - Appeared in 2+ episodes OR have a dedicated framework/skill
   - Haven't appeared recently (check episode IDs — older-format filenames like `title_slug` tend to be older episodes, YouTube IDs like `k7UycsE_QoA` tend to be newer)
   - Run businesses or projects that have likely evolved significantly
4. For each callback candidate, read their people profile and note what they were known for, then identify what might have changed

### Output: Callback Candidates

For each candidate (aim for 5-8):

**Guest:** [Name]
**Last Appearance:** [Episode ID / approximate date]
**Known For:** [Their business/framework from the archive]
**What's Likely Changed:** [Business growth, pivot, new venture, market shift — based on what the archive says plus reasonable inference]
**Callback Topic:** "[Specific episode premise — e.g., 'Have Alex Hormozi back to talk about what Acquisition.com looks like at $500M+ portfolio']"

---

## Mode 4: Clip Mining

**Purpose:** User has a trending topic and wants to know what's already in the archive about it.

**Trigger phrases:** "This is trending — what do I have on it?" / "Find clips about X" / "What's in my archive about [topic]?"

### Workflow

1. User provides the trending topic or theme
2. Grep `references/transcripts/` for the topic and related keywords (brainstorm 3-5 keyword variations)
3. Read the matching transcript sections — look for segments that are:
   - Self-contained (make sense without the full episode context)
   - Quotable (strong opinions, specific numbers, memorable phrasing)
   - Timeless (the insight still applies, not dated by a specific event that's now irrelevant)
4. For each clip candidate, extract the key passage and note which speaker said it

### Output: Clip Candidates

For each candidate (aim for 5-10):

**Episode:** [ID / title]
**Speaker:** [Sam / Shaan / Guest name]
**Key Passage:**
> "[Direct quote from transcript — the clip-worthy section, 2-5 sentences]"

**Suggested Clip Title:** [Punchy title for social media / YouTube Shorts]
**Why It Works Now:** [1 sentence connecting this archive content to the user's trending topic]

---

## Final Synthesis: Top 5 Recommendations

After completing any mode (or multiple modes), end with a ranked list:

### Top 5 Content Opportunities

Rank by two factors:
1. **Content potential** — how compelling would this be as an episode/clip/post?
2. **Archive evidence strength** — how much source material exists to support it?

| Rank | Opportunity | Mode | Evidence Strength | Why Now |
|------|-------------|------|-------------------|---------|
| 1 | [Specific content idea] | [Gap/Revisit/Callback/Clip] | [Strong/Medium — cite episode count or quote quality] | [1 sentence] |
| 2 | ... | ... | ... | ... |
| 3 | ... | ... | ... | ... |
| 4 | ... | ... | ... | ... |
| 5 | ... | ... | ... | ... |

For the #1 recommendation, include a one-paragraph pitch: what the episode/content would be, why it works, and which archive material to pull from.

---

## Deep-Dive References

These framework articles are rich content sources for mining:

- Read `references/frameworks/personal-branding.md` for content angles on personal brand building
- Read `references/frameworks/creator-economy.md` for creator business model evolution
- Read `references/frameworks/content-to-commerce.md` for audience-to-product pipeline stories
- Read `references/frameworks/newsletter-business.md` for newsletter-specific content angles
- Read `references/frameworks/community-building.md` for community-driven content strategies
- Read `references/frameworks/my-first-million.md` for meta-content about the show itself

Company/person profiles that generate repeat content:
- Read `references/frameworks/acquisition-com.md` for Hormozi empire updates and angles
- Read `references/frameworks/morning-brew.md` for newsletter business evolution
- Read `references/frameworks/feastables.md` for MrBeast commerce case study
- Read `references/frameworks/hampton.md` for peer community model updates
- Read `references/frameworks/late-checkout.md` for Greg Isenberg's community plays
- Read `references/frameworks/skool.md` for Hormozi's community platform

## File Paths

All paths are relative to the plugin root (`plugin/`):

| Asset | Path |
|-------|------|
| Topic index | `references/indexes/by-topic.md` |
| Framework index | `references/indexes/by-framework.md` |
| Guest index | `references/indexes/by-guest.md` |
| Transcripts | `references/transcripts/` |
| People profiles | `references/people/` |
| Framework articles | `references/frameworks/` |
