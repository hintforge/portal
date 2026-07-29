# Portal -- Architecture

**status:** research-integrated
**last_reconciled:** 2026-06-02
**research_run:** P1 ingested 2026-06-02 · P2 ingested 2026-06-02 (portal_p2.result.md, deep-research handoff)

Cross-zone structural primitives. The persona reads this file for all cross-zone reasoning -- lookahead warnings (Rule 2), backtrack queries (Rule 3), reachability checks (Rule 4), locks-and-keys notifications (Rule 5). Per-zone gate lists live in `nav/<zone>.md` and reference this file's graph by edge ID. Drift between this file and per-zone files is a bug; run a consistency pass after each ingestion.

## Hintforge manifest

```
corpus-core-version: 5
game-version: "latest"
game-version-platform: "PC / Steam"
game-version-as-of: 2026-06-02
vector-extensions: puzzles, nav
```

## Vector extensions

- `puzzles/` -- discrete puzzle files with hint ladders, indexed by `puzzles/index.md`
- `nav/` -- routing only. `index.md` (rules) + `architecture.md` (zone graph, optional content, support topology, locks-and-keys) + per-zone gate-list files.

## Zone Graph

**Game-type label:** on-rails -- CONFIRMED (P1)
**Localization-mechanism class:** landmark -- CONFIRMED (P1; no map UI)
**Entry node:** chamber_00
**Hub nodes:** none
**Source-language set:** English (Valve, USA); top player-region languages: English, German, Russian

