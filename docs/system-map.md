# System map

I use this map to explain how movement, presentation and survival systems share player and run state in the Unreal game module. It shows conceptual relationships rather than independent services or an exact call sequence.

```mermaid
flowchart TD
    Input[Keyboard and controller input] --> Skate[Skating simulation]
    City[City surfaces, ramps and rails] --> Skate
    Skate --> State[Position, velocity and movement mode]
    Skate --> Tricks[Trick chain and scoring]
    State --> Rig[Board and rider presentation]
    State --> Camera[Chase camera]
    City --> Camera
    State --> Combat[Enemies and combat]
    City --> Combat
    Run[Run progression and upgrades] --> Combat
    Combat --> Rewards[Health, pickups and rewards]
    Rewards --> Run
    Tricks --> Sessions[Claimed skate sessions]
    Sessions --> Rewards
    Sessions --> Pressure[District heat and encounter beats]
    Pressure --> Combat
    Tricks --> Boost[Bounded combat boost]
    Boost --> Combat
    Run --> Result[Recorded run result]
    Result --> Pending[Pending profile write]
    Pending --> Profile[Validated profile and backup]
    Profile --> Garage[Earned starting weapons]
    Garage --> Run
    Tricks --> HUD[Player feedback and HUD]
    Run --> HUD
    Rewards --> HUD
    Combat --> Threats[Grouped approach warnings]
    Combat --> Damage[Actual damage attribution]
    Threats --> HUD
    Damage --> HUD
    Rig --> Visibility[Occluded rider silhouette]
```

## Movement and presentation

Skating advances at a fixed 120 Hz simulation step, with movement interpolation for presentation. The chase camera responds to movement and environment information. The central concern is continuity through landing, manual, ollie, rail catch and departure transitions.

Surface interaction and presentation must agree about board support. To preserve forgiving inputs, I retained generous lateral catch assistance while limiting forward snapping and protecting the intended rail choice. Intermediate camera-clearance checks account for obstacles along the path, even when the destination is clear.

## Survival connection

Combat and run progression share player position and run state. Banked lines advance linked skate sessions and grant a bounded combat boost near enemies. Claimed spots provide experience and gear, increase district heat and advance encounter beats with a recovery interval. Directed packs and committed warnings bring pressure onto the current skating route. The boss and exit use deliberate interactions rather than automatically ending the run.

## District geometry and combat clarity

District geometry also determines weapon visibility, surface-aware hazards and enemy roof approaches. The transit crossing separates its physical underside from its supported top. Navigation reaches its bank crest before aligning on the station roof, avoiding an early turn off the approach. Camera focus can remain beneath the slab while swept obstruction still prevents passing through it.

Approach warnings reuse committed attack geometry and keep a bounded set of directions. Actual mitigated health loss feeds the damage ledger independently of those predictions. The rider and board contribute their animated geometry to a depth/stencil silhouette when occluded; world and enemy shading remain unchanged.

## Persistence and desktop flow

Run accounting rejects duplicate results independently of disk writing. A pending-write state allows garage/start/equip flows to retry a failed save without granting the result again. Validated profile replacement and backups preserve the prior valid state. Earned totals unlock starting weapons; unavailable saved selections fall back safely.

Menu confirmation ownership prevents controller presses from becoming skating actions on transition. Desktop settings persist display, sound-effects and look preferences separately from the progression profile.

## Verification boundary

Automated checks cover specific movement rules, combat interactions, input transitions and persistence boundaries. Rendered captures provide evidence for board support and visibility. Bounded ordinary-run captures include real reward acquisition and losses; they are distinguished from staged fixtures. Measured crowd samples do not establish longer survival or final release performance, and hands-on feel remains a separate question.

The diagram uses [GitHub’s supported Mermaid format](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/creating-diagrams).
