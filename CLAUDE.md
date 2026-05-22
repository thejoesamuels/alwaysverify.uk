# alwaysverify.uk

Personal brand landing page for Joe Samuels, hosted on Cloudflare Pages.

## Project

- **Live domains:** alwaysverify.co.uk, joesamuels.co.uk
- **Hosting:** Cloudflare Pages (connected to this repo, auto-deploys on push to `main`)
- **Build:** None — static HTML, publish directory is `/` (root)

## Structure

```
index.html    — full single-page site
_headers      — Cloudflare Pages security headers (CSP, X-Frame-Options, etc.)
_redirects    — Cloudflare Pages routing (catch-all to index.html)
CLAUDE.md     — this file
```

## Design

- Dark theme (`#0C0C0C` background, `#F5C518` yellow accent)
- Font: DM Mono (Google Fonts) — used for all text
- Yellow highlight block on "VERIFY." in the hero is the primary brand moment
- Staggered CSS entrance animations on page load
- No JS, no build step, no dependencies

## Owner

- **Name:** Joe Samuels
- **Email:** joesamuels98@gmail.com
- **GitHub:** github.com/thejoesamuels
- **LinkedIn:** linkedin.com/in/joesamuels98

## Notes

- www→apex redirects for both domains should be handled via Cloudflare redirect rules at the DNS level, not in `_redirects`
- The `_headers` CSP allows inline styles (needed for the `<style>` block) and Google Fonts
