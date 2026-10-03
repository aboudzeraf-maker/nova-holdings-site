# NOVA HOLDINGS Deployment Runbook

Last deployment check: 2026-10-03 10:31 UTC

## Primary deployment target

- Repository: `aboudzeraf-maker/nova-holdings-site`
- Branch: `main`
- Repository visibility: public
- Expected GitHub Pages URL: `https://aboudzeraf-maker.github.io/nova-holdings-site/`
- Deployment workflow: `.github/workflows/pages.yml`
- Workflow mode: static GitHub Pages deploy using `actions/configure-pages`, `actions/upload-pages-artifact`, and `actions/deploy-pages`

## Current public-status rule

Do **not** claim the website is confirmed live unless one of these happens:

1. A GitHub Pages/Actions deployment tool returns a confirmed public `page_url`, or
2. A live URL-check/fetch tool successfully opens the public URL and confirms the expected NOVA HOLDINGS page content.

Until then, use: **repo deployed / Pages route expected, not independently live-verified**.

## Files required for primary static deploy

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

## GitHub Pages deployment path

1. Keep all static HTML assets in the repository root.
2. Push to `main`.
3. The workflow at `.github/workflows/pages.yml` should run on every push to `main`.
4. If GitHub Pages is enabled with GitHub Actions as the source, the workflow should publish to the expected URL.
5. If the expected URL does not open, check repository Pages settings and set source to **GitHub Actions**. If Actions is not available, set source to **Deploy from branch: `main` / root** as a fallback.

## Alternate deployment paths

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

## Verification checklist

Before saying the site is live:

- Confirm the deployment provider returned a public URL or a URL-check tool verified the page.
- Open/verify the homepage expected content.
- Verify `start-here.html` exists.
- Verify `sitemap.xml` includes newly added route pages.
- Verify no page promises guaranteed revenue, leads, replies, rankings, followers, AI recommendations, conversion lift, or financial outcomes.
- Verify payment language remains behind fit, scope, no-guarantee boundaries, and explicit buyer intent.

## Latest check notes — 2026-10-03 10:31 UTC

- GitHub repository access is active and the repository is public.
- `main` is the default branch.
- Static site files and GitHub Pages workflow are present.
- `README_DEPLOY.md` was added as the primary/alternate deployment runbook.
- The push that adds/updates deployment documentation should re-trigger the Pages workflow.
- No tool in this run returned a confirmed public `page_url`, and no live URL-check tool was available, so public URL status remains **expected, not independently verified**.

## Commercial safety boundary

NOVA HOLDINGS pages are business-development and digital-product assets. They must not promise guaranteed income, lead volume, meetings, replies, followers, conversion lift, AI ranking, AI recommendation, ROI, or financial outcomes. Payment instructions are only appropriate after fit, scope, no-guarantee boundaries, and explicit buyer intent are clear.
