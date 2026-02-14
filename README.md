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

### From Claude Code (recommended)

Add the marketplace and install the plugin:

```
/plugin marketplace add CyranoB/startup-ideas-skill
/plugin install startup-ideas@startup-ideas-marketplace
```

### Manual install

Clone the repo and copy the skill into your Claude skills directory:

```bash
git clone https://github.com/CyranoB/startup-ideas-skill.git
mkdir -p ~/.claude/skills/startup-ideas
cp -r startup-ideas-skill/skills/startup-ideas/* ~/.claude/skills/startup-ideas/
```

## Usage

Ask Claude anything related to startup planning:

- "Help me brainstorm startup ideas"
- "I have a SaaS idea, help me plan it out"
- "Generate personas for my app"
- "Help me with pricing for my product"

## Structure

```
.claude-plugin/
├── plugin.json               # Plugin metadata and configuration
└── marketplace.json          # Marketplace manifest for distribution
skills/
└── startup-ideas/
    ├── SKILL.md              # Workflow and interaction protocol
    └── references/
        └── prompts.md        # Output formats for all 8 stages
```
