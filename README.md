# Vittesh Maganti: portfolio

A one-page static site: plain HTML and CSS, no build step and no framework. Everything is in
`index.html`, and the images are in `assets/img/`.

## Edit it

- All the words are in `index.html`. Each project is one `<article class="sheet">` with the
  same parts: what I built, what was hard, what I learned, and where it stands.
- To add a project, copy an existing `<article class="sheet">`, give it a new `id`, and add a
  matching line to the rail (`.rail nav`) and to the index (`ol.index`).
- Colors and fonts are CSS custom properties at the top of the `<style>` block, with a dark
  palette that follows the visitor's system setting.

## Preview locally

```sh
python3 -m http.server 8000
# open http://localhost:8000
```

## Publish

`.github/workflows/pages.yml` deploys the site to GitHub Pages on every push to `main`. One-time
setup: in the repo, go to **Settings → Pages → Build and deployment → Source** and pick
**GitHub Actions**. The site will be at `https://vittesh12345.github.io/portfolio/`.

## Where the images come from

| File | Source |
|---|---|
| `chip-die-tilt.webp`, `chip-layout-parts.webp` | ORBIT-AI 3D renders, `vittesh12345/chip` (`site/chip-story/img/`) |
| `chip-separated.webp` | Copy-separated routed layout, `vittesh12345/chip` (`reports/pdsep/`) |
| `vantage-console.webp`, `vantage-leo.webp` | `vittesh12345/vantage-defense` (`assets/`) |
| `odrb-fog.webp`, `odrb-patch.webp` | ODRB figures (`figures/`) |
| `tempo-practice.webp`, `tempo-learn.webp` | Screenshots of Tempo in demo mode |
