# Ingested Adventure — Kingmaker Chapter 2: Into the Wild — Hexcrawl (early, Zones 0–6)   (hook: adventure-ingest)
fidelity: full   ·   source: Kingmaker AP 2e, Chapter 2, lines 1931–4400

Atomization of the hexploration SYSTEM plus every keyed encounter site in the EARLY zones
(0 Brevoy → 6 Sellen Hills). Big keyed dungeons (Old Sycamore GB14, Sootscale GB20, Lonely Barrow
TW5, Lizard King KL3, Candlemere KL4, Forgotten Keep NM5) and the Stag Lord's Fort (TW3) are only
*stubbed* here (their interiors live in `ch02-into-the-wild-dungeons.md` and the Ch3/Ch4 files).
All clusters `mode: sandbox`; the engine surfaces by relevance + hexmap ledger, never forced order.

---

### cluster: hex-system — "Hexploring the Stolen Lands"   (source: p.45-49 / L1975)   mode: sandbox
scene: The Stolen Lands (~35,000 sq mi of contested wilderness between Brevoy and the River Kingdoms) is a 20-zone hex map, one hex = 12 miles, run with the Gamemastery Guide hexploration rules (GMG 172-173). Zones 1–19 are keyed to a suggested party level (Zone 0 Brevoy is unkeyed/unsettleable); a zone's level signals the threats there. Each hex may hold an encounter site, tagged with one of four discovery traits — **Landmark** (auto-spotted from any adjacent open hex when Traveling), **Resource** (kingdom-building materials, flagged once kingdom play starts), **Standard** (found by Reconnoitering, or by Traveling in open terrain), **Secret** (found only via NPC tip or a specific skill action). FAIR WARNING guidance: warn players before a hex keyed 4+ levels above them (danger signs, dead monsters, distant giants). Random encounters/hazards: each zone has its own d20 wandering-monster table (flat check or GM fiat), plus reusable hazards (quicksand, yellow mold, scree, flash floods). RUMORS: Gather Information at Oleg's or via friendly NPCs rolls on per-zone rumor tables (success = 1 rumor of current region; crit = 2, or 1 from elsewhere); some rumors are flagged false. Optional camping & weather subsystems (Companion Guide) add fortifying camps, meals, and a quick 3-die temp/precip/wind weather toss. Connections: this procedure governs every other cluster in zones 0–6.
threads: [Settle & claim the Stolen Lands, Stop the Greenbelt banditry, Defeat the Stag Lord]   characters: [Lady Jamandi Aldori, Nyrissa]   elements: [hexploration, exploration mode, kingdom resources, wandering encounters, rumors, fair-warning]   themes: [exploration, sandbox-freedom, frontier-danger]   location: Stolen Lands (whole map)
gate: none
fragments:
  - plot_point: "20-zone map, one hex = 12 mi; zones keyed to suggested level (0 Brevoy unkeyed). Use GMG hexploration (Travel/Reconnoiter/Map the Area/Subsist/Search as individual activities)."   themes: [exploration, structure]   weight: 1
  - plot_point: "Four site-discovery traits: Landmark (auto from adjacent open hex), Resource (kingdom value), Standard (Reconnoiter, or Travel in open terrain), Secret (NPC tip or specific skill action)."   themes: [discovery, mechanics]   weight: 1
  - plot_point: "Fair Warning: hexes 1 level up = no warning needed; 2-3 up = let them find out, be ready to help; 4+ up = signal danger (signs, dead monsters, distant titans, NPC rumors)."   themes: [frontier-danger, gm-aid]   weight: 1
  - plot_point: "Random encounters via per-zone d20 tables (flat check or fiat); spice with reskinned hazards (quicksand/yellow mold/scree/flash flood)."   themes: [wandering-encounters, hazards]   weight: 1
  - plot_point: "Rumors gathered via Gather Information (esp. at Oleg's from Svetlana/Oleg/travelers) on per-zone tables; some flagged false; even false rumors bait adventure."   themes: [rumors, social]   weight: 1
  - plot_point: "Optional camping (Companion Guide 106-119) & weather (120-125 or quick 3-die temp/precip/wind) layers. [convert camping/weather to list_d## generators if desired]"   themes: [camping, weather, flavor]   weight: 1

### cluster: rumor-central — "Central Stolen Lands Rumors (zones 1–6)"   (source: p.49 / L2092)   mode: sandbox
scene: The d20 rumor table heard in Brevoy and zones 1–6 (roll 1d10 to keep low-level PCs to safe sites). Seeds nearly every early plot thread: the Stag Lord's rise, the bone-amulet bandits, Davik Nettles' haunting at the ruined bridge, kobolds/gremlins in the Kamelands, the Hooktongue boggard blockade, the ruined Gyronna monastery now used as the Stag Lord's fort, the vanishing Narlmarches unicorn, unnatural First-World flora, a lost wizard's spellbook, the hateful hermit in his hollow tree, the SP1 drake mistaken for a red dragon, Jubilost's gnome mapping expedition, the Swamp Witch (Old Beldame), a wandering hill giant, a haunted elven ruin, the lizard king, and the Candlemere tower. Several entries are explicitly false or partially false. [convert to list_d20 generator — note false flags inline]
threads: [Stop the Greenbelt banditry, Defeat the Stag Lord, The fey wrongness & vanishings]   characters: [the Stag Lord, Davik Nettles, the Old Beldame, Jubilost Narthropple, the hateful hermit, Nyrissa]   elements: [rumor table, foreshadowing, false rumors]   themes: [rumors, foreshadowing, mystery]   location: Brevoy / zones 1-6
gate: none
fragments:
  - plot_point: "Stag Lord rumors: new bandit leader dressed in bones; bandits wear stag-skull amulets (the demon-cult claim is FALSE); ruined Gyronna monastery on the Tuskwater is now his hideout."   themes: [the-stag-lord, foreshadowing]   weight: 1
  - plot_point: "Davik Nettles rumor: bandits ruined the SE Shrike bridge; the old bridge keeper now haunts it (true — leads to GB15)."   themes: [haunting, hook]   weight: 1
  - plot_point: "Narlmarches unicorn sightings have stopped (NM3 dead unicorn / Nyrissa's trophy); strange unnatural flora & fungi spreading (First-World foreshadow)."   themes: [mystery, first-world, foreshadowing]   weight: 1
  - plot_point: "False/partial leads: Breeg joined a Thorn-River bandit camp (FALSE), Swamp Witch boils children (FALSE — she's the harmless Old Beldame), a red dragon in the Narlmarches (FALSE — it's the SP1 drake), Stag Lord risen as undead (FALSE, post-Ch3 only)."   themes: [false-rumors, misdirection]   weight: 1
  - plot_point: "Lost-wizard spellbook rumor → forgotten cache at GB9; hateful hermit (Bokken's brother) in a hollow tree to the south → TW6; gnome explorers mapping the Greenbelt up the Skunk River → Jubilost at TW2."   themes: [hooks, treasure]   weight: 1

---

### cluster: bv1-restov — "Restov"   (source: p.51 / L2180)   mode: sandbox
scene: LANDMARK. The large city (Settlement 9, CN, pop 18,670) is Rostland's cultural heart, birthplace of the Aldori dueling style, and the campaign's launch point — a wealthy border trade city seething with anti-Surtova/anti-Issian sentiment. It is the PCs' best high-end buy/sell hub until their own settlements mature, and the seat of their long-term patron. Key NPCs: Lord-Mayor Ioseph Sellemius, the renowned swordlord Jamandi Aldori (CG half-elf swordlord 14), and Erastil's high priest Ezvanki Keegh. Aldori dueling swords and the Aldori Duelist archetype are available here.
threads: [Settle & claim the Stolen Lands]   characters: [Jamandi Aldori, Ioseph Sellemius, Ezvanki Keegh]   elements: [city, market, patron, Aldori swordlords]   themes: [civilization, politics, patronage]   location: BV1
gate: none
fragments:
  - plot_point: "Restov is the high-end shopping hub and the seat of patron Jamandi Aldori; political unrest vs. Issia/Surtova simmers in its dueling schools and taprooms."   themes: [market, politics, patronage]   weight: 1

### cluster: bv2-nivakta — "Nivakta's Crossing"   (source: p.52 / L2208)   mode: sandbox
scene: LANDMARK. The southernmost village of Rostland (Settlement 1, CN village, pop 140) on the Shrike River, a palisaded post of serious, humorless traders/trappers; a low bridge with guard towers crosses to the southern wilds. Gossipy locals grant +2 to Gather Information here. This is where Maegar Varn's mercenaries cross to found Varnhold. NPCs: Mayor Irven Revanisu, Sheriff Lorin Kaven, Pharasmin cleric Kara Ilarenika.
threads: [Settle & claim the Stolen Lands]   characters: [Irven Revanisu, Lorin Kaven, Maegar Varn]   elements: [village, river crossing, rumor mill]   themes: [frontier, civilization]   location: BV2
gate: none
fragments:
  - plot_point: "Border village & bridge to the wilds; gossipy folk give +2 to Gather Information. Maegar Varn's column crosses here en route to found Varnhold (foreshadows Ch6)."   themes: [rumors, foreshadowing]   weight: 1

---

