# Set up your `.ai/` folder

Don't want to fill in the templates by hand? Paste everything below this line
into your AI assistant (Claude Code, Cursor, ChatGPT — anything) and it will
interview you, then write the files for you.

---

You are helping me set up a `.ai/` folder for my project. This folder gives AI
coding assistants full context at the start of every session so I never have to
re-explain my project from scratch.

Walk me through a short onboarding interview, then create three files:
`.ai/agents.md`, `.ai/todo.md`, and `.ai/session-opener.md`.

Follow these rules:

- Ask the questions in small groups, not all at once. It should feel like a
  focused conversation, not a form dump.
- If I don't have an answer (especially for conventions or guardrails), suggest
  a sensible default and move on.
- Do not write any files until I confirm.

## Step 1 — Tell me what you're about to do

In 2–3 sentences, explain what the `.ai/` folder is and what you'll create:
`agents.md` (project context), `todo.md` (task list), and `session-opener.md`
(a prompt I paste at the start of every session).

## Step 2 — Ask about the project

1. **Project name** — What's it called?
2. **What it does** — One or two sentences: what does it do, and who is it for?
3. **Frontend** — What's the UI built with? (React, Next.js, plain HTML, none)
4. **Backend** — Any server-side code? (Node.js, Python, Cloudflare Workers, none)
5. **Database** — Are you storing data, and with what? (Postgres, Supabase, SQLite, none)
6. **Hosting** — Where does it live or deploy? (Vercel, Cloudflare Pages, not sure yet)

## Step 3 — Ask about conventions and guardrails

7. **Conventions** — Any rules the AI should follow? (e.g. "keep components
   small", "plain CSS, no Tailwind", "always ask before adding a package")
8. **Never do** — Anything the AI should never do without asking first?
   Default if unsure: "Don't rewrite files I haven't asked you to touch."

## Step 4 — Ask about current work

9. **First task** — What's the first thing you want to build or fix? This
   becomes the first item in `todo.md` and the `Current focus` in `agents.md`.

## Step 5 — Confirm before writing

Summarize the three files and their key contents, then ask: "Ready to create
these files?" Wait for my confirmation.

## Step 6 — Create the files

Write these exact shapes into a `.ai/` folder in the current directory.

### `.ai/agents.md`

```markdown
# Project: {project_name}

## What it does
{one_two_sentence_description}

## Stack
- Frontend: {frontend}
- Backend: {backend}
- Database: {database}
- Hosting: {hosting}

## Conventions
{bullet list — one per line}

## Never
- Rewrite files I haven't asked you to touch
- Add new packages or tools without asking first
- Change the database schema without confirming with me
{any additional guardrails — one per line}

## Current focus
{first_task}
```

### `.ai/todo.md`

```markdown
# Todo

## In progress
- [ ] {first_task}

## Up next
- [ ] (add your next priority here)

## Blocked / Questions
- [ ] (anything waiting on a decision, dependency, or answer)

## Done
- [x] (things you've shipped)

---

## Last session
- Changed:
- Next:
- Watch out for:
```

### `.ai/session-opener.md`

```markdown
# Session Opener

Paste this at the start of every AI coding session:

---

Take a look at the agents.md file and any other markdown files inside the .ai folder.
Once you've reviewed everything, let me know which tasks we have next, prioritized.
Also, let me know what the last change in the git repo was so I can jog my own memory
of where we left off. Then we'll discuss and get started.
```

## Step 7 — Finish with a summary

After writing the files, tell me:

1. The three file paths you created.
2. What to do next: open `.ai/agents.md` and fill in anything left as a
   placeholder, keep `.ai/todo.md` updated as I work, and paste the prompt from
   `.ai/session-opener.md` at the start of every session.
3. That I can add a new markdown file in `.ai/` for each major feature I plan to
   build (see `.ai/example-feature.md` in the template for the shape).
