# Dev Mistakes & Learning Log

A running, real-world log of bugs I've hit while building software, how I
fixed them, and what I'd do differently next time. Entries are logged
through [mistakes_upload](https://github.com/) — a small internal tool
that turns a quick write-up into a structured markdown file and commits
it straight here.

The goal is simple: mistakes are usually where the actual learning
happens, but they rarely get written down anywhere useful. This repo is
that place — for me to look back on, and for anyone else who runs into
the same error to (hopefully) save some time.

## How entries are organized

Every entry lives under `mistakes/{category}/{title-slug}.md`:

```
mistakes/
  nextjs/
  react/
  python/
  vector-db/
  typescript/
  api-backend/
  general/
```

Each file follows the same structure:

```
---
title: "..."
category: "..."
date: "YYYY-MM-DD"
---

## 📌 Problem Overview
What went wrong, and why it caused confusion.

## ✅ Solution & Prevention
How it was fixed, and what to watch for next time.

## 💻 Code Example
(included only when a relevant snippet was logged)
```

## Browsing

- Fastest way: open the `mistakes/` folder above and pick a category.
- GitHub's search bar (top of the repo) works well for finding a
  specific error message across all entries.

## A note on the content

These are personal notes, written quickly, in the moment. They're not
polished tutorials — expect informal language and the occasional
half-finished thought. If something here is wrong, outdated, or you
have a better fix, feel free to open an issue.
