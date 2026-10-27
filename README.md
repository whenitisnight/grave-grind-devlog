# Grave / Grind

**An arcade skating × survival-action prototype in Unreal Engine 5.8.**

I’m combining the momentum and trick chaining of Tony Hawk’s Pro Skater with the enemy pressure and run progression of Megabonk. The goal is a city where skating provides both satisfying movement and routes through survival encounters.

![A street-rail grind in the prototype](media/street-line.png)

*Controller-replay capture from the development build, 27 October 2026.*

## Development library

This portfolio records significant decisions, resolved problems and completed features. Implementation and Unreal assets remain in a private workshop; the public library contains focused case studies and selected evidence.

- [Current status — 27 October 2026](devlog/2026-10-27-03-current-status.md) — implemented systems, verified checkpoint and next priorities.
- [Development library](devlog/README.md) — dated decisions and problem-solving entries.
- [Changelog](CHANGELOG.md) — short chronological index.
- [Product brief](docs/product.md) — player experience and scope.
- [System map](docs/system-map.md) — connections between movement, presentation and survival.
- [Documentation process](docs/progress-workflow.md) — editorial and publishing workflow.

## Current checkpoint

| Area | Recorded evidence |
| --- | --- |
| Skating | A connected ollie, grind, kickflip, two manual landings and second grind preserve a five-trick combo. |
| Inputs | Keyboard/regular and controller/switch automated replays pass the selected street line. |
| Verification | 858 movement checks pass, with controller captures reviewed for visibility. |
| Full game | Survival integration, combat readability and visual presentation remain in development. |

These checks support specific routes and mechanics. Exact THPS feel, finished-game quality and crowded-survival performance remain unverified.

## Development approach

I maintain this project as [whenitisnight](https://github.com/whenitisnight), using AI-assisted implementation with documented verification. Desktop comes first; mobile adaptation, music and detailed balance work are deferred.

This repository contains documentation and selected media. A public playable build has not been released.
