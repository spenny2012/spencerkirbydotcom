# spencerkirbydotcom

A static personal website for Spencer Kirby, built with Astro and TypeScript and deployed to GitHub Pages.

## Local development

Requires Node.js 22.23.4 or newer.

```sh
npm ci
npm run dev
```

Astro prints the local URL in the terminal.

## Checks and production build

```sh
npm run check
npm run build
npm run preview
```

The production site is generated in `dist/` and uses the root path for the custom domain. After running `npm run preview`, open `http://localhost:4321/`.

## Deployment

The workflow in `.github/workflows/deploy.yml` checks and builds the site, then deploys it to GitHub Pages on pushes to `main` or a manual workflow run. In the repository's **Settings → Pages**, select **GitHub Actions** as the source and set the custom domain to `spencerkirby.com`.

The deployed site is `https://spencerkirby.com/`.

## Content

Shared personal details live in `src/data/profile.ts`. Page sections are separate components under `src/components/`, making it straightforward to add resume-driven experience and project sections later. No external fonts, images, analytics, or client-side framework are required.
