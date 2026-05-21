# .ai folder template

A starter template for the `.ai/` folder structure — a simple way to give your AI coding assistant full context at the start of every session.

## What's in here

| File | Purpose |
|------|---------|
| `.ai/agents.md` | Describes your project to the AI: stack, conventions, and things it should never do |
| `.ai/todo.md` | Your running task list: in progress, up next, blocked items, done, and a quick last-session handoff |
| `.ai/session-opener.md` | A ready-to-paste prompt for starting every AI session |

## How to use it

1. Copy the `.ai/` folder into the root of your project
2. Fill in `agents.md` with your actual stack and conventions
3. Update `todo.md` as you work
4. Add a new file for each major feature you plan to build

## Suggested `todo.md` shape

Use `todo.md` as the working document first and the handoff second:

```md
# Todo

## In progress
- [ ] [What you're working on right now]

## Up next
- [ ] [Next priority]
- [ ] [After that]

## Blocked / Questions
- [ ] [Anything waiting on a decision, dependency, or answer]

## Done
- [x] [Things you've shipped]

---

## Last session
- Changed:
- Next:
- Watch out for:
```

## Start every session with this prompt

Paste this at the beginning of every AI conversation:

```
Take a look at the agents.md file and any other markdown files inside the .ai folder.
Once you've reviewed everything, let me know which tasks we have next, prioritized.
Also, let me know what the last change in the git repo was so I can jog my own memory
of where we left off. Then we'll discuss and get started.
```

## Examples

Real-world examples of how this looks across different project types:

| Example | Stack | Description |
|---------|-------|-------------|
| [`examples/mobile-app`](examples/mobile-app/.ai/) | React Native + Expo + Supabase | Personal expense tracking app |
| [`examples/web-app`](examples/web-app/.ai/) | Next.js 15 + Supabase + Vercel | Freelance proposal generator |
| [`examples/ecommerce`](examples/ecommerce/.ai/) | Shopify + Dawn theme | Handmade textile goods store |
| [`examples/marketing-website`](examples/marketing-website/.ai/) | Astro + Netlify | HR consulting firm site |

---

From [Good Code](https://goodcode.danielhayessmith.com) — a practical field guide for non-developers building with AI.
