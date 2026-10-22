# styayur — legacy URL compatibility

[简体中文](README.zh-CN.md) · [Current website](https://styayur.co.uk)

This repository keeps old GitHub Pages URLs usable. It is a minimal redirect entry, not an independently maintained portfolio or the production website source.

## Routes

| Entry | Destination | Mechanism |
| --- | --- | --- |
| [Root](https://styayur.github.io/) and `/index.html` | [styayur.co.uk](https://styayur.co.uk) | JavaScript redirect preserves query/fragment; `/index.html` normalizes to `/` |
| Old paths such as `/projects/` or `/writing/` | Same path on [styayur.co.uk](https://styayur.co.uk) | Minimal `404.html` browser fallback preserves path/query/fragment |
| [`/calligraphy-studio/`](https://styayur.github.io/calligraphy-studio/) | [Calligra demo](https://styayur.github.io/calligra/) | Compatibility page preserves query/hash while redirecting |

Other projects' Pages deployments are independent of the root redirect. A GitHub repository rename does not itself preserve a project's Pages URL. Keep this repository available and unarchived while its Pages deployment serves these entries; do not delete it before a tested replacement exists.

The destination origin is fixed; URL parameters cannot select another host. Pages
serves the old-path fallback with HTTP 404 before its script navigates to the new
page. With JavaScript disabled, the static refresh/link goes to the main homepage;
dynamic path/query/fragment preservation requires JavaScript. Unknown paths may
still be missing on the canonical site. The existing Calligra compatibility page
continues to take precedence for its project URL.

## Maintenance and verification

Edit only the relevant redirect entry and check the destination, fallback link, HTTPS and deployed behavior. Preserve the old URL and test query/fragment handling after deployment. Historical pre-change observations are evidence for their recorded date, not a substitute for a fresh check.

The public [historical engine](https://github.com/styayur/digital-garden-engine) preserves renderer provenance and licenses; it is archived and does not produce the current website. The [GitHub Profile](https://github.com/styayur) is the public account entry.

## License and support

Retain the existing [LICENSE](LICENSE) and historical notices. Use [Issues](https://github.com/styayur/styayur.github.io/issues) for reproducible broken redirects, including the complete non-sensitive URL. No new site features, portfolio dataset or framework belong in this compatibility repository.
