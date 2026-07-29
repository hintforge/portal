# Portal -- Nav: Test Chamber 12

**status:** research-integrated
**last_reconciled:** 2026-06-02
**research_run:** P2 ingested 2026-06-02 (portal_p2.result.md)

**Zone:** `chamber_12` · **Segment:** Dual-portal segment · **Spoiler tier:** progression

## Entry

From `chamber_11` via chamberlock elevator. Autosave on map load (`testchmb_a_06`, shared with chamber_13).

## Exit

To `chamber_13` via chamberlock elevator (one-way, chapter-bound).

## Outgoing edges

- `(chamber_12, chamber_13)` -- story-gate (elevator + grill), solve chamber

## Entry tips

1. **One radio** on the middle support for the higher platforms — grab from the second level.
2. No cameras in this chamber.
3. A tall vertical shaft with platforms on alternating sides, each marked by dot-count symbols — count dots to track which level you're on.

## Sequential gates

| Gate ID | Name | Type | Description | Missable | One-way | Sources |
|---|---|---|---|---|---|---|
| chamber_12-gate-01 | Bottom pit (level dots) | nav | A tall room with alternating-side platforms labeled by dot-count symbols; a pit at the bottom supplies fling momentum. | no | no | [Confirmed: 2] |
| chamber_12-gate-02 | Fling to second level | puzzle | Orange portal in the pit, blue on the panel opposite the level above; fall to ascend one level. | no | no | [Confirmed: 2] |
| chamber_12-gate-03 | Radio on platform support | collectible | Radio rests on the middle support for the higher platforms; reached from the second level. | Radio (yes) | no | [Confirmed: 2] |
| chamber_12-gate-04 | Third level button | puzzle | A button on the third level controls a door on the fourth; a cube dispenser supplies the cube. | no | no | [Confirmed: 2] |
| chamber_12-gate-05 | Fourth level cube placement | puzzle | Carry a cube up, place it on the button, then re-fling to the fourth level to reach the chamberlock. | no | no | [Confirmed: 2] |
| chamber_12-gate-06 | Exit chamberlock elevator | exit | Elevator to chamber_13. | no | yes | [Confirmed: 2] |

**Checkpoint:** Chamber-entry autosave on map load. Vertical dot-numbered climb is unique — no other chamber has this layout. First post-dual-gun chamber requiring both portal types.

_source: deep-research handoff 2026-06-02 · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 1 · category: mainline · spoiler: progression_

## Sources

- StrategyWiki Portal walkthrough: https://strategywiki.org/wiki/Portal/Walkthrough
- ThePortalWiki: https://theportalwiki.com/wiki/Portal_Test_Chamber_12
