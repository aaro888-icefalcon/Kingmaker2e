# Seed Sources — The Stolen Lands (Kingmaker)   (hook: seeds)
- deck size: 35            # 30–40; refresh each bookkeeping
- refresh: each bookkeeping (main AI inline; may offload to the mythic-scout agent)
- sources:
  - **setting-canon entries near the PC** — the current zone's people, places, and tensions
    (`setting-canon.md` + the relevant `adventures/chNN-*.md` clusters/fragments for hexes within
    ~1–2 of the party).
  - **un-used authored fragments** for nearby/relevant clusters (the usage ledger in `hexmap.json`
    leans the deck toward content not yet surfaced — organic coverage, no re-draws).
  - **live world state** — open Threads (`threads.json`), active Characters (`characters.json`),
    revealed-but-unexplored hexes, faction-clock positions (Pitax aggression, Nyrissa's influence,
    troll uprising), Kingdom status (Unrest/Ruin, current projects, pending kingdom events),
    any active Warfare.
  - **random rolls for novelty** on: `generators/hex_feature.json`, `generators/rumor.json`,
    `generators/npc_role.json`, and (when governing) `generators/kingdom_event.json` — rolled with
    `dice.py table <abs path>`.
- consumed when a seed is invoked by a scene / Turning Point / Random Event; replace consumed
  seeds at the next refresh.

# Bias: prefer authored, nearby, un-used content (content bias MEDIUM) — pull a printed fragment
# when reasonably relevant, else a random roll. Keep the deck weighted to where the PC actually is
# and what the open Threads point at, so surfaced content stays contextual and never railroaded.
