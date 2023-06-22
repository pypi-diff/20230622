# Comparing `tmp/fake-bpy-module-latest-20230621.tar.gz` & `tmp/fake-bpy-module-latest-20230622.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fake-bpy-module-latest-20230621.tar", last modified: Wed Jun 21 06:23:21 2023, max compression
+gzip compressed data, was "dist/fake-bpy-module-latest-20230622.tar", last modified: Thu Jun 22 06:24:01 2023, max compression
```

## Comparing `fake-bpy-module-latest-20230621.tar` & `fake-bpy-module-latest-20230622.tar`

### file list

```diff
@@ -1,356 +1,356 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 06:23:21.000000 fake-bpy-module-latest-20230621/
--rw-r--r--   0 runner    (1001) docker     (123)     7193 2023-06-21 06:23:21.000000 fake-bpy-module-latest-20230621/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4958 2023-06-21 06:23:20.000000 fake-bpy-module-latest-20230621/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-21 06:23:19.000000 fake-bpy-module-latest-20230621/addon_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-21 06:21:12.000000 fake-bpy-module-latest-20230621/animsys_refactor.py
--rw-r--r--   0 runner    (1001) docker     (123)    30417 2023-06-21 06:21:08.000000 fake-bpy-module-latest-20230621/aud.py
--rw-r--r--   0 runner    (1001) docker     (123)   116266 2023-06-21 06:21:05.000000 fake-bpy-module-latest-20230621/bgl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 06:23:20.000000 fake-bpy-module-latest-20230621/bl_app_override/
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-21 06:21:12.000000 fake-bpy-module-latest-20230621/bl_app_override/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-21 06:21:12.000000 fake-bpy-module-latest-20230621/bl_app_override/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 06:12:54.000000 fake-bpy-module-latest-20230621/bl_app_override/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-21 06:21:12.000000 fake-bpy-module-latest-20230621/bl_app_template_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 06:23:20.000000 fake-bpy-module-latest-20230621/bl_console_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-21 06:23:19.000000 fake-bpy-module-latest-20230621/bl_console_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 06:23:20.000000 fake-bpy-module-latest-20230621/bl_console_utils/autocomplete/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-21 06:23:19.000000 fake-bpy-module-latest-20230621/bl_console_utils/autocomplete/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-06-21 06:23:19.000000 fake-bpy-module-latest-20230621/bl_console_utils/autocomplete/complete_calltip.py
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-21 06:23:19.000000 fake-bpy-module-latest-20230621/bl_console_utils/autocomplete/complete_import.py
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-21 06:23:19.000000 fake-bpy-module-latest-20230621/bl_console_utils/autocomplete/complete_namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-21 06:23:19.000000 fake-bpy-module-latest-20230621/bl_console_utils/autocomplete/intellisense.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 06:12:54.000000 fake-bpy-module-latest-20230621/bl_console_utils/autocomplete/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 06:12:54.000000 fake-bpy-module-latest-20230621/bl_console_utils/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 06:23:20.000000 fake-bpy-module-latest-20230621/bl_i18n_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-21 06:21:18.000000 fake-bpy-module-latest-20230621/bl_i18n_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-21 06:21:18.000000 fake-bpy-module-latest-20230621/bl_i18n_utils/bl_extract_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-21 06:21:18.000000 fake-bpy-module-latest-20230621/bl_i18n_utils/merge_po.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 06:12:54.000000 fake-bpy-module-latest-20230621/bl_i18n_utils/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-21 06:21:18.000000 fake-bpy-module-latest-20230621/bl_i18n_utils/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-06-21 06:21:18.000000 fake-bpy-module-latest-20230621/bl_i18n_utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-21 06:21:18.000000 fake-bpy-module-latest-20230621/bl_i18n_utils/utils_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-21 06:21:18.000000 fake-bpy-module-latest-20230621/bl_i18n_utils/utils_languages_menu.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-21 06:21:18.000000 fake-bpy-module-latest-20230621/bl_i18n_utils/utils_rtl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 06:23:20.000000 fake-bpy-module-latest-20230621/bl_keymap_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-21 06:21:18.000000 fake-bpy-module-latest-20230621/bl_keymap_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-21 06:21:18.000000 fake-bpy-module-latest-20230621/bl_keymap_utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-21 06:21:18.000000 fake-bpy-module-latest-20230621/bl_keymap_utils/keymap_from_toolbar.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-21 06:21:18.000000 fake-bpy-module-latest-20230621/bl_keymap_utils/keymap_hierarchy.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-21 06:21:18.000000 fake-bpy-module-latest-20230621/bl_keymap_utils/platform_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 06:12:54.000000 fake-bpy-module-latest-20230621/bl_keymap_utils/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-21 06:21:18.000000 fake-bpy-module-latest-20230621/bl_keymap_utils/versioning.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-06-21 06:21:11.000000 fake-bpy-module-latest-20230621/bl_math.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 06:23:20.000000 fake-bpy-module-latest-20230621/bl_operators/
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-06-21 06:21:12.000000 fake-bpy-module-latest-20230621/bl_operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-06-21 06:21:12.000000 fake-bpy-module-latest-20230621/bl_operators/add_mesh_torus.py
--rw-r--r--   0 runner    (1001) docker     (123)     8777 2023-06-21 06:21:12.000000 fake-bpy-module-latest-20230621/bl_operators/anim.py
--rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-06-21 06:21:17.000000 fake-bpy-module-latest-20230621/bl_operators/assets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 06:23:21.000000 fake-bpy-module-latest-20230621/bl_operators/bmesh/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-21 06:21:12.000000 fake-bpy-module-latest-20230621/bl_operators/bmesh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-21 06:21:12.000000 fake-bpy-module-latest-20230621/bl_operators/bmesh/find_adjacent.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 06:12:54.000000 fake-bpy-module-latest-20230621/bl_operators/bmesh/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    22556 2023-06-21 06:21:14.000000 fake-bpy-module-latest-20230621/bl_operators/clip.py
--rw-r--r--   0 runner    (1001) docker     (123)    10879 2023-06-21 06:21:14.000000 fake-bpy-module-latest-20230621/bl_operators/console.py
--rw-r--r--   0 runner    (1001) docker     (123)     8896 2023-06-21 06:21:14.000000 fake-bpy-module-latest-20230621/bl_operators/constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)     6730 2023-06-21 06:21:12.000000 fake-bpy-module-latest-20230621/bl_operators/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     9017 2023-06-21 06:21:17.000000 fake-bpy-module-latest-20230621/bl_operators/freestyle.py
--rw-r--r--   0 runner    (1001) docker     (123)    15010 2023-06-21 06:21:18.000000 fake-bpy-module-latest-20230621/bl_operators/geometry_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6510 2023-06-21 06:21:12.000000 fake-bpy-module-latest-20230621/bl_operators/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-06-21 06:21:12.000000 fake-bpy-module-latest-20230621/bl_operators/mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    18689 2023-06-21 06:21:14.000000 fake-bpy-module-latest-20230621/bl_operators/node.py
--rw-r--r--   0 runner    (1001) docker     (123)    38122 2023-06-21 06:21:17.000000 fake-bpy-module-latest-20230621/bl_operators/object.py
--rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-06-21 06:21:14.000000 fake-bpy-module-latest-20230621/bl_operators/object_align.py
--rw-r--r--   0 runner    (1001) docker     (123)     9176 2023-06-21 06:21:12.000000 fake-bpy-module-latest-20230621/bl_operators/object_quick_effects.py
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-06-21 06:21:17.000000 fake-bpy-module-latest-20230621/bl_operators/object_randomize_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)    45483 2023-06-21 06:21:17.000000 fake-bpy-module-latest-20230621/bl_operators/presets.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 06:12:54.000000 fake-bpy-module-latest-20230621/bl_operators/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     6733 2023-06-21 06:21:16.000000 fake-bpy-module-latest-20230621/bl_operators/rigidbody.py
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-06-21 06:21:14.000000 fake-bpy-module-latest-20230621/bl_operators/screen_play_rendered_anim.py
--rw-r--r--   0 runner    (1001) docker     (123)    12099 2023-06-21 06:21:12.000000 fake-bpy-module-latest-20230621/bl_operators/sequencer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-06-21 06:21:18.000000 fake-bpy-module-latest-20230621/bl_operators/spreadsheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-06-21 06:21:17.000000 fake-bpy-module-latest-20230621/bl_operators/text.py
--rw-r--r--   0 runner    (1001) docker     (123)    56119 2023-06-21 06:21:13.000000 fake-bpy-module-latest-20230621/bl_operators/userpref.py
--rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-06-21 06:21:17.000000 fake-bpy-module-latest-20230621/bl_operators/uvcalc_follow_active.py
--rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-06-21 06:21:12.000000 fake-bpy-module-latest-20230621/bl_operators/uvcalc_lightmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     5708 2023-06-21 06:21:12.000000 fake-bpy-module-latest-20230621/bl_operators/uvcalc_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-06-21 06:21:14.000000 fake-bpy-module-latest-20230621/bl_operators/vertexpaint_dirt.py
--rw-r--r--   0 runner    (1001) docker     (123)    11547 2023-06-21 06:21:17.000000 fake-bpy-module-latest-20230621/bl_operators/view3d.py
--rw-r--r--   0 runner    (1001) docker     (123)    97916 2023-06-21 06:21:16.000000 fake-bpy-module-latest-20230621/bl_operators/wm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 06:23:21.000000 fake-bpy-module-latest-20230621/bl_previews_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-21 06:21:12.000000 fake-bpy-module-latest-20230621/bl_previews_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-21 06:21:12.000000 fake-bpy-module-latest-20230621/bl_previews_utils/bl_previews_render.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 06:12:54.000000 fake-bpy-module-latest-20230621/bl_previews_utils/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 06:23:21.000000 fake-bpy-module-latest-20230621/bl_rna_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-21 06:21:12.000000 fake-bpy-module-latest-20230621/bl_rna_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-21 06:21:12.000000 fake-bpy-module-latest-20230621/bl_rna_utils/data_path.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 06:12:54.000000 fake-bpy-module-latest-20230621/bl_rna_utils/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 06:23:21.000000 fake-bpy-module-latest-20230621/bl_ui/
--rw-r--r--   0 runner    (1001) docker     (123)    10249 2023-06-21 06:21:18.000000 fake-bpy-module-latest-20230621/bl_ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7770 2023-06-21 06:23:12.000000 fake-bpy-module-latest-20230621/bl_ui/generic_ui_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-21 06:21:30.000000 fake-bpy-module-latest-20230621/bl_ui/node_add_menu.py
--rw-r--r--   0 runner    (1001) docker     (123)   110864 2023-06-21 06:22:09.000000 fake-bpy-module-latest-20230621/bl_ui/node_add_menu_geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-21 06:21:59.000000 fake-bpy-module-latest-20230621/bl_ui/properties_animviz.py
--rw-r--r--   0 runner    (1001) docker     (123)    13049 2023-06-21 06:23:18.000000 fake-bpy-module-latest-20230621/bl_ui/properties_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)   385296 2023-06-21 06:21:30.000000 fake-bpy-module-latest-20230621/bl_ui/properties_constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)    25330 2023-06-21 06:22:04.000000 fake-bpy-module-latest-20230621/bl_ui/properties_data_armature.py
--rw-r--r--   0 runner    (1001) docker     (123)    22602 2023-06-21 06:23:14.000000 fake-bpy-module-latest-20230621/bl_ui/properties_data_bone.py
--rw-r--r--   0 runner    (1001) docker     (123)    36945 2023-06-21 06:22:03.000000 fake-bpy-module-latest-20230621/bl_ui/properties_data_camera.py
--rw-r--r--   0 runner    (1001) docker     (123)    38857 2023-06-21 06:21:33.000000 fake-bpy-module-latest-20230621/bl_ui/properties_data_curve.py
--rw-r--r--   0 runner    (1001) docker     (123)    15423 2023-06-21 06:21:34.000000 fake-bpy-module-latest-20230621/bl_ui/properties_data_curves.py
--rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-06-21 06:21:34.000000 fake-bpy-module-latest-20230621/bl_ui/properties_data_empty.py
--rw-r--r--   0 runner    (1001) docker     (123)    46403 2023-06-21 06:22:02.000000 fake-bpy-module-latest-20230621/bl_ui/properties_data_gpencil.py
--rw-r--r--   0 runner    (1001) docker     (123)     7776 2023-06-21 06:21:58.000000 fake-bpy-module-latest-20230621/bl_ui/properties_data_lattice.py
--rw-r--r--   0 runner    (1001) docker     (123)    28154 2023-06-21 06:21:57.000000 fake-bpy-module-latest-20230621/bl_ui/properties_data_light.py
--rw-r--r--   0 runner    (1001) docker     (123)    12933 2023-06-21 06:21:18.000000 fake-bpy-module-latest-20230621/bl_ui/properties_data_lightprobe.py
--rw-r--r--   0 runner    (1001) docker     (123)    52746 2023-06-21 06:22:07.000000 fake-bpy-module-latest-20230621/bl_ui/properties_data_mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    12806 2023-06-21 06:21:49.000000 fake-bpy-module-latest-20230621/bl_ui/properties_data_metaball.py
--rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-06-21 06:23:09.000000 fake-bpy-module-latest-20230621/bl_ui/properties_data_modifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    13050 2023-06-21 06:23:14.000000 fake-bpy-module-latest-20230621/bl_ui/properties_data_pointcloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-06-21 06:22:01.000000 fake-bpy-module-latest-20230621/bl_ui/properties_data_shaderfx.py
--rw-r--r--   0 runner    (1001) docker     (123)    12829 2023-06-21 06:21:49.000000 fake-bpy-module-latest-20230621/bl_ui/properties_data_speaker.py
--rw-r--r--   0 runner    (1001) docker     (123)    20178 2023-06-21 06:21:32.000000 fake-bpy-module-latest-20230621/bl_ui/properties_data_volume.py
--rw-r--r--   0 runner    (1001) docker     (123)    66640 2023-06-21 06:21:58.000000 fake-bpy-module-latest-20230621/bl_ui/properties_freestyle.py
--rw-r--r--   0 runner    (1001) docker     (123)    32219 2023-06-21 06:22:11.000000 fake-bpy-module-latest-20230621/bl_ui/properties_grease_pencil_common.py
--rw-r--r--   0 runner    (1001) docker     (123)    19327 2023-06-21 06:21:32.000000 fake-bpy-module-latest-20230621/bl_ui/properties_mask_common.py
--rw-r--r--   0 runner    (1001) docker     (123)    30514 2023-06-21 06:21:34.000000 fake-bpy-module-latest-20230621/bl_ui/properties_material.py
--rw-r--r--   0 runner    (1001) docker     (123)    25892 2023-06-21 06:21:47.000000 fake-bpy-module-latest-20230621/bl_ui/properties_material_gpencil.py
--rw-r--r--   0 runner    (1001) docker     (123)    35174 2023-06-21 06:23:14.000000 fake-bpy-module-latest-20230621/bl_ui/properties_object.py
--rw-r--r--   0 runner    (1001) docker     (123)    46745 2023-06-21 06:21:32.000000 fake-bpy-module-latest-20230621/bl_ui/properties_output.py
--rw-r--r--   0 runner    (1001) docker     (123)    12467 2023-06-21 06:22:07.000000 fake-bpy-module-latest-20230621/bl_ui/properties_paint_common.py
--rw-r--r--   0 runner    (1001) docker     (123)   133597 2023-06-21 06:23:11.000000 fake-bpy-module-latest-20230621/bl_ui/properties_particle.py
--rw-r--r--   0 runner    (1001) docker     (123)    36563 2023-06-21 06:22:01.000000 fake-bpy-module-latest-20230621/bl_ui/properties_physics_cloth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-06-21 06:22:07.000000 fake-bpy-module-latest-20230621/bl_ui/properties_physics_common.py
--rw-r--r--   0 runner    (1001) docker     (123)    67584 2023-06-21 06:23:16.000000 fake-bpy-module-latest-20230621/bl_ui/properties_physics_dynamicpaint.py
--rw-r--r--   0 runner    (1001) docker     (123)    27217 2023-06-21 06:21:39.000000 fake-bpy-module-latest-20230621/bl_ui/properties_physics_field.py
--rw-r--r--   0 runner    (1001) docker     (123)    91307 2023-06-21 06:23:17.000000 fake-bpy-module-latest-20230621/bl_ui/properties_physics_fluid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-06-21 06:21:57.000000 fake-bpy-module-latest-20230621/bl_ui/properties_physics_geometry_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)    20769 2023-06-21 06:22:04.000000 fake-bpy-module-latest-20230621/bl_ui/properties_physics_rigidbody.py
--rw-r--r--   0 runner    (1001) docker     (123)    33547 2023-06-21 06:22:01.000000 fake-bpy-module-latest-20230621/bl_ui/properties_physics_rigidbody_constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)    39030 2023-06-21 06:23:12.000000 fake-bpy-module-latest-20230621/bl_ui/properties_physics_softbody.py
--rw-r--r--   0 runner    (1001) docker     (123)    89468 2023-06-21 06:22:06.000000 fake-bpy-module-latest-20230621/bl_ui/properties_render.py
--rw-r--r--   0 runner    (1001) docker     (123)    32886 2023-06-21 06:22:02.000000 fake-bpy-module-latest-20230621/bl_ui/properties_scene.py
--rw-r--r--   0 runner    (1001) docker     (123)    66952 2023-06-21 06:21:34.000000 fake-bpy-module-latest-20230621/bl_ui/properties_texture.py
--rw-r--r--   0 runner    (1001) docker     (123)    37695 2023-06-21 06:21:19.000000 fake-bpy-module-latest-20230621/bl_ui/properties_view_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7748 2023-06-21 06:21:58.000000 fake-bpy-module-latest-20230621/bl_ui/properties_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)    15459 2023-06-21 06:23:17.000000 fake-bpy-module-latest-20230621/bl_ui/properties_world.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 06:12:54.000000 fake-bpy-module-latest-20230621/bl_ui/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   176850 2023-06-21 06:21:38.000000 fake-bpy-module-latest-20230621/bl_ui/space_clip.py
--rw-r--r--   0 runner    (1001) docker     (123)    15218 2023-06-21 06:23:18.000000 fake-bpy-module-latest-20230621/bl_ui/space_console.py
--rw-r--r--   0 runner    (1001) docker     (123)    64929 2023-06-21 06:21:59.000000 fake-bpy-module-latest-20230621/bl_ui/space_dopesheet.py
--rw-r--r--   0 runner    (1001) docker     (123)    71853 2023-06-21 06:23:13.000000 fake-bpy-module-latest-20230621/bl_ui/space_filebrowser.py
--rw-r--r--   0 runner    (1001) docker     (123)    50899 2023-06-21 06:22:10.000000 fake-bpy-module-latest-20230621/bl_ui/space_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)   187053 2023-06-21 06:21:47.000000 fake-bpy-module-latest-20230621/bl_ui/space_image.py
--rw-r--r--   0 runner    (1001) docker     (123)    15172 2023-06-21 06:23:17.000000 fake-bpy-module-latest-20230621/bl_ui/space_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    38361 2023-06-21 06:23:03.000000 fake-bpy-module-latest-20230621/bl_ui/space_nla.py
--rw-r--r--   0 runner    (1001) docker     (123)    75065 2023-06-21 06:22:11.000000 fake-bpy-module-latest-20230621/bl_ui/space_node.py
--rw-r--r--   0 runner    (1001) docker     (123)    35830 2023-06-21 06:22:04.000000 fake-bpy-module-latest-20230621/bl_ui/space_outliner.py
--rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-06-21 06:22:07.000000 fake-bpy-module-latest-20230621/bl_ui/space_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)   182398 2023-06-21 06:21:43.000000 fake-bpy-module-latest-20230621/bl_ui/space_sequencer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-06-21 06:23:03.000000 fake-bpy-module-latest-20230621/bl_ui/space_spreadsheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-06-21 06:21:30.000000 fake-bpy-module-latest-20230621/bl_ui/space_statusbar.py
--rw-r--r--   0 runner    (1001) docker     (123)    40008 2023-06-21 06:22:01.000000 fake-bpy-module-latest-20230621/bl_ui/space_text.py
--rw-r--r--   0 runner    (1001) docker     (123)    18254 2023-06-21 06:23:14.000000 fake-bpy-module-latest-20230621/bl_ui/space_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     5550 2023-06-21 06:23:09.000000 fake-bpy-module-latest-20230621/bl_ui/space_toolsystem_common.py
--rw-r--r--   0 runner    (1001) docker     (123)    21636 2023-06-21 06:23:18.000000 fake-bpy-module-latest-20230621/bl_ui/space_toolsystem_toolbar.py
--rw-r--r--   0 runner    (1001) docker     (123)    65863 2023-06-21 06:21:48.000000 fake-bpy-module-latest-20230621/bl_ui/space_topbar.py
--rw-r--r--   0 runner    (1001) docker     (123)   215185 2023-06-21 06:23:07.000000 fake-bpy-module-latest-20230621/bl_ui/space_userpref.py
--rw-r--r--   0 runner    (1001) docker     (123)   616417 2023-06-21 06:23:03.000000 fake-bpy-module-latest-20230621/bl_ui/space_view3d.py
--rw-r--r--   0 runner    (1001) docker     (123)   239548 2023-06-21 06:21:57.000000 fake-bpy-module-latest-20230621/bl_ui/space_view3d_toolbar.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-21 06:23:14.000000 fake-bpy-module-latest-20230621/bl_ui/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 06:23:21.000000 fake-bpy-module-latest-20230621/bl_ui_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-21 06:23:18.000000 fake-bpy-module-latest-20230621/bl_ui_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-21 06:23:18.000000 fake-bpy-module-latest-20230621/bl_ui_utils/bug_report_url.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-21 06:23:18.000000 fake-bpy-module-latest-20230621/bl_ui_utils/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 06:12:54.000000 fake-bpy-module-latest-20230621/bl_ui_utils/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-21 06:21:18.000000 fake-bpy-module-latest-20230621/blend_render_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     5137 2023-06-21 06:21:05.000000 fake-bpy-module-latest-20230621/blf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 06:23:21.000000 fake-bpy-module-latest-20230621/bmesh/
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-06-21 06:21:08.000000 fake-bpy-module-latest-20230621/bmesh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-21 06:21:08.000000 fake-bpy-module-latest-20230621/bmesh/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)    77492 2023-06-21 06:21:11.000000 fake-bpy-module-latest-20230621/bmesh/ops.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 06:12:54.000000 fake-bpy-module-latest-20230621/bmesh/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    36665 2023-06-21 06:21:11.000000 fake-bpy-module-latest-20230621/bmesh/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     6511 2023-06-21 06:21:11.000000 fake-bpy-module-latest-20230621/bmesh/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 06:23:21.000000 fake-bpy-module-latest-20230621/bpy/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-21 06:12:54.000000 fake-bpy-module-latest-20230621/bpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 06:23:21.000000 fake-bpy-module-latest-20230621/bpy/app/
--rw-r--r--   0 runner    (1001) docker     (123)     7378 2023-06-21 06:21:02.000000 fake-bpy-module-latest-20230621/bpy/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5543 2023-06-21 06:21:03.000000 fake-bpy-module-latest-20230621/bpy/app/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-06-21 06:21:02.000000 fake-bpy-module-latest-20230621/bpy/app/icons.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 06:12:54.000000 fake-bpy-module-latest-20230621/bpy/app/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-06-21 06:21:02.000000 fake-bpy-module-latest-20230621/bpy/app/timers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-06-21 06:21:03.000000 fake-bpy-module-latest-20230621/bpy/app/translations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-06-21 06:21:03.000000 fake-bpy-module-latest-20230621/bpy/msgbus.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 06:23:21.000000 fake-bpy-module-latest-20230621/bpy/ops/
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-21 06:20:20.000000 fake-bpy-module-latest-20230621/bpy/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27608 2023-06-21 06:20:44.000000 fake-bpy-module-latest-20230621/bpy/ops/action.py
--rw-r--r--   0 runner    (1001) docker     (123)    35886 2023-06-21 06:20:52.000000 fake-bpy-module-latest-20230621/bpy/ops/anim.py
--rw-r--r--   0 runner    (1001) docker     (123)    25486 2023-06-21 06:21:02.000000 fake-bpy-module-latest-20230621/bpy/ops/armature.py
--rw-r--r--   0 runner    (1001) docker     (123)    13048 2023-06-21 06:20:59.000000 fake-bpy-module-latest-20230621/bpy/ops/asset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-06-21 06:20:42.000000 fake-bpy-module-latest-20230621/bpy/ops/boid.py
--rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-06-21 06:20:43.000000 fake-bpy-module-latest-20230621/bpy/ops/brush.py
--rw-r--r--   0 runner    (1001) docker     (123)    12217 2023-06-21 06:20:59.000000 fake-bpy-module-latest-20230621/bpy/ops/buttons.py
--rw-r--r--   0 runner    (1001) docker     (123)    11603 2023-06-21 06:20:48.000000 fake-bpy-module-latest-20230621/bpy/ops/cachefile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-06-21 06:20:48.000000 fake-bpy-module-latest-20230621/bpy/ops/camera.py
--rw-r--r--   0 runner    (1001) docker     (123)    70588 2023-06-21 06:20:55.000000 fake-bpy-module-latest-20230621/bpy/ops/clip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-06-21 06:20:31.000000 fake-bpy-module-latest-20230621/bpy/ops/cloth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-06-21 06:20:43.000000 fake-bpy-module-latest-20230621/bpy/ops/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)    12767 2023-06-21 06:20:43.000000 fake-bpy-module-latest-20230621/bpy/ops/console.py
--rw-r--r--   0 runner    (1001) docker     (123)    17809 2023-06-21 06:20:50.000000 fake-bpy-module-latest-20230621/bpy/ops/constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)    40670 2023-06-21 06:20:31.000000 fake-bpy-module-latest-20230621/bpy/ops/curve.py
--rw-r--r--   0 runner    (1001) docker     (123)     8236 2023-06-21 06:20:43.000000 fake-bpy-module-latest-20230621/bpy/ops/curves.py
--rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-06-21 06:20:44.000000 fake-bpy-module-latest-20230621/bpy/ops/cycles.py
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-06-21 06:20:44.000000 fake-bpy-module-latest-20230621/bpy/ops/dpaint.py
--rw-r--r--   0 runner    (1001) docker     (123)    10721 2023-06-21 06:20:36.000000 fake-bpy-module-latest-20230621/bpy/ops/ed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-06-21 06:20:31.000000 fake-bpy-module-latest-20230621/bpy/ops/export_anim.py
--rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-06-21 06:20:56.000000 fake-bpy-module-latest-20230621/bpy/ops/export_mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    35992 2023-06-21 06:20:46.000000 fake-bpy-module-latest-20230621/bpy/ops/export_scene.py
--rw-r--r--   0 runner    (1001) docker     (123)    30339 2023-06-21 06:20:43.000000 fake-bpy-module-latest-20230621/bpy/ops/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     7036 2023-06-21 06:20:43.000000 fake-bpy-module-latest-20230621/bpy/ops/fluid.py
--rw-r--r--   0 runner    (1001) docker     (123)    21051 2023-06-21 06:21:01.000000 fake-bpy-module-latest-20230621/bpy/ops/font.py
--rw-r--r--   0 runner    (1001) docker     (123)     6339 2023-06-21 06:20:52.000000 fake-bpy-module-latest-20230621/bpy/ops/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-06-21 06:20:54.000000 fake-bpy-module-latest-20230621/bpy/ops/gizmogroup.py
--rw-r--r--   0 runner    (1001) docker     (123)   132520 2023-06-21 06:20:34.000000 fake-bpy-module-latest-20230621/bpy/ops/gpencil.py
--rw-r--r--   0 runner    (1001) docker     (123)    50489 2023-06-21 06:20:36.000000 fake-bpy-module-latest-20230621/bpy/ops/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     5863 2023-06-21 06:20:42.000000 fake-bpy-module-latest-20230621/bpy/ops/grease_pencil.py
--rw-r--r--   0 runner    (1001) docker     (123)    53280 2023-06-21 06:21:01.000000 fake-bpy-module-latest-20230621/bpy/ops/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-06-21 06:21:01.000000 fake-bpy-module-latest-20230621/bpy/ops/import_anim.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-21 06:20:55.000000 fake-bpy-module-latest-20230621/bpy/ops/import_curve.py
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-06-21 06:20:43.000000 fake-bpy-module-latest-20230621/bpy/ops/import_mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    11561 2023-06-21 06:20:31.000000 fake-bpy-module-latest-20230621/bpy/ops/import_scene.py
--rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-06-21 06:20:28.000000 fake-bpy-module-latest-20230621/bpy/ops/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-06-21 06:20:48.000000 fake-bpy-module-latest-20230621/bpy/ops/lattice.py
--rw-r--r--   0 runner    (1001) docker     (123)     8761 2023-06-21 06:20:51.000000 fake-bpy-module-latest-20230621/bpy/ops/marker.py
--rw-r--r--   0 runner    (1001) docker     (123)    27162 2023-06-21 06:20:44.000000 fake-bpy-module-latest-20230621/bpy/ops/mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-06-21 06:20:49.000000 fake-bpy-module-latest-20230621/bpy/ops/material.py
--rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-06-21 06:20:43.000000 fake-bpy-module-latest-20230621/bpy/ops/mball.py
--rw-r--r--   0 runner    (1001) docker     (123)   179170 2023-06-21 06:20:59.000000 fake-bpy-module-latest-20230621/bpy/ops/mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    28691 2023-06-21 06:20:42.000000 fake-bpy-module-latest-20230621/bpy/ops/nla.py
--rw-r--r--   0 runner    (1001) docker     (123)    72286 2023-06-21 06:20:35.000000 fake-bpy-module-latest-20230621/bpy/ops/node.py
--rw-r--r--   0 runner    (1001) docker     (123)   225774 2023-06-21 06:20:40.000000 fake-bpy-module-latest-20230621/bpy/ops/object.py
--rw-r--r--   0 runner    (1001) docker     (123)    44201 2023-06-21 06:20:47.000000 fake-bpy-module-latest-20230621/bpy/ops/outliner.py
--rw-r--r--   0 runner    (1001) docker     (123)    44093 2023-06-21 06:20:49.000000 fake-bpy-module-latest-20230621/bpy/ops/paint.py
--rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-06-21 06:20:49.000000 fake-bpy-module-latest-20230621/bpy/ops/paintcurve.py
--rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-06-21 06:20:44.000000 fake-bpy-module-latest-20230621/bpy/ops/palette.py
--rw-r--r--   0 runner    (1001) docker     (123)    22863 2023-06-21 06:20:48.000000 fake-bpy-module-latest-20230621/bpy/ops/particle.py
--rw-r--r--   0 runner    (1001) docker     (123)    39854 2023-06-21 06:20:51.000000 fake-bpy-module-latest-20230621/bpy/ops/pose.py
--rw-r--r--   0 runner    (1001) docker     (123)     7616 2023-06-21 06:20:48.000000 fake-bpy-module-latest-20230621/bpy/ops/poselib.py
--rw-r--r--   0 runner    (1001) docker     (123)    32889 2023-06-21 06:20:48.000000 fake-bpy-module-latest-20230621/bpy/ops/preferences.py
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-06-21 06:20:44.000000 fake-bpy-module-latest-20230621/bpy/ops/ptcache.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 06:12:54.000000 fake-bpy-module-latest-20230621/bpy/ops/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    11067 2023-06-21 06:20:47.000000 fake-bpy-module-latest-20230621/bpy/ops/render.py
--rw-r--r--   0 runner    (1001) docker     (123)    10108 2023-06-21 06:20:42.000000 fake-bpy-module-latest-20230621/bpy/ops/rigidbody.py
--rw-r--r--   0 runner    (1001) docker     (123)    25220 2023-06-21 06:20:20.000000 fake-bpy-module-latest-20230621/bpy/ops/scene.py
--rw-r--r--   0 runner    (1001) docker     (123)    31884 2023-06-21 06:20:31.000000 fake-bpy-module-latest-20230621/bpy/ops/screen.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-06-21 06:20:49.000000 fake-bpy-module-latest-20230621/bpy/ops/script.py
--rw-r--r--   0 runner    (1001) docker     (123)    46889 2023-06-21 06:20:52.000000 fake-bpy-module-latest-20230621/bpy/ops/sculpt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-06-21 06:20:59.000000 fake-bpy-module-latest-20230621/bpy/ops/sculpt_curves.py
--rw-r--r--   0 runner    (1001) docker     (123)    94657 2023-06-21 06:20:54.000000 fake-bpy-module-latest-20230621/bpy/ops/sequencer.py
--rw-r--r--   0 runner    (1001) docker     (123)    19928 2023-06-21 06:21:02.000000 fake-bpy-module-latest-20230621/bpy/ops/sound.py
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-06-21 06:20:43.000000 fake-bpy-module-latest-20230621/bpy/ops/spreadsheet.py
--rw-r--r--   0 runner    (1001) docker     (123)    10263 2023-06-21 06:20:49.000000 fake-bpy-module-latest-20230621/bpy/ops/surface.py
--rw-r--r--   0 runner    (1001) docker     (123)    32954 2023-06-21 06:21:00.000000 fake-bpy-module-latest-20230621/bpy/ops/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-06-21 06:20:31.000000 fake-bpy-module-latest-20230621/bpy/ops/text_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-06-21 06:20:51.000000 fake-bpy-module-latest-20230621/bpy/ops/texture.py
--rw-r--r--   0 runner    (1001) docker     (123)    72215 2023-06-21 06:20:30.000000 fake-bpy-module-latest-20230621/bpy/ops/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)    19753 2023-06-21 06:20:55.000000 fake-bpy-module-latest-20230621/bpy/ops/ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-06-21 06:20:48.000000 fake-bpy-module-latest-20230621/bpy/ops/uilist.py
--rw-r--r--   0 runner    (1001) docker     (123)    57291 2023-06-21 06:20:41.000000 fake-bpy-module-latest-20230621/bpy/ops/uv.py
--rw-r--r--   0 runner    (1001) docker     (123)    12023 2023-06-21 06:20:51.000000 fake-bpy-module-latest-20230621/bpy/ops/view2d.py
--rw-r--r--   0 runner    (1001) docker     (123)    55643 2023-06-21 06:20:37.000000 fake-bpy-module-latest-20230621/bpy/ops/view3d.py
--rw-r--r--   0 runner    (1001) docker     (123)   246250 2023-06-21 06:20:28.000000 fake-bpy-module-latest-20230621/bpy/ops/wm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-06-21 06:20:51.000000 fake-bpy-module-latest-20230621/bpy/ops/workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-21 06:20:36.000000 fake-bpy-module-latest-20230621/bpy/ops/world.py
--rw-r--r--   0 runner    (1001) docker     (123)     5949 2023-06-21 06:21:03.000000 fake-bpy-module-latest-20230621/bpy/path.py
--rw-r--r--   0 runner    (1001) docker     (123)    29417 2023-06-21 06:21:03.000000 fake-bpy-module-latest-20230621/bpy/props.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 06:12:54.000000 fake-bpy-module-latest-20230621/bpy/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)  3492134 2023-06-21 06:20:20.000000 fake-bpy-module-latest-20230621/bpy/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 06:23:21.000000 fake-bpy-module-latest-20230621/bpy/utils/
--rw-r--r--   0 runner    (1001) docker     (123)    10832 2023-06-21 06:21:03.000000 fake-bpy-module-latest-20230621/bpy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-06-21 06:21:03.000000 fake-bpy-module-latest-20230621/bpy/utils/previews.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 06:12:54.000000 fake-bpy-module-latest-20230621/bpy/utils/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-06-21 06:21:03.000000 fake-bpy-module-latest-20230621/bpy/utils/units.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 06:23:21.000000 fake-bpy-module-latest-20230621/bpy_extras/
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-21 06:21:08.000000 fake-bpy-module-latest-20230621/bpy_extras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-06-21 06:21:08.000000 fake-bpy-module-latest-20230621/bpy_extras/anim_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-21 06:21:08.000000 fake-bpy-module-latest-20230621/bpy_extras/asset_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-21 06:21:08.000000 fake-bpy-module-latest-20230621/bpy_extras/bmesh_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-21 06:21:08.000000 fake-bpy-module-latest-20230621/bpy_extras/id_map_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-06-21 06:21:08.000000 fake-bpy-module-latest-20230621/bpy_extras/image_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-06-21 06:21:08.000000 fake-bpy-module-latest-20230621/bpy_extras/io_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-21 06:21:08.000000 fake-bpy-module-latest-20230621/bpy_extras/keyconfig_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-06-21 06:21:08.000000 fake-bpy-module-latest-20230621/bpy_extras/mesh_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6722 2023-06-21 06:21:08.000000 fake-bpy-module-latest-20230621/bpy_extras/node_shader_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-21 06:21:08.000000 fake-bpy-module-latest-20230621/bpy_extras/node_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-06-21 06:21:08.000000 fake-bpy-module-latest-20230621/bpy_extras/object_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 06:12:54.000000 fake-bpy-module-latest-20230621/bpy_extras/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-06-21 06:21:08.000000 fake-bpy-module-latest-20230621/bpy_extras/view3d_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 06:23:21.000000 fake-bpy-module-latest-20230621/bpy_extras/wm_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-21 06:21:08.000000 fake-bpy-module-latest-20230621/bpy_extras/wm_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-06-21 06:21:08.000000 fake-bpy-module-latest-20230621/bpy_extras/wm_utils/progress_report.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 06:12:54.000000 fake-bpy-module-latest-20230621/bpy_extras/wm_utils/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-21 06:21:12.000000 fake-bpy-module-latest-20230621/bpy_restrict_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    54167 2023-06-21 06:23:19.000000 fake-bpy-module-latest-20230621/bpy_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-21 06:21:12.000000 fake-bpy-module-latest-20230621/console_python.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-21 06:23:19.000000 fake-bpy-module-latest-20230621/console_shell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 06:23:21.000000 fake-bpy-module-latest-20230621/fake_bpy_module_latest.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7193 2023-06-21 06:23:20.000000 fake-bpy-module-latest-20230621/fake_bpy_module_latest.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7832 2023-06-21 06:23:20.000000 fake-bpy-module-latest-20230621/fake_bpy_module_latest.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 06:23:20.000000 fake-bpy-module-latest-20230621/fake_bpy_module_latest.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 06:23:20.000000 fake-bpy-module-latest-20230621/fake_bpy_module_latest.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-21 06:23:20.000000 fake-bpy-module-latest-20230621/fake_bpy_module_latest.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 06:23:21.000000 fake-bpy-module-latest-20230621/freestyle/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-21 06:21:07.000000 fake-bpy-module-latest-20230621/freestyle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9918 2023-06-21 06:21:07.000000 fake-bpy-module-latest-20230621/freestyle/chainingiterators.py
--rw-r--r--   0 runner    (1001) docker     (123)    47908 2023-06-21 06:21:08.000000 fake-bpy-module-latest-20230621/freestyle/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    13232 2023-06-21 06:21:07.000000 fake-bpy-module-latest-20230621/freestyle/predicates.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 06:12:54.000000 fake-bpy-module-latest-20230621/freestyle/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    23737 2023-06-21 06:21:07.000000 fake-bpy-module-latest-20230621/freestyle/shaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    86403 2023-06-21 06:21:07.000000 fake-bpy-module-latest-20230621/freestyle/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 06:23:21.000000 fake-bpy-module-latest-20230621/freestyle/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-06-21 06:21:07.000000 fake-bpy-module-latest-20230621/freestyle/utils/ContextFunctions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5644 2023-06-21 06:21:07.000000 fake-bpy-module-latest-20230621/freestyle/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 06:12:54.000000 fake-bpy-module-latest-20230621/freestyle/utils/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 06:23:21.000000 fake-bpy-module-latest-20230621/gpu/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-21 06:21:06.000000 fake-bpy-module-latest-20230621/gpu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-06-21 06:21:06.000000 fake-bpy-module-latest-20230621/gpu/capabilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-06-21 06:21:06.000000 fake-bpy-module-latest-20230621/gpu/matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-21 06:21:06.000000 fake-bpy-module-latest-20230621/gpu/platform.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 06:12:54.000000 fake-bpy-module-latest-20230621/gpu/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-21 06:21:06.000000 fake-bpy-module-latest-20230621/gpu/select.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-06-21 06:21:06.000000 fake-bpy-module-latest-20230621/gpu/shader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-06-21 06:21:07.000000 fake-bpy-module-latest-20230621/gpu/state.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-21 06:21:06.000000 fake-bpy-module-latest-20230621/gpu/texture.py
--rw-r--r--   0 runner    (1001) docker     (123)    26992 2023-06-21 06:21:06.000000 fake-bpy-module-latest-20230621/gpu/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 06:23:21.000000 fake-bpy-module-latest-20230621/gpu_extras/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-21 06:21:07.000000 fake-bpy-module-latest-20230621/gpu_extras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-21 06:21:07.000000 fake-bpy-module-latest-20230621/gpu_extras/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-06-21 06:21:07.000000 fake-bpy-module-latest-20230621/gpu_extras/presets.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 06:12:54.000000 fake-bpy-module-latest-20230621/gpu_extras/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-21 06:21:12.000000 fake-bpy-module-latest-20230621/graphviz_export.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 06:23:21.000000 fake-bpy-module-latest-20230621/idprop/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-21 06:21:11.000000 fake-bpy-module-latest-20230621/idprop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 06:12:54.000000 fake-bpy-module-latest-20230621/idprop/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-06-21 06:21:11.000000 fake-bpy-module-latest-20230621/idprop/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 06:23:21.000000 fake-bpy-module-latest-20230621/imbuf/
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-06-21 06:21:11.000000 fake-bpy-module-latest-20230621/imbuf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 06:12:54.000000 fake-bpy-module-latest-20230621/imbuf/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-06-21 06:21:11.000000 fake-bpy-module-latest-20230621/imbuf/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    48637 2023-06-21 06:21:12.000000 fake-bpy-module-latest-20230621/keyingsets_builtins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-21 06:21:12.000000 fake-bpy-module-latest-20230621/keyingsets_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 06:23:21.000000 fake-bpy-module-latest-20230621/mathutils/
--rw-r--r--   0 runner    (1001) docker     (123)    86215 2023-06-21 06:21:06.000000 fake-bpy-module-latest-20230621/mathutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-06-21 06:21:06.000000 fake-bpy-module-latest-20230621/mathutils/bvhtree.py
--rw-r--r--   0 runner    (1001) docker     (123)    22187 2023-06-21 06:21:06.000000 fake-bpy-module-latest-20230621/mathutils/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-21 06:21:06.000000 fake-bpy-module-latest-20230621/mathutils/interpolate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-06-21 06:21:06.000000 fake-bpy-module-latest-20230621/mathutils/kdtree.py
--rw-r--r--   0 runner    (1001) docker     (123)    13248 2023-06-21 06:21:06.000000 fake-bpy-module-latest-20230621/mathutils/noise.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 06:12:54.000000 fake-bpy-module-latest-20230621/mathutils/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-06-21 06:23:19.000000 fake-bpy-module-latest-20230621/nodeitems_builtins.py
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-21 06:23:19.000000 fake-bpy-module-latest-20230621/nodeitems_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-06-21 06:21:18.000000 fake-bpy-module-latest-20230621/rna_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-21 06:23:19.000000 fake-bpy-module-latest-20230621/rna_keymap_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-06-21 06:21:12.000000 fake-bpy-module-latest-20230621/rna_prop_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-21 06:21:12.000000 fake-bpy-module-latest-20230621/rna_xml.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 06:23:21.000000 fake-bpy-module-latest-20230621/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-06-21 06:23:20.000000 fake-bpy-module-latest-20230621/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-21 06:23:19.000000 fake-bpy-module-latest-20230621/sys_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 06:24:01.000000 fake-bpy-module-latest-20230622/
+-rw-r--r--   0 runner    (1001) docker     (123)     7193 2023-06-22 06:24:01.000000 fake-bpy-module-latest-20230622/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4958 2023-06-22 06:24:00.000000 fake-bpy-module-latest-20230622/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-22 06:23:57.000000 fake-bpy-module-latest-20230622/addon_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-22 06:23:59.000000 fake-bpy-module-latest-20230622/animsys_refactor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30417 2023-06-22 06:21:48.000000 fake-bpy-module-latest-20230622/aud.py
+-rw-r--r--   0 runner    (1001) docker     (123)   116266 2023-06-22 06:21:45.000000 fake-bpy-module-latest-20230622/bgl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 06:24:00.000000 fake-bpy-module-latest-20230622/bl_app_override/
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-22 06:23:59.000000 fake-bpy-module-latest-20230622/bl_app_override/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-22 06:23:59.000000 fake-bpy-module-latest-20230622/bl_app_override/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 06:13:37.000000 fake-bpy-module-latest-20230622/bl_app_override/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-22 06:23:59.000000 fake-bpy-module-latest-20230622/bl_app_template_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 06:24:00.000000 fake-bpy-module-latest-20230622/bl_console_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-22 06:23:59.000000 fake-bpy-module-latest-20230622/bl_console_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 06:24:00.000000 fake-bpy-module-latest-20230622/bl_console_utils/autocomplete/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-22 06:23:59.000000 fake-bpy-module-latest-20230622/bl_console_utils/autocomplete/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-06-22 06:23:59.000000 fake-bpy-module-latest-20230622/bl_console_utils/autocomplete/complete_calltip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-22 06:23:59.000000 fake-bpy-module-latest-20230622/bl_console_utils/autocomplete/complete_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-22 06:23:59.000000 fake-bpy-module-latest-20230622/bl_console_utils/autocomplete/complete_namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-22 06:23:59.000000 fake-bpy-module-latest-20230622/bl_console_utils/autocomplete/intellisense.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 06:13:37.000000 fake-bpy-module-latest-20230622/bl_console_utils/autocomplete/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 06:13:37.000000 fake-bpy-module-latest-20230622/bl_console_utils/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 06:24:00.000000 fake-bpy-module-latest-20230622/bl_i18n_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-22 06:23:59.000000 fake-bpy-module-latest-20230622/bl_i18n_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-22 06:23:59.000000 fake-bpy-module-latest-20230622/bl_i18n_utils/bl_extract_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-22 06:23:59.000000 fake-bpy-module-latest-20230622/bl_i18n_utils/merge_po.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 06:13:37.000000 fake-bpy-module-latest-20230622/bl_i18n_utils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-22 06:23:59.000000 fake-bpy-module-latest-20230622/bl_i18n_utils/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-06-22 06:23:59.000000 fake-bpy-module-latest-20230622/bl_i18n_utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-22 06:23:59.000000 fake-bpy-module-latest-20230622/bl_i18n_utils/utils_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-22 06:23:59.000000 fake-bpy-module-latest-20230622/bl_i18n_utils/utils_languages_menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-22 06:23:59.000000 fake-bpy-module-latest-20230622/bl_i18n_utils/utils_rtl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 06:24:00.000000 fake-bpy-module-latest-20230622/bl_keymap_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-22 06:23:59.000000 fake-bpy-module-latest-20230622/bl_keymap_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-22 06:23:59.000000 fake-bpy-module-latest-20230622/bl_keymap_utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-22 06:23:59.000000 fake-bpy-module-latest-20230622/bl_keymap_utils/keymap_from_toolbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-22 06:23:59.000000 fake-bpy-module-latest-20230622/bl_keymap_utils/keymap_hierarchy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-22 06:23:59.000000 fake-bpy-module-latest-20230622/bl_keymap_utils/platform_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 06:13:37.000000 fake-bpy-module-latest-20230622/bl_keymap_utils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-22 06:23:59.000000 fake-bpy-module-latest-20230622/bl_keymap_utils/versioning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-06-22 06:21:51.000000 fake-bpy-module-latest-20230622/bl_math.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 06:24:00.000000 fake-bpy-module-latest-20230622/bl_operators/
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-06-22 06:21:51.000000 fake-bpy-module-latest-20230622/bl_operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-06-22 06:21:52.000000 fake-bpy-module-latest-20230622/bl_operators/add_mesh_torus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8777 2023-06-22 06:21:53.000000 fake-bpy-module-latest-20230622/bl_operators/anim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-06-22 06:21:51.000000 fake-bpy-module-latest-20230622/bl_operators/assets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 06:24:00.000000 fake-bpy-module-latest-20230622/bl_operators/bmesh/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-22 06:21:54.000000 fake-bpy-module-latest-20230622/bl_operators/bmesh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-22 06:21:54.000000 fake-bpy-module-latest-20230622/bl_operators/bmesh/find_adjacent.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 06:13:37.000000 fake-bpy-module-latest-20230622/bl_operators/bmesh/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    22556 2023-06-22 06:21:53.000000 fake-bpy-module-latest-20230622/bl_operators/clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10879 2023-06-22 06:21:51.000000 fake-bpy-module-latest-20230622/bl_operators/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8896 2023-06-22 06:21:53.000000 fake-bpy-module-latest-20230622/bl_operators/constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6730 2023-06-22 06:21:56.000000 fake-bpy-module-latest-20230622/bl_operators/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9017 2023-06-22 06:21:54.000000 fake-bpy-module-latest-20230622/bl_operators/freestyle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15010 2023-06-22 06:21:51.000000 fake-bpy-module-latest-20230622/bl_operators/geometry_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6510 2023-06-22 06:21:54.000000 fake-bpy-module-latest-20230622/bl_operators/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-06-22 06:21:57.000000 fake-bpy-module-latest-20230622/bl_operators/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18689 2023-06-22 06:21:56.000000 fake-bpy-module-latest-20230622/bl_operators/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38122 2023-06-22 06:21:51.000000 fake-bpy-module-latest-20230622/bl_operators/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-06-22 06:21:53.000000 fake-bpy-module-latest-20230622/bl_operators/object_align.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9176 2023-06-22 06:21:53.000000 fake-bpy-module-latest-20230622/bl_operators/object_quick_effects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-06-22 06:21:57.000000 fake-bpy-module-latest-20230622/bl_operators/object_randomize_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45483 2023-06-22 06:21:57.000000 fake-bpy-module-latest-20230622/bl_operators/presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 06:13:37.000000 fake-bpy-module-latest-20230622/bl_operators/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     6733 2023-06-22 06:21:56.000000 fake-bpy-module-latest-20230622/bl_operators/rigidbody.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-06-22 06:21:53.000000 fake-bpy-module-latest-20230622/bl_operators/screen_play_rendered_anim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12099 2023-06-22 06:21:53.000000 fake-bpy-module-latest-20230622/bl_operators/sequencer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-06-22 06:21:57.000000 fake-bpy-module-latest-20230622/bl_operators/spreadsheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-06-22 06:21:57.000000 fake-bpy-module-latest-20230622/bl_operators/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56119 2023-06-22 06:21:53.000000 fake-bpy-module-latest-20230622/bl_operators/userpref.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-06-22 06:21:54.000000 fake-bpy-module-latest-20230622/bl_operators/uvcalc_follow_active.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-06-22 06:21:51.000000 fake-bpy-module-latest-20230622/bl_operators/uvcalc_lightmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5708 2023-06-22 06:21:53.000000 fake-bpy-module-latest-20230622/bl_operators/uvcalc_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-06-22 06:21:55.000000 fake-bpy-module-latest-20230622/bl_operators/vertexpaint_dirt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11547 2023-06-22 06:21:54.000000 fake-bpy-module-latest-20230622/bl_operators/view3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    97916 2023-06-22 06:21:55.000000 fake-bpy-module-latest-20230622/bl_operators/wm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 06:24:00.000000 fake-bpy-module-latest-20230622/bl_previews_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-22 06:23:58.000000 fake-bpy-module-latest-20230622/bl_previews_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-22 06:23:59.000000 fake-bpy-module-latest-20230622/bl_previews_utils/bl_previews_render.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 06:13:37.000000 fake-bpy-module-latest-20230622/bl_previews_utils/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 06:24:00.000000 fake-bpy-module-latest-20230622/bl_rna_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-22 06:23:59.000000 fake-bpy-module-latest-20230622/bl_rna_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-22 06:23:59.000000 fake-bpy-module-latest-20230622/bl_rna_utils/data_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 06:13:37.000000 fake-bpy-module-latest-20230622/bl_rna_utils/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 06:24:01.000000 fake-bpy-module-latest-20230622/bl_ui/
+-rw-r--r--   0 runner    (1001) docker     (123)    10249 2023-06-22 06:21:57.000000 fake-bpy-module-latest-20230622/bl_ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7770 2023-06-22 06:23:45.000000 fake-bpy-module-latest-20230622/bl_ui/generic_ui_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-22 06:22:23.000000 fake-bpy-module-latest-20230622/bl_ui/node_add_menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)   110864 2023-06-22 06:23:54.000000 fake-bpy-module-latest-20230622/bl_ui/node_add_menu_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-22 06:22:07.000000 fake-bpy-module-latest-20230622/bl_ui/properties_animviz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13049 2023-06-22 06:23:54.000000 fake-bpy-module-latest-20230622/bl_ui/properties_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)   385296 2023-06-22 06:22:37.000000 fake-bpy-module-latest-20230622/bl_ui/properties_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25330 2023-06-22 06:23:43.000000 fake-bpy-module-latest-20230622/bl_ui/properties_data_armature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22602 2023-06-22 06:22:47.000000 fake-bpy-module-latest-20230622/bl_ui/properties_data_bone.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36945 2023-06-22 06:21:57.000000 fake-bpy-module-latest-20230622/bl_ui/properties_data_camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38857 2023-06-22 06:23:50.000000 fake-bpy-module-latest-20230622/bl_ui/properties_data_curve.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15423 2023-06-22 06:23:56.000000 fake-bpy-module-latest-20230622/bl_ui/properties_data_curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-06-22 06:22:09.000000 fake-bpy-module-latest-20230622/bl_ui/properties_data_empty.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46403 2023-06-22 06:22:12.000000 fake-bpy-module-latest-20230622/bl_ui/properties_data_gpencil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7776 2023-06-22 06:22:23.000000 fake-bpy-module-latest-20230622/bl_ui/properties_data_lattice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28154 2023-06-22 06:23:44.000000 fake-bpy-module-latest-20230622/bl_ui/properties_data_light.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12933 2023-06-22 06:22:41.000000 fake-bpy-module-latest-20230622/bl_ui/properties_data_lightprobe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52746 2023-06-22 06:22:23.000000 fake-bpy-module-latest-20230622/bl_ui/properties_data_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12806 2023-06-22 06:22:40.000000 fake-bpy-module-latest-20230622/bl_ui/properties_data_metaball.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-06-22 06:23:56.000000 fake-bpy-module-latest-20230622/bl_ui/properties_data_modifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13050 2023-06-22 06:23:57.000000 fake-bpy-module-latest-20230622/bl_ui/properties_data_pointcloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-06-22 06:23:44.000000 fake-bpy-module-latest-20230622/bl_ui/properties_data_shaderfx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12829 2023-06-22 06:22:09.000000 fake-bpy-module-latest-20230622/bl_ui/properties_data_speaker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20178 2023-06-22 06:22:42.000000 fake-bpy-module-latest-20230622/bl_ui/properties_data_volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66640 2023-06-22 06:22:25.000000 fake-bpy-module-latest-20230622/bl_ui/properties_freestyle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32219 2023-06-22 06:22:07.000000 fake-bpy-module-latest-20230622/bl_ui/properties_grease_pencil_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19327 2023-06-22 06:23:45.000000 fake-bpy-module-latest-20230622/bl_ui/properties_mask_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30514 2023-06-22 06:22:51.000000 fake-bpy-module-latest-20230622/bl_ui/properties_material.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25892 2023-06-22 06:22:07.000000 fake-bpy-module-latest-20230622/bl_ui/properties_material_gpencil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35174 2023-06-22 06:23:56.000000 fake-bpy-module-latest-20230622/bl_ui/properties_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46745 2023-06-22 06:22:10.000000 fake-bpy-module-latest-20230622/bl_ui/properties_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12467 2023-06-22 06:22:41.000000 fake-bpy-module-latest-20230622/bl_ui/properties_paint_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)   133597 2023-06-22 06:22:50.000000 fake-bpy-module-latest-20230622/bl_ui/properties_particle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36563 2023-06-22 06:23:52.000000 fake-bpy-module-latest-20230622/bl_ui/properties_physics_cloth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-06-22 06:22:09.000000 fake-bpy-module-latest-20230622/bl_ui/properties_physics_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67584 2023-06-22 06:23:57.000000 fake-bpy-module-latest-20230622/bl_ui/properties_physics_dynamicpaint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27217 2023-06-22 06:22:26.000000 fake-bpy-module-latest-20230622/bl_ui/properties_physics_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)    91307 2023-06-22 06:22:24.000000 fake-bpy-module-latest-20230622/bl_ui/properties_physics_fluid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-06-22 06:23:51.000000 fake-bpy-module-latest-20230622/bl_ui/properties_physics_geometry_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20769 2023-06-22 06:23:49.000000 fake-bpy-module-latest-20230622/bl_ui/properties_physics_rigidbody.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33547 2023-06-22 06:22:21.000000 fake-bpy-module-latest-20230622/bl_ui/properties_physics_rigidbody_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39030 2023-06-22 06:23:51.000000 fake-bpy-module-latest-20230622/bl_ui/properties_physics_softbody.py
+-rw-r--r--   0 runner    (1001) docker     (123)    89468 2023-06-22 06:22:40.000000 fake-bpy-module-latest-20230622/bl_ui/properties_render.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32886 2023-06-22 06:23:51.000000 fake-bpy-module-latest-20230622/bl_ui/properties_scene.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66952 2023-06-22 06:22:11.000000 fake-bpy-module-latest-20230622/bl_ui/properties_texture.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37695 2023-06-22 06:23:55.000000 fake-bpy-module-latest-20230622/bl_ui/properties_view_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7748 2023-06-22 06:23:42.000000 fake-bpy-module-latest-20230622/bl_ui/properties_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15459 2023-06-22 06:22:42.000000 fake-bpy-module-latest-20230622/bl_ui/properties_world.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 06:13:37.000000 fake-bpy-module-latest-20230622/bl_ui/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   176850 2023-06-22 06:23:49.000000 fake-bpy-module-latest-20230622/bl_ui/space_clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15218 2023-06-22 06:23:54.000000 fake-bpy-module-latest-20230622/bl_ui/space_console.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64929 2023-06-22 06:23:43.000000 fake-bpy-module-latest-20230622/bl_ui/space_dopesheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71853 2023-06-22 06:22:09.000000 fake-bpy-module-latest-20230622/bl_ui/space_filebrowser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50899 2023-06-22 06:22:42.000000 fake-bpy-module-latest-20230622/bl_ui/space_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)   187053 2023-06-22 06:22:06.000000 fake-bpy-module-latest-20230622/bl_ui/space_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15172 2023-06-22 06:22:09.000000 fake-bpy-module-latest-20230622/bl_ui/space_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38361 2023-06-22 06:22:41.000000 fake-bpy-module-latest-20230622/bl_ui/space_nla.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75065 2023-06-22 06:22:13.000000 fake-bpy-module-latest-20230622/bl_ui/space_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35830 2023-06-22 06:23:56.000000 fake-bpy-module-latest-20230622/bl_ui/space_outliner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-06-22 06:22:10.000000 fake-bpy-module-latest-20230622/bl_ui/space_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)   182398 2023-06-22 06:22:47.000000 fake-bpy-module-latest-20230622/bl_ui/space_sequencer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-06-22 06:23:49.000000 fake-bpy-module-latest-20230622/bl_ui/space_spreadsheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-06-22 06:23:52.000000 fake-bpy-module-latest-20230622/bl_ui/space_statusbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40008 2023-06-22 06:22:38.000000 fake-bpy-module-latest-20230622/bl_ui/space_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18254 2023-06-22 06:22:10.000000 fake-bpy-module-latest-20230622/bl_ui/space_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5550 2023-06-22 06:23:44.000000 fake-bpy-module-latest-20230622/bl_ui/space_toolsystem_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21636 2023-06-22 06:22:47.000000 fake-bpy-module-latest-20230622/bl_ui/space_toolsystem_toolbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65863 2023-06-22 06:23:50.000000 fake-bpy-module-latest-20230622/bl_ui/space_topbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)   215185 2023-06-22 06:22:02.000000 fake-bpy-module-latest-20230622/bl_ui/space_userpref.py
+-rw-r--r--   0 runner    (1001) docker     (123)   618961 2023-06-22 06:23:42.000000 fake-bpy-module-latest-20230622/bl_ui/space_view3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)   239548 2023-06-22 06:22:21.000000 fake-bpy-module-latest-20230622/bl_ui/space_view3d_toolbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-22 06:22:09.000000 fake-bpy-module-latest-20230622/bl_ui/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 06:24:01.000000 fake-bpy-module-latest-20230622/bl_ui_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-22 06:23:59.000000 fake-bpy-module-latest-20230622/bl_ui_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-22 06:23:59.000000 fake-bpy-module-latest-20230622/bl_ui_utils/bug_report_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-22 06:23:59.000000 fake-bpy-module-latest-20230622/bl_ui_utils/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 06:13:37.000000 fake-bpy-module-latest-20230622/bl_ui_utils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-22 06:23:57.000000 fake-bpy-module-latest-20230622/blend_render_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5137 2023-06-22 06:21:45.000000 fake-bpy-module-latest-20230622/blf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 06:24:01.000000 fake-bpy-module-latest-20230622/bmesh/
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-06-22 06:21:48.000000 fake-bpy-module-latest-20230622/bmesh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-22 06:21:51.000000 fake-bpy-module-latest-20230622/bmesh/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77492 2023-06-22 06:21:50.000000 fake-bpy-module-latest-20230622/bmesh/ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 06:13:37.000000 fake-bpy-module-latest-20230622/bmesh/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    36665 2023-06-22 06:21:51.000000 fake-bpy-module-latest-20230622/bmesh/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6511 2023-06-22 06:21:51.000000 fake-bpy-module-latest-20230622/bmesh/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 06:24:01.000000 fake-bpy-module-latest-20230622/bpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-22 06:13:37.000000 fake-bpy-module-latest-20230622/bpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 06:24:01.000000 fake-bpy-module-latest-20230622/bpy/app/
+-rw-r--r--   0 runner    (1001) docker     (123)     7378 2023-06-22 06:21:42.000000 fake-bpy-module-latest-20230622/bpy/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5543 2023-06-22 06:21:42.000000 fake-bpy-module-latest-20230622/bpy/app/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-06-22 06:21:42.000000 fake-bpy-module-latest-20230622/bpy/app/icons.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 06:13:37.000000 fake-bpy-module-latest-20230622/bpy/app/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-06-22 06:21:42.000000 fake-bpy-module-latest-20230622/bpy/app/timers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-06-22 06:21:42.000000 fake-bpy-module-latest-20230622/bpy/app/translations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-06-22 06:21:43.000000 fake-bpy-module-latest-20230622/bpy/msgbus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 06:24:01.000000 fake-bpy-module-latest-20230622/bpy/ops/
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-22 06:20:59.000000 fake-bpy-module-latest-20230622/bpy/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27608 2023-06-22 06:21:00.000000 fake-bpy-module-latest-20230622/bpy/ops/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35886 2023-06-22 06:21:07.000000 fake-bpy-module-latest-20230622/bpy/ops/anim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25486 2023-06-22 06:21:27.000000 fake-bpy-module-latest-20230622/bpy/ops/armature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13048 2023-06-22 06:21:08.000000 fake-bpy-module-latest-20230622/bpy/ops/asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-06-22 06:21:08.000000 fake-bpy-module-latest-20230622/bpy/ops/boid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-06-22 06:21:20.000000 fake-bpy-module-latest-20230622/bpy/ops/brush.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12217 2023-06-22 06:20:59.000000 fake-bpy-module-latest-20230622/bpy/ops/buttons.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11603 2023-06-22 06:21:23.000000 fake-bpy-module-latest-20230622/bpy/ops/cachefile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-06-22 06:21:29.000000 fake-bpy-module-latest-20230622/bpy/ops/camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70588 2023-06-22 06:21:19.000000 fake-bpy-module-latest-20230622/bpy/ops/clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-06-22 06:21:07.000000 fake-bpy-module-latest-20230622/bpy/ops/cloth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-06-22 06:21:20.000000 fake-bpy-module-latest-20230622/bpy/ops/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12767 2023-06-22 06:21:28.000000 fake-bpy-module-latest-20230622/bpy/ops/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17809 2023-06-22 06:21:38.000000 fake-bpy-module-latest-20230622/bpy/ops/constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40670 2023-06-22 06:21:28.000000 fake-bpy-module-latest-20230622/bpy/ops/curve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8236 2023-06-22 06:21:37.000000 fake-bpy-module-latest-20230622/bpy/ops/curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-06-22 06:21:40.000000 fake-bpy-module-latest-20230622/bpy/ops/cycles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-06-22 06:21:29.000000 fake-bpy-module-latest-20230622/bpy/ops/dpaint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10721 2023-06-22 06:21:07.000000 fake-bpy-module-latest-20230622/bpy/ops/ed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-06-22 06:21:07.000000 fake-bpy-module-latest-20230622/bpy/ops/export_anim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-06-22 06:21:20.000000 fake-bpy-module-latest-20230622/bpy/ops/export_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35992 2023-06-22 06:21:10.000000 fake-bpy-module-latest-20230622/bpy/ops/export_scene.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30339 2023-06-22 06:21:06.000000 fake-bpy-module-latest-20230622/bpy/ops/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7036 2023-06-22 06:21:07.000000 fake-bpy-module-latest-20230622/bpy/ops/fluid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21051 2023-06-22 06:21:20.000000 fake-bpy-module-latest-20230622/bpy/ops/font.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6339 2023-06-22 06:21:06.000000 fake-bpy-module-latest-20230622/bpy/ops/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-06-22 06:21:28.000000 fake-bpy-module-latest-20230622/bpy/ops/gizmogroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)   132520 2023-06-22 06:21:22.000000 fake-bpy-module-latest-20230622/bpy/ops/gpencil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50489 2023-06-22 06:21:08.000000 fake-bpy-module-latest-20230622/bpy/ops/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5863 2023-06-22 06:21:07.000000 fake-bpy-module-latest-20230622/bpy/ops/grease_pencil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53280 2023-06-22 06:21:05.000000 fake-bpy-module-latest-20230622/bpy/ops/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-06-22 06:21:08.000000 fake-bpy-module-latest-20230622/bpy/ops/import_anim.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-22 06:21:40.000000 fake-bpy-module-latest-20230622/bpy/ops/import_curve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-06-22 06:21:28.000000 fake-bpy-module-latest-20230622/bpy/ops/import_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11561 2023-06-22 06:21:12.000000 fake-bpy-module-latest-20230622/bpy/ops/import_scene.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-06-22 06:21:06.000000 fake-bpy-module-latest-20230622/bpy/ops/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-06-22 06:21:05.000000 fake-bpy-module-latest-20230622/bpy/ops/lattice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8761 2023-06-22 06:21:22.000000 fake-bpy-module-latest-20230622/bpy/ops/marker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27162 2023-06-22 06:21:30.000000 fake-bpy-module-latest-20230622/bpy/ops/mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-06-22 06:21:19.000000 fake-bpy-module-latest-20230622/bpy/ops/material.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-06-22 06:21:22.000000 fake-bpy-module-latest-20230622/bpy/ops/mball.py
+-rw-r--r--   0 runner    (1001) docker     (123)   179170 2023-06-22 06:21:26.000000 fake-bpy-module-latest-20230622/bpy/ops/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28691 2023-06-22 06:21:29.000000 fake-bpy-module-latest-20230622/bpy/ops/nla.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72286 2023-06-22 06:21:41.000000 fake-bpy-module-latest-20230622/bpy/ops/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)   225774 2023-06-22 06:21:15.000000 fake-bpy-module-latest-20230622/bpy/ops/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44201 2023-06-22 06:21:00.000000 fake-bpy-module-latest-20230622/bpy/ops/outliner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44093 2023-06-22 06:21:12.000000 fake-bpy-module-latest-20230622/bpy/ops/paint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-06-22 06:21:01.000000 fake-bpy-module-latest-20230622/bpy/ops/paintcurve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-06-22 06:21:41.000000 fake-bpy-module-latest-20230622/bpy/ops/palette.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22863 2023-06-22 06:21:03.000000 fake-bpy-module-latest-20230622/bpy/ops/particle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39854 2023-06-22 06:21:19.000000 fake-bpy-module-latest-20230622/bpy/ops/pose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7616 2023-06-22 06:21:19.000000 fake-bpy-module-latest-20230622/bpy/ops/poselib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32889 2023-06-22 06:21:11.000000 fake-bpy-module-latest-20230622/bpy/ops/preferences.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-06-22 06:21:08.000000 fake-bpy-module-latest-20230622/bpy/ops/ptcache.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 06:13:37.000000 fake-bpy-module-latest-20230622/bpy/ops/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    11067 2023-06-22 06:21:16.000000 fake-bpy-module-latest-20230622/bpy/ops/render.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10108 2023-06-22 06:21:23.000000 fake-bpy-module-latest-20230622/bpy/ops/rigidbody.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25220 2023-06-22 06:21:16.000000 fake-bpy-module-latest-20230622/bpy/ops/scene.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31884 2023-06-22 06:21:27.000000 fake-bpy-module-latest-20230622/bpy/ops/screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-06-22 06:20:59.000000 fake-bpy-module-latest-20230622/bpy/ops/script.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46889 2023-06-22 06:21:42.000000 fake-bpy-module-latest-20230622/bpy/ops/sculpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-06-22 06:21:22.000000 fake-bpy-module-latest-20230622/bpy/ops/sculpt_curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)    94657 2023-06-22 06:21:18.000000 fake-bpy-module-latest-20230622/bpy/ops/sequencer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19928 2023-06-22 06:21:01.000000 fake-bpy-module-latest-20230622/bpy/ops/sound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-06-22 06:21:07.000000 fake-bpy-module-latest-20230622/bpy/ops/spreadsheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10263 2023-06-22 06:21:00.000000 fake-bpy-module-latest-20230622/bpy/ops/surface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32954 2023-06-22 06:21:30.000000 fake-bpy-module-latest-20230622/bpy/ops/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-06-22 06:21:12.000000 fake-bpy-module-latest-20230622/bpy/ops/text_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-06-22 06:21:28.000000 fake-bpy-module-latest-20230622/bpy/ops/texture.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72215 2023-06-22 06:21:40.000000 fake-bpy-module-latest-20230622/bpy/ops/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19753 2023-06-22 06:21:07.000000 fake-bpy-module-latest-20230622/bpy/ops/ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-06-22 06:21:22.000000 fake-bpy-module-latest-20230622/bpy/ops/uilist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57277 2023-06-22 06:21:04.000000 fake-bpy-module-latest-20230622/bpy/ops/uv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12023 2023-06-22 06:21:04.000000 fake-bpy-module-latest-20230622/bpy/ops/view2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55643 2023-06-22 06:21:37.000000 fake-bpy-module-latest-20230622/bpy/ops/view3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)   246250 2023-06-22 06:21:37.000000 fake-bpy-module-latest-20230622/bpy/ops/wm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-06-22 06:21:28.000000 fake-bpy-module-latest-20230622/bpy/ops/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-22 06:21:22.000000 fake-bpy-module-latest-20230622/bpy/ops/world.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5949 2023-06-22 06:21:42.000000 fake-bpy-module-latest-20230622/bpy/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29417 2023-06-22 06:21:43.000000 fake-bpy-module-latest-20230622/bpy/props.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 06:13:37.000000 fake-bpy-module-latest-20230622/bpy/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)  3492236 2023-06-22 06:20:59.000000 fake-bpy-module-latest-20230622/bpy/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 06:24:01.000000 fake-bpy-module-latest-20230622/bpy/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    10832 2023-06-22 06:21:42.000000 fake-bpy-module-latest-20230622/bpy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-06-22 06:21:42.000000 fake-bpy-module-latest-20230622/bpy/utils/previews.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 06:13:37.000000 fake-bpy-module-latest-20230622/bpy/utils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-06-22 06:21:42.000000 fake-bpy-module-latest-20230622/bpy/utils/units.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 06:24:01.000000 fake-bpy-module-latest-20230622/bpy_extras/
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-22 06:21:47.000000 fake-bpy-module-latest-20230622/bpy_extras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-06-22 06:21:47.000000 fake-bpy-module-latest-20230622/bpy_extras/anim_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-22 06:21:47.000000 fake-bpy-module-latest-20230622/bpy_extras/asset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-22 06:21:47.000000 fake-bpy-module-latest-20230622/bpy_extras/bmesh_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-22 06:21:47.000000 fake-bpy-module-latest-20230622/bpy_extras/id_map_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-06-22 06:21:47.000000 fake-bpy-module-latest-20230622/bpy_extras/image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-06-22 06:21:47.000000 fake-bpy-module-latest-20230622/bpy_extras/io_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-22 06:21:47.000000 fake-bpy-module-latest-20230622/bpy_extras/keyconfig_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-06-22 06:21:47.000000 fake-bpy-module-latest-20230622/bpy_extras/mesh_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6722 2023-06-22 06:21:47.000000 fake-bpy-module-latest-20230622/bpy_extras/node_shader_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-22 06:21:47.000000 fake-bpy-module-latest-20230622/bpy_extras/node_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-06-22 06:21:47.000000 fake-bpy-module-latest-20230622/bpy_extras/object_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 06:13:37.000000 fake-bpy-module-latest-20230622/bpy_extras/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-06-22 06:21:47.000000 fake-bpy-module-latest-20230622/bpy_extras/view3d_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 06:24:01.000000 fake-bpy-module-latest-20230622/bpy_extras/wm_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-22 06:21:47.000000 fake-bpy-module-latest-20230622/bpy_extras/wm_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-06-22 06:21:47.000000 fake-bpy-module-latest-20230622/bpy_extras/wm_utils/progress_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 06:13:37.000000 fake-bpy-module-latest-20230622/bpy_extras/wm_utils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-22 06:23:59.000000 fake-bpy-module-latest-20230622/bpy_restrict_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54167 2023-06-22 06:23:59.000000 fake-bpy-module-latest-20230622/bpy_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-22 06:23:59.000000 fake-bpy-module-latest-20230622/console_python.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-22 06:21:51.000000 fake-bpy-module-latest-20230622/console_shell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 06:24:01.000000 fake-bpy-module-latest-20230622/fake_bpy_module_latest.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7193 2023-06-22 06:24:00.000000 fake-bpy-module-latest-20230622/fake_bpy_module_latest.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7832 2023-06-22 06:24:00.000000 fake-bpy-module-latest-20230622/fake_bpy_module_latest.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 06:24:00.000000 fake-bpy-module-latest-20230622/fake_bpy_module_latest.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 06:24:00.000000 fake-bpy-module-latest-20230622/fake_bpy_module_latest.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-22 06:24:00.000000 fake-bpy-module-latest-20230622/fake_bpy_module_latest.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 06:24:01.000000 fake-bpy-module-latest-20230622/freestyle/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-22 06:21:46.000000 fake-bpy-module-latest-20230622/freestyle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9918 2023-06-22 06:21:46.000000 fake-bpy-module-latest-20230622/freestyle/chainingiterators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47908 2023-06-22 06:21:47.000000 fake-bpy-module-latest-20230622/freestyle/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13232 2023-06-22 06:21:47.000000 fake-bpy-module-latest-20230622/freestyle/predicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 06:13:37.000000 fake-bpy-module-latest-20230622/freestyle/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    23737 2023-06-22 06:21:47.000000 fake-bpy-module-latest-20230622/freestyle/shaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86403 2023-06-22 06:21:47.000000 fake-bpy-module-latest-20230622/freestyle/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 06:24:01.000000 fake-bpy-module-latest-20230622/freestyle/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-06-22 06:21:46.000000 fake-bpy-module-latest-20230622/freestyle/utils/ContextFunctions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5644 2023-06-22 06:21:46.000000 fake-bpy-module-latest-20230622/freestyle/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 06:13:37.000000 fake-bpy-module-latest-20230622/freestyle/utils/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 06:24:01.000000 fake-bpy-module-latest-20230622/gpu/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-22 06:21:46.000000 fake-bpy-module-latest-20230622/gpu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-06-22 06:21:46.000000 fake-bpy-module-latest-20230622/gpu/capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-06-22 06:21:46.000000 fake-bpy-module-latest-20230622/gpu/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-22 06:21:46.000000 fake-bpy-module-latest-20230622/gpu/platform.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 06:13:37.000000 fake-bpy-module-latest-20230622/gpu/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-22 06:21:46.000000 fake-bpy-module-latest-20230622/gpu/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-06-22 06:21:46.000000 fake-bpy-module-latest-20230622/gpu/shader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-06-22 06:21:46.000000 fake-bpy-module-latest-20230622/gpu/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-22 06:21:46.000000 fake-bpy-module-latest-20230622/gpu/texture.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26992 2023-06-22 06:21:46.000000 fake-bpy-module-latest-20230622/gpu/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 06:24:01.000000 fake-bpy-module-latest-20230622/gpu_extras/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-22 06:21:46.000000 fake-bpy-module-latest-20230622/gpu_extras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-22 06:21:46.000000 fake-bpy-module-latest-20230622/gpu_extras/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-06-22 06:21:46.000000 fake-bpy-module-latest-20230622/gpu_extras/presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 06:13:37.000000 fake-bpy-module-latest-20230622/gpu_extras/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-22 06:23:59.000000 fake-bpy-module-latest-20230622/graphviz_export.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 06:24:01.000000 fake-bpy-module-latest-20230622/idprop/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-22 06:21:51.000000 fake-bpy-module-latest-20230622/idprop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 06:13:37.000000 fake-bpy-module-latest-20230622/idprop/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-06-22 06:21:51.000000 fake-bpy-module-latest-20230622/idprop/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 06:24:01.000000 fake-bpy-module-latest-20230622/imbuf/
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-06-22 06:21:51.000000 fake-bpy-module-latest-20230622/imbuf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 06:13:37.000000 fake-bpy-module-latest-20230622/imbuf/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-06-22 06:21:51.000000 fake-bpy-module-latest-20230622/imbuf/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48637 2023-06-22 06:23:58.000000 fake-bpy-module-latest-20230622/keyingsets_builtins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-22 06:23:57.000000 fake-bpy-module-latest-20230622/keyingsets_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 06:24:01.000000 fake-bpy-module-latest-20230622/mathutils/
+-rw-r--r--   0 runner    (1001) docker     (123)    86215 2023-06-22 06:21:46.000000 fake-bpy-module-latest-20230622/mathutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-06-22 06:21:46.000000 fake-bpy-module-latest-20230622/mathutils/bvhtree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22187 2023-06-22 06:21:46.000000 fake-bpy-module-latest-20230622/mathutils/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-22 06:21:46.000000 fake-bpy-module-latest-20230622/mathutils/interpolate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-06-22 06:21:46.000000 fake-bpy-module-latest-20230622/mathutils/kdtree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13248 2023-06-22 06:21:46.000000 fake-bpy-module-latest-20230622/mathutils/noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 06:13:37.000000 fake-bpy-module-latest-20230622/mathutils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-06-22 06:23:57.000000 fake-bpy-module-latest-20230622/nodeitems_builtins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-22 06:23:58.000000 fake-bpy-module-latest-20230622/nodeitems_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-06-22 06:23:59.000000 fake-bpy-module-latest-20230622/rna_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-22 06:23:59.000000 fake-bpy-module-latest-20230622/rna_keymap_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-06-22 06:23:58.000000 fake-bpy-module-latest-20230622/rna_prop_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-22 06:23:59.000000 fake-bpy-module-latest-20230622/rna_xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 06:24:01.000000 fake-bpy-module-latest-20230622/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-06-22 06:24:00.000000 fake-bpy-module-latest-20230622/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-22 06:21:51.000000 fake-bpy-module-latest-20230622/sys_info.py
```

### Comparing `fake-bpy-module-latest-20230621/PKG-INFO` & `fake-bpy-module-latest-20230622/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: fake-bpy-module-latest
-Version: 20230621
+Version: 20230622
 Summary: Collection of the fake Blender Python API module for the code completion.
 Home-page: https://github.com/nutti/fake-bpy-module
 Author: nutti
 Author-email: nutti.metro@gmail.com
 Maintainer: nutti
 Maintainer-email: nutti.metro@gmail.com
 License: MIT
```

### Comparing `fake-bpy-module-latest-20230621/README.rst` & `fake-bpy-module-latest-20230622/README.rst`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/addon_utils.py` & `fake-bpy-module-latest-20230622/addon_utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/animsys_refactor.py` & `fake-bpy-module-latest-20230622/animsys_refactor.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/aud.py` & `fake-bpy-module-latest-20230622/aud.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bgl.py` & `fake-bpy-module-latest-20230622/bgl.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_app_override/helpers.py` & `fake-bpy-module-latest-20230622/bl_app_override/helpers.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_i18n_utils/bl_extract_messages.py` & `fake-bpy-module-latest-20230622/bl_i18n_utils/bl_extract_messages.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_i18n_utils/settings.py` & `fake-bpy-module-latest-20230622/bl_i18n_utils/settings.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_i18n_utils/utils.py` & `fake-bpy-module-latest-20230622/bl_i18n_utils/utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_keymap_utils/io.py` & `fake-bpy-module-latest-20230622/bl_keymap_utils/io.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_math.py` & `fake-bpy-module-latest-20230622/bl_math.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_operators/__init__.py` & `fake-bpy-module-latest-20230622/bl_operators/__init__.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 import sys
 import typing
-from . import mesh
-from . import file
-from . import bmesh
-from . import anim
 from . import uvcalc_lightmap
-from . import image
-from . import sequencer
-from . import object_quick_effects
-from . import uvcalc_transform
+from . import assets
+from . import geometry_nodes
+from . import console
+from . import object
 from . import add_mesh_torus
 from . import userpref
+from . import anim
 from . import constraint
+from . import sequencer
+from . import object_quick_effects
+from . import clip
 from . import screen_play_rendered_anim
-from . import console
-from . import vertexpaint_dirt
 from . import object_align
-from . import node
-from . import clip
+from . import uvcalc_transform
+from . import image
+from . import freestyle
+from . import bmesh
+from . import uvcalc_follow_active
+from . import view3d
 from . import wm
+from . import vertexpaint_dirt
 from . import rigidbody
-from . import object
-from . import freestyle
+from . import node
+from . import file
 from . import presets
-from . import assets
-from . import uvcalc_follow_active
-from . import object_randomize_transform
 from . import text
-from . import view3d
+from . import object_randomize_transform
 from . import spreadsheet
-from . import geometry_nodes
+from . import mesh
 
 GenericType = typing.TypeVar("GenericType")
 
 
 def register():
     '''
```

### Comparing `fake-bpy-module-latest-20230621/bl_operators/add_mesh_torus.py` & `fake-bpy-module-latest-20230622/bl_operators/add_mesh_torus.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_operators/anim.py` & `fake-bpy-module-latest-20230622/bl_operators/anim.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_operators/assets.py` & `fake-bpy-module-latest-20230622/bl_operators/assets.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_operators/bmesh/find_adjacent.py` & `fake-bpy-module-latest-20230622/bl_operators/bmesh/find_adjacent.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_operators/clip.py` & `fake-bpy-module-latest-20230622/bl_operators/clip.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_operators/console.py` & `fake-bpy-module-latest-20230622/bl_operators/console.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_operators/constraint.py` & `fake-bpy-module-latest-20230622/bl_operators/constraint.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_operators/file.py` & `fake-bpy-module-latest-20230622/bl_operators/file.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_operators/freestyle.py` & `fake-bpy-module-latest-20230622/bl_operators/freestyle.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_operators/geometry_nodes.py` & `fake-bpy-module-latest-20230622/bl_operators/geometry_nodes.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_operators/image.py` & `fake-bpy-module-latest-20230622/bl_operators/image.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_operators/mesh.py` & `fake-bpy-module-latest-20230622/bl_operators/mesh.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_operators/node.py` & `fake-bpy-module-latest-20230622/bl_operators/node.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_operators/object.py` & `fake-bpy-module-latest-20230622/bl_operators/object.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_operators/object_align.py` & `fake-bpy-module-latest-20230622/bl_operators/object_align.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_operators/object_quick_effects.py` & `fake-bpy-module-latest-20230622/bl_operators/object_quick_effects.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_operators/object_randomize_transform.py` & `fake-bpy-module-latest-20230622/bl_operators/object_randomize_transform.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_operators/presets.py` & `fake-bpy-module-latest-20230622/bl_operators/presets.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_operators/rigidbody.py` & `fake-bpy-module-latest-20230622/bl_operators/rigidbody.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_operators/screen_play_rendered_anim.py` & `fake-bpy-module-latest-20230622/bl_operators/screen_play_rendered_anim.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_operators/sequencer.py` & `fake-bpy-module-latest-20230622/bl_operators/sequencer.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_operators/spreadsheet.py` & `fake-bpy-module-latest-20230622/bl_operators/spreadsheet.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_operators/text.py` & `fake-bpy-module-latest-20230622/bl_operators/text.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_operators/userpref.py` & `fake-bpy-module-latest-20230622/bl_operators/userpref.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_operators/uvcalc_follow_active.py` & `fake-bpy-module-latest-20230622/bl_operators/uvcalc_follow_active.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_operators/uvcalc_lightmap.py` & `fake-bpy-module-latest-20230622/bl_operators/uvcalc_lightmap.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_operators/uvcalc_transform.py` & `fake-bpy-module-latest-20230622/bl_operators/uvcalc_transform.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_operators/vertexpaint_dirt.py` & `fake-bpy-module-latest-20230622/bl_operators/vertexpaint_dirt.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_operators/view3d.py` & `fake-bpy-module-latest-20230622/bl_operators/view3d.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_operators/wm.py` & `fake-bpy-module-latest-20230622/bl_operators/wm.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_previews_utils/bl_previews_render.py` & `fake-bpy-module-latest-20230622/bl_previews_utils/bl_previews_render.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_ui/__init__.py` & `fake-bpy-module-latest-20230622/bl_ui/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,81 +1,81 @@
 import sys
 import typing
 import bpy_types
 
-from . import properties_data_lightprobe
-from . import properties_view_layer
-from . import properties_constraint
-from . import node_add_menu
-from . import space_statusbar
-from . import properties_output
-from . import properties_mask_common
-from . import properties_data_volume
-from . import properties_data_curve
-from . import properties_texture
-from . import properties_data_curves
-from . import properties_material
-from . import properties_data_empty
-from . import space_clip
-from . import properties_physics_field
-from . import space_sequencer
+from . import properties_data_camera
+from . import space_userpref
 from . import space_image
+from . import properties_grease_pencil_common
+from . import properties_animviz
 from . import properties_material_gpencil
-from . import space_topbar
-from . import properties_data_metaball
+from . import space_filebrowser
+from . import properties_physics_common
+from . import properties_data_empty
+from . import utils
 from . import properties_data_speaker
+from . import space_info
+from . import properties_output
+from . import space_time
+from . import space_properties
+from . import properties_texture
+from . import properties_data_gpencil
+from . import space_node
 from . import space_view3d_toolbar
-from . import properties_data_light
-from . import properties_physics_geometry_nodes
-from . import properties_freestyle
-from . import properties_workspace
+from . import properties_physics_rigidbody_constraint
+from . import properties_data_mesh
 from . import properties_data_lattice
-from . import space_dopesheet
-from . import properties_animviz
-from . import properties_physics_cloth
+from . import node_add_menu
+from . import properties_physics_fluid
+from . import properties_freestyle
+from . import properties_physics_field
+from . import properties_constraint
 from . import space_text
-from . import properties_data_shaderfx
-from . import properties_physics_rigidbody_constraint
-from . import properties_scene
-from . import properties_data_gpencil
-from . import properties_data_camera
-from . import properties_physics_rigidbody
-from . import properties_data_armature
-from . import space_outliner
 from . import properties_render
-from . import properties_data_mesh
+from . import properties_data_metaball
+from . import space_nla
 from . import properties_paint_common
-from . import space_properties
-from . import properties_physics_common
-from . import node_add_menu_geometry
+from . import properties_data_lightprobe
 from . import space_graph
-from . import space_node
-from . import properties_grease_pencil_common
+from . import properties_world
+from . import properties_data_volume
+from . import space_sequencer
+from . import space_toolsystem_toolbar
+from . import properties_data_bone
+from . import properties_particle
+from . import properties_material
 from . import space_view3d
-from . import space_nla
-from . import space_spreadsheet
-from . import space_userpref
+from . import properties_workspace
+from . import space_dopesheet
+from . import properties_data_armature
+from . import properties_data_light
+from . import properties_data_shaderfx
 from . import space_toolsystem_common
-from . import properties_data_modifier
-from . import properties_particle
-from . import properties_physics_softbody
 from . import generic_ui_list
-from . import space_filebrowser
-from . import properties_object
-from . import properties_data_bone
-from . import space_time
-from . import properties_data_pointcloud
-from . import utils
-from . import properties_physics_dynamicpaint
-from . import properties_physics_fluid
-from . import properties_world
-from . import space_info
+from . import properties_mask_common
+from . import space_clip
+from . import space_spreadsheet
+from . import properties_physics_rigidbody
+from . import space_topbar
+from . import properties_data_curve
+from . import properties_physics_softbody
+from . import properties_scene
+from . import properties_physics_geometry_nodes
+from . import properties_physics_cloth
+from . import space_statusbar
+from . import node_add_menu_geometry
 from . import space_console
 from . import properties_collection
-from . import space_toolsystem_toolbar
+from . import properties_view_layer
+from . import space_outliner
+from . import properties_data_curves
+from . import properties_data_modifier
+from . import properties_object
+from . import properties_physics_dynamicpaint
+from . import properties_data_pointcloud
 
 GenericType = typing.TypeVar("GenericType")
 
 
 class UI_MT_button_context_menu(bpy_types.Menu, bpy_types._GenericUI):
     bl_idname = None
     ''' '''
```

### Comparing `fake-bpy-module-latest-20230621/bl_ui/generic_ui_list.py` & `fake-bpy-module-latest-20230622/bl_ui/generic_ui_list.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_ui/node_add_menu_geometry.py` & `fake-bpy-module-latest-20230622/bl_ui/node_add_menu_geometry.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_ui/properties_animviz.py` & `fake-bpy-module-latest-20230622/bl_ui/properties_animviz.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_ui/properties_collection.py` & `fake-bpy-module-latest-20230622/bl_ui/properties_collection.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_ui/properties_constraint.py` & `fake-bpy-module-latest-20230622/bl_ui/properties_constraint.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_ui/properties_data_armature.py` & `fake-bpy-module-latest-20230622/bl_ui/properties_data_armature.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_ui/properties_data_bone.py` & `fake-bpy-module-latest-20230622/bl_ui/properties_data_bone.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_ui/properties_data_camera.py` & `fake-bpy-module-latest-20230622/bl_ui/properties_data_camera.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_ui/properties_data_curve.py` & `fake-bpy-module-latest-20230622/bl_ui/properties_data_curve.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_ui/properties_data_curves.py` & `fake-bpy-module-latest-20230622/bl_ui/properties_data_curves.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_ui/properties_data_empty.py` & `fake-bpy-module-latest-20230622/bl_ui/properties_data_empty.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_ui/properties_data_gpencil.py` & `fake-bpy-module-latest-20230622/bl_ui/properties_data_gpencil.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_ui/properties_data_lattice.py` & `fake-bpy-module-latest-20230622/bl_ui/properties_data_lattice.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_ui/properties_data_light.py` & `fake-bpy-module-latest-20230622/bl_ui/properties_data_light.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_ui/properties_data_lightprobe.py` & `fake-bpy-module-latest-20230622/bl_ui/properties_data_lightprobe.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_ui/properties_data_mesh.py` & `fake-bpy-module-latest-20230622/bl_ui/properties_data_mesh.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_ui/properties_data_metaball.py` & `fake-bpy-module-latest-20230622/bl_ui/properties_data_metaball.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_ui/properties_data_modifier.py` & `fake-bpy-module-latest-20230622/bl_ui/properties_data_modifier.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_ui/properties_data_pointcloud.py` & `fake-bpy-module-latest-20230622/bl_ui/properties_data_pointcloud.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_ui/properties_data_shaderfx.py` & `fake-bpy-module-latest-20230622/bl_ui/properties_data_shaderfx.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_ui/properties_data_speaker.py` & `fake-bpy-module-latest-20230622/bl_ui/properties_data_speaker.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_ui/properties_data_volume.py` & `fake-bpy-module-latest-20230622/bl_ui/properties_data_volume.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_ui/properties_freestyle.py` & `fake-bpy-module-latest-20230622/bl_ui/properties_freestyle.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_ui/properties_grease_pencil_common.py` & `fake-bpy-module-latest-20230622/bl_ui/properties_grease_pencil_common.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_ui/properties_mask_common.py` & `fake-bpy-module-latest-20230622/bl_ui/properties_mask_common.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_ui/properties_material.py` & `fake-bpy-module-latest-20230622/bl_ui/properties_material.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_ui/properties_material_gpencil.py` & `fake-bpy-module-latest-20230622/bl_ui/properties_material_gpencil.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_ui/properties_object.py` & `fake-bpy-module-latest-20230622/bl_ui/properties_object.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_ui/properties_output.py` & `fake-bpy-module-latest-20230622/bl_ui/properties_output.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_ui/properties_paint_common.py` & `fake-bpy-module-latest-20230622/bl_ui/properties_paint_common.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_ui/properties_particle.py` & `fake-bpy-module-latest-20230622/bl_ui/properties_particle.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_ui/properties_physics_cloth.py` & `fake-bpy-module-latest-20230622/bl_ui/properties_physics_cloth.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_ui/properties_physics_common.py` & `fake-bpy-module-latest-20230622/bl_ui/properties_physics_common.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_ui/properties_physics_dynamicpaint.py` & `fake-bpy-module-latest-20230622/bl_ui/properties_physics_dynamicpaint.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_ui/properties_physics_field.py` & `fake-bpy-module-latest-20230622/bl_ui/properties_physics_field.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_ui/properties_physics_fluid.py` & `fake-bpy-module-latest-20230622/bl_ui/properties_physics_fluid.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_ui/properties_physics_geometry_nodes.py` & `fake-bpy-module-latest-20230622/bl_ui/properties_physics_geometry_nodes.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_ui/properties_physics_rigidbody.py` & `fake-bpy-module-latest-20230622/bl_ui/properties_physics_rigidbody.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_ui/properties_physics_rigidbody_constraint.py` & `fake-bpy-module-latest-20230622/bl_ui/properties_physics_rigidbody_constraint.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_ui/properties_physics_softbody.py` & `fake-bpy-module-latest-20230622/bl_ui/properties_physics_softbody.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_ui/properties_render.py` & `fake-bpy-module-latest-20230622/bl_ui/properties_render.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_ui/properties_scene.py` & `fake-bpy-module-latest-20230622/bl_ui/properties_scene.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_ui/properties_texture.py` & `fake-bpy-module-latest-20230622/bl_ui/properties_texture.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_ui/properties_view_layer.py` & `fake-bpy-module-latest-20230622/bl_ui/properties_view_layer.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_ui/properties_workspace.py` & `fake-bpy-module-latest-20230622/bl_ui/properties_workspace.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_ui/properties_world.py` & `fake-bpy-module-latest-20230622/bl_ui/properties_world.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_ui/space_clip.py` & `fake-bpy-module-latest-20230622/bl_ui/space_clip.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_ui/space_console.py` & `fake-bpy-module-latest-20230622/bl_ui/space_console.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_ui/space_dopesheet.py` & `fake-bpy-module-latest-20230622/bl_ui/space_dopesheet.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_ui/space_filebrowser.py` & `fake-bpy-module-latest-20230622/bl_ui/space_filebrowser.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_ui/space_graph.py` & `fake-bpy-module-latest-20230622/bl_ui/space_graph.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_ui/space_image.py` & `fake-bpy-module-latest-20230622/bl_ui/space_image.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_ui/space_info.py` & `fake-bpy-module-latest-20230622/bl_ui/space_info.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_ui/space_nla.py` & `fake-bpy-module-latest-20230622/bl_ui/space_nla.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_ui/space_node.py` & `fake-bpy-module-latest-20230622/bl_ui/space_node.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_ui/space_outliner.py` & `fake-bpy-module-latest-20230622/bl_ui/space_outliner.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_ui/space_properties.py` & `fake-bpy-module-latest-20230622/bl_ui/space_properties.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_ui/space_sequencer.py` & `fake-bpy-module-latest-20230622/bl_ui/space_sequencer.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_ui/space_spreadsheet.py` & `fake-bpy-module-latest-20230622/bl_ui/space_spreadsheet.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_ui/space_statusbar.py` & `fake-bpy-module-latest-20230622/bl_ui/space_statusbar.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_ui/space_text.py` & `fake-bpy-module-latest-20230622/bl_ui/space_text.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_ui/space_time.py` & `fake-bpy-module-latest-20230622/bl_ui/space_time.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_ui/space_toolsystem_common.py` & `fake-bpy-module-latest-20230622/bl_ui/space_toolsystem_common.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_ui/space_toolsystem_toolbar.py` & `fake-bpy-module-latest-20230622/bl_ui/space_toolsystem_toolbar.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_ui/space_topbar.py` & `fake-bpy-module-latest-20230622/bl_ui/space_topbar.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_ui/space_userpref.py` & `fake-bpy-module-latest-20230622/bl_ui/space_userpref.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_ui/space_view3d.py` & `fake-bpy-module-latest-20230622/bl_ui/space_view3d.py`

 * *Files 0% similar despite different names*

```diff
@@ -28275,15 +28275,214 @@
 
     def draw_collapsible(self, context, layout):
         ''' 
 
         '''
         pass
 
-    def draw_legacy(self, context):
+    def draw_preset(self, _context):
+        ''' 
+
+        '''
+        pass
+
+    def driver_add(self):
+        ''' 
+
+        '''
+        pass
+
+    def driver_remove(self):
+        ''' 
+
+        '''
+        pass
+
+    def get(self):
+        ''' 
+
+        '''
+        pass
+
+    def id_properties_clear(self):
+        ''' 
+
+        '''
+        pass
+
+    def id_properties_ensure(self):
+        ''' 
+
+        '''
+        pass
+
+    def id_properties_ui(self):
+        ''' 
+
+        '''
+        pass
+
+    def is_extended(self):
+        ''' 
+
+        '''
+        pass
+
+    def is_property_hidden(self):
+        ''' 
+
+        '''
+        pass
+
+    def is_property_overridable_library(self):
+        ''' 
+
+        '''
+        pass
+
+    def is_property_readonly(self):
+        ''' 
+
+        '''
+        pass
+
+    def is_property_set(self):
+        ''' 
+
+        '''
+        pass
+
+    def items(self):
+        ''' 
+
+        '''
+        pass
+
+    def keyframe_delete(self):
+        ''' 
+
+        '''
+        pass
+
+    def keyframe_insert(self):
+        ''' 
+
+        '''
+        pass
+
+    def keys(self):
+        ''' 
+
+        '''
+        pass
+
+    def path_from_id(self):
+        ''' 
+
+        '''
+        pass
+
+    def path_menu(self, searchpaths, operator, props_default, prop_filepath,
+                  filter_ext, filter_path, display_name, add_operator):
+        ''' 
+
+        '''
+        pass
+
+    def path_resolve(self):
+        ''' 
+
+        '''
+        pass
+
+    def pop(self):
+        ''' 
+
+        '''
+        pass
+
+    def prepend(self, draw_func):
+        ''' 
+
+        '''
+        pass
+
+    def property_overridable_library_set(self):
+        ''' 
+
+        '''
+        pass
+
+    def property_unset(self):
+        ''' 
+
+        '''
+        pass
+
+    def remove(self, draw_func):
+        ''' 
+
+        '''
+        pass
+
+    def type_recast(self):
+        ''' 
+
+        '''
+        pass
+
+    def values(self):
+        ''' 
+
+        '''
+        pass
+
+
+class VIEW3D_MT_select_edit_grease_pencil(bpy_types.Menu,
+                                          bpy_types._GenericUI):
+    bl_label = None
+    ''' '''
+
+    bl_rna = None
+    ''' '''
+
+    id_data = None
+    ''' '''
+
+    def append(self, draw_func):
+        ''' 
+
+        '''
+        pass
+
+    def as_pointer(self):
+        ''' 
+
+        '''
+        pass
+
+    def bl_rna_get_subclass(self):
+        ''' 
+
+        '''
+        pass
+
+    def bl_rna_get_subclass_py(self):
+        ''' 
+
+        '''
+        pass
+
+    def draw(self, context):
+        ''' 
+
+        '''
+        pass
+
+    def draw_collapsible(self, context, layout):
         ''' 
 
         '''
         pass
 
     def draw_preset(self, _context):
         '''
```

### Comparing `fake-bpy-module-latest-20230621/bl_ui/space_view3d_toolbar.py` & `fake-bpy-module-latest-20230622/bl_ui/space_view3d_toolbar.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bl_ui/utils.py` & `fake-bpy-module-latest-20230622/bl_ui/utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/blf.py` & `fake-bpy-module-latest-20230622/blf.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bmesh/__init__.py` & `fake-bpy-module-latest-20230622/bmesh/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import sys
 import typing
 import bpy.types
 import bmesh.types
 
-from . import geometry
 from . import ops
 from . import types
 from . import utils
+from . import geometry
 
 GenericType = typing.TypeVar("GenericType")
 
 
 def from_edit_mesh(mesh: 'bpy.types.Mesh') -> 'bmesh.types.BMesh':
     ''' Return a BMesh from this mesh, currently the mesh must already be in editmode.
```

### Comparing `fake-bpy-module-latest-20230621/bmesh/geometry.py` & `fake-bpy-module-latest-20230622/bmesh/geometry.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bmesh/ops.py` & `fake-bpy-module-latest-20230622/bmesh/ops.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bmesh/types.py` & `fake-bpy-module-latest-20230622/bmesh/types.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bmesh/utils.py` & `fake-bpy-module-latest-20230622/bmesh/utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bpy/app/__init__.py` & `fake-bpy-module-latest-20230622/bpy/app/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import sys
 import typing
-from . import timers
 from . import icons
 from . import handlers
 from . import translations
+from . import timers
 
 GenericType = typing.TypeVar("GenericType")
 
 
 def help_text(all: typing.Optional[bool] = False):
     ''' Return the help text as a string.
```

### Comparing `fake-bpy-module-latest-20230621/bpy/app/handlers.py` & `fake-bpy-module-latest-20230622/bpy/app/handlers.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bpy/app/icons.py` & `fake-bpy-module-latest-20230622/bpy/app/icons.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bpy/app/timers.py` & `fake-bpy-module-latest-20230622/bpy/app/timers.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bpy/app/translations.py` & `fake-bpy-module-latest-20230622/bpy/app/translations.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bpy/msgbus.py` & `fake-bpy-module-latest-20230622/bpy/msgbus.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bpy/ops/__init__.py` & `fake-bpy-module-latest-20230622/bpy/ops/__init__.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,81 +1,81 @@
 import sys
 import typing
-from . import scene
-from . import wm
+from . import script
+from . import buttons
+from . import outliner
+from . import surface
+from . import action
+from . import sound
+from . import paintcurve
+from . import particle
+from . import view2d
+from . import uv
+from . import lattice
+from . import image
+from . import file
 from . import info
-from . import transform
-from . import curve
+from . import geometry
+from . import ui
+from . import spreadsheet
+from . import fluid
+from . import ed
+from . import anim
 from . import export_anim
-from . import import_scene
-from . import screen
-from . import text_editor
+from . import grease_pencil
 from . import cloth
-from . import gpencil
-from . import node
+from . import ptcache
 from . import graph
-from . import ed
-from . import world
-from . import view3d
-from . import object
-from . import uv
-from . import nla
-from . import rigidbody
 from . import boid
-from . import grease_pencil
-from . import file
-from . import collection
-from . import brush
-from . import import_mesh
-from . import mball
-from . import curves
-from . import console
-from . import fluid
-from . import spreadsheet
-from . import action
-from . import ptcache
-from . import mask
-from . import palette
-from . import dpaint
-from . import cycles
+from . import asset
+from . import import_anim
 from . import export_scene
-from . import outliner
-from . import render
-from . import particle
-from . import poselib
-from . import lattice
-from . import camera
-from . import cachefile
-from . import uilist
 from . import preferences
-from . import paintcurve
 from . import paint
-from . import surface
+from . import text_editor
+from . import import_scene
+from . import object
+from . import scene
+from . import render
+from . import sequencer
+from . import clip
+from . import poselib
 from . import material
-from . import script
-from . import constraint
 from . import pose
-from . import texture
+from . import font
+from . import brush
+from . import collection
+from . import export_mesh
+from . import gpencil
+from . import world
 from . import marker
-from . import view2d
+from . import mball
+from . import uilist
+from . import sculpt_curves
+from . import rigidbody
+from . import cachefile
+from . import mesh
+from . import screen
+from . import armature
+from . import curve
 from . import workspace
-from . import sculpt
-from . import geometry
-from . import anim
-from . import sequencer
+from . import console
+from . import import_mesh
 from . import gizmogroup
-from . import clip
-from . import ui
-from . import import_curve
-from . import export_mesh
-from . import mesh
-from . import sculpt_curves
-from . import asset
-from . import buttons
+from . import texture
+from . import nla
+from . import dpaint
+from . import camera
 from . import text
-from . import image
-from . import import_anim
-from . import font
-from . import sound
-from . import armature
+from . import mask
+from . import wm
+from . import curves
+from . import view3d
+from . import constraint
+from . import transform
+from . import import_curve
+from . import cycles
+from . import node
+from . import palette
+from . import sculpt
 
 GenericType = typing.TypeVar("GenericType")
```

### Comparing `fake-bpy-module-latest-20230621/bpy/ops/action.py` & `fake-bpy-module-latest-20230622/bpy/ops/action.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bpy/ops/anim.py` & `fake-bpy-module-latest-20230622/bpy/ops/anim.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bpy/ops/armature.py` & `fake-bpy-module-latest-20230622/bpy/ops/armature.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bpy/ops/asset.py` & `fake-bpy-module-latest-20230622/bpy/ops/asset.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bpy/ops/boid.py` & `fake-bpy-module-latest-20230622/bpy/ops/boid.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bpy/ops/brush.py` & `fake-bpy-module-latest-20230622/bpy/ops/brush.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bpy/ops/buttons.py` & `fake-bpy-module-latest-20230622/bpy/ops/buttons.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bpy/ops/cachefile.py` & `fake-bpy-module-latest-20230622/bpy/ops/cachefile.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bpy/ops/camera.py` & `fake-bpy-module-latest-20230622/bpy/ops/camera.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bpy/ops/clip.py` & `fake-bpy-module-latest-20230622/bpy/ops/clip.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bpy/ops/cloth.py` & `fake-bpy-module-latest-20230622/bpy/ops/cloth.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bpy/ops/collection.py` & `fake-bpy-module-latest-20230622/bpy/ops/collection.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bpy/ops/console.py` & `fake-bpy-module-latest-20230622/bpy/ops/console.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bpy/ops/constraint.py` & `fake-bpy-module-latest-20230622/bpy/ops/constraint.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bpy/ops/curve.py` & `fake-bpy-module-latest-20230622/bpy/ops/curve.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bpy/ops/curves.py` & `fake-bpy-module-latest-20230622/bpy/ops/curves.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bpy/ops/cycles.py` & `fake-bpy-module-latest-20230622/bpy/ops/cycles.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bpy/ops/dpaint.py` & `fake-bpy-module-latest-20230622/bpy/ops/dpaint.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bpy/ops/ed.py` & `fake-bpy-module-latest-20230622/bpy/ops/ed.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bpy/ops/export_anim.py` & `fake-bpy-module-latest-20230622/bpy/ops/export_anim.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bpy/ops/export_mesh.py` & `fake-bpy-module-latest-20230622/bpy/ops/export_mesh.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bpy/ops/export_scene.py` & `fake-bpy-module-latest-20230622/bpy/ops/export_scene.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bpy/ops/file.py` & `fake-bpy-module-latest-20230622/bpy/ops/file.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bpy/ops/fluid.py` & `fake-bpy-module-latest-20230622/bpy/ops/fluid.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bpy/ops/font.py` & `fake-bpy-module-latest-20230622/bpy/ops/font.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bpy/ops/geometry.py` & `fake-bpy-module-latest-20230622/bpy/ops/geometry.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bpy/ops/gizmogroup.py` & `fake-bpy-module-latest-20230622/bpy/ops/gizmogroup.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bpy/ops/gpencil.py` & `fake-bpy-module-latest-20230622/bpy/ops/gpencil.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bpy/ops/graph.py` & `fake-bpy-module-latest-20230622/bpy/ops/graph.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bpy/ops/grease_pencil.py` & `fake-bpy-module-latest-20230622/bpy/ops/grease_pencil.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bpy/ops/image.py` & `fake-bpy-module-latest-20230622/bpy/ops/image.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bpy/ops/import_anim.py` & `fake-bpy-module-latest-20230622/bpy/ops/import_anim.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bpy/ops/import_curve.py` & `fake-bpy-module-latest-20230622/bpy/ops/import_curve.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bpy/ops/import_mesh.py` & `fake-bpy-module-latest-20230622/bpy/ops/import_mesh.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bpy/ops/import_scene.py` & `fake-bpy-module-latest-20230622/bpy/ops/import_scene.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bpy/ops/info.py` & `fake-bpy-module-latest-20230622/bpy/ops/info.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bpy/ops/lattice.py` & `fake-bpy-module-latest-20230622/bpy/ops/lattice.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bpy/ops/marker.py` & `fake-bpy-module-latest-20230622/bpy/ops/marker.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bpy/ops/mask.py` & `fake-bpy-module-latest-20230622/bpy/ops/mask.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bpy/ops/material.py` & `fake-bpy-module-latest-20230622/bpy/ops/material.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bpy/ops/mball.py` & `fake-bpy-module-latest-20230622/bpy/ops/mball.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bpy/ops/mesh.py` & `fake-bpy-module-latest-20230622/bpy/ops/mesh.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bpy/ops/nla.py` & `fake-bpy-module-latest-20230622/bpy/ops/nla.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bpy/ops/node.py` & `fake-bpy-module-latest-20230622/bpy/ops/node.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bpy/ops/object.py` & `fake-bpy-module-latest-20230622/bpy/ops/object.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bpy/ops/outliner.py` & `fake-bpy-module-latest-20230622/bpy/ops/outliner.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bpy/ops/paint.py` & `fake-bpy-module-latest-20230622/bpy/ops/paint.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bpy/ops/paintcurve.py` & `fake-bpy-module-latest-20230622/bpy/ops/paintcurve.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bpy/ops/palette.py` & `fake-bpy-module-latest-20230622/bpy/ops/palette.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bpy/ops/particle.py` & `fake-bpy-module-latest-20230622/bpy/ops/particle.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bpy/ops/pose.py` & `fake-bpy-module-latest-20230622/bpy/ops/pose.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bpy/ops/poselib.py` & `fake-bpy-module-latest-20230622/bpy/ops/poselib.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bpy/ops/preferences.py` & `fake-bpy-module-latest-20230622/bpy/ops/preferences.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bpy/ops/ptcache.py` & `fake-bpy-module-latest-20230622/bpy/ops/ptcache.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bpy/ops/render.py` & `fake-bpy-module-latest-20230622/bpy/ops/render.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bpy/ops/rigidbody.py` & `fake-bpy-module-latest-20230622/bpy/ops/rigidbody.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bpy/ops/scene.py` & `fake-bpy-module-latest-20230622/bpy/ops/scene.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bpy/ops/screen.py` & `fake-bpy-module-latest-20230622/bpy/ops/screen.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bpy/ops/script.py` & `fake-bpy-module-latest-20230622/bpy/ops/script.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bpy/ops/sculpt.py` & `fake-bpy-module-latest-20230622/bpy/ops/sculpt.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bpy/ops/sculpt_curves.py` & `fake-bpy-module-latest-20230622/bpy/ops/sculpt_curves.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bpy/ops/sequencer.py` & `fake-bpy-module-latest-20230622/bpy/ops/sequencer.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bpy/ops/sound.py` & `fake-bpy-module-latest-20230622/bpy/ops/sound.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bpy/ops/spreadsheet.py` & `fake-bpy-module-latest-20230622/bpy/ops/spreadsheet.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bpy/ops/surface.py` & `fake-bpy-module-latest-20230622/bpy/ops/surface.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bpy/ops/text.py` & `fake-bpy-module-latest-20230622/bpy/ops/text.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bpy/ops/text_editor.py` & `fake-bpy-module-latest-20230622/bpy/ops/text_editor.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bpy/ops/texture.py` & `fake-bpy-module-latest-20230622/bpy/ops/texture.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bpy/ops/transform.py` & `fake-bpy-module-latest-20230622/bpy/ops/transform.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bpy/ops/ui.py` & `fake-bpy-module-latest-20230622/bpy/ops/ui.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bpy/ops/uilist.py` & `fake-bpy-module-latest-20230622/bpy/ops/uilist.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bpy/ops/uv.py` & `fake-bpy-module-latest-20230622/bpy/ops/uv.py`

 * *Files 2% similar despite different names*

```diff
@@ -203,15 +203,15 @@
 
 def follow_active_quads(override_context: typing.
                         Union[typing.Dict, 'bpy.types.Context'] = None,
                         execution_context: typing.Union[str, int] = None,
                         undo: typing.Optional[bool] = None,
                         *,
                         mode: typing.Optional[typing.Any] = 'LENGTH_AVERAGE'):
-    ''' Follow UVs from active quads along continuous face loops :File: `startup/bl_operators/uvcalc_follow_active.py\:259 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/uvcalc_follow_active.py#L259>`__
+    ''' Follow UVs from active quads along continuous face loops :File: `startup/bl_operators/uvcalc_follow_active.py\:261 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/uvcalc_follow_active.py#L261>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param mode: Edge Length Mode, Method to space UV edge loops * ``EVEN`` Even -- Space all UVs evenly. * ``LENGTH`` Length -- Average space UVs edge length of each loop. * ``LENGTH_AVERAGE`` Length Average -- Average space UVs edge length of each loop.
     :type mode: typing.Optional[typing.Any]
     '''
@@ -876,24 +876,24 @@
 
 
 def select_similar(override_context: typing.
                    Union[typing.Dict, 'bpy.types.Context'] = None,
                    execution_context: typing.Union[str, int] = None,
                    undo: typing.Optional[bool] = None,
                    *,
-                   type: typing.Union[str, int, typing.Any] = 'PIN',
+                   type: typing.Optional[typing.Any] = 'PIN',
                    compare: typing.Optional[typing.Any] = 'EQUAL',
                    threshold: typing.Optional[typing.Any] = 0.0):
     ''' Select similar UVs by property types
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param type: Type
-    :type type: typing.Union[str, int, typing.Any]
+    :type type: typing.Optional[typing.Any]
     :param compare: Compare
     :type compare: typing.Optional[typing.Any]
     :param threshold: Threshold
     :type threshold: typing.Optional[typing.Any]
     '''
 
     pass
```

### Comparing `fake-bpy-module-latest-20230621/bpy/ops/view2d.py` & `fake-bpy-module-latest-20230622/bpy/ops/view2d.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bpy/ops/view3d.py` & `fake-bpy-module-latest-20230622/bpy/ops/view3d.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bpy/ops/wm.py` & `fake-bpy-module-latest-20230622/bpy/ops/wm.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bpy/ops/workspace.py` & `fake-bpy-module-latest-20230622/bpy/ops/workspace.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bpy/ops/world.py` & `fake-bpy-module-latest-20230622/bpy/ops/world.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bpy/path.py` & `fake-bpy-module-latest-20230622/bpy/path.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bpy/props.py` & `fake-bpy-module-latest-20230622/bpy/props.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bpy/types.py` & `fake-bpy-module-latest-20230622/bpy/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,1055 +1,1055 @@
 00000000: 696d 706f 7274 2073 7973 0a69 6d70 6f72  import sys.impor
 00000010: 7420 7479 7069 6e67 0a69 6d70 6f72 7420  t typing.import 
 00000020: 6d61 7468 7574 696c 730a 696d 706f 7274  mathutils.import
 00000030: 2062 7079 0a69 6d70 6f72 7420 626c 5f75   bpy.import bl_u
 00000040: 692e 7072 6f70 6572 7469 6573 5f64 6174  i.properties_dat
-00000050: 615f 6c69 6768 7470 726f 6265 0a69 6d70  a_lightprobe.imp
-00000060: 6f72 7420 626c 5f75 692e 7072 6f70 6572  ort bl_ui.proper
-00000070: 7469 6573 5f76 6965 775f 6c61 7965 720a  ties_view_layer.
-00000080: 696d 706f 7274 2062 6c5f 7569 2e70 726f  import bl_ui.pro
-00000090: 7065 7274 6965 735f 636f 6e73 7472 6169  perties_constrai
-000000a0: 6e74 0a69 6d70 6f72 7420 626c 5f75 692e  nt.import bl_ui.
-000000b0: 7370 6163 655f 7374 6174 7573 6261 720a  space_statusbar.
-000000c0: 696d 706f 7274 2062 6c5f 7569 2e70 726f  import bl_ui.pro
-000000d0: 7065 7274 6965 735f 6f75 7470 7574 0a69  perties_output.i
-000000e0: 6d70 6f72 7420 626c 5f75 692e 7072 6f70  mport bl_ui.prop
-000000f0: 6572 7469 6573 5f6d 6173 6b5f 636f 6d6d  erties_mask_comm
-00000100: 6f6e 0a69 6d70 6f72 7420 626c 5f6f 7065  on.import bl_ope
-00000110: 7261 746f 7273 2e66 696c 650a 696d 706f  rators.file.impo
-00000120: 7274 2062 6c5f 7569 2e70 726f 7065 7274  rt bl_ui.propert
-00000130: 6965 735f 6461 7461 5f76 6f6c 756d 650a  ies_data_volume.
-00000140: 696d 706f 7274 2062 6c5f 7569 2e70 726f  import bl_ui.pro
-00000150: 7065 7274 6965 735f 6461 7461 5f63 7572  perties_data_cur
-00000160: 7665 0a69 6d70 6f72 7420 626c 5f6f 7065  ve.import bl_ope
-00000170: 7261 746f 7273 2e61 6e69 6d0a 696d 706f  rators.anim.impo
-00000180: 7274 2062 6c5f 7569 2e70 726f 7065 7274  rt bl_ui.propert
-00000190: 6965 735f 7465 7874 7572 650a 696d 706f  ies_texture.impo
-000001a0: 7274 2062 6c5f 7569 2e70 726f 7065 7274  rt bl_ui.propert
-000001b0: 6965 735f 6461 7461 5f63 7572 7665 730a  ies_data_curves.
-000001c0: 696d 706f 7274 2062 6c5f 7569 2e70 726f  import bl_ui.pro
-000001d0: 7065 7274 6965 735f 6d61 7465 7269 616c  perties_material
-000001e0: 0a69 6d70 6f72 7420 626c 5f75 692e 7072  .import bl_ui.pr
-000001f0: 6f70 6572 7469 6573 5f64 6174 615f 656d  operties_data_em
-00000200: 7074 790a 696d 706f 7274 2062 6c5f 7569  pty.import bl_ui
-00000210: 2e73 7061 6365 5f63 6c69 700a 696d 706f  .space_clip.impo
-00000220: 7274 2062 6c5f 7569 2e70 726f 7065 7274  rt bl_ui.propert
-00000230: 6965 735f 7068 7973 6963 735f 6669 656c  ies_physics_fiel
-00000240: 640a 696d 706f 7274 2062 6c5f 7569 2e73  d.import bl_ui.s
-00000250: 7061 6365 5f73 6571 7565 6e63 6572 0a69  pace_sequencer.i
-00000260: 6d70 6f72 7420 626c 5f75 692e 7370 6163  mport bl_ui.spac
-00000270: 655f 696d 6167 650a 696d 706f 7274 2062  e_image.import b
-00000280: 6c5f 7569 2e70 726f 7065 7274 6965 735f  l_ui.properties_
-00000290: 6d61 7465 7269 616c 5f67 7065 6e63 696c  material_gpencil
-000002a0: 0a69 6d70 6f72 7420 626c 5f75 692e 7370  .import bl_ui.sp
-000002b0: 6163 655f 746f 7062 6172 0a69 6d70 6f72  ace_topbar.impor
-000002c0: 7420 626c 5f75 692e 7072 6f70 6572 7469  t bl_ui.properti
-000002d0: 6573 5f64 6174 615f 6d65 7461 6261 6c6c  es_data_metaball
-000002e0: 0a69 6d70 6f72 7420 626c 5f75 692e 7072  .import bl_ui.pr
-000002f0: 6f70 6572 7469 6573 5f64 6174 615f 7370  operties_data_sp
-00000300: 6561 6b65 720a 696d 706f 7274 2062 6c5f  eaker.import bl_
-00000310: 7569 2e73 7061 6365 5f76 6965 7733 645f  ui.space_view3d_
-00000320: 746f 6f6c 6261 720a 696d 706f 7274 2062  toolbar.import b
-00000330: 6c5f 7569 0a69 6d70 6f72 7420 626c 5f75  l_ui.import bl_u
-00000340: 692e 7072 6f70 6572 7469 6573 5f64 6174  i.properties_dat
-00000350: 615f 6c69 6768 740a 696d 706f 7274 2062  a_light.import b
-00000360: 6c5f 7569 2e70 726f 7065 7274 6965 735f  l_ui.properties_
-00000370: 7068 7973 6963 735f 6765 6f6d 6574 7279  physics_geometry
-00000380: 5f6e 6f64 6573 0a69 6d70 6f72 7420 626c  _nodes.import bl
-00000390: 5f75 692e 7072 6f70 6572 7469 6573 5f66  _ui.properties_f
-000003a0: 7265 6573 7479 6c65 0a69 6d70 6f72 7420  reestyle.import 
-000003b0: 626c 5f75 692e 7072 6f70 6572 7469 6573  bl_ui.properties
-000003c0: 5f77 6f72 6b73 7061 6365 0a69 6d70 6f72  _workspace.impor
-000003d0: 7420 626c 5f75 692e 7072 6f70 6572 7469  t bl_ui.properti
-000003e0: 6573 5f64 6174 615f 6c61 7474 6963 650a  es_data_lattice.
-000003f0: 696d 706f 7274 2062 6c5f 6f70 6572 6174  import bl_operat
-00000400: 6f72 732e 7573 6572 7072 6566 0a69 6d70  ors.userpref.imp
-00000410: 6f72 7420 626c 5f6f 7065 7261 746f 7273  ort bl_operators
-00000420: 2e63 6f6e 7374 7261 696e 740a 696d 706f  .constraint.impo
-00000430: 7274 2062 6c5f 7569 2e73 7061 6365 5f64  rt bl_ui.space_d
-00000440: 6f70 6573 6865 6574 0a69 6d70 6f72 7420  opesheet.import 
-00000450: 626c 5f75 692e 7072 6f70 6572 7469 6573  bl_ui.properties
-00000460: 5f70 6879 7369 6373 5f63 6c6f 7468 0a69  _physics_cloth.i
-00000470: 6d70 6f72 7420 626c 5f75 692e 7370 6163  mport bl_ui.spac
-00000480: 655f 7465 7874 0a69 6d70 6f72 7420 626c  e_text.import bl
-00000490: 5f6f 7065 7261 746f 7273 2e6e 6f64 650a  _operators.node.
-000004a0: 696d 706f 7274 2062 6c5f 7569 2e70 726f  import bl_ui.pro
-000004b0: 7065 7274 6965 735f 6461 7461 5f73 6861  perties_data_sha
-000004c0: 6465 7266 780a 696d 706f 7274 2062 6c5f  derfx.import bl_
-000004d0: 7569 2e70 726f 7065 7274 6965 735f 7068  ui.properties_ph
-000004e0: 7973 6963 735f 7269 6769 6462 6f64 795f  ysics_rigidbody_
-000004f0: 636f 6e73 7472 6169 6e74 0a69 6d70 6f72  constraint.impor
-00000500: 7420 626c 5f75 692e 7072 6f70 6572 7469  t bl_ui.properti
-00000510: 6573 5f73 6365 6e65 0a69 6d70 6f72 7420  es_scene.import 
-00000520: 626c 5f6f 7065 7261 746f 7273 2e63 6c69  bl_operators.cli
-00000530: 700a 696d 706f 7274 2062 6c5f 6f70 6572  p.import bl_oper
-00000540: 6174 6f72 732e 776d 0a69 6d70 6f72 7420  ators.wm.import 
-00000550: 626c 5f75 692e 7072 6f70 6572 7469 6573  bl_ui.properties
-00000560: 5f64 6174 615f 6770 656e 6369 6c0a 696d  _data_gpencil.im
-00000570: 706f 7274 2062 6c5f 6f70 6572 6174 6f72  port bl_operator
-00000580: 732e 6f62 6a65 6374 0a69 6d70 6f72 7420  s.object.import 
-00000590: 626c 5f75 692e 7072 6f70 6572 7469 6573  bl_ui.properties
-000005a0: 5f64 6174 615f 6361 6d65 7261 0a69 6d70  _data_camera.imp
-000005b0: 6f72 7420 626c 5f75 692e 7072 6f70 6572  ort bl_ui.proper
-000005c0: 7469 6573 5f70 6879 7369 6373 5f72 6967  ties_physics_rig
-000005d0: 6964 626f 6479 0a69 6d70 6f72 7420 626c  idbody.import bl
-000005e0: 5f6f 7065 7261 746f 7273 2e66 7265 6573  _operators.frees
-000005f0: 7479 6c65 0a69 6d70 6f72 7420 626c 5f75  tyle.import bl_u
-00000600: 692e 7072 6f70 6572 7469 6573 5f64 6174  i.properties_dat
-00000610: 615f 6172 6d61 7475 7265 0a69 6d70 6f72  a_armature.impor
-00000620: 7420 626c 5f75 692e 7370 6163 655f 6f75  t bl_ui.space_ou
-00000630: 746c 696e 6572 0a69 6d70 6f72 7420 626c  tliner.import bl
-00000640: 5f75 692e 7072 6f70 6572 7469 6573 5f72  _ui.properties_r
-00000650: 656e 6465 720a 696d 706f 7274 2062 6c5f  ender.import bl_
-00000660: 7569 2e70 726f 7065 7274 6965 735f 6461  ui.properties_da
-00000670: 7461 5f6d 6573 680a 696d 706f 7274 2062  ta_mesh.import b
-00000680: 6c5f 6f70 6572 6174 6f72 732e 7072 6573  l_operators.pres
-00000690: 6574 730a 696d 706f 7274 2062 6c5f 7569  ets.import bl_ui
-000006a0: 2e70 726f 7065 7274 6965 735f 7061 696e  .properties_pain
-000006b0: 745f 636f 6d6d 6f6e 0a69 6d70 6f72 7420  t_common.import 
-000006c0: 626c 5f75 692e 7370 6163 655f 7072 6f70  bl_ui.space_prop
-000006d0: 6572 7469 6573 0a69 6d70 6f72 7420 626c  erties.import bl
-000006e0: 5f75 692e 7072 6f70 6572 7469 6573 5f70  _ui.properties_p
-000006f0: 6879 7369 6373 5f63 6f6d 6d6f 6e0a 696d  hysics_common.im
-00000700: 706f 7274 2062 6c5f 7569 2e6e 6f64 655f  port bl_ui.node_
-00000710: 6164 645f 6d65 6e75 5f67 656f 6d65 7472  add_menu_geometr
-00000720: 790a 696d 706f 7274 2062 6c5f 7569 2e73  y.import bl_ui.s
-00000730: 7061 6365 5f67 7261 7068 0a69 6d70 6f72  pace_graph.impor
-00000740: 7420 626c 5f75 692e 7370 6163 655f 6e6f  t bl_ui.space_no
-00000750: 6465 0a69 6d70 6f72 7420 626c 5f75 692e  de.import bl_ui.
-00000760: 7072 6f70 6572 7469 6573 5f67 7265 6173  properties_greas
-00000770: 655f 7065 6e63 696c 5f63 6f6d 6d6f 6e0a  e_pencil_common.
-00000780: 696d 706f 7274 2062 6c5f 7569 2e73 7061  import bl_ui.spa
-00000790: 6365 5f76 6965 7733 640a 696d 706f 7274  ce_view3d.import
-000007a0: 2062 6c5f 7569 2e73 7061 6365 5f6e 6c61   bl_ui.space_nla
-000007b0: 0a69 6d70 6f72 7420 626c 5f75 692e 7370  .import bl_ui.sp
-000007c0: 6163 655f 7370 7265 6164 7368 6565 740a  ace_spreadsheet.
-000007d0: 696d 706f 7274 2062 6c5f 7569 2e73 7061  import bl_ui.spa
-000007e0: 6365 5f75 7365 7270 7265 660a 696d 706f  ce_userpref.impo
-000007f0: 7274 2062 6c5f 6f70 6572 6174 6f72 732e  rt bl_operators.
-00000800: 6173 7365 7473 0a69 6d70 6f72 7420 626c  assets.import bl
-00000810: 5f75 692e 7370 6163 655f 746f 6f6c 7379  _ui.space_toolsy
-00000820: 7374 656d 5f63 6f6d 6d6f 6e0a 696d 706f  stem_common.impo
-00000830: 7274 2062 6c5f 7569 2e70 726f 7065 7274  rt bl_ui.propert
-00000840: 6965 735f 6461 7461 5f6d 6f64 6966 6965  ies_data_modifie
-00000850: 720a 696d 706f 7274 2062 6c5f 7569 2e70  r.import bl_ui.p
-00000860: 726f 7065 7274 6965 735f 7061 7274 6963  roperties_partic
-00000870: 6c65 0a69 6d70 6f72 7420 626c 5f75 692e  le.import bl_ui.
-00000880: 7072 6f70 6572 7469 6573 5f70 6879 7369  properties_physi
-00000890: 6373 5f73 6f66 7462 6f64 790a 696d 706f  cs_softbody.impo
-000008a0: 7274 2062 6c5f 7569 2e67 656e 6572 6963  rt bl_ui.generic
-000008b0: 5f75 695f 6c69 7374 0a69 6d70 6f72 7420  _ui_list.import 
-000008c0: 626c 5f75 692e 7370 6163 655f 6669 6c65  bl_ui.space_file
-000008d0: 6272 6f77 7365 720a 696d 706f 7274 2062  browser.import b
-000008e0: 6c5f 7569 2e70 726f 7065 7274 6965 735f  l_ui.properties_
-000008f0: 6f62 6a65 6374 0a69 6d70 6f72 7420 626c  object.import bl
-00000900: 5f75 692e 7072 6f70 6572 7469 6573 5f64  _ui.properties_d
-00000910: 6174 615f 626f 6e65 0a69 6d70 6f72 7420  ata_bone.import 
-00000920: 626c 5f6f 7065 7261 746f 7273 2e74 6578  bl_operators.tex
-00000930: 740a 696d 706f 7274 2062 6c5f 6f70 6572  t.import bl_oper
-00000940: 6174 6f72 732e 7669 6577 3364 0a69 6d70  ators.view3d.imp
-00000950: 6f72 7420 626c 5f75 692e 7370 6163 655f  ort bl_ui.space_
-00000960: 7469 6d65 0a69 6d70 6f72 7420 626c 5f75  time.import bl_u
-00000970: 692e 7072 6f70 6572 7469 6573 5f64 6174  i.properties_dat
-00000980: 615f 706f 696e 7463 6c6f 7564 0a69 6d70  a_pointcloud.imp
-00000990: 6f72 7420 626c 5f75 692e 7072 6f70 6572  ort bl_ui.proper
-000009a0: 7469 6573 5f70 6879 7369 6373 5f64 796e  ties_physics_dyn
-000009b0: 616d 6963 7061 696e 740a 696d 706f 7274  amicpaint.import
-000009c0: 2062 6c5f 7569 2e70 726f 7065 7274 6965   bl_ui.propertie
-000009d0: 735f 7068 7973 6963 735f 666c 7569 640a  s_physics_fluid.
+00000050: 615f 6361 6d65 7261 0a69 6d70 6f72 7420  a_camera.import 
+00000060: 626c 5f75 692e 7370 6163 655f 7573 6572  bl_ui.space_user
+00000070: 7072 6566 0a69 6d70 6f72 7420 626c 5f75  pref.import bl_u
+00000080: 692e 7370 6163 655f 696d 6167 650a 696d  i.space_image.im
+00000090: 706f 7274 2062 6c5f 7569 2e70 726f 7065  port bl_ui.prope
+000000a0: 7274 6965 735f 6772 6561 7365 5f70 656e  rties_grease_pen
+000000b0: 6369 6c5f 636f 6d6d 6f6e 0a69 6d70 6f72  cil_common.impor
+000000c0: 7420 626c 5f75 692e 7072 6f70 6572 7469  t bl_ui.properti
+000000d0: 6573 5f6d 6174 6572 6961 6c5f 6770 656e  es_material_gpen
+000000e0: 6369 6c0a 696d 706f 7274 2062 6c5f 7569  cil.import bl_ui
+000000f0: 2e73 7061 6365 5f66 696c 6562 726f 7773  .space_filebrows
+00000100: 6572 0a69 6d70 6f72 7420 626c 5f75 692e  er.import bl_ui.
+00000110: 7072 6f70 6572 7469 6573 5f70 6879 7369  properties_physi
+00000120: 6373 5f63 6f6d 6d6f 6e0a 696d 706f 7274  cs_common.import
+00000130: 2062 6c5f 7569 2e70 726f 7065 7274 6965   bl_ui.propertie
+00000140: 735f 6461 7461 5f65 6d70 7479 0a69 6d70  s_data_empty.imp
+00000150: 6f72 7420 626c 5f6f 7065 7261 746f 7273  ort bl_operators
+00000160: 2e61 7373 6574 730a 696d 706f 7274 2062  .assets.import b
+00000170: 6c5f 7569 2e70 726f 7065 7274 6965 735f  l_ui.properties_
+00000180: 6461 7461 5f73 7065 616b 6572 0a69 6d70  data_speaker.imp
+00000190: 6f72 7420 626c 5f75 692e 7370 6163 655f  ort bl_ui.space_
+000001a0: 696e 666f 0a69 6d70 6f72 7420 626c 5f75  info.import bl_u
+000001b0: 692e 7072 6f70 6572 7469 6573 5f6f 7574  i.properties_out
+000001c0: 7075 740a 696d 706f 7274 2062 6c5f 7569  put.import bl_ui
+000001d0: 2e73 7061 6365 5f74 696d 650a 696d 706f  .space_time.impo
+000001e0: 7274 2062 6c5f 7569 2e73 7061 6365 5f70  rt bl_ui.space_p
+000001f0: 726f 7065 7274 6965 730a 696d 706f 7274  roperties.import
+00000200: 2062 6c5f 7569 2e70 726f 7065 7274 6965   bl_ui.propertie
+00000210: 735f 7465 7874 7572 650a 696d 706f 7274  s_texture.import
+00000220: 2062 6c5f 6f70 6572 6174 6f72 732e 6f62   bl_operators.ob
+00000230: 6a65 6374 0a69 6d70 6f72 7420 626c 5f75  ject.import bl_u
+00000240: 692e 7072 6f70 6572 7469 6573 5f64 6174  i.properties_dat
+00000250: 615f 6770 656e 6369 6c0a 696d 706f 7274  a_gpencil.import
+00000260: 2062 6c5f 6f70 6572 6174 6f72 732e 7573   bl_operators.us
+00000270: 6572 7072 6566 0a69 6d70 6f72 7420 626c  erpref.import bl
+00000280: 5f6f 7065 7261 746f 7273 2e61 6e69 6d0a  _operators.anim.
+00000290: 696d 706f 7274 2062 6c5f 7569 2e73 7061  import bl_ui.spa
+000002a0: 6365 5f6e 6f64 650a 696d 706f 7274 2062  ce_node.import b
+000002b0: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
+000002c0: 645f 746f 6f6c 6261 720a 696d 706f 7274  d_toolbar.import
+000002d0: 2062 6c5f 7569 2e70 726f 7065 7274 6965   bl_ui.propertie
+000002e0: 735f 7068 7973 6963 735f 7269 6769 6462  s_physics_rigidb
+000002f0: 6f64 795f 636f 6e73 7472 6169 6e74 0a69  ody_constraint.i
+00000300: 6d70 6f72 7420 626c 5f75 692e 7072 6f70  mport bl_ui.prop
+00000310: 6572 7469 6573 5f64 6174 615f 6d65 7368  erties_data_mesh
+00000320: 0a69 6d70 6f72 7420 626c 5f75 692e 7072  .import bl_ui.pr
+00000330: 6f70 6572 7469 6573 5f64 6174 615f 6c61  operties_data_la
+00000340: 7474 6963 650a 696d 706f 7274 2062 6c5f  ttice.import bl_
+00000350: 6f70 6572 6174 6f72 732e 636f 6e73 7472  operators.constr
+00000360: 6169 6e74 0a69 6d70 6f72 7420 626c 5f75  aint.import bl_u
+00000370: 692e 7072 6f70 6572 7469 6573 5f70 6879  i.properties_phy
+00000380: 7369 6373 5f66 6c75 6964 0a69 6d70 6f72  sics_fluid.impor
+00000390: 7420 626c 5f6f 7065 7261 746f 7273 2e63  t bl_operators.c
+000003a0: 6c69 700a 696d 706f 7274 2062 6c5f 7569  lip.import bl_ui
+000003b0: 2e70 726f 7065 7274 6965 735f 6672 6565  .properties_free
+000003c0: 7374 796c 650a 696d 706f 7274 2062 6c5f  style.import bl_
+000003d0: 7569 2e70 726f 7065 7274 6965 735f 7068  ui.properties_ph
+000003e0: 7973 6963 735f 6669 656c 640a 696d 706f  ysics_field.impo
+000003f0: 7274 2062 6c5f 7569 2e70 726f 7065 7274  rt bl_ui.propert
+00000400: 6965 735f 636f 6e73 7472 6169 6e74 0a69  ies_constraint.i
+00000410: 6d70 6f72 7420 626c 5f75 692e 7370 6163  mport bl_ui.spac
+00000420: 655f 7465 7874 0a69 6d70 6f72 7420 626c  e_text.import bl
+00000430: 5f75 692e 7072 6f70 6572 7469 6573 5f72  _ui.properties_r
+00000440: 656e 6465 720a 696d 706f 7274 2062 6c5f  ender.import bl_
+00000450: 7569 2e70 726f 7065 7274 6965 735f 6461  ui.properties_da
+00000460: 7461 5f6d 6574 6162 616c 6c0a 696d 706f  ta_metaball.impo
+00000470: 7274 2062 6c5f 7569 2e73 7061 6365 5f6e  rt bl_ui.space_n
+00000480: 6c61 0a69 6d70 6f72 7420 626c 5f75 692e  la.import bl_ui.
+00000490: 7072 6f70 6572 7469 6573 5f70 6169 6e74  properties_paint
+000004a0: 5f63 6f6d 6d6f 6e0a 696d 706f 7274 2062  _common.import b
+000004b0: 6c5f 7569 2e70 726f 7065 7274 6965 735f  l_ui.properties_
+000004c0: 6461 7461 5f6c 6967 6874 7072 6f62 650a  data_lightprobe.
+000004d0: 696d 706f 7274 2062 6c5f 7569 2e73 7061  import bl_ui.spa
+000004e0: 6365 5f67 7261 7068 0a69 6d70 6f72 7420  ce_graph.import 
+000004f0: 626c 5f75 692e 7072 6f70 6572 7469 6573  bl_ui.properties
+00000500: 5f77 6f72 6c64 0a69 6d70 6f72 7420 626c  _world.import bl
+00000510: 5f75 692e 7072 6f70 6572 7469 6573 5f64  _ui.properties_d
+00000520: 6174 615f 766f 6c75 6d65 0a69 6d70 6f72  ata_volume.impor
+00000530: 7420 626c 5f75 692e 7370 6163 655f 7365  t bl_ui.space_se
+00000540: 7175 656e 6365 720a 696d 706f 7274 2062  quencer.import b
+00000550: 6c5f 6f70 6572 6174 6f72 732e 6672 6565  l_operators.free
+00000560: 7374 796c 650a 696d 706f 7274 2062 6c5f  style.import bl_
+00000570: 7569 0a69 6d70 6f72 7420 626c 5f75 692e  ui.import bl_ui.
+00000580: 7370 6163 655f 746f 6f6c 7379 7374 656d  space_toolsystem
+00000590: 5f74 6f6f 6c62 6172 0a69 6d70 6f72 7420  _toolbar.import 
+000005a0: 626c 5f75 692e 7072 6f70 6572 7469 6573  bl_ui.properties
+000005b0: 5f64 6174 615f 626f 6e65 0a69 6d70 6f72  _data_bone.impor
+000005c0: 7420 626c 5f75 692e 7072 6f70 6572 7469  t bl_ui.properti
+000005d0: 6573 5f70 6172 7469 636c 650a 696d 706f  es_particle.impo
+000005e0: 7274 2062 6c5f 7569 2e70 726f 7065 7274  rt bl_ui.propert
+000005f0: 6965 735f 6d61 7465 7269 616c 0a69 6d70  ies_material.imp
+00000600: 6f72 7420 626c 5f75 692e 7370 6163 655f  ort bl_ui.space_
+00000610: 7669 6577 3364 0a69 6d70 6f72 7420 626c  view3d.import bl
+00000620: 5f6f 7065 7261 746f 7273 2e76 6965 7733  _operators.view3
+00000630: 640a 696d 706f 7274 2062 6c5f 7569 2e70  d.import bl_ui.p
+00000640: 726f 7065 7274 6965 735f 776f 726b 7370  roperties_worksp
+00000650: 6163 650a 696d 706f 7274 2062 6c5f 7569  ace.import bl_ui
+00000660: 2e73 7061 6365 5f64 6f70 6573 6865 6574  .space_dopesheet
+00000670: 0a69 6d70 6f72 7420 626c 5f75 692e 7072  .import bl_ui.pr
+00000680: 6f70 6572 7469 6573 5f64 6174 615f 6172  operties_data_ar
+00000690: 6d61 7475 7265 0a69 6d70 6f72 7420 626c  mature.import bl
+000006a0: 5f75 692e 7072 6f70 6572 7469 6573 5f64  _ui.properties_d
+000006b0: 6174 615f 6c69 6768 740a 696d 706f 7274  ata_light.import
+000006c0: 2062 6c5f 7569 2e70 726f 7065 7274 6965   bl_ui.propertie
+000006d0: 735f 6461 7461 5f73 6861 6465 7266 780a  s_data_shaderfx.
+000006e0: 696d 706f 7274 2062 6c5f 7569 2e73 7061  import bl_ui.spa
+000006f0: 6365 5f74 6f6f 6c73 7973 7465 6d5f 636f  ce_toolsystem_co
+00000700: 6d6d 6f6e 0a69 6d70 6f72 7420 626c 5f6f  mmon.import bl_o
+00000710: 7065 7261 746f 7273 2e77 6d0a 696d 706f  perators.wm.impo
+00000720: 7274 2062 6c5f 7569 2e67 656e 6572 6963  rt bl_ui.generic
+00000730: 5f75 695f 6c69 7374 0a69 6d70 6f72 7420  _ui_list.import 
+00000740: 626c 5f75 692e 7072 6f70 6572 7469 6573  bl_ui.properties
+00000750: 5f6d 6173 6b5f 636f 6d6d 6f6e 0a69 6d70  _mask_common.imp
+00000760: 6f72 7420 626c 5f75 692e 7370 6163 655f  ort bl_ui.space_
+00000770: 636c 6970 0a69 6d70 6f72 7420 626c 5f75  clip.import bl_u
+00000780: 692e 7370 6163 655f 7370 7265 6164 7368  i.space_spreadsh
+00000790: 6565 740a 696d 706f 7274 2062 6c5f 7569  eet.import bl_ui
+000007a0: 2e70 726f 7065 7274 6965 735f 7068 7973  .properties_phys
+000007b0: 6963 735f 7269 6769 6462 6f64 790a 696d  ics_rigidbody.im
+000007c0: 706f 7274 2062 6c5f 7569 2e73 7061 6365  port bl_ui.space
+000007d0: 5f74 6f70 6261 720a 696d 706f 7274 2062  _topbar.import b
+000007e0: 6c5f 6f70 6572 6174 6f72 732e 6e6f 6465  l_operators.node
+000007f0: 0a69 6d70 6f72 7420 626c 5f75 692e 7072  .import bl_ui.pr
+00000800: 6f70 6572 7469 6573 5f64 6174 615f 6375  operties_data_cu
+00000810: 7276 650a 696d 706f 7274 2062 6c5f 7569  rve.import bl_ui
+00000820: 2e70 726f 7065 7274 6965 735f 7068 7973  .properties_phys
+00000830: 6963 735f 736f 6674 626f 6479 0a69 6d70  ics_softbody.imp
+00000840: 6f72 7420 626c 5f75 692e 7072 6f70 6572  ort bl_ui.proper
+00000850: 7469 6573 5f73 6365 6e65 0a69 6d70 6f72  ties_scene.impor
+00000860: 7420 626c 5f75 692e 7072 6f70 6572 7469  t bl_ui.properti
+00000870: 6573 5f70 6879 7369 6373 5f67 656f 6d65  es_physics_geome
+00000880: 7472 795f 6e6f 6465 730a 696d 706f 7274  try_nodes.import
+00000890: 2062 6c5f 7569 2e70 726f 7065 7274 6965   bl_ui.propertie
+000008a0: 735f 7068 7973 6963 735f 636c 6f74 680a  s_physics_cloth.
+000008b0: 696d 706f 7274 2062 6c5f 6f70 6572 6174  import bl_operat
+000008c0: 6f72 732e 6669 6c65 0a69 6d70 6f72 7420  ors.file.import 
+000008d0: 626c 5f75 692e 7370 6163 655f 7374 6174  bl_ui.space_stat
+000008e0: 7573 6261 720a 696d 706f 7274 2062 6c5f  usbar.import bl_
+000008f0: 7569 2e6e 6f64 655f 6164 645f 6d65 6e75  ui.node_add_menu
+00000900: 5f67 656f 6d65 7472 790a 696d 706f 7274  _geometry.import
+00000910: 2062 6c5f 6f70 6572 6174 6f72 732e 7072   bl_operators.pr
+00000920: 6573 6574 730a 696d 706f 7274 2062 6c5f  esets.import bl_
+00000930: 7569 2e73 7061 6365 5f63 6f6e 736f 6c65  ui.space_console
+00000940: 0a69 6d70 6f72 7420 626c 5f75 692e 7072  .import bl_ui.pr
+00000950: 6f70 6572 7469 6573 5f63 6f6c 6c65 6374  operties_collect
+00000960: 696f 6e0a 696d 706f 7274 2062 6c5f 7569  ion.import bl_ui
+00000970: 2e70 726f 7065 7274 6965 735f 7669 6577  .properties_view
+00000980: 5f6c 6179 6572 0a69 6d70 6f72 7420 626c  _layer.import bl
+00000990: 5f75 692e 7370 6163 655f 6f75 746c 696e  _ui.space_outlin
+000009a0: 6572 0a69 6d70 6f72 7420 626c 5f6f 7065  er.import bl_ope
+000009b0: 7261 746f 7273 2e74 6578 740a 696d 706f  rators.text.impo
+000009c0: 7274 2062 6c5f 7569 2e70 726f 7065 7274  rt bl_ui.propert
+000009d0: 6965 735f 6461 7461 5f63 7572 7665 730a  ies_data_curves.
 000009e0: 696d 706f 7274 2062 6c5f 7569 2e70 726f  import bl_ui.pro
-000009f0: 7065 7274 6965 735f 776f 726c 640a 696d  perties_world.im
-00000a00: 706f 7274 2062 6c5f 7569 2e73 7061 6365  port bl_ui.space
-00000a10: 5f69 6e66 6f0a 696d 706f 7274 2062 6c5f  _info.import bl_
-00000a20: 7569 2e73 7061 6365 5f63 6f6e 736f 6c65  ui.space_console
-00000a30: 0a69 6d70 6f72 7420 626c 5f6f 7065 7261  .import bl_opera
-00000a40: 746f 7273 2e73 7072 6561 6473 6865 6574  tors.spreadsheet
-00000a50: 0a69 6d70 6f72 7420 626c 5f75 692e 7072  .import bl_ui.pr
-00000a60: 6f70 6572 7469 6573 5f63 6f6c 6c65 6374  operties_collect
-00000a70: 696f 6e0a 696d 706f 7274 2062 6c5f 7569  ion.import bl_ui
-00000a80: 2e73 7061 6365 5f74 6f6f 6c73 7973 7465  .space_toolsyste
-00000a90: 6d5f 746f 6f6c 6261 720a 0a47 656e 6572  m_toolbar..Gener
+000009f0: 7065 7274 6965 735f 6461 7461 5f6d 6f64  perties_data_mod
+00000a00: 6966 6965 720a 696d 706f 7274 2062 6c5f  ifier.import bl_
+00000a10: 7569 2e70 726f 7065 7274 6965 735f 6f62  ui.properties_ob
+00000a20: 6a65 6374 0a69 6d70 6f72 7420 626c 5f75  ject.import bl_u
+00000a30: 692e 7072 6f70 6572 7469 6573 5f70 6879  i.properties_phy
+00000a40: 7369 6373 5f64 796e 616d 6963 7061 696e  sics_dynamicpain
+00000a50: 740a 696d 706f 7274 2062 6c5f 6f70 6572  t.import bl_oper
+00000a60: 6174 6f72 732e 7370 7265 6164 7368 6565  ators.spreadshee
+00000a70: 740a 696d 706f 7274 2062 6c5f 7569 2e70  t.import bl_ui.p
+00000a80: 726f 7065 7274 6965 735f 6461 7461 5f70  roperties_data_p
+00000a90: 6f69 6e74 636c 6f75 640a 0a47 656e 6572  ointcloud..Gener
 00000aa0: 6963 5479 7065 203d 2074 7970 696e 672e  icType = typing.
 00000ab0: 5479 7065 5661 7228 2247 656e 6572 6963  TypeVar("Generic
 00000ac0: 5479 7065 2229 0a0a 0a63 6c61 7373 2062  Type")...class b
-00000ad0: 7079 5f73 7472 7563 743a 0a20 2020 2027  py_struct:.    '
-00000ae0: 2727 2062 7569 6c74 2d69 6e20 6261 7365  '' built-in base
-00000af0: 2063 6c61 7373 2066 6f72 2061 6c6c 2063   class for all c
-00000b00: 6c61 7373 6573 2069 6e20 6270 792e 7479  lasses in bpy.ty
-00000b10: 7065 732e 0a20 2020 2027 2727 0a0a 2020  pes..    '''..  
-00000b20: 2020 6964 5f64 6174 6120 3d20 4e6f 6e65    id_data = None
-00000b30: 0a20 2020 2027 2727 2054 6865 2060 6270  .    ''' The `bp
-00000b40: 792e 7479 7065 732e 4944 6020 6f62 6a65  y.types.ID` obje
-00000b50: 6374 2074 6869 7320 6461 7461 626c 6f63  ct this databloc
-00000b60: 6b20 6973 2066 726f 6d20 6f72 204e 6f6e  k is from or Non
-00000b70: 652c 2028 6e6f 7420 6176 6169 6c61 626c  e, (not availabl
-00000b80: 6520 666f 7220 616c 6c20 6461 7461 2074  e for all data t
-00000b90: 7970 6573 2927 2727 0a0a 2020 2020 6465  ypes)'''..    de
-00000ba0: 6620 6173 5f70 6f69 6e74 6572 2873 656c  f as_pointer(sel
-00000bb0: 6629 202d 3e20 696e 743a 0a20 2020 2020  f) -> int:.     
-00000bc0: 2020 2027 2727 2052 6574 7572 6e73 2074     ''' Returns t
-00000bd0: 6865 206d 656d 6f72 7920 6164 6472 6573  he memory addres
-00000be0: 7320 7768 6963 6820 686f 6c64 7320 6120  s which holds a 
-00000bf0: 706f 696e 7465 7220 746f 2042 6c65 6e64  pointer to Blend
-00000c00: 6572 2773 2069 6e74 6572 6e61 6c20 6461  er's internal da
-00000c10: 7461 0a0a 2020 2020 2020 2020 3a72 7479  ta..        :rty
-00000c20: 7065 3a20 696e 740a 2020 2020 2020 2020  pe: int.        
-00000c30: 3a72 6574 7572 6e3a 2069 6e74 2028 6d65  :return: int (me
-00000c40: 6d6f 7279 2061 6464 7265 7373 292e 0a20  mory address).. 
-00000c50: 2020 2020 2020 2027 2727 0a20 2020 2020         '''.     
-00000c60: 2020 2070 6173 730a 0a20 2020 2064 6566     pass..    def
-00000c70: 2064 7269 7665 725f 6164 6428 7365 6c66   driver_add(self
-00000c80: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00000c90: 2020 2020 2070 6174 683a 2074 7970 696e       path: typin
-00000ca0: 672e 4f70 7469 6f6e 616c 5b73 7472 5d2c  g.Optional[str],
-00000cb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000cc0: 2020 2020 696e 6465 783a 2074 7970 696e      index: typin
-00000cd0: 672e 4f70 7469 6f6e 616c 5b69 6e74 5d20  g.Optional[int] 
-00000ce0: 3d20 2d31 2920 2d3e 2027 4643 7572 7665  = -1) -> 'FCurve
-00000cf0: 273a 0a20 2020 2020 2020 2027 2727 2041  ':.        ''' A
-00000d00: 6464 7320 6472 6976 6572 2873 2920 746f  dds driver(s) to
-00000d10: 2074 6865 2067 6976 656e 2070 726f 7065   the given prope
-00000d20: 7274 790a 0a20 2020 2020 2020 203a 7061  rty..        :pa
-00000d30: 7261 6d20 7061 7468 3a20 7061 7468 2074  ram path: path t
-00000d40: 6f20 7468 6520 7072 6f70 6572 7479 2074  o the property t
-00000d50: 6f20 6472 6976 652c 2061 6e61 6c6f 676f  o drive, analogo
-00000d60: 7573 2074 6f20 7468 6520 6663 7572 7665  us to the fcurve
-00000d70: 2773 2064 6174 6120 7061 7468 2e0a 2020  's data path..  
-00000d80: 2020 2020 2020 3a74 7970 6520 7061 7468        :type path
-00000d90: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
-00000da0: 6c5b 7374 725d 0a20 2020 2020 2020 203a  l[str].        :
-00000db0: 7061 7261 6d20 696e 6465 783a 2061 7272  param index: arr
-00000dc0: 6179 2069 6e64 6578 206f 6620 7468 6520  ay index of the 
-00000dd0: 7072 6f70 6572 7479 2064 7269 7665 2e20  property drive. 
-00000de0: 4465 6661 756c 7473 2074 6f20 2d31 2066  Defaults to -1 f
-00000df0: 6f72 2061 6c6c 2069 6e64 6963 6573 206f  or all indices o
-00000e00: 7220 6120 7369 6e67 6c65 2063 6861 6e6e  r a single chann
-00000e10: 656c 2069 6620 7468 6520 7072 6f70 6572  el if the proper
-00000e20: 7479 2069 7320 6e6f 7420 616e 2061 7272  ty is not an arr
-00000e30: 6179 2e0a 2020 2020 2020 2020 3a74 7970  ay..        :typ
-00000e40: 6520 696e 6465 783a 2074 7970 696e 672e  e index: typing.
-00000e50: 4f70 7469 6f6e 616c 5b69 6e74 5d0a 2020  Optional[int].  
-00000e60: 2020 2020 2020 3a72 7479 7065 3a20 2746        :rtype: 'F
-00000e70: 4375 7276 6527 0a20 2020 2020 2020 203a  Curve'.        :
-00000e80: 7265 7475 726e 3a20 5468 6520 6472 6976  return: The driv
-00000e90: 6572 2873 2920 6164 6465 642e 0a20 2020  er(s) added..   
-00000ea0: 2020 2020 2027 2727 0a20 2020 2020 2020       '''.       
-00000eb0: 2070 6173 730a 0a20 2020 2064 6566 2064   pass..    def d
-00000ec0: 7269 7665 725f 7265 6d6f 7665 2873 656c  river_remove(sel
-00000ed0: 662c 0a20 2020 2020 2020 2020 2020 2020  f,.             
-00000ee0: 2020 2020 2020 2020 2070 6174 683a 2074           path: t
-00000ef0: 7970 696e 672e 4f70 7469 6f6e 616c 5b73  yping.Optional[s
-00000f00: 7472 5d2c 0a20 2020 2020 2020 2020 2020  tr],.           
-00000f10: 2020 2020 2020 2020 2020 2069 6e64 6578             index
-00000f20: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
-00000f30: 6c5b 696e 745d 203d 202d 3129 202d 3e20  l[int] = -1) -> 
-00000f40: 626f 6f6c 3a0a 2020 2020 2020 2020 2727  bool:.        ''
-00000f50: 2720 5265 6d6f 7665 2064 7269 7665 7228  ' Remove driver(
-00000f60: 7329 2066 726f 6d20 7468 6520 6769 7665  s) from the give
-00000f70: 6e20 7072 6f70 6572 7479 0a0a 2020 2020  n property..    
-00000f80: 2020 2020 3a70 6172 616d 2070 6174 683a      :param path:
-00000f90: 2070 6174 6820 746f 2074 6865 2070 726f   path to the pro
-00000fa0: 7065 7274 7920 746f 2064 7269 7665 2c20  perty to drive, 
-00000fb0: 616e 616c 6f67 6f75 7320 746f 2074 6865  analogous to the
-00000fc0: 2066 6375 7276 6527 7320 6461 7461 2070   fcurve's data p
-00000fd0: 6174 682e 0a20 2020 2020 2020 203a 7479  ath..        :ty
-00000fe0: 7065 2070 6174 683a 2074 7970 696e 672e  pe path: typing.
-00000ff0: 4f70 7469 6f6e 616c 5b73 7472 5d0a 2020  Optional[str].  
-00001000: 2020 2020 2020 3a70 6172 616d 2069 6e64        :param ind
-00001010: 6578 3a20 6172 7261 7920 696e 6465 7820  ex: array index 
-00001020: 6f66 2074 6865 2070 726f 7065 7274 7920  of the property 
-00001030: 6472 6976 652e 2044 6566 6175 6c74 7320  drive. Defaults 
-00001040: 746f 202d 3120 666f 7220 616c 6c20 696e  to -1 for all in
-00001050: 6469 6365 7320 6f72 2061 2073 696e 676c  dices or a singl
-00001060: 6520 6368 616e 6e65 6c20 6966 2074 6865  e channel if the
-00001070: 2070 726f 7065 7274 7920 6973 206e 6f74   property is not
-00001080: 2061 6e20 6172 7261 792e 0a20 2020 2020   an array..     
-00001090: 2020 203a 7479 7065 2069 6e64 6578 3a20     :type index: 
-000010a0: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
-000010b0: 696e 745d 0a20 2020 2020 2020 203a 7274  int].        :rt
-000010c0: 7970 653a 2062 6f6f 6c0a 2020 2020 2020  ype: bool.      
-000010d0: 2020 3a72 6574 7572 6e3a 2053 7563 6365    :return: Succe
-000010e0: 7373 206f 6620 6472 6976 6572 2072 656d  ss of driver rem
-000010f0: 6f76 616c 2e0a 2020 2020 2020 2020 2727  oval..        ''
-00001100: 270a 2020 2020 2020 2020 7061 7373 0a0a  '.        pass..
-00001110: 2020 2020 6465 6620 6765 7428 7365 6c66      def get(self
-00001120: 2c0a 2020 2020 2020 2020 2020 2020 6b65  ,.            ke
-00001130: 793a 2074 7970 696e 672e 4f70 7469 6f6e  y: typing.Option
-00001140: 616c 5b73 7472 5d2c 0a20 2020 2020 2020  al[str],.       
-00001150: 2020 2020 2064 6566 6175 6c74 3a20 7479       default: ty
-00001160: 7069 6e67 2e4f 7074 696f 6e61 6c5b 7479  ping.Optional[ty
-00001170: 7069 6e67 2e41 6e79 5d20 3d20 4e6f 6e65  ping.Any] = None
-00001180: 293a 0a20 2020 2020 2020 2027 2727 2052  ):.        ''' R
-00001190: 6574 7572 6e73 2074 6865 2076 616c 7565  eturns the value
-000011a0: 206f 6620 7468 6520 6375 7374 6f6d 2070   of the custom p
-000011b0: 726f 7065 7274 7920 6173 7369 676e 6564  roperty assigned
-000011c0: 2074 6f20 6b65 7920 6f72 2064 6566 6175   to key or defau
-000011d0: 6c74 2077 6865 6e20 6e6f 7420 666f 756e  lt when not foun
-000011e0: 6420 286d 6174 6368 6573 2050 7974 686f  d (matches Pytho
-000011f0: 6e27 7320 6469 6374 696f 6e61 7279 2066  n's dictionary f
-00001200: 756e 6374 696f 6e20 6f66 2074 6865 2073  unction of the s
-00001210: 616d 6520 6e61 6d65 292e 0a0a 2020 2020  ame name)...    
-00001220: 2020 2020 3a70 6172 616d 206b 6579 3a20      :param key: 
-00001230: 5468 6520 6b65 7920 6173 736f 6369 6174  The key associat
-00001240: 6564 2077 6974 6820 7468 6520 6375 7374  ed with the cust
-00001250: 6f6d 2070 726f 7065 7274 792e 0a20 2020  om property..   
-00001260: 2020 2020 203a 7479 7065 206b 6579 3a20       :type key: 
-00001270: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
-00001280: 7374 725d 0a20 2020 2020 2020 203a 7061  str].        :pa
-00001290: 7261 6d20 6465 6661 756c 743a 204f 7074  ram default: Opt
-000012a0: 696f 6e61 6c20 6172 6775 6d65 6e74 2066  ional argument f
-000012b0: 6f72 2074 6865 2076 616c 7565 2074 6f20  or the value to 
-000012c0: 7265 7475 726e 2069 6620 2a6b 6579 2a20  return if *key* 
-000012d0: 6973 206e 6f74 2066 6f75 6e64 2e0a 2020  is not found..  
-000012e0: 2020 2020 2020 3a74 7970 6520 6465 6661        :type defa
-000012f0: 756c 743a 2074 7970 696e 672e 4f70 7469  ult: typing.Opti
-00001300: 6f6e 616c 5b74 7970 696e 672e 416e 795d  onal[typing.Any]
-00001310: 0a20 2020 2020 2020 2027 2727 0a20 2020  .        '''.   
-00001320: 2020 2020 2070 6173 730a 0a20 2020 2064       pass..    d
-00001330: 6566 2069 645f 7072 6f70 6572 7469 6573  ef id_properties
-00001340: 5f63 6c65 6172 2873 656c 6629 3a0a 2020  _clear(self):.  
-00001350: 2020 2020 2020 2727 2720 0a0a 2020 2020        ''' ..    
-00001360: 2020 2020 2727 270a 2020 2020 2020 2020      '''.        
-00001370: 7061 7373 0a0a 2020 2020 6465 6620 6964  pass..    def id
-00001380: 5f70 726f 7065 7274 6965 735f 656e 7375  _properties_ensu
-00001390: 7265 2873 656c 6629 202d 3e20 7479 7069  re(self) -> typi
-000013a0: 6e67 2e41 6e79 3a0a 2020 2020 2020 2020  ng.Any:.        
-000013b0: 2727 2720 0a0a 2020 2020 2020 2020 3a72  ''' ..        :r
-000013c0: 7479 7065 3a20 7479 7069 6e67 2e41 6e79  type: typing.Any
-000013d0: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
-000013e0: 3a20 7468 6520 7061 7265 6e74 2067 726f  : the parent gro
-000013f0: 7570 2066 6f72 2061 6e20 524e 4120 7374  up for an RNA st
-00001400: 7275 6374 2773 2063 7573 746f 6d20 4944  ruct's custom ID
-00001410: 5072 6f70 6572 7469 6573 2e0a 2020 2020  Properties..    
-00001420: 2020 2020 2727 270a 2020 2020 2020 2020      '''.        
-00001430: 7061 7373 0a0a 2020 2020 6465 6620 6964  pass..    def id
-00001440: 5f70 726f 7065 7274 6965 735f 7569 2873  _properties_ui(s
-00001450: 656c 662c 206b 6579 3a20 7479 7069 6e67  elf, key: typing
-00001460: 2e4f 7074 696f 6e61 6c5b 7479 7069 6e67  .Optional[typing
-00001470: 2e41 6e79 5d29 202d 3e20 7479 7069 6e67  .Any]) -> typing
-00001480: 2e41 6e79 3a0a 2020 2020 2020 2020 2727  .Any:.        ''
-00001490: 2720 0a0a 2020 2020 2020 2020 3a70 6172  ' ..        :par
-000014a0: 616d 206b 6579 3a20 2053 7472 696e 6720  am key:  String 
-000014b0: 6e61 6d65 206f 6620 7468 6520 7072 6f70  name of the prop
-000014c0: 6572 7479 2e0a 2020 2020 2020 2020 3a74  erty..        :t
-000014d0: 7970 6520 6b65 793a 2074 7970 696e 672e  ype key: typing.
-000014e0: 4f70 7469 6f6e 616c 5b74 7970 696e 672e  Optional[typing.
-000014f0: 416e 795d 0a20 2020 2020 2020 203a 7274  Any].        :rt
-00001500: 7970 653a 2074 7970 696e 672e 416e 790a  ype: typing.Any.
-00001510: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
-00001520: 2052 6574 7572 6e20 616e 206f 626a 6563   Return an objec
-00001530: 7420 7573 6564 2074 6f20 6d61 6e61 6765  t used to manage
-00001540: 2061 6e20 4944 5072 6f70 6572 7479 2773   an IDProperty's
-00001550: 2055 4920 6461 7461 2e0a 2020 2020 2020   UI data..      
-00001560: 2020 2727 270a 2020 2020 2020 2020 7061    '''.        pa
-00001570: 7373 0a0a 2020 2020 6465 6620 6973 5f70  ss..    def is_p
-00001580: 726f 7065 7274 795f 6869 6464 656e 2873  roperty_hidden(s
-00001590: 656c 662c 2070 726f 7065 7274 7929 202d  elf, property) -
-000015a0: 3e20 626f 6f6c 3a0a 2020 2020 2020 2020  > bool:.        
-000015b0: 2727 2720 4368 6563 6b20 6966 2061 2070  ''' Check if a p
-000015c0: 726f 7065 7274 7920 6973 2068 6964 6465  roperty is hidde
-000015d0: 6e2e 0a0a 2020 2020 2020 2020 3a72 7479  n...        :rty
-000015e0: 7065 3a20 626f 6f6c 0a20 2020 2020 2020  pe: bool.       
-000015f0: 203a 7265 7475 726e 3a20 5472 7565 2077   :return: True w
-00001600: 6865 6e20 7468 6520 7072 6f70 6572 7479  hen the property
-00001610: 2069 7320 6869 6464 656e 2e0a 2020 2020   is hidden..    
-00001620: 2020 2020 2727 270a 2020 2020 2020 2020      '''.        
-00001630: 7061 7373 0a0a 2020 2020 6465 6620 6973  pass..    def is
-00001640: 5f70 726f 7065 7274 795f 6f76 6572 7269  _property_overri
-00001650: 6461 626c 655f 6c69 6272 6172 7928 7365  dable_library(se
-00001660: 6c66 2c20 7072 6f70 6572 7479 2920 2d3e  lf, property) ->
-00001670: 2062 6f6f 6c3a 0a20 2020 2020 2020 2027   bool:.        '
-00001680: 2727 2043 6865 636b 2069 6620 6120 7072  '' Check if a pr
-00001690: 6f70 6572 7479 2069 7320 6f76 6572 7269  operty is overri
-000016a0: 6461 626c 652e 0a0a 2020 2020 2020 2020  dable...        
-000016b0: 3a72 7479 7065 3a20 626f 6f6c 0a20 2020  :rtype: bool.   
-000016c0: 2020 2020 203a 7265 7475 726e 3a20 5472       :return: Tr
-000016d0: 7565 2077 6865 6e20 7468 6520 7072 6f70  ue when the prop
-000016e0: 6572 7479 2069 7320 6f76 6572 7269 6461  erty is overrida
-000016f0: 626c 652e 0a20 2020 2020 2020 2027 2727  ble..        '''
-00001700: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
-00001710: 2020 2064 6566 2069 735f 7072 6f70 6572     def is_proper
-00001720: 7479 5f72 6561 646f 6e6c 7928 7365 6c66  ty_readonly(self
-00001730: 2c20 7072 6f70 6572 7479 2920 2d3e 2062  , property) -> b
-00001740: 6f6f 6c3a 0a20 2020 2020 2020 2027 2727  ool:.        '''
-00001750: 2043 6865 636b 2069 6620 6120 7072 6f70   Check if a prop
-00001760: 6572 7479 2069 7320 7265 6164 6f6e 6c79  erty is readonly
-00001770: 2e0a 0a20 2020 2020 2020 203a 7274 7970  ...        :rtyp
-00001780: 653a 2062 6f6f 6c0a 2020 2020 2020 2020  e: bool.        
-00001790: 3a72 6574 7572 6e3a 2054 7275 6520 7768  :return: True wh
-000017a0: 656e 2074 6865 2070 726f 7065 7274 7920  en the property 
-000017b0: 6973 2072 6561 646f 6e6c 7920 286e 6f74  is readonly (not
-000017c0: 2077 7269 7461 626c 6529 2e0a 2020 2020   writable)..    
-000017d0: 2020 2020 2727 270a 2020 2020 2020 2020      '''.        
-000017e0: 7061 7373 0a0a 2020 2020 6465 6620 6973  pass..    def is
-000017f0: 5f70 726f 7065 7274 795f 7365 7428 7365  _property_set(se
-00001800: 6c66 2c20 7072 6f70 6572 7479 2c0a 2020  lf, property,.  
-00001810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001820: 2020 2020 2020 6768 6f73 743a 2074 7970        ghost: typ
-00001830: 696e 672e 4f70 7469 6f6e 616c 5b62 6f6f  ing.Optional[boo
-00001840: 6c5d 203d 2054 7275 6529 202d 3e20 626f  l] = True) -> bo
-00001850: 6f6c 3a0a 2020 2020 2020 2020 2727 2720  ol:.        ''' 
-00001860: 4368 6563 6b20 6966 2061 2070 726f 7065  Check if a prope
-00001870: 7274 7920 6973 2073 6574 2c20 7573 6520  rty is set, use 
-00001880: 666f 7220 7465 7374 696e 6720 6f70 6572  for testing oper
-00001890: 6174 6f72 2070 726f 7065 7274 6965 732e  ator properties.
-000018a0: 0a0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
-000018b0: 2067 686f 7374 3a20 5573 6564 2066 6f72   ghost: Used for
-000018c0: 206f 7065 7261 746f 7273 2074 6861 7420   operators that 
-000018d0: 7265 2d72 756e 2077 6974 6820 7072 6576  re-run with prev
-000018e0: 696f 7573 2073 6574 7469 6e67 732e 2049  ious settings. I
-000018f0: 6e20 7468 6973 2063 6173 6520 7468 6520  n this case the 
-00001900: 7072 6f70 6572 7479 2069 7320 6e6f 7420  property is not 
-00001910: 6d61 726b 6564 2061 7320 7365 742c 2079  marked as set, y
-00001920: 6574 2074 6865 2076 616c 7565 2066 726f  et the value fro
-00001930: 6d20 7468 6520 7072 6576 696f 7573 2065  m the previous e
-00001940: 7865 6375 7469 6f6e 2069 7320 7573 6564  xecution is used
-00001950: 2e20 496e 2072 6172 6520 6361 7365 7320  . In rare cases 
-00001960: 796f 7520 6d61 7920 7761 6e74 2074 6f20  you may want to 
-00001970: 7365 7420 7468 6973 206f 7074 696f 6e20  set this option 
-00001980: 746f 2066 616c 7365 2e0a 2020 2020 2020  to false..      
-00001990: 2020 3a74 7970 6520 6768 6f73 743a 2074    :type ghost: t
-000019a0: 7970 696e 672e 4f70 7469 6f6e 616c 5b62  yping.Optional[b
-000019b0: 6f6f 6c5d 0a20 2020 2020 2020 203a 7274  ool].        :rt
-000019c0: 7970 653a 2062 6f6f 6c0a 2020 2020 2020  ype: bool.      
-000019d0: 2020 3a72 6574 7572 6e3a 2054 7275 6520    :return: True 
-000019e0: 7768 656e 2074 6865 2070 726f 7065 7274  when the propert
-000019f0: 7920 6861 7320 6265 656e 2073 6574 2e0a  y has been set..
-00001a00: 2020 2020 2020 2020 2727 270a 2020 2020          '''.    
-00001a10: 2020 2020 7061 7373 0a0a 2020 2020 6465      pass..    de
-00001a20: 6620 6974 656d 7328 7365 6c66 2920 2d3e  f items(self) ->
-00001a30: 2074 7970 696e 672e 416e 793a 0a20 2020   typing.Any:.   
-00001a40: 2020 2020 2027 2727 2052 6574 7572 6e73       ''' Returns
-00001a50: 2074 6865 2069 7465 6d73 206f 6620 7468   the items of th
-00001a60: 6973 206f 626a 6563 7473 2063 7573 746f  is objects custo
-00001a70: 6d20 7072 6f70 6572 7469 6573 2028 6d61  m properties (ma
-00001a80: 7463 6865 7320 5079 7468 6f6e 2773 2064  tches Python's d
-00001a90: 6963 7469 6f6e 6172 7920 6675 6e63 7469  ictionary functi
-00001aa0: 6f6e 206f 6620 7468 6520 7361 6d65 206e  on of the same n
-00001ab0: 616d 6529 2e0a 0a20 2020 2020 2020 203a  ame)...        :
-00001ac0: 7274 7970 653a 2074 7970 696e 672e 416e  rtype: typing.An
-00001ad0: 790a 2020 2020 2020 2020 3a72 6574 7572  y.        :retur
-00001ae0: 6e3a 2063 7573 746f 6d20 7072 6f70 6572  n: custom proper
-00001af0: 7479 206b 6579 2c20 7661 6c75 6520 7061  ty key, value pa
-00001b00: 6972 732e 0a20 2020 2020 2020 2027 2727  irs..        '''
-00001b10: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
-00001b20: 2020 2064 6566 206b 6579 6672 616d 655f     def keyframe_
-00001b30: 6465 6c65 7465 280a 2020 2020 2020 2020  delete(.        
-00001b40: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
-00001b50: 2020 2020 2020 6461 7461 5f70 6174 683a        data_path:
-00001b60: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
-00001b70: 5b73 7472 5d2c 0a20 2020 2020 2020 2020  [str],.         
-00001b80: 2020 2069 6e64 6578 3a20 7479 7069 6e67     index: typing
-00001b90: 2e4f 7074 696f 6e61 6c5b 696e 745d 203d  .Optional[int] =
-00001ba0: 202d 312c 0a20 2020 2020 2020 2020 2020   -1,.           
-00001bb0: 2066 7261 6d65 3a20 7479 7069 6e67 2e4f   frame: typing.O
-00001bc0: 7074 696f 6e61 6c5b 666c 6f61 745d 203d  ptional[float] =
-00001bd0: 2027 6270 792e 636f 6e74 6578 742e 7363   'bpy.context.sc
-00001be0: 656e 652e 6672 616d 655f 6375 7272 656e  ene.frame_curren
-00001bf0: 7427 2c0a 2020 2020 2020 2020 2020 2020  t',.            
-00001c00: 6772 6f75 703a 2074 7970 696e 672e 4f70  group: typing.Op
-00001c10: 7469 6f6e 616c 5b73 7472 5d20 3d20 2222  tional[str] = ""
-00001c20: 2920 2d3e 2062 6f6f 6c3a 0a20 2020 2020  ) -> bool:.     
-00001c30: 2020 2027 2727 2052 656d 6f76 6520 6120     ''' Remove a 
-00001c40: 6b65 7966 7261 6d65 2066 726f 6d20 7468  keyframe from th
-00001c50: 6973 2070 726f 7065 7274 6965 7320 6663  is properties fc
-00001c60: 7572 7665 2e0a 0a20 2020 2020 2020 203a  urve...        :
-00001c70: 7061 7261 6d20 6461 7461 5f70 6174 683a  param data_path:
-00001c80: 2070 6174 6820 746f 2074 6865 2070 726f   path to the pro
-00001c90: 7065 7274 7920 746f 2072 656d 6f76 6520  perty to remove 
-00001ca0: 6120 6b65 792c 2061 6e61 6c6f 676f 7573  a key, analogous
-00001cb0: 2074 6f20 7468 6520 6663 7572 7665 2773   to the fcurve's
-00001cc0: 2064 6174 6120 7061 7468 2e0a 2020 2020   data path..    
-00001cd0: 2020 2020 3a74 7970 6520 6461 7461 5f70      :type data_p
-00001ce0: 6174 683a 2074 7970 696e 672e 4f70 7469  ath: typing.Opti
-00001cf0: 6f6e 616c 5b73 7472 5d0a 2020 2020 2020  onal[str].      
-00001d00: 2020 3a70 6172 616d 2069 6e64 6578 3a20    :param index: 
-00001d10: 6172 7261 7920 696e 6465 7820 6f66 2074  array index of t
-00001d20: 6865 2070 726f 7065 7274 7920 746f 2072  he property to r
-00001d30: 656d 6f76 6520 6120 6b65 792e 2044 6566  emove a key. Def
-00001d40: 6175 6c74 7320 746f 202d 3120 7265 6d6f  aults to -1 remo
-00001d50: 7669 6e67 2061 6c6c 2069 6e64 6963 6573  ving all indices
-00001d60: 206f 7220 6120 7369 6e67 6c65 2063 6861   or a single cha
-00001d70: 6e6e 656c 2069 6620 7468 6520 7072 6f70  nnel if the prop
-00001d80: 6572 7479 2069 7320 6e6f 7420 616e 2061  erty is not an a
-00001d90: 7272 6179 2e0a 2020 2020 2020 2020 3a74  rray..        :t
-00001da0: 7970 6520 696e 6465 783a 2074 7970 696e  ype index: typin
-00001db0: 672e 4f70 7469 6f6e 616c 5b69 6e74 5d0a  g.Optional[int].
-00001dc0: 2020 2020 2020 2020 3a70 6172 616d 2066          :param f
-00001dd0: 7261 6d65 3a20 5468 6520 6672 616d 6520  rame: The frame 
-00001de0: 6f6e 2077 6869 6368 2074 6865 206b 6579  on which the key
-00001df0: 6672 616d 6520 6973 2064 656c 6574 6564  frame is deleted
-00001e00: 2c20 6465 6661 756c 7469 6e67 2074 6f20  , defaulting to 
-00001e10: 7468 6520 6375 7272 656e 7420 6672 616d  the current fram
-00001e20: 652e 0a20 2020 2020 2020 203a 7479 7065  e..        :type
-00001e30: 2066 7261 6d65 3a20 7479 7069 6e67 2e4f   frame: typing.O
-00001e40: 7074 696f 6e61 6c5b 666c 6f61 745d 0a20  ptional[float]. 
-00001e50: 2020 2020 2020 203a 7061 7261 6d20 6772         :param gr
-00001e60: 6f75 703a 2054 6865 206e 616d 6520 6f66  oup: The name of
-00001e70: 2074 6865 2067 726f 7570 2074 6865 2046   the group the F
-00001e80: 2d43 7572 7665 2073 686f 756c 6420 6265  -Curve should be
-00001e90: 2061 6464 6564 2074 6f20 6966 2069 7420   added to if it 
-00001ea0: 646f 6573 6e27 7420 6578 6973 7420 7965  doesn't exist ye
-00001eb0: 742e 0a20 2020 2020 2020 203a 7479 7065  t..        :type
-00001ec0: 2067 726f 7570 3a20 7479 7069 6e67 2e4f   group: typing.O
-00001ed0: 7074 696f 6e61 6c5b 7374 725d 0a20 2020  ptional[str].   
-00001ee0: 2020 2020 203a 7274 7970 653a 2062 6f6f       :rtype: boo
-00001ef0: 6c0a 2020 2020 2020 2020 3a72 6574 7572  l.        :retur
-00001f00: 6e3a 2053 7563 6365 7373 206f 6620 6b65  n: Success of ke
-00001f10: 7966 7261 6d65 2064 656c 6574 696f 6e2e  yframe deletion.
-00001f20: 0a20 2020 2020 2020 2027 2727 0a20 2020  .        '''.   
-00001f30: 2020 2020 2070 6173 730a 0a20 2020 2064       pass..    d
-00001f40: 6566 206b 6579 6672 616d 655f 696e 7365  ef keyframe_inse
-00001f50: 7274 280a 2020 2020 2020 2020 2020 2020  rt(.            
-00001f60: 7365 6c66 2c0a 2020 2020 2020 2020 2020  self,.          
-00001f70: 2020 6461 7461 5f70 6174 683a 2074 7970    data_path: typ
-00001f80: 696e 672e 4f70 7469 6f6e 616c 5b73 7472  ing.Optional[str
-00001f90: 5d2c 0a20 2020 2020 2020 2020 2020 2069  ],.            i
-00001fa0: 6e64 6578 3a20 7479 7069 6e67 2e4f 7074  ndex: typing.Opt
-00001fb0: 696f 6e61 6c5b 696e 745d 203d 202d 312c  ional[int] = -1,
-00001fc0: 0a20 2020 2020 2020 2020 2020 2066 7261  .            fra
-00001fd0: 6d65 3a20 7479 7069 6e67 2e4f 7074 696f  me: typing.Optio
-00001fe0: 6e61 6c5b 666c 6f61 745d 203d 2027 6270  nal[float] = 'bp
-00001ff0: 792e 636f 6e74 6578 742e 7363 656e 652e  y.context.scene.
-00002000: 6672 616d 655f 6375 7272 656e 7427 2c0a  frame_current',.
-00002010: 2020 2020 2020 2020 2020 2020 6772 6f75              grou
-00002020: 703a 2074 7970 696e 672e 4f70 7469 6f6e  p: typing.Option
-00002030: 616c 5b73 7472 5d20 3d20 2222 2c0a 2020  al[str] = "",.  
-00002040: 2020 2020 2020 2020 2020 6f70 7469 6f6e            option
-00002050: 733a 2074 7970 696e 672e 4f70 7469 6f6e  s: typing.Option
-00002060: 616c 5b74 7970 696e 672e 416e 795d 203d  al[typing.Any] =
-00002070: 2027 7365 7428 2927 2920 2d3e 2062 6f6f   'set()') -> boo
-00002080: 6c3a 0a20 2020 2020 2020 2027 2727 2049  l:.        ''' I
-00002090: 6e73 6572 7420 6120 6b65 7966 7261 6d65  nsert a keyframe
-000020a0: 206f 6e20 7468 6520 7072 6f70 6572 7479   on the property
-000020b0: 2067 6976 656e 2c20 6164 6469 6e67 2066   given, adding f
-000020c0: 6375 7276 6573 2061 6e64 2061 6e69 6d61  curves and anima
-000020d0: 7469 6f6e 2064 6174 6120 7768 656e 206e  tion data when n
-000020e0: 6563 6573 7361 7279 2e20 5468 6973 2069  ecessary. This i
-000020f0: 7320 7468 6520 6d6f 7374 2073 696d 706c  s the most simpl
-00002100: 6520 6578 616d 706c 6520 6f66 2069 6e73  e example of ins
-00002110: 6572 7469 6e67 2061 206b 6579 6672 616d  erting a keyfram
-00002120: 6520 6672 6f6d 2070 7974 686f 6e2e 204e  e from python. N
-00002130: 6f74 6520 7468 6174 2077 6865 6e20 6b65  ote that when ke
-00002140: 7969 6e67 2064 6174 6120 7061 7468 7320  ying data paths 
-00002150: 7768 6963 6820 636f 6e74 6169 6e20 6e65  which contain ne
-00002160: 7374 6564 2070 726f 7065 7274 6965 7320  sted properties 
-00002170: 7468 6973 206d 7573 7420 6265 2064 6f6e  this must be don
-00002180: 6520 6672 6f6d 2074 6865 2060 4944 6020  e from the `ID` 
-00002190: 7375 6263 6c61 7373 2c20 696e 2074 6869  subclass, in thi
-000021a0: 7320 6361 7365 2074 6865 2060 4172 6d61  s case the `Arma
-000021b0: 7475 7265 6020 7261 7468 6572 2074 6861  ture` rather tha
-000021c0: 6e20 7468 6520 626f 6e65 2e0a 0a20 2020  n the bone...   
-000021d0: 2020 2020 203a 7061 7261 6d20 6461 7461       :param data
-000021e0: 5f70 6174 683a 2070 6174 6820 746f 2074  _path: path to t
-000021f0: 6865 2070 726f 7065 7274 7920 746f 206b  he property to k
-00002200: 6579 2c20 616e 616c 6f67 6f75 7320 746f  ey, analogous to
-00002210: 2074 6865 2066 6375 7276 6527 7320 6461   the fcurve's da
-00002220: 7461 2070 6174 682e 0a20 2020 2020 2020  ta path..       
-00002230: 203a 7479 7065 2064 6174 615f 7061 7468   :type data_path
-00002240: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
-00002250: 6c5b 7374 725d 0a20 2020 2020 2020 203a  l[str].        :
-00002260: 7061 7261 6d20 696e 6465 783a 2061 7272  param index: arr
-00002270: 6179 2069 6e64 6578 206f 6620 7468 6520  ay index of the 
-00002280: 7072 6f70 6572 7479 2074 6f20 6b65 792e  property to key.
-00002290: 2044 6566 6175 6c74 7320 746f 202d 3120   Defaults to -1 
-000022a0: 7768 6963 6820 7769 6c6c 206b 6579 2061  which will key a
-000022b0: 6c6c 2069 6e64 6963 6573 206f 7220 6120  ll indices or a 
-000022c0: 7369 6e67 6c65 2063 6861 6e6e 656c 2069  single channel i
-000022d0: 6620 7468 6520 7072 6f70 6572 7479 2069  f the property i
-000022e0: 7320 6e6f 7420 616e 2061 7272 6179 2e0a  s not an array..
-000022f0: 2020 2020 2020 2020 3a74 7970 6520 696e          :type in
-00002300: 6465 783a 2074 7970 696e 672e 4f70 7469  dex: typing.Opti
-00002310: 6f6e 616c 5b69 6e74 5d0a 2020 2020 2020  onal[int].      
-00002320: 2020 3a70 6172 616d 2066 7261 6d65 3a20    :param frame: 
-00002330: 5468 6520 6672 616d 6520 6f6e 2077 6869  The frame on whi
-00002340: 6368 2074 6865 206b 6579 6672 616d 6520  ch the keyframe 
-00002350: 6973 2069 6e73 6572 7465 642c 2064 6566  is inserted, def
-00002360: 6175 6c74 696e 6720 746f 2074 6865 2063  aulting to the c
-00002370: 7572 7265 6e74 2066 7261 6d65 2e0a 2020  urrent frame..  
-00002380: 2020 2020 2020 3a74 7970 6520 6672 616d        :type fram
-00002390: 653a 2074 7970 696e 672e 4f70 7469 6f6e  e: typing.Option
-000023a0: 616c 5b66 6c6f 6174 5d0a 2020 2020 2020  al[float].      
-000023b0: 2020 3a70 6172 616d 2067 726f 7570 3a20    :param group: 
-000023c0: 5468 6520 6e61 6d65 206f 6620 7468 6520  The name of the 
-000023d0: 6772 6f75 7020 7468 6520 462d 4375 7276  group the F-Curv
-000023e0: 6520 7368 6f75 6c64 2062 6520 6164 6465  e should be adde
-000023f0: 6420 746f 2069 6620 6974 2064 6f65 736e  d to if it doesn
-00002400: 2774 2065 7869 7374 2079 6574 2e0a 2020  't exist yet..  
-00002410: 2020 2020 2020 3a74 7970 6520 6772 6f75        :type grou
-00002420: 703a 2074 7970 696e 672e 4f70 7469 6f6e  p: typing.Option
-00002430: 616c 5b73 7472 5d0a 2020 2020 2020 2020  al[str].        
-00002440: 3a70 6172 616d 2066 6c61 673a 200a 2020  :param flag: .  
-00002450: 2020 2020 2020 3a74 7970 6520 666c 6167        :type flag
-00002460: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
-00002470: 6c5b 7479 7069 6e67 2e53 6574 5d0a 2020  l[typing.Set].  
-00002480: 2020 2020 2020 3a70 6172 616d 206f 7074        :param opt
-00002490: 696f 6e73 3a20 202d 2060 6049 4e53 4552  ions:  - ``INSER
-000024a0: 544b 4559 5f4e 4545 4445 4460 6020 4f6e  TKEY_NEEDED`` On
-000024b0: 6c79 2069 6e73 6572 7420 6b65 7966 7261  ly insert keyfra
-000024c0: 6d65 7320 7768 6572 6520 7468 6579 2772  mes where they'r
-000024d0: 6520 6e65 6564 6564 2069 6e20 7468 6520  e needed in the 
-000024e0: 7265 6c65 7661 6e74 2046 2d43 7572 7665  relevant F-Curve
-000024f0: 732e 202d 2060 6049 4e53 4552 544b 4559  s. - ``INSERTKEY
-00002500: 5f56 4953 5541 4c60 6020 496e 7365 7274  _VISUAL`` Insert
-00002510: 206b 6579 6672 616d 6573 2062 6173 6564   keyframes based
-00002520: 206f 6e20 2776 6973 7561 6c20 7472 616e   on 'visual tran
-00002530: 7366 6f72 6d73 272e 202d 2060 6049 4e53  sforms'. - ``INS
-00002540: 4552 544b 4559 5f58 595a 5f54 4f5f 5247  ERTKEY_XYZ_TO_RG
-00002550: 4260 6020 436f 6c6f 7220 666f 7220 6e65  B`` Color for ne
-00002560: 776c 7920 6164 6465 6420 7472 616e 7366  wly added transf
-00002570: 6f72 6d61 7469 6f6e 2046 2d43 7572 7665  ormation F-Curve
-00002580: 7320 284c 6f63 6174 696f 6e2c 2052 6f74  s (Location, Rot
-00002590: 6174 696f 6e2c 2053 6361 6c65 2920 6973  ation, Scale) is
-000025a0: 2062 6173 6564 206f 6e20 7468 6520 7472   based on the tr
-000025b0: 616e 7366 6f72 6d20 6178 6973 2e20 2d20  ansform axis. - 
-000025c0: 6060 494e 5345 5254 4b45 595f 5245 504c  ``INSERTKEY_REPL
-000025d0: 4143 4560 6020 4f6e 6c79 2072 6570 6c61  ACE`` Only repla
-000025e0: 6365 2061 6c72 6561 6479 2065 7869 7374  ce already exist
-000025f0: 696e 6720 6b65 7966 7261 6d65 732e 202d  ing keyframes. -
-00002600: 2060 6049 4e53 4552 544b 4559 5f41 5641   ``INSERTKEY_AVA
-00002610: 494c 4142 4c45 6060 204f 6e6c 7920 696e  ILABLE`` Only in
-00002620: 7365 7274 2069 6e74 6f20 616c 7265 6164  sert into alread
-00002630: 7920 6578 6973 7469 6e67 2046 2d43 7572  y existing F-Cur
-00002640: 7665 732e 202d 2060 6049 4e53 4552 544b  ves. - ``INSERTK
-00002650: 4559 5f43 5943 4c45 5f41 5741 5245 6060  EY_CYCLE_AWARE``
-00002660: 2054 616b 6520 6379 636c 6963 2065 7874   Take cyclic ext
-00002670: 7261 706f 6c61 7469 6f6e 2069 6e74 6f20  rapolation into 
-00002680: 6163 636f 756e 7420 2843 7963 6c65 2d41  account (Cycle-A
-00002690: 7761 7265 204b 6579 696e 6720 6f70 7469  ware Keying opti
-000026a0: 6f6e 292e 0a20 2020 2020 2020 203a 7479  on)..        :ty
-000026b0: 7065 206f 7074 696f 6e73 3a20 7479 7069  pe options: typi
-000026c0: 6e67 2e4f 7074 696f 6e61 6c5b 7479 7069  ng.Optional[typi
-000026d0: 6e67 2e41 6e79 5d0a 2020 2020 2020 2020  ng.Any].        
-000026e0: 3a72 7479 7065 3a20 626f 6f6c 0a20 2020  :rtype: bool.   
-000026f0: 2020 2020 203a 7265 7475 726e 3a20 5375       :return: Su
-00002700: 6363 6573 7320 6f66 206b 6579 6672 616d  ccess of keyfram
-00002710: 6520 696e 7365 7274 696f 6e2e 0a20 2020  e insertion..   
-00002720: 2020 2020 2027 2727 0a20 2020 2020 2020       '''.       
-00002730: 2070 6173 730a 0a20 2020 2064 6566 206b   pass..    def k
-00002740: 6579 7328 7365 6c66 2920 2d3e 2074 7970  eys(self) -> typ
-00002750: 696e 672e 416e 793a 0a20 2020 2020 2020  ing.Any:.       
-00002760: 2027 2727 2052 6574 7572 6e73 2074 6865   ''' Returns the
-00002770: 206b 6579 7320 6f66 2074 6869 7320 6f62   keys of this ob
-00002780: 6a65 6374 7320 6375 7374 6f6d 2070 726f  jects custom pro
-00002790: 7065 7274 6965 7320 286d 6174 6368 6573  perties (matches
-000027a0: 2050 7974 686f 6e27 7320 6469 6374 696f   Python's dictio
-000027b0: 6e61 7279 2066 756e 6374 696f 6e20 6f66  nary function of
-000027c0: 2074 6865 2073 616d 6520 6e61 6d65 292e   the same name).
-000027d0: 0a0a 2020 2020 2020 2020 3a72 7479 7065  ..        :rtype
-000027e0: 3a20 7479 7069 6e67 2e41 6e79 0a20 2020  : typing.Any.   
-000027f0: 2020 2020 203a 7265 7475 726e 3a20 6375       :return: cu
-00002800: 7374 6f6d 2070 726f 7065 7274 7920 6b65  stom property ke
-00002810: 7973 2e0a 2020 2020 2020 2020 2727 270a  ys..        '''.
-00002820: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
-00002830: 2020 6465 6620 7061 7468 5f66 726f 6d5f    def path_from_
-00002840: 6964 2873 656c 662c 2070 726f 7065 7274  id(self, propert
-00002850: 793a 2074 7970 696e 672e 4f70 7469 6f6e  y: typing.Option
-00002860: 616c 5b73 7472 5d20 3d20 2222 2920 2d3e  al[str] = "") ->
-00002870: 2073 7472 3a0a 2020 2020 2020 2020 2727   str:.        ''
-00002880: 2720 5265 7475 726e 7320 7468 6520 6461  ' Returns the da
-00002890: 7461 2070 6174 6820 6672 6f6d 2074 6865  ta path from the
-000028a0: 2049 4420 746f 2074 6869 7320 6f62 6a65   ID to this obje
-000028b0: 6374 2028 7374 7269 6e67 292e 0a0a 2020  ct (string)...  
-000028c0: 2020 2020 2020 3a70 6172 616d 2070 726f        :param pro
-000028d0: 7065 7274 793a 204f 7074 696f 6e61 6c20  perty: Optional 
-000028e0: 7072 6f70 6572 7479 206e 616d 6520 7768  property name wh
-000028f0: 6963 6820 6361 6e20 6265 2075 7365 6420  ich can be used 
-00002900: 6966 2074 6865 2070 6174 6820 6973 2074  if the path is t
-00002910: 6f20 6120 7072 6f70 6572 7479 206f 6620  o a property of 
-00002920: 7468 6973 206f 626a 6563 742e 0a20 2020  this object..   
-00002930: 2020 2020 203a 7479 7065 2070 726f 7065       :type prope
-00002940: 7274 793a 2074 7970 696e 672e 4f70 7469  rty: typing.Opti
-00002950: 6f6e 616c 5b73 7472 5d0a 2020 2020 2020  onal[str].      
-00002960: 2020 3a72 7479 7065 3a20 7374 720a 2020    :rtype: str.  
-00002970: 2020 2020 2020 3a72 6574 7572 6e3a 2060        :return: `
-00002980: 6270 792e 7479 7065 732e 6270 795f 7374  bpy.types.bpy_st
-00002990: 7275 6374 2e69 645f 6461 7461 6020 746f  ruct.id_data` to
-000029a0: 2074 6869 7320 7374 7275 6374 2061 6e64   this struct and
-000029b0: 2070 726f 7065 7274 7920 2877 6865 6e20   property (when 
-000029c0: 6769 7665 6e29 2e0a 2020 2020 2020 2020  given)..        
-000029d0: 2727 270a 2020 2020 2020 2020 7061 7373  '''.        pass
-000029e0: 0a0a 2020 2020 6465 6620 7061 7468 5f72  ..    def path_r
-000029f0: 6573 6f6c 7665 2873 656c 662c 0a20 2020  esolve(self,.   
-00002a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a10: 2020 7061 7468 3a20 7479 7069 6e67 2e4f    path: typing.O
-00002a20: 7074 696f 6e61 6c5b 7374 725d 2c0a 2020  ptional[str],.  
-00002a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a40: 2020 2063 6f65 7263 653a 2074 7970 696e     coerce: typin
-00002a50: 672e 4f70 7469 6f6e 616c 5b62 6f6f 6c5d  g.Optional[bool]
-00002a60: 203d 2054 7275 6529 3a0a 2020 2020 2020   = True):.      
-00002a70: 2020 2727 2720 5265 7475 726e 7320 7468    ''' Returns th
-00002a80: 6520 7072 6f70 6572 7479 2066 726f 6d20  e property from 
-00002a90: 7468 6520 7061 7468 2c20 7261 6973 6520  the path, raise 
-00002aa0: 616e 2065 7863 6570 7469 6f6e 2077 6865  an exception whe
-00002ab0: 6e20 6e6f 7420 666f 756e 642e 0a0a 2020  n not found...  
-00002ac0: 2020 2020 2020 3a70 6172 616d 2070 6174        :param pat
-00002ad0: 683a 2070 6174 6820 7768 6963 6820 7468  h: path which th
-00002ae0: 6973 2070 726f 7065 7274 7920 7265 736f  is property reso
-00002af0: 6c76 6573 2e0a 2020 2020 2020 2020 3a74  lves..        :t
-00002b00: 7970 6520 7061 7468 3a20 7479 7069 6e67  ype path: typing
-00002b10: 2e4f 7074 696f 6e61 6c5b 7374 725d 0a20  .Optional[str]. 
-00002b20: 2020 2020 2020 203a 7061 7261 6d20 636f         :param co
-00002b30: 6572 6365 3a20 6f70 7469 6f6e 616c 2061  erce: optional a
-00002b40: 7267 756d 656e 742c 2077 6865 6e20 5472  rgument, when Tr
-00002b50: 7565 2c20 7468 6520 7072 6f70 6572 7479  ue, the property
-00002b60: 2077 696c 6c20 6265 2063 6f6e 7665 7274   will be convert
-00002b70: 6564 2069 6e74 6f20 6974 7320 5079 7468  ed into its Pyth
-00002b80: 6f6e 2072 6570 7265 7365 6e74 6174 696f  on representatio
-00002b90: 6e2e 0a20 2020 2020 2020 203a 7479 7065  n..        :type
-00002ba0: 2063 6f65 7263 653a 2074 7970 696e 672e   coerce: typing.
-00002bb0: 4f70 7469 6f6e 616c 5b62 6f6f 6c5d 0a20  Optional[bool]. 
-00002bc0: 2020 2020 2020 2027 2727 0a20 2020 2020         '''.     
-00002bd0: 2020 2070 6173 730a 0a20 2020 2064 6566     pass..    def
-00002be0: 2070 6f70 2873 656c 662c 0a20 2020 2020   pop(self,.     
-00002bf0: 2020 2020 2020 206b 6579 3a20 7479 7069         key: typi
-00002c00: 6e67 2e4f 7074 696f 6e61 6c5b 7374 725d  ng.Optional[str]
-00002c10: 2c0a 2020 2020 2020 2020 2020 2020 6465  ,.            de
-00002c20: 6661 756c 743a 2074 7970 696e 672e 4f70  fault: typing.Op
-00002c30: 7469 6f6e 616c 5b74 7970 696e 672e 416e  tional[typing.An
-00002c40: 795d 203d 204e 6f6e 6529 3a0a 2020 2020  y] = None):.    
-00002c50: 2020 2020 2727 2720 5265 6d6f 7665 2061      ''' Remove a
-00002c60: 6e64 2072 6574 7572 6e20 7468 6520 7661  nd return the va
-00002c70: 6c75 6520 6f66 2074 6865 2063 7573 746f  lue of the custo
-00002c80: 6d20 7072 6f70 6572 7479 2061 7373 6967  m property assig
-00002c90: 6e65 6420 746f 206b 6579 206f 7220 6465  ned to key or de
-00002ca0: 6661 756c 7420 7768 656e 206e 6f74 2066  fault when not f
-00002cb0: 6f75 6e64 2028 6d61 7463 6865 7320 5079  ound (matches Py
-00002cc0: 7468 6f6e 2773 2064 6963 7469 6f6e 6172  thon's dictionar
-00002cd0: 7920 6675 6e63 7469 6f6e 206f 6620 7468  y function of th
-00002ce0: 6520 7361 6d65 206e 616d 6529 2e0a 0a20  e same name)... 
-00002cf0: 2020 2020 2020 203a 7061 7261 6d20 6b65         :param ke
-00002d00: 793a 2054 6865 206b 6579 2061 7373 6f63  y: The key assoc
-00002d10: 6961 7465 6420 7769 7468 2074 6865 2063  iated with the c
-00002d20: 7573 746f 6d20 7072 6f70 6572 7479 2e0a  ustom property..
-00002d30: 2020 2020 2020 2020 3a74 7970 6520 6b65          :type ke
-00002d40: 793a 2074 7970 696e 672e 4f70 7469 6f6e  y: typing.Option
-00002d50: 616c 5b73 7472 5d0a 2020 2020 2020 2020  al[str].        
-00002d60: 3a70 6172 616d 2064 6566 6175 6c74 3a20  :param default: 
-00002d70: 4f70 7469 6f6e 616c 2061 7267 756d 656e  Optional argumen
-00002d80: 7420 666f 7220 7468 6520 7661 6c75 6520  t for the value 
-00002d90: 746f 2072 6574 7572 6e20 6966 202a 6b65  to return if *ke
-00002da0: 792a 2069 7320 6e6f 7420 666f 756e 642e  y* is not found.
-00002db0: 0a20 2020 2020 2020 203a 7479 7065 2064  .        :type d
-00002dc0: 6566 6175 6c74 3a20 7479 7069 6e67 2e4f  efault: typing.O
-00002dd0: 7074 696f 6e61 6c5b 7479 7069 6e67 2e41  ptional[typing.A
-00002de0: 6e79 5d0a 2020 2020 2020 2020 2727 270a  ny].        '''.
-00002df0: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
-00002e00: 2020 6465 6620 7072 6f70 6572 7479 5f6f    def property_o
-00002e10: 7665 7272 6964 6162 6c65 5f6c 6962 7261  verridable_libra
-00002e20: 7279 5f73 6574 2873 656c 662c 2070 726f  ry_set(self, pro
-00002e30: 7065 7274 792c 206f 7665 7272 6964 6162  perty, overridab
-00002e40: 6c65 2920 2d3e 2062 6f6f 6c3a 0a20 2020  le) -> bool:.   
-00002e50: 2020 2020 2027 2727 2044 6566 696e 6520       ''' Define 
-00002e60: 6120 7072 6f70 6572 7479 2061 7320 6f76  a property as ov
-00002e70: 6572 7269 6461 626c 6520 6f72 206e 6f74  erridable or not
-00002e80: 2028 6f6e 6c79 2066 6f72 2063 7573 746f   (only for custo
-00002e90: 6d20 7072 6f70 6572 7469 6573 2129 2e0a  m properties!)..
-00002ea0: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
-00002eb0: 2062 6f6f 6c0a 2020 2020 2020 2020 3a72   bool.        :r
-00002ec0: 6574 7572 6e3a 2054 7275 6520 7768 656e  eturn: True when
-00002ed0: 2074 6865 206f 7665 7272 6964 6162 6c65   the overridable
-00002ee0: 2073 7461 7475 7320 6f66 2074 6865 2070   status of the p
-00002ef0: 726f 7065 7274 7920 7761 7320 7375 6363  roperty was succ
-00002f00: 6573 7366 756c 6c79 2073 6574 2e0a 2020  essfully set..  
-00002f10: 2020 2020 2020 2727 270a 2020 2020 2020        '''.      
-00002f20: 2020 7061 7373 0a0a 2020 2020 6465 6620    pass..    def 
-00002f30: 7072 6f70 6572 7479 5f75 6e73 6574 2873  property_unset(s
-00002f40: 656c 662c 2070 726f 7065 7274 7929 3a0a  elf, property):.
-00002f50: 2020 2020 2020 2020 2727 2720 556e 7365          ''' Unse
-00002f60: 7420 6120 7072 6f70 6572 7479 2c20 7769  t a property, wi
-00002f70: 6c6c 2075 7365 2064 6566 6175 6c74 2076  ll use default v
-00002f80: 616c 7565 2061 6674 6572 7761 7264 2e0a  alue afterward..
-00002f90: 0a20 2020 2020 2020 2027 2727 0a20 2020  .        '''.   
-00002fa0: 2020 2020 2070 6173 730a 0a20 2020 2064       pass..    d
-00002fb0: 6566 2074 7970 655f 7265 6361 7374 2873  ef type_recast(s
-00002fc0: 656c 6629 202d 3e20 2762 7079 5f73 7472  elf) -> 'bpy_str
-00002fd0: 7563 7427 3a0a 2020 2020 2020 2020 2727  uct':.        ''
-00002fe0: 2720 5265 7475 726e 2061 206e 6577 2069  ' Return a new i
-00002ff0: 6e73 7461 6e63 652c 2074 6869 7320 6973  nstance, this is
-00003000: 206e 6565 6465 6420 6265 6361 7573 6520   needed because 
-00003010: 7479 7065 7320 7375 6368 2061 7320 7465  types such as te
-00003020: 7874 7572 6573 2063 616e 2062 6520 6368  xtures can be ch
-00003030: 616e 6765 6420 6174 2072 756e 7469 6d65  anged at runtime
-00003040: 2e0a 0a20 2020 2020 2020 203a 7274 7970  ...        :rtyp
-00003050: 653a 2027 6270 795f 7374 7275 6374 270a  e: 'bpy_struct'.
-00003060: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
-00003070: 2061 206e 6577 2069 6e73 7461 6e63 6520   a new instance 
-00003080: 6f66 2074 6869 7320 6f62 6a65 6374 2077  of this object w
-00003090: 6974 6820 7468 6520 7479 7065 2069 6e69  ith the type ini
-000030a0: 7469 616c 697a 6564 2061 6761 696e 2e0a  tialized again..
-000030b0: 2020 2020 2020 2020 2727 270a 2020 2020          '''.    
-000030c0: 2020 2020 7061 7373 0a0a 2020 2020 6465      pass..    de
-000030d0: 6620 7661 6c75 6573 2873 656c 6629 202d  f values(self) -
-000030e0: 3e20 7479 7069 6e67 2e41 6e79 3a0a 2020  > typing.Any:.  
-000030f0: 2020 2020 2020 2727 2720 5265 7475 726e        ''' Return
-00003100: 7320 7468 6520 7661 6c75 6573 206f 6620  s the values of 
-00003110: 7468 6973 206f 626a 6563 7473 2063 7573  this objects cus
-00003120: 746f 6d20 7072 6f70 6572 7469 6573 2028  tom properties (
-00003130: 6d61 7463 6865 7320 5079 7468 6f6e 2773  matches Python's
-00003140: 2064 6963 7469 6f6e 6172 7920 6675 6e63   dictionary func
-00003150: 7469 6f6e 206f 6620 7468 6520 7361 6d65  tion of the same
-00003160: 206e 616d 6529 2e0a 0a20 2020 2020 2020   name)...       
-00003170: 203a 7274 7970 653a 2074 7970 696e 672e   :rtype: typing.
-00003180: 416e 790a 2020 2020 2020 2020 3a72 6574  Any.        :ret
-00003190: 7572 6e3a 2063 7573 746f 6d20 7072 6f70  urn: custom prop
-000031a0: 6572 7479 2076 616c 7565 732e 0a20 2020  erty values..   
-000031b0: 2020 2020 2027 2727 0a20 2020 2020 2020       '''.       
-000031c0: 2070 6173 730a 0a20 2020 2064 6566 205f   pass..    def _
-000031d0: 5f67 6574 6974 656d 5f5f 2873 656c 662c  _getitem__(self,
-000031e0: 206b 6579 3a20 7479 7069 6e67 2e55 6e69   key: typing.Uni
-000031f0: 6f6e 5b69 6e74 2c20 7374 725d 2920 2d3e  on[int, str]) ->
-00003200: 2027 7479 7069 6e67 2e41 6e79 273a 0a20   'typing.Any':. 
-00003210: 2020 2020 2020 2027 2727 200a 0a20 2020         ''' ..   
-00003220: 2020 2020 203a 7061 7261 6d20 6b65 793a       :param key:
-00003230: 200a 2020 2020 2020 2020 3a74 7970 6520   .        :type 
-00003240: 6b65 793a 2074 7970 696e 672e 556e 696f  key: typing.Unio
-00003250: 6e5b 696e 742c 2073 7472 5d0a 2020 2020  n[int, str].    
-00003260: 2020 2020 3a72 7479 7065 3a20 2774 7970      :rtype: 'typ
-00003270: 696e 672e 416e 7927 0a20 2020 2020 2020  ing.Any'.       
-00003280: 2027 2727 0a20 2020 2020 2020 2070 6173   '''.        pas
-00003290: 730a 0a20 2020 2064 6566 205f 5f73 6574  s..    def __set
-000032a0: 6974 656d 5f5f 2873 656c 662c 206b 6579  item__(self, key
-000032b0: 3a20 7479 7069 6e67 2e55 6e69 6f6e 5b69  : typing.Union[i
-000032c0: 6e74 2c20 7374 725d 2c20 7661 6c75 653a  nt, str], value:
-000032d0: 2027 7479 7069 6e67 2e41 6e79 2729 3a0a   'typing.Any'):.
-000032e0: 2020 2020 2020 2020 2727 2720 0a0a 2020          ''' ..  
-000032f0: 2020 2020 2020 3a70 6172 616d 206b 6579        :param key
-00003300: 3a20 0a20 2020 2020 2020 203a 7479 7065  : .        :type
-00003310: 206b 6579 3a20 7479 7069 6e67 2e55 6e69   key: typing.Uni
-00003320: 6f6e 5b69 6e74 2c20 7374 725d 0a20 2020  on[int, str].   
-00003330: 2020 2020 203a 7061 7261 6d20 7661 6c75       :param valu
-00003340: 653a 200a 2020 2020 2020 2020 3a74 7970  e: .        :typ
-00003350: 6520 7661 6c75 653a 2027 7479 7069 6e67  e value: 'typing
-00003360: 2e41 6e79 270a 2020 2020 2020 2020 2727  .Any'.        ''
-00003370: 270a 2020 2020 2020 2020 7061 7373 0a0a  '.        pass..
-00003380: 2020 2020 6465 6620 5f5f 6465 6c69 7465      def __delite
-00003390: 6d5f 5f28 7365 6c66 2c20 6b65 793a 2074  m__(self, key: t
-000033a0: 7970 696e 672e 556e 696f 6e5b 696e 742c  yping.Union[int,
-000033b0: 2073 7472 5d29 202d 3e20 2774 7970 696e   str]) -> 'typin
-000033c0: 672e 416e 7927 3a0a 2020 2020 2020 2020  g.Any':.        
-000033d0: 2727 2720 0a0a 2020 2020 2020 2020 3a70  ''' ..        :p
-000033e0: 6172 616d 206b 6579 3a20 0a20 2020 2020  aram key: .     
-000033f0: 2020 203a 7479 7065 206b 6579 3a20 7479     :type key: ty
-00003400: 7069 6e67 2e55 6e69 6f6e 5b69 6e74 2c20  ping.Union[int, 
-00003410: 7374 725d 0a20 2020 2020 2020 203a 7274  str].        :rt
-00003420: 7970 653a 2027 7479 7069 6e67 2e41 6e79  ype: 'typing.Any
-00003430: 270a 2020 2020 2020 2020 2727 270a 2020  '.        '''.  
-00003440: 2020 2020 2020 7061 7373 0a0a 0a63 6c61        pass...cla
-00003450: 7373 2062 7079 5f70 726f 705f 636f 6c6c  ss bpy_prop_coll
-00003460: 6563 7469 6f6e 2874 7970 696e 672e 4765  ection(typing.Ge
-00003470: 6e65 7269 635b 4765 6e65 7269 6354 7970  neric[GenericTyp
-00003480: 655d 293a 0a20 2020 2027 2727 2062 7569  e]):.    ''' bui
-00003490: 6c74 2d69 6e20 636c 6173 7320 7573 6564  lt-in class used
-000034a0: 2066 6f72 2061 6c6c 2063 6f6c 6c65 6374   for all collect
-000034b0: 696f 6e73 2e0a 2020 2020 2727 270a 0a20  ions..    '''.. 
-000034c0: 2020 2064 6566 2066 696e 6428 7365 6c66     def find(self
-000034d0: 2c20 6b65 793a 2074 7970 696e 672e 4f70  , key: typing.Op
-000034e0: 7469 6f6e 616c 5b73 7472 5d29 202d 3e20  tional[str]) -> 
-000034f0: 696e 743a 0a20 2020 2020 2020 2027 2727  int:.        '''
-00003500: 2052 6574 7572 6e73 2074 6865 2069 6e64   Returns the ind
-00003510: 6578 206f 6620 6120 6b65 7920 696e 2061  ex of a key in a
-00003520: 2063 6f6c 6c65 6374 696f 6e20 6f72 202d   collection or -
-00003530: 3120 7768 656e 206e 6f74 2066 6f75 6e64  1 when not found
-00003540: 2028 6d61 7463 6865 7320 5079 7468 6f6e   (matches Python
-00003550: 2773 2073 7472 696e 6720 6669 6e64 2066  's string find f
-00003560: 756e 6374 696f 6e20 6f66 2074 6865 2073  unction of the s
-00003570: 616d 6520 6e61 6d65 292e 0a0a 2020 2020  ame name)...    
-00003580: 2020 2020 3a70 6172 616d 206b 6579 3a20      :param key: 
-00003590: 5468 6520 6964 656e 7469 6669 6572 2066  The identifier f
-000035a0: 6f72 2074 6865 2063 6f6c 6c65 6374 696f  or the collectio
-000035b0: 6e20 6d65 6d62 6572 2e0a 2020 2020 2020  n member..      
-000035c0: 2020 3a74 7970 6520 6b65 793a 2074 7970    :type key: typ
-000035d0: 696e 672e 4f70 7469 6f6e 616c 5b73 7472  ing.Optional[str
-000035e0: 5d0a 2020 2020 2020 2020 3a72 7479 7065  ].        :rtype
-000035f0: 3a20 696e 740a 2020 2020 2020 2020 3a72  : int.        :r
-00003600: 6574 7572 6e3a 2069 6e64 6578 206f 6620  eturn: index of 
-00003610: 7468 6520 6b65 792e 0a20 2020 2020 2020  the key..       
-00003620: 2027 2727 0a20 2020 2020 2020 2070 6173   '''.        pas
-00003630: 730a 0a20 2020 2064 6566 2066 6f72 6561  s..    def forea
-00003640: 6368 5f67 6574 2873 656c 662c 2061 7474  ch_get(self, att
-00003650: 722c 2073 6571 293a 0a20 2020 2020 2020  r, seq):.       
-00003660: 2027 2727 2054 6869 7320 6973 2061 2066   ''' This is a f
-00003670: 756e 6374 696f 6e20 746f 2067 6976 6520  unction to give 
-00003680: 6661 7374 2061 6363 6573 7320 746f 2061  fast access to a
-00003690: 7474 7269 6275 7465 7320 7769 7468 696e  ttributes within
-000036a0: 2061 2063 6f6c 6c65 6374 696f 6e2e 204f   a collection. O
-000036b0: 6e6c 7920 776f 726b 7320 666f 7220 2762  nly works for 'b
-000036c0: 6173 6963 2074 7970 6527 2070 726f 7065  asic type' prope
-000036d0: 7274 6965 7320 2862 6f6f 6c2c 2069 6e74  rties (bool, int
-000036e0: 2061 6e64 2066 6c6f 6174 2921 204d 756c   and float)! Mul
-000036f0: 7469 2d64 696d 656e 7369 6f6e 616c 2061  ti-dimensional a
-00003700: 7272 6179 7320 286c 696b 6520 6172 7261  rrays (like arra
-00003710: 7920 6f66 2076 6563 746f 7273 2920 7769  y of vectors) wi
-00003720: 6c6c 2062 6520 666c 6174 7465 6e65 6420  ll be flattened 
-00003730: 696e 746f 2073 6571 2e0a 0a20 2020 2020  into seq...     
-00003740: 2020 2027 2727 0a20 2020 2020 2020 2070     '''.        p
-00003750: 6173 730a 0a20 2020 2064 6566 2066 6f72  ass..    def for
-00003760: 6561 6368 5f73 6574 2873 656c 662c 2061  each_set(self, a
-00003770: 7474 722c 2073 6571 293a 0a20 2020 2020  ttr, seq):.     
-00003780: 2020 2027 2727 2054 6869 7320 6973 2061     ''' This is a
-00003790: 2066 756e 6374 696f 6e20 746f 2067 6976   function to giv
-000037a0: 6520 6661 7374 2061 6363 6573 7320 746f  e fast access to
-000037b0: 2061 7474 7269 6275 7465 7320 7769 7468   attributes with
-000037c0: 696e 2061 2063 6f6c 6c65 6374 696f 6e2e  in a collection.
-000037d0: 204f 6e6c 7920 776f 726b 7320 666f 7220   Only works for 
-000037e0: 2762 6173 6963 2074 7970 6527 2070 726f  'basic type' pro
-000037f0: 7065 7274 6965 7320 2862 6f6f 6c2c 2069  perties (bool, i
-00003800: 6e74 2061 6e64 2066 6c6f 6174 2921 2073  nt and float)! s
-00003810: 6571 206d 7573 7420 6265 2075 6e69 2d64  eq must be uni-d
-00003820: 696d 656e 7369 6f6e 616c 2c20 6d75 6c74  imensional, mult
-00003830: 692d 6469 6d65 6e73 696f 6e61 6c20 6172  i-dimensional ar
-00003840: 7261 7973 2028 6c69 6b65 2061 7272 6179  rays (like array
-00003850: 206f 6620 7665 6374 6f72 7329 2077 696c   of vectors) wil
-00003860: 6c20 6265 2072 652d 6372 6561 7465 6420  l be re-created 
-00003870: 6672 6f6d 2069 742e 0a0a 2020 2020 2020  from it...      
-00003880: 2020 2727 270a 2020 2020 2020 2020 7061    '''.        pa
-00003890: 7373 0a0a 2020 2020 6465 6620 6765 7428  ss..    def get(
-000038a0: 7365 6c66 2c0a 2020 2020 2020 2020 2020  self,.          
-000038b0: 2020 6b65 793a 2074 7970 696e 672e 4f70    key: typing.Op
-000038c0: 7469 6f6e 616c 5b73 7472 5d2c 0a20 2020  tional[str],.   
-000038d0: 2020 2020 2020 2020 2064 6566 6175 6c74           default
-000038e0: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
-000038f0: 6c5b 7479 7069 6e67 2e41 6e79 5d20 3d20  l[typing.Any] = 
-00003900: 4e6f 6e65 293a 0a20 2020 2020 2020 2027  None):.        '
-00003910: 2727 2052 6574 7572 6e73 2074 6865 2076  '' Returns the v
-00003920: 616c 7565 206f 6620 7468 6520 6974 656d  alue of the item
-00003930: 2061 7373 6967 6e65 6420 746f 206b 6579   assigned to key
-00003940: 206f 7220 6465 6661 756c 7420 7768 656e   or default when
-00003950: 206e 6f74 2066 6f75 6e64 2028 6d61 7463   not found (matc
-00003960: 6865 7320 5079 7468 6f6e 2773 2064 6963  hes Python's dic
-00003970: 7469 6f6e 6172 7920 6675 6e63 7469 6f6e  tionary function
-00003980: 206f 6620 7468 6520 7361 6d65 206e 616d   of the same nam
-00003990: 6529 2e0a 0a20 2020 2020 2020 203a 7061  e)...        :pa
-000039a0: 7261 6d20 6b65 793a 2054 6865 2069 6465  ram key: The ide
-000039b0: 6e74 6966 6965 7220 666f 7220 7468 6520  ntifier for the 
-000039c0: 636f 6c6c 6563 7469 6f6e 206d 656d 6265  collection membe
-000039d0: 722e 0a20 2020 2020 2020 203a 7479 7065  r..        :type
-000039e0: 206b 6579 3a20 7479 7069 6e67 2e4f 7074   key: typing.Opt
-000039f0: 696f 6e61 6c5b 7374 725d 0a20 2020 2020  ional[str].     
-00003a00: 2020 203a 7061 7261 6d20 6465 6661 756c     :param defaul
-00003a10: 743a 204f 7074 696f 6e61 6c20 6172 6775  t: Optional argu
-00003a20: 6d65 6e74 2066 6f72 2074 6865 2076 616c  ment for the val
-00003a30: 7565 2074 6f20 7265 7475 726e 2069 6620  ue to return if 
-00003a40: 2a6b 6579 2a20 6973 206e 6f74 2066 6f75  *key* is not fou
-00003a50: 6e64 2e0a 2020 2020 2020 2020 3a74 7970  nd..        :typ
-00003a60: 6520 6465 6661 756c 743a 2074 7970 696e  e default: typin
-00003a70: 672e 4f70 7469 6f6e 616c 5b74 7970 696e  g.Optional[typin
-00003a80: 672e 416e 795d 0a20 2020 2020 2020 2027  g.Any].        '
-00003a90: 2727 0a20 2020 2020 2020 2070 6173 730a  ''.        pass.
-00003aa0: 0a20 2020 2064 6566 2069 7465 6d73 2873  .    def items(s
-00003ab0: 656c 6629 202d 3e20 7479 7069 6e67 2e4c  elf) -> typing.L
-00003ac0: 6973 743a 0a20 2020 2020 2020 2027 2727  ist:.        '''
-00003ad0: 2052 6574 7572 6e20 7468 6520 6964 656e   Return the iden
-00003ae0: 7469 6669 6572 7320 6f66 2063 6f6c 6c65  tifiers of colle
-00003af0: 6374 696f 6e20 6d65 6d62 6572 7320 286d  ction members (m
-00003b00: 6174 6368 696e 6720 5079 7468 6f6e 2773  atching Python's
-00003b10: 2064 6963 742e 6974 656d 7328 2920 6675   dict.items() fu
-00003b20: 6e63 7469 6f6e 616c 6974 7929 2e0a 0a20  nctionality)... 
-00003b30: 2020 2020 2020 203a 7274 7970 653a 2074         :rtype: t
-00003b40: 7970 696e 672e 4c69 7374 0a20 2020 2020  yping.List.     
-00003b50: 2020 203a 7265 7475 726e 3a20 286b 6579     :return: (key
-00003b60: 2c20 7661 6c75 6529 2070 6169 7273 2066  , value) pairs f
-00003b70: 6f72 2065 6163 6820 6d65 6d62 6572 206f  or each member o
-00003b80: 6620 7468 6973 2063 6f6c 6c65 6374 696f  f this collectio
-00003b90: 6e2e 0a20 2020 2020 2020 2027 2727 0a20  n..        '''. 
-00003ba0: 2020 2020 2020 2070 6173 730a 0a20 2020         pass..   
-00003bb0: 2064 6566 206b 6579 7328 7365 6c66 2920   def keys(self) 
-00003bc0: 2d3e 2074 7970 696e 672e 4c69 7374 5b73  -> typing.List[s
-00003bd0: 7472 5d3a 0a20 2020 2020 2020 2027 2727  tr]:.        '''
-00003be0: 2052 6574 7572 6e20 7468 6520 6964 656e   Return the iden
-00003bf0: 7469 6669 6572 7320 6f66 2063 6f6c 6c65  tifiers of colle
-00003c00: 6374 696f 6e20 6d65 6d62 6572 7320 286d  ction members (m
-00003c10: 6174 6368 696e 6720 5079 7468 6f6e 2773  atching Python's
-00003c20: 2064 6963 742e 6b65 7973 2829 2066 756e   dict.keys() fun
-00003c30: 6374 696f 6e61 6c69 7479 292e 0a0a 2020  ctionality)...  
-00003c40: 2020 2020 2020 3a72 7479 7065 3a20 7479        :rtype: ty
-00003c50: 7069 6e67 2e4c 6973 745b 7374 725d 0a20  ping.List[str]. 
-00003c60: 2020 2020 2020 203a 7265 7475 726e 3a20         :return: 
-00003c70: 7468 6520 6964 656e 7469 6669 6572 7320  the identifiers 
-00003c80: 666f 7220 6561 6368 206d 656d 6265 7220  for each member 
-00003c90: 6f66 2074 6869 7320 636f 6c6c 6563 7469  of this collecti
-00003ca0: 6f6e 2e0a 2020 2020 2020 2020 2727 270a  on..        '''.
-00003cb0: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
-00003cc0: 2020 6465 6620 7661 6c75 6573 2873 656c    def values(sel
-00003cd0: 6629 202d 3e20 7479 7069 6e67 2e4c 6973  f) -> typing.Lis
-00003ce0: 743a 0a20 2020 2020 2020 2027 2727 2052  t:.        ''' R
-00003cf0: 6574 7572 6e20 7468 6520 7661 6c75 6573  eturn the values
-00003d00: 206f 6620 636f 6c6c 6563 7469 6f6e 2028   of collection (
-00003d10: 6d61 7463 6869 6e67 2050 7974 686f 6e27  matching Python'
-00003d20: 7320 6469 6374 2e76 616c 7565 7328 2920  s dict.values() 
-00003d30: 6675 6e63 7469 6f6e 616c 6974 7929 2e0a  functionality)..
-00003d40: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
-00003d50: 2074 7970 696e 672e 4c69 7374 0a20 2020   typing.List.   
-00003d60: 2020 2020 203a 7265 7475 726e 3a20 7468       :return: th
-00003d70: 6520 6d65 6d62 6572 7320 6f66 2074 6869  e members of thi
-00003d80: 7320 636f 6c6c 6563 7469 6f6e 2e0a 2020  s collection..  
-00003d90: 2020 2020 2020 2727 270a 2020 2020 2020        '''.      
-00003da0: 2020 7061 7373 0a0a 2020 2020 6465 6620    pass..    def 
-00003db0: 5f5f 6765 7469 7465 6d5f 5f28 7365 6c66  __getitem__(self
-00003dc0: 2c20 6b65 793a 2074 7970 696e 672e 556e  , key: typing.Un
-00003dd0: 696f 6e5b 696e 742c 2073 7472 5d29 202d  ion[int, str]) -
-00003de0: 3e20 2747 656e 6572 6963 5479 7065 273a  > 'GenericType':
-00003df0: 0a20 2020 2020 2020 2027 2727 200a 0a20  .        ''' .. 
-00003e00: 2020 2020 2020 203a 7061 7261 6d20 6b65         :param ke
-00003e10: 793a 200a 2020 2020 2020 2020 3a74 7970  y: .        :typ
-00003e20: 6520 6b65 793a 2074 7970 696e 672e 556e  e key: typing.Un
-00003e30: 696f 6e5b 696e 742c 2073 7472 5d0a 2020  ion[int, str].  
-00003e40: 2020 2020 2020 3a72 7479 7065 3a20 2747        :rtype: 'G
-00003e50: 656e 6572 6963 5479 7065 270a 2020 2020  enericType'.    
-00003e60: 2020 2020 2727 270a 2020 2020 2020 2020      '''.        
-00003e70: 7061 7373 0a0a 2020 2020 6465 6620 5f5f  pass..    def __
-00003e80: 7365 7469 7465 6d5f 5f28 7365 6c66 2c20  setitem__(self, 
-00003e90: 6b65 793a 2074 7970 696e 672e 556e 696f  key: typing.Unio
-00003ea0: 6e5b 696e 742c 2073 7472 5d2c 2076 616c  n[int, str], val
-00003eb0: 7565 3a20 2747 656e 6572 6963 5479 7065  ue: 'GenericType
-00003ec0: 2729 3a0a 2020 2020 2020 2020 2727 2720  '):.        ''' 
-00003ed0: 0a0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
-00003ee0: 206b 6579 3a20 0a20 2020 2020 2020 203a   key: .        :
-00003ef0: 7479 7065 206b 6579 3a20 7479 7069 6e67  type key: typing
-00003f00: 2e55 6e69 6f6e 5b69 6e74 2c20 7374 725d  .Union[int, str]
-00003f10: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-00003f20: 7661 6c75 653a 200a 2020 2020 2020 2020  value: .        
-00003f30: 3a74 7970 6520 7661 6c75 653a 2027 4765  :type value: 'Ge
-00003f40: 6e65 7269 6354 7970 6527 0a20 2020 2020  nericType'.     
-00003f50: 2020 2027 2727 0a20 2020 2020 2020 2070     '''.        p
-00003f60: 6173 730a 0a20 2020 2064 6566 205f 5f64  ass..    def __d
-00003f70: 656c 6974 656d 5f5f 2873 656c 662c 206b  elitem__(self, k
-00003f80: 6579 3a20 7479 7069 6e67 2e55 6e69 6f6e  ey: typing.Union
-00003f90: 5b69 6e74 2c20 7374 725d 2920 2d3e 2027  [int, str]) -> '
-00003fa0: 4765 6e65 7269 6354 7970 6527 3a0a 2020  GenericType':.  
-00003fb0: 2020 2020 2020 2727 2720 0a0a 2020 2020        ''' ..    
-00003fc0: 2020 2020 3a70 6172 616d 206b 6579 3a20      :param key: 
-00003fd0: 0a20 2020 2020 2020 203a 7479 7065 206b  .        :type k
-00003fe0: 6579 3a20 7479 7069 6e67 2e55 6e69 6f6e  ey: typing.Union
-00003ff0: 5b69 6e74 2c20 7374 725d 0a20 2020 2020  [int, str].     
-00004000: 2020 203a 7274 7970 653a 2027 4765 6e65     :rtype: 'Gene
-00004010: 7269 6354 7970 6527 0a20 2020 2020 2020  ricType'.       
-00004020: 2027 2727 0a20 2020 2020 2020 2070 6173   '''.        pas
-00004030: 730a 0a20 2020 2064 6566 205f 5f69 7465  s..    def __ite
-00004040: 725f 5f28 7365 6c66 2920 2d3e 2074 7970  r__(self) -> typ
-00004050: 696e 672e 4974 6572 6174 6f72 5b27 4765  ing.Iterator['Ge
-00004060: 6e65 7269 6354 7970 6527 5d3a 0a20 2020  nericType']:.   
-00004070: 2020 2020 2027 2727 200a 0a20 2020 2020       ''' ..     
-00004080: 2020 203a 7274 7970 653a 2074 7970 696e     :rtype: typin
-00004090: 672e 4974 6572 6174 6f72 5b27 4765 6e65  g.Iterator['Gene
-000040a0: 7269 6354 7970 6527 5d0a 2020 2020 2020  ricType'].      
-000040b0: 2020 2727 270a 2020 2020 2020 2020 7061    '''.        pa
-000040c0: 7373 0a0a 2020 2020 6465 6620 5f5f 6e65  ss..    def __ne
-000040d0: 7874 5f5f 2873 656c 6629 202d 3e20 2747  xt__(self) -> 'G
-000040e0: 656e 6572 6963 5479 7065 273a 0a20 2020  enericType':.   
-000040f0: 2020 2020 2027 2727 200a 0a20 2020 2020       ''' ..     
-00004100: 2020 203a 7274 7970 653a 2027 4765 6e65     :rtype: 'Gene
-00004110: 7269 6354 7970 6527 0a20 2020 2020 2020  ricType'.       
-00004120: 2027 2727 0a20 2020 2020 2020 2070 6173   '''.        pas
-00004130: 730a 0a20 2020 2064 6566 205f 5f6c 656e  s..    def __len
-00004140: 5f5f 2873 656c 6629 202d 3e20 696e 743a  __(self) -> int:
-00004150: 0a20 2020 2020 2020 2027 2727 200a 0a20  .        ''' .. 
-00004160: 2020 2020 2020 203a 7274 7970 653a 2069         :rtype: i
-00004170: 6e74 0a20 2020 2020 2020 2027 2727 0a20  nt.        '''. 
+00000ad0: 7079 5f70 726f 705f 636f 6c6c 6563 7469  py_prop_collecti
+00000ae0: 6f6e 2874 7970 696e 672e 4765 6e65 7269  on(typing.Generi
+00000af0: 635b 4765 6e65 7269 6354 7970 655d 293a  c[GenericType]):
+00000b00: 0a20 2020 2027 2727 2062 7569 6c74 2d69  .    ''' built-i
+00000b10: 6e20 636c 6173 7320 7573 6564 2066 6f72  n class used for
+00000b20: 2061 6c6c 2063 6f6c 6c65 6374 696f 6e73   all collections
+00000b30: 2e0a 2020 2020 2727 270a 0a20 2020 2064  ..    '''..    d
+00000b40: 6566 2066 696e 6428 7365 6c66 2c20 6b65  ef find(self, ke
+00000b50: 793a 2074 7970 696e 672e 4f70 7469 6f6e  y: typing.Option
+00000b60: 616c 5b73 7472 5d29 202d 3e20 696e 743a  al[str]) -> int:
+00000b70: 0a20 2020 2020 2020 2027 2727 2052 6574  .        ''' Ret
+00000b80: 7572 6e73 2074 6865 2069 6e64 6578 206f  urns the index o
+00000b90: 6620 6120 6b65 7920 696e 2061 2063 6f6c  f a key in a col
+00000ba0: 6c65 6374 696f 6e20 6f72 202d 3120 7768  lection or -1 wh
+00000bb0: 656e 206e 6f74 2066 6f75 6e64 2028 6d61  en not found (ma
+00000bc0: 7463 6865 7320 5079 7468 6f6e 2773 2073  tches Python's s
+00000bd0: 7472 696e 6720 6669 6e64 2066 756e 6374  tring find funct
+00000be0: 696f 6e20 6f66 2074 6865 2073 616d 6520  ion of the same 
+00000bf0: 6e61 6d65 292e 0a0a 2020 2020 2020 2020  name)...        
+00000c00: 3a70 6172 616d 206b 6579 3a20 5468 6520  :param key: The 
+00000c10: 6964 656e 7469 6669 6572 2066 6f72 2074  identifier for t
+00000c20: 6865 2063 6f6c 6c65 6374 696f 6e20 6d65  he collection me
+00000c30: 6d62 6572 2e0a 2020 2020 2020 2020 3a74  mber..        :t
+00000c40: 7970 6520 6b65 793a 2074 7970 696e 672e  ype key: typing.
+00000c50: 4f70 7469 6f6e 616c 5b73 7472 5d0a 2020  Optional[str].  
+00000c60: 2020 2020 2020 3a72 7479 7065 3a20 696e        :rtype: in
+00000c70: 740a 2020 2020 2020 2020 3a72 6574 7572  t.        :retur
+00000c80: 6e3a 2069 6e64 6578 206f 6620 7468 6520  n: index of the 
+00000c90: 6b65 792e 0a20 2020 2020 2020 2027 2727  key..        '''
+00000ca0: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
+00000cb0: 2020 2064 6566 2066 6f72 6561 6368 5f67     def foreach_g
+00000cc0: 6574 2873 656c 662c 2061 7474 722c 2073  et(self, attr, s
+00000cd0: 6571 293a 0a20 2020 2020 2020 2027 2727  eq):.        '''
+00000ce0: 2054 6869 7320 6973 2061 2066 756e 6374   This is a funct
+00000cf0: 696f 6e20 746f 2067 6976 6520 6661 7374  ion to give fast
+00000d00: 2061 6363 6573 7320 746f 2061 7474 7269   access to attri
+00000d10: 6275 7465 7320 7769 7468 696e 2061 2063  butes within a c
+00000d20: 6f6c 6c65 6374 696f 6e2e 204f 6e6c 7920  ollection. Only 
+00000d30: 776f 726b 7320 666f 7220 2762 6173 6963  works for 'basic
+00000d40: 2074 7970 6527 2070 726f 7065 7274 6965   type' propertie
+00000d50: 7320 2862 6f6f 6c2c 2069 6e74 2061 6e64  s (bool, int and
+00000d60: 2066 6c6f 6174 2921 204d 756c 7469 2d64   float)! Multi-d
+00000d70: 696d 656e 7369 6f6e 616c 2061 7272 6179  imensional array
+00000d80: 7320 286c 696b 6520 6172 7261 7920 6f66  s (like array of
+00000d90: 2076 6563 746f 7273 2920 7769 6c6c 2062   vectors) will b
+00000da0: 6520 666c 6174 7465 6e65 6420 696e 746f  e flattened into
+00000db0: 2073 6571 2e0a 0a20 2020 2020 2020 2027   seq...        '
+00000dc0: 2727 0a20 2020 2020 2020 2070 6173 730a  ''.        pass.
+00000dd0: 0a20 2020 2064 6566 2066 6f72 6561 6368  .    def foreach
+00000de0: 5f73 6574 2873 656c 662c 2061 7474 722c  _set(self, attr,
+00000df0: 2073 6571 293a 0a20 2020 2020 2020 2027   seq):.        '
+00000e00: 2727 2054 6869 7320 6973 2061 2066 756e  '' This is a fun
+00000e10: 6374 696f 6e20 746f 2067 6976 6520 6661  ction to give fa
+00000e20: 7374 2061 6363 6573 7320 746f 2061 7474  st access to att
+00000e30: 7269 6275 7465 7320 7769 7468 696e 2061  ributes within a
+00000e40: 2063 6f6c 6c65 6374 696f 6e2e 204f 6e6c   collection. Onl
+00000e50: 7920 776f 726b 7320 666f 7220 2762 6173  y works for 'bas
+00000e60: 6963 2074 7970 6527 2070 726f 7065 7274  ic type' propert
+00000e70: 6965 7320 2862 6f6f 6c2c 2069 6e74 2061  ies (bool, int a
+00000e80: 6e64 2066 6c6f 6174 2921 2073 6571 206d  nd float)! seq m
+00000e90: 7573 7420 6265 2075 6e69 2d64 696d 656e  ust be uni-dimen
+00000ea0: 7369 6f6e 616c 2c20 6d75 6c74 692d 6469  sional, multi-di
+00000eb0: 6d65 6e73 696f 6e61 6c20 6172 7261 7973  mensional arrays
+00000ec0: 2028 6c69 6b65 2061 7272 6179 206f 6620   (like array of 
+00000ed0: 7665 6374 6f72 7329 2077 696c 6c20 6265  vectors) will be
+00000ee0: 2072 652d 6372 6561 7465 6420 6672 6f6d   re-created from
+00000ef0: 2069 742e 0a0a 2020 2020 2020 2020 2727   it...        ''
+00000f00: 270a 2020 2020 2020 2020 7061 7373 0a0a  '.        pass..
+00000f10: 2020 2020 6465 6620 6765 7428 7365 6c66      def get(self
+00000f20: 2c0a 2020 2020 2020 2020 2020 2020 6b65  ,.            ke
+00000f30: 793a 2074 7970 696e 672e 4f70 7469 6f6e  y: typing.Option
+00000f40: 616c 5b73 7472 5d2c 0a20 2020 2020 2020  al[str],.       
+00000f50: 2020 2020 2064 6566 6175 6c74 3a20 7479       default: ty
+00000f60: 7069 6e67 2e4f 7074 696f 6e61 6c5b 7479  ping.Optional[ty
+00000f70: 7069 6e67 2e41 6e79 5d20 3d20 4e6f 6e65  ping.Any] = None
+00000f80: 293a 0a20 2020 2020 2020 2027 2727 2052  ):.        ''' R
+00000f90: 6574 7572 6e73 2074 6865 2076 616c 7565  eturns the value
+00000fa0: 206f 6620 7468 6520 6974 656d 2061 7373   of the item ass
+00000fb0: 6967 6e65 6420 746f 206b 6579 206f 7220  igned to key or 
+00000fc0: 6465 6661 756c 7420 7768 656e 206e 6f74  default when not
+00000fd0: 2066 6f75 6e64 2028 6d61 7463 6865 7320   found (matches 
+00000fe0: 5079 7468 6f6e 2773 2064 6963 7469 6f6e  Python's diction
+00000ff0: 6172 7920 6675 6e63 7469 6f6e 206f 6620  ary function of 
+00001000: 7468 6520 7361 6d65 206e 616d 6529 2e0a  the same name)..
+00001010: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+00001020: 6b65 793a 2054 6865 2069 6465 6e74 6966  key: The identif
+00001030: 6965 7220 666f 7220 7468 6520 636f 6c6c  ier for the coll
+00001040: 6563 7469 6f6e 206d 656d 6265 722e 0a20  ection member.. 
+00001050: 2020 2020 2020 203a 7479 7065 206b 6579         :type key
+00001060: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
+00001070: 6c5b 7374 725d 0a20 2020 2020 2020 203a  l[str].        :
+00001080: 7061 7261 6d20 6465 6661 756c 743a 204f  param default: O
+00001090: 7074 696f 6e61 6c20 6172 6775 6d65 6e74  ptional argument
+000010a0: 2066 6f72 2074 6865 2076 616c 7565 2074   for the value t
+000010b0: 6f20 7265 7475 726e 2069 6620 2a6b 6579  o return if *key
+000010c0: 2a20 6973 206e 6f74 2066 6f75 6e64 2e0a  * is not found..
+000010d0: 2020 2020 2020 2020 3a74 7970 6520 6465          :type de
+000010e0: 6661 756c 743a 2074 7970 696e 672e 4f70  fault: typing.Op
+000010f0: 7469 6f6e 616c 5b74 7970 696e 672e 416e  tional[typing.An
+00001100: 795d 0a20 2020 2020 2020 2027 2727 0a20  y].        '''. 
+00001110: 2020 2020 2020 2070 6173 730a 0a20 2020         pass..   
+00001120: 2064 6566 2069 7465 6d73 2873 656c 6629   def items(self)
+00001130: 202d 3e20 7479 7069 6e67 2e4c 6973 743a   -> typing.List:
+00001140: 0a20 2020 2020 2020 2027 2727 2052 6574  .        ''' Ret
+00001150: 7572 6e20 7468 6520 6964 656e 7469 6669  urn the identifi
+00001160: 6572 7320 6f66 2063 6f6c 6c65 6374 696f  ers of collectio
+00001170: 6e20 6d65 6d62 6572 7320 286d 6174 6368  n members (match
+00001180: 696e 6720 5079 7468 6f6e 2773 2064 6963  ing Python's dic
+00001190: 742e 6974 656d 7328 2920 6675 6e63 7469  t.items() functi
+000011a0: 6f6e 616c 6974 7929 2e0a 0a20 2020 2020  onality)...     
+000011b0: 2020 203a 7274 7970 653a 2074 7970 696e     :rtype: typin
+000011c0: 672e 4c69 7374 0a20 2020 2020 2020 203a  g.List.        :
+000011d0: 7265 7475 726e 3a20 286b 6579 2c20 7661  return: (key, va
+000011e0: 6c75 6529 2070 6169 7273 2066 6f72 2065  lue) pairs for e
+000011f0: 6163 6820 6d65 6d62 6572 206f 6620 7468  ach member of th
+00001200: 6973 2063 6f6c 6c65 6374 696f 6e2e 0a20  is collection.. 
+00001210: 2020 2020 2020 2027 2727 0a20 2020 2020         '''.     
+00001220: 2020 2070 6173 730a 0a20 2020 2064 6566     pass..    def
+00001230: 206b 6579 7328 7365 6c66 2920 2d3e 2074   keys(self) -> t
+00001240: 7970 696e 672e 4c69 7374 5b73 7472 5d3a  yping.List[str]:
+00001250: 0a20 2020 2020 2020 2027 2727 2052 6574  .        ''' Ret
+00001260: 7572 6e20 7468 6520 6964 656e 7469 6669  urn the identifi
+00001270: 6572 7320 6f66 2063 6f6c 6c65 6374 696f  ers of collectio
+00001280: 6e20 6d65 6d62 6572 7320 286d 6174 6368  n members (match
+00001290: 696e 6720 5079 7468 6f6e 2773 2064 6963  ing Python's dic
+000012a0: 742e 6b65 7973 2829 2066 756e 6374 696f  t.keys() functio
+000012b0: 6e61 6c69 7479 292e 0a0a 2020 2020 2020  nality)...      
+000012c0: 2020 3a72 7479 7065 3a20 7479 7069 6e67    :rtype: typing
+000012d0: 2e4c 6973 745b 7374 725d 0a20 2020 2020  .List[str].     
+000012e0: 2020 203a 7265 7475 726e 3a20 7468 6520     :return: the 
+000012f0: 6964 656e 7469 6669 6572 7320 666f 7220  identifiers for 
+00001300: 6561 6368 206d 656d 6265 7220 6f66 2074  each member of t
+00001310: 6869 7320 636f 6c6c 6563 7469 6f6e 2e0a  his collection..
+00001320: 2020 2020 2020 2020 2727 270a 2020 2020          '''.    
+00001330: 2020 2020 7061 7373 0a0a 2020 2020 6465      pass..    de
+00001340: 6620 7661 6c75 6573 2873 656c 6629 202d  f values(self) -
+00001350: 3e20 7479 7069 6e67 2e4c 6973 743a 0a20  > typing.List:. 
+00001360: 2020 2020 2020 2027 2727 2052 6574 7572         ''' Retur
+00001370: 6e20 7468 6520 7661 6c75 6573 206f 6620  n the values of 
+00001380: 636f 6c6c 6563 7469 6f6e 2028 6d61 7463  collection (matc
+00001390: 6869 6e67 2050 7974 686f 6e27 7320 6469  hing Python's di
+000013a0: 6374 2e76 616c 7565 7328 2920 6675 6e63  ct.values() func
+000013b0: 7469 6f6e 616c 6974 7929 2e0a 0a20 2020  tionality)...   
+000013c0: 2020 2020 203a 7274 7970 653a 2074 7970       :rtype: typ
+000013d0: 696e 672e 4c69 7374 0a20 2020 2020 2020  ing.List.       
+000013e0: 203a 7265 7475 726e 3a20 7468 6520 6d65   :return: the me
+000013f0: 6d62 6572 7320 6f66 2074 6869 7320 636f  mbers of this co
+00001400: 6c6c 6563 7469 6f6e 2e0a 2020 2020 2020  llection..      
+00001410: 2020 2727 270a 2020 2020 2020 2020 7061    '''.        pa
+00001420: 7373 0a0a 2020 2020 6465 6620 5f5f 6765  ss..    def __ge
+00001430: 7469 7465 6d5f 5f28 7365 6c66 2c20 6b65  titem__(self, ke
+00001440: 793a 2074 7970 696e 672e 556e 696f 6e5b  y: typing.Union[
+00001450: 696e 742c 2073 7472 5d29 202d 3e20 2747  int, str]) -> 'G
+00001460: 656e 6572 6963 5479 7065 273a 0a20 2020  enericType':.   
+00001470: 2020 2020 2027 2727 200a 0a20 2020 2020       ''' ..     
+00001480: 2020 203a 7061 7261 6d20 6b65 793a 200a     :param key: .
+00001490: 2020 2020 2020 2020 3a74 7970 6520 6b65          :type ke
+000014a0: 793a 2074 7970 696e 672e 556e 696f 6e5b  y: typing.Union[
+000014b0: 696e 742c 2073 7472 5d0a 2020 2020 2020  int, str].      
+000014c0: 2020 3a72 7479 7065 3a20 2747 656e 6572    :rtype: 'Gener
+000014d0: 6963 5479 7065 270a 2020 2020 2020 2020  icType'.        
+000014e0: 2727 270a 2020 2020 2020 2020 7061 7373  '''.        pass
+000014f0: 0a0a 2020 2020 6465 6620 5f5f 7365 7469  ..    def __seti
+00001500: 7465 6d5f 5f28 7365 6c66 2c20 6b65 793a  tem__(self, key:
+00001510: 2074 7970 696e 672e 556e 696f 6e5b 696e   typing.Union[in
+00001520: 742c 2073 7472 5d2c 2076 616c 7565 3a20  t, str], value: 
+00001530: 2747 656e 6572 6963 5479 7065 2729 3a0a  'GenericType'):.
+00001540: 2020 2020 2020 2020 2727 2720 0a0a 2020          ''' ..  
+00001550: 2020 2020 2020 3a70 6172 616d 206b 6579        :param key
+00001560: 3a20 0a20 2020 2020 2020 203a 7479 7065  : .        :type
+00001570: 206b 6579 3a20 7479 7069 6e67 2e55 6e69   key: typing.Uni
+00001580: 6f6e 5b69 6e74 2c20 7374 725d 0a20 2020  on[int, str].   
+00001590: 2020 2020 203a 7061 7261 6d20 7661 6c75       :param valu
+000015a0: 653a 200a 2020 2020 2020 2020 3a74 7970  e: .        :typ
+000015b0: 6520 7661 6c75 653a 2027 4765 6e65 7269  e value: 'Generi
+000015c0: 6354 7970 6527 0a20 2020 2020 2020 2027  cType'.        '
+000015d0: 2727 0a20 2020 2020 2020 2070 6173 730a  ''.        pass.
+000015e0: 0a20 2020 2064 6566 205f 5f64 656c 6974  .    def __delit
+000015f0: 656d 5f5f 2873 656c 662c 206b 6579 3a20  em__(self, key: 
+00001600: 7479 7069 6e67 2e55 6e69 6f6e 5b69 6e74  typing.Union[int
+00001610: 2c20 7374 725d 2920 2d3e 2027 4765 6e65  , str]) -> 'Gene
+00001620: 7269 6354 7970 6527 3a0a 2020 2020 2020  ricType':.      
+00001630: 2020 2727 2720 0a0a 2020 2020 2020 2020    ''' ..        
+00001640: 3a70 6172 616d 206b 6579 3a20 0a20 2020  :param key: .   
+00001650: 2020 2020 203a 7479 7065 206b 6579 3a20       :type key: 
+00001660: 7479 7069 6e67 2e55 6e69 6f6e 5b69 6e74  typing.Union[int
+00001670: 2c20 7374 725d 0a20 2020 2020 2020 203a  , str].        :
+00001680: 7274 7970 653a 2027 4765 6e65 7269 6354  rtype: 'GenericT
+00001690: 7970 6527 0a20 2020 2020 2020 2027 2727  ype'.        '''
+000016a0: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
+000016b0: 2020 2064 6566 205f 5f69 7465 725f 5f28     def __iter__(
+000016c0: 7365 6c66 2920 2d3e 2074 7970 696e 672e  self) -> typing.
+000016d0: 4974 6572 6174 6f72 5b27 4765 6e65 7269  Iterator['Generi
+000016e0: 6354 7970 6527 5d3a 0a20 2020 2020 2020  cType']:.       
+000016f0: 2027 2727 200a 0a20 2020 2020 2020 203a   ''' ..        :
+00001700: 7274 7970 653a 2074 7970 696e 672e 4974  rtype: typing.It
+00001710: 6572 6174 6f72 5b27 4765 6e65 7269 6354  erator['GenericT
+00001720: 7970 6527 5d0a 2020 2020 2020 2020 2727  ype'].        ''
+00001730: 270a 2020 2020 2020 2020 7061 7373 0a0a  '.        pass..
+00001740: 2020 2020 6465 6620 5f5f 6e65 7874 5f5f      def __next__
+00001750: 2873 656c 6629 202d 3e20 2747 656e 6572  (self) -> 'Gener
+00001760: 6963 5479 7065 273a 0a20 2020 2020 2020  icType':.       
+00001770: 2027 2727 200a 0a20 2020 2020 2020 203a   ''' ..        :
+00001780: 7274 7970 653a 2027 4765 6e65 7269 6354  rtype: 'GenericT
+00001790: 7970 6527 0a20 2020 2020 2020 2027 2727  ype'.        '''
+000017a0: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
+000017b0: 2020 2064 6566 205f 5f6c 656e 5f5f 2873     def __len__(s
+000017c0: 656c 6629 202d 3e20 696e 743a 0a20 2020  elf) -> int:.   
+000017d0: 2020 2020 2027 2727 200a 0a20 2020 2020       ''' ..     
+000017e0: 2020 203a 7274 7970 653a 2069 6e74 0a20     :rtype: int. 
+000017f0: 2020 2020 2020 2027 2727 0a20 2020 2020         '''.     
+00001800: 2020 2070 6173 730a 0a0a 636c 6173 7320     pass...class 
+00001810: 6270 795f 7374 7275 6374 3a0a 2020 2020  bpy_struct:.    
+00001820: 2727 2720 6275 696c 742d 696e 2062 6173  ''' built-in bas
+00001830: 6520 636c 6173 7320 666f 7220 616c 6c20  e class for all 
+00001840: 636c 6173 7365 7320 696e 2062 7079 2e74  classes in bpy.t
+00001850: 7970 6573 2e0a 2020 2020 2727 270a 0a20  ypes..    '''.. 
+00001860: 2020 2069 645f 6461 7461 203d 204e 6f6e     id_data = Non
+00001870: 650a 2020 2020 2727 2720 5468 6520 6062  e.    ''' The `b
+00001880: 7079 2e74 7970 6573 2e49 4460 206f 626a  py.types.ID` obj
+00001890: 6563 7420 7468 6973 2064 6174 6162 6c6f  ect this datablo
+000018a0: 636b 2069 7320 6672 6f6d 206f 7220 4e6f  ck is from or No
+000018b0: 6e65 2c20 286e 6f74 2061 7661 696c 6162  ne, (not availab
+000018c0: 6c65 2066 6f72 2061 6c6c 2064 6174 6120  le for all data 
+000018d0: 7479 7065 7329 2727 270a 0a20 2020 2064  types)'''..    d
+000018e0: 6566 2061 735f 706f 696e 7465 7228 7365  ef as_pointer(se
+000018f0: 6c66 2920 2d3e 2069 6e74 3a0a 2020 2020  lf) -> int:.    
+00001900: 2020 2020 2727 2720 5265 7475 726e 7320      ''' Returns 
+00001910: 7468 6520 6d65 6d6f 7279 2061 6464 7265  the memory addre
+00001920: 7373 2077 6869 6368 2068 6f6c 6473 2061  ss which holds a
+00001930: 2070 6f69 6e74 6572 2074 6f20 426c 656e   pointer to Blen
+00001940: 6465 7227 7320 696e 7465 726e 616c 2064  der's internal d
+00001950: 6174 610a 0a20 2020 2020 2020 203a 7274  ata..        :rt
+00001960: 7970 653a 2069 6e74 0a20 2020 2020 2020  ype: int.       
+00001970: 203a 7265 7475 726e 3a20 696e 7420 286d   :return: int (m
+00001980: 656d 6f72 7920 6164 6472 6573 7329 2e0a  emory address)..
+00001990: 2020 2020 2020 2020 2727 270a 2020 2020          '''.    
+000019a0: 2020 2020 7061 7373 0a0a 2020 2020 6465      pass..    de
+000019b0: 6620 6472 6976 6572 5f61 6464 2873 656c  f driver_add(sel
+000019c0: 662c 0a20 2020 2020 2020 2020 2020 2020  f,.             
+000019d0: 2020 2020 2020 7061 7468 3a20 7479 7069        path: typi
+000019e0: 6e67 2e4f 7074 696f 6e61 6c5b 7374 725d  ng.Optional[str]
+000019f0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00001a00: 2020 2020 2069 6e64 6578 3a20 7479 7069       index: typi
+00001a10: 6e67 2e4f 7074 696f 6e61 6c5b 696e 745d  ng.Optional[int]
+00001a20: 203d 202d 3129 202d 3e20 2746 4375 7276   = -1) -> 'FCurv
+00001a30: 6527 3a0a 2020 2020 2020 2020 2727 2720  e':.        ''' 
+00001a40: 4164 6473 2064 7269 7665 7228 7329 2074  Adds driver(s) t
+00001a50: 6f20 7468 6520 6769 7665 6e20 7072 6f70  o the given prop
+00001a60: 6572 7479 0a0a 2020 2020 2020 2020 3a70  erty..        :p
+00001a70: 6172 616d 2070 6174 683a 2070 6174 6820  aram path: path 
+00001a80: 746f 2074 6865 2070 726f 7065 7274 7920  to the property 
+00001a90: 746f 2064 7269 7665 2c20 616e 616c 6f67  to drive, analog
+00001aa0: 6f75 7320 746f 2074 6865 2066 6375 7276  ous to the fcurv
+00001ab0: 6527 7320 6461 7461 2070 6174 682e 0a20  e's data path.. 
+00001ac0: 2020 2020 2020 203a 7479 7065 2070 6174         :type pat
+00001ad0: 683a 2074 7970 696e 672e 4f70 7469 6f6e  h: typing.Option
+00001ae0: 616c 5b73 7472 5d0a 2020 2020 2020 2020  al[str].        
+00001af0: 3a70 6172 616d 2069 6e64 6578 3a20 6172  :param index: ar
+00001b00: 7261 7920 696e 6465 7820 6f66 2074 6865  ray index of the
+00001b10: 2070 726f 7065 7274 7920 6472 6976 652e   property drive.
+00001b20: 2044 6566 6175 6c74 7320 746f 202d 3120   Defaults to -1 
+00001b30: 666f 7220 616c 6c20 696e 6469 6365 7320  for all indices 
+00001b40: 6f72 2061 2073 696e 676c 6520 6368 616e  or a single chan
+00001b50: 6e65 6c20 6966 2074 6865 2070 726f 7065  nel if the prope
+00001b60: 7274 7920 6973 206e 6f74 2061 6e20 6172  rty is not an ar
+00001b70: 7261 792e 0a20 2020 2020 2020 203a 7479  ray..        :ty
+00001b80: 7065 2069 6e64 6578 3a20 7479 7069 6e67  pe index: typing
+00001b90: 2e4f 7074 696f 6e61 6c5b 696e 745d 0a20  .Optional[int]. 
+00001ba0: 2020 2020 2020 203a 7274 7970 653a 2027         :rtype: '
+00001bb0: 4643 7572 7665 270a 2020 2020 2020 2020  FCurve'.        
+00001bc0: 3a72 6574 7572 6e3a 2054 6865 2064 7269  :return: The dri
+00001bd0: 7665 7228 7329 2061 6464 6564 2e0a 2020  ver(s) added..  
+00001be0: 2020 2020 2020 2727 270a 2020 2020 2020        '''.      
+00001bf0: 2020 7061 7373 0a0a 2020 2020 6465 6620    pass..    def 
+00001c00: 6472 6976 6572 5f72 656d 6f76 6528 7365  driver_remove(se
+00001c10: 6c66 2c0a 2020 2020 2020 2020 2020 2020  lf,.            
+00001c20: 2020 2020 2020 2020 2020 7061 7468 3a20            path: 
+00001c30: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
+00001c40: 7374 725d 2c0a 2020 2020 2020 2020 2020  str],.          
+00001c50: 2020 2020 2020 2020 2020 2020 696e 6465              inde
+00001c60: 783a 2074 7970 696e 672e 4f70 7469 6f6e  x: typing.Option
+00001c70: 616c 5b69 6e74 5d20 3d20 2d31 2920 2d3e  al[int] = -1) ->
+00001c80: 2062 6f6f 6c3a 0a20 2020 2020 2020 2027   bool:.        '
+00001c90: 2727 2052 656d 6f76 6520 6472 6976 6572  '' Remove driver
+00001ca0: 2873 2920 6672 6f6d 2074 6865 2067 6976  (s) from the giv
+00001cb0: 656e 2070 726f 7065 7274 790a 0a20 2020  en property..   
+00001cc0: 2020 2020 203a 7061 7261 6d20 7061 7468       :param path
+00001cd0: 3a20 7061 7468 2074 6f20 7468 6520 7072  : path to the pr
+00001ce0: 6f70 6572 7479 2074 6f20 6472 6976 652c  operty to drive,
+00001cf0: 2061 6e61 6c6f 676f 7573 2074 6f20 7468   analogous to th
+00001d00: 6520 6663 7572 7665 2773 2064 6174 6120  e fcurve's data 
+00001d10: 7061 7468 2e0a 2020 2020 2020 2020 3a74  path..        :t
+00001d20: 7970 6520 7061 7468 3a20 7479 7069 6e67  ype path: typing
+00001d30: 2e4f 7074 696f 6e61 6c5b 7374 725d 0a20  .Optional[str]. 
+00001d40: 2020 2020 2020 203a 7061 7261 6d20 696e         :param in
+00001d50: 6465 783a 2061 7272 6179 2069 6e64 6578  dex: array index
+00001d60: 206f 6620 7468 6520 7072 6f70 6572 7479   of the property
+00001d70: 2064 7269 7665 2e20 4465 6661 756c 7473   drive. Defaults
+00001d80: 2074 6f20 2d31 2066 6f72 2061 6c6c 2069   to -1 for all i
+00001d90: 6e64 6963 6573 206f 7220 6120 7369 6e67  ndices or a sing
+00001da0: 6c65 2063 6861 6e6e 656c 2069 6620 7468  le channel if th
+00001db0: 6520 7072 6f70 6572 7479 2069 7320 6e6f  e property is no
+00001dc0: 7420 616e 2061 7272 6179 2e0a 2020 2020  t an array..    
+00001dd0: 2020 2020 3a74 7970 6520 696e 6465 783a      :type index:
+00001de0: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
+00001df0: 5b69 6e74 5d0a 2020 2020 2020 2020 3a72  [int].        :r
+00001e00: 7479 7065 3a20 626f 6f6c 0a20 2020 2020  type: bool.     
+00001e10: 2020 203a 7265 7475 726e 3a20 5375 6363     :return: Succ
+00001e20: 6573 7320 6f66 2064 7269 7665 7220 7265  ess of driver re
+00001e30: 6d6f 7661 6c2e 0a20 2020 2020 2020 2027  moval..        '
+00001e40: 2727 0a20 2020 2020 2020 2070 6173 730a  ''.        pass.
+00001e50: 0a20 2020 2064 6566 2067 6574 2873 656c  .    def get(sel
+00001e60: 662c 0a20 2020 2020 2020 2020 2020 206b  f,.            k
+00001e70: 6579 3a20 7479 7069 6e67 2e4f 7074 696f  ey: typing.Optio
+00001e80: 6e61 6c5b 7374 725d 2c0a 2020 2020 2020  nal[str],.      
+00001e90: 2020 2020 2020 6465 6661 756c 743a 2074        default: t
+00001ea0: 7970 696e 672e 4f70 7469 6f6e 616c 5b74  yping.Optional[t
+00001eb0: 7970 696e 672e 416e 795d 203d 204e 6f6e  yping.Any] = Non
+00001ec0: 6529 3a0a 2020 2020 2020 2020 2727 2720  e):.        ''' 
+00001ed0: 5265 7475 726e 7320 7468 6520 7661 6c75  Returns the valu
+00001ee0: 6520 6f66 2074 6865 2063 7573 746f 6d20  e of the custom 
+00001ef0: 7072 6f70 6572 7479 2061 7373 6967 6e65  property assigne
+00001f00: 6420 746f 206b 6579 206f 7220 6465 6661  d to key or defa
+00001f10: 756c 7420 7768 656e 206e 6f74 2066 6f75  ult when not fou
+00001f20: 6e64 2028 6d61 7463 6865 7320 5079 7468  nd (matches Pyth
+00001f30: 6f6e 2773 2064 6963 7469 6f6e 6172 7920  on's dictionary 
+00001f40: 6675 6e63 7469 6f6e 206f 6620 7468 6520  function of the 
+00001f50: 7361 6d65 206e 616d 6529 2e0a 0a20 2020  same name)...   
+00001f60: 2020 2020 203a 7061 7261 6d20 6b65 793a       :param key:
+00001f70: 2054 6865 206b 6579 2061 7373 6f63 6961   The key associa
+00001f80: 7465 6420 7769 7468 2074 6865 2063 7573  ted with the cus
+00001f90: 746f 6d20 7072 6f70 6572 7479 2e0a 2020  tom property..  
+00001fa0: 2020 2020 2020 3a74 7970 6520 6b65 793a        :type key:
+00001fb0: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
+00001fc0: 5b73 7472 5d0a 2020 2020 2020 2020 3a70  [str].        :p
+00001fd0: 6172 616d 2064 6566 6175 6c74 3a20 4f70  aram default: Op
+00001fe0: 7469 6f6e 616c 2061 7267 756d 656e 7420  tional argument 
+00001ff0: 666f 7220 7468 6520 7661 6c75 6520 746f  for the value to
+00002000: 2072 6574 7572 6e20 6966 202a 6b65 792a   return if *key*
+00002010: 2069 7320 6e6f 7420 666f 756e 642e 0a20   is not found.. 
+00002020: 2020 2020 2020 203a 7479 7065 2064 6566         :type def
+00002030: 6175 6c74 3a20 7479 7069 6e67 2e4f 7074  ault: typing.Opt
+00002040: 696f 6e61 6c5b 7479 7069 6e67 2e41 6e79  ional[typing.Any
+00002050: 5d0a 2020 2020 2020 2020 2727 270a 2020  ].        '''.  
+00002060: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
+00002070: 6465 6620 6964 5f70 726f 7065 7274 6965  def id_propertie
+00002080: 735f 636c 6561 7228 7365 6c66 293a 0a20  s_clear(self):. 
+00002090: 2020 2020 2020 2027 2727 200a 0a20 2020         ''' ..   
+000020a0: 2020 2020 2027 2727 0a20 2020 2020 2020       '''.       
+000020b0: 2070 6173 730a 0a20 2020 2064 6566 2069   pass..    def i
+000020c0: 645f 7072 6f70 6572 7469 6573 5f65 6e73  d_properties_ens
+000020d0: 7572 6528 7365 6c66 2920 2d3e 2074 7970  ure(self) -> typ
+000020e0: 696e 672e 416e 793a 0a20 2020 2020 2020  ing.Any:.       
+000020f0: 2027 2727 200a 0a20 2020 2020 2020 203a   ''' ..        :
+00002100: 7274 7970 653a 2074 7970 696e 672e 416e  rtype: typing.An
+00002110: 790a 2020 2020 2020 2020 3a72 6574 7572  y.        :retur
+00002120: 6e3a 2074 6865 2070 6172 656e 7420 6772  n: the parent gr
+00002130: 6f75 7020 666f 7220 616e 2052 4e41 2073  oup for an RNA s
+00002140: 7472 7563 7427 7320 6375 7374 6f6d 2049  truct's custom I
+00002150: 4450 726f 7065 7274 6965 732e 0a20 2020  DProperties..   
+00002160: 2020 2020 2027 2727 0a20 2020 2020 2020       '''.       
+00002170: 2070 6173 730a 0a20 2020 2064 6566 2069   pass..    def i
+00002180: 645f 7072 6f70 6572 7469 6573 5f75 6928  d_properties_ui(
+00002190: 7365 6c66 2c20 6b65 793a 2074 7970 696e  self, key: typin
+000021a0: 672e 4f70 7469 6f6e 616c 5b74 7970 696e  g.Optional[typin
+000021b0: 672e 416e 795d 2920 2d3e 2074 7970 696e  g.Any]) -> typin
+000021c0: 672e 416e 793a 0a20 2020 2020 2020 2027  g.Any:.        '
+000021d0: 2727 200a 0a20 2020 2020 2020 203a 7061  '' ..        :pa
+000021e0: 7261 6d20 6b65 793a 2020 5374 7269 6e67  ram key:  String
+000021f0: 206e 616d 6520 6f66 2074 6865 2070 726f   name of the pro
+00002200: 7065 7274 792e 0a20 2020 2020 2020 203a  perty..        :
+00002210: 7479 7065 206b 6579 3a20 7479 7069 6e67  type key: typing
+00002220: 2e4f 7074 696f 6e61 6c5b 7479 7069 6e67  .Optional[typing
+00002230: 2e41 6e79 5d0a 2020 2020 2020 2020 3a72  .Any].        :r
+00002240: 7479 7065 3a20 7479 7069 6e67 2e41 6e79  type: typing.Any
+00002250: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
+00002260: 3a20 5265 7475 726e 2061 6e20 6f62 6a65  : Return an obje
+00002270: 6374 2075 7365 6420 746f 206d 616e 6167  ct used to manag
+00002280: 6520 616e 2049 4450 726f 7065 7274 7927  e an IDProperty'
+00002290: 7320 5549 2064 6174 612e 0a20 2020 2020  s UI data..     
+000022a0: 2020 2027 2727 0a20 2020 2020 2020 2070     '''.        p
+000022b0: 6173 730a 0a20 2020 2064 6566 2069 735f  ass..    def is_
+000022c0: 7072 6f70 6572 7479 5f68 6964 6465 6e28  property_hidden(
+000022d0: 7365 6c66 2c20 7072 6f70 6572 7479 2920  self, property) 
+000022e0: 2d3e 2062 6f6f 6c3a 0a20 2020 2020 2020  -> bool:.       
+000022f0: 2027 2727 2043 6865 636b 2069 6620 6120   ''' Check if a 
+00002300: 7072 6f70 6572 7479 2069 7320 6869 6464  property is hidd
+00002310: 656e 2e0a 0a20 2020 2020 2020 203a 7274  en...        :rt
+00002320: 7970 653a 2062 6f6f 6c0a 2020 2020 2020  ype: bool.      
+00002330: 2020 3a72 6574 7572 6e3a 2054 7275 6520    :return: True 
+00002340: 7768 656e 2074 6865 2070 726f 7065 7274  when the propert
+00002350: 7920 6973 2068 6964 6465 6e2e 0a20 2020  y is hidden..   
+00002360: 2020 2020 2027 2727 0a20 2020 2020 2020       '''.       
+00002370: 2070 6173 730a 0a20 2020 2064 6566 2069   pass..    def i
+00002380: 735f 7072 6f70 6572 7479 5f6f 7665 7272  s_property_overr
+00002390: 6964 6162 6c65 5f6c 6962 7261 7279 2873  idable_library(s
+000023a0: 656c 662c 2070 726f 7065 7274 7929 202d  elf, property) -
+000023b0: 3e20 626f 6f6c 3a0a 2020 2020 2020 2020  > bool:.        
+000023c0: 2727 2720 4368 6563 6b20 6966 2061 2070  ''' Check if a p
+000023d0: 726f 7065 7274 7920 6973 206f 7665 7272  roperty is overr
+000023e0: 6964 6162 6c65 2e0a 0a20 2020 2020 2020  idable...       
+000023f0: 203a 7274 7970 653a 2062 6f6f 6c0a 2020   :rtype: bool.  
+00002400: 2020 2020 2020 3a72 6574 7572 6e3a 2054        :return: T
+00002410: 7275 6520 7768 656e 2074 6865 2070 726f  rue when the pro
+00002420: 7065 7274 7920 6973 206f 7665 7272 6964  perty is overrid
+00002430: 6162 6c65 2e0a 2020 2020 2020 2020 2727  able..        ''
+00002440: 270a 2020 2020 2020 2020 7061 7373 0a0a  '.        pass..
+00002450: 2020 2020 6465 6620 6973 5f70 726f 7065      def is_prope
+00002460: 7274 795f 7265 6164 6f6e 6c79 2873 656c  rty_readonly(sel
+00002470: 662c 2070 726f 7065 7274 7929 202d 3e20  f, property) -> 
+00002480: 626f 6f6c 3a0a 2020 2020 2020 2020 2727  bool:.        ''
+00002490: 2720 4368 6563 6b20 6966 2061 2070 726f  ' Check if a pro
+000024a0: 7065 7274 7920 6973 2072 6561 646f 6e6c  perty is readonl
+000024b0: 792e 0a0a 2020 2020 2020 2020 3a72 7479  y...        :rty
+000024c0: 7065 3a20 626f 6f6c 0a20 2020 2020 2020  pe: bool.       
+000024d0: 203a 7265 7475 726e 3a20 5472 7565 2077   :return: True w
+000024e0: 6865 6e20 7468 6520 7072 6f70 6572 7479  hen the property
+000024f0: 2069 7320 7265 6164 6f6e 6c79 2028 6e6f   is readonly (no
+00002500: 7420 7772 6974 6162 6c65 292e 0a20 2020  t writable)..   
+00002510: 2020 2020 2027 2727 0a20 2020 2020 2020       '''.       
+00002520: 2070 6173 730a 0a20 2020 2064 6566 2069   pass..    def i
+00002530: 735f 7072 6f70 6572 7479 5f73 6574 2873  s_property_set(s
+00002540: 656c 662c 2070 726f 7065 7274 792c 0a20  elf, property,. 
+00002550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002560: 2020 2020 2020 2067 686f 7374 3a20 7479         ghost: ty
+00002570: 7069 6e67 2e4f 7074 696f 6e61 6c5b 626f  ping.Optional[bo
+00002580: 6f6c 5d20 3d20 5472 7565 2920 2d3e 2062  ol] = True) -> b
+00002590: 6f6f 6c3a 0a20 2020 2020 2020 2027 2727  ool:.        '''
+000025a0: 2043 6865 636b 2069 6620 6120 7072 6f70   Check if a prop
+000025b0: 6572 7479 2069 7320 7365 742c 2075 7365  erty is set, use
+000025c0: 2066 6f72 2074 6573 7469 6e67 206f 7065   for testing ope
+000025d0: 7261 746f 7220 7072 6f70 6572 7469 6573  rator properties
+000025e0: 2e0a 0a20 2020 2020 2020 203a 7061 7261  ...        :para
+000025f0: 6d20 6768 6f73 743a 2055 7365 6420 666f  m ghost: Used fo
+00002600: 7220 6f70 6572 6174 6f72 7320 7468 6174  r operators that
+00002610: 2072 652d 7275 6e20 7769 7468 2070 7265   re-run with pre
+00002620: 7669 6f75 7320 7365 7474 696e 6773 2e20  vious settings. 
+00002630: 496e 2074 6869 7320 6361 7365 2074 6865  In this case the
+00002640: 2070 726f 7065 7274 7920 6973 206e 6f74   property is not
+00002650: 206d 6172 6b65 6420 6173 2073 6574 2c20   marked as set, 
+00002660: 7965 7420 7468 6520 7661 6c75 6520 6672  yet the value fr
+00002670: 6f6d 2074 6865 2070 7265 7669 6f75 7320  om the previous 
+00002680: 6578 6563 7574 696f 6e20 6973 2075 7365  execution is use
+00002690: 642e 2049 6e20 7261 7265 2063 6173 6573  d. In rare cases
+000026a0: 2079 6f75 206d 6179 2077 616e 7420 746f   you may want to
+000026b0: 2073 6574 2074 6869 7320 6f70 7469 6f6e   set this option
+000026c0: 2074 6f20 6661 6c73 652e 0a20 2020 2020   to false..     
+000026d0: 2020 203a 7479 7065 2067 686f 7374 3a20     :type ghost: 
+000026e0: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
+000026f0: 626f 6f6c 5d0a 2020 2020 2020 2020 3a72  bool].        :r
+00002700: 7479 7065 3a20 626f 6f6c 0a20 2020 2020  type: bool.     
+00002710: 2020 203a 7265 7475 726e 3a20 5472 7565     :return: True
+00002720: 2077 6865 6e20 7468 6520 7072 6f70 6572   when the proper
+00002730: 7479 2068 6173 2062 6565 6e20 7365 742e  ty has been set.
+00002740: 0a20 2020 2020 2020 2027 2727 0a20 2020  .        '''.   
+00002750: 2020 2020 2070 6173 730a 0a20 2020 2064       pass..    d
+00002760: 6566 2069 7465 6d73 2873 656c 6629 202d  ef items(self) -
+00002770: 3e20 7479 7069 6e67 2e41 6e79 3a0a 2020  > typing.Any:.  
+00002780: 2020 2020 2020 2727 2720 5265 7475 726e        ''' Return
+00002790: 7320 7468 6520 6974 656d 7320 6f66 2074  s the items of t
+000027a0: 6869 7320 6f62 6a65 6374 7320 6375 7374  his objects cust
+000027b0: 6f6d 2070 726f 7065 7274 6965 7320 286d  om properties (m
+000027c0: 6174 6368 6573 2050 7974 686f 6e27 7320  atches Python's 
+000027d0: 6469 6374 696f 6e61 7279 2066 756e 6374  dictionary funct
+000027e0: 696f 6e20 6f66 2074 6865 2073 616d 6520  ion of the same 
+000027f0: 6e61 6d65 292e 0a0a 2020 2020 2020 2020  name)...        
+00002800: 3a72 7479 7065 3a20 7479 7069 6e67 2e41  :rtype: typing.A
+00002810: 6e79 0a20 2020 2020 2020 203a 7265 7475  ny.        :retu
+00002820: 726e 3a20 6375 7374 6f6d 2070 726f 7065  rn: custom prope
+00002830: 7274 7920 6b65 792c 2076 616c 7565 2070  rty key, value p
+00002840: 6169 7273 2e0a 2020 2020 2020 2020 2727  airs..        ''
+00002850: 270a 2020 2020 2020 2020 7061 7373 0a0a  '.        pass..
+00002860: 2020 2020 6465 6620 6b65 7966 7261 6d65      def keyframe
+00002870: 5f64 656c 6574 6528 0a20 2020 2020 2020  _delete(.       
+00002880: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
+00002890: 2020 2020 2020 2064 6174 615f 7061 7468         data_path
+000028a0: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
+000028b0: 6c5b 7374 725d 2c0a 2020 2020 2020 2020  l[str],.        
+000028c0: 2020 2020 696e 6465 783a 2074 7970 696e      index: typin
+000028d0: 672e 4f70 7469 6f6e 616c 5b69 6e74 5d20  g.Optional[int] 
+000028e0: 3d20 2d31 2c0a 2020 2020 2020 2020 2020  = -1,.          
+000028f0: 2020 6672 616d 653a 2074 7970 696e 672e    frame: typing.
+00002900: 4f70 7469 6f6e 616c 5b66 6c6f 6174 5d20  Optional[float] 
+00002910: 3d20 2762 7079 2e63 6f6e 7465 7874 2e73  = 'bpy.context.s
+00002920: 6365 6e65 2e66 7261 6d65 5f63 7572 7265  cene.frame_curre
+00002930: 6e74 272c 0a20 2020 2020 2020 2020 2020  nt',.           
+00002940: 2067 726f 7570 3a20 7479 7069 6e67 2e4f   group: typing.O
+00002950: 7074 696f 6e61 6c5b 7374 725d 203d 2022  ptional[str] = "
+00002960: 2229 202d 3e20 626f 6f6c 3a0a 2020 2020  ") -> bool:.    
+00002970: 2020 2020 2727 2720 5265 6d6f 7665 2061      ''' Remove a
+00002980: 206b 6579 6672 616d 6520 6672 6f6d 2074   keyframe from t
+00002990: 6869 7320 7072 6f70 6572 7469 6573 2066  his properties f
+000029a0: 6375 7276 652e 0a0a 2020 2020 2020 2020  curve...        
+000029b0: 3a70 6172 616d 2064 6174 615f 7061 7468  :param data_path
+000029c0: 3a20 7061 7468 2074 6f20 7468 6520 7072  : path to the pr
+000029d0: 6f70 6572 7479 2074 6f20 7265 6d6f 7665  operty to remove
+000029e0: 2061 206b 6579 2c20 616e 616c 6f67 6f75   a key, analogou
+000029f0: 7320 746f 2074 6865 2066 6375 7276 6527  s to the fcurve'
+00002a00: 7320 6461 7461 2070 6174 682e 0a20 2020  s data path..   
+00002a10: 2020 2020 203a 7479 7065 2064 6174 615f       :type data_
+00002a20: 7061 7468 3a20 7479 7069 6e67 2e4f 7074  path: typing.Opt
+00002a30: 696f 6e61 6c5b 7374 725d 0a20 2020 2020  ional[str].     
+00002a40: 2020 203a 7061 7261 6d20 696e 6465 783a     :param index:
+00002a50: 2061 7272 6179 2069 6e64 6578 206f 6620   array index of 
+00002a60: 7468 6520 7072 6f70 6572 7479 2074 6f20  the property to 
+00002a70: 7265 6d6f 7665 2061 206b 6579 2e20 4465  remove a key. De
+00002a80: 6661 756c 7473 2074 6f20 2d31 2072 656d  faults to -1 rem
+00002a90: 6f76 696e 6720 616c 6c20 696e 6469 6365  oving all indice
+00002aa0: 7320 6f72 2061 2073 696e 676c 6520 6368  s or a single ch
+00002ab0: 616e 6e65 6c20 6966 2074 6865 2070 726f  annel if the pro
+00002ac0: 7065 7274 7920 6973 206e 6f74 2061 6e20  perty is not an 
+00002ad0: 6172 7261 792e 0a20 2020 2020 2020 203a  array..        :
+00002ae0: 7479 7065 2069 6e64 6578 3a20 7479 7069  type index: typi
+00002af0: 6e67 2e4f 7074 696f 6e61 6c5b 696e 745d  ng.Optional[int]
+00002b00: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+00002b10: 6672 616d 653a 2054 6865 2066 7261 6d65  frame: The frame
+00002b20: 206f 6e20 7768 6963 6820 7468 6520 6b65   on which the ke
+00002b30: 7966 7261 6d65 2069 7320 6465 6c65 7465  yframe is delete
+00002b40: 642c 2064 6566 6175 6c74 696e 6720 746f  d, defaulting to
+00002b50: 2074 6865 2063 7572 7265 6e74 2066 7261   the current fra
+00002b60: 6d65 2e0a 2020 2020 2020 2020 3a74 7970  me..        :typ
+00002b70: 6520 6672 616d 653a 2074 7970 696e 672e  e frame: typing.
+00002b80: 4f70 7469 6f6e 616c 5b66 6c6f 6174 5d0a  Optional[float].
+00002b90: 2020 2020 2020 2020 3a70 6172 616d 2067          :param g
+00002ba0: 726f 7570 3a20 5468 6520 6e61 6d65 206f  roup: The name o
+00002bb0: 6620 7468 6520 6772 6f75 7020 7468 6520  f the group the 
+00002bc0: 462d 4375 7276 6520 7368 6f75 6c64 2062  F-Curve should b
+00002bd0: 6520 6164 6465 6420 746f 2069 6620 6974  e added to if it
+00002be0: 2064 6f65 736e 2774 2065 7869 7374 2079   doesn't exist y
+00002bf0: 6574 2e0a 2020 2020 2020 2020 3a74 7970  et..        :typ
+00002c00: 6520 6772 6f75 703a 2074 7970 696e 672e  e group: typing.
+00002c10: 4f70 7469 6f6e 616c 5b73 7472 5d0a 2020  Optional[str].  
+00002c20: 2020 2020 2020 3a72 7479 7065 3a20 626f        :rtype: bo
+00002c30: 6f6c 0a20 2020 2020 2020 203a 7265 7475  ol.        :retu
+00002c40: 726e 3a20 5375 6363 6573 7320 6f66 206b  rn: Success of k
+00002c50: 6579 6672 616d 6520 6465 6c65 7469 6f6e  eyframe deletion
+00002c60: 2e0a 2020 2020 2020 2020 2727 270a 2020  ..        '''.  
+00002c70: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
+00002c80: 6465 6620 6b65 7966 7261 6d65 5f69 6e73  def keyframe_ins
+00002c90: 6572 7428 0a20 2020 2020 2020 2020 2020  ert(.           
+00002ca0: 2073 656c 662c 0a20 2020 2020 2020 2020   self,.         
+00002cb0: 2020 2064 6174 615f 7061 7468 3a20 7479     data_path: ty
+00002cc0: 7069 6e67 2e4f 7074 696f 6e61 6c5b 7374  ping.Optional[st
+00002cd0: 725d 2c0a 2020 2020 2020 2020 2020 2020  r],.            
+00002ce0: 696e 6465 783a 2074 7970 696e 672e 4f70  index: typing.Op
+00002cf0: 7469 6f6e 616c 5b69 6e74 5d20 3d20 2d31  tional[int] = -1
+00002d00: 2c0a 2020 2020 2020 2020 2020 2020 6672  ,.            fr
+00002d10: 616d 653a 2074 7970 696e 672e 4f70 7469  ame: typing.Opti
+00002d20: 6f6e 616c 5b66 6c6f 6174 5d20 3d20 2762  onal[float] = 'b
+00002d30: 7079 2e63 6f6e 7465 7874 2e73 6365 6e65  py.context.scene
+00002d40: 2e66 7261 6d65 5f63 7572 7265 6e74 272c  .frame_current',
+00002d50: 0a20 2020 2020 2020 2020 2020 2067 726f  .            gro
+00002d60: 7570 3a20 7479 7069 6e67 2e4f 7074 696f  up: typing.Optio
+00002d70: 6e61 6c5b 7374 725d 203d 2022 222c 0a20  nal[str] = "",. 
+00002d80: 2020 2020 2020 2020 2020 206f 7074 696f             optio
+00002d90: 6e73 3a20 7479 7069 6e67 2e4f 7074 696f  ns: typing.Optio
+00002da0: 6e61 6c5b 7479 7069 6e67 2e41 6e79 5d20  nal[typing.Any] 
+00002db0: 3d20 2773 6574 2829 2729 202d 3e20 626f  = 'set()') -> bo
+00002dc0: 6f6c 3a0a 2020 2020 2020 2020 2727 2720  ol:.        ''' 
+00002dd0: 496e 7365 7274 2061 206b 6579 6672 616d  Insert a keyfram
+00002de0: 6520 6f6e 2074 6865 2070 726f 7065 7274  e on the propert
+00002df0: 7920 6769 7665 6e2c 2061 6464 696e 6720  y given, adding 
+00002e00: 6663 7572 7665 7320 616e 6420 616e 696d  fcurves and anim
+00002e10: 6174 696f 6e20 6461 7461 2077 6865 6e20  ation data when 
+00002e20: 6e65 6365 7373 6172 792e 2054 6869 7320  necessary. This 
+00002e30: 6973 2074 6865 206d 6f73 7420 7369 6d70  is the most simp
+00002e40: 6c65 2065 7861 6d70 6c65 206f 6620 696e  le example of in
+00002e50: 7365 7274 696e 6720 6120 6b65 7966 7261  serting a keyfra
+00002e60: 6d65 2066 726f 6d20 7079 7468 6f6e 2e20  me from python. 
+00002e70: 4e6f 7465 2074 6861 7420 7768 656e 206b  Note that when k
+00002e80: 6579 696e 6720 6461 7461 2070 6174 6873  eying data paths
+00002e90: 2077 6869 6368 2063 6f6e 7461 696e 206e   which contain n
+00002ea0: 6573 7465 6420 7072 6f70 6572 7469 6573  ested properties
+00002eb0: 2074 6869 7320 6d75 7374 2062 6520 646f   this must be do
+00002ec0: 6e65 2066 726f 6d20 7468 6520 6049 4460  ne from the `ID`
+00002ed0: 2073 7562 636c 6173 732c 2069 6e20 7468   subclass, in th
+00002ee0: 6973 2063 6173 6520 7468 6520 6041 726d  is case the `Arm
+00002ef0: 6174 7572 6560 2072 6174 6865 7220 7468  ature` rather th
+00002f00: 616e 2074 6865 2062 6f6e 652e 0a0a 2020  an the bone...  
+00002f10: 2020 2020 2020 3a70 6172 616d 2064 6174        :param dat
+00002f20: 615f 7061 7468 3a20 7061 7468 2074 6f20  a_path: path to 
+00002f30: 7468 6520 7072 6f70 6572 7479 2074 6f20  the property to 
+00002f40: 6b65 792c 2061 6e61 6c6f 676f 7573 2074  key, analogous t
+00002f50: 6f20 7468 6520 6663 7572 7665 2773 2064  o the fcurve's d
+00002f60: 6174 6120 7061 7468 2e0a 2020 2020 2020  ata path..      
+00002f70: 2020 3a74 7970 6520 6461 7461 5f70 6174    :type data_pat
+00002f80: 683a 2074 7970 696e 672e 4f70 7469 6f6e  h: typing.Option
+00002f90: 616c 5b73 7472 5d0a 2020 2020 2020 2020  al[str].        
+00002fa0: 3a70 6172 616d 2069 6e64 6578 3a20 6172  :param index: ar
+00002fb0: 7261 7920 696e 6465 7820 6f66 2074 6865  ray index of the
+00002fc0: 2070 726f 7065 7274 7920 746f 206b 6579   property to key
+00002fd0: 2e20 4465 6661 756c 7473 2074 6f20 2d31  . Defaults to -1
+00002fe0: 2077 6869 6368 2077 696c 6c20 6b65 7920   which will key 
+00002ff0: 616c 6c20 696e 6469 6365 7320 6f72 2061  all indices or a
+00003000: 2073 696e 676c 6520 6368 616e 6e65 6c20   single channel 
+00003010: 6966 2074 6865 2070 726f 7065 7274 7920  if the property 
+00003020: 6973 206e 6f74 2061 6e20 6172 7261 792e  is not an array.
+00003030: 0a20 2020 2020 2020 203a 7479 7065 2069  .        :type i
+00003040: 6e64 6578 3a20 7479 7069 6e67 2e4f 7074  ndex: typing.Opt
+00003050: 696f 6e61 6c5b 696e 745d 0a20 2020 2020  ional[int].     
+00003060: 2020 203a 7061 7261 6d20 6672 616d 653a     :param frame:
+00003070: 2054 6865 2066 7261 6d65 206f 6e20 7768   The frame on wh
+00003080: 6963 6820 7468 6520 6b65 7966 7261 6d65  ich the keyframe
+00003090: 2069 7320 696e 7365 7274 6564 2c20 6465   is inserted, de
+000030a0: 6661 756c 7469 6e67 2074 6f20 7468 6520  faulting to the 
+000030b0: 6375 7272 656e 7420 6672 616d 652e 0a20  current frame.. 
+000030c0: 2020 2020 2020 203a 7479 7065 2066 7261         :type fra
+000030d0: 6d65 3a20 7479 7069 6e67 2e4f 7074 696f  me: typing.Optio
+000030e0: 6e61 6c5b 666c 6f61 745d 0a20 2020 2020  nal[float].     
+000030f0: 2020 203a 7061 7261 6d20 6772 6f75 703a     :param group:
+00003100: 2054 6865 206e 616d 6520 6f66 2074 6865   The name of the
+00003110: 2067 726f 7570 2074 6865 2046 2d43 7572   group the F-Cur
+00003120: 7665 2073 686f 756c 6420 6265 2061 6464  ve should be add
+00003130: 6564 2074 6f20 6966 2069 7420 646f 6573  ed to if it does
+00003140: 6e27 7420 6578 6973 7420 7965 742e 0a20  n't exist yet.. 
+00003150: 2020 2020 2020 203a 7479 7065 2067 726f         :type gro
+00003160: 7570 3a20 7479 7069 6e67 2e4f 7074 696f  up: typing.Optio
+00003170: 6e61 6c5b 7374 725d 0a20 2020 2020 2020  nal[str].       
+00003180: 203a 7061 7261 6d20 666c 6167 3a20 0a20   :param flag: . 
+00003190: 2020 2020 2020 203a 7479 7065 2066 6c61         :type fla
+000031a0: 673a 2074 7970 696e 672e 4f70 7469 6f6e  g: typing.Option
+000031b0: 616c 5b74 7970 696e 672e 5365 745d 0a20  al[typing.Set]. 
+000031c0: 2020 2020 2020 203a 7061 7261 6d20 6f70         :param op
+000031d0: 7469 6f6e 733a 2020 2d20 6060 494e 5345  tions:  - ``INSE
+000031e0: 5254 4b45 595f 4e45 4544 4544 6060 204f  RTKEY_NEEDED`` O
+000031f0: 6e6c 7920 696e 7365 7274 206b 6579 6672  nly insert keyfr
+00003200: 616d 6573 2077 6865 7265 2074 6865 7927  ames where they'
+00003210: 7265 206e 6565 6465 6420 696e 2074 6865  re needed in the
+00003220: 2072 656c 6576 616e 7420 462d 4375 7276   relevant F-Curv
+00003230: 6573 2e20 2d20 6060 494e 5345 5254 4b45  es. - ``INSERTKE
+00003240: 595f 5649 5355 414c 6060 2049 6e73 6572  Y_VISUAL`` Inser
+00003250: 7420 6b65 7966 7261 6d65 7320 6261 7365  t keyframes base
+00003260: 6420 6f6e 2027 7669 7375 616c 2074 7261  d on 'visual tra
+00003270: 6e73 666f 726d 7327 2e20 2d20 6060 494e  nsforms'. - ``IN
+00003280: 5345 5254 4b45 595f 5859 5a5f 544f 5f52  SERTKEY_XYZ_TO_R
+00003290: 4742 6060 2043 6f6c 6f72 2066 6f72 206e  GB`` Color for n
+000032a0: 6577 6c79 2061 6464 6564 2074 7261 6e73  ewly added trans
+000032b0: 666f 726d 6174 696f 6e20 462d 4375 7276  formation F-Curv
+000032c0: 6573 2028 4c6f 6361 7469 6f6e 2c20 526f  es (Location, Ro
+000032d0: 7461 7469 6f6e 2c20 5363 616c 6529 2069  tation, Scale) i
+000032e0: 7320 6261 7365 6420 6f6e 2074 6865 2074  s based on the t
+000032f0: 7261 6e73 666f 726d 2061 7869 732e 202d  ransform axis. -
+00003300: 2060 6049 4e53 4552 544b 4559 5f52 4550   ``INSERTKEY_REP
+00003310: 4c41 4345 6060 204f 6e6c 7920 7265 706c  LACE`` Only repl
+00003320: 6163 6520 616c 7265 6164 7920 6578 6973  ace already exis
+00003330: 7469 6e67 206b 6579 6672 616d 6573 2e20  ting keyframes. 
+00003340: 2d20 6060 494e 5345 5254 4b45 595f 4156  - ``INSERTKEY_AV
+00003350: 4149 4c41 424c 4560 6020 4f6e 6c79 2069  AILABLE`` Only i
+00003360: 6e73 6572 7420 696e 746f 2061 6c72 6561  nsert into alrea
+00003370: 6479 2065 7869 7374 696e 6720 462d 4375  dy existing F-Cu
+00003380: 7276 6573 2e20 2d20 6060 494e 5345 5254  rves. - ``INSERT
+00003390: 4b45 595f 4359 434c 455f 4157 4152 4560  KEY_CYCLE_AWARE`
+000033a0: 6020 5461 6b65 2063 7963 6c69 6320 6578  ` Take cyclic ex
+000033b0: 7472 6170 6f6c 6174 696f 6e20 696e 746f  trapolation into
+000033c0: 2061 6363 6f75 6e74 2028 4379 636c 652d   account (Cycle-
+000033d0: 4177 6172 6520 4b65 7969 6e67 206f 7074  Aware Keying opt
+000033e0: 696f 6e29 2e0a 2020 2020 2020 2020 3a74  ion)..        :t
+000033f0: 7970 6520 6f70 7469 6f6e 733a 2074 7970  ype options: typ
+00003400: 696e 672e 4f70 7469 6f6e 616c 5b74 7970  ing.Optional[typ
+00003410: 696e 672e 416e 795d 0a20 2020 2020 2020  ing.Any].       
+00003420: 203a 7274 7970 653a 2062 6f6f 6c0a 2020   :rtype: bool.  
+00003430: 2020 2020 2020 3a72 6574 7572 6e3a 2053        :return: S
+00003440: 7563 6365 7373 206f 6620 6b65 7966 7261  uccess of keyfra
+00003450: 6d65 2069 6e73 6572 7469 6f6e 2e0a 2020  me insertion..  
+00003460: 2020 2020 2020 2727 270a 2020 2020 2020        '''.      
+00003470: 2020 7061 7373 0a0a 2020 2020 6465 6620    pass..    def 
+00003480: 6b65 7973 2873 656c 6629 202d 3e20 7479  keys(self) -> ty
+00003490: 7069 6e67 2e41 6e79 3a0a 2020 2020 2020  ping.Any:.      
+000034a0: 2020 2727 2720 5265 7475 726e 7320 7468    ''' Returns th
+000034b0: 6520 6b65 7973 206f 6620 7468 6973 206f  e keys of this o
+000034c0: 626a 6563 7473 2063 7573 746f 6d20 7072  bjects custom pr
+000034d0: 6f70 6572 7469 6573 2028 6d61 7463 6865  operties (matche
+000034e0: 7320 5079 7468 6f6e 2773 2064 6963 7469  s Python's dicti
+000034f0: 6f6e 6172 7920 6675 6e63 7469 6f6e 206f  onary function o
+00003500: 6620 7468 6520 7361 6d65 206e 616d 6529  f the same name)
+00003510: 2e0a 0a20 2020 2020 2020 203a 7274 7970  ...        :rtyp
+00003520: 653a 2074 7970 696e 672e 416e 790a 2020  e: typing.Any.  
+00003530: 2020 2020 2020 3a72 6574 7572 6e3a 2063        :return: c
+00003540: 7573 746f 6d20 7072 6f70 6572 7479 206b  ustom property k
+00003550: 6579 732e 0a20 2020 2020 2020 2027 2727  eys..        '''
+00003560: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
+00003570: 2020 2064 6566 2070 6174 685f 6672 6f6d     def path_from
+00003580: 5f69 6428 7365 6c66 2c20 7072 6f70 6572  _id(self, proper
+00003590: 7479 3a20 7479 7069 6e67 2e4f 7074 696f  ty: typing.Optio
+000035a0: 6e61 6c5b 7374 725d 203d 2022 2229 202d  nal[str] = "") -
+000035b0: 3e20 7374 723a 0a20 2020 2020 2020 2027  > str:.        '
+000035c0: 2727 2052 6574 7572 6e73 2074 6865 2064  '' Returns the d
+000035d0: 6174 6120 7061 7468 2066 726f 6d20 7468  ata path from th
+000035e0: 6520 4944 2074 6f20 7468 6973 206f 626a  e ID to this obj
+000035f0: 6563 7420 2873 7472 696e 6729 2e0a 0a20  ect (string)... 
+00003600: 2020 2020 2020 203a 7061 7261 6d20 7072         :param pr
+00003610: 6f70 6572 7479 3a20 4f70 7469 6f6e 616c  operty: Optional
+00003620: 2070 726f 7065 7274 7920 6e61 6d65 2077   property name w
+00003630: 6869 6368 2063 616e 2062 6520 7573 6564  hich can be used
+00003640: 2069 6620 7468 6520 7061 7468 2069 7320   if the path is 
+00003650: 746f 2061 2070 726f 7065 7274 7920 6f66  to a property of
+00003660: 2074 6869 7320 6f62 6a65 6374 2e0a 2020   this object..  
+00003670: 2020 2020 2020 3a74 7970 6520 7072 6f70        :type prop
+00003680: 6572 7479 3a20 7479 7069 6e67 2e4f 7074  erty: typing.Opt
+00003690: 696f 6e61 6c5b 7374 725d 0a20 2020 2020  ional[str].     
+000036a0: 2020 203a 7274 7970 653a 2073 7472 0a20     :rtype: str. 
+000036b0: 2020 2020 2020 203a 7265 7475 726e 3a20         :return: 
+000036c0: 6062 7079 2e74 7970 6573 2e62 7079 5f73  `bpy.types.bpy_s
+000036d0: 7472 7563 742e 6964 5f64 6174 6160 2074  truct.id_data` t
+000036e0: 6f20 7468 6973 2073 7472 7563 7420 616e  o this struct an
+000036f0: 6420 7072 6f70 6572 7479 2028 7768 656e  d property (when
+00003700: 2067 6976 656e 292e 0a20 2020 2020 2020   given)..       
+00003710: 2027 2727 0a20 2020 2020 2020 2070 6173   '''.        pas
+00003720: 730a 0a20 2020 2064 6566 2070 6174 685f  s..    def path_
+00003730: 7265 736f 6c76 6528 7365 6c66 2c0a 2020  resolve(self,.  
+00003740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003750: 2020 2070 6174 683a 2074 7970 696e 672e     path: typing.
+00003760: 4f70 7469 6f6e 616c 5b73 7472 5d2c 0a20  Optional[str],. 
+00003770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003780: 2020 2020 636f 6572 6365 3a20 7479 7069      coerce: typi
+00003790: 6e67 2e4f 7074 696f 6e61 6c5b 626f 6f6c  ng.Optional[bool
+000037a0: 5d20 3d20 5472 7565 293a 0a20 2020 2020  ] = True):.     
+000037b0: 2020 2027 2727 2052 6574 7572 6e73 2074     ''' Returns t
+000037c0: 6865 2070 726f 7065 7274 7920 6672 6f6d  he property from
+000037d0: 2074 6865 2070 6174 682c 2072 6169 7365   the path, raise
+000037e0: 2061 6e20 6578 6365 7074 696f 6e20 7768   an exception wh
+000037f0: 656e 206e 6f74 2066 6f75 6e64 2e0a 0a20  en not found... 
+00003800: 2020 2020 2020 203a 7061 7261 6d20 7061         :param pa
+00003810: 7468 3a20 7061 7468 2077 6869 6368 2074  th: path which t
+00003820: 6869 7320 7072 6f70 6572 7479 2072 6573  his property res
+00003830: 6f6c 7665 732e 0a20 2020 2020 2020 203a  olves..        :
+00003840: 7479 7065 2070 6174 683a 2074 7970 696e  type path: typin
+00003850: 672e 4f70 7469 6f6e 616c 5b73 7472 5d0a  g.Optional[str].
+00003860: 2020 2020 2020 2020 3a70 6172 616d 2063          :param c
+00003870: 6f65 7263 653a 206f 7074 696f 6e61 6c20  oerce: optional 
+00003880: 6172 6775 6d65 6e74 2c20 7768 656e 2054  argument, when T
+00003890: 7275 652c 2074 6865 2070 726f 7065 7274  rue, the propert
+000038a0: 7920 7769 6c6c 2062 6520 636f 6e76 6572  y will be conver
+000038b0: 7465 6420 696e 746f 2069 7473 2050 7974  ted into its Pyt
+000038c0: 686f 6e20 7265 7072 6573 656e 7461 7469  hon representati
+000038d0: 6f6e 2e0a 2020 2020 2020 2020 3a74 7970  on..        :typ
+000038e0: 6520 636f 6572 6365 3a20 7479 7069 6e67  e coerce: typing
+000038f0: 2e4f 7074 696f 6e61 6c5b 626f 6f6c 5d0a  .Optional[bool].
+00003900: 2020 2020 2020 2020 2727 270a 2020 2020          '''.    
+00003910: 2020 2020 7061 7373 0a0a 2020 2020 6465      pass..    de
+00003920: 6620 706f 7028 7365 6c66 2c0a 2020 2020  f pop(self,.    
+00003930: 2020 2020 2020 2020 6b65 793a 2074 7970          key: typ
+00003940: 696e 672e 4f70 7469 6f6e 616c 5b73 7472  ing.Optional[str
+00003950: 5d2c 0a20 2020 2020 2020 2020 2020 2064  ],.            d
+00003960: 6566 6175 6c74 3a20 7479 7069 6e67 2e4f  efault: typing.O
+00003970: 7074 696f 6e61 6c5b 7479 7069 6e67 2e41  ptional[typing.A
+00003980: 6e79 5d20 3d20 4e6f 6e65 293a 0a20 2020  ny] = None):.   
+00003990: 2020 2020 2027 2727 2052 656d 6f76 6520       ''' Remove 
+000039a0: 616e 6420 7265 7475 726e 2074 6865 2076  and return the v
+000039b0: 616c 7565 206f 6620 7468 6520 6375 7374  alue of the cust
+000039c0: 6f6d 2070 726f 7065 7274 7920 6173 7369  om property assi
+000039d0: 676e 6564 2074 6f20 6b65 7920 6f72 2064  gned to key or d
+000039e0: 6566 6175 6c74 2077 6865 6e20 6e6f 7420  efault when not 
+000039f0: 666f 756e 6420 286d 6174 6368 6573 2050  found (matches P
+00003a00: 7974 686f 6e27 7320 6469 6374 696f 6e61  ython's dictiona
+00003a10: 7279 2066 756e 6374 696f 6e20 6f66 2074  ry function of t
+00003a20: 6865 2073 616d 6520 6e61 6d65 292e 0a0a  he same name)...
+00003a30: 2020 2020 2020 2020 3a70 6172 616d 206b          :param k
+00003a40: 6579 3a20 5468 6520 6b65 7920 6173 736f  ey: The key asso
+00003a50: 6369 6174 6564 2077 6974 6820 7468 6520  ciated with the 
+00003a60: 6375 7374 6f6d 2070 726f 7065 7274 792e  custom property.
+00003a70: 0a20 2020 2020 2020 203a 7479 7065 206b  .        :type k
+00003a80: 6579 3a20 7479 7069 6e67 2e4f 7074 696f  ey: typing.Optio
+00003a90: 6e61 6c5b 7374 725d 0a20 2020 2020 2020  nal[str].       
+00003aa0: 203a 7061 7261 6d20 6465 6661 756c 743a   :param default:
+00003ab0: 204f 7074 696f 6e61 6c20 6172 6775 6d65   Optional argume
+00003ac0: 6e74 2066 6f72 2074 6865 2076 616c 7565  nt for the value
+00003ad0: 2074 6f20 7265 7475 726e 2069 6620 2a6b   to return if *k
+00003ae0: 6579 2a20 6973 206e 6f74 2066 6f75 6e64  ey* is not found
+00003af0: 2e0a 2020 2020 2020 2020 3a74 7970 6520  ..        :type 
+00003b00: 6465 6661 756c 743a 2074 7970 696e 672e  default: typing.
+00003b10: 4f70 7469 6f6e 616c 5b74 7970 696e 672e  Optional[typing.
+00003b20: 416e 795d 0a20 2020 2020 2020 2027 2727  Any].        '''
+00003b30: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
+00003b40: 2020 2064 6566 2070 726f 7065 7274 795f     def property_
+00003b50: 6f76 6572 7269 6461 626c 655f 6c69 6272  overridable_libr
+00003b60: 6172 795f 7365 7428 7365 6c66 2c20 7072  ary_set(self, pr
+00003b70: 6f70 6572 7479 2c20 6f76 6572 7269 6461  operty, overrida
+00003b80: 626c 6529 202d 3e20 626f 6f6c 3a0a 2020  ble) -> bool:.  
+00003b90: 2020 2020 2020 2727 2720 4465 6669 6e65        ''' Define
+00003ba0: 2061 2070 726f 7065 7274 7920 6173 206f   a property as o
+00003bb0: 7665 7272 6964 6162 6c65 206f 7220 6e6f  verridable or no
+00003bc0: 7420 286f 6e6c 7920 666f 7220 6375 7374  t (only for cust
+00003bd0: 6f6d 2070 726f 7065 7274 6965 7321 292e  om properties!).
+00003be0: 0a0a 2020 2020 2020 2020 3a72 7479 7065  ..        :rtype
+00003bf0: 3a20 626f 6f6c 0a20 2020 2020 2020 203a  : bool.        :
+00003c00: 7265 7475 726e 3a20 5472 7565 2077 6865  return: True whe
+00003c10: 6e20 7468 6520 6f76 6572 7269 6461 626c  n the overridabl
+00003c20: 6520 7374 6174 7573 206f 6620 7468 6520  e status of the 
+00003c30: 7072 6f70 6572 7479 2077 6173 2073 7563  property was suc
+00003c40: 6365 7373 6675 6c6c 7920 7365 742e 0a20  cessfully set.. 
+00003c50: 2020 2020 2020 2027 2727 0a20 2020 2020         '''.     
+00003c60: 2020 2070 6173 730a 0a20 2020 2064 6566     pass..    def
+00003c70: 2070 726f 7065 7274 795f 756e 7365 7428   property_unset(
+00003c80: 7365 6c66 2c20 7072 6f70 6572 7479 293a  self, property):
+00003c90: 0a20 2020 2020 2020 2027 2727 2055 6e73  .        ''' Uns
+00003ca0: 6574 2061 2070 726f 7065 7274 792c 2077  et a property, w
+00003cb0: 696c 6c20 7573 6520 6465 6661 756c 7420  ill use default 
+00003cc0: 7661 6c75 6520 6166 7465 7277 6172 642e  value afterward.
+00003cd0: 0a0a 2020 2020 2020 2020 2727 270a 2020  ..        '''.  
+00003ce0: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
+00003cf0: 6465 6620 7479 7065 5f72 6563 6173 7428  def type_recast(
+00003d00: 7365 6c66 2920 2d3e 2027 6270 795f 7374  self) -> 'bpy_st
+00003d10: 7275 6374 273a 0a20 2020 2020 2020 2027  ruct':.        '
+00003d20: 2727 2052 6574 7572 6e20 6120 6e65 7720  '' Return a new 
+00003d30: 696e 7374 616e 6365 2c20 7468 6973 2069  instance, this i
+00003d40: 7320 6e65 6564 6564 2062 6563 6175 7365  s needed because
+00003d50: 2074 7970 6573 2073 7563 6820 6173 2074   types such as t
+00003d60: 6578 7475 7265 7320 6361 6e20 6265 2063  extures can be c
+00003d70: 6861 6e67 6564 2061 7420 7275 6e74 696d  hanged at runtim
+00003d80: 652e 0a0a 2020 2020 2020 2020 3a72 7479  e...        :rty
+00003d90: 7065 3a20 2762 7079 5f73 7472 7563 7427  pe: 'bpy_struct'
+00003da0: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
+00003db0: 3a20 6120 6e65 7720 696e 7374 616e 6365  : a new instance
+00003dc0: 206f 6620 7468 6973 206f 626a 6563 7420   of this object 
+00003dd0: 7769 7468 2074 6865 2074 7970 6520 696e  with the type in
+00003de0: 6974 6961 6c69 7a65 6420 6167 6169 6e2e  itialized again.
+00003df0: 0a20 2020 2020 2020 2027 2727 0a20 2020  .        '''.   
+00003e00: 2020 2020 2070 6173 730a 0a20 2020 2064       pass..    d
+00003e10: 6566 2076 616c 7565 7328 7365 6c66 2920  ef values(self) 
+00003e20: 2d3e 2074 7970 696e 672e 416e 793a 0a20  -> typing.Any:. 
+00003e30: 2020 2020 2020 2027 2727 2052 6574 7572         ''' Retur
+00003e40: 6e73 2074 6865 2076 616c 7565 7320 6f66  ns the values of
+00003e50: 2074 6869 7320 6f62 6a65 6374 7320 6375   this objects cu
+00003e60: 7374 6f6d 2070 726f 7065 7274 6965 7320  stom properties 
+00003e70: 286d 6174 6368 6573 2050 7974 686f 6e27  (matches Python'
+00003e80: 7320 6469 6374 696f 6e61 7279 2066 756e  s dictionary fun
+00003e90: 6374 696f 6e20 6f66 2074 6865 2073 616d  ction of the sam
+00003ea0: 6520 6e61 6d65 292e 0a0a 2020 2020 2020  e name)...      
+00003eb0: 2020 3a72 7479 7065 3a20 7479 7069 6e67    :rtype: typing
+00003ec0: 2e41 6e79 0a20 2020 2020 2020 203a 7265  .Any.        :re
+00003ed0: 7475 726e 3a20 6375 7374 6f6d 2070 726f  turn: custom pro
+00003ee0: 7065 7274 7920 7661 6c75 6573 2e0a 2020  perty values..  
+00003ef0: 2020 2020 2020 2727 270a 2020 2020 2020        '''.      
+00003f00: 2020 7061 7373 0a0a 2020 2020 6465 6620    pass..    def 
+00003f10: 5f5f 6765 7469 7465 6d5f 5f28 7365 6c66  __getitem__(self
+00003f20: 2c20 6b65 793a 2074 7970 696e 672e 556e  , key: typing.Un
+00003f30: 696f 6e5b 696e 742c 2073 7472 5d29 202d  ion[int, str]) -
+00003f40: 3e20 2774 7970 696e 672e 416e 7927 3a0a  > 'typing.Any':.
+00003f50: 2020 2020 2020 2020 2727 2720 0a0a 2020          ''' ..  
+00003f60: 2020 2020 2020 3a70 6172 616d 206b 6579        :param key
+00003f70: 3a20 0a20 2020 2020 2020 203a 7479 7065  : .        :type
+00003f80: 206b 6579 3a20 7479 7069 6e67 2e55 6e69   key: typing.Uni
+00003f90: 6f6e 5b69 6e74 2c20 7374 725d 0a20 2020  on[int, str].   
+00003fa0: 2020 2020 203a 7274 7970 653a 2027 7479       :rtype: 'ty
+00003fb0: 7069 6e67 2e41 6e79 270a 2020 2020 2020  ping.Any'.      
+00003fc0: 2020 2727 270a 2020 2020 2020 2020 7061    '''.        pa
+00003fd0: 7373 0a0a 2020 2020 6465 6620 5f5f 7365  ss..    def __se
+00003fe0: 7469 7465 6d5f 5f28 7365 6c66 2c20 6b65  titem__(self, ke
+00003ff0: 793a 2074 7970 696e 672e 556e 696f 6e5b  y: typing.Union[
+00004000: 696e 742c 2073 7472 5d2c 2076 616c 7565  int, str], value
+00004010: 3a20 2774 7970 696e 672e 416e 7927 293a  : 'typing.Any'):
+00004020: 0a20 2020 2020 2020 2027 2727 200a 0a20  .        ''' .. 
+00004030: 2020 2020 2020 203a 7061 7261 6d20 6b65         :param ke
+00004040: 793a 200a 2020 2020 2020 2020 3a74 7970  y: .        :typ
+00004050: 6520 6b65 793a 2074 7970 696e 672e 556e  e key: typing.Un
+00004060: 696f 6e5b 696e 742c 2073 7472 5d0a 2020  ion[int, str].  
+00004070: 2020 2020 2020 3a70 6172 616d 2076 616c        :param val
+00004080: 7565 3a20 0a20 2020 2020 2020 203a 7479  ue: .        :ty
+00004090: 7065 2076 616c 7565 3a20 2774 7970 696e  pe value: 'typin
+000040a0: 672e 416e 7927 0a20 2020 2020 2020 2027  g.Any'.        '
+000040b0: 2727 0a20 2020 2020 2020 2070 6173 730a  ''.        pass.
+000040c0: 0a20 2020 2064 6566 205f 5f64 656c 6974  .    def __delit
+000040d0: 656d 5f5f 2873 656c 662c 206b 6579 3a20  em__(self, key: 
+000040e0: 7479 7069 6e67 2e55 6e69 6f6e 5b69 6e74  typing.Union[int
+000040f0: 2c20 7374 725d 2920 2d3e 2027 7479 7069  , str]) -> 'typi
+00004100: 6e67 2e41 6e79 273a 0a20 2020 2020 2020  ng.Any':.       
+00004110: 2027 2727 200a 0a20 2020 2020 2020 203a   ''' ..        :
+00004120: 7061 7261 6d20 6b65 793a 200a 2020 2020  param key: .    
+00004130: 2020 2020 3a74 7970 6520 6b65 793a 2074      :type key: t
+00004140: 7970 696e 672e 556e 696f 6e5b 696e 742c  yping.Union[int,
+00004150: 2073 7472 5d0a 2020 2020 2020 2020 3a72   str].        :r
+00004160: 7479 7065 3a20 2774 7970 696e 672e 416e  type: 'typing.An
+00004170: 7927 0a20 2020 2020 2020 2027 2727 0a20  y'.        '''. 
 00004180: 2020 2020 2020 2070 6173 730a 0a0a 636c         pass...cl
 00004190: 6173 7320 6270 795f 7072 6f70 5f61 7272  ass bpy_prop_arr
 000041a0: 6179 2874 7970 696e 672e 4765 6e65 7269  ay(typing.Generi
 000041b0: 635b 4765 6e65 7269 6354 7970 655d 293a  c[GenericType]):
 000041c0: 0a20 2020 2064 6566 2066 6f72 6561 6368  .    def foreach
 000041d0: 5f67 6574 2873 656c 662c 2061 7474 722c  _get(self, attr,
 000041e0: 2073 6571 293a 0a20 2020 2020 2020 2027   seq):.        '
@@ -216622,1638 +216622,1644 @@
 0034e2d0: 3d20 4e6f 6e65 0a0a 5649 4557 3344 5f4d  = None..VIEW3D_M
 0034e2e0: 545f 7365 6c65 6374 5f65 6469 745f 6770  T_select_edit_gp
 0034e2f0: 656e 6369 6c3a 2027 626c 5f75 692e 7370  encil: 'bl_ui.sp
 0034e300: 6163 655f 7669 6577 3364 2e56 4945 5733  ace_view3d.VIEW3
 0034e310: 445f 4d54 5f73 656c 6563 745f 6564 6974  D_MT_select_edit
 0034e320: 5f67 7065 6e63 696c 2720 3d20 4e6f 6e65  _gpencil' = None
 0034e330: 0a0a 5649 4557 3344 5f4d 545f 7365 6c65  ..VIEW3D_MT_sele
-0034e340: 6374 5f65 6469 745f 6c61 7474 6963 653a  ct_edit_lattice:
-0034e350: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
-0034e360: 6577 3364 2e56 4945 5733 445f 4d54 5f73  ew3d.VIEW3D_MT_s
-0034e370: 656c 6563 745f 6564 6974 5f6c 6174 7469  elect_edit_latti
-0034e380: 6365 2720 3d20 4e6f 6e65 0a0a 5649 4557  ce' = None..VIEW
-0034e390: 3344 5f4d 545f 7365 6c65 6374 5f65 6469  3D_MT_select_edi
-0034e3a0: 745f 6d65 7368 3a20 2762 6c5f 7569 2e73  t_mesh: 'bl_ui.s
-0034e3b0: 7061 6365 5f76 6965 7733 642e 5649 4557  pace_view3d.VIEW
-0034e3c0: 3344 5f4d 545f 7365 6c65 6374 5f65 6469  3D_MT_select_edi
-0034e3d0: 745f 6d65 7368 2720 3d20 4e6f 6e65 0a0a  t_mesh' = None..
-0034e3e0: 5649 4557 3344 5f4d 545f 7365 6c65 6374  VIEW3D_MT_select
-0034e3f0: 5f65 6469 745f 6d65 7461 6261 6c6c 3a20  _edit_metaball: 
-0034e400: 2762 6c5f 7569 2e73 7061 6365 5f76 6965  'bl_ui.space_vie
-0034e410: 7733 642e 5649 4557 3344 5f4d 545f 7365  w3d.VIEW3D_MT_se
-0034e420: 6c65 6374 5f65 6469 745f 6d65 7461 6261  lect_edit_metaba
-0034e430: 6c6c 2720 3d20 4e6f 6e65 0a0a 5649 4557  ll' = None..VIEW
-0034e440: 3344 5f4d 545f 7365 6c65 6374 5f65 6469  3D_MT_select_edi
-0034e450: 745f 7375 7266 6163 653a 2027 626c 5f75  t_surface: 'bl_u
-0034e460: 692e 7370 6163 655f 7669 6577 3364 2e56  i.space_view3d.V
-0034e470: 4945 5733 445f 4d54 5f73 656c 6563 745f  IEW3D_MT_select_
-0034e480: 6564 6974 5f73 7572 6661 6365 2720 3d20  edit_surface' = 
-0034e490: 4e6f 6e65 0a0a 5649 4557 3344 5f4d 545f  None..VIEW3D_MT_
-0034e4a0: 7365 6c65 6374 5f65 6469 745f 7465 7874  select_edit_text
-0034e4b0: 3a20 2762 6c5f 7569 2e73 7061 6365 5f76  : 'bl_ui.space_v
-0034e4c0: 6965 7733 642e 5649 4557 3344 5f4d 545f  iew3d.VIEW3D_MT_
-0034e4d0: 7365 6c65 6374 5f65 6469 745f 7465 7874  select_edit_text
-0034e4e0: 2720 3d20 4e6f 6e65 0a0a 5649 4557 3344  ' = None..VIEW3D
-0034e4f0: 5f4d 545f 7365 6c65 6374 5f6f 626a 6563  _MT_select_objec
-0034e500: 743a 2027 626c 5f75 692e 7370 6163 655f  t: 'bl_ui.space_
-0034e510: 7669 6577 3364 2e56 4945 5733 445f 4d54  view3d.VIEW3D_MT
-0034e520: 5f73 656c 6563 745f 6f62 6a65 6374 2720  _select_object' 
-0034e530: 3d20 4e6f 6e65 0a0a 5649 4557 3344 5f4d  = None..VIEW3D_M
-0034e540: 545f 7365 6c65 6374 5f6f 626a 6563 745f  T_select_object_
-0034e550: 6d6f 7265 5f6c 6573 733a 2027 626c 5f75  more_less: 'bl_u
-0034e560: 692e 7370 6163 655f 7669 6577 3364 2e56  i.space_view3d.V
-0034e570: 4945 5733 445f 4d54 5f73 656c 6563 745f  IEW3D_MT_select_
-0034e580: 6f62 6a65 6374 5f6d 6f72 655f 6c65 7373  object_more_less
-0034e590: 2720 3d20 4e6f 6e65 0a0a 5649 4557 3344  ' = None..VIEW3D
-0034e5a0: 5f4d 545f 7365 6c65 6374 5f70 6169 6e74  _MT_select_paint
-0034e5b0: 5f6d 6173 6b3a 2027 626c 5f75 692e 7370  _mask: 'bl_ui.sp
-0034e5c0: 6163 655f 7669 6577 3364 2e56 4945 5733  ace_view3d.VIEW3
-0034e5d0: 445f 4d54 5f73 656c 6563 745f 7061 696e  D_MT_select_pain
-0034e5e0: 745f 6d61 736b 2720 3d20 4e6f 6e65 0a0a  t_mask' = None..
-0034e5f0: 5649 4557 3344 5f4d 545f 7365 6c65 6374  VIEW3D_MT_select
-0034e600: 5f70 6169 6e74 5f6d 6173 6b5f 7665 7274  _paint_mask_vert
-0034e610: 6578 3a20 2762 6c5f 7569 2e73 7061 6365  ex: 'bl_ui.space
-0034e620: 5f76 6965 7733 642e 5649 4557 3344 5f4d  _view3d.VIEW3D_M
-0034e630: 545f 7365 6c65 6374 5f70 6169 6e74 5f6d  T_select_paint_m
-0034e640: 6173 6b5f 7665 7274 6578 2720 3d20 4e6f  ask_vertex' = No
-0034e650: 6e65 0a0a 5649 4557 3344 5f4d 545f 7365  ne..VIEW3D_MT_se
-0034e660: 6c65 6374 5f70 6172 7469 636c 653a 2027  lect_particle: '
-0034e670: 626c 5f75 692e 7370 6163 655f 7669 6577  bl_ui.space_view
-0034e680: 3364 2e56 4945 5733 445f 4d54 5f73 656c  3d.VIEW3D_MT_sel
-0034e690: 6563 745f 7061 7274 6963 6c65 2720 3d20  ect_particle' = 
-0034e6a0: 4e6f 6e65 0a0a 5649 4557 3344 5f4d 545f  None..VIEW3D_MT_
-0034e6b0: 7365 6c65 6374 5f70 6f73 653a 2027 626c  select_pose: 'bl
-0034e6c0: 5f75 692e 7370 6163 655f 7669 6577 3364  _ui.space_view3d
-0034e6d0: 2e56 4945 5733 445f 4d54 5f73 656c 6563  .VIEW3D_MT_selec
-0034e6e0: 745f 706f 7365 2720 3d20 4e6f 6e65 0a0a  t_pose' = None..
-0034e6f0: 5649 4557 3344 5f4d 545f 7365 6c65 6374  VIEW3D_MT_select
-0034e700: 5f70 6f73 655f 6d6f 7265 5f6c 6573 733a  _pose_more_less:
-0034e710: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
-0034e720: 6577 3364 2e56 4945 5733 445f 4d54 5f73  ew3d.VIEW3D_MT_s
-0034e730: 656c 6563 745f 706f 7365 5f6d 6f72 655f  elect_pose_more_
-0034e740: 6c65 7373 2720 3d20 4e6f 6e65 0a0a 5649  less' = None..VI
-0034e750: 4557 3344 5f4d 545f 7365 6c65 6374 5f73  EW3D_MT_select_s
-0034e760: 6375 6c70 745f 6375 7276 6573 3a20 2762  culpt_curves: 'b
-0034e770: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
-0034e780: 642e 5649 4557 3344 5f4d 545f 7365 6c65  d.VIEW3D_MT_sele
-0034e790: 6374 5f73 6375 6c70 745f 6375 7276 6573  ct_sculpt_curves
-0034e7a0: 2720 3d20 4e6f 6e65 0a0a 5649 4557 3344  ' = None..VIEW3D
-0034e7b0: 5f4d 545f 7368 6164 696e 675f 6578 5f70  _MT_shading_ex_p
-0034e7c0: 6965 3a20 2762 6c5f 7569 2e73 7061 6365  ie: 'bl_ui.space
-0034e7d0: 5f76 6965 7733 642e 5649 4557 3344 5f4d  _view3d.VIEW3D_M
-0034e7e0: 545f 7368 6164 696e 675f 6578 5f70 6965  T_shading_ex_pie
-0034e7f0: 2720 3d20 4e6f 6e65 0a0a 5649 4557 3344  ' = None..VIEW3D
-0034e800: 5f4d 545f 7368 6164 696e 675f 7069 653a  _MT_shading_pie:
-0034e810: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
-0034e820: 6577 3364 2e56 4945 5733 445f 4d54 5f73  ew3d.VIEW3D_MT_s
-0034e830: 6861 6469 6e67 5f70 6965 2720 3d20 4e6f  hading_pie' = No
-0034e840: 6e65 0a0a 5649 4557 3344 5f4d 545f 736e  ne..VIEW3D_MT_sn
-0034e850: 6170 3a20 2762 6c5f 7569 2e73 7061 6365  ap: 'bl_ui.space
-0034e860: 5f76 6965 7733 642e 5649 4557 3344 5f4d  _view3d.VIEW3D_M
-0034e870: 545f 736e 6170 2720 3d20 4e6f 6e65 0a0a  T_snap' = None..
-0034e880: 5649 4557 3344 5f4d 545f 736e 6170 5f70  VIEW3D_MT_snap_p
-0034e890: 6965 3a20 2762 6c5f 7569 2e73 7061 6365  ie: 'bl_ui.space
-0034e8a0: 5f76 6965 7733 642e 5649 4557 3344 5f4d  _view3d.VIEW3D_M
-0034e8b0: 545f 736e 6170 5f70 6965 2720 3d20 4e6f  T_snap_pie' = No
-0034e8c0: 6e65 0a0a 5649 4557 3344 5f4d 545f 7375  ne..VIEW3D_MT_su
-0034e8d0: 7266 6163 655f 6164 643a 2027 626c 5f75  rface_add: 'bl_u
-0034e8e0: 692e 7370 6163 655f 7669 6577 3364 2e56  i.space_view3d.V
-0034e8f0: 4945 5733 445f 4d54 5f73 7572 6661 6365  IEW3D_MT_surface
-0034e900: 5f61 6464 2720 3d20 4e6f 6e65 0a0a 5649  _add' = None..VI
-0034e910: 4557 3344 5f4d 545f 746f 6f6c 735f 7072  EW3D_MT_tools_pr
-0034e920: 6f6a 6563 7470 6169 6e74 5f63 6c6f 6e65  ojectpaint_clone
-0034e930: 3a20 2762 6c5f 7569 2e70 726f 7065 7274  : 'bl_ui.propert
-0034e940: 6965 735f 7061 696e 745f 636f 6d6d 6f6e  ies_paint_common
-0034e950: 2e56 4945 5733 445f 4d54 5f74 6f6f 6c73  .VIEW3D_MT_tools
-0034e960: 5f70 726f 6a65 6374 7061 696e 745f 636c  _projectpaint_cl
-0034e970: 6f6e 6527 203d 204e 6f6e 650a 0a56 4945  one' = None..VIE
-0034e980: 5733 445f 4d54 5f74 6f6f 6c73 5f70 726f  W3D_MT_tools_pro
-0034e990: 6a65 6374 7061 696e 745f 7374 656e 6369  jectpaint_stenci
-0034e9a0: 6c3a 2027 626c 5f75 692e 7370 6163 655f  l: 'bl_ui.space_
-0034e9b0: 7669 6577 3364 5f74 6f6f 6c62 6172 2e56  view3d_toolbar.V
-0034e9c0: 4945 5733 445f 4d54 5f74 6f6f 6c73 5f70  IEW3D_MT_tools_p
-0034e9d0: 726f 6a65 6374 7061 696e 745f 7374 656e  rojectpaint_sten
-0034e9e0: 6369 6c27 203d 204e 6f6e 650a 0a56 4945  cil' = None..VIE
-0034e9f0: 5733 445f 4d54 5f74 6f6f 6c73 5f70 726f  W3D_MT_tools_pro
-0034ea00: 6a65 6374 7061 696e 745f 7576 6c61 7965  jectpaint_uvlaye
-0034ea10: 723a 2027 626c 5f75 692e 7370 6163 655f  r: 'bl_ui.space_
-0034ea20: 7669 6577 3364 5f74 6f6f 6c62 6172 2e56  view3d_toolbar.V
-0034ea30: 4945 5733 445f 4d54 5f74 6f6f 6c73 5f70  IEW3D_MT_tools_p
-0034ea40: 726f 6a65 6374 7061 696e 745f 7576 6c61  rojectpaint_uvla
-0034ea50: 7965 7227 203d 204e 6f6e 650a 0a56 4945  yer' = None..VIE
-0034ea60: 5733 445f 4d54 5f74 7261 6e73 666f 726d  W3D_MT_transform
-0034ea70: 3a20 2762 6c5f 7569 2e73 7061 6365 5f76  : 'bl_ui.space_v
-0034ea80: 6965 7733 642e 5649 4557 3344 5f4d 545f  iew3d.VIEW3D_MT_
-0034ea90: 7472 616e 7366 6f72 6d27 203d 204e 6f6e  transform' = Non
-0034eaa0: 650a 0a56 4945 5733 445f 4d54 5f74 7261  e..VIEW3D_MT_tra
-0034eab0: 6e73 666f 726d 5f61 726d 6174 7572 653a  nsform_armature:
-0034eac0: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
-0034ead0: 6577 3364 2e56 4945 5733 445f 4d54 5f74  ew3d.VIEW3D_MT_t
-0034eae0: 7261 6e73 666f 726d 5f61 726d 6174 7572  ransform_armatur
-0034eaf0: 6527 203d 204e 6f6e 650a 0a56 4945 5733  e' = None..VIEW3
-0034eb00: 445f 4d54 5f74 7261 6e73 666f 726d 5f67  D_MT_transform_g
-0034eb10: 697a 6d6f 5f70 6965 3a20 2762 6c5f 7569  izmo_pie: 'bl_ui
-0034eb20: 2e73 7061 6365 5f76 6965 7733 642e 5649  .space_view3d.VI
-0034eb30: 4557 3344 5f4d 545f 7472 616e 7366 6f72  EW3D_MT_transfor
-0034eb40: 6d5f 6769 7a6d 6f5f 7069 6527 203d 204e  m_gizmo_pie' = N
-0034eb50: 6f6e 650a 0a56 4945 5733 445f 4d54 5f74  one..VIEW3D_MT_t
-0034eb60: 7261 6e73 666f 726d 5f6f 626a 6563 743a  ransform_object:
-0034eb70: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
-0034eb80: 6577 3364 2e56 4945 5733 445f 4d54 5f74  ew3d.VIEW3D_MT_t
-0034eb90: 7261 6e73 666f 726d 5f6f 626a 6563 7427  ransform_object'
-0034eba0: 203d 204e 6f6e 650a 0a56 4945 5733 445f   = None..VIEW3D_
-0034ebb0: 4d54 5f75 765f 6d61 703a 2027 626c 5f75  MT_uv_map: 'bl_u
-0034ebc0: 692e 7370 6163 655f 7669 6577 3364 2e56  i.space_view3d.V
-0034ebd0: 4945 5733 445f 4d54 5f75 765f 6d61 7027  IEW3D_MT_uv_map'
-0034ebe0: 203d 204e 6f6e 650a 0a56 4945 5733 445f   = None..VIEW3D_
-0034ebf0: 4d54 5f76 6572 7465 785f 6772 6f75 703a  MT_vertex_group:
-0034ec00: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
-0034ec10: 6577 3364 2e56 4945 5733 445f 4d54 5f76  ew3d.VIEW3D_MT_v
-0034ec20: 6572 7465 785f 6772 6f75 7027 203d 204e  ertex_group' = N
-0034ec30: 6f6e 650a 0a56 4945 5733 445f 4d54 5f76  one..VIEW3D_MT_v
-0034ec40: 6965 773a 2027 626c 5f75 692e 7370 6163  iew: 'bl_ui.spac
-0034ec50: 655f 7669 6577 3364 2e56 4945 5733 445f  e_view3d.VIEW3D_
-0034ec60: 4d54 5f76 6965 7727 203d 204e 6f6e 650a  MT_view' = None.
-0034ec70: 0a56 4945 5733 445f 4d54 5f76 6965 775f  .VIEW3D_MT_view_
-0034ec80: 616c 6967 6e3a 2027 626c 5f75 692e 7370  align: 'bl_ui.sp
-0034ec90: 6163 655f 7669 6577 3364 2e56 4945 5733  ace_view3d.VIEW3
-0034eca0: 445f 4d54 5f76 6965 775f 616c 6967 6e27  D_MT_view_align'
-0034ecb0: 203d 204e 6f6e 650a 0a56 4945 5733 445f   = None..VIEW3D_
-0034ecc0: 4d54 5f76 6965 775f 616c 6967 6e5f 7365  MT_view_align_se
-0034ecd0: 6c65 6374 6564 3a20 2762 6c5f 7569 2e73  lected: 'bl_ui.s
-0034ece0: 7061 6365 5f76 6965 7733 642e 5649 4557  pace_view3d.VIEW
-0034ecf0: 3344 5f4d 545f 7669 6577 5f61 6c69 676e  3D_MT_view_align
-0034ed00: 5f73 656c 6563 7465 6427 203d 204e 6f6e  _selected' = Non
-0034ed10: 650a 0a56 4945 5733 445f 4d54 5f76 6965  e..VIEW3D_MT_vie
-0034ed20: 775f 6361 6d65 7261 733a 2027 626c 5f75  w_cameras: 'bl_u
-0034ed30: 692e 7370 6163 655f 7669 6577 3364 2e56  i.space_view3d.V
-0034ed40: 4945 5733 445f 4d54 5f76 6965 775f 6361  IEW3D_MT_view_ca
-0034ed50: 6d65 7261 7327 203d 204e 6f6e 650a 0a56  meras' = None..V
-0034ed60: 4945 5733 445f 4d54 5f76 6965 775f 6c6f  IEW3D_MT_view_lo
-0034ed70: 6361 6c3a 2027 626c 5f75 692e 7370 6163  cal: 'bl_ui.spac
-0034ed80: 655f 7669 6577 3364 2e56 4945 5733 445f  e_view3d.VIEW3D_
-0034ed90: 4d54 5f76 6965 775f 6c6f 6361 6c27 203d  MT_view_local' =
-0034eda0: 204e 6f6e 650a 0a56 4945 5733 445f 4d54   None..VIEW3D_MT
-0034edb0: 5f76 6965 775f 6e61 7669 6761 7469 6f6e  _view_navigation
-0034edc0: 3a20 2762 6c5f 7569 2e73 7061 6365 5f76  : 'bl_ui.space_v
-0034edd0: 6965 7733 642e 5649 4557 3344 5f4d 545f  iew3d.VIEW3D_MT_
-0034ede0: 7669 6577 5f6e 6176 6967 6174 696f 6e27  view_navigation'
-0034edf0: 203d 204e 6f6e 650a 0a56 4945 5733 445f   = None..VIEW3D_
-0034ee00: 4d54 5f76 6965 775f 7069 653a 2027 626c  MT_view_pie: 'bl
-0034ee10: 5f75 692e 7370 6163 655f 7669 6577 3364  _ui.space_view3d
-0034ee20: 2e56 4945 5733 445f 4d54 5f76 6965 775f  .VIEW3D_MT_view_
-0034ee30: 7069 6527 203d 204e 6f6e 650a 0a56 4945  pie' = None..VIE
-0034ee40: 5733 445f 4d54 5f76 6965 775f 7265 6769  W3D_MT_view_regi
-0034ee50: 6f6e 733a 2027 626c 5f75 692e 7370 6163  ons: 'bl_ui.spac
-0034ee60: 655f 7669 6577 3364 2e56 4945 5733 445f  e_view3d.VIEW3D_
-0034ee70: 4d54 5f76 6965 775f 7265 6769 6f6e 7327  MT_view_regions'
-0034ee80: 203d 204e 6f6e 650a 0a56 4945 5733 445f   = None..VIEW3D_
-0034ee90: 4d54 5f76 6965 775f 7669 6577 706f 696e  MT_view_viewpoin
-0034eea0: 743a 2027 626c 5f75 692e 7370 6163 655f  t: 'bl_ui.space_
-0034eeb0: 7669 6577 3364 2e56 4945 5733 445f 4d54  view3d.VIEW3D_MT
-0034eec0: 5f76 6965 775f 7669 6577 706f 696e 7427  _view_viewpoint'
-0034eed0: 203d 204e 6f6e 650a 0a56 4945 5733 445f   = None..VIEW3D_
-0034eee0: 4d54 5f76 6f6c 756d 655f 6164 643a 2027  MT_volume_add: '
-0034eef0: 626c 5f75 692e 7370 6163 655f 7669 6577  bl_ui.space_view
-0034ef00: 3364 2e56 4945 5733 445f 4d54 5f76 6f6c  3d.VIEW3D_MT_vol
-0034ef10: 756d 655f 6164 6427 203d 204e 6f6e 650a  ume_add' = None.
-0034ef20: 0a56 4945 5733 445f 4d54 5f77 6569 6768  .VIEW3D_MT_weigh
-0034ef30: 745f 6770 656e 6369 6c3a 2027 626c 5f75  t_gpencil: 'bl_u
-0034ef40: 692e 7370 6163 655f 7669 6577 3364 2e56  i.space_view3d.V
-0034ef50: 4945 5733 445f 4d54 5f77 6569 6768 745f  IEW3D_MT_weight_
-0034ef60: 6770 656e 6369 6c27 203d 204e 6f6e 650a  gpencil' = None.
-0034ef70: 0a56 4945 5733 445f 4d54 5f77 7061 696e  .VIEW3D_MT_wpain
-0034ef80: 745f 7667 726f 7570 5f6c 6f63 6b5f 7069  t_vgroup_lock_pi
-0034ef90: 653a 2027 626c 5f75 692e 7370 6163 655f  e: 'bl_ui.space_
-0034efa0: 7669 6577 3364 2e56 4945 5733 445f 4d54  view3d.VIEW3D_MT
-0034efb0: 5f77 7061 696e 745f 7667 726f 7570 5f6c  _wpaint_vgroup_l
-0034efc0: 6f63 6b5f 7069 6527 203d 204e 6f6e 650a  ock_pie' = None.
-0034efd0: 0a56 4945 5733 445f 4f54 5f65 6469 745f  .VIEW3D_OT_edit_
-0034efe0: 6d65 7368 5f65 7874 7275 6465 5f69 6e64  mesh_extrude_ind
-0034eff0: 6976 6964 7561 6c5f 6d6f 7665 3a20 2762  ividual_move: 'b
-0034f000: 6c5f 6f70 6572 6174 6f72 732e 7669 6577  l_operators.view
-0034f010: 3364 2e56 4945 5733 445f 4f54 5f65 6469  3d.VIEW3D_OT_edi
-0034f020: 745f 6d65 7368 5f65 7874 7275 6465 5f69  t_mesh_extrude_i
-0034f030: 6e64 6976 6964 7561 6c5f 6d6f 7665 2720  ndividual_move' 
-0034f040: 3d20 4e6f 6e65 0a0a 5649 4557 3344 5f4f  = None..VIEW3D_O
-0034f050: 545f 6564 6974 5f6d 6573 685f 6578 7472  T_edit_mesh_extr
-0034f060: 7564 655f 6d61 6e69 666f 6c64 5f6e 6f72  ude_manifold_nor
-0034f070: 6d61 6c3a 2027 626c 5f6f 7065 7261 746f  mal: 'bl_operato
-0034f080: 7273 2e76 6965 7733 642e 5649 4557 3344  rs.view3d.VIEW3D
-0034f090: 5f4f 545f 6564 6974 5f6d 6573 685f 6578  _OT_edit_mesh_ex
-0034f0a0: 7472 7564 655f 6d61 6e69 666f 6c64 5f6e  trude_manifold_n
-0034f0b0: 6f72 6d61 6c27 203d 204e 6f6e 650a 0a56  ormal' = None..V
-0034f0c0: 4945 5733 445f 4f54 5f74 7261 6e73 666f  IEW3D_OT_transfo
-0034f0d0: 726d 5f67 697a 6d6f 5f73 6574 3a20 2762  rm_gizmo_set: 'b
-0034f0e0: 6c5f 6f70 6572 6174 6f72 732e 7669 6577  l_operators.view
-0034f0f0: 3364 2e56 4945 5733 445f 4f54 5f74 7261  3d.VIEW3D_OT_tra
-0034f100: 6e73 666f 726d 5f67 697a 6d6f 5f73 6574  nsform_gizmo_set
-0034f110: 2720 3d20 4e6f 6e65 0a0a 5649 4557 3344  ' = None..VIEW3D
-0034f120: 5f50 545f 6163 7469 7665 5f74 6f6f 6c3a  _PT_active_tool:
-0034f130: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
-0034f140: 6577 3364 2e56 4945 5733 445f 5054 5f61  ew3d.VIEW3D_PT_a
-0034f150: 6374 6976 655f 746f 6f6c 2720 3d20 4e6f  ctive_tool' = No
-0034f160: 6e65 0a0a 5649 4557 3344 5f50 545f 6163  ne..VIEW3D_PT_ac
-0034f170: 7469 7665 5f74 6f6f 6c5f 6475 706c 6963  tive_tool_duplic
-0034f180: 6174 653a 2027 626c 5f75 692e 7370 6163  ate: 'bl_ui.spac
-0034f190: 655f 7669 6577 3364 2e56 4945 5733 445f  e_view3d.VIEW3D_
-0034f1a0: 5054 5f61 6374 6976 655f 746f 6f6c 5f64  PT_active_tool_d
-0034f1b0: 7570 6c69 6361 7465 2720 3d20 4e6f 6e65  uplicate' = None
-0034f1c0: 0a0a 5649 4557 3344 5f50 545f 616e 6e6f  ..VIEW3D_PT_anno
-0034f1d0: 7461 7469 6f6e 5f6f 6e69 6f6e 3a20 2762  tation_onion: 'b
-0034f1e0: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
-0034f1f0: 642e 5649 4557 3344 5f50 545f 616e 6e6f  d.VIEW3D_PT_anno
-0034f200: 7461 7469 6f6e 5f6f 6e69 6f6e 2720 3d20  tation_onion' = 
-0034f210: 4e6f 6e65 0a0a 5649 4557 3344 5f50 545f  None..VIEW3D_PT_
-0034f220: 636f 6c6c 6563 7469 6f6e 733a 2027 626c  collections: 'bl
-0034f230: 5f75 692e 7370 6163 655f 7669 6577 3364  _ui.space_view3d
-0034f240: 2e56 4945 5733 445f 5054 5f63 6f6c 6c65  .VIEW3D_PT_colle
-0034f250: 6374 696f 6e73 2720 3d20 4e6f 6e65 0a0a  ctions' = None..
-0034f260: 5649 4557 3344 5f50 545f 636f 6e74 6578  VIEW3D_PT_contex
-0034f270: 745f 7072 6f70 6572 7469 6573 3a20 2762  t_properties: 'b
-0034f280: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
-0034f290: 642e 5649 4557 3344 5f50 545f 636f 6e74  d.VIEW3D_PT_cont
-0034f2a0: 6578 745f 7072 6f70 6572 7469 6573 2720  ext_properties' 
-0034f2b0: 3d20 4e6f 6e65 0a0a 5649 4557 3344 5f50  = None..VIEW3D_P
-0034f2c0: 545f 6375 7276 6573 5f73 6375 6c70 745f  T_curves_sculpt_
-0034f2d0: 6164 645f 7368 6170 653a 2027 626c 5f75  add_shape: 'bl_u
-0034f2e0: 692e 7370 6163 655f 7669 6577 3364 2e56  i.space_view3d.V
-0034f2f0: 4945 5733 445f 5054 5f63 7572 7665 735f  IEW3D_PT_curves_
-0034f300: 7363 756c 7074 5f61 6464 5f73 6861 7065  sculpt_add_shape
-0034f310: 2720 3d20 4e6f 6e65 0a0a 5649 4557 3344  ' = None..VIEW3D
-0034f320: 5f50 545f 6375 7276 6573 5f73 6375 6c70  _PT_curves_sculp
-0034f330: 745f 6772 6f77 5f73 6872 696e 6b5f 7363  t_grow_shrink_sc
-0034f340: 616c 696e 673a 2027 626c 5f75 692e 7370  aling: 'bl_ui.sp
-0034f350: 6163 655f 7669 6577 3364 2e56 4945 5733  ace_view3d.VIEW3
-0034f360: 445f 5054 5f63 7572 7665 735f 7363 756c  D_PT_curves_scul
-0034f370: 7074 5f67 726f 775f 7368 7269 6e6b 5f73  pt_grow_shrink_s
-0034f380: 6361 6c69 6e67 2720 3d20 4e6f 6e65 0a0a  caling' = None..
-0034f390: 5649 4557 3344 5f50 545f 6375 7276 6573  VIEW3D_PT_curves
-0034f3a0: 5f73 6375 6c70 745f 7061 7261 6d65 7465  _sculpt_paramete
-0034f3b0: 725f 6661 6c6c 6f66 663a 2027 626c 5f75  r_falloff: 'bl_u
-0034f3c0: 692e 7370 6163 655f 7669 6577 3364 2e56  i.space_view3d.V
-0034f3d0: 4945 5733 445f 5054 5f63 7572 7665 735f  IEW3D_PT_curves_
-0034f3e0: 7363 756c 7074 5f70 6172 616d 6574 6572  sculpt_parameter
-0034f3f0: 5f66 616c 6c6f 6666 2720 3d20 4e6f 6e65  _falloff' = None
-0034f400: 0a0a 5649 4557 3344 5f50 545f 6375 7276  ..VIEW3D_PT_curv
-0034f410: 6573 5f73 6375 6c70 745f 7379 6d6d 6574  es_sculpt_symmet
-0034f420: 7279 3a20 2762 6c5f 7569 2e73 7061 6365  ry: 'bl_ui.space
-0034f430: 5f76 6965 7733 645f 746f 6f6c 6261 722e  _view3d_toolbar.
-0034f440: 5649 4557 3344 5f50 545f 6375 7276 6573  VIEW3D_PT_curves
-0034f450: 5f73 6375 6c70 745f 7379 6d6d 6574 7279  _sculpt_symmetry
-0034f460: 2720 3d20 4e6f 6e65 0a0a 5649 4557 3344  ' = None..VIEW3D
-0034f470: 5f50 545f 6375 7276 6573 5f73 6375 6c70  _PT_curves_sculp
-0034f480: 745f 7379 6d6d 6574 7279 5f66 6f72 5f74  t_symmetry_for_t
-0034f490: 6f70 6261 723a 2027 626c 5f75 692e 7370  opbar: 'bl_ui.sp
-0034f4a0: 6163 655f 7669 6577 3364 5f74 6f6f 6c62  ace_view3d_toolb
-0034f4b0: 6172 2e56 4945 5733 445f 5054 5f63 7572  ar.VIEW3D_PT_cur
-0034f4c0: 7665 735f 7363 756c 7074 5f73 796d 6d65  ves_sculpt_symme
-0034f4d0: 7472 795f 666f 725f 746f 7062 6172 2720  try_for_topbar' 
-0034f4e0: 3d20 4e6f 6e65 0a0a 5649 4557 3344 5f50  = None..VIEW3D_P
-0034f4f0: 545f 6769 7a6d 6f5f 6469 7370 6c61 793a  T_gizmo_display:
-0034f500: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
-0034f510: 6577 3364 2e56 4945 5733 445f 5054 5f67  ew3d.VIEW3D_PT_g
-0034f520: 697a 6d6f 5f64 6973 706c 6179 2720 3d20  izmo_display' = 
-0034f530: 4e6f 6e65 0a0a 5649 4557 3344 5f50 545f  None..VIEW3D_PT_
-0034f540: 6770 656e 6369 6c5f 6272 7573 685f 7072  gpencil_brush_pr
-0034f550: 6573 6574 733a 2027 626c 5f75 692e 7370  esets: 'bl_ui.sp
-0034f560: 6163 655f 7669 6577 3364 5f74 6f6f 6c62  ace_view3d_toolb
-0034f570: 6172 2e56 4945 5733 445f 5054 5f67 7065  ar.VIEW3D_PT_gpe
-0034f580: 6e63 696c 5f62 7275 7368 5f70 7265 7365  ncil_brush_prese
-0034f590: 7473 2720 3d20 4e6f 6e65 0a0a 5649 4557  ts' = None..VIEW
-0034f5a0: 3344 5f50 545f 6770 656e 6369 6c5f 6375  3D_PT_gpencil_cu
-0034f5b0: 7276 655f 6564 6974 3a20 2762 6c5f 7569  rve_edit: 'bl_ui
-0034f5c0: 2e73 7061 6365 5f76 6965 7733 642e 5649  .space_view3d.VI
-0034f5d0: 4557 3344 5f50 545f 6770 656e 6369 6c5f  EW3D_PT_gpencil_
-0034f5e0: 6375 7276 655f 6564 6974 2720 3d20 4e6f  curve_edit' = No
-0034f5f0: 6e65 0a0a 5649 4557 3344 5f50 545f 6770  ne..VIEW3D_PT_gp
-0034f600: 656e 6369 6c5f 6472 6177 5f63 6f6e 7465  encil_draw_conte
-0034f610: 7874 5f6d 656e 753a 2027 626c 5f75 692e  xt_menu: 'bl_ui.
-0034f620: 7370 6163 655f 7669 6577 3364 2e56 4945  space_view3d.VIE
-0034f630: 5733 445f 5054 5f67 7065 6e63 696c 5f64  W3D_PT_gpencil_d
-0034f640: 7261 775f 636f 6e74 6578 745f 6d65 6e75  raw_context_menu
+0034e340: 6374 5f65 6469 745f 6772 6561 7365 5f70  ct_edit_grease_p
+0034e350: 656e 6369 6c3a 2027 626c 5f75 692e 7370  encil: 'bl_ui.sp
+0034e360: 6163 655f 7669 6577 3364 2e56 4945 5733  ace_view3d.VIEW3
+0034e370: 445f 4d54 5f73 656c 6563 745f 6564 6974  D_MT_select_edit
+0034e380: 5f67 7265 6173 655f 7065 6e63 696c 2720  _grease_pencil' 
+0034e390: 3d20 4e6f 6e65 0a0a 5649 4557 3344 5f4d  = None..VIEW3D_M
+0034e3a0: 545f 7365 6c65 6374 5f65 6469 745f 6c61  T_select_edit_la
+0034e3b0: 7474 6963 653a 2027 626c 5f75 692e 7370  ttice: 'bl_ui.sp
+0034e3c0: 6163 655f 7669 6577 3364 2e56 4945 5733  ace_view3d.VIEW3
+0034e3d0: 445f 4d54 5f73 656c 6563 745f 6564 6974  D_MT_select_edit
+0034e3e0: 5f6c 6174 7469 6365 2720 3d20 4e6f 6e65  _lattice' = None
+0034e3f0: 0a0a 5649 4557 3344 5f4d 545f 7365 6c65  ..VIEW3D_MT_sele
+0034e400: 6374 5f65 6469 745f 6d65 7368 3a20 2762  ct_edit_mesh: 'b
+0034e410: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
+0034e420: 642e 5649 4557 3344 5f4d 545f 7365 6c65  d.VIEW3D_MT_sele
+0034e430: 6374 5f65 6469 745f 6d65 7368 2720 3d20  ct_edit_mesh' = 
+0034e440: 4e6f 6e65 0a0a 5649 4557 3344 5f4d 545f  None..VIEW3D_MT_
+0034e450: 7365 6c65 6374 5f65 6469 745f 6d65 7461  select_edit_meta
+0034e460: 6261 6c6c 3a20 2762 6c5f 7569 2e73 7061  ball: 'bl_ui.spa
+0034e470: 6365 5f76 6965 7733 642e 5649 4557 3344  ce_view3d.VIEW3D
+0034e480: 5f4d 545f 7365 6c65 6374 5f65 6469 745f  _MT_select_edit_
+0034e490: 6d65 7461 6261 6c6c 2720 3d20 4e6f 6e65  metaball' = None
+0034e4a0: 0a0a 5649 4557 3344 5f4d 545f 7365 6c65  ..VIEW3D_MT_sele
+0034e4b0: 6374 5f65 6469 745f 7375 7266 6163 653a  ct_edit_surface:
+0034e4c0: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
+0034e4d0: 6577 3364 2e56 4945 5733 445f 4d54 5f73  ew3d.VIEW3D_MT_s
+0034e4e0: 656c 6563 745f 6564 6974 5f73 7572 6661  elect_edit_surfa
+0034e4f0: 6365 2720 3d20 4e6f 6e65 0a0a 5649 4557  ce' = None..VIEW
+0034e500: 3344 5f4d 545f 7365 6c65 6374 5f65 6469  3D_MT_select_edi
+0034e510: 745f 7465 7874 3a20 2762 6c5f 7569 2e73  t_text: 'bl_ui.s
+0034e520: 7061 6365 5f76 6965 7733 642e 5649 4557  pace_view3d.VIEW
+0034e530: 3344 5f4d 545f 7365 6c65 6374 5f65 6469  3D_MT_select_edi
+0034e540: 745f 7465 7874 2720 3d20 4e6f 6e65 0a0a  t_text' = None..
+0034e550: 5649 4557 3344 5f4d 545f 7365 6c65 6374  VIEW3D_MT_select
+0034e560: 5f6f 626a 6563 743a 2027 626c 5f75 692e  _object: 'bl_ui.
+0034e570: 7370 6163 655f 7669 6577 3364 2e56 4945  space_view3d.VIE
+0034e580: 5733 445f 4d54 5f73 656c 6563 745f 6f62  W3D_MT_select_ob
+0034e590: 6a65 6374 2720 3d20 4e6f 6e65 0a0a 5649  ject' = None..VI
+0034e5a0: 4557 3344 5f4d 545f 7365 6c65 6374 5f6f  EW3D_MT_select_o
+0034e5b0: 626a 6563 745f 6d6f 7265 5f6c 6573 733a  bject_more_less:
+0034e5c0: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
+0034e5d0: 6577 3364 2e56 4945 5733 445f 4d54 5f73  ew3d.VIEW3D_MT_s
+0034e5e0: 656c 6563 745f 6f62 6a65 6374 5f6d 6f72  elect_object_mor
+0034e5f0: 655f 6c65 7373 2720 3d20 4e6f 6e65 0a0a  e_less' = None..
+0034e600: 5649 4557 3344 5f4d 545f 7365 6c65 6374  VIEW3D_MT_select
+0034e610: 5f70 6169 6e74 5f6d 6173 6b3a 2027 626c  _paint_mask: 'bl
+0034e620: 5f75 692e 7370 6163 655f 7669 6577 3364  _ui.space_view3d
+0034e630: 2e56 4945 5733 445f 4d54 5f73 656c 6563  .VIEW3D_MT_selec
+0034e640: 745f 7061 696e 745f 6d61 736b 2720 3d20  t_paint_mask' = 
+0034e650: 4e6f 6e65 0a0a 5649 4557 3344 5f4d 545f  None..VIEW3D_MT_
+0034e660: 7365 6c65 6374 5f70 6169 6e74 5f6d 6173  select_paint_mas
+0034e670: 6b5f 7665 7274 6578 3a20 2762 6c5f 7569  k_vertex: 'bl_ui
+0034e680: 2e73 7061 6365 5f76 6965 7733 642e 5649  .space_view3d.VI
+0034e690: 4557 3344 5f4d 545f 7365 6c65 6374 5f70  EW3D_MT_select_p
+0034e6a0: 6169 6e74 5f6d 6173 6b5f 7665 7274 6578  aint_mask_vertex
+0034e6b0: 2720 3d20 4e6f 6e65 0a0a 5649 4557 3344  ' = None..VIEW3D
+0034e6c0: 5f4d 545f 7365 6c65 6374 5f70 6172 7469  _MT_select_parti
+0034e6d0: 636c 653a 2027 626c 5f75 692e 7370 6163  cle: 'bl_ui.spac
+0034e6e0: 655f 7669 6577 3364 2e56 4945 5733 445f  e_view3d.VIEW3D_
+0034e6f0: 4d54 5f73 656c 6563 745f 7061 7274 6963  MT_select_partic
+0034e700: 6c65 2720 3d20 4e6f 6e65 0a0a 5649 4557  le' = None..VIEW
+0034e710: 3344 5f4d 545f 7365 6c65 6374 5f70 6f73  3D_MT_select_pos
+0034e720: 653a 2027 626c 5f75 692e 7370 6163 655f  e: 'bl_ui.space_
+0034e730: 7669 6577 3364 2e56 4945 5733 445f 4d54  view3d.VIEW3D_MT
+0034e740: 5f73 656c 6563 745f 706f 7365 2720 3d20  _select_pose' = 
+0034e750: 4e6f 6e65 0a0a 5649 4557 3344 5f4d 545f  None..VIEW3D_MT_
+0034e760: 7365 6c65 6374 5f70 6f73 655f 6d6f 7265  select_pose_more
+0034e770: 5f6c 6573 733a 2027 626c 5f75 692e 7370  _less: 'bl_ui.sp
+0034e780: 6163 655f 7669 6577 3364 2e56 4945 5733  ace_view3d.VIEW3
+0034e790: 445f 4d54 5f73 656c 6563 745f 706f 7365  D_MT_select_pose
+0034e7a0: 5f6d 6f72 655f 6c65 7373 2720 3d20 4e6f  _more_less' = No
+0034e7b0: 6e65 0a0a 5649 4557 3344 5f4d 545f 7365  ne..VIEW3D_MT_se
+0034e7c0: 6c65 6374 5f73 6375 6c70 745f 6375 7276  lect_sculpt_curv
+0034e7d0: 6573 3a20 2762 6c5f 7569 2e73 7061 6365  es: 'bl_ui.space
+0034e7e0: 5f76 6965 7733 642e 5649 4557 3344 5f4d  _view3d.VIEW3D_M
+0034e7f0: 545f 7365 6c65 6374 5f73 6375 6c70 745f  T_select_sculpt_
+0034e800: 6375 7276 6573 2720 3d20 4e6f 6e65 0a0a  curves' = None..
+0034e810: 5649 4557 3344 5f4d 545f 7368 6164 696e  VIEW3D_MT_shadin
+0034e820: 675f 6578 5f70 6965 3a20 2762 6c5f 7569  g_ex_pie: 'bl_ui
+0034e830: 2e73 7061 6365 5f76 6965 7733 642e 5649  .space_view3d.VI
+0034e840: 4557 3344 5f4d 545f 7368 6164 696e 675f  EW3D_MT_shading_
+0034e850: 6578 5f70 6965 2720 3d20 4e6f 6e65 0a0a  ex_pie' = None..
+0034e860: 5649 4557 3344 5f4d 545f 7368 6164 696e  VIEW3D_MT_shadin
+0034e870: 675f 7069 653a 2027 626c 5f75 692e 7370  g_pie: 'bl_ui.sp
+0034e880: 6163 655f 7669 6577 3364 2e56 4945 5733  ace_view3d.VIEW3
+0034e890: 445f 4d54 5f73 6861 6469 6e67 5f70 6965  D_MT_shading_pie
+0034e8a0: 2720 3d20 4e6f 6e65 0a0a 5649 4557 3344  ' = None..VIEW3D
+0034e8b0: 5f4d 545f 736e 6170 3a20 2762 6c5f 7569  _MT_snap: 'bl_ui
+0034e8c0: 2e73 7061 6365 5f76 6965 7733 642e 5649  .space_view3d.VI
+0034e8d0: 4557 3344 5f4d 545f 736e 6170 2720 3d20  EW3D_MT_snap' = 
+0034e8e0: 4e6f 6e65 0a0a 5649 4557 3344 5f4d 545f  None..VIEW3D_MT_
+0034e8f0: 736e 6170 5f70 6965 3a20 2762 6c5f 7569  snap_pie: 'bl_ui
+0034e900: 2e73 7061 6365 5f76 6965 7733 642e 5649  .space_view3d.VI
+0034e910: 4557 3344 5f4d 545f 736e 6170 5f70 6965  EW3D_MT_snap_pie
+0034e920: 2720 3d20 4e6f 6e65 0a0a 5649 4557 3344  ' = None..VIEW3D
+0034e930: 5f4d 545f 7375 7266 6163 655f 6164 643a  _MT_surface_add:
+0034e940: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
+0034e950: 6577 3364 2e56 4945 5733 445f 4d54 5f73  ew3d.VIEW3D_MT_s
+0034e960: 7572 6661 6365 5f61 6464 2720 3d20 4e6f  urface_add' = No
+0034e970: 6e65 0a0a 5649 4557 3344 5f4d 545f 746f  ne..VIEW3D_MT_to
+0034e980: 6f6c 735f 7072 6f6a 6563 7470 6169 6e74  ols_projectpaint
+0034e990: 5f63 6c6f 6e65 3a20 2762 6c5f 7569 2e70  _clone: 'bl_ui.p
+0034e9a0: 726f 7065 7274 6965 735f 7061 696e 745f  roperties_paint_
+0034e9b0: 636f 6d6d 6f6e 2e56 4945 5733 445f 4d54  common.VIEW3D_MT
+0034e9c0: 5f74 6f6f 6c73 5f70 726f 6a65 6374 7061  _tools_projectpa
+0034e9d0: 696e 745f 636c 6f6e 6527 203d 204e 6f6e  int_clone' = Non
+0034e9e0: 650a 0a56 4945 5733 445f 4d54 5f74 6f6f  e..VIEW3D_MT_too
+0034e9f0: 6c73 5f70 726f 6a65 6374 7061 696e 745f  ls_projectpaint_
+0034ea00: 7374 656e 6369 6c3a 2027 626c 5f75 692e  stencil: 'bl_ui.
+0034ea10: 7370 6163 655f 7669 6577 3364 5f74 6f6f  space_view3d_too
+0034ea20: 6c62 6172 2e56 4945 5733 445f 4d54 5f74  lbar.VIEW3D_MT_t
+0034ea30: 6f6f 6c73 5f70 726f 6a65 6374 7061 696e  ools_projectpain
+0034ea40: 745f 7374 656e 6369 6c27 203d 204e 6f6e  t_stencil' = Non
+0034ea50: 650a 0a56 4945 5733 445f 4d54 5f74 6f6f  e..VIEW3D_MT_too
+0034ea60: 6c73 5f70 726f 6a65 6374 7061 696e 745f  ls_projectpaint_
+0034ea70: 7576 6c61 7965 723a 2027 626c 5f75 692e  uvlayer: 'bl_ui.
+0034ea80: 7370 6163 655f 7669 6577 3364 5f74 6f6f  space_view3d_too
+0034ea90: 6c62 6172 2e56 4945 5733 445f 4d54 5f74  lbar.VIEW3D_MT_t
+0034eaa0: 6f6f 6c73 5f70 726f 6a65 6374 7061 696e  ools_projectpain
+0034eab0: 745f 7576 6c61 7965 7227 203d 204e 6f6e  t_uvlayer' = Non
+0034eac0: 650a 0a56 4945 5733 445f 4d54 5f74 7261  e..VIEW3D_MT_tra
+0034ead0: 6e73 666f 726d 3a20 2762 6c5f 7569 2e73  nsform: 'bl_ui.s
+0034eae0: 7061 6365 5f76 6965 7733 642e 5649 4557  pace_view3d.VIEW
+0034eaf0: 3344 5f4d 545f 7472 616e 7366 6f72 6d27  3D_MT_transform'
+0034eb00: 203d 204e 6f6e 650a 0a56 4945 5733 445f   = None..VIEW3D_
+0034eb10: 4d54 5f74 7261 6e73 666f 726d 5f61 726d  MT_transform_arm
+0034eb20: 6174 7572 653a 2027 626c 5f75 692e 7370  ature: 'bl_ui.sp
+0034eb30: 6163 655f 7669 6577 3364 2e56 4945 5733  ace_view3d.VIEW3
+0034eb40: 445f 4d54 5f74 7261 6e73 666f 726d 5f61  D_MT_transform_a
+0034eb50: 726d 6174 7572 6527 203d 204e 6f6e 650a  rmature' = None.
+0034eb60: 0a56 4945 5733 445f 4d54 5f74 7261 6e73  .VIEW3D_MT_trans
+0034eb70: 666f 726d 5f67 697a 6d6f 5f70 6965 3a20  form_gizmo_pie: 
+0034eb80: 2762 6c5f 7569 2e73 7061 6365 5f76 6965  'bl_ui.space_vie
+0034eb90: 7733 642e 5649 4557 3344 5f4d 545f 7472  w3d.VIEW3D_MT_tr
+0034eba0: 616e 7366 6f72 6d5f 6769 7a6d 6f5f 7069  ansform_gizmo_pi
+0034ebb0: 6527 203d 204e 6f6e 650a 0a56 4945 5733  e' = None..VIEW3
+0034ebc0: 445f 4d54 5f74 7261 6e73 666f 726d 5f6f  D_MT_transform_o
+0034ebd0: 626a 6563 743a 2027 626c 5f75 692e 7370  bject: 'bl_ui.sp
+0034ebe0: 6163 655f 7669 6577 3364 2e56 4945 5733  ace_view3d.VIEW3
+0034ebf0: 445f 4d54 5f74 7261 6e73 666f 726d 5f6f  D_MT_transform_o
+0034ec00: 626a 6563 7427 203d 204e 6f6e 650a 0a56  bject' = None..V
+0034ec10: 4945 5733 445f 4d54 5f75 765f 6d61 703a  IEW3D_MT_uv_map:
+0034ec20: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
+0034ec30: 6577 3364 2e56 4945 5733 445f 4d54 5f75  ew3d.VIEW3D_MT_u
+0034ec40: 765f 6d61 7027 203d 204e 6f6e 650a 0a56  v_map' = None..V
+0034ec50: 4945 5733 445f 4d54 5f76 6572 7465 785f  IEW3D_MT_vertex_
+0034ec60: 6772 6f75 703a 2027 626c 5f75 692e 7370  group: 'bl_ui.sp
+0034ec70: 6163 655f 7669 6577 3364 2e56 4945 5733  ace_view3d.VIEW3
+0034ec80: 445f 4d54 5f76 6572 7465 785f 6772 6f75  D_MT_vertex_grou
+0034ec90: 7027 203d 204e 6f6e 650a 0a56 4945 5733  p' = None..VIEW3
+0034eca0: 445f 4d54 5f76 6965 773a 2027 626c 5f75  D_MT_view: 'bl_u
+0034ecb0: 692e 7370 6163 655f 7669 6577 3364 2e56  i.space_view3d.V
+0034ecc0: 4945 5733 445f 4d54 5f76 6965 7727 203d  IEW3D_MT_view' =
+0034ecd0: 204e 6f6e 650a 0a56 4945 5733 445f 4d54   None..VIEW3D_MT
+0034ece0: 5f76 6965 775f 616c 6967 6e3a 2027 626c  _view_align: 'bl
+0034ecf0: 5f75 692e 7370 6163 655f 7669 6577 3364  _ui.space_view3d
+0034ed00: 2e56 4945 5733 445f 4d54 5f76 6965 775f  .VIEW3D_MT_view_
+0034ed10: 616c 6967 6e27 203d 204e 6f6e 650a 0a56  align' = None..V
+0034ed20: 4945 5733 445f 4d54 5f76 6965 775f 616c  IEW3D_MT_view_al
+0034ed30: 6967 6e5f 7365 6c65 6374 6564 3a20 2762  ign_selected: 'b
+0034ed40: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
+0034ed50: 642e 5649 4557 3344 5f4d 545f 7669 6577  d.VIEW3D_MT_view
+0034ed60: 5f61 6c69 676e 5f73 656c 6563 7465 6427  _align_selected'
+0034ed70: 203d 204e 6f6e 650a 0a56 4945 5733 445f   = None..VIEW3D_
+0034ed80: 4d54 5f76 6965 775f 6361 6d65 7261 733a  MT_view_cameras:
+0034ed90: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
+0034eda0: 6577 3364 2e56 4945 5733 445f 4d54 5f76  ew3d.VIEW3D_MT_v
+0034edb0: 6965 775f 6361 6d65 7261 7327 203d 204e  iew_cameras' = N
+0034edc0: 6f6e 650a 0a56 4945 5733 445f 4d54 5f76  one..VIEW3D_MT_v
+0034edd0: 6965 775f 6c6f 6361 6c3a 2027 626c 5f75  iew_local: 'bl_u
+0034ede0: 692e 7370 6163 655f 7669 6577 3364 2e56  i.space_view3d.V
+0034edf0: 4945 5733 445f 4d54 5f76 6965 775f 6c6f  IEW3D_MT_view_lo
+0034ee00: 6361 6c27 203d 204e 6f6e 650a 0a56 4945  cal' = None..VIE
+0034ee10: 5733 445f 4d54 5f76 6965 775f 6e61 7669  W3D_MT_view_navi
+0034ee20: 6761 7469 6f6e 3a20 2762 6c5f 7569 2e73  gation: 'bl_ui.s
+0034ee30: 7061 6365 5f76 6965 7733 642e 5649 4557  pace_view3d.VIEW
+0034ee40: 3344 5f4d 545f 7669 6577 5f6e 6176 6967  3D_MT_view_navig
+0034ee50: 6174 696f 6e27 203d 204e 6f6e 650a 0a56  ation' = None..V
+0034ee60: 4945 5733 445f 4d54 5f76 6965 775f 7069  IEW3D_MT_view_pi
+0034ee70: 653a 2027 626c 5f75 692e 7370 6163 655f  e: 'bl_ui.space_
+0034ee80: 7669 6577 3364 2e56 4945 5733 445f 4d54  view3d.VIEW3D_MT
+0034ee90: 5f76 6965 775f 7069 6527 203d 204e 6f6e  _view_pie' = Non
+0034eea0: 650a 0a56 4945 5733 445f 4d54 5f76 6965  e..VIEW3D_MT_vie
+0034eeb0: 775f 7265 6769 6f6e 733a 2027 626c 5f75  w_regions: 'bl_u
+0034eec0: 692e 7370 6163 655f 7669 6577 3364 2e56  i.space_view3d.V
+0034eed0: 4945 5733 445f 4d54 5f76 6965 775f 7265  IEW3D_MT_view_re
+0034eee0: 6769 6f6e 7327 203d 204e 6f6e 650a 0a56  gions' = None..V
+0034eef0: 4945 5733 445f 4d54 5f76 6965 775f 7669  IEW3D_MT_view_vi
+0034ef00: 6577 706f 696e 743a 2027 626c 5f75 692e  ewpoint: 'bl_ui.
+0034ef10: 7370 6163 655f 7669 6577 3364 2e56 4945  space_view3d.VIE
+0034ef20: 5733 445f 4d54 5f76 6965 775f 7669 6577  W3D_MT_view_view
+0034ef30: 706f 696e 7427 203d 204e 6f6e 650a 0a56  point' = None..V
+0034ef40: 4945 5733 445f 4d54 5f76 6f6c 756d 655f  IEW3D_MT_volume_
+0034ef50: 6164 643a 2027 626c 5f75 692e 7370 6163  add: 'bl_ui.spac
+0034ef60: 655f 7669 6577 3364 2e56 4945 5733 445f  e_view3d.VIEW3D_
+0034ef70: 4d54 5f76 6f6c 756d 655f 6164 6427 203d  MT_volume_add' =
+0034ef80: 204e 6f6e 650a 0a56 4945 5733 445f 4d54   None..VIEW3D_MT
+0034ef90: 5f77 6569 6768 745f 6770 656e 6369 6c3a  _weight_gpencil:
+0034efa0: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
+0034efb0: 6577 3364 2e56 4945 5733 445f 4d54 5f77  ew3d.VIEW3D_MT_w
+0034efc0: 6569 6768 745f 6770 656e 6369 6c27 203d  eight_gpencil' =
+0034efd0: 204e 6f6e 650a 0a56 4945 5733 445f 4d54   None..VIEW3D_MT
+0034efe0: 5f77 7061 696e 745f 7667 726f 7570 5f6c  _wpaint_vgroup_l
+0034eff0: 6f63 6b5f 7069 653a 2027 626c 5f75 692e  ock_pie: 'bl_ui.
+0034f000: 7370 6163 655f 7669 6577 3364 2e56 4945  space_view3d.VIE
+0034f010: 5733 445f 4d54 5f77 7061 696e 745f 7667  W3D_MT_wpaint_vg
+0034f020: 726f 7570 5f6c 6f63 6b5f 7069 6527 203d  roup_lock_pie' =
+0034f030: 204e 6f6e 650a 0a56 4945 5733 445f 4f54   None..VIEW3D_OT
+0034f040: 5f65 6469 745f 6d65 7368 5f65 7874 7275  _edit_mesh_extru
+0034f050: 6465 5f69 6e64 6976 6964 7561 6c5f 6d6f  de_individual_mo
+0034f060: 7665 3a20 2762 6c5f 6f70 6572 6174 6f72  ve: 'bl_operator
+0034f070: 732e 7669 6577 3364 2e56 4945 5733 445f  s.view3d.VIEW3D_
+0034f080: 4f54 5f65 6469 745f 6d65 7368 5f65 7874  OT_edit_mesh_ext
+0034f090: 7275 6465 5f69 6e64 6976 6964 7561 6c5f  rude_individual_
+0034f0a0: 6d6f 7665 2720 3d20 4e6f 6e65 0a0a 5649  move' = None..VI
+0034f0b0: 4557 3344 5f4f 545f 6564 6974 5f6d 6573  EW3D_OT_edit_mes
+0034f0c0: 685f 6578 7472 7564 655f 6d61 6e69 666f  h_extrude_manifo
+0034f0d0: 6c64 5f6e 6f72 6d61 6c3a 2027 626c 5f6f  ld_normal: 'bl_o
+0034f0e0: 7065 7261 746f 7273 2e76 6965 7733 642e  perators.view3d.
+0034f0f0: 5649 4557 3344 5f4f 545f 6564 6974 5f6d  VIEW3D_OT_edit_m
+0034f100: 6573 685f 6578 7472 7564 655f 6d61 6e69  esh_extrude_mani
+0034f110: 666f 6c64 5f6e 6f72 6d61 6c27 203d 204e  fold_normal' = N
+0034f120: 6f6e 650a 0a56 4945 5733 445f 4f54 5f74  one..VIEW3D_OT_t
+0034f130: 7261 6e73 666f 726d 5f67 697a 6d6f 5f73  ransform_gizmo_s
+0034f140: 6574 3a20 2762 6c5f 6f70 6572 6174 6f72  et: 'bl_operator
+0034f150: 732e 7669 6577 3364 2e56 4945 5733 445f  s.view3d.VIEW3D_
+0034f160: 4f54 5f74 7261 6e73 666f 726d 5f67 697a  OT_transform_giz
+0034f170: 6d6f 5f73 6574 2720 3d20 4e6f 6e65 0a0a  mo_set' = None..
+0034f180: 5649 4557 3344 5f50 545f 6163 7469 7665  VIEW3D_PT_active
+0034f190: 5f74 6f6f 6c3a 2027 626c 5f75 692e 7370  _tool: 'bl_ui.sp
+0034f1a0: 6163 655f 7669 6577 3364 2e56 4945 5733  ace_view3d.VIEW3
+0034f1b0: 445f 5054 5f61 6374 6976 655f 746f 6f6c  D_PT_active_tool
+0034f1c0: 2720 3d20 4e6f 6e65 0a0a 5649 4557 3344  ' = None..VIEW3D
+0034f1d0: 5f50 545f 6163 7469 7665 5f74 6f6f 6c5f  _PT_active_tool_
+0034f1e0: 6475 706c 6963 6174 653a 2027 626c 5f75  duplicate: 'bl_u
+0034f1f0: 692e 7370 6163 655f 7669 6577 3364 2e56  i.space_view3d.V
+0034f200: 4945 5733 445f 5054 5f61 6374 6976 655f  IEW3D_PT_active_
+0034f210: 746f 6f6c 5f64 7570 6c69 6361 7465 2720  tool_duplicate' 
+0034f220: 3d20 4e6f 6e65 0a0a 5649 4557 3344 5f50  = None..VIEW3D_P
+0034f230: 545f 616e 6e6f 7461 7469 6f6e 5f6f 6e69  T_annotation_oni
+0034f240: 6f6e 3a20 2762 6c5f 7569 2e73 7061 6365  on: 'bl_ui.space
+0034f250: 5f76 6965 7733 642e 5649 4557 3344 5f50  _view3d.VIEW3D_P
+0034f260: 545f 616e 6e6f 7461 7469 6f6e 5f6f 6e69  T_annotation_oni
+0034f270: 6f6e 2720 3d20 4e6f 6e65 0a0a 5649 4557  on' = None..VIEW
+0034f280: 3344 5f50 545f 636f 6c6c 6563 7469 6f6e  3D_PT_collection
+0034f290: 733a 2027 626c 5f75 692e 7370 6163 655f  s: 'bl_ui.space_
+0034f2a0: 7669 6577 3364 2e56 4945 5733 445f 5054  view3d.VIEW3D_PT
+0034f2b0: 5f63 6f6c 6c65 6374 696f 6e73 2720 3d20  _collections' = 
+0034f2c0: 4e6f 6e65 0a0a 5649 4557 3344 5f50 545f  None..VIEW3D_PT_
+0034f2d0: 636f 6e74 6578 745f 7072 6f70 6572 7469  context_properti
+0034f2e0: 6573 3a20 2762 6c5f 7569 2e73 7061 6365  es: 'bl_ui.space
+0034f2f0: 5f76 6965 7733 642e 5649 4557 3344 5f50  _view3d.VIEW3D_P
+0034f300: 545f 636f 6e74 6578 745f 7072 6f70 6572  T_context_proper
+0034f310: 7469 6573 2720 3d20 4e6f 6e65 0a0a 5649  ties' = None..VI
+0034f320: 4557 3344 5f50 545f 6375 7276 6573 5f73  EW3D_PT_curves_s
+0034f330: 6375 6c70 745f 6164 645f 7368 6170 653a  culpt_add_shape:
+0034f340: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
+0034f350: 6577 3364 2e56 4945 5733 445f 5054 5f63  ew3d.VIEW3D_PT_c
+0034f360: 7572 7665 735f 7363 756c 7074 5f61 6464  urves_sculpt_add
+0034f370: 5f73 6861 7065 2720 3d20 4e6f 6e65 0a0a  _shape' = None..
+0034f380: 5649 4557 3344 5f50 545f 6375 7276 6573  VIEW3D_PT_curves
+0034f390: 5f73 6375 6c70 745f 6772 6f77 5f73 6872  _sculpt_grow_shr
+0034f3a0: 696e 6b5f 7363 616c 696e 673a 2027 626c  ink_scaling: 'bl
+0034f3b0: 5f75 692e 7370 6163 655f 7669 6577 3364  _ui.space_view3d
+0034f3c0: 2e56 4945 5733 445f 5054 5f63 7572 7665  .VIEW3D_PT_curve
+0034f3d0: 735f 7363 756c 7074 5f67 726f 775f 7368  s_sculpt_grow_sh
+0034f3e0: 7269 6e6b 5f73 6361 6c69 6e67 2720 3d20  rink_scaling' = 
+0034f3f0: 4e6f 6e65 0a0a 5649 4557 3344 5f50 545f  None..VIEW3D_PT_
+0034f400: 6375 7276 6573 5f73 6375 6c70 745f 7061  curves_sculpt_pa
+0034f410: 7261 6d65 7465 725f 6661 6c6c 6f66 663a  rameter_falloff:
+0034f420: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
+0034f430: 6577 3364 2e56 4945 5733 445f 5054 5f63  ew3d.VIEW3D_PT_c
+0034f440: 7572 7665 735f 7363 756c 7074 5f70 6172  urves_sculpt_par
+0034f450: 616d 6574 6572 5f66 616c 6c6f 6666 2720  ameter_falloff' 
+0034f460: 3d20 4e6f 6e65 0a0a 5649 4557 3344 5f50  = None..VIEW3D_P
+0034f470: 545f 6375 7276 6573 5f73 6375 6c70 745f  T_curves_sculpt_
+0034f480: 7379 6d6d 6574 7279 3a20 2762 6c5f 7569  symmetry: 'bl_ui
+0034f490: 2e73 7061 6365 5f76 6965 7733 645f 746f  .space_view3d_to
+0034f4a0: 6f6c 6261 722e 5649 4557 3344 5f50 545f  olbar.VIEW3D_PT_
+0034f4b0: 6375 7276 6573 5f73 6375 6c70 745f 7379  curves_sculpt_sy
+0034f4c0: 6d6d 6574 7279 2720 3d20 4e6f 6e65 0a0a  mmetry' = None..
+0034f4d0: 5649 4557 3344 5f50 545f 6375 7276 6573  VIEW3D_PT_curves
+0034f4e0: 5f73 6375 6c70 745f 7379 6d6d 6574 7279  _sculpt_symmetry
+0034f4f0: 5f66 6f72 5f74 6f70 6261 723a 2027 626c  _for_topbar: 'bl
+0034f500: 5f75 692e 7370 6163 655f 7669 6577 3364  _ui.space_view3d
+0034f510: 5f74 6f6f 6c62 6172 2e56 4945 5733 445f  _toolbar.VIEW3D_
+0034f520: 5054 5f63 7572 7665 735f 7363 756c 7074  PT_curves_sculpt
+0034f530: 5f73 796d 6d65 7472 795f 666f 725f 746f  _symmetry_for_to
+0034f540: 7062 6172 2720 3d20 4e6f 6e65 0a0a 5649  pbar' = None..VI
+0034f550: 4557 3344 5f50 545f 6769 7a6d 6f5f 6469  EW3D_PT_gizmo_di
+0034f560: 7370 6c61 793a 2027 626c 5f75 692e 7370  splay: 'bl_ui.sp
+0034f570: 6163 655f 7669 6577 3364 2e56 4945 5733  ace_view3d.VIEW3
+0034f580: 445f 5054 5f67 697a 6d6f 5f64 6973 706c  D_PT_gizmo_displ
+0034f590: 6179 2720 3d20 4e6f 6e65 0a0a 5649 4557  ay' = None..VIEW
+0034f5a0: 3344 5f50 545f 6770 656e 6369 6c5f 6272  3D_PT_gpencil_br
+0034f5b0: 7573 685f 7072 6573 6574 733a 2027 626c  ush_presets: 'bl
+0034f5c0: 5f75 692e 7370 6163 655f 7669 6577 3364  _ui.space_view3d
+0034f5d0: 5f74 6f6f 6c62 6172 2e56 4945 5733 445f  _toolbar.VIEW3D_
+0034f5e0: 5054 5f67 7065 6e63 696c 5f62 7275 7368  PT_gpencil_brush
+0034f5f0: 5f70 7265 7365 7473 2720 3d20 4e6f 6e65  _presets' = None
+0034f600: 0a0a 5649 4557 3344 5f50 545f 6770 656e  ..VIEW3D_PT_gpen
+0034f610: 6369 6c5f 6375 7276 655f 6564 6974 3a20  cil_curve_edit: 
+0034f620: 2762 6c5f 7569 2e73 7061 6365 5f76 6965  'bl_ui.space_vie
+0034f630: 7733 642e 5649 4557 3344 5f50 545f 6770  w3d.VIEW3D_PT_gp
+0034f640: 656e 6369 6c5f 6375 7276 655f 6564 6974  encil_curve_edit
 0034f650: 2720 3d20 4e6f 6e65 0a0a 5649 4557 3344  ' = None..VIEW3D
-0034f660: 5f50 545f 6770 656e 6369 6c5f 6775 6964  _PT_gpencil_guid
-0034f670: 653a 2027 626c 5f75 692e 7370 6163 655f  e: 'bl_ui.space_
-0034f680: 7669 6577 3364 2e56 4945 5733 445f 5054  view3d.VIEW3D_PT
-0034f690: 5f67 7065 6e63 696c 5f67 7569 6465 2720  _gpencil_guide' 
-0034f6a0: 3d20 4e6f 6e65 0a0a 5649 4557 3344 5f50  = None..VIEW3D_P
-0034f6b0: 545f 6770 656e 6369 6c5f 6c6f 636b 3a20  T_gpencil_lock: 
-0034f6c0: 2762 6c5f 7569 2e73 7061 6365 5f76 6965  'bl_ui.space_vie
-0034f6d0: 7733 642e 5649 4557 3344 5f50 545f 6770  w3d.VIEW3D_PT_gp
-0034f6e0: 656e 6369 6c5f 6c6f 636b 2720 3d20 4e6f  encil_lock' = No
-0034f6f0: 6e65 0a0a 5649 4557 3344 5f50 545f 6770  ne..VIEW3D_PT_gp
-0034f700: 656e 6369 6c5f 6d75 6c74 695f 6672 616d  encil_multi_fram
-0034f710: 653a 2027 626c 5f75 692e 7370 6163 655f  e: 'bl_ui.space_
-0034f720: 7669 6577 3364 2e56 4945 5733 445f 5054  view3d.VIEW3D_PT
-0034f730: 5f67 7065 6e63 696c 5f6d 756c 7469 5f66  _gpencil_multi_f
-0034f740: 7261 6d65 2720 3d20 4e6f 6e65 0a0a 5649  rame' = None..VI
-0034f750: 4557 3344 5f50 545f 6770 656e 6369 6c5f  EW3D_PT_gpencil_
-0034f760: 6f72 6967 696e 3a20 2762 6c5f 7569 2e73  origin: 'bl_ui.s
-0034f770: 7061 6365 5f76 6965 7733 642e 5649 4557  pace_view3d.VIEW
-0034f780: 3344 5f50 545f 6770 656e 6369 6c5f 6f72  3D_PT_gpencil_or
-0034f790: 6967 696e 2720 3d20 4e6f 6e65 0a0a 5649  igin' = None..VI
-0034f7a0: 4557 3344 5f50 545f 6770 656e 6369 6c5f  EW3D_PT_gpencil_
-0034f7b0: 7363 756c 7074 5f61 7574 6f6d 6173 6b69  sculpt_automaski
-0034f7c0: 6e67 3a20 2762 6c5f 7569 2e73 7061 6365  ng: 'bl_ui.space
-0034f7d0: 5f76 6965 7733 642e 5649 4557 3344 5f50  _view3d.VIEW3D_P
-0034f7e0: 545f 6770 656e 6369 6c5f 7363 756c 7074  T_gpencil_sculpt
-0034f7f0: 5f61 7574 6f6d 6173 6b69 6e67 2720 3d20  _automasking' = 
-0034f800: 4e6f 6e65 0a0a 5649 4557 3344 5f50 545f  None..VIEW3D_PT_
-0034f810: 6770 656e 6369 6c5f 7363 756c 7074 5f63  gpencil_sculpt_c
-0034f820: 6f6e 7465 7874 5f6d 656e 753a 2027 626c  ontext_menu: 'bl
-0034f830: 5f75 692e 7370 6163 655f 7669 6577 3364  _ui.space_view3d
-0034f840: 2e56 4945 5733 445f 5054 5f67 7065 6e63  .VIEW3D_PT_gpenc
-0034f850: 696c 5f73 6375 6c70 745f 636f 6e74 6578  il_sculpt_contex
-0034f860: 745f 6d65 6e75 2720 3d20 4e6f 6e65 0a0a  t_menu' = None..
-0034f870: 5649 4557 3344 5f50 545f 6770 656e 6369  VIEW3D_PT_gpenci
-0034f880: 6c5f 7665 7274 6578 5f63 6f6e 7465 7874  l_vertex_context
-0034f890: 5f6d 656e 753a 2027 626c 5f75 692e 7370  _menu: 'bl_ui.sp
-0034f8a0: 6163 655f 7669 6577 3364 2e56 4945 5733  ace_view3d.VIEW3
-0034f8b0: 445f 5054 5f67 7065 6e63 696c 5f76 6572  D_PT_gpencil_ver
-0034f8c0: 7465 785f 636f 6e74 6578 745f 6d65 6e75  tex_context_menu
-0034f8d0: 2720 3d20 4e6f 6e65 0a0a 5649 4557 3344  ' = None..VIEW3D
-0034f8e0: 5f50 545f 6770 656e 6369 6c5f 7765 6967  _PT_gpencil_weig
-0034f8f0: 6874 5f63 6f6e 7465 7874 5f6d 656e 753a  ht_context_menu:
-0034f900: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
-0034f910: 6577 3364 2e56 4945 5733 445f 5054 5f67  ew3d.VIEW3D_PT_g
-0034f920: 7065 6e63 696c 5f77 6569 6768 745f 636f  pencil_weight_co
-0034f930: 6e74 6578 745f 6d65 6e75 2720 3d20 4e6f  ntext_menu' = No
-0034f940: 6e65 0a0a 5649 4557 3344 5f50 545f 6772  ne..VIEW3D_PT_gr
-0034f950: 6561 7365 5f70 656e 6369 6c3a 2027 626c  ease_pencil: 'bl
-0034f960: 5f75 692e 7370 6163 655f 7669 6577 3364  _ui.space_view3d
-0034f970: 2e56 4945 5733 445f 5054 5f67 7265 6173  .VIEW3D_PT_greas
-0034f980: 655f 7065 6e63 696c 2720 3d20 4e6f 6e65  e_pencil' = None
-0034f990: 0a0a 5649 4557 3344 5f50 545f 6d61 736b  ..VIEW3D_PT_mask
-0034f9a0: 3a20 2762 6c5f 7569 2e73 7061 6365 5f76  : 'bl_ui.space_v
-0034f9b0: 6965 7733 645f 746f 6f6c 6261 722e 5649  iew3d_toolbar.VI
-0034f9c0: 4557 3344 5f50 545f 6d61 736b 2720 3d20  EW3D_PT_mask' = 
-0034f9d0: 4e6f 6e65 0a0a 5649 4557 3344 5f50 545f  None..VIEW3D_PT_
-0034f9e0: 6f62 6a65 6374 5f74 7970 655f 7669 7369  object_type_visi
-0034f9f0: 6269 6c69 7479 3a20 2762 6c5f 7569 2e73  bility: 'bl_ui.s
-0034fa00: 7061 6365 5f76 6965 7733 642e 5649 4557  pace_view3d.VIEW
-0034fa10: 3344 5f50 545f 6f62 6a65 6374 5f74 7970  3D_PT_object_typ
-0034fa20: 655f 7669 7369 6269 6c69 7479 2720 3d20  e_visibility' = 
-0034fa30: 4e6f 6e65 0a0a 5649 4557 3344 5f50 545f  None..VIEW3D_PT_
-0034fa40: 6f76 6572 6c61 793a 2027 626c 5f75 692e  overlay: 'bl_ui.
-0034fa50: 7370 6163 655f 7669 6577 3364 2e56 4945  space_view3d.VIE
-0034fa60: 5733 445f 5054 5f6f 7665 726c 6179 2720  W3D_PT_overlay' 
-0034fa70: 3d20 4e6f 6e65 0a0a 5649 4557 3344 5f50  = None..VIEW3D_P
-0034fa80: 545f 6f76 6572 6c61 795f 626f 6e65 733a  T_overlay_bones:
-0034fa90: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
-0034faa0: 6577 3364 2e56 4945 5733 445f 5054 5f6f  ew3d.VIEW3D_PT_o
-0034fab0: 7665 726c 6179 5f62 6f6e 6573 2720 3d20  verlay_bones' = 
-0034fac0: 4e6f 6e65 0a0a 5649 4557 3344 5f50 545f  None..VIEW3D_PT_
-0034fad0: 6f76 6572 6c61 795f 6564 6974 5f63 7572  overlay_edit_cur
-0034fae0: 7665 3a20 2762 6c5f 7569 2e73 7061 6365  ve: 'bl_ui.space
-0034faf0: 5f76 6965 7733 642e 5649 4557 3344 5f50  _view3d.VIEW3D_P
-0034fb00: 545f 6f76 6572 6c61 795f 6564 6974 5f63  T_overlay_edit_c
-0034fb10: 7572 7665 2720 3d20 4e6f 6e65 0a0a 5649  urve' = None..VI
-0034fb20: 4557 3344 5f50 545f 6f76 6572 6c61 795f  EW3D_PT_overlay_
-0034fb30: 6564 6974 5f6d 6573 683a 2027 626c 5f75  edit_mesh: 'bl_u
-0034fb40: 692e 7370 6163 655f 7669 6577 3364 2e56  i.space_view3d.V
-0034fb50: 4945 5733 445f 5054 5f6f 7665 726c 6179  IEW3D_PT_overlay
-0034fb60: 5f65 6469 745f 6d65 7368 2720 3d20 4e6f  _edit_mesh' = No
-0034fb70: 6e65 0a0a 5649 4557 3344 5f50 545f 6f76  ne..VIEW3D_PT_ov
-0034fb80: 6572 6c61 795f 6564 6974 5f6d 6573 685f  erlay_edit_mesh_
-0034fb90: 6672 6565 7374 796c 653a 2027 626c 5f75  freestyle: 'bl_u
-0034fba0: 692e 7370 6163 655f 7669 6577 3364 2e56  i.space_view3d.V
-0034fbb0: 4945 5733 445f 5054 5f6f 7665 726c 6179  IEW3D_PT_overlay
-0034fbc0: 5f65 6469 745f 6d65 7368 5f66 7265 6573  _edit_mesh_frees
-0034fbd0: 7479 6c65 2720 3d20 4e6f 6e65 0a0a 5649  tyle' = None..VI
-0034fbe0: 4557 3344 5f50 545f 6f76 6572 6c61 795f  EW3D_PT_overlay_
-0034fbf0: 6564 6974 5f6d 6573 685f 6d65 6173 7572  edit_mesh_measur
-0034fc00: 656d 656e 743a 2027 626c 5f75 692e 7370  ement: 'bl_ui.sp
-0034fc10: 6163 655f 7669 6577 3364 2e56 4945 5733  ace_view3d.VIEW3
-0034fc20: 445f 5054 5f6f 7665 726c 6179 5f65 6469  D_PT_overlay_edi
-0034fc30: 745f 6d65 7368 5f6d 6561 7375 7265 6d65  t_mesh_measureme
-0034fc40: 6e74 2720 3d20 4e6f 6e65 0a0a 5649 4557  nt' = None..VIEW
-0034fc50: 3344 5f50 545f 6f76 6572 6c61 795f 6564  3D_PT_overlay_ed
-0034fc60: 6974 5f6d 6573 685f 6e6f 726d 616c 733a  it_mesh_normals:
-0034fc70: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
-0034fc80: 6577 3364 2e56 4945 5733 445f 5054 5f6f  ew3d.VIEW3D_PT_o
-0034fc90: 7665 726c 6179 5f65 6469 745f 6d65 7368  verlay_edit_mesh
-0034fca0: 5f6e 6f72 6d61 6c73 2720 3d20 4e6f 6e65  _normals' = None
+0034f660: 5f50 545f 6770 656e 6369 6c5f 6472 6177  _PT_gpencil_draw
+0034f670: 5f63 6f6e 7465 7874 5f6d 656e 753a 2027  _context_menu: '
+0034f680: 626c 5f75 692e 7370 6163 655f 7669 6577  bl_ui.space_view
+0034f690: 3364 2e56 4945 5733 445f 5054 5f67 7065  3d.VIEW3D_PT_gpe
+0034f6a0: 6e63 696c 5f64 7261 775f 636f 6e74 6578  ncil_draw_contex
+0034f6b0: 745f 6d65 6e75 2720 3d20 4e6f 6e65 0a0a  t_menu' = None..
+0034f6c0: 5649 4557 3344 5f50 545f 6770 656e 6369  VIEW3D_PT_gpenci
+0034f6d0: 6c5f 6775 6964 653a 2027 626c 5f75 692e  l_guide: 'bl_ui.
+0034f6e0: 7370 6163 655f 7669 6577 3364 2e56 4945  space_view3d.VIE
+0034f6f0: 5733 445f 5054 5f67 7065 6e63 696c 5f67  W3D_PT_gpencil_g
+0034f700: 7569 6465 2720 3d20 4e6f 6e65 0a0a 5649  uide' = None..VI
+0034f710: 4557 3344 5f50 545f 6770 656e 6369 6c5f  EW3D_PT_gpencil_
+0034f720: 6c6f 636b 3a20 2762 6c5f 7569 2e73 7061  lock: 'bl_ui.spa
+0034f730: 6365 5f76 6965 7733 642e 5649 4557 3344  ce_view3d.VIEW3D
+0034f740: 5f50 545f 6770 656e 6369 6c5f 6c6f 636b  _PT_gpencil_lock
+0034f750: 2720 3d20 4e6f 6e65 0a0a 5649 4557 3344  ' = None..VIEW3D
+0034f760: 5f50 545f 6770 656e 6369 6c5f 6d75 6c74  _PT_gpencil_mult
+0034f770: 695f 6672 616d 653a 2027 626c 5f75 692e  i_frame: 'bl_ui.
+0034f780: 7370 6163 655f 7669 6577 3364 2e56 4945  space_view3d.VIE
+0034f790: 5733 445f 5054 5f67 7065 6e63 696c 5f6d  W3D_PT_gpencil_m
+0034f7a0: 756c 7469 5f66 7261 6d65 2720 3d20 4e6f  ulti_frame' = No
+0034f7b0: 6e65 0a0a 5649 4557 3344 5f50 545f 6770  ne..VIEW3D_PT_gp
+0034f7c0: 656e 6369 6c5f 6f72 6967 696e 3a20 2762  encil_origin: 'b
+0034f7d0: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
+0034f7e0: 642e 5649 4557 3344 5f50 545f 6770 656e  d.VIEW3D_PT_gpen
+0034f7f0: 6369 6c5f 6f72 6967 696e 2720 3d20 4e6f  cil_origin' = No
+0034f800: 6e65 0a0a 5649 4557 3344 5f50 545f 6770  ne..VIEW3D_PT_gp
+0034f810: 656e 6369 6c5f 7363 756c 7074 5f61 7574  encil_sculpt_aut
+0034f820: 6f6d 6173 6b69 6e67 3a20 2762 6c5f 7569  omasking: 'bl_ui
+0034f830: 2e73 7061 6365 5f76 6965 7733 642e 5649  .space_view3d.VI
+0034f840: 4557 3344 5f50 545f 6770 656e 6369 6c5f  EW3D_PT_gpencil_
+0034f850: 7363 756c 7074 5f61 7574 6f6d 6173 6b69  sculpt_automaski
+0034f860: 6e67 2720 3d20 4e6f 6e65 0a0a 5649 4557  ng' = None..VIEW
+0034f870: 3344 5f50 545f 6770 656e 6369 6c5f 7363  3D_PT_gpencil_sc
+0034f880: 756c 7074 5f63 6f6e 7465 7874 5f6d 656e  ulpt_context_men
+0034f890: 753a 2027 626c 5f75 692e 7370 6163 655f  u: 'bl_ui.space_
+0034f8a0: 7669 6577 3364 2e56 4945 5733 445f 5054  view3d.VIEW3D_PT
+0034f8b0: 5f67 7065 6e63 696c 5f73 6375 6c70 745f  _gpencil_sculpt_
+0034f8c0: 636f 6e74 6578 745f 6d65 6e75 2720 3d20  context_menu' = 
+0034f8d0: 4e6f 6e65 0a0a 5649 4557 3344 5f50 545f  None..VIEW3D_PT_
+0034f8e0: 6770 656e 6369 6c5f 7665 7274 6578 5f63  gpencil_vertex_c
+0034f8f0: 6f6e 7465 7874 5f6d 656e 753a 2027 626c  ontext_menu: 'bl
+0034f900: 5f75 692e 7370 6163 655f 7669 6577 3364  _ui.space_view3d
+0034f910: 2e56 4945 5733 445f 5054 5f67 7065 6e63  .VIEW3D_PT_gpenc
+0034f920: 696c 5f76 6572 7465 785f 636f 6e74 6578  il_vertex_contex
+0034f930: 745f 6d65 6e75 2720 3d20 4e6f 6e65 0a0a  t_menu' = None..
+0034f940: 5649 4557 3344 5f50 545f 6770 656e 6369  VIEW3D_PT_gpenci
+0034f950: 6c5f 7765 6967 6874 5f63 6f6e 7465 7874  l_weight_context
+0034f960: 5f6d 656e 753a 2027 626c 5f75 692e 7370  _menu: 'bl_ui.sp
+0034f970: 6163 655f 7669 6577 3364 2e56 4945 5733  ace_view3d.VIEW3
+0034f980: 445f 5054 5f67 7065 6e63 696c 5f77 6569  D_PT_gpencil_wei
+0034f990: 6768 745f 636f 6e74 6578 745f 6d65 6e75  ght_context_menu
+0034f9a0: 2720 3d20 4e6f 6e65 0a0a 5649 4557 3344  ' = None..VIEW3D
+0034f9b0: 5f50 545f 6772 6561 7365 5f70 656e 6369  _PT_grease_penci
+0034f9c0: 6c3a 2027 626c 5f75 692e 7370 6163 655f  l: 'bl_ui.space_
+0034f9d0: 7669 6577 3364 2e56 4945 5733 445f 5054  view3d.VIEW3D_PT
+0034f9e0: 5f67 7265 6173 655f 7065 6e63 696c 2720  _grease_pencil' 
+0034f9f0: 3d20 4e6f 6e65 0a0a 5649 4557 3344 5f50  = None..VIEW3D_P
+0034fa00: 545f 6d61 736b 3a20 2762 6c5f 7569 2e73  T_mask: 'bl_ui.s
+0034fa10: 7061 6365 5f76 6965 7733 645f 746f 6f6c  pace_view3d_tool
+0034fa20: 6261 722e 5649 4557 3344 5f50 545f 6d61  bar.VIEW3D_PT_ma
+0034fa30: 736b 2720 3d20 4e6f 6e65 0a0a 5649 4557  sk' = None..VIEW
+0034fa40: 3344 5f50 545f 6f62 6a65 6374 5f74 7970  3D_PT_object_typ
+0034fa50: 655f 7669 7369 6269 6c69 7479 3a20 2762  e_visibility: 'b
+0034fa60: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
+0034fa70: 642e 5649 4557 3344 5f50 545f 6f62 6a65  d.VIEW3D_PT_obje
+0034fa80: 6374 5f74 7970 655f 7669 7369 6269 6c69  ct_type_visibili
+0034fa90: 7479 2720 3d20 4e6f 6e65 0a0a 5649 4557  ty' = None..VIEW
+0034faa0: 3344 5f50 545f 6f76 6572 6c61 793a 2027  3D_PT_overlay: '
+0034fab0: 626c 5f75 692e 7370 6163 655f 7669 6577  bl_ui.space_view
+0034fac0: 3364 2e56 4945 5733 445f 5054 5f6f 7665  3d.VIEW3D_PT_ove
+0034fad0: 726c 6179 2720 3d20 4e6f 6e65 0a0a 5649  rlay' = None..VI
+0034fae0: 4557 3344 5f50 545f 6f76 6572 6c61 795f  EW3D_PT_overlay_
+0034faf0: 626f 6e65 733a 2027 626c 5f75 692e 7370  bones: 'bl_ui.sp
+0034fb00: 6163 655f 7669 6577 3364 2e56 4945 5733  ace_view3d.VIEW3
+0034fb10: 445f 5054 5f6f 7665 726c 6179 5f62 6f6e  D_PT_overlay_bon
+0034fb20: 6573 2720 3d20 4e6f 6e65 0a0a 5649 4557  es' = None..VIEW
+0034fb30: 3344 5f50 545f 6f76 6572 6c61 795f 6564  3D_PT_overlay_ed
+0034fb40: 6974 5f63 7572 7665 3a20 2762 6c5f 7569  it_curve: 'bl_ui
+0034fb50: 2e73 7061 6365 5f76 6965 7733 642e 5649  .space_view3d.VI
+0034fb60: 4557 3344 5f50 545f 6f76 6572 6c61 795f  EW3D_PT_overlay_
+0034fb70: 6564 6974 5f63 7572 7665 2720 3d20 4e6f  edit_curve' = No
+0034fb80: 6e65 0a0a 5649 4557 3344 5f50 545f 6f76  ne..VIEW3D_PT_ov
+0034fb90: 6572 6c61 795f 6564 6974 5f6d 6573 683a  erlay_edit_mesh:
+0034fba0: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
+0034fbb0: 6577 3364 2e56 4945 5733 445f 5054 5f6f  ew3d.VIEW3D_PT_o
+0034fbc0: 7665 726c 6179 5f65 6469 745f 6d65 7368  verlay_edit_mesh
+0034fbd0: 2720 3d20 4e6f 6e65 0a0a 5649 4557 3344  ' = None..VIEW3D
+0034fbe0: 5f50 545f 6f76 6572 6c61 795f 6564 6974  _PT_overlay_edit
+0034fbf0: 5f6d 6573 685f 6672 6565 7374 796c 653a  _mesh_freestyle:
+0034fc00: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
+0034fc10: 6577 3364 2e56 4945 5733 445f 5054 5f6f  ew3d.VIEW3D_PT_o
+0034fc20: 7665 726c 6179 5f65 6469 745f 6d65 7368  verlay_edit_mesh
+0034fc30: 5f66 7265 6573 7479 6c65 2720 3d20 4e6f  _freestyle' = No
+0034fc40: 6e65 0a0a 5649 4557 3344 5f50 545f 6f76  ne..VIEW3D_PT_ov
+0034fc50: 6572 6c61 795f 6564 6974 5f6d 6573 685f  erlay_edit_mesh_
+0034fc60: 6d65 6173 7572 656d 656e 743a 2027 626c  measurement: 'bl
+0034fc70: 5f75 692e 7370 6163 655f 7669 6577 3364  _ui.space_view3d
+0034fc80: 2e56 4945 5733 445f 5054 5f6f 7665 726c  .VIEW3D_PT_overl
+0034fc90: 6179 5f65 6469 745f 6d65 7368 5f6d 6561  ay_edit_mesh_mea
+0034fca0: 7375 7265 6d65 6e74 2720 3d20 4e6f 6e65  surement' = None
 0034fcb0: 0a0a 5649 4557 3344 5f50 545f 6f76 6572  ..VIEW3D_PT_over
-0034fcc0: 6c61 795f 6564 6974 5f6d 6573 685f 7368  lay_edit_mesh_sh
-0034fcd0: 6164 696e 673a 2027 626c 5f75 692e 7370  ading: 'bl_ui.sp
+0034fcc0: 6c61 795f 6564 6974 5f6d 6573 685f 6e6f  lay_edit_mesh_no
+0034fcd0: 726d 616c 733a 2027 626c 5f75 692e 7370  rmals: 'bl_ui.sp
 0034fce0: 6163 655f 7669 6577 3364 2e56 4945 5733  ace_view3d.VIEW3
 0034fcf0: 445f 5054 5f6f 7665 726c 6179 5f65 6469  D_PT_overlay_edi
-0034fd00: 745f 6d65 7368 5f73 6861 6469 6e67 2720  t_mesh_shading' 
+0034fd00: 745f 6d65 7368 5f6e 6f72 6d61 6c73 2720  t_mesh_normals' 
 0034fd10: 3d20 4e6f 6e65 0a0a 5649 4557 3344 5f50  = None..VIEW3D_P
-0034fd20: 545f 6f76 6572 6c61 795f 6765 6f6d 6574  T_overlay_geomet
-0034fd30: 7279 3a20 2762 6c5f 7569 2e73 7061 6365  ry: 'bl_ui.space
-0034fd40: 5f76 6965 7733 642e 5649 4557 3344 5f50  _view3d.VIEW3D_P
-0034fd50: 545f 6f76 6572 6c61 795f 6765 6f6d 6574  T_overlay_geomet
-0034fd60: 7279 2720 3d20 4e6f 6e65 0a0a 5649 4557  ry' = None..VIEW
-0034fd70: 3344 5f50 545f 6f76 6572 6c61 795f 6770  3D_PT_overlay_gp
-0034fd80: 656e 6369 6c5f 6f70 7469 6f6e 733a 2027  encil_options: '
-0034fd90: 626c 5f75 692e 7370 6163 655f 7669 6577  bl_ui.space_view
-0034fda0: 3364 2e56 4945 5733 445f 5054 5f6f 7665  3d.VIEW3D_PT_ove
-0034fdb0: 726c 6179 5f67 7065 6e63 696c 5f6f 7074  rlay_gpencil_opt
-0034fdc0: 696f 6e73 2720 3d20 4e6f 6e65 0a0a 5649  ions' = None..VI
-0034fdd0: 4557 3344 5f50 545f 6f76 6572 6c61 795f  EW3D_PT_overlay_
-0034fde0: 6775 6964 6573 3a20 2762 6c5f 7569 2e73  guides: 'bl_ui.s
-0034fdf0: 7061 6365 5f76 6965 7733 642e 5649 4557  pace_view3d.VIEW
-0034fe00: 3344 5f50 545f 6f76 6572 6c61 795f 6775  3D_PT_overlay_gu
-0034fe10: 6964 6573 2720 3d20 4e6f 6e65 0a0a 5649  ides' = None..VI
-0034fe20: 4557 3344 5f50 545f 6f76 6572 6c61 795f  EW3D_PT_overlay_
-0034fe30: 6d6f 7469 6f6e 5f74 7261 636b 696e 673a  motion_tracking:
-0034fe40: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
-0034fe50: 6577 3364 2e56 4945 5733 445f 5054 5f6f  ew3d.VIEW3D_PT_o
-0034fe60: 7665 726c 6179 5f6d 6f74 696f 6e5f 7472  verlay_motion_tr
-0034fe70: 6163 6b69 6e67 2720 3d20 4e6f 6e65 0a0a  acking' = None..
-0034fe80: 5649 4557 3344 5f50 545f 6f76 6572 6c61  VIEW3D_PT_overla
-0034fe90: 795f 6f62 6a65 6374 3a20 2762 6c5f 7569  y_object: 'bl_ui
-0034fea0: 2e73 7061 6365 5f76 6965 7733 642e 5649  .space_view3d.VI
-0034feb0: 4557 3344 5f50 545f 6f76 6572 6c61 795f  EW3D_PT_overlay_
-0034fec0: 6f62 6a65 6374 2720 3d20 4e6f 6e65 0a0a  object' = None..
-0034fed0: 5649 4557 3344 5f50 545f 6f76 6572 6c61  VIEW3D_PT_overla
-0034fee0: 795f 7363 756c 7074 3a20 2762 6c5f 7569  y_sculpt: 'bl_ui
-0034fef0: 2e73 7061 6365 5f76 6965 7733 642e 5649  .space_view3d.VI
-0034ff00: 4557 3344 5f50 545f 6f76 6572 6c61 795f  EW3D_PT_overlay_
-0034ff10: 7363 756c 7074 2720 3d20 4e6f 6e65 0a0a  sculpt' = None..
-0034ff20: 5649 4557 3344 5f50 545f 6f76 6572 6c61  VIEW3D_PT_overla
-0034ff30: 795f 7363 756c 7074 5f63 7572 7665 733a  y_sculpt_curves:
-0034ff40: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
-0034ff50: 6577 3364 2e56 4945 5733 445f 5054 5f6f  ew3d.VIEW3D_PT_o
-0034ff60: 7665 726c 6179 5f73 6375 6c70 745f 6375  verlay_sculpt_cu
-0034ff70: 7276 6573 2720 3d20 4e6f 6e65 0a0a 5649  rves' = None..VI
-0034ff80: 4557 3344 5f50 545f 6f76 6572 6c61 795f  EW3D_PT_overlay_
-0034ff90: 7465 7874 7572 655f 7061 696e 743a 2027  texture_paint: '
-0034ffa0: 626c 5f75 692e 7370 6163 655f 7669 6577  bl_ui.space_view
-0034ffb0: 3364 2e56 4945 5733 445f 5054 5f6f 7665  3d.VIEW3D_PT_ove
-0034ffc0: 726c 6179 5f74 6578 7475 7265 5f70 6169  rlay_texture_pai
-0034ffd0: 6e74 2720 3d20 4e6f 6e65 0a0a 5649 4557  nt' = None..VIEW
-0034ffe0: 3344 5f50 545f 6f76 6572 6c61 795f 7665  3D_PT_overlay_ve
-0034fff0: 7274 6578 5f70 6169 6e74 3a20 2762 6c5f  rtex_paint: 'bl_
-00350000: 7569 2e73 7061 6365 5f76 6965 7733 642e  ui.space_view3d.
-00350010: 5649 4557 3344 5f50 545f 6f76 6572 6c61  VIEW3D_PT_overla
-00350020: 795f 7665 7274 6578 5f70 6169 6e74 2720  y_vertex_paint' 
-00350030: 3d20 4e6f 6e65 0a0a 5649 4557 3344 5f50  = None..VIEW3D_P
-00350040: 545f 6f76 6572 6c61 795f 7765 6967 6874  T_overlay_weight
-00350050: 5f70 6169 6e74 3a20 2762 6c5f 7569 2e73  _paint: 'bl_ui.s
-00350060: 7061 6365 5f76 6965 7733 642e 5649 4557  pace_view3d.VIEW
-00350070: 3344 5f50 545f 6f76 6572 6c61 795f 7765  3D_PT_overlay_we
-00350080: 6967 6874 5f70 6169 6e74 2720 3d20 4e6f  ight_paint' = No
-00350090: 6e65 0a0a 5649 4557 3344 5f50 545f 7061  ne..VIEW3D_PT_pa
-003500a0: 696e 745f 7465 7874 7572 655f 636f 6e74  int_texture_cont
-003500b0: 6578 745f 6d65 6e75 3a20 2762 6c5f 7569  ext_menu: 'bl_ui
-003500c0: 2e73 7061 6365 5f76 6965 7733 642e 5649  .space_view3d.VI
-003500d0: 4557 3344 5f50 545f 7061 696e 745f 7465  EW3D_PT_paint_te
-003500e0: 7874 7572 655f 636f 6e74 6578 745f 6d65  xture_context_me
-003500f0: 6e75 2720 3d20 4e6f 6e65 0a0a 5649 4557  nu' = None..VIEW
-00350100: 3344 5f50 545f 7061 696e 745f 7665 7274  3D_PT_paint_vert
-00350110: 6578 5f63 6f6e 7465 7874 5f6d 656e 753a  ex_context_menu:
-00350120: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
-00350130: 6577 3364 2e56 4945 5733 445f 5054 5f70  ew3d.VIEW3D_PT_p
-00350140: 6169 6e74 5f76 6572 7465 785f 636f 6e74  aint_vertex_cont
+0034fd20: 545f 6f76 6572 6c61 795f 6564 6974 5f6d  T_overlay_edit_m
+0034fd30: 6573 685f 7368 6164 696e 673a 2027 626c  esh_shading: 'bl
+0034fd40: 5f75 692e 7370 6163 655f 7669 6577 3364  _ui.space_view3d
+0034fd50: 2e56 4945 5733 445f 5054 5f6f 7665 726c  .VIEW3D_PT_overl
+0034fd60: 6179 5f65 6469 745f 6d65 7368 5f73 6861  ay_edit_mesh_sha
+0034fd70: 6469 6e67 2720 3d20 4e6f 6e65 0a0a 5649  ding' = None..VI
+0034fd80: 4557 3344 5f50 545f 6f76 6572 6c61 795f  EW3D_PT_overlay_
+0034fd90: 6765 6f6d 6574 7279 3a20 2762 6c5f 7569  geometry: 'bl_ui
+0034fda0: 2e73 7061 6365 5f76 6965 7733 642e 5649  .space_view3d.VI
+0034fdb0: 4557 3344 5f50 545f 6f76 6572 6c61 795f  EW3D_PT_overlay_
+0034fdc0: 6765 6f6d 6574 7279 2720 3d20 4e6f 6e65  geometry' = None
+0034fdd0: 0a0a 5649 4557 3344 5f50 545f 6f76 6572  ..VIEW3D_PT_over
+0034fde0: 6c61 795f 6770 656e 6369 6c5f 6f70 7469  lay_gpencil_opti
+0034fdf0: 6f6e 733a 2027 626c 5f75 692e 7370 6163  ons: 'bl_ui.spac
+0034fe00: 655f 7669 6577 3364 2e56 4945 5733 445f  e_view3d.VIEW3D_
+0034fe10: 5054 5f6f 7665 726c 6179 5f67 7065 6e63  PT_overlay_gpenc
+0034fe20: 696c 5f6f 7074 696f 6e73 2720 3d20 4e6f  il_options' = No
+0034fe30: 6e65 0a0a 5649 4557 3344 5f50 545f 6f76  ne..VIEW3D_PT_ov
+0034fe40: 6572 6c61 795f 6775 6964 6573 3a20 2762  erlay_guides: 'b
+0034fe50: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
+0034fe60: 642e 5649 4557 3344 5f50 545f 6f76 6572  d.VIEW3D_PT_over
+0034fe70: 6c61 795f 6775 6964 6573 2720 3d20 4e6f  lay_guides' = No
+0034fe80: 6e65 0a0a 5649 4557 3344 5f50 545f 6f76  ne..VIEW3D_PT_ov
+0034fe90: 6572 6c61 795f 6d6f 7469 6f6e 5f74 7261  erlay_motion_tra
+0034fea0: 636b 696e 673a 2027 626c 5f75 692e 7370  cking: 'bl_ui.sp
+0034feb0: 6163 655f 7669 6577 3364 2e56 4945 5733  ace_view3d.VIEW3
+0034fec0: 445f 5054 5f6f 7665 726c 6179 5f6d 6f74  D_PT_overlay_mot
+0034fed0: 696f 6e5f 7472 6163 6b69 6e67 2720 3d20  ion_tracking' = 
+0034fee0: 4e6f 6e65 0a0a 5649 4557 3344 5f50 545f  None..VIEW3D_PT_
+0034fef0: 6f76 6572 6c61 795f 6f62 6a65 6374 3a20  overlay_object: 
+0034ff00: 2762 6c5f 7569 2e73 7061 6365 5f76 6965  'bl_ui.space_vie
+0034ff10: 7733 642e 5649 4557 3344 5f50 545f 6f76  w3d.VIEW3D_PT_ov
+0034ff20: 6572 6c61 795f 6f62 6a65 6374 2720 3d20  erlay_object' = 
+0034ff30: 4e6f 6e65 0a0a 5649 4557 3344 5f50 545f  None..VIEW3D_PT_
+0034ff40: 6f76 6572 6c61 795f 7363 756c 7074 3a20  overlay_sculpt: 
+0034ff50: 2762 6c5f 7569 2e73 7061 6365 5f76 6965  'bl_ui.space_vie
+0034ff60: 7733 642e 5649 4557 3344 5f50 545f 6f76  w3d.VIEW3D_PT_ov
+0034ff70: 6572 6c61 795f 7363 756c 7074 2720 3d20  erlay_sculpt' = 
+0034ff80: 4e6f 6e65 0a0a 5649 4557 3344 5f50 545f  None..VIEW3D_PT_
+0034ff90: 6f76 6572 6c61 795f 7363 756c 7074 5f63  overlay_sculpt_c
+0034ffa0: 7572 7665 733a 2027 626c 5f75 692e 7370  urves: 'bl_ui.sp
+0034ffb0: 6163 655f 7669 6577 3364 2e56 4945 5733  ace_view3d.VIEW3
+0034ffc0: 445f 5054 5f6f 7665 726c 6179 5f73 6375  D_PT_overlay_scu
+0034ffd0: 6c70 745f 6375 7276 6573 2720 3d20 4e6f  lpt_curves' = No
+0034ffe0: 6e65 0a0a 5649 4557 3344 5f50 545f 6f76  ne..VIEW3D_PT_ov
+0034fff0: 6572 6c61 795f 7465 7874 7572 655f 7061  erlay_texture_pa
+00350000: 696e 743a 2027 626c 5f75 692e 7370 6163  int: 'bl_ui.spac
+00350010: 655f 7669 6577 3364 2e56 4945 5733 445f  e_view3d.VIEW3D_
+00350020: 5054 5f6f 7665 726c 6179 5f74 6578 7475  PT_overlay_textu
+00350030: 7265 5f70 6169 6e74 2720 3d20 4e6f 6e65  re_paint' = None
+00350040: 0a0a 5649 4557 3344 5f50 545f 6f76 6572  ..VIEW3D_PT_over
+00350050: 6c61 795f 7665 7274 6578 5f70 6169 6e74  lay_vertex_paint
+00350060: 3a20 2762 6c5f 7569 2e73 7061 6365 5f76  : 'bl_ui.space_v
+00350070: 6965 7733 642e 5649 4557 3344 5f50 545f  iew3d.VIEW3D_PT_
+00350080: 6f76 6572 6c61 795f 7665 7274 6578 5f70  overlay_vertex_p
+00350090: 6169 6e74 2720 3d20 4e6f 6e65 0a0a 5649  aint' = None..VI
+003500a0: 4557 3344 5f50 545f 6f76 6572 6c61 795f  EW3D_PT_overlay_
+003500b0: 7765 6967 6874 5f70 6169 6e74 3a20 2762  weight_paint: 'b
+003500c0: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
+003500d0: 642e 5649 4557 3344 5f50 545f 6f76 6572  d.VIEW3D_PT_over
+003500e0: 6c61 795f 7765 6967 6874 5f70 6169 6e74  lay_weight_paint
+003500f0: 2720 3d20 4e6f 6e65 0a0a 5649 4557 3344  ' = None..VIEW3D
+00350100: 5f50 545f 7061 696e 745f 7465 7874 7572  _PT_paint_textur
+00350110: 655f 636f 6e74 6578 745f 6d65 6e75 3a20  e_context_menu: 
+00350120: 2762 6c5f 7569 2e73 7061 6365 5f76 6965  'bl_ui.space_vie
+00350130: 7733 642e 5649 4557 3344 5f50 545f 7061  w3d.VIEW3D_PT_pa
+00350140: 696e 745f 7465 7874 7572 655f 636f 6e74  int_texture_cont
 00350150: 6578 745f 6d65 6e75 2720 3d20 4e6f 6e65  ext_menu' = None
 00350160: 0a0a 5649 4557 3344 5f50 545f 7061 696e  ..VIEW3D_PT_pain
-00350170: 745f 7765 6967 6874 5f63 6f6e 7465 7874  t_weight_context
+00350170: 745f 7665 7274 6578 5f63 6f6e 7465 7874  t_vertex_context
 00350180: 5f6d 656e 753a 2027 626c 5f75 692e 7370  _menu: 'bl_ui.sp
 00350190: 6163 655f 7669 6577 3364 2e56 4945 5733  ace_view3d.VIEW3
-003501a0: 445f 5054 5f70 6169 6e74 5f77 6569 6768  D_PT_paint_weigh
-003501b0: 745f 636f 6e74 6578 745f 6d65 6e75 2720  t_context_menu' 
+003501a0: 445f 5054 5f70 6169 6e74 5f76 6572 7465  D_PT_paint_verte
+003501b0: 785f 636f 6e74 6578 745f 6d65 6e75 2720  x_context_menu' 
 003501c0: 3d20 4e6f 6e65 0a0a 5649 4557 3344 5f50  = None..VIEW3D_P
-003501d0: 545f 7072 6f70 6f72 7469 6f6e 616c 5f65  T_proportional_e
-003501e0: 6469 743a 2027 626c 5f75 692e 7370 6163  dit: 'bl_ui.spac
-003501f0: 655f 7669 6577 3364 2e56 4945 5733 445f  e_view3d.VIEW3D_
-00350200: 5054 5f70 726f 706f 7274 696f 6e61 6c5f  PT_proportional_
-00350210: 6564 6974 2720 3d20 4e6f 6e65 0a0a 5649  edit' = None..VI
-00350220: 4557 3344 5f50 545f 7175 6164 5f76 6965  EW3D_PT_quad_vie
-00350230: 773a 2027 626c 5f75 692e 7370 6163 655f  w: 'bl_ui.space_
-00350240: 7669 6577 3364 2e56 4945 5733 445f 5054  view3d.VIEW3D_PT
-00350250: 5f71 7561 645f 7669 6577 2720 3d20 4e6f  _quad_view' = No
-00350260: 6e65 0a0a 5649 4557 3344 5f50 545f 7363  ne..VIEW3D_PT_sc
-00350270: 756c 7074 5f61 7574 6f6d 6173 6b69 6e67  ulpt_automasking
-00350280: 3a20 2762 6c5f 7569 2e73 7061 6365 5f76  : 'bl_ui.space_v
-00350290: 6965 7733 642e 5649 4557 3344 5f50 545f  iew3d.VIEW3D_PT_
-003502a0: 7363 756c 7074 5f61 7574 6f6d 6173 6b69  sculpt_automaski
-003502b0: 6e67 2720 3d20 4e6f 6e65 0a0a 5649 4557  ng' = None..VIEW
-003502c0: 3344 5f50 545f 7363 756c 7074 5f63 6f6e  3D_PT_sculpt_con
-003502d0: 7465 7874 5f6d 656e 753a 2027 626c 5f75  text_menu: 'bl_u
-003502e0: 692e 7370 6163 655f 7669 6577 3364 2e56  i.space_view3d.V
-003502f0: 4945 5733 445f 5054 5f73 6375 6c70 745f  IEW3D_PT_sculpt_
-00350300: 636f 6e74 6578 745f 6d65 6e75 2720 3d20  context_menu' = 
-00350310: 4e6f 6e65 0a0a 5649 4557 3344 5f50 545f  None..VIEW3D_PT_
-00350320: 7363 756c 7074 5f64 796e 746f 706f 3a20  sculpt_dyntopo: 
-00350330: 2762 6c5f 7569 2e73 7061 6365 5f76 6965  'bl_ui.space_vie
-00350340: 7733 645f 746f 6f6c 6261 722e 5649 4557  w3d_toolbar.VIEW
-00350350: 3344 5f50 545f 7363 756c 7074 5f64 796e  3D_PT_sculpt_dyn
-00350360: 746f 706f 2720 3d20 4e6f 6e65 0a0a 5649  topo' = None..VI
-00350370: 4557 3344 5f50 545f 7363 756c 7074 5f6f  EW3D_PT_sculpt_o
-00350380: 7074 696f 6e73 3a20 2762 6c5f 7569 2e73  ptions: 'bl_ui.s
-00350390: 7061 6365 5f76 6965 7733 645f 746f 6f6c  pace_view3d_tool
-003503a0: 6261 722e 5649 4557 3344 5f50 545f 7363  bar.VIEW3D_PT_sc
-003503b0: 756c 7074 5f6f 7074 696f 6e73 2720 3d20  ulpt_options' = 
-003503c0: 4e6f 6e65 0a0a 5649 4557 3344 5f50 545f  None..VIEW3D_PT_
-003503d0: 7363 756c 7074 5f6f 7074 696f 6e73 5f67  sculpt_options_g
-003503e0: 7261 7669 7479 3a20 2762 6c5f 7569 2e73  ravity: 'bl_ui.s
-003503f0: 7061 6365 5f76 6965 7733 645f 746f 6f6c  pace_view3d_tool
-00350400: 6261 722e 5649 4557 3344 5f50 545f 7363  bar.VIEW3D_PT_sc
-00350410: 756c 7074 5f6f 7074 696f 6e73 5f67 7261  ulpt_options_gra
-00350420: 7669 7479 2720 3d20 4e6f 6e65 0a0a 5649  vity' = None..VI
-00350430: 4557 3344 5f50 545f 7363 756c 7074 5f73  EW3D_PT_sculpt_s
-00350440: 796d 6d65 7472 793a 2027 626c 5f75 692e  ymmetry: 'bl_ui.
-00350450: 7370 6163 655f 7669 6577 3364 5f74 6f6f  space_view3d_too
-00350460: 6c62 6172 2e56 4945 5733 445f 5054 5f73  lbar.VIEW3D_PT_s
-00350470: 6375 6c70 745f 7379 6d6d 6574 7279 2720  culpt_symmetry' 
-00350480: 3d20 4e6f 6e65 0a0a 5649 4557 3344 5f50  = None..VIEW3D_P
-00350490: 545f 7363 756c 7074 5f73 796d 6d65 7472  T_sculpt_symmetr
-003504a0: 795f 666f 725f 746f 7062 6172 3a20 2762  y_for_topbar: 'b
-003504b0: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
-003504c0: 645f 746f 6f6c 6261 722e 5649 4557 3344  d_toolbar.VIEW3D
-003504d0: 5f50 545f 7363 756c 7074 5f73 796d 6d65  _PT_sculpt_symme
-003504e0: 7472 795f 666f 725f 746f 7062 6172 2720  try_for_topbar' 
-003504f0: 3d20 4e6f 6e65 0a0a 5649 4557 3344 5f50  = None..VIEW3D_P
-00350500: 545f 7363 756c 7074 5f76 6f78 656c 5f72  T_sculpt_voxel_r
-00350510: 656d 6573 683a 2027 626c 5f75 692e 7370  emesh: 'bl_ui.sp
-00350520: 6163 655f 7669 6577 3364 5f74 6f6f 6c62  ace_view3d_toolb
-00350530: 6172 2e56 4945 5733 445f 5054 5f73 6375  ar.VIEW3D_PT_scu
-00350540: 6c70 745f 766f 7865 6c5f 7265 6d65 7368  lpt_voxel_remesh
-00350550: 2720 3d20 4e6f 6e65 0a0a 5649 4557 3344  ' = None..VIEW3D
-00350560: 5f50 545f 7368 6164 696e 673a 2027 626c  _PT_shading: 'bl
-00350570: 5f75 692e 7370 6163 655f 7669 6577 3364  _ui.space_view3d
-00350580: 2e56 4945 5733 445f 5054 5f73 6861 6469  .VIEW3D_PT_shadi
-00350590: 6e67 2720 3d20 4e6f 6e65 0a0a 5649 4557  ng' = None..VIEW
-003505a0: 3344 5f50 545f 7368 6164 696e 675f 636f  3D_PT_shading_co
-003505b0: 6c6f 723a 2027 626c 5f75 692e 7370 6163  lor: 'bl_ui.spac
-003505c0: 655f 7669 6577 3364 2e56 4945 5733 445f  e_view3d.VIEW3D_
-003505d0: 5054 5f73 6861 6469 6e67 5f63 6f6c 6f72  PT_shading_color
-003505e0: 2720 3d20 4e6f 6e65 0a0a 5649 4557 3344  ' = None..VIEW3D
-003505f0: 5f50 545f 7368 6164 696e 675f 636f 6d70  _PT_shading_comp
-00350600: 6f73 6974 6f72 3a20 2762 6c5f 7569 2e73  ositor: 'bl_ui.s
-00350610: 7061 6365 5f76 6965 7733 642e 5649 4557  pace_view3d.VIEW
-00350620: 3344 5f50 545f 7368 6164 696e 675f 636f  3D_PT_shading_co
-00350630: 6d70 6f73 6974 6f72 2720 3d20 4e6f 6e65  mpositor' = None
-00350640: 0a0a 5649 4557 3344 5f50 545f 7368 6164  ..VIEW3D_PT_shad
-00350650: 696e 675f 6c69 6768 7469 6e67 3a20 2762  ing_lighting: 'b
-00350660: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
-00350670: 642e 5649 4557 3344 5f50 545f 7368 6164  d.VIEW3D_PT_shad
-00350680: 696e 675f 6c69 6768 7469 6e67 2720 3d20  ing_lighting' = 
-00350690: 4e6f 6e65 0a0a 5649 4557 3344 5f50 545f  None..VIEW3D_PT_
-003506a0: 7368 6164 696e 675f 6f70 7469 6f6e 733a  shading_options:
-003506b0: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
-003506c0: 6577 3364 2e56 4945 5733 445f 5054 5f73  ew3d.VIEW3D_PT_s
-003506d0: 6861 6469 6e67 5f6f 7074 696f 6e73 2720  hading_options' 
-003506e0: 3d20 4e6f 6e65 0a0a 5649 4557 3344 5f50  = None..VIEW3D_P
-003506f0: 545f 7368 6164 696e 675f 6f70 7469 6f6e  T_shading_option
-00350700: 735f 7368 6164 6f77 3a20 2762 6c5f 7569  s_shadow: 'bl_ui
-00350710: 2e73 7061 6365 5f76 6965 7733 642e 5649  .space_view3d.VI
-00350720: 4557 3344 5f50 545f 7368 6164 696e 675f  EW3D_PT_shading_
-00350730: 6f70 7469 6f6e 735f 7368 6164 6f77 2720  options_shadow' 
-00350740: 3d20 4e6f 6e65 0a0a 5649 4557 3344 5f50  = None..VIEW3D_P
-00350750: 545f 7368 6164 696e 675f 6f70 7469 6f6e  T_shading_option
-00350760: 735f 7373 616f 3a20 2762 6c5f 7569 2e73  s_ssao: 'bl_ui.s
-00350770: 7061 6365 5f76 6965 7733 642e 5649 4557  pace_view3d.VIEW
-00350780: 3344 5f50 545f 7368 6164 696e 675f 6f70  3D_PT_shading_op
-00350790: 7469 6f6e 735f 7373 616f 2720 3d20 4e6f  tions_ssao' = No
-003507a0: 6e65 0a0a 5649 4557 3344 5f50 545f 7368  ne..VIEW3D_PT_sh
-003507b0: 6164 696e 675f 7265 6e64 6572 5f70 6173  ading_render_pas
-003507c0: 733a 2027 626c 5f75 692e 7370 6163 655f  s: 'bl_ui.space_
-003507d0: 7669 6577 3364 2e56 4945 5733 445f 5054  view3d.VIEW3D_PT
-003507e0: 5f73 6861 6469 6e67 5f72 656e 6465 725f  _shading_render_
-003507f0: 7061 7373 2720 3d20 4e6f 6e65 0a0a 5649  pass' = None..VI
-00350800: 4557 3344 5f50 545f 736c 6f74 735f 7061  EW3D_PT_slots_pa
-00350810: 696e 745f 6361 6e76 6173 3a20 2762 6c5f  int_canvas: 'bl_
-00350820: 7569 2e73 7061 6365 5f76 6965 7733 645f  ui.space_view3d_
-00350830: 746f 6f6c 6261 722e 5649 4557 3344 5f50  toolbar.VIEW3D_P
-00350840: 545f 736c 6f74 735f 7061 696e 745f 6361  T_slots_paint_ca
-00350850: 6e76 6173 2720 3d20 4e6f 6e65 0a0a 5649  nvas' = None..VI
-00350860: 4557 3344 5f50 545f 736c 6f74 735f 7072  EW3D_PT_slots_pr
-00350870: 6f6a 6563 7470 6169 6e74 3a20 2762 6c5f  ojectpaint: 'bl_
-00350880: 7569 2e73 7061 6365 5f76 6965 7733 645f  ui.space_view3d_
-00350890: 746f 6f6c 6261 722e 5649 4557 3344 5f50  toolbar.VIEW3D_P
-003508a0: 545f 736c 6f74 735f 7072 6f6a 6563 7470  T_slots_projectp
-003508b0: 6169 6e74 2720 3d20 4e6f 6e65 0a0a 5649  aint' = None..VI
-003508c0: 4557 3344 5f50 545f 736e 6170 7069 6e67  EW3D_PT_snapping
-003508d0: 3a20 2762 6c5f 7569 2e73 7061 6365 5f76  : 'bl_ui.space_v
-003508e0: 6965 7733 642e 5649 4557 3344 5f50 545f  iew3d.VIEW3D_PT_
-003508f0: 736e 6170 7069 6e67 2720 3d20 4e6f 6e65  snapping' = None
-00350900: 0a0a 5649 4557 3344 5f50 545f 7374 656e  ..VIEW3D_PT_sten
-00350910: 6369 6c5f 7072 6f6a 6563 7470 6169 6e74  cil_projectpaint
-00350920: 3a20 2762 6c5f 7569 2e73 7061 6365 5f76  : 'bl_ui.space_v
-00350930: 6965 7733 645f 746f 6f6c 6261 722e 5649  iew3d_toolbar.VI
-00350940: 4557 3344 5f50 545f 7374 656e 6369 6c5f  EW3D_PT_stencil_
-00350950: 7072 6f6a 6563 7470 6169 6e74 2720 3d20  projectpaint' = 
-00350960: 4e6f 6e65 0a0a 5649 4557 3344 5f50 545f  None..VIEW3D_PT_
-00350970: 746f 6f6c 735f 6163 7469 7665 3a20 2762  tools_active: 'b
-00350980: 6c5f 7569 2e73 7061 6365 5f74 6f6f 6c73  l_ui.space_tools
-00350990: 7973 7465 6d5f 746f 6f6c 6261 722e 5649  ystem_toolbar.VI
-003509a0: 4557 3344 5f50 545f 746f 6f6c 735f 6163  EW3D_PT_tools_ac
-003509b0: 7469 7665 2720 3d20 4e6f 6e65 0a0a 5649  tive' = None..VI
-003509c0: 4557 3344 5f50 545f 746f 6f6c 735f 6172  EW3D_PT_tools_ar
-003509d0: 6d61 7475 7265 6564 6974 5f6f 7074 696f  matureedit_optio
-003509e0: 6e73 3a20 2762 6c5f 7569 2e73 7061 6365  ns: 'bl_ui.space
-003509f0: 5f76 6965 7733 645f 746f 6f6c 6261 722e  _view3d_toolbar.
-00350a00: 5649 4557 3344 5f50 545f 746f 6f6c 735f  VIEW3D_PT_tools_
-00350a10: 6172 6d61 7475 7265 6564 6974 5f6f 7074  armatureedit_opt
-00350a20: 696f 6e73 2720 3d20 4e6f 6e65 0a0a 5649  ions' = None..VI
-00350a30: 4557 3344 5f50 545f 746f 6f6c 735f 6272  EW3D_PT_tools_br
-00350a40: 7573 685f 636c 6f6e 653a 2027 626c 5f75  ush_clone: 'bl_u
-00350a50: 692e 7370 6163 655f 7669 6577 3364 5f74  i.space_view3d_t
-00350a60: 6f6f 6c62 6172 2e56 4945 5733 445f 5054  oolbar.VIEW3D_PT
-00350a70: 5f74 6f6f 6c73 5f62 7275 7368 5f63 6c6f  _tools_brush_clo
-00350a80: 6e65 2720 3d20 4e6f 6e65 0a0a 5649 4557  ne' = None..VIEW
-00350a90: 3344 5f50 545f 746f 6f6c 735f 6272 7573  3D_PT_tools_brus
-00350aa0: 685f 636f 6c6f 723a 2027 626c 5f75 692e  h_color: 'bl_ui.
-00350ab0: 7370 6163 655f 7669 6577 3364 5f74 6f6f  space_view3d_too
-00350ac0: 6c62 6172 2e56 4945 5733 445f 5054 5f74  lbar.VIEW3D_PT_t
-00350ad0: 6f6f 6c73 5f62 7275 7368 5f63 6f6c 6f72  ools_brush_color
-00350ae0: 2720 3d20 4e6f 6e65 0a0a 5649 4557 3344  ' = None..VIEW3D
-00350af0: 5f50 545f 746f 6f6c 735f 6272 7573 685f  _PT_tools_brush_
-00350b00: 6469 7370 6c61 793a 2027 626c 5f75 692e  display: 'bl_ui.
-00350b10: 7370 6163 655f 7669 6577 3364 5f74 6f6f  space_view3d_too
-00350b20: 6c62 6172 2e56 4945 5733 445f 5054 5f74  lbar.VIEW3D_PT_t
-00350b30: 6f6f 6c73 5f62 7275 7368 5f64 6973 706c  ools_brush_displ
-00350b40: 6179 2720 3d20 4e6f 6e65 0a0a 5649 4557  ay' = None..VIEW
-00350b50: 3344 5f50 545f 746f 6f6c 735f 6272 7573  3D_PT_tools_brus
-00350b60: 685f 6661 6c6c 6f66 663a 2027 626c 5f75  h_falloff: 'bl_u
-00350b70: 692e 7370 6163 655f 7669 6577 3364 5f74  i.space_view3d_t
-00350b80: 6f6f 6c62 6172 2e56 4945 5733 445f 5054  oolbar.VIEW3D_PT
-00350b90: 5f74 6f6f 6c73 5f62 7275 7368 5f66 616c  _tools_brush_fal
-00350ba0: 6c6f 6666 2720 3d20 4e6f 6e65 0a0a 5649  loff' = None..VI
-00350bb0: 4557 3344 5f50 545f 746f 6f6c 735f 6272  EW3D_PT_tools_br
-00350bc0: 7573 685f 6661 6c6c 6f66 665f 6672 6f6e  ush_falloff_fron
-00350bd0: 7466 6163 653a 2027 626c 5f75 692e 7370  tface: 'bl_ui.sp
-00350be0: 6163 655f 7669 6577 3364 5f74 6f6f 6c62  ace_view3d_toolb
-00350bf0: 6172 2e56 4945 5733 445f 5054 5f74 6f6f  ar.VIEW3D_PT_too
-00350c00: 6c73 5f62 7275 7368 5f66 616c 6c6f 6666  ls_brush_falloff
-00350c10: 5f66 726f 6e74 6661 6365 2720 3d20 4e6f  _frontface' = No
-00350c20: 6e65 0a0a 5649 4557 3344 5f50 545f 746f  ne..VIEW3D_PT_to
-00350c30: 6f6c 735f 6272 7573 685f 6661 6c6c 6f66  ols_brush_fallof
-00350c40: 665f 6e6f 726d 616c 3a20 2762 6c5f 7569  f_normal: 'bl_ui
-00350c50: 2e73 7061 6365 5f76 6965 7733 645f 746f  .space_view3d_to
-00350c60: 6f6c 6261 722e 5649 4557 3344 5f50 545f  olbar.VIEW3D_PT_
-00350c70: 746f 6f6c 735f 6272 7573 685f 6661 6c6c  tools_brush_fall
-00350c80: 6f66 665f 6e6f 726d 616c 2720 3d20 4e6f  off_normal' = No
-00350c90: 6e65 0a0a 5649 4557 3344 5f50 545f 746f  ne..VIEW3D_PT_to
-00350ca0: 6f6c 735f 6272 7573 685f 7365 6c65 6374  ols_brush_select
-00350cb0: 3a20 2762 6c5f 7569 2e73 7061 6365 5f76  : 'bl_ui.space_v
-00350cc0: 6965 7733 645f 746f 6f6c 6261 722e 5649  iew3d_toolbar.VI
-00350cd0: 4557 3344 5f50 545f 746f 6f6c 735f 6272  EW3D_PT_tools_br
-00350ce0: 7573 685f 7365 6c65 6374 2720 3d20 4e6f  ush_select' = No
-00350cf0: 6e65 0a0a 5649 4557 3344 5f50 545f 746f  ne..VIEW3D_PT_to
-00350d00: 6f6c 735f 6272 7573 685f 7365 7474 696e  ols_brush_settin
-00350d10: 6773 3a20 2762 6c5f 7569 2e73 7061 6365  gs: 'bl_ui.space
-00350d20: 5f76 6965 7733 645f 746f 6f6c 6261 722e  _view3d_toolbar.
-00350d30: 5649 4557 3344 5f50 545f 746f 6f6c 735f  VIEW3D_PT_tools_
-00350d40: 6272 7573 685f 7365 7474 696e 6773 2720  brush_settings' 
-00350d50: 3d20 4e6f 6e65 0a0a 5649 4557 3344 5f50  = None..VIEW3D_P
-00350d60: 545f 746f 6f6c 735f 6272 7573 685f 7365  T_tools_brush_se
-00350d70: 7474 696e 6773 5f61 6476 616e 6365 643a  ttings_advanced:
-00350d80: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
-00350d90: 6577 3364 5f74 6f6f 6c62 6172 2e56 4945  ew3d_toolbar.VIE
-00350da0: 5733 445f 5054 5f74 6f6f 6c73 5f62 7275  W3D_PT_tools_bru
-00350db0: 7368 5f73 6574 7469 6e67 735f 6164 7661  sh_settings_adva
-00350dc0: 6e63 6564 2720 3d20 4e6f 6e65 0a0a 5649  nced' = None..VI
-00350dd0: 4557 3344 5f50 545f 746f 6f6c 735f 6272  EW3D_PT_tools_br
-00350de0: 7573 685f 7374 726f 6b65 3a20 2762 6c5f  ush_stroke: 'bl_
-00350df0: 7569 2e73 7061 6365 5f76 6965 7733 645f  ui.space_view3d_
-00350e00: 746f 6f6c 6261 722e 5649 4557 3344 5f50  toolbar.VIEW3D_P
-00350e10: 545f 746f 6f6c 735f 6272 7573 685f 7374  T_tools_brush_st
-00350e20: 726f 6b65 2720 3d20 4e6f 6e65 0a0a 5649  roke' = None..VI
-00350e30: 4557 3344 5f50 545f 746f 6f6c 735f 6272  EW3D_PT_tools_br
-00350e40: 7573 685f 7374 726f 6b65 5f73 6d6f 6f74  ush_stroke_smoot
-00350e50: 685f 7374 726f 6b65 3a20 2762 6c5f 7569  h_stroke: 'bl_ui
-00350e60: 2e73 7061 6365 5f76 6965 7733 645f 746f  .space_view3d_to
-00350e70: 6f6c 6261 722e 5649 4557 3344 5f50 545f  olbar.VIEW3D_PT_
-00350e80: 746f 6f6c 735f 6272 7573 685f 7374 726f  tools_brush_stro
-00350e90: 6b65 5f73 6d6f 6f74 685f 7374 726f 6b65  ke_smooth_stroke
-00350ea0: 2720 3d20 4e6f 6e65 0a0a 5649 4557 3344  ' = None..VIEW3D
-00350eb0: 5f50 545f 746f 6f6c 735f 6272 7573 685f  _PT_tools_brush_
-00350ec0: 7377 6174 6368 6573 3a20 2762 6c5f 7569  swatches: 'bl_ui
-00350ed0: 2e73 7061 6365 5f76 6965 7733 645f 746f  .space_view3d_to
-00350ee0: 6f6c 6261 722e 5649 4557 3344 5f50 545f  olbar.VIEW3D_PT_
-00350ef0: 746f 6f6c 735f 6272 7573 685f 7377 6174  tools_brush_swat
-00350f00: 6368 6573 2720 3d20 4e6f 6e65 0a0a 5649  ches' = None..VI
-00350f10: 4557 3344 5f50 545f 746f 6f6c 735f 6272  EW3D_PT_tools_br
-00350f20: 7573 685f 7465 7874 7572 653a 2027 626c  ush_texture: 'bl
-00350f30: 5f75 692e 7370 6163 655f 7669 6577 3364  _ui.space_view3d
-00350f40: 5f74 6f6f 6c62 6172 2e56 4945 5733 445f  _toolbar.VIEW3D_
-00350f50: 5054 5f74 6f6f 6c73 5f62 7275 7368 5f74  PT_tools_brush_t
-00350f60: 6578 7475 7265 2720 3d20 4e6f 6e65 0a0a  exture' = None..
-00350f70: 5649 4557 3344 5f50 545f 746f 6f6c 735f  VIEW3D_PT_tools_
-00350f80: 6772 6561 7365 5f70 656e 6369 6c5f 6272  grease_pencil_br
-00350f90: 7573 685f 6164 7661 6e63 6564 3a20 2762  ush_advanced: 'b
-00350fa0: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
-00350fb0: 645f 746f 6f6c 6261 722e 5649 4557 3344  d_toolbar.VIEW3D
-00350fc0: 5f50 545f 746f 6f6c 735f 6772 6561 7365  _PT_tools_grease
-00350fd0: 5f70 656e 6369 6c5f 6272 7573 685f 6164  _pencil_brush_ad
-00350fe0: 7661 6e63 6564 2720 3d20 4e6f 6e65 0a0a  vanced' = None..
-00350ff0: 5649 4557 3344 5f50 545f 746f 6f6c 735f  VIEW3D_PT_tools_
-00351000: 6772 6561 7365 5f70 656e 6369 6c5f 6272  grease_pencil_br
-00351010: 7573 685f 6761 705f 636c 6f73 7572 653a  ush_gap_closure:
-00351020: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
-00351030: 6577 3364 5f74 6f6f 6c62 6172 2e56 4945  ew3d_toolbar.VIE
-00351040: 5733 445f 5054 5f74 6f6f 6c73 5f67 7265  W3D_PT_tools_gre
-00351050: 6173 655f 7065 6e63 696c 5f62 7275 7368  ase_pencil_brush
-00351060: 5f67 6170 5f63 6c6f 7375 7265 2720 3d20  _gap_closure' = 
-00351070: 4e6f 6e65 0a0a 5649 4557 3344 5f50 545f  None..VIEW3D_PT_
-00351080: 746f 6f6c 735f 6772 6561 7365 5f70 656e  tools_grease_pen
-00351090: 6369 6c5f 6272 7573 685f 6d69 785f 7061  cil_brush_mix_pa
-003510a0: 6c65 7474 653a 2027 626c 5f75 692e 7370  lette: 'bl_ui.sp
-003510b0: 6163 655f 7669 6577 3364 5f74 6f6f 6c62  ace_view3d_toolb
-003510c0: 6172 2e56 4945 5733 445f 5054 5f74 6f6f  ar.VIEW3D_PT_too
-003510d0: 6c73 5f67 7265 6173 655f 7065 6e63 696c  ls_grease_pencil
-003510e0: 5f62 7275 7368 5f6d 6978 5f70 616c 6574  _brush_mix_palet
-003510f0: 7465 2720 3d20 4e6f 6e65 0a0a 5649 4557  te' = None..VIEW
-00351100: 3344 5f50 545f 746f 6f6c 735f 6772 6561  3D_PT_tools_grea
-00351110: 7365 5f70 656e 6369 6c5f 6272 7573 685f  se_pencil_brush_
-00351120: 6d69 7863 6f6c 6f72 3a20 2762 6c5f 7569  mixcolor: 'bl_ui
-00351130: 2e73 7061 6365 5f76 6965 7733 645f 746f  .space_view3d_to
-00351140: 6f6c 6261 722e 5649 4557 3344 5f50 545f  olbar.VIEW3D_PT_
-00351150: 746f 6f6c 735f 6772 6561 7365 5f70 656e  tools_grease_pen
-00351160: 6369 6c5f 6272 7573 685f 6d69 7863 6f6c  cil_brush_mixcol
-00351170: 6f72 2720 3d20 4e6f 6e65 0a0a 5649 4557  or' = None..VIEW
-00351180: 3344 5f50 545f 746f 6f6c 735f 6772 6561  3D_PT_tools_grea
-00351190: 7365 5f70 656e 6369 6c5f 6272 7573 685f  se_pencil_brush_
-003511a0: 7061 696e 745f 6661 6c6c 6f66 663a 2027  paint_falloff: '
-003511b0: 626c 5f75 692e 7370 6163 655f 7669 6577  bl_ui.space_view
-003511c0: 3364 5f74 6f6f 6c62 6172 2e56 4945 5733  3d_toolbar.VIEW3
-003511d0: 445f 5054 5f74 6f6f 6c73 5f67 7265 6173  D_PT_tools_greas
-003511e0: 655f 7065 6e63 696c 5f62 7275 7368 5f70  e_pencil_brush_p
-003511f0: 6169 6e74 5f66 616c 6c6f 6666 2720 3d20  aint_falloff' = 
-00351200: 4e6f 6e65 0a0a 5649 4557 3344 5f50 545f  None..VIEW3D_PT_
-00351210: 746f 6f6c 735f 6772 6561 7365 5f70 656e  tools_grease_pen
-00351220: 6369 6c5f 6272 7573 685f 706f 7374 5f70  cil_brush_post_p
-00351230: 726f 6365 7373 696e 673a 2027 626c 5f75  rocessing: 'bl_u
-00351240: 692e 7370 6163 655f 7669 6577 3364 5f74  i.space_view3d_t
-00351250: 6f6f 6c62 6172 2e56 4945 5733 445f 5054  oolbar.VIEW3D_PT
-00351260: 5f74 6f6f 6c73 5f67 7265 6173 655f 7065  _tools_grease_pe
-00351270: 6e63 696c 5f62 7275 7368 5f70 6f73 745f  ncil_brush_post_
-00351280: 7072 6f63 6573 7369 6e67 2720 3d20 4e6f  processing' = No
-00351290: 6e65 0a0a 5649 4557 3344 5f50 545f 746f  ne..VIEW3D_PT_to
-003512a0: 6f6c 735f 6772 6561 7365 5f70 656e 6369  ols_grease_penci
-003512b0: 6c5f 6272 7573 685f 7261 6e64 6f6d 3a20  l_brush_random: 
-003512c0: 2762 6c5f 7569 2e73 7061 6365 5f76 6965  'bl_ui.space_vie
-003512d0: 7733 645f 746f 6f6c 6261 722e 5649 4557  w3d_toolbar.VIEW
-003512e0: 3344 5f50 545f 746f 6f6c 735f 6772 6561  3D_PT_tools_grea
-003512f0: 7365 5f70 656e 6369 6c5f 6272 7573 685f  se_pencil_brush_
-00351300: 7261 6e64 6f6d 2720 3d20 4e6f 6e65 0a0a  random' = None..
-00351310: 5649 4557 3344 5f50 545f 746f 6f6c 735f  VIEW3D_PT_tools_
-00351320: 6772 6561 7365 5f70 656e 6369 6c5f 6272  grease_pencil_br
-00351330: 7573 685f 7363 756c 7074 5f66 616c 6c6f  ush_sculpt_fallo
-00351340: 6666 3a20 2762 6c5f 7569 2e73 7061 6365  ff: 'bl_ui.space
-00351350: 5f76 6965 7733 645f 746f 6f6c 6261 722e  _view3d_toolbar.
-00351360: 5649 4557 3344 5f50 545f 746f 6f6c 735f  VIEW3D_PT_tools_
-00351370: 6772 6561 7365 5f70 656e 6369 6c5f 6272  grease_pencil_br
-00351380: 7573 685f 7363 756c 7074 5f66 616c 6c6f  ush_sculpt_fallo
-00351390: 6666 2720 3d20 4e6f 6e65 0a0a 5649 4557  ff' = None..VIEW
-003513a0: 3344 5f50 545f 746f 6f6c 735f 6772 6561  3D_PT_tools_grea
-003513b0: 7365 5f70 656e 6369 6c5f 6272 7573 685f  se_pencil_brush_
-003513c0: 7365 6c65 6374 3a20 2762 6c5f 7569 2e73  select: 'bl_ui.s
-003513d0: 7061 6365 5f76 6965 7733 645f 746f 6f6c  pace_view3d_tool
-003513e0: 6261 722e 5649 4557 3344 5f50 545f 746f  bar.VIEW3D_PT_to
-003513f0: 6f6c 735f 6772 6561 7365 5f70 656e 6369  ols_grease_penci
-00351400: 6c5f 6272 7573 685f 7365 6c65 6374 2720  l_brush_select' 
-00351410: 3d20 4e6f 6e65 0a0a 5649 4557 3344 5f50  = None..VIEW3D_P
-00351420: 545f 746f 6f6c 735f 6772 6561 7365 5f70  T_tools_grease_p
-00351430: 656e 6369 6c5f 6272 7573 685f 7365 7474  encil_brush_sett
-00351440: 696e 6773 3a20 2762 6c5f 7569 2e73 7061  ings: 'bl_ui.spa
-00351450: 6365 5f76 6965 7733 645f 746f 6f6c 6261  ce_view3d_toolba
-00351460: 722e 5649 4557 3344 5f50 545f 746f 6f6c  r.VIEW3D_PT_tool
-00351470: 735f 6772 6561 7365 5f70 656e 6369 6c5f  s_grease_pencil_
-00351480: 6272 7573 685f 7365 7474 696e 6773 2720  brush_settings' 
-00351490: 3d20 4e6f 6e65 0a0a 5649 4557 3344 5f50  = None..VIEW3D_P
-003514a0: 545f 746f 6f6c 735f 6772 6561 7365 5f70  T_tools_grease_p
-003514b0: 656e 6369 6c5f 6272 7573 685f 7374 6162  encil_brush_stab
-003514c0: 696c 697a 6572 3a20 2762 6c5f 7569 2e73  ilizer: 'bl_ui.s
-003514d0: 7061 6365 5f76 6965 7733 645f 746f 6f6c  pace_view3d_tool
-003514e0: 6261 722e 5649 4557 3344 5f50 545f 746f  bar.VIEW3D_PT_to
-003514f0: 6f6c 735f 6772 6561 7365 5f70 656e 6369  ols_grease_penci
-00351500: 6c5f 6272 7573 685f 7374 6162 696c 697a  l_brush_stabiliz
-00351510: 6572 2720 3d20 4e6f 6e65 0a0a 5649 4557  er' = None..VIEW
-00351520: 3344 5f50 545f 746f 6f6c 735f 6772 6561  3D_PT_tools_grea
-00351530: 7365 5f70 656e 6369 6c5f 6272 7573 685f  se_pencil_brush_
-00351540: 7374 726f 6b65 3a20 2762 6c5f 7569 2e73  stroke: 'bl_ui.s
-00351550: 7061 6365 5f76 6965 7733 645f 746f 6f6c  pace_view3d_tool
-00351560: 6261 722e 5649 4557 3344 5f50 545f 746f  bar.VIEW3D_PT_to
-00351570: 6f6c 735f 6772 6561 7365 5f70 656e 6369  ols_grease_penci
-00351580: 6c5f 6272 7573 685f 7374 726f 6b65 2720  l_brush_stroke' 
-00351590: 3d20 4e6f 6e65 0a0a 5649 4557 3344 5f50  = None..VIEW3D_P
-003515a0: 545f 746f 6f6c 735f 6772 6561 7365 5f70  T_tools_grease_p
-003515b0: 656e 6369 6c5f 6272 7573 685f 7665 7274  encil_brush_vert
-003515c0: 6578 5f63 6f6c 6f72 3a20 2762 6c5f 7569  ex_color: 'bl_ui
-003515d0: 2e73 7061 6365 5f76 6965 7733 645f 746f  .space_view3d_to
-003515e0: 6f6c 6261 722e 5649 4557 3344 5f50 545f  olbar.VIEW3D_PT_
-003515f0: 746f 6f6c 735f 6772 6561 7365 5f70 656e  tools_grease_pen
-00351600: 6369 6c5f 6272 7573 685f 7665 7274 6578  cil_brush_vertex
-00351610: 5f63 6f6c 6f72 2720 3d20 4e6f 6e65 0a0a  _color' = None..
-00351620: 5649 4557 3344 5f50 545f 746f 6f6c 735f  VIEW3D_PT_tools_
-00351630: 6772 6561 7365 5f70 656e 6369 6c5f 6272  grease_pencil_br
-00351640: 7573 685f 7665 7274 6578 5f66 616c 6c6f  ush_vertex_fallo
-00351650: 6666 3a20 2762 6c5f 7569 2e73 7061 6365  ff: 'bl_ui.space
-00351660: 5f76 6965 7733 645f 746f 6f6c 6261 722e  _view3d_toolbar.
-00351670: 5649 4557 3344 5f50 545f 746f 6f6c 735f  VIEW3D_PT_tools_
-00351680: 6772 6561 7365 5f70 656e 6369 6c5f 6272  grease_pencil_br
-00351690: 7573 685f 7665 7274 6578 5f66 616c 6c6f  ush_vertex_fallo
-003516a0: 6666 2720 3d20 4e6f 6e65 0a0a 5649 4557  ff' = None..VIEW
-003516b0: 3344 5f50 545f 746f 6f6c 735f 6772 6561  3D_PT_tools_grea
-003516c0: 7365 5f70 656e 6369 6c5f 6272 7573 685f  se_pencil_brush_
-003516d0: 7665 7274 6578 5f70 616c 6574 7465 3a20  vertex_palette: 
-003516e0: 2762 6c5f 7569 2e73 7061 6365 5f76 6965  'bl_ui.space_vie
-003516f0: 7733 645f 746f 6f6c 6261 722e 5649 4557  w3d_toolbar.VIEW
-00351700: 3344 5f50 545f 746f 6f6c 735f 6772 6561  3D_PT_tools_grea
-00351710: 7365 5f70 656e 6369 6c5f 6272 7573 685f  se_pencil_brush_
-00351720: 7665 7274 6578 5f70 616c 6574 7465 2720  vertex_palette' 
-00351730: 3d20 4e6f 6e65 0a0a 5649 4557 3344 5f50  = None..VIEW3D_P
-00351740: 545f 746f 6f6c 735f 6772 6561 7365 5f70  T_tools_grease_p
-00351750: 656e 6369 6c5f 6272 7573 685f 7765 6967  encil_brush_weig
-00351760: 6874 5f66 616c 6c6f 6666 3a20 2762 6c5f  ht_falloff: 'bl_
-00351770: 7569 2e73 7061 6365 5f76 6965 7733 645f  ui.space_view3d_
-00351780: 746f 6f6c 6261 722e 5649 4557 3344 5f50  toolbar.VIEW3D_P
-00351790: 545f 746f 6f6c 735f 6772 6561 7365 5f70  T_tools_grease_p
-003517a0: 656e 6369 6c5f 6272 7573 685f 7765 6967  encil_brush_weig
-003517b0: 6874 5f66 616c 6c6f 6666 2720 3d20 4e6f  ht_falloff' = No
-003517c0: 6e65 0a0a 5649 4557 3344 5f50 545f 746f  ne..VIEW3D_PT_to
-003517d0: 6f6c 735f 6772 6561 7365 5f70 656e 6369  ols_grease_penci
-003517e0: 6c5f 7061 696e 745f 6170 7065 6172 616e  l_paint_appearan
-003517f0: 6365 3a20 2762 6c5f 7569 2e73 7061 6365  ce: 'bl_ui.space
-00351800: 5f76 6965 7733 645f 746f 6f6c 6261 722e  _view3d_toolbar.
-00351810: 5649 4557 3344 5f50 545f 746f 6f6c 735f  VIEW3D_PT_tools_
-00351820: 6772 6561 7365 5f70 656e 6369 6c5f 7061  grease_pencil_pa
-00351830: 696e 745f 6170 7065 6172 616e 6365 2720  int_appearance' 
-00351840: 3d20 4e6f 6e65 0a0a 5649 4557 3344 5f50  = None..VIEW3D_P
-00351850: 545f 746f 6f6c 735f 6772 6561 7365 5f70  T_tools_grease_p
-00351860: 656e 6369 6c5f 7363 756c 7074 5f61 7070  encil_sculpt_app
-00351870: 6561 7261 6e63 653a 2027 626c 5f75 692e  earance: 'bl_ui.
-00351880: 7370 6163 655f 7669 6577 3364 5f74 6f6f  space_view3d_too
-00351890: 6c62 6172 2e56 4945 5733 445f 5054 5f74  lbar.VIEW3D_PT_t
-003518a0: 6f6f 6c73 5f67 7265 6173 655f 7065 6e63  ools_grease_penc
-003518b0: 696c 5f73 6375 6c70 745f 6170 7065 6172  il_sculpt_appear
-003518c0: 616e 6365 2720 3d20 4e6f 6e65 0a0a 5649  ance' = None..VI
-003518d0: 4557 3344 5f50 545f 746f 6f6c 735f 6772  EW3D_PT_tools_gr
-003518e0: 6561 7365 5f70 656e 6369 6c5f 7363 756c  ease_pencil_scul
-003518f0: 7074 5f62 7275 7368 5f61 6476 616e 6365  pt_brush_advance
-00351900: 643a 2027 626c 5f75 692e 7370 6163 655f  d: 'bl_ui.space_
-00351910: 7669 6577 3364 5f74 6f6f 6c62 6172 2e56  view3d_toolbar.V
-00351920: 4945 5733 445f 5054 5f74 6f6f 6c73 5f67  IEW3D_PT_tools_g
-00351930: 7265 6173 655f 7065 6e63 696c 5f73 6375  rease_pencil_scu
-00351940: 6c70 745f 6272 7573 685f 6164 7661 6e63  lpt_brush_advanc
-00351950: 6564 2720 3d20 4e6f 6e65 0a0a 5649 4557  ed' = None..VIEW
-00351960: 3344 5f50 545f 746f 6f6c 735f 6772 6561  3D_PT_tools_grea
-00351970: 7365 5f70 656e 6369 6c5f 7363 756c 7074  se_pencil_sculpt
-00351980: 5f62 7275 7368 5f70 6f70 6f76 6572 3a20  _brush_popover: 
-00351990: 2762 6c5f 7569 2e73 7061 6365 5f76 6965  'bl_ui.space_vie
-003519a0: 7733 645f 746f 6f6c 6261 722e 5649 4557  w3d_toolbar.VIEW
-003519b0: 3344 5f50 545f 746f 6f6c 735f 6772 6561  3D_PT_tools_grea
-003519c0: 7365 5f70 656e 6369 6c5f 7363 756c 7074  se_pencil_sculpt
-003519d0: 5f62 7275 7368 5f70 6f70 6f76 6572 2720  _brush_popover' 
-003519e0: 3d20 4e6f 6e65 0a0a 5649 4557 3344 5f50  = None..VIEW3D_P
-003519f0: 545f 746f 6f6c 735f 6772 6561 7365 5f70  T_tools_grease_p
-00351a00: 656e 6369 6c5f 7363 756c 7074 5f73 656c  encil_sculpt_sel
-00351a10: 6563 743a 2027 626c 5f75 692e 7370 6163  ect: 'bl_ui.spac
-00351a20: 655f 7669 6577 3364 5f74 6f6f 6c62 6172  e_view3d_toolbar
-00351a30: 2e56 4945 5733 445f 5054 5f74 6f6f 6c73  .VIEW3D_PT_tools
-00351a40: 5f67 7265 6173 655f 7065 6e63 696c 5f73  _grease_pencil_s
-00351a50: 6375 6c70 745f 7365 6c65 6374 2720 3d20  culpt_select' = 
-00351a60: 4e6f 6e65 0a0a 5649 4557 3344 5f50 545f  None..VIEW3D_PT_
-00351a70: 746f 6f6c 735f 6772 6561 7365 5f70 656e  tools_grease_pen
-00351a80: 6369 6c5f 7363 756c 7074 5f73 6574 7469  cil_sculpt_setti
-00351a90: 6e67 733a 2027 626c 5f75 692e 7370 6163  ngs: 'bl_ui.spac
-00351aa0: 655f 7669 6577 3364 5f74 6f6f 6c62 6172  e_view3d_toolbar
-00351ab0: 2e56 4945 5733 445f 5054 5f74 6f6f 6c73  .VIEW3D_PT_tools
-00351ac0: 5f67 7265 6173 655f 7065 6e63 696c 5f73  _grease_pencil_s
-00351ad0: 6375 6c70 745f 7365 7474 696e 6773 2720  culpt_settings' 
-00351ae0: 3d20 4e6f 6e65 0a0a 5649 4557 3344 5f50  = None..VIEW3D_P
-00351af0: 545f 746f 6f6c 735f 6772 6561 7365 5f70  T_tools_grease_p
-00351b00: 656e 6369 6c5f 7665 7274 6578 5f61 7070  encil_vertex_app
-00351b10: 6561 7261 6e63 653a 2027 626c 5f75 692e  earance: 'bl_ui.
-00351b20: 7370 6163 655f 7669 6577 3364 5f74 6f6f  space_view3d_too
-00351b30: 6c62 6172 2e56 4945 5733 445f 5054 5f74  lbar.VIEW3D_PT_t
-00351b40: 6f6f 6c73 5f67 7265 6173 655f 7065 6e63  ools_grease_penc
-00351b50: 696c 5f76 6572 7465 785f 6170 7065 6172  il_vertex_appear
-00351b60: 616e 6365 2720 3d20 4e6f 6e65 0a0a 5649  ance' = None..VI
-00351b70: 4557 3344 5f50 545f 746f 6f6c 735f 6772  EW3D_PT_tools_gr
-00351b80: 6561 7365 5f70 656e 6369 6c5f 7665 7274  ease_pencil_vert
-00351b90: 6578 5f70 6169 6e74 5f73 656c 6563 743a  ex_paint_select:
-00351ba0: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
-00351bb0: 6577 3364 5f74 6f6f 6c62 6172 2e56 4945  ew3d_toolbar.VIE
-00351bc0: 5733 445f 5054 5f74 6f6f 6c73 5f67 7265  W3D_PT_tools_gre
-00351bd0: 6173 655f 7065 6e63 696c 5f76 6572 7465  ase_pencil_verte
-00351be0: 785f 7061 696e 745f 7365 6c65 6374 2720  x_paint_select' 
-00351bf0: 3d20 4e6f 6e65 0a0a 5649 4557 3344 5f50  = None..VIEW3D_P
-00351c00: 545f 746f 6f6c 735f 6772 6561 7365 5f70  T_tools_grease_p
-00351c10: 656e 6369 6c5f 7665 7274 6578 5f70 6169  encil_vertex_pai
-00351c20: 6e74 5f73 6574 7469 6e67 733a 2027 626c  nt_settings: 'bl
-00351c30: 5f75 692e 7370 6163 655f 7669 6577 3364  _ui.space_view3d
-00351c40: 5f74 6f6f 6c62 6172 2e56 4945 5733 445f  _toolbar.VIEW3D_
-00351c50: 5054 5f74 6f6f 6c73 5f67 7265 6173 655f  PT_tools_grease_
-00351c60: 7065 6e63 696c 5f76 6572 7465 785f 7061  pencil_vertex_pa
-00351c70: 696e 745f 7365 7474 696e 6773 2720 3d20  int_settings' = 
-00351c80: 4e6f 6e65 0a0a 5649 4557 3344 5f50 545f  None..VIEW3D_PT_
-00351c90: 746f 6f6c 735f 6772 6561 7365 5f70 656e  tools_grease_pen
-00351ca0: 6369 6c5f 7765 6967 6874 5f61 7070 6561  cil_weight_appea
-00351cb0: 7261 6e63 653a 2027 626c 5f75 692e 7370  rance: 'bl_ui.sp
-00351cc0: 6163 655f 7669 6577 3364 5f74 6f6f 6c62  ace_view3d_toolb
-00351cd0: 6172 2e56 4945 5733 445f 5054 5f74 6f6f  ar.VIEW3D_PT_too
-00351ce0: 6c73 5f67 7265 6173 655f 7065 6e63 696c  ls_grease_pencil
-00351cf0: 5f77 6569 6768 745f 6170 7065 6172 616e  _weight_appearan
-00351d00: 6365 2720 3d20 4e6f 6e65 0a0a 5649 4557  ce' = None..VIEW
-00351d10: 3344 5f50 545f 746f 6f6c 735f 6772 6561  3D_PT_tools_grea
-00351d20: 7365 5f70 656e 6369 6c5f 7765 6967 6874  se_pencil_weight
-00351d30: 5f6f 7074 696f 6e73 3a20 2762 6c5f 7569  _options: 'bl_ui
-00351d40: 2e73 7061 6365 5f76 6965 7733 645f 746f  .space_view3d_to
-00351d50: 6f6c 6261 722e 5649 4557 3344 5f50 545f  olbar.VIEW3D_PT_
-00351d60: 746f 6f6c 735f 6772 6561 7365 5f70 656e  tools_grease_pen
-00351d70: 6369 6c5f 7765 6967 6874 5f6f 7074 696f  cil_weight_optio
-00351d80: 6e73 2720 3d20 4e6f 6e65 0a0a 5649 4557  ns' = None..VIEW
-00351d90: 3344 5f50 545f 746f 6f6c 735f 6772 6561  3D_PT_tools_grea
-00351da0: 7365 5f70 656e 6369 6c5f 7765 6967 6874  se_pencil_weight
-00351db0: 5f70 6169 6e74 5f73 656c 6563 743a 2027  _paint_select: '
-00351dc0: 626c 5f75 692e 7370 6163 655f 7669 6577  bl_ui.space_view
-00351dd0: 3364 5f74 6f6f 6c62 6172 2e56 4945 5733  3d_toolbar.VIEW3
-00351de0: 445f 5054 5f74 6f6f 6c73 5f67 7265 6173  D_PT_tools_greas
-00351df0: 655f 7065 6e63 696c 5f77 6569 6768 745f  e_pencil_weight_
-00351e00: 7061 696e 745f 7365 6c65 6374 2720 3d20  paint_select' = 
-00351e10: 4e6f 6e65 0a0a 5649 4557 3344 5f50 545f  None..VIEW3D_PT_
-00351e20: 746f 6f6c 735f 6772 6561 7365 5f70 656e  tools_grease_pen
-00351e30: 6369 6c5f 7765 6967 6874 5f70 6169 6e74  cil_weight_paint
-00351e40: 5f73 6574 7469 6e67 733a 2027 626c 5f75  _settings: 'bl_u
-00351e50: 692e 7370 6163 655f 7669 6577 3364 5f74  i.space_view3d_t
-00351e60: 6f6f 6c62 6172 2e56 4945 5733 445f 5054  oolbar.VIEW3D_PT
-00351e70: 5f74 6f6f 6c73 5f67 7265 6173 655f 7065  _tools_grease_pe
-00351e80: 6e63 696c 5f77 6569 6768 745f 7061 696e  ncil_weight_pain
-00351e90: 745f 7365 7474 696e 6773 2720 3d20 4e6f  t_settings' = No
-00351ea0: 6e65 0a0a 5649 4557 3344 5f50 545f 746f  ne..VIEW3D_PT_to
-00351eb0: 6f6c 735f 696d 6167 6570 6169 6e74 5f6f  ols_imagepaint_o
-00351ec0: 7074 696f 6e73 3a20 2762 6c5f 7569 2e73  ptions: 'bl_ui.s
-00351ed0: 7061 6365 5f76 6965 7733 645f 746f 6f6c  pace_view3d_tool
-00351ee0: 6261 722e 5649 4557 3344 5f50 545f 746f  bar.VIEW3D_PT_to
-00351ef0: 6f6c 735f 696d 6167 6570 6169 6e74 5f6f  ols_imagepaint_o
-00351f00: 7074 696f 6e73 2720 3d20 4e6f 6e65 0a0a  ptions' = None..
-00351f10: 5649 4557 3344 5f50 545f 746f 6f6c 735f  VIEW3D_PT_tools_
-00351f20: 696d 6167 6570 6169 6e74 5f6f 7074 696f  imagepaint_optio
-00351f30: 6e73 5f63 6176 6974 793a 2027 626c 5f75  ns_cavity: 'bl_u
-00351f40: 692e 7370 6163 655f 7669 6577 3364 5f74  i.space_view3d_t
-00351f50: 6f6f 6c62 6172 2e56 4945 5733 445f 5054  oolbar.VIEW3D_PT
-00351f60: 5f74 6f6f 6c73 5f69 6d61 6765 7061 696e  _tools_imagepain
-00351f70: 745f 6f70 7469 6f6e 735f 6361 7669 7479  t_options_cavity
-00351f80: 2720 3d20 4e6f 6e65 0a0a 5649 4557 3344  ' = None..VIEW3D
-00351f90: 5f50 545f 746f 6f6c 735f 696d 6167 6570  _PT_tools_imagep
-00351fa0: 6169 6e74 5f6f 7074 696f 6e73 5f65 7874  aint_options_ext
-00351fb0: 6572 6e61 6c3a 2027 626c 5f75 692e 7370  ernal: 'bl_ui.sp
-00351fc0: 6163 655f 7669 6577 3364 5f74 6f6f 6c62  ace_view3d_toolb
-00351fd0: 6172 2e56 4945 5733 445f 5054 5f74 6f6f  ar.VIEW3D_PT_too
-00351fe0: 6c73 5f69 6d61 6765 7061 696e 745f 6f70  ls_imagepaint_op
-00351ff0: 7469 6f6e 735f 6578 7465 726e 616c 2720  tions_external' 
-00352000: 3d20 4e6f 6e65 0a0a 5649 4557 3344 5f50  = None..VIEW3D_P
-00352010: 545f 746f 6f6c 735f 696d 6167 6570 6169  T_tools_imagepai
-00352020: 6e74 5f73 796d 6d65 7472 793a 2027 626c  nt_symmetry: 'bl
-00352030: 5f75 692e 7370 6163 655f 7669 6577 3364  _ui.space_view3d
-00352040: 5f74 6f6f 6c62 6172 2e56 4945 5733 445f  _toolbar.VIEW3D_
-00352050: 5054 5f74 6f6f 6c73 5f69 6d61 6765 7061  PT_tools_imagepa
-00352060: 696e 745f 7379 6d6d 6574 7279 2720 3d20  int_symmetry' = 
-00352070: 4e6f 6e65 0a0a 5649 4557 3344 5f50 545f  None..VIEW3D_PT_
-00352080: 746f 6f6c 735f 6d61 736b 5f74 6578 7475  tools_mask_textu
-00352090: 7265 3a20 2762 6c5f 7569 2e73 7061 6365  re: 'bl_ui.space
-003520a0: 5f76 6965 7733 645f 746f 6f6c 6261 722e  _view3d_toolbar.
-003520b0: 5649 4557 3344 5f50 545f 746f 6f6c 735f  VIEW3D_PT_tools_
-003520c0: 6d61 736b 5f74 6578 7475 7265 2720 3d20  mask_texture' = 
-003520d0: 4e6f 6e65 0a0a 5649 4557 3344 5f50 545f  None..VIEW3D_PT_
-003520e0: 746f 6f6c 735f 6d65 7368 6564 6974 5f6f  tools_meshedit_o
-003520f0: 7074 696f 6e73 3a20 2762 6c5f 7569 2e73  ptions: 'bl_ui.s
-00352100: 7061 6365 5f76 6965 7733 645f 746f 6f6c  pace_view3d_tool
-00352110: 6261 722e 5649 4557 3344 5f50 545f 746f  bar.VIEW3D_PT_to
-00352120: 6f6c 735f 6d65 7368 6564 6974 5f6f 7074  ols_meshedit_opt
-00352130: 696f 6e73 2720 3d20 4e6f 6e65 0a0a 5649  ions' = None..VI
-00352140: 4557 3344 5f50 545f 746f 6f6c 735f 6d65  EW3D_PT_tools_me
-00352150: 7368 6564 6974 5f6f 7074 696f 6e73 5f74  shedit_options_t
-00352160: 7261 6e73 666f 726d 3a20 2762 6c5f 7569  ransform: 'bl_ui
-00352170: 2e73 7061 6365 5f76 6965 7733 645f 746f  .space_view3d_to
-00352180: 6f6c 6261 722e 5649 4557 3344 5f50 545f  olbar.VIEW3D_PT_
-00352190: 746f 6f6c 735f 6d65 7368 6564 6974 5f6f  tools_meshedit_o
-003521a0: 7074 696f 6e73 5f74 7261 6e73 666f 726d  ptions_transform
-003521b0: 2720 3d20 4e6f 6e65 0a0a 5649 4557 3344  ' = None..VIEW3D
-003521c0: 5f50 545f 746f 6f6c 735f 6d65 7368 6564  _PT_tools_meshed
-003521d0: 6974 5f6f 7074 696f 6e73 5f75 7673 3a20  it_options_uvs: 
-003521e0: 2762 6c5f 7569 2e73 7061 6365 5f76 6965  'bl_ui.space_vie
-003521f0: 7733 645f 746f 6f6c 6261 722e 5649 4557  w3d_toolbar.VIEW
-00352200: 3344 5f50 545f 746f 6f6c 735f 6d65 7368  3D_PT_tools_mesh
-00352210: 6564 6974 5f6f 7074 696f 6e73 5f75 7673  edit_options_uvs
-00352220: 2720 3d20 4e6f 6e65 0a0a 5649 4557 3344  ' = None..VIEW3D
-00352230: 5f50 545f 746f 6f6c 735f 6f62 6a65 6374  _PT_tools_object
-00352240: 5f6f 7074 696f 6e73 3a20 2762 6c5f 7569  _options: 'bl_ui
-00352250: 2e73 7061 6365 5f76 6965 7733 645f 746f  .space_view3d_to
-00352260: 6f6c 6261 722e 5649 4557 3344 5f50 545f  olbar.VIEW3D_PT_
-00352270: 746f 6f6c 735f 6f62 6a65 6374 5f6f 7074  tools_object_opt
-00352280: 696f 6e73 2720 3d20 4e6f 6e65 0a0a 5649  ions' = None..VI
-00352290: 4557 3344 5f50 545f 746f 6f6c 735f 6f62  EW3D_PT_tools_ob
-003522a0: 6a65 6374 5f6f 7074 696f 6e73 5f74 7261  ject_options_tra
-003522b0: 6e73 666f 726d 3a20 2762 6c5f 7569 2e73  nsform: 'bl_ui.s
-003522c0: 7061 6365 5f76 6965 7733 645f 746f 6f6c  pace_view3d_tool
-003522d0: 6261 722e 5649 4557 3344 5f50 545f 746f  bar.VIEW3D_PT_to
-003522e0: 6f6c 735f 6f62 6a65 6374 5f6f 7074 696f  ols_object_optio
-003522f0: 6e73 5f74 7261 6e73 666f 726d 2720 3d20  ns_transform' = 
-00352300: 4e6f 6e65 0a0a 5649 4557 3344 5f50 545f  None..VIEW3D_PT_
-00352310: 746f 6f6c 735f 7061 7274 6963 6c65 6d6f  tools_particlemo
-00352320: 6465 3a20 2762 6c5f 7569 2e73 7061 6365  de: 'bl_ui.space
-00352330: 5f76 6965 7733 645f 746f 6f6c 6261 722e  _view3d_toolbar.
-00352340: 5649 4557 3344 5f50 545f 746f 6f6c 735f  VIEW3D_PT_tools_
-00352350: 7061 7274 6963 6c65 6d6f 6465 2720 3d20  particlemode' = 
-00352360: 4e6f 6e65 0a0a 5649 4557 3344 5f50 545f  None..VIEW3D_PT_
-00352370: 746f 6f6c 735f 7061 7274 6963 6c65 6d6f  tools_particlemo
-00352380: 6465 5f6f 7074 696f 6e73 3a20 2762 6c5f  de_options: 'bl_
-00352390: 7569 2e73 7061 6365 5f76 6965 7733 645f  ui.space_view3d_
-003523a0: 746f 6f6c 6261 722e 5649 4557 3344 5f50  toolbar.VIEW3D_P
-003523b0: 545f 746f 6f6c 735f 7061 7274 6963 6c65  T_tools_particle
-003523c0: 6d6f 6465 5f6f 7074 696f 6e73 2720 3d20  mode_options' = 
-003523d0: 4e6f 6e65 0a0a 5649 4557 3344 5f50 545f  None..VIEW3D_PT_
-003523e0: 746f 6f6c 735f 7061 7274 6963 6c65 6d6f  tools_particlemo
-003523f0: 6465 5f6f 7074 696f 6e73 5f64 6973 706c  de_options_displ
-00352400: 6179 3a20 2762 6c5f 7569 2e73 7061 6365  ay: 'bl_ui.space
-00352410: 5f76 6965 7733 645f 746f 6f6c 6261 722e  _view3d_toolbar.
-00352420: 5649 4557 3344 5f50 545f 746f 6f6c 735f  VIEW3D_PT_tools_
-00352430: 7061 7274 6963 6c65 6d6f 6465 5f6f 7074  particlemode_opt
-00352440: 696f 6e73 5f64 6973 706c 6179 2720 3d20  ions_display' = 
-00352450: 4e6f 6e65 0a0a 5649 4557 3344 5f50 545f  None..VIEW3D_PT_
-00352460: 746f 6f6c 735f 7061 7274 6963 6c65 6d6f  tools_particlemo
-00352470: 6465 5f6f 7074 696f 6e73 5f73 6861 7065  de_options_shape
-00352480: 6375 743a 2027 626c 5f75 692e 7370 6163  cut: 'bl_ui.spac
-00352490: 655f 7669 6577 3364 5f74 6f6f 6c62 6172  e_view3d_toolbar
-003524a0: 2e56 4945 5733 445f 5054 5f74 6f6f 6c73  .VIEW3D_PT_tools
-003524b0: 5f70 6172 7469 636c 656d 6f64 655f 6f70  _particlemode_op
-003524c0: 7469 6f6e 735f 7368 6170 6563 7574 2720  tions_shapecut' 
-003524d0: 3d20 4e6f 6e65 0a0a 5649 4557 3344 5f50  = None..VIEW3D_P
-003524e0: 545f 746f 6f6c 735f 706f 7365 6d6f 6465  T_tools_posemode
-003524f0: 5f6f 7074 696f 6e73 3a20 2762 6c5f 7569  _options: 'bl_ui
-00352500: 2e73 7061 6365 5f76 6965 7733 645f 746f  .space_view3d_to
-00352510: 6f6c 6261 722e 5649 4557 3344 5f50 545f  olbar.VIEW3D_PT_
-00352520: 746f 6f6c 735f 706f 7365 6d6f 6465 5f6f  tools_posemode_o
-00352530: 7074 696f 6e73 2720 3d20 4e6f 6e65 0a0a  ptions' = None..
-00352540: 5649 4557 3344 5f50 545f 746f 6f6c 735f  VIEW3D_PT_tools_
-00352550: 7665 7274 6578 7061 696e 745f 6f70 7469  vertexpaint_opti
-00352560: 6f6e 733a 2027 626c 5f75 692e 7370 6163  ons: 'bl_ui.spac
-00352570: 655f 7669 6577 3364 5f74 6f6f 6c62 6172  e_view3d_toolbar
-00352580: 2e56 4945 5733 445f 5054 5f74 6f6f 6c73  .VIEW3D_PT_tools
-00352590: 5f76 6572 7465 7870 6169 6e74 5f6f 7074  _vertexpaint_opt
-003525a0: 696f 6e73 2720 3d20 4e6f 6e65 0a0a 5649  ions' = None..VI
-003525b0: 4557 3344 5f50 545f 746f 6f6c 735f 7665  EW3D_PT_tools_ve
-003525c0: 7274 6578 7061 696e 745f 7379 6d6d 6574  rtexpaint_symmet
-003525d0: 7279 3a20 2762 6c5f 7569 2e73 7061 6365  ry: 'bl_ui.space
-003525e0: 5f76 6965 7733 645f 746f 6f6c 6261 722e  _view3d_toolbar.
-003525f0: 5649 4557 3344 5f50 545f 746f 6f6c 735f  VIEW3D_PT_tools_
-00352600: 7665 7274 6578 7061 696e 745f 7379 6d6d  vertexpaint_symm
-00352610: 6574 7279 2720 3d20 4e6f 6e65 0a0a 5649  etry' = None..VI
-00352620: 4557 3344 5f50 545f 746f 6f6c 735f 7665  EW3D_PT_tools_ve
-00352630: 7274 6578 7061 696e 745f 7379 6d6d 6574  rtexpaint_symmet
-00352640: 7279 5f66 6f72 5f74 6f70 6261 723a 2027  ry_for_topbar: '
-00352650: 626c 5f75 692e 7370 6163 655f 7669 6577  bl_ui.space_view
-00352660: 3364 5f74 6f6f 6c62 6172 2e56 4945 5733  3d_toolbar.VIEW3
-00352670: 445f 5054 5f74 6f6f 6c73 5f76 6572 7465  D_PT_tools_verte
-00352680: 7870 6169 6e74 5f73 796d 6d65 7472 795f  xpaint_symmetry_
-00352690: 666f 725f 746f 7062 6172 2720 3d20 4e6f  for_topbar' = No
-003526a0: 6e65 0a0a 5649 4557 3344 5f50 545f 746f  ne..VIEW3D_PT_to
-003526b0: 6f6c 735f 7765 6967 6874 5f67 7261 6469  ols_weight_gradi
-003526c0: 656e 743a 2027 626c 5f75 692e 7370 6163  ent: 'bl_ui.spac
-003526d0: 655f 7669 6577 3364 5f74 6f6f 6c62 6172  e_view3d_toolbar
-003526e0: 2e56 4945 5733 445f 5054 5f74 6f6f 6c73  .VIEW3D_PT_tools
-003526f0: 5f77 6569 6768 745f 6772 6164 6965 6e74  _weight_gradient
+003501d0: 545f 7061 696e 745f 7765 6967 6874 5f63  T_paint_weight_c
+003501e0: 6f6e 7465 7874 5f6d 656e 753a 2027 626c  ontext_menu: 'bl
+003501f0: 5f75 692e 7370 6163 655f 7669 6577 3364  _ui.space_view3d
+00350200: 2e56 4945 5733 445f 5054 5f70 6169 6e74  .VIEW3D_PT_paint
+00350210: 5f77 6569 6768 745f 636f 6e74 6578 745f  _weight_context_
+00350220: 6d65 6e75 2720 3d20 4e6f 6e65 0a0a 5649  menu' = None..VI
+00350230: 4557 3344 5f50 545f 7072 6f70 6f72 7469  EW3D_PT_proporti
+00350240: 6f6e 616c 5f65 6469 743a 2027 626c 5f75  onal_edit: 'bl_u
+00350250: 692e 7370 6163 655f 7669 6577 3364 2e56  i.space_view3d.V
+00350260: 4945 5733 445f 5054 5f70 726f 706f 7274  IEW3D_PT_proport
+00350270: 696f 6e61 6c5f 6564 6974 2720 3d20 4e6f  ional_edit' = No
+00350280: 6e65 0a0a 5649 4557 3344 5f50 545f 7175  ne..VIEW3D_PT_qu
+00350290: 6164 5f76 6965 773a 2027 626c 5f75 692e  ad_view: 'bl_ui.
+003502a0: 7370 6163 655f 7669 6577 3364 2e56 4945  space_view3d.VIE
+003502b0: 5733 445f 5054 5f71 7561 645f 7669 6577  W3D_PT_quad_view
+003502c0: 2720 3d20 4e6f 6e65 0a0a 5649 4557 3344  ' = None..VIEW3D
+003502d0: 5f50 545f 7363 756c 7074 5f61 7574 6f6d  _PT_sculpt_autom
+003502e0: 6173 6b69 6e67 3a20 2762 6c5f 7569 2e73  asking: 'bl_ui.s
+003502f0: 7061 6365 5f76 6965 7733 642e 5649 4557  pace_view3d.VIEW
+00350300: 3344 5f50 545f 7363 756c 7074 5f61 7574  3D_PT_sculpt_aut
+00350310: 6f6d 6173 6b69 6e67 2720 3d20 4e6f 6e65  omasking' = None
+00350320: 0a0a 5649 4557 3344 5f50 545f 7363 756c  ..VIEW3D_PT_scul
+00350330: 7074 5f63 6f6e 7465 7874 5f6d 656e 753a  pt_context_menu:
+00350340: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
+00350350: 6577 3364 2e56 4945 5733 445f 5054 5f73  ew3d.VIEW3D_PT_s
+00350360: 6375 6c70 745f 636f 6e74 6578 745f 6d65  culpt_context_me
+00350370: 6e75 2720 3d20 4e6f 6e65 0a0a 5649 4557  nu' = None..VIEW
+00350380: 3344 5f50 545f 7363 756c 7074 5f64 796e  3D_PT_sculpt_dyn
+00350390: 746f 706f 3a20 2762 6c5f 7569 2e73 7061  topo: 'bl_ui.spa
+003503a0: 6365 5f76 6965 7733 645f 746f 6f6c 6261  ce_view3d_toolba
+003503b0: 722e 5649 4557 3344 5f50 545f 7363 756c  r.VIEW3D_PT_scul
+003503c0: 7074 5f64 796e 746f 706f 2720 3d20 4e6f  pt_dyntopo' = No
+003503d0: 6e65 0a0a 5649 4557 3344 5f50 545f 7363  ne..VIEW3D_PT_sc
+003503e0: 756c 7074 5f6f 7074 696f 6e73 3a20 2762  ulpt_options: 'b
+003503f0: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
+00350400: 645f 746f 6f6c 6261 722e 5649 4557 3344  d_toolbar.VIEW3D
+00350410: 5f50 545f 7363 756c 7074 5f6f 7074 696f  _PT_sculpt_optio
+00350420: 6e73 2720 3d20 4e6f 6e65 0a0a 5649 4557  ns' = None..VIEW
+00350430: 3344 5f50 545f 7363 756c 7074 5f6f 7074  3D_PT_sculpt_opt
+00350440: 696f 6e73 5f67 7261 7669 7479 3a20 2762  ions_gravity: 'b
+00350450: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
+00350460: 645f 746f 6f6c 6261 722e 5649 4557 3344  d_toolbar.VIEW3D
+00350470: 5f50 545f 7363 756c 7074 5f6f 7074 696f  _PT_sculpt_optio
+00350480: 6e73 5f67 7261 7669 7479 2720 3d20 4e6f  ns_gravity' = No
+00350490: 6e65 0a0a 5649 4557 3344 5f50 545f 7363  ne..VIEW3D_PT_sc
+003504a0: 756c 7074 5f73 796d 6d65 7472 793a 2027  ulpt_symmetry: '
+003504b0: 626c 5f75 692e 7370 6163 655f 7669 6577  bl_ui.space_view
+003504c0: 3364 5f74 6f6f 6c62 6172 2e56 4945 5733  3d_toolbar.VIEW3
+003504d0: 445f 5054 5f73 6375 6c70 745f 7379 6d6d  D_PT_sculpt_symm
+003504e0: 6574 7279 2720 3d20 4e6f 6e65 0a0a 5649  etry' = None..VI
+003504f0: 4557 3344 5f50 545f 7363 756c 7074 5f73  EW3D_PT_sculpt_s
+00350500: 796d 6d65 7472 795f 666f 725f 746f 7062  ymmetry_for_topb
+00350510: 6172 3a20 2762 6c5f 7569 2e73 7061 6365  ar: 'bl_ui.space
+00350520: 5f76 6965 7733 645f 746f 6f6c 6261 722e  _view3d_toolbar.
+00350530: 5649 4557 3344 5f50 545f 7363 756c 7074  VIEW3D_PT_sculpt
+00350540: 5f73 796d 6d65 7472 795f 666f 725f 746f  _symmetry_for_to
+00350550: 7062 6172 2720 3d20 4e6f 6e65 0a0a 5649  pbar' = None..VI
+00350560: 4557 3344 5f50 545f 7363 756c 7074 5f76  EW3D_PT_sculpt_v
+00350570: 6f78 656c 5f72 656d 6573 683a 2027 626c  oxel_remesh: 'bl
+00350580: 5f75 692e 7370 6163 655f 7669 6577 3364  _ui.space_view3d
+00350590: 5f74 6f6f 6c62 6172 2e56 4945 5733 445f  _toolbar.VIEW3D_
+003505a0: 5054 5f73 6375 6c70 745f 766f 7865 6c5f  PT_sculpt_voxel_
+003505b0: 7265 6d65 7368 2720 3d20 4e6f 6e65 0a0a  remesh' = None..
+003505c0: 5649 4557 3344 5f50 545f 7368 6164 696e  VIEW3D_PT_shadin
+003505d0: 673a 2027 626c 5f75 692e 7370 6163 655f  g: 'bl_ui.space_
+003505e0: 7669 6577 3364 2e56 4945 5733 445f 5054  view3d.VIEW3D_PT
+003505f0: 5f73 6861 6469 6e67 2720 3d20 4e6f 6e65  _shading' = None
+00350600: 0a0a 5649 4557 3344 5f50 545f 7368 6164  ..VIEW3D_PT_shad
+00350610: 696e 675f 636f 6c6f 723a 2027 626c 5f75  ing_color: 'bl_u
+00350620: 692e 7370 6163 655f 7669 6577 3364 2e56  i.space_view3d.V
+00350630: 4945 5733 445f 5054 5f73 6861 6469 6e67  IEW3D_PT_shading
+00350640: 5f63 6f6c 6f72 2720 3d20 4e6f 6e65 0a0a  _color' = None..
+00350650: 5649 4557 3344 5f50 545f 7368 6164 696e  VIEW3D_PT_shadin
+00350660: 675f 636f 6d70 6f73 6974 6f72 3a20 2762  g_compositor: 'b
+00350670: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
+00350680: 642e 5649 4557 3344 5f50 545f 7368 6164  d.VIEW3D_PT_shad
+00350690: 696e 675f 636f 6d70 6f73 6974 6f72 2720  ing_compositor' 
+003506a0: 3d20 4e6f 6e65 0a0a 5649 4557 3344 5f50  = None..VIEW3D_P
+003506b0: 545f 7368 6164 696e 675f 6c69 6768 7469  T_shading_lighti
+003506c0: 6e67 3a20 2762 6c5f 7569 2e73 7061 6365  ng: 'bl_ui.space
+003506d0: 5f76 6965 7733 642e 5649 4557 3344 5f50  _view3d.VIEW3D_P
+003506e0: 545f 7368 6164 696e 675f 6c69 6768 7469  T_shading_lighti
+003506f0: 6e67 2720 3d20 4e6f 6e65 0a0a 5649 4557  ng' = None..VIEW
+00350700: 3344 5f50 545f 7368 6164 696e 675f 6f70  3D_PT_shading_op
+00350710: 7469 6f6e 733a 2027 626c 5f75 692e 7370  tions: 'bl_ui.sp
+00350720: 6163 655f 7669 6577 3364 2e56 4945 5733  ace_view3d.VIEW3
+00350730: 445f 5054 5f73 6861 6469 6e67 5f6f 7074  D_PT_shading_opt
+00350740: 696f 6e73 2720 3d20 4e6f 6e65 0a0a 5649  ions' = None..VI
+00350750: 4557 3344 5f50 545f 7368 6164 696e 675f  EW3D_PT_shading_
+00350760: 6f70 7469 6f6e 735f 7368 6164 6f77 3a20  options_shadow: 
+00350770: 2762 6c5f 7569 2e73 7061 6365 5f76 6965  'bl_ui.space_vie
+00350780: 7733 642e 5649 4557 3344 5f50 545f 7368  w3d.VIEW3D_PT_sh
+00350790: 6164 696e 675f 6f70 7469 6f6e 735f 7368  ading_options_sh
+003507a0: 6164 6f77 2720 3d20 4e6f 6e65 0a0a 5649  adow' = None..VI
+003507b0: 4557 3344 5f50 545f 7368 6164 696e 675f  EW3D_PT_shading_
+003507c0: 6f70 7469 6f6e 735f 7373 616f 3a20 2762  options_ssao: 'b
+003507d0: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
+003507e0: 642e 5649 4557 3344 5f50 545f 7368 6164  d.VIEW3D_PT_shad
+003507f0: 696e 675f 6f70 7469 6f6e 735f 7373 616f  ing_options_ssao
+00350800: 2720 3d20 4e6f 6e65 0a0a 5649 4557 3344  ' = None..VIEW3D
+00350810: 5f50 545f 7368 6164 696e 675f 7265 6e64  _PT_shading_rend
+00350820: 6572 5f70 6173 733a 2027 626c 5f75 692e  er_pass: 'bl_ui.
+00350830: 7370 6163 655f 7669 6577 3364 2e56 4945  space_view3d.VIE
+00350840: 5733 445f 5054 5f73 6861 6469 6e67 5f72  W3D_PT_shading_r
+00350850: 656e 6465 725f 7061 7373 2720 3d20 4e6f  ender_pass' = No
+00350860: 6e65 0a0a 5649 4557 3344 5f50 545f 736c  ne..VIEW3D_PT_sl
+00350870: 6f74 735f 7061 696e 745f 6361 6e76 6173  ots_paint_canvas
+00350880: 3a20 2762 6c5f 7569 2e73 7061 6365 5f76  : 'bl_ui.space_v
+00350890: 6965 7733 645f 746f 6f6c 6261 722e 5649  iew3d_toolbar.VI
+003508a0: 4557 3344 5f50 545f 736c 6f74 735f 7061  EW3D_PT_slots_pa
+003508b0: 696e 745f 6361 6e76 6173 2720 3d20 4e6f  int_canvas' = No
+003508c0: 6e65 0a0a 5649 4557 3344 5f50 545f 736c  ne..VIEW3D_PT_sl
+003508d0: 6f74 735f 7072 6f6a 6563 7470 6169 6e74  ots_projectpaint
+003508e0: 3a20 2762 6c5f 7569 2e73 7061 6365 5f76  : 'bl_ui.space_v
+003508f0: 6965 7733 645f 746f 6f6c 6261 722e 5649  iew3d_toolbar.VI
+00350900: 4557 3344 5f50 545f 736c 6f74 735f 7072  EW3D_PT_slots_pr
+00350910: 6f6a 6563 7470 6169 6e74 2720 3d20 4e6f  ojectpaint' = No
+00350920: 6e65 0a0a 5649 4557 3344 5f50 545f 736e  ne..VIEW3D_PT_sn
+00350930: 6170 7069 6e67 3a20 2762 6c5f 7569 2e73  apping: 'bl_ui.s
+00350940: 7061 6365 5f76 6965 7733 642e 5649 4557  pace_view3d.VIEW
+00350950: 3344 5f50 545f 736e 6170 7069 6e67 2720  3D_PT_snapping' 
+00350960: 3d20 4e6f 6e65 0a0a 5649 4557 3344 5f50  = None..VIEW3D_P
+00350970: 545f 7374 656e 6369 6c5f 7072 6f6a 6563  T_stencil_projec
+00350980: 7470 6169 6e74 3a20 2762 6c5f 7569 2e73  tpaint: 'bl_ui.s
+00350990: 7061 6365 5f76 6965 7733 645f 746f 6f6c  pace_view3d_tool
+003509a0: 6261 722e 5649 4557 3344 5f50 545f 7374  bar.VIEW3D_PT_st
+003509b0: 656e 6369 6c5f 7072 6f6a 6563 7470 6169  encil_projectpai
+003509c0: 6e74 2720 3d20 4e6f 6e65 0a0a 5649 4557  nt' = None..VIEW
+003509d0: 3344 5f50 545f 746f 6f6c 735f 6163 7469  3D_PT_tools_acti
+003509e0: 7665 3a20 2762 6c5f 7569 2e73 7061 6365  ve: 'bl_ui.space
+003509f0: 5f74 6f6f 6c73 7973 7465 6d5f 746f 6f6c  _toolsystem_tool
+00350a00: 6261 722e 5649 4557 3344 5f50 545f 746f  bar.VIEW3D_PT_to
+00350a10: 6f6c 735f 6163 7469 7665 2720 3d20 4e6f  ols_active' = No
+00350a20: 6e65 0a0a 5649 4557 3344 5f50 545f 746f  ne..VIEW3D_PT_to
+00350a30: 6f6c 735f 6172 6d61 7475 7265 6564 6974  ols_armatureedit
+00350a40: 5f6f 7074 696f 6e73 3a20 2762 6c5f 7569  _options: 'bl_ui
+00350a50: 2e73 7061 6365 5f76 6965 7733 645f 746f  .space_view3d_to
+00350a60: 6f6c 6261 722e 5649 4557 3344 5f50 545f  olbar.VIEW3D_PT_
+00350a70: 746f 6f6c 735f 6172 6d61 7475 7265 6564  tools_armatureed
+00350a80: 6974 5f6f 7074 696f 6e73 2720 3d20 4e6f  it_options' = No
+00350a90: 6e65 0a0a 5649 4557 3344 5f50 545f 746f  ne..VIEW3D_PT_to
+00350aa0: 6f6c 735f 6272 7573 685f 636c 6f6e 653a  ols_brush_clone:
+00350ab0: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
+00350ac0: 6577 3364 5f74 6f6f 6c62 6172 2e56 4945  ew3d_toolbar.VIE
+00350ad0: 5733 445f 5054 5f74 6f6f 6c73 5f62 7275  W3D_PT_tools_bru
+00350ae0: 7368 5f63 6c6f 6e65 2720 3d20 4e6f 6e65  sh_clone' = None
+00350af0: 0a0a 5649 4557 3344 5f50 545f 746f 6f6c  ..VIEW3D_PT_tool
+00350b00: 735f 6272 7573 685f 636f 6c6f 723a 2027  s_brush_color: '
+00350b10: 626c 5f75 692e 7370 6163 655f 7669 6577  bl_ui.space_view
+00350b20: 3364 5f74 6f6f 6c62 6172 2e56 4945 5733  3d_toolbar.VIEW3
+00350b30: 445f 5054 5f74 6f6f 6c73 5f62 7275 7368  D_PT_tools_brush
+00350b40: 5f63 6f6c 6f72 2720 3d20 4e6f 6e65 0a0a  _color' = None..
+00350b50: 5649 4557 3344 5f50 545f 746f 6f6c 735f  VIEW3D_PT_tools_
+00350b60: 6272 7573 685f 6469 7370 6c61 793a 2027  brush_display: '
+00350b70: 626c 5f75 692e 7370 6163 655f 7669 6577  bl_ui.space_view
+00350b80: 3364 5f74 6f6f 6c62 6172 2e56 4945 5733  3d_toolbar.VIEW3
+00350b90: 445f 5054 5f74 6f6f 6c73 5f62 7275 7368  D_PT_tools_brush
+00350ba0: 5f64 6973 706c 6179 2720 3d20 4e6f 6e65  _display' = None
+00350bb0: 0a0a 5649 4557 3344 5f50 545f 746f 6f6c  ..VIEW3D_PT_tool
+00350bc0: 735f 6272 7573 685f 6661 6c6c 6f66 663a  s_brush_falloff:
+00350bd0: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
+00350be0: 6577 3364 5f74 6f6f 6c62 6172 2e56 4945  ew3d_toolbar.VIE
+00350bf0: 5733 445f 5054 5f74 6f6f 6c73 5f62 7275  W3D_PT_tools_bru
+00350c00: 7368 5f66 616c 6c6f 6666 2720 3d20 4e6f  sh_falloff' = No
+00350c10: 6e65 0a0a 5649 4557 3344 5f50 545f 746f  ne..VIEW3D_PT_to
+00350c20: 6f6c 735f 6272 7573 685f 6661 6c6c 6f66  ols_brush_fallof
+00350c30: 665f 6672 6f6e 7466 6163 653a 2027 626c  f_frontface: 'bl
+00350c40: 5f75 692e 7370 6163 655f 7669 6577 3364  _ui.space_view3d
+00350c50: 5f74 6f6f 6c62 6172 2e56 4945 5733 445f  _toolbar.VIEW3D_
+00350c60: 5054 5f74 6f6f 6c73 5f62 7275 7368 5f66  PT_tools_brush_f
+00350c70: 616c 6c6f 6666 5f66 726f 6e74 6661 6365  alloff_frontface
+00350c80: 2720 3d20 4e6f 6e65 0a0a 5649 4557 3344  ' = None..VIEW3D
+00350c90: 5f50 545f 746f 6f6c 735f 6272 7573 685f  _PT_tools_brush_
+00350ca0: 6661 6c6c 6f66 665f 6e6f 726d 616c 3a20  falloff_normal: 
+00350cb0: 2762 6c5f 7569 2e73 7061 6365 5f76 6965  'bl_ui.space_vie
+00350cc0: 7733 645f 746f 6f6c 6261 722e 5649 4557  w3d_toolbar.VIEW
+00350cd0: 3344 5f50 545f 746f 6f6c 735f 6272 7573  3D_PT_tools_brus
+00350ce0: 685f 6661 6c6c 6f66 665f 6e6f 726d 616c  h_falloff_normal
+00350cf0: 2720 3d20 4e6f 6e65 0a0a 5649 4557 3344  ' = None..VIEW3D
+00350d00: 5f50 545f 746f 6f6c 735f 6272 7573 685f  _PT_tools_brush_
+00350d10: 7365 6c65 6374 3a20 2762 6c5f 7569 2e73  select: 'bl_ui.s
+00350d20: 7061 6365 5f76 6965 7733 645f 746f 6f6c  pace_view3d_tool
+00350d30: 6261 722e 5649 4557 3344 5f50 545f 746f  bar.VIEW3D_PT_to
+00350d40: 6f6c 735f 6272 7573 685f 7365 6c65 6374  ols_brush_select
+00350d50: 2720 3d20 4e6f 6e65 0a0a 5649 4557 3344  ' = None..VIEW3D
+00350d60: 5f50 545f 746f 6f6c 735f 6272 7573 685f  _PT_tools_brush_
+00350d70: 7365 7474 696e 6773 3a20 2762 6c5f 7569  settings: 'bl_ui
+00350d80: 2e73 7061 6365 5f76 6965 7733 645f 746f  .space_view3d_to
+00350d90: 6f6c 6261 722e 5649 4557 3344 5f50 545f  olbar.VIEW3D_PT_
+00350da0: 746f 6f6c 735f 6272 7573 685f 7365 7474  tools_brush_sett
+00350db0: 696e 6773 2720 3d20 4e6f 6e65 0a0a 5649  ings' = None..VI
+00350dc0: 4557 3344 5f50 545f 746f 6f6c 735f 6272  EW3D_PT_tools_br
+00350dd0: 7573 685f 7365 7474 696e 6773 5f61 6476  ush_settings_adv
+00350de0: 616e 6365 643a 2027 626c 5f75 692e 7370  anced: 'bl_ui.sp
+00350df0: 6163 655f 7669 6577 3364 5f74 6f6f 6c62  ace_view3d_toolb
+00350e00: 6172 2e56 4945 5733 445f 5054 5f74 6f6f  ar.VIEW3D_PT_too
+00350e10: 6c73 5f62 7275 7368 5f73 6574 7469 6e67  ls_brush_setting
+00350e20: 735f 6164 7661 6e63 6564 2720 3d20 4e6f  s_advanced' = No
+00350e30: 6e65 0a0a 5649 4557 3344 5f50 545f 746f  ne..VIEW3D_PT_to
+00350e40: 6f6c 735f 6272 7573 685f 7374 726f 6b65  ols_brush_stroke
+00350e50: 3a20 2762 6c5f 7569 2e73 7061 6365 5f76  : 'bl_ui.space_v
+00350e60: 6965 7733 645f 746f 6f6c 6261 722e 5649  iew3d_toolbar.VI
+00350e70: 4557 3344 5f50 545f 746f 6f6c 735f 6272  EW3D_PT_tools_br
+00350e80: 7573 685f 7374 726f 6b65 2720 3d20 4e6f  ush_stroke' = No
+00350e90: 6e65 0a0a 5649 4557 3344 5f50 545f 746f  ne..VIEW3D_PT_to
+00350ea0: 6f6c 735f 6272 7573 685f 7374 726f 6b65  ols_brush_stroke
+00350eb0: 5f73 6d6f 6f74 685f 7374 726f 6b65 3a20  _smooth_stroke: 
+00350ec0: 2762 6c5f 7569 2e73 7061 6365 5f76 6965  'bl_ui.space_vie
+00350ed0: 7733 645f 746f 6f6c 6261 722e 5649 4557  w3d_toolbar.VIEW
+00350ee0: 3344 5f50 545f 746f 6f6c 735f 6272 7573  3D_PT_tools_brus
+00350ef0: 685f 7374 726f 6b65 5f73 6d6f 6f74 685f  h_stroke_smooth_
+00350f00: 7374 726f 6b65 2720 3d20 4e6f 6e65 0a0a  stroke' = None..
+00350f10: 5649 4557 3344 5f50 545f 746f 6f6c 735f  VIEW3D_PT_tools_
+00350f20: 6272 7573 685f 7377 6174 6368 6573 3a20  brush_swatches: 
+00350f30: 2762 6c5f 7569 2e73 7061 6365 5f76 6965  'bl_ui.space_vie
+00350f40: 7733 645f 746f 6f6c 6261 722e 5649 4557  w3d_toolbar.VIEW
+00350f50: 3344 5f50 545f 746f 6f6c 735f 6272 7573  3D_PT_tools_brus
+00350f60: 685f 7377 6174 6368 6573 2720 3d20 4e6f  h_swatches' = No
+00350f70: 6e65 0a0a 5649 4557 3344 5f50 545f 746f  ne..VIEW3D_PT_to
+00350f80: 6f6c 735f 6272 7573 685f 7465 7874 7572  ols_brush_textur
+00350f90: 653a 2027 626c 5f75 692e 7370 6163 655f  e: 'bl_ui.space_
+00350fa0: 7669 6577 3364 5f74 6f6f 6c62 6172 2e56  view3d_toolbar.V
+00350fb0: 4945 5733 445f 5054 5f74 6f6f 6c73 5f62  IEW3D_PT_tools_b
+00350fc0: 7275 7368 5f74 6578 7475 7265 2720 3d20  rush_texture' = 
+00350fd0: 4e6f 6e65 0a0a 5649 4557 3344 5f50 545f  None..VIEW3D_PT_
+00350fe0: 746f 6f6c 735f 6772 6561 7365 5f70 656e  tools_grease_pen
+00350ff0: 6369 6c5f 6272 7573 685f 6164 7661 6e63  cil_brush_advanc
+00351000: 6564 3a20 2762 6c5f 7569 2e73 7061 6365  ed: 'bl_ui.space
+00351010: 5f76 6965 7733 645f 746f 6f6c 6261 722e  _view3d_toolbar.
+00351020: 5649 4557 3344 5f50 545f 746f 6f6c 735f  VIEW3D_PT_tools_
+00351030: 6772 6561 7365 5f70 656e 6369 6c5f 6272  grease_pencil_br
+00351040: 7573 685f 6164 7661 6e63 6564 2720 3d20  ush_advanced' = 
+00351050: 4e6f 6e65 0a0a 5649 4557 3344 5f50 545f  None..VIEW3D_PT_
+00351060: 746f 6f6c 735f 6772 6561 7365 5f70 656e  tools_grease_pen
+00351070: 6369 6c5f 6272 7573 685f 6761 705f 636c  cil_brush_gap_cl
+00351080: 6f73 7572 653a 2027 626c 5f75 692e 7370  osure: 'bl_ui.sp
+00351090: 6163 655f 7669 6577 3364 5f74 6f6f 6c62  ace_view3d_toolb
+003510a0: 6172 2e56 4945 5733 445f 5054 5f74 6f6f  ar.VIEW3D_PT_too
+003510b0: 6c73 5f67 7265 6173 655f 7065 6e63 696c  ls_grease_pencil
+003510c0: 5f62 7275 7368 5f67 6170 5f63 6c6f 7375  _brush_gap_closu
+003510d0: 7265 2720 3d20 4e6f 6e65 0a0a 5649 4557  re' = None..VIEW
+003510e0: 3344 5f50 545f 746f 6f6c 735f 6772 6561  3D_PT_tools_grea
+003510f0: 7365 5f70 656e 6369 6c5f 6272 7573 685f  se_pencil_brush_
+00351100: 6d69 785f 7061 6c65 7474 653a 2027 626c  mix_palette: 'bl
+00351110: 5f75 692e 7370 6163 655f 7669 6577 3364  _ui.space_view3d
+00351120: 5f74 6f6f 6c62 6172 2e56 4945 5733 445f  _toolbar.VIEW3D_
+00351130: 5054 5f74 6f6f 6c73 5f67 7265 6173 655f  PT_tools_grease_
+00351140: 7065 6e63 696c 5f62 7275 7368 5f6d 6978  pencil_brush_mix
+00351150: 5f70 616c 6574 7465 2720 3d20 4e6f 6e65  _palette' = None
+00351160: 0a0a 5649 4557 3344 5f50 545f 746f 6f6c  ..VIEW3D_PT_tool
+00351170: 735f 6772 6561 7365 5f70 656e 6369 6c5f  s_grease_pencil_
+00351180: 6272 7573 685f 6d69 7863 6f6c 6f72 3a20  brush_mixcolor: 
+00351190: 2762 6c5f 7569 2e73 7061 6365 5f76 6965  'bl_ui.space_vie
+003511a0: 7733 645f 746f 6f6c 6261 722e 5649 4557  w3d_toolbar.VIEW
+003511b0: 3344 5f50 545f 746f 6f6c 735f 6772 6561  3D_PT_tools_grea
+003511c0: 7365 5f70 656e 6369 6c5f 6272 7573 685f  se_pencil_brush_
+003511d0: 6d69 7863 6f6c 6f72 2720 3d20 4e6f 6e65  mixcolor' = None
+003511e0: 0a0a 5649 4557 3344 5f50 545f 746f 6f6c  ..VIEW3D_PT_tool
+003511f0: 735f 6772 6561 7365 5f70 656e 6369 6c5f  s_grease_pencil_
+00351200: 6272 7573 685f 7061 696e 745f 6661 6c6c  brush_paint_fall
+00351210: 6f66 663a 2027 626c 5f75 692e 7370 6163  off: 'bl_ui.spac
+00351220: 655f 7669 6577 3364 5f74 6f6f 6c62 6172  e_view3d_toolbar
+00351230: 2e56 4945 5733 445f 5054 5f74 6f6f 6c73  .VIEW3D_PT_tools
+00351240: 5f67 7265 6173 655f 7065 6e63 696c 5f62  _grease_pencil_b
+00351250: 7275 7368 5f70 6169 6e74 5f66 616c 6c6f  rush_paint_fallo
+00351260: 6666 2720 3d20 4e6f 6e65 0a0a 5649 4557  ff' = None..VIEW
+00351270: 3344 5f50 545f 746f 6f6c 735f 6772 6561  3D_PT_tools_grea
+00351280: 7365 5f70 656e 6369 6c5f 6272 7573 685f  se_pencil_brush_
+00351290: 706f 7374 5f70 726f 6365 7373 696e 673a  post_processing:
+003512a0: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
+003512b0: 6577 3364 5f74 6f6f 6c62 6172 2e56 4945  ew3d_toolbar.VIE
+003512c0: 5733 445f 5054 5f74 6f6f 6c73 5f67 7265  W3D_PT_tools_gre
+003512d0: 6173 655f 7065 6e63 696c 5f62 7275 7368  ase_pencil_brush
+003512e0: 5f70 6f73 745f 7072 6f63 6573 7369 6e67  _post_processing
+003512f0: 2720 3d20 4e6f 6e65 0a0a 5649 4557 3344  ' = None..VIEW3D
+00351300: 5f50 545f 746f 6f6c 735f 6772 6561 7365  _PT_tools_grease
+00351310: 5f70 656e 6369 6c5f 6272 7573 685f 7261  _pencil_brush_ra
+00351320: 6e64 6f6d 3a20 2762 6c5f 7569 2e73 7061  ndom: 'bl_ui.spa
+00351330: 6365 5f76 6965 7733 645f 746f 6f6c 6261  ce_view3d_toolba
+00351340: 722e 5649 4557 3344 5f50 545f 746f 6f6c  r.VIEW3D_PT_tool
+00351350: 735f 6772 6561 7365 5f70 656e 6369 6c5f  s_grease_pencil_
+00351360: 6272 7573 685f 7261 6e64 6f6d 2720 3d20  brush_random' = 
+00351370: 4e6f 6e65 0a0a 5649 4557 3344 5f50 545f  None..VIEW3D_PT_
+00351380: 746f 6f6c 735f 6772 6561 7365 5f70 656e  tools_grease_pen
+00351390: 6369 6c5f 6272 7573 685f 7363 756c 7074  cil_brush_sculpt
+003513a0: 5f66 616c 6c6f 6666 3a20 2762 6c5f 7569  _falloff: 'bl_ui
+003513b0: 2e73 7061 6365 5f76 6965 7733 645f 746f  .space_view3d_to
+003513c0: 6f6c 6261 722e 5649 4557 3344 5f50 545f  olbar.VIEW3D_PT_
+003513d0: 746f 6f6c 735f 6772 6561 7365 5f70 656e  tools_grease_pen
+003513e0: 6369 6c5f 6272 7573 685f 7363 756c 7074  cil_brush_sculpt
+003513f0: 5f66 616c 6c6f 6666 2720 3d20 4e6f 6e65  _falloff' = None
+00351400: 0a0a 5649 4557 3344 5f50 545f 746f 6f6c  ..VIEW3D_PT_tool
+00351410: 735f 6772 6561 7365 5f70 656e 6369 6c5f  s_grease_pencil_
+00351420: 6272 7573 685f 7365 6c65 6374 3a20 2762  brush_select: 'b
+00351430: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
+00351440: 645f 746f 6f6c 6261 722e 5649 4557 3344  d_toolbar.VIEW3D
+00351450: 5f50 545f 746f 6f6c 735f 6772 6561 7365  _PT_tools_grease
+00351460: 5f70 656e 6369 6c5f 6272 7573 685f 7365  _pencil_brush_se
+00351470: 6c65 6374 2720 3d20 4e6f 6e65 0a0a 5649  lect' = None..VI
+00351480: 4557 3344 5f50 545f 746f 6f6c 735f 6772  EW3D_PT_tools_gr
+00351490: 6561 7365 5f70 656e 6369 6c5f 6272 7573  ease_pencil_brus
+003514a0: 685f 7365 7474 696e 6773 3a20 2762 6c5f  h_settings: 'bl_
+003514b0: 7569 2e73 7061 6365 5f76 6965 7733 645f  ui.space_view3d_
+003514c0: 746f 6f6c 6261 722e 5649 4557 3344 5f50  toolbar.VIEW3D_P
+003514d0: 545f 746f 6f6c 735f 6772 6561 7365 5f70  T_tools_grease_p
+003514e0: 656e 6369 6c5f 6272 7573 685f 7365 7474  encil_brush_sett
+003514f0: 696e 6773 2720 3d20 4e6f 6e65 0a0a 5649  ings' = None..VI
+00351500: 4557 3344 5f50 545f 746f 6f6c 735f 6772  EW3D_PT_tools_gr
+00351510: 6561 7365 5f70 656e 6369 6c5f 6272 7573  ease_pencil_brus
+00351520: 685f 7374 6162 696c 697a 6572 3a20 2762  h_stabilizer: 'b
+00351530: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
+00351540: 645f 746f 6f6c 6261 722e 5649 4557 3344  d_toolbar.VIEW3D
+00351550: 5f50 545f 746f 6f6c 735f 6772 6561 7365  _PT_tools_grease
+00351560: 5f70 656e 6369 6c5f 6272 7573 685f 7374  _pencil_brush_st
+00351570: 6162 696c 697a 6572 2720 3d20 4e6f 6e65  abilizer' = None
+00351580: 0a0a 5649 4557 3344 5f50 545f 746f 6f6c  ..VIEW3D_PT_tool
+00351590: 735f 6772 6561 7365 5f70 656e 6369 6c5f  s_grease_pencil_
+003515a0: 6272 7573 685f 7374 726f 6b65 3a20 2762  brush_stroke: 'b
+003515b0: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
+003515c0: 645f 746f 6f6c 6261 722e 5649 4557 3344  d_toolbar.VIEW3D
+003515d0: 5f50 545f 746f 6f6c 735f 6772 6561 7365  _PT_tools_grease
+003515e0: 5f70 656e 6369 6c5f 6272 7573 685f 7374  _pencil_brush_st
+003515f0: 726f 6b65 2720 3d20 4e6f 6e65 0a0a 5649  roke' = None..VI
+00351600: 4557 3344 5f50 545f 746f 6f6c 735f 6772  EW3D_PT_tools_gr
+00351610: 6561 7365 5f70 656e 6369 6c5f 6272 7573  ease_pencil_brus
+00351620: 685f 7665 7274 6578 5f63 6f6c 6f72 3a20  h_vertex_color: 
+00351630: 2762 6c5f 7569 2e73 7061 6365 5f76 6965  'bl_ui.space_vie
+00351640: 7733 645f 746f 6f6c 6261 722e 5649 4557  w3d_toolbar.VIEW
+00351650: 3344 5f50 545f 746f 6f6c 735f 6772 6561  3D_PT_tools_grea
+00351660: 7365 5f70 656e 6369 6c5f 6272 7573 685f  se_pencil_brush_
+00351670: 7665 7274 6578 5f63 6f6c 6f72 2720 3d20  vertex_color' = 
+00351680: 4e6f 6e65 0a0a 5649 4557 3344 5f50 545f  None..VIEW3D_PT_
+00351690: 746f 6f6c 735f 6772 6561 7365 5f70 656e  tools_grease_pen
+003516a0: 6369 6c5f 6272 7573 685f 7665 7274 6578  cil_brush_vertex
+003516b0: 5f66 616c 6c6f 6666 3a20 2762 6c5f 7569  _falloff: 'bl_ui
+003516c0: 2e73 7061 6365 5f76 6965 7733 645f 746f  .space_view3d_to
+003516d0: 6f6c 6261 722e 5649 4557 3344 5f50 545f  olbar.VIEW3D_PT_
+003516e0: 746f 6f6c 735f 6772 6561 7365 5f70 656e  tools_grease_pen
+003516f0: 6369 6c5f 6272 7573 685f 7665 7274 6578  cil_brush_vertex
+00351700: 5f66 616c 6c6f 6666 2720 3d20 4e6f 6e65  _falloff' = None
+00351710: 0a0a 5649 4557 3344 5f50 545f 746f 6f6c  ..VIEW3D_PT_tool
+00351720: 735f 6772 6561 7365 5f70 656e 6369 6c5f  s_grease_pencil_
+00351730: 6272 7573 685f 7665 7274 6578 5f70 616c  brush_vertex_pal
+00351740: 6574 7465 3a20 2762 6c5f 7569 2e73 7061  ette: 'bl_ui.spa
+00351750: 6365 5f76 6965 7733 645f 746f 6f6c 6261  ce_view3d_toolba
+00351760: 722e 5649 4557 3344 5f50 545f 746f 6f6c  r.VIEW3D_PT_tool
+00351770: 735f 6772 6561 7365 5f70 656e 6369 6c5f  s_grease_pencil_
+00351780: 6272 7573 685f 7665 7274 6578 5f70 616c  brush_vertex_pal
+00351790: 6574 7465 2720 3d20 4e6f 6e65 0a0a 5649  ette' = None..VI
+003517a0: 4557 3344 5f50 545f 746f 6f6c 735f 6772  EW3D_PT_tools_gr
+003517b0: 6561 7365 5f70 656e 6369 6c5f 6272 7573  ease_pencil_brus
+003517c0: 685f 7765 6967 6874 5f66 616c 6c6f 6666  h_weight_falloff
+003517d0: 3a20 2762 6c5f 7569 2e73 7061 6365 5f76  : 'bl_ui.space_v
+003517e0: 6965 7733 645f 746f 6f6c 6261 722e 5649  iew3d_toolbar.VI
+003517f0: 4557 3344 5f50 545f 746f 6f6c 735f 6772  EW3D_PT_tools_gr
+00351800: 6561 7365 5f70 656e 6369 6c5f 6272 7573  ease_pencil_brus
+00351810: 685f 7765 6967 6874 5f66 616c 6c6f 6666  h_weight_falloff
+00351820: 2720 3d20 4e6f 6e65 0a0a 5649 4557 3344  ' = None..VIEW3D
+00351830: 5f50 545f 746f 6f6c 735f 6772 6561 7365  _PT_tools_grease
+00351840: 5f70 656e 6369 6c5f 7061 696e 745f 6170  _pencil_paint_ap
+00351850: 7065 6172 616e 6365 3a20 2762 6c5f 7569  pearance: 'bl_ui
+00351860: 2e73 7061 6365 5f76 6965 7733 645f 746f  .space_view3d_to
+00351870: 6f6c 6261 722e 5649 4557 3344 5f50 545f  olbar.VIEW3D_PT_
+00351880: 746f 6f6c 735f 6772 6561 7365 5f70 656e  tools_grease_pen
+00351890: 6369 6c5f 7061 696e 745f 6170 7065 6172  cil_paint_appear
+003518a0: 616e 6365 2720 3d20 4e6f 6e65 0a0a 5649  ance' = None..VI
+003518b0: 4557 3344 5f50 545f 746f 6f6c 735f 6772  EW3D_PT_tools_gr
+003518c0: 6561 7365 5f70 656e 6369 6c5f 7363 756c  ease_pencil_scul
+003518d0: 7074 5f61 7070 6561 7261 6e63 653a 2027  pt_appearance: '
+003518e0: 626c 5f75 692e 7370 6163 655f 7669 6577  bl_ui.space_view
+003518f0: 3364 5f74 6f6f 6c62 6172 2e56 4945 5733  3d_toolbar.VIEW3
+00351900: 445f 5054 5f74 6f6f 6c73 5f67 7265 6173  D_PT_tools_greas
+00351910: 655f 7065 6e63 696c 5f73 6375 6c70 745f  e_pencil_sculpt_
+00351920: 6170 7065 6172 616e 6365 2720 3d20 4e6f  appearance' = No
+00351930: 6e65 0a0a 5649 4557 3344 5f50 545f 746f  ne..VIEW3D_PT_to
+00351940: 6f6c 735f 6772 6561 7365 5f70 656e 6369  ols_grease_penci
+00351950: 6c5f 7363 756c 7074 5f62 7275 7368 5f61  l_sculpt_brush_a
+00351960: 6476 616e 6365 643a 2027 626c 5f75 692e  dvanced: 'bl_ui.
+00351970: 7370 6163 655f 7669 6577 3364 5f74 6f6f  space_view3d_too
+00351980: 6c62 6172 2e56 4945 5733 445f 5054 5f74  lbar.VIEW3D_PT_t
+00351990: 6f6f 6c73 5f67 7265 6173 655f 7065 6e63  ools_grease_penc
+003519a0: 696c 5f73 6375 6c70 745f 6272 7573 685f  il_sculpt_brush_
+003519b0: 6164 7661 6e63 6564 2720 3d20 4e6f 6e65  advanced' = None
+003519c0: 0a0a 5649 4557 3344 5f50 545f 746f 6f6c  ..VIEW3D_PT_tool
+003519d0: 735f 6772 6561 7365 5f70 656e 6369 6c5f  s_grease_pencil_
+003519e0: 7363 756c 7074 5f62 7275 7368 5f70 6f70  sculpt_brush_pop
+003519f0: 6f76 6572 3a20 2762 6c5f 7569 2e73 7061  over: 'bl_ui.spa
+00351a00: 6365 5f76 6965 7733 645f 746f 6f6c 6261  ce_view3d_toolba
+00351a10: 722e 5649 4557 3344 5f50 545f 746f 6f6c  r.VIEW3D_PT_tool
+00351a20: 735f 6772 6561 7365 5f70 656e 6369 6c5f  s_grease_pencil_
+00351a30: 7363 756c 7074 5f62 7275 7368 5f70 6f70  sculpt_brush_pop
+00351a40: 6f76 6572 2720 3d20 4e6f 6e65 0a0a 5649  over' = None..VI
+00351a50: 4557 3344 5f50 545f 746f 6f6c 735f 6772  EW3D_PT_tools_gr
+00351a60: 6561 7365 5f70 656e 6369 6c5f 7363 756c  ease_pencil_scul
+00351a70: 7074 5f73 656c 6563 743a 2027 626c 5f75  pt_select: 'bl_u
+00351a80: 692e 7370 6163 655f 7669 6577 3364 5f74  i.space_view3d_t
+00351a90: 6f6f 6c62 6172 2e56 4945 5733 445f 5054  oolbar.VIEW3D_PT
+00351aa0: 5f74 6f6f 6c73 5f67 7265 6173 655f 7065  _tools_grease_pe
+00351ab0: 6e63 696c 5f73 6375 6c70 745f 7365 6c65  ncil_sculpt_sele
+00351ac0: 6374 2720 3d20 4e6f 6e65 0a0a 5649 4557  ct' = None..VIEW
+00351ad0: 3344 5f50 545f 746f 6f6c 735f 6772 6561  3D_PT_tools_grea
+00351ae0: 7365 5f70 656e 6369 6c5f 7363 756c 7074  se_pencil_sculpt
+00351af0: 5f73 6574 7469 6e67 733a 2027 626c 5f75  _settings: 'bl_u
+00351b00: 692e 7370 6163 655f 7669 6577 3364 5f74  i.space_view3d_t
+00351b10: 6f6f 6c62 6172 2e56 4945 5733 445f 5054  oolbar.VIEW3D_PT
+00351b20: 5f74 6f6f 6c73 5f67 7265 6173 655f 7065  _tools_grease_pe
+00351b30: 6e63 696c 5f73 6375 6c70 745f 7365 7474  ncil_sculpt_sett
+00351b40: 696e 6773 2720 3d20 4e6f 6e65 0a0a 5649  ings' = None..VI
+00351b50: 4557 3344 5f50 545f 746f 6f6c 735f 6772  EW3D_PT_tools_gr
+00351b60: 6561 7365 5f70 656e 6369 6c5f 7665 7274  ease_pencil_vert
+00351b70: 6578 5f61 7070 6561 7261 6e63 653a 2027  ex_appearance: '
+00351b80: 626c 5f75 692e 7370 6163 655f 7669 6577  bl_ui.space_view
+00351b90: 3364 5f74 6f6f 6c62 6172 2e56 4945 5733  3d_toolbar.VIEW3
+00351ba0: 445f 5054 5f74 6f6f 6c73 5f67 7265 6173  D_PT_tools_greas
+00351bb0: 655f 7065 6e63 696c 5f76 6572 7465 785f  e_pencil_vertex_
+00351bc0: 6170 7065 6172 616e 6365 2720 3d20 4e6f  appearance' = No
+00351bd0: 6e65 0a0a 5649 4557 3344 5f50 545f 746f  ne..VIEW3D_PT_to
+00351be0: 6f6c 735f 6772 6561 7365 5f70 656e 6369  ols_grease_penci
+00351bf0: 6c5f 7665 7274 6578 5f70 6169 6e74 5f73  l_vertex_paint_s
+00351c00: 656c 6563 743a 2027 626c 5f75 692e 7370  elect: 'bl_ui.sp
+00351c10: 6163 655f 7669 6577 3364 5f74 6f6f 6c62  ace_view3d_toolb
+00351c20: 6172 2e56 4945 5733 445f 5054 5f74 6f6f  ar.VIEW3D_PT_too
+00351c30: 6c73 5f67 7265 6173 655f 7065 6e63 696c  ls_grease_pencil
+00351c40: 5f76 6572 7465 785f 7061 696e 745f 7365  _vertex_paint_se
+00351c50: 6c65 6374 2720 3d20 4e6f 6e65 0a0a 5649  lect' = None..VI
+00351c60: 4557 3344 5f50 545f 746f 6f6c 735f 6772  EW3D_PT_tools_gr
+00351c70: 6561 7365 5f70 656e 6369 6c5f 7665 7274  ease_pencil_vert
+00351c80: 6578 5f70 6169 6e74 5f73 6574 7469 6e67  ex_paint_setting
+00351c90: 733a 2027 626c 5f75 692e 7370 6163 655f  s: 'bl_ui.space_
+00351ca0: 7669 6577 3364 5f74 6f6f 6c62 6172 2e56  view3d_toolbar.V
+00351cb0: 4945 5733 445f 5054 5f74 6f6f 6c73 5f67  IEW3D_PT_tools_g
+00351cc0: 7265 6173 655f 7065 6e63 696c 5f76 6572  rease_pencil_ver
+00351cd0: 7465 785f 7061 696e 745f 7365 7474 696e  tex_paint_settin
+00351ce0: 6773 2720 3d20 4e6f 6e65 0a0a 5649 4557  gs' = None..VIEW
+00351cf0: 3344 5f50 545f 746f 6f6c 735f 6772 6561  3D_PT_tools_grea
+00351d00: 7365 5f70 656e 6369 6c5f 7765 6967 6874  se_pencil_weight
+00351d10: 5f61 7070 6561 7261 6e63 653a 2027 626c  _appearance: 'bl
+00351d20: 5f75 692e 7370 6163 655f 7669 6577 3364  _ui.space_view3d
+00351d30: 5f74 6f6f 6c62 6172 2e56 4945 5733 445f  _toolbar.VIEW3D_
+00351d40: 5054 5f74 6f6f 6c73 5f67 7265 6173 655f  PT_tools_grease_
+00351d50: 7065 6e63 696c 5f77 6569 6768 745f 6170  pencil_weight_ap
+00351d60: 7065 6172 616e 6365 2720 3d20 4e6f 6e65  pearance' = None
+00351d70: 0a0a 5649 4557 3344 5f50 545f 746f 6f6c  ..VIEW3D_PT_tool
+00351d80: 735f 6772 6561 7365 5f70 656e 6369 6c5f  s_grease_pencil_
+00351d90: 7765 6967 6874 5f6f 7074 696f 6e73 3a20  weight_options: 
+00351da0: 2762 6c5f 7569 2e73 7061 6365 5f76 6965  'bl_ui.space_vie
+00351db0: 7733 645f 746f 6f6c 6261 722e 5649 4557  w3d_toolbar.VIEW
+00351dc0: 3344 5f50 545f 746f 6f6c 735f 6772 6561  3D_PT_tools_grea
+00351dd0: 7365 5f70 656e 6369 6c5f 7765 6967 6874  se_pencil_weight
+00351de0: 5f6f 7074 696f 6e73 2720 3d20 4e6f 6e65  _options' = None
+00351df0: 0a0a 5649 4557 3344 5f50 545f 746f 6f6c  ..VIEW3D_PT_tool
+00351e00: 735f 6772 6561 7365 5f70 656e 6369 6c5f  s_grease_pencil_
+00351e10: 7765 6967 6874 5f70 6169 6e74 5f73 656c  weight_paint_sel
+00351e20: 6563 743a 2027 626c 5f75 692e 7370 6163  ect: 'bl_ui.spac
+00351e30: 655f 7669 6577 3364 5f74 6f6f 6c62 6172  e_view3d_toolbar
+00351e40: 2e56 4945 5733 445f 5054 5f74 6f6f 6c73  .VIEW3D_PT_tools
+00351e50: 5f67 7265 6173 655f 7065 6e63 696c 5f77  _grease_pencil_w
+00351e60: 6569 6768 745f 7061 696e 745f 7365 6c65  eight_paint_sele
+00351e70: 6374 2720 3d20 4e6f 6e65 0a0a 5649 4557  ct' = None..VIEW
+00351e80: 3344 5f50 545f 746f 6f6c 735f 6772 6561  3D_PT_tools_grea
+00351e90: 7365 5f70 656e 6369 6c5f 7765 6967 6874  se_pencil_weight
+00351ea0: 5f70 6169 6e74 5f73 6574 7469 6e67 733a  _paint_settings:
+00351eb0: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
+00351ec0: 6577 3364 5f74 6f6f 6c62 6172 2e56 4945  ew3d_toolbar.VIE
+00351ed0: 5733 445f 5054 5f74 6f6f 6c73 5f67 7265  W3D_PT_tools_gre
+00351ee0: 6173 655f 7065 6e63 696c 5f77 6569 6768  ase_pencil_weigh
+00351ef0: 745f 7061 696e 745f 7365 7474 696e 6773  t_paint_settings
+00351f00: 2720 3d20 4e6f 6e65 0a0a 5649 4557 3344  ' = None..VIEW3D
+00351f10: 5f50 545f 746f 6f6c 735f 696d 6167 6570  _PT_tools_imagep
+00351f20: 6169 6e74 5f6f 7074 696f 6e73 3a20 2762  aint_options: 'b
+00351f30: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
+00351f40: 645f 746f 6f6c 6261 722e 5649 4557 3344  d_toolbar.VIEW3D
+00351f50: 5f50 545f 746f 6f6c 735f 696d 6167 6570  _PT_tools_imagep
+00351f60: 6169 6e74 5f6f 7074 696f 6e73 2720 3d20  aint_options' = 
+00351f70: 4e6f 6e65 0a0a 5649 4557 3344 5f50 545f  None..VIEW3D_PT_
+00351f80: 746f 6f6c 735f 696d 6167 6570 6169 6e74  tools_imagepaint
+00351f90: 5f6f 7074 696f 6e73 5f63 6176 6974 793a  _options_cavity:
+00351fa0: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
+00351fb0: 6577 3364 5f74 6f6f 6c62 6172 2e56 4945  ew3d_toolbar.VIE
+00351fc0: 5733 445f 5054 5f74 6f6f 6c73 5f69 6d61  W3D_PT_tools_ima
+00351fd0: 6765 7061 696e 745f 6f70 7469 6f6e 735f  gepaint_options_
+00351fe0: 6361 7669 7479 2720 3d20 4e6f 6e65 0a0a  cavity' = None..
+00351ff0: 5649 4557 3344 5f50 545f 746f 6f6c 735f  VIEW3D_PT_tools_
+00352000: 696d 6167 6570 6169 6e74 5f6f 7074 696f  imagepaint_optio
+00352010: 6e73 5f65 7874 6572 6e61 6c3a 2027 626c  ns_external: 'bl
+00352020: 5f75 692e 7370 6163 655f 7669 6577 3364  _ui.space_view3d
+00352030: 5f74 6f6f 6c62 6172 2e56 4945 5733 445f  _toolbar.VIEW3D_
+00352040: 5054 5f74 6f6f 6c73 5f69 6d61 6765 7061  PT_tools_imagepa
+00352050: 696e 745f 6f70 7469 6f6e 735f 6578 7465  int_options_exte
+00352060: 726e 616c 2720 3d20 4e6f 6e65 0a0a 5649  rnal' = None..VI
+00352070: 4557 3344 5f50 545f 746f 6f6c 735f 696d  EW3D_PT_tools_im
+00352080: 6167 6570 6169 6e74 5f73 796d 6d65 7472  agepaint_symmetr
+00352090: 793a 2027 626c 5f75 692e 7370 6163 655f  y: 'bl_ui.space_
+003520a0: 7669 6577 3364 5f74 6f6f 6c62 6172 2e56  view3d_toolbar.V
+003520b0: 4945 5733 445f 5054 5f74 6f6f 6c73 5f69  IEW3D_PT_tools_i
+003520c0: 6d61 6765 7061 696e 745f 7379 6d6d 6574  magepaint_symmet
+003520d0: 7279 2720 3d20 4e6f 6e65 0a0a 5649 4557  ry' = None..VIEW
+003520e0: 3344 5f50 545f 746f 6f6c 735f 6d61 736b  3D_PT_tools_mask
+003520f0: 5f74 6578 7475 7265 3a20 2762 6c5f 7569  _texture: 'bl_ui
+00352100: 2e73 7061 6365 5f76 6965 7733 645f 746f  .space_view3d_to
+00352110: 6f6c 6261 722e 5649 4557 3344 5f50 545f  olbar.VIEW3D_PT_
+00352120: 746f 6f6c 735f 6d61 736b 5f74 6578 7475  tools_mask_textu
+00352130: 7265 2720 3d20 4e6f 6e65 0a0a 5649 4557  re' = None..VIEW
+00352140: 3344 5f50 545f 746f 6f6c 735f 6d65 7368  3D_PT_tools_mesh
+00352150: 6564 6974 5f6f 7074 696f 6e73 3a20 2762  edit_options: 'b
+00352160: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
+00352170: 645f 746f 6f6c 6261 722e 5649 4557 3344  d_toolbar.VIEW3D
+00352180: 5f50 545f 746f 6f6c 735f 6d65 7368 6564  _PT_tools_meshed
+00352190: 6974 5f6f 7074 696f 6e73 2720 3d20 4e6f  it_options' = No
+003521a0: 6e65 0a0a 5649 4557 3344 5f50 545f 746f  ne..VIEW3D_PT_to
+003521b0: 6f6c 735f 6d65 7368 6564 6974 5f6f 7074  ols_meshedit_opt
+003521c0: 696f 6e73 5f74 7261 6e73 666f 726d 3a20  ions_transform: 
+003521d0: 2762 6c5f 7569 2e73 7061 6365 5f76 6965  'bl_ui.space_vie
+003521e0: 7733 645f 746f 6f6c 6261 722e 5649 4557  w3d_toolbar.VIEW
+003521f0: 3344 5f50 545f 746f 6f6c 735f 6d65 7368  3D_PT_tools_mesh
+00352200: 6564 6974 5f6f 7074 696f 6e73 5f74 7261  edit_options_tra
+00352210: 6e73 666f 726d 2720 3d20 4e6f 6e65 0a0a  nsform' = None..
+00352220: 5649 4557 3344 5f50 545f 746f 6f6c 735f  VIEW3D_PT_tools_
+00352230: 6d65 7368 6564 6974 5f6f 7074 696f 6e73  meshedit_options
+00352240: 5f75 7673 3a20 2762 6c5f 7569 2e73 7061  _uvs: 'bl_ui.spa
+00352250: 6365 5f76 6965 7733 645f 746f 6f6c 6261  ce_view3d_toolba
+00352260: 722e 5649 4557 3344 5f50 545f 746f 6f6c  r.VIEW3D_PT_tool
+00352270: 735f 6d65 7368 6564 6974 5f6f 7074 696f  s_meshedit_optio
+00352280: 6e73 5f75 7673 2720 3d20 4e6f 6e65 0a0a  ns_uvs' = None..
+00352290: 5649 4557 3344 5f50 545f 746f 6f6c 735f  VIEW3D_PT_tools_
+003522a0: 6f62 6a65 6374 5f6f 7074 696f 6e73 3a20  object_options: 
+003522b0: 2762 6c5f 7569 2e73 7061 6365 5f76 6965  'bl_ui.space_vie
+003522c0: 7733 645f 746f 6f6c 6261 722e 5649 4557  w3d_toolbar.VIEW
+003522d0: 3344 5f50 545f 746f 6f6c 735f 6f62 6a65  3D_PT_tools_obje
+003522e0: 6374 5f6f 7074 696f 6e73 2720 3d20 4e6f  ct_options' = No
+003522f0: 6e65 0a0a 5649 4557 3344 5f50 545f 746f  ne..VIEW3D_PT_to
+00352300: 6f6c 735f 6f62 6a65 6374 5f6f 7074 696f  ols_object_optio
+00352310: 6e73 5f74 7261 6e73 666f 726d 3a20 2762  ns_transform: 'b
+00352320: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
+00352330: 645f 746f 6f6c 6261 722e 5649 4557 3344  d_toolbar.VIEW3D
+00352340: 5f50 545f 746f 6f6c 735f 6f62 6a65 6374  _PT_tools_object
+00352350: 5f6f 7074 696f 6e73 5f74 7261 6e73 666f  _options_transfo
+00352360: 726d 2720 3d20 4e6f 6e65 0a0a 5649 4557  rm' = None..VIEW
+00352370: 3344 5f50 545f 746f 6f6c 735f 7061 7274  3D_PT_tools_part
+00352380: 6963 6c65 6d6f 6465 3a20 2762 6c5f 7569  iclemode: 'bl_ui
+00352390: 2e73 7061 6365 5f76 6965 7733 645f 746f  .space_view3d_to
+003523a0: 6f6c 6261 722e 5649 4557 3344 5f50 545f  olbar.VIEW3D_PT_
+003523b0: 746f 6f6c 735f 7061 7274 6963 6c65 6d6f  tools_particlemo
+003523c0: 6465 2720 3d20 4e6f 6e65 0a0a 5649 4557  de' = None..VIEW
+003523d0: 3344 5f50 545f 746f 6f6c 735f 7061 7274  3D_PT_tools_part
+003523e0: 6963 6c65 6d6f 6465 5f6f 7074 696f 6e73  iclemode_options
+003523f0: 3a20 2762 6c5f 7569 2e73 7061 6365 5f76  : 'bl_ui.space_v
+00352400: 6965 7733 645f 746f 6f6c 6261 722e 5649  iew3d_toolbar.VI
+00352410: 4557 3344 5f50 545f 746f 6f6c 735f 7061  EW3D_PT_tools_pa
+00352420: 7274 6963 6c65 6d6f 6465 5f6f 7074 696f  rticlemode_optio
+00352430: 6e73 2720 3d20 4e6f 6e65 0a0a 5649 4557  ns' = None..VIEW
+00352440: 3344 5f50 545f 746f 6f6c 735f 7061 7274  3D_PT_tools_part
+00352450: 6963 6c65 6d6f 6465 5f6f 7074 696f 6e73  iclemode_options
+00352460: 5f64 6973 706c 6179 3a20 2762 6c5f 7569  _display: 'bl_ui
+00352470: 2e73 7061 6365 5f76 6965 7733 645f 746f  .space_view3d_to
+00352480: 6f6c 6261 722e 5649 4557 3344 5f50 545f  olbar.VIEW3D_PT_
+00352490: 746f 6f6c 735f 7061 7274 6963 6c65 6d6f  tools_particlemo
+003524a0: 6465 5f6f 7074 696f 6e73 5f64 6973 706c  de_options_displ
+003524b0: 6179 2720 3d20 4e6f 6e65 0a0a 5649 4557  ay' = None..VIEW
+003524c0: 3344 5f50 545f 746f 6f6c 735f 7061 7274  3D_PT_tools_part
+003524d0: 6963 6c65 6d6f 6465 5f6f 7074 696f 6e73  iclemode_options
+003524e0: 5f73 6861 7065 6375 743a 2027 626c 5f75  _shapecut: 'bl_u
+003524f0: 692e 7370 6163 655f 7669 6577 3364 5f74  i.space_view3d_t
+00352500: 6f6f 6c62 6172 2e56 4945 5733 445f 5054  oolbar.VIEW3D_PT
+00352510: 5f74 6f6f 6c73 5f70 6172 7469 636c 656d  _tools_particlem
+00352520: 6f64 655f 6f70 7469 6f6e 735f 7368 6170  ode_options_shap
+00352530: 6563 7574 2720 3d20 4e6f 6e65 0a0a 5649  ecut' = None..VI
+00352540: 4557 3344 5f50 545f 746f 6f6c 735f 706f  EW3D_PT_tools_po
+00352550: 7365 6d6f 6465 5f6f 7074 696f 6e73 3a20  semode_options: 
+00352560: 2762 6c5f 7569 2e73 7061 6365 5f76 6965  'bl_ui.space_vie
+00352570: 7733 645f 746f 6f6c 6261 722e 5649 4557  w3d_toolbar.VIEW
+00352580: 3344 5f50 545f 746f 6f6c 735f 706f 7365  3D_PT_tools_pose
+00352590: 6d6f 6465 5f6f 7074 696f 6e73 2720 3d20  mode_options' = 
+003525a0: 4e6f 6e65 0a0a 5649 4557 3344 5f50 545f  None..VIEW3D_PT_
+003525b0: 746f 6f6c 735f 7665 7274 6578 7061 696e  tools_vertexpain
+003525c0: 745f 6f70 7469 6f6e 733a 2027 626c 5f75  t_options: 'bl_u
+003525d0: 692e 7370 6163 655f 7669 6577 3364 5f74  i.space_view3d_t
+003525e0: 6f6f 6c62 6172 2e56 4945 5733 445f 5054  oolbar.VIEW3D_PT
+003525f0: 5f74 6f6f 6c73 5f76 6572 7465 7870 6169  _tools_vertexpai
+00352600: 6e74 5f6f 7074 696f 6e73 2720 3d20 4e6f  nt_options' = No
+00352610: 6e65 0a0a 5649 4557 3344 5f50 545f 746f  ne..VIEW3D_PT_to
+00352620: 6f6c 735f 7665 7274 6578 7061 696e 745f  ols_vertexpaint_
+00352630: 7379 6d6d 6574 7279 3a20 2762 6c5f 7569  symmetry: 'bl_ui
+00352640: 2e73 7061 6365 5f76 6965 7733 645f 746f  .space_view3d_to
+00352650: 6f6c 6261 722e 5649 4557 3344 5f50 545f  olbar.VIEW3D_PT_
+00352660: 746f 6f6c 735f 7665 7274 6578 7061 696e  tools_vertexpain
+00352670: 745f 7379 6d6d 6574 7279 2720 3d20 4e6f  t_symmetry' = No
+00352680: 6e65 0a0a 5649 4557 3344 5f50 545f 746f  ne..VIEW3D_PT_to
+00352690: 6f6c 735f 7665 7274 6578 7061 696e 745f  ols_vertexpaint_
+003526a0: 7379 6d6d 6574 7279 5f66 6f72 5f74 6f70  symmetry_for_top
+003526b0: 6261 723a 2027 626c 5f75 692e 7370 6163  bar: 'bl_ui.spac
+003526c0: 655f 7669 6577 3364 5f74 6f6f 6c62 6172  e_view3d_toolbar
+003526d0: 2e56 4945 5733 445f 5054 5f74 6f6f 6c73  .VIEW3D_PT_tools
+003526e0: 5f76 6572 7465 7870 6169 6e74 5f73 796d  _vertexpaint_sym
+003526f0: 6d65 7472 795f 666f 725f 746f 7062 6172  metry_for_topbar
 00352700: 2720 3d20 4e6f 6e65 0a0a 5649 4557 3344  ' = None..VIEW3D
 00352710: 5f50 545f 746f 6f6c 735f 7765 6967 6874  _PT_tools_weight
-00352720: 7061 696e 745f 6f70 7469 6f6e 733a 2027  paint_options: '
-00352730: 626c 5f75 692e 7370 6163 655f 7669 6577  bl_ui.space_view
-00352740: 3364 5f74 6f6f 6c62 6172 2e56 4945 5733  3d_toolbar.VIEW3
-00352750: 445f 5054 5f74 6f6f 6c73 5f77 6569 6768  D_PT_tools_weigh
-00352760: 7470 6169 6e74 5f6f 7074 696f 6e73 2720  tpaint_options' 
-00352770: 3d20 4e6f 6e65 0a0a 5649 4557 3344 5f50  = None..VIEW3D_P
-00352780: 545f 746f 6f6c 735f 7765 6967 6874 7061  T_tools_weightpa
-00352790: 696e 745f 7379 6d6d 6574 7279 3a20 2762  int_symmetry: 'b
-003527a0: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
-003527b0: 645f 746f 6f6c 6261 722e 5649 4557 3344  d_toolbar.VIEW3D
-003527c0: 5f50 545f 746f 6f6c 735f 7765 6967 6874  _PT_tools_weight
-003527d0: 7061 696e 745f 7379 6d6d 6574 7279 2720  paint_symmetry' 
-003527e0: 3d20 4e6f 6e65 0a0a 5649 4557 3344 5f50  = None..VIEW3D_P
-003527f0: 545f 746f 6f6c 735f 7765 6967 6874 7061  T_tools_weightpa
-00352800: 696e 745f 7379 6d6d 6574 7279 5f66 6f72  int_symmetry_for
-00352810: 5f74 6f70 6261 723a 2027 626c 5f75 692e  _topbar: 'bl_ui.
-00352820: 7370 6163 655f 7669 6577 3364 5f74 6f6f  space_view3d_too
-00352830: 6c62 6172 2e56 4945 5733 445f 5054 5f74  lbar.VIEW3D_PT_t
-00352840: 6f6f 6c73 5f77 6569 6768 7470 6169 6e74  ools_weightpaint
-00352850: 5f73 796d 6d65 7472 795f 666f 725f 746f  _symmetry_for_to
-00352860: 7062 6172 2720 3d20 4e6f 6e65 0a0a 5649  pbar' = None..VI
-00352870: 4557 3344 5f50 545f 7472 616e 7366 6f72  EW3D_PT_transfor
-00352880: 6d5f 6f72 6965 6e74 6174 696f 6e73 3a20  m_orientations: 
-00352890: 2762 6c5f 7569 2e73 7061 6365 5f76 6965  'bl_ui.space_vie
-003528a0: 7733 642e 5649 4557 3344 5f50 545f 7472  w3d.VIEW3D_PT_tr
-003528b0: 616e 7366 6f72 6d5f 6f72 6965 6e74 6174  ansform_orientat
-003528c0: 696f 6e73 2720 3d20 4e6f 6e65 0a0a 5649  ions' = None..VI
-003528d0: 4557 3344 5f50 545f 7669 6577 3364 5f63  EW3D_PT_view3d_c
-003528e0: 7572 736f 723a 2027 626c 5f75 692e 7370  ursor: 'bl_ui.sp
-003528f0: 6163 655f 7669 6577 3364 2e56 4945 5733  ace_view3d.VIEW3
-00352900: 445f 5054 5f76 6965 7733 645f 6375 7273  D_PT_view3d_curs
-00352910: 6f72 2720 3d20 4e6f 6e65 0a0a 5649 4557  or' = None..VIEW
-00352920: 3344 5f50 545f 7669 6577 3364 5f6c 6f63  3D_PT_view3d_loc
-00352930: 6b3a 2027 626c 5f75 692e 7370 6163 655f  k: 'bl_ui.space_
-00352940: 7669 6577 3364 2e56 4945 5733 445f 5054  view3d.VIEW3D_PT
-00352950: 5f76 6965 7733 645f 6c6f 636b 2720 3d20  _view3d_lock' = 
-00352960: 4e6f 6e65 0a0a 5649 4557 3344 5f50 545f  None..VIEW3D_PT_
-00352970: 7669 6577 3364 5f70 726f 7065 7274 6965  view3d_propertie
-00352980: 733a 2027 626c 5f75 692e 7370 6163 655f  s: 'bl_ui.space_
-00352990: 7669 6577 3364 2e56 4945 5733 445f 5054  view3d.VIEW3D_PT
-003529a0: 5f76 6965 7733 645f 7072 6f70 6572 7469  _view3d_properti
-003529b0: 6573 2720 3d20 4e6f 6e65 0a0a 5649 4557  es' = None..VIEW
-003529c0: 3344 5f50 545f 7669 6577 3364 5f73 7465  3D_PT_view3d_ste
-003529d0: 7265 6f3a 2027 626c 5f75 692e 7370 6163  reo: 'bl_ui.spac
-003529e0: 655f 7669 6577 3364 2e56 4945 5733 445f  e_view3d.VIEW3D_
-003529f0: 5054 5f76 6965 7733 645f 7374 6572 656f  PT_view3d_stereo
-00352a00: 2720 3d20 4e6f 6e65 0a0a 5649 4557 3344  ' = None..VIEW3D
-00352a10: 5f50 545f 7669 6577 706f 7274 5f64 6562  _PT_viewport_deb
-00352a20: 7567 3a20 2762 6c5f 7569 2e73 7061 6365  ug: 'bl_ui.space
-00352a30: 5f76 6965 7733 642e 5649 4557 3344 5f50  _view3d.VIEW3D_P
-00352a40: 545f 7669 6577 706f 7274 5f64 6562 7567  T_viewport_debug
-00352a50: 2720 3d20 4e6f 6e65 0a0a 5649 4557 4c41  ' = None..VIEWLA
-00352a60: 5945 525f 4d54 5f6c 6967 6874 6772 6f75  YER_MT_lightgrou
-00352a70: 705f 7379 6e63 3a20 2762 6c5f 7569 2e70  p_sync: 'bl_ui.p
-00352a80: 726f 7065 7274 6965 735f 7669 6577 5f6c  roperties_view_l
-00352a90: 6179 6572 2e56 4945 574c 4159 4552 5f4d  ayer.VIEWLAYER_M
-00352aa0: 545f 6c69 6768 7467 726f 7570 5f73 796e  T_lightgroup_syn
-00352ab0: 6327 203d 204e 6f6e 650a 0a56 4945 574c  c' = None..VIEWL
-00352ac0: 4159 4552 5f50 545f 6565 7665 655f 6c61  AYER_PT_eevee_la
-00352ad0: 7965 725f 7061 7373 6573 5f64 6174 613a  yer_passes_data:
-00352ae0: 2027 626c 5f75 692e 7072 6f70 6572 7469   'bl_ui.properti
-00352af0: 6573 5f76 6965 775f 6c61 7965 722e 5649  es_view_layer.VI
-00352b00: 4557 4c41 5945 525f 5054 5f65 6576 6565  EWLAYER_PT_eevee
-00352b10: 5f6c 6179 6572 5f70 6173 7365 735f 6461  _layer_passes_da
-00352b20: 7461 2720 3d20 4e6f 6e65 0a0a 5649 4557  ta' = None..VIEW
-00352b30: 4c41 5945 525f 5054 5f65 6576 6565 5f6c  LAYER_PT_eevee_l
-00352b40: 6179 6572 5f70 6173 7365 735f 6566 6665  ayer_passes_effe
-00352b50: 6374 733a 2027 626c 5f75 692e 7072 6f70  cts: 'bl_ui.prop
-00352b60: 6572 7469 6573 5f76 6965 775f 6c61 7965  erties_view_laye
-00352b70: 722e 5649 4557 4c41 5945 525f 5054 5f65  r.VIEWLAYER_PT_e
-00352b80: 6576 6565 5f6c 6179 6572 5f70 6173 7365  evee_layer_passe
-00352b90: 735f 6566 6665 6374 7327 203d 204e 6f6e  s_effects' = Non
-00352ba0: 650a 0a56 4945 574c 4159 4552 5f50 545f  e..VIEWLAYER_PT_
-00352bb0: 6565 7665 655f 6c61 7965 725f 7061 7373  eevee_layer_pass
-00352bc0: 6573 5f6c 6967 6874 3a20 2762 6c5f 7569  es_light: 'bl_ui
-00352bd0: 2e70 726f 7065 7274 6965 735f 7669 6577  .properties_view
-00352be0: 5f6c 6179 6572 2e56 4945 574c 4159 4552  _layer.VIEWLAYER
-00352bf0: 5f50 545f 6565 7665 655f 6c61 7965 725f  _PT_eevee_layer_
-00352c00: 7061 7373 6573 5f6c 6967 6874 2720 3d20  passes_light' = 
-00352c10: 4e6f 6e65 0a0a 5649 4557 4c41 5945 525f  None..VIEWLAYER_
-00352c20: 5054 5f65 6576 6565 5f6e 6578 745f 6c61  PT_eevee_next_la
-00352c30: 7965 725f 7061 7373 6573 5f64 6174 613a  yer_passes_data:
-00352c40: 2027 626c 5f75 692e 7072 6f70 6572 7469   'bl_ui.properti
-00352c50: 6573 5f76 6965 775f 6c61 7965 722e 5649  es_view_layer.VI
-00352c60: 4557 4c41 5945 525f 5054 5f65 6576 6565  EWLAYER_PT_eevee
-00352c70: 5f6e 6578 745f 6c61 7965 725f 7061 7373  _next_layer_pass
-00352c80: 6573 5f64 6174 6127 203d 204e 6f6e 650a  es_data' = None.
-00352c90: 0a56 4945 574c 4159 4552 5f50 545f 6672  .VIEWLAYER_PT_fr
-00352ca0: 6565 7374 796c 653a 2027 626c 5f75 692e  eestyle: 'bl_ui.
-00352cb0: 7072 6f70 6572 7469 6573 5f66 7265 6573  properties_frees
-00352cc0: 7479 6c65 2e56 4945 574c 4159 4552 5f50  tyle.VIEWLAYER_P
-00352cd0: 545f 6672 6565 7374 796c 6527 203d 204e  T_freestyle' = N
-00352ce0: 6f6e 650a 0a56 4945 574c 4159 4552 5f50  one..VIEWLAYER_P
-00352cf0: 545f 6672 6565 7374 796c 655f 6564 6765  T_freestyle_edge
-00352d00: 5f64 6574 6563 7469 6f6e 3a20 2762 6c5f  _detection: 'bl_
-00352d10: 7569 2e70 726f 7065 7274 6965 735f 6672  ui.properties_fr
-00352d20: 6565 7374 796c 652e 5649 4557 4c41 5945  eestyle.VIEWLAYE
-00352d30: 525f 5054 5f66 7265 6573 7479 6c65 5f65  R_PT_freestyle_e
-00352d40: 6467 655f 6465 7465 6374 696f 6e27 203d  dge_detection' =
-00352d50: 204e 6f6e 650a 0a56 4945 574c 4159 4552   None..VIEWLAYER
-00352d60: 5f50 545f 6672 6565 7374 796c 655f 6c69  _PT_freestyle_li
-00352d70: 6e65 7365 743a 2027 626c 5f75 692e 7072  neset: 'bl_ui.pr
-00352d80: 6f70 6572 7469 6573 5f66 7265 6573 7479  operties_freesty
-00352d90: 6c65 2e56 4945 574c 4159 4552 5f50 545f  le.VIEWLAYER_PT_
-00352da0: 6672 6565 7374 796c 655f 6c69 6e65 7365  freestyle_linese
-00352db0: 7427 203d 204e 6f6e 650a 0a56 4945 574c  t' = None..VIEWL
-00352dc0: 4159 4552 5f50 545f 6672 6565 7374 796c  AYER_PT_freestyl
-00352dd0: 655f 6c69 6e65 7365 745f 636f 6c6c 6563  e_lineset_collec
-00352de0: 7469 6f6e 3a20 2762 6c5f 7569 2e70 726f  tion: 'bl_ui.pro
-00352df0: 7065 7274 6965 735f 6672 6565 7374 796c  perties_freestyl
-00352e00: 652e 5649 4557 4c41 5945 525f 5054 5f66  e.VIEWLAYER_PT_f
-00352e10: 7265 6573 7479 6c65 5f6c 696e 6573 6574  reestyle_lineset
-00352e20: 5f63 6f6c 6c65 6374 696f 6e27 203d 204e  _collection' = N
-00352e30: 6f6e 650a 0a56 4945 574c 4159 4552 5f50  one..VIEWLAYER_P
-00352e40: 545f 6672 6565 7374 796c 655f 6c69 6e65  T_freestyle_line
-00352e50: 7365 745f 6564 6765 7479 7065 3a20 2762  set_edgetype: 'b
-00352e60: 6c5f 7569 2e70 726f 7065 7274 6965 735f  l_ui.properties_
-00352e70: 6672 6565 7374 796c 652e 5649 4557 4c41  freestyle.VIEWLA
-00352e80: 5945 525f 5054 5f66 7265 6573 7479 6c65  YER_PT_freestyle
-00352e90: 5f6c 696e 6573 6574 5f65 6467 6574 7970  _lineset_edgetyp
-00352ea0: 6527 203d 204e 6f6e 650a 0a56 4945 574c  e' = None..VIEWL
-00352eb0: 4159 4552 5f50 545f 6672 6565 7374 796c  AYER_PT_freestyl
-00352ec0: 655f 6c69 6e65 7365 745f 6661 6365 6d61  e_lineset_facema
-00352ed0: 726b 733a 2027 626c 5f75 692e 7072 6f70  rks: 'bl_ui.prop
-00352ee0: 6572 7469 6573 5f66 7265 6573 7479 6c65  erties_freestyle
-00352ef0: 2e56 4945 574c 4159 4552 5f50 545f 6672  .VIEWLAYER_PT_fr
-00352f00: 6565 7374 796c 655f 6c69 6e65 7365 745f  eestyle_lineset_
-00352f10: 6661 6365 6d61 726b 7327 203d 204e 6f6e  facemarks' = Non
-00352f20: 650a 0a56 4945 574c 4159 4552 5f50 545f  e..VIEWLAYER_PT_
-00352f30: 6672 6565 7374 796c 655f 6c69 6e65 7365  freestyle_linese
-00352f40: 745f 7669 7369 6269 6c74 793a 2027 626c  t_visibilty: 'bl
-00352f50: 5f75 692e 7072 6f70 6572 7469 6573 5f66  _ui.properties_f
-00352f60: 7265 6573 7479 6c65 2e56 4945 574c 4159  reestyle.VIEWLAY
-00352f70: 4552 5f50 545f 6672 6565 7374 796c 655f  ER_PT_freestyle_
-00352f80: 6c69 6e65 7365 745f 7669 7369 6269 6c74  lineset_visibilt
-00352f90: 7927 203d 204e 6f6e 650a 0a56 4945 574c  y' = None..VIEWL
-00352fa0: 4159 4552 5f50 545f 6672 6565 7374 796c  AYER_PT_freestyl
-00352fb0: 655f 6c69 6e65 7374 796c 655f 616c 7068  e_linestyle_alph
-00352fc0: 613a 2027 626c 5f75 692e 7072 6f70 6572  a: 'bl_ui.proper
-00352fd0: 7469 6573 5f66 7265 6573 7479 6c65 2e56  ties_freestyle.V
-00352fe0: 4945 574c 4159 4552 5f50 545f 6672 6565  IEWLAYER_PT_free
-00352ff0: 7374 796c 655f 6c69 6e65 7374 796c 655f  style_linestyle_
-00353000: 616c 7068 6127 203d 204e 6f6e 650a 0a56  alpha' = None..V
-00353010: 4945 574c 4159 4552 5f50 545f 6672 6565  IEWLAYER_PT_free
-00353020: 7374 796c 655f 6c69 6e65 7374 796c 655f  style_linestyle_
-00353030: 636f 6c6f 723a 2027 626c 5f75 692e 7072  color: 'bl_ui.pr
-00353040: 6f70 6572 7469 6573 5f66 7265 6573 7479  operties_freesty
-00353050: 6c65 2e56 4945 574c 4159 4552 5f50 545f  le.VIEWLAYER_PT_
-00353060: 6672 6565 7374 796c 655f 6c69 6e65 7374  freestyle_linest
-00353070: 796c 655f 636f 6c6f 7227 203d 204e 6f6e  yle_color' = Non
-00353080: 650a 0a56 4945 574c 4159 4552 5f50 545f  e..VIEWLAYER_PT_
-00353090: 6672 6565 7374 796c 655f 6c69 6e65 7374  freestyle_linest
-003530a0: 796c 655f 6765 6f6d 6574 7279 3a20 2762  yle_geometry: 'b
-003530b0: 6c5f 7569 2e70 726f 7065 7274 6965 735f  l_ui.properties_
-003530c0: 6672 6565 7374 796c 652e 5649 4557 4c41  freestyle.VIEWLA
-003530d0: 5945 525f 5054 5f66 7265 6573 7479 6c65  YER_PT_freestyle
-003530e0: 5f6c 696e 6573 7479 6c65 5f67 656f 6d65  _linestyle_geome
-003530f0: 7472 7927 203d 204e 6f6e 650a 0a56 4945  try' = None..VIE
-00353100: 574c 4159 4552 5f50 545f 6672 6565 7374  WLAYER_PT_freest
-00353110: 796c 655f 6c69 6e65 7374 796c 655f 7374  yle_linestyle_st
-00353120: 726f 6b65 733a 2027 626c 5f75 692e 7072  rokes: 'bl_ui.pr
-00353130: 6f70 6572 7469 6573 5f66 7265 6573 7479  operties_freesty
-00353140: 6c65 2e56 4945 574c 4159 4552 5f50 545f  le.VIEWLAYER_PT_
-00353150: 6672 6565 7374 796c 655f 6c69 6e65 7374  freestyle_linest
-00353160: 796c 655f 7374 726f 6b65 7327 203d 204e  yle_strokes' = N
-00353170: 6f6e 650a 0a56 4945 574c 4159 4552 5f50  one..VIEWLAYER_P
-00353180: 545f 6672 6565 7374 796c 655f 6c69 6e65  T_freestyle_line
-00353190: 7374 796c 655f 7374 726f 6b65 735f 6368  style_strokes_ch
-003531a0: 6169 6e69 6e67 3a20 2762 6c5f 7569 2e70  aining: 'bl_ui.p
-003531b0: 726f 7065 7274 6965 735f 6672 6565 7374  roperties_freest
-003531c0: 796c 652e 5649 4557 4c41 5945 525f 5054  yle.VIEWLAYER_PT
-003531d0: 5f66 7265 6573 7479 6c65 5f6c 696e 6573  _freestyle_lines
-003531e0: 7479 6c65 5f73 7472 6f6b 6573 5f63 6861  tyle_strokes_cha
-003531f0: 696e 696e 6727 203d 204e 6f6e 650a 0a56  ining' = None..V
-00353200: 4945 574c 4159 4552 5f50 545f 6672 6565  IEWLAYER_PT_free
-00353210: 7374 796c 655f 6c69 6e65 7374 796c 655f  style_linestyle_
-00353220: 7374 726f 6b65 735f 6461 7368 6564 6c69  strokes_dashedli
-00353230: 6e65 3a20 2762 6c5f 7569 2e70 726f 7065  ne: 'bl_ui.prope
-00353240: 7274 6965 735f 6672 6565 7374 796c 652e  rties_freestyle.
-00353250: 5649 4557 4c41 5945 525f 5054 5f66 7265  VIEWLAYER_PT_fre
-00353260: 6573 7479 6c65 5f6c 696e 6573 7479 6c65  estyle_linestyle
-00353270: 5f73 7472 6f6b 6573 5f64 6173 6865 646c  _strokes_dashedl
-00353280: 696e 6527 203d 204e 6f6e 650a 0a56 4945  ine' = None..VIE
-00353290: 574c 4159 4552 5f50 545f 6672 6565 7374  WLAYER_PT_freest
-003532a0: 796c 655f 6c69 6e65 7374 796c 655f 7374  yle_linestyle_st
-003532b0: 726f 6b65 735f 7365 6c65 6374 696f 6e3a  rokes_selection:
-003532c0: 2027 626c 5f75 692e 7072 6f70 6572 7469   'bl_ui.properti
-003532d0: 6573 5f66 7265 6573 7479 6c65 2e56 4945  es_freestyle.VIE
-003532e0: 574c 4159 4552 5f50 545f 6672 6565 7374  WLAYER_PT_freest
-003532f0: 796c 655f 6c69 6e65 7374 796c 655f 7374  yle_linestyle_st
-00353300: 726f 6b65 735f 7365 6c65 6374 696f 6e27  rokes_selection'
-00353310: 203d 204e 6f6e 650a 0a56 4945 574c 4159   = None..VIEWLAY
-00353320: 4552 5f50 545f 6672 6565 7374 796c 655f  ER_PT_freestyle_
-00353330: 6c69 6e65 7374 796c 655f 7374 726f 6b65  linestyle_stroke
-00353340: 735f 736f 7274 696e 673a 2027 626c 5f75  s_sorting: 'bl_u
-00353350: 692e 7072 6f70 6572 7469 6573 5f66 7265  i.properties_fre
-00353360: 6573 7479 6c65 2e56 4945 574c 4159 4552  estyle.VIEWLAYER
-00353370: 5f50 545f 6672 6565 7374 796c 655f 6c69  _PT_freestyle_li
-00353380: 6e65 7374 796c 655f 7374 726f 6b65 735f  nestyle_strokes_
-00353390: 736f 7274 696e 6727 203d 204e 6f6e 650a  sorting' = None.
-003533a0: 0a56 4945 574c 4159 4552 5f50 545f 6672  .VIEWLAYER_PT_fr
-003533b0: 6565 7374 796c 655f 6c69 6e65 7374 796c  eestyle_linestyl
-003533c0: 655f 7374 726f 6b65 735f 7370 6c69 7474  e_strokes_splitt
-003533d0: 696e 673a 2027 626c 5f75 692e 7072 6f70  ing: 'bl_ui.prop
-003533e0: 6572 7469 6573 5f66 7265 6573 7479 6c65  erties_freestyle
-003533f0: 2e56 4945 574c 4159 4552 5f50 545f 6672  .VIEWLAYER_PT_fr
-00353400: 6565 7374 796c 655f 6c69 6e65 7374 796c  eestyle_linestyl
-00353410: 655f 7374 726f 6b65 735f 7370 6c69 7474  e_strokes_splitt
-00353420: 696e 6727 203d 204e 6f6e 650a 0a56 4945  ing' = None..VIE
-00353430: 574c 4159 4552 5f50 545f 6672 6565 7374  WLAYER_PT_freest
-00353440: 796c 655f 6c69 6e65 7374 796c 655f 7374  yle_linestyle_st
-00353450: 726f 6b65 735f 7370 6c69 7474 696e 675f  rokes_splitting_
-00353460: 7061 7474 6572 6e3a 2027 626c 5f75 692e  pattern: 'bl_ui.
-00353470: 7072 6f70 6572 7469 6573 5f66 7265 6573  properties_frees
-00353480: 7479 6c65 2e56 4945 574c 4159 4552 5f50  tyle.VIEWLAYER_P
-00353490: 545f 6672 6565 7374 796c 655f 6c69 6e65  T_freestyle_line
-003534a0: 7374 796c 655f 7374 726f 6b65 735f 7370  style_strokes_sp
-003534b0: 6c69 7474 696e 675f 7061 7474 6572 6e27  litting_pattern'
-003534c0: 203d 204e 6f6e 650a 0a56 4945 574c 4159   = None..VIEWLAY
-003534d0: 4552 5f50 545f 6672 6565 7374 796c 655f  ER_PT_freestyle_
-003534e0: 6c69 6e65 7374 796c 655f 7465 7874 7572  linestyle_textur
-003534f0: 653a 2027 626c 5f75 692e 7072 6f70 6572  e: 'bl_ui.proper
-00353500: 7469 6573 5f66 7265 6573 7479 6c65 2e56  ties_freestyle.V
-00353510: 4945 574c 4159 4552 5f50 545f 6672 6565  IEWLAYER_PT_free
-00353520: 7374 796c 655f 6c69 6e65 7374 796c 655f  style_linestyle_
-00353530: 7465 7874 7572 6527 203d 204e 6f6e 650a  texture' = None.
-00353540: 0a56 4945 574c 4159 4552 5f50 545f 6672  .VIEWLAYER_PT_fr
-00353550: 6565 7374 796c 655f 6c69 6e65 7374 796c  eestyle_linestyl
-00353560: 655f 7468 6963 6b6e 6573 733a 2027 626c  e_thickness: 'bl
-00353570: 5f75 692e 7072 6f70 6572 7469 6573 5f66  _ui.properties_f
-00353580: 7265 6573 7479 6c65 2e56 4945 574c 4159  reestyle.VIEWLAY
-00353590: 4552 5f50 545f 6672 6565 7374 796c 655f  ER_PT_freestyle_
-003535a0: 6c69 6e65 7374 796c 655f 7468 6963 6b6e  linestyle_thickn
-003535b0: 6573 7327 203d 204e 6f6e 650a 0a56 4945  ess' = None..VIE
-003535c0: 574c 4159 4552 5f50 545f 6672 6565 7374  WLAYER_PT_freest
-003535d0: 796c 655f 7374 796c 655f 6d6f 6475 6c65  yle_style_module
-003535e0: 733a 2027 626c 5f75 692e 7072 6f70 6572  s: 'bl_ui.proper
-003535f0: 7469 6573 5f66 7265 6573 7479 6c65 2e56  ties_freestyle.V
-00353600: 4945 574c 4159 4552 5f50 545f 6672 6565  IEWLAYER_PT_free
-00353610: 7374 796c 655f 7374 796c 655f 6d6f 6475  style_style_modu
-00353620: 6c65 7327 203d 204e 6f6e 650a 0a56 4945  les' = None..VIE
-00353630: 574c 4159 4552 5f50 545f 6c61 7965 723a  WLAYER_PT_layer:
-00353640: 2027 626c 5f75 692e 7072 6f70 6572 7469   'bl_ui.properti
-00353650: 6573 5f76 6965 775f 6c61 7965 722e 5649  es_view_layer.VI
-00353660: 4557 4c41 5945 525f 5054 5f6c 6179 6572  EWLAYER_PT_layer
-00353670: 2720 3d20 4e6f 6e65 0a0a 5649 4557 4c41  ' = None..VIEWLA
-00353680: 5945 525f 5054 5f6c 6179 6572 5f63 7573  YER_PT_layer_cus
-00353690: 746f 6d5f 7072 6f70 733a 2027 626c 5f75  tom_props: 'bl_u
-003536a0: 692e 7072 6f70 6572 7469 6573 5f76 6965  i.properties_vie
-003536b0: 775f 6c61 7965 722e 5649 4557 4c41 5945  w_layer.VIEWLAYE
-003536c0: 525f 5054 5f6c 6179 6572 5f63 7573 746f  R_PT_layer_custo
-003536d0: 6d5f 7072 6f70 7327 203d 204e 6f6e 650a  m_props' = None.
-003536e0: 0a56 4945 574c 4159 4552 5f50 545f 6c61  .VIEWLAYER_PT_la
-003536f0: 7965 725f 7061 7373 6573 3a20 2762 6c5f  yer_passes: 'bl_
-00353700: 7569 2e70 726f 7065 7274 6965 735f 7669  ui.properties_vi
-00353710: 6577 5f6c 6179 6572 2e56 4945 574c 4159  ew_layer.VIEWLAY
-00353720: 4552 5f50 545f 6c61 7965 725f 7061 7373  ER_PT_layer_pass
-00353730: 6573 2720 3d20 4e6f 6e65 0a0a 5649 4557  es' = None..VIEW
-00353740: 4c41 5945 525f 5054 5f6c 6179 6572 5f70  LAYER_PT_layer_p
-00353750: 6173 7365 735f 616f 763a 2027 626c 5f75  asses_aov: 'bl_u
-00353760: 692e 7072 6f70 6572 7469 6573 5f76 6965  i.properties_vie
-00353770: 775f 6c61 7965 722e 5649 4557 4c41 5945  w_layer.VIEWLAYE
-00353780: 525f 5054 5f6c 6179 6572 5f70 6173 7365  R_PT_layer_passe
-00353790: 735f 616f 7627 203d 204e 6f6e 650a 0a56  s_aov' = None..V
-003537a0: 4945 574c 4159 4552 5f50 545f 6c61 7965  IEWLAYER_PT_laye
-003537b0: 725f 7061 7373 6573 5f63 7279 7074 6f6d  r_passes_cryptom
-003537c0: 6174 7465 3a20 2762 6c5f 7569 2e70 726f  atte: 'bl_ui.pro
-003537d0: 7065 7274 6965 735f 7669 6577 5f6c 6179  perties_view_lay
-003537e0: 6572 2e56 4945 574c 4159 4552 5f50 545f  er.VIEWLAYER_PT_
-003537f0: 6c61 7965 725f 7061 7373 6573 5f63 7279  layer_passes_cry
-00353800: 7074 6f6d 6174 7465 2720 3d20 4e6f 6e65  ptomatte' = None
-00353810: 0a0a 5649 4557 4c41 5945 525f 5054 5f6c  ..VIEWLAYER_PT_l
-00353820: 6179 6572 5f70 6173 7365 735f 6c69 6768  ayer_passes_ligh
-00353830: 7467 726f 7570 733a 2027 626c 5f75 692e  tgroups: 'bl_ui.
-00353840: 7072 6f70 6572 7469 6573 5f76 6965 775f  properties_view_
-00353850: 6c61 7965 722e 5649 4557 4c41 5945 525f  layer.VIEWLAYER_
-00353860: 5054 5f6c 6179 6572 5f70 6173 7365 735f  PT_layer_passes_
-00353870: 6c69 6768 7467 726f 7570 7327 203d 204e  lightgroups' = N
-00353880: 6f6e 650a 0a56 4945 574c 4159 4552 5f55  one..VIEWLAYER_U
-00353890: 4c5f 616f 763a 2027 626c 5f75 692e 7072  L_aov: 'bl_ui.pr
-003538a0: 6f70 6572 7469 6573 5f76 6965 775f 6c61  operties_view_la
-003538b0: 7965 722e 5649 4557 4c41 5945 525f 554c  yer.VIEWLAYER_UL
-003538c0: 5f61 6f76 2720 3d20 4e6f 6e65 0a0a 5649  _aov' = None..VI
-003538d0: 4557 4c41 5945 525f 554c 5f6c 696e 6573  EWLAYER_UL_lines
-003538e0: 6574 733a 2027 626c 5f75 692e 7072 6f70  ets: 'bl_ui.prop
-003538f0: 6572 7469 6573 5f66 7265 6573 7479 6c65  erties_freestyle
-00353900: 2e56 4945 574c 4159 4552 5f55 4c5f 6c69  .VIEWLAYER_UL_li
-00353910: 6e65 7365 7473 2720 3d20 4e6f 6e65 0a0a  nesets' = None..
-00353920: 564f 4c55 4d45 5f55 4c5f 6772 6964 733a  VOLUME_UL_grids:
-00353930: 2027 626c 5f75 692e 7072 6f70 6572 7469   'bl_ui.properti
-00353940: 6573 5f64 6174 615f 766f 6c75 6d65 2e56  es_data_volume.V
-00353950: 4f4c 554d 455f 554c 5f67 7269 6473 2720  OLUME_UL_grids' 
-00353960: 3d20 4e6f 6e65 0a0a 574d 5f4d 545f 6f70  = None..WM_MT_op
-00353970: 6572 6174 6f72 5f70 7265 7365 7473 3a20  erator_presets: 
-00353980: 2762 6c5f 6f70 6572 6174 6f72 732e 7072  'bl_operators.pr
-00353990: 6573 6574 732e 574d 5f4d 545f 6f70 6572  esets.WM_MT_oper
-003539a0: 6174 6f72 5f70 7265 7365 7473 2720 3d20  ator_presets' = 
-003539b0: 4e6f 6e65 0a0a 574d 5f4d 545f 7370 6c61  None..WM_MT_spla
-003539c0: 7368 3a20 2762 6c5f 6f70 6572 6174 6f72  sh: 'bl_operator
-003539d0: 732e 776d 2e57 4d5f 4d54 5f73 706c 6173  s.wm.WM_MT_splas
-003539e0: 6827 203d 204e 6f6e 650a 0a57 4d5f 4d54  h' = None..WM_MT
-003539f0: 5f73 706c 6173 685f 6162 6f75 743a 2027  _splash_about: '
-00353a00: 626c 5f6f 7065 7261 746f 7273 2e77 6d2e  bl_operators.wm.
-00353a10: 574d 5f4d 545f 7370 6c61 7368 5f61 626f  WM_MT_splash_abo
-00353a20: 7574 2720 3d20 4e6f 6e65 0a0a 574d 5f4d  ut' = None..WM_M
-00353a30: 545f 7370 6c61 7368 5f71 7569 636b 5f73  T_splash_quick_s
-00353a40: 6574 7570 3a20 2762 6c5f 6f70 6572 6174  etup: 'bl_operat
-00353a50: 6f72 732e 776d 2e57 4d5f 4d54 5f73 706c  ors.wm.WM_MT_spl
-00353a60: 6173 685f 7175 6963 6b5f 7365 7475 7027  ash_quick_setup'
-00353a70: 203d 204e 6f6e 650a 0a57 4d5f 4d54 5f74   = None..WM_MT_t
-00353a80: 6f6f 6c73 7973 7465 6d5f 7375 626d 656e  oolsystem_submen
-00353a90: 753a 2027 626c 5f75 692e 7370 6163 655f  u: 'bl_ui.space_
-00353aa0: 746f 6f6c 7379 7374 656d 5f63 6f6d 6d6f  toolsystem_commo
-00353ab0: 6e2e 574d 5f4d 545f 746f 6f6c 7379 7374  n.WM_MT_toolsyst
-00353ac0: 656d 5f73 7562 6d65 6e75 2720 3d20 4e6f  em_submenu' = No
-00353ad0: 6e65 0a0a 574d 5f4f 545f 6261 7463 685f  ne..WM_OT_batch_
-00353ae0: 7265 6e61 6d65 3a20 2762 6c5f 6f70 6572  rename: 'bl_oper
-00353af0: 6174 6f72 732e 776d 2e57 4d5f 4f54 5f62  ators.wm.WM_OT_b
-00353b00: 6174 6368 5f72 656e 616d 6527 203d 204e  atch_rename' = N
-00353b10: 6f6e 650a 0a57 4d5f 4f54 5f62 6c65 6e64  one..WM_OT_blend
-00353b20: 5f73 7472 696e 6773 5f75 7466 385f 7661  _strings_utf8_va
-00353b30: 6c69 6461 7465 3a20 2762 6c5f 6f70 6572  lidate: 'bl_oper
-00353b40: 6174 6f72 732e 6669 6c65 2e57 4d5f 4f54  ators.file.WM_OT
-00353b50: 5f62 6c65 6e64 5f73 7472 696e 6773 5f75  _blend_strings_u
-00353b60: 7466 385f 7661 6c69 6461 7465 2720 3d20  tf8_validate' = 
-00353b70: 4e6f 6e65 0a0a 574d 5f4f 545f 636f 6e74  None..WM_OT_cont
-00353b80: 6578 745f 636f 6c6c 6563 7469 6f6e 5f62  ext_collection_b
-00353b90: 6f6f 6c65 616e 5f73 6574 3a20 2762 6c5f  oolean_set: 'bl_
-00353ba0: 6f70 6572 6174 6f72 732e 776d 2e57 4d5f  operators.wm.WM_
-00353bb0: 4f54 5f63 6f6e 7465 7874 5f63 6f6c 6c65  OT_context_colle
-00353bc0: 6374 696f 6e5f 626f 6f6c 6561 6e5f 7365  ction_boolean_se
-00353bd0: 7427 203d 204e 6f6e 650a 0a57 4d5f 4f54  t' = None..WM_OT
-00353be0: 5f63 6f6e 7465 7874 5f63 7963 6c65 5f61  _context_cycle_a
-00353bf0: 7272 6179 3a20 2762 6c5f 6f70 6572 6174  rray: 'bl_operat
-00353c00: 6f72 732e 776d 2e57 4d5f 4f54 5f63 6f6e  ors.wm.WM_OT_con
-00353c10: 7465 7874 5f63 7963 6c65 5f61 7272 6179  text_cycle_array
-00353c20: 2720 3d20 4e6f 6e65 0a0a 574d 5f4f 545f  ' = None..WM_OT_
-00353c30: 636f 6e74 6578 745f 6379 636c 655f 656e  context_cycle_en
-00353c40: 756d 3a20 2762 6c5f 6f70 6572 6174 6f72  um: 'bl_operator
-00353c50: 732e 776d 2e57 4d5f 4f54 5f63 6f6e 7465  s.wm.WM_OT_conte
-00353c60: 7874 5f63 7963 6c65 5f65 6e75 6d27 203d  xt_cycle_enum' =
-00353c70: 204e 6f6e 650a 0a57 4d5f 4f54 5f63 6f6e   None..WM_OT_con
-00353c80: 7465 7874 5f63 7963 6c65 5f69 6e74 3a20  text_cycle_int: 
-00353c90: 2762 6c5f 6f70 6572 6174 6f72 732e 776d  'bl_operators.wm
-00353ca0: 2e57 4d5f 4f54 5f63 6f6e 7465 7874 5f63  .WM_OT_context_c
-00353cb0: 7963 6c65 5f69 6e74 2720 3d20 4e6f 6e65  ycle_int' = None
-00353cc0: 0a0a 574d 5f4f 545f 636f 6e74 6578 745f  ..WM_OT_context_
-00353cd0: 6d65 6e75 5f65 6e75 6d3a 2027 626c 5f6f  menu_enum: 'bl_o
-00353ce0: 7065 7261 746f 7273 2e77 6d2e 574d 5f4f  perators.wm.WM_O
-00353cf0: 545f 636f 6e74 6578 745f 6d65 6e75 5f65  T_context_menu_e
-00353d00: 6e75 6d27 203d 204e 6f6e 650a 0a57 4d5f  num' = None..WM_
-00353d10: 4f54 5f63 6f6e 7465 7874 5f6d 6f64 616c  OT_context_modal
-00353d20: 5f6d 6f75 7365 3a20 2762 6c5f 6f70 6572  _mouse: 'bl_oper
-00353d30: 6174 6f72 732e 776d 2e57 4d5f 4f54 5f63  ators.wm.WM_OT_c
-00353d40: 6f6e 7465 7874 5f6d 6f64 616c 5f6d 6f75  ontext_modal_mou
-00353d50: 7365 2720 3d20 4e6f 6e65 0a0a 574d 5f4f  se' = None..WM_O
-00353d60: 545f 636f 6e74 6578 745f 7069 655f 656e  T_context_pie_en
-00353d70: 756d 3a20 2762 6c5f 6f70 6572 6174 6f72  um: 'bl_operator
-00353d80: 732e 776d 2e57 4d5f 4f54 5f63 6f6e 7465  s.wm.WM_OT_conte
-00353d90: 7874 5f70 6965 5f65 6e75 6d27 203d 204e  xt_pie_enum' = N
-00353da0: 6f6e 650a 0a57 4d5f 4f54 5f63 6f6e 7465  one..WM_OT_conte
-00353db0: 7874 5f73 6361 6c65 5f66 6c6f 6174 3a20  xt_scale_float: 
-00353dc0: 2762 6c5f 6f70 6572 6174 6f72 732e 776d  'bl_operators.wm
-00353dd0: 2e57 4d5f 4f54 5f63 6f6e 7465 7874 5f73  .WM_OT_context_s
-00353de0: 6361 6c65 5f66 6c6f 6174 2720 3d20 4e6f  cale_float' = No
-00353df0: 6e65 0a0a 574d 5f4f 545f 636f 6e74 6578  ne..WM_OT_contex
-00353e00: 745f 7363 616c 655f 696e 743a 2027 626c  t_scale_int: 'bl
-00353e10: 5f6f 7065 7261 746f 7273 2e77 6d2e 574d  _operators.wm.WM
-00353e20: 5f4f 545f 636f 6e74 6578 745f 7363 616c  _OT_context_scal
-00353e30: 655f 696e 7427 203d 204e 6f6e 650a 0a57  e_int' = None..W
-00353e40: 4d5f 4f54 5f63 6f6e 7465 7874 5f73 6574  M_OT_context_set
-00353e50: 5f62 6f6f 6c65 616e 3a20 2762 6c5f 6f70  _boolean: 'bl_op
-00353e60: 6572 6174 6f72 732e 776d 2e57 4d5f 4f54  erators.wm.WM_OT
-00353e70: 5f63 6f6e 7465 7874 5f73 6574 5f62 6f6f  _context_set_boo
-00353e80: 6c65 616e 2720 3d20 4e6f 6e65 0a0a 574d  lean' = None..WM
-00353e90: 5f4f 545f 636f 6e74 6578 745f 7365 745f  _OT_context_set_
-00353ea0: 656e 756d 3a20 2762 6c5f 6f70 6572 6174  enum: 'bl_operat
-00353eb0: 6f72 732e 776d 2e57 4d5f 4f54 5f63 6f6e  ors.wm.WM_OT_con
-00353ec0: 7465 7874 5f73 6574 5f65 6e75 6d27 203d  text_set_enum' =
-00353ed0: 204e 6f6e 650a 0a57 4d5f 4f54 5f63 6f6e   None..WM_OT_con
-00353ee0: 7465 7874 5f73 6574 5f66 6c6f 6174 3a20  text_set_float: 
-00353ef0: 2762 6c5f 6f70 6572 6174 6f72 732e 776d  'bl_operators.wm
-00353f00: 2e57 4d5f 4f54 5f63 6f6e 7465 7874 5f73  .WM_OT_context_s
-00353f10: 6574 5f66 6c6f 6174 2720 3d20 4e6f 6e65  et_float' = None
-00353f20: 0a0a 574d 5f4f 545f 636f 6e74 6578 745f  ..WM_OT_context_
-00353f30: 7365 745f 6964 3a20 2762 6c5f 6f70 6572  set_id: 'bl_oper
-00353f40: 6174 6f72 732e 776d 2e57 4d5f 4f54 5f63  ators.wm.WM_OT_c
-00353f50: 6f6e 7465 7874 5f73 6574 5f69 6427 203d  ontext_set_id' =
-00353f60: 204e 6f6e 650a 0a57 4d5f 4f54 5f63 6f6e   None..WM_OT_con
-00353f70: 7465 7874 5f73 6574 5f69 6e74 3a20 2762  text_set_int: 'b
-00353f80: 6c5f 6f70 6572 6174 6f72 732e 776d 2e57  l_operators.wm.W
-00353f90: 4d5f 4f54 5f63 6f6e 7465 7874 5f73 6574  M_OT_context_set
-00353fa0: 5f69 6e74 2720 3d20 4e6f 6e65 0a0a 574d  _int' = None..WM
-00353fb0: 5f4f 545f 636f 6e74 6578 745f 7365 745f  _OT_context_set_
-00353fc0: 7374 7269 6e67 3a20 2762 6c5f 6f70 6572  string: 'bl_oper
-00353fd0: 6174 6f72 732e 776d 2e57 4d5f 4f54 5f63  ators.wm.WM_OT_c
-00353fe0: 6f6e 7465 7874 5f73 6574 5f73 7472 696e  ontext_set_strin
-00353ff0: 6727 203d 204e 6f6e 650a 0a57 4d5f 4f54  g' = None..WM_OT
-00354000: 5f63 6f6e 7465 7874 5f73 6574 5f76 616c  _context_set_val
-00354010: 7565 3a20 2762 6c5f 6f70 6572 6174 6f72  ue: 'bl_operator
-00354020: 732e 776d 2e57 4d5f 4f54 5f63 6f6e 7465  s.wm.WM_OT_conte
-00354030: 7874 5f73 6574 5f76 616c 7565 2720 3d20  xt_set_value' = 
-00354040: 4e6f 6e65 0a0a 574d 5f4f 545f 636f 6e74  None..WM_OT_cont
-00354050: 6578 745f 746f 6767 6c65 3a20 2762 6c5f  ext_toggle: 'bl_
-00354060: 6f70 6572 6174 6f72 732e 776d 2e57 4d5f  operators.wm.WM_
-00354070: 4f54 5f63 6f6e 7465 7874 5f74 6f67 676c  OT_context_toggl
-00354080: 6527 203d 204e 6f6e 650a 0a57 4d5f 4f54  e' = None..WM_OT
-00354090: 5f63 6f6e 7465 7874 5f74 6f67 676c 655f  _context_toggle_
-003540a0: 656e 756d 3a20 2762 6c5f 6f70 6572 6174  enum: 'bl_operat
-003540b0: 6f72 732e 776d 2e57 4d5f 4f54 5f63 6f6e  ors.wm.WM_OT_con
-003540c0: 7465 7874 5f74 6f67 676c 655f 656e 756d  text_toggle_enum
-003540d0: 2720 3d20 4e6f 6e65 0a0a 574d 5f4f 545f  ' = None..WM_OT_
-003540e0: 646f 635f 7669 6577 3a20 2762 6c5f 6f70  doc_view: 'bl_op
-003540f0: 6572 6174 6f72 732e 776d 2e57 4d5f 4f54  erators.wm.WM_OT
-00354100: 5f64 6f63 5f76 6965 7727 203d 204e 6f6e  _doc_view' = Non
-00354110: 650a 0a57 4d5f 4f54 5f64 6f63 5f76 6965  e..WM_OT_doc_vie
-00354120: 775f 6d61 6e75 616c 3a20 2762 6c5f 6f70  w_manual: 'bl_op
-00354130: 6572 6174 6f72 732e 776d 2e57 4d5f 4f54  erators.wm.WM_OT
-00354140: 5f64 6f63 5f76 6965 775f 6d61 6e75 616c  _doc_view_manual
-00354150: 2720 3d20 4e6f 6e65 0a0a 574d 5f4f 545f  ' = None..WM_OT_
-00354160: 6472 6f70 5f62 6c65 6e64 5f66 696c 653a  drop_blend_file:
-00354170: 2027 626c 5f6f 7065 7261 746f 7273 2e77   'bl_operators.w
-00354180: 6d2e 574d 5f4f 545f 6472 6f70 5f62 6c65  m.WM_OT_drop_ble
-00354190: 6e64 5f66 696c 6527 203d 204e 6f6e 650a  nd_file' = None.
-003541a0: 0a57 4d5f 4f54 5f6f 7065 7261 746f 725f  .WM_OT_operator_
-003541b0: 6368 6561 745f 7368 6565 743a 2027 626c  cheat_sheet: 'bl
-003541c0: 5f6f 7065 7261 746f 7273 2e77 6d2e 574d  _operators.wm.WM
-003541d0: 5f4f 545f 6f70 6572 6174 6f72 5f63 6865  _OT_operator_che
-003541e0: 6174 5f73 6865 6574 2720 3d20 4e6f 6e65  at_sheet' = None
-003541f0: 0a0a 574d 5f4f 545f 6f70 6572 6174 6f72  ..WM_OT_operator
-00354200: 5f70 6965 5f65 6e75 6d3a 2027 626c 5f6f  _pie_enum: 'bl_o
-00354210: 7065 7261 746f 7273 2e77 6d2e 574d 5f4f  perators.wm.WM_O
-00354220: 545f 6f70 6572 6174 6f72 5f70 6965 5f65  T_operator_pie_e
-00354230: 6e75 6d27 203d 204e 6f6e 650a 0a57 4d5f  num' = None..WM_
-00354240: 4f54 5f6f 776e 6572 5f64 6973 6162 6c65  OT_owner_disable
-00354250: 3a20 2762 6c5f 6f70 6572 6174 6f72 732e  : 'bl_operators.
-00354260: 776d 2e57 4d5f 4f54 5f6f 776e 6572 5f64  wm.WM_OT_owner_d
-00354270: 6973 6162 6c65 2720 3d20 4e6f 6e65 0a0a  isable' = None..
-00354280: 574d 5f4f 545f 6f77 6e65 725f 656e 6162  WM_OT_owner_enab
-00354290: 6c65 3a20 2762 6c5f 6f70 6572 6174 6f72  le: 'bl_operator
-003542a0: 732e 776d 2e57 4d5f 4f54 5f6f 776e 6572  s.wm.WM_OT_owner
-003542b0: 5f65 6e61 626c 6527 203d 204e 6f6e 650a  _enable' = None.
-003542c0: 0a57 4d5f 4f54 5f70 6174 685f 6f70 656e  .WM_OT_path_open
-003542d0: 3a20 2762 6c5f 6f70 6572 6174 6f72 732e  : 'bl_operators.
-003542e0: 776d 2e57 4d5f 4f54 5f70 6174 685f 6f70  wm.WM_OT_path_op
-003542f0: 656e 2720 3d20 4e6f 6e65 0a0a 574d 5f4f  en' = None..WM_O
-00354300: 545f 7072 6576 6965 7773 5f62 6174 6368  T_previews_batch
-00354310: 5f63 6c65 6172 3a20 2762 6c5f 6f70 6572  _clear: 'bl_oper
-00354320: 6174 6f72 732e 6669 6c65 2e57 4d5f 4f54  ators.file.WM_OT
-00354330: 5f70 7265 7669 6577 735f 6261 7463 685f  _previews_batch_
-00354340: 636c 6561 7227 203d 204e 6f6e 650a 0a57  clear' = None..W
-00354350: 4d5f 4f54 5f70 7265 7669 6577 735f 6261  M_OT_previews_ba
-00354360: 7463 685f 6765 6e65 7261 7465 3a20 2762  tch_generate: 'b
-00354370: 6c5f 6f70 6572 6174 6f72 732e 6669 6c65  l_operators.file
-00354380: 2e57 4d5f 4f54 5f70 7265 7669 6577 735f  .WM_OT_previews_
-00354390: 6261 7463 685f 6765 6e65 7261 7465 2720  batch_generate' 
-003543a0: 3d20 4e6f 6e65 0a0a 574d 5f4f 545f 7072  = None..WM_OT_pr
-003543b0: 6f70 6572 7469 6573 5f61 6464 3a20 2762  operties_add: 'b
-003543c0: 6c5f 6f70 6572 6174 6f72 732e 776d 2e57  l_operators.wm.W
-003543d0: 4d5f 4f54 5f70 726f 7065 7274 6965 735f  M_OT_properties_
-003543e0: 6164 6427 203d 204e 6f6e 650a 0a57 4d5f  add' = None..WM_
-003543f0: 4f54 5f70 726f 7065 7274 6965 735f 636f  OT_properties_co
-00354400: 6e74 6578 745f 6368 616e 6765 3a20 2762  ntext_change: 'b
-00354410: 6c5f 6f70 6572 6174 6f72 732e 776d 2e57  l_operators.wm.W
-00354420: 4d5f 4f54 5f70 726f 7065 7274 6965 735f  M_OT_properties_
-00354430: 636f 6e74 6578 745f 6368 616e 6765 2720  context_change' 
-00354440: 3d20 4e6f 6e65 0a0a 574d 5f4f 545f 7072  = None..WM_OT_pr
-00354450: 6f70 6572 7469 6573 5f65 6469 743a 2027  operties_edit: '
-00354460: 626c 5f6f 7065 7261 746f 7273 2e77 6d2e  bl_operators.wm.
-00354470: 574d 5f4f 545f 7072 6f70 6572 7469 6573  WM_OT_properties
-00354480: 5f65 6469 7427 203d 204e 6f6e 650a 0a57  _edit' = None..W
-00354490: 4d5f 4f54 5f70 726f 7065 7274 6965 735f  M_OT_properties_
-003544a0: 6564 6974 5f76 616c 7565 3a20 2762 6c5f  edit_value: 'bl_
-003544b0: 6f70 6572 6174 6f72 732e 776d 2e57 4d5f  operators.wm.WM_
-003544c0: 4f54 5f70 726f 7065 7274 6965 735f 6564  OT_properties_ed
-003544d0: 6974 5f76 616c 7565 2720 3d20 4e6f 6e65  it_value' = None
-003544e0: 0a0a 574d 5f4f 545f 7072 6f70 6572 7469  ..WM_OT_properti
-003544f0: 6573 5f72 656d 6f76 653a 2027 626c 5f6f  es_remove: 'bl_o
-00354500: 7065 7261 746f 7273 2e77 6d2e 574d 5f4f  perators.wm.WM_O
-00354510: 545f 7072 6f70 6572 7469 6573 5f72 656d  T_properties_rem
-00354520: 6f76 6527 203d 204e 6f6e 650a 0a57 4d5f  ove' = None..WM_
-00354530: 4f54 5f73 7973 696e 666f 3a20 2762 6c5f  OT_sysinfo: 'bl_
-00354540: 6f70 6572 6174 6f72 732e 776d 2e57 4d5f  operators.wm.WM_
-00354550: 4f54 5f73 7973 696e 666f 2720 3d20 4e6f  OT_sysinfo' = No
-00354560: 6e65 0a0a 574d 5f4f 545f 746f 6f6c 5f73  ne..WM_OT_tool_s
-00354570: 6574 5f62 795f 6964 3a20 2762 6c5f 6f70  et_by_id: 'bl_op
-00354580: 6572 6174 6f72 732e 776d 2e57 4d5f 4f54  erators.wm.WM_OT
-00354590: 5f74 6f6f 6c5f 7365 745f 6279 5f69 6427  _tool_set_by_id'
-003545a0: 203d 204e 6f6e 650a 0a57 4d5f 4f54 5f74   = None..WM_OT_t
-003545b0: 6f6f 6c5f 7365 745f 6279 5f69 6e64 6578  ool_set_by_index
-003545c0: 3a20 2762 6c5f 6f70 6572 6174 6f72 732e  : 'bl_operators.
-003545d0: 776d 2e57 4d5f 4f54 5f74 6f6f 6c5f 7365  wm.WM_OT_tool_se
-003545e0: 745f 6279 5f69 6e64 6578 2720 3d20 4e6f  t_by_index' = No
-003545f0: 6e65 0a0a 574d 5f4f 545f 746f 6f6c 6261  ne..WM_OT_toolba
-00354600: 723a 2027 626c 5f6f 7065 7261 746f 7273  r: 'bl_operators
-00354610: 2e77 6d2e 574d 5f4f 545f 746f 6f6c 6261  .wm.WM_OT_toolba
-00354620: 7227 203d 204e 6f6e 650a 0a57 4d5f 4f54  r' = None..WM_OT
-00354630: 5f74 6f6f 6c62 6172 5f66 616c 6c62 6163  _toolbar_fallbac
-00354640: 6b5f 7069 653a 2027 626c 5f6f 7065 7261  k_pie: 'bl_opera
-00354650: 746f 7273 2e77 6d2e 574d 5f4f 545f 746f  tors.wm.WM_OT_to
-00354660: 6f6c 6261 725f 6661 6c6c 6261 636b 5f70  olbar_fallback_p
-00354670: 6965 2720 3d20 4e6f 6e65 0a0a 574d 5f4f  ie' = None..WM_O
-00354680: 545f 746f 6f6c 6261 725f 7072 6f6d 7074  T_toolbar_prompt
-00354690: 3a20 2762 6c5f 6f70 6572 6174 6f72 732e  : 'bl_operators.
-003546a0: 776d 2e57 4d5f 4f54 5f74 6f6f 6c62 6172  wm.WM_OT_toolbar
-003546b0: 5f70 726f 6d70 7427 203d 204e 6f6e 650a  _prompt' = None.
-003546c0: 0a57 4d5f 4f54 5f75 726c 5f6f 7065 6e3a  .WM_OT_url_open:
-003546d0: 2027 626c 5f6f 7065 7261 746f 7273 2e77   'bl_operators.w
-003546e0: 6d2e 574d 5f4f 545f 7572 6c5f 6f70 656e  m.WM_OT_url_open
-003546f0: 2720 3d20 4e6f 6e65 0a0a 574d 5f4f 545f  ' = None..WM_OT_
-00354700: 7572 6c5f 6f70 656e 5f70 7265 7365 743a  url_open_preset:
-00354710: 2027 626c 5f6f 7065 7261 746f 7273 2e77   'bl_operators.w
-00354720: 6d2e 574d 5f4f 545f 7572 6c5f 6f70 656e  m.WM_OT_url_open
-00354730: 5f70 7265 7365 7427 203d 204e 6f6e 650a  _preset' = None.
-00354740: 0a57 4f52 4b53 5041 4345 5f50 545f 6164  .WORKSPACE_PT_ad
-00354750: 646f 6e73 3a20 2762 6c5f 7569 2e70 726f  dons: 'bl_ui.pro
-00354760: 7065 7274 6965 735f 776f 726b 7370 6163  perties_workspac
-00354770: 652e 574f 524b 5350 4143 455f 5054 5f61  e.WORKSPACE_PT_a
-00354780: 6464 6f6e 7327 203d 204e 6f6e 650a 0a57  ddons' = None..W
-00354790: 4f52 4b53 5041 4345 5f50 545f 6375 7374  ORKSPACE_PT_cust
-003547a0: 6f6d 5f70 726f 7073 3a20 2762 6c5f 7569  om_props: 'bl_ui
-003547b0: 2e70 726f 7065 7274 6965 735f 776f 726b  .properties_work
-003547c0: 7370 6163 652e 574f 524b 5350 4143 455f  space.WORKSPACE_
-003547d0: 5054 5f63 7573 746f 6d5f 7072 6f70 7327  PT_custom_props'
-003547e0: 203d 204e 6f6e 650a 0a57 4f52 4b53 5041   = None..WORKSPA
-003547f0: 4345 5f50 545f 6d61 696e 3a20 2762 6c5f  CE_PT_main: 'bl_
-00354800: 7569 2e70 726f 7065 7274 6965 735f 776f  ui.properties_wo
-00354810: 726b 7370 6163 652e 574f 524b 5350 4143  rkspace.WORKSPAC
-00354820: 455f 5054 5f6d 6169 6e27 203d 204e 6f6e  E_PT_main' = Non
-00354830: 650a 0a57 4f52 4c44 5f50 545f 636f 6e74  e..WORLD_PT_cont
-00354840: 6578 745f 776f 726c 643a 2027 626c 5f75  ext_world: 'bl_u
-00354850: 692e 7072 6f70 6572 7469 6573 5f77 6f72  i.properties_wor
-00354860: 6c64 2e57 4f52 4c44 5f50 545f 636f 6e74  ld.WORLD_PT_cont
-00354870: 6578 745f 776f 726c 6427 203d 204e 6f6e  ext_world' = Non
-00354880: 650a 0a57 4f52 4c44 5f50 545f 6375 7374  e..WORLD_PT_cust
-00354890: 6f6d 5f70 726f 7073 3a20 2762 6c5f 7569  om_props: 'bl_ui
-003548a0: 2e70 726f 7065 7274 6965 735f 776f 726c  .properties_worl
-003548b0: 642e 574f 524c 445f 5054 5f63 7573 746f  d.WORLD_PT_custo
-003548c0: 6d5f 7072 6f70 7327 203d 204e 6f6e 650a  m_props' = None.
-003548d0: 0a57 4f52 4c44 5f50 545f 7669 6577 706f  .WORLD_PT_viewpo
-003548e0: 7274 5f64 6973 706c 6179 3a20 2762 6c5f  rt_display: 'bl_
-003548f0: 7569 2e70 726f 7065 7274 6965 735f 776f  ui.properties_wo
-00354900: 726c 642e 574f 524c 445f 5054 5f76 6965  rld.WORLD_PT_vie
-00354910: 7770 6f72 745f 6469 7370 6c61 7927 203d  wport_display' =
-00354920: 204e 6f6e 650a                            None.
+00352720: 5f67 7261 6469 656e 743a 2027 626c 5f75  _gradient: 'bl_u
+00352730: 692e 7370 6163 655f 7669 6577 3364 5f74  i.space_view3d_t
+00352740: 6f6f 6c62 6172 2e56 4945 5733 445f 5054  oolbar.VIEW3D_PT
+00352750: 5f74 6f6f 6c73 5f77 6569 6768 745f 6772  _tools_weight_gr
+00352760: 6164 6965 6e74 2720 3d20 4e6f 6e65 0a0a  adient' = None..
+00352770: 5649 4557 3344 5f50 545f 746f 6f6c 735f  VIEW3D_PT_tools_
+00352780: 7765 6967 6874 7061 696e 745f 6f70 7469  weightpaint_opti
+00352790: 6f6e 733a 2027 626c 5f75 692e 7370 6163  ons: 'bl_ui.spac
+003527a0: 655f 7669 6577 3364 5f74 6f6f 6c62 6172  e_view3d_toolbar
+003527b0: 2e56 4945 5733 445f 5054 5f74 6f6f 6c73  .VIEW3D_PT_tools
+003527c0: 5f77 6569 6768 7470 6169 6e74 5f6f 7074  _weightpaint_opt
+003527d0: 696f 6e73 2720 3d20 4e6f 6e65 0a0a 5649  ions' = None..VI
+003527e0: 4557 3344 5f50 545f 746f 6f6c 735f 7765  EW3D_PT_tools_we
+003527f0: 6967 6874 7061 696e 745f 7379 6d6d 6574  ightpaint_symmet
+00352800: 7279 3a20 2762 6c5f 7569 2e73 7061 6365  ry: 'bl_ui.space
+00352810: 5f76 6965 7733 645f 746f 6f6c 6261 722e  _view3d_toolbar.
+00352820: 5649 4557 3344 5f50 545f 746f 6f6c 735f  VIEW3D_PT_tools_
+00352830: 7765 6967 6874 7061 696e 745f 7379 6d6d  weightpaint_symm
+00352840: 6574 7279 2720 3d20 4e6f 6e65 0a0a 5649  etry' = None..VI
+00352850: 4557 3344 5f50 545f 746f 6f6c 735f 7765  EW3D_PT_tools_we
+00352860: 6967 6874 7061 696e 745f 7379 6d6d 6574  ightpaint_symmet
+00352870: 7279 5f66 6f72 5f74 6f70 6261 723a 2027  ry_for_topbar: '
+00352880: 626c 5f75 692e 7370 6163 655f 7669 6577  bl_ui.space_view
+00352890: 3364 5f74 6f6f 6c62 6172 2e56 4945 5733  3d_toolbar.VIEW3
+003528a0: 445f 5054 5f74 6f6f 6c73 5f77 6569 6768  D_PT_tools_weigh
+003528b0: 7470 6169 6e74 5f73 796d 6d65 7472 795f  tpaint_symmetry_
+003528c0: 666f 725f 746f 7062 6172 2720 3d20 4e6f  for_topbar' = No
+003528d0: 6e65 0a0a 5649 4557 3344 5f50 545f 7472  ne..VIEW3D_PT_tr
+003528e0: 616e 7366 6f72 6d5f 6f72 6965 6e74 6174  ansform_orientat
+003528f0: 696f 6e73 3a20 2762 6c5f 7569 2e73 7061  ions: 'bl_ui.spa
+00352900: 6365 5f76 6965 7733 642e 5649 4557 3344  ce_view3d.VIEW3D
+00352910: 5f50 545f 7472 616e 7366 6f72 6d5f 6f72  _PT_transform_or
+00352920: 6965 6e74 6174 696f 6e73 2720 3d20 4e6f  ientations' = No
+00352930: 6e65 0a0a 5649 4557 3344 5f50 545f 7669  ne..VIEW3D_PT_vi
+00352940: 6577 3364 5f63 7572 736f 723a 2027 626c  ew3d_cursor: 'bl
+00352950: 5f75 692e 7370 6163 655f 7669 6577 3364  _ui.space_view3d
+00352960: 2e56 4945 5733 445f 5054 5f76 6965 7733  .VIEW3D_PT_view3
+00352970: 645f 6375 7273 6f72 2720 3d20 4e6f 6e65  d_cursor' = None
+00352980: 0a0a 5649 4557 3344 5f50 545f 7669 6577  ..VIEW3D_PT_view
+00352990: 3364 5f6c 6f63 6b3a 2027 626c 5f75 692e  3d_lock: 'bl_ui.
+003529a0: 7370 6163 655f 7669 6577 3364 2e56 4945  space_view3d.VIE
+003529b0: 5733 445f 5054 5f76 6965 7733 645f 6c6f  W3D_PT_view3d_lo
+003529c0: 636b 2720 3d20 4e6f 6e65 0a0a 5649 4557  ck' = None..VIEW
+003529d0: 3344 5f50 545f 7669 6577 3364 5f70 726f  3D_PT_view3d_pro
+003529e0: 7065 7274 6965 733a 2027 626c 5f75 692e  perties: 'bl_ui.
+003529f0: 7370 6163 655f 7669 6577 3364 2e56 4945  space_view3d.VIE
+00352a00: 5733 445f 5054 5f76 6965 7733 645f 7072  W3D_PT_view3d_pr
+00352a10: 6f70 6572 7469 6573 2720 3d20 4e6f 6e65  operties' = None
+00352a20: 0a0a 5649 4557 3344 5f50 545f 7669 6577  ..VIEW3D_PT_view
+00352a30: 3364 5f73 7465 7265 6f3a 2027 626c 5f75  3d_stereo: 'bl_u
+00352a40: 692e 7370 6163 655f 7669 6577 3364 2e56  i.space_view3d.V
+00352a50: 4945 5733 445f 5054 5f76 6965 7733 645f  IEW3D_PT_view3d_
+00352a60: 7374 6572 656f 2720 3d20 4e6f 6e65 0a0a  stereo' = None..
+00352a70: 5649 4557 3344 5f50 545f 7669 6577 706f  VIEW3D_PT_viewpo
+00352a80: 7274 5f64 6562 7567 3a20 2762 6c5f 7569  rt_debug: 'bl_ui
+00352a90: 2e73 7061 6365 5f76 6965 7733 642e 5649  .space_view3d.VI
+00352aa0: 4557 3344 5f50 545f 7669 6577 706f 7274  EW3D_PT_viewport
+00352ab0: 5f64 6562 7567 2720 3d20 4e6f 6e65 0a0a  _debug' = None..
+00352ac0: 5649 4557 4c41 5945 525f 4d54 5f6c 6967  VIEWLAYER_MT_lig
+00352ad0: 6874 6772 6f75 705f 7379 6e63 3a20 2762  htgroup_sync: 'b
+00352ae0: 6c5f 7569 2e70 726f 7065 7274 6965 735f  l_ui.properties_
+00352af0: 7669 6577 5f6c 6179 6572 2e56 4945 574c  view_layer.VIEWL
+00352b00: 4159 4552 5f4d 545f 6c69 6768 7467 726f  AYER_MT_lightgro
+00352b10: 7570 5f73 796e 6327 203d 204e 6f6e 650a  up_sync' = None.
+00352b20: 0a56 4945 574c 4159 4552 5f50 545f 6565  .VIEWLAYER_PT_ee
+00352b30: 7665 655f 6c61 7965 725f 7061 7373 6573  vee_layer_passes
+00352b40: 5f64 6174 613a 2027 626c 5f75 692e 7072  _data: 'bl_ui.pr
+00352b50: 6f70 6572 7469 6573 5f76 6965 775f 6c61  operties_view_la
+00352b60: 7965 722e 5649 4557 4c41 5945 525f 5054  yer.VIEWLAYER_PT
+00352b70: 5f65 6576 6565 5f6c 6179 6572 5f70 6173  _eevee_layer_pas
+00352b80: 7365 735f 6461 7461 2720 3d20 4e6f 6e65  ses_data' = None
+00352b90: 0a0a 5649 4557 4c41 5945 525f 5054 5f65  ..VIEWLAYER_PT_e
+00352ba0: 6576 6565 5f6c 6179 6572 5f70 6173 7365  evee_layer_passe
+00352bb0: 735f 6566 6665 6374 733a 2027 626c 5f75  s_effects: 'bl_u
+00352bc0: 692e 7072 6f70 6572 7469 6573 5f76 6965  i.properties_vie
+00352bd0: 775f 6c61 7965 722e 5649 4557 4c41 5945  w_layer.VIEWLAYE
+00352be0: 525f 5054 5f65 6576 6565 5f6c 6179 6572  R_PT_eevee_layer
+00352bf0: 5f70 6173 7365 735f 6566 6665 6374 7327  _passes_effects'
+00352c00: 203d 204e 6f6e 650a 0a56 4945 574c 4159   = None..VIEWLAY
+00352c10: 4552 5f50 545f 6565 7665 655f 6c61 7965  ER_PT_eevee_laye
+00352c20: 725f 7061 7373 6573 5f6c 6967 6874 3a20  r_passes_light: 
+00352c30: 2762 6c5f 7569 2e70 726f 7065 7274 6965  'bl_ui.propertie
+00352c40: 735f 7669 6577 5f6c 6179 6572 2e56 4945  s_view_layer.VIE
+00352c50: 574c 4159 4552 5f50 545f 6565 7665 655f  WLAYER_PT_eevee_
+00352c60: 6c61 7965 725f 7061 7373 6573 5f6c 6967  layer_passes_lig
+00352c70: 6874 2720 3d20 4e6f 6e65 0a0a 5649 4557  ht' = None..VIEW
+00352c80: 4c41 5945 525f 5054 5f65 6576 6565 5f6e  LAYER_PT_eevee_n
+00352c90: 6578 745f 6c61 7965 725f 7061 7373 6573  ext_layer_passes
+00352ca0: 5f64 6174 613a 2027 626c 5f75 692e 7072  _data: 'bl_ui.pr
+00352cb0: 6f70 6572 7469 6573 5f76 6965 775f 6c61  operties_view_la
+00352cc0: 7965 722e 5649 4557 4c41 5945 525f 5054  yer.VIEWLAYER_PT
+00352cd0: 5f65 6576 6565 5f6e 6578 745f 6c61 7965  _eevee_next_laye
+00352ce0: 725f 7061 7373 6573 5f64 6174 6127 203d  r_passes_data' =
+00352cf0: 204e 6f6e 650a 0a56 4945 574c 4159 4552   None..VIEWLAYER
+00352d00: 5f50 545f 6672 6565 7374 796c 653a 2027  _PT_freestyle: '
+00352d10: 626c 5f75 692e 7072 6f70 6572 7469 6573  bl_ui.properties
+00352d20: 5f66 7265 6573 7479 6c65 2e56 4945 574c  _freestyle.VIEWL
+00352d30: 4159 4552 5f50 545f 6672 6565 7374 796c  AYER_PT_freestyl
+00352d40: 6527 203d 204e 6f6e 650a 0a56 4945 574c  e' = None..VIEWL
+00352d50: 4159 4552 5f50 545f 6672 6565 7374 796c  AYER_PT_freestyl
+00352d60: 655f 6564 6765 5f64 6574 6563 7469 6f6e  e_edge_detection
+00352d70: 3a20 2762 6c5f 7569 2e70 726f 7065 7274  : 'bl_ui.propert
+00352d80: 6965 735f 6672 6565 7374 796c 652e 5649  ies_freestyle.VI
+00352d90: 4557 4c41 5945 525f 5054 5f66 7265 6573  EWLAYER_PT_frees
+00352da0: 7479 6c65 5f65 6467 655f 6465 7465 6374  tyle_edge_detect
+00352db0: 696f 6e27 203d 204e 6f6e 650a 0a56 4945  ion' = None..VIE
+00352dc0: 574c 4159 4552 5f50 545f 6672 6565 7374  WLAYER_PT_freest
+00352dd0: 796c 655f 6c69 6e65 7365 743a 2027 626c  yle_lineset: 'bl
+00352de0: 5f75 692e 7072 6f70 6572 7469 6573 5f66  _ui.properties_f
+00352df0: 7265 6573 7479 6c65 2e56 4945 574c 4159  reestyle.VIEWLAY
+00352e00: 4552 5f50 545f 6672 6565 7374 796c 655f  ER_PT_freestyle_
+00352e10: 6c69 6e65 7365 7427 203d 204e 6f6e 650a  lineset' = None.
+00352e20: 0a56 4945 574c 4159 4552 5f50 545f 6672  .VIEWLAYER_PT_fr
+00352e30: 6565 7374 796c 655f 6c69 6e65 7365 745f  eestyle_lineset_
+00352e40: 636f 6c6c 6563 7469 6f6e 3a20 2762 6c5f  collection: 'bl_
+00352e50: 7569 2e70 726f 7065 7274 6965 735f 6672  ui.properties_fr
+00352e60: 6565 7374 796c 652e 5649 4557 4c41 5945  eestyle.VIEWLAYE
+00352e70: 525f 5054 5f66 7265 6573 7479 6c65 5f6c  R_PT_freestyle_l
+00352e80: 696e 6573 6574 5f63 6f6c 6c65 6374 696f  ineset_collectio
+00352e90: 6e27 203d 204e 6f6e 650a 0a56 4945 574c  n' = None..VIEWL
+00352ea0: 4159 4552 5f50 545f 6672 6565 7374 796c  AYER_PT_freestyl
+00352eb0: 655f 6c69 6e65 7365 745f 6564 6765 7479  e_lineset_edgety
+00352ec0: 7065 3a20 2762 6c5f 7569 2e70 726f 7065  pe: 'bl_ui.prope
+00352ed0: 7274 6965 735f 6672 6565 7374 796c 652e  rties_freestyle.
+00352ee0: 5649 4557 4c41 5945 525f 5054 5f66 7265  VIEWLAYER_PT_fre
+00352ef0: 6573 7479 6c65 5f6c 696e 6573 6574 5f65  estyle_lineset_e
+00352f00: 6467 6574 7970 6527 203d 204e 6f6e 650a  dgetype' = None.
+00352f10: 0a56 4945 574c 4159 4552 5f50 545f 6672  .VIEWLAYER_PT_fr
+00352f20: 6565 7374 796c 655f 6c69 6e65 7365 745f  eestyle_lineset_
+00352f30: 6661 6365 6d61 726b 733a 2027 626c 5f75  facemarks: 'bl_u
+00352f40: 692e 7072 6f70 6572 7469 6573 5f66 7265  i.properties_fre
+00352f50: 6573 7479 6c65 2e56 4945 574c 4159 4552  estyle.VIEWLAYER
+00352f60: 5f50 545f 6672 6565 7374 796c 655f 6c69  _PT_freestyle_li
+00352f70: 6e65 7365 745f 6661 6365 6d61 726b 7327  neset_facemarks'
+00352f80: 203d 204e 6f6e 650a 0a56 4945 574c 4159   = None..VIEWLAY
+00352f90: 4552 5f50 545f 6672 6565 7374 796c 655f  ER_PT_freestyle_
+00352fa0: 6c69 6e65 7365 745f 7669 7369 6269 6c74  lineset_visibilt
+00352fb0: 793a 2027 626c 5f75 692e 7072 6f70 6572  y: 'bl_ui.proper
+00352fc0: 7469 6573 5f66 7265 6573 7479 6c65 2e56  ties_freestyle.V
+00352fd0: 4945 574c 4159 4552 5f50 545f 6672 6565  IEWLAYER_PT_free
+00352fe0: 7374 796c 655f 6c69 6e65 7365 745f 7669  style_lineset_vi
+00352ff0: 7369 6269 6c74 7927 203d 204e 6f6e 650a  sibilty' = None.
+00353000: 0a56 4945 574c 4159 4552 5f50 545f 6672  .VIEWLAYER_PT_fr
+00353010: 6565 7374 796c 655f 6c69 6e65 7374 796c  eestyle_linestyl
+00353020: 655f 616c 7068 613a 2027 626c 5f75 692e  e_alpha: 'bl_ui.
+00353030: 7072 6f70 6572 7469 6573 5f66 7265 6573  properties_frees
+00353040: 7479 6c65 2e56 4945 574c 4159 4552 5f50  tyle.VIEWLAYER_P
+00353050: 545f 6672 6565 7374 796c 655f 6c69 6e65  T_freestyle_line
+00353060: 7374 796c 655f 616c 7068 6127 203d 204e  style_alpha' = N
+00353070: 6f6e 650a 0a56 4945 574c 4159 4552 5f50  one..VIEWLAYER_P
+00353080: 545f 6672 6565 7374 796c 655f 6c69 6e65  T_freestyle_line
+00353090: 7374 796c 655f 636f 6c6f 723a 2027 626c  style_color: 'bl
+003530a0: 5f75 692e 7072 6f70 6572 7469 6573 5f66  _ui.properties_f
+003530b0: 7265 6573 7479 6c65 2e56 4945 574c 4159  reestyle.VIEWLAY
+003530c0: 4552 5f50 545f 6672 6565 7374 796c 655f  ER_PT_freestyle_
+003530d0: 6c69 6e65 7374 796c 655f 636f 6c6f 7227  linestyle_color'
+003530e0: 203d 204e 6f6e 650a 0a56 4945 574c 4159   = None..VIEWLAY
+003530f0: 4552 5f50 545f 6672 6565 7374 796c 655f  ER_PT_freestyle_
+00353100: 6c69 6e65 7374 796c 655f 6765 6f6d 6574  linestyle_geomet
+00353110: 7279 3a20 2762 6c5f 7569 2e70 726f 7065  ry: 'bl_ui.prope
+00353120: 7274 6965 735f 6672 6565 7374 796c 652e  rties_freestyle.
+00353130: 5649 4557 4c41 5945 525f 5054 5f66 7265  VIEWLAYER_PT_fre
+00353140: 6573 7479 6c65 5f6c 696e 6573 7479 6c65  estyle_linestyle
+00353150: 5f67 656f 6d65 7472 7927 203d 204e 6f6e  _geometry' = Non
+00353160: 650a 0a56 4945 574c 4159 4552 5f50 545f  e..VIEWLAYER_PT_
+00353170: 6672 6565 7374 796c 655f 6c69 6e65 7374  freestyle_linest
+00353180: 796c 655f 7374 726f 6b65 733a 2027 626c  yle_strokes: 'bl
+00353190: 5f75 692e 7072 6f70 6572 7469 6573 5f66  _ui.properties_f
+003531a0: 7265 6573 7479 6c65 2e56 4945 574c 4159  reestyle.VIEWLAY
+003531b0: 4552 5f50 545f 6672 6565 7374 796c 655f  ER_PT_freestyle_
+003531c0: 6c69 6e65 7374 796c 655f 7374 726f 6b65  linestyle_stroke
+003531d0: 7327 203d 204e 6f6e 650a 0a56 4945 574c  s' = None..VIEWL
+003531e0: 4159 4552 5f50 545f 6672 6565 7374 796c  AYER_PT_freestyl
+003531f0: 655f 6c69 6e65 7374 796c 655f 7374 726f  e_linestyle_stro
+00353200: 6b65 735f 6368 6169 6e69 6e67 3a20 2762  kes_chaining: 'b
+00353210: 6c5f 7569 2e70 726f 7065 7274 6965 735f  l_ui.properties_
+00353220: 6672 6565 7374 796c 652e 5649 4557 4c41  freestyle.VIEWLA
+00353230: 5945 525f 5054 5f66 7265 6573 7479 6c65  YER_PT_freestyle
+00353240: 5f6c 696e 6573 7479 6c65 5f73 7472 6f6b  _linestyle_strok
+00353250: 6573 5f63 6861 696e 696e 6727 203d 204e  es_chaining' = N
+00353260: 6f6e 650a 0a56 4945 574c 4159 4552 5f50  one..VIEWLAYER_P
+00353270: 545f 6672 6565 7374 796c 655f 6c69 6e65  T_freestyle_line
+00353280: 7374 796c 655f 7374 726f 6b65 735f 6461  style_strokes_da
+00353290: 7368 6564 6c69 6e65 3a20 2762 6c5f 7569  shedline: 'bl_ui
+003532a0: 2e70 726f 7065 7274 6965 735f 6672 6565  .properties_free
+003532b0: 7374 796c 652e 5649 4557 4c41 5945 525f  style.VIEWLAYER_
+003532c0: 5054 5f66 7265 6573 7479 6c65 5f6c 696e  PT_freestyle_lin
+003532d0: 6573 7479 6c65 5f73 7472 6f6b 6573 5f64  estyle_strokes_d
+003532e0: 6173 6865 646c 696e 6527 203d 204e 6f6e  ashedline' = Non
+003532f0: 650a 0a56 4945 574c 4159 4552 5f50 545f  e..VIEWLAYER_PT_
+00353300: 6672 6565 7374 796c 655f 6c69 6e65 7374  freestyle_linest
+00353310: 796c 655f 7374 726f 6b65 735f 7365 6c65  yle_strokes_sele
+00353320: 6374 696f 6e3a 2027 626c 5f75 692e 7072  ction: 'bl_ui.pr
+00353330: 6f70 6572 7469 6573 5f66 7265 6573 7479  operties_freesty
+00353340: 6c65 2e56 4945 574c 4159 4552 5f50 545f  le.VIEWLAYER_PT_
+00353350: 6672 6565 7374 796c 655f 6c69 6e65 7374  freestyle_linest
+00353360: 796c 655f 7374 726f 6b65 735f 7365 6c65  yle_strokes_sele
+00353370: 6374 696f 6e27 203d 204e 6f6e 650a 0a56  ction' = None..V
+00353380: 4945 574c 4159 4552 5f50 545f 6672 6565  IEWLAYER_PT_free
+00353390: 7374 796c 655f 6c69 6e65 7374 796c 655f  style_linestyle_
+003533a0: 7374 726f 6b65 735f 736f 7274 696e 673a  strokes_sorting:
+003533b0: 2027 626c 5f75 692e 7072 6f70 6572 7469   'bl_ui.properti
+003533c0: 6573 5f66 7265 6573 7479 6c65 2e56 4945  es_freestyle.VIE
+003533d0: 574c 4159 4552 5f50 545f 6672 6565 7374  WLAYER_PT_freest
+003533e0: 796c 655f 6c69 6e65 7374 796c 655f 7374  yle_linestyle_st
+003533f0: 726f 6b65 735f 736f 7274 696e 6727 203d  rokes_sorting' =
+00353400: 204e 6f6e 650a 0a56 4945 574c 4159 4552   None..VIEWLAYER
+00353410: 5f50 545f 6672 6565 7374 796c 655f 6c69  _PT_freestyle_li
+00353420: 6e65 7374 796c 655f 7374 726f 6b65 735f  nestyle_strokes_
+00353430: 7370 6c69 7474 696e 673a 2027 626c 5f75  splitting: 'bl_u
+00353440: 692e 7072 6f70 6572 7469 6573 5f66 7265  i.properties_fre
+00353450: 6573 7479 6c65 2e56 4945 574c 4159 4552  estyle.VIEWLAYER
+00353460: 5f50 545f 6672 6565 7374 796c 655f 6c69  _PT_freestyle_li
+00353470: 6e65 7374 796c 655f 7374 726f 6b65 735f  nestyle_strokes_
+00353480: 7370 6c69 7474 696e 6727 203d 204e 6f6e  splitting' = Non
+00353490: 650a 0a56 4945 574c 4159 4552 5f50 545f  e..VIEWLAYER_PT_
+003534a0: 6672 6565 7374 796c 655f 6c69 6e65 7374  freestyle_linest
+003534b0: 796c 655f 7374 726f 6b65 735f 7370 6c69  yle_strokes_spli
+003534c0: 7474 696e 675f 7061 7474 6572 6e3a 2027  tting_pattern: '
+003534d0: 626c 5f75 692e 7072 6f70 6572 7469 6573  bl_ui.properties
+003534e0: 5f66 7265 6573 7479 6c65 2e56 4945 574c  _freestyle.VIEWL
+003534f0: 4159 4552 5f50 545f 6672 6565 7374 796c  AYER_PT_freestyl
+00353500: 655f 6c69 6e65 7374 796c 655f 7374 726f  e_linestyle_stro
+00353510: 6b65 735f 7370 6c69 7474 696e 675f 7061  kes_splitting_pa
+00353520: 7474 6572 6e27 203d 204e 6f6e 650a 0a56  ttern' = None..V
+00353530: 4945 574c 4159 4552 5f50 545f 6672 6565  IEWLAYER_PT_free
+00353540: 7374 796c 655f 6c69 6e65 7374 796c 655f  style_linestyle_
+00353550: 7465 7874 7572 653a 2027 626c 5f75 692e  texture: 'bl_ui.
+00353560: 7072 6f70 6572 7469 6573 5f66 7265 6573  properties_frees
+00353570: 7479 6c65 2e56 4945 574c 4159 4552 5f50  tyle.VIEWLAYER_P
+00353580: 545f 6672 6565 7374 796c 655f 6c69 6e65  T_freestyle_line
+00353590: 7374 796c 655f 7465 7874 7572 6527 203d  style_texture' =
+003535a0: 204e 6f6e 650a 0a56 4945 574c 4159 4552   None..VIEWLAYER
+003535b0: 5f50 545f 6672 6565 7374 796c 655f 6c69  _PT_freestyle_li
+003535c0: 6e65 7374 796c 655f 7468 6963 6b6e 6573  nestyle_thicknes
+003535d0: 733a 2027 626c 5f75 692e 7072 6f70 6572  s: 'bl_ui.proper
+003535e0: 7469 6573 5f66 7265 6573 7479 6c65 2e56  ties_freestyle.V
+003535f0: 4945 574c 4159 4552 5f50 545f 6672 6565  IEWLAYER_PT_free
+00353600: 7374 796c 655f 6c69 6e65 7374 796c 655f  style_linestyle_
+00353610: 7468 6963 6b6e 6573 7327 203d 204e 6f6e  thickness' = Non
+00353620: 650a 0a56 4945 574c 4159 4552 5f50 545f  e..VIEWLAYER_PT_
+00353630: 6672 6565 7374 796c 655f 7374 796c 655f  freestyle_style_
+00353640: 6d6f 6475 6c65 733a 2027 626c 5f75 692e  modules: 'bl_ui.
+00353650: 7072 6f70 6572 7469 6573 5f66 7265 6573  properties_frees
+00353660: 7479 6c65 2e56 4945 574c 4159 4552 5f50  tyle.VIEWLAYER_P
+00353670: 545f 6672 6565 7374 796c 655f 7374 796c  T_freestyle_styl
+00353680: 655f 6d6f 6475 6c65 7327 203d 204e 6f6e  e_modules' = Non
+00353690: 650a 0a56 4945 574c 4159 4552 5f50 545f  e..VIEWLAYER_PT_
+003536a0: 6c61 7965 723a 2027 626c 5f75 692e 7072  layer: 'bl_ui.pr
+003536b0: 6f70 6572 7469 6573 5f76 6965 775f 6c61  operties_view_la
+003536c0: 7965 722e 5649 4557 4c41 5945 525f 5054  yer.VIEWLAYER_PT
+003536d0: 5f6c 6179 6572 2720 3d20 4e6f 6e65 0a0a  _layer' = None..
+003536e0: 5649 4557 4c41 5945 525f 5054 5f6c 6179  VIEWLAYER_PT_lay
+003536f0: 6572 5f63 7573 746f 6d5f 7072 6f70 733a  er_custom_props:
+00353700: 2027 626c 5f75 692e 7072 6f70 6572 7469   'bl_ui.properti
+00353710: 6573 5f76 6965 775f 6c61 7965 722e 5649  es_view_layer.VI
+00353720: 4557 4c41 5945 525f 5054 5f6c 6179 6572  EWLAYER_PT_layer
+00353730: 5f63 7573 746f 6d5f 7072 6f70 7327 203d  _custom_props' =
+00353740: 204e 6f6e 650a 0a56 4945 574c 4159 4552   None..VIEWLAYER
+00353750: 5f50 545f 6c61 7965 725f 7061 7373 6573  _PT_layer_passes
+00353760: 3a20 2762 6c5f 7569 2e70 726f 7065 7274  : 'bl_ui.propert
+00353770: 6965 735f 7669 6577 5f6c 6179 6572 2e56  ies_view_layer.V
+00353780: 4945 574c 4159 4552 5f50 545f 6c61 7965  IEWLAYER_PT_laye
+00353790: 725f 7061 7373 6573 2720 3d20 4e6f 6e65  r_passes' = None
+003537a0: 0a0a 5649 4557 4c41 5945 525f 5054 5f6c  ..VIEWLAYER_PT_l
+003537b0: 6179 6572 5f70 6173 7365 735f 616f 763a  ayer_passes_aov:
+003537c0: 2027 626c 5f75 692e 7072 6f70 6572 7469   'bl_ui.properti
+003537d0: 6573 5f76 6965 775f 6c61 7965 722e 5649  es_view_layer.VI
+003537e0: 4557 4c41 5945 525f 5054 5f6c 6179 6572  EWLAYER_PT_layer
+003537f0: 5f70 6173 7365 735f 616f 7627 203d 204e  _passes_aov' = N
+00353800: 6f6e 650a 0a56 4945 574c 4159 4552 5f50  one..VIEWLAYER_P
+00353810: 545f 6c61 7965 725f 7061 7373 6573 5f63  T_layer_passes_c
+00353820: 7279 7074 6f6d 6174 7465 3a20 2762 6c5f  ryptomatte: 'bl_
+00353830: 7569 2e70 726f 7065 7274 6965 735f 7669  ui.properties_vi
+00353840: 6577 5f6c 6179 6572 2e56 4945 574c 4159  ew_layer.VIEWLAY
+00353850: 4552 5f50 545f 6c61 7965 725f 7061 7373  ER_PT_layer_pass
+00353860: 6573 5f63 7279 7074 6f6d 6174 7465 2720  es_cryptomatte' 
+00353870: 3d20 4e6f 6e65 0a0a 5649 4557 4c41 5945  = None..VIEWLAYE
+00353880: 525f 5054 5f6c 6179 6572 5f70 6173 7365  R_PT_layer_passe
+00353890: 735f 6c69 6768 7467 726f 7570 733a 2027  s_lightgroups: '
+003538a0: 626c 5f75 692e 7072 6f70 6572 7469 6573  bl_ui.properties
+003538b0: 5f76 6965 775f 6c61 7965 722e 5649 4557  _view_layer.VIEW
+003538c0: 4c41 5945 525f 5054 5f6c 6179 6572 5f70  LAYER_PT_layer_p
+003538d0: 6173 7365 735f 6c69 6768 7467 726f 7570  asses_lightgroup
+003538e0: 7327 203d 204e 6f6e 650a 0a56 4945 574c  s' = None..VIEWL
+003538f0: 4159 4552 5f55 4c5f 616f 763a 2027 626c  AYER_UL_aov: 'bl
+00353900: 5f75 692e 7072 6f70 6572 7469 6573 5f76  _ui.properties_v
+00353910: 6965 775f 6c61 7965 722e 5649 4557 4c41  iew_layer.VIEWLA
+00353920: 5945 525f 554c 5f61 6f76 2720 3d20 4e6f  YER_UL_aov' = No
+00353930: 6e65 0a0a 5649 4557 4c41 5945 525f 554c  ne..VIEWLAYER_UL
+00353940: 5f6c 696e 6573 6574 733a 2027 626c 5f75  _linesets: 'bl_u
+00353950: 692e 7072 6f70 6572 7469 6573 5f66 7265  i.properties_fre
+00353960: 6573 7479 6c65 2e56 4945 574c 4159 4552  estyle.VIEWLAYER
+00353970: 5f55 4c5f 6c69 6e65 7365 7473 2720 3d20  _UL_linesets' = 
+00353980: 4e6f 6e65 0a0a 564f 4c55 4d45 5f55 4c5f  None..VOLUME_UL_
+00353990: 6772 6964 733a 2027 626c 5f75 692e 7072  grids: 'bl_ui.pr
+003539a0: 6f70 6572 7469 6573 5f64 6174 615f 766f  operties_data_vo
+003539b0: 6c75 6d65 2e56 4f4c 554d 455f 554c 5f67  lume.VOLUME_UL_g
+003539c0: 7269 6473 2720 3d20 4e6f 6e65 0a0a 574d  rids' = None..WM
+003539d0: 5f4d 545f 6f70 6572 6174 6f72 5f70 7265  _MT_operator_pre
+003539e0: 7365 7473 3a20 2762 6c5f 6f70 6572 6174  sets: 'bl_operat
+003539f0: 6f72 732e 7072 6573 6574 732e 574d 5f4d  ors.presets.WM_M
+00353a00: 545f 6f70 6572 6174 6f72 5f70 7265 7365  T_operator_prese
+00353a10: 7473 2720 3d20 4e6f 6e65 0a0a 574d 5f4d  ts' = None..WM_M
+00353a20: 545f 7370 6c61 7368 3a20 2762 6c5f 6f70  T_splash: 'bl_op
+00353a30: 6572 6174 6f72 732e 776d 2e57 4d5f 4d54  erators.wm.WM_MT
+00353a40: 5f73 706c 6173 6827 203d 204e 6f6e 650a  _splash' = None.
+00353a50: 0a57 4d5f 4d54 5f73 706c 6173 685f 6162  .WM_MT_splash_ab
+00353a60: 6f75 743a 2027 626c 5f6f 7065 7261 746f  out: 'bl_operato
+00353a70: 7273 2e77 6d2e 574d 5f4d 545f 7370 6c61  rs.wm.WM_MT_spla
+00353a80: 7368 5f61 626f 7574 2720 3d20 4e6f 6e65  sh_about' = None
+00353a90: 0a0a 574d 5f4d 545f 7370 6c61 7368 5f71  ..WM_MT_splash_q
+00353aa0: 7569 636b 5f73 6574 7570 3a20 2762 6c5f  uick_setup: 'bl_
+00353ab0: 6f70 6572 6174 6f72 732e 776d 2e57 4d5f  operators.wm.WM_
+00353ac0: 4d54 5f73 706c 6173 685f 7175 6963 6b5f  MT_splash_quick_
+00353ad0: 7365 7475 7027 203d 204e 6f6e 650a 0a57  setup' = None..W
+00353ae0: 4d5f 4d54 5f74 6f6f 6c73 7973 7465 6d5f  M_MT_toolsystem_
+00353af0: 7375 626d 656e 753a 2027 626c 5f75 692e  submenu: 'bl_ui.
+00353b00: 7370 6163 655f 746f 6f6c 7379 7374 656d  space_toolsystem
+00353b10: 5f63 6f6d 6d6f 6e2e 574d 5f4d 545f 746f  _common.WM_MT_to
+00353b20: 6f6c 7379 7374 656d 5f73 7562 6d65 6e75  olsystem_submenu
+00353b30: 2720 3d20 4e6f 6e65 0a0a 574d 5f4f 545f  ' = None..WM_OT_
+00353b40: 6261 7463 685f 7265 6e61 6d65 3a20 2762  batch_rename: 'b
+00353b50: 6c5f 6f70 6572 6174 6f72 732e 776d 2e57  l_operators.wm.W
+00353b60: 4d5f 4f54 5f62 6174 6368 5f72 656e 616d  M_OT_batch_renam
+00353b70: 6527 203d 204e 6f6e 650a 0a57 4d5f 4f54  e' = None..WM_OT
+00353b80: 5f62 6c65 6e64 5f73 7472 696e 6773 5f75  _blend_strings_u
+00353b90: 7466 385f 7661 6c69 6461 7465 3a20 2762  tf8_validate: 'b
+00353ba0: 6c5f 6f70 6572 6174 6f72 732e 6669 6c65  l_operators.file
+00353bb0: 2e57 4d5f 4f54 5f62 6c65 6e64 5f73 7472  .WM_OT_blend_str
+00353bc0: 696e 6773 5f75 7466 385f 7661 6c69 6461  ings_utf8_valida
+00353bd0: 7465 2720 3d20 4e6f 6e65 0a0a 574d 5f4f  te' = None..WM_O
+00353be0: 545f 636f 6e74 6578 745f 636f 6c6c 6563  T_context_collec
+00353bf0: 7469 6f6e 5f62 6f6f 6c65 616e 5f73 6574  tion_boolean_set
+00353c00: 3a20 2762 6c5f 6f70 6572 6174 6f72 732e  : 'bl_operators.
+00353c10: 776d 2e57 4d5f 4f54 5f63 6f6e 7465 7874  wm.WM_OT_context
+00353c20: 5f63 6f6c 6c65 6374 696f 6e5f 626f 6f6c  _collection_bool
+00353c30: 6561 6e5f 7365 7427 203d 204e 6f6e 650a  ean_set' = None.
+00353c40: 0a57 4d5f 4f54 5f63 6f6e 7465 7874 5f63  .WM_OT_context_c
+00353c50: 7963 6c65 5f61 7272 6179 3a20 2762 6c5f  ycle_array: 'bl_
+00353c60: 6f70 6572 6174 6f72 732e 776d 2e57 4d5f  operators.wm.WM_
+00353c70: 4f54 5f63 6f6e 7465 7874 5f63 7963 6c65  OT_context_cycle
+00353c80: 5f61 7272 6179 2720 3d20 4e6f 6e65 0a0a  _array' = None..
+00353c90: 574d 5f4f 545f 636f 6e74 6578 745f 6379  WM_OT_context_cy
+00353ca0: 636c 655f 656e 756d 3a20 2762 6c5f 6f70  cle_enum: 'bl_op
+00353cb0: 6572 6174 6f72 732e 776d 2e57 4d5f 4f54  erators.wm.WM_OT
+00353cc0: 5f63 6f6e 7465 7874 5f63 7963 6c65 5f65  _context_cycle_e
+00353cd0: 6e75 6d27 203d 204e 6f6e 650a 0a57 4d5f  num' = None..WM_
+00353ce0: 4f54 5f63 6f6e 7465 7874 5f63 7963 6c65  OT_context_cycle
+00353cf0: 5f69 6e74 3a20 2762 6c5f 6f70 6572 6174  _int: 'bl_operat
+00353d00: 6f72 732e 776d 2e57 4d5f 4f54 5f63 6f6e  ors.wm.WM_OT_con
+00353d10: 7465 7874 5f63 7963 6c65 5f69 6e74 2720  text_cycle_int' 
+00353d20: 3d20 4e6f 6e65 0a0a 574d 5f4f 545f 636f  = None..WM_OT_co
+00353d30: 6e74 6578 745f 6d65 6e75 5f65 6e75 6d3a  ntext_menu_enum:
+00353d40: 2027 626c 5f6f 7065 7261 746f 7273 2e77   'bl_operators.w
+00353d50: 6d2e 574d 5f4f 545f 636f 6e74 6578 745f  m.WM_OT_context_
+00353d60: 6d65 6e75 5f65 6e75 6d27 203d 204e 6f6e  menu_enum' = Non
+00353d70: 650a 0a57 4d5f 4f54 5f63 6f6e 7465 7874  e..WM_OT_context
+00353d80: 5f6d 6f64 616c 5f6d 6f75 7365 3a20 2762  _modal_mouse: 'b
+00353d90: 6c5f 6f70 6572 6174 6f72 732e 776d 2e57  l_operators.wm.W
+00353da0: 4d5f 4f54 5f63 6f6e 7465 7874 5f6d 6f64  M_OT_context_mod
+00353db0: 616c 5f6d 6f75 7365 2720 3d20 4e6f 6e65  al_mouse' = None
+00353dc0: 0a0a 574d 5f4f 545f 636f 6e74 6578 745f  ..WM_OT_context_
+00353dd0: 7069 655f 656e 756d 3a20 2762 6c5f 6f70  pie_enum: 'bl_op
+00353de0: 6572 6174 6f72 732e 776d 2e57 4d5f 4f54  erators.wm.WM_OT
+00353df0: 5f63 6f6e 7465 7874 5f70 6965 5f65 6e75  _context_pie_enu
+00353e00: 6d27 203d 204e 6f6e 650a 0a57 4d5f 4f54  m' = None..WM_OT
+00353e10: 5f63 6f6e 7465 7874 5f73 6361 6c65 5f66  _context_scale_f
+00353e20: 6c6f 6174 3a20 2762 6c5f 6f70 6572 6174  loat: 'bl_operat
+00353e30: 6f72 732e 776d 2e57 4d5f 4f54 5f63 6f6e  ors.wm.WM_OT_con
+00353e40: 7465 7874 5f73 6361 6c65 5f66 6c6f 6174  text_scale_float
+00353e50: 2720 3d20 4e6f 6e65 0a0a 574d 5f4f 545f  ' = None..WM_OT_
+00353e60: 636f 6e74 6578 745f 7363 616c 655f 696e  context_scale_in
+00353e70: 743a 2027 626c 5f6f 7065 7261 746f 7273  t: 'bl_operators
+00353e80: 2e77 6d2e 574d 5f4f 545f 636f 6e74 6578  .wm.WM_OT_contex
+00353e90: 745f 7363 616c 655f 696e 7427 203d 204e  t_scale_int' = N
+00353ea0: 6f6e 650a 0a57 4d5f 4f54 5f63 6f6e 7465  one..WM_OT_conte
+00353eb0: 7874 5f73 6574 5f62 6f6f 6c65 616e 3a20  xt_set_boolean: 
+00353ec0: 2762 6c5f 6f70 6572 6174 6f72 732e 776d  'bl_operators.wm
+00353ed0: 2e57 4d5f 4f54 5f63 6f6e 7465 7874 5f73  .WM_OT_context_s
+00353ee0: 6574 5f62 6f6f 6c65 616e 2720 3d20 4e6f  et_boolean' = No
+00353ef0: 6e65 0a0a 574d 5f4f 545f 636f 6e74 6578  ne..WM_OT_contex
+00353f00: 745f 7365 745f 656e 756d 3a20 2762 6c5f  t_set_enum: 'bl_
+00353f10: 6f70 6572 6174 6f72 732e 776d 2e57 4d5f  operators.wm.WM_
+00353f20: 4f54 5f63 6f6e 7465 7874 5f73 6574 5f65  OT_context_set_e
+00353f30: 6e75 6d27 203d 204e 6f6e 650a 0a57 4d5f  num' = None..WM_
+00353f40: 4f54 5f63 6f6e 7465 7874 5f73 6574 5f66  OT_context_set_f
+00353f50: 6c6f 6174 3a20 2762 6c5f 6f70 6572 6174  loat: 'bl_operat
+00353f60: 6f72 732e 776d 2e57 4d5f 4f54 5f63 6f6e  ors.wm.WM_OT_con
+00353f70: 7465 7874 5f73 6574 5f66 6c6f 6174 2720  text_set_float' 
+00353f80: 3d20 4e6f 6e65 0a0a 574d 5f4f 545f 636f  = None..WM_OT_co
+00353f90: 6e74 6578 745f 7365 745f 6964 3a20 2762  ntext_set_id: 'b
+00353fa0: 6c5f 6f70 6572 6174 6f72 732e 776d 2e57  l_operators.wm.W
+00353fb0: 4d5f 4f54 5f63 6f6e 7465 7874 5f73 6574  M_OT_context_set
+00353fc0: 5f69 6427 203d 204e 6f6e 650a 0a57 4d5f  _id' = None..WM_
+00353fd0: 4f54 5f63 6f6e 7465 7874 5f73 6574 5f69  OT_context_set_i
+00353fe0: 6e74 3a20 2762 6c5f 6f70 6572 6174 6f72  nt: 'bl_operator
+00353ff0: 732e 776d 2e57 4d5f 4f54 5f63 6f6e 7465  s.wm.WM_OT_conte
+00354000: 7874 5f73 6574 5f69 6e74 2720 3d20 4e6f  xt_set_int' = No
+00354010: 6e65 0a0a 574d 5f4f 545f 636f 6e74 6578  ne..WM_OT_contex
+00354020: 745f 7365 745f 7374 7269 6e67 3a20 2762  t_set_string: 'b
+00354030: 6c5f 6f70 6572 6174 6f72 732e 776d 2e57  l_operators.wm.W
+00354040: 4d5f 4f54 5f63 6f6e 7465 7874 5f73 6574  M_OT_context_set
+00354050: 5f73 7472 696e 6727 203d 204e 6f6e 650a  _string' = None.
+00354060: 0a57 4d5f 4f54 5f63 6f6e 7465 7874 5f73  .WM_OT_context_s
+00354070: 6574 5f76 616c 7565 3a20 2762 6c5f 6f70  et_value: 'bl_op
+00354080: 6572 6174 6f72 732e 776d 2e57 4d5f 4f54  erators.wm.WM_OT
+00354090: 5f63 6f6e 7465 7874 5f73 6574 5f76 616c  _context_set_val
+003540a0: 7565 2720 3d20 4e6f 6e65 0a0a 574d 5f4f  ue' = None..WM_O
+003540b0: 545f 636f 6e74 6578 745f 746f 6767 6c65  T_context_toggle
+003540c0: 3a20 2762 6c5f 6f70 6572 6174 6f72 732e  : 'bl_operators.
+003540d0: 776d 2e57 4d5f 4f54 5f63 6f6e 7465 7874  wm.WM_OT_context
+003540e0: 5f74 6f67 676c 6527 203d 204e 6f6e 650a  _toggle' = None.
+003540f0: 0a57 4d5f 4f54 5f63 6f6e 7465 7874 5f74  .WM_OT_context_t
+00354100: 6f67 676c 655f 656e 756d 3a20 2762 6c5f  oggle_enum: 'bl_
+00354110: 6f70 6572 6174 6f72 732e 776d 2e57 4d5f  operators.wm.WM_
+00354120: 4f54 5f63 6f6e 7465 7874 5f74 6f67 676c  OT_context_toggl
+00354130: 655f 656e 756d 2720 3d20 4e6f 6e65 0a0a  e_enum' = None..
+00354140: 574d 5f4f 545f 646f 635f 7669 6577 3a20  WM_OT_doc_view: 
+00354150: 2762 6c5f 6f70 6572 6174 6f72 732e 776d  'bl_operators.wm
+00354160: 2e57 4d5f 4f54 5f64 6f63 5f76 6965 7727  .WM_OT_doc_view'
+00354170: 203d 204e 6f6e 650a 0a57 4d5f 4f54 5f64   = None..WM_OT_d
+00354180: 6f63 5f76 6965 775f 6d61 6e75 616c 3a20  oc_view_manual: 
+00354190: 2762 6c5f 6f70 6572 6174 6f72 732e 776d  'bl_operators.wm
+003541a0: 2e57 4d5f 4f54 5f64 6f63 5f76 6965 775f  .WM_OT_doc_view_
+003541b0: 6d61 6e75 616c 2720 3d20 4e6f 6e65 0a0a  manual' = None..
+003541c0: 574d 5f4f 545f 6472 6f70 5f62 6c65 6e64  WM_OT_drop_blend
+003541d0: 5f66 696c 653a 2027 626c 5f6f 7065 7261  _file: 'bl_opera
+003541e0: 746f 7273 2e77 6d2e 574d 5f4f 545f 6472  tors.wm.WM_OT_dr
+003541f0: 6f70 5f62 6c65 6e64 5f66 696c 6527 203d  op_blend_file' =
+00354200: 204e 6f6e 650a 0a57 4d5f 4f54 5f6f 7065   None..WM_OT_ope
+00354210: 7261 746f 725f 6368 6561 745f 7368 6565  rator_cheat_shee
+00354220: 743a 2027 626c 5f6f 7065 7261 746f 7273  t: 'bl_operators
+00354230: 2e77 6d2e 574d 5f4f 545f 6f70 6572 6174  .wm.WM_OT_operat
+00354240: 6f72 5f63 6865 6174 5f73 6865 6574 2720  or_cheat_sheet' 
+00354250: 3d20 4e6f 6e65 0a0a 574d 5f4f 545f 6f70  = None..WM_OT_op
+00354260: 6572 6174 6f72 5f70 6965 5f65 6e75 6d3a  erator_pie_enum:
+00354270: 2027 626c 5f6f 7065 7261 746f 7273 2e77   'bl_operators.w
+00354280: 6d2e 574d 5f4f 545f 6f70 6572 6174 6f72  m.WM_OT_operator
+00354290: 5f70 6965 5f65 6e75 6d27 203d 204e 6f6e  _pie_enum' = Non
+003542a0: 650a 0a57 4d5f 4f54 5f6f 776e 6572 5f64  e..WM_OT_owner_d
+003542b0: 6973 6162 6c65 3a20 2762 6c5f 6f70 6572  isable: 'bl_oper
+003542c0: 6174 6f72 732e 776d 2e57 4d5f 4f54 5f6f  ators.wm.WM_OT_o
+003542d0: 776e 6572 5f64 6973 6162 6c65 2720 3d20  wner_disable' = 
+003542e0: 4e6f 6e65 0a0a 574d 5f4f 545f 6f77 6e65  None..WM_OT_owne
+003542f0: 725f 656e 6162 6c65 3a20 2762 6c5f 6f70  r_enable: 'bl_op
+00354300: 6572 6174 6f72 732e 776d 2e57 4d5f 4f54  erators.wm.WM_OT
+00354310: 5f6f 776e 6572 5f65 6e61 626c 6527 203d  _owner_enable' =
+00354320: 204e 6f6e 650a 0a57 4d5f 4f54 5f70 6174   None..WM_OT_pat
+00354330: 685f 6f70 656e 3a20 2762 6c5f 6f70 6572  h_open: 'bl_oper
+00354340: 6174 6f72 732e 776d 2e57 4d5f 4f54 5f70  ators.wm.WM_OT_p
+00354350: 6174 685f 6f70 656e 2720 3d20 4e6f 6e65  ath_open' = None
+00354360: 0a0a 574d 5f4f 545f 7072 6576 6965 7773  ..WM_OT_previews
+00354370: 5f62 6174 6368 5f63 6c65 6172 3a20 2762  _batch_clear: 'b
+00354380: 6c5f 6f70 6572 6174 6f72 732e 6669 6c65  l_operators.file
+00354390: 2e57 4d5f 4f54 5f70 7265 7669 6577 735f  .WM_OT_previews_
+003543a0: 6261 7463 685f 636c 6561 7227 203d 204e  batch_clear' = N
+003543b0: 6f6e 650a 0a57 4d5f 4f54 5f70 7265 7669  one..WM_OT_previ
+003543c0: 6577 735f 6261 7463 685f 6765 6e65 7261  ews_batch_genera
+003543d0: 7465 3a20 2762 6c5f 6f70 6572 6174 6f72  te: 'bl_operator
+003543e0: 732e 6669 6c65 2e57 4d5f 4f54 5f70 7265  s.file.WM_OT_pre
+003543f0: 7669 6577 735f 6261 7463 685f 6765 6e65  views_batch_gene
+00354400: 7261 7465 2720 3d20 4e6f 6e65 0a0a 574d  rate' = None..WM
+00354410: 5f4f 545f 7072 6f70 6572 7469 6573 5f61  _OT_properties_a
+00354420: 6464 3a20 2762 6c5f 6f70 6572 6174 6f72  dd: 'bl_operator
+00354430: 732e 776d 2e57 4d5f 4f54 5f70 726f 7065  s.wm.WM_OT_prope
+00354440: 7274 6965 735f 6164 6427 203d 204e 6f6e  rties_add' = Non
+00354450: 650a 0a57 4d5f 4f54 5f70 726f 7065 7274  e..WM_OT_propert
+00354460: 6965 735f 636f 6e74 6578 745f 6368 616e  ies_context_chan
+00354470: 6765 3a20 2762 6c5f 6f70 6572 6174 6f72  ge: 'bl_operator
+00354480: 732e 776d 2e57 4d5f 4f54 5f70 726f 7065  s.wm.WM_OT_prope
+00354490: 7274 6965 735f 636f 6e74 6578 745f 6368  rties_context_ch
+003544a0: 616e 6765 2720 3d20 4e6f 6e65 0a0a 574d  ange' = None..WM
+003544b0: 5f4f 545f 7072 6f70 6572 7469 6573 5f65  _OT_properties_e
+003544c0: 6469 743a 2027 626c 5f6f 7065 7261 746f  dit: 'bl_operato
+003544d0: 7273 2e77 6d2e 574d 5f4f 545f 7072 6f70  rs.wm.WM_OT_prop
+003544e0: 6572 7469 6573 5f65 6469 7427 203d 204e  erties_edit' = N
+003544f0: 6f6e 650a 0a57 4d5f 4f54 5f70 726f 7065  one..WM_OT_prope
+00354500: 7274 6965 735f 6564 6974 5f76 616c 7565  rties_edit_value
+00354510: 3a20 2762 6c5f 6f70 6572 6174 6f72 732e  : 'bl_operators.
+00354520: 776d 2e57 4d5f 4f54 5f70 726f 7065 7274  wm.WM_OT_propert
+00354530: 6965 735f 6564 6974 5f76 616c 7565 2720  ies_edit_value' 
+00354540: 3d20 4e6f 6e65 0a0a 574d 5f4f 545f 7072  = None..WM_OT_pr
+00354550: 6f70 6572 7469 6573 5f72 656d 6f76 653a  operties_remove:
+00354560: 2027 626c 5f6f 7065 7261 746f 7273 2e77   'bl_operators.w
+00354570: 6d2e 574d 5f4f 545f 7072 6f70 6572 7469  m.WM_OT_properti
+00354580: 6573 5f72 656d 6f76 6527 203d 204e 6f6e  es_remove' = Non
+00354590: 650a 0a57 4d5f 4f54 5f73 7973 696e 666f  e..WM_OT_sysinfo
+003545a0: 3a20 2762 6c5f 6f70 6572 6174 6f72 732e  : 'bl_operators.
+003545b0: 776d 2e57 4d5f 4f54 5f73 7973 696e 666f  wm.WM_OT_sysinfo
+003545c0: 2720 3d20 4e6f 6e65 0a0a 574d 5f4f 545f  ' = None..WM_OT_
+003545d0: 746f 6f6c 5f73 6574 5f62 795f 6964 3a20  tool_set_by_id: 
+003545e0: 2762 6c5f 6f70 6572 6174 6f72 732e 776d  'bl_operators.wm
+003545f0: 2e57 4d5f 4f54 5f74 6f6f 6c5f 7365 745f  .WM_OT_tool_set_
+00354600: 6279 5f69 6427 203d 204e 6f6e 650a 0a57  by_id' = None..W
+00354610: 4d5f 4f54 5f74 6f6f 6c5f 7365 745f 6279  M_OT_tool_set_by
+00354620: 5f69 6e64 6578 3a20 2762 6c5f 6f70 6572  _index: 'bl_oper
+00354630: 6174 6f72 732e 776d 2e57 4d5f 4f54 5f74  ators.wm.WM_OT_t
+00354640: 6f6f 6c5f 7365 745f 6279 5f69 6e64 6578  ool_set_by_index
+00354650: 2720 3d20 4e6f 6e65 0a0a 574d 5f4f 545f  ' = None..WM_OT_
+00354660: 746f 6f6c 6261 723a 2027 626c 5f6f 7065  toolbar: 'bl_ope
+00354670: 7261 746f 7273 2e77 6d2e 574d 5f4f 545f  rators.wm.WM_OT_
+00354680: 746f 6f6c 6261 7227 203d 204e 6f6e 650a  toolbar' = None.
+00354690: 0a57 4d5f 4f54 5f74 6f6f 6c62 6172 5f66  .WM_OT_toolbar_f
+003546a0: 616c 6c62 6163 6b5f 7069 653a 2027 626c  allback_pie: 'bl
+003546b0: 5f6f 7065 7261 746f 7273 2e77 6d2e 574d  _operators.wm.WM
+003546c0: 5f4f 545f 746f 6f6c 6261 725f 6661 6c6c  _OT_toolbar_fall
+003546d0: 6261 636b 5f70 6965 2720 3d20 4e6f 6e65  back_pie' = None
+003546e0: 0a0a 574d 5f4f 545f 746f 6f6c 6261 725f  ..WM_OT_toolbar_
+003546f0: 7072 6f6d 7074 3a20 2762 6c5f 6f70 6572  prompt: 'bl_oper
+00354700: 6174 6f72 732e 776d 2e57 4d5f 4f54 5f74  ators.wm.WM_OT_t
+00354710: 6f6f 6c62 6172 5f70 726f 6d70 7427 203d  oolbar_prompt' =
+00354720: 204e 6f6e 650a 0a57 4d5f 4f54 5f75 726c   None..WM_OT_url
+00354730: 5f6f 7065 6e3a 2027 626c 5f6f 7065 7261  _open: 'bl_opera
+00354740: 746f 7273 2e77 6d2e 574d 5f4f 545f 7572  tors.wm.WM_OT_ur
+00354750: 6c5f 6f70 656e 2720 3d20 4e6f 6e65 0a0a  l_open' = None..
+00354760: 574d 5f4f 545f 7572 6c5f 6f70 656e 5f70  WM_OT_url_open_p
+00354770: 7265 7365 743a 2027 626c 5f6f 7065 7261  reset: 'bl_opera
+00354780: 746f 7273 2e77 6d2e 574d 5f4f 545f 7572  tors.wm.WM_OT_ur
+00354790: 6c5f 6f70 656e 5f70 7265 7365 7427 203d  l_open_preset' =
+003547a0: 204e 6f6e 650a 0a57 4f52 4b53 5041 4345   None..WORKSPACE
+003547b0: 5f50 545f 6164 646f 6e73 3a20 2762 6c5f  _PT_addons: 'bl_
+003547c0: 7569 2e70 726f 7065 7274 6965 735f 776f  ui.properties_wo
+003547d0: 726b 7370 6163 652e 574f 524b 5350 4143  rkspace.WORKSPAC
+003547e0: 455f 5054 5f61 6464 6f6e 7327 203d 204e  E_PT_addons' = N
+003547f0: 6f6e 650a 0a57 4f52 4b53 5041 4345 5f50  one..WORKSPACE_P
+00354800: 545f 6375 7374 6f6d 5f70 726f 7073 3a20  T_custom_props: 
+00354810: 2762 6c5f 7569 2e70 726f 7065 7274 6965  'bl_ui.propertie
+00354820: 735f 776f 726b 7370 6163 652e 574f 524b  s_workspace.WORK
+00354830: 5350 4143 455f 5054 5f63 7573 746f 6d5f  SPACE_PT_custom_
+00354840: 7072 6f70 7327 203d 204e 6f6e 650a 0a57  props' = None..W
+00354850: 4f52 4b53 5041 4345 5f50 545f 6d61 696e  ORKSPACE_PT_main
+00354860: 3a20 2762 6c5f 7569 2e70 726f 7065 7274  : 'bl_ui.propert
+00354870: 6965 735f 776f 726b 7370 6163 652e 574f  ies_workspace.WO
+00354880: 524b 5350 4143 455f 5054 5f6d 6169 6e27  RKSPACE_PT_main'
+00354890: 203d 204e 6f6e 650a 0a57 4f52 4c44 5f50   = None..WORLD_P
+003548a0: 545f 636f 6e74 6578 745f 776f 726c 643a  T_context_world:
+003548b0: 2027 626c 5f75 692e 7072 6f70 6572 7469   'bl_ui.properti
+003548c0: 6573 5f77 6f72 6c64 2e57 4f52 4c44 5f50  es_world.WORLD_P
+003548d0: 545f 636f 6e74 6578 745f 776f 726c 6427  T_context_world'
+003548e0: 203d 204e 6f6e 650a 0a57 4f52 4c44 5f50   = None..WORLD_P
+003548f0: 545f 6375 7374 6f6d 5f70 726f 7073 3a20  T_custom_props: 
+00354900: 2762 6c5f 7569 2e70 726f 7065 7274 6965  'bl_ui.propertie
+00354910: 735f 776f 726c 642e 574f 524c 445f 5054  s_world.WORLD_PT
+00354920: 5f63 7573 746f 6d5f 7072 6f70 7327 203d  _custom_props' =
+00354930: 204e 6f6e 650a 0a57 4f52 4c44 5f50 545f   None..WORLD_PT_
+00354940: 7669 6577 706f 7274 5f64 6973 706c 6179  viewport_display
+00354950: 3a20 2762 6c5f 7569 2e70 726f 7065 7274  : 'bl_ui.propert
+00354960: 6965 735f 776f 726c 642e 574f 524c 445f  ies_world.WORLD_
+00354970: 5054 5f76 6965 7770 6f72 745f 6469 7370  PT_viewport_disp
+00354980: 6c61 7927 203d 204e 6f6e 650a            lay' = None.
```

### Comparing `fake-bpy-module-latest-20230621/bpy/utils/__init__.py` & `fake-bpy-module-latest-20230622/bpy/utils/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import sys
 import typing
 import bpy.types
 
-from . import previews
 from . import units
+from . import previews
 
 GenericType = typing.TypeVar("GenericType")
 
 
 def app_template_paths(*, path: typing.Optional[str] = None) -> typing.Any:
     ''' Returns valid application template paths.
```

### Comparing `fake-bpy-module-latest-20230621/bpy/utils/previews.py` & `fake-bpy-module-latest-20230622/bpy/utils/previews.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bpy/utils/units.py` & `fake-bpy-module-latest-20230622/bpy/utils/units.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bpy_extras/anim_utils.py` & `fake-bpy-module-latest-20230622/bpy_extras/anim_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,16 +108,16 @@
     '''
 
     pass
 
 
 def bake_action_objects_iter(
         object_action_pairs: typing.
-        Union['bpy.types.Object', 'bpy.types.Action', 'bpy.types.Sequence'],
+        Union['bpy.types.Action', 'bpy.types.Sequence', 'bpy.types.Object'],
         **kwargs):
     ''' An coroutine that bakes actions for multiple objects.
 
     :param object_action_pairs: Sequence of object action tuples, action is the destination for the baked data. When None a new action will be created.
-    :type object_action_pairs: typing.Union['bpy.types.Object', 'bpy.types.Action', 'bpy.types.Sequence']
+    :type object_action_pairs: typing.Union['bpy.types.Action', 'bpy.types.Sequence', 'bpy.types.Object']
     '''
 
     pass
```

### Comparing `fake-bpy-module-latest-20230621/bpy_extras/image_utils.py` & `fake-bpy-module-latest-20230622/bpy_extras/image_utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bpy_extras/io_utils.py` & `fake-bpy-module-latest-20230622/bpy_extras/io_utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bpy_extras/mesh_utils.py` & `fake-bpy-module-latest-20230622/bpy_extras/mesh_utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bpy_extras/node_shader_utils.py` & `fake-bpy-module-latest-20230622/bpy_extras/node_shader_utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bpy_extras/object_utils.py` & `fake-bpy-module-latest-20230622/bpy_extras/object_utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bpy_extras/view3d_utils.py` & `fake-bpy-module-latest-20230622/bpy_extras/view3d_utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bpy_extras/wm_utils/progress_report.py` & `fake-bpy-module-latest-20230622/bpy_extras/wm_utils/progress_report.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/bpy_types.py` & `fake-bpy-module-latest-20230622/bpy_types.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/fake_bpy_module_latest.egg-info/PKG-INFO` & `fake-bpy-module-latest-20230622/fake_bpy_module_latest.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: fake-bpy-module-latest
-Version: 20230621
+Version: 20230622
 Summary: Collection of the fake Blender Python API module for the code completion.
 Home-page: https://github.com/nutti/fake-bpy-module
 Author: nutti
 Author-email: nutti.metro@gmail.com
 Maintainer: nutti
 Maintainer-email: nutti.metro@gmail.com
 License: MIT
```

### Comparing `fake-bpy-module-latest-20230621/fake_bpy_module_latest.egg-info/SOURCES.txt` & `fake-bpy-module-latest-20230622/fake_bpy_module_latest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/freestyle/chainingiterators.py` & `fake-bpy-module-latest-20230622/freestyle/chainingiterators.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/freestyle/functions.py` & `fake-bpy-module-latest-20230622/freestyle/functions.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/freestyle/predicates.py` & `fake-bpy-module-latest-20230622/freestyle/predicates.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/freestyle/shaders.py` & `fake-bpy-module-latest-20230622/freestyle/shaders.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/freestyle/types.py` & `fake-bpy-module-latest-20230622/freestyle/types.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/freestyle/utils/ContextFunctions.py` & `fake-bpy-module-latest-20230622/freestyle/utils/ContextFunctions.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/freestyle/utils/__init__.py` & `fake-bpy-module-latest-20230622/freestyle/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/gpu/capabilities.py` & `fake-bpy-module-latest-20230622/gpu/capabilities.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/gpu/matrix.py` & `fake-bpy-module-latest-20230622/gpu/matrix.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/gpu/platform.py` & `fake-bpy-module-latest-20230622/gpu/platform.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/gpu/shader.py` & `fake-bpy-module-latest-20230622/gpu/shader.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/gpu/state.py` & `fake-bpy-module-latest-20230622/gpu/state.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/gpu/texture.py` & `fake-bpy-module-latest-20230622/gpu/texture.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/gpu/types.py` & `fake-bpy-module-latest-20230622/gpu/types.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/gpu_extras/batch.py` & `fake-bpy-module-latest-20230622/gpu_extras/batch.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/gpu_extras/presets.py` & `fake-bpy-module-latest-20230622/gpu_extras/presets.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/idprop/types.py` & `fake-bpy-module-latest-20230622/idprop/types.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/imbuf/__init__.py` & `fake-bpy-module-latest-20230622/imbuf/__init__.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/imbuf/types.py` & `fake-bpy-module-latest-20230622/imbuf/types.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/keyingsets_builtins.py` & `fake-bpy-module-latest-20230622/keyingsets_builtins.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/keyingsets_utils.py` & `fake-bpy-module-latest-20230622/keyingsets_utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/mathutils/__init__.py` & `fake-bpy-module-latest-20230622/mathutils/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import sys
 import typing
+from . import geometry
 from . import kdtree
 from . import noise
-from . import bvhtree
 from . import interpolate
-from . import geometry
+from . import bvhtree
 
 GenericType = typing.TypeVar("GenericType")
 
 
 class Color:
     ''' This object gives access to Colors in Blender. Most colors returned by Blender APIs are in scene linear color space, as defined by the OpenColorIO configuration. The notable exception is user interface theming colors, which are in sRGB color space. :arg rgb: (r, g, b) color values :type rgb: 3d vector
     '''
```

### Comparing `fake-bpy-module-latest-20230621/mathutils/bvhtree.py` & `fake-bpy-module-latest-20230622/mathutils/bvhtree.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/mathutils/geometry.py` & `fake-bpy-module-latest-20230622/mathutils/geometry.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/mathutils/kdtree.py` & `fake-bpy-module-latest-20230622/mathutils/kdtree.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/mathutils/noise.py` & `fake-bpy-module-latest-20230622/mathutils/noise.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/nodeitems_builtins.py` & `fake-bpy-module-latest-20230622/nodeitems_builtins.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/nodeitems_utils.py` & `fake-bpy-module-latest-20230622/nodeitems_utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/rna_info.py` & `fake-bpy-module-latest-20230622/rna_info.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/rna_keymap_ui.py` & `fake-bpy-module-latest-20230622/rna_keymap_ui.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/rna_prop_ui.py` & `fake-bpy-module-latest-20230622/rna_prop_ui.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/rna_xml.py` & `fake-bpy-module-latest-20230622/rna_xml.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230621/setup.py` & `fake-bpy-module-latest-20230622/setup.py`

 * *Files identical despite different names*

