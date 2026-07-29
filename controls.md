# Portal -- Controls Reference

**status:** research-integrated
**last_reconciled:** 2026-06-02
**research_run:** P1 ingested 2026-06-02 (portal_p1.result.md)

## Default PC keybindings (keyboard + mouse)

| Action | Default binding |
|---|---|
| Move forward / back / strafe | W / S / A / D |
| Fire **blue** portal | Left Mouse Button |
| Fire **orange** portal | Right Mouse Button |
| Use / pick up / drop object | E |
| Jump | Space |
| Crouch | Ctrl |
| Look | Mouse |
| Pause / menu | Esc |

_source: deep-research handoff 2026-06-02 · capture: web_fetch · confidence: medium · enemy-tier: 0 · puzzle-tier: 0 · category: mainline · spoiler: none_

> Note: blue = Left-click, orange = Right-click (the earlier scaffold had these reversed; corrected from P1).

## Developer console

Enable via **Options → Keyboard → Advanced → Enable developer console**, then open with `~`.
_source: deep-research handoff 2026-06-02 · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 0 · category: mainline · spoiler: none_

### Useful console commands

| Command | Effect |
|---|---|
| `sv_cheats 1` | Enables cheats. **Disables achievement unlocks and challenge-medal submission for the session** -- challenge medals must be earned legitimately. |
| `cl_showpos 1` | On-screen position/velocity readout (used by speedrunners) |
| `cl_drawhud 0/1` | Toggle HUD |
| `sv_portal_placement_never_fail 1` | Forces portal placements to succeed |
| `portals_resizeall <w> <h>` | Resize all portals |
| `sv_gravity <value>` | Adjust gravity (default 600) |
| `host_timescale <value>` | Speed up / slow down game time |
| `fov` / `cl_fov` / `fov_desired <value>` | Field of view (FOV commands require `sv_cheats`) |
| `sensitivity <value>` | Mouse sensitivity |

_source: deep-research handoff 2026-06-02 · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 0 · category: mainline · spoiler: none_

## Controller layout

Controller is supported. Specific button mapping not documented in the P1 sources -- defer to live lookup or P2/P3. _source: deep-research handoff 2026-06-02 · capture: web_fetch · confidence: low · enemy-tier: 0 · puzzle-tier: 0 · category: mainline · spoiler: none_

## Commonly recommended remaps / technique notes

- **Mouse sensitivity matters for portal-aiming precision.** The speedrun Glitchless category caps sensitivity at 10.0. Tune sensitivity for accurate edge placements (important for Camera Shy). _source: deep-research handoff 2026-06-02 · capture: web_fetch · confidence: medium · enemy-tier: 0 · puzzle-tier: 0 · category: mainline · spoiler: none_
- **Fling (momentum conservation):** falling into a floor portal and exiting a wall portal converts fall speed to horizontal velocity. Full mechanic in `mechanics.md`.
- **Crosshair colour:** the crosshair changes colour over a valid portal surface -- learn to read it for fast orientation and edge placements.

## Sources

- ThePortalWiki.com; StrategyWiki; Steam Community guides (community-wiki / forum)
- speedrun.com/portal (Glitchless sensitivity cap)
