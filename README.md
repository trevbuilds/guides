# Field Guides & Working Papers

> A small, evolving library of practitioner notes — written to be used in real work, not admired on a shelf.

A working library of long-form field guides on business analysis, transformation leadership, ERP, and requirements engineering. Each guide is a self-contained static HTML page; each is aligned to an industry standard and reads as a working reference, not a textbook.

**Live site:** <https://trevbuilds.github.io/guides/>

---

## The library

| № | Guide | Standard | Path |
|---|---|---|---|
| 01 | [The Minimum Viable BA Practice](businessanalysis/MVBA/index.html) | IIBA BABOK® Guide v3 | `businessanalysis/MVBA/` |
| 02 | [The Transformation Leader's Field Guide](transformation/leader/index.html) | PMI Program Management + Benefits Realization Management (Axelos MoP/MSP parallel reference) | `transformation/leader/` |
| 03 | [The ERP Field Guide](erp/index.html) | Operating-model commitments; integration spine; controls fabric | `erp/` |
| 04 | [Requirements Engineering](businessanalysis/Requirements/index.html) | IIBA BABOK® RADD + IEEE 29148 | `businessanalysis/Requirements/` |

Each guide is reachable from every other guide via the **Parallel volumes** block in its footer, and every guide links back to this library index.

### Companion artefacts

- [Core HR transformation explorer](businessanalysis/Requirements/explorer.html) — a navigable view over the 426-item working JIRA dataset (13 service journeys · 310 requirements · 60 integration pairs) used as the worked example throughout Field Guide 4.

---

## How to read

The guides are designed to be skimmed first and read in depth second. Each opens with a masthead and a sidebar table of contents; each section is independently useful. Suggested reading paths:

- **Business analyst:** start with No. 01 (MVBA), then No. 04 (Requirements Engineering). MVBA establishes the conditions under which good requirements work is possible; No. 04 is the requirements work itself.
- **Transformation leader:** start with No. 02 (Transformation Leader), then dip into No. 03 (ERP) for the operating-model layer.
- **ERP programme leader:** start with No. 03 (ERP), then No. 02 for the governance and benefits-realisation rhythm.

---

## Repo conventions

**Static HTML, no build step.** Each guide is a single, self-contained `.html` file with inline CSS and JS. Open one in a browser and it works — no toolchain, no dependencies beyond Google Fonts.

**Relative cross-links only.** All cross-guide hyperlinks use relative paths (`../`, `../../`) rather than absolute `https://trevbuilds.github.io/...` URLs. This means the site continues to work if the repo is renamed, the GitHub Pages path changes, a custom domain is added, or you clone and read offline.

**Analytics.** Google Analytics (gtag.js, property `G-DS33NXD3JT`) is included in the `<head>` of every page.

**Deployment.** GitHub Pages, served from `main` branch root. The published URL is `https://trevbuilds.github.io/guides/`.

---

## Changelog

Release notes for the library are in [CHANGELOG.md](CHANGELOG.md), following the [Keep a Changelog](https://keepachangelog.com/en/1.1.0/) convention and [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

---

## License

Published under the [GNU General Public License v3.0](LICENSE). The frameworks, templates, prompts, and worked examples in these guides are intended for use inside the reader's own practice — attribution appreciated.

---

## Author

**Trevin Nimaladasa** — senior business analyst, transformation advisor, and proprietor of [Clariti](https://clariti.com.au). [Connect on LinkedIn](https://www.linkedin.com/in/trev1n/).
