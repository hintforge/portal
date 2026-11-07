# Portal -- Nav: Test Chamber 16

**status:** research-integrated
**last_reconciled:** 2026-11-06
**research_run:** P2 ingested 2026-06-02 (portal_p2.result.md)

**Zone:** `chamber_16` · **Segment:** Dual-portal segment · **Spoiler tier:** late-game

## Entry

From `chamber_15` via chamberlock elevator. Autosave on map load (`testchmb_a_11`, which holds Chamber 16 only).
_source: 2026-11-06 https://theportalwiki.com/wiki/List_of_Portal_chambers, https://wiki.sourceruns.org/Portal-Maps.html · capture: browser_fetch · confidence: high · enemy-tier: 2 · puzzle-tier: 0 · category: mainline · spoiler: late-game_ [Confirmed: 2]

## Exit

To `chamber_17` via chamberlock elevator (one-way, chapter-bound).

## Outgoing edges

- `(chamber_16, chamber_17)` -- story-gate (elevator + grill), solve chamber; last-but-one turret chamber

## Entry tips

1. **Five cameras** and **one radio** (in the side room with the stacked cubes, past the two side-by-side turrets; its signal spot is the hidden crawlspace behind the extended panel, next to the writing) — collectible; radio signal only activates post-completion (Transmission Received).
2. **"Friendly Fire" achievement opportunity** at gate-05 — knocking one turret over with another. This is the most reliable spot; turrets also appear later, in chamber_18 and in the escape.
3. Turrets fire on line-of-sight; bullet-proof glass blocks their shots. Use portals or the cube dispenser's cubes as shields to neutralize them.

## Sequential gates

| Gate ID | Name | Type | Description | Missable | One-way | Sources |
|---|---|---|---|---|---|---|
| chamber_16-gate-01 | First turret (facing away) | hazard | GLaDOS frames a "live-fire course for military androids." First turret faces away from the entrance; disarm by portal-drop or pickup. | Camera (yes) | no | [Confirmed: 2] |
| chamber_16-gate-02 | Bullet-proof glass turret trio | hazard | Three turrets fire through entry glass (glass is bullet-proof). | no | no | [Confirmed: 2] |
| chamber_16-gate-03 | Malfunctioning cube dispenser side room | puzzle | A side room dispenses many cubes usable as shields against turret fire. | no | no | [Confirmed: 2] |
| chamber_16-gate-04 | Button room (three X-marked turrets) | hazard | Three turrets marked with red X; disable and place a cube on the button to open the door. | no | no | [Confirmed: 2] |
| chamber_16-gate-05 | Friendly Fire opportunity | hazard | Knocking one turret over with another earns "Friendly Fire — Knock down a turret with another turret." An early, turret-dense place to earn it; turrets also appear later, in chamber_18 and in the escape, so it is not lost by leaving this chamber. | Achievement (yes) | no | [Confirmed: 3] |
| chamber_16-gate-06 | Fenced exit turrets | hazard | The exit is blocked by fencing and turrets; shoot portals through the fences to disable them. | no | no | [Confirmed: 2] |
| chamber_16-gate-07 | Five cameras + radio | collectible | Cameras: above the window across from entrance; after the first turret around the corner; behind the third turret in the alcove; in the button room across from the door; after the first fence. Radio in the side room with the stacked cubes (the malfunctioning cube dispenser room), past two side-by-side turrets; its signal spot is the hidden crawlspace behind the extended panel, next to the writing. | Cameras ×5 + Radio (yes) | partial | [Single source -- verify · class:walkthrough] |
| chamber_16-gate-08 | Exit chamberlock elevator | exit | Elevator to chamber_17. | no | yes | [Confirmed: 2] |

**Checkpoint:** Chamber-entry autosave on map load. Radio signal in chamber_16 activates ONLY on a second playthrough (Transmission Received is post-completion). "Friendly Fire" is not lost by leaving this chamber — turrets also appear in chamber_18 and in the escape. Turrets are the first new enemy type; see `mechanics.md` for turret behaviour.

_source: deep-research handoff 2026-06-02 · capture: web_fetch · confidence: high · enemy-tier: 2 · puzzle-tier: 0 · category: mainline · spoiler: late-game_
_source: 2026-11-06 (entry tip 1) https://strategywiki.org/wiki/Portal/Chamber_16, https://www.thonky.com/portal-walkthrough/transmission-received · capture: browser_fetch · confidence: high · enemy-tier: 2 · puzzle-tier: 0 · category: mainline · spoiler: late-game_ [Confirmed: 2]
_source: 2026-11-06 (chamber_16-gate-07) https://strategywiki.org/wiki/Portal/Chamber_16 · capture: browser_fetch · confidence: medium · enemy-tier: 2 · puzzle-tier: 0 · category: mainline · spoiler: late-game_ [Single source -- verify · class:walkthrough]
_source: 2026-11-06 (entry tip 2, chamber_16-gate-05, checkpoint) https://theportalwiki.com/wiki/Turrets, https://strategywiki.org/wiki/Portal/Transmission_Received, https://www.thonky.com/portal-walkthrough/test-chamber-19 · capture: browser_fetch · confidence: high · enemy-tier: 2 · puzzle-tier: 0 · category: mainline · spoiler: late-game_ [Confirmed: 3]

## Sources

- StrategyWiki Portal walkthrough: https://strategywiki.org/wiki/Portal/Walkthrough
- ThePortalWiki: https://theportalwiki.com/wiki/Portal_Test_Chamber_16
- Steam Community Friendly Fire guide: https://steamcommunity.com/sharedfiles/filedetails/?id=816584967
