# Portal -- Nav: Test Chamber 07

**status:** research-integrated
**last_reconciled:** 2026-11-06
**research_run:** P2 ingested 2026-06-02 (portal_p2.result.md)

**Zone:** `chamber_07` · **Segment:** Blue-portal segment · **Spoiler tier:** none

## Entry

From `chamber_06` via chamberlock elevator. Autosave on inter-chamber elevator transition (within `testchmb_a_03`, shared with chamber_06).

## Exit

To `chamber_08` via chamberlock elevator (one-way, chapter-bound).

## Outgoing edges

- `(chamber_07, chamber_08)` -- story-gate (elevator + grill), solve chamber

## Entry tips

1. **One radio** beneath the entrance stairs — grab it before dropping in; the gate is one-way (yes).
2. No cameras in this chamber.
3. Pellet receiver powers a **moving platform** (not a fixed lift like chamber_06) — board the platform once it starts.

## Sequential gates

| Gate ID | Name | Type | Description | Missable | One-way | Sources |
|---|---|---|---|---|---|---|
| chamber_07-gate-01 | Radio under entrance stairs | collectible | Radio is beneath the entrance platform behind the stairs; reachable by crouch or portal. | Radio (yes) | yes | [Confirmed: 2] |
| chamber_07-gate-02 | Pellet launcher & scorch mark | hazard | Pellet bounces and leaves a scorch mark on the far wall; fixed orange portal on the floor routes it. | no | no | [Confirmed: 2] |
| chamber_07-gate-03 | Pellet receiver powers platform | puzzle | Routing the pellet into the receiver starts a moving platform. | no | no | [Confirmed: 2] |
| chamber_07-gate-04 | Board the moving platform | nav | Place a blue portal on the ceiling above the left side of the platform's path, then drop through the fixed orange portal in the floor when the platform is directly below it, and ride the platform toward the chamberlock. | no | no | [Confirmed: 2] |
| chamber_07-gate-05 | Exit chamberlock elevator | exit | Elevator to chamber_08. | no | yes | [Confirmed: 2] |

**Checkpoint:** Chamber-entry autosave on inter-chamber elevator transition. No lethal floor (distinguishes from chamber_08's acid floor). Moving platform (vs. fixed lift in chamber_06).

_source: deep-research handoff 2026-06-02 · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 0 · category: mainline · spoiler: none_
_source: 2026-11-06 (chamber_07-gate-04) https://strategywiki.org/wiki/Portal/Chamber_07, https://www.thonky.com/portal-walkthrough/test-chamber-07 · capture: browser_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 0 · category: mainline · spoiler: none_ [Confirmed: 2]

## Sources

- StrategyWiki Portal walkthrough: https://strategywiki.org/wiki/Portal/Walkthrough
- ThePortalWiki: https://theportalwiki.com/wiki/Portal_Test_Chamber_07
