---
name: people-intel
description: "Build a dossier on any person in Sam's network — episodes, quotes, relationships, draft intro email. Use when someone says 'what do I know about [person],' 'tell me about [person],' 'who is [person],' or wants intelligence before a meeting, partnership, or outreach."
---

# People Intel

Build a structured intelligence dossier on any person mentioned across 793 episodes of My First Million and 83 episodes of MoneyWise. You bring a name, you get everything Sam knows about them — episodes, quotes, relationships, frameworks, and a draft intro email referencing specific conversations.

## When to Use

The user wants intel on a specific person. They might say:
- "What do I know about Alex Hormozi?"
- "Tell me about Codie Sanchez"
- "I have a meeting with Chris Voss next week — what's the background?"
- "Who is Elaine Zelby?"
- "I want to reach out to Andrew Wilkinson — what should I reference?"
- "Pull up everything on [name]"

## The Intelligence Gathering Process

Run these sources in order. Each layer adds depth. Not every person will have data in every layer — that is fine. Report what exists.

### Layer 1: Pre-Built Profile

Check if a profile exists at `site/content/people/` (38 profiles built). Filename format: `lowercase-hyphenated-name.md`.

If found, this is your richest source. Extract:
- Bio summary and career trajectory
- Key quotes with episode attribution
- Frameworks associated with them
- Related people (from the `## Related` section)
- Episode list (from frontmatter `episodes:` field and `## Sources and Episodes` section)

If not found, move to Layer 2. The dossier still works — it just requires more assembly.

### Layer 2: Entity Data

Check `data/entities/top-entities.json` for the person's entry. This file contains the top ~200 entities across the corpus with structured metadata.

If found, extract:
- **Mention count** — how often they come up (more mentions = more signal)
- **Source count** — how many distinct episodes reference them
- **Sentiment breakdown** — positive / negative / neutral ratio
- **Top co-occurrences** — the 5 people/companies most frequently mentioned alongside them

The co-occurrence data is gold for the relationship map. If Alex Hormozi co-occurs with Leila Hormozi (16), Acquisition.com (11), and Gym Launch (11), that tells you the conversation clusters.

### Layer 3: Guest Index

Check `plugin/references/indexes/by-guest.md` for a guest index entry. This maps each guest to:
- Episode IDs
- Framework articles they appear in
- Skills they informed
- Key topics

This layer connects the person to specific *teachable content* — not just mentions but frameworks built from their appearances.

### Layer 4: Transcript Search

Search across `data/polished/` (690 MFM transcripts) for additional mentions. Use targeted grep:

```
grep -rl "Person Name" data/polished/
```

This catches mentions the profile and entity data may miss — passing references, comparisons, stories told about them by other guests. For each hit, pull the surrounding context (2-3 paragraphs) to understand *how* they were mentioned.

For people NOT in the pre-built profiles, this is the primary data source. Read the relevant transcript sections and extract quotes, context, and Sam/Shaan's commentary.

### Layer 5: Framework Articles

Search `plugin/references/frameworks/` and `site/content/articles/` for articles that reference the person. These are the distilled, teachable frameworks — if someone appears in a framework article, they contributed something specific enough to become methodology.

```
grep -rl "Person Name" site/content/articles/
grep -rl "Person Name" plugin/references/frameworks/
```

## The Dossier

Compile everything into this format. Be specific. Use real quotes. Reference real episodes. No filler.

---

### [Person Name] — Intelligence Dossier

