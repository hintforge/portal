# Nav -- Index

**status:** research-integrated
**last_reconciled:** 2026-06-02 (P2 ingestion)

Sequential gate lists per zone. The persona consults files in this folder first for nav-class questions ("where do I go?", "how do I get to X?", "I'm stuck at Y", "I just entered <zone>").

For the cross-zone structural backbone -- zone graph, edges, support topology, locks-and-keys -- see [`architecture.md`](architecture.md). For underlying puzzle mechanics, boss strategies, and per-zone hint ladders, see `puzzles/`. For per-region missables, see `sections/`. **This folder is routing only.**

## Files in this folder

| File | Type | Linear? | Status |
|---|---|---|---|
| [`architecture.md`](architecture.md) | zone graph + cascade outputs | n/a | research-integrated (P1+P2) |
| [`localization.md`](localization.md) | landmark toolkit | n/a | research-integrated (P2) |
| [`chamber_00.md`](chamber_00.md) | gate list | yes | research-integrated (P2) |
| [`chamber_01.md`](chamber_01.md) | gate list | yes | research-integrated (P2) |
| [`chamber_02.md`](chamber_02.md) | gate list | yes | research-integrated (P2) |
| [`chamber_03.md`](chamber_03.md) | gate list | yes | research-integrated (P2) |
| [`chamber_04.md`](chamber_04.md) | gate list | yes | research-integrated (P2) |
| [`chamber_05.md`](chamber_05.md) | gate list | yes | research-integrated (P2) |
| [`chamber_06.md`](chamber_06.md) | gate list | yes | research-integrated (P2) |
| [`chamber_07.md`](chamber_07.md) | gate list | yes | research-integrated (P2) |
| [`chamber_08.md`](chamber_08.md) | gate list | yes | research-integrated (P2) |
| [`chamber_09.md`](chamber_09.md) | gate list | yes | research-integrated (P2) |
| [`chamber_10.md`](chamber_10.md) | gate list | yes | research-integrated (P2) |
| [`chamber_11.md`](chamber_11.md) | gate list | yes | research-integrated (P2) |
| [`chamber_12.md`](chamber_12.md) | gate list | yes | research-integrated (P2) |
| [`chamber_13.md`](chamber_13.md) | gate list | yes | research-integrated (P2) |
| [`chamber_14.md`](chamber_14.md) | gate list | yes | research-integrated (P2) |
| [`chamber_15.md`](chamber_15.md) | gate list | yes | research-integrated (P2) |
| [`chamber_16.md`](chamber_16.md) | gate list | yes | research-integrated (P2) |
| [`chamber_17.md`](chamber_17.md) | gate list | yes | research-integrated (P2) |
| [`chamber_18.md`](chamber_18.md) | gate list | yes | research-integrated (P2) |
| [`chamber_19.md`](chamber_19.md) | gate list | yes | research-integrated (P2) |
| [`escape_seq.md`](escape_seq.md) | gate list | yes | research-integrated (P2) |

## Routing rules (apply to ALL nav files in this folder)

### NEVER use left/right -- anchor to features

Left and right are perspective-dependent -- they depend on which way the player is currently facing.

**The rule:**
- The **chamber entrance** (elevator arrival point, entry doorway) is the canonical reference.
- Describe paths by what they *contain* or *lead to*, not by left/right. Examples:
  - ✅ "From the chamber entrance, the button platform is directly ahead. The portal surface is on the wall to the side of the button."
  - ✅ "The exit elevator is at the far end, past the energy ball receptor."
  - ❌ "Go right." (whose right?)
- Cardinal directions are not meaningful inside test chambers -- feature anchors always.

### Flag the checkpoint mechanism on zone entry

Portal autosaves on chamber entry and at certain mid-chamber progress points. When the player enters a chamber, note that progress is autosaved at entry. Mid-chamber autosave locations are documented per-chamber in P2 gate-list files.

### Hint format on chamber entry

When the player arrives at a chamber and asks for help, **before any puzzle solutions**, give them **2-3 short navigation tips**:
1. What surface types are portal-compatible in this chamber (helps with quick orientation).
2. Any missable interactions in this chamber (cameras, radios -- marked per chamber in P2 files).
3. The exit direction / what to look for as the goal.

Keep to **3 tips max**. Solutions live in `puzzles/` -- these are orientation notes only.

## Scaffold-file fallback

When the player asks about a chamber whose nav file is still a scaffold (no gates yet), **web-search before asking a clarifying question**. Nav-class questions default search-first.

## Localization toolkit

Portal uses `landmark` localization. The player's position can be inferred from:
- **Chamber number signs** at the entry doorway (most reliable -- explicitly numbered)
- **Distinctive chamber features**: Companion Cube (Chamber 17), energy ball tracks (Chambers 14-15), live-fire turret course (Chamber 16+), GLaDOS speaker spheres
- **Audio cues**: GLaDOS delivers chamber-specific dialogue that marks progress

Localization toolkit (per-chamber landmark list) -- populated via P2 ingestion and stored in `nav/localization.md` (to be created at P2 ingestion).
