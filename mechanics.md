# Portal -- Core Mechanics

**status:** research-integrated
**last_reconciled:** 2026-06-02
**research_run:** P1 ingested 2026-06-02 (portal_p1.result.md)

Portal is a physics-based puzzle game. All gameplay derives from one core tool (the portal gun) and one core rule (momentum is conserved between portals). Deep weapon-item detail for the ASHPD lives in `items/weapons.md`; this file covers the systems and hazards.

> **Portal-2 conflation guard.** The original Portal does NOT contain Aerial Faith Plates, Thermal Discouragement Beams (lasers), gels, Hard Light Bridges, or Excursion Funnels -- those are Portal 2. Original-Portal systems are limited to: portals, buttons, Weighted/Companion Cubes, High Energy Pellets, Unstationary Scaffolds, goo, Emancipation Grills, Sentry Turrets, the rocket turret, and personality cores. _source: deep-research handoff 2026-06-02 · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 0 · category: mainline · spoiler: none_

---

## Portal mechanics (primary system)

The ASHPD fires two linked portals (blue and orange). Only one of each color exists at a time; firing a new blue portal moves the existing blue one. The player and objects pass through one aperture and exit the other instantaneously.

- **Surface compatibility:** portals attach only to flat, light-colored/concrete-type surfaces. Dark metallic brown/black panels are deliberately non-portalable; the developer commentary notes this colour choice was made so non-portalable surfaces are easy to spot from a distance. Glass and moving surfaces reject portals. _source: deep-research handoff 2026-06-02 · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 0 · category: mainline · spoiler: none_
- **Crosshair feedback:** the crosshair indicator changes colour when it is over a valid portal-placement surface -- the primary read for spotting portalable surfaces and edge placements. _source: deep-research handoff 2026-06-02 · capture: web_fetch · confidence: medium · enemy-tier: 0 · puzzle-tier: 0 · category: mainline · spoiler: none_
- **Acquisition timing:** Chambers 00-01 have no player gun (automated portals). The blue-only ASHPD is retrieved in **Chamber 02**; the fully powered dual-portal (blue+orange) device is acquired in **Chamber 11** (triggers "Lab Rat"). _source: deep-research handoff 2026-06-02 · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 0 · category: mainline · spoiler: progression_

See `items/weapons.md` for the full weapon-item summary.

---

## Momentum conservation / fling mechanic

**Core rule:** momentum is conserved; exit speed equals entry speed, redirected along the exit portal's surface normal. GLaDOS states it in Chamber 11: *"Momentum, a function of mass and velocity, is conserved between portals. In layman's terms, speedy thing goes in, speedy thing comes out."* _source: deep-research handoff 2026-06-02 · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 0 · category: mainline · spoiler: none_

