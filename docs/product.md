# Product brief

I’m building Grave / Grind to combine arcade skating with survival action. Movement should remain satisfying on its own while providing routes, escapes and opportunities during enemy encounters.

## Intended experience

- Momentum and responsive trick inputs carry the skating experience.
- Rails, ledges, ramps and buildings connect into routes through the city.
- Survival pressure makes those route choices matter during a run.
- Camera and rider presentation keep the board, landing opportunities and nearby threats readable.

Tony Hawk’s Pro Skater is the skating reference; Megabonk is the survival reference. Exact equivalence to either game remains unverified.

## Current implementation

The prototype includes skating, tricks, surface interactions, camera and rider presentation, together with six weapon families, skating-linked evolutions, movement-triggered equipment, horde encounters, bosses and run progression. Claimed sessions deliver experience and gear while advancing district pressure. A deliberate gate interaction connects boss defeat to extraction or another district with the earned build.

The street-line work resolved specific rail-acquisition, edge-contact and shelter-camera defects. The animation pass ties foot return to the board’s remaining flip rotation and gives kickflips and heelflips opposite flick directions. I am preserving that foundation while finishing the connected survival experience.

Five selected connected routes now pass the [technical acceptance check](../devlog/2026-10-27-05-skating-acceptance.md). That result closes this bounded verification pass; subjective feel and the combined survival experience remain separate acceptance questions.

The garage now offers starting weapons earned through completed runs. Desktop options, controller transitions and pending-save recovery support the session loop. [The hybrid milestone](../devlog/2026-10-28-01-skating-survival-loop.md) records a current standalone two-district win, save recovery and fresh-launch restoration, alongside earlier wins and losses; those outcomes remain version-specific.

## Scope

Borough, Hollow and Neon now provide distinct street and rooftop arrangements. Hollow's Bell Warden changes the encounter sequence, while Neon adds a route above and below an elevated crossing. Grouped threat cues, actual damage attribution and an occluded rider silhouette support combat readability. The [district record](../devlog/2026-10-28-03-districts-and-combat-clarity.md) separates implemented behavior, rendered review and remaining acceptance work.

Development uses Unreal Engine 5.8 for desktop. Mobile adaptation, music and detailed balancing are deferred. Additional level themes remain concepts until implemented and demonstrated.

My process uses AI-assisted development with documented verification. Automated checks, rendered review and hands-on play are distinguished in the project records.
