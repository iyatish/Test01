---
title: "The Case for Boring Technology"
description: "New tools are exciting. Mature tools are reliable. Knowing when to reach for which is a skill."
pubDate: "2025-03-20"
tags: ["software", "engineering", "opinion"]
---

There's a predictable arc to software careers. In the beginning, every new framework is a revelation. Later, you start to notice that the fundamentals keep reappearing under new names.

The industry has a word for this: churn. And it's expensive.

## What makes technology "boring"

Boring technology is mature, well-understood, and unremarkable. PostgreSQL is boring. Linux is boring. HTTP is boring. They've been around long enough that the failure modes are documented, the tooling is excellent, and the pool of people who can reason about them is large.

The unsexy truth is that boring technology has a dramatically better reliability track record than exciting technology. The bugs are known. The scaling limits are mapped. The runbooks exist.

## The cost of novelty

New technology comes with real costs that are easy to underestimate:

- **Unknown failure modes.** You will discover them in production.
- **Thin hiring pool.** The people who deeply understand it are rare and expensive.
- **Incomplete tooling.** Observability, debugging, migration paths — all immature.
- **Churn risk.** The project might be abandoned before you're done with it.

These aren't reasons to never adopt new technology. They're reasons to price it honestly.

## When new technology earns its place

New tools earn their place when they solve a problem that genuinely can't be solved well with what exists. Not "this is slightly more ergonomic" — but "the old tool fundamentally can't do this."

That bar is higher than it looks. Most problems that feel unique have been solved before with boring tools.

## A rule of thumb

Before reaching for something new, ask: what would I have to give up to use the boring solution here? If the answer is "nothing important," use the boring solution. You'll thank yourself in two years.
