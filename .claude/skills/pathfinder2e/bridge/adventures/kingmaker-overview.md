# Ingested Adventure — Kingmaker (Stolen Lands)   (hook: adventure-ingest; pure sandbox + keyed dungeons)
fidelity: full   ·   source: Pathfinder Kingmaker Adventure Path (2e hardcover)

This is the **master index** for the atomized AP. The book is chopped into **clusters** (authored
scenes/keyed locations/nodes — scene framing kept ~whole) each holding member **fragments** (atomic
beats), tagged `threads/characters/elements/themes/location` and **cited to source** (page/line).
Per chapter file: `chNN-*.md`. The engine surfaces this content by **contextual relevance** (never a
forced order): Expected Scenes can draw a whole relevant cluster; Turning Points prefer sibling
fragments (cluster cohesion); fragments seed the Lists, the seed deck, and Random-Event invokes.

## Per-content-type mode (how the Scene Test applies)
Each cluster is tagged `mode:`
- **`mode: sandbox`** — open overworld hex sites, settlements, events. Pure sandbox: Altered/
  Interrupt ON; surfaces by relevance + the hexmap usage ledger.
- **`mode: keyed-rooms`** — linear set-piece **dungeons** (Stag Lord's Fort, Sootscale Caverns,
  Vordakai's Tomb, the Troll Lair, Candlemere depths, the House at the Edge of Time, …). Run as
  rooms in their **own internal geography**: fragments = rooms in sequence; Scene-Test only at
  meaningful thresholds (entry, a major branch, a boss room), not every door.

## Cluster index (chapter files)
| File | Chapter | Zones / parts | Mostly |
|---|---|---|---|
| `ch01-call-for-heroes.md` | 1. A Call for Heroes | Restov; Aldori manor | sandbox social + keyed-rooms (manor) |
| `ch02-into-the-wild-hexcrawl-early.md` | 2. Into the Wild (hexcrawl, early) | Hexploration system; Zones 0–6 (Hinterlands→Sellen Hills) | sandbox |
| `ch02-into-the-wild-hexcrawl-late.md` | 2. Into the Wild (hexcrawl, late) | Zones 7–19 (Dunsward→Branthlend); rumor/encounter tables | sandbox |
| `ch02-into-the-wild-dungeons.md` | 2. Into the Wild (dungeons) | Old Sycamore, Sootscale, Lonely Barrow, Isle of the Lizard King, Candlemere, Forgotten Keep, M'Botuu | keyed-rooms |
| `ch03-stolen-lands.md` | 3. Stolen Lands | Oleg's; Thorn River Camp; Stag Lord's Fort | sandbox + keyed-rooms |
| `ch04-rivers-run-red.md` | 4. Rivers Run Red | Founding & kingdom events; Troll Lair; the Beast's Den | sandbox + keyed-rooms |
| `ch05-cult-of-the-bloom.md` | 5. Cult of the Bloom | Hunting Lodge; Glenebon; Cradle of Lamashtu | sandbox + keyed-rooms |
| `ch06-varnhold-vanishing.md` | 6. The Varnhold Vanishing | Varnhold; the Nomen; Vordakai's Tomb | sandbox + keyed-rooms |
| `ch07-blood-for-blood.md` | 7. Blood for Blood | Tatzlford; Fort Drelev (warfare); Armag's Tomb | sandbox + warfare + keyed-rooms |
| `ch08-war-of-the-river-kings.md` | 8. War of the River Kings | Rushlight; infiltration of Pitax; Irovetti's palace | sandbox + warfare + keyed-rooms |
| `ch09-they-lurk-below.md` | 9. They Lurk Below | Candlemere contested level; Foras | keyed-rooms |
| `ch10-sound-of-a-thousand-screams.md` | 10. Sound of a Thousand Screams | the Bloom; Thousandbreaths; House at the Edge of Time | sandbox + keyed-rooms |
| `ch11-curse-of-the-lantern-king.md` | 11. Curse of the Lantern King | twin conclusions; the Lantern Kingdom | keyed-rooms |

## Diminisher (solo scaling)
The AP assumes a **4-PC party**. For a single solo PC the default **Diminisher = ¼** of the printed
encounter budget (use weak adjustments, fewer foes, or down-tiered creatures; apply to the
on-the-fly statting benchmarks in `reference/pf2e-core.md`). Tune to the actual table: 2 PCs ≈ ½,
3 PCs ≈ ¾, a PC + companion/animal ≈ ⅓–½. The engine's honest dice still decide; the Diminisher
only sets the challenge scale so a lone hero isn't auto-killed.

## Story-milestone level arc (20 beats — the campaign's spine, not a railroad)
Use as soft level gates; the dice still decide *how* each is reached (or skipped).

| → Level | Milestone | Where |
|--|--|--|
| 2 | Defend Oleg's Trading Post | Ch 3 p1 |
| 3 | Defeat the Thorn River bandits | Ch 3 p2 |
| 4 | Defeat the Stag Lord | Ch 3 p3 |
| 5 | Complete your first Kingdom Turn | Ch 4 p1 |
| 6 | Defeat Hargulka & the Beast | Ch 4 p2–3 |
| 7 | Discover the Cradle of Lamashtu | Ch 5 p1–2 |
| 8 | Defeat the Cult of the Bloom | Ch 5 p3 |
| 9 | Reach Vordakai's Tomb | Ch 6 p1–3 |
| 10 | Defeat Vordakai | Ch 6 p4 |
| 11 | Defend Tatzlford | Ch 7 p1 |
| 12 | Liberate Fort Drelev | Ch 7 p2 |
| 13 | Defeat Armag the Twice-Born | Ch 7 p3 |
| 14 | Complete the Rushlight Festival | Ch 8 p1 |
| 15 | Rescue Evindra / break Pitax's hold | Ch 8 p3–4 |
| 16 | Defeat King Irovetti | Ch 8 p5 |
| 17 | Defeat Foras | Ch 9 p2 |
| 18 | Find the way into Thousandbreaths | Ch 9 p2 |
| 19 | Reach the House at the Edge of Time | Ch 10 p2–3 |
| 20 | Confront Nyrissa (defeat / forgive / ally) — then the Lantern King | Ch 10 p3 → Ch 11 |

## Global seed — load these into the campaign's JSON Lists at Session Zero / on discovery
(Use `state.py thread|char add <campaign> "<name>"`. Seed the **opening** now; add the rest as the
PC reaches them — Player ≠ PC knowledge for [HIDDEN] entries.)

**Threads (objectives):**
- Settle & claim the Stolen Lands (the master charter goal) — *active from the start*
- Stop the banditry plaguing the Greenbelt / Oleg's — *opening*
- Defeat the Stag Lord — *opening (rumored)*
- Who is really behind the bandits? *(→ Pitax)* [HIDDEN] — *opening as a question*
- Found and grow your kingdom *(opens Ch 4)*
- The vanishings & the fey wrongness *(seeds toward Ch 6 / the curse)* [HIDDEN]
- (later) Survive the rivals: Drelev, the Tiger Lords, Pitax; (endgame) the Bloom & Nyrissa [HIDDEN]

**Characters (NPCs/forces):**
- Lady Jamandi Aldori (patron), Oleg & Svetlana Leveton (first allies), the Stag Lord (antagonist),
  Tartuccio (rival), Kressle (bandit lt.), the Sootscale kobolds (faction) — *opening seeds*
- Akiros Ismort, Hargulka, Maegar Varn, Vordakai, Hannis Drelev, Armag, King Irovetti, Evindra,
  Nyrissa [HIDDEN], the Lantern King [HIDDEN] — *add on discovery*

**Adventure Features (locations/hazards):**
- Oleg's Trading Post, the Greenbelt (Zone 2), the Thorn River Bandit Camp, the Old Sycamore,
  the Sootscale Caverns, the Stag Lord's Fort — *opening*; the wider zones/dungeons as revealed.

## How a chapter file is structured (schema each `chNN-*.md` follows)
```
### cluster: <id> — "<scene name>"   (source: p.NN / line LNNNN)   mode: sandbox|keyed-rooms
scene: <authored framing, kept ~whole>
threads: [...]   characters: [...]   elements: [...]   themes: [...]   location: <hexcode/area>
gate: <optional soft precondition, else none>
fragments:
  - plot_point: "<a beat>"   themes: [...]   weight: 1
  - plot_point: "<another>"  themes: [...]   weight: 1
```
