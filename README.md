# Saturday World Kitchen

A small static website for tracking a cooking project by country.

## How to use it locally

Because the page loads `dishes.json`, open the folder through a tiny local web server rather than double-clicking `index.html`.

On macOS:

1. Open Terminal.
2. `cd` into this folder.
3. Run:

    python3 -m http.server 8000

4. Open `http://localhost:8000` in your browser.

## Add a dish

Edit `dishes.json` and add an entry like:

```json
{
  "country": "Georgia",
  "dish": "Khachapuri",
  "date": "2026-11-14",
  "rating": 9.4,
  "difficulty": 3,
  "would_make_again": "Yes",
  "notes": "Very rich, very good.",
  "photo": "photos/georgia-khachapuri.jpg"
}
```

Put the matching image file in the `photos` folder.

You can add multiple dishes for the same country. The map will open a country journal containing every logged dish for that country.

## Publish for free with GitHub Pages

Create a GitHub repository, upload the contents of this folder, then enable GitHub Pages from the repository settings.

The site has no backend, database, framework, or build step.
