# Hexploration — procedure (Kingmaker Chapter 2)   (world-tick subsystem)

How the party crosses and reveals the Stolen Lands, and the **Hybrid binding** that ties hexes to
the engine's loop. Based on the PF2e hexploration rules (Gamemastery Guide) as used by Kingmaker
Ch 2. Per-hex authored content lives in `adventures/ch02-into-the-wild-*.md` (each site tagged
`location:<hexcode>`); spatial state lives in `campaigns/kingmaker/hexmap.json`.

## The daily procedure
- Each day of overland travel the party has a number of **Hexploration Activities** set by their
  slowest **travel speed** (baseline **2/day**; faster speeds, roads, and mounts can give 3+).
- Spend activities on:
  - **Reconnoiter a hex** — fully explore it: reveals terrain, any **encounter site**, resources,
    and routes. Cost by terrain: **open 1, difficult 2, greater-difficult 3** activities.
  - **Travel** — move through an already-explored hex (cheaper).
  - **Map the Area** (Survival/Cartography), **Fortify Camp**, **Hustle** (extra movement, fatigue),
    **Search** for a known-but-hidden site, **Subsist/Hunt** (Survival).
- Reconnoitering may call for a **PF2e check** (Perception to spot, Survival to traverse, Nature to
  read the land) — resolved on the four-degree ladder; a crit fail can cost extra activities or
  trigger an encounter.

## What's in a hex (Hybrid: geography decides the contents)
On reconnoiter, determine the hex's content:
1. **Keyed encounter site** (the printed map has one here) → load its bridge cluster
   (`location:<hexcode>`); that cluster's scene becomes the **Expected Scene**. Encounter-site types:
   - **Landmark** — obvious, seen from afar; no check to find.
   - **Resource** — materials/worksite for the kingdom (claim later in a Kingdom Turn).
   - **Standard** — a normal keyed encounter found by reconnoitering.
   - **Secret** — hidden; needs a successful Perception/Survival check (or a rumor/clue) to find.
2. **Unkeyed hex** → roll `generators/hex_feature.json` for terrain/feature, and (if an encounter
   occurs — judge by zone danger + CF, or a Fate Question) the **current zone's random-encounter
   table**. Or the hex is simply empty/quiet.
3. Either way, **then run the engine's Scene Test** (`dice.py scene <CF>`): Expected = site/feature
   as found · Altered = it's twisted · Interrupt = a Turning Point fires before the party arrives
   (invoking the Characters List — a patrol, a rival, a fey).

## The 20 zones (level-keyed regions of the Stolen Lands)
Travel deeper = tougher. Use the zone to pick the encounter table and the level baseline for any
on-the-fly statting. (Codes are the hex-site prefixes used in the atomized adventure.)

| Zone | Region | ~Level | Notes / key sites |
|--|--|--|--|
| 0 | Brevoy | — | Restov (BV), Nivakta's Crossing — the launch/safe north |
| 1 | Rostland Hinterlands | 1 | Oleg's Trading Post (RL1), Bokken's hut — first foothold |
| 2 | Greenbelt | 1–3 | Thorn River, Old Sycamore, Sootscale Caverns, Temple of the Elk, Tuskgutter — the starting sandbox |
| 3 | Tuskwater | 3–4 | the Stag Lord's Fort (TW3); future capital site |
| 4 | Kamelands | 5–6 | Candlemere Island, the Lizard King |
| 5 | Narlmarches | 6 | Hargulka's stronghold, the Forgotten Keep, fey |
| 6 | Sellen Hills | 7 | Cradle of Lamashtu (cult of the Bloom) |
| 7 | Dunsward | 8 | Varnhold (DS) |
| 8 | Nomen Heights | 9 | Nomen centaurs |
| 9 | Tors of Levenies | 10 | Vordakai's Tomb (LV6) |
| 10 | Hooktongue | 11 | Fort Drelev, M'Botuu boggards |
| 11 | Drelev | 12 | Speartooth, Fort Drelev environs |
| 12 | Tiger Lords | 13 | Armag's Tomb |
| 13 | Rushlight | 14 | Rushlight Festival grounds (Ch 8) |
| 14 | Glenebon Lowlands | 16 | approach to Pitax |
| 15 | Pitax | 17 | Littletown, Pitax (Irovetti) |
| 16 | Glenebon Uplands | 16–17 | Whiterose, Ilora's camp |
| 17 | Numeria | — | the Mammoth Graveyard |
| 18 | Thousand Voices | 18+ | First-World fey wood; Castle of Knives |
| 19 | Branthlend Mountains | 19 | Ilthuliak's lair, Hungerdark |

## hexmap.json (spatial state — the bridge tracks what the engine doesn't)
A simple ledger updated at bookkeeping:
```json
{ "current_hex": "RL1", "current_zone": 1,
  "explored": ["BV1","RL1"],                  // reconnoitered hexes
  "revealed_sites": ["RL1:Oleg's Trading Post"],
  "claimed_hexes": [],                          // claimed by the kingdom
  "usage_ledger": { "RL1": 1 },               // times a hex's content has surfaced (un-used lean)
  "notes": "Bandits extorting Oleg's; expedition staged here." }
```
The Hexploration subsystem reads/writes this; the **usage ledger** leans the seed deck and cluster
draws toward un-surfaced content (organic coverage, no re-draws — `seeds.md`).
