# human-like

Claude Code skill for honest, brutally realistic feedback on product ideas, startup pitches, Reddit posts, and business concepts.

No cheerful AI positivity. Just a skeptical human perspective that saves you months of wasted effort.

## What it does

- Evaluates ideas on a skepticism spectrum and gives a direct verdict
- Points out competitors, weak assumptions, missing monetization, lack of moat
- Asks uncomfortable questions a real investor or experienced founder would ask
- Responds in the same language as your input
- Short by default (3-7 sentences), expands on request

## Install

### Option 1: Copy manually

```bash
mkdir -p ~/.claude/skills/human-like
curl -o ~/.claude/skills/human-like/SKILL.md \
  https://raw.githubusercontent.com/seoshmeo/human-like-skill/master/human-like/SKILL.md
```

### Option 2: Clone the repo

```bash
git clone https://github.com/seoshmeo/human-like-skill.git /tmp/human-like-skill
cp -r /tmp/human-like-skill/human-like ~/.claude/skills/human-like
rm -rf /tmp/human-like-skill
```

### Option 3: Download `.skill` file

```bash
curl -L -o /tmp/human-like.skill \
  https://github.com/seoshmeo/human-like-skill/raw/master/human-like.skill
unzip -o /tmp/human-like.skill -d ~/.claude/skills/
rm /tmp/human-like.skill
```

## Usage

The skill activates automatically when you ask Claude Code to evaluate, review, roast, or critique an idea. You can also trigger it explicitly:

```
/human-like My SaaS idea is a Notion plugin that uses AI to auto-organize pages
```

Or just share an idea and say things like:
- "be honest"
- "what do you really think"
- "would this work"
- "tear this apart"
- "thoughts?"

## Example

**You:** I want to build an AI wrapper that summarizes YouTube videos. Thoughts?

**Claude (with human-like):** Honestly? There are already dozens of these — Eightify, Summarize.tech, dozens of Chrome extensions. The space is completely commoditized and most of them are free. Unless you have a genuinely different angle (and "better summaries" isn't one — everyone says that), you're entering a race to zero with no moat. Who's paying $10/month for this when a free extension does 90% of the job?

## License

MIT
