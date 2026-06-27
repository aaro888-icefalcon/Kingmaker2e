# Theme Weights — Kingmaker (Stolen Lands)   (hook: themes; FIXED for the whole campaign)
# Every adventure within the campaign rolls its 5 Theme priorities from these weights (the engine's
# adventure_crafter.py reads the resulting order; these weights bias the roll). Kingmaker is an
# exploration-and-realm saga with a creeping mythic threat, so Action and Personal lead, Tension
# runs constant (Nyrissa's curse), Social rises as the kingdom and its rivals grow, Mystery seeds
# the hidden spine.
Action: 3       # hexcrawl, monster lairs, bandits, war — the campaign's default motion
Tension: 3      # the frontier's danger + the slow tightening of the Lantern King's curse
Personal: 2     # the PCs' kingdom, their subjects, companions, rivals made personal
Social: 2       # patrons (Restov), rivals (Pitax), factions, kingdom governance, diplomacy
Mystery: 1      # the vanishings, the fey, "who is really behind all this?"

# Optional fixed First-Priority theme. Left as 'none' so each adventure's lead theme is rolled
# from the weights above (a hexcrawl expedition may lead Action; a kingdom-politics arc, Social;
# the Varnhold Vanishing or Candlemere, Mystery). For a darker, more curse-forward campaign set
# first_priority: Tension.
first_priority: none
