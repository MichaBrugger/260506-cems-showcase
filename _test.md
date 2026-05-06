# Test — Stage 5

## Option A: Show the pre-built output (recommended for live demo)

Just open `daily-plan.md` and walk through it. No Claude session needed.

## Option B: Run it live

### Prompt

> Run the evening planner for tomorrow.

### What to check

- [ ] Claude reads `skills/evening-planner.md` and follows it
- [ ] Claude checks ALL emails (both Elon and Lisa threads)
- [ ] Claude checks the CEMS-Showcase calendar for Thursday
- [ ] Claude reads brain notes for Elon and Lisa
- [ ] Claude reads existing todos in `todos/2025-05-06.md`
- [ ] Output includes: schedule with prep notes, email drafts, prioritized tasks, flags
- [ ] Claude writes or overwrites `daily-plan.md`
- [ ] The plan connects the dots (Elon ↔ Lisa intro, adaptive learning overlap)

## Reset after test

```bash
# Reset daily-plan.md and any other changes
git checkout .
git clean -fd
```
