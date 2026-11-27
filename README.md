# ytob-rules

Ad blocking rules for the Ytob app. The app's "Обновить фильтры" button downloads
`https://raw.githubusercontent.com/AdirDiz/ytob-rules/main/rules.json`.

To publish a change, edit `rules.json` and **increase `version`**: the app only takes a file
with a higher version than the one it already has. The same file is bundled in the app at
`app/src/main/assets/rules.json` in `ytob-app`; keep both in sync.

## user.css and user.js

`user.css` (your own styles) and `user.js` (your own script) are downloaded by the same
"Обновить фильтры" button from this folder. They need no version number: the app always takes
what is here. CSS applies at once, JS after the page reloads (the app reloads it when the file
changed). Hints and examples are inside the files. Delete a file to go back to the app's
built-in copy. In the app: shield → "Как поправить свой CSS и JS…" opens the GitHub editor.

## Ymuz (YouTube Music)

The folder `ymuz/` holds the same three files for the Ymuz app (music.youtube.com,
`AdirDiz/Ymuz`): `ymuz/rules.json`, `ymuz/user.css`, `ymuz/user.js`. Its "Обновить фильтры" downloads
`https://raw.githubusercontent.com/AdirDiz/ytob-rules/main/ymuz/rules.json` and the user files next to
it. Same rule: increase `version` in `ymuz/rules.json` to publish a change, and keep it in sync with
`app/src/main/assets/rules.json` in `Ymuz`.
