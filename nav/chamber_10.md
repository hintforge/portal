# Portal -- Nav: Test Chamber 10

**status:** research-integrated
**last_reconciled:** 2026-06-02
**research_run:** P2 ingested 2026-06-02 (portal_p2.result.md)

**Zone:** `chamber_10` · **Segment:** Blue-portal segment · **Spoiler tier:** progression

## Entry

From `chamber_09` via chamberlock elevator. Autosave on map load (`testchmb_a_05`, shared with chamber_11).

## Exit

To `chamber_11` via chamberlock elevator (one-way, chapter-bound).

## Outgoing edges

- `(chamber_10, chamber_11)` -- story-gate (elevator + grill), solve chamber

## Entry tips

1. **One camera** (upper corner of the first room) and **one radio** (third section, mid-climb) — collectible.
2. Floor diagrams in the first room explain the momentum mechanic; study them before proceeding.
3. Goal: chain three momentum/fling rooms from entry to chamberlock — downward momentum converts to horizontal, then stacked portals fling upward.

## Sequential gates

| Gate ID | Name | Type | Description | Missable | One-way | Sources |
|---|---|---|---|---|---|---|
| chamber_10-gate-01 | First momentum room | nav | A step too high to jump; a fixed orange portal sits on a suspended panel above. Fire a blue portal in a wall and walk in to gain momentum onto the step. | Camera (yes) | no | [Confirmed: 2] |
| chamber_10-gate-02 | Camera in first room | collectible | The chamber's single camera is in the upper corner of the first room. | Camera (yes) | no | [Confirmed: 2] |
| chamber_10-gate-03 | Second room (down→horizontal) | puzzle | Floor diagrams show downward momentum converting to horizontal; drop into a floor portal to cross the pit. | no | no | [Confirmed: 2] |
| chamber_10-gate-04 | Third room double-fling | puzzle | An extending wall panel; enter backwards to trigger it, then fall through stacked portals to fling up to the higher level. | Radio (yes) | no | [Confirmed: 2] |
| chamber_10-gate-05 | Radio on third section | collectible | Radio sits in the third section; grab mid-climb on the middle level. | Radio (yes) | no | [Confirmed: 2] |
| chamber_10-gate-06 | Exit chamberlock elevator | exit | Elevator to chamber_11. | no | yes | [Confirmed: 2] |

**Checkpoint:** Chamber-entry autosave on map load. First fling/momentum tutorial chamber — floor diagrams illustrate the mechanic. One camera (upper corner, first room) is the most distinctive landmark.

_source: deep-research handoff 2026-06-02 · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 1 · category: mainline · spoiler: progression_

## Sources

- StrategyWiki Portal walkthrough: https://strategywiki.org/wiki/Portal/Walkthrough
- ThePortalWiki: https://theportalwiki.com/wiki/Portal_Test_Chamber_10
