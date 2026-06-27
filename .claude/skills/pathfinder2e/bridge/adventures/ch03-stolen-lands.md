# Ingested Adventure — Kingmaker Chapter 3: Stolen Lands   (hook: adventure-ingest)
fidelity: full   ·   source: Kingmaker AP 2e, Chapter 3, lines 7513–8382

The chapter has three parts, mapped to story milestones: defend Oleg's (→2), break the Thorn River
camp (→3), topple the Stag Lord (→4). Part 1 keys Oleg's buildings (A1–A11); Part 2 keys the bandit
camp (B1–B5); Part 3 keys the fort (C1–C11) with multiple approaches. Sandbox clusters handle the
ambush tactics, interrogations, and methods-of-approach; keyed-rooms clusters handle the three
location maps.

---

### cluster: oleg-post — "Oleg's Trading Post (the home base)"   (source: p.163 / L7537)   mode: keyed-rooms
scene: A repurposed border fort (area RL1) at the southern edge of Rostland/Brevoy, run by gruff Oleg Leveton and his warm wife Svetlana, who've been shaken down monthly by the Stag Lord's bandits for three months. A 10-ft palisade (Climb DC 20) with four ruined catapults and a 30-ft gate rings the post. The Levetons expect the PCs as chartered help and offer free room and board to fight off the bandits' next "tax" visit. This is the campaign's first home base — a hub for rumors, quests, and visiting NPCs (Kesten Garess, Jhod Kavken; Ch2 p52). Key items live in the stockroom; the hidden office key gates them.
threads: [stop-the-banditry, settle-the-stolen-lands, svetlanas-ring]   characters: [Oleg Leveton, Svetlana Leveton, Bokken (mentioned)]   elements: [palisade-climb-DC20, ruined-catapults, stockroom-loot, Stag-Lord-amulet-lore]   themes: [refuge, frontier, oppression]   location: A1–A11
gate: none
fragments:
  - plot_point: "A1 Market Yard — open trade area with fire pit and two tables; where the bandit confrontation plays out"   themes: [gathering]   weight: 1
  - plot_point: "A2 Guesthouse — rentable beds (5 cp/night w/ meals); a suggested ambush hide-spot; Oleg is repairing its roof leak on arrival"   themes: [refuge]   weight: 1
  - plot_point: "A3 Stable — holds Oleg's jittery horse Claptrap (riding horse, Creature 1); rentable stalls; alt ambush hide-spot, vulnerable to Happs's fire"   themes: [animals]   weight: 1
  - plot_point: "A4 Storage Pen — roofed pen, currently empty because Oleg keeps surrendering his stock to the bandits"   themes: [oppression]   weight: 1
  - plot_point: "A5 Middens — 3-ft composting pits dug into the soil"   themes: [squalor]   weight: 1
  - plot_point: "A6 Main Hall — the Levetons' home and storeroom; double doors to the yard can be barred, not locked"   themes: [home]   weight: 1
  - plot_point: "A7 Dining Room — small comfortable room, rarely used for meals due to size"   themes: [home]   weight: 1
  - plot_point: "A8 Office — Oleg's ledgers; DC 20 Perception finds an iron key behind a loose board that unlocks the stockroom (A9)"   themes: [secret]   weight: 1
  - plot_point: "A9 Stockroom — locked (DC 20 Thievery; key in A8); holds leather armor, heavy wooden shield, 2 hand axes, 5 javelins, longbow, 2 dozen arrows, scythe, 2 spears, 2 minor healing potions, lesser antidote, lesser antiplague, torches, rations, furs (3 gp), chest of 7 gp / 27 sp / 108 cp"   themes: [reward, supply]   weight: 1
  - plot_point: "A10 Storeroom — drinking water, lantern oil, lamps, candles, firewood, hooded lantern, cookware, 70 ft rope, a tent, ~2 weeks of food"   themes: [supply]   weight: 1
  - plot_point: "A11 Bedroom — the Levetons' modest sleeping quarters"   themes: [home]   weight: 1

