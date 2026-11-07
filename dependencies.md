# Dependencies -- Portal
<!-- hintforge · stitch pass · last run: 2026-06-03 -->

**status:** research-integrated
**last_reconciled:** 2026-11-06
<!-- Every stitch run re-audits ALL existing edges + adds new ones. The per-edge convergence audit (open each cited source, verify the specific value) applies to every row in this file on every run, not just new candidates. A game patch, DLC, or new ingestion phase can change facts that existing edges cite -- only a full re-audit catches that. See `stitch_and_zipper.md` Phase B "Re-run scope: always full." Inconsistencies (cited source contradicts edge text) land in the `## Corpus inconsistencies` section; the edge row stays in place. -->

## Cross-system edges

| Edge ID | System A | System B | Dependency description | Confidence | Source files |
|---------|----------|----------|------------------------|------------|--------------|

_(No DEP-class cross-system edges written on first pass; the primary cross-system dependencies for Portal are captured as sequencing and PoNR edges below. All mechanic-stack interactions (portal/momentum, pellet routing, grill resets) are single-directory or already fully cross-referenced in-file.)_

## PoNR / lockout edges

| Edge ID | Trigger | Locked out | Notes | Source files |
|---------|---------|------------|-------|--------------|
| PON-002 | Transition to `escape_seq` via chamber_19-gate-07 (oven escape / Partygoer) — no return to test chambers | Camera Shy achievement; also locally: no cameras accessible after the platform hallway in chamber_19 (before the fire pit) | Latest cameras (3) are in chamber_19 (gates 01-03, all before the fire pit). No cameras exist in escape_seq or after. Skipping or replaying a chamber resets the Camera Shy counter. | achievements.md, sections/missables.md, nav/chamber_19.md, nav/architecture.md |

_source: 2026-11-06 https://strategywiki.org/wiki/Portal/Camera_Shy, https://www.thonky.com/portal-walkthrough/achievements, https://strategywiki.org/wiki/Portal/Chamber_19 · capture: browser_fetch · confidence: medium · enemy-tier: 0 · puzzle-tier: 0 · category: mainline · spoiler: late-game_ [Single source -- verify · class:walkthrough]

## Missable / sequencing dependencies

| Edge ID | Action | Window | Consequence | Source files |
|---------|--------|--------|-------------|--------------|
| SEQ-001 | Collect all 26 hidden radios and bring each to its signal spot | Post-completion only — radios must be collected on a dedicated second run after the game is beaten once | Only the Chamber 00 radio exists on a first playthrough; the other radios appear once the game has been completed (escape_seq → Heartbreaker), so there is **no Transmission Received achievement progress** to make before then. Plan a dedicated post-completion radio run. | achievements.md, items/collectibles.md, nav/architecture.md |
| SEQ-002 | Complete the game — defeat GLaDOS and trigger Heartbreaker (escape_seq → end) | n/a (post-game unlock; no time limit) | Unlocks: (1) Advanced Test Chambers (6 variants of chambers 13-18; feeds Cupcake / Fruitcake / Vanilla Crazy Cake achievements); (2) Portal Challenges (18 tasks across chambers 13-18 × least portals / least steps / least time; feeds Basic Science / Rocket Science / Aperture Science). Both become available from the main menu post-completion. | achievements.md, nav/architecture.md |

_source: 2026-11-06 (SEQ-001) https://theportalwiki.com/wiki/Obtaining_Portal_achievements, https://strategywiki.org/wiki/Portal/Transmission_Received, https://www.pcgamingwiki.com/wiki/Portal · capture: browser_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 0 · category: mainline · spoiler: late-game_ [Confirmed: 3]

## Stitch run log

| Date | Scope | Edges written | Inconsistencies surfaced | Model |
|------|-------|---------------|--------------------------|-------|
| 2026-06-03 | full | 4 (PON-001, PON-002, SEQ-001, SEQ-002) | 1 | claude-sonnet-4-6 |

## Corpus inconsistencies

Stitch's per-edge convergence audit populates this section when a candidate edge's cited sources contradict each other.

| Detected | Files | Conflicting values | Suspected authoritative source | Status |
|----------|-------|--------------------|--------------------------------|--------|
| 2026-06-03 | nav/chamber_17.md (Entry), nav/architecture.md (Support Topology map pairing) | chamber_17.md said "Autosave on map load (within testchmb_a_08)"; architecture.md said the second chamber in a pair autosaves on the inter-chamber elevator transition and paired chamber_17 with chamber_16 in testchmb_a_08 | The pairing itself was wrong: chamber_17 is alone in testchmb_a_13 (corrected 2026-11-06 from the Portal Wiki and SourceRuns map lists), so it autosaves on map load | resolved 2026-11-06 |
