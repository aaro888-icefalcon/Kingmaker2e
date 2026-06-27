# Warfare — procedure (Kingmaker Appendix 3)   (world-tick subsystem)

Mass combat between **armies** treated as single creature-like units, run as a structured
procedure; every roll is a PF2e check/attack read on the four-degree ladder. This is the runnable
outline; recruitable armies + their stat lines are in `generators/army.json`, and the page-cited
specifics in the AP's **Appendix 3**. Warfare matters most in **Chapter 7** (Fort Drelev / the
Tatzlford assault) and **Chapter 8** (War of the River Kings).

## Armies as units
An **army** has a stat block resembling a creature of its **level**:
- **AC**, and two saves — **Maneuver** (like Reflex/Fort: formation, terrain) and **Morale**
  (like Will: nerve, rout).
- **HP** with a **Rout Threshold**; when HP drops to the threshold the army must check Morale or
  break.
- **Attacks:** a **melee** and/or **ranged** strike (`1d20 + army attack` vs enemy army AC);
  a hit deals a **condition/HP** result rather than rolling lots of dice.
- **Tactics** (learned maneuvers, e.g. coordinated assault, hold-the-line) and **special
  abilities**; **gear** from Outfit.
- **Consumption:** armies eat **Food** each Kingdom Turn; unpaid → **+Unrest**.
- **Army conditions:** **efficient, weary, shaken, mired, lost, defeated, damaged** — accrued from
  hits and recovered via the Recover activity.

## Army types & recruiting
- Basic types: **Infantry** (~Lvl 1), **Cavalry** (~Lvl 3), **Skirmishers** (~Lvl 5), **Siege**
  (~Lvl 7). **Specialized armies** (Sootscale Warriors, Lizardfolk Defenders, Nomen Scouts, M'Botuu
  Frog Riders, Greengripe Bombardiers, Tok-Nikrat Scouts, Tiger Lord Berserkers, …) unlock after the
  PCs **encounter and win over that faction in hexploration** — then **Recruit Army** (a Warfare/
  Statecraft Kingdom check vs a Recruitment DC by army level).
- Track each fielded army in `generators/army.json` usage + `campaign-state.md` Clocks; add a war
  as a **Thread** and the enemy commander as a **Character**.

## Army activities (Kingdom-Turn / war integration)
The **General** (and warfare-capable leaders) direct armies: **Deploy** (move; terrain/road
modifiers), **Garrison** (fortify in a settlement/refuge), **Recruit**, **Train** (learn a Tactic;
Scholarship/Warfare), **Outfit** (gear; Trade), **Recover** (remove conditions), **Offensive
Gambit** (start a war encounter with an initiative edge via Intrigue/Warfare).

## War encounters (the battle)
Resolve as rounds, like a duel between units:
1. **Initiative** — Warfare/Intrigue or the army's bonus; Offensive Gambit can grant the edge.
2. **Each round** armies act: a **Strike** (`1d20 + attack` vs target army AC). **Crit/normal hit →
   bigger/standard effect** (HP loss + a condition like weary/shaken/mired); **miss/crit miss →
   none or a self-setback**. Tactics and terrain modify.
3. **Morale/Rout** — at the Rout Threshold (or on a fear effect) check **Morale** or the army flees;
   a routed army is **defeated** (removed from the battle), not necessarily destroyed.
4. **Victory** — when one side routs/destroys the other. Model an extended campaign as **Victory
   Points** accrued across several encounters/turns toward the war's objective.
5. **Aftermath** — apply conditions/HP to surviving armies (Recover later), update Unrest/RP, and
   feed the result back to Threads/Clocks (a won war may conclude a Thread; a lost one spikes
   Chaos and Unrest).

## Solo-play guidance
Keep battles abstract and quick: a few army Strikes and a Morale check often settle it. The PC may
personally join a war encounter as a **special unit/commander** (a PF2e character acting within the
mass-combat frame) — their heroics grant circumstance bonuses to their army's checks. Honor the
dice: armies can be lost, commanders can fall, and a war can go badly — those are real stakes.
