# Portal -- Nav: Test Chamber 13

**status:** research-integrated
**last_reconciled:** 2026-11-06
**research_run:** P2 ingested 2026-06-02 (portal_p2.result.md)

**Zone:** `chamber_13` · **Segment:** Dual-portal segment · **Spoiler tier:** progression

## Entry

From `chamber_12` via chamberlock elevator. Autosave on map load (`testchmb_a_08`, which holds Chamber 13 only).
_source: 2026-11-06 https://theportalwiki.com/wiki/List_of_Portal_chambers, https://wiki.sourceruns.org/Portal-Maps.html · capture: browser_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 1 · category: mainline · spoiler: progression_ [Confirmed: 2]

## Exit

To `chamber_14` via exit pedestal + door + chamberlock elevator (one-way, chapter-bound).

## Outgoing edges

- `(chamber_13, chamber_14)` -- story-gate (elevator + grill), solve chamber

## Entry tips

1. **Three cameras** (above main entranceway; main-room wall beside entrance; final-passage wall) and **one radio** (on a small ledge in the main room that the moving platform passes; grab it from the platform) — all collectible.
2. First of six chambers with post-game Advanced/Challenge variants — the core puzzle structure is what those modes remit.
3. Exit via: step on the exit button, fire a portal through the opened door, drop through, reach the chamberlock.

## Sequential gates

| Gate ID | Name | Type | Description | Missable | One-way | Sources |
|---|---|---|---|---|---|---|
| chamber_13-gate-01 | First room cube + door | puzzle | Grab a cube and reach the door using two created portals. | Camera (yes) | no | [Confirmed: 2] |
| chamber_13-gate-02 | Pellet to receiver (platform) | puzzle | Portal the pellet (scorch-mark wall to ceiling red-spot) into the receiver to start a moving platform. | no | no | [Confirmed: 2] |
| chamber_13-gate-03 | First cube to the higher button | puzzle | Pull the cube off the platform and place it on the higher button: put a portal on the one-dot ceiling symbol above that button, carry the cube through and set it down. | no | no | [Single source -- verify · class:walkthrough] |
| chamber_13-gate-04 | Second cube to the other button | puzzle | Fetch the second cube from the first room's button (portals connecting the two rooms let you carry it through) and put it on the other button using the two-dot ceiling symbol, or stand on that button yourself; with both buttons held the exit door opens. | no | no | [Single source -- verify · class:walkthrough] |
| chamber_13-gate-05 | Three cameras | collectible | Cameras above the main entranceway, on the main-room wall beside the entrance, and on the final-passage wall. | Cameras ×3 (yes) | no | [Confirmed: 2] |
| chamber_13-gate-06 | Radio on the platform ledge | collectible | Radio is on a small ledge in the main room that the moving platform passes; grab it from the platform. Bring it back to the first room, near the window above the button. | Radio (yes) | no | [Confirmed: 2] |
| chamber_13-gate-07 | Exit pedestal & door | exit | Step on the exit button, fire a portal through the opened door, drop, and reach the chamberlock. Elevator to chamber_14. | no | yes | [Confirmed: 2] |

**Checkpoint:** Chamber-entry autosave. First of six chambers with Advanced/Challenge variants (unlock on game completion). Two-button puzzle requires both buttons held simultaneously via cube + pellet platform.

_source: deep-research handoff 2026-06-02 · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 1 · category: mainline · spoiler: progression_
_source: 2026-11-06 (entry tip 1, chamber_13-gate-06) https://strategywiki.org/wiki/Portal/Chamber_13, https://www.thonky.com/portal-walkthrough/transmission-received · capture: browser_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 1 · category: mainline · spoiler: progression_ [Confirmed: 2]
_source: 2026-11-06 (chamber_13-gate-03, chamber_13-gate-04) https://strategywiki.org/wiki/Portal/Chamber_13 · capture: browser_fetch · confidence: medium · enemy-tier: 0 · puzzle-tier: 1 · category: mainline · spoiler: progression_ [Single source -- verify · class:walkthrough]

## Sources

- StrategyWiki Portal walkthrough: https://strategywiki.org/wiki/Portal/Walkthrough
- ThePortalWiki: https://theportalwiki.com/wiki/Portal_Test_Chamber_13
- StrategyWiki Advanced Chambers: https://strategywiki.org/wiki/Portal/Advanced_Chambers
