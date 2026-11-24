# RV Learn

Personal study app served at https://rvlearn.vibgen.com (GitHub Pages, republishes on every push to `main`).

- `index.html`: the whole app (markup, styles, script).
- `seed.js`: first-run cards, used only when the `topics` table is empty.
- Data: Supabase project `rvlearn` (ref `rfjztjhdbasdgdtzlrvj`), table `public.topics`, one row per topic with its cards in a JSON column.
- Tapping a topic opens rapid flashcards (know it / do not know). The Qstream tab runs multiple-choice questions on the most recently opened topic. Analytics shows mastery per topic.
- Sign-in: Supabase email and password for one fixed owner account. The passcode is not stored in this repo.
