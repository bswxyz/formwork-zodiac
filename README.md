<!-- parable:beautified -->
<div align="center">

<h1>Zodiac</h1>

<p><strong>Celestial star map with interactive constellations.</strong></p>

<p>
  <a href="https://bswxyz.github.io/formwork-zodiac/"><img alt="Live demo" src="https://img.shields.io/badge/demo-live-8b5cf6?style=flat-square&labelColor=1a1a1a"></a>
  <img alt="Family" src="https://img.shields.io/badge/family-Formwork-ec4899?style=flat-square&labelColor=1a1a1a">
  <img alt="Stack" src="https://img.shields.io/badge/stack-HTML%2FJS-f5a623?style=flat-square&labelColor=1a1a1a">
  <a href="LICENSE"><img alt="MIT License" src="https://img.shields.io/badge/license-MIT-22c55e?style=flat-square&labelColor=1a1a1a"></a>
</p>

<p>
  <a href="https://bswxyz.github.io/formwork-zodiac/"><b>Live demo</b></a>
  &nbsp;·&nbsp;
  <a href="https://bswxyz.github.io/formwork-zodiac/guide/">Build notes</a>
  &nbsp;·&nbsp;
  <a href="https://parable-three.vercel.app/templates">More templates</a>
</p>

<a href="https://bswxyz.github.io/formwork-zodiac/">
  <img src=".github/preview.jpg" alt="Zodiac — live preview" width="100%">
</a>

</div>

**Use this template** — copy the source into a new project:

```bash
npx degit bswxyz/formwork-zodiac my-app
```


**Live demo → https://bswxyz.github.io/formwork-zodiac/** · [How it was built](https://bswxyz.github.io/formwork-zodiac/guide/)

> A gold-on-midnight star chart: twinkling generative sky, constellations that ignite, the twelve signs.

A free, MIT-licensed website template. Good for: **astrology apps, planetariums, event themes, editorial features**.
The demo brand ("ZODIAC") is fictional — every word and colour is meant to be replaced with yours.

## The signature technique

- Generative canvas star field with cursor parallax, slow drift and shooting stars
- Constellations as connected star nodes — hovering (or picking a sign) brightens its figure
- 'The sky tonight' ephemeris panel; the Twelve as an interactive grid

## Use this as your own site

This repo is a **template** — everything is plain HTML/CSS/JS with **relative paths**, so it
works under *any* repo name with zero configuration.

1. Click **Use this template → Create a new repository** (top of this page).
   **Name it whatever you like** — `my-site`, `portfolio`, anything.
2. In your new repo: **Settings → Pages → Build and deployment → Deploy from a branch**,
   then pick `main` / `/ (root)` and save. (CLI: see below.)
3. Wait ~1 minute. Your site is live at `https://YOUR-USERNAME.github.io/YOUR-REPO-NAME/`.

<details>
<summary>Prefer the command line?</summary>

```bash
gh repo create my-site --template bswxyz/formwork-zodiac --public --clone
cd my-site
gh api --method POST /repos/YOUR-USERNAME/my-site/pages \
  -f 'source[branch]=main' -f 'source[path]=/'
```
</details>

No build step, no dependencies to install — edit the files, push, done.
The only external requests are Google Fonts and (where used) pinned CDN copies of GSAP/three.js.

## Customize it

- Constellations: the node/edge data lives in `main.js` — add your own figures
- Signs grid: glyphs, dates and elements are plain HTML
- Gold: `--gold` on midnight in `:root`

The `/guide/` page documents the signature technique in depth (with code) — keep it, rewrite it,
or delete the folder entirely.

## Files

```
index.html        the page
styles.css        all styling (design tokens in :root at the top)
main.js           the signature effect + motion
guide/index.html  how-it-works write-up (optional — yours to keep or delete)
```

## Built-in quality

- Works with JS disabled or a CDN failure (content is never permanently hidden)
- Respects `prefers-reduced-motion`; keyboard focus styles throughout
- Canvas/WebGL feature-detected with graceful fallbacks; devicePixelRatio capped for performance
- Responsive at phone / tablet / desktop widths

## License & credit

[MIT](LICENSE) — free for personal and commercial use, no attribution required
(a link back is always appreciated). Part of **FORMWORK** — a collection of
25 free website templates: **[the full gallery →](https://bswxyz.github.io/formwork/)**
