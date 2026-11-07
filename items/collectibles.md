# Portal -- Collectibles (Cameras & Radios)

**status:** research-integrated
**last_reconciled:** 2026-11-06
**research_run:** P1 ingested 2026-06-02 (portal_p1.result.md)

The two finite sets Portal counts toward achievements: cameras you detach from walls (Camera Shy) and radios you carry to a signal spot (Transmission Received). Each row is a set-member claim feeding a collection achievement; the aggregated achievement entries live in `achievements.md`, and the missable summary in `sections/missables.md`.

- **Security cameras (33):** `missable: yes` -- Camera Shy needs all 33 detached; skipping or replaying a chamber resets the counter, so get every camera the first time through each chamber.
- **Hidden radios (26):** only the Chamber 00 radio exists on a first run; the other 25 appear once the game has been completed, and carrying them to their signal spots earns Transmission Received.

Routing follows the "NEVER left/right -- anchor to features" rule (`nav/index.md`); descriptions are quoted from the research source and use feature anchors.

_source: deep-research handoff 2026-06-02 · capture: web_fetch · confidence: high (counts confirmed across StrategyWiki, Steam community guides, ThePortalWiki) · enemy-tier: 0 · puzzle-tier: 0 · category: easter-egg_
_source: 2026-11-06 (opening paragraph) https://theportalwiki.com/wiki/Radio, https://theportalwiki.com/wiki/Security_Camera, https://strategywiki.org/wiki/Portal/Camera_Shy, https://www.pcgamingwiki.com/wiki/Portal · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 0 · category: easter-egg_ [Confirmed: 3]
_source: 2026-11-06 (Camera Shy bullet) https://strategywiki.org/wiki/Portal/Camera_Shy, https://www.thonky.com/portal-walkthrough/achievements · capture: browser_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 0 · category: easter-egg_ [Confirmed: 2]
_source: 2026-11-06 (hidden radios bullet) https://theportalwiki.com/wiki/Obtaining_Portal_achievements, https://strategywiki.org/wiki/Portal/Transmission_Received, https://www.pcgamingwiki.com/wiki/Portal · capture: browser_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 0 · category: easter-egg_ [Confirmed: 3]

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
| 9 | chamber_05 | Above the doorway next to the chamber number (a camera only falls once both portals exist, so shoot it after the orange portal appears) | progression |
| 10 | chamber_05 | Near the two-button exit | progression |
| 11 | chamber_05 | In the room beyond the door | progression |
| 12 | chamber_10 | The upper left corner of the first room | progression |
| 13 | chamber_11 | Above the archway in the starting observation room | progression |
| 14 | chamber_13 | Above the elevator hallway in the first cube/button room | progression |
| 15 | chamber_13 | On the wall of the main room, to the left of the entrance door as you enter | progression |
| 16 | chamber_13 | In the exit room before the elevator | progression |
| 17 | chamber_15 | On the right wall as you are about to enter the first room | progression |
| 18 | chamber_15 | Across the Emancipation Grill above the doorway | progression |
| 19 | chamber_15 | Above and to the right of the exit lift of the second room | progression |
| 20 | chamber_15 | In the side room of the next area | progression |
| 21 | chamber_15 | Above the entrance in the final room | progression |
| 22 | chamber_16 | In front of you as the door opens | late-game |
| 23 | chamber_16 | Entering the next room past the first turret | late-game |
| 24 | chamber_16 | At the top of the stairs by the red-X turret | late-game |
| 25 | chamber_16 | In the button room, across from the door | late-game |
| 26 | chamber_16 | After the first fence, on the left wall | late-game |
| 27 | chamber_17 | Next to where the second pellet hits the wall | late-game |
| 28 | chamber_17 | In the main hall above the doorway to the ball-catcher side room | late-game |
| 29 | chamber_18 | On the wall near the observation glass in the main turret room | late-game |
| 30 | chamber_18 | On the wall of the entrance of the final room | late-game |
| 31 | chamber_19 | To your right entering the first room | late-game |
| 32 | chamber_19 | In the button alcove for the blast door (act fast -- the platform moves quickly) | late-game |
| 33 | chamber_19 | At the end of the first long track segment with the green pellet | late-game |

