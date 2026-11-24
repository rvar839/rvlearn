# RV Learn

Personal study app served at https://rvlearn.vibgen.com (GitHub Pages, republishes on every push to `main`).

- `index.html`: the whole app (markup, styles, script).
- `seed.js`: first-run cards, used only when the `topics` table is empty.
- Data: Supabase project `rvlearn` (ref `rfjztjhdbasdgdtzlrvj`), table `public.topics`, one row per topic with its cards in a JSON column.
- Each topic's `mode` sets how it is studied: `mix` (alternates multiple choice and flashcards), `mcq`, `flash`, or `know` (know it / don't know).
- Sign-in: Supabase email and password for one fixed owner account. The passcode is not stored in this repo.
