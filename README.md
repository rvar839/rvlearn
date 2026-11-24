# RV Learn

Personal study app served at https://rvlearn.vibgen.com (GitHub Pages, republishes on every push to `main`).

- `index.html`: the whole app (markup, styles, script).
- `seed.js`: first-run cards, used only when the `topics` table is empty.
- Data: Supabase project `rvlearn` (ref `rfjztjhdbasdgdtzlrvj`), table `public.topics`, one row per topic with its cards in a JSON column.
- Tapping a topic opens an endless stream of flashcards (know it / do not know), picked at random and weighted toward weak cards. The Qstream tab runs the same stream as multiple choice on the most recently opened topic. Cards with a `map` field (the Countries by map topic) are answered by typing in the Topics tab, checked letter by letter with no Enter: the first wrong letter shows the right answer, and typing it moves on. Maps of islands zoom out until neighbouring land is in view. Countries that border the highlighted one are labelled. Analytics shows mastery, accuracy, a world map coloured by how well each country is known, a 14-day activity chart and gaps. Topics and cards are added by Claude straight into Supabase; the app has no editing screens.
- Daily answer counts live in `public.activity` (one row per day).
- Sign-in: Supabase email and password for one fixed owner account. The passcode is not stored in this repo.
