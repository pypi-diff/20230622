# Comparing `tmp/dnd5epy-1.0.2.tar.gz` & `tmp/dnd5epy-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dnd5epy-1.0.2.tar", max compression
+gzip compressed data, was "dnd5epy-1.0.3.tar", max compression
```

## Comparing `dnd5epy-1.0.2.tar` & `dnd5epy-1.0.3.tar`

### file list

```diff
@@ -1,146 +1,146 @@
--rwxr-xr-x   0        0        0    26846 2023-06-22 14:49:33.138072 dnd5epy-1.0.2/README.md
--rwxr-xr-x   0        0        0    20295 2023-06-22 14:49:33.158072 dnd5epy-1.0.2/dnd5epy/__init__.py
--rwxr-xr-x   0        0        0      965 2023-06-22 14:49:33.162072 dnd5epy-1.0.2/dnd5epy/api/__init__.py
--rwxr-xr-x   0        0        0    57612 2023-06-22 15:21:18.080377 dnd5epy-1.0.2/dnd5epy/api/character_data_api.py
--rwxr-xr-x   0        0        0    29929 2023-06-22 14:49:32.914071 dnd5epy-1.0.2/dnd5epy/api/class_api.py
--rwxr-xr-x   0        0        0    37751 2023-06-22 14:49:32.934071 dnd5epy-1.0.2/dnd5epy/api/class_levels_api.py
--rwxr-xr-x   0        0        0    35153 2023-06-22 14:49:32.946071 dnd5epy-1.0.2/dnd5epy/api/class_resource_lists_api.py
--rwxr-xr-x   0        0        0    22854 2023-06-22 14:49:32.962071 dnd5epy-1.0.2/dnd5epy/api/common_api.py
--rwxr-xr-x   0        0        0    37171 2023-06-22 14:49:32.974071 dnd5epy-1.0.2/dnd5epy/api/equipment_api.py
--rwxr-xr-x   0        0        0    16996 2023-06-22 14:49:32.986071 dnd5epy-1.0.2/dnd5epy/api/feats_api.py
--rwxr-xr-x   0        0        0    17817 2023-06-22 14:49:33.002071 dnd5epy-1.0.2/dnd5epy/api/features_api.py
--rwxr-xr-x   0        0        0    30716 2023-06-22 14:49:33.022071 dnd5epy-1.0.2/dnd5epy/api/game_mechanics_api.py
--rwxr-xr-x   0        0        0    23276 2023-06-22 14:49:33.042072 dnd5epy-1.0.2/dnd5epy/api/monsters_api.py
--rwxr-xr-x   0        0        0    35140 2023-06-22 14:49:33.062072 dnd5epy-1.0.2/dnd5epy/api/races_api.py
--rwxr-xr-x   0        0        0    23641 2023-06-22 14:49:33.074072 dnd5epy-1.0.2/dnd5epy/api/rules_api.py
--rwxr-xr-x   0        0        0    23977 2023-06-22 14:49:33.086072 dnd5epy-1.0.2/dnd5epy/api/spells_api.py
--rwxr-xr-x   0        0        0    42903 2023-06-22 14:49:33.102072 dnd5epy-1.0.2/dnd5epy/api/subclasses_api.py
--rwxr-xr-x   0        0        0    29225 2023-06-22 14:49:33.118072 dnd5epy-1.0.2/dnd5epy/api/subraces_api.py
--rwxr-xr-x   0        0        0    16775 2023-06-22 14:49:33.126072 dnd5epy-1.0.2/dnd5epy/api/traits_api.py
--rwxr-xr-x   0        0        0    39842 2023-06-22 14:49:33.174072 dnd5epy-1.0.2/dnd5epy/api_client.py
--rwxr-xr-x   0        0        0      844 2023-06-22 14:49:33.174072 dnd5epy-1.0.2/dnd5epy/api_response.py
--rwxr-xr-x   0        0        0    24352 2023-06-22 14:49:33.154072 dnd5epy-1.0.2/dnd5epy/configuration.py
--rwxr-xr-x   0        0        0    15141 2023-06-22 14:49:33.166072 dnd5epy-1.0.2/dnd5epy/exceptions.py
--rwxr-xr-x   0        0        0    18834 2023-06-22 14:49:33.162072 dnd5epy-1.0.2/dnd5epy/models/__init__.py
--rwxr-xr-x   0        0        0    12234 2023-06-22 14:49:31.414062 dnd5epy-1.0.2/dnd5epy/models/ability_bonus.py
--rwxr-xr-x   0        0        0    12955 2023-06-22 14:49:31.438063 dnd5epy-1.0.2/dnd5epy/models/ability_score.py
--rwxr-xr-x   0        0        0    12324 2023-06-22 14:49:31.454063 dnd5epy-1.0.2/dnd5epy/models/alignment.py
--rwxr-xr-x   0        0        0    12024 2023-06-22 14:49:31.378062 dnd5epy-1.0.2/dnd5epy/models/api_reference.py
--rwxr-xr-x   0        0        0    12400 2023-06-22 14:49:31.398062 dnd5epy-1.0.2/dnd5epy/models/api_reference_list.py
--rwxr-xr-x   0        0        0    12171 2023-06-22 14:49:31.466063 dnd5epy-1.0.2/dnd5epy/models/area_of_effect.py
--rwxr-xr-x   0        0        0    13936 2023-06-22 14:49:31.478063 dnd5epy-1.0.2/dnd5epy/models/armor.py
--rwxr-xr-x   0        0        0    15994 2023-06-22 14:49:31.490063 dnd5epy-1.0.2/dnd5epy/models/background.py
--rwxr-xr-x   0        0        0    11904 2023-06-22 14:49:31.506063 dnd5epy-1.0.2/dnd5epy/models/background_all_of_feature.py
--rwxr-xr-x   0        0        0    12383 2023-06-22 14:49:31.514063 dnd5epy-1.0.2/dnd5epy/models/choice.py
--rwxr-xr-x   0        0        0    12264 2023-06-22 14:49:31.526063 dnd5epy-1.0.2/dnd5epy/models/class_all_of_starting_equipment.py
--rwxr-xr-x   0        0        0    14189 2023-06-22 14:49:31.538063 dnd5epy-1.0.2/dnd5epy/models/class_level.py
--rwxr-xr-x   0        0        0    23842 2023-06-22 14:49:31.550063 dnd5epy-1.0.2/dnd5epy/models/class_level_class_specific.py
--rwxr-xr-x   0        0        0    12196 2023-06-22 14:49:31.562063 dnd5epy-1.0.2/dnd5epy/models/class_level_class_specific_any_of.py
--rwxr-xr-x   0        0        0    12590 2023-06-22 14:49:31.570063 dnd5epy-1.0.2/dnd5epy/models/class_level_class_specific_any_of1.py
--rwxr-xr-x   0        0        0    12611 2023-06-22 14:49:31.578063 dnd5epy-1.0.2/dnd5epy/models/class_level_class_specific_any_of10.py
--rwxr-xr-x   0        0        0    11931 2023-06-22 14:49:31.590063 dnd5epy-1.0.2/dnd5epy/models/class_level_class_specific_any_of11.py
--rwxr-xr-x   0        0        0    12090 2023-06-22 14:49:31.594063 dnd5epy-1.0.2/dnd5epy/models/class_level_class_specific_any_of2.py
--rwxr-xr-x   0        0        0    12169 2023-06-22 14:49:31.606063 dnd5epy-1.0.2/dnd5epy/models/class_level_class_specific_any_of3.py
--rwxr-xr-x   0        0        0    12181 2023-06-22 14:49:31.614063 dnd5epy-1.0.2/dnd5epy/models/class_level_class_specific_any_of4.py
--rwxr-xr-x   0        0        0    12586 2023-06-22 14:49:31.622063 dnd5epy-1.0.2/dnd5epy/models/class_level_class_specific_any_of5.py
--rwxr-xr-x   0        0        0    12093 2023-06-22 14:49:31.630064 dnd5epy-1.0.2/dnd5epy/models/class_level_class_specific_any_of5_martial_arts.py
--rwxr-xr-x   0        0        0    11881 2023-06-22 14:49:31.642064 dnd5epy-1.0.2/dnd5epy/models/class_level_class_specific_any_of6.py
--rwxr-xr-x   0        0        0    12045 2023-06-22 14:49:31.646064 dnd5epy-1.0.2/dnd5epy/models/class_level_class_specific_any_of7.py
--rwxr-xr-x   0        0        0    12275 2023-06-22 14:49:31.658064 dnd5epy-1.0.2/dnd5epy/models/class_level_class_specific_any_of8.py
--rwxr-xr-x   0        0        0    12904 2023-06-22 14:49:31.666064 dnd5epy-1.0.2/dnd5epy/models/class_level_class_specific_any_of9.py
--rwxr-xr-x   0        0        0    12245 2023-06-22 14:49:31.674064 dnd5epy-1.0.2/dnd5epy/models/class_level_class_specific_any_of9_creating_spell_slots_inner.py
--rwxr-xr-x   0        0        0    12157 2023-06-22 14:49:31.682064 dnd5epy-1.0.2/dnd5epy/models/condition.py
--rwxr-xr-x   0        0        0    11862 2023-06-22 14:49:31.690064 dnd5epy-1.0.2/dnd5epy/models/cost.py
--rwxr-xr-x   0        0        0    12089 2023-06-22 14:49:31.710064 dnd5epy-1.0.2/dnd5epy/models/damage.py
--rwxr-xr-x   0        0        0    12268 2023-06-22 14:49:31.718064 dnd5epy-1.0.2/dnd5epy/models/damage_at_character_level.py
--rwxr-xr-x   0        0        0    12213 2023-06-22 14:49:31.726064 dnd5epy-1.0.2/dnd5epy/models/damage_at_slot_level.py
--rwxr-xr-x   0        0        0    12165 2023-06-22 14:49:31.738064 dnd5epy-1.0.2/dnd5epy/models/damage_type.py
--rwxr-xr-x   0        0        0    12320 2023-06-22 14:49:31.698064 dnd5epy-1.0.2/dnd5epy/models/dc.py
--rwxr-xr-x   0        0        0    15427 2023-06-22 14:49:31.746064 dnd5epy-1.0.2/dnd5epy/models/equipment.py
--rwxr-xr-x   0        0        0    12735 2023-06-22 14:49:31.758064 dnd5epy-1.0.2/dnd5epy/models/equipment_category.py
--rwxr-xr-x   0        0        0    13967 2023-06-22 14:49:31.766064 dnd5epy-1.0.2/dnd5epy/models/equipment_pack.py
--rwxr-xr-x   0        0        0    11667 2023-06-22 14:49:31.778064 dnd5epy-1.0.2/dnd5epy/models/error_response.py
--rwxr-xr-x   0        0        0    12818 2023-06-22 14:49:31.790064 dnd5epy-1.0.2/dnd5epy/models/feat.py
--rwxr-xr-x   0        0        0    14363 2023-06-22 14:49:31.798065 dnd5epy-1.0.2/dnd5epy/models/feature.py
--rwxr-xr-x   0        0        0    16063 2023-06-22 14:49:31.810065 dnd5epy-1.0.2/dnd5epy/models/feature_all_of_prerequisites_inner.py
--rwxr-xr-x   0        0        0    12000 2023-06-22 14:49:31.814065 dnd5epy-1.0.2/dnd5epy/models/feature_all_of_prerequisites_inner_any_of.py
--rwxr-xr-x   0        0        0    11965 2023-06-22 14:49:31.826065 dnd5epy-1.0.2/dnd5epy/models/feature_all_of_prerequisites_inner_any_of1.py
--rwxr-xr-x   0        0        0    11957 2023-06-22 14:49:31.830065 dnd5epy-1.0.2/dnd5epy/models/feature_all_of_prerequisites_inner_any_of2.py
--rwxr-xr-x   0        0        0    13516 2023-06-22 14:49:31.838065 dnd5epy-1.0.2/dnd5epy/models/gear.py
--rwxr-xr-x   0        0        0    12900 2023-06-22 14:49:31.850065 dnd5epy-1.0.2/dnd5epy/models/language.py
--rwxr-xr-x   0        0        0    13735 2023-06-22 14:49:31.858065 dnd5epy-1.0.2/dnd5epy/models/magic_item.py
--rwxr-xr-x   0        0        0    12219 2023-06-22 14:49:31.866065 dnd5epy-1.0.2/dnd5epy/models/magic_item_all_of_rarity.py
--rwxr-xr-x   0        0        0    12155 2023-06-22 14:49:31.874065 dnd5epy-1.0.2/dnd5epy/models/magic_school.py
--rwxr-xr-x   0        0        0    17637 2023-06-22 14:49:31.878065 dnd5epy-1.0.2/dnd5epy/models/model_class.py
--rwxr-xr-x   0        0        0    24067 2023-06-22 14:49:31.890065 dnd5epy-1.0.2/dnd5epy/models/monster.py
--rwxr-xr-x   0        0        0    12777 2023-06-22 14:49:31.898065 dnd5epy-1.0.2/dnd5epy/models/monster_ability.py
--rwxr-xr-x   0        0        0    14898 2023-06-22 14:49:31.906065 dnd5epy-1.0.2/dnd5epy/models/monster_action.py
--rwxr-xr-x   0        0        0    13280 2023-06-22 14:49:31.910065 dnd5epy-1.0.2/dnd5epy/models/monster_all_of_senses.py
--rwxr-xr-x   0        0        0    12898 2023-06-22 14:49:31.922065 dnd5epy-1.0.2/dnd5epy/models/monster_all_of_speed.py
--rwxr-xr-x   0        0        0    17721 2023-06-22 14:49:31.926065 dnd5epy-1.0.2/dnd5epy/models/monster_armor_class.py
--rwxr-xr-x   0        0        0    12343 2023-06-22 14:49:31.934065 dnd5epy-1.0.2/dnd5epy/models/monster_armor_class_one_of.py
--rwxr-xr-x   0        0        0    12275 2023-06-22 14:49:31.942065 dnd5epy-1.0.2/dnd5epy/models/monster_armor_class_one_of1.py
--rwxr-xr-x   0        0        0    12829 2023-06-22 14:49:31.950065 dnd5epy-1.0.2/dnd5epy/models/monster_armor_class_one_of2.py
--rwxr-xr-x   0        0        0    12644 2023-06-22 14:49:31.958065 dnd5epy-1.0.2/dnd5epy/models/monster_armor_class_one_of3.py
--rwxr-xr-x   0        0        0    12688 2023-06-22 14:49:31.962066 dnd5epy-1.0.2/dnd5epy/models/monster_armor_class_one_of4.py
--rwxr-xr-x   0        0        0    12349 2023-06-22 14:49:31.970065 dnd5epy-1.0.2/dnd5epy/models/monster_attack.py
--rwxr-xr-x   0        0        0    12367 2023-06-22 14:49:31.982066 dnd5epy-1.0.2/dnd5epy/models/monster_multi_attack_action.py
--rwxr-xr-x   0        0        0    12198 2023-06-22 14:49:31.990066 dnd5epy-1.0.2/dnd5epy/models/monster_proficiency.py
--rwxr-xr-x   0        0        0    13149 2023-06-22 14:49:31.998066 dnd5epy-1.0.2/dnd5epy/models/monster_sense.py
--rwxr-xr-x   0        0        0    13497 2023-06-22 14:49:32.010066 dnd5epy-1.0.2/dnd5epy/models/monster_special_ability.py
--rwxr-xr-x   0        0        0    12267 2023-06-22 14:49:32.018066 dnd5epy-1.0.2/dnd5epy/models/monster_spell.py
--rwxr-xr-x   0        0        0    13218 2023-06-22 14:49:32.026066 dnd5epy-1.0.2/dnd5epy/models/monster_spellcasting.py
--rwxr-xr-x   0        0        0    12343 2023-06-22 14:49:32.034066 dnd5epy-1.0.2/dnd5epy/models/monster_usage.py
--rwxr-xr-x   0        0        0    14391 2023-06-22 14:49:32.042066 dnd5epy-1.0.2/dnd5epy/models/multiclassing.py
--rwxr-xr-x   0        0        0    20796 2023-06-22 14:49:32.054066 dnd5epy-1.0.2/dnd5epy/models/option.py
--rwxr-xr-x   0        0        0    12137 2023-06-22 14:49:32.062066 dnd5epy-1.0.2/dnd5epy/models/option_one_of.py
--rwxr-xr-x   0        0        0    12672 2023-06-22 14:49:32.070066 dnd5epy-1.0.2/dnd5epy/models/option_one_of1.py
--rwxr-xr-x   0        0        0    12532 2023-06-22 14:49:32.078066 dnd5epy-1.0.2/dnd5epy/models/option_one_of10.py
--rwxr-xr-x   0        0        0    12266 2023-06-22 14:49:32.086066 dnd5epy-1.0.2/dnd5epy/models/option_one_of2.py
--rwxr-xr-x   0        0        0    12090 2023-06-22 14:49:32.094066 dnd5epy-1.0.2/dnd5epy/models/option_one_of3.py
--rwxr-xr-x   0        0        0    11905 2023-06-22 14:49:32.110066 dnd5epy-1.0.2/dnd5epy/models/option_one_of4.py
--rwxr-xr-x   0        0        0    12596 2023-06-22 14:49:32.122066 dnd5epy-1.0.2/dnd5epy/models/option_one_of5.py
--rwxr-xr-x   0        0        0    12292 2023-06-22 14:49:32.130066 dnd5epy-1.0.2/dnd5epy/models/option_one_of6.py
--rwxr-xr-x   0        0        0    12473 2023-06-22 14:49:32.142067 dnd5epy-1.0.2/dnd5epy/models/option_one_of7.py
--rwxr-xr-x   0        0        0    12430 2023-06-22 14:49:32.146067 dnd5epy-1.0.2/dnd5epy/models/option_one_of8.py
--rwxr-xr-x   0        0        0    12816 2023-06-22 14:49:32.158067 dnd5epy-1.0.2/dnd5epy/models/option_one_of9.py
--rwxr-xr-x   0        0        0    15531 2023-06-22 14:49:32.166067 dnd5epy-1.0.2/dnd5epy/models/option_set.py
--rwxr-xr-x   0        0        0    12429 2023-06-22 14:49:32.178067 dnd5epy-1.0.2/dnd5epy/models/option_set_one_of.py
--rwxr-xr-x   0        0        0    12315 2023-06-22 14:49:32.186067 dnd5epy-1.0.2/dnd5epy/models/option_set_one_of1.py
--rwxr-xr-x   0        0        0    12019 2023-06-22 14:49:32.194067 dnd5epy-1.0.2/dnd5epy/models/option_set_one_of2.py
--rwxr-xr-x   0        0        0    12321 2023-06-22 14:49:32.198067 dnd5epy-1.0.2/dnd5epy/models/prerequisite.py
--rwxr-xr-x   0        0        0    12117 2023-06-22 14:49:32.206067 dnd5epy-1.0.2/dnd5epy/models/prerequisite_ability_score.py
--rwxr-xr-x   0        0        0    13808 2023-06-22 14:49:32.214067 dnd5epy-1.0.2/dnd5epy/models/proficiency.py
--rwxr-xr-x   0        0        0    12164 2023-06-22 14:49:32.218067 dnd5epy-1.0.2/dnd5epy/models/proficiency_all_of_reference.py
--rwxr-xr-x   0        0        0    16807 2023-06-22 14:49:32.230067 dnd5epy-1.0.2/dnd5epy/models/race.py
--rwxr-xr-x   0        0        0    11817 2023-06-22 14:49:32.234067 dnd5epy-1.0.2/dnd5epy/models/resource_description.py
--rwxr-xr-x   0        0        0    12792 2023-06-22 14:49:32.242067 dnd5epy-1.0.2/dnd5epy/models/rule.py
--rwxr-xr-x   0        0        0    12145 2023-06-22 14:49:32.246067 dnd5epy-1.0.2/dnd5epy/models/rule_section.py
--rwxr-xr-x   0        0        0    12570 2023-06-22 14:49:32.254067 dnd5epy-1.0.2/dnd5epy/models/skill.py
--rwxr-xr-x   0        0        0    16680 2023-06-22 14:49:32.262067 dnd5epy-1.0.2/dnd5epy/models/spell.py
--rwxr-xr-x   0        0        0    15091 2023-06-22 14:49:32.274067 dnd5epy-1.0.2/dnd5epy/models/spell_all_of_damage.py
--rwxr-xr-x   0        0        0    12194 2023-06-22 14:49:32.278067 dnd5epy-1.0.2/dnd5epy/models/spell_prerequisite.py
--rwxr-xr-x   0        0        0    13068 2023-06-22 14:49:32.286067 dnd5epy-1.0.2/dnd5epy/models/spellcasting.py
--rwxr-xr-x   0        0        0    11943 2023-06-22 14:49:32.294067 dnd5epy-1.0.2/dnd5epy/models/spellcasting_info_inner.py
--rwxr-xr-x   0        0        0    12209 2023-06-22 14:49:32.306067 dnd5epy-1.0.2/dnd5epy/models/spellcasting_spellcasting_ability.py
--rwxr-xr-x   0        0        0    13559 2023-06-22 14:49:32.318067 dnd5epy-1.0.2/dnd5epy/models/subclass.py
--rwxr-xr-x   0        0        0    12665 2023-06-22 14:49:32.326068 dnd5epy-1.0.2/dnd5epy/models/subclass_all_of_spells.py
--rwxr-xr-x   0        0        0    13956 2023-06-22 14:49:32.338068 dnd5epy-1.0.2/dnd5epy/models/subclass_level.py
--rwxr-xr-x   0        0        0    13255 2023-06-22 14:49:32.346068 dnd5epy-1.0.2/dnd5epy/models/subclass_level_resource.py
--rwxr-xr-x   0        0        0    13468 2023-06-22 14:49:32.354068 dnd5epy-1.0.2/dnd5epy/models/subclass_level_spellcasting.py
--rwxr-xr-x   0        0        0    15650 2023-06-22 14:49:32.362068 dnd5epy-1.0.2/dnd5epy/models/subrace.py
--rwxr-xr-x   0        0        0    12065 2023-06-22 14:49:32.378068 dnd5epy-1.0.2/dnd5epy/models/subrace_all_of_race.py
--rwxr-xr-x   0        0        0    15311 2023-06-22 14:49:32.386068 dnd5epy-1.0.2/dnd5epy/models/trait.py
--rwxr-xr-x   0        0        0    15624 2023-06-22 14:49:32.402068 dnd5epy-1.0.2/dnd5epy/models/trait_all_of_trait_specific.py
--rwxr-xr-x   0        0        0    12881 2023-06-22 14:49:32.406068 dnd5epy-1.0.2/dnd5epy/models/trait_all_of_trait_specific_one_of.py
--rwxr-xr-x   0        0        0    13805 2023-06-22 14:49:32.414068 dnd5epy-1.0.2/dnd5epy/models/trait_all_of_trait_specific_one_of_breath_weapon.py
--rwxr-xr-x   0        0        0    12528 2023-06-22 14:49:32.422068 dnd5epy-1.0.2/dnd5epy/models/trait_all_of_trait_specific_one_of_breath_weapon_damage.py
--rwxr-xr-x   0        0        0    12087 2023-06-22 14:49:32.426068 dnd5epy-1.0.2/dnd5epy/models/trait_all_of_trait_specific_one_of_breath_weapon_usage.py
--rwxr-xr-x   0        0        0    12232 2023-06-22 14:49:32.434068 dnd5epy-1.0.2/dnd5epy/models/trait_all_of_trait_specific_one_of_damage_type.py
--rwxr-xr-x   0        0        0    15456 2023-06-22 14:49:32.446068 dnd5epy-1.0.2/dnd5epy/models/weapon.py
--rwxr-xr-x   0        0        0    11980 2023-06-22 14:49:32.458068 dnd5epy-1.0.2/dnd5epy/models/weapon_all_of_range.py
--rwxr-xr-x   0        0        0    12194 2023-06-22 14:49:32.466068 dnd5epy-1.0.2/dnd5epy/models/weapon_property.py
--rwxr-xr-x   0        0        0        0 2023-06-22 14:49:33.154072 dnd5epy-1.0.2/dnd5epy/py.typed
--rwxr-xr-x   0        0        0    22711 2023-06-22 14:49:33.174072 dnd5epy-1.0.2/dnd5epy/rest.py
--rwxr-xr-x   0        0        0      698 2023-06-22 15:29:38.301197 dnd5epy-1.0.2/pyproject.toml
--rw-r--r--   0        0        0    27720 1970-01-01 00:00:00.000000 dnd5epy-1.0.2/PKG-INFO
+-rwxr-xr-x   0        0        0    26797 2023-06-22 15:33:23.768866 dnd5epy-1.0.3/README.md
+-rwxr-xr-x   0        0        0    19294 2023-06-22 15:33:23.768866 dnd5epy-1.0.3/dnd5epy/__init__.py
+-rwxr-xr-x   0        0        0      853 2023-06-22 15:33:23.776866 dnd5epy-1.0.3/dnd5epy/api/__init__.py
+-rwxr-xr-x   0        0        0    57549 2023-06-22 15:33:23.768866 dnd5epy-1.0.3/dnd5epy/api/character_data_api.py
+-rwxr-xr-x   0        0        0    29887 2023-06-22 15:33:23.776866 dnd5epy-1.0.3/dnd5epy/api/class_api.py
+-rwxr-xr-x   0        0        0    37716 2023-06-22 15:33:23.776866 dnd5epy-1.0.3/dnd5epy/api/class_levels_api.py
+-rwxr-xr-x   0        0        0    35125 2023-06-22 15:33:23.772866 dnd5epy-1.0.3/dnd5epy/api/class_resource_lists_api.py
+-rwxr-xr-x   0        0        0    22826 2023-06-22 15:33:23.772866 dnd5epy-1.0.3/dnd5epy/api/common_api.py
+-rwxr-xr-x   0        0        0    37122 2023-06-22 15:33:23.772866 dnd5epy-1.0.3/dnd5epy/api/equipment_api.py
+-rwxr-xr-x   0        0        0    16968 2023-06-22 15:33:23.776866 dnd5epy-1.0.3/dnd5epy/api/feats_api.py
+-rwxr-xr-x   0        0        0    17789 2023-06-22 15:33:23.772866 dnd5epy-1.0.3/dnd5epy/api/features_api.py
+-rwxr-xr-x   0        0        0    30674 2023-06-22 15:33:23.776866 dnd5epy-1.0.3/dnd5epy/api/game_mechanics_api.py
+-rwxr-xr-x   0        0        0    23241 2023-06-22 15:33:23.772866 dnd5epy-1.0.3/dnd5epy/api/monsters_api.py
+-rwxr-xr-x   0        0        0    35105 2023-06-22 15:33:23.772866 dnd5epy-1.0.3/dnd5epy/api/races_api.py
+-rwxr-xr-x   0        0        0    23606 2023-06-22 15:33:23.772866 dnd5epy-1.0.3/dnd5epy/api/rules_api.py
+-rwxr-xr-x   0        0        0    23942 2023-06-22 15:33:23.772866 dnd5epy-1.0.3/dnd5epy/api/spells_api.py
+-rwxr-xr-x   0        0        0    42854 2023-06-22 15:33:23.768866 dnd5epy-1.0.3/dnd5epy/api/subclasses_api.py
+-rwxr-xr-x   0        0        0    29190 2023-06-22 15:33:23.776866 dnd5epy-1.0.3/dnd5epy/api/subraces_api.py
+-rwxr-xr-x   0        0        0    16747 2023-06-22 15:33:23.776866 dnd5epy-1.0.3/dnd5epy/api/traits_api.py
+-rwxr-xr-x   0        0        0    39800 2023-06-22 15:33:23.768866 dnd5epy-1.0.3/dnd5epy/api_client.py
+-rwxr-xr-x   0        0        0      844 2023-06-22 14:49:33.174072 dnd5epy-1.0.3/dnd5epy/api_response.py
+-rwxr-xr-x   0        0        0    24338 2023-06-22 15:33:23.768866 dnd5epy-1.0.3/dnd5epy/configuration.py
+-rwxr-xr-x   0        0        0    15141 2023-06-22 14:49:33.166072 dnd5epy-1.0.3/dnd5epy/exceptions.py
+-rwxr-xr-x   0        0        0    18008 2023-06-22 15:33:23.792867 dnd5epy-1.0.3/dnd5epy/models/__init__.py
+-rwxr-xr-x   0        0        0    12227 2023-06-22 15:33:23.788867 dnd5epy-1.0.3/dnd5epy/models/ability_bonus.py
+-rwxr-xr-x   0        0        0    12948 2023-06-22 15:33:23.796867 dnd5epy-1.0.3/dnd5epy/models/ability_score.py
+-rwxr-xr-x   0        0        0    12324 2023-06-22 14:49:31.454063 dnd5epy-1.0.3/dnd5epy/models/alignment.py
+-rwxr-xr-x   0        0        0    12024 2023-06-22 14:49:31.378062 dnd5epy-1.0.3/dnd5epy/models/api_reference.py
+-rwxr-xr-x   0        0        0    12393 2023-06-22 15:33:23.796867 dnd5epy-1.0.3/dnd5epy/models/api_reference_list.py
+-rwxr-xr-x   0        0        0    12171 2023-06-22 14:49:31.466063 dnd5epy-1.0.3/dnd5epy/models/area_of_effect.py
+-rwxr-xr-x   0        0        0    13922 2023-06-22 15:33:23.784866 dnd5epy-1.0.3/dnd5epy/models/armor.py
+-rwxr-xr-x   0        0        0    15973 2023-06-22 15:33:23.788867 dnd5epy-1.0.3/dnd5epy/models/background.py
+-rwxr-xr-x   0        0        0    11904 2023-06-22 14:49:31.506063 dnd5epy-1.0.3/dnd5epy/models/background_all_of_feature.py
+-rwxr-xr-x   0        0        0    12383 2023-06-22 14:49:31.514063 dnd5epy-1.0.3/dnd5epy/models/choice.py
+-rwxr-xr-x   0        0        0    12257 2023-06-22 15:33:23.796867 dnd5epy-1.0.3/dnd5epy/models/class_all_of_starting_equipment.py
+-rwxr-xr-x   0        0        0    14168 2023-06-22 15:33:23.776866 dnd5epy-1.0.3/dnd5epy/models/class_level.py
+-rwxr-xr-x   0        0        0    23758 2023-06-22 15:33:23.788867 dnd5epy-1.0.3/dnd5epy/models/class_level_class_specific.py
+-rwxr-xr-x   0        0        0    12196 2023-06-22 14:49:31.562063 dnd5epy-1.0.3/dnd5epy/models/class_level_class_specific_any_of.py
+-rwxr-xr-x   0        0        0    12590 2023-06-22 14:49:31.570063 dnd5epy-1.0.3/dnd5epy/models/class_level_class_specific_any_of1.py
+-rwxr-xr-x   0        0        0    12611 2023-06-22 14:49:31.578063 dnd5epy-1.0.3/dnd5epy/models/class_level_class_specific_any_of10.py
+-rwxr-xr-x   0        0        0    11931 2023-06-22 14:49:31.590063 dnd5epy-1.0.3/dnd5epy/models/class_level_class_specific_any_of11.py
+-rwxr-xr-x   0        0        0    12090 2023-06-22 14:49:31.594063 dnd5epy-1.0.3/dnd5epy/models/class_level_class_specific_any_of2.py
+-rwxr-xr-x   0        0        0    12169 2023-06-22 14:49:31.606063 dnd5epy-1.0.3/dnd5epy/models/class_level_class_specific_any_of3.py
+-rwxr-xr-x   0        0        0    12181 2023-06-22 14:49:31.614063 dnd5epy-1.0.3/dnd5epy/models/class_level_class_specific_any_of4.py
+-rwxr-xr-x   0        0        0    12579 2023-06-22 15:33:23.784866 dnd5epy-1.0.3/dnd5epy/models/class_level_class_specific_any_of5.py
+-rwxr-xr-x   0        0        0    12093 2023-06-22 14:49:31.630064 dnd5epy-1.0.3/dnd5epy/models/class_level_class_specific_any_of5_martial_arts.py
+-rwxr-xr-x   0        0        0    11881 2023-06-22 14:49:31.642064 dnd5epy-1.0.3/dnd5epy/models/class_level_class_specific_any_of6.py
+-rwxr-xr-x   0        0        0    12045 2023-06-22 14:49:31.646064 dnd5epy-1.0.3/dnd5epy/models/class_level_class_specific_any_of7.py
+-rwxr-xr-x   0        0        0    12268 2023-06-22 15:33:23.784866 dnd5epy-1.0.3/dnd5epy/models/class_level_class_specific_any_of8.py
+-rwxr-xr-x   0        0        0    12897 2023-06-22 15:33:23.796867 dnd5epy-1.0.3/dnd5epy/models/class_level_class_specific_any_of9.py
+-rwxr-xr-x   0        0        0    12245 2023-06-22 14:49:31.674064 dnd5epy-1.0.3/dnd5epy/models/class_level_class_specific_any_of9_creating_spell_slots_inner.py
+-rwxr-xr-x   0        0        0    12157 2023-06-22 14:49:31.682064 dnd5epy-1.0.3/dnd5epy/models/condition.py
+-rwxr-xr-x   0        0        0    11862 2023-06-22 14:49:31.690064 dnd5epy-1.0.3/dnd5epy/models/cost.py
+-rwxr-xr-x   0        0        0    12082 2023-06-22 15:33:23.796867 dnd5epy-1.0.3/dnd5epy/models/damage.py
+-rwxr-xr-x   0        0        0    12261 2023-06-22 15:33:23.788867 dnd5epy-1.0.3/dnd5epy/models/damage_at_character_level.py
+-rwxr-xr-x   0        0        0    12206 2023-06-22 15:33:23.784866 dnd5epy-1.0.3/dnd5epy/models/damage_at_slot_level.py
+-rwxr-xr-x   0        0        0    12165 2023-06-22 14:49:31.738064 dnd5epy-1.0.3/dnd5epy/models/damage_type.py
+-rwxr-xr-x   0        0        0    12313 2023-06-22 15:33:23.796867 dnd5epy-1.0.3/dnd5epy/models/dc.py
+-rwxr-xr-x   0        0        0    15399 2023-06-22 15:33:23.776866 dnd5epy-1.0.3/dnd5epy/models/equipment.py
+-rwxr-xr-x   0        0        0    12728 2023-06-22 15:33:23.804867 dnd5epy-1.0.3/dnd5epy/models/equipment_category.py
+-rwxr-xr-x   0        0        0    13953 2023-06-22 15:33:23.776866 dnd5epy-1.0.3/dnd5epy/models/equipment_pack.py
+-rwxr-xr-x   0        0        0    11667 2023-06-22 14:49:31.778064 dnd5epy-1.0.3/dnd5epy/models/error_response.py
+-rwxr-xr-x   0        0        0    12811 2023-06-22 15:33:23.808867 dnd5epy-1.0.3/dnd5epy/models/feat.py
+-rwxr-xr-x   0        0        0    14349 2023-06-22 15:33:23.804867 dnd5epy-1.0.3/dnd5epy/models/feature.py
+-rwxr-xr-x   0        0        0    16042 2023-06-22 15:33:23.796867 dnd5epy-1.0.3/dnd5epy/models/feature_all_of_prerequisites_inner.py
+-rwxr-xr-x   0        0        0    12000 2023-06-22 14:49:31.814065 dnd5epy-1.0.3/dnd5epy/models/feature_all_of_prerequisites_inner_any_of.py
+-rwxr-xr-x   0        0        0    11965 2023-06-22 14:49:31.826065 dnd5epy-1.0.3/dnd5epy/models/feature_all_of_prerequisites_inner_any_of1.py
+-rwxr-xr-x   0        0        0    11957 2023-06-22 14:49:31.830065 dnd5epy-1.0.3/dnd5epy/models/feature_all_of_prerequisites_inner_any_of2.py
+-rwxr-xr-x   0        0        0    13502 2023-06-22 15:33:23.808867 dnd5epy-1.0.3/dnd5epy/models/gear.py
+-rwxr-xr-x   0        0        0    12900 2023-06-22 14:49:31.850065 dnd5epy-1.0.3/dnd5epy/models/language.py
+-rwxr-xr-x   0        0        0    13721 2023-06-22 15:33:23.796867 dnd5epy-1.0.3/dnd5epy/models/magic_item.py
+-rwxr-xr-x   0        0        0    12219 2023-06-22 14:49:31.866065 dnd5epy-1.0.3/dnd5epy/models/magic_item_all_of_rarity.py
+-rwxr-xr-x   0        0        0    12155 2023-06-22 14:49:31.874065 dnd5epy-1.0.3/dnd5epy/models/magic_school.py
+-rwxr-xr-x   0        0        0    17602 2023-06-22 15:33:23.796867 dnd5epy-1.0.3/dnd5epy/models/model_class.py
+-rwxr-xr-x   0        0        0    24018 2023-06-22 15:33:23.796867 dnd5epy-1.0.3/dnd5epy/models/monster.py
+-rwxr-xr-x   0        0        0    12777 2023-06-22 14:49:31.898065 dnd5epy-1.0.3/dnd5epy/models/monster_ability.py
+-rwxr-xr-x   0        0        0    14863 2023-06-22 15:33:23.784866 dnd5epy-1.0.3/dnd5epy/models/monster_action.py
+-rwxr-xr-x   0        0        0    13280 2023-06-22 14:49:31.910065 dnd5epy-1.0.3/dnd5epy/models/monster_all_of_senses.py
+-rwxr-xr-x   0        0        0    12898 2023-06-22 14:49:31.922065 dnd5epy-1.0.3/dnd5epy/models/monster_all_of_speed.py
+-rwxr-xr-x   0        0        0    17686 2023-06-22 15:33:23.796867 dnd5epy-1.0.3/dnd5epy/models/monster_armor_class.py
+-rwxr-xr-x   0        0        0    12343 2023-06-22 14:49:31.934065 dnd5epy-1.0.3/dnd5epy/models/monster_armor_class_one_of.py
+-rwxr-xr-x   0        0        0    12275 2023-06-22 14:49:31.942065 dnd5epy-1.0.3/dnd5epy/models/monster_armor_class_one_of1.py
+-rwxr-xr-x   0        0        0    12822 2023-06-22 15:33:23.776866 dnd5epy-1.0.3/dnd5epy/models/monster_armor_class_one_of2.py
+-rwxr-xr-x   0        0        0    12637 2023-06-22 15:33:23.808867 dnd5epy-1.0.3/dnd5epy/models/monster_armor_class_one_of3.py
+-rwxr-xr-x   0        0        0    12681 2023-06-22 15:33:23.788867 dnd5epy-1.0.3/dnd5epy/models/monster_armor_class_one_of4.py
+-rwxr-xr-x   0        0        0    12335 2023-06-22 15:33:23.788867 dnd5epy-1.0.3/dnd5epy/models/monster_attack.py
+-rwxr-xr-x   0        0        0    12367 2023-06-22 14:49:31.982066 dnd5epy-1.0.3/dnd5epy/models/monster_multi_attack_action.py
+-rwxr-xr-x   0        0        0    12191 2023-06-22 15:33:23.796867 dnd5epy-1.0.3/dnd5epy/models/monster_proficiency.py
+-rwxr-xr-x   0        0        0    13149 2023-06-22 14:49:31.998066 dnd5epy-1.0.3/dnd5epy/models/monster_sense.py
+-rwxr-xr-x   0        0        0    13469 2023-06-22 15:33:23.796867 dnd5epy-1.0.3/dnd5epy/models/monster_special_ability.py
+-rwxr-xr-x   0        0        0    12260 2023-06-22 15:33:23.784866 dnd5epy-1.0.3/dnd5epy/models/monster_spell.py
+-rwxr-xr-x   0        0        0    13204 2023-06-22 15:33:23.780866 dnd5epy-1.0.3/dnd5epy/models/monster_spellcasting.py
+-rwxr-xr-x   0        0        0    12343 2023-06-22 14:49:32.034066 dnd5epy-1.0.3/dnd5epy/models/monster_usage.py
+-rwxr-xr-x   0        0        0    14370 2023-06-22 15:33:23.796867 dnd5epy-1.0.3/dnd5epy/models/multiclassing.py
+-rwxr-xr-x   0        0        0    20733 2023-06-22 15:33:23.780866 dnd5epy-1.0.3/dnd5epy/models/option.py
+-rwxr-xr-x   0        0        0    12130 2023-06-22 15:33:23.808867 dnd5epy-1.0.3/dnd5epy/models/option_one_of.py
+-rwxr-xr-x   0        0        0    12672 2023-06-22 14:49:32.070066 dnd5epy-1.0.3/dnd5epy/models/option_one_of1.py
+-rwxr-xr-x   0        0        0    12525 2023-06-22 15:33:23.808867 dnd5epy-1.0.3/dnd5epy/models/option_one_of10.py
+-rwxr-xr-x   0        0        0    12266 2023-06-22 14:49:32.086066 dnd5epy-1.0.3/dnd5epy/models/option_one_of2.py
+-rwxr-xr-x   0        0        0    12090 2023-06-22 14:49:32.094066 dnd5epy-1.0.3/dnd5epy/models/option_one_of3.py
+-rwxr-xr-x   0        0        0    11905 2023-06-22 14:49:32.110066 dnd5epy-1.0.3/dnd5epy/models/option_one_of4.py
+-rwxr-xr-x   0        0        0    12589 2023-06-22 15:33:23.796867 dnd5epy-1.0.3/dnd5epy/models/option_one_of5.py
+-rwxr-xr-x   0        0        0    12285 2023-06-22 15:33:23.792867 dnd5epy-1.0.3/dnd5epy/models/option_one_of6.py
+-rwxr-xr-x   0        0        0    12466 2023-06-22 15:33:23.788867 dnd5epy-1.0.3/dnd5epy/models/option_one_of7.py
+-rwxr-xr-x   0        0        0    12423 2023-06-22 15:33:23.804867 dnd5epy-1.0.3/dnd5epy/models/option_one_of8.py
+-rwxr-xr-x   0        0        0    12802 2023-06-22 15:33:23.780866 dnd5epy-1.0.3/dnd5epy/models/option_one_of9.py
+-rwxr-xr-x   0        0        0    15517 2023-06-22 15:33:23.788867 dnd5epy-1.0.3/dnd5epy/models/option_set.py
+-rwxr-xr-x   0        0        0    12429 2023-06-22 14:49:32.178067 dnd5epy-1.0.3/dnd5epy/models/option_set_one_of.py
+-rwxr-xr-x   0        0        0    12308 2023-06-22 15:33:23.796867 dnd5epy-1.0.3/dnd5epy/models/option_set_one_of1.py
+-rwxr-xr-x   0        0        0    12019 2023-06-22 14:49:32.194067 dnd5epy-1.0.3/dnd5epy/models/option_set_one_of2.py
+-rwxr-xr-x   0        0        0    12314 2023-06-22 15:33:23.792867 dnd5epy-1.0.3/dnd5epy/models/prerequisite.py
+-rwxr-xr-x   0        0        0    12117 2023-06-22 14:49:32.206067 dnd5epy-1.0.3/dnd5epy/models/prerequisite_ability_score.py
+-rwxr-xr-x   0        0        0    13794 2023-06-22 15:33:23.808867 dnd5epy-1.0.3/dnd5epy/models/proficiency.py
+-rwxr-xr-x   0        0        0    12164 2023-06-22 14:49:32.218067 dnd5epy-1.0.3/dnd5epy/models/proficiency_all_of_reference.py
+-rwxr-xr-x   0        0        0    16786 2023-06-22 15:33:23.796867 dnd5epy-1.0.3/dnd5epy/models/race.py
+-rwxr-xr-x   0        0        0    11817 2023-06-22 14:49:32.234067 dnd5epy-1.0.3/dnd5epy/models/resource_description.py
+-rwxr-xr-x   0        0        0    12785 2023-06-22 15:33:23.776866 dnd5epy-1.0.3/dnd5epy/models/rule.py
+-rwxr-xr-x   0        0        0    12145 2023-06-22 14:49:32.246067 dnd5epy-1.0.3/dnd5epy/models/rule_section.py
+-rwxr-xr-x   0        0        0    12563 2023-06-22 15:33:23.792867 dnd5epy-1.0.3/dnd5epy/models/skill.py
+-rwxr-xr-x   0        0        0    16659 2023-06-22 15:33:23.788867 dnd5epy-1.0.3/dnd5epy/models/spell.py
+-rwxr-xr-x   0        0        0    15077 2023-06-22 15:33:23.796867 dnd5epy-1.0.3/dnd5epy/models/spell_all_of_damage.py
+-rwxr-xr-x   0        0        0    12194 2023-06-22 14:49:32.278067 dnd5epy-1.0.3/dnd5epy/models/spell_prerequisite.py
+-rwxr-xr-x   0        0        0    13054 2023-06-22 15:33:23.788867 dnd5epy-1.0.3/dnd5epy/models/spellcasting.py
+-rwxr-xr-x   0        0        0    11943 2023-06-22 14:49:32.294067 dnd5epy-1.0.3/dnd5epy/models/spellcasting_info_inner.py
+-rwxr-xr-x   0        0        0    12209 2023-06-22 14:49:32.306067 dnd5epy-1.0.3/dnd5epy/models/spellcasting_spellcasting_ability.py
+-rwxr-xr-x   0        0        0    13545 2023-06-22 15:33:23.796867 dnd5epy-1.0.3/dnd5epy/models/subclass.py
+-rwxr-xr-x   0        0        0    12651 2023-06-22 15:33:23.808867 dnd5epy-1.0.3/dnd5epy/models/subclass_all_of_spells.py
+-rwxr-xr-x   0        0        0    13942 2023-06-22 15:33:23.788867 dnd5epy-1.0.3/dnd5epy/models/subclass_level.py
+-rwxr-xr-x   0        0        0    13248 2023-06-22 15:33:23.804867 dnd5epy-1.0.3/dnd5epy/models/subclass_level_resource.py
+-rwxr-xr-x   0        0        0    13468 2023-06-22 14:49:32.354068 dnd5epy-1.0.3/dnd5epy/models/subclass_level_spellcasting.py
+-rwxr-xr-x   0        0        0    15622 2023-06-22 15:33:23.796867 dnd5epy-1.0.3/dnd5epy/models/subrace.py
+-rwxr-xr-x   0        0        0    12065 2023-06-22 14:49:32.378068 dnd5epy-1.0.3/dnd5epy/models/subrace_all_of_race.py
+-rwxr-xr-x   0        0        0    15290 2023-06-22 15:33:23.796867 dnd5epy-1.0.3/dnd5epy/models/trait.py
+-rwxr-xr-x   0        0        0    15610 2023-06-22 15:33:23.788867 dnd5epy-1.0.3/dnd5epy/models/trait_all_of_trait_specific.py
+-rwxr-xr-x   0        0        0    12867 2023-06-22 15:33:23.808867 dnd5epy-1.0.3/dnd5epy/models/trait_all_of_trait_specific_one_of.py
+-rwxr-xr-x   0        0        0    13777 2023-06-22 15:33:23.804867 dnd5epy-1.0.3/dnd5epy/models/trait_all_of_trait_specific_one_of_breath_weapon.py
+-rwxr-xr-x   0        0        0    12521 2023-06-22 15:33:23.788867 dnd5epy-1.0.3/dnd5epy/models/trait_all_of_trait_specific_one_of_breath_weapon_damage.py
+-rwxr-xr-x   0        0        0    12087 2023-06-22 14:49:32.426068 dnd5epy-1.0.3/dnd5epy/models/trait_all_of_trait_specific_one_of_breath_weapon_usage.py
+-rwxr-xr-x   0        0        0    12232 2023-06-22 14:49:32.434068 dnd5epy-1.0.3/dnd5epy/models/trait_all_of_trait_specific_one_of_damage_type.py
+-rwxr-xr-x   0        0        0    15428 2023-06-22 15:33:23.784866 dnd5epy-1.0.3/dnd5epy/models/weapon.py
+-rwxr-xr-x   0        0        0    11980 2023-06-22 14:49:32.458068 dnd5epy-1.0.3/dnd5epy/models/weapon_all_of_range.py
+-rwxr-xr-x   0        0        0    12194 2023-06-22 14:49:32.466068 dnd5epy-1.0.3/dnd5epy/models/weapon_property.py
+-rwxr-xr-x   0        0        0        0 2023-06-22 14:49:33.154072 dnd5epy-1.0.3/dnd5epy/py.typed
+-rwxr-xr-x   0        0        0    22704 2023-06-22 15:33:23.768866 dnd5epy-1.0.3/dnd5epy/rest.py
+-rwxr-xr-x   0        0        0      691 2023-06-22 15:34:41.323504 dnd5epy-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0    27671 1970-01-01 00:00:00.000000 dnd5epy-1.0.3/PKG-INFO
```

### Comparing `dnd5epy-1.0.2/README.md` & `dnd5epy-1.0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -223,58 +223,58 @@
 ```sh
 pip install git+https://github.com/GIT_USER_ID/GIT_REPO_ID.git
 ```
 (you may need to run `pip` with root permission: `sudo pip install git+https://github.com/GIT_USER_ID/GIT_REPO_ID.git`)
 
 Then import the package:
 ```python
-import openapi_client
+import dnd5epy
 ```
 
 ### Setuptools
 
 Install via [Setuptools](http://pypi.python.org/pypi/setuptools).
 
 ```sh
 python setup.py install --user
 ```
 (or `sudo python setup.py install` to install the package for all users)
 
 Then import the package:
 ```python
-import openapi_client
+import dnd5epy
 ```
 
 ### Tests
 
 Execute `pytest` to run the tests.
 
 ## Getting Started
 
 Please follow the [installation procedure](#installation--usage) and then run the following:
 
 ```python
 
 import time
-import openapi_client
-from openapi_client.rest import ApiException
+import dnd5epy
+from dnd5epy.rest import ApiException
 from pprint import pprint
 
 # Defining the host is optional and defaults to https://www.dnd5eapi.co
 # See configuration.py for a list of all supported configuration parameters.
-configuration = openapi_client.Configuration(
+configuration = dnd5epy.Configuration(
     host = "https://www.dnd5eapi.co"
 )
 
 
 
 # Enter a context with an instance of the API client
-with openapi_client.ApiClient(configuration) as api_client:
+with dnd5epy.ApiClient(configuration) as api_client:
     # Create an instance of the API class
-    api_instance = openapi_client.CharacterDataApi(api_client)
+    api_instance = dnd5epy.CharacterDataApi(api_client)
 
     try:
         # Get all ability scores.
         api_response = api_instance.api_ability_scores_get()
         print("The response of CharacterDataApi->api_ability_scores_get:\n")
         pprint(api_response)
     except ApiException as e:
```

### Comparing `dnd5epy-1.0.2/dnd5epy/api/character_data_api.py` & `dnd5epy-1.0.3/dnd5epy/api/character_data_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,24 +19,24 @@
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
 from pydantic import Field, StrictStr
 
 from typing import List
 
-from openapi_client.models.ability_score import AbilityScore
-from openapi_client.models.alignment import Alignment
-from openapi_client.models.background import Background
-from openapi_client.models.language import Language
-from openapi_client.models.proficiency import Proficiency
-from openapi_client.models.skill import Skill
-
-from openapi_client.api_client import ApiClient
-from openapi_client.api_response import ApiResponse
-from openapi_client.exceptions import (  # noqa: F401
+from dnd5epy.models.ability_score import AbilityScore
+from dnd5epy.models.alignment import Alignment
+from dnd5epy.models.background import Background
+from dnd5epy.models.language import Language
+from dnd5epy.models.proficiency import Proficiency
+from dnd5epy.models.skill import Skill
+
+from dnd5epy.api_client import ApiClient
+from dnd5epy.api_response import ApiResponse
+from dnd5epy.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 
 class CharacterDataApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
```

### Comparing `dnd5epy-1.0.2/dnd5epy/api/class_api.py` & `dnd5epy-1.0.3/dnd5epy/api/class_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,21 +17,21 @@
 import warnings
 
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
 from pydantic import Field, StrictStr
 
-from openapi_client.models.model_class import ModelClass
-from openapi_client.models.multiclassing import Multiclassing
-from openapi_client.models.spellcasting import Spellcasting
-
-from openapi_client.api_client import ApiClient
-from openapi_client.api_response import ApiResponse
-from openapi_client.exceptions import (  # noqa: F401
+from dnd5epy.models.model_class import ModelClass
+from dnd5epy.models.multiclassing import Multiclassing
+from dnd5epy.models.spellcasting import Spellcasting
+
+from dnd5epy.api_client import ApiClient
+from dnd5epy.api_response import ApiResponse
+from dnd5epy.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 
 class ClassApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
```

### Comparing `dnd5epy-1.0.2/dnd5epy/api/class_levels_api.py` & `dnd5epy-1.0.3/dnd5epy/api/class_levels_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,20 +19,20 @@
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
 from pydantic import Field, StrictStr, confloat, conint
 
 from typing import List, Optional, Union
 
-from openapi_client.models.api_reference_list import APIReferenceList
-from openapi_client.models.class_level import ClassLevel
+from dnd5epy.models.api_reference_list import APIReferenceList
+from dnd5epy.models.class_level import ClassLevel
 
-from openapi_client.api_client import ApiClient
-from openapi_client.api_response import ApiResponse
-from openapi_client.exceptions import (  # noqa: F401
+from dnd5epy.api_client import ApiClient
+from dnd5epy.api_response import ApiResponse
+from dnd5epy.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 
 class ClassLevelsApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
```

### Comparing `dnd5epy-1.0.2/dnd5epy/api/class_resource_lists_api.py` & `dnd5epy-1.0.3/dnd5epy/api/class_resource_lists_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,19 +17,19 @@
 import warnings
 
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
 from pydantic import Field, StrictStr
 
-from openapi_client.models.api_reference_list import APIReferenceList
+from dnd5epy.models.api_reference_list import APIReferenceList
 
-from openapi_client.api_client import ApiClient
-from openapi_client.api_response import ApiResponse
-from openapi_client.exceptions import (  # noqa: F401
+from dnd5epy.api_client import ApiClient
+from dnd5epy.api_response import ApiResponse
+from dnd5epy.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 
 class ClassResourceListsApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
```

### Comparing `dnd5epy-1.0.2/dnd5epy/api/common_api.py` & `dnd5epy-1.0.3/dnd5epy/api/common_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,19 +19,19 @@
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
 from pydantic import StrictStr
 
 from typing import Dict
 
-from openapi_client.models.api_reference_list import APIReferenceList
+from dnd5epy.models.api_reference_list import APIReferenceList
 
-from openapi_client.api_client import ApiClient
-from openapi_client.api_response import ApiResponse
-from openapi_client.exceptions import (  # noqa: F401
+from dnd5epy.api_client import ApiClient
+from dnd5epy.api_response import ApiResponse
+from dnd5epy.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 
 class CommonApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
```

### Comparing `dnd5epy-1.0.2/dnd5epy/api/equipment_api.py` & `dnd5epy-1.0.3/dnd5epy/api/equipment_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,22 +17,22 @@
 import warnings
 
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
 from pydantic import Field, StrictStr
 
-from openapi_client.models.equipment import Equipment
-from openapi_client.models.equipment_category import EquipmentCategory
-from openapi_client.models.magic_item import MagicItem
-from openapi_client.models.weapon_property import WeaponProperty
-
-from openapi_client.api_client import ApiClient
-from openapi_client.api_response import ApiResponse
-from openapi_client.exceptions import (  # noqa: F401
+from dnd5epy.models.equipment import Equipment
+from dnd5epy.models.equipment_category import EquipmentCategory
+from dnd5epy.models.magic_item import MagicItem
+from dnd5epy.models.weapon_property import WeaponProperty
+
+from dnd5epy.api_client import ApiClient
+from dnd5epy.api_response import ApiResponse
+from dnd5epy.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 
 class EquipmentApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
```

### Comparing `dnd5epy-1.0.2/dnd5epy/api/feats_api.py` & `dnd5epy-1.0.3/dnd5epy/api/feats_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,19 +17,19 @@
 import warnings
 
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
 from pydantic import Field, StrictStr
 
-from openapi_client.models.feat import Feat
+from dnd5epy.models.feat import Feat
 
-from openapi_client.api_client import ApiClient
-from openapi_client.api_response import ApiResponse
-from openapi_client.exceptions import (  # noqa: F401
+from dnd5epy.api_client import ApiClient
+from dnd5epy.api_response import ApiResponse
+from dnd5epy.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 
 class FeatsApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
```

### Comparing `dnd5epy-1.0.2/dnd5epy/api/features_api.py` & `dnd5epy-1.0.3/dnd5epy/api/features_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,19 +17,19 @@
 import warnings
 
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
 from pydantic import Field, StrictStr
 
-from openapi_client.models.feature import Feature
+from dnd5epy.models.feature import Feature
 
-from openapi_client.api_client import ApiClient
-from openapi_client.api_response import ApiResponse
-from openapi_client.exceptions import (  # noqa: F401
+from dnd5epy.api_client import ApiClient
+from dnd5epy.api_response import ApiResponse
+from dnd5epy.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 
 class FeaturesApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
```

### Comparing `dnd5epy-1.0.2/dnd5epy/api/game_mechanics_api.py` & `dnd5epy-1.0.3/dnd5epy/api/game_mechanics_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,21 +17,21 @@
 import warnings
 
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
 from pydantic import Field, StrictStr
 
-from openapi_client.models.condition import Condition
-from openapi_client.models.damage_type import DamageType
-from openapi_client.models.magic_school import MagicSchool
-
-from openapi_client.api_client import ApiClient
-from openapi_client.api_response import ApiResponse
-from openapi_client.exceptions import (  # noqa: F401
+from dnd5epy.models.condition import Condition
+from dnd5epy.models.damage_type import DamageType
+from dnd5epy.models.magic_school import MagicSchool
+
+from dnd5epy.api_client import ApiClient
+from dnd5epy.api_response import ApiResponse
+from dnd5epy.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 
 class GameMechanicsApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
```

### Comparing `dnd5epy-1.0.2/dnd5epy/api/monsters_api.py` & `dnd5epy-1.0.3/dnd5epy/api/monsters_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,20 +19,20 @@
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
 from pydantic import Field, StrictFloat, StrictInt, StrictStr, conlist
 
 from typing import Optional, Union
 
-from openapi_client.models.api_reference_list import APIReferenceList
-from openapi_client.models.monster import Monster
+from dnd5epy.models.api_reference_list import APIReferenceList
+from dnd5epy.models.monster import Monster
 
-from openapi_client.api_client import ApiClient
-from openapi_client.api_response import ApiResponse
-from openapi_client.exceptions import (  # noqa: F401
+from dnd5epy.api_client import ApiClient
+from dnd5epy.api_response import ApiResponse
+from dnd5epy.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 
 class MonstersApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
```

### Comparing `dnd5epy-1.0.2/dnd5epy/api/races_api.py` & `dnd5epy-1.0.3/dnd5epy/api/races_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,20 +17,20 @@
 import warnings
 
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
 from pydantic import Field, StrictStr
 
-from openapi_client.models.api_reference_list import APIReferenceList
-from openapi_client.models.race import Race
+from dnd5epy.models.api_reference_list import APIReferenceList
+from dnd5epy.models.race import Race
 
-from openapi_client.api_client import ApiClient
-from openapi_client.api_response import ApiResponse
-from openapi_client.exceptions import (  # noqa: F401
+from dnd5epy.api_client import ApiClient
+from dnd5epy.api_response import ApiResponse
+from dnd5epy.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 
 class RacesApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
```

### Comparing `dnd5epy-1.0.2/dnd5epy/api/rules_api.py` & `dnd5epy-1.0.3/dnd5epy/api/rules_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,20 +17,20 @@
 import warnings
 
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
 from pydantic import Field, StrictStr
 
-from openapi_client.models.rule import Rule
-from openapi_client.models.rule_section import RuleSection
+from dnd5epy.models.rule import Rule
+from dnd5epy.models.rule_section import RuleSection
 
-from openapi_client.api_client import ApiClient
-from openapi_client.api_response import ApiResponse
-from openapi_client.exceptions import (  # noqa: F401
+from dnd5epy.api_client import ApiClient
+from dnd5epy.api_response import ApiResponse
+from dnd5epy.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 
 class RulesApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
```

### Comparing `dnd5epy-1.0.2/dnd5epy/api/spells_api.py` & `dnd5epy-1.0.3/dnd5epy/api/spells_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,20 +19,20 @@
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
 from pydantic import Field, StrictInt, StrictStr, conlist
 
 from typing import Optional
 
-from openapi_client.models.api_reference_list import APIReferenceList
-from openapi_client.models.spell import Spell
+from dnd5epy.models.api_reference_list import APIReferenceList
+from dnd5epy.models.spell import Spell
 
-from openapi_client.api_client import ApiClient
-from openapi_client.api_response import ApiResponse
-from openapi_client.exceptions import (  # noqa: F401
+from dnd5epy.api_client import ApiClient
+from dnd5epy.api_response import ApiResponse
+from dnd5epy.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 
 class SpellsApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
```

### Comparing `dnd5epy-1.0.2/dnd5epy/api/subclasses_api.py` & `dnd5epy-1.0.3/dnd5epy/api/subclasses_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,22 +19,22 @@
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
 from pydantic import Field, StrictStr, conint
 
 from typing import List
 
-from openapi_client.models.api_reference_list import APIReferenceList
-from openapi_client.models.subclass import Subclass
-from openapi_client.models.subclass_level import SubclassLevel
-from openapi_client.models.subclass_level_resource import SubclassLevelResource
-
-from openapi_client.api_client import ApiClient
-from openapi_client.api_response import ApiResponse
-from openapi_client.exceptions import (  # noqa: F401
+from dnd5epy.models.api_reference_list import APIReferenceList
+from dnd5epy.models.subclass import Subclass
+from dnd5epy.models.subclass_level import SubclassLevel
+from dnd5epy.models.subclass_level_resource import SubclassLevelResource
+
+from dnd5epy.api_client import ApiClient
+from dnd5epy.api_response import ApiResponse
+from dnd5epy.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 
 class SubclassesApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
```

### Comparing `dnd5epy-1.0.2/dnd5epy/api/subraces_api.py` & `dnd5epy-1.0.3/dnd5epy/api/subraces_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,20 +17,20 @@
 import warnings
 
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
 from pydantic import Field, StrictStr
 
-from openapi_client.models.api_reference_list import APIReferenceList
-from openapi_client.models.subrace import Subrace
+from dnd5epy.models.api_reference_list import APIReferenceList
+from dnd5epy.models.subrace import Subrace
 
-from openapi_client.api_client import ApiClient
-from openapi_client.api_response import ApiResponse
-from openapi_client.exceptions import (  # noqa: F401
+from dnd5epy.api_client import ApiClient
+from dnd5epy.api_response import ApiResponse
+from dnd5epy.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 
 class SubracesApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
```

### Comparing `dnd5epy-1.0.2/dnd5epy/api/traits_api.py` & `dnd5epy-1.0.3/dnd5epy/api/traits_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,19 +17,19 @@
 import warnings
 
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
 from pydantic import Field, StrictStr
 
-from openapi_client.models.trait import Trait
+from dnd5epy.models.trait import Trait
 
-from openapi_client.api_client import ApiClient
-from openapi_client.api_response import ApiResponse
-from openapi_client.exceptions import (  # noqa: F401
+from dnd5epy.api_client import ApiClient
+from dnd5epy.api_response import ApiResponse
+from dnd5epy.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 
 class TraitsApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
```

### Comparing `dnd5epy-1.0.2/dnd5epy/api_client.py` & `dnd5epy-1.0.3/dnd5epy/api_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,19 +20,19 @@
 from multiprocessing.pool import ThreadPool
 import os
 import re
 import tempfile
 
 from urllib.parse import quote
 
-from openapi_client.configuration import Configuration
-from openapi_client.api_response import ApiResponse
-import openapi_client.models
-from openapi_client import rest
-from openapi_client.exceptions import ApiValueError, ApiException
+from dnd5epy.configuration import Configuration
+from dnd5epy.api_response import ApiResponse
+import dnd5epy.models
+from dnd5epy import rest
+from dnd5epy.exceptions import ApiValueError, ApiException
 
 
 class ApiClient(object):
     """Generic API client for OpenAPI client library builds.
 
     OpenAPI generic API client. This client handles the client-
     server communication, and is invariant across implementations. Specifics of
@@ -337,15 +337,15 @@
                 return {k: self.__deserialize(v, sub_kls)
                         for k, v in data.items()}
 
             # convert str to class
             if klass in self.NATIVE_TYPES_MAPPING:
                 klass = self.NATIVE_TYPES_MAPPING[klass]
             else:
-                klass = getattr(openapi_client.models, klass)
+                klass = getattr(dnd5epy.models, klass)
 
         if klass in self.PRIMITIVE_TYPES:
             return self.__deserialize_primitive(data, klass)
         elif klass == object:
             return self.__deserialize_object(data)
         elif klass == datetime.date:
             return self.__deserialize_date(data)
```

### Comparing `dnd5epy-1.0.2/dnd5epy/api_response.py` & `dnd5epy-1.0.3/dnd5epy/api_response.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.2/dnd5epy/configuration.py` & `dnd5epy-1.0.3/dnd5epy/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 import copy
 import logging
 import multiprocessing
 import sys
 import urllib3
 
 import http.client as httplib
-from openapi_client.exceptions import ApiValueError
+from dnd5epy.exceptions import ApiValueError
 
 JSON_SCHEMA_VALIDATION_KEYWORDS = {
     'multipleOf', 'maximum', 'exclusiveMaximum',
     'minimum', 'exclusiveMinimum', 'maxLength',
     'minLength', 'pattern', 'maxItems', 'minItems'
 }
 
@@ -103,15 +103,15 @@
         """
         self.access_token = access_token
         """Access token
         """
         self.logger = {}
         """Logging Settings
         """
-        self.logger["package_logger"] = logging.getLogger("openapi_client")
+        self.logger["package_logger"] = logging.getLogger("dnd5epy")
         self.logger["urllib3_logger"] = logging.getLogger("urllib3")
         self.logger_format = '%(asctime)s %(levelname)s %(message)s'
         """Log format
         """
         self.logger_stream_handler = None
         """Log stream handler
         """
```

### Comparing `dnd5epy-1.0.2/dnd5epy/exceptions.py` & `dnd5epy-1.0.3/dnd5epy/exceptions.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.2/dnd5epy/models/__init__.py` & `dnd5epy-1.0.3/dnd5epy/models/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -10,125 +10,125 @@
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 # import models into model package
-from openapi_client.models.api_reference import APIReference
-from openapi_client.models.api_reference_list import APIReferenceList
-from openapi_client.models.ability_bonus import AbilityBonus
-from openapi_client.models.ability_score import AbilityScore
-from openapi_client.models.alignment import Alignment
-from openapi_client.models.area_of_effect import AreaOfEffect
-from openapi_client.models.armor import Armor
-from openapi_client.models.background import Background
-from openapi_client.models.background_all_of_feature import BackgroundAllOfFeature
-from openapi_client.models.choice import Choice
-from openapi_client.models.class_all_of_starting_equipment import ClassAllOfStartingEquipment
-from openapi_client.models.class_level import ClassLevel
-from openapi_client.models.class_level_class_specific import ClassLevelClassSpecific
-from openapi_client.models.class_level_class_specific_any_of import ClassLevelClassSpecificAnyOf
-from openapi_client.models.class_level_class_specific_any_of1 import ClassLevelClassSpecificAnyOf1
-from openapi_client.models.class_level_class_specific_any_of10 import ClassLevelClassSpecificAnyOf10
-from openapi_client.models.class_level_class_specific_any_of11 import ClassLevelClassSpecificAnyOf11
-from openapi_client.models.class_level_class_specific_any_of2 import ClassLevelClassSpecificAnyOf2
-from openapi_client.models.class_level_class_specific_any_of3 import ClassLevelClassSpecificAnyOf3
-from openapi_client.models.class_level_class_specific_any_of4 import ClassLevelClassSpecificAnyOf4
-from openapi_client.models.class_level_class_specific_any_of5 import ClassLevelClassSpecificAnyOf5
-from openapi_client.models.class_level_class_specific_any_of5_martial_arts import ClassLevelClassSpecificAnyOf5MartialArts
-from openapi_client.models.class_level_class_specific_any_of6 import ClassLevelClassSpecificAnyOf6
-from openapi_client.models.class_level_class_specific_any_of7 import ClassLevelClassSpecificAnyOf7
-from openapi_client.models.class_level_class_specific_any_of8 import ClassLevelClassSpecificAnyOf8
-from openapi_client.models.class_level_class_specific_any_of9 import ClassLevelClassSpecificAnyOf9
-from openapi_client.models.class_level_class_specific_any_of9_creating_spell_slots_inner import ClassLevelClassSpecificAnyOf9CreatingSpellSlotsInner
-from openapi_client.models.condition import Condition
-from openapi_client.models.cost import Cost
-from openapi_client.models.dc import DC
-from openapi_client.models.damage import Damage
-from openapi_client.models.damage_at_character_level import DamageAtCharacterLevel
-from openapi_client.models.damage_at_slot_level import DamageAtSlotLevel
-from openapi_client.models.damage_type import DamageType
-from openapi_client.models.equipment import Equipment
-from openapi_client.models.equipment_category import EquipmentCategory
-from openapi_client.models.equipment_pack import EquipmentPack
-from openapi_client.models.error_response import ErrorResponse
-from openapi_client.models.feat import Feat
-from openapi_client.models.feature import Feature
-from openapi_client.models.feature_all_of_prerequisites_inner import FeatureAllOfPrerequisitesInner
-from openapi_client.models.feature_all_of_prerequisites_inner_any_of import FeatureAllOfPrerequisitesInnerAnyOf
-from openapi_client.models.feature_all_of_prerequisites_inner_any_of1 import FeatureAllOfPrerequisitesInnerAnyOf1
-from openapi_client.models.feature_all_of_prerequisites_inner_any_of2 import FeatureAllOfPrerequisitesInnerAnyOf2
-from openapi_client.models.gear import Gear
-from openapi_client.models.language import Language
-from openapi_client.models.magic_item import MagicItem
-from openapi_client.models.magic_item_all_of_rarity import MagicItemAllOfRarity
-from openapi_client.models.magic_school import MagicSchool
-from openapi_client.models.model_class import ModelClass
-from openapi_client.models.monster import Monster
-from openapi_client.models.monster_ability import MonsterAbility
-from openapi_client.models.monster_action import MonsterAction
-from openapi_client.models.monster_all_of_senses import MonsterAllOfSenses
-from openapi_client.models.monster_all_of_speed import MonsterAllOfSpeed
-from openapi_client.models.monster_armor_class import MonsterArmorClass
-from openapi_client.models.monster_armor_class_one_of import MonsterArmorClassOneOf
-from openapi_client.models.monster_armor_class_one_of1 import MonsterArmorClassOneOf1
-from openapi_client.models.monster_armor_class_one_of2 import MonsterArmorClassOneOf2
-from openapi_client.models.monster_armor_class_one_of3 import MonsterArmorClassOneOf3
-from openapi_client.models.monster_armor_class_one_of4 import MonsterArmorClassOneOf4
-from openapi_client.models.monster_attack import MonsterAttack
-from openapi_client.models.monster_multi_attack_action import MonsterMultiAttackAction
-from openapi_client.models.monster_proficiency import MonsterProficiency
-from openapi_client.models.monster_sense import MonsterSense
-from openapi_client.models.monster_special_ability import MonsterSpecialAbility
-from openapi_client.models.monster_spell import MonsterSpell
-from openapi_client.models.monster_spellcasting import MonsterSpellcasting
-from openapi_client.models.monster_usage import MonsterUsage
-from openapi_client.models.multiclassing import Multiclassing
-from openapi_client.models.option import Option
-from openapi_client.models.option_one_of import OptionOneOf
-from openapi_client.models.option_one_of1 import OptionOneOf1
-from openapi_client.models.option_one_of10 import OptionOneOf10
-from openapi_client.models.option_one_of2 import OptionOneOf2
-from openapi_client.models.option_one_of3 import OptionOneOf3
-from openapi_client.models.option_one_of4 import OptionOneOf4
-from openapi_client.models.option_one_of5 import OptionOneOf5
-from openapi_client.models.option_one_of6 import OptionOneOf6
-from openapi_client.models.option_one_of7 import OptionOneOf7
-from openapi_client.models.option_one_of8 import OptionOneOf8
-from openapi_client.models.option_one_of9 import OptionOneOf9
-from openapi_client.models.option_set import OptionSet
-from openapi_client.models.option_set_one_of import OptionSetOneOf
-from openapi_client.models.option_set_one_of1 import OptionSetOneOf1
-from openapi_client.models.option_set_one_of2 import OptionSetOneOf2
-from openapi_client.models.prerequisite import Prerequisite
-from openapi_client.models.prerequisite_ability_score import PrerequisiteAbilityScore
-from openapi_client.models.proficiency import Proficiency
-from openapi_client.models.proficiency_all_of_reference import ProficiencyAllOfReference
-from openapi_client.models.race import Race
-from openapi_client.models.resource_description import ResourceDescription
-from openapi_client.models.rule import Rule
-from openapi_client.models.rule_section import RuleSection
-from openapi_client.models.skill import Skill
-from openapi_client.models.spell import Spell
-from openapi_client.models.spell_all_of_damage import SpellAllOfDamage
-from openapi_client.models.spell_prerequisite import SpellPrerequisite
-from openapi_client.models.spellcasting import Spellcasting
-from openapi_client.models.spellcasting_info_inner import SpellcastingInfoInner
-from openapi_client.models.spellcasting_spellcasting_ability import SpellcastingSpellcastingAbility
-from openapi_client.models.subclass import Subclass
-from openapi_client.models.subclass_all_of_spells import SubclassAllOfSpells
-from openapi_client.models.subclass_level import SubclassLevel
-from openapi_client.models.subclass_level_resource import SubclassLevelResource
-from openapi_client.models.subclass_level_spellcasting import SubclassLevelSpellcasting
-from openapi_client.models.subrace import Subrace
-from openapi_client.models.subrace_all_of_race import SubraceAllOfRace
-from openapi_client.models.trait import Trait
-from openapi_client.models.trait_all_of_trait_specific import TraitAllOfTraitSpecific
-from openapi_client.models.trait_all_of_trait_specific_one_of import TraitAllOfTraitSpecificOneOf
-from openapi_client.models.trait_all_of_trait_specific_one_of_breath_weapon import TraitAllOfTraitSpecificOneOfBreathWeapon
-from openapi_client.models.trait_all_of_trait_specific_one_of_breath_weapon_damage import TraitAllOfTraitSpecificOneOfBreathWeaponDamage
-from openapi_client.models.trait_all_of_trait_specific_one_of_breath_weapon_usage import TraitAllOfTraitSpecificOneOfBreathWeaponUsage
-from openapi_client.models.trait_all_of_trait_specific_one_of_damage_type import TraitAllOfTraitSpecificOneOfDamageType
-from openapi_client.models.weapon import Weapon
-from openapi_client.models.weapon_all_of_range import WeaponAllOfRange
-from openapi_client.models.weapon_property import WeaponProperty
+from dnd5epy.models.api_reference import APIReference
+from dnd5epy.models.api_reference_list import APIReferenceList
+from dnd5epy.models.ability_bonus import AbilityBonus
+from dnd5epy.models.ability_score import AbilityScore
+from dnd5epy.models.alignment import Alignment
+from dnd5epy.models.area_of_effect import AreaOfEffect
+from dnd5epy.models.armor import Armor
+from dnd5epy.models.background import Background
+from dnd5epy.models.background_all_of_feature import BackgroundAllOfFeature
+from dnd5epy.models.choice import Choice
+from dnd5epy.models.class_all_of_starting_equipment import ClassAllOfStartingEquipment
+from dnd5epy.models.class_level import ClassLevel
+from dnd5epy.models.class_level_class_specific import ClassLevelClassSpecific
+from dnd5epy.models.class_level_class_specific_any_of import ClassLevelClassSpecificAnyOf
+from dnd5epy.models.class_level_class_specific_any_of1 import ClassLevelClassSpecificAnyOf1
+from dnd5epy.models.class_level_class_specific_any_of10 import ClassLevelClassSpecificAnyOf10
+from dnd5epy.models.class_level_class_specific_any_of11 import ClassLevelClassSpecificAnyOf11
+from dnd5epy.models.class_level_class_specific_any_of2 import ClassLevelClassSpecificAnyOf2
+from dnd5epy.models.class_level_class_specific_any_of3 import ClassLevelClassSpecificAnyOf3
+from dnd5epy.models.class_level_class_specific_any_of4 import ClassLevelClassSpecificAnyOf4
+from dnd5epy.models.class_level_class_specific_any_of5 import ClassLevelClassSpecificAnyOf5
+from dnd5epy.models.class_level_class_specific_any_of5_martial_arts import ClassLevelClassSpecificAnyOf5MartialArts
+from dnd5epy.models.class_level_class_specific_any_of6 import ClassLevelClassSpecificAnyOf6
+from dnd5epy.models.class_level_class_specific_any_of7 import ClassLevelClassSpecificAnyOf7
+from dnd5epy.models.class_level_class_specific_any_of8 import ClassLevelClassSpecificAnyOf8
+from dnd5epy.models.class_level_class_specific_any_of9 import ClassLevelClassSpecificAnyOf9
+from dnd5epy.models.class_level_class_specific_any_of9_creating_spell_slots_inner import ClassLevelClassSpecificAnyOf9CreatingSpellSlotsInner
+from dnd5epy.models.condition import Condition
+from dnd5epy.models.cost import Cost
+from dnd5epy.models.dc import DC
+from dnd5epy.models.damage import Damage
+from dnd5epy.models.damage_at_character_level import DamageAtCharacterLevel
+from dnd5epy.models.damage_at_slot_level import DamageAtSlotLevel
+from dnd5epy.models.damage_type import DamageType
+from dnd5epy.models.equipment import Equipment
+from dnd5epy.models.equipment_category import EquipmentCategory
+from dnd5epy.models.equipment_pack import EquipmentPack
+from dnd5epy.models.error_response import ErrorResponse
+from dnd5epy.models.feat import Feat
+from dnd5epy.models.feature import Feature
+from dnd5epy.models.feature_all_of_prerequisites_inner import FeatureAllOfPrerequisitesInner
+from dnd5epy.models.feature_all_of_prerequisites_inner_any_of import FeatureAllOfPrerequisitesInnerAnyOf
+from dnd5epy.models.feature_all_of_prerequisites_inner_any_of1 import FeatureAllOfPrerequisitesInnerAnyOf1
+from dnd5epy.models.feature_all_of_prerequisites_inner_any_of2 import FeatureAllOfPrerequisitesInnerAnyOf2
+from dnd5epy.models.gear import Gear
+from dnd5epy.models.language import Language
+from dnd5epy.models.magic_item import MagicItem
+from dnd5epy.models.magic_item_all_of_rarity import MagicItemAllOfRarity
+from dnd5epy.models.magic_school import MagicSchool
+from dnd5epy.models.model_class import ModelClass
+from dnd5epy.models.monster import Monster
+from dnd5epy.models.monster_ability import MonsterAbility
+from dnd5epy.models.monster_action import MonsterAction
+from dnd5epy.models.monster_all_of_senses import MonsterAllOfSenses
+from dnd5epy.models.monster_all_of_speed import MonsterAllOfSpeed
+from dnd5epy.models.monster_armor_class import MonsterArmorClass
+from dnd5epy.models.monster_armor_class_one_of import MonsterArmorClassOneOf
+from dnd5epy.models.monster_armor_class_one_of1 import MonsterArmorClassOneOf1
+from dnd5epy.models.monster_armor_class_one_of2 import MonsterArmorClassOneOf2
+from dnd5epy.models.monster_armor_class_one_of3 import MonsterArmorClassOneOf3
+from dnd5epy.models.monster_armor_class_one_of4 import MonsterArmorClassOneOf4
+from dnd5epy.models.monster_attack import MonsterAttack
+from dnd5epy.models.monster_multi_attack_action import MonsterMultiAttackAction
+from dnd5epy.models.monster_proficiency import MonsterProficiency
+from dnd5epy.models.monster_sense import MonsterSense
+from dnd5epy.models.monster_special_ability import MonsterSpecialAbility
+from dnd5epy.models.monster_spell import MonsterSpell
+from dnd5epy.models.monster_spellcasting import MonsterSpellcasting
+from dnd5epy.models.monster_usage import MonsterUsage
+from dnd5epy.models.multiclassing import Multiclassing
+from dnd5epy.models.option import Option
+from dnd5epy.models.option_one_of import OptionOneOf
+from dnd5epy.models.option_one_of1 import OptionOneOf1
+from dnd5epy.models.option_one_of10 import OptionOneOf10
+from dnd5epy.models.option_one_of2 import OptionOneOf2
+from dnd5epy.models.option_one_of3 import OptionOneOf3
+from dnd5epy.models.option_one_of4 import OptionOneOf4
+from dnd5epy.models.option_one_of5 import OptionOneOf5
+from dnd5epy.models.option_one_of6 import OptionOneOf6
+from dnd5epy.models.option_one_of7 import OptionOneOf7
+from dnd5epy.models.option_one_of8 import OptionOneOf8
+from dnd5epy.models.option_one_of9 import OptionOneOf9
+from dnd5epy.models.option_set import OptionSet
+from dnd5epy.models.option_set_one_of import OptionSetOneOf
+from dnd5epy.models.option_set_one_of1 import OptionSetOneOf1
+from dnd5epy.models.option_set_one_of2 import OptionSetOneOf2
+from dnd5epy.models.prerequisite import Prerequisite
+from dnd5epy.models.prerequisite_ability_score import PrerequisiteAbilityScore
+from dnd5epy.models.proficiency import Proficiency
+from dnd5epy.models.proficiency_all_of_reference import ProficiencyAllOfReference
+from dnd5epy.models.race import Race
+from dnd5epy.models.resource_description import ResourceDescription
+from dnd5epy.models.rule import Rule
+from dnd5epy.models.rule_section import RuleSection
+from dnd5epy.models.skill import Skill
+from dnd5epy.models.spell import Spell
+from dnd5epy.models.spell_all_of_damage import SpellAllOfDamage
+from dnd5epy.models.spell_prerequisite import SpellPrerequisite
+from dnd5epy.models.spellcasting import Spellcasting
+from dnd5epy.models.spellcasting_info_inner import SpellcastingInfoInner
+from dnd5epy.models.spellcasting_spellcasting_ability import SpellcastingSpellcastingAbility
+from dnd5epy.models.subclass import Subclass
+from dnd5epy.models.subclass_all_of_spells import SubclassAllOfSpells
+from dnd5epy.models.subclass_level import SubclassLevel
+from dnd5epy.models.subclass_level_resource import SubclassLevelResource
+from dnd5epy.models.subclass_level_spellcasting import SubclassLevelSpellcasting
+from dnd5epy.models.subrace import Subrace
+from dnd5epy.models.subrace_all_of_race import SubraceAllOfRace
+from dnd5epy.models.trait import Trait
+from dnd5epy.models.trait_all_of_trait_specific import TraitAllOfTraitSpecific
+from dnd5epy.models.trait_all_of_trait_specific_one_of import TraitAllOfTraitSpecificOneOf
+from dnd5epy.models.trait_all_of_trait_specific_one_of_breath_weapon import TraitAllOfTraitSpecificOneOfBreathWeapon
+from dnd5epy.models.trait_all_of_trait_specific_one_of_breath_weapon_damage import TraitAllOfTraitSpecificOneOfBreathWeaponDamage
+from dnd5epy.models.trait_all_of_trait_specific_one_of_breath_weapon_usage import TraitAllOfTraitSpecificOneOfBreathWeaponUsage
+from dnd5epy.models.trait_all_of_trait_specific_one_of_damage_type import TraitAllOfTraitSpecificOneOfDamageType
+from dnd5epy.models.weapon import Weapon
+from dnd5epy.models.weapon_all_of_range import WeaponAllOfRange
+from dnd5epy.models.weapon_property import WeaponProperty
```

### Comparing `dnd5epy-1.0.2/dnd5epy/models/ability_bonus.py` & `dnd5epy-1.0.3/dnd5epy/models/ability_bonus.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional, Union
 from pydantic import BaseModel, Field, StrictFloat, StrictInt
-from openapi_client.models.api_reference import APIReference
+from dnd5epy.models.api_reference import APIReference
 
 class AbilityBonus(BaseModel):
     """
     AbilityBonus
     """
     bonus: Optional[Union[StrictFloat, StrictInt]] = Field(None, description="Bonus amount for this ability score.")
     ability_score: Optional[APIReference] = None
```

### Comparing `dnd5epy-1.0.2/dnd5epy/models/ability_score.py` & `dnd5epy-1.0.3/dnd5epy/models/ability_score.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List, Optional
 from pydantic import BaseModel, Field, StrictStr, conlist
-from openapi_client.models.api_reference import APIReference
+from dnd5epy.models.api_reference import APIReference
 
 class AbilityScore(BaseModel):
     """
     `AbilityScore` 
     """
     index: Optional[StrictStr] = Field(None, description="Resource index for shorthand searching.")
     name: Optional[StrictStr] = Field(None, description="Name of the referenced resource.")
```

### Comparing `dnd5epy-1.0.2/dnd5epy/models/alignment.py` & `dnd5epy-1.0.3/dnd5epy/models/alignment.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.2/dnd5epy/models/api_reference.py` & `dnd5epy-1.0.3/dnd5epy/models/api_reference.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.2/dnd5epy/models/api_reference_list.py` & `dnd5epy-1.0.3/dnd5epy/models/api_reference_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List, Optional, Union
 from pydantic import BaseModel, Field, StrictFloat, StrictInt, conlist
-from openapi_client.models.api_reference import APIReference
+from dnd5epy.models.api_reference import APIReference
 
 class APIReferenceList(BaseModel):
     """
     `APIReferenceList` 
     """
     count: Optional[Union[StrictFloat, StrictInt]] = Field(None, description="Total number of resources available.")
     results: Optional[conlist(APIReference)] = None
```

### Comparing `dnd5epy-1.0.2/dnd5epy/models/area_of_effect.py` & `dnd5epy-1.0.3/dnd5epy/models/area_of_effect.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.2/dnd5epy/models/armor.py` & `dnd5epy-1.0.3/dnd5epy/models/armor.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Dict, List, Optional, Union
 from pydantic import BaseModel, Field, StrictBool, StrictFloat, StrictInt, StrictStr, conlist
-from openapi_client.models.api_reference import APIReference
-from openapi_client.models.cost import Cost
+from dnd5epy.models.api_reference import APIReference
+from dnd5epy.models.cost import Cost
 
 class Armor(BaseModel):
     """
     `Armor` 
     """
     index: Optional[StrictStr] = Field(None, description="Resource index for shorthand searching.")
     name: Optional[StrictStr] = Field(None, description="Name of the referenced resource.")
```

### Comparing `dnd5epy-1.0.2/dnd5epy/models/background.py` & `dnd5epy-1.0.3/dnd5epy/models/background.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,17 +16,17 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, List, Optional
 from pydantic import BaseModel, Field, StrictStr, conlist
-from openapi_client.models.api_reference import APIReference
-from openapi_client.models.background_all_of_feature import BackgroundAllOfFeature
-from openapi_client.models.choice import Choice
+from dnd5epy.models.api_reference import APIReference
+from dnd5epy.models.background_all_of_feature import BackgroundAllOfFeature
+from dnd5epy.models.choice import Choice
 
 class Background(BaseModel):
     """
     `Background` 
     """
     index: Optional[StrictStr] = Field(None, description="Resource index for shorthand searching.")
     name: Optional[StrictStr] = Field(None, description="Name of the referenced resource.")
```

### Comparing `dnd5epy-1.0.2/dnd5epy/models/background_all_of_feature.py` & `dnd5epy-1.0.3/dnd5epy/models/background_all_of_feature.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.2/dnd5epy/models/choice.py` & `dnd5epy-1.0.3/dnd5epy/models/choice.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.2/dnd5epy/models/class_all_of_starting_equipment.py` & `dnd5epy-1.0.3/dnd5epy/models/class_all_of_starting_equipment.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional, Union
 from pydantic import BaseModel, StrictFloat, StrictInt
-from openapi_client.models.api_reference import APIReference
+from dnd5epy.models.api_reference import APIReference
 
 class ClassAllOfStartingEquipment(BaseModel):
     """
     ClassAllOfStartingEquipment
     """
     quantity: Optional[Union[StrictFloat, StrictInt]] = None
     equipment: Optional[APIReference] = None
```

### Comparing `dnd5epy-1.0.2/dnd5epy/models/class_level.py` & `dnd5epy-1.0.3/dnd5epy/models/class_level.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,17 +16,17 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List, Optional, Union
 from pydantic import BaseModel, Field, StrictFloat, StrictInt, StrictStr, conlist
-from openapi_client.models.api_reference import APIReference
-from openapi_client.models.class_level_class_specific import ClassLevelClassSpecific
-from openapi_client.models.subclass_level_spellcasting import SubclassLevelSpellcasting
+from dnd5epy.models.api_reference import APIReference
+from dnd5epy.models.class_level_class_specific import ClassLevelClassSpecific
+from dnd5epy.models.subclass_level_spellcasting import SubclassLevelSpellcasting
 
 class ClassLevel(BaseModel):
     """
     `ClassLevel` 
     """
     index: Optional[StrictStr] = Field(None, description="Resource index for shorthand searching.")
     url: Optional[StrictStr] = Field(None, description="URL of the referenced resource.")
```

### Comparing `dnd5epy-1.0.2/dnd5epy/models/class_level_class_specific.py` & `dnd5epy-1.0.3/dnd5epy/models/class_level_class_specific.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,26 +16,26 @@
 from inspect import getfullargspec
 import json
 import pprint
 import re  # noqa: F401
 
 from typing import Optional
 from pydantic import BaseModel, Field, StrictStr, ValidationError, validator
-from openapi_client.models.class_level_class_specific_any_of import ClassLevelClassSpecificAnyOf
-from openapi_client.models.class_level_class_specific_any_of1 import ClassLevelClassSpecificAnyOf1
-from openapi_client.models.class_level_class_specific_any_of10 import ClassLevelClassSpecificAnyOf10
-from openapi_client.models.class_level_class_specific_any_of11 import ClassLevelClassSpecificAnyOf11
-from openapi_client.models.class_level_class_specific_any_of2 import ClassLevelClassSpecificAnyOf2
-from openapi_client.models.class_level_class_specific_any_of3 import ClassLevelClassSpecificAnyOf3
-from openapi_client.models.class_level_class_specific_any_of4 import ClassLevelClassSpecificAnyOf4
-from openapi_client.models.class_level_class_specific_any_of5 import ClassLevelClassSpecificAnyOf5
-from openapi_client.models.class_level_class_specific_any_of6 import ClassLevelClassSpecificAnyOf6
-from openapi_client.models.class_level_class_specific_any_of7 import ClassLevelClassSpecificAnyOf7
-from openapi_client.models.class_level_class_specific_any_of8 import ClassLevelClassSpecificAnyOf8
-from openapi_client.models.class_level_class_specific_any_of9 import ClassLevelClassSpecificAnyOf9
+from dnd5epy.models.class_level_class_specific_any_of import ClassLevelClassSpecificAnyOf
+from dnd5epy.models.class_level_class_specific_any_of1 import ClassLevelClassSpecificAnyOf1
+from dnd5epy.models.class_level_class_specific_any_of10 import ClassLevelClassSpecificAnyOf10
+from dnd5epy.models.class_level_class_specific_any_of11 import ClassLevelClassSpecificAnyOf11
+from dnd5epy.models.class_level_class_specific_any_of2 import ClassLevelClassSpecificAnyOf2
+from dnd5epy.models.class_level_class_specific_any_of3 import ClassLevelClassSpecificAnyOf3
+from dnd5epy.models.class_level_class_specific_any_of4 import ClassLevelClassSpecificAnyOf4
+from dnd5epy.models.class_level_class_specific_any_of5 import ClassLevelClassSpecificAnyOf5
+from dnd5epy.models.class_level_class_specific_any_of6 import ClassLevelClassSpecificAnyOf6
+from dnd5epy.models.class_level_class_specific_any_of7 import ClassLevelClassSpecificAnyOf7
+from dnd5epy.models.class_level_class_specific_any_of8 import ClassLevelClassSpecificAnyOf8
+from dnd5epy.models.class_level_class_specific_any_of9 import ClassLevelClassSpecificAnyOf9
 from typing import Any, List
 from pydantic import StrictStr, Field
 
 CLASSLEVELCLASSSPECIFIC_ANY_OF_SCHEMAS = ["ClassLevelClassSpecificAnyOf", "ClassLevelClassSpecificAnyOf1", "ClassLevelClassSpecificAnyOf10", "ClassLevelClassSpecificAnyOf11", "ClassLevelClassSpecificAnyOf2", "ClassLevelClassSpecificAnyOf3", "ClassLevelClassSpecificAnyOf4", "ClassLevelClassSpecificAnyOf5", "ClassLevelClassSpecificAnyOf6", "ClassLevelClassSpecificAnyOf7", "ClassLevelClassSpecificAnyOf8", "ClassLevelClassSpecificAnyOf9"]
 
 class ClassLevelClassSpecific(BaseModel):
     """
```

### Comparing `dnd5epy-1.0.2/dnd5epy/models/class_level_class_specific_any_of.py` & `dnd5epy-1.0.3/dnd5epy/models/class_level_class_specific_any_of.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.2/dnd5epy/models/class_level_class_specific_any_of1.py` & `dnd5epy-1.0.3/dnd5epy/models/class_level_class_specific_any_of1.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.2/dnd5epy/models/class_level_class_specific_any_of10.py` & `dnd5epy-1.0.3/dnd5epy/models/class_level_class_specific_any_of10.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.2/dnd5epy/models/class_level_class_specific_any_of11.py` & `dnd5epy-1.0.3/dnd5epy/models/class_level_class_specific_any_of11.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.2/dnd5epy/models/class_level_class_specific_any_of2.py` & `dnd5epy-1.0.3/dnd5epy/models/class_level_class_specific_any_of2.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.2/dnd5epy/models/class_level_class_specific_any_of3.py` & `dnd5epy-1.0.3/dnd5epy/models/class_level_class_specific_any_of3.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.2/dnd5epy/models/class_level_class_specific_any_of4.py` & `dnd5epy-1.0.3/dnd5epy/models/class_level_class_specific_any_of4.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.2/dnd5epy/models/class_level_class_specific_any_of5.py` & `dnd5epy-1.0.3/dnd5epy/models/class_level_class_specific_any_of5.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional, Union
 from pydantic import BaseModel, StrictFloat, StrictInt
-from openapi_client.models.class_level_class_specific_any_of5_martial_arts import ClassLevelClassSpecificAnyOf5MartialArts
+from dnd5epy.models.class_level_class_specific_any_of5_martial_arts import ClassLevelClassSpecificAnyOf5MartialArts
 
 class ClassLevelClassSpecificAnyOf5(BaseModel):
     """
     Monk Class Specific Features
     """
     ki_points: Optional[Union[StrictFloat, StrictInt]] = None
     unarmored_movement: Optional[Union[StrictFloat, StrictInt]] = None
```

### Comparing `dnd5epy-1.0.2/dnd5epy/models/class_level_class_specific_any_of5_martial_arts.py` & `dnd5epy-1.0.3/dnd5epy/models/class_level_class_specific_any_of5_martial_arts.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.2/dnd5epy/models/class_level_class_specific_any_of6.py` & `dnd5epy-1.0.3/dnd5epy/models/class_level_class_specific_any_of6.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.2/dnd5epy/models/class_level_class_specific_any_of7.py` & `dnd5epy-1.0.3/dnd5epy/models/class_level_class_specific_any_of7.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.2/dnd5epy/models/class_level_class_specific_any_of8.py` & `dnd5epy-1.0.3/dnd5epy/models/class_level_class_specific_any_of8.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
 from pydantic import BaseModel
-from openapi_client.models.class_level_class_specific_any_of5_martial_arts import ClassLevelClassSpecificAnyOf5MartialArts
+from dnd5epy.models.class_level_class_specific_any_of5_martial_arts import ClassLevelClassSpecificAnyOf5MartialArts
 
 class ClassLevelClassSpecificAnyOf8(BaseModel):
     """
     Bard Rogue Specific Features
     """
     sneak_attack: Optional[ClassLevelClassSpecificAnyOf5MartialArts] = None
     __properties = ["sneak_attack"]
```

### Comparing `dnd5epy-1.0.2/dnd5epy/models/class_level_class_specific_any_of9.py` & `dnd5epy-1.0.3/dnd5epy/models/class_level_class_specific_any_of9.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List, Optional, Union
 from pydantic import BaseModel, StrictFloat, StrictInt, conlist
-from openapi_client.models.class_level_class_specific_any_of9_creating_spell_slots_inner import ClassLevelClassSpecificAnyOf9CreatingSpellSlotsInner
+from dnd5epy.models.class_level_class_specific_any_of9_creating_spell_slots_inner import ClassLevelClassSpecificAnyOf9CreatingSpellSlotsInner
 
 class ClassLevelClassSpecificAnyOf9(BaseModel):
     """
     Bard Sorcerer Specific Features
     """
     sorcery_points: Optional[Union[StrictFloat, StrictInt]] = None
     metamagic_known: Optional[Union[StrictFloat, StrictInt]] = None
```

### Comparing `dnd5epy-1.0.2/dnd5epy/models/class_level_class_specific_any_of9_creating_spell_slots_inner.py` & `dnd5epy-1.0.3/dnd5epy/models/class_level_class_specific_any_of9_creating_spell_slots_inner.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.2/dnd5epy/models/condition.py` & `dnd5epy-1.0.3/dnd5epy/models/condition.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.2/dnd5epy/models/cost.py` & `dnd5epy-1.0.3/dnd5epy/models/cost.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.2/dnd5epy/models/damage.py` & `dnd5epy-1.0.3/dnd5epy/models/damage.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
 from pydantic import BaseModel, StrictStr
-from openapi_client.models.api_reference import APIReference
+from dnd5epy.models.api_reference import APIReference
 
 class Damage(BaseModel):
     """
     `Damage` 
     """
     damage_dice: Optional[StrictStr] = None
     damage_type: Optional[APIReference] = None
```

### Comparing `dnd5epy-1.0.2/dnd5epy/models/damage_at_character_level.py` & `dnd5epy-1.0.3/dnd5epy/models/damage_at_character_level.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, Optional
 from pydantic import BaseModel
-from openapi_client.models.api_reference import APIReference
+from dnd5epy.models.api_reference import APIReference
 
 class DamageAtCharacterLevel(BaseModel):
     """
     'Spell Damage' 
     """
     damage_at_character_level: Optional[Dict[str, Any]] = None
     damage_type: Optional[APIReference] = None
```

### Comparing `dnd5epy-1.0.2/dnd5epy/models/damage_at_slot_level.py` & `dnd5epy-1.0.3/dnd5epy/models/damage_at_slot_level.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, Optional
 from pydantic import BaseModel
-from openapi_client.models.api_reference import APIReference
+from dnd5epy.models.api_reference import APIReference
 
 class DamageAtSlotLevel(BaseModel):
     """
     'Spell Damage' 
     """
     damage_at_slot_level: Optional[Dict[str, Any]] = None
     damage_type: Optional[APIReference] = None
```

### Comparing `dnd5epy-1.0.2/dnd5epy/models/damage_type.py` & `dnd5epy-1.0.3/dnd5epy/models/damage_type.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.2/dnd5epy/models/dc.py` & `dnd5epy-1.0.3/dnd5epy/models/dc.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional, Union
 from pydantic import BaseModel, Field, StrictFloat, StrictInt, StrictStr
-from openapi_client.models.api_reference import APIReference
+from dnd5epy.models.api_reference import APIReference
 
 class DC(BaseModel):
     """
     `DC` 
     """
     dc_type: Optional[APIReference] = None
     dc_value: Optional[Union[StrictFloat, StrictInt]] = Field(None, description="Value to beat")
```

### Comparing `dnd5epy-1.0.2/dnd5epy/models/equipment.py` & `dnd5epy-1.0.3/dnd5epy/models/equipment.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 from inspect import getfullargspec
 import json
 import pprint
 import re  # noqa: F401
 
 from typing import Optional
 from pydantic import BaseModel, Field, StrictStr, ValidationError, validator
-from openapi_client.models.armor import Armor
-from openapi_client.models.equipment_pack import EquipmentPack
-from openapi_client.models.gear import Gear
-from openapi_client.models.weapon import Weapon
+from dnd5epy.models.armor import Armor
+from dnd5epy.models.equipment_pack import EquipmentPack
+from dnd5epy.models.gear import Gear
+from dnd5epy.models.weapon import Weapon
 from typing import Any, List
 from pydantic import StrictStr, Field
 
 EQUIPMENT_ANY_OF_SCHEMAS = ["Armor", "EquipmentPack", "Gear", "Weapon"]
 
 class Equipment(BaseModel):
     """
```

### Comparing `dnd5epy-1.0.2/dnd5epy/models/equipment_category.py` & `dnd5epy-1.0.3/dnd5epy/models/equipment_category.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List, Optional
 from pydantic import BaseModel, Field, StrictStr, conlist
-from openapi_client.models.api_reference import APIReference
+from dnd5epy.models.api_reference import APIReference
 
 class EquipmentCategory(BaseModel):
     """
     `EquipmentCategory` 
     """
     index: Optional[StrictStr] = Field(None, description="Resource index for shorthand searching.")
     name: Optional[StrictStr] = Field(None, description="Name of the referenced resource.")
```

### Comparing `dnd5epy-1.0.2/dnd5epy/models/equipment_pack.py` & `dnd5epy-1.0.3/dnd5epy/models/equipment_pack.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List, Optional
 from pydantic import BaseModel, Field, StrictStr, conlist
-from openapi_client.models.api_reference import APIReference
-from openapi_client.models.cost import Cost
+from dnd5epy.models.api_reference import APIReference
+from dnd5epy.models.cost import Cost
 
 class EquipmentPack(BaseModel):
     """
     `EquipmentPack` 
     """
     index: Optional[StrictStr] = Field(None, description="Resource index for shorthand searching.")
     name: Optional[StrictStr] = Field(None, description="Name of the referenced resource.")
```

### Comparing `dnd5epy-1.0.2/dnd5epy/models/error_response.py` & `dnd5epy-1.0.3/dnd5epy/models/error_response.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.2/dnd5epy/models/feat.py` & `dnd5epy-1.0.3/dnd5epy/models/feat.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List, Optional
 from pydantic import BaseModel, Field, StrictStr, conlist
-from openapi_client.models.prerequisite import Prerequisite
+from dnd5epy.models.prerequisite import Prerequisite
 
 class Feat(BaseModel):
     """
     `Feat` 
     """
     index: Optional[StrictStr] = Field(None, description="Resource index for shorthand searching.")
     name: Optional[StrictStr] = Field(None, description="Name of the referenced resource.")
```

### Comparing `dnd5epy-1.0.2/dnd5epy/models/feature.py` & `dnd5epy-1.0.3/dnd5epy/models/feature.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, List, Optional, Union
 from pydantic import BaseModel, Field, StrictFloat, StrictInt, StrictStr, conlist
-from openapi_client.models.api_reference import APIReference
-from openapi_client.models.feature_all_of_prerequisites_inner import FeatureAllOfPrerequisitesInner
+from dnd5epy.models.api_reference import APIReference
+from dnd5epy.models.feature_all_of_prerequisites_inner import FeatureAllOfPrerequisitesInner
 
 class Feature(BaseModel):
     """
     `Feature` 
     """
     index: Optional[StrictStr] = Field(None, description="Resource index for shorthand searching.")
     name: Optional[StrictStr] = Field(None, description="Name of the referenced resource.")
```

### Comparing `dnd5epy-1.0.2/dnd5epy/models/feature_all_of_prerequisites_inner.py` & `dnd5epy-1.0.3/dnd5epy/models/feature_all_of_prerequisites_inner.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,17 +16,17 @@
 from inspect import getfullargspec
 import json
 import pprint
 import re  # noqa: F401
 
 from typing import Optional
 from pydantic import BaseModel, Field, StrictStr, ValidationError, validator
-from openapi_client.models.feature_all_of_prerequisites_inner_any_of import FeatureAllOfPrerequisitesInnerAnyOf
-from openapi_client.models.feature_all_of_prerequisites_inner_any_of1 import FeatureAllOfPrerequisitesInnerAnyOf1
-from openapi_client.models.feature_all_of_prerequisites_inner_any_of2 import FeatureAllOfPrerequisitesInnerAnyOf2
+from dnd5epy.models.feature_all_of_prerequisites_inner_any_of import FeatureAllOfPrerequisitesInnerAnyOf
+from dnd5epy.models.feature_all_of_prerequisites_inner_any_of1 import FeatureAllOfPrerequisitesInnerAnyOf1
+from dnd5epy.models.feature_all_of_prerequisites_inner_any_of2 import FeatureAllOfPrerequisitesInnerAnyOf2
 from typing import Any, List
 from pydantic import StrictStr, Field
 
 FEATUREALLOFPREREQUISITESINNER_ANY_OF_SCHEMAS = ["FeatureAllOfPrerequisitesInnerAnyOf", "FeatureAllOfPrerequisitesInnerAnyOf1", "FeatureAllOfPrerequisitesInnerAnyOf2"]
 
 class FeatureAllOfPrerequisitesInner(BaseModel):
     """
```

### Comparing `dnd5epy-1.0.2/dnd5epy/models/feature_all_of_prerequisites_inner_any_of.py` & `dnd5epy-1.0.3/dnd5epy/models/feature_all_of_prerequisites_inner_any_of.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.2/dnd5epy/models/feature_all_of_prerequisites_inner_any_of1.py` & `dnd5epy-1.0.3/dnd5epy/models/feature_all_of_prerequisites_inner_any_of1.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.2/dnd5epy/models/feature_all_of_prerequisites_inner_any_of2.py` & `dnd5epy-1.0.3/dnd5epy/models/feature_all_of_prerequisites_inner_any_of2.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.2/dnd5epy/models/gear.py` & `dnd5epy-1.0.3/dnd5epy/models/gear.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List, Optional, Union
 from pydantic import BaseModel, Field, StrictFloat, StrictInt, StrictStr, conlist
-from openapi_client.models.api_reference import APIReference
-from openapi_client.models.cost import Cost
+from dnd5epy.models.api_reference import APIReference
+from dnd5epy.models.cost import Cost
 
 class Gear(BaseModel):
     """
     `Gear` 
     """
     index: Optional[StrictStr] = Field(None, description="Resource index for shorthand searching.")
     name: Optional[StrictStr] = Field(None, description="Name of the referenced resource.")
```

### Comparing `dnd5epy-1.0.2/dnd5epy/models/language.py` & `dnd5epy-1.0.3/dnd5epy/models/language.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.2/dnd5epy/models/magic_item.py` & `dnd5epy-1.0.3/dnd5epy/models/magic_item.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List, Optional
 from pydantic import BaseModel, Field, StrictBool, StrictStr, conlist
-from openapi_client.models.api_reference import APIReference
-from openapi_client.models.magic_item_all_of_rarity import MagicItemAllOfRarity
+from dnd5epy.models.api_reference import APIReference
+from dnd5epy.models.magic_item_all_of_rarity import MagicItemAllOfRarity
 
 class MagicItem(BaseModel):
     """
     `MagicItem` 
     """
     index: Optional[StrictStr] = Field(None, description="Resource index for shorthand searching.")
     name: Optional[StrictStr] = Field(None, description="Name of the referenced resource.")
```

### Comparing `dnd5epy-1.0.2/dnd5epy/models/magic_item_all_of_rarity.py` & `dnd5epy-1.0.3/dnd5epy/models/magic_item_all_of_rarity.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.2/dnd5epy/models/magic_school.py` & `dnd5epy-1.0.3/dnd5epy/models/magic_school.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.2/dnd5epy/models/model_class.py` & `dnd5epy-1.0.3/dnd5epy/models/model_class.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,19 +16,19 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List, Optional, Union
 from pydantic import BaseModel, Field, StrictFloat, StrictInt, StrictStr, conlist
-from openapi_client.models.api_reference import APIReference
-from openapi_client.models.choice import Choice
-from openapi_client.models.class_all_of_starting_equipment import ClassAllOfStartingEquipment
-from openapi_client.models.multiclassing import Multiclassing
-from openapi_client.models.spellcasting import Spellcasting
+from dnd5epy.models.api_reference import APIReference
+from dnd5epy.models.choice import Choice
+from dnd5epy.models.class_all_of_starting_equipment import ClassAllOfStartingEquipment
+from dnd5epy.models.multiclassing import Multiclassing
+from dnd5epy.models.spellcasting import Spellcasting
 
 class ModelClass(BaseModel):
     """
     `Class` 
     """
     index: Optional[StrictStr] = Field(None, description="Resource index for shorthand searching.")
     name: Optional[StrictStr] = Field(None, description="Name of the referenced resource.")
```

### Comparing `dnd5epy-1.0.2/dnd5epy/models/monster.py` & `dnd5epy-1.0.3/dnd5epy/models/monster.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,21 +16,21 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List, Optional, Union
 from pydantic import BaseModel, Field, StrictFloat, StrictInt, StrictStr, confloat, conint, conlist, validator
-from openapi_client.models.api_reference import APIReference
-from openapi_client.models.monster_action import MonsterAction
-from openapi_client.models.monster_all_of_senses import MonsterAllOfSenses
-from openapi_client.models.monster_all_of_speed import MonsterAllOfSpeed
-from openapi_client.models.monster_armor_class import MonsterArmorClass
-from openapi_client.models.monster_proficiency import MonsterProficiency
-from openapi_client.models.monster_special_ability import MonsterSpecialAbility
+from dnd5epy.models.api_reference import APIReference
+from dnd5epy.models.monster_action import MonsterAction
+from dnd5epy.models.monster_all_of_senses import MonsterAllOfSenses
+from dnd5epy.models.monster_all_of_speed import MonsterAllOfSpeed
+from dnd5epy.models.monster_armor_class import MonsterArmorClass
+from dnd5epy.models.monster_proficiency import MonsterProficiency
+from dnd5epy.models.monster_special_ability import MonsterSpecialAbility
 
 class Monster(BaseModel):
     """
     `Monster` 
     """
     index: Optional[StrictStr] = Field(None, description="Resource index for shorthand searching.")
     name: Optional[StrictStr] = Field(None, description="Name of the referenced resource.")
```

### Comparing `dnd5epy-1.0.2/dnd5epy/models/monster_ability.py` & `dnd5epy-1.0.3/dnd5epy/models/monster_ability.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.2/dnd5epy/models/monster_action.py` & `dnd5epy-1.0.3/dnd5epy/models/monster_action.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,19 +16,19 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List, Optional, Union
 from pydantic import BaseModel, StrictFloat, StrictInt, StrictStr, conlist
-from openapi_client.models.choice import Choice
-from openapi_client.models.damage import Damage
-from openapi_client.models.dc import DC
-from openapi_client.models.monster_attack import MonsterAttack
-from openapi_client.models.monster_multi_attack_action import MonsterMultiAttackAction
+from dnd5epy.models.choice import Choice
+from dnd5epy.models.damage import Damage
+from dnd5epy.models.dc import DC
+from dnd5epy.models.monster_attack import MonsterAttack
+from dnd5epy.models.monster_multi_attack_action import MonsterMultiAttackAction
 
 class MonsterAction(BaseModel):
     """
     Action available to a `Monster` in addition to the standard creature actions.
     """
     name: Optional[StrictStr] = None
     desc: Optional[StrictStr] = None
```

### Comparing `dnd5epy-1.0.2/dnd5epy/models/monster_all_of_senses.py` & `dnd5epy-1.0.3/dnd5epy/models/monster_all_of_senses.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.2/dnd5epy/models/monster_all_of_speed.py` & `dnd5epy-1.0.3/dnd5epy/models/monster_all_of_speed.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.2/dnd5epy/models/monster_armor_class.py` & `dnd5epy-1.0.3/dnd5epy/models/monster_armor_class.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,19 +16,19 @@
 from inspect import getfullargspec
 import json
 import pprint
 import re  # noqa: F401
 
 from typing import Any, List, Optional
 from pydantic import BaseModel, Field, StrictStr, ValidationError, validator
-from openapi_client.models.monster_armor_class_one_of import MonsterArmorClassOneOf
-from openapi_client.models.monster_armor_class_one_of1 import MonsterArmorClassOneOf1
-from openapi_client.models.monster_armor_class_one_of2 import MonsterArmorClassOneOf2
-from openapi_client.models.monster_armor_class_one_of3 import MonsterArmorClassOneOf3
-from openapi_client.models.monster_armor_class_one_of4 import MonsterArmorClassOneOf4
+from dnd5epy.models.monster_armor_class_one_of import MonsterArmorClassOneOf
+from dnd5epy.models.monster_armor_class_one_of1 import MonsterArmorClassOneOf1
+from dnd5epy.models.monster_armor_class_one_of2 import MonsterArmorClassOneOf2
+from dnd5epy.models.monster_armor_class_one_of3 import MonsterArmorClassOneOf3
+from dnd5epy.models.monster_armor_class_one_of4 import MonsterArmorClassOneOf4
 from typing import Any, List
 from pydantic import StrictStr, Field
 
 MONSTERARMORCLASS_ONE_OF_SCHEMAS = ["MonsterArmorClassOneOf", "MonsterArmorClassOneOf1", "MonsterArmorClassOneOf2", "MonsterArmorClassOneOf3", "MonsterArmorClassOneOf4"]
 
 class MonsterArmorClass(BaseModel):
     """
```

### Comparing `dnd5epy-1.0.2/dnd5epy/models/monster_armor_class_one_of.py` & `dnd5epy-1.0.3/dnd5epy/models/monster_armor_class_one_of.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.2/dnd5epy/models/monster_armor_class_one_of1.py` & `dnd5epy-1.0.3/dnd5epy/models/monster_armor_class_one_of1.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.2/dnd5epy/models/monster_armor_class_one_of2.py` & `dnd5epy-1.0.3/dnd5epy/models/monster_armor_class_one_of2.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List, Optional, Union
 from pydantic import BaseModel, StrictFloat, StrictInt, StrictStr, conlist, validator
-from openapi_client.models.api_reference import APIReference
+from dnd5epy.models.api_reference import APIReference
 
 class MonsterArmorClassOneOf2(BaseModel):
     """
     MonsterArmorClassOneOf2
     """
     type: Optional[StrictStr] = None
     value: Optional[Union[StrictFloat, StrictInt]] = None
```

### Comparing `dnd5epy-1.0.2/dnd5epy/models/monster_armor_class_one_of3.py` & `dnd5epy-1.0.3/dnd5epy/models/monster_armor_class_one_of3.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional, Union
 from pydantic import BaseModel, StrictFloat, StrictInt, StrictStr, validator
-from openapi_client.models.api_reference import APIReference
+from dnd5epy.models.api_reference import APIReference
 
 class MonsterArmorClassOneOf3(BaseModel):
     """
     MonsterArmorClassOneOf3
     """
     type: Optional[StrictStr] = None
     value: Optional[Union[StrictFloat, StrictInt]] = None
```

### Comparing `dnd5epy-1.0.2/dnd5epy/models/monster_armor_class_one_of4.py` & `dnd5epy-1.0.3/dnd5epy/models/monster_armor_class_one_of4.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional, Union
 from pydantic import BaseModel, StrictFloat, StrictInt, StrictStr, validator
-from openapi_client.models.api_reference import APIReference
+from dnd5epy.models.api_reference import APIReference
 
 class MonsterArmorClassOneOf4(BaseModel):
     """
     MonsterArmorClassOneOf4
     """
     type: Optional[StrictStr] = None
     value: Optional[Union[StrictFloat, StrictInt]] = None
```

### Comparing `dnd5epy-1.0.2/dnd5epy/models/monster_attack.py` & `dnd5epy-1.0.3/dnd5epy/models/monster_attack.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
 from pydantic import BaseModel, StrictStr
-from openapi_client.models.damage import Damage
-from openapi_client.models.dc import DC
+from dnd5epy.models.damage import Damage
+from dnd5epy.models.dc import DC
 
 class MonsterAttack(BaseModel):
     """
     MonsterAttack
     """
     name: Optional[StrictStr] = None
     dc: Optional[DC] = None
```

### Comparing `dnd5epy-1.0.2/dnd5epy/models/monster_multi_attack_action.py` & `dnd5epy-1.0.3/dnd5epy/models/monster_multi_attack_action.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.2/dnd5epy/models/monster_proficiency.py` & `dnd5epy-1.0.3/dnd5epy/models/monster_proficiency.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional, Union
 from pydantic import BaseModel, StrictFloat, StrictInt
-from openapi_client.models.api_reference import APIReference
+from dnd5epy.models.api_reference import APIReference
 
 class MonsterProficiency(BaseModel):
     """
     MonsterProficiency
     """
     value: Optional[Union[StrictFloat, StrictInt]] = None
     proficiency: Optional[APIReference] = None
```

### Comparing `dnd5epy-1.0.2/dnd5epy/models/monster_sense.py` & `dnd5epy-1.0.3/dnd5epy/models/monster_sense.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.2/dnd5epy/models/monster_special_ability.py` & `dnd5epy-1.0.3/dnd5epy/models/monster_special_ability.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional, Union
 from pydantic import BaseModel, StrictFloat, StrictInt, StrictStr
-from openapi_client.models.damage import Damage
-from openapi_client.models.dc import DC
-from openapi_client.models.monster_spellcasting import MonsterSpellcasting
-from openapi_client.models.monster_usage import MonsterUsage
+from dnd5epy.models.damage import Damage
+from dnd5epy.models.dc import DC
+from dnd5epy.models.monster_spellcasting import MonsterSpellcasting
+from dnd5epy.models.monster_usage import MonsterUsage
 
 class MonsterSpecialAbility(BaseModel):
     """
     MonsterSpecialAbility
     """
     name: Optional[StrictStr] = None
     desc: Optional[StrictStr] = None
```

### Comparing `dnd5epy-1.0.2/dnd5epy/models/monster_spell.py` & `dnd5epy-1.0.3/dnd5epy/models/monster_spell.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional, Union
 from pydantic import BaseModel, StrictFloat, StrictInt, StrictStr
-from openapi_client.models.monster_usage import MonsterUsage
+from dnd5epy.models.monster_usage import MonsterUsage
 
 class MonsterSpell(BaseModel):
     """
     MonsterSpell
     """
     name: Optional[StrictStr] = None
     level: Optional[Union[StrictFloat, StrictInt]] = None
```

### Comparing `dnd5epy-1.0.2/dnd5epy/models/monster_spellcasting.py` & `dnd5epy-1.0.3/dnd5epy/models/monster_spellcasting.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Dict, List, Optional, Union
 from pydantic import BaseModel, StrictFloat, StrictInt, StrictStr, conlist
-from openapi_client.models.api_reference import APIReference
-from openapi_client.models.monster_spell import MonsterSpell
+from dnd5epy.models.api_reference import APIReference
+from dnd5epy.models.monster_spell import MonsterSpell
 
 class MonsterSpellcasting(BaseModel):
     """
     MonsterSpellcasting
     """
     ability: Optional[APIReference] = None
     dc: Optional[Union[StrictFloat, StrictInt]] = None
```

### Comparing `dnd5epy-1.0.2/dnd5epy/models/monster_usage.py` & `dnd5epy-1.0.3/dnd5epy/models/monster_usage.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.2/dnd5epy/models/multiclassing.py` & `dnd5epy-1.0.3/dnd5epy/models/multiclassing.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,17 +16,17 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List, Optional
 from pydantic import BaseModel, Field, conlist
-from openapi_client.models.api_reference import APIReference
-from openapi_client.models.choice import Choice
-from openapi_client.models.prerequisite import Prerequisite
+from dnd5epy.models.api_reference import APIReference
+from dnd5epy.models.choice import Choice
+from dnd5epy.models.prerequisite import Prerequisite
 
 class Multiclassing(BaseModel):
     """
     `Multiclassing` 
     """
     prerequisites: Optional[conlist(Prerequisite)] = Field(None, description="List of prerequisites that must be met.")
     prerequisite_options: Optional[conlist(Choice)] = Field(None, description="List of choices of prerequisites to meet for.")
```

### Comparing `dnd5epy-1.0.2/dnd5epy/models/option.py` & `dnd5epy-1.0.3/dnd5epy/models/option.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,23 +16,23 @@
 from inspect import getfullargspec
 import json
 import pprint
 import re  # noqa: F401
 
 from typing import Any, List, Optional
 from pydantic import BaseModel, Field, StrictStr, ValidationError, validator
-from openapi_client.models.option_one_of import OptionOneOf
-from openapi_client.models.option_one_of1 import OptionOneOf1
-from openapi_client.models.option_one_of10 import OptionOneOf10
-from openapi_client.models.option_one_of4 import OptionOneOf4
-from openapi_client.models.option_one_of5 import OptionOneOf5
-from openapi_client.models.option_one_of6 import OptionOneOf6
-from openapi_client.models.option_one_of7 import OptionOneOf7
-from openapi_client.models.option_one_of8 import OptionOneOf8
-from openapi_client.models.option_one_of9 import OptionOneOf9
+from dnd5epy.models.option_one_of import OptionOneOf
+from dnd5epy.models.option_one_of1 import OptionOneOf1
+from dnd5epy.models.option_one_of10 import OptionOneOf10
+from dnd5epy.models.option_one_of4 import OptionOneOf4
+from dnd5epy.models.option_one_of5 import OptionOneOf5
+from dnd5epy.models.option_one_of6 import OptionOneOf6
+from dnd5epy.models.option_one_of7 import OptionOneOf7
+from dnd5epy.models.option_one_of8 import OptionOneOf8
+from dnd5epy.models.option_one_of9 import OptionOneOf9
 from typing import Any, List
 from pydantic import StrictStr, Field
 
 OPTION_ONE_OF_SCHEMAS = ["OptionOneOf", "OptionOneOf1", "OptionOneOf10", "OptionOneOf2", "OptionOneOf3", "OptionOneOf4", "OptionOneOf5", "OptionOneOf6", "OptionOneOf7", "OptionOneOf8", "OptionOneOf9"]
 
 class Option(BaseModel):
     """
```

### Comparing `dnd5epy-1.0.2/dnd5epy/models/option_one_of.py` & `dnd5epy-1.0.3/dnd5epy/models/option_one_of.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
 from pydantic import BaseModel, Field, StrictStr
-from openapi_client.models.api_reference import APIReference
+from dnd5epy.models.api_reference import APIReference
 
 class OptionOneOf(BaseModel):
     """
     OptionOneOf
     """
     option_type: Optional[StrictStr] = Field(None, description="Type of option; determines other attributes.")
     item: Optional[APIReference] = None
```

### Comparing `dnd5epy-1.0.2/dnd5epy/models/option_one_of1.py` & `dnd5epy-1.0.3/dnd5epy/models/option_one_of1.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.2/dnd5epy/models/option_one_of10.py` & `dnd5epy-1.0.3/dnd5epy/models/option_one_of10.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
 from pydantic import BaseModel, Field, StrictStr
-from openapi_client.models.api_reference import APIReference
+from dnd5epy.models.api_reference import APIReference
 
 class OptionOneOf10(BaseModel):
     """
     OptionOneOf10
     """
     option_type: Optional[StrictStr] = Field(None, description="Type of option; determines other attributes.")
     damage_type: Optional[APIReference] = None
```

### Comparing `dnd5epy-1.0.2/dnd5epy/models/option_one_of2.py` & `dnd5epy-1.0.3/dnd5epy/models/option_one_of2.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.2/dnd5epy/models/option_one_of3.py` & `dnd5epy-1.0.3/dnd5epy/models/option_one_of3.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.2/dnd5epy/models/option_one_of4.py` & `dnd5epy-1.0.3/dnd5epy/models/option_one_of4.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.2/dnd5epy/models/option_one_of5.py` & `dnd5epy-1.0.3/dnd5epy/models/option_one_of5.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List, Optional
 from pydantic import BaseModel, Field, StrictStr, conlist
-from openapi_client.models.api_reference import APIReference
+from dnd5epy.models.api_reference import APIReference
 
 class OptionOneOf5(BaseModel):
     """
     OptionOneOf5
     """
     option_type: Optional[StrictStr] = Field(None, description="Type of option; determines other attributes.")
     desc: Optional[StrictStr] = Field(None, description="A description of the ideal.")
```

### Comparing `dnd5epy-1.0.2/dnd5epy/models/option_one_of6.py` & `dnd5epy-1.0.3/dnd5epy/models/option_one_of6.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional, Union
 from pydantic import BaseModel, Field, StrictFloat, StrictInt, StrictStr
-from openapi_client.models.api_reference import APIReference
+from dnd5epy.models.api_reference import APIReference
 
 class OptionOneOf6(BaseModel):
     """
     OptionOneOf6
     """
     option_type: Optional[StrictStr] = Field(None, description="Type of option; determines other attributes.")
     count: Optional[Union[StrictFloat, StrictInt]] = Field(None, description="Count")
```

### Comparing `dnd5epy-1.0.2/dnd5epy/models/option_one_of7.py` & `dnd5epy-1.0.3/dnd5epy/models/option_one_of7.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional, Union
 from pydantic import BaseModel, Field, StrictFloat, StrictInt, StrictStr
-from openapi_client.models.api_reference import APIReference
+from dnd5epy.models.api_reference import APIReference
 
 class OptionOneOf7(BaseModel):
     """
     OptionOneOf7
     """
     option_type: Optional[StrictStr] = Field(None, description="Type of option; determines other attributes.")
     ability_score: Optional[APIReference] = None
```

### Comparing `dnd5epy-1.0.2/dnd5epy/models/option_one_of8.py` & `dnd5epy-1.0.3/dnd5epy/models/option_one_of8.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional, Union
 from pydantic import BaseModel, Field, StrictFloat, StrictInt, StrictStr
-from openapi_client.models.api_reference import APIReference
+from dnd5epy.models.api_reference import APIReference
 
 class OptionOneOf8(BaseModel):
     """
     OptionOneOf8
     """
     option_type: Optional[StrictStr] = Field(None, description="Type of option; determines other attributes.")
     ability_score: Optional[APIReference] = None
```

### Comparing `dnd5epy-1.0.2/dnd5epy/models/option_one_of9.py` & `dnd5epy-1.0.3/dnd5epy/models/option_one_of9.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List, Optional
 from pydantic import BaseModel, Field, StrictStr, conlist
-from openapi_client.models.damage import Damage
-from openapi_client.models.dc import DC
+from dnd5epy.models.damage import Damage
+from dnd5epy.models.dc import DC
 
 class OptionOneOf9(BaseModel):
     """
     OptionOneOf9
     """
     option_type: Optional[StrictStr] = Field(None, description="Type of option; determines other attributes.")
     name: Optional[StrictStr] = Field(None, description="Name of the breath")
```

### Comparing `dnd5epy-1.0.2/dnd5epy/models/option_set.py` & `dnd5epy-1.0.3/dnd5epy/models/option_set.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 from inspect import getfullargspec
 import json
 import pprint
 import re  # noqa: F401
 
 from typing import Any, List, Optional
 from pydantic import BaseModel, Field, StrictStr, ValidationError, validator
-from openapi_client.models.option_set_one_of1 import OptionSetOneOf1
-from openapi_client.models.option_set_one_of2 import OptionSetOneOf2
+from dnd5epy.models.option_set_one_of1 import OptionSetOneOf1
+from dnd5epy.models.option_set_one_of2 import OptionSetOneOf2
 from typing import Any, List
 from pydantic import StrictStr, Field
 
 OPTIONSET_ONE_OF_SCHEMAS = ["OptionSetOneOf", "OptionSetOneOf1", "OptionSetOneOf2"]
 
 class OptionSet(BaseModel):
     """
```

### Comparing `dnd5epy-1.0.2/dnd5epy/models/option_set_one_of.py` & `dnd5epy-1.0.3/dnd5epy/models/option_set_one_of.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.2/dnd5epy/models/option_set_one_of1.py` & `dnd5epy-1.0.3/dnd5epy/models/option_set_one_of1.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
 from pydantic import BaseModel, Field, StrictStr
-from openapi_client.models.api_reference import APIReference
+from dnd5epy.models.api_reference import APIReference
 
 class OptionSetOneOf1(BaseModel):
     """
     OptionSetOneOf1
     """
     option_set_type: Optional[StrictStr] = Field(None, description="Type of option set; determines other attributes.")
     equipment_category: Optional[APIReference] = None
```

### Comparing `dnd5epy-1.0.2/dnd5epy/models/option_set_one_of2.py` & `dnd5epy-1.0.3/dnd5epy/models/option_set_one_of2.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.2/dnd5epy/models/prerequisite.py` & `dnd5epy-1.0.3/dnd5epy/models/prerequisite.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional, Union
 from pydantic import BaseModel, Field, StrictFloat, StrictInt
-from openapi_client.models.prerequisite_ability_score import PrerequisiteAbilityScore
+from dnd5epy.models.prerequisite_ability_score import PrerequisiteAbilityScore
 
 class Prerequisite(BaseModel):
     """
     `Prerequisite` 
     """
     ability_score: Optional[PrerequisiteAbilityScore] = None
     minimum_score: Optional[Union[StrictFloat, StrictInt]] = Field(None, description="Minimum score to meet the prerequisite.")
```

### Comparing `dnd5epy-1.0.2/dnd5epy/models/prerequisite_ability_score.py` & `dnd5epy-1.0.3/dnd5epy/models/prerequisite_ability_score.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.2/dnd5epy/models/proficiency.py` & `dnd5epy-1.0.3/dnd5epy/models/proficiency.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List, Optional
 from pydantic import BaseModel, Field, StrictStr, conlist
-from openapi_client.models.api_reference import APIReference
-from openapi_client.models.proficiency_all_of_reference import ProficiencyAllOfReference
+from dnd5epy.models.api_reference import APIReference
+from dnd5epy.models.proficiency_all_of_reference import ProficiencyAllOfReference
 
 class Proficiency(BaseModel):
     """
     `Proficiency` 
     """
     index: Optional[StrictStr] = Field(None, description="Resource index for shorthand searching.")
     name: Optional[StrictStr] = Field(None, description="Name of the referenced resource.")
```

### Comparing `dnd5epy-1.0.2/dnd5epy/models/proficiency_all_of_reference.py` & `dnd5epy-1.0.3/dnd5epy/models/proficiency_all_of_reference.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.2/dnd5epy/models/race.py` & `dnd5epy-1.0.3/dnd5epy/models/race.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,17 +16,17 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List, Optional, Union
 from pydantic import BaseModel, Field, StrictFloat, StrictInt, StrictStr, conlist
-from openapi_client.models.ability_bonus import AbilityBonus
-from openapi_client.models.api_reference import APIReference
-from openapi_client.models.choice import Choice
+from dnd5epy.models.ability_bonus import AbilityBonus
+from dnd5epy.models.api_reference import APIReference
+from dnd5epy.models.choice import Choice
 
 class Race(BaseModel):
     """
     `Race` 
     """
     index: Optional[StrictStr] = Field(None, description="Resource index for shorthand searching.")
     name: Optional[StrictStr] = Field(None, description="Name of the referenced resource.")
```

### Comparing `dnd5epy-1.0.2/dnd5epy/models/resource_description.py` & `dnd5epy-1.0.3/dnd5epy/models/resource_description.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.2/dnd5epy/models/rule.py` & `dnd5epy-1.0.3/dnd5epy/models/rule.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List, Optional
 from pydantic import BaseModel, Field, StrictStr, conlist
-from openapi_client.models.api_reference import APIReference
+from dnd5epy.models.api_reference import APIReference
 
 class Rule(BaseModel):
     """
     `Rule` 
     """
     index: Optional[StrictStr] = Field(None, description="Resource index for shorthand searching.")
     name: Optional[StrictStr] = Field(None, description="Name of the referenced resource.")
```

### Comparing `dnd5epy-1.0.2/dnd5epy/models/rule_section.py` & `dnd5epy-1.0.3/dnd5epy/models/rule_section.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.2/dnd5epy/models/skill.py` & `dnd5epy-1.0.3/dnd5epy/models/skill.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List, Optional
 from pydantic import BaseModel, Field, StrictStr, conlist
-from openapi_client.models.api_reference import APIReference
+from dnd5epy.models.api_reference import APIReference
 
 class Skill(BaseModel):
     """
     `Skill` 
     """
     index: Optional[StrictStr] = Field(None, description="Resource index for shorthand searching.")
     name: Optional[StrictStr] = Field(None, description="Name of the referenced resource.")
```

### Comparing `dnd5epy-1.0.2/dnd5epy/models/spell.py` & `dnd5epy-1.0.3/dnd5epy/models/spell.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,17 +16,17 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List, Optional, Union
 from pydantic import BaseModel, Field, StrictBool, StrictFloat, StrictInt, StrictStr, conlist, validator
-from openapi_client.models.api_reference import APIReference
-from openapi_client.models.area_of_effect import AreaOfEffect
-from openapi_client.models.spell_all_of_damage import SpellAllOfDamage
+from dnd5epy.models.api_reference import APIReference
+from dnd5epy.models.area_of_effect import AreaOfEffect
+from dnd5epy.models.spell_all_of_damage import SpellAllOfDamage
 
 class Spell(BaseModel):
     """
     `Spell` 
     """
     index: Optional[StrictStr] = Field(None, description="Resource index for shorthand searching.")
     name: Optional[StrictStr] = Field(None, description="Name of the referenced resource.")
```

### Comparing `dnd5epy-1.0.2/dnd5epy/models/spell_all_of_damage.py` & `dnd5epy-1.0.3/dnd5epy/models/spell_all_of_damage.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 from inspect import getfullargspec
 import json
 import pprint
 import re  # noqa: F401
 
 from typing import Any, List, Optional
 from pydantic import BaseModel, Field, StrictStr, ValidationError, validator
-from openapi_client.models.damage_at_character_level import DamageAtCharacterLevel
-from openapi_client.models.damage_at_slot_level import DamageAtSlotLevel
+from dnd5epy.models.damage_at_character_level import DamageAtCharacterLevel
+from dnd5epy.models.damage_at_slot_level import DamageAtSlotLevel
 from typing import Any, List
 from pydantic import StrictStr, Field
 
 SPELLALLOFDAMAGE_ONE_OF_SCHEMAS = ["DamageAtCharacterLevel", "DamageAtSlotLevel"]
 
 class SpellAllOfDamage(BaseModel):
     """
```

### Comparing `dnd5epy-1.0.2/dnd5epy/models/spell_prerequisite.py` & `dnd5epy-1.0.3/dnd5epy/models/spell_prerequisite.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.2/dnd5epy/models/spellcasting.py` & `dnd5epy-1.0.3/dnd5epy/models/spellcasting.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List, Optional, Union
 from pydantic import BaseModel, Field, StrictFloat, StrictInt, conlist
-from openapi_client.models.spellcasting_info_inner import SpellcastingInfoInner
-from openapi_client.models.spellcasting_spellcasting_ability import SpellcastingSpellcastingAbility
+from dnd5epy.models.spellcasting_info_inner import SpellcastingInfoInner
+from dnd5epy.models.spellcasting_spellcasting_ability import SpellcastingSpellcastingAbility
 
 class Spellcasting(BaseModel):
     """
     `Spellcasting` 
     """
     level: Optional[Union[StrictFloat, StrictInt]] = Field(None, description="Level at which the class can start using its spellcasting abilities.")
     info: Optional[conlist(SpellcastingInfoInner)] = Field(None, description="Descriptions of the class' ability to cast spells.")
```

### Comparing `dnd5epy-1.0.2/dnd5epy/models/spellcasting_info_inner.py` & `dnd5epy-1.0.3/dnd5epy/models/spellcasting_info_inner.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.2/dnd5epy/models/spellcasting_spellcasting_ability.py` & `dnd5epy-1.0.3/dnd5epy/models/spellcasting_spellcasting_ability.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.2/dnd5epy/models/subclass.py` & `dnd5epy-1.0.3/dnd5epy/models/subclass.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List, Optional
 from pydantic import BaseModel, Field, StrictStr, conlist
-from openapi_client.models.api_reference import APIReference
-from openapi_client.models.subclass_all_of_spells import SubclassAllOfSpells
+from dnd5epy.models.api_reference import APIReference
+from dnd5epy.models.subclass_all_of_spells import SubclassAllOfSpells
 
 class Subclass(BaseModel):
     """
     `Subclass` 
     """
     index: Optional[StrictStr] = Field(None, description="Resource index for shorthand searching.")
     name: Optional[StrictStr] = Field(None, description="Name of the referenced resource.")
```

### Comparing `dnd5epy-1.0.2/dnd5epy/models/subclass_all_of_spells.py` & `dnd5epy-1.0.3/dnd5epy/models/subclass_all_of_spells.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List, Optional
 from pydantic import BaseModel, conlist
-from openapi_client.models.api_reference import APIReference
-from openapi_client.models.spell_prerequisite import SpellPrerequisite
+from dnd5epy.models.api_reference import APIReference
+from dnd5epy.models.spell_prerequisite import SpellPrerequisite
 
 class SubclassAllOfSpells(BaseModel):
     """
     SubclassAllOfSpells
     """
     prerequisites: Optional[conlist(SpellPrerequisite)] = None
     spell: Optional[APIReference] = None
```

### Comparing `dnd5epy-1.0.2/dnd5epy/models/subclass_level.py` & `dnd5epy-1.0.3/dnd5epy/models/subclass_level.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, List, Optional, Union
 from pydantic import BaseModel, Field, StrictFloat, StrictInt, StrictStr, conlist
-from openapi_client.models.api_reference import APIReference
-from openapi_client.models.subclass_level_spellcasting import SubclassLevelSpellcasting
+from dnd5epy.models.api_reference import APIReference
+from dnd5epy.models.subclass_level_spellcasting import SubclassLevelSpellcasting
 
 class SubclassLevel(BaseModel):
     """
     `SubclassLevel` 
     """
     index: Optional[StrictStr] = Field(None, description="Resource index for shorthand searching.")
     url: Optional[StrictStr] = Field(None, description="URL of the referenced resource.")
```

### Comparing `dnd5epy-1.0.2/dnd5epy/models/subclass_level_resource.py` & `dnd5epy-1.0.3/dnd5epy/models/subclass_level_resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List, Optional, Union
 from pydantic import BaseModel, Field, StrictFloat, StrictInt, StrictStr, conlist
-from openapi_client.models.api_reference import APIReference
+from dnd5epy.models.api_reference import APIReference
 
 class SubclassLevelResource(BaseModel):
     """
     SubclassLevelResource
     """
     index: Optional[StrictStr] = None
     url: Optional[StrictStr] = None
```

### Comparing `dnd5epy-1.0.2/dnd5epy/models/subclass_level_spellcasting.py` & `dnd5epy-1.0.3/dnd5epy/models/subclass_level_spellcasting.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.2/dnd5epy/models/subrace.py` & `dnd5epy-1.0.3/dnd5epy/models/subrace.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List, Optional
 from pydantic import BaseModel, Field, StrictStr, conlist
-from openapi_client.models.ability_bonus import AbilityBonus
-from openapi_client.models.api_reference import APIReference
-from openapi_client.models.choice import Choice
-from openapi_client.models.subrace_all_of_race import SubraceAllOfRace
+from dnd5epy.models.ability_bonus import AbilityBonus
+from dnd5epy.models.api_reference import APIReference
+from dnd5epy.models.choice import Choice
+from dnd5epy.models.subrace_all_of_race import SubraceAllOfRace
 
 class Subrace(BaseModel):
     """
     `Subrace` 
     """
     index: Optional[StrictStr] = Field(None, description="Resource index for shorthand searching.")
     name: Optional[StrictStr] = Field(None, description="Name of the referenced resource.")
```

### Comparing `dnd5epy-1.0.2/dnd5epy/models/subrace_all_of_race.py` & `dnd5epy-1.0.3/dnd5epy/models/subrace_all_of_race.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.2/dnd5epy/models/trait.py` & `dnd5epy-1.0.3/dnd5epy/models/trait.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,17 +16,17 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List, Optional
 from pydantic import BaseModel, Field, StrictStr, conlist
-from openapi_client.models.api_reference import APIReference
-from openapi_client.models.choice import Choice
-from openapi_client.models.trait_all_of_trait_specific import TraitAllOfTraitSpecific
+from dnd5epy.models.api_reference import APIReference
+from dnd5epy.models.choice import Choice
+from dnd5epy.models.trait_all_of_trait_specific import TraitAllOfTraitSpecific
 
 class Trait(BaseModel):
     """
     `Trait` 
     """
     index: Optional[StrictStr] = Field(None, description="Resource index for shorthand searching.")
     name: Optional[StrictStr] = Field(None, description="Name of the referenced resource.")
```

### Comparing `dnd5epy-1.0.2/dnd5epy/models/trait_all_of_trait_specific.py` & `dnd5epy-1.0.3/dnd5epy/models/trait_all_of_trait_specific.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 from inspect import getfullargspec
 import json
 import pprint
 import re  # noqa: F401
 
 from typing import Any, List, Optional
 from pydantic import BaseModel, Field, StrictStr, ValidationError, validator
-from openapi_client.models.choice import Choice
-from openapi_client.models.trait_all_of_trait_specific_one_of import TraitAllOfTraitSpecificOneOf
+from dnd5epy.models.choice import Choice
+from dnd5epy.models.trait_all_of_trait_specific_one_of import TraitAllOfTraitSpecificOneOf
 from typing import Any, List
 from pydantic import StrictStr, Field
 
 TRAITALLOFTRAITSPECIFIC_ONE_OF_SCHEMAS = ["Choice", "TraitAllOfTraitSpecificOneOf"]
 
 class TraitAllOfTraitSpecific(BaseModel):
     """
```

### Comparing `dnd5epy-1.0.2/dnd5epy/models/trait_all_of_trait_specific_one_of.py` & `dnd5epy-1.0.3/dnd5epy/models/trait_all_of_trait_specific_one_of.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
 from pydantic import BaseModel, Field
-from openapi_client.models.trait_all_of_trait_specific_one_of_breath_weapon import TraitAllOfTraitSpecificOneOfBreathWeapon
-from openapi_client.models.trait_all_of_trait_specific_one_of_damage_type import TraitAllOfTraitSpecificOneOfDamageType
+from dnd5epy.models.trait_all_of_trait_specific_one_of_breath_weapon import TraitAllOfTraitSpecificOneOfBreathWeapon
+from dnd5epy.models.trait_all_of_trait_specific_one_of_damage_type import TraitAllOfTraitSpecificOneOfDamageType
 
 class TraitAllOfTraitSpecificOneOf(BaseModel):
     """
     TraitAllOfTraitSpecificOneOf
     """
     damage_type: Optional[TraitAllOfTraitSpecificOneOfDamageType] = Field(None, alias="damage-type")
     breath_weapon: Optional[TraitAllOfTraitSpecificOneOfBreathWeapon] = Field(None, alias="breath-weapon")
```

### Comparing `dnd5epy-1.0.2/dnd5epy/models/trait_all_of_trait_specific_one_of_breath_weapon.py` & `dnd5epy-1.0.3/dnd5epy/models/trait_all_of_trait_specific_one_of_breath_weapon.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
 from pydantic import BaseModel, StrictStr
-from openapi_client.models.area_of_effect import AreaOfEffect
-from openapi_client.models.dc import DC
-from openapi_client.models.trait_all_of_trait_specific_one_of_breath_weapon_damage import TraitAllOfTraitSpecificOneOfBreathWeaponDamage
-from openapi_client.models.trait_all_of_trait_specific_one_of_breath_weapon_usage import TraitAllOfTraitSpecificOneOfBreathWeaponUsage
+from dnd5epy.models.area_of_effect import AreaOfEffect
+from dnd5epy.models.dc import DC
+from dnd5epy.models.trait_all_of_trait_specific_one_of_breath_weapon_damage import TraitAllOfTraitSpecificOneOfBreathWeaponDamage
+from dnd5epy.models.trait_all_of_trait_specific_one_of_breath_weapon_usage import TraitAllOfTraitSpecificOneOfBreathWeaponUsage
 
 class TraitAllOfTraitSpecificOneOfBreathWeapon(BaseModel):
     """
     The breath weapon action associated with a draconic ancestry.
     """
     name: Optional[StrictStr] = None
     desc: Optional[StrictStr] = None
```

### Comparing `dnd5epy-1.0.2/dnd5epy/models/trait_all_of_trait_specific_one_of_breath_weapon_damage.py` & `dnd5epy-1.0.3/dnd5epy/models/trait_all_of_trait_specific_one_of_breath_weapon_damage.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Dict, Optional
 from pydantic import BaseModel, StrictStr
-from openapi_client.models.prerequisite_ability_score import PrerequisiteAbilityScore
+from dnd5epy.models.prerequisite_ability_score import PrerequisiteAbilityScore
 
 class TraitAllOfTraitSpecificOneOfBreathWeaponDamage(BaseModel):
     """
     TraitAllOfTraitSpecificOneOfBreathWeaponDamage
     """
     damage_at_character_level: Optional[Dict[str, StrictStr]] = None
     damage_type: Optional[PrerequisiteAbilityScore] = None
```

### Comparing `dnd5epy-1.0.2/dnd5epy/models/trait_all_of_trait_specific_one_of_breath_weapon_usage.py` & `dnd5epy-1.0.3/dnd5epy/models/trait_all_of_trait_specific_one_of_breath_weapon_usage.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.2/dnd5epy/models/trait_all_of_trait_specific_one_of_damage_type.py` & `dnd5epy-1.0.3/dnd5epy/models/trait_all_of_trait_specific_one_of_damage_type.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.2/dnd5epy/models/weapon.py` & `dnd5epy-1.0.3/dnd5epy/models/weapon.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List, Optional, Union
 from pydantic import BaseModel, Field, StrictFloat, StrictInt, StrictStr, conlist
-from openapi_client.models.api_reference import APIReference
-from openapi_client.models.cost import Cost
-from openapi_client.models.damage import Damage
-from openapi_client.models.weapon_all_of_range import WeaponAllOfRange
+from dnd5epy.models.api_reference import APIReference
+from dnd5epy.models.cost import Cost
+from dnd5epy.models.damage import Damage
+from dnd5epy.models.weapon_all_of_range import WeaponAllOfRange
 
 class Weapon(BaseModel):
     """
     `Weapon` 
     """
     index: Optional[StrictStr] = Field(None, description="Resource index for shorthand searching.")
     name: Optional[StrictStr] = Field(None, description="Name of the referenced resource.")
```

### Comparing `dnd5epy-1.0.2/dnd5epy/models/weapon_all_of_range.py` & `dnd5epy-1.0.3/dnd5epy/models/weapon_all_of_range.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.2/dnd5epy/models/weapon_property.py` & `dnd5epy-1.0.3/dnd5epy/models/weapon_property.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.2/dnd5epy/rest.py` & `dnd5epy-1.0.3/dnd5epy/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import logging
 import re
 import ssl
 
 from urllib.parse import urlencode, quote_plus
 import urllib3
 
-from openapi_client.exceptions import ApiException, UnauthorizedException, ForbiddenException, NotFoundException, ServiceException, ApiValueError, BadRequestException
+from dnd5epy.exceptions import ApiException, UnauthorizedException, ForbiddenException, NotFoundException, ServiceException, ApiValueError, BadRequestException
 
 
 logger = logging.getLogger(__name__)
 
 
 class RESTResponse(io.IOBase):
```

### Comparing `dnd5epy-1.0.2/pyproject.toml` & `dnd5epy-1.0.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "dnd5epy"
-version = "1.0.2"
+version = "1.0.3"
 description = "D&D 5e API"
 authors = ["5eBits <team@openapitools.org>"]
 license = "MIT License"
 readme = "README.md"
 repository = "https://github.com/GIT_USER_ID/GIT_REPO_ID"
 keywords = ["OpenAPI", "OpenAPI-Generator", "D&D 5e API"]
-include = ["openapi_client/py.typed"]
+include = ["dnd5epy/py.typed"]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 
 urllib3 = ">= 1.25.3"
 python-dateutil = ">=2.8.2"
 pydantic = "^1.10.5, <2"
```

### Comparing `dnd5epy-1.0.2/PKG-INFO` & `dnd5epy-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dnd5epy
-Version: 1.0.2
+Version: 1.0.3
 Summary: D&D 5e API
 Home-page: https://github.com/GIT_USER_ID/GIT_REPO_ID
 License: MIT
 Keywords: OpenAPI,OpenAPI-Generator,D&D 5e API
 Author: 5eBits
 Author-email: team@openapitools.org
 Requires-Python: >=3.7,<4.0
@@ -247,58 +247,58 @@
 ```sh
 pip install git+https://github.com/GIT_USER_ID/GIT_REPO_ID.git
 ```
 (you may need to run `pip` with root permission: `sudo pip install git+https://github.com/GIT_USER_ID/GIT_REPO_ID.git`)
 
 Then import the package:
 ```python
-import openapi_client
+import dnd5epy
 ```
 
 ### Setuptools
 
 Install via [Setuptools](http://pypi.python.org/pypi/setuptools).
 
 ```sh
 python setup.py install --user
 ```
 (or `sudo python setup.py install` to install the package for all users)
 
 Then import the package:
 ```python
-import openapi_client
+import dnd5epy
 ```
 
 ### Tests
 
 Execute `pytest` to run the tests.
 
 ## Getting Started
 
 Please follow the [installation procedure](#installation--usage) and then run the following:
 
 ```python
 
 import time
-import openapi_client
-from openapi_client.rest import ApiException
+import dnd5epy
+from dnd5epy.rest import ApiException
 from pprint import pprint
 
 # Defining the host is optional and defaults to https://www.dnd5eapi.co
 # See configuration.py for a list of all supported configuration parameters.
-configuration = openapi_client.Configuration(
+configuration = dnd5epy.Configuration(
     host = "https://www.dnd5eapi.co"
 )
 
 
 
 # Enter a context with an instance of the API client
-with openapi_client.ApiClient(configuration) as api_client:
+with dnd5epy.ApiClient(configuration) as api_client:
     # Create an instance of the API class
-    api_instance = openapi_client.CharacterDataApi(api_client)
+    api_instance = dnd5epy.CharacterDataApi(api_client)
 
     try:
         # Get all ability scores.
         api_response = api_instance.api_ability_scores_get()
         print("The response of CharacterDataApi->api_ability_scores_get:\n")
         pprint(api_response)
     except ApiException as e:
```

