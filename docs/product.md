# Product brief

I’m building Grave / Grind to combine arcade skating with survival action. Movement should remain satisfying on its own while providing routes, escapes and opportunities during enemy encounters.

## Intended experience

- Momentum and responsive trick inputs carry the skating experience.
- Rails, ledges, ramps and buildings connect into routes through the city.
- Survival pressure makes those route choices matter during a run.
- Camera and rider presentation keep the board, landing opportunities and nearby threats readable.

Tony Hawk’s Pro Skater is the skating reference; Megabonk is the survival reference. Exact equivalence to either game remains unverified.

## Current implementation

The prototype includes skating, tricks, surface interactions, camera and rider presentation, together with combat, enemies, pickups and run progression. Recent verification concentrated on movement. The intended quality of the combined experience still needs to be established.

The street-line work resolved specific rail-acquisition, edge-contact and shelter-camera defects. I’m prioritizing skating transitions, rider/board presentation and camera continuity before returning to survival integration. The current animation pass ties foot return to the board’s remaining flip rotation and gives kickflips and heelflips opposite flick directions.

Five selected connected routes now pass the [technical acceptance check](../devlog/2026-10-27-05-skating-acceptance.md). That result closes this bounded verification pass; subjective feel and the combined survival experience remain separate acceptance questions.

## Scope

Development uses Unreal Engine 5.8 for desktop. Mobile adaptation, music and detailed balancing are deferred. Additional level themes remain concepts until implemented and demonstrated.

My process uses AI-assisted development with documented verification. Automated checks, rendered review and hands-on play are distinguished in the project records.
