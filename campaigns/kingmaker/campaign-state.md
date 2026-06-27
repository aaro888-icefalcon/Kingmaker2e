# Campaign State — Kingmaker: The Stolen Lands (solo)

> The single source of truth. Overwrite this at the end of **every** scene.
> If a change happened in the fiction but isn't written here, it didn't happen.
> Companion bridge: `.claude/skills/pathfinder2e/bridge` (load at session start:
> `python3 .claude/skills/mythic-gm/scripts/bridge.py summary .claude/skills/pathfinder2e/bridge`).

## Frame
- **Adventure Source mode:** Prepared Adventure (atomized AP, **pure sandbox**) + Adventure Crafter always-on. Per-content-type: overworld = sandbox (Altered/Interrupt ON); set-piece dungeons = keyed-rooms.
- **RPG / System Profile:** Pathfinder Second Edition → `.claude/skills/pathfinder2e/bridge/system-profile.md` (+ `reference/pf2e-core.md`)
- **Setting / canon:** The Stolen Lands / Golarion → `.claude/skills/pathfinder2e/bridge/setting-canon.md`
- **Genre & stakes vocabulary:** frontier-survival → kingdom/realm drama — death/maiming/capture early; ruin/war/lost-subjects/fallen-kingdom later. Honesty never relaxes.
- **Resolution:** Fate Chart   ·   **Chaos flavor:** standard (see `chaos-tendency.md` for region floors)
- **Discipline:** HARDCORE (no softening; Peril Points OFF unless the player opts in)
- **Solo scaling:** Diminisher = ¼ for one PC (tune to party size — see `adventures/kingmaker-overview.md`)

## CURRENT ADVENTURE: A Call for Heroes → Into the Stolen Lands (Chapters 1–3 in play)
_Each adventure has its **own** Threads & Characters Lists and Theme priority. The Lists + Theme order +
tens-counter are the machine source of truth in **`threads.json` / `characters.json` / `adventure.json`**
(the dice roll those, any length); the sections below are a human-readable **snapshot** — keep them
roughly in sync but edit the JSON via `state.py`._
_A **new adventure** begins when the current one's main Thread(s) Conclude (`threads.json` empties) or the
player declares one — then roll new Themes (`adventure_crafter.py themes --campaign <dir>`), clear the
Threads List, carry over only still-relevant Characters, archive the rest._

- **Adventure status:** active
- **Theme priority (this adventure):** in `adventure.json` → `state.py adventure show <campaign>`
  _(currently: Social, Tension, Action, Personal, Mystery — rolled, style "action")_

## Chaos Factor: 5
_(1–9; −1 if the PC was mostly in control of the last scene, +1 if it was chaotic. Region floors apply — see chaos-tendency.md)_

## Threads List — snapshot of `threads.json` (the dice roll the JSON, not this)
_Manage with `state.py thread add|weight|remove|show <campaign> "<name>"`._
1. Settle and claim the Stolen Lands  (the master charter goal)
2. Stop the Greenbelt banditry
3. Defeat the Stag Lord
4. Who is really behind the bandits?  _(→ Pitax)_ [HIDDEN to the PC]

## Characters List (NPCs/forces; PC is NOT listed) — snapshot of `characters.json`
_Same: `state.py char add|weight|remove|show <campaign> "<name>"`._
1. Lady Jamandi Aldori  (patron, Restov swordlord)
2. Oleg and Svetlana Leveton  (first allies, Oleg's Trading Post)
3. The Stag Lord  (bandit warlord, antagonist)
4. Tartuccio  (rival charter-holder) [HIDDEN: Pitax spy]
5. Kressle  (bandit lieutenant, Thorn River Camp)
6. The Sootscale kobolds  (cursed kobold tribe, potential ally/foe)

## Tens-cycle counter (Theme-die 10s rolled so far): in `adventure.json` _(auto-updated by turning-point)_

## Adventure Features List (prepared-adventure mode; locations/hazards)
1. Oleg's Trading Post (Zone 1 / RL1) — the staging foothold
2. The Greenbelt (Zone 2) — the starting wilderness sandbox
3. Thorn River Bandit Camp (Zone 2) — Kressle's camp
4. The Old Sycamore (Zone 2 / GB14) — mite/mitflit lair
5. The Sootscale Caverns (Zone 2 / GB20) — the cursed kobolds
6. The Stag Lord's Fort (Zone 3 / TW3) — the chapter's keep
_(Add zones/sites to this list as the PC reveals them via hexploration; full atomized library in `.claude/skills/pathfinder2e/bridge/adventures/`.)_

## Campaign roster (persists across adventures: recurring NPCs, long arcs)
- [HIDDEN, unrevealed] Nyrissa (the cursed nymph queen behind events) · the Lantern King (the curse's source) · King Irovetti of Pitax (the looming rival).

## PC(s)
- See `character-sheet.md` (create at Session Zero — `reference/pf2e-character-creation.md`). Conditions/injuries: none. Resources: —.

## Overlays
- **Keyed Scenes:** _(Trigger → Event; Count)_ none (using sandbox cluster surfacing, not fixed keys)
- **Thread Progress Track:** none
- **Peril Points:** OFF _(player-invoked only)_

## Clocks (offscreen factions/threats — advanced by tick.py / subsystems.md)
- **Pitax pressure** (every 6 scenes): 0 — Irovetti's deniable hand funds the bandits; escalates toward the War of the River Kings (Ch 8).
- **Nyrissa's influence** (every 10 scenes): 0 — the curse tightens; surfaces as small fey wrongness; the Bloom in the endgame (Ch 10). [HIDDEN]
- **Offscreen threats** (every 4 scenes): the nearest un-cleared authored threat (bandits, a monster lair) presses toward the settlements.
- **Kingdom Turn** (on trigger: opens Ch 4, after the Stag Lord falls): not yet active.

## Adventure Crafter state (crafter mode)
- Active Turning Point: —   ·   Theme priority: Social, Tension, Action, Personal, Mystery
- Hexmap / spatial state: `hexmap.json` (current hex, explored set, usage ledger)

## Scene
- **Last scene recap (2–3 sentences):** The campaign opens at Session Zero. Build the PC
  (`reference/pf2e-character-creation.md`), confirm the hardcore frame, then begin in Restov at
  Lady Jamandi's feast (Ch 1) or jump to Oleg's Trading Post (Ch 3) to start the hexcrawl — the GM
  frames the First Scene (NOT tested), seeds the Lists, describes it, and asks "What do you do?"
- **Self-audit drift counter (consecutive soft scenes):** 0

## Archive pointer
- Resolved threads / dead characters → `archive.md`
