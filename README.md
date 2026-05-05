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

## Adding content

Content lives in `src/content/`. Each subfolder is a content collection (blog posts, publications, projects). Drop a new `.md` file in the relevant folder to add an entry.
