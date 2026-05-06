# Test — Stage 5

## What's different from Stage 4

- Second calendar added: **CEMS-Private** (gym, dinners, appointments) — Claude checks both
- `skills/evening-planner.md` added — a full daily planning workflow
- `daily-plan.md` output — what Andrew sees each morning
- `emails/lisa-research-update.md` and `brain/people/lisa-chen.md` added — a second thread to handle
- Todoist has **seed tasks** (overdue intro, Q3 roadmap review, investor call prep, etc.) — Claude incorporates them
- Claude now connects the dots across all data sources in one pass

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
- [ ] Claude checks Todoist ("CEMS Showcase" project) and finds existing tasks (overdue intro, Q3 prep, investor call, etc.)
- [ ] Overdue "Send intro email: Elon ↔ Lisa" task is flagged prominently
- [ ] Output includes: schedule with prep notes, email drafts, prioritized tasks, flags
- [ ] Claude writes or overwrites `daily-plan.md`
- [ ] The plan connects the dots (Elon ↔ Lisa intro, adaptive learning overlap)
- [ ] Personal events are accounted for (not double-booked over gym/dinner)
- [ ] Calendar events created for any confirmed meetings
- [ ] Prep blockers added before meetings

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

Also delete any Gmail drafts and calendar events created during the test.
