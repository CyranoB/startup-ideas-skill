# Startup Ideas Skill

An interactive startup ideation and planning skill for Claude Code, adapted from the [Startup Factory](../startup-factory/) web app.

## What It Does

Walks you through an 8-stage startup planning pipeline:

1. **Generate Ideas** — 4 business concepts tailored to your domain/constraints
2. **Personas** — 2 structured target audience profiles
3. **Pitch** — Elevator pitch, problem statement, target audience, USP
4. **Avatar** — Detailed problem-aware customer avatar (A–H framework)
5. **Diary** — First-person diary entry from the avatar's perspective
6. **Features** — Avatar-aligned feature list
7. **Pricing** — Single-model pricing strategy (max 3 tiers)
8. **Landing Page Outline** — CRO-focused, section-by-section outline

Each stage pauses for your input — continue, regenerate, or adjust before moving on. You can also jump to any stage if you already have context (e.g., "I have an idea, help me with pricing").

## Install

```bash
claude install-skill /path/to/startup-ideas.skill
```

Or copy the `startup-ideas/` directory into your Claude Code skills folder.

## Usage

Ask Claude anything related to startup planning:

- "Help me brainstorm startup ideas"
- "I have a SaaS idea, help me plan it out"
- "Generate personas for my app"
- "Help me with pricing for my product"

## Structure

```
startup-ideas/
├── SKILL.md                  # Workflow and interaction protocol
└── references/
    └── prompts.md            # Output formats for all 8 stages
```
