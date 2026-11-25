---
name: new-skill
description: Scaffold a new slash-command skill in .claude/skills/ and register it in CLAUDE.md. Use when Ethan says "make this a skill", "/new-skill", or a repeatable workflow should be saved for reuse.
---

# New Skill

Create a new skill so a workflow can be rerun with `/<name>`.

## Steps
1. **Gather** (ask only for what's missing):
   - Name — short, kebab-case (e.g. `weekly-report`).
   - What it does and when it should trigger.
   - The steps, inputs, and expected output.
2. **Create** `.claude/skills/<name>/SKILL.md` using the template below.
3. **Register** it under *Registry → Skills* in `CLAUDE.md` with a one-line description.
4. **Confirm** with Ethan: show the file path and how to invoke it.

## Template
```markdown
---
name: <name>
description: <what it does + when to use it, in one or two sentences>
---

# <Title>

## Steps
1. ...

## Output
...
```

Put supporting files (templates, scripts, examples) alongside `SKILL.md` in the same folder.
