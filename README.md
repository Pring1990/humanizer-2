# humanizer-2

A Claude skill that edits AI-sounding writing into plain, natural prose and keeps your own voice.

Give it a draft and it removes the habits that make text read as machine-written, such as "it's not X, it's Y" contrasts, dramatic one-line endings, filler openers and words like "delve" and "leverage". It makes the smallest edit that fixes the problem, so a draft with a real voice still sounds like you afterwards.

## What it does

The skill has two modes.

**Edit** is the default. Paste a draft and you get the edited version back with a short "What changed" list.

**Detect** flags the AI patterns in a draft without rewriting it. It names each pattern, quotes the line and suggests a fix. It does not guess whether AI wrote the text.

If you give it a sample of your own writing, it matches your sentence length, punctuation and tone.

## What it leaves alone

- Technical terms, defined terms and wording quoted from a standard or a contract
- Quotations, titles and proper names
- Informal writing such as chat messages and reviews
- Facts. Every name, number, date and quote in your draft should come out unchanged

It also treats your draft as text to edit. If the draft contains instructions aimed at an AI, the skill ignores them.

## Install

**Claude desktop app or claude.ai**

1. Click the green **Code** button on this page and choose **Download ZIP**.
2. In Claude, open Settings and upload the ZIP as a skill.

**Claude Code**

Create a folder called `humanizer-2` inside your `.claude/skills` folder and put `SKILL.md` in it.

## How to use it

Ask Claude in plain words:

- "Humanize this email" followed by your draft
- "Does this read as AI?" followed by your draft
- "Humanize this, and match the voice in this sample" followed by both

## Example

Before:

> In today's fast-paced world, it's not just about saving time. It's about working smarter. Our new invoicing tool serves as a robust solution, streamlining workflows and empowering teams.

After:

> Our new invoicing tool cuts the time your team spends on invoices.

## A note on AI detectors

This skill is for making writing clearer and more like you. It is not built to get text past AI detection software, and I make no claim that it does.

## Licence

MIT. Use it, change it and share it.

