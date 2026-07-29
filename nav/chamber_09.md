# Portal -- Nav: Test Chamber 09

**status:** research-integrated
**last_reconciled:** 2026-06-02
**research_run:** P2 ingested 2026-06-02 (portal_p2.result.md)

**Zone:** `chamber_09` · **Segment:** Blue-portal segment · **Spoiler tier:** progression

## Entry

From `chamber_08` via chamberlock elevator. Autosave on inter-chamber elevator transition (within `testchmb_a_04`, shared with chamber_08).

## Exit

To `chamber_10` via chamberlock elevator (one-way, chapter-bound).

## Outgoing edges

- `(chamber_09, chamber_10)` -- story-gate (elevator + grill), solve chamber

## Entry tips

1. **One radio** wedged in the gap between the two sections — risky to grab (can be destroyed in the emancipation grid); **quicksave (F6) first**.
2. No cameras in this chamber.
3. The emancipation grid mid-room destroys the cube — if lost, approach the dispenser platform again to receive a replacement.

## Sequential gates

| Gate ID | Name | Type | Description | Missable | One-way | Sources |
|---|---|---|---|---|---|---|
| chamber_09-gate-01 | "This test is impossible" line | story | GLaDOS declares the test impossible and tells the player not to attempt it. | no | no | [Confirmed: 2] |
| chamber_09-gate-02 | Cube dispenser + emancipation grid | puzzle | Cube is taken up to a platform via a fixed orange portal; an emancipation grid separates the two sections (destroyed cubes are re-dispensed). | no | no | [Confirmed: 2] |
| chamber_09-gate-03 | Radio in the section gap | collectible | Radio is wedged in the small opening between the two sections; risky to grab (can be destroyed in the grid — save first). | Radio (yes) | no | [Confirmed: 2] |
| chamber_09-gate-04 | Button across the grid | puzzle | Pass a cube through to the button section and place it to open the chamberlock door. | no | no | [Confirmed: 2] |
| chamber_09-gate-05 | Exit chamberlock elevator | exit | Elevator to chamber_10. | no | yes | [Confirmed: 2] |

**Checkpoint:** Chamber-entry autosave on inter-chamber elevator transition. Note: chamber_09's main room is revisited (rearranged) during the escape sequence. The emancipation grid here is used as a puzzle element, not just an exit device.

_source: deep-research handoff 2026-06-02 · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 1 · category: mainline · spoiler: progression_

## Sources

- StrategyWiki Portal walkthrough: https://strategywiki.org/wiki/Portal/Walkthrough
- ThePortalWiki: https://theportalwiki.com/wiki/Portal_Test_Chamber_09
