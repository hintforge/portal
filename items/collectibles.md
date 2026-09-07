# Portal -- Collectibles (Cameras & Radios)

**status:** research-integrated
**last_reconciled:** 2026-06-02
**research_run:** P1 ingested 2026-06-02 (portal_p1.result.md)

The two finite collectible sets in Portal. Each row is a set-member claim feeding a collection achievement; the aggregated achievement entries live in `achievements.md`, and the missable summary in `sections/missables.md`.

- **Security cameras (33):** `missable: yes` -- Camera Shy needs all 33 detached in a single no-load run.
- **Hidden radios (26):** present from a first run but only grant Transmission Received progress after one full completion.

Routing follows the "NEVER left/right -- anchor to features" rule (`nav/index.md`); descriptions are quoted from the research source and use feature anchors.

_source: deep-research handoff 2026-06-02 · capture: web_fetch · confidence: high (counts confirmed across StrategyWiki, Steam community guides, ThePortalWiki) · enemy-tier: 0 · puzzle-tier: 0 · category: easter-egg_

---

## Security cameras (33 -- `ach: camera_shy` · trigger_type: collection · achievement-hidden: no)

Detach a camera by placing a linked portal on the wall **behind** it. Present in 12 chambers; none after Chamber 19.

| # | Chamber | Location (feature-anchored) | spoiler |
|---|---|---|---|
| 1 | chamber_02 | At the entrance, accessible after you acquire the gun | progression |
| 2 | chamber_02 | End of the entry hall | progression |
| 3 | chamber_02 | Above the observation window over the main room | progression |
| 4 | chamber_03 | Beside the Chamber 03 plaque | progression |
| 5 | chamber_03 | Across the first gap | progression |
| 6 | chamber_03 | Beyond the second gap near the exit | progression |
| 7 | chamber_04 | Above the button near the entrance | progression |
| 8 | chamber_04 | Opposite wall near the exit | progression |
| 9 | chamber_05 | Behind a wall whose portal won't connect until you enter the main room | progression |
| 10 | chamber_05 | Near the two-button exit | progression |
| 11 | chamber_05 | In the room beyond the door | progression |
| 12 | chamber_10 | On the wall by the first staircase you fling onto | progression |
| 13 | chamber_11 | Above the archway in the starting observation room | progression |
| 14 | chamber_13 | Above the elevator hallway in the first cube/button room | progression |
| 15 | chamber_13 | Near the highest button platform in the main room | progression |
| 16 | chamber_13 | In the exit room before the elevator | progression |
| 17 | chamber_15 | By the Chamber 15 plaque | progression |
| 18 | chamber_15 | Across the Emancipation Grill above the doorway | progression |
| 19 | chamber_15 | Around the corner in the ball/catcher room | progression |
| 20 | chamber_15 | In the side room of the next area | progression |
| 21 | chamber_15 | At the end of the moving-platform/acid hallway | progression |
| 22 | chamber_16 | In front of you as the door opens | late-game |
| 23 | chamber_16 | Entering the next room past the first turret | late-game |
| 24 | chamber_16 | At the top of the stairs by the red-X turret | late-game |
| 25 | chamber_16 | On the back wall of the second-section alcove | late-game |
| 26 | chamber_16 | In the first of the two final rooms before the second grating (easy to miss) | late-game |
| 27 | chamber_17 | At the end of the second narrow hallway into the main hall | late-game |
| 28 | chamber_17 | In the main hall above the doorway to the ball-catcher side room | late-game |
| 29 | chamber_18 | On the wall near the observation glass in the main turret room | late-game |
| 30 | chamber_18 | Down the hallway before the platforming section | late-game |
| 31 | chamber_19 | To your right entering the first room | late-game |
| 32 | chamber_19 | In the button alcove for the blast door (act fast -- the platform moves quickly) | late-game |
| 33 | chamber_19 | At the end of the first long track segment with the green pellet | late-game |

_source: deep-research handoff 2026-06-02 · capture: web_fetch · confidence: medium (per-camera positions: community-wiki + forum, ≤2 sources) · enemy-tier: 0 · puzzle-tier: 0 · category: easter-egg · spoiler: see per-row · missable: yes · ach: camera_shy · achievement-hidden: no · trigger_type: collection_

> see achievements.md for the Camera Shy entry and the run-state reset rules.
> see sections/missables.md for the run-missable summary.

---

## Hidden radios (26 -- `ach: transmission_received` · trigger_type: collection · achievement-hidden: yes)

> **Cross-system dependency** -- see `dependencies.md` SEQ-001: Collecting radios grants no Transmission Received progress until the game is beaten once; do a dedicated post-completion pass.

Carry each radio to its signal spot; the light turns green when placed correctly. Radios are added to existing chambers (not a separate area) and only grant achievement progress after the game is completed once.

| # | Chamber | Location / note (feature-anchored) |
|---|---|---|
| 1 | chamber_00 | On a table in the corner of the starting room; carry it to the special spot near the button. The only radio present on a first playthrough. |
| 2 | chamber_01 | Present in chamber |
| 3 | chamber_02 | Present in chamber |
| 4 | chamber_03 | Present in chamber |
| 5 | chamber_04 | Present in chamber |
| 6 | chamber_05 | **Pull it through a portal -- do NOT walk it through the exit door or you'll lose access.** |
| 7 | chamber_06 | Above the pellet launcher, corner nearest the entrance |
| 8 | chamber_07 | Present in chamber |
| 9 | chamber_08 | Present in chamber |
| 10 | chamber_09 | Present in chamber |
| 11 | chamber_10 | Present in chamber |
| 12 | chamber_11 | Present in chamber |
| 13 | chamber_12 | Present in chamber |
| 14 | chamber_13 | Present in chamber |
| 15 | chamber_14 | Present in chamber |
| 16 | chamber_15 | First of two radios in this chamber |
| 17 | chamber_15 | Second of two radios in this chamber |
| 18 | chamber_16 | Present in chamber |
| 19 | chamber_17 | Present in chamber |
| 20 | chamber_18 | First of three radios in this chamber |
| 21 | chamber_18 | Second of three radios in this chamber |
| 22 | chamber_18 | Third of three radios in this chamber |
| 23 | chamber_19 | Present in chamber |
| 24 | escape_seq | In the escape maps (escape_00/01/02) |
| 25 | escape_seq | In the escape maps (escape_00/01/02) |
| 26 | escape_seq | In the final large turret room with the muddy trench; bring it to the two large electrical engines/generators near the top |

_source: deep-research handoff 2026-06-02 · capture: web_fetch · confidence: medium (per-radio positions: community-wiki, ≤2 sources) · enemy-tier: 0 · puzzle-tier: 0 · category: easter-egg · spoiler: none (escape rows: late-game by location) · ach: transmission_received · achievement-hidden: yes · trigger_type: collection_

> see achievements.md for the Transmission Received entry (hidden; post-completion gating).

## Sources

- StrategyWiki Portal; Steam Community camera/radio guides; ThePortalWiki.com (community-wiki / forum)
