# Grave / Grind

**An arcade skating × survival-action prototype in Unreal Engine 5.8.**

I’m combining the momentum and trick chaining of Tony Hawk’s Pro Skater with the enemy pressure and run progression of Megabonk. The goal is a city where skating provides both satisfying movement and routes through survival encounters.

![A street-rail grind in the prototype](media/street-line.png)

*Controller-replay capture from the development build, 27 October 2026.*

## Development library

This portfolio records significant decisions, resolved problems and completed features. Implementation and Unreal assets remain in a private workshop; the public library contains focused case studies and selected evidence.

- [Current status — 27 October 2026](devlog/2026-10-27-03-current-status.md) — implemented systems, verified checkpoint and next priorities.
- [Latest skating improvement](devlog/2026-10-27-04-flip-catch.md) — synchronized foot catches and distinct flip motions.
- [Skating acceptance and lessons](devlog/2026-10-27-05-skating-acceptance.md) — five connected routes, a misleading replay and a more focused verification process.
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
| Animation | Feet return with the completed flip; kickflips and heelflips use opposite flick directions. |
| Verification | Earlier 864-check result plus five fresh connected-route passes; the wall replay now requests its flip after rail departure. |
| Current phase | Skating transitions, rider/board presentation and camera continuity come before further survival integration. |

These checks support specific routes and mechanics. Exact THPS feel, finished-game quality and crowded-survival performance remain unverified.

Significant case studies include problems encountered, lessons supported by evidence and concrete improvements to the next approach.

## Development approach

I maintain this project as [whenitisnight](https://github.com/whenitisnight), using AI-assisted implementation with documented verification. Desktop comes first; mobile adaptation, music and detailed balance work are deferred.

This repository contains documentation and selected media. A public playable build has not been released.
