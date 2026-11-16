# michaeldhebert-site

Personal portfolio site for Michael Hebert: digital marketing and operations, with a background in sports journalism.

## Structure
- `public/index.html`: the whole site (styles and script are inline)
- `public/assets/headshot.jpg`: headshot used on the press credential
- `wrangler.jsonc`: tells Cloudflare to serve the `public/` folder as a static site

## Updating
Edit `public/index.html` (or ask Claude to) and commit to `main`. Cloudflare redeploys automatically.

## Before launch on a custom domain
In the `<head>` of `public/index.html`, replace the `SITE_URL` comment with:
- `<link rel="canonical" href="https://YOUR-DOMAIN/">`
- `<meta property="og:url" content="https://YOUR-DOMAIN/">`
- `<meta property="og:image" content="https://YOUR-DOMAIN/assets/og-image.jpg">`
and add `"url"` and `"image"` to the Person JSON-LD.
