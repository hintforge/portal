# Dependencies -- Portal
<!-- hintforge · stitch pass · last run: 2026-06-03 -->
<!-- Every stitch run re-audits ALL existing edges + adds new ones. The per-edge convergence audit (open each cited source, verify the specific value) applies to every row in this file on every run, not just new candidates. A game patch, DLC, or new ingestion phase can change facts that existing edges cite -- only a full re-audit catches that. See `stitch_and_zipper.md` Phase B "Re-run scope: always full." Inconsistencies (cited source contradicts edge text) land in the `## Corpus inconsistencies` section; the edge row stays in place. -->

## Cross-system edges

| Edge ID | System A | System B | Dependency description | Confidence | Source files |
|---------|----------|----------|------------------------|------------|--------------|

_(No DEP-class cross-system edges written on first pass; the primary cross-system dependencies for Portal are captured as sequencing and PoNR edges below. All mechanic-stack interactions (portal/momentum, pellet routing, grill resets) are single-directory or already fully cross-referenced in-file.)_

## PoNR / lockout edges

| Edge ID | Trigger | Locked out | Notes | Source files |
|---------|---------|------------|-------|--------------|
| PON-001 | Exit `chamber_18` via chamberlock elevator to `chamber_19` (chapter-bound, one-way) | Friendly Fire achievement — physically knock one turret over with another | Chamber 18 is the last turret chamber on a linear playthrough. Achievement can be earned in chamber_16 (gate-05, most reliable) or chamber_18 — once the elevator to chamber_19 is taken, no turrets remain. | achievements.md, sections/missables.md, nav/chamber_18.md, nav/architecture.md |
| PON-002 | Transition to `escape_seq` via chamber_19-gate-07 (oven escape / Partygoer) — no return to test chambers | Camera Shy achievement; also locally: no cameras accessible after chamber_19-gate-05 (malfunctioning chamberlock drop) | Latest cameras (3) are in chamber_19 (gates 01-03, before gate-05). No cameras exist in escape_seq or after. Camera Shy counter also resets on any death-restart or reload — treat every death during a Camera Shy run as a counter reset requiring restart from chamber_02. | achievements.md, sections/missables.md, nav/chamber_19.md, nav/architecture.md |

## Missable / sequencing dependencies

| Edge ID | Action | Window | Consequence | Source files |
|---------|--------|--------|-------------|--------------|
| SEQ-001 | Collect all 26 hidden radios and bring each to its signal spot | Post-completion only — radios must be collected on a dedicated second run after the game is beaten once | Radios are physically present from a first playthrough but grant **no Transmission Received achievement progress** until the game is completed at least once (escape_seq → Heartbreaker). Plan a dedicated post-completion radio run. | achievements.md, items/collectibles.md, nav/architecture.md |
| SEQ-002 | Complete the game — defeat GLaDOS and trigger Heartbreaker (escape_seq → end) | n/a (post-game unlock; no time limit) | Unlocks: (1) Advanced Test Chambers (6 variants of chambers 13-18; feeds Cupcake / Fruitcake / Vanilla Crazy Cake achievements); (2) Portal Challenges (18 tasks across chambers 13-18 × least portals / least steps / least time; feeds Basic Science / Rocket Science / Aperture Science). Both become available from the main menu post-completion. | achievements.md, nav/architecture.md |

## Stitch run log

| Date | Scope | Edges written | Inconsistencies surfaced | Model |
|------|-------|---------------|--------------------------|-------|
| 2026-06-03 | full | 4 (PON-001, PON-002, SEQ-001, SEQ-002) | 1 | claude-sonnet-4-6 |

## Corpus inconsistencies

Stitch's per-edge convergence audit populates this section when a candidate edge's cited sources contradict each other.

| Detected | Files | Conflicting values | Suspected authoritative source | Status |
|----------|-------|--------------------|--------------------------------|--------|
| 2026-06-03 | nav/chamber_17.md (Entry), nav/architecture.md (Support Topology map pairing) | chamber_17.md says "Autosave on map load (within testchmb_a_08)"; architecture.md says "the autosave for the second chamber in a pair fires on the inter-chamber elevator transition, not a fresh map load" — chamber_17 is the second chamber in testchmb_a_08 | nav/architecture.md (explicitly distinguishes map-load vs elevator-transition autosave; all other second-chamber nav files use correct phrasing) | resolved 2026-06-03 |
