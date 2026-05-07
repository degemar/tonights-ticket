# Tonight's Ticket

A no-build GitHub Pages app for choosing easy, funny at-home plans with small kids around.

## What It Does

- Choose between `With kids` and `Without kids` before the lottery board.
- Pick a number from that board and reveal a plan.
- Includes 100 built-in plan tickets.
- Filter by time and energy level.
- Keep the plans cheap, low-prep, and apartment/house friendly.
- Save favorites and keep a draw history on the same device.
- Optionally sync draw history to Supabase later.

## Architecture

- Static GitHub Pages site: `index.html`, `styles.css`, and browser JavaScript.
- Local-first storage with `localStorage`.
- Optional Supabase browser client loaded from CDN.
- No npm install, no build step, no local dev environment required.

## Files

- `index.html` - app shell
- `styles.css` - responsive app styling
- `src/app.js` - UI and interaction logic
- `src/plans.js` - plan content
- `src/storage.js` - localStorage and optional Supabase sync
- `src/config.js` - Supabase placeholders
- `supabase/schema.sql` - database tables and policies
- `TASKS.md` - content and technology task backlog

## Use Locally

Open `index.html` in a browser. Supabase sync is skipped until configured.

## Configure Supabase Later

1. Create a Supabase project.
2. Run `supabase/schema.sql` in the SQL editor.
3. Edit `src/config.js`:

```js
window.FRIDAY_PLAN_CONFIG = {
  supabaseUrl: "https://your-project.supabase.co",
  supabaseAnonKey: "your-public-anon-key",
  appSlug: "tonights-ticket"
};
```

The anon key is public by design. Do not put service-role keys in this app.

## Deploy To GitHub Pages

Upload these files to a GitHub repository and enable Pages from the repository root. No GitHub Action is required.
