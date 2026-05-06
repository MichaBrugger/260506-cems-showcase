# Claude Showcase — Personal Assistant

Built step by step during the CEMS lecture. Each branch adds one building block.

| Branch | What's added | The employee can now… |
|--------|-------------|----------------------|
| `stage-0` | Nothing — raw Claude | Read what you paste, write generic replies |
| `stage-1` | Email context | Read the thread itself instead of waiting for copy-paste |
| `stage-2` | Calendar + Gmail tools + first skill | Check real availability, draft the reply, and create the meeting workflow |
| `stage-3` | Obsidian brain | Personalize the reply with relationship and project context |
| `stage-4` | Todoist + stronger skill workflow | Run the full playbook and create follow-up tasks |
| `stage-5` | Full planner across all systems | Review everything and prepare tomorrow proactively |

## Current stage: 4 — Skill + Todos

The email-reply skill is now a full playbook: read email, check brain, check calendar, check todos, draft reply, **and** create follow-up tasks. Ask:

> Use the email-reply skill on the latest thread from Elon.

## Building Blocks

- `Context`: information Claude can read
- `Tool`: something Claude can query or do
- `MCP`: the connection layer that exposes tools and resources to Claude
- `Skill`: a reusable playbook for how Claude should work
- `Automation`: running the same setup proactively instead of one prompt at a time

## How to follow along

Switch between stages with `git checkout stage-X` to see what changes at each step.
