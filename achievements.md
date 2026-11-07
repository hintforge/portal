# Portal -- Achievements

**status:** research-integrated
**last_reconciled:** 2026-11-06
**research_run:** P1 ingested 2026-06-02 (portal_p1.result.md)
**stub_source:** Steam (via pandallax.com + Wikipedia cross-check), Stage 0 2026-06-02
**coverage:** 15 stubs / 15 resolved / 0 deferred / 0 unreachable

## Why this file exists

Single source of truth for "what achievements does this game have, and what do I need for each." Organized into trigger-type sections (`progression | branch | mastery | collection | threshold | discovery`); sections with no entries are omitted (Portal has no `branch` achievements). The reader consults it for any achievement-class question; per-claim trigger detail lives in the vector-binding files noted on each entry.

## Genre vocabulary

- `mission` -- per-level scored mastery (time / portal-count / step-count medals); Hitman/Forza pattern.

---

## Progression

Every player who reaches the point gets these on the default path.

### Lab Rat
- **id:** lab_rat · **hidden:** no · **trigger_type:** progression
- **trigger:** Pick up the orange portion of the ASHPD (the fully powered dual-portal gun) in **Chamber 11**.
- **missable:** no · **ponr-window:** n/a (unmissable on normal play) · **prereqs:** none
- **vector-binding:** `items/weapons.md`, `mechanics.md`
- enemy-tier 0 · puzzle-tier 0 · spoiler: progression

### Fratricide
- **id:** fratricide · **hidden:** no · **trigger_type:** progression
- **trigger:** Incinerate the Weighted Companion Cube in the Incinerator at the end of **Chamber 17** (required to open the exit).
- **missable:** no · **ponr-window:** n/a (required to advance) · **prereqs:** none
- **vector-binding:** `mechanics.md` (object interaction), `sections/story_notes.md`
- enemy-tier 0 · puzzle-tier 0 · spoiler: story

### Partygoer
- **id:** partygoer · **hidden:** no · **trigger_type:** progression
- **trigger:** Escape the fire pit with portals, reaching the ledge/platform above it, at the end of **Chamber 19** ("make the correct party escort submission position decision").
- **missable:** no · **ponr-window:** n/a (unmissable) · **prereqs:** none
- **vector-binding:** `nav/architecture.md` (chamber_19 → escape_seq edge)
- enemy-tier 0 · puzzle-tier 0 · spoiler: late-game
_source: 2026-11-06 https://strategywiki.org/wiki/Portal/Chamber_19, https://www.thonky.com/portal-walkthrough/test-chamber-19 · capture: browser_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 0 · category: mainline · spoiler: late-game_ [Confirmed: 2]

### Heartbreaker
- **id:** heartbreaker · **hidden:** no · **trigger_type:** progression
- **trigger:** Destroy GLaDOS -- incinerate the final core in the escape/boss fight (completes the game).
- **missable:** no · **ponr-window:** n/a (completion) · **prereqs:** reach the boss
- **vector-binding:** `sections/escape_seq.md`
- enemy-tier 2 · puzzle-tier 0 · spoiler: story

---

## Mastery

Skill or accepted restriction beyond normal play.

> **Cross-system dependency** -- see `dependencies.md` SEQ-002: Completing the game (Heartbreaker) unlocks Advanced Chambers (feeds Cupcake/Fruitcake/Vanilla Crazy Cake) and Portal Challenges (feeds Basic Science/Rocket Science/Aperture Science); none of these six achievements are accessible on a first run.

### Long Jump
- **id:** long_jump · **hidden:** no · **trigger_type:** mastery
- **trigger:** Travel **300 feet in a single jump/fling** -- best in the large escape-sequence room with the muddy trench.
- **missable:** no · **ponr-window:** n/a · **prereqs:** dual-portal gun (Chamber 11)
- **vector-binding:** `mechanics.md` (fling), `sections/escape_seq.md`
- enemy-tier 0 · puzzle-tier 0 · spoiler: none

### Cupcake
- **id:** cupcake · **hidden:** no · **trigger_type:** mastery
- **trigger:** Beat **2** of the 6 Advanced Test Chambers (Advanced 13-18).
- **missable:** no · **ponr-window:** n/a · **prereqs:** complete the main game (unlocks Advanced Chambers)
- **vector-binding:** `nav/architecture.md` (optional-content registry)
- enemy-tier 0 · puzzle-tier 0 · spoiler: none

