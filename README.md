# Stya Yur — Digital Garden (Legacy GitHub Pages)

> **Legacy deployment repository.** Retained temporarily for rollback and URL continuity. Do not edit generated site files manually.

The active production site is now served by Cloudflare Pages:

- **Production:** [https://styayur-digital-garden.pages.dev](https://styayur-digital-garden.pages.dev)
- **Public engine:** [styayur/digital-garden-engine](https://github.com/styayur/digital-garden-engine)
- **Private content:** [styayur/ui-ux-engineering-literature-digital-garden](https://github.com/styayur/ui-ux-engineering-literature-digital-garden)

This repository contains the previous static GitHub Pages export:

- **Legacy URL:** [https://styayur.github.io](https://styayur.github.io/)
- **Status:** legacy/public, not part of the new production publishing pipeline
- **Rollback source:** `legacy-github-pages-pipeline` branch in the private source repository

The new pipeline validates and stages only published content, excludes `/admin` and `/api`, audits the generated artifact, and deploys `out/` directly to Cloudflare Pages.

Keep this repository until the Cloudflare URL or a custom domain has been verified over the desired retention period. Do not treat this repository as source.
