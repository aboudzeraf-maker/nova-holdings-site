# Deployment Status

## Current verified public status
Last broad live URL verification: **2026-10-03 11:46 UTC** using `read_url_content`.

Verified live NOVA HTML was returned for the homepage and the following high-priority routes in recent checks:

- Homepage: `https://aboudzeraf-maker.github.io/nova-holdings-site/`
- Start Here: `https://aboudzeraf-maker.github.io/nova-holdings-site/start-here.html`
- AUDIT reply handling: `audit-reply-handling.html`
- SPRINT fit-check: `sprint-fit-check.html`
- SPRINT reply handling: `sprint-reply-handling.html`
- Route-first diagnostic and reply handling: `route-first-diagnostic.html`, `route-first-reply-handling.html`
- SOURCE readiness scorecard: `source-credibility-scorecard.html`
- SCORE/FILTER/VISIBILITY/profile/research routes: `score-reply-handling.html`, `filter-reply-handling.html`, `visibility-intake.html`, `profile-conversion-kit.html`, `research-before-outreach.html`
- Product ladder routes: `filter-kit.html`, `filter-validation.html`, `proof-to-pipeline.html`, `growth-sprint.html`, `templates.html`, `signal-brief.html`, `builder.html`, `builder-validation.html`
- Trust/evidence/proof routes: `trust-route-checklist.html`, `trust-route-reply-handling.html`, `trust-route-micro-audit.html`, `evidence-map.html`, `evidence-reply-handling.html`, `evidence-to-answer-pack.html`, `evidence-question-bank.html`, `evidence-route-qa.html`, `evidence-to-route-matrix.html`, `proof-verification-burden.html`

## Newly added route pending verification
2026-10-03 12:00 UTC:

- Added `sprint-proposal-confirmation.html` as the NOVA Revenue Sprint Proposal + Scope Confirmation route.
- Updated `sitemap.xml` to include the new route.
- Expected public URL: `https://aboudzeraf-maker.github.io/nova-holdings-site/sprint-proposal-confirmation.html`
- Status: **uploaded to GitHub repository / expected Pages path / not independently live-verified yet**. Do not claim this new route is live until `read_url_content` or a hosting/status tool verifies expected NOVA content.

## Repository
https://github.com/aboudzeraf-maker/nova-holdings-site

Repository status observed previously: public, active, default branch `main`.

## Expected public URL
https://aboudzeraf-maker.github.io/nova-holdings-site/

Current status: **GitHub Pages is live for verified routes; newly added routes require individual live verification before being called live.**

## Primary deployment route
GitHub Pages via `.github/workflows/pages.yml`.

Workflow file expected path:

- `.github/workflows/pages.yml`

Workflow uses:

- `actions/configure-pages@v5`
- `actions/upload-pages-artifact@v3`
- `actions/deploy-pages@v4`

## Branch-source fallback route
A `gh-pages` branch exists and mirrors an earlier static site state. If GitHub Pages is configured to deploy from a branch, use `gh-pages` / root or `main` / root. If Pages is configured for GitHub Actions, keep using the workflow route.

## Alternate provider fallback route
If GitHub Pages becomes unavailable or returns 404 again, deploy the static repository root through one of the included fallback providers:

- Netlify: build command empty, publish directory `.`
- Vercel: static/other framework, build command empty, output directory `.`
- Cloudflare Pages: static HTML, build command empty, output directory `.`

Only record a provider URL as live after the provider returns a public URL and a live URL check verifies expected NOVA page content.

## Verification checklist before calling a route live

- Verify the URL returns a successful response and contains expected NOVA HOLDINGS content.
- Verify active route pages before using them as public CTAs.
- Verify no page promises guaranteed revenue, leads, replies, rankings, followers, AI recommendations, conversion lift, ROI, or financial outcomes.
- Verify payment language remains behind fit, scope, no-guarantee boundaries, and explicit buyer intent.

## Latest deployment/file actions

- 2026-10-03 12:00 `sprint-proposal-confirmation.html` uploaded for qualified Revenue Sprint proposal/scope confirmation conversations.
- 2026-10-03 12:00 `sitemap.xml` updated with the SPRINT proposal confirmation route.
- 2026-10-03 11:46 trust/evidence/proof route verification returned live NOVA HTML for checked pages.
- 2026-10-03 11:30 product-ladder route verification returned live NOVA HTML for checked pages.
- 2026-10-03 11:15 Start Here support route verification returned live NOVA HTML for checked pages.
- 2026-10-03 11:00 homepage, Start Here, AUDIT, SPRINT, Route-First, SOURCE, and OPS route verification returned live NOVA HTML for checked pages.
- 2026-10-03 10:45 fallback `gh-pages` branch was created after earlier URL checks returned 404.

## Commercial safety boundary
NOVA HOLDINGS content is for business development, digital product creation, route-first acquisition diagnostics, and growth-system execution. No guaranteed revenue, investment return, lead volume, meetings, replies, followers, conversion lift, AI ranking, AI recommendation, ROI, or financial outcome is promised. Payment instructions are only provided after qualification, scope clarity, no-guarantee boundaries, and explicit buyer intent. The agent must not execute financial transactions, withdrawals, refunds, or payment-account operations.
