# Installing Ask Sam

## Prerequisites

- [Claude Code](https://docs.anthropic.com/en/docs/claude-code) installed

## Setup

### 1. Clone the repo

```bash
git clone https://github.com/cdeistopened/samparr-wiki.git
```

Put it wherever you keep plugins. Common locations:
- `~/.claude/plugins/samparr-wiki`
- `~/plugins/samparr-wiki`
- Anywhere — just note the path

### 2. Add to Claude Code

Add the plugin path to your settings. For global access (available in every project), edit `~/.claude/settings.json`:

```json
{
  "plugins": [
    "/absolute/path/to/samparr-wiki"
  ]
}
```

For project-specific access, add it to your project's `.claude/settings.json` instead.

### 3. Restart Claude Code

Plugins load on startup. After editing settings, restart your session for the skills to appear.

### 4. Verify

```
/ask-sam
```

You should see the router respond. If it says the skill isn't found, check that the path in your settings.json is correct and absolute.

## Optional: Index with QMD

If you have [QMD](https://github.com/cdeistopened/qmd) installed, you can index the transcripts for semantic search. This makes cross-archive questions significantly more accurate — instead of grep, Claude can do vector similarity search across all 773 episodes.

Add to your `~/.config/qmd/index.yml`:

```yaml
ask-sam-mfm:
  path: /path/to/ask-sam/references/transcripts/mfm
  glob: "**/*.md"

ask-sam-moneywise:
  path: /path/to/ask-sam/references/transcripts/moneywise
  glob: "**/*.md"
```

Then:

```bash
qmd reindex ask-sam-mfm ask-sam-moneywise
qmd embed ask-sam-mfm ask-sam-moneywise
```

The plugin works without QMD — it uses framework indexes and grep. QMD just makes retrieval better for open-ended questions that span many episodes.

## First Questions to Try

**Run the gauntlet** (5-stage business evaluation):
```
I want to start a premium dog food subscription box. Run the gauntlet.
```

**People intelligence:**
```
Build me a dossier on Alex Hormozi — every episode, key quotes, who he's connected to.
```

**Decision skill:**
```
I'm thinking about buying a laundromat chain for $1.2M — is it a good deal?
```

**Content mining:**
```
What topics have been discussed across many episodes but never got a dedicated deep dive?
```

## Troubleshooting

- **Skills not found:** Check the path in `settings.json` is absolute (starts with `/`). Restart Claude Code after editing.
- **Generic answers:** Invoke a skill directly — e.g., `/ask-sam:idea-vetter` — to use the structured framework path instead of open-ended chat.


## Learn More

[creativeintel.agency](https://creativeintel.agency)
