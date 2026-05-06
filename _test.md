# Test — Stage 5

## Option A: Show the pre-built output (recommended for live demo)

Just open `daily-plan.md` and walk through it. No Claude session needed.

## Option B: Run it live

### Prompt

> Run the evening planner for tomorrow.

### What to check

- [ ] Claude reads `skills/evening-planner.md` and follows it
- [ ] Claude checks ALL emails (both Elon and Lisa threads)
- [ ] Claude checks **both** calendars: CEMS-Business and CEMS-Private
- [ ] Claude reads brain notes for Elon and Lisa
- [ ] Claude checks Todoist ("CEMS Showcase" project) for existing tasks
- [ ] Output includes: schedule with prep notes, email drafts, prioritized tasks, flags
- [ ] Claude writes or overwrites `daily-plan.md`
- [ ] The plan connects the dots (Elon ↔ Lisa intro, adaptive learning overlap)
- [ ] Personal events are accounted for (not double-booked over gym/dinner)

### Reset after test

```bash
# 1. Before exiting, ask Claude:
#    "Delete all tasks you just created in the CEMS Showcase Todoist project"

# 2. Exit Claude
/exit

# 3. Reset local files
git checkout .
git clean -fd
```
