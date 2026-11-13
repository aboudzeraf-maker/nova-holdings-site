# NOVA HOLDINGS Deployment Runbook

Last deployment check: **2026-11-13 10:30 UTC**

## Current public status

Live URL checks on 2026-11-13 10:30 UTC using `read_url_content` returned expected NOVA HOLDINGS content for:

- `https://aboudzeraf-maker.github.io/nova-holdings-site/` — homepage / Route-First + SOURCE growth router
- `https://aboudzeraf-maker.github.io/nova-holdings-site/start-here.html` — social Start Here router
- `https://aboudzeraf-maker.github.io/nova-holdings-site/route-first-diagnostic.html` — Route-First Acquisition Diagnostic
- `https://aboudzeraf-maker.github.io/nova-holdings-site/source-credibility-scorecard.html` — SOURCE Credibility Readiness Scorecard
- `https://aboudzeraf-maker.github.io/nova-holdings-site/sprint-readiness-pack.html` — Revenue Sprint Readiness Pack
- `https://aboudzeraf-maker.github.io/nova-holdings-site/first-5-client-success-proof-loop.html` — First-5 Client Success & Proof Loop
- `https://aboudzeraf-maker.github.io/nova-holdings-site/sitemap.xml` — sitemap XML including `first-5-client-success-proof-loop.html`

The public `sprint-readiness-pack.html` page now returned the First-5 cross-link in the fetched HTML, so the previously repository-confirmed cross-link is now public-live-verified in this cycle.

Current status wording:

> GitHub Pages is publicly live for the verified NOVA HOLDINGS homepage and checked route pages. Newly added or unchecked routes require individual live URL verification before being called live.

Do **not** claim any new route page is live until a URL-check tool successfully opens the public URL and confirms expected NOVA HOLDINGS content, or a deployment/status tool returns a confirmed public `page_url`.

## Repository

- Repository: `aboudzeraf-maker/nova-holdings-site`
- Branch: `main`
- Repository visibility: public
- Repository status observed 2026-11-13: active, unarchived, default branch `main`, language HTML
- Verified public GitHub Pages URL: `https://aboudzeraf-maker.github.io/nova-holdings-site/`
- Primary workflow: `.github/workflows/pages.yml`
- Workflow mode: static GitHub Pages deploy using `actions/configure-pages`, `actions/upload-pages-artifact`, and `actions/deploy-pages`

## Primary deployment route: GitHub Actions Pages

1. Keep all static HTML assets in the repository root.
2. Push to `main`.
3. The workflow at `.github/workflows/pages.yml` should run on every push to `main`.
4. GitHub Pages must be configured to use **GitHub Actions** as the source for the workflow route.
5. Verify the public URL using a live URL-check/fetch tool before claiming the site or any new route is live.

## Branch-source fallback route

A `gh-pages` branch exists and is maintained as a branch-source fallback for fast public route recovery.

If the Actions route becomes unavailable or returns 404 for a newly added route, use the safe fallback:

- Upload the route file to `gh-pages` / root.
- Upload matching `sitemap.xml` changes to `gh-pages` / root.
- Re-run live URL checks.
- Only mark the route live after expected NOVA HTML returns from the public URL.

## Alternate provider fallback routes

Use these only if GitHub Pages cannot be verified or activated.

### Netlify fallback

- Import the GitHub repository into Netlify.
- Build command: leave empty.
- Publish directory: `.`
- Existing config file: `netlify.toml`.
- After Netlify returns a public URL, record it in `DEPLOYMENT_STATUS.md`, `/memories/nova-holdings-owned-assets.md`, and `/memories/nova-public-url-verification-log.md`.

### Vercel fallback

- Import the GitHub repository into Vercel.
- Framework preset: Other / Static.
- Build command: leave empty.
- Output directory: `.`
- Existing config file: `vercel.json`.
- After Vercel returns a public URL, record it in `DEPLOYMENT_STATUS.md`, `/memories/nova-holdings-owned-assets.md`, and `/memories/nova-public-url-verification-log.md`.

### Cloudflare Pages fallback

- Connect the GitHub repository to Cloudflare Pages.
- Framework preset: None / Static HTML.
- Build command: leave empty.
- Output directory: `.`
- After Cloudflare Pages returns a public URL, record it in `DEPLOYMENT_STATUS.md`, `/memories/nova-holdings-owned-assets.md`, and `/memories/nova-public-url-verification-log.md`.

## Local/static package restoration

If the workspace package disappears, restore `/nova-holdings-site/` from the GitHub repository and these persistent memory sources:

- `/memories/nova-holdings-official-website-source.html` for homepage source reference
- `/memories/nova-social-start-here-hub-source.html` for Start Here source reference
- `/memories/nova-revenue-sprint-first-5-client-success-proof-loop-page-source.html` for the First-5 route source reference

Minimum package files:

- `index.html`
- `start-here.html`
- active product/route HTML pages
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

Before saying the site or a route is live:

- Confirm the deployment provider returned a public URL or a URL-check tool verified the page.
- Verify the homepage opens and contains NOVA HOLDINGS content.
- Verify `start-here.html` opens before using it in public social CTAs.
- Verify key active route pages open before using them as public CTAs.
- Verify `sitemap.xml` includes newly added route pages.
- Verify no page promises guaranteed revenue, leads, replies, rankings, followers, AI recommendations, conversion lift, ROI, or financial outcomes.
- Verify payment language remains behind fit, scope, no-guarantee boundaries, and explicit buyer intent.

## Commercial safety boundary

NOVA HOLDINGS pages are business-development and digital-product assets. They must not promise guaranteed income, lead volume, meetings, replies, followers, conversion lift, AI ranking, AI recommendation, ROI, or financial outcomes. Payment instructions are only appropriate after fit, scope, no-guarantee boundaries, and explicit buyer intent are clear. Live page availability is not a lead, inquiry, customer, proof item, referral, or revenue signal.
