# Connecting skating, survival pressure and the campaign

The hybrid needed more than automatic attacks attached to a skateboard. I focused this milestone on making the skating line affect combat, keeping encounters useful beyond the opening, and carrying a legitimately earned build through a complete campaign.

## Skating changes the attack

Orbital Trucks now sweep through enemies along the rider's actual path. Attack-speed changes preserve the orbit angle, and a manual can prepare a burst released by banking the line. Afterburner follows the ridden street, roof or rail as connected tracks; overlapping a previous track extends coverage without multiplying its damage.

Moving grinds charge Rail Reaper attacks for a short carry window after leaving the rail. Ollies and manuals can continue that attack window, including cuts from elevated lines toward reachable enemies. Meaningful moving landings can release Landing Quake during an ongoing combo. These interactions give different builds a reason to use different skating routes.

## A run develops into a campaign

Recurring elite hunts and swarms replace the exhausted opening event list. District gates lead through three warned showdown phases before a boss. Real kills and moving combo banks advance that encounter, while exploration remains available between commitments. The Circuit Marshal adds fixed electric crossbars and charge recovery; the Night Mayor provides a phased campaign finale.

Departure also settles earned rewards. An ordinary result exposed finishing-hit credits that did not match awarded kills when the final bank killed enemies during extraction. Settlement now accounts for those deaths and eligible loose rewards before recording the result. Paid or still-locked caches remain excluded.

A recorded development run completed Hollow, Neon and Borough in 308.22 game seconds with four earned weapons, two evolutions and 4,896 kills. Attributed finishes, awarded kills and the saved total matched. A fresh process restored the earned result and an alternative starter without duplicating rewards. This was automated steering and upgrade selection with ordinary damage and rewards, not hands-on play. It predates the fourth district and does not prove the newer tour complete.

## Crowds have to remain usable

I retained the shared city geometry while changing how expensive work is scheduled: indexed geometry queries, local enemy-neighbour queries, cached distant routing and retained render-instance buffers support the larger horde. Visible-body generation and a foreground cutaway keep nearby enemies from completely covering the board and escape line.

In standalone 0.97, one 25-second staged sample reached 639 enemies at 1280×720, D3D11 and a 60 fps cap on a Ryzen 5 1600 / GTX 1060 6 GB. Mean frame time was 16.835 ms, with a 17.974 ms 95th percentile. The scene used injected late-run population and protection. It demonstrates bounded rendering performance, not ordinary difficulty, sustained locked 60 fps or current-version release acceptance.

## Problems and changes to the process

Feature checks did not expose every complete-run problem. Ordinary traces revealed inaccessible approaches, close camera pockets and the final-bank accounting mismatch. The useful evidence was the actual route, rendered frame and saved result, not the number of passing assertions. A separate full movement pass still recorded one canopy boom-distance failure; bounded framing review is not a substitute for resolving that requirement.

Future verification starts from the largest observed interruption, preserves the failed trace, and checks the correction locally before repeating a whole campaign. Profiling scenes and ordinary survival attempts stay explicitly separate. Damage changes made solely to rescue an automated policy would hide the underlying problem.

The desktop game remains an alpha. Broader build viability, consistent movement/camera quality and finished presentation remain open. [The kitchen and four-district tour](2026-10-29-02-kitchen-and-tour.md) record the next delivery and its newer acceptance boundary.