### cluster: oleg-arrival — "Arrival at Oleg's & the bandit intel"   (source: p.165 / L7657)   mode: sandbox
scene: Svetlana greets the PCs warmly with stew, bread, and wine; Oleg stays gruff, unsettled that Restov wants to "explore the Greenbelt" and reabsorb his refuge into civilization, but he won't countermand his wife's offer of free board. The Levetons brief the PCs: the bandits first came three months ago threatening arson, return within an hour of sunrise on the first of each month, and seem based ~a day's ride south. Numbers have dwindled (12 → 7 → 5), and the dangerous hatchet-woman (Kressle) only came the first time; the crude hooded man (Happs) leads now. On that first visit, Kressle stole Svetlana's wedding ring and tossed it to a man as "payment." This seeds the Slay-the-Stag-Lord quest (80 XP; charter from Restov; proof = body or helm; reward 200 gp + a kingdom-founding charter).
threads: [stop-the-banditry, slay-the-stag-lord, svetlanas-ring]   characters: [Oleg Leveton, Svetlana Leveton, Happs Bydon (described), Kressle (described)]   elements: [stag-lord-quest-80xp, restov-charter, monthly-tax-pattern, wedding-ring-theft]   themes: [forewarning, frontier-politics, hospitality]   location: A1
gate: none
fragments:
  - plot_point: "Svetlana's welcome (stew/bread/wine) vs Oleg's gruffness — Oleg fears civilization swallowing his home but accepts the help"   themes: [hospitality, tension]   weight: 1
  - plot_point: "Bandit briefing: monthly visit, first-of-month near sunrise, camp ~a day's ride south; numbers shrinking each visit"   themes: [intel]   weight: 1
  - plot_point: "The hatchet-woman's first visit — black humor, nearly maimed Oleg's hand, stole Svetlana's wedding ring (seeds the ring quest)"   themes: [cruelty, loss]   weight: 1
  - plot_point: "The Stag Lord quest goes live — 80 XP; proof of death (body or helm) or a swordlord agent (Ivenzi) confirms; reward 200 gp + kingdom charter"   themes: [mandate, stakes]   weight: 1

### cluster: oleg-ambush — "Ambushing the bandits (Happs Bydon)"   (source: p.166 / L7679)   mode: sandbox
scene: MODERATE 1. The PCs have a day and night to fortify and plan; the Levetons suggest hiding in the guesthouse or stable and striking once the bandits start loading furs. Oleg will play it straight as the deal begins but Svetlana can't credibly hide (each hidden Leveton imposes a cumulative –1 to trick checks). About an hour after sunrise, Happs Bydon and three Thorn River bandits ride in from the south. If ambushed, the surprised bandits take a –2 to initiative and are flat-footed round 1, and PCs may roll any tactic-appropriate skill (Deception/Stealth/Survival) for initiative. Open confrontation forfeits surprise; waiting them out makes Happs return in two days with five bandits, more aggressive. Happs (Creature 0) prefers his bow, boasts, uses alchemist's fire on grouped PCs or the stable as a distraction, and fights to the death while a flunky watches him; lone or wounded, he flees or surrenders. Minion bandits (Creature –1) flank, blunder tactically, and flee at <6 HP toward the camp.
threads: [stop-the-banditry, slay-the-stag-lord]   characters: [Happs Bydon, Thorn River Bandits, Oleg Leveton, Svetlana Leveton]   elements: [moderate-1, surprise-round, flat-footed-r1, alchemists-fire, fire-on-stable, flee-at-<6hp]   themes: [ambush, defense, cowardice]   location: A1
gate: none
fragments:
  - plot_point: "Set the trap — a day/night to prepare; hide in guesthouse (A2) or stable (A3); each Leveton who hides costs –1 cumulative to trick checks"   themes: [tactics]   weight: 1
  - plot_point: "The bandits arrive — Happs Bydon + 3 Thorn River bandits ride in from the south an hour past sunrise to load the 'tax'"   themes: [confrontation]   weight: 1
  - plot_point: "Ambush bonus — surprised bandits take –2 initiative and are flat-footed round 1; PCs roll any tactic-fitting skill for initiative"   themes: [advantage]   weight: 1
  - plot_point: "Fight Happs Bydon (Creature 0) — bow-fighter, boasts, alchemist's fire on groups or the stable; fights to death while watched, else flees/surrenders"   themes: [boss, bravado]   weight: 1
  - plot_point: "Thorn River Bandits (Creature –1) — flank and blunder; shriek and flee toward the camp at <6 HP; on horseback if able"   themes: [minions, cowardice]   weight: 1
  - plot_point: "Blowing the ambush — open confrontation forfeits surprise; waiting them out makes Happs return in 2 days with 5 bandits, more hostile, eroding the Levetons' trust"   themes: [consequence]   weight: 1

