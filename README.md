# Assignment Container App

This repository is structured as a static container site for multiple assignment mini-apps.

## Structure

- `/index.html`: Assignment directory homepage.
- `/assignments/manifest.json`: Registry used by homepage cards.
- `/assignments/<assignment-name>/index.html`: Individual assignment pages.
- `/shared/`: Shared static assets (styles, scripts).
- `/vercel.json`: Vercel static hosting config.

## Local Preview

Use any static server from the repository root, for example:

```bash
python3 -m http.server 8080
```

Then open `http://localhost:8080`.

## Add a New Assignment

1. Create a new folder: `/assignments/<id>/`.
2. Add `/assignments/<id>/index.html`.
3. Add an entry in `/assignments/manifest.json` with:
   - `id`
   - `title`
   - `description`
   - `path`
   - `status`
   - `tags`

## Deploy to Vercel

This is a static site, so you can import the repo directly in Vercel.
No build command is required.
