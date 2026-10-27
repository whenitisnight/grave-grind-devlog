# Grave / Grind

**An arcade skating × survival-action prototype in Unreal Engine 5.8.**

Build momentum, connect tricks and use a skateable city while navigating enemy pressure. The project takes movement inspiration from Tony Hawk's Pro Skater and survival-run inspiration from Megabonk.

![The current prototype riding a street rail](media/street-line.png)

*Actual development-build capture from the verified controller street line, 27 October 2026.*

## Follow development

This is the project's living portfolio and development journal. Every completed private change set gets a public explanation here, including smaller fixes, tooling and documentation work. The implementation and Unreal assets remain in a separate private repository.

- [Changelog](CHANGELOG.md) — chronological index of changes.
- [Movement foundation](devlog/2026-10-27-01-movement-foundation.md) — rail selection, edge contact and shelter camera fixes.
- [Continuous public logging](devlog/2026-10-27-02-public-progress-workflow.md) — how private development becomes public evidence.
- [Product brief](docs/product.md) — intended player experience and current scope.
- [System map](docs/system-map.md) — how movement, presentation and survival systems relate.
- [Update process](docs/progress-workflow.md) — what each entry records.

## Current checkpoint

| Area | Observed status |
| --- | --- |
| Skating | Grounded ollie → grind → kickflip → two manual landings → second grind in one continuous five-trick combo |
| Inputs | Keyboard/regular and controller/switch automated routes pass |
| Verification | 858 movement checks pass; selected rendered controller frames reviewed |
| Full game | Prototype under development; survival integration, combat readability and visual polish remain active work |

These checks demonstrate specific behavior in the tested routes. They do not establish identical THPS feel, finished-game quality or crowded-survival performance. No new gameplay checks were run merely to publish this journal.

## Development approach

Maintained by [whenitisnight](https://github.com/whenitisnight), with AI-assisted implementation and documented verification. Entries explain what changed, what evidence supports it and what still needs work. Desktop comes first; mobile adaptation, music and detailed balance work are deferred.

This repository contains portfolio documentation and selected media. A public playable build is not included at this stage.