- **Fall→fling conversion:** falling into a floor portal and exiting a wall portal flings you horizontally at the speed you reached falling. This underlies most advanced solutions from Chamber 10 onward. _source: deep-research handoff 2026-06-02 · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 0 · category: mainline · spoiler: progression_
- **Engine constants:** gravity is governed by `sv_gravity`, which defaults to **600** in Portal (Valve's Source default is 800 in other games). `sv_maxvelocity` caps ballistic speed at **3500 per axis** -- not total magnitude, so diagonal flings can exceed 3500 total. _source: deep-research handoff 2026-06-02 · capture: web_fetch · confidence: medium (engine-wide default, not a Portal-specific Valve page) · enemy-tier: 0 · puzzle-tier: 0 · category: mainline · spoiler: none · conflicts: frequently misstated as a total-magnitude cap_
- **Air-strafe:** Portal 1 allows air-strafing during a fling to bend the arc (more air control than Portal 2). _source: deep-research handoff 2026-06-02 · capture: web_fetch · confidence: low [single source] · enemy-tier: 0 · puzzle-tier: 1 · category: mainline · spoiler: progression_
- **Edge cases:** on non-parallel portals the player is reoriented upright to gravity after exit; "portal bumping" (placing a portal onto another bumps it aside and pushes the player) is used to skip Chambers 16-17; the edge-glitch / portal-ledging lets a portal sit on otherwise-invalid edges. _source: deep-research handoff 2026-06-02 · capture: web_fetch · confidence: medium · enemy-tier: 0 · puzzle-tier: 2 · category: easter-egg · spoiler: late-game_
- **Speedrun characterization (Accelerated Back Hopping):** the dominant movement tech is ABH, a Source/OrangeBox glitch replacing the patched-out bunny hop. New speed per perfect hop ≈ (current speed × 2 − speed limit); gain is exponential. Per the SourceRuns Wiki, the speed limit is **165 UPS while crouched in Portal specifically** (vs. 209 elsewhere), 225 walking, 285 running, 352 sprinting. Discovered by Spider-Waffle. _source: deep-research handoff 2026-06-02 · capture: web_fetch · confidence: medium · enemy-tier: 0 · puzzle-tier: 2 · category: easter-egg · spoiler: none_
- **Fall-velocity reset on death/respawn:** not documented in reviewed sources. _source: deep-research handoff 2026-06-02 · capture: web_fetch · confidence: low [hypothesis -- unverified] · enemy-tier: 0 · puzzle-tier: 1 · category: mainline · spoiler: none_

---

## Emancipation Grills (fizzlers)

- **Function:** vaporize unauthorized objects (cubes, turrets, cameras, radios, rockets), block portal shots, and reset the player's active portals on pass-through. The player and the ASHPD pass through unharmed. _source: deep-research handoff 2026-06-02 · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 0 · category: mainline · spoiler: none_
- **Pass vs. dissolve:** the test subject and portal gun pass; cubes, turrets, cameras, radios, and rockets are vaporized (a dissolving turret emits a long "owowowow"). Portals cannot be placed through or across a grill, and portals on the far side are unreachable. High Energy Pellets are destroyed on contact like other objects. _source: deep-research handoff 2026-06-02 · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 0 · category: mainline · spoiler: none_
- **Documented exception:** some square metal maintenance panels are NOT affected by the grill -- a developer oversight. _source: deep-research handoff 2026-06-02 · capture: web_fetch · confidence: low [single source] · enemy-tier: 0 · puzzle-tier: 1 · category: easter-egg · spoiler: none_
- **Naming note:** subtitles and the Prima guide call it the "Grid"; GLaDOS pronounces it "Grill" in-game -- a documented inconsistency. _source: deep-research handoff 2026-06-02 · capture: web_fetch · confidence: medium · enemy-tier: 0 · puzzle-tier: 0 · category: mainline · spoiler: none_

---

## Hazard systems

### Sentry Turrets (introduced Chamber 16)
- Detect player line-of-sight, deploy laser sights, then open fire. Can be picked up with the portal gun and toppled. Entrance glass in Chamber 16 is bulletproof. _source: deep-research handoff 2026-06-02 · capture: web_fetch · confidence: high · enemy-tier: 2 · puzzle-tier: 0 · category: mainline · spoiler: late-game · vector: enemy_
- **Tactics:** place a portal behind/under a turret to topple it; for alcove turrets you can't portal under, place a portal on the red X above them and drop a cube / camera / turret onto it. Waiting for a turret's laser to settle gives more reaction time. _source: deep-research handoff 2026-06-02 · capture: web_fetch · confidence: medium · enemy-tier: 2 · puzzle-tier: 0 · category: mainline · spoiler: late-game · vector: enemy_

### Toxic goo / acid (introduced Chamber 08)
- Instant-kill floor hazard. Developer note: Chamber 08 was originally meant to be the first pellet chamber, but playtesters found too many mechanics at once, so Chambers 06-07 were inserted before it. _source: deep-research handoff 2026-06-02 · capture: web_fetch · confidence: medium · enemy-tier: 0 · puzzle-tier: 0 · category: lore · spoiler: none · vector: lore_

### High Energy Pellet (introduced Chamber 06)
- A bouncing energy ball that kills in one hit; route it through a portal into a receiver to power lifts/doors. The receiver shines a red light on the ceiling to help aim the portal. _source: deep-research handoff 2026-06-02 · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 1 · category: mainline · spoiler: none · vector: puzzle_
- **Underexplained:** pellets recharge their lifespan when passing through a portal, extending the window before they disintegrate. _source: deep-research handoff 2026-06-02 · capture: web_fetch · confidence: low [single source] · enemy-tier: 0 · puzzle-tier: 1 · category: mainline · spoiler: none_
- A **green, non-disintegrating** variant of the High Energy Pellet appears in Chamber 19. _source: deep-research handoff 2026-06-02 · capture: web_fetch · confidence: medium · enemy-tier: 0 · puzzle-tier: 0 · category: mainline · spoiler: late-game_

### Unstationary Scaffold (introduced Chamber 07)
- A moving platform the player rides, typically combined with pellet routing. _source: deep-research handoff 2026-06-02 · capture: web_fetch · confidence: medium · enemy-tier: 0 · puzzle-tier: 0 · category: mainline · spoiler: none_

> Energy-pellet projectiles in Portal 1 are **High Energy Pellets** -- not "Thermal Discouragement Beams" (a Portal 2 laser system). The earlier scaffold label was a Portal-2 conflation and has been corrected.

---

## Object interaction

### Weighted Storage Cubes
- Primary puzzle prop: placed on buttons to hold doors/mechanisms open; can be carried through portals; used as height boosts and turret-drop weapons. _source: deep-research handoff 2026-06-02 · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 0 · category: mainline · spoiler: none_

### Weighted Companion Cube (Chamber 17)
- A special named cube introduced in Chamber 17; **functions identically** to a normal Weighted Storage Cube. Must be incinerated in the Incinerator Room to open the chamber exit (triggers "Fratricide"). Narrative detail in `sections/story_notes.md`. _source: deep-research handoff 2026-06-02 · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 0 · category: mainline · spoiler: story_

### Buttons
- Large floor buttons (hold-to-activate; need a cube or the player's weight) and wall buttons. _source: deep-research handoff 2026-06-02 · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 0 · category: mainline · spoiler: none_

---

## Autosave / checkpoint system

Portal uses automatic checkpoints triggered at chamber entry and at certain mid-chamber progress points; there are no manual save stations. Death returns the player to the most recent checkpoint within the current chamber. Exact mid-chamber autosave trigger locations are P2 scope.
_source: deep-research handoff 2026-06-02 · capture: web_fetch · confidence: medium · enemy-tier: 0 · puzzle-tier: 0 · category: mainline · spoiler: none_

---

## Sources

- ThePortalWiki.com; StrategyWiki Portal; Wikipedia *Portal (video game)* (community-wiki / editorial-en)
- Valve Developer Community "Gravity" page; cvar databases gamerconfig.eu, totalcsgo.com (`sv_gravity`, `sv_maxvelocity`)
- SourceRuns Wiki "Accelerated Back Hopping"; speedrun.com/portal (speedrun-wiki)
- German (GameStar, 4players.de) and Russian (StopGame.ru) checked -- no original-Portal edge case missed by English sources.