### cluster: oleg-aftermath — "Captives, settling in & the home base"   (source: p.167 / L7717)   mode: sandbox
scene: Captured bandits warn that Kressle will come for the Levetons and will take revenge if she hears any escaped; Coerced, they reveal the camp's location (or guide there) and can answer most Stag Lord questions (see Interrogations), while warning the PCs are no match for him. Each bandit wears a silver Stag Lord amulet (worth 3 gp; a fanged-skull helm with antlers) — DC 17 Banditry Lore or DC 20 Society to Recall Knowledge surfaces rumors of the Stag Lord recruiting smaller gangs under his banner. Settling in: Oleg rewards the group with 12 gp and all the stockroom potions/elixirs, free guesthouse lodging and meals, and lets them keep the bandits' gear (buying leftovers at full price this once, regular prices after). The post becomes the PCs' home base for rumors, quests, and visiting NPCs.
threads: [stop-the-banditry, slay-the-stag-lord, settle-the-stolen-lands]   characters: [Oleg Leveton, Svetlana Leveton, captured bandits, Kressle (threatened), Kesten Garess (mentioned), Jhod Kavken (mentioned)]   elements: [stag-lord-amulet-3gp, banditry-lore-DC17, society-DC20, coerce-for-camp, reward-12gp+potions, free-board]   themes: [interrogation, reward, home-base]   location: A1, A9
gate: none
fragments:
  - plot_point: "Captives talk — warn that Kressle will retaliate; Coerced, reveal/lead to the Thorn River camp and answer Stag Lord questions, but warn the PCs are outmatched"   themes: [intel, threat]   weight: 1
  - plot_point: "Stag Lord amulets — silver antlered fanged-skull tokens (3 gp); DC 17 Banditry Lore / DC 20 Society reveals the Stag Lord is uniting bandit gangs under his banner"   themes: [lore, foreshadow]   weight: 1
  - plot_point: "Oleg's reward — 12 gp + all stockroom potions/elixirs, free lodging and meals, and the bandits' gear (full price once, then market)"   themes: [reward, gratitude]   weight: 1
  - plot_point: "Oleg's becomes home base — a hub to introduce rumors, wanted posters, quests, and key NPCs (Kesten Garess, Jhod Kavken) as the AP unfolds"   themes: [home-base, sandbox-hub]   weight: 1

---

