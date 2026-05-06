# Test — Stage 1

## Prompt

> Read the latest email thread in the emails folder and draft a reply.

## What to check

- [ ] Claude finds and reads `emails/elon-coffee-chat.md` on its own (you didn't paste it)
- [ ] Claude understands Elon wants coffee Tuesday or Wednesday afternoon
- [ ] Reply matches Elon's casual tone (not corporate fluff)
- [ ] Reply is still generic — "let me check my schedule" or similar (no real availability info)
- [ ] No calendar check, no brain lookup — just the email

## What's different from stage 0

- You didn't paste anything — Claude read the email itself from `emails/`
- Claude has the full thread (all 3 messages), not just the last one
- It knows the subject, who's writing, and the full context
- But the reply is still limited — no calendar, no real answer

## Reset after test

```bash
/exit
git checkout .
git clean -fd
```
