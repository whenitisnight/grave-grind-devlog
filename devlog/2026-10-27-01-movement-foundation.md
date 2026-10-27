# Connecting a street skating line

**27 October 2026 · My verified movement checkpoint**

## My goal

I wanted a street line that preserved momentum and trick continuity through a grounded ollie, rail catch, kickflip, planter manual, street manual and second grind. I chose a connected route because isolated trick checks would miss interruptions between these actions.

I found an early catch pulling my skater too far toward a rail end, neighboring rails stealing the intended catch, and planter contact causing false landings or sticky motion. I also found the camera collapsing toward my skater while leaving a shelter.

## My architectural decisions

### Separate forward acquisition from side assistance

I limited forward rail-end acquisition independently from the generous lateral catch range. I gave an aligned, imminently reachable rail preference without attaching early. I chose this separation to preserve forgiving grind inputs while reducing forward snapping and unintended catches.

### Make landing agree with wheel support

I gave landing and riding the same conservative wheel-support footprint. I separated broad body clearance from legitimate top support and resolved the full lateral penetration when brushing an edge. I made these changes to prevent false ground/air transitions and repeated contact corrections from interrupting the line.

### Check the camera path, not just its destination

I allowed lower pitch candidates so my camera could remain beneath the shelter roof during departure. I added a continuity cost to discourage switching through the roof slab and checked clearance at the next interpolated orbit step before moving around a post. When straight chase remained clear, I returned toward it.

I chose those mechanisms because a clear destination beyond an obstacle did not guarantee a clear path to it. I retained the earlier body follow-through, manual counterbalance, rail settling and landing compression.

## My evidence

I verified the 2.3-second street line with keyboard/regular and controller/switch Unreal input replays, preserving an unbroken five-trick combo. I recorded **858 passing movement checks and zero failures**.

I measured first catch-frame travel in the clean approach falling from 230.494 cm to 105.946 cm. In the controller shelter case, I measured minimum camera distance increasing from 156.28 cm to 575.33 cm after the clearance fix. I use these measurements to assess the selected route, not as overall quality scores.

![My skater and board remain visible beneath the shelter](../media/shelter-clearance.png)

*My selected controller-replay frame beneath the shelter.*

![My skater reaches the intended second street rail](../media/street-line.png)

*My connected line reaches the intended second rail with the combo intact.*

## My current limits and next step

I resolved the specific route defects and saved a private source-and-asset rollback checkpoint. I used automated Unreal input events and rendered-frame review, with audio disabled; I have not established hands-on equivalence to THPS.

I still need to refine the full skating-survival experience, crowded combat readability and visual presentation. I use this entry as my public journal’s starting baseline, rather than attributing every earlier development session to this date.
