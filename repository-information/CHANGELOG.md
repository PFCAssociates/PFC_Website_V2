# Changelog

All notable changes to this project are documented here.
Format follows [Keep a Changelog](https://keepachangelog.com/en/1.1.0/).

Version suffixes: `w` = website (HTML pages), `g` = Google Apps Script.

## [Unreleased] — 2026-02-19 13:21:25 EST

- `2026-02-19 13:21:25 EST` — Fixed auto-merge workflow merge conflict handling: added `-X theirs` strategy to prefer incoming branch changes when content conflicts occur (e.g. CHANGELOG.md). This prevents exit code 1 failures when main and the claude branch modify the same file
- `2026-02-19 13:09:12 EST` — Added placeholder images throughout the site: hero background image, PFC logo in nav and footer, clinic building and medical team photos in About section, first-responders image banner between Services and Staff. Created images/ directory with 5 labeled SVG placeholders ready for real photo replacement. Adjusted styling for image overlays, z-indexing, and institutional feel. Build-version bumped to 01.02w
- `2026-02-19 12:25:44 EST` — Redesigned front page with modern layout: fixed nav, full-viewport hero with stats, About/Mission section, 9-card services grid, staff directory with admin team and agency reps, FAQ accordion, resources/documents/policies section, memorial tribute, and 3-column footer. All original content preserved. Build-version bumped to 01.01w

Developed by: PFCAssociates