### cluster: rl1-olegs — "Oleg's Trading Post"   (source: p.53-55 / L2258)   mode: sandbox
scene: LANDMARK RESOURCE. The true starting hub of the campaign: a rebuilt fort run by Oleg Leveton (Creature 1) and his wife Svetlana (Creature 1), who on first arrival are dreading an imminent bandit raid (the defense is Ch3). After the Stag Lord falls, mercenary Kesten Garess (CN fighter 3) and later the disgraced Erastil druid Jhod Kavken (NG druid 4) arrive as fixtures. The post is the PCs' safe haven for rest, downtime, shopping (assume any affordable CRB gear; rare items special-ordered in 2d6+4 days), selling loot, hearing rumors, and picking up wanted posters. Mechanically a Refuge if the hex is Claimed (or a free General Store if a settlement is built). Hub for many early quests (Oleg's Trophy, Radish Soup, Svetlana's Ring, wanted posters, Find Falgrim, Vision of the Elk). Connections: gateway to the whole Greenbelt; ties to GB4 (radishes), GB6/NM (Temple of the Elk), GB20 Sootscale.
threads: [Stop the Greenbelt banditry, Settle & claim the Stolen Lands, Defeat the Stag Lord]   characters: [Oleg Leveton, Svetlana Leveton, Kesten Garess, Jhod Kavken]   elements: [trading post, safe haven, market, quest hub, wanted posters, Refuge]   themes: [home-base, allies, civilization]   location: RL1
gate: none
fragments:
  - plot_point: "Oleg & Svetlana run the post; first visit they fear a bandit raid (the defense itself is Ch3). Once defended, it's a free safe haven / Refuge for rest, downtime, shopping and selling."   themes: [home-base, allies]   weight: 1
  - plot_point: "Oleg's Trophy (10 XP): bring an intact tatzlwyrm head → Oleg's 5 lover's knots. (Tatzlwyrms live at GB16.)"   themes: [quest, reward]   weight: 1
  - plot_point: "Radish Soup (10 XP): bring Svetlana a basket of moon radishes from GB4 → 15 gp + moon-radish soup unlocked."   themes: [quest, errand]   weight: 1
  - plot_point: "Svetlana's Ring (30 XP): recover her stolen wedding ring from the bandits → 50 gp trading-post credit."   themes: [quest, bandits]   weight: 1
  - plot_point: "Wanted posters (from Restov Swordlords): WANTED Kobolds (30 XP, pacify/ally Sootscale → 40 gp), WANTED Tuskgutter (10 XP, the boar's head → Vekkel's composite longbow + 3 beacon shot arrows), WANTED Bandits (30 XP, defeat 6 bandits → 30 gp)."   themes: [bounties, hooks]   weight: 1
  - plot_point: "Kesten Garess arrives (CN fighter 3 + 3 mercenaries) after the bandit defense — moody guard, potential ally; gives quest FIND FALGRIM (30 XP, capture Varisian turncoat Falgrim Sneeg alive → three +1 weapons, or one if dead)."   themes: [allies, quest]   weight: 1
  - plot_point: "Jhod Kavken arrives later (NG druid 4, exiled Erastil priest seeking redemption); gives VISION OF THE ELK (30 XP) — find & cleanse the Temple of the Elk at GB6 → Jhod grants free spellcasting for life (PCs supply costly components)."   themes: [allies, quest, erastil]   weight: 1

### cluster: rl2-bokken — "Bokken's Hut"   (source: p.56 / L2448)   mode: sandbox
scene: STANDARD RESOURCE. The hut of eccentric, bird-twitchy alchemist Bokken (CN human alchemist 4), who sells potions (typically 2 minor healing, 2 lesser healing, 1 moderate healing, 1 lesser fire-resistance, 1 lesser cold-resistance) — usually to Oleg, but to the PCs if asked. He bitterly mentions his estranged, abusive younger brother Kurmil, who cut off Bokken's pinkie and fled to live "in a hollow tree down south" (the hateful hermit at TW6). Resource: a free Alchemy Laboratory if a settlement is built here. Quest: GATHERING FANGBERRIES.
threads: [Stop the Greenbelt banditry]   characters: [Bokken, the hateful hermit]   elements: [alchemist, potions shop, Alchemy Lab]   themes: [allies, commerce, family-grudge]   location: RL2
gate: none
fragments:
  - plot_point: "Bokken sells healing & resistance potions; bitterly recalls his brother who fled to a hollow tree south — the hateful hermit (TW6)."   themes: [merchant, foreshadowing]   weight: 1
  - plot_point: "GATHERING FANGBERRIES (30 XP): fetch a full basket from the fangberry thicket (GB18) → 25% off potions for a month, or any 3 in-stock potions free."   themes: [quest, errand]   weight: 1

### cluster: rl3-spider-nest — "Spider Nest"   (source: p.57 / L2592)   mode: sandbox
scene: STANDARD, Low 1. A web-lined, 25-ft-deep shaft (DC 10 Athletics to climb) is the den of a pony-sized **giant trapdoor spider** (Creature 2; Trapdoor Lunge reaction; jaws +11, 1d10+3 + incapacitation venom DC 18). Bones of boars/deer/bears/humans ring the den ~200 ft out. Treasure: a bandit corpse with leather, shortsword, 10 sp, a silver Stag Lord amulet (3 gp), and a blood-X treasure map to the lightning-struck oak at GB9.
threads: [Defeat the Stag Lord]   characters: []   elements: [spider lair, ambush predator, treasure map]   themes: [wilderness-danger, treasure]   location: RL3
gate: none
fragments:
  - plot_point: "Giant trapdoor spider (Creature 2) lurks in a 25-ft web shaft; Trapdoor Lunge surprise; venom DC 18 (paralyze at stage 3)."   themes: [combat, ambush]   weight: 1
  - plot_point: "Treasure: dead bandit with a Stag Lord amulet and a crude blood-X map pointing to the forgotten cache at GB9 (claw-shaped dead tree)."   themes: [treasure, clue]   weight: 1

### cluster: rl4-crooked-falls — "Crooked Falls"   (source: p.57 / L2616)   mode: sandbox
scene: LANDMARK. The Shrike River cascades over five waterfalls (10-30 ft drops) across a mile, where the Crooked River joins. These falls (plus Shrike Cascade GB10) make the Shrike useless for trade, so river commerce runs the East Sellen through Hooktongue instead. DC 20 Athletics to clamber the banks.
threads: [Settle & claim the Stolen Lands]   characters: []   elements: [waterfalls, river terrain]   themes: [scenery, terrain-obstacle]   location: RL4
gate: none
fragments:
  - plot_point: "Five-stage Shrike waterfall (DC 20 Athletics to climb banks); explains why trade avoids the Shrike for the East Sellen/Hooktongue route."   themes: [terrain, lore]   weight: 1

### cluster: rl5-fort-serenko — "Fort Serenko"   (source: p.57 / L2726)   mode: sandbox
scene: RESOURCE STANDARD. An empty wooden border fort, recently and orderly abandoned as soldiers were recalled to Restov amid Rostland-Issia tensions. Resource: a Structure terrain feature / Barracks if Claimed or settled — but it lies in Rostland's claimed holdings, so incorporating it without prior diplomacy raises Rostland's Negotiation DC to 20.
threads: [Settle & claim the Stolen Lands]   characters: []   elements: [abandoned fort, Barracks, political friction]   themes: [politics, kingdom-building]   location: RL5
gate: none
fragments:
  - plot_point: "Empty border fort = free Barracks if Claimed/settled, but claiming it without diplomacy raises Rostland's Negotiation DC to 20 (seen as aggressive)."   themes: [kingdom-building, politics]   weight: 1

### cluster: rl6-dead-noble — "Dead Noble"   (source: p.58 / L2798)   mode: sandbox
scene: SECRET. Empty until the post-kingdom quest "A Missing Brother" (Edrist Hanvaki, Appx 2 p.521) activates. Then the body of his sibling Temin — who slipped and broke his neck en route to Varnhold — lies in a gulch, found via wheeling buzzards (DC 13 Hills/Hunting/Nature/Survival or DC 17 Perception). Treasure: a mother-of-pearl brooch (10 gp) Edrist seeks.
threads: [Settle & claim the Stolen Lands]   characters: [Edrist Hanvaki, Temin Hanvaki]   elements: [secret site, corpse, kingdom quest]   themes: [mystery, kingdom-events]   location: RL6
gate: kingdom established & "A Missing Brother" quest active
fragments:
  - plot_point: "Secret: after kingdom quest 'A Missing Brother' activates, find Temin Hanvaki's body (buzzards, DC 13/17 checks) wearing a 10 gp brooch Edrist wants."   themes: [mystery, kingdom-quest]   weight: 1

---

### cluster: gb1-snare-glade — "Snare-Filled Glade"   (source: p.59 / L2826)   mode: sandbox
scene: STANDARD, Trivial 2. The cruel trapper Breeg Orlivanch's hidden trapping grounds. Breeg's Traps (Hazard 3, Stealth DC 20, Disable DC 17 Survival): dozens of bear-trap spike snares — Traveling snaps 1 PC, Reconnoitering snaps 1d4; each does a bear-trap Strike +14 (2d10+7). Triggers up to 5 times. Salvage: materials for 6 spike snares if all disarmed.
threads: []   characters: [Breeg Orlivanch]   elements: [trap hazard, snares]   themes: [wilderness-danger, traps]   location: GB1
gate: none
fragments:
  - plot_point: "Breeg's Traps (Hazard 3): hidden bear-trap snares, +14 to hit 2d10+7; Travel snaps 1 PC / Reconnoiter snaps 1d4; DC 17 Survival to disarm (salvages 6 spike snares)."   themes: [hazard, traps]   weight: 1

