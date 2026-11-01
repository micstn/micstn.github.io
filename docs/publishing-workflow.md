# Publishing essays with Astro

This project now uses Astro to render essay pages from markdown files in the content collection.

## 1. Add a new essay

Create a new markdown file in `src/content/essays/`.

Example:

```md
---
title: "My Essay"
description: "A brief summary shown in the archive listings."
pubDate: 2026-11-01
---

Your essay body starts here.
```

## 2. Run the site locally

```bash
npm install
npm run dev
```

Then open the local Astro preview in the browser.

## 3. Publish a new page

The essay will appear automatically on:

- the home archive page
- the essays index page
- its own individual route at `/essays/<slug>/`

## 4. Update metadata if needed

The frontmatter fields are:

- `title`: shown as the page title
- `description`: used in the archive list
- `pubDate`: optional publication date used in the article header
- `thumbnail`: optional future field for cover-art support

## 5. Build for production

```bash
npm run build
```

The static site is generated into the `dist/` directory and is ready to deploy to GitHub Pages.

## 6. Push to GitHub Pages

If GitHub Pages is configured to deploy from the repository root or from the generated `dist/` output, push the built content or configure the deployment source accordingly.

.
