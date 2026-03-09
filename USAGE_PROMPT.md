# Voice Skill Generator — Usage Prompt

Copy everything below the horizontal line and paste it into a new Claude conversation. Then follow the instructions inside it.

---

## Instructions for the user reading this

1. Copy the entire block below starting at "--- BEGIN PROMPT ---"
2. Paste it into a new Claude conversation (claude.ai works fine)
3. Follow the prompts Claude gives you
4. Copy the output into the template folder structure, or ask Claude to format it as a `.skill` file for you

---

--- BEGIN PROMPT ---

I want to create a personal voice skill for Claude that will make it write in my style for any content I ask it to produce.

Here is what I need you to do:

**Step 1: Analyze my writing samples**

I'm going to share my writing samples below. Please read all of them carefully and identify:
- My sentence length and rhythm patterns
- My paragraph length and structure
- My punctuation habits (parentheticals, ellipses, capitalization, etc.)
- My humor style (if any)
- Specific words and phrases I actually use
- Things I clearly do NOT do (corporate-speak, filler words, hedging, etc.)
- Any signature structural moves I repeat

**Step 2: Generate my voice skill**

After analyzing my samples, generate a complete `SKILL.md` file using this exact structure:

```
---
name: [my-name]-voice
description: Apply [my name]'s personal writing style when generating [list the content types I write]. Use this skill EVERY TIME content is being written on my behalf. Triggers on phrases like "write in my voice", "make it sound like me", "draft this for me".
---

# [My Name]'s Voice & Writing Style Guide

## Core Voice Identity
[2-3 sentences describing who I am as a writer and what my writing feels like to read]

## Sentence & Paragraph Patterns
[Specific observations about my rhythm, length, and structure]

## Punctuation & Formatting Quirks
[Specific habits — parentheticals, capitalization, lists, etc.]

## Humor Style
[How I use humor, or note that I don't]

## Vocabulary & Word Choice
[Actual words and phrases I use, my register, my jargon approach]

## Structural Patterns
[How I open pieces, build the middle, close them]

## Tone Calibration
[A table or list mapping content types to tone descriptions]

## What I Do NOT Do
[Hard rules — things that are clearly not my style]

## Signature Moves
[3-7 repeatable structural or stylistic habits that are distinctly mine]

## Application Checklist
[5-8 yes/no questions Claude should verify before finalizing any content in my voice]
```

**My writing samples:**

Share as many samples as you have. More is better. Paste each one below, separated by a horizontal rule (---). Label each one if you want (e.g. "Newsletter intro", "Twitter thread", "Long article") but it's not required — Claude will infer the context.

[PASTE SAMPLE 1 HERE]

---

[PASTE SAMPLE 2 HERE]

---

[PASTE SAMPLE 3 HERE — add as many as you have, just keep the --- between each one]

---

After generating the SKILL.md, also tell me:
1. How confident you are in the skill (1-10) based on how distinctive and clear my writing patterns were
2. What types of samples would most improve the skill if I wanted to regenerate it later

--- END PROMPT ---

---

## After you get your output

**Option A: Manual install (developers)**
1. Create a folder named `your-name-voice/`
2. Save the generated content as `SKILL.md` inside that folder
3. Add it to your Claude skills directory

**Option B: .skill file upload**
Ask Claude to format your skill as an installable `.skill` file, then:
1. Download the file
2. Go to Claude Settings → Skills → Upload Skill
3. Upload your `.skill` file

Your skill is now active. Test it by saying "write a short paragraph in my voice about [any topic]" and see how it does.
