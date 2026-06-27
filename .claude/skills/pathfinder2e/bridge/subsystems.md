# World Subsystems — Kingmaker (Stolen Lands)   (hook: world-tick; fired by tick.py at bookkeeping)
#
# tick.py reads the table below: `every scene` fires every bookkeeping; `every N scenes` fires when
# scene # % N == 0; `on trigger: …` is surfaced for the GM to judge. Each row's "advance by" points
# at the procedure (reference/*.md) and the table to roll (generators/*.json via `dice.py table`).
# Individual checks inside these subsystems are PF2e checks vs a DC, read on the four-degree ladder
# (see system-profile.md) — the engine still rolls and shows every die.

| subsystem | cadence | advance by |
|---|---|---|
| Hexploration | on trigger: overland travel / a Hexploration activity is taken | Run reference/hexploration.md: spend the day's Hexploration Activities, reveal the hex (keyed → its `location:<hexcode>` cluster becomes the Expected Scene; unkeyed → roll generators/hex_feature.json and/or the current zone's encounter table). Record the hex + any site in hexmap.json (usage ledger). Resource/Landmark/Secret hexes feed the Kingdom subsystem. |
| Kingdom Turn | on trigger: one in-world month elapses / the players declare a Kingdom Turn | Run reference/kingdom-turn.md in order — Upkeep (pay Consumption, adjust Unrest, collect resources/RP), Commerce, Activity (leadership + civic activities, each a Kingdom-skill PF2e check vs DC), Event (roll generators/kingdom_event.json; on a hit resolve it; otherwise note "no event"). Apply Ruin (Corruption/Crime/Strife/Decay) on crit-fails and unpaid Consumption. Update campaign-state Clocks + threads.json. |
| Warfare | on trigger: an army is fielded or a war encounter begins | Run reference/warfare.md: resolve army activities (Deploy/Garrison/Recruit/Train/Outfit/Recover) and Victory-Point war encounters using army stat blocks (generators/army.json). Armies consume Food each Kingdom Turn; unpaid consumption raises Unrest. Record outcomes to threads.json + Clocks. |
| Pitax pressure clock | every 6 scenes | Advance King Irovetti's offscreen scheming +1. Early: bandit funding / propaganda (Grigori). Mid: spies, sabotage, tournament bait. At full (or Ch 8 trigger): the War of the River Kings opens. Roll a Fate Question or generators/kingdom_event.json for the specific move; record to Clocks + Threads. |
| Nyrissa's influence clock | every 10 scenes | Tighten the Lantern King's curse offscreen +1. Surface as small fey wrongness near the kingdom (a bloom-flower image, a fey bargain, a vanishing). Stays mostly hidden until late chapters; at full in the endgame it becomes the Bloom (Chapter 10). Do NOT reveal cause — Player ≠ PC knowledge. |
| Offscreen threats (regional) | every 4 scenes | Advance the nearest un-cleared authored threat toward the kingdom (troll uprising / owlbear / cult of the Bloom / a monster lair the PC bypassed). A far hex you never cleared becomes a Random-Event raid on a settlement. Pick the most contextually-relevant Adventure Feature; roll its consequence honestly. |
| Camp & weather | on trigger: a night/rest in the wilderness | Roll for a night encounter (zone table, odds by zone danger + CF) and weather/conditions if relevant; apply rest, healing (Treat Wounds / daily preparations), and any random encounter. Default when nothing else is due: simply advance offscreen clocks. |

# Default (RAW) when nothing companion-specific is due: advance offscreen clocks (the engine's
# baseline). The faction clocks above are the Kingmaker-specific offscreen pressure that keeps the
# sandbox alive between the PC's expeditions and turns.
