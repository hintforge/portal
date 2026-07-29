# Portal -- Nav: Test Chamber 03

**status:** research-integrated
**last_reconciled:** 2026-06-02
**research_run:** P2 ingested 2026-06-02 (portal_p2.result.md)

**Zone:** `chamber_03` · **Segment:** Blue-portal segment · **Spoiler tier:** none

## Entry

From `chamber_02` via chamberlock elevator. Autosave on inter-chamber elevator transition (within `testchmb_a_01`, shared with chamber_02).

## Exit

To `chamber_04` via chamberlock elevator (one-way, chapter-bound).

## Outgoing edges

- `(chamber_03, chamber_04)` -- story-gate (elevator + grill), solve chamber

## Entry tips

1. **Three cameras** (next to the chamber number sign, above the orange portal, on the wall before the chamberlock) and **one radio** — all collectible.
2. No cubes or buttons — this chamber is pure portal traversal across three piers.
3. Goal: use the permanent orange portal on the middle pier to chain blue portals and reach the third pier / chamberlock.

## Sequential gates

| Gate ID | Name | Type | Description | Missable | One-way | Sources |
|---|---|---|---|---|---|---|
| chamber_03-gate-01 | First pier (start) | nav | Player stands on the first of three piers; the chamberlock sits on the third. No doors, buttons, or cubes. | no | no | [Confirmed: 2] |
| chamber_03-gate-02 | Permanent orange portal (middle pier) | nav | A fixed orange portal occupies the middle pier; firing a blue portal beside the start traverses to it. | no | no | [Confirmed: 2] |
| chamber_03-gate-03 | Chamber-number signage camera | collectible | Camera mounted next to the chamber number sign. | Camera (yes) | no | [Confirmed: 2] |
| chamber_03-gate-04 | Radio near exit camera | collectible | Radio is obtained after detaching the camera by the exit; routed through the orange portal. | Radio (yes) | no | [Confirmed: 2] |
| chamber_03-gate-05 | Second traverse to third pier | puzzle | Fire a blue portal reachable from the middle pier to reach the third pier / chamberlock. | no | no | [Confirmed: 2] |
| chamber_03-gate-06 | Exit chamberlock elevator | exit | Elevator to chamber_04. | no | yes | [Confirmed: 2] |

**Checkpoint:** Chamber-entry autosave on inter-chamber elevator transition. Three cameras total: next to chamber number, above the orange portal, right wall before chamberlock.

_source: deep-research handoff 2026-06-02 · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 0 · category: mainline · spoiler: none_

## Sources

- StrategyWiki Portal walkthrough: https://strategywiki.org/wiki/Portal/Walkthrough
- ThePortalWiki: https://theportalwiki.com/wiki/Portal_Test_Chamber_03
