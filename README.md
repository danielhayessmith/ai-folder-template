# .ai folder template

A starter template for the `.ai/` folder structure — a simple way to give your AI coding assistant full context at the start of every session.

## What's in here

| File | Purpose |
|------|---------|
| `.ai/agents.md` | Describes your project to the AI: stack, conventions, and things it should never do |
| `.ai/todo.md` | Your running task list — what's done, what's next |
| `.ai/example-feature.md` | An example feature plan — one file per major thing you're building |

## How to use it

1. Copy the `.ai/` folder into the root of your project
2. Fill in `agents.md` with your actual stack and conventions
3. Update `todo.md` as you work
4. Add a new file for each major feature you plan to build

## Start every session with this prompt

Paste this at the beginning of every AI conversation:

```
Take a look at the agents.md file and any other markdown files inside the .ai folder.
Once you've reviewed everything, let me know which tasks we have next, prioritized.
Also, let me know what the last change in the git repo was so I can jog my own memory
of where we left off. Then we'll discuss and get started.
```

---

From [Good Code](https://goodcode.schutzsmith.com) — a practical field guide for non-developers building with AI.
