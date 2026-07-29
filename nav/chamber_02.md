# Portal -- Nav: Test Chamber 02

**status:** research-integrated
**last_reconciled:** 2026-06-02
**research_run:** P2 ingested 2026-06-02 (portal_p2.result.md)

**Zone:** `chamber_02` · **Segment:** Blue-portal segment · **Spoiler tier:** none

## Entry

From `chamber_01` via chamberlock elevator. Autosave on map load (`testchmb_a_01`, shared with chamber_03).

## Exit

To `chamber_03` via chamberlock elevator (one-way, chapter-bound).

## Outgoing edges

- `(chamber_02, chamber_03)` -- story-gate (elevator + grill), solve chamber

## Entry tips

1. **Three cameras** and **one radio** here — all collectible (missable: partial). Detach cameras before passing the emancipation grill at exit.
2. Picking up the blue-only portal gun does NOT trigger "Lab Rat" — that achievement fires in chamber_11 on the fully powered dual device.
3. Goal: use the blue portal gun (acquired mid-chamber) to fire a blue portal and return to the entry ledge; the chamberlock door opens automatically.

## Sequential gates

| Gate ID | Name | Type | Description | Missable | One-way | Sources |
|---|---|---|---|---|---|---|
| chamber_02-gate-01 | Observation window overview | nav | Entry is a ledge behind a window overlooking the whole chamber; a portal gun rotates on a central stand below, auto-firing portals. | no | yes | [Confirmed: 2] |
| chamber_02-gate-02 | Stairwell auto-portal | nav | Descending the stairway, a static portal appears; passing through lands the player on the opposite ledge. | Camera (yes) | partial | [Confirmed: 2] |
| chamber_02-gate-03 | Portal gun pickup (blue-only) | story | Walking onto the rotating stand grants the single-portal (blue) device; a permanent orange portal remains fixed on the ledge. | no | no | [Confirmed: 2] |
| chamber_02-gate-04 | Radio on holed wall | collectible | The radio sits on the wall section with a hole; reachable by a ceiling portal above it. | Radio (yes) | no | [Confirmed: 2] |
| chamber_02-gate-05 | First player-made portal | puzzle | With the gun, fire a blue portal to a reachable wall to return to the ledge; the chamberlock door is now open. | no | no | [Confirmed: 2] |
| chamber_02-gate-06 | Three detachable cameras | collectible | Cameras above the main window, at the end of the stairway, and in the entranceway. | Cameras ×3 (yes) | partial | [Confirmed: 2] |
| chamber_02-gate-07 | Exit chamberlock elevator | exit | Elevator to chamber_03. | no | yes | [Confirmed: 2] |

**Checkpoint:** Chamber-entry autosave on map load. Note: the blue-only gun acquired here is NOT the "Lab Rat" trigger — that fires on the fully powered dual device in chamber_11.

_source: deep-research handoff 2026-06-02 · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 0 · category: mainline · spoiler: none_

## Sources

- StrategyWiki Portal walkthrough: https://strategywiki.org/wiki/Portal/Walkthrough
- ThePortalWiki: https://theportalwiki.com/wiki/Portal_Test_Chamber_02
- Steam Community Camera Shy guide: https://steamcommunity.com/sharedfiles/filedetails/?id=1915501465
