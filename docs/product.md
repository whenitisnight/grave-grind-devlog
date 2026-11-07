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

The [combat rescue](../devlog/2026-11-04-01-skating-as-combat.md) makes ordinary momentum, tricks and banked lines direct attacks. Defeated bodies can strike nearby foes, skating loot pursues the rider and weapon drafts preserve a chosen upgrade path. Clearer priorities and dedicated sound cues connect movement to its consequences. The combined game's enjoyment remains unaccepted despite mechanical progress.

## Scope

Borough, Hollow, Neon and After Hours provide distinct routes. The kitchen adds circular bowls, cutlery grinds, a mug and raised household surfaces. Its Head Chef joins the Groundskeeper, Bell Warden and Circuit Marshal; longer campaigns end with the Night Mayor. Players choose unvisited destinations while carrying their earned build through a one- to four-district run.

Moving grinds, landings, manuals and banked lines affect weapon behavior. Recurring encounters and three-wave gate showdowns develop survival pressure beyond the opening. Grouped threat cues, damage attribution, a rider silhouette and foreground crowd clearance support readability. The [campaign record](../devlog/2026-10-29-01-connected-campaign.md) and [kitchen/tour record](../devlog/2026-10-29-02-kitchen-and-tour.md) distinguish implementation from acceptance.

The desktop candidate includes optional First Ride lessons on actual city geometry, event-driven survival guidance, protected in-game exit paths, background pause and persistent display/comfort settings. Window changes require confirmation and otherwise revert. A local Windows 0.125.0 Shipping ZIP includes the guide, runtime and accumulated gameplay changes; a public playable release remains separate.

The [subsequent campaign record](../devlog/2026-11-04-02-skating-survival-routes.md) completes an earned four-district tour with three evolved skating weapons, final extraction and successful fresh-process restoration. Free Drop-In and Rail Runner starts, stored Reaper power and formed encounters support skating-led builds. The campaign predates grouped upgrades; it is not full acceptance of the latest standalone. Broader completed builds, heavier ordinary crowds, hands-on enjoyment and finished presentation remain open.

The [earlier build milestone](../devlog/2026-11-04-03-skating-builds-and-campaign.md) covers matching starter gear, preserved pair focus, three weapon pairings, linked landing attacks, route guidance, recovery packs and fixed formations during pressure phases. Windows 0.116 completes an ordinary scripted Orbit/Thunder four-district win and fresh-process save restoration. Enjoyment, sustained crowded performance, exploration quality and human input acceptance remain open.

The [earlier city-encounter milestone](../devlog/2026-11-05-01-connected-city-encounters.md) connects street and rooftop routes, fixed crowd rows, named roof rewards and painted characters. Windows 0.119 completes a scripted Sawline/Bolts tour and restores its earned result.

The [current combat-flow milestone](../devlog/2026-11-06-01-combat-flow-and-readable-payoffs.md) adds carried manual volleys, powerslide attacks, airborne board contact, sustained rushes, animated crowds, boss aftermath and bounded secondary feedback. Windows 0.124 supplies a later earned tour and save result; Windows 0.125 packages the contact/readability corrections with its own checks. Overall enjoyment and sustained heavy-load acceptance remain unresolved.

Development uses Unreal Engine 5.8 for desktop. The supplied Borough track loops with independently saved music volume. Mobile adaptation, broader soundtrack work and detailed balancing are deferred. Additional level themes remain concepts until implemented and demonstrated.

My process uses AI-assisted development with documented verification. Automated checks, rendered review and hands-on play are distinguished in the project records.