**Numbering note (P1 correction):** In-game chamber plaques use **0-indexed** display numbering -- Test Chamber **00** through Test Chamber 19, 20 navigable areas plus the unnumbered Escape Sequence. The earlier scaffold omitted Chamber 00 and implicitly began at 01; corrected here. (BSP map files group two chambers per file -- `testchmb_a_00` holds Chambers 00-01, etc.; the escape spans `escape_00/01/02` plus GLaDOS' chamber.)
_source: deep-research handoff 2026-06-02 · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 0 · category: mainline · spoiler: none_

**Stage 0 rationale (confirmed):**
- `on-rails`: strictly linear sequence of numbered test chambers; the player cannot skip, reorder, or revisit chambers. Every Emancipation Grill + elevator transition is a one-way chapter gate.
- `landmark`: no in-game map UI. Player position is identifiable by chamber-number plaques at entry, distinctive environmental features (Companion Cube in 17, turret course in 16+, energy-pellet equipment in 06+), and chamber-specific GLaDOS audio.

**Nodes:**

| zone-id | Canonical name | Introduces / notable |
|---|---|---|
| chamber_00 | Test Chamber 00 | Relaxation Vault; button, Weighted Storage Cube, Vital Apparatus Vent, Emancipation Grill. Only chamber with no portals. |
| chamber_01 | Test Chamber 01 | Advanced button/cube test; portals automated (no gun yet) |
| chamber_02 | Test Chamber 02 | Blue-only ASHPD acquired |
| chamber_03 | Test Chamber 03 | Cube/button across gaps |
| chamber_04 | Test Chamber 04 | Cube-in-pit, portals required |
| chamber_05 | Test Chamber 05 | Two-cube, two-button room |
| chamber_06 | Test Chamber 06 | High Energy Pellet introduced; non-portalable brown walls introduced |
| chamber_07 | Test Chamber 07 | Unstationary Scaffold introduced |
| chamber_08 | Test Chamber 08 | Acid/goo introduced |
| chamber_09 | Test Chamber 09 | Emancipation Grill used as a puzzle element |
| chamber_10 | Test Chamber 10 | Momentum/fling lessons begin |
| chamber_11 | Test Chamber 11 | Dual-portal ASHPD acquired ("Lab Rat"); GLaDOS "speedy thing" line |
| chamber_12 | Test Chamber 12 | Combined puzzle |
| chamber_13 | Test Chamber 13 | First "review" chamber; first Advanced/Challenge variant |
| chamber_14 | Test Chamber 14 | Challenge chamber; finishable from the first room via a fling |
| chamber_15 | Test Chamber 15 | Advanced flinging / double-fling |
| chamber_16 | Test Chamber 16 | Sentry Turrets introduced ("Friendly Fire") |
| chamber_17 | Test Chamber 17 | Weighted Companion Cube; ends at Incinerator Room ("Fratricide") |
| chamber_18 | Test Chamber 18 | Turrets + flinging |
| chamber_19 | Test Chamber 19 | Final test; fire pit / Incinerator Room ("Partygoer") |
| escape_seq | Escape Sequence / Surface Finale | Behind-the-scenes maintenance areas + GLaDOS boss fight ("Heartbreaker") |

**Edges (all transitions one-way story-gates):**

| From | To | Type | Direction | Condition | Point of no return | Notes |
|---|---|---|---|---|---|---|
| chamber_00 | chamber_01 | story-gate (elevator) | one-way src→tgt | Clear button/cube test | chapter-bound | No backtracking once elevator boards |
| chamber_01 | chamber_02 | story-gate (elevator + grill) | one-way src→tgt | Solve chamber | chapter-bound | |
| chamber_02 | chamber_03 | story-gate (elevator + grill) | one-way src→tgt | Solve chamber | chapter-bound | |
| chamber_03 | chamber_04 | story-gate (elevator + grill) | one-way src→tgt | Solve chamber | chapter-bound | |
| chamber_04 | chamber_05 | story-gate (elevator + grill) | one-way src→tgt | Solve chamber | chapter-bound | |
| chamber_05 | chamber_06 | story-gate (elevator + grill) | one-way src→tgt | Solve chamber | chapter-bound | |
| chamber_06 | chamber_07 | story-gate (elevator + grill) | one-way src→tgt | Solve chamber | chapter-bound | |
| chamber_07 | chamber_08 | story-gate (elevator + grill) | one-way src→tgt | Solve chamber | chapter-bound | |
| chamber_08 | chamber_09 | story-gate (elevator + grill) | one-way src→tgt | Solve chamber | chapter-bound | |
| chamber_09 | chamber_10 | story-gate (elevator + grill) | one-way src→tgt | Solve chamber | chapter-bound | |
| chamber_10 | chamber_11 | story-gate (elevator + grill) | one-way src→tgt | Solve chamber | chapter-bound | |
| chamber_11 | chamber_12 | story-gate (elevator + grill) | one-way src→tgt | Solve chamber; dual-portal ASHPD acquired here | chapter-bound | Dual-portal capability unlocked |
| chamber_12 | chamber_13 | story-gate (elevator + grill) | one-way src→tgt | Solve chamber | chapter-bound | |
| chamber_13 | chamber_14 | story-gate (elevator + grill) | one-way src→tgt | Solve chamber | chapter-bound | |
| chamber_14 | chamber_15 | story-gate (elevator + grill) | one-way src→tgt | Solve chamber | chapter-bound | |
| chamber_15 | chamber_16 | story-gate (elevator + grill) | one-way src→tgt | Solve chamber | chapter-bound | |
| chamber_16 | chamber_17 | story-gate (elevator + grill) | one-way src→tgt | Solve chamber | chapter-bound | Last-but-one turret chamber; Friendly Fire still earnable in 18 |
| chamber_17 | chamber_18 | story-gate (elevator, post-Incinerator) | one-way src→tgt | Incinerate Companion Cube to open exit | permanent (within run) | Cube destruction irreversible (Fratricide) |
| chamber_18 | chamber_19 | story-gate (elevator + grill) | one-way src→tgt | Solve chamber | chapter-bound | Last turret chamber (Friendly Fire PoNR) |
| chamber_19 | escape_seq | fall into Incinerator Room → fling out | one-way src→tgt | Survive the fire-pit fling | permanent | Partygoer; no return to test chambers |
| escape_seq | [end / credits] | implosion after GLaDOS defeat | one-way src→tgt | Destroy all 4 cores | permanent | Heartbreaker; game ends |

_source: deep-research handoff 2026-06-02 · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 0 · category: mainline · spoiler: progression (gun/turret rows late-game where noted)_

- **Backtracking: NO chamber allows return to a prior chamber.** Each Emancipation Grill + elevator transition is a hard chapter boundary by design; the grill also resets the player's active portals on pass-through.
- **Three permanent points of no return:** Chamber 17→18 (cube incineration), Chamber 19→Escape (fire-pit fling), Escape→End (post-GLaDOS implosion).

## DLC list (names only -- out of P1 scope)

Portal: Still Alive (Xbox 360, +chambers); Portal with RTX (2022 ray-tracing remaster); Portal: Companion Collection (Switch port, 2022). No DLC facts ingested in P1.

## Chapter ↔ Zone Mapping

Portal has no named chapters; the narrative is continuous. For tracking:

| Segment | Zones | Notes |
|---|---|---|
| Pre-gun tutorial | chamber_00 -- chamber_01 | No player-controlled portals; automated portals only |
| Blue-portal segment | chamber_02 -- chamber_10 | Blue-only ASHPD from Chamber 02; single-portal puzzles, fling lessons begin Ch10 |
| Dual-portal segment | chamber_11 -- chamber_19 | Orange portal acquired Chamber 11; dual portals enable the fling mechanic |
| Escape Sequence | escape_seq | Post-Chamber-19; no more test chambers; GLaDOS boss fight + ending |

## Optional Content

> **Cross-system dependency** -- see `dependencies.md` SEQ-002: Advanced Chambers and Portal Challenges both require game completion (Heartbreaker) to unlock; see achievements.md for Cupcake/Fruitcake/Vanilla Crazy Cake and Basic/Rocket/Aperture Science.

| Name | Count | Unlock / access | Window & missability | Notes |
|---|---|---|---|---|
| Security cameras | 33 (CONFIRMED) | Detach by placing a linked portal on the wall behind the camera | **Run-missable** -- Camera Shy requires all 33 in a single no-load run; counter resets on level skip / reload / death-restart and at game end. Latest camera in Chamber 19; none post-19. | Present in Chambers 02,03,04,05,10,11,13,15,16,17,18,19. Full per-chamber locations in `items/collectibles.md`. |
| Hidden radios | 26 (CONFIRMED) | Carry each radio to its signal spot (light turns green) | Appear in Chambers 00-19 + escape. **Only count after completing the game once** (Transmission Received). Chamber 00's radio is the only one present/functional on a first run but still grants no achievement progress pre-completion. | Added to existing chambers, not a separate area. Full locations in `items/collectibles.md`. |
| Advanced Chambers | 6 | Complete the main game | Post-game menu; always-available once unlocked | Advanced variants of Chambers 13-18. Feed Cupcake/Fruitcake/Vanilla Crazy Cake. |
| Portal Challenges | 18 tasks | Complete the main game | Post-game menu; always-available once unlocked | Chambers 13-18 each have Challenge mode (least portals / least steps / least time = 3 tasks × 6 chambers = 18). Feed Basic/Rocket/Aperture Science. |

_source: deep-research handoff 2026-06-02 · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 0 · category: easter-egg · spoiler: none_

## Support Topology

### Save stations

Portal uses automatic checkpoints only -- no manual save stations.

**Baseline: chamber-entry autosave (confirmed).** Portal runs on the Source 2007 engine. Per the Source engine source code (`engine/host_saverestore.cpp`), the console variable `sv_autosave` defaults to `"1"` — verbatim: *"Set to 1 to autosave game on level transition. Does not affect autosave triggers."* Because each Portal chamber (or chamber pair) is a separate `.bsp` map, the engine writes an autosave whenever a new map loads — i.e. effectively at chamber entry / elevator transition. This is the player's reliable recovery point on death. `[Confirmed: engine source + Valve Developer Community]`

**No systematic mid-chamber autosaves.** The engine performs no timed/periodic in-level autosave. Mid-chamber autosaves exist ONLY where a level designer hand-placed a `trigger_autosave` (or `logic_autosave`) brush entity; per the VDC, *"trigger_autosave… triggers an auto-save when the player enters its volume"* and fires once. These are not systematic across Portal's chambers, and no published per-chamber enumeration exists. Treat mid-chamber autosave points as `[Hypothesis — unverified]` per chamber. `[Confirmed: VDC + engine source]`

**On death:** Portal automatically reloads the most recent autosave (normally the chamber start). Manual quicksave (default **F6**) is strongly advised before hazardous sections, especially chambers 08, 09, 11, 16, 17, 18, 19, and the escape. `[Confirmed: walkthrough]`

**Map pairing (routing-relevant).** Several chambers share a single `.bsp` map file; the autosave for the second chamber in a pair fires on the inter-chamber elevator transition, not a fresh map load:

| Map file | Chambers |
|---|---|
| `testchmb_a_00` | 00 – 01 |
| `testchmb_a_01` | 02 – 03 |
| `testchmb_a_02` | 04 – 05 |
| `testchmb_a_03` | 06 – 07 |
| `testchmb_a_04` | 08 – 09 |
| `testchmb_a_05` | 10 – 11 |
| `testchmb_a_06` | 12 – 13 |
| `testchmb_a_07` | 14 – 15 |
| `testchmb_a_08` | 16 – 17 |
| `testchmb_a_09` | 18 – 19 |
| `testchmb_a_15` (+ escape_00) | chamber_19 → escape start (seamless, no load screen) |
| `escape_00`, `escape_01`, `escape_02` | Escape Sequence (three separate map loads → three autosaves) |

`[Confirmed: Speed Demos Archive / speedrun map list]`

_source: deep-research handoff 2026-06-02 · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 0 · category: mainline · spoiler: none_

### Fast-travel network

None -- no fast-travel in this game. All progression is linear and one-way.

### Hub access

None -- no hub structure. Portal is strictly linear (on-rails).

## Locks and Keys

| Lock location | Key required | Key source | Visible before key? | Notes |
|---|---|---|---|---|
| Orange portal apertures (all chambers before 11) | Orange portal-gun component (dual-portal ASHPD) | chamber_11 (acquired mid-chamber) | no | Chambers 00-01 have no player gun at all; 02-10 are blue-only. |
| Chamber 17 exit (Incinerator Room) | Incinerate the Weighted Companion Cube | chamber_17 (in-chamber action) | yes | Required to advance; triggers Fratricide. Permanent within the run. |
| Advanced Chambers (menu) | Complete the main game | escape_seq completion (Heartbreaker) | no | Unlocks all 6 Advanced variants. |
| Portal Challenges (menu) | Complete the main game | escape_seq completion (Heartbreaker) | no | Unlocks all 18 Challenge tasks. |
| Radio achievement progress (Transmission Received) | One full completion | escape_seq completion | no | Radios are present earlier but grant no achievement progress until the game is beaten once. |
| chamber_00 exit door | Cube on the Heavy Duty Super-Colliding Super Button | in-chamber | yes | First cube-on-button door. [Confirmed: 2] |
| Every chamberlock exit (all zones) | Pass the Material Emancipation Grill (drops carried objects/portals) | in-chamber | yes | One-way state gate; cube/objects cannot be carried through. [Confirmed: 2] |
| chamber_01 exit | Cube on button + correct portal-cycle timing | in-chamber | yes | Sequence lock via the cycling static portal. [Confirmed: 2] |
| chamber_02 chamberlock door | Pick up the blue portal gun | in-chamber | yes | Door opens on gun pickup. [Confirmed: 2] |
| chamber_04 exit door | Cube on the floor button | in-chamber | yes | [Confirmed: 2] |
| chamber_05 exit door | Two cubes on two buttons | in-chamber | yes | Both buttons must be held simultaneously. [Confirmed: 2] |
| chamber_06 victory lift | High Energy Pellet in the receiver | in-chamber | yes | Pellet powers the lift. [Confirmed: 2] |
| chamber_07 / chamber_08 moving platform | High Energy Pellet in the receiver | in-chamber | yes | Pellet starts the platform. [Confirmed: 2] |
| chamber_09 exit door | Cube on button (across emancipation grid) | in-chamber | yes | [Confirmed: 2] |
| chamber_11 dual-gun pedestal access | High Energy Pellet powers the moving platform | in-chamber | yes | Platform carries player to the dual gun. [Confirmed: 2] |
| chamber_12 fourth-level door | Cube on third-level button | in-chamber | yes | Button on one level controls a door on another. [Confirmed: 2] |
| chamber_13 exit door | Two buttons held (cube on one + route on the other) + pellet platform | in-chamber | yes | Two-step lock. [Confirmed: 2] |
| chamber_14 corridor door | Cube on button | in-chamber | yes | Opens the sludge-room corridor. [Confirmed: 2] |
| chamber_14 victory lift | Pellet routed into receiver | in-chamber | yes | [Confirmed: 2] |
| chamber_15 exit lift | Two side-room buttons + pellet in receiver | in-chamber | yes | Buttons open doors; pellet lowers the lift. [Confirmed: 2] |
| chamber_16 button-room door | Cube on button (turrets disabled) | in-chamber | yes | Turrets must be neutralized to survive placement. [Confirmed: 2] |
| chamber_17 platform crossings | Three pellets into three receivers | in-chamber | yes | Raises the three platforms. [Confirmed: 2] |
| chamber_17 twin-door pellet room | Two buttons (cube + player) | in-chamber | yes | Opens both doors to the receiver. [Confirmed: 2] |
| chamber_18 turret-room door (Part 1→2) | Cube on button | in-chamber | yes | [Confirmed: 2] |
| chamber_19 chamberlock (malfunctioning) | Central button + manual drop-down (door malfunctions) | in-chamber | yes | Forces the escape route. [Confirmed: 2] |
| escape_seq GLaDOS defeat | All four personality cores incinerated (rocket-redirect) | in-zone | yes | Rockets dislodge cores; incinerator destroys them. [Confirmed: 2] |

_source: deep-research handoff 2026-06-02 · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 0 · category: mainline · spoiler: progression_

> Per-chamber gate lists are in `nav/<zone>.md`. Localization toolkit is in `nav/localization.md`. Both populated via P2 ingestion (2026-06-02).
