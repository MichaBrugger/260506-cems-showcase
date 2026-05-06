# Test — Stage 4

## What's different from Stage 3

- Todoist MCP connected — Claude can read and create tasks
- Skill now checks Todoist for existing tasks (step 4)
- Skill creates follow-up tasks in Todoist with due dates and Gmail draft link (step 9)
- CLAUDE.md lists Todoist as a data source
- The prompt is now just "use the skill" — Claude follows the playbook without step-by-step instructions

## Prompt

> Use the email-reply skill on the latest thread from Elon.

## What to check

- [ ] Claude reads `skills/email-reply.md` and follows the steps in order
- [ ] Everything from stage-3 still works (email, calendar, brain)
- [ ] Claude checks Todoist ("CEMS Showcase" project) for existing tasks
- [ ] Gmail draft created (not sent)
- [ ] Calendar event created for coffee with Elon on Thursday afternoon
- [ ] 30-min prep blocker created before the coffee event
- [ ] Claude **creates tasks in Todoist** with follow-up actions (e.g. "intro Elon to Lisa")
- [ ] Todoist task description includes a link to the Gmail draft
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

Also delete any Gmail drafts and calendar events created during the test.
