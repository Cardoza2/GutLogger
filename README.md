# Gut log

A single-page web app for logging meals and bowel movements on your phone. It is one `index.html` file with no build step, no server and no account.

## Features

- **Meals:** log meals, snacks and drinks with a time, a description, tags you can customize (dairy, gluten, caffeine, and so on) and notes.
- **Bowel movements:** log the Bristol stool type (1–7), amount, gas, urgency, discomfort, whether blood was seen, and notes. There is also a "gas only" entry type.
- **Timeline:** entries are grouped by day, and the header shows how long it has been since your last meal and your last BM. Tap any entry to edit or delete it.
- **Export:** CSV with one row per entry, ready for pandas or R. Tags are separated by semicolons and times include your UTC offset.
- **Backup and restore:** save a full JSON backup and merge it back in without creating duplicates. The Data button shows a dot when a backup is due.

## Data and privacy

Everything is stored in your browser's `localStorage` on your device. Nothing is sent anywhere. Because of that, your log belongs to one browser at one web address. If you switch phones or browsers, or the app moves to a new URL, export a backup first and restore it at the new location. Safari may clear site data when the phone is low on storage, so export regularly.

## Usage

Open `index.html` in a browser, or host it with GitHub Pages (Settings → Pages → deploy from the `main` branch, root folder). On iPhone, open the page in Safari and choose Share → Add to Home Screen to use it like an app.

## License

MIT. See [LICENSE](LICENSE).
