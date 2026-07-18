# aaronmatson.com

Personal portfolio for Aaron Matson — software engineer, AI integration & full-stack development.

## Stack

Hand-built static site. No framework, no build step.

- `index.html` — single-page site
- `assets/css/style.css` — custom stylesheet (deep indigo-ink theme, fully responsive)
- `assets/js/main.js` — vanilla JS (mobile nav, scroll reveal, sticky header)
- `images/` — portrait and project imagery

Fonts: Bricolage Grotesque (display), Inter (body), JetBrains Mono (utility) via Google Fonts.

## Hosting

Served by GitHub Pages from the `master` branch. The `CNAME` file points the
site at the custom domain `aaronmatson.com`.

### DNS setup for aaronmatson.com

At your domain registrar, add these records:

**Apex domain (`aaronmatson.com`)** — four `A` records:

```
185.199.108.153
185.199.109.153
185.199.110.153
185.199.111.153
```

**`www` subdomain** — one `CNAME` record pointing to `aaronmatson1.github.io`.

Then in the repo: **Settings → Pages → Custom domain**, enter `aaronmatson.com`
and enable **Enforce HTTPS** once the certificate is issued.

## Local preview

```bash
python3 -m http.server 8000
# open http://localhost:8000
```
