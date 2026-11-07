# Portal -- Nav: Test Chamber 06

**status:** research-integrated
**last_reconciled:** 2026-11-06
**research_run:** P2 ingested 2026-06-02 (portal_p2.result.md)

**Zone:** `chamber_06` · **Segment:** Blue-portal segment · **Spoiler tier:** none

## Entry

From `chamber_05` via chamberlock elevator. Autosave on map load (`testchmb_a_03`, shared with chamber_07).

## Exit

To `chamber_07` via chamberlock elevator (one-way, chapter-bound).

## Outgoing edges

- `(chamber_06, chamber_07)` -- story-gate (elevator + grill), solve chamber

## Entry tips

1. **One radio** above the pellet launcher, on the corner nearest the entrance (on the edge of the ceiling piece the launcher hangs from) — fire a portal on the ceiling near it, grab the radio through the portal, and carry it to the victory lift.
2. No cameras in this chamber.
3. High Energy Pellet (the bouncing energy ball) kills on contact — keep distance until you understand the routing.

## Sequential gates

| Gate ID | Name | Type | Description | Missable | One-way | Sources |
|---|---|---|---|---|---|---|
| chamber_06-gate-01 | Portal-proof wall introduction | nav | From here some walls are dark/brown (non-portalable) versus light-grey portalable panels. | no | no | [Confirmed: 2] |
| chamber_06-gate-02 | Pellet launcher + fixed orange portal | hazard | A High Energy Pellet launcher fires a pellet that instantly kills on contact; a fixed orange portal sits beneath the launcher. | no | no | [Confirmed: 2] |
| chamber_06-gate-03 | Pellet receiver (red glow) | puzzle | Place a blue portal across from the receiver (located via the red light it casts on the ceiling) to route the pellet in. | no | no | [Confirmed: 2] |
| chamber_06-gate-04 | Radio above pellet launcher | collectible | Radio sits above the pellet launcher, on the corner nearest the entrance; put a portal on the ceiling near it and grab the radio through the portal, then carry it to the victory lift. | Radio (yes) | no | [Confirmed: 2] |
| chamber_06-gate-05 | Victory lift to chamberlock | nav | The captured pellet powers a lift up to the chamberlock. | no | yes | [Confirmed: 2] |
| chamber_06-gate-06 | Exit chamberlock elevator | exit | Elevator to chamber_07. | no | yes | [Confirmed: 2] |

**Checkpoint:** Chamber-entry autosave on map load. First High Energy Pellet chamber — simplest layout (single pellet → fixed lift). Portalable vs. non-portalable wall textures introduced here.

_source: deep-research handoff 2026-06-02 · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 0 · category: mainline · spoiler: none_
_source: 2026-11-06 (entry tip 1, chamber_06-gate-04) https://strategywiki.org/wiki/Portal/Chamber_06, https://www.thonky.com/portal-walkthrough/transmission-received · capture: browser_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 0 · category: mainline · spoiler: none_ [Confirmed: 2]

## Sources

- StrategyWiki Portal walkthrough: https://strategywiki.org/wiki/Portal/Walkthrough
- ThePortalWiki: https://theportalwiki.com/wiki/Portal_Test_Chamber_06