### Fruitcake
- **id:** fruitcake · **hidden:** no · **trigger_type:** mastery
- **trigger:** Beat **4** Advanced Test Chambers.
- **missable:** no · **ponr-window:** n/a · **prereqs:** complete the main game
- **vector-binding:** `nav/architecture.md` (optional-content registry)
- enemy-tier 0 · puzzle-tier 0 · spoiler: none

### Vanilla Crazy Cake
- **id:** vanilla_crazy_cake · **hidden:** no · **trigger_type:** mastery
- **trigger:** Beat **all 6** Advanced Test Chambers (Advanced 13-18).
- **missable:** no · **ponr-window:** n/a · **prereqs:** complete the main game
- **vector-binding:** `nav/architecture.md` (optional-content registry)
- enemy-tier 0 · puzzle-tier 0 · spoiler: none

### Basic Science
- **id:** basic_science · **hidden:** no · **trigger_type:** mastery · **genre:** mission
- **trigger:** Earn **bronze medals on all 18** Challenge tasks (Chambers 13-18 × least portals / least steps / least time). *(Corrected from the Stage-0 stub, which mis-stated this as a single gold medal on map 13.)*
- **missable:** no · **ponr-window:** n/a · **prereqs:** complete the main game (unlocks Portal Challenges)
- **vector-binding:** `nav/architecture.md` (optional-content registry)
- enemy-tier 0 · puzzle-tier 0 · spoiler: none

### Rocket Science
- **id:** rocket_science · **hidden:** no · **trigger_type:** mastery · **genre:** mission
- **trigger:** Earn **silver medals on all 18** Challenge tasks. *(Corrected from the stub: not a gold on map 14.)*
- **missable:** no · **ponr-window:** n/a · **prereqs:** complete the main game
- **vector-binding:** `nav/architecture.md` (optional-content registry)
- enemy-tier 0 · puzzle-tier 0 · spoiler: none

### Aperture Science
- **id:** aperture_science · **hidden:** no · **trigger_type:** mastery · **genre:** mission
- **trigger:** Earn **gold medals on all 18** Challenge tasks. *(Corrected from the stub: not a gold on map 15 alone.)* Note: `sv_cheats`/no-clip disables medal submission -- earn legitimately.
- **missable:** no · **ponr-window:** n/a · **prereqs:** complete the main game
- **vector-binding:** `nav/architecture.md` (optional-content registry)
- enemy-tier 0 · puzzle-tier 0 · spoiler: none

---

## Collection

A finite, enumerable set completed in full.

### Camera Shy
- **id:** camera_shy · **hidden:** no · **trigger_type:** collection
- **trigger:** Detach **all 33 security cameras** with the portal gun, getting every camera the first time through each chamber (Chambers 02,03,04,05,10,11,13,15,16,17,18,19).
- **missable:** **yes** -- the counter resets if you skip or replay a chamber. · **ponr-window:** latest camera in **Chamber 19**; none after. · **prereqs:** dual-portal gun for most cameras
- **set members:** all 33 enumerated in `items/collectibles.md`
- **vector-binding:** `items/collectibles.md`, `sections/missables.md`
- enemy-tier 0 · puzzle-tier 0 · spoiler: none
- **Note:** the common-knowledge claim that interrupting GLaDOS's camera voice lines breaks this is **false** -- detach counter and voice-line counter are separate.
_source: 2026-11-06 https://strategywiki.org/wiki/Portal/Camera_Shy, https://www.thonky.com/portal-walkthrough/achievements · capture: browser_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 0 · category: mainline · spoiler: none_ [Confirmed: 2]

> **Cross-system dependency** -- see `dependencies.md` PON-002: No cameras exist in escape_seq or after; all chamber_19 cameras (3) must be collected before the fire pit (chamber_19 gate-06); transitioning to escape_seq at gate-07 is the final PoNR. Skipping or replaying a chamber resets the counter.
_source: 2026-11-06 https://strategywiki.org/wiki/Portal/Camera_Shy, https://strategywiki.org/wiki/Portal/Chamber_19 · capture: browser_fetch · confidence: medium · enemy-tier: 0 · puzzle-tier: 0 · category: mainline · spoiler: late-game_ [Single source -- verify · class:walkthrough]

