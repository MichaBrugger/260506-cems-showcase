# Test — Stage 0

## Prompt

Draft a reply to this email I just received:

Hey Andrew,

Great — thanks for getting back to me! Tuesday or Wednesday afternoon would be ideal for me. Shall we say somewhere in the city center? Let me know what time works best and I'll book a spot.

Cheers,
Elon

## What to check

- [ ] Claude drafts a reply from only the pasted email
- [ ] Reply is generic — "sounds great, let me check" or similar
- [ ] No real scheduling info (Claude doesn't know Andrew's calendar)
- [ ] No personal context (Claude doesn't know anything about Elon)
- [ ] You had to paste the email yourself — Claude didn't read it from any file or tool

## What's different from the previous stage

Nothing — this is the baseline. The model has no connected context, no tools, and no reusable workflow yet.

## Reset after test

```bash
/exit
git checkout .
git clean -fd
```
