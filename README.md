# Personal Résumé Website

Live site: https://etarambis.github.io

A single-page, trilingual (Spanish, English, Portuguese) résumé hosted on GitHub Pages.

## Structure

```
.
├── index.html       # Markup, styles, scripts and translations (all in one file)
└── fotoPerfil.jpg   # Profile picture
```

## Run locally

No build step or dependencies are required. Serve the folder with any static server:

```bash
python -m http.server 8000
```

Then open http://localhost:8000/index.html.

## Editing content

Text is translated through `data-i18n` attributes. Each key has three entries (`es`, `en`, `pt`) in the translations dictionary inside the `<script>` block of `index.html`.

When changing a piece of content, update **both**:

1. The element in the HTML (the default Spanish text).
2. The matching key in the dictionary, for all three languages.

Skipping either one leaves the page inconsistent when the language is switched.

## Stack

- HTML, CSS and vanilla JavaScript
- Google Analytics 4 for the visit counter
- GitHub Pages for hosting

## Deployment

Pushing to `main` publishes the site automatically through GitHub Pages.
