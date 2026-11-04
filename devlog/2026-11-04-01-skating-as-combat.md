# Making skating the combat loop

The skating foundation was working, but the combined game still felt awkward and unsatisfying. I chose to preserve that foundation and test a narrower rescue: momentum, tricks and banked lines should directly clear enemies, deliver rewards and shape the next upgrade. More content would not answer that central problem.

## Attacks that follow the line

Every starting loadout now has a skating attack. Forward riding above the momentum threshold hits ordinary enemies ahead of the board; moving tricks charge a wider breakthrough. Meaningful landings release a blast, earned rail departures launch a piercing cut, and banked combat lines create a nearby burst. Bosses and committed hazards retain their counterplay.

Skating finishers launch defeated bodies through nearby enemies. The visible body follows the same swept position used for collision, with world obstruction, height checks and bounded flight. Secondary defeats preserve the attack's rewards and attribution without recursively launching more bodies. Orbital, quake and Reaper attacks share this payoff. XP and gold from skating attacks pursue the rider.

Automatic choices wait for a break in the line and leave space after a chosen power. A pending-XP deadline prevents indefinite delay; deliberate interaction can request a queued choice immediately. Weapon drafts preserve access to the chosen weapon's next upgrade alongside alternatives and support. First style gear proposes a matching weapon on the next earned level, while evolution cards show actual skating requirements. XP costs and the four-weapon limit remain.

## Feedback that explains the result

The display gives the most urgent threat one reaction prompt, keeps charge bars with weapon icons, and counts actual skating finishes beside the combo score. Pause retains detailed weapon actions and evolution requirements. Shared notices prioritize damage and new messages without hiding the next evolution; guidance yields during immediate danger.

Seven original synthesized effects distinguish board hits, body crashes, blasts, travelling cuts, rush warnings, area warnings and rider damage. Actual damage and committed attacks trigger them. Three event lanes feed six reused audio components, grouping crowded impacts while separating warnings and hurt cues. Pause, mute, focus loss and resets stop the layer and discard stale events. The supplied Borough soundtrack loops under an independently saved music control.

## Problems and lessons

The first momentum candidate delayed upgrades indefinitely during continuous tricks. A short ordinary opening exposed zero choices despite sufficient XP. The pending-XP deadline addresses that failure. Progression needs verification while the player performs the very behavior the system encourages.

A camera path could cross a shelter post even when both endpoints were clear. Checking the predicted midpoint closed that obstruction; the selected route's minimum camera arm increased from about 66 cm to 685 cm. This was a specific defect, not a reason to retune accepted movement.

The first positive body-collision fixture crossed shelter geometry. Its blocked result was correct. Moving that case into a verified open corridor, while retaining the wall case, separated a bad fixture from a collision defect.

Reducing clutter risked losing essential instructions. Keeping the full reference in pause and reviewing notice priority preserved those details. Audio verification also needed actual cooked playback and recorded output; requested-sound counters alone were insufficient.

The larger lesson is that mechanical completion does not establish an enjoyable game. I am treating this as a focused rescue candidate. Its next acceptance question is whether attacking, collecting and choosing upgrades while skating forms a satisfying loop, not how many more systems can be added.

## Delivery and evidence

One 50-second automated opening earned orbitals and three upgrades, reaching level six. Orbitals accounted for 66 of 277 finishes and baseline skating for 68. That sample did not demonstrate an evolution, boss victory or full-run viability.

Local Windows 0.105.0 Shipping packages the combined momentum, body-collision, draft, display and audio work. The portable archive passes integrity and embedded-executable checks and excludes local profiles and captures. Earlier packages remain preserved. This journal does not distribute a playable build.

The rebuilt editor passes 943 mechanics checks. Audio-enabled editor and Shipping checks each pass 16 cases covering imported playback, event storms and lifecycle behavior. Recorded game-master output contains sound with no clipped samples; this establishes output and headroom for that sample, not listening quality. Four staged crowded/boss/pause views were reviewed during the display pass. The final standalone passes a 4.833-second prepared keyboard route through skating, banking, purchase, upgrade and gate activation.

These are automated and rendered checks, not hands-on enjoyment acceptance. Broader naturally earned builds, sustained current late-horde performance, clean-machine compatibility and finished presentation remain open. Exact THPS or Megabonk equivalence is not established.
