# AI-GCLM Readiness Assessment

A browser-based self-assessment tool that operationalises the six-pillar AI-GCLM
framework for construction leadership. No install, no build step, no data leaves the
browser.

**[Open the tool →](https://mrahamangm-droid.github.io/aigclm-readiness/)**

## Overview

The AI-GCLM framework describes how artificial intelligence can be integrated into
*construction leadership judgment* — the executive layer where prediction becomes
decision, and where accountability and contractual exposure concentrate — rather than
into project tooling alone.

This tool turns that framework into a practical instrument. Twenty-four statements,
four per pillar, produce a readiness profile across the six pillars and a prioritised
set of next actions focused on the weakest areas.

It is designed to be used by a leadership team together, as a structured way to
surface disagreement about where an organisation actually stands.

## What it is not

This is a **structured reflection aid, not a validated psychometric instrument.**

- The underlying framework is conceptual and awaits empirical validation
- The 24 statements are an operationalisation written for this tool; they are not part
  of the published paper and have not been validated
- Scores are not comparable between organisations and are not a benchmark

Treat the output as a discussion starter, not a measurement.

## Features

- Six-pillar assessment — 24 statements on a five-point scale
- Live readiness profile with per-pillar scores and levels
- Prioritised guidance targeting the three weakest pillars
- Example responses, so the output can be understood before committing real answers
- Progress saved in the browser between visits
- Printable report (Print / Save as PDF) with the questionnaire stripped out
- Light and dark themes; works on mobile

## Technology stack

Plain HTML, CSS and JavaScript in a single file. No frameworks, no build tooling, no
dependencies. Typography via Google Fonts (IBM Plex Sans / Mono), with system-font
fallbacks if unavailable.

## Installation

None required. Either open `index.html` directly in a browser, or serve it locally:

    python3 -m http.server 8000
    # then visit http://localhost:8000

## Usage

1. Open the tool
2. Answer the 24 statements — or click **Load example responses** to see how the output
   reads first
3. Review the readiness profile and the "Where to focus" section
4. Click **Print / save report** to produce a PDF for circulation

Answers persist in the browser via `localStorage`. **Clear answers** removes them.

## Project structure

    index.html    The complete application — markup, styles, logic
    README.md     This file
    LICENSE       MIT licence covering the code

## Configuration

There is none. To adapt the instrument, edit the `PILLARS` array near the top of the
script block in `index.html` — each entry holds a pillar's name, description, four
statements, and the guidance shown for low and high scores. Score bands are defined in
the adjacent `BANDS` array.

## Environment variables

None. The tool makes no network requests other than loading its web fonts, and
transmits no data.

## Development

The whole application is one file. Edit `index.html` and reload the browser.

Contributions that improve the wording of the statements are welcome — open an issue
describing the change and the reasoning behind it. Please do not add build tooling or
dependencies; the single-file design is deliberate, so the tool keeps working
unattended for years.

## Deployment

Deployed via GitHub Pages from the default branch. Any static host will serve it, as
will opening the file directly from disk.

## Framework and citation

The framework this tool implements is published open-access:

> Rahaman, M. H. (2025). AI-GCLM: A Conceptual Framework for Artificial
> Intelligence–Enhanced Leadership in Global Construction Management.
> *International Journal of Engineering Technology Research & Management*, 9(5), 609–615.
> https://doi.org/10.5281/zenodo.21373248

The six pillars assessed here — Strategic Visioning, Data-Driven Decision Making,
Digital Workforce Leadership, AI-Augmented Risk Governance, Sustainable & Ethical
Delivery, and Adaptive Stakeholder Systems — are taken from that paper. Related work,
including the four-layer data-to-decision model and the human-in-the-loop
accountability cycle, is collected in
[construction-research](https://github.com/mrahamangm-droid/construction-research).

## License

Code released under the [MIT License](LICENSE) — permissive, so the tool can be adapted
freely inside an organisation. The underlying research is separately licensed CC BY 4.0
in the [construction-research](https://github.com/mrahamangm-droid/construction-research)
repository.

## Author

**Mohammad Habibur Rahaman**
Civil engineer and construction executive · Ras Al Khaimah, UAE

ORCID: [0009-0000-2294-8968](https://orcid.org/0009-0000-2294-8968) ·
[mrahaman.com](https://mrahaman.com/)