### cluster: gb2-dead-trapper — "Dead Trapper"   (source: p.59 / L2850)   mode: sandbox
scene: STANDARD. Breeg Orlivanch lies pinned under his own collapsed deadfall — but it was murder: the faerie dragon Perlivash (GB3), sick of Breeg's cruelty, cut the ropes (DC 14 Perception/Survival reveals cut ropes; crit finds a faerie-dragon tooth, DC 21 Arcana to ID as Perlivash's). Treasure: a cold iron hatchet, supplies, materials for 3 spike snares, 3 beaver pelts (1 gp ea), skinning knife, leatherworker's tools.
threads: []   characters: [Breeg Orlivanch, Perlivash]   elements: [corpse, murder clue, fey mischief]   themes: [mystery, fey, treasure]   location: GB2
gate: none
fragments:
  - plot_point: "Breeg found dead under his own deadfall — actually killed by the faerie dragon Perlivash (cut ropes, DC 14; tooth clue DC 21 Arcana ties to GB3)."   themes: [mystery, fey]   weight: 1

### cluster: gb3-fairy-nest — "Fairy Nest"   (source: p.60-61 / L2860)   mode: sandbox
scene: HIDDEN, Moderate 2. Home of the grig **Tyg-Titter-Tut** (Creature 1) and the faerie dragon **Perlivash** (Creature 2), good-hearted tricksters who initially mistake the PCs for bandits and trail them, playing pranks twice/day (ghost sound, dancing lights, prestidigitation) while secretly guarding them. PCs can deduce fey are responsible (DC 16 Nature/Forest, DC 14 Fey Lore), catch one in the act (Search + DC 17-20 Perception), and appease with gifts worth 5+ sp + DC 20 Diplomacy (cold iron is hated). Befriended, they map the Thorn River bandit camp (GB7), and reveal GB1 traps, GB4 radishes, GB5 hot springs, and GB6 Temple of the Elk; they may later visit the PCs' kingdom. They killed Breeg (GB2) and admit it bashfully if asked. Reward: XP as if defeated + recurring fey ally.
threads: [Stop the Greenbelt banditry]   characters: [Tyg-Titter-Tut, Perlivash]   elements: [fey, tricksters, informants, gift-diplomacy]   themes: [fey, allies, mischief]   location: GB3
gate: none
fragments:
  - plot_point: "Grig Tyg-Titter-Tut & faerie dragon Perlivash prank the party (twice/day) but secretly protect them; appease with gifts (5+ sp) + DC 20 Diplomacy; cold iron is hated."   themes: [fey, mischief]   weight: 1
  - plot_point: "Befriended, they reveal the Thorn River bandit camp (GB7, with a dirt map & headcount) plus GB1 traps, GB4 radishes, GB5 springs, GB6 Temple; can recur as kingdom allies. (They killed Breeg at GB2.)"   themes: [allies, intel]   weight: 1

### cluster: gb4-radish-patch — "Radish Patch"   (source: p.61 / L2904)   mode: sandbox
scene: STANDARD, Low 2. An arrowhead clearing of delicious moon radishes (the GB4 source for Svetlana's Radish Soup quest). Four **kobold warriors** (Creature -1) lie bloated and sickened 1 from gorging, with three baskets of radishes — but they fight to the death to defend "their" patch.
threads: [Stop the Greenbelt banditry]   characters: []   elements: [resource patch, kobolds]   themes: [errand, combat]   location: GB4
gate: none
fragments:
  - plot_point: "Moon-radish patch (for the Radish Soup quest) guarded by 4 gorged, sickened kobold warriors (Creature -1) who fight to the death."   themes: [errand, combat]   weight: 1

### cluster: gb5-frog-pond — "Frog Pond"   (source: p.61 / L2918)   mode: sandbox
scene: STANDARD, Low 2. Two rotten-egg-smelling hot springs at the source of the Skunk River feed a 150-ft swampy pond home to a pair of aggressive **giant frogs** (Creature 1); a frog below 10 HP flees into the pond.
threads: []   characters: []   elements: [hot springs, giant frogs]   themes: [wilderness-danger]   location: GB5
gate: none
fragments:
  - plot_point: "Sulfurous hot springs & pond at the Skunk River's source; 2 giant frogs (Creature 1) attack approachers."   themes: [combat, terrain]   weight: 1

### cluster: gb6-temple-elk — "Temple of the Elk"   (source: p.61-63 / L2938)   mode: sandbox
scene: HIDDEN RESOURCE, Moderate 2. An overgrown Erastil shrine carved into a 100-ft elk-faced escarpment with a 50-ft cave mouth and an algae-choked pool (found via DC 16 Perception, or the GB3 fey's directions). Its mad last keeper sacrificed a grizzly bear "to any who would answer," fell from grace, and his cruel spirit reanimated the bear. The **Cursed Guardian** (Creature 4, unique; Deadeye's Shame = weakness 5 / -2 saves vs. Erastil worshippers, Rush, Mauler) bellows out of the cave when it hears speech — give PCs a chance to flee first; it fights to the death in its lair. This is the target of Jhod's "Vision of the Elk" quest. Once slain, the bear crumbles to dust, the shrine revives, and the pool grants a moderate-healing effect (first drink only, 24 hrs). Restore the Temple of the Elk (Downtime Leadership: 1d6 RP + DC 25 Folklore) → Refuge / free Shrine, with Erastil's boon on a crit.
threads: [Settle & claim the Stolen Lands]   characters: [the Cursed Guardian, Jhod Kavken]   elements: [ruined shrine, cursed bear, Erastil, healing pool, Refuge]   themes: [erastil, redemption, undead-ish, kingdom-building]   location: GB6
gate: none
fragments:
  - plot_point: "Overgrown Erastil shrine (DC 16 Perception to find) guarded by the Cursed Guardian (Creature 4 unique reanimated grizzly); it frenzies at the sound of speech and has weakness 5 to Erastil worshippers (Deadeye's Shame)."   themes: [combat, erastil, curse]   weight: 1
  - plot_point: "Completes Jhod's VISION OF THE ELK. Slain, the bear becomes a peaceful old man then dust; the pool gives a one-time moderate-healing drink (24 hrs)."   themes: [quest, redemption]   weight: 1
  - plot_point: "Restore the Temple (Downtime Leadership: 1d6 RP + DC 25 Folklore) → Refuge / free Shrine; crit grants Erastil's boon (no crit-fail on Subsist). Crit-fail collapses the cavern (Decay + 1d4 Unrest, +4 DC)."   themes: [kingdom-building, erastil]   weight: 1

### cluster: gb7-thorn-river-camp — "Thorn River Bandit Camp"   (source: p.63 / L3010)   mode: sandbox
scene: STANDARD. Stub only — the bandit camp is fully detailed in Ch3 Part 2 (p.168). A key early target in the war on the Stag Lord's bandits; the GB3 fey can provide a map and roster.
threads: [Stop the Greenbelt banditry, Defeat the Stag Lord]   characters: [Kressle]   elements: [bandit camp, set-piece]   themes: [bandits, the-stag-lord]   location: GB7
gate: none
fragments:
  - plot_point: "Thorn River Bandit Camp — detailed in Ch3 (p.168); a major bandit set-piece. GB3 fey can supply a map and headcount."   themes: [bandits, set-piece]   weight: 1

### cluster: gb8-gold-mine — "Gold Mine"   (source: p.63 / L3014)   mode: sandbox
scene: HIDDEN RESOURCE. A hidden crevice (DC 16 Perception/Hills Lore while Reconnoitering) opens to a cave with a glittering gold-ore vein (DC 16 Nature/Mining Lore to ID). Resource: doubles a Mine's output established here.
threads: [Settle & claim the Stolen Lands]   characters: []   elements: [hidden cave, gold vein, Mine resource]   themes: [kingdom-building, treasure]   location: GB8
gate: none
fragments:
  - plot_point: "Hidden gold-ore vein (DC 16 to find/ID) → doubles the output of a Mine established here."   themes: [kingdom-resource]   weight: 1

### cluster: gb9-forgotten-cache — "Forgotten Cache"   (source: p.63-64 / L3020)   mode: sandbox
scene: HIDDEN. A lone lightning-struck oak on a low hill (claw-shaped from the north) hides loot a bandit stashed from the Stag Lord — and was executed for; the RL3 map points here. Disturbed ground found via DC 20 Survival to Track; 10 min to dig. Treasure: a +1 dagger, a wand of burning hands, a silver ring (10 gp), and a rain-damaged spellbook with 5 legible spells (dispel magic, illusory object, mage armor, shrink, unseen servant).
threads: [Defeat the Stag Lord]   characters: []   elements: [buried treasure, spellbook, landmark tree]   themes: [treasure, clue-payoff]   location: GB9
gate: none
fragments:
  - plot_point: "Buried cache under the claw-shaped oak (DC 20 Survival/Track; map from RL3): +1 dagger, wand of burning hands, silver ring, and a spellbook with 5 salvageable spells."   themes: [treasure, payoff]   weight: 1

### cluster: gb10-shrike-cascade — "Shrike Cascade"   (source: p.64 / L3030)   mode: sandbox
scene: LANDMARK. A single 50-ft Shrike waterfall, impassable by boat but a breathtaking vista; DC 20 Athletics to climb the slick cliff edge.
threads: []   characters: []   elements: [waterfall, terrain]   themes: [scenery, terrain-obstacle]   location: GB10
gate: none
fragments:
  - plot_point: "50-ft Shrike waterfall, impassable by boat; DC 20 Athletics to climb the edge."   themes: [terrain]   weight: 1

### cluster: gb11-boggard-lair — "Boggard Lair"   (source: p.64-65 / L3040)   mode: sandbox
scene: STANDARD RESOURCE, Moderate 2. Two ruined stone buildings in a mire claimed by the exiled boggard **Garuum** (Creature 2) and his slurk pet **Ubagub** (Creature 2). Exiled from M'botuu (HT6) for a failed coup (he ate the knot's sacred blue dragonflies), Garuum just wants to be left alone and croaks "Truce!"; he knows ~10 Common words. Befriended/spared, he reveals NM2 Erastil statue, GB6 Temple, GB12 Tuskgutter, GB16 tatzlwyrms, and may host or join the party. Treasure: 21 gp + gems (iolite 5gp, spinel 9gp, blue quartz 11gp). Resource: Refuge if Claimed / Houses if settled. Quest GARUUM'S REVENGE (level 10): kill M'botuu's priest-king Sepoko → greater invisibility armor runestone.
threads: [Settle & claim the Stolen Lands]   characters: [Garuum, Ubagub, Sepoko]   elements: [boggard exile, slurk, informant, Refuge]   themes: [unlikely-ally, frontier-diplomacy]   location: GB11
gate: none
fragments:
  - plot_point: "Exiled boggard Garuum + slurk Ubagub (both Creature 2) croak 'Truce!'; befriend/spare him for intel on NM2, GB6, GB12, GB16 and possible hosting/companionship."   themes: [unlikely-ally, intel]   weight: 1
  - plot_point: "Resource: Refuge if Claimed / Houses if settled. GARUUM'S REVENGE (30 XP, level 10): kill priest-king Sepoko at M'botuu → greater invisibility armor runestone."   themes: [kingdom-resource, quest]   weight: 1

