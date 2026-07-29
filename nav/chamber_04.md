# Portal -- Nav: Test Chamber 04

**status:** research-integrated
**last_reconciled:** 2026-06-02
**research_run:** P2 ingested 2026-06-02 (portal_p2.result.md)

**Zone:** `chamber_04` · **Segment:** Blue-portal segment · **Spoiler tier:** none

## Entry

From `chamber_03` via chamberlock elevator. Autosave on map load (`testchmb_a_02`, shared with chamber_05).

## Exit

To `chamber_05` via chamberlock elevator (one-way, chapter-bound).

## Outgoing edges

- `(chamber_04, chamber_05)` -- story-gate (elevator + grill), solve chamber

## Entry tips

1. **Radio** drops with the cube from the dispenser into the pit — grab it when retrieving the cube.
2. **Two cameras** (above the button; beside the exit) — collectible before the emancipation grill.
3. Goal: retrieve the cube from the pit via the permanent orange portal at the pit floor, then place it on the floor button.

## Sequential gates

| Gate ID | Name | Type | Description | Missable | One-way | Sources |
|---|---|---|---|---|---|---|
| chamber_04-gate-01 | Cube dispenser over pit | puzzle | A dispenser drops a cube into a pit; a permanent orange portal sits at the pit floor. | Radio drops with cube (yes) | no | [Confirmed: 2] |
| chamber_04-gate-02 | Pit descent & portal exit | nav | Fire a blue portal on a pit-floor wall, then walk in to exit via the orange portal back up with the cube. | no | no | [Confirmed: 2] |
| chamber_04-gate-03 | Floor button | puzzle | Place the cube on the button to open the exit door. | no | no | [Confirmed: 2] |
| chamber_04-gate-04 | Two cameras | collectible | Cameras above the button and on the wall beside the exit. | Cameras ×2 (yes) | no | [Confirmed: 2] |
| chamber_04-gate-05 | GLaDOS "we will not monitor" line | story | On exit GLaDOS states the next chamber will be unmonitored. | no | yes | [Confirmed: 2] |
| chamber_04-gate-06 | Exit chamberlock elevator | exit | Elevator to chamber_05. | no | yes | [Confirmed: 2] |

**Checkpoint:** Chamber-entry autosave on map load (`testchmb_a_02`, shared with chamber_05). No mid-chamber autosave. ONE cube, ONE button — distinguishes this chamber from chamber_05's two-cube/two-button layout.

_source: deep-research handoff 2026-06-02 · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 0 · category: mainline · spoiler: none_

## Sources

- StrategyWiki Portal walkthrough: https://strategywiki.org/wiki/Portal/Walkthrough
- ThePortalWiki: https://theportalwiki.com/wiki/Portal_Test_Chamber_04
