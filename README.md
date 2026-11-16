# michaeldhebert-site

Personal portfolio site for Michael Hebert: digital marketing and operations, with a background in sports journalism.

## Structure
- `index.html`: the whole site (styles and script are inline)
- `assets/headshot.jpg`: headshot used on the press credential

## Updating
Edit `index.html` (or ask Claude to) and commit to `main`. The connected host redeploys automatically.

## Before launch on a custom domain
In the `<head>` of `index.html`, replace the `SITE_URL` comment with:
- `<link rel="canonical" href="https://YOUR-DOMAIN/">`
- `<meta property="og:url" content="https://YOUR-DOMAIN/">`
- `<meta property="og:image" content="https://YOUR-DOMAIN/assets/og-image.jpg">`
and add `"url"` and `"image"` to the Person JSON-LD.
