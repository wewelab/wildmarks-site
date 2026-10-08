# wildmarks.net

Static marketing site for Wildmarks, served by GitHub Pages at
https://wildmarks.net.

## Layout

- `index.html` — the single page
- `404.html` — not-found page
- `assets/css/site.css`, `assets/js/site.js` — styles and a tiny script
  (mobile menu, reveal-on-scroll)
- `assets/img/` — optimized captures and item art
- `CNAME` — custom domain for GitHub Pages
- `.nojekyll` — serve files as-is

## Deploy

Push to `main`. GitHub Pages is configured to serve from the `main`
branch root. The `CNAME` file binds the custom domain.

DNS (Cloudflare, DNS-only / grey cloud):

```
A     @    185.199.108.153
A     @    185.199.109.153
A     @    185.199.110.153
A     @    185.199.111.153
CNAME www  <github-username>.github.io
```

After DNS resolves, enable "Enforce HTTPS" in the repository's Pages
settings.

## Updating images

Source captures live in the Unity project. Re-export with Pillow at
1920 px (hero), 1400 px (gallery) and 520 px WebP (gear icons).
