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

## Current stage: 2 — Calendar MCP

Claude can now read emails **and** check your real Google Calendar. Ask:

> Read the latest email thread in the emails folder, check my calendar for next week, and draft a reply suggesting a time that works.

## How to follow along

Switch between stages with `git checkout stage-X` to see what changes at each step.
