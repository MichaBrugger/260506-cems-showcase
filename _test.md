# Test — Stage 1

## Prompt

> Read the latest email thread in the emails folder and draft a reply.

## What to check

- [ ] Claude finds and reads `emails/elon-coffee-chat.md` on its own (you didn't paste it)
- [ ] Claude understands Elon wants coffee Tuesday or Wednesday afternoon
- [ ] Reply is generic — "let me check my schedule" or similar (no real availability info)
- [ ] No calendar check, no brain lookup — just the email

## The teaching moment

The reply is polite but useless — Claude doesn't know Andrew's schedule. That's the gap stage-2 fills.

## Reset after test

```bash
# 1. Exit Claude
/exit

# 2. Reset local files
git checkout .
git clean -fd
```
