---
description: CxD fork of /last30days. Researches a topic across Reddit, X, YouTube, TikTok, Hacker News, Polymarket, GitHub, and the web. Writes a 2-3 paragraph synopsis plus bullet-point breakdown to ~/01.Business.CxD/Research/Last30days/ and shows only the saved file path in chat.
argument-hint: <topic> — e.g. "nvidia earnings reaction" or "best noise cancelling headphones"
allowed-tools: [Bash, Read, Write, AskUserQuestion, WebSearch]
---

Invoke the `last30days-cxd` skill with the user's arguments: $ARGUMENTS

Use the skill's canonical pipeline (plan → retrieve → normalize → fuse → rerank → cluster → render). The CxD fork overrides the OUTPUT step: instead of emitting the synthesis to chat, write a 2-3 paragraph synopsis plus bullet-point breakdown to a dated file under `~/01.Business.CxD/Research/Last30days/` and show ONLY the saved file path in chat. See STEP -1 at the top of SKILL.md for the full output contract. If the user provided no arguments, ask them for a topic before proceeding.
