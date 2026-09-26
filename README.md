# StudyOS · Academic OS

A polished, offline-first academic command center built as a dependency-free PWA.

## What changed

- Rebuilt the information architecture around **Overview, Focus room, Tasks, Subjects, Error log, Schedule, Analytics, and Settings**.
- Replaced fragile `prompt()` flows with accessible modal forms.
- Added a circular focus timer with session logging, subject selection, and live progress.
- Added task completion, mastery editing, error redo workflow, schedule blocks, search, export/import backup, reset workspace, and offline caching.
- Added responsive layouts for desktop, tablet, and mobile with bottom navigation on small screens.
- Added a more investment-ready visual system: clear hierarchy, restrained color, meaningful states, privacy-first copy, and coach-style insights.

## Run locally

Because it is a PWA, serve the folder over HTTP instead of opening the file directly:

```bash
python3 -m http.server 4173
```

Then open `http://localhost:4173`.

## Data model

All workspace data is stored locally in the browser under `studyos_v2`. Use **Settings → Export backup** before clearing browser data or moving devices.

## Files

- `index.html` — application UI, styles, and client-side logic
- `manifest.json` — installable PWA metadata
- `sw.js` — offline cache and update strategy
- `icon-192.png`, `icon-512.png` — app icons
