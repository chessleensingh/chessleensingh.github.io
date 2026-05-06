# chessleensingh.github.io

Personal academic website for Sachleen Singh, PhD candidate in Molecular Biosciences at Arkansas State University.

Built with [Astro](https://astro.build) and deployed to GitHub Pages via GitHub Actions.

## Local development

```bash
npm install
npm run dev
```

Open http://localhost:4321.

## Build

```bash
npm run build
npm run preview   # serves dist/ locally to verify
```

## Deploy

Push to `main`. The GitHub Actions workflow (`.github/workflows/deploy.yml`) builds and deploys automatically.

GitHub Pages must be configured to use **GitHub Actions** as the source (repo Settings > Pages > Source).

## Content workflow

All content lives in `src/content/`. Adding or editing an entry requires no code changes — just edit or create a Markdown file with the correct frontmatter.

### Add a publication

Create `src/content/publications/<slug>.md`:

```markdown
---
title: "Full paper title"
authors: "Last, First and Last, First"
venue: "Journal or Conference Name"
year: 2026
type: journal   # journal | conference | poster
doi: 10.1234/example   # optional
url: https://example.com   # optional
description: "One or two sentence summary."   # optional
---
```

### Add a project

Create `src/content/projects/<slug>.md`:

```markdown
---
title: "Project Name"
description: "What it does, in one or two sentences."
status: active   # active | archived
tags: ["python", "genomics"]
github: https://github.com/chessleensingh/repo   # optional
url: https://example.com   # optional
---
```

### Add a blog post

Create `src/content/blog/<slug>.md`:

```markdown
---
title: "Post title"
description: "One sentence summary shown in the post list."
pubDate: 2026-05-05
---

Post content here in Markdown.
```

### Update the CV PDF

Drop a file named `cv.pdf` into the `public/` directory and push. It will be served at `/cv.pdf` and the CV page links to it automatically.
