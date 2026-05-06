# Claude Showcase — Personal Assistant

Built step by step during the CEMS lecture. Each branch adds one building block.

| Branch | What's added | The employee can now… |
|--------|-------------|----------------------|
| `stage-0` | Nothing — raw Claude | Read what you paste, write generic replies |
| `stage-1` | Gmail MCP | Read emails themselves |
| `stage-2` | + Calendar MCP | Cross-reference your schedule |
| `stage-3` | + CLAUDE.md | Match your tone and follow your rules |
| `stage-4` | + Email reply skill | Run the whole workflow on command |
| `stage-5` | + Obsidian brain + planner skill | Plan your entire day using all your data |

## Current stage: 3 — Obsidian Brain

Claude can now read emails, check your calendar, **and** look up your personal notes about people and projects. Ask:

> Read the latest email from Elon, check my calendar for next week, and check my notes about him. Draft a reply that suggests a time and references anything relevant from my notes.

## How to follow along

Switch between stages with `git checkout stage-X` to see what changes at each step.
