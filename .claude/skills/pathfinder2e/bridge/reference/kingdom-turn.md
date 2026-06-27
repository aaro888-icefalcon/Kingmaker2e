# Kingdom Turn — procedure (Kingmaker Appendix 2)   (world-tick subsystem)

The kingdom-building minigame, run as a **structured procedure**: every internal check is a PF2e
**Kingdom skill** check vs the **Control DC** read on the four-degree ladder (`system-profile.md`).
This is the runnable outline + key tables; the page-cited specifics live in the atomized
`adventures/ch04-rivers-run-red.md` (kingdom rules introduced) and the AP's **Appendix 2**. Roll
events with `dice.py table .../generators/kingdom_event.json`.

A **Kingdom Turn** covers ~1 month and is triggered by the world-tick subsystem (one month elapses
or the player declares a turn). The kingdom first comes into being after the Stag Lord falls
(Chapter 4).

## Kingdom anatomy
- **Four kingdom ability scores:** **Culture, Economy, Loyalty, Stability** (start 10, modified by
  Charter, Heartland, Government at founding; raised by Kingdom level/boosts).
- **16 Kingdom skills** (each ability governs four):
  - **Culture:** Arts, Folklore, Magic, Scholarship
  - **Economy:** Boating, Exploration, Industry, Trade
  - **Loyalty:** Intrigue, Politics, Statecraft, Warfare
  - **Stability:** Agriculture, Defense, Engineering, Wilderness
  Each has a proficiency (Trained→Legendary) like a PC skill; the bonus = ability mod + proficiency
  (+ kingdom level when trained) ± status/circumstance/item (from structures, leaders, feats).
- **Control DC** — set by kingdom level (the level-based DC table, +size adjustments). The standard
  DC for kingdom activities.
- **Leadership roles (8):** **Ruler, Counselor, Emissary, General, Magister, Treasurer, Viceroy,
  Warden.** Each assigned to a PC (or trusted NPC); each grants its leader's role bonus to certain
  kingdom skills and an invested benefit. A **vacant** role penalizes related activities and may
  raise Unrest. (In solo play one PC may hold several roles; spread them to recruited NPCs as the
  realm grows — the engine's Characters List tracks them.)
- **Resource Points (RP):** the abstract monthly budget; collected in Upkeep (Resource Dice by
  level + claimed hexes/worksites), spent on activities/structures. Unspent RP largely lapse.
- **Commodities:** Food, Lumber, Stone, Ore, Luxuries — stored and consumed (esp. Food →
  Consumption).
- **Unrest** — discontent; high Unrest penalizes all kingdom checks and at thresholds forces Ruin
  gains; at the cap the kingdom falls into **anarchy**. **Ruin (four tracks): Corruption, Crime,
  Decay, Strife** — each with a threshold; crossing it increases the Ruin and degrades the linked
  ability. Crit-failures, unpaid Consumption, and bad events feed Unrest/Ruin.

## The turn, in order
1. **Upkeep Phase**
   - Assign/confirm **Leadership** roles (note vacancies).
   - Adjust scores for ongoing effects; recalculate **Control DC**.
   - **Collect Resources:** roll Resource Dice (by level) + bonuses; gain RP and claimed-hex
     commodities/worksites (resource hexes found in Hexploration pay off here).
   - **Pay Consumption** (Food/RP for settlements + armies). **Shortfall → +Unrest.**
   - Apply standing **Unrest/Ruin** effects.
2. **Commerce Phase** — collect taxes/tribute, resolve **trade agreements** and Sell/Establish
   Trade-Route activities; convert commodities ↔ RP as the rules allow.
3. **Activity Phase** — the kingdom takes a set number of **activities** (scales with level), split
   among **Leadership** activities (e.g. *Capital Investment, Pledge of Fealty, Quell Unrest,
   Hire Adventurers, Pursue Project, New Leadership, Send Diplomatic Envoy, Establish Work Site*),
   **Region** activities (*Claim Hex, Build Roads, Clear Hex/Build Structure, Establish Settlement,
   Fortify Hex, Establish Farmland*), and **Civic** activities within settlements (*Build Structure*).
   Each is a Kingdom-skill check vs Control DC; read the degree (crit success = bonus outcome,
   crit fail = setback/Ruin).
4. **Event Phase** — make the **Kingdom Event** check (a flat check whose chance rises each turn
   without an event). On a hit, roll `generators/kingdom_event.json` and resolve it (many events
   are skill-check challenges or ongoing situations); on a miss, no event this turn. **Story events**
   from the chapters (e.g. Chapter 4's Grigori, the troll sightings) are scripted events that fire
   regardless and seed Threads.

## Settlements (brief)
A settlement is a grid of **blocks** filled with **structures** (each grants kingdom bonuses, item
access, or activity unlocks). Villages → Towns → Cities → Metropolises by occupied blocks. Build
with Civic activities; structures cost RP/commodities and time. Track each settlement's level,
structures, and any special edicts in `campaign-state.md`.

## Solo-play guidance
- Run kingdom turns between expeditions; one turn ≈ one bookkeeping cycle that may itself produce
  scenes (an event becomes a Turning Point; an Unrest spike a Random Event). Tie outcomes back to
  the JSON Lists: a new project → a Thread; a problem NPC → a Character; a threatened settlement →
  an Adventure Feature.
- Keep it as light or crunchy as the player wants — at minimum: collect RP, pay Consumption, take a
  couple of activities, roll the event. The Chaos Factor and faction clocks supply the pressure.
