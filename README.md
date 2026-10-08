# wildmarks.net

Static site for Wildmarks, served by GitHub Pages at https://wildmarks.net.
One page, one font, no images beyond the logo and the social preview.

## Files

- `index.html` — the page
- `404.html` — not-found page
- `assets/css/site.css` — styles
- `assets/img/og.png` — social preview card
- `favicon.svg` — logo mark
- `CNAME` — custom domain for GitHub Pages
- `.nojekyll` — serve files as-is

## Deploy

Push to `main`. GitHub Pages serves from the `main` branch root; the
`CNAME` file binds the custom domain.

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
