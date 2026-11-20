# Making skating and automatic weapons cooperate

Published November 19, 2026. Implementation and verification recorded November 6, 2026; Windows development checkpoint 0.127.

I want a strong weapon build to make a skating line more useful. Earlier combat could undermine that goal in two ways: incidental automatic damage broke a planned enemy formation before contact, and weapon-specific power kept growing after baseline skating damage reached its cap. This milestone connects formation behavior, board damage and ranged targeting while preserving the skating controls.

## Holding a useful approach

Enemies assigned to a rail, street, roof or landing approach now retain their original formation deadline after incidental damage when the rider is still moving toward the intended line. Contact, turning away, stopping, expiry or a committed warning still releases pursuit. The change grants no healing, immunity or additional population.

Source review then exposed a second interaction: holding a formation also skipped specialist attack updates. Specialist cooldowns and warning logic now continue while locomotion is held, and committing an attack releases the formation permanently. Existing range, cover, emergence grace and warning limits remain authoritative.

## Carrying build power into skating

Board attacks inherit the highest damage-power multiplier among owned weapons. They use one multiplier rather than summing or multiplying the inventory. Unowned values cannot contribute, and global damage modifiers still apply once. Damage attribution stays with the skating action; it does not create weapon-evolution credit. Upgrade cards preview the actual board-power change and explicitly show when another weapon already supplies a higher value.

During a grounded, moving, charged approach, three ranged weapon families prefer other reachable targets over an ordinary walker immediately inside the board corridor. The preference is finite: close targets remain eligible when alternatives run out. Bosses, elites, specialists, ordinary uncharged cruising and airborne skating retain their existing rules. Movement, collision, fire rate and enemy health are unchanged.

## Keeping the next action visible

Purchases, queued confirmations, nearby spot progress and gate interactions share a dock beside the riding corridor. The optional route card yields its space while an immediate action is present. Desktop click bounds follow the rendered rectangle; keyboard, controller and touch controls retain their existing bindings.

## Verification and its limits

The November 6 record reports a successful Windows 0.127 Shipping build and 1,797 passing packaged mechanics checks. A fresh-process reload of the earned profile passed seven checks after the verification helper was corrected to copy the separate starter-preference file as well as progression. The initial omission and failed check remain documented. Archive integrity, payload hashes, guide contents and exclusion of private runtime data were checked for that local delivery.

A prepared late-build powerslide comparison demonstrated stronger crowd removal at the same initial motion when weapon power was applied. It injected the build and enemies and disabled automatic weapon stepping, so it is mechanism evidence rather than earned play. A separate 60-second ordinary automated opening exercised earned rewards, actual damage and the combined systems. It produced no damaging powerslide sweep hits, leaving practical sweep usefulness unresolved. Neither sample establishes a causal improvement in enjoyment.

The performance analyzer was also corrected to separate stage age and living enemies from cumulative campaign time and occupied pool slots. This prevents a new district or pending defeated bodies from qualifying as sustained late-stage load. The acceptance threshold was preserved; sustained heavy-load performance remains unproven.

No new gameplay test or build was performed for this publication. The 0.126 campaign and 0.127 mechanics checks remain evidence for their respective versions. Physical-input acceptance, clean-machine compatibility, sustained crowded performance and human enjoyment remain open. This is a development checkpoint; no public playable release is claimed.

## Lessons and next priorities

The failures came from interactions between otherwise working systems: locomotion ownership suppressed attacks, weapon growth bypassed skating growth, and the verification setup omitted a separately stored preference. The next pass should assess the combined player experience and useful skating decisions, with targeted checks for those boundaries. Repeating a completed campaign or adding isolated damage totals would not resolve the outstanding enjoyment question.

See the [previous combat-flow milestone](2026-11-06-01-combat-flow-and-readable-payoffs.md), [product brief](../docs/product.md) and [system map](../docs/system-map.md).
