# michaeldhebert-site

Personal portfolio site for Michael Hebert: digital marketing and operations, with a background in sports journalism.

## Structure
- `public/index.html`: the whole site (styles and script are inline)
- `public/assets/headshot.jpg`: headshot used on the press credential
- `wrangler.jsonc`: tells Cloudflare to serve the `public/` folder as a static site

## Updating
Edit `public/index.html` (or ask Claude to) and commit to `main`. Cloudflare redeploys automatically.

## Live URL
https://michaeldhebert.com/

## If a custom domain is added later
In the `<head>` of `public/index.html`, update these to the new domain:
- `<link rel="canonical" href="https://YOUR-DOMAIN/">`
- `<meta property="og:url" content="https://YOUR-DOMAIN/">`
- `<meta property="og:image" content="https://YOUR-DOMAIN/assets/og-image.jpg">`
and the `"url"` and `"image"` values in the Person JSON-LD.
