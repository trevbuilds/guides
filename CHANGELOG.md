# Changelog

All notable changes to this library will be documented in this file.

The format is based on [Keep a Changelog 1.1.0](https://keepachangelog.com/en/1.1.0/), and this project adheres to [Semantic Versioning 2.0.0](https://semver.org/spec/v2.0.0.html).

Versioning conventions for this library:
- **MAJOR** — restructuring of the library, breaking re-organisation of guide URLs, or a guide rewritten end-to-end.
- **MINOR** — a new field guide, companion artefact, or substantive new section added.
- **PATCH** — copy edits, link fixes, styling polish, analytics, and other non-content changes.

---

## [Unreleased]

Nothing pending.

---

## [0.7.0] — 2026-06-16

### Added
- **Companion maturity model — The Scalable BA Practice.** A maturity model for business analysis built on the MVBA framework: the six capability dimensions scored against the CMMI 1–5 ladder, the climb from Author Factory to Architect Practice, and a one-slide sponsor view shaped like a NIST CSF assessment. Lives at `businessanalysis/scale/index.html`.
- **Scale linked from Field Guide No. 01 (MVBA) footer** as a "Companion maturity model" col-block, beside the existing companion-diagnostic block.
- **Scale linked from the MVBA Practice Score** as a third resource card so the diagnostic surfaces the maturity model as a natural next step.
- **Scale listed on the root library index** as a "Companion maturity model" aux entry beside the two scorecards.
- **Library back-references inside scale's footer**: a six-link library nav and a Field Guides & Working Papers link in the colophon, matching the convention used by the score and explorer pages.

### Fixed
- **Scale's MVBA link** was `../mvba/index.html` and would 404 on case-sensitive GitHub Pages (the folder is uppercase `MVBA`). Corrected to `../MVBA/index.html`. Same class of bug fixed in 0.5.0 for the score page.

---

## [0.6.0] — 2026-05-28

### Added
- **Companion diagnostic — The ERP Operating-Model Score.** A 15-question diagnostic for leaders accountable for an ERP, scoring a core system across five dimensions (decision integrity, data & integration backbone, controls & assurance, delivery & adoption, lifecycle continuity) and returning the one dimension to fix first. Lives at `erp/score/index.html`.
- **ERP scorecard linked from Field Guide No. 03 (ERP)** as a prominent "Start here · A first step" callout in the masthead beside the byline, plus a "Companion diagnostic" block in the footer.
- **MVBA scorecard linked from Field Guide No. 01 (MVBA) footer** as a matching "Companion diagnostic" block, so the diagnostic is reachable from both the open and the close of the guide.
- **Both scorecards listed on the root library index** as companion-diagnostic aux entries with their dimensions and question counts.

### Fixed
- **ERP scorecard's own outbound links** were absolute `https://trevbuilds.github.io/guides/...` URLs that break on repo rename or path change. Converted to relative paths (`../index.html`, `../../businessanalysis/MVBA/index.html`, `../../index.html`) — matches the library-wide relative-link convention.

---

## [0.5.0] — 2026-05-22

### Added
- **Companion diagnostic — The Minimum Viable BA Practice Score.** A 12-question diagnostic for BA practice leaders, scoring a practice across four dimensions (system-of-work maturity, traceability, stakeholder co-production, AI governance) and returning a practice archetype. Lives at `businessanalysis/score/index.html`.
- **Scorecard linked from Field Guide No. 01 (MVBA)** as a prominent "Start here · A first step" callout directly beneath the masthead.
- **Scorecard linked from Field Guide No. 04 (Requirements Engineering)** in the "Read MVBA first" readiness card (it tests exactly the upstream foundations the guide depends on) and in the footer library nav.
- **Google Analytics** (`gtag.js`, `G-DS33NXD3JT`) wired into the scorecard `<head>`.
- **Library back-references** from the scorecard: "Browse the full library" link and a library link in the results colophon.

### Fixed
- **Scorecard's own outbound links** were broken and would 404 on case-sensitive GitHub Pages: `../mvba/index.html` → `../MVBA/index.html` (folder is uppercase `MVBA`), and `../req-eng/index.html` → `../Requirements/index.html` (folder is `Requirements`).

---

## [0.4.0] — 2026-05-20

### Added
- **Field Guide No. 04 — Requirements Engineering.** Long-form working reference covering the requirements-engineering discipline: a hierarchy, naming convention, work-type templates, traceability model, workflow per type, quality gates, and an AI-augmented prompt chain. Aligned to IIBA BABOK® RADD and IEEE 29148. Picks up where Field Guide No. 01 (MVBA) ends.
- **Companion artefact — Core HR transformation explorer.** Navigable view over a working 426-item JIRA dataset (13 service journeys, 310 requirements, 60 integration pairs) used as the worked example throughout Field Guide No. 04. Lives at `businessanalysis/Requirements/explorer.html`.
- **Library-wide "Parallel volumes" block** in every guide footer, cross-linking all four guides and the library index.
- **README.md** at repo root documenting the library, conventions, and how to read.
- **CHANGELOG.md** at repo root following Keep a Changelog and SemVer.

### Changed
- **All cross-guide hyperlinks converted to relative paths** (`../`, `../../`). Guides are now deployment-root agnostic — the same file works at `/guides/`, `/ba/`, a custom domain, or opened locally from disk.
- **Root library index** updated with Field Guide No. 04 entry and an explicit link to the companion explorer.

### Fixed
- **20 broken sibling-path links in Requirements Engineering** repointed to relative paths: 18 references to `mvba.html` → `../MVBA/index.html`, and 2 references to `erp-implementation.html` → `../../erp/index.html`.
- **ERP Field Guide footer** had hardcoded `https://trevbuilds.github.io/guides/...` URLs that broke when the repo was renamed from `ba` to `guides` (and would break again on any future rename). Replaced with relative paths.
- **"Open the live explorer" CTA** inside Requirements Engineering (§ explorer build section) was a `href="#"` placeholder; now correctly opens `explorer.html` in a new tab. Stale "replace the link target" instructional note removed.

---

## [0.3.1] — 2026-05-18

### Added
- **Google Analytics 4** (`gtag.js`, property `G-DS33NXD3JT`) wired into the `<head>` of the root index and ERP guide.

---

## [0.3.0] — 2026-05-15

### Added
- **Field Guide No. 03 — The ERP Field Guide.** Working reference for the senior leader accountable for an ERP decision: the five layers, twelve modules, master data, the integration spine, the controls fabric, eighteen named roles, ten industry dial-ups, the six-phase lifecycle, the ten-stage rhythm, vendor and SI relationship discipline, benefits realisation, AI prompts, and the five decisions a leader cannot delegate. Entry added to the root library index.

### Changed
- **Repository renamed** `trevbuilds/ba` → `trevbuilds/guides`. Published URL moved from `https://trevbuilds.github.io/ba/` to `https://trevbuilds.github.io/guides/`.

---

## [0.2.0] — 2026-05-14

### Added
- **Field Guide No. 02 — The Transformation Leader's Field Guide.** Working reference for the senior leader accountable for whether a transformation programme actually pays back: postures, artefacts, governance discipline, benefits rhythm, named tools, gates, and industry dial-ups. Aligned to PMI Program Management and PMI Benefits Realization Management; parallel reference to Axelos MoP/MSP. Entry added to the root library index.

---

## [0.1.0] — 2026-05-08

### Added
- **Field Guide No. 01 — The Minimum Viable BA Practice.** Working field guide for what a world-class BA practice looks like — standards, templates, methods, and operating rhythm. Aligned to the IIBA BABOK® Guide v3.
- **Library index** (`index.html`) with editorial styling — slate, brass, and paper palette; Fraunces / Inter Tight / JetBrains Mono typography.
- **GPL-3.0 license**.

---

[Unreleased]: https://github.com/trevbuilds/guides/compare/v0.7.0...HEAD
[0.7.0]: https://github.com/trevbuilds/guides/releases/tag/v0.7.0
[0.6.0]: https://github.com/trevbuilds/guides/releases/tag/v0.6.0
[0.5.0]: https://github.com/trevbuilds/guides/releases/tag/v0.5.0
[0.4.0]: https://github.com/trevbuilds/guides/releases/tag/v0.4.0
[0.3.1]: https://github.com/trevbuilds/guides/releases/tag/v0.3.1
[0.3.0]: https://github.com/trevbuilds/guides/releases/tag/v0.3.0
[0.2.0]: https://github.com/trevbuilds/guides/releases/tag/v0.2.0
[0.1.0]: https://github.com/trevbuilds/guides/releases/tag/v0.1.0