### Transmission Received
- **id:** transmission_received · **hidden:** unknown (listed on Steam by name with the placeholder description "..?"; the sources checked state no hidden flag) · **trigger_type:** collection
- **trigger:** Collect **all 26 hidden radios** and bring each to its signal spot (light turns green).
- **missable:** no · **ponr-window:** n/a · **prereqs:** **complete the game once** -- the radios other than Chamber 00's only appear after a full completion.
- **set members:** all 26 enumerated in `items/collectibles.md`
- **vector-binding:** `items/collectibles.md`
- enemy-tier 0 · puzzle-tier 0 · spoiler: none (achievement *name* gated by hidden flag)
_source: 2026-11-06 https://theportalwiki.com/wiki/Obtaining_Portal_achievements, https://strategywiki.org/wiki/Portal/Transmission_Received, https://www.pcgamingwiki.com/wiki/Portal, https://www.thonky.com/portal-walkthrough/achievements · capture: browser_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 0 · category: mainline · spoiler: none_ [Confirmed: 3]

> **Cross-system dependency** -- see `dependencies.md` SEQ-001: Radios other than the Chamber 00 one do not exist until the game is completed once; plan a dedicated post-completion radio run.

---

## Threshold

A cumulative count without a finite-set ceiling.

### Terminal Velocity
- **id:** terminal_velocity · **hidden:** no · **trigger_type:** threshold *(reclassified from the Stage-0 stub's "discovery": the trigger is a cumulative fall distance, not a hidden interaction)*
- **trigger:** Fall **30,000 feet** -- in any test chamber where you can put portals on both the ceiling and the floor, place one above and one below you, jump in and wait about 5 minutes.
_source: 2026-11-07 https://theportalwiki.com/wiki/Obtaining_Portal_achievements · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 0 · category: mainline · spoiler: none_ [Single source]
- **missable:** no (doable in any chamber with facing portalable ceiling+floor) · **ponr-window:** n/a · **prereqs:** dual-portal gun (Chamber 11)
- **vector-binding:** `mechanics.md` (fling), `puzzles/chamber_14.md`
- enemy-tier 0 · puzzle-tier 0 · spoiler: none

---

## Discovery

Found by deliberate exploration of a non-obvious interaction.

### Friendly Fire
- **id:** friendly_fire · **hidden:** no · **trigger_type:** discovery
- **trigger:** Pick up **one turret** and use it to **physically knock over another turret**. Easiest in Chamber 16 (turret-dense); turrets also appear in Chamber 18 and in the escape.
- **missable:** no -- turrets keep appearing after Chamber 18 (a three-turret ambush in Escape 01, a turret arena in Escape 02), so leaving Chamber 18 does not lock it out. · **prereqs:** reach a turret chamber (16)
- **vector-binding:** `mechanics.md` (turret tactics)
- enemy-tier 2 · puzzle-tier 0 · spoiler: late-game
_source: 2026-11-06 https://theportalwiki.com/wiki/Turrets, https://strategywiki.org/wiki/Portal/Transmission_Received, https://www.thonky.com/portal-walkthrough/test-chamber-19 · capture: browser_fetch · confidence: high · enemy-tier: 2 · puzzle-tier: 0 · category: mainline · spoiler: late-game_ [Confirmed: 3]

---

## Coverage check (P1 ingestion contract -- satisfied)

All 15 stubs **resolved** -- each carries an `ach:` overlay on at least one corpus claim and a populated entry above. Stub corrections applied: Basic/Rocket/Aperture Science triggers (tiered medals across all 18 tasks, not per-map gold); Transmission Received hidden flag (unknown -- Steam lists it by name with the placeholder description "..?" and the sources checked state no hidden flag); Terminal Velocity reclassified to threshold. No deferrals, no unreachable entries.

## Sources

- https://www.pandallax.com/guides/portal-100-achievement-guide
- https://en.wikipedia.org/wiki/Portal_(video_game)
- https://store.steampowered.com/app/400/Portal/ (canonical count/name verification, via deep-research handoff)
- ThePortalWiki.com; StrategyWiki; Steam Community guides
