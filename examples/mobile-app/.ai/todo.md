# Todo

## In progress
- [ ] Expense logging screen (amount, category, date, note → save to Supabase)

## Up next
- [ ] Budget setup screen — set monthly limits per category
- [ ] Home screen — show this month's spending vs budget per category
- [ ] Weekly summary push notification

## Blocked / Questions
- [ ] Need to decide whether categories are fixed defaults or user-editable

## Done
- [x] Expo project initialized with Expo Router
- [x] Supabase project created, auth working (email + password)
- [x] expenses table created with: id, user_id, amount, category, date, note, created_at

---

## Last session
- Changed: got auth working, connected Supabase, and created the base expenses table
- Next: finish the expense logging screen and confirm entries save cleanly with the right user_id
- Watch out for: date handling can get weird between local device time and stored timestamps
