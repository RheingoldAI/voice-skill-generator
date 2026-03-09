# 🎙️ Voice Skill Generator for Claude

**Turn your writing samples into a personal Claude skill that writes exactly like you.**

Built by [@RheezyBuilds](https://x.com/RheezyBuilds) — creator of the [Cursed With Knowledge](https://substack.com/@rheezybuilds) AI newsletter.

---

## What is a "skill" and why does it matter?

A Claude skill is a small instruction file that you install into your Claude workspace once, and it persists across every conversation. When Claude detects you're doing something the skill covers, it reads the file first and uses it as a north star for everything it produces.

Without a voice skill, Claude writes in its default style. Fine, but generic. With a voice skill, Claude writes in *your* style — your sentence rhythm, your humor, your vocabulary, your quirks. The difference is immediately obvious.

This repo gives you a simple system to generate that skill from your own writing, in about 10 minutes, with no coding required.

---

## What you'll end up with

A `.skill` file you install into Claude that makes it write like you, every time, for:

- Newsletters and Substack posts
- X / LinkedIn / social content
- Blog articles and long-form pieces
- Email drafts
- Anything else you write regularly

---

## How it works (3 steps)

### Step 1: Gather your writing samples

The more authentic, the better. AI-assisted writing will produce a weaker skill. Aim for variety:

- Something **structured** — a longer article, essay, or how-to post where you were being thoughtful
- Something **casual** — a quick social post, a thread, a short blog entry where you were just talking
- Anything else you write regularly — newsletters, emails, LinkedIn posts, whatever

One sample works. Two is better. Five is great. The more Claude has to work with, the more accurately it can identify your patterns across different contexts.

> **Tip:** Longer is better. 300+ words per sample is ideal. The more text Claude has, the more accurately it can identify your patterns.

### Step 2: Run the generation prompt

Open Claude (claude.ai or any Claude interface with skills support). Paste the full contents of [`USAGE_PROMPT.md`](./USAGE_PROMPT.md) into a new conversation, then follow the instructions inside it — it will walk you through exactly what to share and what to ask for.

The output will be a complete `SKILL.md` file personalized to your voice.

### Step 3: Install your skill

**Option A: .skill file (easiest)**
1. Copy your generated `SKILL.md` content into the template folder structure
2. Package it using the instructions in [`USAGE_PROMPT.md`](./USAGE_PROMPT.md)
3. Upload the `.skill` file to Claude via Settings → Skills → Upload

**Option B: Manual install (for developers)**
1. Copy your generated `SKILL.md` into a folder named `your-name-voice/`
2. Add it to your Claude skills directory

Both options are covered in detail in [`USAGE_PROMPT.md`](./USAGE_PROMPT.md).

---

## Example output

The [`example/`](./example/) folder contains a real, working voice skill built from two writing samples — the newsletter "Cursed With Knowledge" and a vibe coding guide, both written by [@RheezyBuilds](https://x.com/RheezyBuilds).

The [`example/sample-newsletter.md`](./example/sample-newsletter.md) shows what Claude produces when it uses that skill to generate a weekly AI news recap. Judge for yourself whether it sounds human.

---

## What makes a good voice skill?

Claude will extract and encode:

- **Sentence rhythm** — how long your sentences run, when you punch short
- **Paragraph patterns** — how much you write before you breathe
- **Punctuation quirks** — parentheticals, ellipses, capitalization for emphasis
- **Humor style** — self-deprecating, dry, deadpan, absurdist, or none of the above
- **Vocabulary** — actual words and phrases you use, jargon you embrace or avoid
- **What you don't do** — corporate-speak, filler words, moralizing, over-hedging
- **Signature moves** — the structural and stylistic habits that are distinctly you

The more distinctive your writing, the better the skill. If you write like a press release, the skill will work less well (but will still be better than nothing).

---

## Repo structure

```
voice-skill-generator/
├── README.md               ← you are here
├── USAGE_PROMPT.md         ← paste this into Claude to generate your skill
├── template/
│   └── SKILL.md            ← blank template for developers
├── example/
│   ├── jake-rheezy-voice/
│   │   └── SKILL.md        ← a real, complete voice skill (Jake/@RheezyBuilds)
│   └── sample-newsletter.md ← example output generated using that skill
└── CONTRIBUTING.md         ← how to give feedback or contribute
```

---

## FAQ

**Do I need to know how to code?**
Nope. Steps 1 and 2 are just Claude conversations. Step 3 is a file upload. That's it.

**Will this work for languages other than English?**
Probably, but it hasn't been tested. If you try it, open an issue and let us know how it went.

**Can I update my skill over time?**
Yes. Run the generation prompt again with new writing samples, or manually edit the `SKILL.md` file to add or remove patterns as your writing evolves.

**What if the skill doesn't sound like me?**
Share longer or more authentic samples and regenerate. The quality of the input directly determines the quality of the output. Also check that your samples weren't AI-assisted — that's the most common reason a skill feels off.

**Does this work with Claude Code and Claude Cowork too?**
Yes. The `.skill` format works across Claude interfaces that support skills.

---

## Contributing

Found a bug, have a better template structure, or want to share a voice skill you built? See [`CONTRIBUTING.md`](./CONTRIBUTING.md).

---

*Built with Claude. Shared because it should exist.*

[@RheezyBuilds](https://x.com/RheezyBuilds) — follow for more AI builder content.
