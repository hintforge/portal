# Portal — Hintforge Companion

![Portal companion status — coverage, how current it is, and spoiler control](assets/readme-status-card.svg)

A spoiler-controlled hint companion for **Portal**, Aperture Science's first-person puzzler about a portal gun, a series of test chambers, and a passive-aggressive AI. Built in the [Hintforge](https://github.com/hintforge/builder) format: a loyal sidekick that answers only from these guide files — never from guesswork — at the spoiler level you set.

## Use it

You need a Hintforge reader running in Claude Code, Codex, or OpenClaw. Point it at this repo:

> Load the Portal guide from github.com/hintforge/portal

Then just ask — *"how do I solve this chamber," "where do I put the portal," "how do I beat the ending."* Runtime setup lives in [`hintforge/reader`](https://github.com/hintforge/reader).

## Spoilers

**You** set two independent dials — enemy/threat warnings (Tier 0–5) and puzzle-hint warnings (Tier 0–3) — both **silent by default**; the guide volunteers nothing until you raise one. Puzzle hints come on a request ladder (a light nudge → more → step-by-step), so you can ask for exactly as much as you want. There's no save-state reader, so every answer comes from this guide's files.

## What's inside

A structured Markdown corpus — every test chamber, the portal/momentum mechanics, puzzle solutions, and all achievements. Interactive tools (a per-chamber technique tracker is the obvious fit) aren't built yet. The companion reads and writes only the files you control.