_source: deep-research handoff 2026-06-02 · capture: web_fetch · confidence: medium (per-camera positions: community-wiki + forum, ≤2 sources) · enemy-tier: 0 · puzzle-tier: 0 · category: easter-egg · spoiler: see per-row · missable: yes · ach: camera_shy · achievement-hidden: no · trigger_type: collection_
_source: 2026-11-06 (camera rows 9, 12, 15, 17, 19, 21, 25, 26, 27, 30) https://strategywiki.org/wiki/Portal/Chamber_05, https://strategywiki.org/wiki/Portal/Chamber_10, https://strategywiki.org/wiki/Portal/Chamber_13, https://strategywiki.org/wiki/Portal/Chamber_15, https://strategywiki.org/wiki/Portal/Chamber_16, https://strategywiki.org/wiki/Portal/Chamber_17, https://strategywiki.org/wiki/Portal/Chamber_18 · capture: browser_fetch · confidence: medium · enemy-tier: 0 · puzzle-tier: 0 · category: easter-egg · spoiler: see per-row · missable: yes · ach: camera_shy · achievement-hidden: no · trigger_type: collection_ [Single source -- verify · class:walkthrough]

> see achievements.md for the Camera Shy entry and the run-state reset rules.
> see sections/missables.md for the run-missable summary.

---

## Hidden radios (26 -- `ach: transmission_received` · trigger_type: collection · achievement-hidden: unknown)

> **Cross-system dependency** -- see `dependencies.md` SEQ-001: Radios other than the Chamber 00 one do not exist until the game is beaten once; do a dedicated post-completion pass.

Carry each radio to its signal spot; the light turns green when placed correctly. Radios are added to existing chambers (not a separate area); apart from the Chamber 00 radio they only appear after the game is completed once.

| # | Chamber | Location / note (feature-anchored) |
|---|---|---|
| 1 | chamber_00 | On a table in the corner of the starting room; carry it to the special spot near the button. The only radio present on a first playthrough. |
| 2 | chamber_01 | Present in chamber |
| 3 | chamber_02 | Present in chamber |
| 4 | chamber_03 | Present in chamber |
| 5 | chamber_04 | Present in chamber |
| 6 | chamber_05 | Behind the door opened by the two buttons: fire a portal under the radio before you step through that door (it shuts behind you), then drop it into the pit that held a cube. |
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
| 24 | escape_seq | Escape (`escape_00`): just after the load screen, under the stairs (portal through the fence and crawl into the vent to a small supplies area); the signal spot is the top of the platform just above the two vertical pistons. |
| 25 | escape_seq | Escape (`escape_01`): after the three-turret ambush, near the broken sentry; the signal spot is the supplies alcove in the next room, after knocking down the turret. |
| 26 | escape_seq | In the final large turret room with the muddy trench; bring it to the two large electrical engines/generators near the top |

_source: deep-research handoff 2026-06-02 · capture: web_fetch · confidence: medium (per-radio positions: community-wiki, ≤2 sources) · enemy-tier: 0 · puzzle-tier: 0 · category: easter-egg · spoiler: none (escape rows: late-game by location) · ach: transmission_received · achievement-hidden: unknown · trigger_type: collection_
_source: 2026-11-06 (radio 6) https://strategywiki.org/wiki/Portal/Chamber_05, https://www.thonky.com/portal-walkthrough/transmission-received · capture: browser_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 0 · category: easter-egg · spoiler: none · ach: transmission_received · achievement-hidden: unknown · trigger_type: collection_ [Confirmed: 2]
_source: 2026-11-06 (radio 24) https://strategywiki.org/wiki/Portal/Transmission_Received, https://www.thonky.com/portal-walkthrough/transmission-received · capture: browser_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 0 · category: easter-egg · spoiler: late-game · ach: transmission_received · achievement-hidden: unknown · trigger_type: collection_ [Confirmed: 2]
_source: 2026-11-06 (radio 25) https://strategywiki.org/wiki/Portal/Transmission_Received · capture: browser_fetch · confidence: medium · enemy-tier: 0 · puzzle-tier: 0 · category: easter-egg · spoiler: late-game · ach: transmission_received · achievement-hidden: unknown · trigger_type: collection_ [Single source -- verify · class:walkthrough]

> see achievements.md for the Transmission Received entry (hidden; post-completion gating).

## Sources

- StrategyWiki Portal; Steam Community camera/radio guides; ThePortalWiki.com (community-wiki / forum)
