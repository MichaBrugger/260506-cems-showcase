# Test — Stage 3

## What's different from Stage 2

- `brain/` is added — personal notes on people and projects (Obsidian vault)
- Skill now checks brain notes before drafting (step 2)
- Reply should reference context from notes (shared interests, open promises)
- CLAUDE.md points to `brain/` as a data source

## Prompt

> Read the latest email from Elon, check my calendar for next week, and check my notes about him. Draft a reply that suggests a time and references anything relevant from my notes.

## What to check

- [ ] Claude reads `emails/elon-coffee-chat.md`
- [ ] Claude reads `brain/people/elon.md`
- [ ] Claude reads `brain/projects/ai-tutoring-platform.md`
- [ ] Claude checks the **CEMS-Business** calendar (not primary)
- [ ] Claude suggests **Thursday afternoon** as an alternative
- [ ] Reply mentions the **intro to Lisa Chen** (an open promise from the notes)
- [ ] Reply references **adaptive learning** or the ed-tech project naturally
- [ ] Reply feels like it comes from someone who knows Elon, not a stranger
- [ ] Gmail draft created (not sent)
- [ ] Calendar event created for coffee with Elon on Thursday afternoon
- [ ] 30-min prep blocker created before the coffee event

## Reset after test

```bash
# 1. Exit Claude
/exit

# 2. Reset local files
git checkout .
git clean -fd
```

Also delete any Gmail drafts and calendar events created during the test.
