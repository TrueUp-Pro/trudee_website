# Trudee Website

Marketing site for **Trudee** — *text a video, get a report.* Trudee turns a quick
phone video into an organized, professional field report for the trades
([trudee.pro](https://trudee.pro)). It's the productized evolution of TrueUp's
VidSummary.

Jekyll static site, deployed via GitHub Pages. Built from the same template +
brand palette as the TrueUp_Website (shared orange/blue, Segoe UI), with the copy
rewritten for the video→report product.

## Local setup

1. Install Ruby (2.7+).
2. `bundle install`
3. `bundle exec jekyll serve`
4. Open [http://localhost:4000](http://localhost:4000).

## Deploy to GitHub Pages

Push to GitHub, then **Settings → Pages** → build from `main` (GitHub Actions or
branch deploy). `CNAME` points the site at `trudee.pro`.

## Structure

- `index.html` — home (hero, how-it-works, features, platform, scenarios, CTA)
- `pricing.html` — plan comparison (Free / Contractor / Company / Enterprise)
- `plumbing.html` — `/plumbing/` vertical landing page for residential plumbing
  service shops (Seattle-area outbound target); not linked from nav by design
- `privacy-policy.html`, `terms-of-service.html` — legal
- `_layouts/default.html` — page shell (head, SEO, analytics)
- `_includes/` — `header`, `footer`, `beta-form-modal`
- `css/main.css` — brand tokens + all styling
- `assets/` — images + favicons
- `CNAME` — trudee.pro

## TODO before launch (carried over from the TrueUp template)

- Replace the placeholder text wordmark with a real Trudee logo/mark
  (`_includes/header.html`, favicons, `assets/images/og-image.png`).
- Swap the beta Google Form in `_includes/beta-form-modal.html` (currently TrueUp's).
- Add Trudee's own Google Analytics ID in `_layouts/default.html`.
- Confirm the pricing numbers (currently placeholder tiers).
- `docs/` still holds TrueUp brand/pricing notes (excluded from the build) — update or remove.
