# Connecting a street skating line

**27 October 2026 · Verified movement checkpoint**

## Goal

A connected skating line needs to preserve momentum and trick continuity through an ollie, rail catch, kickflip, planter manual, street manual and second grind. I chose this route because isolated trick checks would miss interruptions between actions.

The route exposed early catches pulling the skater too far toward a rail end, neighboring rails stealing the intended catch, and planter contact causing false landings or sticky motion. Leaving a shelter also caused the camera to collapse toward the skater.

## Architectural decisions

### Separate forward acquisition from side assistance

I limited forward rail-end acquisition independently from the generous lateral catch range. An aligned, imminently reachable rail now reserves preference without attaching early. This preserves forgiving grind inputs while reducing forward snapping and unintended catches.

### Make landing agree with wheel support

Landing and riding now use the same conservative wheel-support footprint. Broad body clearance is separate from legitimate top support, and edge brushes resolve the full lateral penetration. These changes prevent false ground/air transitions and repeated contact corrections from interrupting the line.

### Check the camera path, not just its destination

A clear destination beyond an obstacle does not guarantee a clear path to it. I added lower pitch candidates so the camera could remain beneath the shelter roof during departure, with a continuity cost to discourage switching through the slab.

The next interpolated orbit step also checks clearance before moving around a post. When straight chase remains clear, the camera returns toward it. Earlier body follow-through, manual counterbalance, rail settling and landing compression remain intact.

## Evidence

The 2.3-second street line passed keyboard/regular and controller/switch Unreal input replays, preserving an unbroken five-trick combo. The movement checks recorded **858 passes and zero failures**.

First catch-frame travel in the clean approach fell from 230.494 cm to 105.946 cm. In the controller shelter case, minimum camera distance increased from 156.28 cm to 575.33 cm after the clearance fix. These measurements describe the selected route; they are not overall quality scores.

![The skater and board remain visible beneath the shelter](../media/shelter-clearance.png)

*Selected controller-replay frame beneath the shelter.*

![The skater reaches the intended second street rail](../media/street-line.png)

*The connected line reaches the intended second rail with the combo intact.*

## Limits and next step

The specific route defects are resolved, with a private source-and-asset rollback checkpoint retained. Verification used automated Unreal input events and rendered-frame review, with audio disabled. Hands-on equivalence to THPS remains unverified.

I’m using this checkpoint as the public journal’s starting baseline, without attributing every earlier development session to this date. The next phase is the combined skating-survival experience, crowded combat readability and visual presentation.
