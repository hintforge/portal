# Portal -- Nav: Test Chamber 14

**status:** research-integrated
**last_reconciled:** 2026-06-02
**research_run:** P2 ingested 2026-06-02 (portal_p2.result.md)

**Zone:** `chamber_14` · **Segment:** Dual-portal segment · **Spoiler tier:** progression

## Entry

From `chamber_13` via chamberlock elevator. Autosave on map load (`testchmb_a_07`, shared with chamber_15).

## Exit

To `chamber_15` via victory lift + chamberlock elevator (one-way, chapter-bound).

## Outgoing edges

- `(chamber_14, chamber_15)` -- story-gate (elevator + grill), pellet routed into receiver

## Entry tips

1. **One radio** on the support for the extended platform in the first room — collectible on entry.
2. No cameras in this chamber.
3. Two-part layout: first room (stairs + raised cube + button) opens into a sludge room with sinking platforms; the pellet antechamber beyond that ends at the victory lift.

## Sequential gates

| Gate ID | Name | Type | Description | Missable | One-way | Sources |
|---|---|---|---|---|---|---|
| chamber_14-gate-01 | Rising stairs / raised cube | puzzle | Walking forward raises stairs to the pellet-receiver area; a cube sits on an unclimbable raised platform reached by a fling. | Radio (yes) | no | [Confirmed: 2] |
| chamber_14-gate-02 | Radio on extended-platform support | collectible | Radio is on the support for the extended platform in the first room. | Radio (yes) | no | [Confirmed: 2] |
| chamber_14-gate-03 | Cube to button (open corridor) | puzzle | Place the cube on the button to open the door to the sludge room. | no | no | [Confirmed: 2] |
| chamber_14-gate-04 | Sludge room moving platforms | hazard | A goo-filled room with platforms that rise and sink; cross to the pellet-launcher antechamber. | no | no | [Confirmed: 2] |
| chamber_14-gate-05 | Long pellet route to receiver | puzzle | Place a portal on the scorch mark and another above the receiver to route the pellet around corners. | no | no | [Confirmed: 2] |
| chamber_14-gate-06 | Victory lift to chamberlock | exit | The captured pellet activates a victory lift. Elevator to chamber_15. | no | yes | [Confirmed: 2] |

**Checkpoint:** Chamber-entry autosave on map load. Rising-and-retracting stairs + long pellet routing is the distinctive layout. Sludge platforms are hazardous but not instantly lethal.

_source: deep-research handoff 2026-06-02 · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 1 · category: mainline · spoiler: progression_

## Sources

- StrategyWiki Portal walkthrough: https://strategywiki.org/wiki/Portal/Walkthrough
- ThePortalWiki: https://theportalwiki.com/wiki/Portal_Test_Chamber_14
