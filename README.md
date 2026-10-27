# Grave / Grind

**My arcade skating × survival-action prototype in Unreal Engine 5.8.**

I’m combining the momentum and trick chaining of Tony Hawk’s Pro Skater with the enemy pressure and run progression of Megabonk. I want a city where skating provides both satisfying movement and routes through survival encounters.

![My prototype riding a street rail](media/street-line.png)

*My controller-replay capture from the development build, 27 October 2026.*

## My development library

I document significant decisions, resolved problems and completed features as development progresses. I keep implementation and Unreal assets in my private workshop and publish focused case studies with evidence here.

- [Development library](devlog/README.md) — my dated decisions and problem-solving entries.
- [Current status — 27 October 2026](devlog/2026-10-27-03-current-status.md) — my implemented foundation, verified checkpoint and next priorities.
- [Changelog](CHANGELOG.md) — my short chronological index.
- [Product brief](docs/product.md) — my player experience and scope.
- [System map](docs/system-map.md) — how I connect movement, presentation and survival.
- [Documentation process](docs/progress-workflow.md) — how I organize my records.

## My current checkpoint

| Area | What I have verified |
| --- | --- |
| Skating | I connect an ollie, grind, kickflip, two manual landings and second grind into one five-trick combo. |
| Inputs | I verify the street line with keyboard/regular and controller/switch automated replays. |
| Evidence | I have 858 passing movement checks and reviewed controller captures. |
| Full game | I’m still refining survival integration, combat readability and visual presentation. |

I treat these checks as evidence for specific routes and mechanics. I have not established identical THPS feel, finished-game quality or crowded-survival performance.

## My development approach

I maintain this project as [whenitisnight](https://github.com/whenitisnight), using AI-assisted implementation with documented verification. I build for desktop first; I have deferred mobile adaptation, music and detailed balance work.

I currently publish documentation and selected media here. I have not released a public playable build.
