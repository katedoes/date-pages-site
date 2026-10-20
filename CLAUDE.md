# Date Pages — home page

Static single page: `index.html` plus `img/`, both at the repo root. No build step.
Public repo `katedoes/date-pages-site`, served by GitHub Pages from the root of `main`.

The brand name is a placeholder in two places — the header logo and the footer logo, both
`<span class="wordmark">date pages</span>`. Change both when the real name is decided, and
update `<title>` and the og: tags with it.

Photos in `img/` were taken from `~/Projects/date-kate/site/index.html`, where they are
embedded as base64. If Kate replaces a photo there, re-export it here too.

## Hosting
- Cloudflare Pages, project name: `datepages`
- Deploy folder: the repo root

## Deploy
```
npx wrangler pages deploy . --project-name datepages
```
- First run opens a browser to log in to Cloudflare (`npx wrangler login` if needed).
- If the project doesn't exist yet, wrangler offers to create it; choose production branch `main`.

## Local preview
```
python3 -m http.server 4321
```

## Rules
- Kate writes the copy. Structure, layout and markup only unless she asks.
- Every CTA is currently `href="#"` with a TODO comment — the builder and shop don't exist yet.
- Never commit or print Cloudflare tokens.
