# Academic Homepage — Project Instructions

This is an [AcademicPages](https://academicpages.github.io/) (Jekyll) site published via GitHub Pages at https://okongoyango.github.io/ . Content lives in collection folders (`_talks/`, `_publications/`, `_portfolio/`, …) and the header menu order is controlled by `_data/navigation.yml`.

## Talk Entry Template (canonical)

When adding or updating an entry in the **Talks** section (`_talks/`), always follow this template. One file per talk, named `YYYY-MM-<venue>-<slug>.md`.

```markdown
---
title: "<Full talk title>"
collection: talks
type: "Talk"
permalink: /talks/YYYY-MM-<venue>-<slug>
venue: "<Conference / event name>"
date: YYYY-MM-DD
location: "<City, State/Country>"
link: "<URL to the official abstract / program page>"
excerpt: "Contributed oral talk in the session '<Session name>'."
---
Contributed oral talk, session *<Session name>*.

**Abstract:** <Full abstract text, single paragraph.>

Authors: <Name> (<Affiliation>), <Name> (<Affiliation>), ...

Related publication: <Author(s)> (<Year>). *<Title>.* [<ref label>](<URL>).
```

### Rules
- `type` is `"Talk"`; `link` points to the official abstract/program page so the title becomes clickable and a **"Direct Link"** button renders on the talk detail page.
- `excerpt` is a one-line summary used in list views; mirror the session name there.
- Body order: session line → `**Abstract:**` paragraph → `Authors:` line (one affiliation per author in parentheses) → optional `Related publication:` line with a link (arXiv/DOI).
- Omit the `Related publication:` line only when there is no associated paper.
- Keep formatting consistent with existing entries: `_talks/2025-03-aps-emca.md` and `_talks/2026-03-aps-nonreciprocal-thermal.md` are the reference examples.

## Navigation
- Header menu order is defined solely by `_data/navigation.yml` and is shared across all pages — there is no per-page override.

## Workflow
- After editing site content, commit and push to `origin/master` (GitHub Pages rebuilds in ~1–2 min). End commit messages with the `Co-Authored-By: Claude` trailer.
