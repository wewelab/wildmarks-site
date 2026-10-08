# wildmarks.net

Static site for Wildmarks. One page, one font, no build step.

## Files

- `index.html` — the page
- `404.html` — not-found page
- `assets/css/site.css` — styles
- `assets/img/` — logo, favicons, social preview card
- `_headers` — cache and security headers for Cloudflare Pages

## Deploy (Cloudflare Pages)

Connect this repository in Cloudflare Pages:

- Framework preset: None
- Build command: leave empty
- Build output directory: `/`

Every push to `main` deploys. Add `wildmarks.net` under Custom domains;
Cloudflare creates the DNS records itself because the zone is already
on Cloudflare.