**Identity:** [One sentence — who they are and why they matter in Sam's world]

**Signal strength:** [X mentions across Y episodes] | Sentiment: [positive/negative/neutral breakdown]

---

#### 1. Summary

Two to three paragraphs covering:
- Who they are and what they have built
- Their relationship to Sam, Shaan, and the MFM universe (guest? frequent reference? business connection?)
- The one thing Sam's audience knows them for

Write this in Sam's voice — direct, specific, no throat-clearing. Lead with the most interesting fact.

#### 2. Episode Appearances & Mentions

List every episode where they appeared as a guest or were discussed, with context:

| Episode | Role | What Was Discussed |
|---------|------|--------------------|
| [Title] (ep. ID) | Guest | [Specific topics — not "business advice" but "client-financed acquisition math, the $300M gym CRM mistake"] |
| [Title] (ep. ID) | Mentioned | [Context — who mentioned them, why, what was said] |

#### 3. Key Quotes

Pull the strongest 3-5 direct quotes, attributed to specific episodes:

> "Quote here." — [Person Name], *[Episode Title]* (ep. ID)

If the person was not a guest but was discussed, pull Sam or Shaan's quotes *about* them:

> "Quote about them here." — Sam Parr, *[Episode Title]* (ep. ID)

#### 4. Relationship Map

Based on co-occurrence data and transcript context:

| Connected To | Relationship | Evidence |
|-------------|-------------|----------|
| [Name] | [Business partner / competitor / friend / mentor / co-guest] | [Specific — "Co-appeared on ep. X", "Sam compared their approaches in ep. Y"] |

#### 5. Frameworks & Articles

List every framework article or skill where they appear:

| Framework/Skill | Their Role |
|----------------|-----------|
| [Framework name] | [What they contributed — a quote, a case study, a counter-example] |

If none: "No framework articles reference [Name] directly. Their mentions are conversational rather than methodological."

#### 6. What Sam Thinks

This is the editorial section. Based on sentiment data and actual quotes, give an honest read on Sam's posture toward this person:
- Does Sam admire them? Quote the evidence.
- Does Sam have reservations? Quote those too.
- Has Sam's view changed over time? (Early episodes vs. recent)
- Would Sam take a meeting with them? Is there an existing relationship?

Be honest. If Sam roasted them, say so. If Sam fanboys, say so. No diplomacy — Sam wouldn't want it.

#### 7. Draft Intro Email

Write a short email Sam could send to this person (or that the user could send referencing Sam's content). The email must:
- Reference a specific episode or quote (not generic)
- Name a specific topic they discussed or were discussed in connection with
- Have a clear ask or reason for reaching out
- Sound like Sam — short sentences, no corporate speak, gets to the point in 3 lines

Format:

```
Subject: [Specific, referencing shared context]

[Name] —

[2-3 sentences max. Reference the specific episode, quote, or framework. State the reason for reaching out. End with a clear next step.]

— Sam
```

If writing for the user (not Sam), adjust the voice but keep the specificity:

```
Subject: [Specific reference]

[Name] —

[Reference that you heard them on MFM ep. X discussing Y. State what resonated. Clear ask.]

— [User]
```

---

## Handling Unknown People

If a name returns zero results across all five layers:

1. Say so directly: "[Name] does not appear in the MFM/MoneyWise archive."
2. Suggest similar names if there is a possible misspelling or alternate name (e.g., "Did you mean Codie Sanchez?" if they searched "Cody Sanchez")
3. Offer to search for their company name or a topic associated with them instead
4. If the user provides context ("they're in the SaaS space"), search transcripts for that context to see if the person was mentioned without being named

## Pre-Built People Profiles

38 profiles exist at `references/people/`. When building a dossier, always check for a pre-built profile first. Available profiles: alex-hormozi, alex-lieberman, amjad-masad, andrew-wilkinson, austin-rief, ben-horowitz, blake-scholl, brent-beshore, brian-halligan, chamath-palihapitiya, charlie-munger, chris-koerner, codie-sanchez, dharmesh-shah, elon-musk, greg-isenberg, hayes-barnard, james-currier, jesse-cole, jesse-itzler, kevin-espiritu, leila-hormozi, logan-paul, marc-andreessen, mohnish-pabrai, mrbeast, naval-ravikant, nick-huber, paul-graham, peter-thiel, sam-parr, scott-galloway, shaan-puri, steve-jobs, tim-ferriss, walt-disney, warren-buffett.

Many guests also have companion framework articles at `references/frameworks/` with the same filename — these contain the distilled methodology or case study associated with that person. Always check both locations.

Person-specific framework articles (contain case studies, business breakdowns, and methodology beyond the people profile):
- Read `references/frameworks/alex-lieberman.md` for Morning Brew co-founder business breakdown
- Read `references/frameworks/amjad-masad.md` for Replit founder's product and AI strategy
- Read `references/frameworks/austin-rief.md` for Morning Brew operator perspective
- Read `references/frameworks/brian-halligan.md` for HubSpot founder's inbound playbook
- Read `references/frameworks/dharmesh-shah.md` for HubSpot CTO's product philosophy
- Read `references/frameworks/elon-musk.md` for Musk's first-principles and negotiation analysis
- Read `references/frameworks/hayes-barnard.md` for solar industry disruption case study
- Read `references/frameworks/kevin-espiritu.md` for Epic Gardening content-to-commerce breakdown
- Read `references/frameworks/logan-paul.md` for creator commerce and Feastables case study
- Read `references/frameworks/marc-andreessen.md` for VC perspective and "software eating the world"
- Read `references/frameworks/naval-ravikant.md` for leverage, judgment, and wealth creation philosophy
- Read `references/frameworks/paul-graham.md` for startup philosophy and YC frameworks
- Read `references/frameworks/peter-thiel.md` for contrarian thinking and zero-to-one analysis
- Read `references/frameworks/steve-jobs.md` for product obsession and reality distortion field
- Read `references/frameworks/walt-disney.md` for vertical integration and entertainment empire building

## Handling Thin Profiles

If a name appears in only 1-2 episodes with minimal context:

1. Report what exists — even one mention is useful
2. Flag the thinness: "Limited data — [Name] appears in [X] episodes. Here's what's there."
3. Still produce the full dossier format but mark empty sections as "No data in archive" rather than omitting them
4. The draft intro email becomes more important here — reference the specific mention to show you did the homework
