# kerrischneiderphd.com

Static site (plain HTML/CSS, no build step) for Kerri Schneider, Ph.D., P.A., hosted on GitHub Pages from `main`. Each page is `<slug>/index.html`; shared styles are in `style.css`.

## Standing rule: keep SEO current on every change

Marc asked that every change to the site keeps SEO up to date. Whenever you add, remove, rename or substantially edit a page or its content:

1. **Title and description**: each page has a unique `<title>` (about 50–65 chars, includes "Lake Worth, FL" where natural) and `<meta name="description">` (about 140–160 chars) that reflect the page's current content.
2. **Canonical and Open Graph**: `<link rel="canonical">`, `og:title`, `og:description` and `og:url` use `https://kerrischneiderphd.com/<slug>/` and match the title/description.
3. **sitemap.xml**: lists every live page; add or remove entries when pages change.
4. **Structured data**: the `Psychologist` JSON-LD block in `index.html` must match the real address, phone, fax, email, payment methods and services. Update it when any of these change.
5. **Navigation**: every page's nav lists the same pages.
6. **Images**: every `<img>` has a descriptive `alt` (empty `alt=""` only for decorative images).
7. **One `<h1>` per page**, with headings in order.
8. **Consistent business details** (name, address, phone) everywhere on the site, matching the JSON-LD.
9. **Cache-busting**: when `style.css` changes, bump the `?v=N` query on the stylesheet link in every page.