### cluster: thorn-river-find — "Finding the Thorn River camp"   (source: p.169 / L7767)   mode: sandbox
scene: The Stag Lord's second camp sits at area GB7 on the Thorn River, controlling the Greenbelt's northernmost ford and serving as a gathering point for his wandering bandits — and it's where Oleg's tormentors hail from. Left alone over a month, the bandits double their numbers and resources, then launch a torch-the-post raid in revenge for the PCs' defiance, so dealing with them should be a priority. The PCs reach the camp via a captured/interrogated bandit's guidance, or by a DC 15 Survival check to Track a fled bandit south to the creekside campsite (a path skirts the Thorn's north bank, the camp ~60 ft from the bank with a 200-ft approach path).
threads: [stop-the-banditry, slay-the-stag-lord]   characters: [Thorn River Bandits]   elements: [GB7-northern-ford, survival-DC15-track, time-pressure-doubling, retaliation-raid]   themes: [pursuit, escalation, urgency]   location: GB7 (approach)
gate: none
fragments:
  - plot_point: "Strategic stakes — the camp guards the northernmost Greenbelt ford and gathers wandering bandits; left a month, they double and raid Oleg's to burn it down"   themes: [stakes, ticking-clock]   weight: 1
  - plot_point: "Tracking in — follow a captive's lead or make a DC 15 Survival check to Track a fled bandit south along the Thorn's north bank to the creekside camp"   themes: [tracking]   weight: 1

### cluster: thorn-river-camp — "The Thorn River Bandit Camp"   (source: p.170 / L7779)   mode: keyed-rooms
scene: A fairly large creekside camp defended by hidden tree platforms, ~60 ft from the Thorn's north bank along a winding creek path. The layout (B1–B5) supports ranged defense from watch posts and trap setups for the unwary. Watch platforms grant a +1 Stealth circumstance bonus to those hiding on them; each post keeps a lesser thunderstone to raise the alarm. Loot is stashed under a tarp at B2. If the bandits expect the PCs, they add a hidden bandit at the logs (B4) and bait a spike snare on the wagon (B5).
threads: [stop-the-banditry, slay-the-stag-lord, svetlanas-ring]   characters: [Thorn River Bandits, Kressle]   elements: [tree-platforms, lesser-thunderstone-alarm, spike-snare-trap, loot-stash, ford-control]   themes: [encampment, defenses, traps]   location: B1–B5
gate: none
fragments:
  - plot_point: "B1 Clearing — cut campsite with log seats around a stone-lined campfire; bandits sleep under the stars, with 6 folded tents stored under the B2 platform"   themes: [camp]   weight: 1
  - plot_point: "B2 East Watch Post — 20-ft tree platform overlooking camp and the west trail; rope ladder (or DC 10 Athletics to climb a nearby tree); +1 Stealth on platform; lesser thunderstone in a tree hollow; the loot stash is beneath its tarp"   themes: [overwatch, loot]   weight: 1
  - plot_point: "B3 West Watch Post — identical to B2 but holds only a lesser thunderstone alarm, no supplies"   themes: [overwatch]   weight: 1
  - plot_point: "B4 The Logs — two thick logs beside the trail; usable as cover or rolled across the path (DC 20 Athletics, 3-action Interact); a hidden bandit posts here if the PCs are expected"   themes: [cover, ambush]   weight: 1
  - plot_point: "B5 The Wagon — old broken wagon with the components for a spike snare (Core Rulebook 591) handy; loot is baited atop a built snare if the PCs are expected"   themes: [trap, bait]   weight: 1

### cluster: thorn-river-fight — "Kressle and the Thorn River bandits"   (source: p.171 / L7809)   mode: sandbox
scene: SEVERE 2. Kressle (Creature 1, unique) leads; a career River Kingdoms bandit recruited after she maimed two of the Stag Lord's men, now running this camp. She and Happs lived here with nine other bandits; with Happs's three dead/away, Kressle holds six. Preparedness scales the encounter: a day's warning = all six present and ready; no warning = only four on site (others off hunting/patrolling); taking >3 days = the bandits learn Happs's fate and all stay. One bandit each holds B2 and B3 to thunderstone-alarm and rain arrows while the rest grab weapons; if expecting the PCs they add a logs ambusher (B4) and the wagon snare (B5). Kressle dual-wields hatchets (Hatchet Flurry; Maiming Chop can inflict clumsy on a crit). Loot stash at B2 includes coin, jewelry, a music box, fur crates, and 8 bottles of herbal liquor specifically destined for the Stag Lord — a key lever for infiltrating the fort. Svetlana's ring is NOT here; mitflits stole it to the Old Sycamore (GB14).
threads: [stop-the-banditry, slay-the-stag-lord, svetlanas-ring]   characters: [Kressle, Thorn River Bandits]   elements: [severe-2, hatchet-flurry, maiming-chop-clumsy, preparedness-scaling, herbal-liquor-8-bottles, ring-not-here]   themes: [boss, banditry, leverage]   location: B1–B5
gate: none
fragments:
  - plot_point: "Fight Kressle (Creature 1, unique) — dual hatchets, Hatchet Flurry, Maiming Chop inflicts clumsy on a crit; while she lives the bandits stay loyal"   themes: [boss]   weight: 1
  - plot_point: "Garrison scaling — a day's warning = 6 bandits ready; surprise = only 4 on site; >3 days = all present, having learned Happs's fate"   themes: [readiness]   weight: 1
  - plot_point: "Defensive playbook — B2/B3 sentries thunderstone-alarm and snipe; prepared bandits add a B4 logs ambusher and bait the B5 spike snare"   themes: [defenses]   weight: 1
  - plot_point: "The liquor stash — 8 bottles of herbal liquor at B2 are the Stag Lord's; withholding them makes him aggressive, but they're the ticket to infiltrate his fort"   themes: [leverage, foreshadow]   weight: 1
  - plot_point: "The ring isn't here — Svetlana's wedding ring was stolen by mitflits and spirited to the Old Sycamore (GB14)"   themes: [redirect, quest-thread]   weight: 1

### cluster: thorn-river-interrogations — "Interrogating the captives"   (source: p.171 / L7871)   mode: sandbox
scene: Once Kressle falls, surviving bandits lose their loyalty and surrender — they fear the Stag Lord (whose grip on reality is slipping into a whiskey cask) but won't die for him, and after learning they're outclassed will give up crucial intel. Their answers reveal the Stag Lord's stat-line as a story hook: a brutal bowman who never removes his stag helm; a master-phrase password to enter the fort on the NE shore of the Tuskwater; his drunkenness and instability; the strange old man locked in the fort's basement (rumored to be the real power); and that Svetlana's ring went to the gremlins under the old sycamore to the east. Asked to help fight the Stag Lord, they blanch and refuse.
threads: [slay-the-stag-lord, svetlanas-ring, who-is-behind-the-bandits]   characters: [captured bandits, the Stag Lord (described), Nugrah (rumored)]   elements: [master-phrase-clue, saint-gilmorg-password, stag-helm-face, basement-old-man, ring->old-sycamore]   themes: [interrogation, foreshadow, mystery]   location: B1
gate: none
fragments:
  - plot_point: "Who's your boss? — 'the Stag Lord,' a deadeye bowman who crushed a hand to mush in one fist and is never seen without his creepy stag helm"   themes: [intel, dread]   weight: 1
  - plot_point: "How to get in? — bandits use a master phrase as a password at the fort on the NE shore of the Tuskwater"   themes: [infiltration-clue]   weight: 1
  - plot_point: "The password — 'By the bloody bones of Saint Gilmorg, who wants to know?' (unless recently changed)"   themes: [password]   weight: 1
  - plot_point: "The booze & the Stag Lord — a bitter drunk, 'half of what he used to be,' never right in the head, but still dangerous"   themes: [weakness, foreshadow]   weight: 1
  - plot_point: "The strange old man — a terrifying old man locked in the basement, suspected of secretly running the show via the Stag Lord"   themes: [mystery, hidden-power]   weight: 1
  - plot_point: "Svetlana's ring — stolen by gremlins under the old sycamore to the east; was in the bag of loot taken from the trader woman"   themes: [quest-thread]   weight: 1
  - plot_point: "Will you help fight the Stag Lord? — they blanch and refuse out of fear"   themes: [fear]   weight: 1

---

### cluster: stag-fort-overview — "Against the Stag Lord — the fort & its garrison"   (source: p.173 / L7897)   mode: sandbox
scene: The Stag Lord's fort (area TW3, on the largest lake in the Greenbelt) is the chapter's climax and the symbol of the PCs' growing dominion. Of all his bandits, only ten live in the fort: three lieutenants and seven rank-and-file (each a named individual usable for infiltration roleplay). If the PCs thin the ranks, the Stag Lord replenishes 1d6 ordinary bandits per day but can't replace his officers. The seven rank-and-file (Creature 0, identical stats) include Ayles Megesen (torturer), Cragger Kench, Backhanded Jeb Megesen, Falgrim Sneeg (target of Kesten Garess's revenge, Finding Falgrim quest), Norry "Gorgon" Driper, Jex the Snitch (the Stag Lord's informant favorite), and Topper Red (failed Pitax poet). FIGHTING BANDITS guidance: all 10 at once exceeds Extreme 3, so rally them in waves and avoid all three lieutenants at once; time the Stag Lord's entrance for drama.
threads: [slay-the-stag-lord, who-is-behind-the-bandits, finding-falgrim]   characters: [the Stag Lord, Akiros Ismort, Dovan from Nisroch, Auchs, Ayles Megesen, Cragger Kench, Backhanded Jeb, Falgrim Sneeg, Norry Driper, Jex the Snitch, Topper Red, Kesten Garess (quest)]   elements: [TW3-fort, 3-lieutenants+7-bandits, 1d6-replenish, waves-not-swarm, extreme-3-cap]   themes: [climax, garrison, set-piece]   location: TW3 (fort overview)
gate: thorn-river-camp resolved (location & password typically learned there); PCs ~3rd level
fragments:
  - plot_point: "The fort at TW3 — on the largest lake in the Greenbelt; a landmark hard to miss; learn its location by interrogation or exploration"   themes: [destination]   weight: 1
  - plot_point: "Garrison — 3 lieutenants + 7 rank-and-file live in the fort; ordinary bandits replenish 1d6/day, officers cannot be replaced"   themes: [forces]   weight: 1
  - plot_point: "The seven named bandits — Ayles (torturer), Cragger, Backhanded Jeb, Falgrim Sneeg (Kesten's revenge target), Norry Driper, Jex the Snitch, Topper Red — flavor for infiltration"   themes: [characters, infiltration]   weight: 1
  - plot_point: "Pacing rule — all 10 bandits at once exceeds Extreme 3; rally in waves, avoid all three lieutenants together, time the Stag Lord's entrance for drama"   themes: [pacing, gm-guidance]   weight: 1

### cluster: stag-lieutenants — "The three lieutenants"   (source: p.174 / L7933)   mode: sandbox
scene: Three lieutenants serve the Stag Lord, their interplay a lever for the PCs. Akiros Ismort — a fallen paladin of Erastil from Taldor who murdered a lover and her husband in a rage, now second-in-command and bitterly disillusioned; once the fort battle begins he can tear off his amulet and fight alongside the PCs (GM-timed, for drama or rescue), and only Akiros stays to offer continued aid after the Stag Lord dies. Auchs — a simpleminded lummox, cruel and toy-obsessed, traveling with Dovan but warming to Akiros. Dovan from Nisroch — a sadistic Ustalavic torturer (claims Nisroch) who secretly feeds the Stag Lord's alcoholism to gain power and is plotting to murder Akiros; he flees with the rest after the boss dies but may return for revenge (prefers elf victims). Bandit cant: the master phrase ('By the bloody bones of Saint Gilmorg, who wants to know?') opens the gate; the infiltrated phrase ('And so the stink marks the jackal in a den of wolves') flags a suspected spy/traitor.
threads: [slay-the-stag-lord, recruit-or-turn-the-lieutenants, who-is-behind-the-bandits]   characters: [Akiros Ismort, Auchs, Dovan from Nisroch]   elements: [akiros-defection, dovan-plots-akiros, master-phrase, infiltrated-phrase, dovan-returns-later]   themes: [intrigue, redemption, treachery]   location: TW3 (social)
gate: none
fragments:
  - plot_point: "Akiros Ismort — fallen Erastil paladin, second-in-command, disillusioned; can defect mid-battle (tear off amulet, fight for the PCs) and is the only one who stays to aid afterward"   themes: [redemption, ally]   weight: 1
  - plot_point: "Auchs — simpleminded brutal lummox, devoted to Dovan but warming to Akiros; a candidate to be 'saved' and recruited"   themes: [pawn]   weight: 1
  - plot_point: "Dovan from Nisroch — sadistic Ustalavic torturer feeding the Stag Lord's drinking for power, plotting to kill Akiros; flees the boss's death but may return for revenge (prefers elves)"   themes: [treachery, recurring-villain]   weight: 1
  - plot_point: "Bandit cant — master phrase opens the gate ('Saint Gilmorg...'); infiltrated phrase ('the stink marks the jackal...') flags a suspected spy"   themes: [passwords, infiltration]   weight: 1

### cluster: stag-approach — "Methods of approach (infiltration vs assault)"   (source: p.175 / L7961)   mode: sandbox
scene: How the PCs take the fort is open, but two paths dominate. Infiltration: with the master phrase and bandit disguises/stolen goods, PCs gain +2 to Disguise/Lie; displaying the Thorn River alcohol shifts those checks up one degree of success. An alcohol delivery brings the Stag Lord joyfully out of C8 to seize the liquor (and tip 5 gp each via Akiros); he drinks himself unconscious in an hour, opening a window to steal in and ambush him, or to poison the liquor — but a failed kill wakes him to a full-camp alarm. Crafty PCs can lure off, kill, recruit, or sow dissent among individual bandits (Diplomacy/Deception/Intimidation to turn them on each other). Assault: the fort is heavily defended; a combo of infiltration to get in and assault once positioned often works best. Once fighting starts, bandits shout the alarm but the Stag Lord — sick and dizzy from his binge — can be delayed for a dramatic entrance; his death breaks the bandits, who flee (only Akiros stays).
threads: [slay-the-stag-lord, recruit-or-turn-the-lieutenants]   characters: [the Stag Lord, Akiros Ismort, Dovan, Auchs]   elements: [+2-disguise-lie, liquor-shifts-degree, poison-the-liquor, sow-dissent, delay-stag-lord-entrance]   themes: [infiltration, assault, stratagem]   location: TW3 (tactics)
gate: master phrase learned (for infiltration path)
fragments:
  - plot_point: "Infiltration — master phrase + bandit disguise/loot grant +2 Disguise/Lie; flashing the Thorn River alcohol shifts those checks up one degree"   themes: [disguise]   weight: 1
  - plot_point: "The liquor gambit — a delivery lures the Stag Lord out of C8 to seize it and pass out in an hour (steal in to ambush, or poison the liquor); a failed kill wakes him to a full alarm"   themes: [trap, risk]   weight: 1
  - plot_point: "Sow dissent — lure off, kill, recruit, or turn individual bandits against each other with Diplomacy/Deception/Intimidation, exploiting their personalities"   themes: [subterfuge, social]   weight: 1
  - plot_point: "Assault — heavily defended; best paired with infiltration to get inside; alarm is shouted but the binge-sick Stag Lord can be delayed for a dramatic entrance"   themes: [assault, pacing]   weight: 1

### cluster: stag-haunted-hillside — "The Haunted Hillside & Palisade (approach hazards)"   (source: p.176 / L7977)   mode: sandbox
scene: SEVERE 3. The main path up to the fort (30 ft wide, 300 ft long, no cover) is safe, but the surrounding hillsides hide a cursed graveyard: the ruins were once a monastery to Gyronna, and her curse raised the dead against the lapsed monks. Approaching by any non-path landward route within 30–150 ft of the fort rouses zombie shamblers (Creature –1) — four erupt on first contact (prone, leaving difficult-terrain divots), with a DC 10 flat check each round summoning 1 more (2 on a crit) until all 12 emerge; fighting them draws the bandits' attention. The 15-ft spiked palisade (Climb DC 20; DC 15 Reflex over the top or take 1d6 piercing, crit-fail falls for +7 bludgeoning) has a 30-ft no-zombie zone around it. SE of the fort, a sunken stone trapdoor (DC 20 Perception to notice) can be dug up (Dig Up the Trapdoor exploration activity, DC 18 Athletics, Stealth checks to stay unheard — DC 25 day / DC 15 night) for a 10-ft shaft into the cellar (C11b), bypassing the gate.
threads: [slay-the-stag-lord]   characters: [zombie shamblers, Gyronna (lore)]   elements: [severe-3, 12-zombies, DC10-flat-summon, palisade-climb-DC20, reflex-DC15-spikes, trapdoor-to-C11b, dig-up-trapdoor]   themes: [undead, curse, stealth-route]   location: fort exterior (hillside, palisade, SE trapdoor)
gate: none
fragments:
  - plot_point: "The Haunted Hillside (SEVERE 3) — straying off the main path within 30–150 ft of the fort raises zombie shamblers; 4 erupt at once, then DC 10 flat each round adds 1 (2 on crit) up to 12; the fight alerts the bandits"   themes: [undead-trap, alarm]   weight: 1
  - plot_point: "Gyronna's curse (lore) — the ruins were a lapsed monastery to Gyronna; she raised its graveyard dead to drag the monks under (DC 15 Religion later IDs the C5 graffiti)"   themes: [backstory, curse]   weight: 1
  - plot_point: "The palisade — 15-ft spiked logs; Climb DC 20, DC 15 Reflex over the top (1d6 piercing; crit-fail falls for +7 bludgeoning); a 30-ft no-zombie band rings it"   themes: [obstacle]   weight: 1
  - plot_point: "The SE trapdoor — sunken stone trapdoor (DC 20 Perception); Dig Up the Trapdoor (DC 18 Athletics + Stealth checks, DC 25 day/DC 15 night) opens a 10-ft shaft into the cellar (C11b), bypassing the gate"   themes: [secret-entrance, stealth]   weight: 1

### cluster: stag-fort-rooms — "The Stag Lord's Fort (keyed map C1–C11)"   (source: p.177 / L8003)   mode: keyed-rooms
scene: A reclaimed Gyronnan monastery: a spiked palisade rings a central stone structure with three watchtowers, two creaky 20-ft walkways, an owlbear pen, a barracks, an armory, and a hidden cellar. Each room is its own combat node — the boss room is C8 (the Stag Lord, Creature 6), with the cellar (C11) hiding Nugrah (Creature 5) and the bulk of the loot. Run rooms in sequence; Scene-Test at meaningful thresholds (the yard/gate, the central room brawl, the boss barracks, the cellar). Beaky the owlbear (Creature 4) in C6 is a wildcard the bandits can unleash — it turns on the Stag Lord if confronted.
threads: [slay-the-stag-lord, who-is-behind-the-bandits, svetlanas-ring (loot)]   characters: [the Stag Lord, Akiros Ismort, Dovan from Nisroch, Auchs, Beaky the owlbear, Nugrah, Stag Lord bandits]   elements: [keyed-fort, beaky-wildcard, gyronna-graffiti, hidden-cellar, boss-C8]   themes: [dungeon, set-piece, climax]   location: C1–C11
gate: inside the fort (via approach cluster)
fragments:
  - plot_point: "C1 The Yard (TRIVIAL 3) — dusty inner yard with water barrels (fire-fighting); 2 skittish riding horses (Creature 1) under the NE watchtower (DC 15 Nature to calm both); speak-with-animals reveals bandit habits and the horse-eating 'monster' in a cave"   themes: [entry, animals]   weight: 1
  - plot_point: "C2 Walkways — two 20-ft wooden walkways (C2a north to armory/NE tower, C2b to SW/NW towers); steep stairs are difficult terrain; creaky boards give –2 Stealth"   themes: [traversal]   weight: 1
  - plot_point: "C3 Watchtowers (TRIVIAL 3) — three 20-ft towers with railing cover; one Stag Lord bandit (Creature 0) each: Ayles at C3a, Falgrim at C3b, Jex at C3c; if one dies the other two flee to C5 to warn the rest"   themes: [overwatch, alarm]   weight: 1
  - plot_point: "C4 Central Tower (TRIVIAL 3) — flat stone roof platform; Auchs (Creature 2, unique) sleeps here amid his prized toy knights and dragons — touching/harming the toys triggers instant rage; fights to death while Dovan is visible, else surrenders at <5 HP and can be recruited"   themes: [mini-boss, pathos]   weight: 1
  - plot_point: "C5 Central Room (MODERATE 3) — drafty bandit common room with Gyronna graffiti (DC 15 Religion); Dovan (Creature 2, unique) + 4 bandits (Creature 0); a rope opens the C6 owlbear gate; Dovan baits and releases Beaky, flees to C9→C2a, fights to death only if cornered (flees at <7 HP)"   themes: [brawl, treachery]   weight: 1
  - plot_point: "C6 Owlbear Pen (LOW 3) — foul cave-cage holding Beaky (owlbear, Creature 4); opening the gate makes noise that rouses the Stag Lord (1d4+4 rounds); Beaky attacks the nearest target and betrays the Stag Lord if confronted"   themes: [wildcard, monster]   weight: 1
  - plot_point: "C7 Storage Room (TRIVIAL 3) — supplies and the second-in-command's quarters; Akiros Ismort (Creature 3, unique) broods here, sharpening gear and writing his memoirs; rages round 1, targets healers→casters→others, fights to death (Shameful Memories triggers near an open Erastil symbol)"   themes: [lieutenant, redemption]   weight: 1
  - plot_point: "C8 The Stag Lord's Barracks (SEVERE 3) — hide-lined room reeking of liquor; the acid-scarred Stag Lord (Creature 6, p.604) drinks and broods, favors his bow, hunts humans (his father's face), drinks a healing potion below 20 HP, fights to the end; chest hides gems/jewelry (~21 gp + carnelian, red garnet 30 gp, charm bracelet 20 gp, etc.) and three leather masks"   themes: [boss, treasure]   weight: 1
  - plot_point: "C9 Armory — mostly collapsed roof; unlocked chests hold 10 longbows, 260 arrows, 5 short swords, 5 spears, rope, tools, 4 leather armors; creaky stairs to C2a give –2 Stealth"   themes: [supply, loot]   weight: 1
  - plot_point: "C10 Pig-Roast Room — drunken feast room; DC 15 Perception spots a wood slab hiding the stairway down to the cellar (C11); bandits avoid going down because of the 'freak' (Nugrah)"   themes: [secret-passage]   weight: 1
  - plot_point: "C11 Cellar (MODERATE 3) — damp moldy storeroom of stolen goods across three vaults; Nugrah (Creature 5, unique druid of Gozreh) — the Stag Lord's imprisoned, abusive father — melds into stone, buffs, summons a giant ant, casts from the ceiling, fights to the death but won't leave the cellar; ~45 gp trade goods + chests (2 pp/21 gp/42 sp/800 cp; 30 gp jewelry)"   themes: [hidden-truth, boss, treasure]   weight: 1

### cluster: stag-conclusion — "Concluding the chapter"   (source: p.183 / L8359)   mode: sandbox
scene: With the Stag Lord ousted, the bandits — bound by greed and fear — quickly rout, though the lieutenants may linger to torment the PCs or join them. The PCs have fulfilled a major part of their charter; Lady Jamandi is pleased when word reaches her. Much of the northern Greenbelt remains unexplored, but a new and bigger charter awaits: the swordlords expect the PCs to claim the lands they've explored in Brevoy's name — the road to founding a kingdom (Chapter 4).
threads: [slay-the-stag-lord, settle-the-stolen-lands, found-your-kingdom]   characters: [the Stag Lord (defeated), Akiros Ismort, Dovan, Lady Jamandi Aldori]   elements: [bandits-rout, charter-fulfilled, kingdom-charter-next, jamandi-pleased]   themes: [resolution, transition, ascension]   location: TW3 (aftermath)
gate: Stag Lord defeated
fragments:
  - plot_point: "The bandits rout — held by greed and fear, they scatter once the Stag Lord falls; lieutenants may linger to torment the PCs or join them"   themes: [aftermath]   weight: 1
  - plot_point: "Charter fulfilled — a major part of the Restov charter is done; Lady Jamandi is pleased when word reaches her"   themes: [reward, recognition]   weight: 1
  - plot_point: "The road to rulership — the swordlords' new charter asks the PCs to claim the explored lands in Brevoy's name, opening kingdom-founding (Chapter 4)"   themes: [transition, ambition]   weight: 1

---

## Seed the Lists  (names only; [HIDDEN] for unearned spoilers)
Threads: Stop the banditry plaguing the Greenbelt · Slay the Stag Lord (80 XP quest) · Recover Svetlana's wedding ring (→ Old Sycamore / GB14) · Settle & claim the Stolen Lands · Who is really behind the bandits? [HIDDEN: Nugrah pulling strings] · Finding Falgrim (Kesten Garess's revenge) · Recruit or turn the Stag Lord's lieutenants · Found and grow your kingdom (opens Ch 4)
Characters: Oleg Leveton · Svetlana Leveton · Happs Bydon · Kressle · the Stag Lord · Akiros Ismort · Dovan from Nisroch · Auchs · Beaky (owlbear) · Ayles Megesen · Cragger Kench · Backhanded Jeb Megesen · Falgrim Sneeg · Norry "Gorgon" Driper · Jex the Snitch · Topper Red · Kesten Garess (mentioned) · Jhod Kavken (mentioned) · Lady Jamandi Aldori · Nugrah [HIDDEN until the cellar]
Adventure Features (locations/hazards): Oleg's Trading Post (A1–A11, RL1) · the Thorn River Bandit Camp (B1–B5, GB7) · the northernmost Greenbelt ford · the Stag Lord's Fort (C1–C11, TW3) · the Haunted Hillside (Gyronna's cursed graveyard / zombie shamblers) · the spiked palisade · the SE buried trapdoor (→ cellar) · the owlbear pen · the hidden cellar · Stag Lord amulets · the herbal-liquor lever · the Old Sycamore (GB14, ring's destination)
## Diminisher: ¼ for a solo PC — scale printed encounters down.
