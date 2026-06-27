# Ingested Adventure — Kingmaker Chapter 2: Into the Wild — Hexcrawl (late, Zones 7–19)   (hook: adventure-ingest)
fidelity: full   ·   source: Kingmaker AP 2e, Chapter 2, lines 4386–5836

> Scope note: covers Zones 7–19. Zone 7 (Dunsward, DS sites incl. the Varnhold hex) was added by a follow-up patch (source p.87–91 / L4238–4380); Zones 8–19 were atomized from the L4386–5836 range. Per-zone wandering-monster tables are captured as their own clusters flagged for list_d100 conversion.

---

### cluster: nh-zone-table — "Nomen Heights — Wandering Encounters (Zone 8)"   (source: p.91 / L4386)   mode: sandbox
scene: d20 random-encounter table for Zone 8 (Nomen Heights), creatures level ~8. Rolls 1–5 fall back to the Zone 7 (Dunsward) table; 6–8 = 6 centaurs (trivial), 9–11 = 4 cyclopes, 12–13 = 2 chimeras, 14–15 = 1 peluda, 16–17 = 4 zombie hulks, 18–19 = 4 wyverns, 20 = 2 mastodons (severe). Centaurs (Nomen clan, detailed Ch.6) observe rather than initiate, flee at half losses, can be parleyed. Zombie hulks are cyclopes raised by the reawakened lich Vordakai, increasingly common here. Convert to list_d100 generator.
threads: [The Nomen Problem]   characters: [Nomen centaur clan, Vordakai]   elements: [Nomen Heights, zombie hulks, mastodons]   themes: [wilderness, undead, centaurs]   location: NH
gate: none
fragments:
  - plot_point: "Nomen centaurs observe intruders, let PCs make first move; parleyable, flee at half losses"   themes: [diplomacy, centaurs]   weight: 1
  - plot_point: "Zombie hulks (undead cyclopes) signal Vordakai's renewed activity in the Heights"   themes: [undead, foreshadow]   weight: 1
  - plot_point: "Roll 20: 2 mastodons (Severe 8) — apex random encounter"   themes: [megafauna, danger]   weight: 1

### cluster: nh-quest-problem — "The Nomen Problem (quest)"   (source: p.91 / L4396)   mode: sandbox
scene: At PC level 8, a Restov envoy hands the PCs the "Nomen problem": the centaur clan has long vexed Restov's neighbors. Goal is to either drive off the Nomen centaur clan OR forge an alliance/diplomatic relations with them (war or peace both qualify). Reward: 500 gp from the swordlords of Restov. 30 XP.
threads: [The Nomen Problem]   characters: [Restov envoy, swordlords of Restov, Nomen centaur clan]   elements: [Nomen Heights]   themes: [diplomacy, faction, quest]   location: NH
gate: PC level 8 (envoy arrives)
fragments:
  - plot_point: "Restov asks PCs to either ally with or drive out the Nomen centaurs"   themes: [quest, faction]   weight: 1
  - plot_point: "Completion (diplomacy OR warfare) earns 500 gp from Restov"   themes: [reward]   weight: 1

### cluster: nh1 — "NH1. Nomen Campsite"   (source: p.91 / L4404)   mode: sandbox
scene: The home of the Nomen centaur clan; STANDARD site, fully detailed in Chapter 6. Placeholder here — the clan dwells at this hex.
threads: [The Nomen Problem]   characters: [Nomen centaur clan]   elements: [Nomen Campsite]   themes: [centaurs, settlement]   location: NH1
gate: none
fragments:
  - plot_point: "Nomen clan home camp (see Ch.6 for full detail)"   themes: [centaurs, location]   weight: 1

