# Portal -- Nav: Test Chamber 08

**status:** research-integrated
**last_reconciled:** 2026-11-06
**research_run:** P2 ingested 2026-06-02 (portal_p2.result.md)

**Zone:** `chamber_08` · **Segment:** Blue-portal segment · **Spoiler tier:** progression

## Entry

From `chamber_07` via chamberlock elevator. Autosave on map load (`testchmb_a_04`, which holds Chamber 08 only).
_source: 2026-11-06 https://theportalwiki.com/wiki/List_of_Portal_chambers, https://wiki.sourceruns.org/Portal-Maps.html · capture: browser_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 1 · category: mainline · spoiler: progression_ [Confirmed: 2]

## Exit

To `chamber_09` via chamberlock elevator (one-way, chapter-bound).

## Outgoing edges

- `(chamber_08, chamber_09)` -- story-gate (elevator + grill), solve chamber

## Entry tips

1. **One radio** under the moving platform's start position — grab it from the fixed platform that holds the orange portal (not while riding): put a blue portal behind or near the radio and reach through. Bring it back to the entrance, near the chamber number.
2. No cameras in this chamber.
3. The entire floor is lethal acid — **manual quicksave (F6) strongly advised** before hazardous moves. Automatic save is only at chamber entry.

## Sequential gates

| Gate ID | Name | Type | Description | Missable | One-way | Sources |
|---|---|---|---|---|---|---|
| chamber_08-gate-01 | Acid floor warning | hazard | GLaDOS announces a "consequence for failure"; any contact with the chamber floor (acid) is fatal. | no | no | [Confirmed: 2] |
| chamber_08-gate-02 | Pellet reorientation portal | puzzle | Place a blue portal on the far-wall burn mark to redirect the pellet out of the floor orange portal. | no | no | [Confirmed: 2] |
| chamber_08-gate-03 | Feed the pellet receiver | puzzle | Second portal routes the reoriented pellet into the receiver, starting the moving platform. | no | no | [Confirmed: 2] |
| chamber_08-gate-04 | Radio under moving platform | collectible | Radio sits beneath the platform's initial position; grab it from the fixed platform with the orange portal (not while riding) by putting a blue portal behind or near the radio, then bring it back to the entrance near the chamber number. | Radio (yes) | no | [Confirmed: 2] |
| chamber_08-gate-05 | Two-stage platform ride | nav | Portal to the ledge, then portal beside the platform track and ride it to the chamberlock. | no | no | [Confirmed: 2] |
| chamber_08-gate-06 | Exit chamberlock elevator | exit | Elevator to chamber_09. | no | yes | [Confirmed: 2] |

**Checkpoint:** Chamber-entry autosave on map load. Manual quicksave (F6) strongly advised — lethal acid floor throughout. Pellet must bounce off a wall before reaching the receiver (more complex routing than chamber_06/07).

_source: deep-research handoff 2026-06-02 · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 1 · category: mainline · spoiler: progression_
_source: 2026-11-06 (entry tip 1, chamber_08-gate-04) https://strategywiki.org/wiki/Portal/Chamber_08, https://www.thonky.com/portal-walkthrough/transmission-received · capture: browser_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 1 · category: mainline · spoiler: progression_ [Confirmed: 2]

## Sources

- StrategyWiki Portal walkthrough: https://strategywiki.org/wiki/Portal/Walkthrough
- ThePortalWiki: https://theportalwiki.com/wiki/Portal_Test_Chamber_08
- StrategyWiki Tips (death-reload behavior): https://strategywiki.org/wiki/Portal/Tips_and_advanced_techniques
