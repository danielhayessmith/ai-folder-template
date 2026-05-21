# Todo

## In progress
- [ ] Proposal creation form (client name, title, scope, price, timeline → save + redirect)

## Up next
- [ ] Shareable proposal page at /p/[id] — public, no login required
- [ ] Dashboard — list of all proposals with status (draft, sent, accepted)
- [ ] "Mark as accepted" button on proposal page that notifies the owner by email

## Blocked / Questions
- [ ] Need a decision on whether public proposal links should expire or stay permanently accessible

## Done
- [x] Next.js project set up with App Router
- [x] Supabase connected, proposals table created
- [x] Auth working — email magic link via Supabase Auth
- [x] Basic layout and nav

---

## Last session
- Changed: got the app shell running, wired auth, and created the proposals table in Supabase
- Next: build the proposal creation form and make sure it saves, then redirects to the generated proposal page
- Watch out for: proposal scope and pricing fields may need validation rules before this goes in front of real users
