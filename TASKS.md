# Tonight's Ticket Tasks

## Content

- [x] Define the app promise: quick, funny, at-home Friday plans for parents with small kids.
- [x] Create a first batch of low-cost, low-prep plans.
- [x] Expand the built-in lottery to 100 plans.
- [x] Give every plan a number, title, duration, kid mode, setup, rules, and playful twist.
- [x] Add filters for realistic Friday constraints: time, energy, and kids.
- [x] Split the lottery into `With kids` and `Without kids` before picking a number.
- [x] Add a playful reveal flow so choosing a number feels like winning.
- [x] Include enough variety: silly games, tiny rituals, food-adjacent plans, cozy resets, and after-bed options.
- [ ] Add personal plans that only make sense for your family.
- [ ] Add private jokes, favorite snacks, and your wife-specific winner text.
- [ ] Translate labels to Spanish or make the app bilingual if preferred.
- [ ] Add seasonal plan packs for rainy days, Christmas, summer balcony nights, and tired Fridays.

## Technology

- [x] Use a static GitHub Pages architecture with no build step.
- [x] Keep the app functional without installing packages.
- [x] Store favorites and history locally in the browser.
- [x] Add optional Supabase support behind a config file.
- [x] Provide Supabase SQL schema for plans and draw history.
- [x] Make the app responsive for phone-first use.
- [x] Keep Supabase keys out of source except the public anon key placeholder.
- [ ] Create the target GitHub repository.
- [ ] Replace `appSlug` if the GitHub repo gets a different name.
- [ ] Paste Supabase URL and public anon key into `src/config.js`.
- [ ] Run the SQL in Supabase and optionally insert custom plans.
- [ ] Enable GitHub Pages from the repo root.
- [ ] Test on both phones before the first Friday reveal.

## Nice Next Iterations

- [ ] Add an admin-only page for adding plans from the phone.
- [ ] Add "avoid last 3 winners" logic across devices using Supabase.
- [ ] Add a hidden "emergency tired parent" button.
- [ ] Add printable lottery slips for analog Friday mode.
- [ ] Add anniversary or birthday jackpot plans.
