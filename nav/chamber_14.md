# Portal -- Nav: Test Chamber 14

**status:** research-integrated
**last_reconciled:** 2026-11-06
**research_run:** P2 ingested 2026-06-02 (portal_p2.result.md)

**Zone:** `chamber_14` · **Segment:** Dual-portal segment · **Spoiler tier:** progression

## Entry

From `chamber_13` via chamberlock elevator. Autosave on map load (`testchmb_a_09`, which holds Chamber 14 only).
_source: 2026-11-06 https://theportalwiki.com/wiki/List_of_Portal_chambers, https://wiki.sourceruns.org/Portal-Maps.html · capture: browser_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 1 · category: mainline · spoiler: progression_ [Confirmed: 2]

## Exit

To `chamber_15` via victory lift + chamberlock elevator (one-way, chapter-bound).

## Outgoing edges

- `(chamber_14, chamber_15)` -- story-gate (elevator + grill), pellet routed into receiver

## Entry tips

1. **One radio** on a ledge on the right: between the button and the door it powers, on the right wall (also described as a ledge to the right of the hallway you arrive from). Grab it with momentum and a portal below it as you fall past; the extended-platform-support radio belongs to chamber_15.
2. No cameras in this chamber.
3. Two-part layout: first room (stairs + raised cube + button) opens into a sludge room with sinking platforms; the pellet antechamber beyond that ends at the victory lift.

## Sequential gates

| Gate ID | Name | Type | Description | Missable | One-way | Sources |
|---|---|---|---|---|---|---|
| chamber_14-gate-01 | Rising stairs / raised cube | puzzle | Walking forward raises stairs to the pellet-receiver area; a cube sits on an unclimbable raised platform reached by a fling. | Radio (yes) | no | [Confirmed: 2] |
| chamber_14-gate-02 | Radio on the right-hand ledge | collectible | Radio is on a ledge on the right, between the button and the door it powers (also described as a ledge to the right of the arrival hallway); use momentum and a portal below it to grab it. Bring it to the stationary platform in the middle of the sludge. | Radio (yes) | no | [Confirmed: 2] |
| chamber_14-gate-03 | Cube to button (open corridor) | puzzle | Place the cube on the button to open the door to the sludge room. | no | no | [Confirmed: 2] |
| chamber_14-gate-04 | Sludge room moving platforms | hazard | A goo-filled room with platforms that rise and sink; cross to the pellet-launcher antechamber. | no | no | [Confirmed: 2] |
| chamber_14-gate-05 | Long pellet route to receiver | puzzle | Place a portal on the scorch mark and another above the receiver to route the pellet around corners. | no | no | [Confirmed: 2] |
| chamber_14-gate-06 | Victory lift to chamberlock | exit | The captured pellet activates a victory lift. Elevator to chamber_15. | no | yes | [Confirmed: 2] |

**Checkpoint:** Chamber-entry autosave on map load. Rising-and-retracting stairs + long pellet routing is the distinctive layout. Sludge platforms are hazardous but not instantly lethal.

_source: deep-research handoff 2026-06-02 · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 1 · category: mainline · spoiler: progression_
_source: 2026-11-06 (entry tip 1, chamber_14-gate-02) https://strategywiki.org/wiki/Portal/Chamber_14, https://www.thonky.com/portal-walkthrough/transmission-received · capture: browser_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 1 · category: mainline · spoiler: progression_ [Confirmed: 2]

## Sources

- StrategyWiki Portal walkthrough: https://strategywiki.org/wiki/Portal/Walkthrough
- ThePortalWiki: https://theportalwiki.com/wiki/Portal_Test_Chamber_14
