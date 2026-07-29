# Portal -- Nav: Test Chamber 18

**status:** research-integrated
**last_reconciled:** 2026-06-02
**research_run:** P2 ingested 2026-06-02 (portal_p2.result.md)

**Zone:** `chamber_18` · **Segment:** Dual-portal segment · **Spoiler tier:** late-game

## Entry

From `chamber_17` via chamberlock elevator. Autosave on map load (`testchmb_a_09`, shared with chamber_19).

## Exit

To `chamber_19` via chamberlock elevator (one-way, chapter-bound). Last turret chamber — **"Friendly Fire" PoNR**.

> **Cross-system dependency** -- see `dependencies.md` PON-001: Exiting this chamber permanently locks out the Friendly Fire achievement; no turrets remain after chamber_18.

## Outgoing edges

- `(chamber_18, chamber_19)` -- story-gate (elevator + grill); last turret chamber (Friendly Fire PoNR)

## Entry tips

1. **Two cameras** and **three radios** (18A, 18B, 18C) — most radios of any single chamber. All collectible.
2. **"Friendly Fire" last chance** — this is the final chamber with turrets on a linear playthrough. If missed in chamber_16, prioritize it here.
3. Three-part gauntlet: (1) fling platform chain → (2) turret+pellet+moving platform section → (3) linked flings to exit. Each part has distinct hazards.

## Sequential gates

| Gate ID | Name | Type | Description | Missable | One-way | Sources |
|---|---|---|---|---|---|---|
| chamber_18-gate-01 | Part 1 — drops & flings (dot platforms) | puzzle | Entry shelf overlooks platforms marked with dot symbols (one-, two-, three-dot); chain flings toward the button outside the turret room. | Radio 18A (yes) | no | [Confirmed: 2] |
| chamber_18-gate-02 | Radio 18A (first side room) | collectible | First radio is in the side room after the first gap. | Radio 18A (yes) | no | [Confirmed: 2] |
| chamber_18-gate-03 | Pedestal button + piston door | nav | Press the pedestal button and crouch under the door piston to enter the turret room without immediate fire. | no | no | [Confirmed: 2] |
| chamber_18-gate-04 | Part 2 — turret room + pellets + platform | hazard | Turrets and energy pellets; a cube must be retrieved and placed on a button; a moving platform crosses (or fling across the angled door panel). | Radios 18B/18C + Camera (yes) | no | [Confirmed: 2] |
| chamber_18-gate-05 | Second Rattman den | story | The chamber houses the second Rattman den (cameras stackable from it). | Lore (yes) | no | [Confirmed: 2] |
| chamber_18-gate-06 | Part 3 — linked flings | puzzle | A sequence of linked flings between higher platforms to the exit. | no | no | [Confirmed: 2] |
| chamber_18-gate-07 | Two cameras | collectible | Cameras: next to the window at the turret-room entrance; on the wall of the final-room entrance. | Cameras ×2 (yes) | partial | [Confirmed: 2] |
| chamber_18-gate-08 | Exit chamberlock elevator | exit | Elevator to chamber_19. | no | yes | [Confirmed: 2] |

**Checkpoint:** Chamber-entry autosave on map load. Three radios + two cameras. The chamber start (vertical ceiling/floor surface) is a common spot for the "Terminal Velocity" achievement via an infinite portal fall. Second Rattman den is optional/lore.

_source: deep-research handoff 2026-06-02 · capture: web_fetch · confidence: high · enemy-tier: 2 · puzzle-tier: 0 · category: mainline · spoiler: late-game_

## Sources

- StrategyWiki Portal walkthrough: https://strategywiki.org/wiki/Portal/Walkthrough
- ThePortalWiki: https://theportalwiki.com/wiki/Portal_Test_Chamber_18
- Steam Community Friendly Fire guide: https://steamcommunity.com/sharedfiles/filedetails/?id=816584967
