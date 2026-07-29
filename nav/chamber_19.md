# Portal -- Nav: Test Chamber 19

**status:** research-integrated
**last_reconciled:** 2026-06-02
**research_run:** P2 ingested 2026-06-02 (portal_p2.result.md)

**Zone:** `chamber_19` · **Segment:** Dual-portal segment · **Spoiler tier:** story

## Entry

From `chamber_18` via chamberlock elevator. Autosave on inter-chamber elevator transition (within `testchmb_a_09`, shared with chamber_18). Chamber_19 continues seamlessly into the first escape segment (no loading screen).

## Exit

To `escape_seq` via the oven escape — **permanent point of no return**. No return to test chambers after this point.

## Outgoing edges

- `(chamber_19, escape_seq)` -- permanent (Partygoer); survive the fire-pit fling

## Entry tips

1. **Three cameras** and **one radio** — all collectible in the first room / annex area before the malfunctioning chamberlock.
2. The chamberlock at gate-05 **malfunctions** and forces a drop — this is scripted, not a puzzle failure.
3. After gate-07, you leave the test chambers permanently. Collect everything before reaching the oven.

## Sequential gates

| Gate ID | Name | Type | Description | Missable | One-way | Sources |
|---|---|---|---|---|---|---|
| chamber_19-gate-01 | Pellet launcher + two angled platforms | puzzle | The first room has a pellet launcher, a receiver, and two platforms angled at 45°; a permanent (green) pellet exists. | Camera (yes) | no | [Confirmed: 2] |
| chamber_19-gate-02 | "Promised cake" announcement | story | GLaDOS frames the final test and the equipment recovery annex ("both hands empty before any cake"). | no | no | [Confirmed: 2] |
| chamber_19-gate-03 | Three cameras | collectible | Cameras: right wall of the first room; above the small button in the annex; at the end of the hallway with the permanent pellet. | Cameras ×3 (yes) | partial | [Confirmed: 2] |
| chamber_19-gate-04 | Radio in first room | collectible | Radio is on the right wall of the first room area. | Radio (yes) | no | [Confirmed: 2] |
| chamber_19-gate-05 | Annex button + malfunctioning chamberlock | nav | Stand on the central button, portal through the opened door; the chamberlock malfunctions, forcing a drop down. | no | yes | [Confirmed: 2] |
| chamber_19-gate-06 | Fire pit / incinerator approach | hazard | The conveyor/track leads toward a fire pit (the "party escort" oven). | no | yes | [Confirmed: 2] |
| chamber_19-gate-07 | Escape the oven (Partygoer decision) | story | Instead of riding into the fire, portal up to the platform above the oven — earns "Partygoer — Make the correct party escort submission position decision." Begins the escape. | Achievement (yes) | yes | [Confirmed: 2] |
| chamber_19-gate-08 | Transition to escape_seq | exit | After escaping the platform, proceed into the maintenance areas (escape sequence). | no | yes | [Confirmed: 2] |

**Checkpoint:** Chamber-entry autosave. No cameras post-gate-05. Gate-07 is the point of no return to the test chambers. "Partygoer" is unavoidable if you survive the oven section. Permanent green pellet (distinctive: green glow) is unique to this chamber.

> **Cross-system dependency** -- see `dependencies.md` PON-002: Gate-07 is the Camera Shy PoNR — no cameras exist in escape_seq; collect all chamber_19 cameras (gates 01-03) before gate-05.

_source: deep-research handoff 2026-06-02 · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 3 · category: mainline · spoiler: story_

## Sources

- StrategyWiki Portal walkthrough: https://strategywiki.org/wiki/Portal/Walkthrough
- ThePortalWiki: https://theportalwiki.com/wiki/Portal_Test_Chamber_19
