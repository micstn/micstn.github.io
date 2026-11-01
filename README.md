# Prismary

A minimal editorial archive for essays and notes, built as a static site with an Astro markdown workflow.

## Local development

```bash
npm install
npm run dev
```

## Production build

```bash
npm run build
```

## Content model

Essays live in `src/content/essays/` as markdown files. Each article uses frontmatter:

```md
---
title: "Essay Title"
description: "Short summary for the index."
pubDate: 2026-11-01
---

Essay body here.
```

The site automatically generates:

- the homepage archive
- the essays index
- individual essay pages at `/essays/<slug>/`

## Publishing workflow

1. Add a new markdown file in `src/content/essays/`
2. Include a title and description in frontmatter
3. Write the essay body in markdown
4. Run `npm run dev` to preview locally
5. Run `npm run build` before deployment
6. Push the generated static site or configure GitHub Pages to publish the project

See [docs/publishing-workflow.md](docs/publishing-workflow.md) for the full publishing guide.

## Site

https://micstn.github.io/
