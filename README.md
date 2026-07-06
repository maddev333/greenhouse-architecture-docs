# Greenhouse Architecture Docs

Documentation site and workshop materials for the Greenhouse architecture content.

## Repository purpose

This repository contains a lightweight static documentation experience for:
- the Greenhouse architecture overview
- supporting workshop materials
- configuration that drives lab and workshop navigation

The site content currently lives under `docs/` and is structured for simple hosting from that folder.

## Repository structure

- `docs/index.html` – landing page for the documentation site
- `docs/architecture.html` – architecture overview page
- `docs/labs-config.json` – configuration used by the site to render labs/workshop content
- `docs/workshop/` – workshop pages, markdown content, assets, and supporting scripts
- `docs/media/` – shared media assets
- `docs/app.js`, `docs/styles.css` – shared site behavior and styling

## Source of truth

- Narrative site content is primarily stored in the files under `docs/`.
- Workshop content is primarily stored under `docs/workshop/`.
- `docs/labs-config.json` is the source of truth for lab metadata and site-driven navigation/configuration.

When updating content, keep configuration and referenced pages aligned so navigation labels, links, and rendered content stay consistent.

## Editing guidance

1. Update page content in the relevant HTML or Markdown file.
2. If the change affects workshop/lab navigation, also update `docs/labs-config.json`.
3. Keep titles, section names, and links consistent across the site and workshop content.
4. Avoid committing local/editor artifacts such as `.DS_Store` or `.vscode/` files.

## Publishing notes

If this repository is published via GitHub Pages or another static host, ensure the published root points at the `docs/` directory so the site assets resolve correctly.
