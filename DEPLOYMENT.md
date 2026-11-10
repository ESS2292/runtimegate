# Deploying the RuntimeGate marketing site

This folder is the public GitHub Pages site for RuntimeGate, served at https://ess2292.github.io/runtimegate/. The paid CLI source is not in this repository.

The site stays **noindex**. Every HTML page includes `<meta name="robots" content="noindex">` and `robots.txt` disallows all crawlers. Do not replace `robots.txt` with `robots.launch.txt`, and do not remove `noindex`, until launch is approved.

The buy button stays disabled while `data-checkout-url` is empty. Do not point it at a test-mode checkout on this public site, and do not set a live Lemon Squeezy URL until publish approval.

Support contact on these pages links to GitHub Issues on [ESS2292/runtimegate-action](https://github.com/ESS2292/runtimegate-action/issues). Do not invent a support email.

## Files

- `index.html`, `privacy.html`, `terms.html`, `styles.css`, `og-image.svg`, `robots.txt`, `.nojekyll`
- `guides/` (index plus six guides)
- `sitemap.xml` (prepared for launch; not referenced by the live `robots.txt`)

## When launch is approved

1. Confirm canonical and absolute `og:url` / `og:image` tags (a PNG export is more widely accepted than SVG).
2. Replace `robots.txt` with `robots.launch.txt` only when the site should be indexed.
3. Remove `noindex` (or set `index,follow`) on every HTML page.
4. Set `data-checkout-url` to the live Lemon Squeezy URL after publish approval.
5. Replace the GitHub Issues support contact with a real seller support email. Do not invent an address.
