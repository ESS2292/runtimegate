# Deploying the RuntimeGate marketing site

This folder is a **local draft**. It has no public URL. Do not create a GitHub repository, Pages site, or store listing from this file. Publish only after owner approval.

Until launch, every HTML page includes `<meta name="robots" content="noindex">` and `robots.txt` disallows all crawlers. There is no canonical URL because no public URL exists yet.

## Files

- `index.html`, `privacy.html`, `terms.html`, `styles.css`, `og-image.svg`, `robots.txt`, `.nojekyll`
- `guides/` (index plus three draft guides)

The buy button stays disabled while `data-checkout-url` is empty. Do not point it at a test-mode checkout on a public site.

## When a public URL exists

1. Add canonical and absolute `og:url` / `og:image` tags (a PNG export is more widely accepted than SVG).
2. Replace `robots.txt` with `robots.launch.txt` only when the site should be indexed.
3. Remove `noindex` (or set `index,follow`) on every HTML page.
4. Set `data-checkout-url` to the live Lemon Squeezy URL after publish approval.
5. Replace every `TODO: add the seller support email before launch.` placeholder. Do not invent an address.
