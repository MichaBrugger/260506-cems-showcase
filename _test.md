# Test — Stage 4

## Prompt

> Use the email-reply skill on the latest thread from Elon.

## What to check

- [ ] Claude reads `skills/email-reply.md` and follows the steps in order
- [ ] Everything from stage-3 still works (email, calendar, brain)
- [ ] Claude checks Todoist ("CEMS Showcase" project) for existing tasks
- [ ] Claude **creates tasks in Todoist** with follow-up actions (e.g. "intro Elon to Lisa")
- [ ] Reply still suggests Thursday, still references brain context
- [ ] The skill drove the workflow — you didn't have to spell out every step

## Reset after test

```bash
# 1. Before exiting, ask Claude:
#    "Delete all tasks you just created in the CEMS Showcase Todoist project"

# 2. Exit Claude
/exit

# 3. Reset local files
git checkout .
git clean -fd
```
