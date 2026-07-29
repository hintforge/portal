# Portal -- Nav: Test Chamber 05

**status:** research-integrated
**last_reconciled:** 2026-06-02
**research_run:** P2 ingested 2026-06-02 (portal_p2.result.md)

**Zone:** `chamber_05` · **Segment:** Blue-portal segment · **Spoiler tier:** none

## Entry

From `chamber_04` via chamberlock elevator. Autosave on inter-chamber elevator transition (within `testchmb_a_02`, shared with chamber_04).

## Exit

To `chamber_06` via chamberlock elevator (one-way, chapter-bound).

## Outgoing edges

- `(chamber_05, chamber_06)` -- story-gate (elevator + grill), solve chamber

## Entry tips

1. **Three cameras** and **one radio** (behind the two-button door) — collectible.
2. Two cubes, two buttons — both buttons must be held simultaneously to open the exit door.
3. A permanent orange portal in the ceiling leads to the chamberlock; fire a blue portal beside yourself to ascend once both buttons are held.

## Sequential gates

| Gate ID | Name | Type | Description | Missable | One-way | Sources |
|---|---|---|---|---|---|---|
| chamber_05-gate-01 | Pit cube retrieval | puzzle | One cube lies in a pit (as in chamber_04); fire a blue portal into the pit and retrieve it. | no | no | [Confirmed: 2] |
| chamber_05-gate-02 | First button | puzzle | Place the first cube on one of two floor buttons. | no | no | [Confirmed: 2] |
| chamber_05-gate-03 | Platform cube + permanent orange portal | puzzle | A second cube sits on one of two raised platforms; the other platform holds a fixed orange portal used to reach it. | no | no | [Confirmed: 2] |
| chamber_05-gate-04 | Second button (two-button door) | puzzle | Place the second cube on the second button; both buttons open the door. | no | no | [Confirmed: 2] |
| chamber_05-gate-05 | Radio behind two-button door | collectible | Radio sits behind the door opened by both buttons; can be dropped into the pit and carried out. | Radio (yes) | no | [Confirmed: 2] |
| chamber_05-gate-06 | GLaDOS "outright fabrication" line | story | GLaDOS admits the prior no-monitoring claim was false. | no | yes | [Confirmed: 2] |
| chamber_05-gate-07 | Ceiling orange portal to chamberlock | nav | A fixed orange portal in the ceiling above the chamberlock (one floor up); fire a blue portal beside you to reach it. | Cameras ×3 (yes) | yes | [Confirmed: 2] |
| chamber_05-gate-08 | Exit chamberlock elevator | exit | Elevator to chamber_06. | no | yes | [Confirmed: 2] |

**Checkpoint:** Chamber-entry autosave on inter-chamber elevator transition. Three cameras: above doorway next to chamber number, above/beside first exit door, in the final ceiling-portal section. Two cubes and two buttons distinguishes this from chamber_04 (one cube/one button).

_source: deep-research handoff 2026-06-02 · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 0 · category: mainline · spoiler: none_

## Sources

- StrategyWiki Portal walkthrough: https://strategywiki.org/wiki/Portal/Walkthrough
- ThePortalWiki: https://theportalwiki.com/wiki/Portal_Test_Chamber_05
