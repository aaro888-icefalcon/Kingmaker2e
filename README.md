# Kingmaker 2e — solo, on the Mythic GM engine

This repository is set up to play **Pathfinder Second Edition: Kingmaker** solo / GM-less, driven
by the **mythic-gm** engine (Mythic GME 2e + The Adventure Crafter) with a **Pathfinder 2e
companion skill** that supplies the rules, the Stolen Lands setting, the three Kingmaker
subsystems, and the **fully atomized Adventure Path**.

Everything runs through honest, shown, scripted dice — the engine never fudges, never softens, and
plays the world to find out what happens.

## Architecture (engine + companion + campaign)

```
.claude/skills/
  mythic-gm/        ← the ENGINE (installed verbatim; do not edit). Runs the scene/Chaos/Fate/
                      Random-Event/Turning-Point loop, the discipline, and all Mythic + AC tables.
  pathfinder2e/     ← the COMPANION (this repo's contribution). A bridge/ fills the engine's hooks:
    SKILL.md          how the two skills combine; how to load the bridge.
    bridge/
      bridge.md           manifest (which hooks override; the machine-readable contract)
      system-profile.md   PF2e resolution: d20 vs DC, four degrees of success, the SKILLS system,
                          three-action combat, dying/death            (hook: resolve)
      interpretation.md   Stolen Lands / Golarion GM lens              (hook: meaning)
      chaos-tendency.md   chaos start/lean/region-floors               (hook: chaos)
      theme-weights.md    fixed Adventure-Crafter weights for Kingmaker(hook: themes)
      subsystems.md       Kingdom Turn / Hexploration / Warfare / clocks (hook: world-tick)
      seeds.md            seed-deck sources                            (hook: seeds)
      setting-canon.md    ground-truth lore (Brevoy, Pitax, Nyrissa, the Lantern King)
      reference/          step-by-step rules the GM follows: pf2e-core, pf2e-character-creation,
                          kingdom-turn, hexploration, warfare
      generators/         list_d100 tables: npc_role, kingdom_event, hex_feature, rumor, army
      adventures/         the ATOMIZED AP — kingmaker-overview.md (master index + seed + the
                          20-milestone arc + Diminisher) and ch01…ch11 cluster/fragment files
campaigns/kingmaker/  ← the LIVE campaign (scaffolded, ready to play)
  campaign-state.md   the human-readable source of truth (frame, snapshot, clocks, recap)
  threads.json        the Threads List      (machine-rollable; the dice roll this)
  characters.json     the Characters List   (machine-rollable; the dice roll this)
  adventure.json      Theme priority + tens-cycle counter
  hexmap.json         explored hexes + revealed sites + usage ledger (Hybrid hexploration)
source/               ← raw Kingmaker AP markdown (gitignored — see "Content & copyright")
```

The engine holds **no** game content; the companion holds **no** oracle. They meet only at the
nine documented hooks. The bridge is validated and every generator roll-tested:

```
python3 .claude/skills/mythic-gm/scripts/bridge.py validate .claude/skills/pathfinder2e/bridge
# → Bridge valid ✓  (9 overrides, 5 generator tables roll-tested)
```

## How the adventure is atomized (and why it surfaces well)

The whole AP is chopped into **clusters** (authored scenes / keyed locations / nodes — framing kept
~whole) holding **fragments** (atomic, page-cited beats). **~300 clusters / ~900 fragments** across
all 11 chapters, each tagged `threads/characters/elements/themes/location` and cited to source.

The engine surfaces this content by **contextual relevance**, never a forced order:
- **Threads & Characters are tracked in JSON** and the dice roll those lists. Discovering a site
  adds its objective to `threads.json` and its NPCs to `characters.json`, so they keep getting
  weighted and **invoked in later Turning Points and Random Events** even after the party moves on.
- **Turning Points** roll the Thread (two-stage over `threads.json`) and auto-invoke a Character
  (firing the Stolen Lands `npc_role` generator on a NEW result).
- **Hexploration is Hybrid:** geography is authoritative *inside* a hex (a keyed hex → its
  `location:<hexcode>` cluster becomes the Expected Scene; an unkeyed hex → a generator roll),
  while Mythic governs pacing, Scene-Test Alterations/Interrupts, and the off-screen world. Linear
  set-piece **dungeons** run as keyed rooms in their own internal geography (`mode: keyed-rooms`).

## Play it

1. Open this repo with Claude Code (the two skills under `.claude/skills/` are auto-discovered).
2. Say e.g. **"Be my GM — let's play solo Kingmaker"** (or "run my Pathfinder 2e Kingmaker game").
   The engine starts at Session Zero: confirm the hardcore frame, build a PF2e PC
   (`pathfinder2e/bridge/reference/pf2e-character-creation.md`), and open in Restov (Ch 1) or at
   Oleg's Trading Post (Ch 3) to start the hexcrawl.
3. Each **Turn**: the engine frames a scene, Scene-Tests it, plays it out (PF2e checks via the
   system profile; Fate Questions for open detail), then bookkeeps — Chaos, the JSON Lists, the
   world-tick subsystems, the seed deck — and asks **"What do you do?"**

The campaign is pre-seeded with the opening Threads (*Settle the Stolen Lands*, *Stop the
banditry*, *Defeat the Stag Lord*, *Who's behind the bandits?*), Characters (Jamandi, Oleg &
Svetlana, the Stag Lord, Tartuccio, Kressle, the Sootscales), and Adventure Features (Oleg's, the
Greenbelt, the Thorn River Camp, the Old Sycamore, the Sootscale Caverns, the Stag Lord's Fort).

## Verify the setup (one smoke-test Turn)

```bash
ENG=.claude/skills/mythic-gm/scripts ; CAMP=campaigns/kingmaker ; BR=.claude/skills/pathfinder2e/bridge

python3 $ENG/build_data.py            # engine tables → VERIFICATION PASSED ✓
python3 $ENG/bridge.py validate $BR   # bridge → Bridge valid ✓
python3 $ENG/bridge.py summary  $BR   # which hooks override
python3 $ENG/state.py list-count $CAMP                       # seeded Threads/Characters
python3 $ENG/adventure_crafter.py turning-point --campaign $CAMP --bridge $BR  # rolls threads.json, auto-invokes a Character
python3 $ENG/tick.py $BR 6            # Kingdom/Hexploration/Warfare/Pitax subsystems report
python3 $ENG/dice.py scene 5         # Scene Test
python3 $ENG/dice.py roll 1d20+9     # a PF2e check (read the degree vs the DC)
```

All randomness lives in those scripts and is shown — that is the point.

## Content & copyright

The Mythic GME 2e / Adventure Crafter tables bundled in the engine are © Tana Pigeon / Word Mill
Games (bundled for personal use). The Kingmaker Adventure Path is © Paizo Inc. **You supply your
own copy of the Kingmaker book.** The raw book text lives in `source/` and is **gitignored** — only
the page-cited atomized digests the engine needs (the bridge) are committed. This repo is for
personal solo play.
