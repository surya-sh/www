# surya.sh

Personal portfolio of Surya Venkatesan. Plain HTML + CSS, no build step, hosted on GitHub Pages.

## Files

- `index.html` — the whole site
- `styles.css` — Swiss / International Typographic Style layout (12-col grid, Inter, one red accent, auto light/dark)
- `404.html`, `favicon.svg`
- `CNAME` — custom domain for GitHub Pages
- `.nojekyll` — serve files as-is

## Local preview

    python3 -m http.server 8000   # or: npx serve .

## Deploy

1. Push to a GitHub repo (e.g. `surya-sh/surya.sh`) on `main`.
2. Repo → Settings → Pages → Source: *Deploy from a branch*, `main` / `/ (root)`.
3. DNS at your registrar for `surya.sh`:
   - `A` @ → 185.199.108.153, 185.199.109.153, 185.199.110.153, 185.199.111.153
   - `AAAA` @ → 2606:50c0:8000::153, 2606:50c0:8001::153, 2606:50c0:8002::153, 2606:50c0:8003::153
   - `CNAME` www → `surya-sh.github.io`
4. Once the certificate is issued, tick **Enforce HTTPS**.