### cluster: gb12-tuskgutter — "Tuskgutter's Lair"   (source: p.65-66 / L3094)   mode: sandbox
scene: STANDARD, Low 2. The notorious gray-bristled boar **Tuskgutter** (Creature 3, elite boar) lairs in a hollow under a fallen pine. Roll DC 6 flat check: home or returns in 1d6 hrs. Target of the WANTED: Tuskgutter quest (head → Vekkel Benzen's composite longbow + 3 beacon shot arrows).
threads: [Stop the Greenbelt banditry]   characters: [Tuskgutter, Vekkel Benzen]   elements: [legendary boar, bounty]   themes: [hunt, bounty]   location: GB12
gate: none
fragments:
  - plot_point: "Tuskgutter (Creature 3 elite boar); DC 6 flat check if home. Kill for the WANTED bounty → Vekkel's composite longbow + 3 beacon shot arrows."   themes: [hunt, bounty]   weight: 1

### cluster: gb13-rickety-bridge — "Rickety Bridge"   (source: p.66 / L3112)   mode: sandbox
scene: LANDMARK, Trivial 2. An old wooden bridge over a 20-ft Thorn River gulch, safe for one Medium / two Small at a time. Rickety Bridge (Hazard 4, Stealth DC 22, Disable Crafting DC 25): if 2+ Medium or a Large crosses, it collapses — fallers take 2d8+5 from debris (DC 21 basic Reflex), then DC 20 Athletics to swim the churning water.
threads: []   characters: []   elements: [collapsing bridge hazard]   themes: [terrain-obstacle, hazard]   location: GB13
gate: none
fragments:
  - plot_point: "Rickety Bridge (Hazard 4): collapses under 2+ Medium/1 Large crossers; 2d8+5 debris (DC 21 Reflex) then DC 20 swim."   themes: [hazard, terrain]   weight: 1

### cluster: gb14-old-sycamore — "Old Sycamore"   (source: p.66 / L3136)   mode: sandbox
scene: LANDMARK. Stub only — a mitflit-gremlin den detailed as a keyed dungeon in Ch2 Part 3 (p.120). PCs should be 2nd level before exploring it.
threads: [Stop the Greenbelt banditry]   characters: []   elements: [gremlin den, keyed dungeon]   themes: [dungeon-entrance]   location: GB14
gate: none
fragments:
  - plot_point: "Old Sycamore = mitflit-gremlin den; interior is a keyed dungeon (Ch2 Part 3 / dungeons file). Suggested 2nd level."   themes: [dungeon-stub]   weight: 1

### cluster: gb15-nettles-crossing — "Nettles' Crossing"   (source: p.67-69 / L3142)   mode: sandbox
scene: LANDMARK, Moderate 2. A ruined toll bridge where Brevic engineer Davik Nettles refused the Stag Lord's extortion and was burned out, drowned when the bandits cut his bridge — and rose as **Davik Nettles** (Creature 4, unique undead; +1 ranseur, Fearsome Gaze aura, Rotting Stench, nightmare, water walk, Rejuvenation, Sure Possession). Ringing a bell or crossing summons him over the water; he calls out, "You are not my tormentors. Bring me the Stag Lord's body... Or join me instead." If attacked he rages and rejuvenates nightly, plaguing a PC with nightmare unless they keep hunting the Stag Lord. Quest DAVIK'S REVENGE (30 XP): throw the Stag Lord's remains into the Shrike → Davik finds peace, his +1 ranseur washes ashore as a gift.
threads: [Defeat the Stag Lord]   characters: [Davik Nettles, the Stag Lord]   elements: [undead ghost-bridge, ranseur, vengeance quest]   themes: [haunting, vengeance, the-stag-lord]   location: GB15
gate: none
fragments:
  - plot_point: "Davik Nettles (Creature 4 unique undead) rises from the river when a bell rings; he wants the Stag Lord's body thrown in the Shrike — 'Bring me the Stag Lord's body... or join me instead.'"   themes: [haunting, the-stag-lord]   weight: 1
  - plot_point: "Attacking him: rage + nightly Rejuvenation + nightmare on the destroyer (dispel magic breaks the link). DAVIK'S REVENGE (30 XP): give the Stag Lord's remains to the Shrike → peace + his +1 ranseur as a parting gift."   themes: [vengeance, quest, reward]   weight: 1

### cluster: gb16-tatzlwyrm-den — "Tatzlwyrm Den"   (source: p.69 / L3230)   mode: sandbox
scene: STANDARD, Moderate 2. A Skunk River ford-island nest of a mated pair of **tatzlwyrms** (Creature 2; DC 11 flat check whether one is out hunting). Treasure: a long-dead explorer's skeleton with ruined scale mail and a +1 cold iron longsword; digging reveals 12 gp, 62 sp, valuables, and a map of the NW Greenbelt granting +2 item bonus to Map the Area in Rostland/Greenbelt hexes. (Source of tatzlwyrm head for Oleg's Trophy.)
threads: [Stop the Greenbelt banditry]   characters: []   elements: [tatzlwyrm nest, explorer's map, treasure]   themes: [hunt, treasure, exploration-aid]   location: GB16
gate: none
fragments:
  - plot_point: "Mated tatzlwyrms (Creature 2; DC 11 flat check if one is out). Source for Oleg's Trophy. Loot includes a +1 cold iron longsword and a Greenbelt map (+2 item to Map the Area)."   themes: [hunt, treasure]   weight: 1

### cluster: gb17-trapped-thylacine — "Trapped Thylacine"   (source: p.69-70 / L3250)   mode: sandbox
scene: STANDARD, Trivial 2. A frenzied **brush thylacine** (Creature 2) is trapped in a 20-ft pit. Unstable Pit (Hazard 0): coming within 5 ft crumbles the edge (DC 19 Reflex — fall prone / slide in for 1d6 / 2d6).
threads: []   characters: []   elements: [trapped beast, unstable pit]   themes: [wilderness-danger, hazard]   location: GB17
gate: none
fragments:
  - plot_point: "A brush thylacine (Creature 2) is stuck in a 20-ft pit; Unstable Pit (Hazard 0) crumbles its edge (DC 19 Reflex)."   themes: [hazard, combat]   weight: 1

### cluster: gb18-fangberry-thicket — "Fangberry Thicket"   (source: p.69-70 / L3280)   mode: sandbox
scene: STANDARD, Moderate 2. A thorny, web-draped fangberry thicket (difficult terrain; reckless movement = 1 piercing). Two **chew spiders** swarms (Creature 2, unique; web sense, chewing bites = bleed + venom) attack when harvesting starts. Gather Fangberries activity (10 min, DC 18 Survival; armor helps) completes Bokken's quest. The webs guard the berries Bokken needs (RL2).
threads: [Stop the Greenbelt banditry]   characters: [Bokken]   elements: [berry thicket, chew spider swarms, harvest activity]   themes: [errand, swarm-combat]   location: GB18
gate: none
fragments:
  - plot_point: "Fangberry thicket guarded by 2 chew-spider swarms (Creature 2, bleed + venom). Gather Fangberries (DC 18 Survival) completes Bokken's quest (RL2)."   themes: [errand, swarm-combat]   weight: 1

### cluster: gb19-river-crossing — "River Crossing"   (source: p.70 / L3318)   mode: sandbox
scene: STANDARD. A shallow Thorn River ford, never deeper than 3 ft.
threads: []   characters: []   elements: [river ford]   themes: [terrain]   location: GB19
gate: none
fragments:
  - plot_point: "Shallow Thorn River ford (max 3 ft deep)."   themes: [terrain]   weight: 1

### cluster: gb20-sootscale — "Sootscale Caverns"   (source: p.70 / L3322)   mode: sandbox
scene: HIDDEN. Stub only — well-hidden entrance to the Sootscale kobold caverns, a keyed dungeon detailed in Ch2 Part 4 (p.126). PCs should be 2nd level. Target of WANTED: Kobolds.
threads: [Stop the Greenbelt banditry]   characters: [the Sootscale kobolds]   elements: [hidden entrance, kobold faction, keyed dungeon]   themes: [dungeon-entrance, faction]   location: GB20
gate: none
fragments:
  - plot_point: "Sootscale Caverns — hidden kobold-lair entrance; interior is a keyed dungeon (Ch2 Part 4 / dungeons file). Completes WANTED: Kobolds. Suggested 2nd level."   themes: [dungeon-stub, faction]   weight: 1

---

### cluster: tw1-delicate-situation — "A Delicate Situation"   (source: p.70-73 / L3356)   mode: sandbox
scene: STANDARD, Severe 3. (Triggers only after the Stag Lord is driven off.) A logger crew under foreman **Corax** (Creature 3, unique) clashes with the nixie sorcerer **Melianse** (Creature 5, unique) over a felled 200-year-old grove; she has inveigled two loggers to guard her pool, creating a standoff. Both sides beg the PCs to take their side. Resolve by combat (Corax surrenders at ≤10 HP; Melianse fights to the death) or by negotiating an accord (calm both, satisfy Corax's lumber + Melianse's release + reparation — e.g., point loggers to an untouched coachwood grove 10 mi north near the old tatzlwyrm den, and replant). Quest MELIANSE'S TREES (30 XP): replace 3 trees (easiest via tree feather tokens, e.g. from Tiressia KL1) → she teaches the inveigle ritual, watches the rivers, and grants +2 to resolve this zone's events if the hex stays undeveloped.
threads: [Settle & claim the Stolen Lands]   characters: [Corax, Melianse]   elements: [logger-vs-fey standoff, nixie, negotiation, inveigle ritual]   themes: [fey, conflict-resolution, ecology]   location: TW1
gate: Stag Lord defeated
fragments:
  - plot_point: "Loggers (Corax, Creature 3) vs. nixie Melianse (Creature 5, 2 inveigled loggers) standoff; both appeal to the PCs. Combat or negotiated accord (lumber + freedom + reparation)."   themes: [fey, conflict-resolution]   weight: 1
  - plot_point: "MELIANSE'S TREES (30 XP): replant 3 trees (tree feather tokens, e.g. from Tiressia KL1) → she teaches the inveigle ritual and gives +2 to this zone's events if the hex stays undeveloped."   themes: [quest, fey-ally]   weight: 1

### cluster: tw2-endangered-expedition — "Endangered Expedition"   (source: p.73-74 / L3440)   mode: sandbox
scene: STANDARD, Moderate 5. (Only after the Stag Lord is defeated.) A gnome surveying expedition led by the flamboyant **Jubilost Narthropple** (Creature 1, Companion Guide) plus 9 **gnome explorers** (Creature 0) has a supply wagon and two ponies stuck mid-river after a kobold attack. PCs have 6 rounds to rescue (Swim DC 15, unhitch ponies, Command Animal DC 18, Shove the wagon DC 20). Jubilost's maps mark every Landmark in zones 1–5 plus up to 5 more sites (not the Beast SP4 or troll NM7); made helpful (DC 20 Make an Impression + DC 24 Request), he sells them at 10 gp/site (half-price if rescued) or trades for Hidden sites. May become a loyal companion (Companion Guide). Reward 30 XP + 200 gp supplies in the wagons.
threads: [Settle & claim the Stolen Lands, The fey wrongness & vanishings]   characters: [Jubilost Narthropple]   elements: [gnome cartographers, river rescue, map trade, companion]   themes: [allies, exploration-aid, first-world-foreshadow]   location: TW2
gate: Stag Lord defeated
fragments:
  - plot_point: "Rescue Jubilost Narthropple's mired wagon (6 rounds: Swim/unhitch/Command/Shove) → friendship + half-price maps marking every Landmark in zones 1-5 (plus up to 5 sites); possible loyal companion."   themes: [allies, exploration-aid]   weight: 1

### cluster: tw3-stag-lords-fort — "Stag Lord's Fort"   (source: p.74 / L3516)   mode: sandbox
scene: LANDMARK RESOURCE. Stub only — the Stag Lord's hilltop fort on the NE Tuskwater (a repurposed ruined Gyronna monastery) is the climactic set-piece of Ch3 Part 3 (p.172). Resource: a free Town Hall if a settlement is built here.
threads: [Defeat the Stag Lord]   characters: [the Stag Lord]   elements: [bandit fortress, set-piece, Town Hall]   themes: [the-stag-lord, climax]   location: TW3
gate: none
fragments:
  - plot_point: "Stag Lord's Fort — climactic keyed set-piece (Ch3 p.172); a free Town Hall if settled here. Throwing his remains in the Shrike afterward resolves Davik (GB15)."   themes: [the-stag-lord, set-piece]   weight: 1

### cluster: tw4-on-the-prowl — "On the Prowl"   (source: p.74-75 / L3522)   mode: sandbox
scene: STANDARD, Moderate 3. The cruel, talking warg **Howl-of-the-North-Wind** (Creature 2) and his pack of 3 **wolves** (Creature 1) claim this Tuskwater stretch; he's negotiating alliance with the troll Hargulka (Ch4) and pursues intruders for miles. WANTED: Howl-of-the-North-Wind (30 XP, level 5+): slay him → 140 gp bounty.
threads: [Defeat the Stag Lord]   characters: [Howl-of-the-North-Wind, Hargulka]   elements: [intelligent warg, wolf pack, bounty]   themes: [predator, foreshadow-trolls]   location: TW4
gate: none
fragments:
  - plot_point: "Talking warg Howl-of-the-North-Wind (Creature 2) + 3 wolves; allied-to-be with the troll Hargulka. WANTED bounty (level 5+) → 140 gp."   themes: [predator, bounty, foreshadow]   weight: 1

### cluster: tw5-lonely-barrow — "Lonely Barrow"   (source: p.75 / L3554)   mode: sandbox
scene: HIDDEN RESOURCE. Stub only — keyed dungeon in Ch2 Part 5 (p.132); PCs should be 3rd level. Pointed to by the Tomb Treasure map (from TW6). Resource: a Refuge once cleared.
threads: [Defeat the Stag Lord]   characters: []   elements: [burial cairn, undead guardian, flaming weapon, keyed dungeon]   themes: [dungeon-entrance, treasure]   location: TW5
gate: none
fragments:
  - plot_point: "Lonely Barrow — keyed dungeon (Ch2 Part 5); holds a magic flaming weapon and an undead guardian; reached via the Tomb Treasure map from TW6. Refuge once cleared. Suggested 3rd level."   themes: [dungeon-stub, treasure]   weight: 1

### cluster: tw6-hateful-hermit — "The Hateful Hermit"   (source: p.75-76 / L3560)   mode: sandbox
scene: STANDARD, Severe 3. Bokken's estranged murderous younger brother — the **Hateful Hermit** (Creature 5, unique; sneak attack, Focus Hatred, trackless step, +1 whip, blowgun w/ graveroot) lives in a hollow oak with his trained puma **Cat** (Creature 3). Craving a fresh kill, he ambushes the PCs, or poses as a peaceful druid to backstab them; flees at ≤10 HP to plot revenge (even infiltrating the PCs' city). Treasure: a lesser healing potion, invisibility potion, 64 cp, a silver locket of his and Bokken's mother (Bokken pays 10 gp / 100 gp in potions), wrapped in a faded map → the TOMB TREASURE quest. Quest TOMB TREASURE (30 XP): the map leads to the Lonely Barrow (TW5); reward is a magic flaming weapon tuned to a PC's favored weapon.
threads: [Stop the Greenbelt banditry]   characters: [the hateful hermit, Bokken]   elements: [serial-killer hermit, puma, treasure map, revenge]   themes: [murder, family-grudge, treasure]   location: TW6
gate: none
fragments:
  - plot_point: "The Hateful Hermit (Creature 5, Bokken's brother) + puma Cat (Creature 3) ambush from a hollow oak (or poses as a peaceful druid); flees at ≤10 HP to plot revenge."   themes: [murder, combat]   weight: 1
  - plot_point: "Treasure: a mother's locket (Bokken pays 10 gp / 100 gp potions) wrapped in a faded map → TOMB TREASURE (30 XP): leads to Lonely Barrow TW5 for a magic flaming weapon."   themes: [treasure, quest, family]   weight: 1

