# Kinusaiga noindex preview skeleton

This repository holds a **noindex preview skeleton** for a kinusaiga (Japanese no-sew fabric art) tutorial site. It exists so people can review page structure and copy placement.

It is not a live store, not a public launch, and not a checkout site.

- Every page is `noindex, nofollow`. `robots.txt` disallows all paths.
- Payments are not connected. There is no cart, no checkout, and no order form.
- No domain is connected. No production canonical URL is set. The canonical host is pending.
- The shop is a placeholder with three categories only. No prices, stock counts, or SKUs are listed. The status line is “Coming once supply is confirmed.”
- Do not deploy this preview publicly. Do not enable GitHub Pages, Vercel, Netlify, or any other public host, and do not attach a custom domain.

## Routes in this batch

- `/`
- `/guides/kinusaiga-for-beginners`
- `/guides/kinusaiga-foam-and-supplies`
- `/guides/kinusaiga-vs-kimekomi`
- `/guides/kinusaiga-kit-vs-materials`
- `/shop`

There is no `/patterns` page and no standalone `/about` or `/faq` page. Shop categories are anchors on `/shop`, not separate item pages.

## Schematic diagrams

Original line diagrams live in `images/diagrams/`. Each figure is labeled on the page as a schematic. They are not photographs, not product shots, and not items for sale. The shop placeholder still has no images and no prices.

## Local preview

From the repository root, serve the files only on this machine:

```bash
python3 -m http.server 8080 --bind 127.0.0.1
```

Open `http://127.0.0.1:8080/` in a browser. Stop the server with Ctrl+C.

That command does not publish the site. Root-absolute links and the stylesheet assume this local server. Opening the HTML files directly from disk will not resolve them.

The same server may redirect `/shop` to `/shop/`. Both show the shop placeholder.
