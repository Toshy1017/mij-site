# M.I.J — site source

This repo is the public-facing Jekyll site for M.I.J, hosted via GitHub Pages. It is separate from the private research/drafting tool (`amazon-japan-ranking-tool`) — only reviewed, finalized articles get committed here.

## Structure

- `_config.yml` — site settings
- `index.md` — homepage
- `about.md` — About page + required Amazon Associates affiliate disclosure
- `_posts/` — published articles, one file per post, named `YYYY-MM-DD-title.md`

## Publishing a new post

1. Take a reviewed, fact-checked draft from `amazon-japan-ranking-tool/output/` (or write one directly).
2. Copy it into `_posts/YYYY-MM-DD-title.md` here, with Jekyll front matter:
   ```yaml
   ---
   layout: post
   title: "Top Japan-Made Shampoo on Amazon (US)"
   date: YYYY-MM-DD
   ---
   ```
3. Replace any `[insert Associates link]` placeholders with real Amazon Associates tracking links (only once registered — see the tool project's README for registration steps).
4. Resolve any `⚠️ NEEDS VERIFICATION` flags before publishing — don't ship an unverified country-of-manufacture claim.
5. Commit and push to `master`. GitHub Pages rebuilds automatically.

## Setup (one-time, on GitHub.com)

This repo needs to be created on GitHub.com and connected as the `origin` remote before the first push — see the setup instructions given alongside this file's creation.
