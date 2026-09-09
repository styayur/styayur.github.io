# Stya Yur — Digital Garden (GitHub Pages)

This repository **hosts the published website** at
[https://styayur.github.io](https://styayur.github.io/).

It contains only the **statically exported output** (`out/`) of the source
project and is updated automatically:

- **Source repository:** [styayur/ui-ux-engineering-literature-digital-garden](https://github.com/styayur/ui-ux-engineering-literature-digital-garden)
- **Pipeline:** on every push to `main`, the source repo's GitHub Actions
  workflow runs a static export build (`NEXT_STATIC_EXPORT=true`) and pushes
  the generated `out/` folder here.
- **Root files** (`README.md`, `LICENSE`, `.nojekyll`) are preserved by the
  sync job — do not hand-edit site files in this repo; edit `content/` in the
  source repository instead.

The site is built with Next.js + MDX and is set in Cormorant Garamond,
Source Serif, Inter and JetBrains Mono. License: GPL-3.0 (see `LICENSE`).