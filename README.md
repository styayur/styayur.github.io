# Stya Yur — Legacy GitHub Pages deployment

> **Legacy deployment repository.** Retained for rollback reference and URL
> continuity. It is **not** a source of truth and does not maintain portfolio data.

The live site is served by Cloudflare Pages at <https://styayur.co.uk>.

- **Source of truth (private unified site):** `styayur/site`
- **Historical engine source:** `styayur/digital-garden-engine`
- **Profile front door:** `styayur/styayur`

This repository previously hosted a static portfolio on GitHub Pages. That data has
been migrated into the private content repository; this repo is kept for history and rollback only.

Keep this small compatibility repository unarchived while GitHub Pages serves it.
Its root and `/index.html` preserve the existing meta-refresh, with a canonical
URL and a readable fallback link. Project Pages deployments in their own repositories
remain independent; no project assets or paths are replaced by the root redirect.

On 2026-10-08, before the redirect metadata change, the root, index.html and the
Calligraphy Studio, STEM Visual Explorer, mini-market, Musical Spinningtop,
Nickspeare, LGXT Assistant and Windows New PC Setup project paths returned HTTP 200;
21 referenced same-host assets also returned HTTP 200. Recheck after deployment.
