# NOVA HOLDINGS Deployment Runbook

Last deployment check: **2026-10-03 10:45 UTC**

## Current public status

Live URL checks on 2026-10-03 10:45 UTC returned **404 Not Found** for:

- `https://aboudzeraf-maker.github.io/nova-holdings-site/`
- `https://aboudzeraf-maker.github.io/nova-holdings-site/audit-reply-handling.html`
- `https://aboudzeraf-maker.github.io/nova-holdings-site/ops-fit-check.html`

Use this status wording until a later verification succeeds:

> Repository deployed; GitHub Pages route expected; live public URLs currently return 404 / not confirmed live.

Do **not** claim the website or route pages are live until a URL-check tool successfully opens the public URL and confirms expected NOVA HOLDINGS content, or a deployment/status tool returns a confirmed public `page_url`.

## Repository

- Repository: `aboudzeraf-maker/nova-holdings-site`
- Branch: `main`
- Repository visibility: public
- Expected GitHub Pages URL: `https://aboudzeraf-maker.github.io/nova-holdings-site/`
- Primary workflow: `.github/workflows/pages.yml`
- Workflow mode: static GitHub Pages deploy using `actions/configure-pages`, `actions/upload-pages-artifact`, and `actions/deploy-pages`

## Primary deployment route: GitHub Actions Pages

1. Keep all static HTML assets in the repository root.
2. Push to `main`.
3. The workflow at `.github/workflows/pages.yml` should run on every push to `main`.
4. GitHub Pages must be configured to use **GitHub Actions** as the source for the workflow route.
5. Verify the public URL using a live URL-check/fetch tool before claiming the site is live.

## Branch-source fallback route

A `gh-pages` branch was created on 2026-10-03 10:45 UTC from `main` commit `31c5d1f05624d77201920d502c19dffc90eece97`.

If the Actions route stays unavailable or returns 404, configure GitHub Pages to deploy from one of these branch/root sources:

- `gh-pages` / root, or
- `main` / root.

Then re-run live URL checks before calling the site live.

## Alternate provider fallback routes

Use these only if GitHub Pages cannot be verified or activated.

### Netlify fallback

- Import the GitHub repository into Netlify.
- Build command: leave empty.
- Publish directory: `.`
- Existing config file: `netlify.toml`.
- After Netlify returns a public URL, record it in `DEPLOYMENT_STATUS.md` and `/memories/nova-holdings-owned-assets.md`.

### Vercel fallback

- Import the GitHub repository into Vercel.
- Framework preset: Other / Static.
- Build command: leave empty.
- Output directory: `.`
- Existing config file: `vercel.json`.
- After Vercel returns a public URL, record it in `DEPLOYMENT_STATUS.md` and `/memories/nova-holdings-owned-assets.md`.

### Cloudflare Pages fallback

- Connect the GitHub repository to Cloudflare Pages.
- Framework preset: None / Static HTML.
- Build command: leave empty.
- Output directory: `.`
- After Cloudflare Pages returns a public URL, record it in `DEPLOYMENT_STATUS.md` and `/memories/nova-holdings-owned-assets.md`.

## Files required for static deploy

The repository root should contain:

- `index.html`
- `start-here.html`
- all active product/route HTML pages
- `robots.txt`
- `sitemap.xml`
- `.nojekyll`
- `README.md`
- `README_DEPLOY.md`
- `DEPLOYMENT_STATUS.md`
- `netlify.toml`
- `vercel.json`
- `.github/workflows/pages.yml`

## Verification checklist

Before saying the site is live:

- Confirm the deployment provider returned a public URL or a URL-check tool verified the page.
- Verify the homepage opens and contains NOVA HOLDINGS content.
- Verify `start-here.html` opens.
- Verify key active route pages open, especially `audit-reply-handling.html`, `sprint-fit-check.html`, and `ops-fit-check.html` before using them in public CTAs.
- Verify `sitemap.xml` includes newly added route pages.
- Verify no page promises guaranteed revenue, leads, replies, rankings, followers, AI recommendations, conversion lift, ROI, or financial outcomes.
- Verify payment language remains behind fit, scope, no-guarantee boundaries, and explicit buyer intent.

## Commercial safety boundary

NOVA HOLDINGS pages are business-development and digital-product assets. They must not promise guaranteed income, lead volume, meetings, replies, followers, conversion lift, AI ranking, AI recommendation, ROI, or financial outcomes. Payment instructions are only appropriate after fit, scope, no-guarantee boundaries, and explicit buyer intent are clear.
