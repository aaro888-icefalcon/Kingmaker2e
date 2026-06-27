# System Profile — Pathfinder Second Edition   (hook: resolve)

The engine owns scenes, pacing, and oracle questions; **PF2e owns task resolution and combat.**
When the System Profile has a mechanic → roll it with honest dice (`dice.py roll …`) and read the
**degree of success**. When it is silent → ask a Fate Question. Deep rules quick-reference lives
in `reference/pf2e-core.md`; PC build in `reference/pf2e-character-creation.md`.

- **Dice convention:** `1d20 + modifier` vs a **DC** (Difficulty Class). Damage/effects use
  the listed dice (e.g. `1d8+4`, `2d6`).
- **Express a roll as:** `dice.py roll 1d20+<mod>` (add `adv`/`dis` for fortune/misfortune —
  rolls twice, keeps higher/lower). Damage: `dice.py roll 2d6+3`. **Always state the DC and the
  stakes BEFORE rolling** (pre-commit), then read the degree from the result.
- **Core resolution — FOUR DEGREES OF SUCCESS:**
  - **Critical Success** — total ≥ DC + 10, **or** a natural 20 that is already a success (a
    nat 20 also bumps the result one step up).
  - **Success** — total ≥ DC.
  - **Failure** — total < DC.
  - **Critical Failure** — total ≤ DC − 10, **or** a natural 1 (a nat 1 bumps the result one
    step down).
  - Nat 20 / nat 1 shift the degree by **one step** after comparing to DC (so a nat 20 that
    misses by <10 is a Success; a nat 1 that beats the DC is still a Success-downgraded-to-Failure
    only if it would have been a Success — i.e. one step down).
- **Degrees of success?: YES.** This drives the Fate-Question Exceptional mapping in rule-mode:
  Exceptional Yes ≈ Critical Success, Yes ≈ Success, No ≈ Failure, Exceptional No ≈ Critical
  Failure (`dice.py fate <odds> <cf> --mode rule`, used only when no PF2e mechanic applies).
- **Stats / skills (the skill system):** six abilities (Str, Dex, Con, Int, Wis, Cha). Skills:
  Acrobatics, Arcana, Athletics, Crafting, Deception, Diplomacy, Intimidation, Medicine, Nature,
  Occultism, Performance, Religion, Society, Stealth, Survival, Thievery, plus **Lore**
  specialties (Kingmaker-relevant: Brevoy, Pitax, Warfare, Politics, First World, Hunting, Forest,
  Mercantile, etc.). Proficiency tiers add to the d20: **Untrained +0, Trained +2, Expert +4,
  Master +6, Legendary +8**, each **+ the character's level** when at least Trained. Modifier =
  ability mod + proficiency (+ level if trained) + item/circumstance/status bonuses − penalties.
  Skill **actions** (Recall Knowledge, Sense Motive, Demoralize, Make an Impression, Trip,
  Grapple, Sneak, Track, Treat Wounds, …) are detailed in `reference/pf2e-core.md`.
- **Defenses / health:** **AC** = 10 + Dex (cap by armor) + proficiency (+level) + item. Three
  **saves** — Fortitude, Reflex, Will. **HP** = ancestry + (class HP + Con) per level. Conditions
  are mechanical (frightened, off-guard/flat-footed, clumsy, enfeebled, drained, etc. — see
  reference).
- **Combat:** **three-action economy** per turn (Strike, Stride, Step, Cast a Spell [usually 2
  actions], Raise a Shield, Interact, etc.) + 1 reaction. **Initiative** = usually a Perception
  check (or a skill the GM calls for). **Attack:** `1d20 + attack mod` vs target AC; the
  **Multiple Attack Penalty** is −5 on the 2nd attack, −10 on the 3rd (−4/−8 with agile).
  **Damage** on a hit; **double dice** on a crit. **Defeat/death:** at 0 HP a creature is **dying**
  (Dying 1, or Dying 2 if hit by a crit); each turn a **recovery check** (flat DC 10 + dying
  value); Dying 4 = **dead**. Gaining the **wounded** condition raises future dying. These are
  **real stakes** — death, maiming, and capture are honest outcomes; Peril Points stay OFF unless
  the player opts into a scarce announced pool (engine discipline).
- **NPC stat units (on-the-fly statting):** when an unstatted foe appears, set the expected value
  → Fate Question → read `mythic/npc_statistics` (Yes = as expected; ExcYes +25%; No −25%;
  ExcNo −50%), expressed in PF2e terms for the creature's **level**: AC, HP, save mods, Perception,
  the best attack bonus + its damage dice, and key DCs. Use the **Building Creatures** benchmarks
  by level in `reference/pf2e-core.md`. Apply the solo **Diminisher** (default ¼ — see
  `adventures/kingmaker-overview.md`) when scaling printed encounters for one PC.
- **Routing default:** PF2e resolves **combat, skill checks, saves, attacks, and the three
  subsystems' individual checks** (`dice.py roll`, degree read here). Defer to **Fate Questions**
  for world/uncertainty questions the rules don't cover ("is the bridge guarded?", "does Oleg
  trust us yet?"). `system.py route` prints this rule.
- **Subsystems as structured procedures (not Fate Questions):** Kingmaker's **Kingdom Turn**,
  **Hexploration**, and **Warfare** each run as their own procedure — see `subsystems.md` (the
  world-tick registry) and `reference/{kingdom-turn,hexploration,warfare}.md`. Their internal
  checks (Kingdom skills, hexploration activities, army maneuvers) are still **PF2e checks vs a
  DC read on the four-degree ladder** — resolved here, not invented. PF2e's smaller subsystems
  (Influence, Research, Chase, Infiltration, Victory Points) are summarized in `reference/pf2e-core.md`.

**Precedence:** this System Profile > the user's recollection of a rule > training knowledge.
When all are silent, a Fate Question decides and the answer is recorded to state/canon.
