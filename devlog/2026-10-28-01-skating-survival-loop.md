# Making skating drive the survival run

I kept the skating foundation and made its routes matter to combat, progression and encounters. The central problem was a disconnect: a satisfying trick line could exist beside a survival system without changing what the player needed to do next.

## A connected route

Completed lines now contribute to skate spots, which award experience and useful gear. A stable objective marker connects the current session, nearby affordable equipment, the boss and the exit. Approaching a chest or gate can queue a deliberate interaction without requiring an abrupt stop or discarding an active combo. Upgrade selection respects those transitions.

Banking a varied line near enemies activates a bounded combat boost and pulls nearby rewards toward the rider. Six weapon families have evolutions linked to skating accomplishments. Movement-triggered equipment adds different reasons to ollie, grind, manual or bank a line, while ordinary attacks continue automatically. Pickups that have engaged the rider can keep up through fast movement and jumps.

The boss commits to readable charges and slams. Its recovery window creates a reason to complete a nearby line, then convert that opening into damage. Defeating it awards gear and opens a deliberate choice to extract or continue with the earned build and remaining health.

## Pressure that reaches a fast skater

An ordinary route exposed a pacing mismatch: a district could end before its first timed elite. Completed skate spots now advance the existing encounter sequence as well as increasing the nearby horde target. A recovery interval separates encounter beats, and time remains a fallback for players who explore without claiming spots. Safe spawn distances and committed attack warnings remain part of the system.

City geometry exposed a second mismatch. Some relics still measured distance on a flat plane, allowing effects on a rooftop to hit an unrelated street below. Fire trails and manual pulses now follow their supporting surface; grind bolts and banked lightning require reachable targets; crow projectiles stop on walls or terrain. Damage and presentation need to describe the same event.

## Evidence and limits

| Checkpoint | Observed result |
| --- | --- |
| Earlier standalone 0.81 | An automated ordinary-starter route cleared two districts in 98 seconds through earned rewards and real boss damage. |
| Current focused integration | 259 checks passed across the connected systems, including city relic interactions and session-driven encounters. |
| New encounter pressure | The first rendered route met an elite by 15 seconds, reached three weapon evolutions and lost near the first boss at 70 seconds. |
| Current standalone 0.82 | An ordinary bolt-priority route cleared both districts in 95 seconds with 797 defeats, three earned evolutions and 62 remaining health. |
| Crowd sample | The run reached 194 active enemies, with a peak of 47 relevant enemies ahead of the rider. |

The 0.82 win includes the newer pressure rules; the earlier win and losses remain separate evidence. These routes use scripted actions and reward choices; they do not inject gear, health, teleports or boss death, and they are not hands-on play. One successful policy does not establish that every build or pacing choice works well.

A 720p development-build sample on a Ryzen 5 1600 and GTX 1060 had a 16.7 ms median frame time and 19.6 ms 95th percentile after explicitly excluding startup and the terminal diagnostic screenshot. A 56 ms gameplay hitch remains in that interval. This is useful ordinary-run evidence, not ten-minute overtime or release-performance acceptance.

## Lessons and next decisions

Feature presence was a weak measure of integration. The elapsed run revealed encounters the player could skip unintentionally; the city exposed attacks whose visible path disagreed with their damage. Future iterations start with those observed interruptions, then use narrow checks before another connected route.

The profiler also captured the final screenshot despite receiving a stop command first: stopping completed at the frame boundary. Performance captures now omit screenshots entirely. The original contaminated sample remains part of the private evidence instead of disappearing from the record.

I am keeping the losses visible while assessing build viability and crowded readability. The current standalone demonstrates the connected run, but broader level variety, prolonged horde performance and complete desktop acceptance remain open. [Earned progression and save recovery](2026-10-28-02-earned-progression.md) cover the persistent side of this milestone.
