# Portal -- Nav: Test Chamber 15

**status:** research-integrated
**last_reconciled:** 2026-11-06
**research_run:** P2 ingested 2026-06-02 (portal_p2.result.md)

**Zone:** `chamber_15` · **Segment:** Dual-portal segment · **Spoiler tier:** progression

## Entry

From `chamber_14` via chamberlock elevator. Autosave on map load (`testchmb_a_10`, which holds Chamber 15 only).
_source: 2026-11-06 https://theportalwiki.com/wiki/List_of_Portal_chambers, https://wiki.sourceruns.org/Portal-Maps.html · capture: browser_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 1 · category: mainline · spoiler: progression_ [Confirmed: 2]

## Exit

To `chamber_16` via chamberlock elevator (one-way, chapter-bound).

## Outgoing edges

- `(chamber_15, chamber_16)` -- story-gate (elevator + grill), solve chamber

## Entry tips

1. **Five cameras** (Chamber 16 also has five) and **two radios** — the highest collectible density in the early/mid game. Take note of all locations listed in gate-06 and gates-02/05.
2. Emancipation grids appear MID-puzzle (not just at the exit) — plan portal placement before passing through them.
3. Four-room structure: double-fling entry room → second room where a pellet must cross two force fields into its receiver → third room (double fling, angled-panel pellet game, backwards conveyor) → final room with a pellet launcher, two side-room buttons and the receiver that lowers the exit lift.

## Sequential gates

| Gate ID | Name | Type | Description | Missable | One-way | Sources |
|---|---|---|---|---|---|---|
| chamber_15-gate-01 | First room double-fling | puzzle | Orange portal on the extended panel above the entrance, blue on the checkered floor; fall twice to gain momentum through a force field. | Camera + Radio A (yes) | no | [Confirmed: 2] |
| chamber_15-gate-02 | Radio A on extended platform | collectible | First radio is on the support for the first room's extended platform. | Radio A (yes) | no | [Confirmed: 2] |
| chamber_15-gate-03 | Second room pellet crossing | puzzle | A pellet has to cross two force fields into the receiver: put portals on the burn mark and on another wall so the pellet flies into the receiver's side of the room, then portal in front of the pellet and the red light above the receiver before the pellet disappears. A camera sits above and to the right of this room's exit lift. | Camera (yes) | no | [Single source -- verify · class:walkthrough] |
| chamber_15-gate-04 | Third room fling side room | nav | Drop into a side room to start the third-room fling; a camera sits here. | Camera (yes) | no | [Single source -- verify · class:walkthrough] |
| chamber_15-gate-05 | Twin side-room buttons + pellet | puzzle | Two doors open via buttons in two side rooms; then route the pellet (extended panel → scorch mark) into the receiver to lower the exit lift. The second radio (15B) is in this final room, inside the glass enclosure that holds the pellet receiver: press the two buttons, then use portals (two on the ground, one in front of the enclosure) to jump into the enclosed area. | Radio B (yes) | no | [Single source -- verify · class:walkthrough] |
| chamber_15-gate-06 | Five cameras | collectible | Cameras: right wall before first room; above/beside first-room exit; above/beside second-room exit lift; in the third-room fling side room; above the final-room entrance. | Cameras ×5 (yes) | partial | [Confirmed: 2] |
| chamber_15-gate-07 | Exit lift to chamberlock | exit | Elevator to chamber_16. | no | yes | [Confirmed: 2] |

**Checkpoint:** Chamber-entry autosave on map load. Two radios (15A, 15B). Five cameras — tied with chamber_16 for the most cameras in a single chamber. Emancipation grids mid-puzzle is unique to this chamber.

_source: deep-research handoff 2026-06-02 · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 1 · category: mainline · spoiler: progression_
_source: 2026-11-06 (entry tips 1 and 3, chamber_15-gate-03, chamber_15-gate-04, chamber_15-gate-05, checkpoint) https://strategywiki.org/wiki/Portal/Chamber_15, https://strategywiki.org/wiki/Portal/Camera_Shy, https://www.thonky.com/portal-walkthrough/transmission-received · capture: browser_fetch · confidence: medium · enemy-tier: 0 · puzzle-tier: 1 · category: mainline · spoiler: progression_ [Single source -- verify · class:walkthrough]

## Sources

- StrategyWiki Portal walkthrough: https://strategywiki.org/wiki/Portal/Walkthrough
- ThePortalWiki: https://theportalwiki.com/wiki/Portal_Test_Chamber_15
- Steam Community Camera Shy guide: https://steamcommunity.com/sharedfiles/filedetails/?id=1915501465
