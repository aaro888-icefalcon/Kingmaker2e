# Generator Index — Kingmaker (Stolen Lands)   (hooks: generate:*)
# need | when it's called | table(s) | mode (replace | conjunction | default)
# Anything not listed -> Mythic/AC default. Tables are list_d100 JSON in this folder, rolled with:
#   python3 .claude/skills/mythic-gm/scripts/dice.py table <abs path to the json>
# Only `character` auto-fires (wired in bridge.md generators_map); the rest are rolled on demand by
# the subsystems / reference docs / seed refresh.

| need | when called | table(s) | mode |
|---|---|---|---|
| new NPC (any) | any NEW CHARACTER result (character-list NEW, Event Focus "New NPC", an AC Plot Point that calls for a Character) | AC Character Crafter + `npc_role.json` | conjunction |
| hex contents | reconnoitering an UNKEYED hex (reference/hexploration.md) | `hex_feature.json` (+ the zone's encounter table) | replace |
| kingdom event | Event Phase of a Kingdom Turn, on an event hit (reference/kingdom-turn.md) | `kingdom_event.json` | replace |
| rumor / lead | seed-deck refresh; asking around at a settlement/tavern | `rumor.json` | replace |
| army available / encountered | Recruit Army, or a war force appears (reference/warfare.md) | `army.json` | replace |
| location / generic inspiration | a scene needs a place with no authored site & no specific need | Mythic Elements (engine default) | default |

# Notes
# - `npc_role.json` LAYERS on the AC Character Crafter (conjunction): roll both, then flesh the NPC
#   from setting-canon factions + the current zone; stat via the NPC Statistics oracle (PF2e units).
# - Native d20 source tables (the zone encounter tables in the AP) are encoded here as list_d100 with
#   5-wide bands (1-5, 6-10, ...) — identical distribution, and valid for `bridge.py validate` /
#   `dice.py table` (which support list_d100 and list_d10 only).
# - Per-zone random-encounter tables from the AP are atomized alongside their zone in
#   `adventures/ch02-into-the-wild-*.md`; convert any you want to roll directly into a list_d100 here
#   using the same banding.
