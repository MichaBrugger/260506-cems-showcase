# Test — Stage 2

## What's different from Stage 1

- Google Calendar and Gmail tools are connected — Claude can check real availability and create a draft
- `skills/email-reply.md` is added — the first reusable playbook for handling emails
- `CLAUDE.md` now defines data sources and points to the skill

## Prompt

> Read the latest email thread in the emails folder, check my calendar for next week, and draft a reply suggesting a time that works.

## What to check

- [ ] Claude reads `emails/elon-coffee-chat.md`
- [ ] Claude follows `skills/email-reply.md` step by step
- [ ] Claude checks the **CEMS-Business** calendar (not primary)
- [ ] Claude sees Tuesday afternoon is blocked (Strategy offsite 13–17)
- [ ] Claude sees Wednesday afternoon is blocked (Q3 planning 14–16)
- [ ] Claude suggests **Thursday afternoon** as an alternative
- [ ] Reply tone is professional but warm
- [ ] Gmail draft created (not sent)
- [ ] Calendar event created for coffee with Elon on Thursday afternoon
- [ ] 30-min prep blocker created before the coffee event

## Reset after test

```bash
# 1. Exit Claude
/exit

# 2. Reset local files
git checkout .
git clean -fd
```

Also delete any Gmail drafts and calendar events created during the test.
