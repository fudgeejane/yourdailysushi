# Your Daily Sushi

A responsive React frontend for a sushi delivery and marketing site. Built with Vite for fast local development and Tailwind CSS for utility-first styling.

## Project summary

- **Purpose:** Landing pages and storefront UI to promote a sushi delivery service and collect orders.
- **Status:** Frontend-only React app (Vite) with modular components for the landing pages and a simple login view.

## Tech stack

- **React:** UI library (react, react-dom)
- **Vite:** Development server and build tooling
- **Tailwind CSS:** Utility-first styling (configured via PostCSS)
- **PostCSS & Autoprefixer:** CSS tooling
- **ESLint:** Linting and code quality
- **GSAP:** Animations
- **lucide-react:** Icon components

You can see the actual dependencies in `package.json`.

## Quick start (development)

Install dependencies and start the dev server:

```bash
npm install
npm run dev
```

Open the dev server (Vite default): http://localhost:5173

## Build & preview (production)

```bash
npm run build
npm run preview
```

## Other useful scripts

- `npm run lint` — run ESLint across the repo

## Project structure (high level)

- `src/` — application source code
	- `App.jsx`, `main.jsx` — app entry and bootstrapping
	- `assets/` — images and static media used by the UI
	- `components/` — shared UI components and theme helpers
	- `landing/` — landing page and subcomponents (hero, featured products, reviews, CTA, etc.)
	- `login/` — `Login.jsx` and authentication UI
- `public/` — static files served at root
- `vite.config.js`, `postcss.config.mjs` — build and PostCSS/Tailwind configuration

## Notes & recommendations

- Tailwind is already present in `devDependencies`. If you want to customize the design system, add or update `tailwind.config.js` and extend the theme there.
- There's a `next.config.ts` file in the repo — remove it if you are not using Next.js to avoid confusion.
- Add a `LICENSE` file and repository `description` if you plan to publish this project publicly.

## Deploying

This is a static frontend app produced by `vite build`. Deploy the `dist/` output to any static host (Netlify, Vercel, GitHub Pages, AWS S3 + CloudFront, etc.).

## Contributing

- Fork the repository, create a feature branch, and open a pull request with a clear summary of changes.

If you'd like, I can also:

- Add screenshots or a GIF to the README
- Add a `tailwind.config.js` starter and example components
- Add CI (GitHub Actions) to run linting and builds on PRs

---
_Updated README — tell me if you want it shorter, more visual, or expanded with CI/deployment steps._
