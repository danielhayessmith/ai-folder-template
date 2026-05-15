# Feature: Stripe Checkout

## Goal
Add Stripe checkout for the Pro plan.

## Steps
- [ ] Add Stripe to the project
- [ ] Create a checkout endpoint
- [ ] Add success and cancel pages
- [ ] Save subscription status to the database

## Open questions
- Do we use webhooks or check status on each visit?
- Where does the subscription status live — users table or separate?

## Decisions made
- Using Stripe Checkout (hosted page) rather than building a custom form
