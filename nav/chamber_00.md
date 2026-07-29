# Portal -- Nav: Test Chamber 00

**status:** research-integrated
**last_reconciled:** 2026-06-02
**research_run:** P2 ingested 2026-06-02 (portal_p2.result.md)

**Zone:** `chamber_00` · **Segment:** Pre-gun tutorial · **Spoiler tier:** none

## Entry

From game start (entry vault). Autosave on map load (`testchmb_a_00`, shared with chamber_01). No portal gun in this chamber.

## Exit

To `chamber_01` via chamberlock elevator (one-way, chapter-bound).

## Outgoing edges

- `(chamber_00, chamber_01)` -- story-gate (elevator), pass button/cube test

## Entry tips

1. No portal gun here -- all interactions use the cube and button only.
2. **Radio** on the table in the Relaxation Vault is collectible but grants no achievement on a first playthrough (Transmission Received requires a full completion first).
3. Goal: place the Weighted Storage Cube on the large round floor button to open the exit door.

## Sequential gates

| Gate ID | Name | Type | Description | Missable | One-way | Sources |
|---|---|---|---|---|---|---|
| chamber_00-gate-01 | Relaxation Vault wake-up | story | Player wakes inside a glass-walled vault resembling a small bedroom; a radio sits on the table playing music; a countdown timer is mounted above the future portal location. | Radio (yes) | no | [Confirmed: 2] walkthrough+wiki |
| chamber_00-gate-02 | Vault exit portal | nav | After the countdown a static portal opens in the vault wall; stepping through deposits the player outside, facing the vault exterior. | no | yes | [Confirmed: 2] |
| chamber_00-gate-03 | Vital Apparatus Vent (cube drop) | puzzle | Approaching the main room triggers a Weighted Storage Cube to drop from a ceiling dispenser. | no | no | [Confirmed: 2] |
| chamber_00-gate-04 | Heavy Duty Super-Colliding Super Button | puzzle | A large round floor button; placing the cube on it opens the exit door. | no | no | [Confirmed: 2] |
| chamber_00-gate-05 | Material Emancipation Grill | hazard | The incandescent particle field across the exit; vaporizes carried objects (cube cannot pass). | no | yes | [Confirmed: 2] |
| chamber_00-gate-06 | Exit chamberlock elevator | exit | Elevator to chamber_01. | no | yes | [Confirmed: 2] |

**Checkpoint:** Chamber-entry autosave at map load. No mid-chamber autosave observed. Manual quicksave not needed here (no lethal hazards).

_source: deep-research handoff 2026-06-02 · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 0 · category: mainline · spoiler: none_

## Sources

- StrategyWiki Portal walkthrough: https://strategywiki.org/wiki/Portal/Walkthrough
- ThePortalWiki: https://theportalwiki.com/wiki/Portal_Test_Chamber_00
- Thonky Portal walkthrough: https://www.thonky.com/portal-walkthrough/