### cluster: nh2 — "NH2. The Linnorm's Grave"   (source: p.91 / L4408)   mode: sandbox
scene: LANDMARK. Bleached ribs and a moss-draped skull of a long-dead crag linnorm crown a hilltop; DC 36 Arcana / DC 31 Dragon Lore identifies it. Local centaurs revere the site, leaving meat-and-wine offerings to keep the linnorm's ghost from returning. A herd of 15 mastodons grazes the hex; each hexploration attempt needs a DC 26 Nature check to avoid angering them — failure sends 2 mastodons (Creature 9) charging while the rest stampede. Severe 8. First non-angering hexploration grants 80 XP.
threads: []   characters: [Nomen centaur clan]   elements: [Linnorm's Grave, mastodon herd]   themes: [megafauna, reverence, landmark]   location: NH2
gate: none
fragments:
  - plot_point: "Crag linnorm skeleton landmark revered by centaurs (DC 36 Arcana to ID)"   themes: [lore, landmark]   weight: 1
  - plot_point: "DC 26 Nature each hexploration or 2 mastodons (Creature 9) charge"   themes: [hazard, megafauna]   weight: 1
  - plot_point: "First clean hexploration here awards 80 XP"   themes: [reward]   weight: 1

### cluster: lv-zone-table — "Tors of Levenies — Wandering Encounters (Zone 9)"   (source: p.92 / L4436)   mode: sandbox
scene: d20 Zone 9 table, level ~9. 1–5 = Zone 8 table; 6–8 = 4 zombie hulks, 9–11 = 2 chimeras, 12–13 = 2 leukodaemons, 14–15 = 1 meladaemon, 16–17 = 1 thunderbird, 18–19 = 6 wyverns, 20 = one great cyclops (severe). Daemons here were drawn to this plane by Vordakai and set loose; a captured/forced daemon could lead PCs toward Vordakai's Tomb — or betray them. Convert to list_d100 generator.
threads: [Find Vordakai's Tomb]   characters: [Vordakai]   elements: [Tors of Levenies, daemons]   themes: [undead, daemons, mountains]   location: LV
gate: none
fragments:
  - plot_point: "Daemons in the Tors are Vordakai's summoned servants; a forced one may guide PCs to the tomb"   themes: [daemons, lead, foreshadow]   weight: 1
  - plot_point: "Roll 20: one great cyclops (Severe 9)"   themes: [danger]   weight: 1

### cluster: lv1 — "LV1. Varnhold Pass"   (source: p.92 / L4440)   mode: sandbox
scene: LANDMARK RESOURCE. A natural east–west pass where the Crooked River cascades out of the mountains under 150-ft cliffs; a single abandoned stone watchtower sits at the top, no signs of struggle. From the 30-ft tower on a clear day Varnhold is visible to the southeast (foreshadows the Varnhold disappearance, Ch.6). Resource: if Claimed, the building is a Refuge; a settlement here gains a free Watchtower.
threads: [Find Vordakai's Tomb, Varnhold mystery]   characters: []   elements: [Varnhold Pass, abandoned watchtower]   themes: [landmark, foreshadow, resource]   location: LV1
gate: none
fragments:
  - plot_point: "Abandoned watchtower with no signs of struggle overlooks Varnhold (foreshadows its fate)"   themes: [mystery, foreshadow]   weight: 1
  - plot_point: "Claimed: Refuge; settlement gains free Watchtower"   themes: [kingdom, resource]   weight: 1

### cluster: lv2 — "LV2. Talon Peak"   (source: p.92 / L4448)   mode: sandbox
scene: LANDMARK RESOURCE, Severe 9. A crumbling claw-like tower atop a steep mountain, longtime roc nesting ground. The hex is greater difficult terrain; the final 250 ft to the tower needs a DC 25 Athletics Climb (failure = 8d6 bludgeoning, DC 28 basic Reflex; crit fail aborts). Creature: the unique Talon Peak Roc (Creature 12, HP 220, AC 33), a black-plumed female who relocated after the black dragon Ilthuliak killed her mate. On arrival DC 11 flat check decides if she's present; if hunting she returns in 1d4 hrs. Treasure in nest: 30 gp, gold ring (50 gp), staff of evocation, +1 full plate, +1 scimitar, type I bag of holding (with valueless gremlin skulls). Three roc eggs satisfy the Omelet King quest (p.525); each egg is 22 Bulk and needs the Transport a Roc Egg group activity (DC 25/27 Athletics). Resource: settlement here gains a Ruined Watchtower.
threads: [Omelet King quest]   characters: [Talon Peak Roc, Ilthuliak]   elements: [Talon Peak, roc nest, roc eggs]   themes: [aerial predator, climbing hazard, treasure]   location: LV2
gate: none
fragments:
  - plot_point: "Talon Peak Roc (Creature 12, HP 220) defends nest; DC 11 flat check for presence"   themes: [boss, aerial]   weight: 1
  - plot_point: "Climb the final 250 ft (DC 25 Athletics) or take 8d6 falling damage"   themes: [hazard, climb]   weight: 1
  - plot_point: "Nest loot: staff of evocation, +1 full plate, +1 scimitar, type I bag of holding"   themes: [treasure]   weight: 1
  - plot_point: "Three 22-Bulk roc eggs satisfy the Omelet King quest via Transport a Roc Egg activity"   themes: [quest, logistics]   weight: 1

### cluster: lv3 — "LV3. Culchek Cave"   (source: p.93 / L4506)   mode: sandbox
scene: HIDDEN RESOURCE. Former lair of the Culchek spriggans (who invade Varnhold in Ch.6); by the time PCs arrive it's likely abandoned and stripped bare. Entrance hidden behind a rock spur and brush — DC 20 Perception during Reconnoiter to find. 15-room complex, empty. Resource: if Claimed after abandonment, serves as a Refuge.
threads: [Varnhold mystery]   characters: [Culchek spriggans]   elements: [Culchek Cave]   themes: [foreshadow, hidden, resource]   location: LV3
gate: none
fragments:
  - plot_point: "Hidden spriggan cave (DC 20 Perception to find), emptied — ties to Varnhold invasion in Ch.6"   themes: [foreshadow, hidden]   weight: 1
  - plot_point: "Claimed after abandonment: Refuge"   themes: [kingdom, resource]   weight: 1

### cluster: lv4 — "LV4. The Ghost Stone"   (source: p.93 / L4516)   mode: sandbox
scene: STANDARD, Moderate 9. A polished gray elven monolith (15 ft) at a valley's western end; at night a 120-ft radius glows and ghostly shapes writhe — a thinned boundary to the Ethereal Plane, an old portal foundation. Creature: Zzamas, a friendly ether spider (Creature 5) speaking broken Common, asks the PCs' help (an easier parley if a PC speaks Aklo) to kill six xills that took her home. The Drunken Xills (6, Creature 6) are sickened 1 from the Stone's intoxicating aura (can't reduce below 1 while present) and fight to the death; Zzamas aids if allied. Quest: The Ghost Stone War, 30 XP — reward is a drifting Ethereal chest (DC 25 Thievery), holding a wand of shrink item and a wizard's spellbook (six spells lvl 1–5 plus legend lore and unseen custodians rituals).
threads: [The Ghost Stone War]   characters: [Zzamas the ether spider, the xills]   elements: [Ghost Stone, Ethereal portal]   themes: [otherplanar, alliance, quest]   location: LV4
gate: none
fragments:
  - plot_point: "Zzamas the ether spider seeks help (Aklo eases parley) against six Drunken Xills"   themes: [alliance, otherplanar]   weight: 1
  - plot_point: "Six Drunken Xills (Creature 6) are sickened 1 by the Stone's aura, fight to the death"   themes: [combat]   weight: 1
  - plot_point: "Reward chest: wand of shrink item + spellbook with legend lore & unseen custodians rituals"   themes: [reward, treasure]   weight: 1

### cluster: lv5 — "LV5. Ironstone Gully"   (source: p.93 / L4550)   mode: sandbox
scene: RESOURCE site. A shallow bat-colony cave whose far wall hides a rich iron-ore vein — DC 25 Nature or Perception to discover the truth. Resource: if Claimed and a mine Work Site is established, it provides double the normal Ore Commodities.
threads: []   characters: []   elements: [Ironstone Gully, iron vein]   themes: [resource, mining]   location: LV5
gate: none
fragments:
  - plot_point: "Hidden rich iron vein (DC 25 Nature/Perception); mine here yields double Ore Commodities"   themes: [resource, kingdom]   weight: 1

### cluster: lv6 — "LV6. Vordakai's Tomb"   (source: p.94 / L4556)   mode: sandbox
scene: RESOURCE STANDARD. The lair of the lich Vordakai, presented in full in Chapter 6 — the climactic dungeon of the Varnhold arc. Approached via the stairway from LV7 (Valley of the Dead). Resource: if Claimed after all the tomb's dangers are defeated, the hex provides a Refuge.
threads: [Find Vordakai's Tomb, Defeat Vordakai]   characters: [Vordakai]   elements: [Vordakai's Tomb]   themes: [undead, lich, dungeon]   location: LV6
gate: none
fragments:
  - plot_point: "Vordakai's Tomb — lich lair, full dungeon in Ch.6 (reached via LV7 stairway)"   themes: [lich, dungeon]   weight: 1
  - plot_point: "Claimed after clearing: Refuge"   themes: [kingdom, resource]   weight: 1

### cluster: lv7 — "LV7. Valley of the Dead"   (source: p.94 / L4562)   mode: sandbox
scene: STANDARD, Severe 9. A six-mile-wide valley entrance the Nomen call "Olah-Kakanket," marked by skull-and-bone totem posts. Inside, oppression grows; thousands of weathered Cyclops-runed gravestones (DC 25 Society to read) mark long-decayed cyclops dead. At the west end a 15-ft stone stairway winds 8 miles up to LV6 (Vordakai's Tomb). Creature: six Skeletal Hulks (Creature 7), guardians raised from great cyclopes, loom at the throat of the stairs.
threads: [Find Vordakai's Tomb]   characters: [Vordakai, Nomen centaur clan]   elements: [Valley of the Dead, cyclops gravestones, stairway to LV6]   themes: [undead, foreboding, gateway]   location: LV7
gate: none
fragments:
  - plot_point: "Bone-totem warning wall marks the cyclops Valley of the Dead (Olah-Kakanket)"   themes: [foreboding, lore]   weight: 1
  - plot_point: "8-mile stairway at the valley's west end ascends to Vordakai's Tomb (LV6)"   themes: [gateway, path]   weight: 1
  - plot_point: "Six Skeletal Hulks (Creature 7) guard the stairway throat"   themes: [undead, combat]   weight: 1

### cluster: lv8 — "LV8. Empty Dragon Lair"   (source: p.94 / L4590)   mode: sandbox
scene: RESOURCE STANDARD. A 300-ft tunnel opens into a 140-ft vaulted chamber holding the dry skeleton of an adult silver dragon — right arm/wing melted by acid, skull and treasure gone. DC 20 Perception spots scattered silver AND black dragon scales: the black dragon Ilthuliak slew the silver dragon Amvarean years ago and stole her hoard (Amvarean's silver skull resurfaces at BR2). Ilthuliak is alive (Ch.10). Resource: Claimed serves as a Refuge.
threads: [Ilthuliak]   characters: [Amvarean (silver dragon), Ilthuliak]   elements: [Empty Dragon Lair, silver dragon skeleton]   themes: [dragon lore, foreshadow, resource]   location: LV8
gate: none
fragments:
  - plot_point: "Acid-melted silver dragon skeleton + black dragon scales: Ilthuliak killed Amvarean and looted her"   themes: [lore, foreshadow]   weight: 1
  - plot_point: "Claimed: Refuge"   themes: [kingdom, resource]   weight: 1

### cluster: ht-zone-table — "Hooktongue — Wandering Encounters (Zone 10)"   (source: p.95 / L4630)   mode: sandbox
scene: d20 Zone 10 table, level ~10. 1–3 = 6 bog striders (trivial), 4–8 = 2 boggard wardens, 9–11 = 6 will-o'-wisps, 12–13 = 3 nuckelavees, 14–15 = 4 marsh giants, 16–17 = 2 giant flytraps, 18–19 = 1 catoblepas, 20 = 1 froghemoth (severe). Bog striders are from Tok-Nikrat (HT12), parley-able and can guide. Boggard wardens are M'botuu (HT6) reinforcements who try to capture PCs alive. Marsh giants are nomadic, hate boggards; beating three may earn a (treacherous) guide. Hooktongue swamp = greater difficult terrain (downgradeable to difficult with rafts + a Fishing/River/Sailor/Swamp Lore expert). Convert to list_d100 generator.
threads: [Save the Bog Strider]   characters: [Tok-Nikrat bog striders, M'botuu boggards, marsh giants]   elements: [Hooktongue Slough]   themes: [swamp, boggards, faction]   location: HT
gate: none
fragments:
  - plot_point: "Swamp is greater difficult terrain; rafts + a swamp-lore expert downgrade it to difficult"   themes: [terrain, logistics]   weight: 1
  - plot_point: "Bog strider encounters tie to Tok-Nikrat (HT12); boggard wardens try to take PCs alive to M'botuu"   themes: [faction, lead]   weight: 1
  - plot_point: "Roll 20: froghemoth (Severe 10)"   themes: [danger]   weight: 1

### cluster: ht1 — "HT1. Wyvernstone Bridge"   (source: p.96 / L4638)   mode: sandbox
scene: LANDMARK RESOURCE. A still-intact stone bridge spanning the East Sellen River gorge, built ~200 years ago after Choral the Conqueror united Brevoy, just before the river empties into Hooktongue Slough. The old roads are gone but the bridge endures.
threads: []   characters: [Choral the Conqueror (lore)]   elements: [Wyvernstone Bridge, East Sellen River]   themes: [landmark, infrastructure]   location: HT1
gate: none
fragments:
  - plot_point: "Intact 200-year-old stone bridge over the East Sellen River gorge"   themes: [landmark, crossing]   weight: 1

### cluster: ht2 — "HT2. Cloudberry Field"   (source: p.96 / L4642)   mode: sandbox
scene: RESOURCE STANDARD. A several-acre meadow of golden cloudberries overlooking northern Hooktongue; it attracts wildlife and predators, so PCs automatically trigger a wandering-monster encounter on first entry. Resource: Harvest Crops / Gather Livestock here succeeds one degree better than rolled.
threads: []   characters: []   elements: [Cloudberry Field]   themes: [resource, foraging]   location: HT2
gate: none
fragments:
  - plot_point: "Cloudberry meadow: auto wandering-monster encounter on first entry"   themes: [hazard, encounter]   weight: 1
  - plot_point: "Harvest/Gather here is one degree of success better"   themes: [resource]   weight: 1

### cluster: ht3 — "HT3. Boggard Ambush"   (source: p.96 / L4650)   mode: sandbox
scene: RESOURCE STANDARD, Moderate 10. An old East Sellen waystation of stilt-buildings, now a ruined ambush nest. The East Sellen trade route is closed due to M'botuu boggard aggression. Creatures: four Boggard Cultists (Creature 8, rare CE; divine casters, Gogunta's Croak fear aura, giant-wasp-venom blowguns, +1 striking whip) — survivors of cleric Sepoko's purge (he tried to sacrifice his cult to the spirit naga Ngara, HT9). They ambush non-stealthy parties; last one standing begs mercy, likely to misdirect PCs toward a predator's den rather than to M'botuu. Resource: ruins can be rebuilt (if Claimed/settled) into Houses, Inns, and Piers.
threads: [Sepoko & Ngara]   characters: [boggard cultists, Sepoko, Ngara]   elements: [Boggard Ambush ruins, East Sellen trade route]   themes: [ambush, boggards, betrayal]   location: HT3
gate: none
fragments:
  - plot_point: "Four Boggard Cultists (Creature 8) ambush from stilt-ruins; survivors of Sepoko's cult purge"   themes: [ambush, boggards]   weight: 1
  - plot_point: "Last survivor begs mercy and misdirects PCs toward a predator den"   themes: [betrayal, lead]   weight: 1
  - plot_point: "Claimed ruins rebuild into Houses, Inns, Piers"   themes: [kingdom, resource]   weight: 1

### cluster: ht4 — "HT4. The Sinking Bog"   (source: p.97 / L4692)   mode: sandbox
scene: STANDARD, Trivial 10. A quicksand-riddled swampland; the hex cannot host roads, settlements, Farmlands, Work Sites, or structures. Hazard: travel auto-exposes PCs to Quicksand (Hazard 3); Reconnoitering additionally exposes them to Green Slime (Hazard 9).
threads: []   characters: []   elements: [Sinking Bog, quicksand, green slime]   themes: [hazard, swamp]   location: HT4
gate: none
fragments:
  - plot_point: "Travel auto-exposes PCs to Quicksand; Reconnoiter adds Green Slime (Hazard 9)"   themes: [hazard]   weight: 1
  - plot_point: "Hex cannot be built on (no roads/settlements/Work Sites)"   themes: [terrain, kingdom]   weight: 1

### cluster: ht5 — "HT5. Haunted Fen"   (source: p.97 / L4714)   mode: sandbox
scene: STANDARD, Severe 10. The most notorious stretch of Lake Hooktongue's haunted north shore; victims turn up missing eyes and fingers. DC 20 Swamp Lore / DC 25 Nature or Society recalls the legend (crit success names an ahuizotl). Creature: Irahkatu, a unique ahuizotl (Creature 13, HP 235), a cunning predator who stalks and uses Voice Imitation to lure stragglers, ambushing the smallest PC, then fighting to the death. Treasure (DC 28 Survival Track / DC 30 Perception to find nest): skulls bearing a silver moonstone circlet (300 gp), 7 gold teeth (70 gp), and a mask of the banshee.
threads: []   characters: [Irahkatu the ahuizotl]   elements: [Haunted Fen, Irahkatu's nest]   themes: [predator, ambush, lake]   location: HT5
gate: none
fragments:
  - plot_point: "Irahkatu the ahuizotl (Creature 13) uses Voice Imitation to lure and ambush the smallest PC"   themes: [predator, ambush]   weight: 1
  - plot_point: "Nest treasure includes a mask of the banshee (DC 28 Survival to locate)"   themes: [treasure]   weight: 1

### cluster: ht6 — "HT6. M'botuu"   (source: p.97 / L4748)   mode: sandbox
scene: LANDMARK RESOURCE. The largest boggard settlement in Hooktongue, detailed in Part 9 of this chapter (p.154); ruled by priest-king Sepoko as proxy for the naga Ngara. Ka-Kekt (the captured bog strider) is held here (prison at G4). Resource: M'botuu is a Freehold; integrated, it gives a village with free Barracks and Tenements and one Water-border Urban Grid edge.
threads: [Save the Bog Strider, Sepoko & Ngara]   characters: [Sepoko, M'botuu boggards, Ka-Kekt]   elements: [M'botuu village]   themes: [boggards, settlement, faction]   location: HT6
gate: none
fragments:
  - plot_point: "M'botuu — largest boggard village, ruled by Sepoko as Ngara's proxy (full detail p.154)"   themes: [settlement, boggards]   weight: 1
  - plot_point: "Ka-Kekt held prisoner here (cell at G4) — target of Save the Bog Strider quest"   themes: [quest, rescue]   weight: 1
  - plot_point: "Integrated as Freehold: village with free Barracks + Tenements"   themes: [kingdom, resource]   weight: 1

### cluster: ht7 — "HT7. Lake Hooktongue"   (source: p.98 / L4754)   mode: sandbox
scene: LANDMARK RESOURCE, Extreme 10. The heart of the slough, up to 900 ft deep, rumored lair of the water orm Hooktongue (DC 15 River Lore / DC 20 Nature/Society for legend; many think it dead). Creature: Hooktongue, a unique water orm (Creature 14, HP 275, Undetectable, Poison Spray, Capsize), recently awoken and hungry — it endangers all who travel/fish the lake. Reduced to ≤30 HP it flees upriver. Treasure: a sunken barge (DC 20 Perception, water-breathing) holds a chest with coins, lifting belt, wand of remove disease, moonlit chain, minor sturdy shield. Resource: while it lives, Boating checks here drop one degree; slaying it reduces Unrest by 4, makes the hex a Landmark, and cuts kingdom Consumption by 1.
threads: [Slay Hooktongue]   characters: [Hooktongue the water orm]   elements: [Lake Hooktongue, sunken barge]   themes: [lake monster, treasure, kingdom-boon]   location: HT7
gate: none
fragments:
  - plot_point: "Hooktongue the water orm (Creature 14, Extreme) endangers all lake travel; flees at ≤30 HP"   themes: [boss, lake]   weight: 1
  - plot_point: "Sunken barge treasure: lifting belt, wand of remove disease, moonlit chain"   themes: [treasure]   weight: 1
  - plot_point: "Slaying Hooktongue: Unrest -4, hex becomes Landmark, Consumption -1"   themes: [kingdom, reward]   weight: 1

### cluster: ht8 — "HT8. Dragonfly Glade"   (source: p.98 / L4810)   mode: sandbox
scene: STANDARD, Severe 10. A beautiful glade of dragonflies; most are harmless but four Enormous Dragonflies (Creature 9, HP 165, 16-ft wingspans) attack on sight and fight to the death. Treasure: a boggard skeleton holds a greater animal staff. Quest: Dragonfly Cloak, 30 XP — Erastil cleric Berzaki (offered at PC level 9) wants a set of large dragonfly wings; harvesting all four enormous dragonflies' wings yields a cape of the mountebank as reward.
threads: [Dragonfly Cloak quest]   characters: [Berzaki the cleric, enormous dragonflies]   elements: [Dragonfly Glade]   themes: [insects, quest, crafting]   location: HT8
gate: none
fragments:
  - plot_point: "Four Enormous Dragonflies (Creature 9) attack on sight"   themes: [combat]   weight: 1
  - plot_point: "Harvest their wings for Berzaki's Dragonfly Cloak quest → cape of the mountebank"   themes: [quest, reward]   weight: 1
  - plot_point: "greater animal staff on a dead boggard nearby"   themes: [treasure]   weight: 1

### cluster: ht9 — "HT9. The Swamp Scar"   (source: p.100 / L4850)   mode: sandbox
scene: LANDMARK, Severe 10. A 500-ft-long, 40-ft-high mound of decaying logs riddled with burrows. Creature: Ngara, a unique spirit naga (Creature 12, HP 215, occult caster with dominate/feeblemind, the inveigle ritual) who enslaves humanoids as hunters or eats them. She keeps two inveigled Marsh Giants (Creature 8) as guards and runs M'botuu through her enthralled proxy Sepoko. Treasure: her dangling ring collection — 15 nonmagical rings (500 gp total), a ring of the ram, and a ring of wizardry I.
threads: [Sepoko & Ngara]   characters: [Ngara the spirit naga, Sepoko, marsh giants]   elements: [Swamp Scar]   themes: [naga, mind-control, mastermind]   location: HT9
gate: none
fragments:
  - plot_point: "Ngara the spirit naga (Creature 12) — the true power behind M'botuu, controls Sepoko via inveigle"   themes: [mastermind, mind-control]   weight: 1
  - plot_point: "Two inveigled Marsh Giants (Creature 8) guard her lair"   themes: [combat]   weight: 1
  - plot_point: "Ring hoard: ring of the ram, ring of wizardry I, + 15 rings (500 gp)"   themes: [treasure]   weight: 1

### cluster: ht10 — "HT10. Chuul Lair"   (source: p.101 / L4884)   mode: sandbox
scene: STANDARD, Moderate 10. A rushes-hidden shore cave, den of four Elite Chuuls (Creature 8); one waits inside, three ambush from the water. Walls bear blood paintings of chuuls eating humans. They flank and fight to the death. Treasure: silver-shod +1 quarterstaff (carved, 180 gp), boots of bounding, coral Gozreh holy symbol (50 gp), mithral brooch (100 gp), iron medallion talisman.
threads: []   characters: [chuuls]   elements: [Chuul Lair]   themes: [ambush, predator]   location: HT10
gate: none
fragments:
  - plot_point: "Four Elite Chuuls (Creature 8) ambush from cave and water, fight to the death"   themes: [combat, ambush]   weight: 1
  - plot_point: "Trophy hoard: boots of bounding, +1 quarterstaff, iron medallion talisman"   themes: [treasure]   weight: 1

### cluster: ht11 — "HT11. Lily Patch"   (source: p.101 / L4902)   mode: sandbox
scene: RESOURCE STANDARD, Moderate 10. A rare grove of carnivorous Azure Lilies on a hummock. Hazard: Azure Lilies (Hazard 12, rare environmental; Pollen Burst, 30-ft radius, DC 30 Will, up to 20d6 mental + confusion). Travel = DC 11 flat check to avoid; Reconnoiter = automatic full-party exposure. Disable (DC 33 Nature/Survival) harvests pollen. Treasure: harvest yields up to 5 doses of azure lily pollen toxin (p.584). Resource: Claimed + Master Agriculture enables the Harvest Azure Lily Pollen downtime Region activity (DC 30 Agriculture; can raise Crime/Unrest on failure).
threads: []   characters: []   elements: [Azure Lily patch]   themes: [hazard, poison, resource]   location: HT11
gate: none
fragments:
  - plot_point: "Azure Lilies (Hazard 12): Pollen Burst up to 20d6 mental + 1-minute confusion (DC 30 Will)"   themes: [hazard, poison]   weight: 1
  - plot_point: "Disable (DC 33) to harvest up to 5 doses of azure lily pollen toxin"   themes: [resource, crafting]   weight: 1
  - plot_point: "Claimed + Master Agriculture: Harvest Azure Lily Pollen downtime activity"   themes: [kingdom, resource]   weight: 1

### cluster: ht12 — "HT12. Tok-Nikrat"   (source: p.102 / L4948)   mode: sandbox
scene: STANDARD, Trivial 10. A wooded island ringed by open water, home to ~a dozen Bog Striders (Creature 2) led by aging Tok-Tekt (Creature 3), waging attrition against the swamp's boggards. His son Ka-Kekt was captured by M'botuu raiders. Bog striders are insular and initially hostile; PCs must shift them friendly (or rescue Ka-Kekt) to be welcomed. Quest: Save the Bog Strider, 30 XP / 30 Kingdom XP — free Ka-Kekt from G4; reward is "bog friend" status, full knowledge of every Hooktongue encounter area, and automatic integration of Tok-Nikrat (very small Freehold; village with one Tenements lot, all-Water borders).
threads: [Save the Bog Strider]   characters: [Tok-Tekt, Ka-Kekt, bog striders]   elements: [Tok-Nikrat island]   themes: [faction, rescue, settlement]   location: HT12
gate: none
fragments:
  - plot_point: "Tok-Tekt (Creature 3) leads ~12 bog striders; begs PCs to rescue his son Ka-Kekt from M'botuu"   themes: [quest, faction]   weight: 1
  - plot_point: "Quest reward: full intel on all Hooktongue encounter areas + Tok-Nikrat integration"   themes: [reward, intel]   weight: 1

### cluster: ht13 — "HT13. Bog of Bones"   (source: p.102 / L4984)   mode: sandbox
scene: STANDARD, Moderate 10. A chill, silent marsh of swamp-gas plumes. Creatures: three Bog Mummy Cultists (Creature 9, rare NE; once Urgathoa priests from Pitax who murdered a fourth, then were cursed into bog mummies and forbidden to leave). They have Breath of the Bog aura (drowning), Bog Rot disease, and Rejuvenation (only positive damage or a consecrate ritual stops it). Rise Up reaction lets a buried mummy Burrow before initiative.
threads: []   characters: [bog mummy cultists]   elements: [Bog of Bones]   themes: [undead, curse, swamp]   location: HT13
gate: none
fragments:
  - plot_point: "Three Bog Mummy Cultists (Creature 9), cursed Urgathoa priests bound to the bog forever"   themes: [undead, lore]   weight: 1
  - plot_point: "Rejuvenation: stopped only by positive damage or a consecrate ritual"   themes: [undead, mechanic]   weight: 1

### cluster: ht14 — "HT14. Hydra Den"   (source: p.103 / L5022)   mode: sandbox
scene: STANDARD, Severe 10. A deep pond and reed bog; lair of the Hooktongue Hydra, a unique 12-headed hydra (Creature 13, HP 240, hydra regeneration 15, weakness slashing 5). It ambushes from the water, rolling Stealth for initiative. Treasure: a dead elf traveler's mud-caked but undamaged oathbow.
threads: []   characters: [Hooktongue Hydra]   elements: [Hydra Den]   themes: [predator, ambush]   location: HT14
gate: none
fragments:
  - plot_point: "Hooktongue Hydra (Creature 13, 12 heads) ambushes from the water; weak to slashing"   themes: [boss, combat]   weight: 1
  - plot_point: "oathbow in the den"   themes: [treasure]   weight: 1

### cluster: ht15 — "HT15. Slug Bog"   (source: p.103 / L5044)   mode: sandbox
scene: STANDARD, Severe 10. A giant-slug mating ground where six agitated Giant Slugs (Creature 8) thrash and spit acid, aggressively attacking passers-by. Quest: Wanted: Slug Spit, 30 XP — eccentric alchemist Chesk Umberweed (wanted posters at PC level 10) needs a dozen vials of giant slug acid, harvestable within an hour of a slug's death; reward is 4 moderate elixirs of life + 3 greater alchemist's fires.
threads: [Wanted: Slug Spit]   characters: [giant slugs, Chesk Umberweed]   elements: [Slug Bog]   themes: [vermin, quest, harvest]   location: HT15
gate: none
fragments:
  - plot_point: "Six Giant Slugs (Creature 8) spit acid and attack all comers"   themes: [combat]   weight: 1
  - plot_point: "Harvest slug acid (within 1 hr of death) for Chesk Umberweed's Wanted: Slug Spit quest"   themes: [quest, harvest]   weight: 1

### cluster: dr-zone-table — "Drelev — Wandering Encounters (Zone 11)"   (source: p.104 / L5076)   mode: sandbox
scene: d20 Zone 11 table, level ~11. 1–5 = Zone 10 table; 6–8 = 6 hill giants, 9–11 = 1 cauthooj, 12–13 = 3 giant flytraps, 14–15 = 4 aurumvoraxes, 16–17 = 1 irlgaunt, 18–19 = 1 viper vine, 20 = 1 ankou (severe). Any wild ankou is secretly an agent of Nyrissa testing the PCs (recurs through later zones). Hill giants were driven south from Glenebon/Tiger Lords; eager to rob PCs but break and sue for peace at half losses. Convert to list_d100 generator.
threads: [Nyrissa's agents]   characters: [Nyrissa, ankou, hill giants]   elements: [Drelev grasslands]   themes: [fey, faction, foreshadow]   location: DR
gate: none
fragments:
  - plot_point: "Wild ankou encounters are Nyrissa's agents testing the PCs (recurring across zones 11–18)"   themes: [foreshadow, fey]   weight: 1
  - plot_point: "Hill giants break and sue for peace at half losses"   themes: [combat, diplomacy]   weight: 1

### cluster: dr1 — "DR1. Speartooth's Den"   (source: p.104 / L5088)   mode: sandbox
scene: HIDDEN, Severe 11. A thorny valley; DC 30 Nature/Perception or DC 25 Plains Lore (during Reconnoiter) reveals a great cat's sign, then DC 30 Survival to Track it through a thorn tunnel. Creature: Speartooth, a unique scarred man-eating smilodon (Creature 14, HP 255) revered as a god by the Tiger Lords, dreaded by Fort Drelev (it has killed two dozen guards). DC 11 flat check for presence; fights to the death. Treasure: among 24 dead Drelev guards lies a Pitax hunter's +1 striking shock composite longbow and two viper arrows. Tied to the Wanted: Speartooth quest below.
threads: [Wanted: Speartooth]   characters: [Speartooth the smilodon, Tiger Lords]   elements: [Speartooth's Den]   themes: [man-eater, hidden, predator]   location: DR1
gate: none
fragments:
  - plot_point: "Speartooth, unique man-eating smilodon (Creature 14), revered by Tiger Lords; fights to the death"   themes: [boss, predator]   weight: 1
  - plot_point: "Hidden lair: DC 30 Survival to Track through the thorn tunnel"   themes: [hidden, tracking]   weight: 1
  - plot_point: "Loot: +1 striking shock composite longbow + viper arrows from a dead Pitax hunter"   themes: [treasure]   weight: 1

### cluster: dr1-quest — "Wanted: Speartooth (quest)"   (source: p.105 / L5116)   mode: sandbox
scene: Wanted poster (appears at PC level 11): kill the saber-toothed man-eater Speartooth and deliver its 22-inch fangs to any settlement's captain of the guard. 30 XP. Reward: 2,000 gp bounty.
threads: [Wanted: Speartooth]   characters: [Speartooth]   elements: [bounty]   themes: [quest, bounty]   location: DR1
gate: PC level 11 (poster appears)
fragments:
  - plot_point: "Deliver Speartooth's fangs to a guard captain for a 2,000 gp bounty"   themes: [quest, reward]   weight: 1

### cluster: dr2 — "DR2. Fort Drelev"   (source: p.105 / L5126)   mode: sandbox
scene: LANDMARK RESOURCE. Baron Hannis Drelev's fort-and-town on Lake Hooktongue's solid shore; under construction if visited before Ch.7, fully detailed in Part 2 of Ch.7 (p.308). Resource: a Freehold town (kingdom must be ≥3rd level to integrate); four blocks, 16 built lots including Festival Hall, Keep, Temple, Watchtower, Smithy, etc.
threads: [Fort Drelev arc]   characters: [Baron Hannis Drelev]   elements: [Fort Drelev]   themes: [settlement, faction]   location: DR2
gate: none
fragments:
  - plot_point: "Fort Drelev — Baron Hannis Drelev's town (full detail Ch.7 Part 2, p.308)"   themes: [settlement, faction]   weight: 1
  - plot_point: "Integrated: Freehold town with 16 built lots (Keep, Temple, Watchtower...)"   themes: [kingdom, resource]   weight: 1

### cluster: dr3 — "DR3. Wild Horses"   (source: p.105 / L5136)   mode: sandbox
scene: STANDARD, Trivial 11. A herd of 16 Riding Horses (Creature 1) led by Windchaser, a unique awakened, speaking war horse (Creature 8, CN) freed and uplifted by a dying druid (the same druid who awakened Hillstomper at NU1). Initially unfriendly; if made friendly, Windchaser reveals all non-hidden encounter areas in the Slough's hills/plains, including the location of Armag's Tomb and that the Tiger Lords hide in a valley there. Made helpful, may become a PC's mount.
threads: [Find Armag's Tomb]   characters: [Windchaser]   elements: [wild horse herd]   themes: [awakened beast, intel, mount]   location: DR3
gate: none
fragments:
  - plot_point: "Windchaser, awakened speaking war horse (Creature 8); befriend for intel on encounter areas"   themes: [awakened beast, intel]   weight: 1
  - plot_point: "Windchaser reveals Armag's Tomb location and the Tiger Lords' hidden valley"   themes: [lead, faction]   weight: 1

### cluster: dr4 — "DR4. Desperate Refugees"   (source: p.105 / L5158)   mode: sandbox
scene: RESOURCE STANDARD. Empty at campaign start; once Chapter 5 begins, a band of Pitaxian refugees (merchants, performers, Hanspur worshippers) huddle here, too afraid to advance or retreat. They beg the PCs to escort them east. Resource: safely delivering them to a settlement reduces Unrest by 2 and grants a free Trade Shop (no Civic-activity-limit cost).
threads: [Pitax refugees]   characters: [Pitaxian refugees]   elements: [refugee camp]   themes: [escort, kindness, kingdom]   location: DR4
gate: Chapter 5 begins (refugees appear)
fragments:
  - plot_point: "Pitaxian refugees beg escort east (appears once Ch.5 begins)"   themes: [escort, quest]   weight: 1
  - plot_point: "Safe delivery: Unrest -2 and a free Trade Shop"   themes: [kingdom, reward]   weight: 1

### cluster: tl-zone-table — "Tiger Lords — Wandering Encounters (Zone 12)"   (source: p.105 / L5176)   mode: sandbox
scene: d20 Zone 12 table, level ~12. 1–5 = Zone 11 table; 6–8 = 4 aurumvoraxes, 9–11 = 4 mastodons, 12–13 = 4 Tiger Lords, 14–15 = 1 ankou, 16–17 = 2 athachs, 18–19 = 1 doprillu, 20 = 1 jotund troll (severe). A Tiger Lord warband is four barbarians tied to (but distinct from) the camp at Armag's Tomb (TL3); they attack on sight, but captives may boast clues to the tomb's location. Convert to list_d100 generator.
threads: [Find Armag's Tomb]   characters: [Tiger Lords, ankou]   elements: [Tiger Lord hills]   themes: [barbarians, faction]   location: TL
gate: none
fragments:
  - plot_point: "Tiger Lord warbands (4 each) attack on sight; captives may reveal Armag's Tomb clues"   themes: [faction, lead]   weight: 1
  - plot_point: "Roll 20: jotund troll (Severe 12)"   themes: [danger]   weight: 1

### cluster: tl1 — "TL1. Flooded Mine"   (source: p.106 / L5182)   mode: sandbox
scene: RESOURCE STANDARD. A silver mine Hannis Drelev's men dug, abandoned after striking an aquifer that flooded it; the Tiger Lords later cut off access. Resource: Claimed, it needs the Repair the Flooded Mine Leadership downtime activity (kingdom Master rank Engineering, spend 20 RP, DC 32 Engineering) to become a Work Site producing 2 Ore Commodities.
threads: []   characters: [Hannis Drelev (lore)]   elements: [Flooded Mine]   themes: [resource, mining, kingdom]   location: TL1
gate: none
fragments:
  - plot_point: "Flooded silver mine; Repair the Flooded Mine activity (Master Engineering, 20 RP, DC 32) yields 2 Ore"   themes: [resource, kingdom]   weight: 1

### cluster: tl2 — "TL2. Giant's Cave"   (source: p.106 / L5206)   mode: sandbox
scene: RESOURCE STANDARD, Severe 12. Wrecked wagons litter a hill cave. Creatures: Darg, Fesl, and Urda — three unique Hill Giants (Creature 12, HP 250) who refused Armag's alliance and waylay border travelers; they bicker over loot (–2 Perception) and fight to the death. Treasure: 700 sp, 208 gp, +1 resilient half-plate, spyglass, greater juggernaut mutagen, potion of flying, +2 striking dwarven waraxe. Resource: their wagonloads of tools grant 4 bonus Resource Dice next turn; cleared + Claimed, the hex is a Refuge.
threads: []   characters: [Darg, Fesl, Urda]   elements: [Giant's Cave]   themes: [giants, banditry, treasure]   location: TL2
gate: none
fragments:
  - plot_point: "Darg, Fesl, and Urda — three unique Hill Giants (Creature 12) bandits; fight to the death"   themes: [giants, combat]   weight: 1
  - plot_point: "Loot: +2 striking dwarven waraxe, +1 resilient half-plate, potion of flying"   themes: [treasure]   weight: 1
  - plot_point: "Salvaged tools = 4 bonus Resource Dice; cleared hex = Refuge"   themes: [kingdom, resource]   weight: 1

### cluster: tl3 — "TL3. Armag's Tomb"   (source: p.107 / L5234)   mode: sandbox
scene: RESOURCE STANDARD. The Tiger Lord barbarian holy site and camp, fully detailed in Part 3 of Chapter 7 — the climax of the Tiger Lords arc. Resource: clearing all dangers and Claiming the hex makes it a Refuge.
threads: [Find Armag's Tomb, Tiger Lords arc]   characters: [Armag, Tiger Lords]   elements: [Armag's Tomb]   themes: [barbarians, dungeon, faction]   location: TL3
gate: none
fragments:
  - plot_point: "Armag's Tomb — Tiger Lord holy site and camp (full dungeon in Ch.7 Part 3)"   themes: [dungeon, faction]   weight: 1
  - plot_point: "Cleared + Claimed: Refuge"   themes: [kingdom, resource]   weight: 1

### cluster: tl4 — "TL4. Explorer's Grave"   (source: p.107 / L5240)   mode: sandbox
scene: HIDDEN. A long-dead Taldan explorer half-buried in a cleft; DC 30 Perception (during Reconnoiter) to find the body. Treasure: his usable moderate sturdy steel shield bearing a defunct Taldan noble family's coat of arms.
threads: []   characters: []   elements: [Explorer's Grave]   themes: [hidden, treasure]   location: TL4
gate: none
fragments:
  - plot_point: "Hidden Taldan explorer corpse (DC 30 Perception) with a moderate sturdy steel shield"   themes: [hidden, treasure]   weight: 1

### cluster: tl5 — "TL5. Aurumvorax Den"   (source: p.108 / L5250)   mode: sandbox
scene: STANDARD, Severe 12. A honeycombed granite hill, warren of six hardy Aurumvoraxes (two Elite, Creature 10) that strayed from Numeria; very territorial, pursue for miles, fight to the death. Treasure: reaching the central den (DC 30 Survival / DC 35 Perception, 4-hr Investigate; Medium creatures must Squeeze) yields 3,360 sp, a scepter (250 gp), pearl necklace (80 gp), golden lions figurine, +1 flaming kukri, wand of levitate.
threads: []   characters: [aurumvoraxes]   elements: [Aurumvorax Den]   themes: [predator, treasure]   location: TL5
gate: none
fragments:
  - plot_point: "Six territorial Aurumvoraxes (2 Elite, Creature 10) pursue intruders for miles"   themes: [combat, predator]   weight: 1
  - plot_point: "Central den (DC 30 Survival, must Squeeze): golden lions figurine, +1 flaming kukri, wand of levitate"   themes: [treasure]   weight: 1

### cluster: tl6 — "TL6. Chimera Pride"   (source: p.108 / L5268)   mode: sandbox
scene: STANDARD, Severe 12. A bone-strewn hilltop cave; a pride of three Oversized Chimeras (Creature 12, rare CE, HP 220, fire breath, Triple Opportunity) that hunt wild horses. They strafe with breath weapons before swooping; the last flees below 25 HP. Treasure: a torn boggard sorcerer's body holds type I bracers of armor, wand of lightning bolt, +1 corrosive striking whip.
threads: []   characters: [oversized chimeras]   elements: [Chimera Pride cave]   themes: [aerial predator, treasure]   location: TL6
gate: none
fragments:
  - plot_point: "Three Oversized Chimeras (Creature 12) strafe with fire breath; last flees below 25 HP"   themes: [combat, aerial]   weight: 1
  - plot_point: "Loot: type I bracers of armor, wand of lightning bolt, +1 corrosive striking whip"   themes: [treasure]   weight: 1

### cluster: ru-zone-table — "Rushlight — Wandering Encounters (Zone 13)"   (source: p.109 / L5308)   mode: sandbox
scene: d20 Zone 13 table, level ~13. 1–5 = Zone 12 table; 6–8 = 6 mastodons, 9–11 = 1 ankou, 12–13 = 3 cauthoojes, 14–15 = 2 irlgaunts, 16–17 = 1 wemmuth, 18–19 = 3 Pitax wardens, 20 = 1 warsworn (severe). King Irovetti stocked Rushlight (his private hunting grounds) with dangerous creatures. Pitax wardens (3) interrogate or attack depending on war state and answers; if war is won, reroll on the Zone 14 table. Warsworns only appear after the War of the River Kings begins. Convert to list_d100 generator.
threads: [War of the River Kings]   characters: [Pitax wardens, Irovetti]   elements: [Rushlight]   themes: [pitax, faction, war]   location: RU
gate: none
fragments:
  - plot_point: "Irovetti stocked Rushlight (his hunting grounds) with dangerous beasts"   themes: [pitax, lore]   weight: 1
  - plot_point: "Pitax wardens interrogate or attack; warsworns appear only after the War begins"   themes: [faction, war]   weight: 1

### cluster: ru1 — "RU1. Hemlock Island"   (source: p.109 / L5316)   mode: sandbox
scene: LANDMARK. A scenic island reputed (like Candlemere) to be haunted by "lights," but holding only rainbow egrets that scream like humans when slain and a deep central spring feeding Rushlight's lake/rivers. No ruins or monsters. It is Ilora Nuski's proposed meeting place with the PCs (see GU3) once the War of the River Kings begins.
threads: [War of the River Kings, Ilora's alliance]   characters: [Ilora Nuski]   elements: [Hemlock Island]   themes: [landmark, rendezvous]   location: RU1
gate: none
fragments:
  - plot_point: "Hemlock Island — Ilora Nuski's rendezvous point with the PCs once the War begins"   themes: [rendezvous, alliance]   weight: 1

### cluster: ru2 — "RU2. Rushlight Festival Grounds"   (source: p.109 / L5322)   mode: sandbox
scene: LANDMARK RESOURCE. Irovetti's tournament/festival grounds, road-connected to Pitax and well patrolled (all wandering encounters here are Pitax wardens until the War begins). Detailed in Part 1 of Chapter 8. Resource: Claiming it is an act of war (ends Pitax diplomacy, raises Pitax Negotiation DC to 40); a settlement here gains free Cistern + Houses and halves the cost of an Arena.
threads: [War of the River Kings, Rushlight Tournament]   characters: [Irovetti, Pitax wardens]   elements: [Rushlight Festival Grounds, coliseum]   themes: [pitax, festival, war]   location: RU2
gate: none
fragments:
  - plot_point: "Rushlight Festival Grounds — Irovetti's tournament site (full detail Ch.8 Part 1)"   themes: [pitax, festival]   weight: 1
  - plot_point: "Claiming it is an act of war; coliseum halves Arena cost"   themes: [war, kingdom]   weight: 1

### cluster: ru3 — "RU3. Catspaw Camp"   (source: p.109 / L5332)   mode: sandbox
scene: STANDARD. Empty until the War of the River Kings, when the Catspaw Marauders camp here (see Ch.8 p.353).
threads: [War of the River Kings]   characters: [Catspaw Marauders]   elements: [Catspaw Camp]   themes: [war, faction]   location: RU3
gate: War of the River Kings begins (marauders appear)
fragments:
  - plot_point: "Catspaw Marauders camp here once the War begins (Ch.8 p.353)"   themes: [war, faction]   weight: 1

### cluster: gl-zone-table — "Glenebon Lowlands — Wandering Encounters (Zone 14)"   (source: p.109 / L5342)   mode: sandbox
scene: d20 Zone 14 table, level ~14. 1–5 = Zone 13 table; 6–8 = 6 mammoths, 9–11 = 1 jotund troll, 12–13 = 3 irlgaunts, 14–15 = 4 athachs, 16–17 = 2 ankous, 18–19 = 1 warsworn, 20 = wild hunt (severe; a wild hunt archer + hound). The wild hunt are First World scouts "practicing" for a greater hunt; they break off and call truce below 60 HP. Convert to list_d100 generator.
threads: [Wild Hunt, War of the River Kings]   characters: [wild hunt, ankou]   elements: [Glenebon Lowlands]   themes: [fey, war, foreshadow]   location: GL
gate: none
fragments:
  - plot_point: "Wild hunt scouts (archer + hound) attack for sport, truce below 60 HP — foreshadow Ch.10"   themes: [fey, foreshadow]   weight: 1

### cluster: gl1 — "GL1. Tusker's Stomping Ground"   (source: p.110 / L5352)   mode: sandbox
scene: STANDARD. Empty until the War; then it becomes the camp of Tusker's Raiders (hill giants under Castruccio's banner) — see Ch.8 p.351.
threads: [War of the River Kings]   characters: [Tusker's Raiders]   elements: [Tusker's Stomping Ground]   themes: [war, giants]   location: GL1
gate: War of the River Kings begins
fragments:
  - plot_point: "Tusker's Raiders (hill giants) camp here once the War begins (Ch.8 p.351)"   themes: [war, giants]   weight: 1

### cluster: gl2 — "GL2. Marshaling Ground"   (source: p.110 / L5356)   mode: sandbox
scene: STANDARD. Empty until the War; then the marshaling ground for the Pitax Horde (Ch.8 p.353).
threads: [War of the River Kings]   characters: [Pitax Horde]   elements: [Marshaling Ground]   themes: [war, army]   location: GL2
gate: War of the River Kings begins
fragments:
  - plot_point: "Pitax Horde marshals here once the War begins (Ch.8 p.353)"   themes: [war, army]   weight: 1

### cluster: px-zone-table — "Pitax — Wandering Encounters (Zone 15)"   (source: p.110 / L5368)   mode: sandbox
scene: d20 Zone 15 table, level ~15. 1–12 = 4 Pitax wardens (low), 13–16 = 2 ankous, 17–19 = wild hunt (archer + hound), 20 = 2 warsworns (severe). All zone hexes are officially Pitax — Claiming any is an act of war (allowed only after Pitax is defeated). If the war is already won, reroll wardens via 1d8+12. Wild hunt here avoid combat and merely observe, teasing the PCs about "the coming chase." Convert to list_d100 generator.
threads: [War of the River Kings, Wild Hunt]   characters: [Pitax wardens, wild hunt, warsworns]   elements: [Pitax nation]   themes: [pitax, war, fey]   location: PX
gate: none
fragments:
  - plot_point: "Claiming any Pitax hex is an act of war (allowed only after Pitax falls)"   themes: [war, kingdom]   weight: 1
  - plot_point: "Wild hunt here observe rather than fight, foreshadowing the final chapter"   themes: [fey, foreshadow]   weight: 1

### cluster: px1 — "PX1. Littletown"   (source: p.110 / L5380)   mode: sandbox
scene: LANDMARK RESOURCE. A cozy LN village (Settlement 2, pop. 297) of farmers and vintners upstream from Pitax, mayor Lorthy Kullden, ignorant of Irovetti's plan to sacrifice it to the war. Cozy and Fortunate: long-term rest here grants +5 HP. If visited after the War begins, it's in ruins (Ch.8 p.353). Resource: only available after its destruction; rebuilds into Houses, General Store, Town Hall.
threads: [War of the River Kings]   characters: [Lorthy Kullden, Irovetti]   elements: [Littletown]   themes: [pitax, village, tragedy]   location: PX1
gate: none
fragments:
  - plot_point: "Littletown — cozy LN vintner village (pop. 297), doomed by Irovetti's war plans"   themes: [village, tragedy]   weight: 1
  - plot_point: "Long-term rest here grants +5 HP (Cozy and Fortunate)"   themes: [rest, boon]   weight: 1

### cluster: px2 — "PX2. Pitax"   (source: p.110 / L5398)   mode: sandbox
scene: LANDMARK RESOURCE. The capital city of Pitax, Irovetti's seat, fully detailed in Chapter 8 (stat block + integration resources).
threads: [War of the River Kings, Defeat Irovetti]   characters: [Irovetti]   elements: [Pitax city]   themes: [pitax, capital, war]   location: PX2
gate: none
fragments:
  - plot_point: "Pitax — Irovetti's capital city (full detail Ch.8)"   themes: [capital, faction]   weight: 1

### cluster: gu-zone-table — "Glenebon Uplands — Wandering Encounters (Zone 16)"   (source: p.110 / L5410)   mode: sandbox
scene: d20 Zone 16 table, level ~16. 1–5 = Zone 14 list; 6–8 = 3 ankous, 9–11 = 2 wemmuths, 12–13 = wild hunt, 14–15 = 6 elite athachs, 16–17 = 2 skulltakers, 18–19 = 4 hill giant butchers, 20 = Minognos-Ushad (severe). Hill Giant Butchers (Creature 14, rare CE; Menace Prey, Twin Butchery, Sneak Attack) serve Kob Moleg, hunting humanoids (esp. adventurers) for food. Minognos-Ushad the "Eater of Kings" wyvern overflies to scare but won't attack unprovoked; if fought she flees to BR3 at ≤100 HP. Wild hunt = archer (mounted) + hound, truce below 60 HP. Convert to list_d100 generator.
threads: [The Eater of Kings, Wild Hunt]   characters: [hill giant butchers, Kob Moleg, Minognos-Ushad, wild hunt]   elements: [Glenebon Uplands]   themes: [giants, wyvern, fey]   location: GU
gate: none
fragments:
  - plot_point: "Hill Giant Butchers (Creature 14) serve Kob Moleg, hunting humanoids for meat"   themes: [giants, faction]   weight: 1
  - plot_point: "Minognos-Ushad overflies to scare; flees to Hungerdark (BR3) at ≤100 HP if fought"   themes: [wyvern, lead]   weight: 1

### cluster: gu-quest-eater — "The Eater of Kings (quest)"   (source: p.111 / L5442)   mode: sandbox
scene: At PC level 15, rumors of Minognos-Ushad ("Eater of Kings") spread through the kingdom. Research via DC 39 Arcana / DC 34 Dragon Lore: failure still reveals she hunts the Glenebon Uplands and Numeria; success reveals her lair is in the Branthlend Mountains; crit success names Hungerdark (BR3). 30 XP / 30 Kingdom XP. Completion: kill her (random encounter or in her lair). Reward: the Tiger Lords are so impressed they pledge fealty (auto crit success at Pledge of Fealty), or, if already pledged, bring 6 bonus Resource Dice.
threads: [The Eater of Kings]   characters: [Minognos-Ushad, Tiger Lords]   elements: [Hungerdark]   themes: [quest, wyvern, faction]   location: GU
gate: PC level 15 (rumors begin)
fragments:
  - plot_point: "Research Minognos-Ushad (DC 39 Arcana/34 Dragon Lore) to locate her at Hungerdark (BR3)"   themes: [quest, investigation]   weight: 1
  - plot_point: "Killing her wins the Tiger Lords' fealty (auto crit Pledge) or 6 bonus Resource Dice"   themes: [reward, faction]   weight: 1

### cluster: gu1 — "GU1. Steamgrotto"   (source: p.111 / L5456)   mode: sandbox
scene: LANDMARK, Low 16. Sulfurous geyser ponds erupting boiling water/steam at unpredictable timing. Travel auto-triggers the Navigate Steamgrotto exploration activity (Nature/Perception/Survival, DC 35; failure 10d6 fire, crit fail 20d6, DC 36 basic Reflex); Reconnoiter worsens the result one degree. Hex cannot be built on. First time Navigating Steamgrotto (any result) earns 30 XP.
threads: []   characters: []   elements: [Steamgrotto geysers]   themes: [hazard, landmark]   location: GU1
gate: none
fragments:
  - plot_point: "Navigate Steamgrotto activity (DC 35); failure 10d6 / crit fail 20d6 fire"   themes: [hazard]   weight: 1
  - plot_point: "First Navigate (any result) awards 30 XP; hex cannot be built on"   themes: [reward, terrain]   weight: 1

### cluster: gu2 — "GU2. Whiterose"   (source: p.112 / L5480)   mode: sandbox
scene: LANDMARK RESOURCE. Whiterose and its hilltop abbey, fully detailed in Part 3 of Chapter 8. Resource: once the abbey and its dangers are dealt with, it is a Refuge if Claimed; a settlement gains a free Temple (abbey) and free Brewery (winery).
threads: [Whiterose arc]   characters: []   elements: [Whiterose Abbey]   themes: [pitax, abbey, resource]   location: GU2
gate: none
fragments:
  - plot_point: "Whiterose Abbey (full detail Ch.8 Part 3); cleared + Claimed = Refuge, free Temple + Brewery"   themes: [abbey, resource]   weight: 1

### cluster: gu3 — "GU3. Ilora's Camp"   (source: p.112 / L5486)   mode: sandbox
scene: SECRET, Trivial 16. A hidden bramble campsite (greater difficult terrain; DC 35 Perception during Reconnoiter to find) by the narrowing Pitax River. Creature: Ilora Nuski, a unique CN human ranger (Creature 12, HP 220, dual shortswords, primal caster), last survivor of the River Razors bandit-rebels who oppose King Castruccio. She knows Pitax's defenses well. If not found, she contacts the PCs once the War begins (via animal messenger) to meet at Hemlock Island (RU1). Befriended early, she grants war advice immediately. Award: securing her aid earns 80 XP.
threads: [War of the River Kings, Ilora's alliance]   characters: [Ilora Nuski, Castruccio Irovetti]   elements: [Ilora's Camp]   themes: [rebel, ally, intel]   location: GU3
gate: none
fragments:
  - plot_point: "Ilora Nuski (Creature 12), last River Razor rebel, knows Pitax's defenses — a key war ally"   themes: [ally, intel]   weight: 1
  - plot_point: "Hidden camp (DC 35 Perception); she invites PCs to Hemlock Island once the War begins"   themes: [secret, rendezvous]   weight: 1
  - plot_point: "Securing Ilora's aid against Pitax awards 80 XP"   themes: [reward]   weight: 1

### cluster: nu-zone-table — "Numeria — Wandering Encounters (Zone 17)"   (source: p.113 / L5544)   mode: sandbox
scene: d20 Zone 17 table, level ~17. 1–3 = Zone 16 table; 4–6 = mammoth herd (trivial), 7–9 = 4 hill giant butchers, 10–11 = 4 ankous, 12–13 = Minognos-Ushad, 14–15 = 2 radiant wardens, 16–17 = 1 elite adamantine golem, 18–19 = wild hunt (scout + 2 hounds), 20 = one elite guthallath (severe). Constructs here are ancient robotic versions (re-skinned with tech: nanites, plasma, laser cones; all gain weakness 15 to crit hits and electricity); GMs may use standard versions or reroll. Mammoth herd encounters can be flavorful non-combat. Convert to list_d100 generator.
threads: [Numerian Trade, The Eater of Kings, Wild Hunt]   characters: [hill giant butchers, Minognos-Ushad, robotic constructs, wild hunt]   elements: [Numeria badlands]   themes: [technology, megafauna, fey]   location: NU
gate: none
fragments:
  - plot_point: "Numerian constructs are ancient robots (tech re-skin; weakness 15 to crits/electricity)"   themes: [technology, lore]   weight: 1
  - plot_point: "Roll 20: elite guthallath (Severe 17)"   themes: [danger]   weight: 1

### cluster: nu-quest-trade — "Numerian Trade (quest)"   (source: p.113 / L5564)   mode: sandbox
scene: At PC level 17, merchant Malchar Tevalkan wants a road built to open a Numerian trade route. 30 XP / 30 Kingdom XP. Completion: build roads connecting a city/metropolis in the kingdom to any Zone 17 hex. Reward: a free Trade Agreement that adds +2 Resource Dice when Managing Trade Agreements (except on a critical failure).
threads: [Numerian Trade]   characters: [Malchar Tevalkan]   elements: [Numeria road]   themes: [quest, kingdom, trade]   location: NU
gate: PC level 17 (Malchar appears)
fragments:
  - plot_point: "Build roads connecting a city to Zone 17 for Malchar's Numerian Trade quest → free Trade Agreement"   themes: [quest, kingdom]   weight: 1

### cluster: nu1 — "NU1. The Mammoth Graveyard"   (source: p.114 / L5572)   mode: sandbox
scene: LANDMARK RESOURCE, Severe 17. A box canyon where dying mammoths gather; a legendary ivory trove (difficult terrain for Huge-or-smaller). Creature: Hillstomper, a unique awakened, speaking mammoth (Creature 11, HP 200, CN-feeling but N) wounded and ashamed — he was charged to guard the graveyard but two Cairn Linnorms (Creature 18!) seized it and maimed him in two failed attempts. Quest: The Mammoth's Shame, 30 XP / 30 Kingdom XP — kill the cairn linnorms; reward is automatic critical-success Claim of the hex. Treasure (the linnorms' hoard): a massive trove incl. 18,200 cp/3,204 sp/260 gp/32 pp, +2 resilient elven chain, +2 greater striking cold iron scimitar, scroll of summon dragon, major staff of fire, boots of speed, dust of disappearance, etc. Resource: Claimed, choose Landmark (+3 Fame) or plunder ivory (+6 Resource Dice, +3 Infamy).
threads: [The Mammoth's Shame]   characters: [Hillstomper, cairn linnorms]   elements: [Mammoth Graveyard]   themes: [awakened beast, linnorm, treasure]   location: NU1
gate: none
fragments:
  - plot_point: "Hillstomper, awakened speaking mammoth (Creature 11), begs help reclaiming the graveyard"   themes: [awakened beast, quest]   weight: 1
  - plot_point: "Two Cairn Linnorms (Creature 18) hold the graveyard — a deadly fight; fight to the death"   themes: [boss, danger]   weight: 1
  - plot_point: "Linnorm hoard: +2 greater striking cold iron scimitar, major staff of fire, boots of speed, scroll of summon dragon"   themes: [treasure]   weight: 1
  - plot_point: "Claimed: choose Landmark (+3 Fame) or plunder ivory (+6 Resource Dice, +3 Infamy)"   themes: [kingdom, choice]   weight: 1

### cluster: tv-zone-table — "Thousand Voices — Wandering Encounters (Zone 18)"   (source: p.115 / L5654)   mode: sandbox
scene: d20 Zone 18 table, level ~18. 1–5 = Zone 16 table; 6–8 = 1 sard, 9–11 = 1 bandersnatch, 12–13 = 6 elite ankous, 14–15 = 3 whimwyrms, 16–17 = wild hunt (2 archers + 4 hounds), 18–19 = Lantern King's emissary, 20 = 1 mu spore (severe). Zone-wide: Nyrissa's whispers impose –1 status to all Will saves (–2 vs emotion; emotion/mental/primal) until she is defeated (end Ch.10); zone is difficult terrain. The Lantern King's emissary is a vilderavn herald on a zomok who poses as Nyrissa's servant, wanting the PCs to keep building their kingdom (so Nyrissa can absorb it); slain, it's replaced by the wild hunt. Convert to list_d100 generator.
threads: [Nyrissa, Lantern King, Wild Hunt]   characters: [vilderavn herald, wild hunt, Nyrissa, Lantern King]   elements: [Thousand Voices forest]   themes: [fey, dread, foreshadow]   location: TV
gate: none
fragments:
  - plot_point: "Nyrissa's whispers: –1 status to Will saves (–2 vs emotion) zone-wide until Ch.10's end"   themes: [curse, fey]   weight: 1
  - plot_point: "Lantern King's emissary (vilderavn on a zomok) secretly wants the PCs to keep building their kingdom"   themes: [mastermind, foreshadow]   weight: 1

### cluster: tv1 — "TV1. Castle of Knives"   (source: p.116 / L5668)   mode: sandbox
scene: RESOURCE SECRET. Blade-like stone monoliths jut skyward — the anchor point for Nyrissa's First World realm of Thousandbreaths, less than a decade old despite looking ancient (DC 38 Architecture/First World Lore confirms; crit success: it's a projection of a larger First World region). Nyrissa and her agents (and the dragon Ilthuliak) open a portal here; in Ch.10 it anchors her blooms. Full travel rules to Thousandbreaths on p.443 (Ch.10). Resource: cannot be salvaged or made a Refuge; if Claimed before Ch.10 ends, Nyrissa's influence makes the hex (and everything built on it) vanish each Kingdom turn.
threads: [Nyrissa, Thousandbreaths portal]   characters: [Nyrissa, Ilthuliak]   elements: [Castle of Knives]   themes: [fey, portal, mystery]   location: TV1
gate: none
fragments:
  - plot_point: "Castle of Knives — recent First World anchor for Nyrissa's Thousandbreaths (DC 38 to reveal its true nature)"   themes: [portal, mystery]   weight: 1
  - plot_point: "Portal route to Thousandbreaths (full rules Ch.10 p.443); also Ilthuliak's travel route"   themes: [gateway, foreshadow]   weight: 1
  - plot_point: "Claimed before Ch.10's end: the hex and its improvements vanish each turn"   themes: [kingdom, curse]   weight: 1

### cluster: tv2 — "TV2. The Weeping Grove"   (source: p.117 / L5700)   mode: sandbox
scene: STANDARD, Severe 18. A lightly forested grove holding three Trees that Weep — unique Gargantuan scythe trees (Creature 18, rare CE, HP 400; Weeping Aura: 30 ft, DC 40 Will, paralysis/sickened; Axe Vulnerability +20; Dead Tree + Woodland Ambush). They pose as dead trees and ambush, rolling Stealth for initiative. Treasure: a long-dead adventurer's skeleton at the grove's center wears +3 greater resilient breastplate and clutches a +3 greater striking bastard sword.
threads: []   characters: [Trees that Weep]   elements: [Weeping Grove]   themes: [plant horror, ambush, treasure]   location: TV2
gate: none
fragments:
  - plot_point: "Three Trees that Weep (Creature 18) ambush from disguise; Weeping Aura paralyzes (DC 40 Will)"   themes: [combat, ambush]   weight: 1
  - plot_point: "Axe Vulnerability: +20 damage from axes"   themes: [tactics]   weight: 1
  - plot_point: "Loot: +3 greater resilient breastplate, +3 greater striking bastard sword"   themes: [treasure]   weight: 1

### cluster: br-zone-table — "Branthlend Mountains — Wandering Encounters (Zone 19)"   (source: p.118 / L5750)   mode: sandbox
scene: d20 Zone 19 table, level ~19. 1–5 = Zone 18 table; 6–8 = 2 skulltakers, 9–11 = wild hunt (2 scouts), 12–13 = 2 bandersnatches, 14–15 = 1 tor linnorm, 16–17 = Ilthuliak, 18–19 = 4 whimwyrms, 20 = 1 elite lerritan (severe). Zone is greater difficult terrain. Ilthuliak (the black dragon, full stats Ch.10 p.454) usually lairs in the First World now; this encounter is a distant glimpse unless the PCs already fought her in Ch.10, in which case she hunts them for revenge. Wild hunt = 2 scouts, truce below 60 HP. Convert to list_d100 generator.
threads: [Ilthuliak, Wild Hunt]   characters: [Ilthuliak, wild hunt scouts]   elements: [Branthlend Mountains]   themes: [dragon, mountains, fey]   location: BR
gate: none
fragments:
  - plot_point: "Ilthuliak the black dragon (Ch.10 p.454): a distant glimpse, unless she's already met the PCs — then she hunts them"   themes: [dragon, foreshadow]   weight: 1
  - plot_point: "Roll 20: elite lerritan (Severe 19)"   themes: [danger]   weight: 1

### cluster: br1 — "BR1. Mount Branthlend"   (source: p.118 / L5762)   mode: sandbox
scene: LANDMARK. The tallest peak in the Stolen Lands (5,400 ft), a white-stone pinnacle. Nomad clans tell that its summit was scoured of life when a scorned warlord's queen transformed into a Numerian spine dragon atop its crown.
threads: []   characters: []   elements: [Mount Branthlend]   themes: [landmark, legend]   location: BR1
gate: none
fragments:
  - plot_point: "Mount Branthlend — tallest peak (5,400 ft); legend of a queen turned spine dragon"   themes: [landmark, lore]   weight: 1

### cluster: br2 — "BR2. Ilthuliak's Lair"   (source: p.118 / L5766)   mode: sandbox
scene: LANDMARK. A 2-mile swamp around a deep tarn beneath a 900-ft waterfall; half-melted rocks, countless bones, and a silver dragon's skull impaled on a dead oak. DC 30 Arcana reads a black dragon's lair-signs (crit: a great wyrm); DC 26 Dragon Lore/Society recalls tales of Ilthuliak; DC 32 Arcana / DC 28 Dragon Lore IDs the skull as the silver dragon Amvarean. Ilthuliak relocated to Thousandbreaths via her Nyrissa alliance (she and her hoard are in Ch.10 p.454); only Amvarean's skull and an empty underwater black-dragon nest remain.
threads: [Ilthuliak]   characters: [Ilthuliak, Amvarean]   elements: [Ilthuliak's Lair, Amvarean's skull]   themes: [dragon, lore, foreshadow]   location: BR2
gate: none
fragments:
  - plot_point: "Ilthuliak's abandoned tarn lair, marked by Amvarean's impaled silver skull; she's relocated to Thousandbreaths (Ch.10)"   themes: [dragon, lore]   weight: 1
  - plot_point: "Only an empty underwater black-dragon nest remains; no hoard"   themes: [foreshadow]   weight: 1

### cluster: br3 — "BR3. Hungerdark"   (source: p.119 / L5774)   mode: sandbox
scene: RESOURCE STANDARD, Severe 19. A 1,500-ft cleft cavern, lair of Minognos-Ushad ("Eater of Kings"), a unique matriarch wyvern (Creature 19, HP 295, poison breath 20d6, Powerful Dive, wyvern venom). An extremely light sleeper (no Perception penalty asleep), present unless already defeated, fights to the death; she shares the lair with four Whimwyrms (Creature 17). Treasure: a vast hoard incl. 28,110 cp / 13,905 sp / 7,452 gp / 333 pp, an elixir of life + elixir of rejuvenation + an empty Sun Orchid Elixir vial, three monarchs' crowns (500 gp each), anklets of alacrity, greater flame tongue, scroll of meteor swarm, ghost dust talisman. Resource: Claimed, Hungerdark is a Refuge. Completes The Eater of Kings quest (GU).
threads: [The Eater of Kings]   characters: [Minognos-Ushad, whimwyrms]   elements: [Hungerdark]   themes: [wyvern, boss, treasure]   location: BR3
gate: none
fragments:
  - plot_point: "Minognos-Ushad (Creature 19) + four Whimwyrms (Creature 17) lair here; she fights to the death"   themes: [boss, wyvern]   weight: 1
  - plot_point: "Hoard: anklets of alacrity, greater flame tongue, scroll of meteor swarm, elixir of life/rejuvenation, empty Sun Orchid vial"   themes: [treasure]   weight: 1
  - plot_point: "Killing her here completes The Eater of Kings quest (winning the Tiger Lords)"   themes: [quest, faction]   weight: 1

---

## Zone 7 — Dunsward (DS) — added by follow-up patch (source p.87–91 / L4238–4380)

### cluster: ds-zone-table — "Dunsward — Wandering Encounters (Zone 7)"   (source: p.87 / L4242)   mode: sandbox
scene: d20 random-encounter table for Zone 7 (Dunsward), creatures level ~7. 1–5 = 6 centaurs (Low), 6–8 = 3 ogre spiders (Low), 9–11 = 1 bulette (Low), 12–15 = 4 spriggans (Low), 16–17 = 4 cyclopes (Moderate), 18–19 = 1 roc (Moderate), 20 = 1 peluda (Severe). Centaurs (Nomen clan, Ch.6) observe and let the PCs make the first move — parley is possible; they flee at half losses. Spriggan bands here are NOT the ones who later sack Varnhold. Convert to list_d100 generator.
threads: [The Nomen Problem]   characters: [Nomen centaur clan, Dunsward spriggans]   elements: [Dunsward grasslands, ogre spiders]   themes: [wilderness, centaurs]   location: DS
gate: none
fragments:
  - plot_point: "Centaurs observe from afar; violence makes them attack, but they can be parleyed (Nomen clan, Ch.6)"   themes: [Social, Tension]   weight: 1
  - plot_point: "WANTED: Spidersilk — weaver Chamaie Lerian pays slippers of spider climbing for ~dozens of sq yds of ogre-spider silk (DC 25 Nature per harvest, 5 successes)"   themes: [quest]   weight: 1

### cluster: ds1 — "DS1. Nomen Burial Mounds"   (source: p.88 / L4258)   mode: sandbox
scene: RESOURCE STANDARD, Severe 7. Twenty-nine 8-ft stone mounds linked by low walls in an asymmetric spiral — centaur burial mounds (DC 25 Society/Religion to confirm; crit-fail misreads them as Pharasma/eldritch summoning glyphs). Four manticores (Creature 6) now claim the area, swooping with tail spikes then landing; the last flees if three die. Resource: Claiming this hex deeply offends the Nomen clan (+4 Negotiation DC until Abandoned).
threads: [The Nomen Problem]   characters: [manticores, Nomen centaur clan]   elements: [centaur burial mounds]   themes: [Tension, Social]   location: DS1
gate: none
fragments:
  - plot_point: "4 manticores (Creature 6) hold the mounds; aerial spike attacks, last one flees"   themes: [Action]   weight: 1
  - plot_point: "Claiming the hex offends the Nomen (+4 Negotiation DC) — a faction choice"   themes: [Social]   weight: 1

### cluster: ds2 — "DS2. Web Lurker Lair"   (source: p.89 / L4276)   mode: sandbox
scene: STANDARD, Moderate 7. A 30-ft-wide spider-web bridge over a 50-ft chasm; a long-dead dwarf on the far ledge clutches a glowing warhammer as bait. Four elite web lurkers (Creature 4) + a pet ogre spider (Creature 5) wait in the caves below; the bridge is a Dropping Web Trap (Hazard 2, Stealth DC 21, Reflex DC 18 to Grab an Edge, 15 bludgeoning + 30-ft fall). If no one falls, the lurkers bicker 1d3 rounds before attacking. Treasure: +1 striking warhammer, grim trophy talisman, 435 sp/108 cp.
threads: []   characters: [elite web lurkers, ogre spider]   elements: [web bridge, dead dwarf, warhammer]   themes: [Tension, Action]   location: DS2
gate: none
fragments:
  - plot_point: "Dropping Web Trap (Hazard 2) bridge — DC 18 Reflex or fall 30 ft; disable DC 15 Crafting / DC 18 Thievery"   themes: [Tension]   weight: 1
  - plot_point: "4 elite web lurkers + ogre spider ambush; treasure incl. +1 striking warhammer & grim trophy talisman"   themes: [Action]   weight: 1

### cluster: ds3 — "DS3. Kiravoy Bridge"   (source: p.90 / L4320)   mode: sandbox
scene: LANDMARK RESOURCE. A sturdy new wooden bridge built by Varnhold's settlers (still under construction if visited before the Stag Lord falls). Claiming it before Varnhold vanishes severs relations and raises Varnhold Negotiation DCs to 30; after the vanishing it Claims freely and grants +2 (and one degree better) on Establish Farmland here.
threads: [Settle and claim the Stolen Lands]   characters: [Varnhold settlers]   elements: [Kiravoy Bridge]   themes: [Social]   location: DS3
gate: none
fragments:
  - plot_point: "Claiming before Varnhold vanishes severs relations (+Negotiation DC 30) — a diplomatic landmine"   themes: [Social, Tension]   weight: 1

### cluster: ds4 — "DS4. Spider Fields"   (source: p.90 / L4328)   mode: sandbox
scene: STANDARD, Severe 7. Barren fields dotted with grassy hummocks — trapdoor lids hiding six trapdoor ogre spiders (Creature 5; HP 70, AC 23, Trapdoor Lunge reaction, ogre spider venom, greater cover in their pits). Treasure: each pit ~20 gp in coins/gems; one holds a half-eaten human with +1 striking handwraps of mighty blows and boots of elvenkind.
threads: []   characters: [trapdoor ogre spiders]   elements: [spider fields]   themes: [Tension, Action]   location: DS4
gate: none
fragments:
  - plot_point: "6 trapdoor ogre spiders (Creature 5) ambush from pits (Trapdoor Lunge); venom paralyzes at stage 4"   themes: [Action]   weight: 1
  - plot_point: "Treasure: +1 striking handwraps of mighty blows, boots of elvenkind, scattered gems"   themes: [Action]   weight: 1

### cluster: ds5 — "DS5. Varnhold"   (source: p.91 / L4356)   mode: sandbox
scene: LANDMARK RESOURCE. Maegar Varn's village (under construction before the Stag Lord falls; full detail in Ch.6). Resource: a Freehold town the PCs' kingdom can integrate at 3rd level — 4 Urban-Grid blocks, all 16 lots built (Brewery, 4 Houses, Inn, Shrine, Smithy, Stable, Tannery, Town Hall, and Trade Shops: gemcutter, potter, tailor, weaver). [HIDDEN] its people will vanish (Ch.6, the Varnhold Vanishing → Vordakai).
threads: [Settle and claim the Stolen Lands, The Varnhold mystery]   characters: [Maegar Varn]   elements: [Varnhold settlement]   themes: [Social, Mystery]   location: DS5
gate: none
fragments:
  - plot_point: "Varnhold is a 4-block Freehold town integratable at kingdom level 3 (16 built lots)"   themes: [Social]   weight: 1
  - plot_point: "[HIDDEN] foreshadows the Varnhold Vanishing (Ch.6) — Maegar Varn and the whole village will disappear"   themes: [Mystery, Tension]   weight: 1

### cluster: ds6 — "DS6. Blood Furrows"   (source: p.91 / L4362)   mode: sandbox
scene: STANDARD, Moderate 7. Furrowed, sinkhole-pocked grassland — the decades-old territory of Kankerata ("world chewer"), an elite bulette (Creature 9) the Nomen use as a rite-of-courage gauntlet. Observant and swift, it attacks anyone who loiters.
threads: [The Nomen Problem]   characters: [Kankerata the bulette, Nomen centaur clan]   elements: [Blood Furrows]   themes: [Action, Social]   location: DS6
gate: none
fragments:
  - plot_point: "Kankerata, an elite bulette (Creature 9), ambushes from underground; the Nomen race its drifts to prove courage"   themes: [Action, Social]   weight: 1

---

## Seed the Lists  (names only; [HIDDEN] for unearned spoilers)
Threads: The Nomen Problem · Find Vordakai's Tomb · The Ghost Stone War · Save the Bog Strider · Slay Hooktongue · Dragonfly Cloak · Wanted: Slug Spit · [HIDDEN] Sepoko & Ngara · Wanted: Speartooth · Find Armag's Tomb · Pitax Refugees · War of the River Kings · Ilora's Alliance · The Eater of Kings · Numerian Trade · The Mammoth's Shame · [HIDDEN] Nyrissa & the Thousandbreaths Portal · [HIDDEN] Ilthuliak · [HIDDEN] The Lantern King · Wild Hunt
Characters: Nomen centaur clan · Restov envoy / swordlords of Restov · [HIDDEN] Vordakai · Talon Peak Roc · Zzamas the ether spider · [HIDDEN] Culchek spriggans · Irahkatu the ahuizotl · Sepoko · [HIDDEN] Ngara the spirit naga · Tok-Tekt · Ka-Kekt · Hooktongue the water orm · Berzaki · Chesk Umberweed · Speartooth · Baron Hannis Drelev · Windchaser · Darg/Fesl/Urda · [HIDDEN] Armag · Pitaxian refugees · King Castruccio Irovetti · Pitax wardens · Ilora Nuski · Kob Moleg · Hill giant butchers · Minognos-Ushad · Hillstomper · [HIDDEN] cairn linnorms · Malchar Tevalkan · [HIDDEN] Nyrissa · [HIDDEN] Lantern King's vilderavn emissary · Trees that Weep · [HIDDEN] Ilthuliak · Amvarean · wild hunt
Adventure Features (locations/hazards): Nomen Campsite (NH1) · Linnorm's Grave (NH2) · Varnhold Pass (LV1) · Talon Peak (LV2) · Culchek Cave (LV3) · Ghost Stone (LV4) · Ironstone Gully (LV5) · Vordakai's Tomb (LV6) · Valley of the Dead (LV7) · Empty Dragon Lair (LV8) · Wyvernstone Bridge (HT1) · Cloudberry Field (HT2) · Boggard Ambush (HT3) · Sinking Bog (HT4) · Haunted Fen (HT5) · M'botuu (HT6) · Lake Hooktongue (HT7) · Dragonfly Glade (HT8) · Swamp Scar (HT9) · Chuul Lair (HT10) · Lily Patch / Azure Lilies (HT11) · Tok-Nikrat (HT12) · Bog of Bones (HT13) · Hydra Den (HT14) · Slug Bog (HT15) · Speartooth's Den (DR1) · Fort Drelev (DR2) · Wild Horses (DR3) · Desperate Refugees (DR4) · Flooded Mine (TL1) · Giant's Cave (TL2) · Armag's Tomb (TL3) · Explorer's Grave (TL4) · Aurumvorax Den (TL5) · Chimera Pride (TL6) · Hemlock Island (RU1) · Rushlight Festival Grounds (RU2) · Catspaw Camp (RU3) · Tusker's Stomping Ground (GL1) · Marshaling Ground (GL2) · Littletown (PX1) · Pitax (PX2) · Steamgrotto (GU1) · Whiterose (GU2) · Ilora's Camp (GU3) · Mammoth Graveyard (NU1) · Castle of Knives (TV1) · Weeping Grove (TV2) · Mount Branthlend (BR1) · Ilthuliak's Lair (BR2) · Hungerdark (BR3) · per-zone wandering tables (NH/LV/HT/DR/TL/RU/GL/PX/GU/NU/TV/BR — convert each to list_d100)

## Diminisher: ¼ for a solo PC — scale printed encounters down.
