# Portal -- Nav: Escape Sequence

**status:** research-integrated
**last_reconciled:** 2026-06-02
**research_run:** P2 ingested 2026-06-02 (portal_p2.result.md)

**Zone:** `escape_seq` · **Segment:** Escape Sequence · **Spoiler tier:** story

## Entry

From `chamber_19` (fire-pit escape, gate-07) — no loading screen between chamber_19's exit and the first escape segment. Autosave on each escape map load (`escape_00`, `escape_01`, `escape_02`); designer-placed autosave triggers may occur before the boss arena `[Hypothesis — unverified]`.

## Exit

To `[end / credits]` via GLaDOS defeat — **permanent, game ends**.

## Outgoing edges

- `(escape_seq, [end])` -- permanent; destroy all 4 personality cores

## Entry tips

1. **Three radios** (24, 25, 26) spread across the escape maps — collectible. No cameras (Camera Shy set ends at chamber_19).
2. The "Long Jump" achievement (travel 300 feet in a single fling) is best attempted in the large room with the muddy trench early in the escape.
3. Rusty maintenance tunnels with Rattman's red directional arrows point the route — follow the arrows.

## Sequential gates

| Gate ID | Name | Type | Description | Missable | One-way | Sources |
|---|---|---|---|---|---|---|
| escape_seq-gate-01 | Maintenance corridors (Rattman arrows) | nav | Rusty back stairways and tunnels marked with Rattman writings and red arrows pointing the route. | no | yes | [Confirmed: 2] |
| escape_seq-gate-02 | Five-piston room | hazard | A room of five large vertical pistons; portal-stand past them. Radio is in a side room reached by a portal through a gate before this room. | Radio 24 (yes) | yes | [Confirmed: 2] |
| escape_seq-gate-03 | Ceiling-piston room | nav | Pistons that strike the ceiling; ride a piston and double-fling up to the next landing. | no | yes | [Confirmed: 2] |
| escape_seq-gate-04 | Cube tubes & fan vent | nav | Walk along cube-transport tubes over goo; a fan vent leads to a sewage area (`escape_00` → `escape_01`). | no | yes | [Confirmed: 2] |
| escape_seq-gate-05 | Turret ambush room | hazard | Three doors open in sequence, each revealing a turret; disable each quickly. Radio is on a table in the malfunctioning turret room. | Radio 25 (yes) | yes | [Confirmed: 2] |
| escape_seq-gate-06 | Rocket turret + cube tube | hazard | A rocket-firing turret (cannot be destroyed); trick its rockets to break a storage-cube tube and free a cube. | no | yes | [Confirmed: 2] |
| escape_seq-gate-07 | Fan / sewage to GLaDOS approach | nav | Portal through a fan and across goo/sewers toward GLaDOS's chamber (`escape_01` → `escape_02`). | no | yes | [Confirmed: 2] |
| escape_seq-gate-08 | Green generators & fling to walkway | nav | Non-lethal goo with green generators; radio is in the goo. Fling up to the suspended walkway leading to GLaDOS. | Radio 26 (yes) | yes | [Confirmed: 2] |
| escape_seq-gate-09 | GLaDOS — morality core | story | GLaDOS drops a morality core; carry it to the incinerator, press the switch, and incinerate it (triggers a neurotoxin countdown). | no | no | [Confirmed: 2] |
| escape_seq-gate-10 | GLaDOS — rocket-redirect cores | story | Redirect the rocket turret's rockets (through portals) into GLaDOS to dislodge each of her remaining cores; incinerate all four. | no | no | [Confirmed: 2] |
| escape_seq-gate-11 | Ending | exit | After the final core, the boss sequence concludes and the game completes — earns "Heartbreaker — Complete Portal" (credits / "Still Alive"). | Achievement (yes) | yes | [Confirmed: 2] |

**Checkpoint:** Autosave on each escape map load (`escape_00`, `escape_01`, `escape_02`); possible designer-placed autosave before boss arena `[Hypothesis — unverified]`. Three radios across the escape (24/25/26). No cameras (Camera Shy count ends at chamber_19). All escape gates are one-way.

_source: deep-research handoff 2026-06-02 · capture: web_fetch · confidence: high · enemy-tier: 2 · puzzle-tier: 3 · category: mainline · spoiler: story_

## Design split

This file owns sequential gate routing for the escape sequence. Boss-fight mechanics, story beats, collectibles summary, and the faster-exploit strategy live in `sections/escape_seq.md`. Gates 09-10 above are condensed to routing-level descriptions; full boss strategy is in `sections/escape_seq.md`. This split is intentional — do not merge.

## Sources

- StrategyWiki Portal walkthrough: https://strategywiki.org/wiki/Portal/Walkthrough
- ThePortalWiki: https://theportalwiki.com/wiki/Portal_Escape_(Part_1)
- Combine OverWiki / Half-Life Wiki, "GLaDOS' testing track (Portal)": https://combineoverwiki.net/wiki/GLaDOS'_testing_track_(Portal)
