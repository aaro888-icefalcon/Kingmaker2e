# Bridge manifest — Pathfinder 2e: Kingmaker (Stolen Lands)

This companion supplies **Pathfinder Second Edition** as the resolution system (the `resolve`
hook: d20 vs DC, four degrees of success, the full skills system, three-action combat, dying)
and the **Kingmaker Adventure Path** as content (the Stolen Lands setting, three signature
subsystems — Kingdom-building, Hexploration, Warfare — wired into `world-tick`, plus the whole
AP atomized into clusters + fragments for `adventure-ingest`). Generators add Stolen Lands NPC
roles, kingdom events, hex features, rumors, and recruitable armies. Everything else falls back
to the Mythic/Adventure-Crafter engine defaults; all randomness still runs through the engine's
honest, shown, cited scripts.

```json
{
  "companion": "Pathfinder 2e — Kingmaker",
  "engine": "mythic-gm>=2",
  "overrides": ["resolve","meaning","chaos","themes","world-tick","seeds",
                "generate:character","generate:element","adventure-ingest"],
  "files": {
    "system_profile": "system-profile.md",
    "interpretation": "interpretation.md",
    "chaos": "chaos-tendency.md",
    "themes": "theme-weights.md",
    "generators": "generators/registry.md",
    "subsystems": "subsystems.md",
    "seeds": "seeds.md",
    "canon": "setting-canon.md",
    "ref_pf2e_core": "reference/pf2e-core.md",
    "ref_character_creation": "reference/pf2e-character-creation.md",
    "ref_kingdom_turn": "reference/kingdom-turn.md",
    "ref_hexploration": "reference/hexploration.md",
    "ref_warfare": "reference/warfare.md",
    "adventures_index": "adventures/kingmaker-overview.md"
  },
  "generators_map": {
    "character": {
      "mode": "conjunction",
      "table": "generators/npc_role.json",
      "note": "Layer the rolled Stolen Lands role onto the AC Character Crafter, then flesh the NPC from setting-canon factions (Restov/Brevoy, Pitax, Tiger Lords, Nomen centaurs, fey/First World, bandits) and the current scene/zone. Stat on the fly via the engine NPC Statistics oracle, expressed in PF2e units (AC/HP/attack/DC by level, scaled by the solo Diminisher)."
    }
  }
}
```

`overrides` lists the hooks this bridge fills; everything else uses the engine default. `files`
are checked for existence by `bridge.py validate`. `generators_map.character` is the one
auto-fire hook today: every NEW-CHARACTER result (a `character-list` NEW, an Event Focus of
*New NPC*, or an Adventure-Crafter Plot Point that calls for a Character) rolls `npc_role.json`
**and** the AC Character Crafter (mode `conjunction`); pass `--bridge .claude/skills/pathfinder2e/bridge`
to the roller scripts so the override is seen (the loop does this automatically). Other
generators (`kingdom_event`, `hex_feature`, `rumor`, `army`) are rolled on demand with
`dice.py table <abs path>` as the subsystems and `reference/` docs direct.
