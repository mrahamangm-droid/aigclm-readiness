# CLAUDE.md

Guidance for Claude working in this repo.

## What this repo is

AI-GCLM Readiness Assessment: a single-page, browser-only self-assessment
tool (`index.html`, inline JS/CSS) for the six-pillar AI-GCLM construction
leadership framework. It has 24 statements, four per pillar, and produces a
readiness profile with prioritised next actions. Served by GitHub Pages at
https://mrahamangm-droid.github.io/aigclm-readiness/.

## Current state (2026-10-01)

- Files: `index.html`, `README.md`, `CITATION.cff`, `LICENSE`, `SECURITY.md`,
  `.github/dependabot.yml` (github-actions only) and
  `.github/workflows/codeql.yml` (scans the inline JS and workflows).
- No build step and no tests. Open PRs: none. Open issues: none.

## Rules

- **No data leaves the browser.** Don't add analytics, external requests,
  CDNs or form posts without the owner asking. The README promises this.
- It's a structured reflection aid, **not a validated psychometric
  instrument**. Don't add wording that implies validation, norms or
  benchmarks.
- Keep statements and pillar names consistent with the published AI-GCLM
  papers (DOIs in the profile and construction-research repos). Don't
  invent new pillars or citations.
- Changes go live on merge to `main` via Pages. Open a PR for every
  change; never push to `main`.

## Verifying a change

Open `index.html` in a browser (or serve the folder) and click through the
full assessment, including the results view, on mobile and desktop widths.
