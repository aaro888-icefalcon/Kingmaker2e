---
name: pathfinder2e
description: >-
  Companion content-pack skill for the mythic-gm engine that supplies Pathfinder Second Edition
  (PF2e) rules and the Kingmaker Adventure Path (Stolen Lands sandbox). Use ALONGSIDE mythic-gm
  whenever the user wants to play, run, or continue a solo/GM-less Pathfinder 2e game, the
  Kingmaker campaign, build a kingdom in the Stolen Lands, hexplore the Greenbelt, fight the
  Stag Lord / Vordakai / King Irovetti / Nyrissa, or resolve any PF2e check, skill action, or
  subsystem (Kingdom turns, Hexploration, Warfare, Influence, Research). Triggers on
  "Pathfinder 2e", "PF2e", "Kingmaker", "Stolen Lands", "kingdom building", "hexploration",
  "run my Kingmaker game", or "be my GM for Pathfinder". This skill is the BRIDGE; mythic-gm is
  the ENGINE — it owns scenes, the Scene Test, Chaos, Fate Questions, Random Events, Turning
  Points, and the no-softening discipline. This skill never re-implements the oracle; it fills
  the engine's hooks with PF2e rules, the Stolen Lands setting, generators, subsystems, and the
  atomized adventure.
---

# pathfinder2e — Kingmaker companion for the mythic-gm engine

This is a **companion content pack**, not a standalone game. It pairs with the **mythic-gm**
engine (`.claude/skills/mythic-gm/`). The engine runs the loop; this skill supplies *the world*:
Pathfinder 2e rules, the Stolen Lands setting, generators, the three Kingmaker subsystems, and
the fully-atomized Kingmaker Adventure Path.

## How the two skills combine

1. **The user wants to play.** mythic-gm is the engine of play — always start there. Its
   `SKILL.md` is the operating manual (the Turn, the discipline, the scripts).
2. **Load this bridge at session start.** The engine reads a companion bridge declared by its
   path. This bridge lives at:

   ```
   .claude/skills/pathfinder2e/bridge
   ```

   Load it with the engine's own tooling (run from the engine root
   `.claude/skills/mythic-gm/`):

   ```
   python3 scripts/bridge.py summary   ../pathfinder2e/bridge   # which hooks override vs default
   python3 scripts/bridge.py validate  ../pathfinder2e/bridge   # files present + generators roll-tested
   ```

3. **Use an override where present, else the engine default.** Per hook
   (`resolve`/`meaning`/`chaos`/`themes`/`world-tick`/`seeds`/`generate:*`/`adventure-ingest`)
   the bridge file replaces or layers on the Mythic/AC default. The machine-readable contract is
   `bridge/bridge.md` (the ```json manifest).

## What this bridge fills (hook → file)

| Hook | File | What it teaches the engine |
|---|---|---|
| `resolve` | `bridge/system-profile.md` (+ `reference/pf2e-core.md`) | PF2e `1d20+mod vs DC`, four degrees of success, the **skills system**, three-action combat, dying/death |
| `meaning` | `bridge/interpretation.md` | Stolen Lands / Golarion GM lens — how factions want and act |
| `chaos` | `bridge/chaos-tendency.md` | Chaos start/lean/flavor for a frontier-survival + kingdom-drama campaign |
| `themes` | `bridge/theme-weights.md` | Fixed Adventure-Crafter theme weights for Kingmaker |
| `world-tick` | `bridge/subsystems.md` (+ `reference/{kingdom-turn,hexploration,warfare}.md`) | **Kingdom Turn, Hexploration, Warfare** + offscreen faction clocks |
| `seeds` | `bridge/seeds.md` | Seed-deck sources for the Stolen Lands |
| `generate:character` (+ others) | `bridge/generators/` + `bridge/bridge.md` `generators_map` | PF2e/Kingmaker tables (NPC roles, kingdom events, hex features, rumors, armies) |
| `adventure-ingest` | `bridge/adventures/` | The **atomized Kingmaker AP** (clusters + fragments, page-cited) |

Setting ground-truth (never invent over it): `bridge/setting-canon.md`.

## The campaign

The live campaign lives at `campaigns/kingmaker/` (created with `scripts/state.py init`). Its
`threads.json` / `characters.json` / `adventure.json` are the machine-rollable source of truth
for the Threads & Characters Lists and the Adventure-Crafter Theme order; `campaign-state.md` is
the human-readable snapshot; `hexmap.json` tracks explored hexes + a usage ledger for the
Hybrid hex integration (see `reference/hexploration.md`).

## Hexploration ↔ keyed encounters (Hybrid; the binding the GM must hold)

Geography is authoritative **inside** a hex; Mythic governs **between** hexes. One reconnoitered
hex = one Turn of the engine loop:

1. **Frame** from player travel intent.
2. **Reveal** via `reference/hexploration.md`: a **keyed** hex → the bridge cluster tagged
   `location:<hexcode>` becomes the Expected Scene; an **unkeyed** hex → roll `hex_feature.json`
   and/or the zone's encounter table (honest `dice.py table`), or it's empty.
3. **Scene Test** as normal (`dice.py scene <CF>`): Expected = site as written · Altered = site
   twisted · Interrupt = a Turning Point fires *before* arrival (invoking the Characters List).
4. **Play** with PF2e checks (`system-profile.md`); Fate Questions for open detail; a
   doubles-≤-CF Fate Question fires a Random Event mid-exploration.
5. **Bookkeep — the memory:** add the site's objective to `threads.json` and its NPCs to
   `characters.json` (so they keep getting weighted/invoked after the PC leaves the hex), put the
   location on the **Adventure Features** list, mark the hex in `hexmap.json`, judge Chaos ±1,
   and tick the faction clocks.

**Per-content-type mode:** overworld hex sites run as **pure sandbox** (Altered/Interrupt ON);
linear set-piece **dungeons** (Stag Lord's Fort, Vordakai's Tomb, …) run as **keyed rooms in
their own internal geography** (fragments = rooms, Scene-Tested at meaningful thresholds). Each
cluster is tagged with its `mode` in `bridge/adventures/`.

## What stays the engine's (never overridden here)
Scenes, the Scene Test, Chaos math, Fate Questions, Random Events, Turning Points, the
seed/list machinery, and the no-softening discipline. This skill supplies the *world*, not the
*engine*. The dice are always the engine's, always shown, never fudged.
