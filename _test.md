# Test — Stage 4

## Prompt

> Use the email-reply skill on the latest thread from Elon.

## What to check

- [ ] Claude reads `skills/email-reply.md` and follows the steps in order
- [ ] Everything from stage-3 still works (email, calendar, brain)
- [ ] Claude checks `todos/` for existing tasks (should be empty)
- [ ] Claude **creates a todo file** in `todos/` with follow-up actions (e.g. "intro Elon to Lisa")
- [ ] Reply still suggests Thursday, still references brain context
- [ ] The skill drove the workflow — you didn't have to spell out every step

## Reset after test

```bash
# Important: Claude creates files in todos/ — this cleans them up
git checkout .
git clean -fd
```
