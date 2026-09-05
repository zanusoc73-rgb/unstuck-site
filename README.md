# Unstuck — project notes

## Structure
- `index.html` — homepage with the directory of guides
- `fixes/*.html` — one file per guide
- `about.html`, `contact.html`, `privacy.html`, `404.html` — support pages
- `styles.css` — shared design system
- `sitemap.xml`, `robots.txt` — for search engines

## Before you publish
Replace every `https://example.com` with your real domain, in:
`index.html`, every file in `fixes/`, `about.html`, `contact.html`,
`privacy.html`, `sitemap.xml`, `robots.txt`.
Also replace `hello@example.com` in `contact.html` and `privacy.html`
with your real email.

## Adding a new guide
1. Copy any file in `fixes/` as a starting template.
2. Change the `<title>`, `<meta name="description">`, `<link rel="canonical">`,
   the breadcrumb tag, and the `<h1>`.
3. Rewrite the diagnostic steps for the new problem — same structure,
   most likely cause first.
4. Add a new `<li>` to the `fix-list` in `index.html` pointing to the new file.
5. Add a new `<url>` entry to `sitemap.xml`.

Keep the ad slots (`.ad-slot` divs) where they are — swap the placeholder
text for your AdSense/Ezoic embed code once you're approved.
