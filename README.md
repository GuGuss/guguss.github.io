# guguss.me

Personal site of Augustin Delaporte — product leader, developer platforms and cloud
infrastructure.

Single self-contained `index.html`: no build step, no dependencies, no external
requests. All CSS is inline, icons are one inline SVG sprite, and the only assets are
four photos.

## Local preview

```bash
python3 -m http.server 8000
# → http://localhost:8000
```

## Deploy

GitHub Pages serves the default branch of `GuGuss/guguss.github.io`. The `CNAME` file
pins the custom domain, so the site is published at **https://guguss.me**.

DNS (apex `A` records): `185.199.108.153`, `185.199.109.153`, `185.199.110.153`,
`185.199.111.153`.

## Photos

`photos/` holds four optimised JPEGs (~1 MB total): `portrait.jpg` (1:1) plus
`van.jpg`, `ironman.jpg` and `family.jpg` (4:3). To swap one, drop a file in under the
same name — no code change needed; each is a CSS `background-image` with a gradient
fallback beneath it, so a missing file degrades to a designed placeholder rather than a
broken image.

## Update

Edit `index.html`, commit, push.
