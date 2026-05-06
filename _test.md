# Test — Stage 2

## Prompt

> Read the latest email thread in the emails folder, check my calendar for next week, and draft a reply suggesting a time that works.

## What to check

- [ ] Claude reads `emails/elon-coffee-chat.md`
- [ ] Claude checks the **CEMS-Business** calendar (not primary)
- [ ] Claude sees Tuesday afternoon is blocked (Strategy offsite 13–17)
- [ ] Claude sees Wednesday afternoon is blocked (Q3 planning 14–16)
- [ ] Claude suggests **Thursday afternoon** as an alternative
- [ ] Reply tone is professional but warm

## Reset after test

```bash
# 1. Exit Claude
/exit

# 2. Reset local files
git checkout .
git clean -fd
```

No external cleanup needed — this stage only reads the calendar.
