# Portal -- Puzzles Index

**status:** research-integrated
**last_reconciled:** 2026-06-02
**research_run:** P1 ingested 2026-06-02

Portal's core gameplay is puzzle-solving via portal placement and physics exploitation. Each test chamber is a discrete puzzle.

> **P1 coverage note.** The P1 deep-research result focused on architecture, mechanics, collectibles, and achievements rather than per-chamber step-by-step solutions. Puzzle files exist where P1 surfaced a concrete solution or a notable trick (Chambers 06 and 14). Remaining per-chamber solution files are deferred to live play (the player solves a chamber, the hint ladder gets refined from what they hit) -- P2 is navigation-only and does not add puzzle solutions.

## How puzzles are organized

- Per-chamber puzzle files are created during P1 ingestion.
- Each file covers: puzzle type / mechanic identification (Tier 1 auto-deliver), hint ladder (Lvl 1 nudge → Lvl 2 more detail → Lvl 3 full step-by-step), and any alternative solutions.

## Puzzle type taxonomy for Portal

| Type | Mechanic | First appearance |
|---|---|---|
| Portal placement | Place portals to create traversal path | Chamber 02 (blue gun acquired) |
| Button activation | Move cube to button; hold to activate mechanism | Chamber 00 |
| Height gain | Use portals to reach elevated surfaces | Early chambers |
| Fling / momentum | Use floor→wall portal to convert fall to horizontal velocity | Chamber 10 (lessons begin); dual-portal from Chamber 11 |
| Energy-pellet redirect | Direct the High Energy Pellet through portals into a receiver | Chamber 06 |
| Turret avoidance / redirect | Navigate around or reposition Sentry Turrets via portals | Chamber 16+ |

## Chamber files

| File | Chamber | Puzzle type | Status |
|---|---|---|---|
| [`chamber_06.md`](chamber_06.md) | Chamber 06 | Energy-pellet routing | research-integrated |
| [`chamber_14.md`](chamber_14.md) | Chamber 14 | Fling / momentum (early-exit) | research-integrated |
| Other chambers | Chambers 00-05, 07-13, 15-19 + escape | See taxonomy above | deferred to live play (no P1 solution surfaced) |

## Hint ladder format (standard for all puzzle entries)

```
**Lvl 1 nudge:** [identify the mechanic; one sentence; what to notice, not what to do]
**Lvl 2 hint:** [directional hint; what to try, without the full solution]
**Lvl 3 solution:** [complete step-by-step]
```

Tier 1 (current setting) auto-delivers mechanic identification on chamber entry. Full hints require player request.
