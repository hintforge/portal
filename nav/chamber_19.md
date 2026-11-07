# Portal -- Nav: Test Chamber 19

**status:** research-integrated
**last_reconciled:** 2026-11-06
**research_run:** P2 ingested 2026-06-02 (portal_p2.result.md)

**Zone:** `chamber_19` · **Segment:** Dual-portal segment · **Spoiler tier:** story

## Entry

From `chamber_18` via chamberlock elevator. Autosave on map load (`testchmb_a_15`, which also holds the first stretch of the escape, Escape (Part 1)).
_source: 2026-11-06 https://theportalwiki.com/wiki/List_of_Portal_chambers, https://wiki.sourceruns.org/Portal-Maps.html · capture: browser_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 3 · category: mainline · spoiler: story_ [Confirmed: 2]

A brief "Loading" message comes later, before the five-piston area.
_source: 2026-11-06 https://www.thonky.com/portal-walkthrough/test-chamber-19 · capture: browser_fetch · confidence: medium · enemy-tier: 0 · puzzle-tier: 3 · category: mainline · spoiler: story_ [Single source -- verify · class:walkthrough]

## Exit

To `escape_seq` via the oven escape — **permanent point of no return**. No return to test chambers after this point.

## Outgoing edges

- `(chamber_19, escape_seq)` -- permanent (Partygoer); escape the fire pit

## Entry tips

1. **Three cameras** (first room, annex, end of the platform hallway) and **one radio** (in the fire pit) — the cameras are all collected before the fire pit; fetch the radio with a portal once you are on the platform above the pit.
2. Much later, after the fire pit, the side rooms, the fans and the cube tube, you land back in the Test Chamber 01 room, where the chamberlock **malfunctions** and forces a drop down the elevator shaft — this is scripted, not a puzzle failure.
3. After gate-07, you leave the test chambers permanently. Collect everything before reaching the oven.

## Sequential gates

| Gate ID | Name | Type | Description | Missable | One-way | Sources |
|---|---|---|---|---|---|---|
| chamber_19-gate-01 | Pellet launcher + two angled platforms | puzzle | The first room has a pellet launcher, a receiver, and two platforms angled at 45°; routing the pellet into the receiver starts the moving platforms. The permanent (green) pellet is not in this room: it is in the hallway you ride through on the platform. | Camera (yes) | no | [Single source -- verify · class:walkthrough] |
| chamber_19-gate-02 | "Promised cake" announcement | story | GLaDOS frames the final test and the equipment recovery annex ("both hands empty before any cake"). | no | no | [Confirmed: 2] |
| chamber_19-gate-03 | Three cameras | collectible | Cameras: right wall of the first room; above the small button in the annex; at the end of the hallway with the permanent pellet. | Cameras ×3 (yes) | partial | [Confirmed: 2] |
| chamber_19-gate-04 | Radio in the fire pit | collectible | Radio is in the giant incinerator (the fire pit), against a wall; spot it from the balcony above, then put a portal near you and another behind the radio and grab it partway through the portal. Carry it on through the side rooms; its signal spot is the center of the side office after the two big fans. | Radio (yes) | no | [Confirmed: 2] |
| chamber_19-gate-05 | Annex button | nav | Ride the moving platform to the side room (annex) with a button: it opens a nearby door only briefly, so put a portal on the wall near the button, press it, put the other portal on the wall behind the door that opened, and step through onto the platform as it passes. | no | yes | [Confirmed: 2] |
| chamber_19-gate-06 | Fire pit / incinerator approach | hazard | The moving platform carries you on from the hallway (permanent green pellet, a wall in its path) straight to the fire pit (the "party escort" oven). | no | yes | [Confirmed: 2] |
| chamber_19-gate-07 | Escape the oven (Partygoer decision) | story | Instead of riding into the fire, portal up to the platform above the oven — earns "Partygoer — Make the correct party escort submission position decision." Begins the escape. | Achievement (yes) | yes | [Confirmed: 2] |
| chamber_19-gate-08 | Transition to escape_seq | exit | After escaping the pit, go on through the side rooms (collapsing stairs, locked mesh door), the two big fans, the poison-pit walkway and the cube tube, which drops you into the Test Chamber 01 room (stand on the big button; the chamberlock malfunctions and you jump down the elevator shaft); the maintenance areas of the escape continue from there. | no | yes | [Confirmed: 2] |

**Checkpoint:** Chamber-entry autosave. The last camera is at the end of the platform hallway, before the fire pit; none after. Gate-07 is the point of no return to the test chambers. "Partygoer" is unavoidable if you survive the oven section. Permanent green pellet (distinctive: green glow) is unique to this chamber.

> **Cross-system dependency** -- see `dependencies.md` PON-002: Gate-07 is the Camera Shy PoNR — no cameras exist in escape_seq; collect all chamber_19 cameras (gates 01-03) before the fire pit (gate-06).

_source: deep-research handoff 2026-06-02 · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 3 · category: mainline · spoiler: story_
_source: 2026-11-06 (entry tip 1, chamber_19-gate-04) https://strategywiki.org/wiki/Portal/Chamber_19, https://www.thonky.com/portal-walkthrough/transmission-received · capture: browser_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 3 · category: mainline · spoiler: story_ [Confirmed: 2]
_source: 2026-11-06 (entry tip 2, chamber_19-gate-05, chamber_19-gate-06, chamber_19-gate-08, edge line) https://strategywiki.org/wiki/Portal/Chamber_19, https://www.thonky.com/portal-walkthrough/test-chamber-19 · capture: browser_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 3 · category: mainline · spoiler: story_ [Confirmed: 2]
_source: 2026-11-06 (chamber_19-gate-01, checkpoint paragraph, cross-system callout) https://strategywiki.org/wiki/Portal/Chamber_19 · capture: browser_fetch · confidence: medium · enemy-tier: 0 · puzzle-tier: 3 · category: mainline · spoiler: story_ [Single source -- verify · class:walkthrough]

## Sources

- StrategyWiki Portal walkthrough: https://strategywiki.org/wiki/Portal/Walkthrough
- ThePortalWiki: https://theportalwiki.com/wiki/Portal_Test_Chamber_19
