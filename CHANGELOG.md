# Changelog

I record significant changes, resolved problems, architectural pivots and completed features here, newest first. I group related commits under one explanatory entry and keep routine edits in Git history.

I adapt [Keep a Changelog](https://keepachangelog.com/en/1.1.0/) to dated development entries. I do not present these checkpoints as released game versions.

## 2026-10-27 — Current-status record

I documented my implemented systems, verified movement checkpoint, current build availability and remaining integration work. I separated existing evidence from future priorities without claiming a new gameplay milestone.

[My current project status](devlog/2026-10-27-03-current-status.md).

## 2026-10-27 — Public project library

### Added

- I established a separate public portfolio with a product brief, system map, focused case studies and selected gameplay captures.
- I linked documented private changes to their public entries while keeping game source, assets and implementation history private.

### Changed

- I publish significant progress as I complete it, using my first-person voice to explain the goal, technical mechanism, reasoning and evidence.
- I keep the changelog short and link individual topic documents through a development-library index.

[My project-library decision](devlog/2026-10-27-02-public-progress-workflow.md).

## 2026-10-27 — Movement foundation checkpoint

### Fixed

- I separated forward rail-end acquisition from lateral assistance to reduce excessive snapping and unintended catches.
- I aligned wheel support and landing checks to remove false landings and sticky movement at planter edges.
- I checked camera continuity and intermediate clearance to resolve shelter close-ups in the connected street line.

### Added

- I saved a private source-and-asset checkpoint with a rollback tag.
- I verified the street line with keyboard and controller replays and recorded 858 passing movement checks.

[My street-line case study](devlog/2026-10-27-01-movement-foundation.md).
