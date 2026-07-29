# Portal -- Nav: Test Chamber 01

**status:** research-integrated
**last_reconciled:** 2026-06-02
**research_run:** P2 ingested 2026-06-02 (portal_p2.result.md)

**Zone:** `chamber_01` · **Segment:** Pre-gun tutorial · **Spoiler tier:** none

## Entry

From `chamber_00` via chamberlock elevator. Autosave on inter-chamber elevator transition (within `testchmb_a_00`). No portal gun.

## Exit

To `chamber_02` via chamberlock elevator (one-way, chapter-bound).

## Outgoing edges

- `(chamber_01, chamber_02)` -- story-gate (elevator + grill), solve chamber

## Entry tips

1. No portal gun -- the static portal cycles automatically; observe the pattern before acting.
2. **Radio** atop a camera unit beside the entrance -- collectible immediately on entry (missable if you drop in without grabbing it first; gate-01 is one-way).
3. Goal: get the cube into the button room via the cycling portal, then reach the exit room the same way.

## Sequential gates

| Gate ID | Name | Type | Description | Missable | One-way | Sources |
|---|---|---|---|---|---|---|
| chamber_01-gate-01 | Entry drop / radio pickup | collectible | Entry overlooks the main pit; the radio rests atop a camera unit beside the entrance and can be grabbed before dropping in. | Radio (yes) | yes | [Confirmed: 2] |
| chamber_01-gate-02 | Cycling static portal | nav | A single orange static portal cycles between three sealed side rooms (cube room, button room, exit room); the player times entry through the matching blue side. | no | no | [Confirmed: 2] |
| chamber_01-gate-03 | Cube room | puzzle | When the portal shows the cube room, enter and retrieve the Weighted Storage Cube. | no | no | [Confirmed: 2] |
| chamber_01-gate-04 | Button room | puzzle | When the portal shows the button room, carry the cube in and place it on the button. | no | no | [Confirmed: 2] |
| chamber_01-gate-05 | Exit room reveal | nav | When the portal shows the exit-door room, pass through to reach the chamberlock. | no | yes | [Confirmed: 2] |
| chamber_01-gate-06 | Exit chamberlock elevator | exit | Elevator to chamber_02. | no | yes | [Confirmed: 2] |

**Checkpoint:** Autosave at chamber entry (inter-chamber elevator transition within `testchmb_a_00`). No mid-chamber autosave observed. No portal gun.

_source: deep-research handoff 2026-06-02 · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 0 · category: mainline · spoiler: none_

## Sources

- StrategyWiki Portal walkthrough: https://strategywiki.org/wiki/Portal/Walkthrough
- ThePortalWiki: https://theportalwiki.com/wiki/Portal_Test_Chamber_01
- Thonky Portal walkthrough: https://www.thonky.com/portal-walkthrough/
