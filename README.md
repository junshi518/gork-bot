# Kinusaiga noindex preview

This repository holds a **noindex preview** of a kinusaiga tutorial: follow-along pages for a first flat fabric picture on scored foam.

It is not a live shop, and it is not publicly hosted. Do not enable GitHub Pages, Vercel, Netlify, Cloudflare Workers, or a custom domain.

- Every page is `noindex, nofollow`. `robots.txt` disallows all paths.
- No domain is connected. No page sets a canonical URL.
- Payments are not connected. There is no cart and no checkout.
- The shop is a text list of three categories. No prices and no product images. The line under each category is “Coming once supply is confirmed.”

## Routes

- `/` — what kinusaiga is, what to make first, and the learning path
- `/guides/kinusaiga-vs-kimekomi` — flat foam picture or a three-dimensional form
- `/guides/kinusaiga-foam-and-supplies` — board, adhesive, knife, and tucking tool
- `/guides/kinusaiga-kit-vs-materials` — one box or separate materials, with no prices
- `/guides/kinusaiga-first-pattern` — draw and transfer the first leaf
- `/guides/kinusaiga-choosing-and-cutting-fabric` — cotton, grain, and the tuck margin
- `/guides/kinusaiga-for-beginners` — the first session, through the last side
- `/guides/kinusaiga-finishing-and-framing` — edges, frame, and hanging
- `/guides/kinusaiga-troubleshooting` — shallow grooves, popped edges, wrinkles, and crushed foam
- `/shop` — category list only

There is no `/patterns` download and no checkout page. Shop categories are anchors on `/shop`.

## Schematic diagrams

Original line diagrams live in `images/diagrams/`. Each figure is captioned on the page as a schematic. They are not photographs and not items for sale.

## Local preview

From the repository root, serve the files only on this machine:

```bash
python3 -m http.server 8080 --bind 127.0.0.1
```

Open `http://127.0.0.1:8080/` in a browser. Stop the server with Ctrl+C.

That command does not publish the site. Root-absolute links and the stylesheet assume this local server. Opening the HTML files directly from disk will not resolve them.

The same server may redirect `/shop` to `/shop/`. Both show the shop list.
