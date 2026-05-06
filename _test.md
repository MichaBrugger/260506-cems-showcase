# Test — Stage 2

## Prompt

> Read the latest email thread in the emails folder, check my calendar for next week, and draft a reply suggesting a time that works.

## What to check

- [ ] Claude reads `emails/elon-coffee-chat.md`
- [ ] Claude checks the **CEMS-Showcase** calendar (not primary)
- [ ] Claude sees Tuesday afternoon is blocked (Strategy offsite 13–17)
- [ ] Claude sees Wednesday afternoon is blocked (Q3 planning 14–16)
- [ ] Claude suggests **Thursday afternoon** as an alternative
- [ ] Reply tone is professional but warm

## Reset after test

```bash
# Reset any files Claude may have created or modified
git checkout .
git clean -fd
```

## Calendar setup

If the CEMS-Showcase calendar events were deleted or need to be recreated, run this session in the lecture repo:

```
cd /Users/micha/Documents/github/260506-cems-how-to-claude
claude
# Then ask: "Recreate the CEMS-Showcase calendar events for the week of May 11 based on showcase/stage-2.md"
```
