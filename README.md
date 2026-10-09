# HVAC AI Build Journal

A public build journal for the HVAC Voice AI and short-call recovery product.

## Site structure

- `index.html` — current product status and journal index.
- `entries/2026-10-09-short-call-recovery.html` — first full decision record.
- `entries/template.html` — reusable structure for future entries.
- `assets/styles.css` — shared visual system.
- `PRODUCT.md` — product truth, scope, audience, and delivery criteria.
- `DESIGN.md` — visual direction and reuse rules.

## Add a new journal entry

1. Copy `entries/template.html` and rename it `YYYY-MM-DD-short-topic.html`.
2. Replace every bracketed placeholder.
3. Keep confirmed decisions separate from assumptions and risks.
4. End with one immediate action followed by three continuation steps.
5. Add the new entry to the top of the journal section in `index.html`.
6. Test links and layout on desktop and mobile before publishing.

## Local preview

Open `index.html` directly or serve the repository root with any static file server.

## Publishing

The project is designed to publish from the repository root with GitHub Pages. No build step is required.

## Scope note

This journal documents product and operational decisions. It is not legal advice and does not replace telecommunications compliance review for a live messaging program.
