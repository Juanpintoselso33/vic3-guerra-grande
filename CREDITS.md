# Credits

## Uruguayan party flags

Used as the end icons of the war bar (`gfx/interface/progressbar/twospains_*_marker.dds`).

- `twospains_radicalism_marker.dds` (Partido Colorado)
  - Source: [Flag of Colorado Party (Uruguay).svg](https://commons.wikimedia.org/wiki/File:Flag_of_Colorado_Party_(Uruguay).svg), Wikimedia Commons.
  - Author: vectorised by Froztbyte.
  - License: [CC BY-SA 3.0](https://creativecommons.org/licenses/by-sa/3.0/).
  - Changes: rasterised, resized to 120x80, framed on a 128x128 transparent canvas and converted to DDS. This texture is shared under the same license.
- `twospains_conservatism_marker.dds` (Partido Nacional)
  - Source: [Flag of the National Party (Uruguay).svg](https://commons.wikimedia.org/wiki/File:Flag_of_the_National_Party_(Uruguay).svg), Wikimedia Commons.
  - License: public domain.
  - Changes: rasterised, resized, framed and converted to DDS.

## «la Argentina» (Steam Workshop 2982907360)

The map and the South American history this mod ships are **la Argentina's**, by its authors, reworked
only where the five oriental states need it. Until 24/9/2026 they lived in the compatch «Guerra Grande x
la Argentina», now merged into this mod.

- `map_data/state_regions/07_south_america.txt`: la Argentina's states (plus the local "estados divididos"
  fix), their three oriental states replaced by this mod's five over the same 44 provinces.
- `common/history/states/00_states.txt`, `common/history/pops/07_south_america.txt`,
  `common/history/buildings/07_south_america.txt`: la Argentina's files without their three oriental states.
- `gfx/map/map_object_data/generated_map_object_locators_*.txt`: la Argentina's locators merged with this
  mod's for the five oriental states (`tools/merge_map_locators.py` in the design repo).
- `common/history/military_formations/02_military_formations_south_america.txt`: la Argentina's Chilean HQ
  lines (`sr:region_south_andes`).
- `REPLACE:PLT` / `REPLACE:Great_ARG`, `geographic_region_colonial_la_plata`, the Misiones and Entre Ríos
  alternatives of `je_expanding_paraguay`: la Argentina's definitions with the five oriental states.
- `common/character_templates/zz_gg_dna_argentina.txt`: five of la Argentina's Argentine templates, verbatim
  plus a portrait (`dna`) line.

## Community Mod Framework (Steam Workshop 3385002128)

`annex_country`, `conquer_state` and `return_state` (`common/war_goal_types/zz_guerra_grande_war_goals.txt`)
and `law_oligarchy` (`common/laws/zz_gg_rosas_no_vote.txt`) are CMF's versions, verbatim, with one guard
line each.
