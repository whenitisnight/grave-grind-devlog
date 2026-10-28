# Keeping earned progress across runs and failures

I wanted completed runs to change the next session without replacing the skating foundation with permanent movement bonuses. The garage now offers starting weapon choices earned through banked score, enemy defeats and extraction. Requirements and equipped status are visible, and each choice occupies one ordinary starting weapon slot.

## From a result to the next run

The default projectile starter is joined by earned orbiting, lightning and disc playstyles. A finished defeat can contribute its legitimate score and kills; abandoning a run does not grant those rewards. Unlocks derive from saved totals, and an unavailable saved preference falls back to the default starter.

Keyboard and controller flows connect the garage, run tiers, upgrades, pause, trick book, defeat, victory and retry. Consuming menu confirmations until release prevents the same button from becoming an unintended skating action. Desktop settings expose graphics quality, frame limit, V-sync, effects volume, camera sensitivity and vertical inversion. Camera preferences affect look input while preserving the underlying skating rules.

## A recorded reward was not necessarily saved

A lifecycle review found that a completed run was marked as recorded even when its disk write failed. Returning to the garage could then skip the promised retry. The accounting guard correctly prevented duplicate rewards, but it also concealed unfinished persistence.

Pending writes now have their own state. Garage return, retry and equip actions can save the already-recorded profile without awarding the run again. The interface retains an unsaved-progress warning until the write succeeds. Atomic replacement, validated backups and protection for newer profile versions remain in place.

## Evidence

An ordinary automated run earned 69 credits, 286 kills and 40,638 banked points before losing near the boss. An isolated acceptance directory deliberately blocked the profile write. After removing that exact obstruction, normal garage calls saved the earned profile once and equipped the newly unlocked lightning starter.

A separate process restored the credits, earned unlock and equipped choice. Starting the next run produced the real lightning weapon at ordinary starter health and level, with no duplicate credit or kill reward. Four recovery checks and five fresh-process assertions passed. The broader focused integration pass remained at 259 passing checks.

Settings received separate evidence: 36 menu/input checks, a rendered 720p screen review and a fresh-process reload of the saved audio, camera and frame-limit preferences. These are automated checks, not claims about physical controller latency or audio listening.

The Windows 0.82 standalone then completed both districts, earned 116 credits and unlocked the disc starter. The same controlled write failure recovered through the garage, and a separate launch restored that actual result and equipped weapon. All four recovery checks and five reload assertions passed for this packaged run too.

## Problems and improved approach

The settings acceptance guard initially rejected its own destination because the engine supplied a symbolic configuration identifier rather than a file path. Resolving the real destination corrected the isolation check without weakening it. Another check caught Escape closing options and then unpausing on the following frame; consuming the held state fixed that transition.

Packaged acceptance also exposed an assertion that treated a harmless floating-point representation of 90% volume as failure. An explicit tolerance corrected the check. The final executable passes 36 menu/input checks and both fresh-launch settings assertions. A subsequent cook hit the asset cache's storage limit; because only that diagnostic comparison had changed, the rebuilt executable could use the already-successful package's unchanged cooked content. The original cook failure remains documented, and new content will require a successful new cook.

The main lesson is to verify persistence at lifecycle boundaries. Saving a profile in isolation does not prove that the result screen, garage and next launch reach that code correctly. I now keep reward accounting separate from write completion and exercise a real earned result through failure, recovery and reload.

The desktop remains a prototype. A persistent storage failure must be resolved before closing the game; this recovery path cannot recover data that was never written. The [survival-loop record](2026-10-28-01-skating-survival-loop.md) preserves both successful routes and losses under the newer encounter changes.
