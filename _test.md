# Test — Stage 0

## Prompt

Draft a reply to this email I just received:

Hey Andrew,

Great — thanks for getting back to me! Tuesday or Wednesday afternoon would be ideal for me. Shall we say somewhere in the city center? Let me know what time works best and I'll book a spot.

Cheers,
Elon

## What to check

- [ ] Claude drafts a reply without any context — just the pasted email
- [ ] Reply is generic — "sounds great, let me check" or similar
- [ ] No real scheduling info (Claude doesn't know Andrew's calendar)
- [ ] No personal context (Claude doesn't know anything about Elon)
- [ ] You had to paste the email yourself — Claude didn't read it from anywhere

## The teaching moment

"This is how most people use AI today. Copy, paste, get a generic reply, rewrite half of it. The employee showed up on day one with zero onboarding."

## Reset after test

```bash
# 1. Exit Claude
/exit

# 2. Reset local files
git checkout .
git clean -fd
```
