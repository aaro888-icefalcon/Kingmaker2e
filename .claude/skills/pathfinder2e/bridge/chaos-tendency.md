# Chaos Tendency — The Stolen Lands (Kingmaker)   (hook: chaos)
# The Chaos Factor step is ALWAYS ±1 per scene (RAW). A setting tunes the LEAN (how readily a
# scene counts as "in control" vs "chaotic") and the FLAVOR (Fate Chart dampening) — not the step.
- start: 5
- control_lean: harsh        # The frontier does not grant control cheaply. Early survival play:
                             # bandits, predators, weather, and the wilderness keep the PC reacting.
                             # Lower CF only when the PC DECISIVELY ends a scene on their own terms.
- floor: |
    Per-region minimums (the wilds and the war stay tense):
      - Deep/late zones (level 11+ hexes: Hooktongue, Tors of Levenies, Thousand Voices, Branthlend) >= 4
      - Active war (Chapter 8 War of the River Kings; any ongoing Warfare subsystem conflict) >= 5
      - The Bloom (Chapter 10, Nyrissa's invasion of the kingdom) >= 6
    A settled, well-governed home region in peacetime may fall as low as 2-3.
- flavor: standard           # Full chaos influence on the Fate Chart. Kingmaker swings hard between
                             # quiet governance and sudden violence — keep the oracle's teeth.

# Notes for the GM:
# - The two registers move CF differently. A clean kingdom turn or a hex handled flawlessly earns
#   -1. A botched check, an Interrupt, a Random Event, a lost army, an Unrest spike, or any scene
#   that ends NOT on the PC's terms is +1. When unsure -> +1 (a CF that only falls is drift).
# - As the kingdom stabilizes mid-campaign, CF naturally drifts down in the home region; the
#   region floors above keep the frontier and the endgame dangerous regardless.
