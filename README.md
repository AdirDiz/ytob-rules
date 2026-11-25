# ytob-rules

Ad blocking rules for the Ytob app. The app's "Обновить фильтры" button downloads
`https://raw.githubusercontent.com/AdirDiz/ytob-rules/main/rules.json`.

To publish a change, edit `rules.json` and **increase `version`**: the app only takes a file
with a higher version than the one it already has. The same file is bundled in the app at
`app/src/main/assets/rules.json` in `ytob-app`; keep both in sync.
