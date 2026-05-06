# Test — Stage 3

## Prompt

> Read the latest email from Elon, check my calendar for next week, and check my notes about him. Draft a reply that suggests a time and references anything relevant from my notes.

## What to check

- [ ] Everything from stage-2 still works (calendar check, Thursday suggestion)
- [ ] Claude reads `brain/people/elon.md`
- [ ] Claude reads `brain/projects/ai-tutoring-platform.md`
- [ ] Reply mentions the **intro to Lisa Chen** (an open promise from the notes)
- [ ] Reply references **adaptive learning** or the ed-tech project naturally
- [ ] Reply feels like it comes from someone who knows Elon, not a stranger

## Reset after test

```bash
# 1. Exit Claude
/exit

# 2. Reset local files
git checkout .
git clean -fd
```

No external cleanup needed — this stage only reads calendar and local files.
