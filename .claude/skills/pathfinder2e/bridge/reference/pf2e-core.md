# PF2e Core — GM quick-reference (resolve hook detail)

Companion to `system-profile.md`. Everything here resolves through the engine's honest dice
(`dice.py roll 1d20+<mod>`); the GM sets the **DC** and the **stakes** first, then reads the
**degree of success**. This is a play aid, not the rulebook — when a precise rule matters and is
in doubt, verify with the player; if still unresolved, a rule-mode Fate Question decides and is
recorded.

## Degrees of success (the four-rung ladder)
- **Crit Success:** ≥ DC + 10.   **Success:** ≥ DC.   **Failure:** < DC.   **Crit Failure:** ≤ DC − 10.
- **Natural 20** = one step better than rolled; **Natural 1** = one step worse (applied after
  comparing total to DC). So a nat 20 that only meets the DC becomes a Crit Success; a nat 1 on a
  clear success becomes a plain Success; etc.

## Setting the DC
**Level-based DCs** (use the creature/hazard/task level):

| Lvl | DC | Lvl | DC | Lvl | DC | Lvl | DC |
|--|--|--|--|--|--|--|--|
| 0 | 14 | 6 | 22 | 12 | 30 | 18 | 38 |
| 1 | 15 | 7 | 23 | 13 | 31 | 19 | 39 |
| 2 | 16 | 8 | 24 | 14 | 32 | 20 | 40 |
| 3 | 18 | 9 | 26 | 15 | 34 | 21 | 42 |
| 4 | 19 | 10 | 27 | 16 | 35 | 22 | 44 |
| 5 | 20 | 11 | 28 | 17 | 36 | 23 | 46 |

**Simple DCs** (no obvious level — by the required proficiency): Untrained **10**, Trained **15**,
Expert **20**, Master **30**, Legendary **40**.

**Adjust** for difficulty: incredibly easy −10, very easy −5, easy −2, **hard +2**, very hard +5,
incredibly hard +10. Rarity bumps (uncommon +2, rare +5) for tasks against obscure knowledge.

## Modifier math (what goes on the d20)
`1d20 + ability mod + proficiency`, where **proficiency = (Untrained 0 / Trained 2 / Expert 4 /
Master 6 / Legendary 8) + character level** (the level is added only when at least Trained), plus
**bonuses/penalties** of three types that **don't stack within a type** (keep the highest):
**circumstance**, **status**, **item**. Cover, aid, flanking (off-guard), frightened, etc. feed
these.

## Conditions you'll touch most (mechanical, not flavor)
- **Off-guard** (flat-footed): −2 AC. **Frightened N:** −N to all checks/DCs (ticks down 1/round).
- **Clumsy N** (−N Dex-based), **Enfeebled N** (−N Str-based), **Stupefied N** (−N spell stuff &
  casting DC), **Drained N** (−N Con, lose HP), **Sickened N** (−N + can't ingest).
- **Slowed N / Quickened:** −N / +1 actions next turn. **Stunned N:** lose N actions.
- **Dying N / Wounded N:** at 0 HP → Dying 1 (Dying 2 if downed by a crit, +Wounded). Recovery flat
  check **DC 10 + Dying** each turn: success −1 Dying, crit success −2, failure +1, crit fail +2.
  **Dying 4 = dead.** Healing to ≥1 HP ends Dying but leaves Wounded (raises future Dying).
- **Persistent damage:** roll the listed dice at end of turn; flat DC 15 to end (or assisted).

## Common skill actions (DC notes)
- **Recall Knowledge** (Arcana/Nature/Religion/Society/Lore by topic): vs the subject's level DC;
  crit gives extra/precise info, crit fail gives a false detail.
- **Sense Motive** (Perception) vs **Deception/Will**. **Seek** (Perception) to find hidden.
- **Demoralize** (Intimidation) vs Will → frightened. **Make an Impression** (Diplomacy) vs Will
  shifts attitude; **Request** then asks a favor. **Coerce** (Intimidation).
- **Athletics:** Trip/Shove/Grapple/Disarm vs Fortitude or Reflex DC; **Climb/Swim/Jump** vs DC.
- **Stealth:** **Hide/Sneak** vs Perception DC. **Thievery:** Pick a Lock / Disable a Device vs DC.
- **Medicine:** **Treat Wounds** (DC 15 trained, higher tiers heal more; crit fail deals damage),
  10-min activity; **Battle Medicine** in combat.
- **Survival:** **Track**, **Subsist**; **Nature/Survival** drive hexploration activities.
- **Crafting:** Repair, Craft, Earn Income (downtime).

## Building/statting a creature on the fly (benchmarks by level)
When a foe is unstatted, set the expected power via the engine's NPC-Statistics oracle, then
express it in PF2e terms for the creature's **level** (moderate baselines):

| Lvl | AC | HP (mod) | High atk | Best save | Low save | Save DC / Spell DC | Striking dmg |
|--|--|--|--|--|--|--|--|
| 0 | 15 | 17 | +8 | +8 | +2 | 16 | 1d6+1 |
| 1 | 16 | 24 | +9 | +9 | +4 | 17 | 1d8+3 |
| 3 | 18 | 45 | +12 | +12 | +6 | 20 | 2d6+5 |
| 5 | 21 | 75 | +15 | +14 | +9 | 22 | 2d8+7 |
| 7 | 24 | 110 | +18 | +17 | +11 | 25 | 2d10+9 |
| 10 | 28 | 165 | +22 | +21 | +14 | 30 | 3d10+11 |
| 13 | 32 | 220 | +26 | +24 | +17 | 33 | 3d12+13 |
| 16 | 36 | 270 | +30 | +28 | +20 | 36 | 4d12+15 |
| 20 | 42 | 350 | +36 | +33 | +25 | 42 | 6d12+17 |
Adjust ±2 (AC/atk/DC) and ±25%/±50% HP for elite/weak, and apply the solo **Diminisher** for a
single PC. (Full Building Creatures benchmarks scale every level; interpolate between rows.)

## PF2e's smaller subsystems (used in Kingmaker)
- **Influence** (social, e.g. winning over Maegar Varn, festival NPCs): an NPC has a **Discovery
  DC** (learn their wants/biases) and **Influence DCs** per skill; accrue **Influence Points** over
  rounds/scenes to cross **thresholds** that improve attitude or grant aid. Resistances/weaknesses
  modify the DC. Run as repeated skill checks vs the NPC's DCs; the engine's Fate Questions cover
  off-table reactions.
- **Research** (libraries/archives, e.g. the Spiral Seal at Candlemere): accrue **Research Points**
  via Library checks against a threshold to unlock facts; crit fail can introduce a setback.
- **Victory Points (generic):** any extended contest (chase, infiltration, a war encounter,
  a kingdom project) can be modeled as accruing VP toward a goal with success/failure ticks.
- **Chase:** sequential obstacle checks; success advances, failure costs ground/actions.
- **Infiltration:** accrue progress vs an **Awareness Points** clock the opposition tracks.
These all decompose into PF2e checks (this file) + the engine's Chaos/Fate/Random-Event machinery.
