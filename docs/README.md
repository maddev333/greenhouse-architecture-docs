# Greenhouse Architecture Documentation

This folder contains the static site assets and content for the Greenhouse architecture documentation experience.

## Contents

- `index.html` – main documentation landing page
- `architecture.html` – architecture overview content
- `app.js` – shared site behavior
- `styles.css` – shared styling
- `labs-config.json` – lab/workshop configuration used by the site
- `workshop/` – workshop pages, markdown, scripts, and media
- `media/` – shared media assets

## Content model

Use the files in this folder as the primary source for published documentation content.

- Update HTML files when changing the main site pages.
- Update `workshop/` content when changing guided lab or workshop material.
- Update `labs-config.json` when changing lab metadata, ordering, labels, or navigation behavior.

## Configuration guidance

`labs-config.json` should stay aligned with the workshop content it references.

Before committing changes:
- verify that linked files still exist
- verify that titles and labels match the rendered experience
- verify that lab ordering and grouping still reflect the intended flow

## Publishing

If hosted as a static site, publish from the `docs/` directory so page and asset paths remain valid.
