# Changelog

Significant changes, resolved problems, architectural pivots and completed features appear here, newest first. Related commits share one explanatory entry; routine edits remain in Git history.

I adapt [Keep a Changelog](https://keepachangelog.com/en/1.1.0/) to dated development entries. These checkpoints are not released game versions.

## 2026-10-28 — Districts and combat clarity

- Expanded Hollow and replaced the third practice arena with Neon's roof approaches, street routes and elevated transit crossing.
- Added the Bell Warden's timed waves and skating recovery counterplay.
- Grouped approaching threats, recorded actual damage sources and kept the animated rider visible through foreground enemies.
- Documented navigation, rendering, verification and packaging failures alongside the corrected results.
- Cooked Windows 0.85 and recorded an ordinary Neon victory with an earned orbit-focused build; 362 focused integration checks pass.

[District decisions, evidence and lessons](devlog/2026-10-28-03-districts-and-combat-clarity.md).

## 2026-10-28 — Connected survival and earned progression

- Banked lines, skate sessions, equipment, committed boss encounters and extraction now form a connected run.
- Completed spots advance enemy encounters; skating relics respect city height and walls.
- Earned starting weapons, controller flows and persistent desktop settings connect sessions.
- Separate pending-save state recovers an actual completed run after a controlled disk failure without duplicating rewards.
- Recorded earlier standalone wins, new-pressure losses, an ordinary-run performance sample and verification lessons.

[Skating-survival milestone](devlog/2026-10-28-01-skating-survival-loop.md) · [Earned progression and recovery](devlog/2026-10-28-02-earned-progression.md).

## 2026-10-27 — Skating acceptance and lessons

- Five selected city routes pass, covering switch street combos, analog camera return, repeated ramps, walls and rooftops.
- Corrected the wall replay's input timing, the analog report mapping and access to the existing rooftop replay. Production movement rules remain unchanged.
- Significant case studies now document encountered problems, evidence-based lessons and a better next approach.

[Acceptance results and retrospective](devlog/2026-10-27-05-skating-acceptance.md).

## 2026-10-27 — Flip-catch continuity

- Foot return now follows the final board rotation, removing the trailing released pose after a completed flip.
- Kickflips and heelflips use opposite leading-foot flicks; double flips retain clearance through intermediate turns.
- The editor build, 864 movement checks and a brief rendered controller line pass. Skating remains the active phase before survival integration.

[Flip-catch decision and evidence](devlog/2026-10-27-04-flip-catch.md).

## 2026-10-27 — Current-status record

Documented implemented systems, the verified movement checkpoint, build availability and remaining integration work. This records existing evidence and future priorities without claiming a new gameplay milestone.

[Current project status](devlog/2026-10-27-03-current-status.md).

## 2026-10-27 — Public project library

### Added

- Separate public portfolio with a product brief, system map, focused case studies and selected gameplay captures.
- Traceability between documented private changes and public entries, while keeping source, assets and implementation history private.

### Changed

- Significant progress is documented as work is completed, explaining the goal, technical mechanism, reasoning and evidence.
- A concise changelog and development-library index link individual topic documents.
- Editorial guidance distinguishes first-person decisions from technical explanations led by the system, behavior or evidence.

[Project-library decision](devlog/2026-10-27-02-public-progress-workflow.md).

## 2026-10-27 — Movement foundation checkpoint

### Fixed

- Forward rail-end acquisition separated from lateral assistance to reduce excessive snapping and unintended catches.
- Wheel support and landing checks aligned to remove false landings and sticky movement at planter edges.
- Camera continuity and intermediate clearance checked to resolve shelter close-ups in the connected street line.

### Added

- Private source-and-asset checkpoint with a rollback tag.
- Keyboard and controller street-line replays, plus 858 passing movement checks.

[Street-line case study](devlog/2026-10-27-01-movement-foundation.md).
