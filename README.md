# IVZN Screening Room

> Every InavizionMedia build, one room — screen the latest previews, hop into the repos, check the branches.

**Branch policy:** work happens on the latest *-vN / project branch. List branches before editing. Never assume the GitHub default is the working line. Working line: IVZN-Screening-Room-v2 (GitHub default is main).

[![Pages](https://img.shields.io/badge/Pages-live-brightgreen)](https://inavizionmedia.github.io/IVZN-Screening-Room/)
[![Preview](https://img.shields.io/badge/Preview-live-red)](https://inavizionmedia.github.io/IVZN-Screening-Room/)
[![Static site](https://img.shields.io/badge/site-static-blue)]()
![Last commit](https://img.shields.io/github/last-commit/InavizionMedia/IVZN-Screening-Room)
![Repo size](https://img.shields.io/github/repo-size/InavizionMedia/IVZN-Screening-Room)

## Live preview

**https://inavizionmedia.github.io/IVZN-Screening-Room/**

![IVZN Screening Room](assets/screenshot.png?v=20261007g)

## What's inside

One card per InavizionMedia project — live screenshot, one-line description, last-push date, branch pills, and three links: **Preview** (the live site), **Repo**, **Branches**. Branch data loads live from the GitHub API so it never goes stale. Adding a project = one entry in the `PROJECTS` array.

Current rooms: InavizionMedia, The Starting Blocks, My Studio Channel, Yolando Mitchell Brown, Every Way Woman — plus Talkshow Land (in production, preview coming soon).

## Design language

InavizionMedia light brand: ivory paper, true red (`#d52620`), Barlow Condensed display + Source Sans 3 body. Light-first, 390px-mobile-friendly grid.

## Tech stack

| Layer | Choice |
|---|---|
| Page | Single static `index.html` |
| Fonts | Google Fonts (Barlow Condensed, Source Sans 3) |
| Data | Inline `PROJECTS` array + live GitHub REST API (no key, public repos) |
| Hosting | GitHub Pages from `main` |

## Project structure

```
IVZN-Screening-Room/
├── index.html          # the whole room
├── assets/
│   └── screenshot.png  # hero / social preview
├── .nojekyll
└── README.md
```

## Adding a project

1. Add one object to `PROJECTS` in `index.html` (repo, name, desc, preview URL, screenshot URL).
2. Push to `main` — Pages redeploys automatically.
3. Refresh `assets/screenshot.png` so the hero stays current.

## License

MIT — InavizionMedia.