### cluster: tw7-old-beldame — "The Old Beldame"   (source: p.76-78 / L3626)   mode: sandbox
scene: RESOURCE STANDARD, Severe 3. A mud hut in a fetid marsh, home of **Elga Verniex** (Creature 6, unique; fey-touched human sorcerer) — the "Swamp Witch" of rumor, actually a crotchety but not-evil recluse with a guard **Scarecrow** (Creature 4). Crossing her fence triggers the scarecrow; ringing the gate bell lets PCs parley (she's hard of hearing, initially unfriendly; Diplomacy can defuse). Befriended, she warns of TW6 hermit, KL4 Candlemere, KL3 lizardfolk, TW5 barrow, and offers crafting/spellcasting at standard prices. Treasure: coins + a scroll of scrying + legend lore ritual instructions. Resource: a free herbalist structure if allied & settled. Quest BLACK RATTLECAPS (30 XP): gather rattlecap mushrooms from the Mud Bowl (KL5) → 5 gp each.
threads: [Settle & claim the Stolen Lands]   characters: [Elga Verniex (the Old Beldame)]   elements: [swamp witch, scarecrow guardian, crafting/spellcasting ally, herbalist]   themes: [unlikely-ally, false-rumor, fey-blood]   location: TW7
gate: none
fragments:
  - plot_point: "Elga Verniex the 'Old Beldame' (Creature 6) — not a child-boiling hag but a recluse; ring the gate bell to parley past her Scarecrow (Creature 4). Befriended: warnings, crafting & spellcasting, free herbalist if settled."   themes: [unlikely-ally, false-rumor]   weight: 1
  - plot_point: "BLACK RATTLECAPS (30 XP): harvest rattlecap mushrooms from the Mud Bowl (KL5) → 5 gp each."   themes: [quest, errand]   weight: 1

### cluster: tw8-old-crackjaw — "Old Crackjaw's Den"   (source: p.78-79 / L3696)   mode: sandbox
scene: HIDDEN, Moderate 3. Cliffs over the Tuskwater hide a trail (DC 20 Survival, or auto if learned from Arven the fisherman) to a pool den of **Old Crackjaw** (Creature 5, unique giant hookjaw turtle; Clench Jaws, Shell Defense), a legendary man-killer that attacks anyone in the water. Hazard: Stinging Nettles (Hazard 1) on the cliff tops (DC 17/20 Fort, sickened/clumsy). Treasure: a +1 striking sickle in the mud (DC 20 Perception).
threads: [Settle & claim the Stolen Lands]   characters: [Old Crackjaw, Arven]   elements: [monster turtle, hidden trail, nettle hazard]   themes: [wilderness-danger, local-legend]   location: TW8
gate: none
fragments:
  - plot_point: "Old Crackjaw (Creature 5 giant turtle) guards a hidden Tuskwater pool (trail DC 20 Survival, or from Arven); cliff-top Stinging Nettles (Hazard 1). Loot: +1 striking sickle."   themes: [combat, hazard, legend]   weight: 1

### cluster: tw9-gudrin-ford — "Gudrin River Ford"   (source: p.79 / L3748)   mode: sandbox
scene: LANDMARK. A shallow, navigable ford across the normally deep Gudrin River.
threads: []   characters: []   elements: [river ford]   themes: [terrain]   location: TW9
gate: none
fragments:
  - plot_point: "Navigable shallow ford across the deep Gudrin River."   themes: [terrain]   weight: 1

---

### cluster: kl1-tiressia-grove — "Tiressia's Grove"   (source: p.79-80 / L3768)   mode: sandbox
scene: RESOURCE STANDARD, Moderate 4. A sunlit glade home to the dryad **Tiressia** (Creature 4 elite) and her satyr consort **Falchos** (Creature 4), menaced by a scythe tree (KL2) that craves dryad flesh and already wounded Falchos. Tiressia plays the damsel; if PCs won't help, the pair fall back on suggestion/charm (they don't otherwise attack). Quest WRATH OF THE SCYTHE TREE (30 XP + 30 Kingdom XP): slay the scythe tree at KL2 → Tiressia gives a primeval mistletoe + 5 tree feather tokens (these solve Melianse's Trees, TW1); if helped without compulsion, she guards the Narlmarches and grants Refuge + +2 to this zone's dangerous events if the hex stays unsettled.
threads: [Settle & claim the Stolen Lands]   characters: [Tiressia, Falchos]   elements: [dryad & satyr, scythe-tree threat, fey-ally, tree feather tokens]   themes: [fey, ecology, alliance]   location: KL1
gate: none
fragments:
  - plot_point: "Dryad Tiressia (Creature 4 elite) + satyr Falchos (Creature 4) beg help vs. the scythe tree (KL2); if refused, they use suggestion/charm. WRATH OF THE SCYTHE TREE (30 XP + 30 Kingdom XP)."   themes: [fey, quest]   weight: 1
  - plot_point: "Reward: primeval mistletoe + 5 tree feather tokens (solve Melianse's Trees TW1); uncompelled help grants Narlmarches Refuge + +2 to this zone's events while undeveloped."   themes: [fey-ally, reward, kingdom]   weight: 1

### cluster: kl2-blighted-hollow — "The Blighted Hollow"   (source: p.80-81 / L3812)   mode: sandbox
scene: STANDARD, Moderate 4. A bone-strewn, decaying clearing where a hidden **scythe tree** (Creature 6) ambushes prey from the north side (intelligent, cruel; the WRATH OF THE SCYTHE TREE target). Treasure: 42 cp/55 sp/26 gp, a silver ring, and (DC 20 Perception) a dancing scarf wrapped around 3 amber (10 gp ea).
threads: [Settle & claim the Stolen Lands]   characters: []   elements: [scythe tree, ambush, blight]   themes: [fey-corruption, combat]   location: KL2
gate: none
fragments:
  - plot_point: "Scythe tree (Creature 6) ambushes from a blighted, bone-littered hollow — the target of Tiressia's quest. Loot: a dancing scarf + amber."   themes: [combat, quest-target, treasure]   weight: 1

### cluster: kl3-lizard-king — "Lair of the Lizard King"   (source: p.81 / L3834)   mode: sandbox
scene: LANDMARK RESOURCE. Stub only — Isle of the Lizard King, keyed dungeon in Ch2 Part 6 (p.136); PCs should be 4th level. Resource: the lizardfolk function as a Freehold → a free village (Barracks, Houses, Shrine, Wooden Walls, all-Water borders) if integrated.
threads: [Settle & claim the Stolen Lands]   characters: [the Lizard King]   elements: [lizardfolk village, keyed dungeon, Freehold]   themes: [dungeon-entrance, faction]   location: KL3
gate: none
fragments:
  - plot_point: "Lair of the Lizard King — keyed island dungeon (Ch2 Part 6); a Freehold → free lizardfolk village if brought into the kingdom. Suggested 4th level."   themes: [dungeon-stub, faction]   weight: 1

### cluster: kl4-candlemere — "Candlemere Island"   (source: p.81 / L3840)   mode: sandbox
scene: LANDMARK RESOURCE. Stub only — Candlemere Island, keyed dungeon in Ch2 Part 7 (p.142, severe; deeper levels in Ch9); PCs should be 4th level. The rumored "thin boundary" tower guarded by a deadly monster. Resource: a Refuge if claimed & cleared (above-ground + basement); a settlement here gets a free Watchtower (all-Water borders).
threads: [Settle & claim the Stolen Lands, The fey wrongness & vanishings]   characters: []   elements: [haunted tower island, planar thin spot, keyed dungeon]   themes: [dungeon-entrance, first-world, danger]   location: KL4
gate: none
fragments:
  - plot_point: "Candlemere Island — keyed tower dungeon (Ch2 Part 7; deeper in Ch9), a planar thin spot. Refuge if cleared / free Watchtower if settled. Suggested 4th level (basement skews severe)."   themes: [dungeon-stub, first-world]   weight: 1

### cluster: kl5-mud-bowl — "The Mud Bowl"   (source: p.81 / L3848)   mode: sandbox
scene: STANDARD, Severe 6. A bubbling geothermal mud pool (difficult terrain; inhaled poison, DC 17 Fort or sickened 1) ringed by giant fungi. A disguised **tendriculos** (Creature 7) lurches up to swallow prey. Treasure: 18 black rattlecap mushrooms (1d4-1 crushed per round of nearby combat) — harvest for the Old Beldame's BLACK RATTLECAPS quest (TW7).
threads: [Settle & claim the Stolen Lands]   characters: []   elements: [mud pit, tendriculos, rattlecap mushrooms]   themes: [wilderness-danger, errand-payoff]   location: KL5
gate: none
fragments:
  - plot_point: "Mud Bowl: noxious geothermal mud + a disguised tendriculos (Creature 7). Harvest black rattlecaps here for the Old Beldame (TW7)."   themes: [combat, errand-payoff]   weight: 1

### cluster: kl6-cry-for-help — "A Cry for Help"   (source: p.81-82 / L3866)   mode: sandbox
scene: STANDARD, Severe 4. Two **leucrottas** (Creature 5) allied with the troll Hargulka use voice mimicry to lure PCs with fake cries for help. A spared survivor (reduce one to ≤20 HP) warns that "King Hargulka" will soon rule and that his lair is in the southern Narlmarches (location unknown).
threads: [Defeat the Stag Lord]   characters: [Hargulka]   elements: [leucrotta ambush, voice mimicry, troll intel]   themes: [predator, foreshadow-trolls]   location: KL6
gate: none
fragments:
  - plot_point: "2 leucrottas (Creature 5, Hargulka's scouts) mimic cries for help; a spared one warns of 'King Hargulka' rising in the southern Narlmarches (foreshadows Ch4)."   themes: [ambush, foreshadow]   weight: 1

### cluster: kl7-hunters-lodge — "Hunter's Lodge"   (source: p.82 / L3884)   mode: sandbox
scene: RESOURCE STANDARD. An abandoned lodge; after the kingdom is founded, a group rebuilds it and invites the PCs on a dangerous hunt (Ch5). Resource: a Refuge if Claimed / free Popular Tavern if settled.
threads: [Settle & claim the Stolen Lands]   characters: []   elements: [abandoned lodge, future hunt, Popular Tavern]   themes: [kingdom-building, foreshadow]   location: KL7
gate: none
fragments:
  - plot_point: "Abandoned hunter's lodge → Refuge / free Popular Tavern; later hosts a dangerous hunt (Ch5)."   themes: [kingdom-resource, foreshadow]   weight: 1

### cluster: kl8-hunting-grounds — "Hunting Grounds"   (source: p.82 / L3890)   mode: sandbox
scene: STANDARD. A monster-infested hex — auto wandering-monster encounter if explored before Ch5; later a hunting venue (Ch5 Part 2).
threads: []   characters: []   elements: [monster-rich hex, wandering encounter]   themes: [wilderness-danger]   location: KL8
gate: none
fragments:
  - plot_point: "Monster-infested hex; explore before Ch5 = an automatic wandering-monster encounter; later a hunting venue."   themes: [wandering-encounter]   weight: 1

### cluster: kl9-lake-silverstep — "Lake Silverstep"   (source: p.82-83 / L3894)   mode: sandbox
scene: LANDMARK RESOURCE, Severe 4. The clearest lake in the Stolen Lands (named for a silver dragon's legendary footprint), rich in prized silver eels; shy nixies/grigs/faerie dragons haunt the western banks. A **freshwater elasmosaurus** (Creature 7) may surface to threaten lingerers. Resource: +1 (or +2 if settled) to Fishing kingdom checks if Claimed. Quest MMMMMMM... EELS! (30 XP + 30 Kingdom XP, level 6): catch 12 eels for chef Beven Armaki → a +1 buckler + an optional free Popular Tavern.
threads: [Settle & claim the Stolen Lands]   characters: [Beven Armaki]   elements: [pristine lake, silver eels, lake monster, fishing resource]   themes: [resource, beauty, hidden-danger]   location: KL9
gate: none
fragments:
  - plot_point: "Lake Silverstep: pristine eel-rich lake; a freshwater elasmosaurus (Creature 7) lurks. Claim → Fishing bonus. MMMMMMM... EELS! (level 6): 12 eels for Beven Armaki → +1 buckler + free tavern."   themes: [resource, quest]   weight: 1

### cluster: kl10-mudflats — "Mudflats"   (source: p.83 / L3928)   mode: sandbox
scene: STANDARD, Moderate 6. A geothermal lakeshore mud expanse (difficult terrain) home to a pack of 8 **mudwretches** (Creature 2), leftover elementals from an ancient elven Plane-of-Earth/Water experiment; they fight to the death to be left alone. Treasure: a mud-mummified Taldan captain-general with a platinum skull idol (100 gp).
threads: []   characters: []   elements: [mud elementals, ancient elven experiment, treasure]   themes: [wilderness-danger, ancient-mystery]   location: KL10
gate: none
fragments:
  - plot_point: "8 mudwretches (Creature 2, ancient elven experiment leftovers) defend the mudflats to the death; a mummified Taldan captain holds a 100 gp platinum skull idol."   themes: [combat, ancient-mystery, treasure]   weight: 1

---

### cluster: nm1-warrior-cairn — "Warrior Cairn"   (source: p.83 / L3956)   mode: sandbox
scene: SECRET. An overgrown cairn (DC 15 Perception) of a forgotten Tiger Lord chieftain's son. Treasure: a ring of the tiger (green wood, tigers chasing) — recognizable (DC 20 Society / DC 15 Heraldry Lore) and politically charged: openly wearing it can help or hurt with the Tiger Lords (Ch7).
threads: []   characters: []   elements: [hidden grave, ring of the tiger, Tiger Lord token]   themes: [treasure, foreshadow-rivals]   location: NM1
gate: none
fragments:
  - plot_point: "Hidden Tiger Lord cairn (DC 15 Perception) holds a ring of the tiger — politically charged with the Tiger Lords (Ch7)."   themes: [treasure, foreshadow]   weight: 1

### cluster: nm2-statue-erastil — "Statue of Erastil"   (source: p.83-84 / L3962)   mode: sandbox
scene: RESOURCE STANDARD. A 15-ft Erastil statue, all that survives of a burned hunter's lodge, still sacred. Erastil worshippers feel safe within 60 ft and no wild animals approach (negate wild-animal wandering rolls here — an excellent campsite). Cleaning it + prayer by an Erastil worshipper grants a one-time minor boon (no crit-fail on Subsist). Resource: a free Monument if settled.
threads: [Settle & claim the Stolen Lands]   characters: []   elements: [sacred statue, safe campsite, Erastil boon, Monument]   themes: [erastil, sanctuary, kingdom-building]   location: NM2
gate: none
fragments:
  - plot_point: "Erastil statue: a safe camp (no wild-animal encounters within 60 ft); clean + pray for a one-time Subsist boon; free Monument if settled."   themes: [erastil, sanctuary]   weight: 1

### cluster: nm3-dead-unicorn — "Dead Unicorn"   (source: p.84 / L3976)   mode: sandbox
scene: STANDARD. A blind, oddly-odorless dead unicorn by a fouled pond, horn removed post-mortem; killed by a primal finger of death and "marked" by First-World fey so scavengers shun it (DC 33 Arcana/DC 31 Nature to confirm the spell; DC 18/15 First World Lore for the marking). The nymph **Nyrissa** killed it for a trophy as she prepares to claim the Stolen Lands — the horn appears in her lair late in the AP. Restored or via talking corpse, it names its killer only as "purest, corrupted beauty."
threads: [The fey wrongness & vanishings]   characters: [Nyrissa]   elements: [murdered unicorn, First-World trophy, central mystery clue]   themes: [first-world, mystery, foreshadow-nyrissa]   location: NM3
gate: none
fragments:
  - plot_point: "Dead unicorn slain by primal finger of death and First-World 'marked' — Nyrissa took its horn as a trophy (foreshadows the AP's true villain). Talking corpse: 'purest, corrupted beauty.'"   themes: [first-world, foreshadow-nyrissa, mystery]   weight: 1

### cluster: nm4-fey-pranksters — "Fey Pranksters"   (source: p.84-85 / L3990)   mode: sandbox
scene: STANDARD, Moderate 5. Two sadistic **pixies** (Creature 4) mounted on 2 befriended **wargs** (Creature 2) wage a cruel-pranks contest (poisoned milk, kidnapped babies, shaved bear cubs in cribs) hoping to attract Nyrissa's notice. They go invisible and order the wargs to attack while firing arrows/spells from warg-back.
threads: [The fey wrongness & vanishings]   characters: []   elements: [malevolent pixies, warg mounts, Nyrissa-seekers]   themes: [fey-corruption, foreshadow-nyrissa]   location: NM4
gate: none
fragments:
  - plot_point: "2 cruel pixies (Creature 4) on warg mounts (Creature 2) run a vicious-prank contest hoping to attract Nyrissa; go invisible and attack from warg-back."   themes: [fey-corruption, combat]   weight: 1

### cluster: nm5-forgotten-keep — "The Forgotten Keep"   (source: p.85 / L4050)   mode: sandbox
scene: RESOURCE STANDARD. Stub only — keyed dungeon in Ch2 Part 8 (p.148); PCs should be 5th level. Resource: a ruined Castle; settling here halves the cost of building a Castle.
threads: [Settle & claim the Stolen Lands]   characters: []   elements: [ruined keep, keyed dungeon, Castle discount]   themes: [dungeon-entrance, kingdom-building]   location: NM5
gate: none
fragments:
  - plot_point: "The Forgotten Keep — keyed dungeon (Ch2 Part 8); a ruined Castle (halves Castle build cost if settled). Suggested 5th level."   themes: [dungeon-stub, kingdom]   weight: 1

### cluster: nm6-hodag-den — "Hodag Den"   (source: p.85 / L4056)   mode: sandbox
scene: HIDDEN, Moderate 5. A windstorm deadfall riddled with hollows; one deep cavern (DC 20 Perception) is the den of a cantankerous **elite hodag** (Creature 7) that immediately attacks amid bones of loggers and bandits. Treasure: 3 battleaxes, a greataxe, +1 studded leather, and a +1 striking spear.
threads: []   characters: []   elements: [hodag lair, deadfall]   themes: [wilderness-danger, treasure]   location: NM6
gate: none
fragments:
  - plot_point: "Elite hodag (Creature 7) in a hidden deadfall cavern (DC 20 Perception); loot includes +1 striking spear and +1 studded leather."   themes: [combat, treasure]   weight: 1

### cluster: nm7-hargulka-stronghold — "Hargulka's Stronghold"   (source: p.85 / L4070)   mode: sandbox
scene: HIDDEN RESOURCE. Stub only — an ancient dwarven ruin now home to a troll clan (Hargulka); detailed in Ch4. Pointed to by Munguk's map (SH2) and leucrotta intel (KL6). Resource: a Refuge once cleared & Claimed.
threads: [Defeat the Stag Lord, Settle & claim the Stolen Lands]   characters: [Hargulka]   elements: [troll lair, dwarven ruin, keyed set-piece]   themes: [foreshadow-trolls, dungeon-entrance]   location: NM7
gate: none
fragments:
  - plot_point: "Hargulka's Stronghold — troll-clan dwarven ruin (Ch4 set-piece); reached via Munguk's map (SH2) / leucrotta intel (KL6). Refuge once cleared."   themes: [foreshadow-trolls, dungeon-stub]   weight: 1

---

### cluster: sh1-drake-nest — "Drake Nest"   (source: p.86 / L4100)   mode: sandbox
scene: STANDARD, Moderate 6. A lone, oversized **enormous flame drake** (Creature 8, unique; Fireball Breath 9d6, Draconic Frenzy, smoke vision) — the source of the false "red dragon in the Narlmarches" rumor — lairs by a pool littered with charred remains. Treasure: +1 chain shirt, +1 composite longbow, cloak of elvenkind. WANTED: Flame Drake (30 XP, level 6) → 400 gp bounty.
threads: [Settle & claim the Stolen Lands]   characters: []   elements: [flame drake, false-dragon rumor, bounty]   themes: [wilderness-danger, bounty, rumor-payoff]   location: SH1
gate: none
fragments:
  - plot_point: "Enormous flame drake (Creature 8, Fireball Breath 9d6) — the 'red dragon' rumor's true source. Loot: cloak of elvenkind etc. WANTED bounty (level 6) → 400 gp."   themes: [combat, bounty, rumor-payoff]   weight: 1

### cluster: sh2-wandering-giant — "The Wandering Giant"   (source: p.86-87 / L4134)   mode: sandbox
scene: STANDARD, Low 6. **Munguk** (Creature 7, hill giant), rejected by Hargulka's trolls (NM7), wanders depressed and drunk (sickened 1, -2 Perception) seeking wolfberries, game, and a mate. Gifting 3+ gallons of alcohol gives +2 to Make an Impression (initially unfriendly); friendly → intel on NM5 keep, KL3 lizardfolk, NM7 troll lair; helpful → his map (DC 20 Society to decipher Jotun) marking Hargulka's lair as "mean ugly troll-bully." Fights until 30 HP then blubbers for mercy. Peaceful resolution = full XP.
threads: [Defeat the Stag Lord, Settle & claim the Stolen Lands]   characters: [Munguk, Hargulka]   elements: [lonely drunk giant, informant, troll-lair map]   themes: [unlikely-ally, comedy, foreshadow-trolls]   location: SH2
gate: none
fragments:
  - plot_point: "Munguk (Creature 7 hill giant), drunk & rejected by the trolls, can be befriended with booze for intel on NM5/KL3/NM7 and a map (DC 20 Society) marking Hargulka's lair."   themes: [unlikely-ally, intel, foreshadow]   weight: 1

### cluster: sh3-abandoned-ferry — "Abandoned Ferry Station"   (source: p.87 / L4160)   mode: sandbox
scene: LANDMARK RESOURCE. Half-collapsed ferry buildings where the Shrike branches off the Little Sellen, formerly used by kobolds/mites/bandits, now empty. Resource: functional docks → a free pier structure if settled.
threads: [Settle & claim the Stolen Lands]   characters: []   elements: [ruined ferry, docks, pier]   themes: [kingdom-building]   location: SH3
gate: none
fragments:
  - plot_point: "Abandoned ferry station; salvageable docks → a free pier if a settlement is built here."   themes: [kingdom-resource]   weight: 1

### cluster: sh4-beasts-lair — "Beast's Lair"   (source: p.87 / L4178)   mode: sandbox
scene: HIDDEN RESOURCE. Stub only — den of an enormous owlbear (the Beast); detailed in Ch4. Not on Jubilost's maps (TW2). Resource: a Refuge if Claimed & cleared.
threads: [Settle & claim the Stolen Lands]   characters: [the Beast]   elements: [owlbear lair, keyed set-piece]   themes: [dungeon-entrance, wilderness-danger]   location: SH4
gate: none
fragments:
  - plot_point: "Beast's Lair — enormous owlbear den (Ch4 set-piece), not on Jubilost's maps; Refuge once cleared."   themes: [dungeon-stub]   weight: 1

### cluster: sh5-greengripe — "Greengripe"   (source: p.87 / L4184)   mode: sandbox
scene: LANDMARK. Stub only — a hilltop goblin village; detailed in Ch5. Resource: a Freehold → a free goblin village (Alchemy Lab, Shrine, Stables, Tenements, Wooden Walls, all-Land borders) if integrated.
threads: [Settle & claim the Stolen Lands]   characters: []   elements: [goblin village, Freehold]   themes: [faction, kingdom-building]   location: SH5
gate: none
fragments:
  - plot_point: "Greengripe goblin village (Ch5); a Freehold → free goblin village if brought into the kingdom."   themes: [faction, kingdom]   weight: 1

### cluster: sh6-whispering-grotto — "Whispering Grotto"   (source: p.87-88 / L4204)   mode: sandbox
scene: RESOURCE SECRET. A dale where wind over ground fissures makes an unsettling whispering (DC 12 Perception while Reconnoitering; crit spots the holes). Peering in reveals crystal-filled caverns. Resource: a specialized mine here generates 1 Luxury Commodity/turn instead of Ore.
threads: [Settle & claim the Stolen Lands]   characters: []   elements: [whispering fissures, gem deposit, luxury mine]   themes: [resource, eerie-atmosphere]   location: SH6
gate: none
fragments:
  - plot_point: "Whispering Grotto: wind-whistling fissures (DC 12 Perception) over a gem deposit → a specialized mine yields 1 Luxury Commodity/turn."   themes: [kingdom-resource, atmosphere]   weight: 1

### cluster: sh7-dragonleaf-gulch — "Dragonleaf Gulch"   (source: p.88 / L4212)   mode: sandbox
scene: STANDARD, Moderate 6. A river gully island choked with vegetation hides six **snapping flytraps** (Creature 3) that lunge at anyone Small+ near the banks or clinging to the cliffs. Treasure (DC 25 Perception): 320 cp/345 sp/13 gp, a darkwood-scabbarded bastard sword, a wand of continuation (2nd), and a salvageable heartbond ritual formula.
threads: []   characters: []   elements: [carnivorous plants, river gully]   themes: [wilderness-danger, treasure]   location: SH7
gate: none
fragments:
  - plot_point: "6 snapping flytraps (Creature 3) on a river-gully island snap at bank-walkers and cliff-climbers; loot includes a wand of continuation and a heartbond ritual formula."   themes: [combat, treasure]   weight: 1

### cluster: sh8-cradle-lamashtu — "Cradle of Lamashtu"   (source: p.88 / L4228)   mode: sandbox
scene: RESOURCE SECRET. A hidden cave (DC 30 Perception while Reconnoitering) in low tors; empty/GM-stocked before Ch5, then headquarters of the Cult of the Bloom once the Season of Bloom begins (Ch5). Resource: a Refuge once cleared & the cult defeated.
threads: [The fey wrongness & vanishings]   characters: []   elements: [hidden cult cave, Cult of the Bloom, keyed set-piece]   themes: [foreshadow-bloom, dungeon-entrance]   location: SH8
gate: none
fragments:
  - plot_point: "Cradle of Lamashtu — hidden cave (DC 30 Perception) that becomes the Cult of the Bloom's HQ in Ch5; Refuge once the cult is cleared."   themes: [foreshadow-bloom, dungeon-stub]   weight: 1

---

## Seed the Lists  (names only; [HIDDEN] for unearned spoilers)

**Threads:**
- Settle & claim the Stolen Lands (master charter goal) — *active from start*
- Stop the Greenbelt banditry / clear the bandits — *opening*
- Defeat the Stag Lord — *opening (rumored)*
- Recover Davik Nettles' peace / hunt the Stag Lord (GB15) — *on discovery*
- The fey wrongness & vanishings (NM3 unicorn, NM4 pixies, SH8 Cradle) [HIDDEN] — *as encountered*
- Found & grow your kingdom (resource sites: GB8 gold, KL9 eels, SH6 luxury, forts/lodges) — *opens Ch4*
- Foreshadowed rivals: the trolls under Hargulka (KL6/NM7/SH2), the Tiger Lords (NM1) [HIDDEN]

**Characters:**
- Oleg & Svetlana Leveton, Kesten Garess, Jhod Kavken (Oleg's allies) — *opening*
- Jamandi Aldori (patron) — *opening*
- Bokken (alchemist), the GB3 fey Perlivash & Tyg-Titter-Tut, Garuum (boggard), Melianse (nixie), Tiressia & Falchos (dryad/satyr), Jubilost Narthropple (gnome), the Old Beldame / Elga Verniex — *on discovery (potential allies)*
- The Stag Lord (antagonist), Davik Nettles, the hateful hermit, Howl-of-the-North-Wind — *on discovery (foes)*
- Hargulka, the Beast, the Lizard King [HIDDEN], Nyrissa [HIDDEN] — *foreshadowed; add on discovery*

**Adventure Features (locations/hazards):**
- Oleg's Trading Post (RL1), the Greenbelt zone, Temple of the Elk (GB6), Nettles' Crossing (GB15), Old Sycamore (GB14), Sootscale Caverns (GB20), the Stag Lord's Fort (TW3) — *opening / early*
- Resource sites: Gold Mine (GB8), Fort Serenko (RL5), Lake Silverstep (KL9), Whispering Grotto (SH6), Hunter's Lodge (KL7), Abandoned Ferry (SH3) — *as found*
- Hazards: Breeg's Traps (GB1), Rickety Bridge (GB13), Unstable Pit (GB17), Stinging Nettles (TW8), chew-spider thicket (GB18), the Mud Bowl/Mudflats geothermal mud (KL5/KL10) — *as encountered*
- Dungeon entrances (interiors elsewhere): Old Sycamore, Sootscale, Lonely Barrow, Lizard King's Isle, Candlemere, Forgotten Keep, Hargulka's Stronghold, the Beast's Lair, Cradle of Lamashtu

## Diminisher: ¼ for a solo PC — scale printed encounters down.
The AP assumes a 4-PC party; printed Trivial→Severe ratings here are for four. For a lone hero apply
the ¼ Diminisher (weak adjustments / fewer foes / down-tiered creatures). Severe-rated sites (TW1
Melianse, TW6 hermit, TW7 Old Beldame, KL5 Mud Bowl, KL6 leucrottas, KL9 elasmosaurus) are lethal
to a solo PC at the suggested level — flag for caution or scale hard. Many "encounters" here are
negotiable (GB3, GB11, KL1, SH2, TW1, TW7): reward parley over combat.
