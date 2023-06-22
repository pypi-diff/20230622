# Comparing `tmp/nerfstudio-0.3.1.tar.gz` & `tmp/nerfstudio-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nerfstudio-0.3.1.tar", last modified: Mon May 22 17:46:49 2023, max compression
+gzip compressed data, was "nerfstudio-0.3.2.tar", last modified: Thu Jun 22 16:29:28 2023, max compression
```

## Comparing `nerfstudio-0.3.1.tar` & `nerfstudio-0.3.2.tar`

### file list

```diff
@@ -1,241 +1,243 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:46:49.570284 nerfstudio-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19536 2023-05-22 17:46:49.570284 nerfstudio-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19115 2023-05-22 17:46:42.000000 nerfstudio-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:46:49.542284 nerfstudio-0.3.1/nerfstudio/
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:46:49.546284 nerfstudio-0.3.1/nerfstudio/cameras/
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/cameras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/cameras/camera_optimizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6146 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/cameras/camera_paths.py
--rw-r--r--   0 runner    (1001) docker     (123)    22947 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/cameras/camera_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    41172 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/cameras/cameras.py
--rw-r--r--   0 runner    (1001) docker     (123)     4790 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/cameras/lie_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)    11014 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/cameras/rays.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:46:49.546284 nerfstudio-0.3.1/nerfstudio/configs/
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/configs/base_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/configs/config_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/configs/dataparser_configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5218 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/configs/experiment_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/configs/external_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)    24040 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/configs/method_configs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:46:49.546284 nerfstudio-0.3.1/nerfstudio/data/
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:46:49.546284 nerfstudio-0.3.1/nerfstudio/data/datamanagers/
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/data/datamanagers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22616 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/data/datamanagers/base_datamanager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:46:49.546284 nerfstudio-0.3.1/nerfstudio/data/dataparsers/
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/data/dataparsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9203 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/data/dataparsers/arkitscenes_dataparser.py
--rw-r--r--   0 runner    (1001) docker     (123)     7332 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/data/dataparsers/base_dataparser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/data/dataparsers/blender_dataparser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/data/dataparsers/dnerf_dataparser.py
--rw-r--r--   0 runner    (1001) docker     (123)    13637 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/data/dataparsers/dycheck_dataparser.py
--rw-r--r--   0 runner    (1001) docker     (123)     6826 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/data/dataparsers/instant_ngp_dataparser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/data/dataparsers/minimal_dataparser.py
--rw-r--r--   0 runner    (1001) docker     (123)     8519 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/data/dataparsers/nerfosr_dataparser.py
--rw-r--r--   0 runner    (1001) docker     (123)    14785 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/data/dataparsers/nerfstudio_dataparser.py
--rw-r--r--   0 runner    (1001) docker     (123)     8629 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/data/dataparsers/nuscenes_dataparser.py
--rw-r--r--   0 runner    (1001) docker     (123)     6987 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/data/dataparsers/phototourism_dataparser.py
--rw-r--r--   0 runner    (1001) docker     (123)     6805 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/data/dataparsers/scannet_dataparser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5732 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/data/dataparsers/sdfstudio_dataparser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5984 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/data/dataparsers/sitcoms3d_dataparser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:46:49.550284 nerfstudio-0.3.1/nerfstudio/data/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/data/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5056 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/data/datasets/base_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/data/datasets/depth_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/data/datasets/sdf_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/data/datasets/semantic_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    12600 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/data/pixel_samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/data/scene_box.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:46:49.550284 nerfstudio-0.3.1/nerfstudio/data/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/data/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20474 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/data/utils/colmap_parsing_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/data/utils/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8836 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/data/utils/dataloaders.py
--rw-r--r--   0 runner    (1001) docker     (123)     9476 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/data/utils/nerfstudio_collate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:46:49.550284 nerfstudio-0.3.1/nerfstudio/engine/
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/engine/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)     5898 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/engine/optimizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/engine/schedulers.py
--rw-r--r--   0 runner    (1001) docker     (123)    22239 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/engine/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:46:49.550284 nerfstudio-0.3.1/nerfstudio/exporter/
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/exporter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12333 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/exporter/exporter_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10659 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/exporter/marching_cubes.py
--rw-r--r--   0 runner    (1001) docker     (123)    20982 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/exporter/texture_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14061 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/exporter/tsdf_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:46:49.550284 nerfstudio-0.3.1/nerfstudio/field_components/
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/field_components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/field_components/activations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/field_components/base_field_component.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:46:49.554284 nerfstudio-0.3.1/nerfstudio/field_components/cuda/
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/field_components/cuda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/field_components/cuda/_backend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:46:49.554284 nerfstudio-0.3.1/nerfstudio/field_components/cuda/csrc/
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/field_components/cuda/csrc/pybind.cu
--rw-r--r--   0 runner    (1001) docker     (123)    25118 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/field_components/cuda/csrc/temporal_gridencoder.cu
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/field_components/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)    26803 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/field_components/encodings.py
--rw-r--r--   0 runner    (1001) docker     (123)     6935 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/field_components/field_heads.py
--rw-r--r--   0 runner    (1001) docker     (123)     3698 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/field_components/mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/field_components/spatial_distortions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/field_components/temporal_distortions.py
--rw-r--r--   0 runner    (1001) docker     (123)    16465 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/field_components/temporal_grid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:46:49.554284 nerfstudio-0.3.1/nerfstudio/fields/
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/fields/base_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     4931 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/fields/density_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     8010 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/fields/instant_ngp_field.py
--rw-r--r--   0 runner    (1001) docker     (123)    17976 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/fields/nerfacto_field.py
--rw-r--r--   0 runner    (1001) docker     (123)    17707 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/fields/nerfplayer_nerfacto_field.py
--rw-r--r--   0 runner    (1001) docker     (123)    10849 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/fields/nerfplayer_ngp_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/fields/nerfw_field.py
--rw-r--r--   0 runner    (1001) docker     (123)    18147 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/fields/sdf_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/fields/semantic_nerf_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/fields/tensorf_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/fields/vanilla_nerf_field.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:46:49.554284 nerfstudio-0.3.1/nerfstudio/generative/
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/generative/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12638 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/generative/stable_diffusion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:46:49.554284 nerfstudio-0.3.1/nerfstudio/model_components/
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/model_components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21440 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/model_components/losses.py
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/model_components/ray_generators.py
--rw-r--r--   0 runner    (1001) docker     (123)    29126 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/model_components/ray_samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)    12618 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/model_components/renderers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6776 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/model_components/scene_colliders.py
--rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/model_components/shaders.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:46:49.558284 nerfstudio-0.3.1/nerfstudio/models/
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8361 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/models/base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    16762 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/models/base_surface_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5558 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/models/depth_nerfacto.py
--rw-r--r--   0 runner    (1001) docker     (123)     9838 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/models/instant_ngp.py
--rw-r--r--   0 runner    (1001) docker     (123)     8339 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/models/mipnerf.py
--rw-r--r--   0 runner    (1001) docker     (123)    16436 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/models/nerfacto.py
--rw-r--r--   0 runner    (1001) docker     (123)    11612 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/models/nerfplayer_nerfacto.py
--rw-r--r--   0 runner    (1001) docker     (123)    11898 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/models/nerfplayer_ngp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/models/neus.py
--rw-r--r--   0 runner    (1001) docker     (123)     9511 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/models/neus_facto.py
--rw-r--r--   0 runner    (1001) docker     (123)    13425 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/models/semantic_nerfw.py
--rw-r--r--   0 runner    (1001) docker     (123)    14365 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/models/tensorf.py
--rw-r--r--   0 runner    (1001) docker     (123)    10159 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/models/vanilla_nerf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:46:49.558284 nerfstudio-0.3.1/nerfstudio/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16647 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/pipelines/base_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/pipelines/dynamic_batch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:46:49.558284 nerfstudio-0.3.1/nerfstudio/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/plugins/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/plugins/registry_dataparser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/plugins/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:46:49.558284 nerfstudio-0.3.1/nerfstudio/process_data/
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/process_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/process_data/base_converter_to_nerfstudio_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     9661 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/process_data/colmap_converter_to_nerfstudio_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    24480 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/process_data/colmap_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8283 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/process_data/equirect_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5089 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/process_data/hloc_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/process_data/images_to_nerfstudio_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     7747 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/process_data/metashape_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9227 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/process_data/polycam_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    20456 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/process_data/process_data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4841 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/process_data/realitycapture_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/process_data/record3d_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4677 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/process_data/video_to_nerfstudio_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:46:49.562284 nerfstudio-0.3.1/nerfstudio/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/scripts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:46:49.562284 nerfstudio-0.3.1/nerfstudio/scripts/blender/
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/scripts/blender/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17246 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/scripts/blender/nerfstudio_blender.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:46:49.562284 nerfstudio-0.3.1/nerfstudio/scripts/completions/
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/scripts/completions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15549 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/scripts/completions/install.py
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/scripts/completions/setup.bash
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/scripts/completions/setup.zsh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:46:49.562284 nerfstudio-0.3.1/nerfstudio/scripts/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)     6544 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/scripts/datasets/process_nuscenes_masks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:46:49.562284 nerfstudio-0.3.1/nerfstudio/scripts/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/scripts/docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/scripts/docs/add_nb_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/scripts/docs/build_docs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:46:49.562284 nerfstudio-0.3.1/nerfstudio/scripts/downloads/
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/scripts/downloads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20378 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/scripts/downloads/download_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/scripts/eval.py
--rw-r--r--   0 runner    (1001) docker     (123)    18536 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/scripts/exporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:46:49.562284 nerfstudio-0.3.1/nerfstudio/scripts/github/
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/scripts/github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/scripts/github/run_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)    17084 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/scripts/process_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    18627 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/scripts/render.py
--rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/scripts/texture.py
--rw-r--r--   0 runner    (1001) docker     (123)     9460 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/scripts/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:46:49.562284 nerfstudio-0.3.1/nerfstudio/scripts/viewer/
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/scripts/viewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3927 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/scripts/viewer/run_viewer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/scripts/viewer/sync_viser_message_defs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:46:49.566284 nerfstudio-0.3.1/nerfstudio/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6976 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/utils/colormaps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/utils/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/utils/comms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4397 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/utils/eval_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/utils/install_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    11515 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/utils/math.py
--rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    16855 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/utils/plotly_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/utils/poses.py
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/utils/printing.py
--rw-r--r--   0 runner    (1001) docker     (123)     8012 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/utils/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/utils/rich_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/utils/scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)    13273 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/utils/tensor_dataclass.py
--rw-r--r--   0 runner    (1001) docker     (123)    17354 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/utils/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:46:49.566284 nerfstudio-0.3.1/nerfstudio/viewer/
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/viewer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:46:49.566284 nerfstudio-0.3.1/nerfstudio/viewer/app/
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/viewer/app/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:46:49.566284 nerfstudio-0.3.1/nerfstudio/viewer/app/public/
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/viewer/app/public/manifest.json
--rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/viewer/app/run_deploy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:46:49.542284 nerfstudio-0.3.1/nerfstudio/viewer/app/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:46:49.566284 nerfstudio-0.3.1/nerfstudio/viewer/app/src/themes/
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/viewer/app/src/themes/leva_theme.json
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/viewer/app/tsconfig.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:46:49.566284 nerfstudio-0.3.1/nerfstudio/viewer/server/
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/viewer/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14690 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/viewer/server/control_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/viewer/server/gui_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/viewer/server/path.py
--rw-r--r--   0 runner    (1001) docker     (123)    12040 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/viewer/server/render_state_machine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:46:49.566284 nerfstudio-0.3.1/nerfstudio/viewer/server/state/
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/viewer/server/state/node.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/viewer/server/state/state_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/viewer/server/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    18286 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/viewer/server/viewer_elements.py
--rw-r--r--   0 runner    (1001) docker     (123)    18597 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/viewer/server/viewer_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/viewer/server/viewer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:46:49.570284 nerfstudio-0.3.1/nerfstudio/viewer/viser/
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/viewer/viser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6437 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/viewer/viser/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)    21893 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/viewer/viser/message_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7353 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/viewer/viser/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/nerfstudio/viewer/viser/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:46:49.542284 nerfstudio-0.3.1/nerfstudio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19536 2023-05-22 17:46:49.000000 nerfstudio-0.3.1/nerfstudio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7540 2023-05-22 17:46:49.000000 nerfstudio-0.3.1/nerfstudio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 17:46:49.000000 nerfstudio-0.3.1/nerfstudio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-22 17:46:49.000000 nerfstudio-0.3.1/nerfstudio.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-05-22 17:46:49.000000 nerfstudio-0.3.1/nerfstudio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-22 17:46:49.000000 nerfstudio-0.3.1/nerfstudio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4945 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 17:46:49.570284 nerfstudio-0.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:46:49.570284 nerfstudio-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-05-22 17:46:34.000000 nerfstudio-0.3.1/tests/test_train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:28.096534 nerfstudio-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19581 2023-06-22 16:29:28.096534 nerfstudio-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19160 2023-06-22 16:29:19.000000 nerfstudio-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:28.056534 nerfstudio-0.3.2/nerfstudio/
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:28.060534 nerfstudio-0.3.2/nerfstudio/cameras/
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/cameras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/cameras/camera_optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6423 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/cameras/camera_paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22947 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/cameras/camera_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44827 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/cameras/cameras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4790 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/cameras/lie_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11014 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/cameras/rays.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:28.060534 nerfstudio-0.3.2/nerfstudio/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5638 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/configs/base_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/configs/config_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/configs/dataparser_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5448 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/configs/experiment_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6608 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/configs/external_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25119 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/configs/method_configs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:28.060534 nerfstudio-0.3.2/nerfstudio/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:28.060534 nerfstudio-0.3.2/nerfstudio/data/datamanagers/
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/data/datamanagers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23744 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/data/datamanagers/base_datamanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12052 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/data/datamanagers/random_cameras_datamanager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:28.064534 nerfstudio-0.3.2/nerfstudio/data/dataparsers/
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/data/dataparsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9203 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/data/dataparsers/arkitscenes_dataparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7518 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/data/dataparsers/base_dataparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/data/dataparsers/blender_dataparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/data/dataparsers/dnerf_dataparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13637 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/data/dataparsers/dycheck_dataparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6827 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/data/dataparsers/instant_ngp_dataparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/data/dataparsers/minimal_dataparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8519 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/data/dataparsers/nerfosr_dataparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14280 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/data/dataparsers/nerfstudio_dataparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8629 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/data/dataparsers/nuscenes_dataparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6987 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/data/dataparsers/phototourism_dataparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6849 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/data/dataparsers/scannet_dataparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5732 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/data/dataparsers/sdfstudio_dataparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5984 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/data/dataparsers/sitcoms3d_dataparser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:28.064534 nerfstudio-0.3.2/nerfstudio/data/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/data/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/data/datasets/base_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/data/datasets/depth_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/data/datasets/sdf_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/data/datasets/semantic_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12601 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/data/pixel_samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/data/scene_box.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:28.064534 nerfstudio-0.3.2/nerfstudio/data/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/data/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20474 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/data/utils/colmap_parsing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/data/utils/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9141 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/data/utils/dataloaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9840 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/data/utils/nerfstudio_collate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:28.068534 nerfstudio-0.3.2/nerfstudio/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/engine/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5898 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/engine/optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6170 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/engine/schedulers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23874 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/engine/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:28.068534 nerfstudio-0.3.2/nerfstudio/exporter/
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/exporter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12333 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/exporter/exporter_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10659 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/exporter/marching_cubes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20982 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/exporter/texture_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14061 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/exporter/tsdf_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:28.072534 nerfstudio-0.3.2/nerfstudio/field_components/
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/field_components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/field_components/activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/field_components/base_field_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/field_components/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28637 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/field_components/encodings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/field_components/field_heads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6800 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/field_components/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/field_components/spatial_distortions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/field_components/temporal_distortions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:28.072534 nerfstudio-0.3.2/nerfstudio/fields/
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/fields/base_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/fields/density_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6099 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/fields/generfacto_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8066 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/fields/instant_ngp_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13001 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/fields/nerfacto_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/fields/nerfw_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18147 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/fields/sdf_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/fields/semantic_nerf_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/fields/tensorf_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/fields/vanilla_nerf_field.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:28.072534 nerfstudio-0.3.2/nerfstudio/generative/
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/generative/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8743 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/generative/deepfloyd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5410 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/generative/positional_text_embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11747 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/generative/stable_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/generative/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:28.076534 nerfstudio-0.3.2/nerfstudio/model_components/
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/model_components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21445 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/model_components/losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/model_components/ray_generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29117 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/model_components/ray_samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12618 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/model_components/renderers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6675 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/model_components/scene_colliders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/model_components/shaders.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:28.076534 nerfstudio-0.3.2/nerfstudio/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8480 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/models/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16756 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/models/base_surface_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5574 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/models/depth_nerfacto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21923 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/models/generfacto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9826 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/models/instant_ngp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8339 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/models/mipnerf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17036 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/models/nerfacto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/models/neus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9511 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/models/neus_facto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13449 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/models/semantic_nerfw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14365 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/models/tensorf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10159 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/models/vanilla_nerf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:28.076534 nerfstudio-0.3.2/nerfstudio/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16904 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/pipelines/base_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/pipelines/dynamic_batch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:28.076534 nerfstudio-0.3.2/nerfstudio/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/plugins/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/plugins/registry_dataparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/plugins/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:28.080534 nerfstudio-0.3.2/nerfstudio/process_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/process_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/process_data/base_converter_to_nerfstudio_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9821 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/process_data/colmap_converter_to_nerfstudio_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24486 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/process_data/colmap_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8283 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/process_data/equirect_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5089 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/process_data/hloc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/process_data/images_to_nerfstudio_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/process_data/metashape_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9227 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/process_data/polycam_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20540 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/process_data/process_data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4841 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/process_data/realitycapture_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/process_data/record3d_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4677 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/process_data/video_to_nerfstudio_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:28.084534 nerfstudio-0.3.2/nerfstudio/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/scripts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:28.084534 nerfstudio-0.3.2/nerfstudio/scripts/blender/
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/scripts/blender/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17248 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/scripts/blender/nerfstudio_blender.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:28.084534 nerfstudio-0.3.2/nerfstudio/scripts/completions/
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/scripts/completions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15547 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/scripts/completions/install.py
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/scripts/completions/setup.bash
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/scripts/completions/setup.zsh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:28.084534 nerfstudio-0.3.2/nerfstudio/scripts/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)     6544 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/scripts/datasets/process_nuscenes_masks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:28.084534 nerfstudio-0.3.2/nerfstudio/scripts/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/scripts/docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/scripts/docs/add_nb_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/scripts/docs/build_docs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:28.084534 nerfstudio-0.3.2/nerfstudio/scripts/downloads/
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/scripts/downloads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20378 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/scripts/downloads/download_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/scripts/eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19071 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/scripts/exporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:28.084534 nerfstudio-0.3.2/nerfstudio/scripts/github/
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/scripts/github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/scripts/github/run_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17084 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/scripts/process_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22196 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/scripts/render.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/scripts/texture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9806 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/scripts/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:28.084534 nerfstudio-0.3.2/nerfstudio/scripts/viewer/
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/scripts/viewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3927 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/scripts/viewer/run_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/scripts/viewer/sync_viser_message_defs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:28.088534 nerfstudio-0.3.2/nerfstudio/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/utils/colormaps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/utils/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/utils/comms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/utils/eval_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/utils/install_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11519 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/utils/math.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5991 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16856 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/utils/plotly_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/utils/poses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/utils/printing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8012 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/utils/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/utils/rich_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/utils/scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13273 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/utils/tensor_dataclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17377 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/utils/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:28.088534 nerfstudio-0.3.2/nerfstudio/viewer/
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/viewer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:28.088534 nerfstudio-0.3.2/nerfstudio/viewer/app/
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/viewer/app/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:28.088534 nerfstudio-0.3.2/nerfstudio/viewer/app/public/
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/viewer/app/public/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/viewer/app/run_deploy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:28.056534 nerfstudio-0.3.2/nerfstudio/viewer/app/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:28.088534 nerfstudio-0.3.2/nerfstudio/viewer/app/src/themes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/viewer/app/src/themes/leva_theme.json
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/viewer/app/tsconfig.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:28.092534 nerfstudio-0.3.2/nerfstudio/viewer/server/
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/viewer/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14703 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/viewer/server/control_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/viewer/server/gui_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/viewer/server/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12041 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/viewer/server/render_state_machine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:28.092534 nerfstudio-0.3.2/nerfstudio/viewer/server/state/
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/viewer/server/state/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/viewer/server/state/state_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/viewer/server/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18286 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/viewer/server/viewer_elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18596 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/viewer/server/viewer_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/viewer/server/viewer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:28.096534 nerfstudio-0.3.2/nerfstudio/viewer/viser/
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/viewer/viser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6437 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/viewer/viser/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21891 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/viewer/viser/message_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7352 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/viewer/viser/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/viewer/viser/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:28.096534 nerfstudio-0.3.2/nerfstudio/viewer_beta/
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/viewer_beta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14756 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/viewer_beta/control_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12362 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/viewer_beta/render_state_machine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/viewer_beta/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10609 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/viewer_beta/viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14288 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/nerfstudio/viewer_beta/viewer_elements.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:28.060534 nerfstudio-0.3.2/nerfstudio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19581 2023-06-22 16:29:28.000000 nerfstudio-0.3.2/nerfstudio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7605 2023-06-22 16:29:28.000000 nerfstudio-0.3.2/nerfstudio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 16:29:28.000000 nerfstudio-0.3.2/nerfstudio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-22 16:29:28.000000 nerfstudio-0.3.2/nerfstudio.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-06-22 16:29:28.000000 nerfstudio-0.3.2/nerfstudio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-22 16:29:28.000000 nerfstudio-0.3.2/nerfstudio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5095 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 16:29:28.096534 nerfstudio-0.3.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:28.096534 nerfstudio-0.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-06-22 16:29:08.000000 nerfstudio-0.3.2/tests/test_train.py
```

### Comparing `nerfstudio-0.3.1/LICENSE` & `nerfstudio-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/PKG-INFO` & `nerfstudio-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nerfstudio
-Version: 0.3.1
+Version: 0.3.2
 Summary: All-in-one repository for state-of-the-art NeRFs
 License: Apache 2.0
 Project-URL: Documentation, https://docs.nerf.studio
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
@@ -306,21 +306,25 @@
 # Citation
 
 You can find a paper writeup of the framework on [arXiv](https://arxiv.org/abs/2302.04264).
 
 If you use this library or find the documentation useful for your research, please consider citing:
 
 ```
-@article{nerfstudio,
-    author = {Tancik, Matthew and Weber, Ethan and Ng, Evonne and Li, Ruilong and Yi,
-            Brent and Kerr, Justin and Wang, Terrance and Kristoffersen, Alexander and Austin,
-            Jake and Salahi, Kamyar and Ahuja, Abhik and McAllister, David and Kanazawa, Angjoo},
-    title = {Nerfstudio: A Modular Framework for Neural Radiance Field Development},
-    journal = {arXiv preprint arXiv:2302.04264},
-    year = {2023},
+@inproceedings{nerfstudio,
+	title        = {Nerfstudio: A Modular Framework for Neural Radiance Field Development},
+	author       = {
+		Tancik, Matthew and Weber, Ethan and Ng, Evonne and Li, Ruilong and Yi, Brent
+		and Kerr, Justin and Wang, Terrance and Kristoffersen, Alexander and Austin,
+		Jake and Salahi, Kamyar and Ahuja, Abhik and McAllister, David and Kanazawa,
+		Angjoo
+	},
+	year         = 2023,
+	booktitle    = {ACM SIGGRAPH 2023 Conference Proceedings},
+	series       = {SIGGRAPH '23}
 }
 ```
 
 # Contributors
 
 <a href="https://github.com/nerfstudio-project/nerfstudio/graphs/contributors">
   <img src="https://contrib.rocks/image?repo=nerfstudio-project/nerfstudio" />
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nerfstudio Version: 0.3.1 Summary: All-in-one
+Metadata-Version: 2.1 Name: nerfstudio Version: 0.3.2 Summary: All-in-one
 repository for state-of-the-art NeRFs License: Apache 2.0 Project-URL:
 Documentation, https://docs.nerf.studio Classifier: Development Status :: 3 -
 Alpha Classifier: Programming Language :: Python Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown Provides-Extra: gen Provides-Extra: dev
 Provides-Extra: docs License-File: LICENSE
  [https://img.shields.io/badge/Join-Discord-blue.svg]  [Documentation_Status]
         [PyPI_version]  [Test_Status] [Viewer_build_Status]  [License]
@@ -185,14 +185,15 @@
 on the Blender dataset - :iphone: Full pipeline support (w/ Colmap, Polycam, or
 Record3D) for going from a video on your phone to a full 3D render. # Built On
 [tyro_logo] - Easy-to-use config system - Developed by [Brent Yi](https://
 brentyi.com/) [tyro_logo] - Library for accelerating NeRF renders - Developed
 by [Ruilong Li](https://www.liruilong.cn/) # Citation You can find a paper
 writeup of the framework on [arXiv](https://arxiv.org/abs/2302.04264). If you
 use this library or find the documentation useful for your research, please
-consider citing: ``` @article{nerfstudio, author = {Tancik, Matthew and Weber,
-Ethan and Ng, Evonne and Li, Ruilong and Yi, Brent and Kerr, Justin and Wang,
-Terrance and Kristoffersen, Alexander and Austin, Jake and Salahi, Kamyar and
-Ahuja, Abhik and McAllister, David and Kanazawa, Angjoo}, title = {Nerfstudio:
-A Modular Framework for Neural Radiance Field Development}, journal = {arXiv
-preprint arXiv:2302.04264}, year = {2023}, } ``` # Contributors [https://
-contrib.rocks/image?repo=nerfstudio-project/nerfstudio]
+consider citing: ``` @inproceedings{nerfstudio, title = {Nerfstudio: A Modular
+Framework for Neural Radiance Field Development}, author = { Tancik, Matthew
+and Weber, Ethan and Ng, Evonne and Li, Ruilong and Yi, Brent and Kerr, Justin
+and Wang, Terrance and Kristoffersen, Alexander and Austin, Jake and Salahi,
+Kamyar and Ahuja, Abhik and McAllister, David and Kanazawa, Angjoo }, year =
+2023, booktitle = {ACM SIGGRAPH 2023 Conference Proceedings}, series =
+{SIGGRAPH '23} } ``` # Contributors [https://contrib.rocks/
+image?repo=nerfstudio-project/nerfstudio]
```

### Comparing `nerfstudio-0.3.1/README.md` & `nerfstudio-0.3.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -291,21 +291,25 @@
 # Citation
 
 You can find a paper writeup of the framework on [arXiv](https://arxiv.org/abs/2302.04264).
 
 If you use this library or find the documentation useful for your research, please consider citing:
 
 ```
-@article{nerfstudio,
-    author = {Tancik, Matthew and Weber, Ethan and Ng, Evonne and Li, Ruilong and Yi,
-            Brent and Kerr, Justin and Wang, Terrance and Kristoffersen, Alexander and Austin,
-            Jake and Salahi, Kamyar and Ahuja, Abhik and McAllister, David and Kanazawa, Angjoo},
-    title = {Nerfstudio: A Modular Framework for Neural Radiance Field Development},
-    journal = {arXiv preprint arXiv:2302.04264},
-    year = {2023},
+@inproceedings{nerfstudio,
+	title        = {Nerfstudio: A Modular Framework for Neural Radiance Field Development},
+	author       = {
+		Tancik, Matthew and Weber, Ethan and Ng, Evonne and Li, Ruilong and Yi, Brent
+		and Kerr, Justin and Wang, Terrance and Kristoffersen, Alexander and Austin,
+		Jake and Salahi, Kamyar and Ahuja, Abhik and McAllister, David and Kanazawa,
+		Angjoo
+	},
+	year         = 2023,
+	booktitle    = {ACM SIGGRAPH 2023 Conference Proceedings},
+	series       = {SIGGRAPH '23}
 }
 ```
 
 # Contributors
 
 <a href="https://github.com/nerfstudio-project/nerfstudio/graphs/contributors">
   <img src="https://contrib.rocks/image?repo=nerfstudio-project/nerfstudio" />
```

#### html2text {}

```diff
@@ -179,14 +179,15 @@
 on the Blender dataset - :iphone: Full pipeline support (w/ Colmap, Polycam, or
 Record3D) for going from a video on your phone to a full 3D render. # Built On
 [tyro_logo] - Easy-to-use config system - Developed by [Brent Yi](https://
 brentyi.com/) [tyro_logo] - Library for accelerating NeRF renders - Developed
 by [Ruilong Li](https://www.liruilong.cn/) # Citation You can find a paper
 writeup of the framework on [arXiv](https://arxiv.org/abs/2302.04264). If you
 use this library or find the documentation useful for your research, please
-consider citing: ``` @article{nerfstudio, author = {Tancik, Matthew and Weber,
-Ethan and Ng, Evonne and Li, Ruilong and Yi, Brent and Kerr, Justin and Wang,
-Terrance and Kristoffersen, Alexander and Austin, Jake and Salahi, Kamyar and
-Ahuja, Abhik and McAllister, David and Kanazawa, Angjoo}, title = {Nerfstudio:
-A Modular Framework for Neural Radiance Field Development}, journal = {arXiv
-preprint arXiv:2302.04264}, year = {2023}, } ``` # Contributors [https://
-contrib.rocks/image?repo=nerfstudio-project/nerfstudio]
+consider citing: ``` @inproceedings{nerfstudio, title = {Nerfstudio: A Modular
+Framework for Neural Radiance Field Development}, author = { Tancik, Matthew
+and Weber, Ethan and Ng, Evonne and Li, Ruilong and Yi, Brent and Kerr, Justin
+and Wang, Terrance and Kristoffersen, Alexander and Austin, Jake and Salahi,
+Kamyar and Ahuja, Abhik and McAllister, David and Kanazawa, Angjoo }, year =
+2023, booktitle = {ACM SIGGRAPH 2023 Conference Proceedings}, series =
+{SIGGRAPH '23} } ``` # Contributors [https://contrib.rocks/
+image?repo=nerfstudio-project/nerfstudio]
```

### Comparing `nerfstudio-0.3.1/nerfstudio/__init__.py` & `nerfstudio-0.3.2/nerfstudio/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/cameras/__init__.py` & `nerfstudio-0.3.2/nerfstudio/cameras/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/cameras/camera_optimizers.py` & `nerfstudio-0.3.2/nerfstudio/cameras/camera_optimizers.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 Pose and Intrinsics Optimizers
 """
 
 from __future__ import annotations
 
 import functools
 from dataclasses import dataclass, field
-from typing import Literal, Type, Union
+from typing import Literal, Optional, Type, Union
 
 import torch
 import tyro
 from jaxtyping import Float, Int
 from torch import Tensor, nn
 from typing_extensions import assert_never
 
@@ -49,18 +49,18 @@
 
     position_noise_std: float = 0.0
     """Noise to add to initial positions. Useful for debugging."""
 
     orientation_noise_std: float = 0.0
     """Noise to add to initial orientations. Useful for debugging."""
 
-    optimizer: OptimizerConfig = AdamOptimizerConfig(lr=6e-4, eps=1e-15)
+    optimizer: OptimizerConfig = field(default_factory=lambda: AdamOptimizerConfig(lr=6e-4, eps=1e-15))
     """ADAM parameters for camera optimization."""
 
-    scheduler: SchedulerConfig = ExponentialDecaySchedulerConfig(max_steps=10000)
+    scheduler: SchedulerConfig = field(default_factory=lambda: ExponentialDecaySchedulerConfig(max_steps=10000))
     """Learning rate scheduler for camera optimizer.."""
 
     param_group: tyro.conf.Suppress[str] = "camera_opt"
     """Name of the parameter group used for pose optimization. Can be any string that doesn't conflict with other
     groups."""
 
 
@@ -70,20 +70,22 @@
     config: CameraOptimizerConfig
 
     def __init__(
         self,
         config: CameraOptimizerConfig,
         num_cameras: int,
         device: Union[torch.device, str],
+        non_trainable_camera_indices: Optional[Int[Tensor, "num_non_trainable_cameras"]] = None,
         **kwargs,
     ) -> None:
         super().__init__()
         self.config = config
         self.num_cameras = num_cameras
         self.device = device
+        self.non_trainable_camera_indices = non_trainable_camera_indices
 
         # Initialize learnable parameters.
         if self.config.mode == "off":
             pass
         elif self.config.mode in ("SO3xR3", "SE3"):
             self.pose_adjustment = torch.nn.Parameter(torch.zeros((num_cameras, 6), device=device))
         else:
@@ -117,17 +119,19 @@
             pass
         elif self.config.mode == "SO3xR3":
             outputs.append(exp_map_SO3xR3(self.pose_adjustment[indices, :]))
         elif self.config.mode == "SE3":
             outputs.append(exp_map_SE3(self.pose_adjustment[indices, :]))
         else:
             assert_never(self.config.mode)
+        # Detach non-trainable indices by setting to identity transform
+        if self.non_trainable_camera_indices is not None:
+            outputs[0][self.non_trainable_camera_indices] = torch.eye(4, device=self.device)[:3, :4]
 
         # Apply initial pose noise.
         if self.pose_noise is not None:
             outputs.append(self.pose_noise[indices, :, :])
-
         # Return: identity if no transforms are needed, otherwise multiply transforms together.
         if len(outputs) == 0:
             # Note that using repeat() instead of tile() here would result in unnecessary copies.
             return torch.eye(4, device=self.device)[None, :3, :4].tile(indices.shape[0], 1, 1)
         return functools.reduce(pose_utils.multiply, outputs)
```

### Comparing `nerfstudio-0.3.1/nerfstudio/cameras/camera_paths.py` & `nerfstudio-0.3.2/nerfstudio/cameras/camera_paths.py`

 * *Files 5% similar despite different names*

```diff
@@ -135,25 +135,31 @@
 
     if "camera_type" not in camera_path:
         camera_type = CameraType.PERSPECTIVE
     elif camera_path["camera_type"] == "fisheye":
         camera_type = CameraType.FISHEYE
     elif camera_path["camera_type"] == "equirectangular":
         camera_type = CameraType.EQUIRECTANGULAR
+    elif camera_path["camera_type"].lower() == "omnidirectional":
+        camera_type = CameraType.OMNIDIRECTIONALSTEREO_L
     else:
         camera_type = CameraType.PERSPECTIVE
 
     c2ws = []
     fxs = []
     fys = []
     for camera in camera_path["camera_path"]:
         # pose
         c2w = torch.tensor(camera["camera_to_world"]).view(4, 4)[:3]
         c2ws.append(c2w)
-        if camera_type == CameraType.EQUIRECTANGULAR:
+        if (
+            camera_type == CameraType.EQUIRECTANGULAR
+            or camera_type == CameraType.OMNIDIRECTIONALSTEREO_L
+            or camera_type == CameraType.OMNIDIRECTIONALSTEREO_R
+        ):
             fxs.append(image_width / 2)
             fys.append(image_height)
         else:
             # field of view
             fov = camera["fov"]
             focal_length = three_js_perspective_camera_focal_length(fov, image_height)
             fxs.append(focal_length)
```

### Comparing `nerfstudio-0.3.1/nerfstudio/cameras/camera_utils.py` & `nerfstudio-0.3.2/nerfstudio/cameras/camera_utils.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/cameras/cameras.py` & `nerfstudio-0.3.2/nerfstudio/cameras/cameras.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 """
 Camera Models
 """
 import base64
 import math
 from dataclasses import dataclass
 from enum import Enum, auto
-from typing import Dict, List, Optional, Tuple, Union
+from typing import Dict, List, Literal, Optional, Tuple, Union
 
 import cv2
 import torch
 import torchvision
 from jaxtyping import Float, Int, Shaped
 from torch import Tensor
 from torch.nn import Parameter
@@ -40,24 +40,28 @@
 
 class CameraType(Enum):
     """Supported camera types."""
 
     PERSPECTIVE = auto()
     FISHEYE = auto()
     EQUIRECTANGULAR = auto()
+    OMNIDIRECTIONALSTEREO_L = auto()
+    OMNIDIRECTIONALSTEREO_R = auto()
 
 
 CAMERA_MODEL_TO_TYPE = {
     "SIMPLE_PINHOLE": CameraType.PERSPECTIVE,
     "PINHOLE": CameraType.PERSPECTIVE,
     "SIMPLE_RADIAL": CameraType.PERSPECTIVE,
     "RADIAL": CameraType.PERSPECTIVE,
     "OPENCV": CameraType.PERSPECTIVE,
     "OPENCV_FISHEYE": CameraType.FISHEYE,
     "EQUIRECTANGULAR": CameraType.EQUIRECTANGULAR,
+    "OMNIDIRECTIONALSTEREO_L": CameraType.OMNIDIRECTIONALSTEREO_L,
+    "OMNIDIRECTIONALSTEREO_R": CameraType.OMNIDIRECTIONALSTEREO_R,
 }
 
 
 @dataclass(init=False)
 class Cameras(TensorDataclass):
     """Dataparser outputs for the image dataset and the ray generator.
 
@@ -353,15 +357,15 @@
             coords: Coordinates of the pixels to generate rays for. If None, the full image will be rendered.
             camera_opt_to_camera: Optional transform for the camera to world matrices.
             distortion_params_delta: Optional delta for the distortion parameters.
             keep_shape: If None, then we default to the regular behavior of flattening if cameras is jagged, otherwise
                 keeping dimensions. If False, we flatten at the end. If True, then we keep the shape of the
                 camera_indices and coords tensors (if we can).
             disable_distortion: If True, disables distortion.
-            aabb_box: if not None will calculate nears and fars of the ray according to aabb box intesection
+            aabb_box: if not None will calculate nears and fars of the ray according to aabb box intersection
 
         Returns:
             Rays for the given camera indices and coords.
         """
         # Check the argument types to make sure they're valid and all shaped correctly
         assert isinstance(camera_indices, (torch.Tensor, int)), "camera_indices must be a tensor or int"
         assert coords is None or isinstance(coords, torch.Tensor), "coords must be a tensor or None"
@@ -639,55 +643,127 @@
         # Gets our directions for all our rays in camera coordinates and checks shapes at the end
         # Here, directions_stack is of shape (3, num_rays, 3)
         # directions_stack[0] is the direction for ray in camera coordinates
         # directions_stack[1] is the direction for ray in camera coordinates offset by 1 in x
         # directions_stack[2] is the direction for ray in camera coordinates offset by 1 in y
         cam_types = torch.unique(self.camera_type, sorted=False)
         directions_stack = torch.empty((3,) + num_rays_shape + (3,), device=self.device)
-        if CameraType.PERSPECTIVE.value in cam_types:
-            mask = (self.camera_type[true_indices] == CameraType.PERSPECTIVE.value).squeeze(-1)  # (num_rays)
-            mask = torch.stack([mask, mask, mask], dim=0)
-            directions_stack[..., 0][mask] = torch.masked_select(coord_stack[..., 0], mask).float()
-            directions_stack[..., 1][mask] = torch.masked_select(coord_stack[..., 1], mask).float()
-            directions_stack[..., 2][mask] = -1.0
-
-        if CameraType.FISHEYE.value in cam_types:
-            mask = (self.camera_type[true_indices] == CameraType.FISHEYE.value).squeeze(-1)  # (num_rays)
-            mask = torch.stack([mask, mask, mask], dim=0)
-
-            theta = torch.sqrt(torch.sum(coord_stack**2, dim=-1))
-            theta = torch.clip(theta, 0.0, math.pi)
 
-            sin_theta = torch.sin(theta)
-
-            directions_stack[..., 0][mask] = torch.masked_select(coord_stack[..., 0] * sin_theta / theta, mask).float()
-            directions_stack[..., 1][mask] = torch.masked_select(coord_stack[..., 1] * sin_theta / theta, mask).float()
-            directions_stack[..., 2][mask] = -torch.masked_select(torch.cos(theta), mask).float()
+        c2w = self.camera_to_worlds[true_indices]
+        assert c2w.shape == num_rays_shape + (3, 4)
 
-        if CameraType.EQUIRECTANGULAR.value in cam_types:
-            mask = (self.camera_type[true_indices] == CameraType.EQUIRECTANGULAR.value).squeeze(-1)  # (num_rays)
+        def _compute_rays_for_omnidirectional_stereo(
+            eye: Literal["left", "right"]
+        ) -> Tuple[Float[Tensor, "num_rays_shape 3"], Float[Tensor, "3 num_rays_shape 3"]]:
+            """Compute the rays for an omnidirectional stereo camera
+
+            Args:
+                eye: Which eye to compute rays for.
+
+            Returns:
+                A tuple containing the origins and the directions of the rays.
+            """
+            # Directions calculated similarly to equirectangular
+            ods_cam_type = (
+                CameraType.OMNIDIRECTIONALSTEREO_R.value if eye == "right" else CameraType.OMNIDIRECTIONALSTEREO_L.value
+            )
+            mask = (self.camera_type[true_indices] == ods_cam_type).squeeze(-1)
             mask = torch.stack([mask, mask, mask], dim=0)
-
-            # For equirect, fx = fy = height = width/2
-            # Then coord[..., 0] goes from -1 to 1 and coord[..., 1] goes from -1/2 to 1/2
-            theta = -torch.pi * coord_stack[..., 0]  # minus sign for right-handed
+            theta = -torch.pi * coord_stack[..., 0]
             phi = torch.pi * (0.5 - coord_stack[..., 1])
-            # use spherical in local camera coordinates (+y up, x=0 and z<0 is theta=0)
+
             directions_stack[..., 0][mask] = torch.masked_select(-torch.sin(theta) * torch.sin(phi), mask).float()
             directions_stack[..., 1][mask] = torch.masked_select(torch.cos(phi), mask).float()
             directions_stack[..., 2][mask] = torch.masked_select(-torch.cos(theta) * torch.sin(phi), mask).float()
 
-        for value in cam_types:
-            if value not in [CameraType.PERSPECTIVE.value, CameraType.FISHEYE.value, CameraType.EQUIRECTANGULAR.value]:
-                raise ValueError(f"Camera type {value} not supported.")
+            vr_ipd = 0.064  # IPD in meters (note: scale of NeRF must be true to life and can be adjusted with the Blender add-on)
+            isRightEye = 1 if eye == "right" else -1
 
-        assert directions_stack.shape == (3,) + num_rays_shape + (3,)
+            # find ODS camera position
+            c2w = self.camera_to_worlds[true_indices]
+            assert c2w.shape == num_rays_shape + (3, 4)
+            transposedC2W = c2w[0][0].t()
+            ods_cam_position = transposedC2W[3].repeat(c2w.shape[1], 1)
+
+            rotation = c2w[..., :3, :3]
+
+            ods_theta = -torch.pi * ((x - cx) / fx)[0]
+
+            # local axes of ODS camera
+            ods_x_axis = torch.tensor([1, 0, 0], device=c2w.device)
+            ods_z_axis = torch.tensor([0, 0, -1], device=c2w.device)
+
+            # circle of ODS ray origins
+            ods_origins_circle = (
+                ods_cam_position
+                + isRightEye * (vr_ipd / 2.0) * (ods_x_axis.repeat(c2w.shape[1], 1)) * (torch.cos(ods_theta))[:, None]
+                + isRightEye * (vr_ipd / 2.0) * (ods_z_axis.repeat(c2w.shape[1], 1)) * (torch.sin(ods_theta))[:, None]
+            )
 
-        c2w = self.camera_to_worlds[true_indices]
-        assert c2w.shape == num_rays_shape + (3, 4)
+            # rotate origins to match the camera rotation
+            for i in range(ods_origins_circle.shape[0]):
+                ods_origins_circle[i] = rotation[0][0] @ ods_origins_circle[i] + ods_cam_position[0]
+            ods_origins_circle = ods_origins_circle.unsqueeze(0).repeat(c2w.shape[0], 1, 1)
+
+            # assign final camera origins
+            c2w[..., :3, 3] = ods_origins_circle
+
+            return ods_origins_circle, directions_stack
+
+        for cam in cam_types:
+            if CameraType.PERSPECTIVE.value in cam_types:
+                mask = (self.camera_type[true_indices] == CameraType.PERSPECTIVE.value).squeeze(-1)  # (num_rays)
+                mask = torch.stack([mask, mask, mask], dim=0)
+                directions_stack[..., 0][mask] = torch.masked_select(coord_stack[..., 0], mask).float()
+                directions_stack[..., 1][mask] = torch.masked_select(coord_stack[..., 1], mask).float()
+                directions_stack[..., 2][mask] = -1.0
+
+            elif CameraType.FISHEYE.value in cam_types:
+                mask = (self.camera_type[true_indices] == CameraType.FISHEYE.value).squeeze(-1)  # (num_rays)
+                mask = torch.stack([mask, mask, mask], dim=0)
+
+                theta = torch.sqrt(torch.sum(coord_stack**2, dim=-1))
+                theta = torch.clip(theta, 0.0, math.pi)
+
+                sin_theta = torch.sin(theta)
+
+                directions_stack[..., 0][mask] = torch.masked_select(
+                    coord_stack[..., 0] * sin_theta / theta, mask
+                ).float()
+                directions_stack[..., 1][mask] = torch.masked_select(
+                    coord_stack[..., 1] * sin_theta / theta, mask
+                ).float()
+                directions_stack[..., 2][mask] = -torch.masked_select(torch.cos(theta), mask).float()
+
+            elif CameraType.EQUIRECTANGULAR.value in cam_types:
+                mask = (self.camera_type[true_indices] == CameraType.EQUIRECTANGULAR.value).squeeze(-1)  # (num_rays)
+                mask = torch.stack([mask, mask, mask], dim=0)
+
+                # For equirect, fx = fy = height = width/2
+                # Then coord[..., 0] goes from -1 to 1 and coord[..., 1] goes from -1/2 to 1/2
+                theta = -torch.pi * coord_stack[..., 0]  # minus sign for right-handed
+                phi = torch.pi * (0.5 - coord_stack[..., 1])
+                # use spherical in local camera coordinates (+y up, x=0 and z<0 is theta=0)
+                directions_stack[..., 0][mask] = torch.masked_select(-torch.sin(theta) * torch.sin(phi), mask).float()
+                directions_stack[..., 1][mask] = torch.masked_select(torch.cos(phi), mask).float()
+                directions_stack[..., 2][mask] = torch.masked_select(-torch.cos(theta) * torch.sin(phi), mask).float()
+
+            elif CameraType.OMNIDIRECTIONALSTEREO_L.value in cam_types:
+                ods_origins_circle, directions_stack = _compute_rays_for_omnidirectional_stereo("left")
+                # assign final camera origins
+                c2w[..., :3, 3] = ods_origins_circle
+
+            elif CameraType.OMNIDIRECTIONALSTEREO_R.value in cam_types:
+                ods_origins_circle, directions_stack = _compute_rays_for_omnidirectional_stereo("right")
+                # assign final camera origins
+                c2w[..., :3, 3] = ods_origins_circle
+            else:
+                raise ValueError(f"Camera type {cam} not supported.")
+
+        assert directions_stack.shape == (3,) + num_rays_shape + (3,)
 
         if camera_opt_to_camera is not None:
             c2w = pose_utils.multiply(c2w, camera_opt_to_camera)
         rotation = c2w[..., :3, :3]  # (..., 3, 3)
         assert rotation.shape == num_rays_shape + (3, 3)
 
         directions_stack = torch.sum(
@@ -758,15 +834,15 @@
             "camera_index": camera_idx,
             "times": times,
         }
         if image is not None:
             image_uint8 = (image * 255).detach().type(torch.uint8)
             if max_size is not None:
                 image_uint8 = image_uint8.permute(2, 0, 1)
-                image_uint8 = torchvision.transforms.functional.resize(image_uint8, max_size)  # type: ignore
+                image_uint8 = torchvision.transforms.functional.resize(image_uint8, max_size, antialias=None)  # type: ignore
                 image_uint8 = image_uint8.permute(1, 2, 0)
             image_uint8 = image_uint8.cpu().numpy()
             data = cv2.imencode(".jpg", image_uint8)[1].tobytes()  # type: ignore
             json_["image"] = str("data:image/jpeg;base64," + base64.b64encode(data).decode("ascii"))
         return json_
 
     def get_intrinsics_matrices(self) -> Float[Tensor, "*num_cameras 3 3"]:
```

### Comparing `nerfstudio-0.3.1/nerfstudio/cameras/lie_groups.py` & `nerfstudio-0.3.2/nerfstudio/cameras/lie_groups.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/cameras/rays.py` & `nerfstudio-0.3.2/nerfstudio/cameras/rays.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/configs/__init__.py` & `nerfstudio-0.3.2/nerfstudio/configs/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/configs/base_config.py` & `nerfstudio-0.3.2/nerfstudio/configs/base_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,22 +60,24 @@
 # Machine related configs
 @dataclass
 class MachineConfig(PrintableConfig):
     """Configuration of machine setup"""
 
     seed: int = 42
     """random seed initialization"""
-    num_gpus: int = 1
-    """total number of gpus available for train/eval"""
+    num_devices: int = 1
+    """total number of devices (e.g., gpus) available for train/eval"""
     num_machines: int = 1
     """total number of distributed machines available (for DDP)"""
     machine_rank: int = 0
     """current machine's rank (for DDP)"""
     dist_url: str = "auto"
     """distributed connection point (for DDP)"""
+    device_type: Literal["cpu", "cuda", "mps"] = "cuda"
+    """device type to use for training"""
 
 
 @dataclass
 class LocalWriterConfig(InstantiateConfig):
     """Local Writer config"""
 
     _target: Type = writer.LocalWriter
```

### Comparing `nerfstudio-0.3.1/nerfstudio/configs/config_utils.py` & `nerfstudio-0.3.2/nerfstudio/configs/config_utils.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/configs/dataparser_configs.py` & `nerfstudio-0.3.2/nerfstudio/configs/dataparser_configs.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/configs/experiment_config.py` & `nerfstudio-0.3.2/nerfstudio/configs/experiment_config.py`

 * *Files 11% similar despite different names*

```diff
@@ -64,25 +64,31 @@
             "fields": {
                 "optimizer": OptimizerConfig(),
                 "scheduler": SchedulerConfig(),
             }
         }
     )
     """Dictionary of optimizer groups and their schedulers"""
-    vis: Literal["viewer", "wandb", "tensorboard", "viewer+wandb", "viewer+tensorboard"] = "wandb"
+    vis: Literal["viewer", "wandb", "tensorboard", "viewer+wandb", "viewer+tensorboard", "viewer_beta"] = "wandb"
     """Which visualizer to use."""
     data: Optional[Path] = None
     """Alias for --pipeline.datamanager.data"""
+    prompt: Optional[str] = None
+    """Alias for --pipeline.model.prompt"""
     relative_model_dir: Path = Path("nerfstudio_models/")
     """Relative path to save all checkpoints."""
 
     def is_viewer_enabled(self) -> bool:
         """Checks if a viewer is enabled."""
         return ("viewer" == self.vis) | ("viewer+wandb" == self.vis) | ("viewer+tensorboard" == self.vis)
 
+    def is_viewer_beta_enabled(self) -> bool:
+        """Checks if a viewer beta is enabled."""
+        return "viewer_beta" == self.vis
+
     def is_wandb_enabled(self) -> bool:
         """Checks if wandb is enabled."""
         return ("wandb" == self.vis) | ("viewer+wandb" == self.vis)
 
     def is_tensorboard_enabled(self) -> bool:
         """Checks if tensorboard is enabled."""
         return ("tensorboard" == self.vis) | ("viewer+tensorboard" == self.vis)
```

### Comparing `nerfstudio-0.3.1/nerfstudio/configs/external_methods.py` & `nerfstudio-0.3.2/nerfstudio/configs/external_methods.py`

 * *Files 5% similar despite different names*

```diff
@@ -102,14 +102,29 @@
         configurations=[
             ("tetra-nerf-original", "Tetra-NeRF. Official implementation from the paper"),
             ("tetra-nerf", "Tetra-NeRF. Different sampler - faster and better"),
         ],
     )
 )
 
+# NeRFPlayer
+external_methods.append(
+    ExternalMethod(
+        """[bold yellow]NeRFPlayer[/bold yellow]
+For more information visit: https://docs.nerf.studio/en/latest/nerfology/methods/nerfplayer.html
+
+To enable NeRFPlayer, you must install it first by running:
+  [grey]pip install git+https://github.com/lsongx/nerfplayer-nerfstudio[/grey]""",
+        configurations=[
+            ("nerfplayer-nerfacto", "NeRFPlayer with nerfacto backbone"),
+            ("nerfplayer-ngp", "NeRFPlayer with instang-ngp-bounded backbone"),
+        ],
+    )
+)
+
 
 @dataclass
 class ExternalMethodTrainerConfig(TrainerConfig):
     """
     Trainer config for external methods which does not have an implementation in this repository.
     """
```

### Comparing `nerfstudio-0.3.1/nerfstudio/configs/method_configs.py` & `nerfstudio-0.3.2/nerfstudio/configs/method_configs.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,28 +22,23 @@
 from typing import Dict
 
 import tyro
 
 from nerfstudio.cameras.camera_optimizers import CameraOptimizerConfig
 from nerfstudio.configs.base_config import ViewerConfig
 from nerfstudio.configs.external_methods import get_external_methods
-from nerfstudio.data.datamanagers.base_datamanager import (
-    VanillaDataManager,
-    VanillaDataManagerConfig,
-)
+
+from nerfstudio.data.datamanagers.random_cameras_datamanager import RandomCamerasDataManagerConfig
+from nerfstudio.data.datamanagers.base_datamanager import VanillaDataManager, VanillaDataManagerConfig
+
 from nerfstudio.data.dataparsers.blender_dataparser import BlenderDataParserConfig
 from nerfstudio.data.dataparsers.dnerf_dataparser import DNeRFDataParserConfig
-from nerfstudio.data.dataparsers.dycheck_dataparser import DycheckDataParserConfig
-from nerfstudio.data.dataparsers.instant_ngp_dataparser import (
-    InstantNGPDataParserConfig,
-)
+from nerfstudio.data.dataparsers.instant_ngp_dataparser import InstantNGPDataParserConfig
 from nerfstudio.data.dataparsers.nerfstudio_dataparser import NerfstudioDataParserConfig
-from nerfstudio.data.dataparsers.phototourism_dataparser import (
-    PhototourismDataParserConfig,
-)
+from nerfstudio.data.dataparsers.phototourism_dataparser import PhototourismDataParserConfig
 from nerfstudio.data.dataparsers.sdfstudio_dataparser import SDFStudioDataParserConfig
 from nerfstudio.data.dataparsers.sitcoms3d_dataparser import Sitcoms3DDataParserConfig
 from nerfstudio.data.datasets.depth_dataset import DepthDataset
 from nerfstudio.data.datasets.sdf_dataset import SDFDataset
 from nerfstudio.data.datasets.semantic_dataset import SemanticDataset
 from nerfstudio.engine.optimizers import AdamOptimizerConfig, RAdamOptimizerConfig
 from nerfstudio.engine.schedulers import (
@@ -51,19 +46,18 @@
     ExponentialDecaySchedulerConfig,
     MultiStepSchedulerConfig,
 )
 from nerfstudio.engine.trainer import TrainerConfig
 from nerfstudio.field_components.temporal_distortions import TemporalDistortionKind
 from nerfstudio.fields.sdf_field import SDFFieldConfig
 from nerfstudio.models.depth_nerfacto import DepthNerfactoModelConfig
+from nerfstudio.models.generfacto import GenerfactoModelConfig
 from nerfstudio.models.instant_ngp import InstantNGPModelConfig
 from nerfstudio.models.mipnerf import MipNerfModel
 from nerfstudio.models.nerfacto import NerfactoModelConfig
-from nerfstudio.models.nerfplayer_nerfacto import NerfplayerNerfactoModelConfig
-from nerfstudio.models.nerfplayer_ngp import NerfplayerNGPModelConfig
 from nerfstudio.models.neus import NeuSModelConfig
 from nerfstudio.models.neus_facto import NeuSFactoModelConfig
 from nerfstudio.models.semantic_nerfw import SemanticNerfWModelConfig
 from nerfstudio.models.tensorf import TensoRFModelConfig
 from nerfstudio.models.vanilla_nerf import NeRFModel, VanillaModelConfig
 from nerfstudio.pipelines.base_pipeline import VanillaPipelineConfig
 from nerfstudio.pipelines.dynamic_batch import DynamicBatchPipelineConfig
@@ -78,16 +72,15 @@
     "instant-ngp-bounded": "Implementation of Instant-NGP. Recommended for bounded real and synthetic scenes",
     "mipnerf": "High quality model for bounded scenes. (slow)",
     "semantic-nerfw": "Predicts semantic segmentations and filters out transient objects.",
     "vanilla-nerf": "Original NeRF model. (slow)",
     "tensorf": "tensorf",
     "dnerf": "Dynamic-NeRF model. (slow)",
     "phototourism": "Uses the Phototourism data.",
-    "nerfplayer-nerfacto": "NeRFPlayer with nerfacto backbone.",
-    "nerfplayer-ngp": "NeRFPlayer with InstantNGP backbone.",
+    "generfacto": "Generative Text to NeRF model",
     "neus": "Implementation of NeuS. (slow)",
     "neus-facto": "Implementation of NeuS-Facto. (slow)",
 }
 
 method_configs["nerfacto"] = TrainerConfig(
     method_name="nerfacto",
     steps_per_eval_batch=500,
@@ -125,41 +118,90 @@
     steps_per_eval_batch=500,
     steps_per_save=2000,
     max_num_iterations=100000,
     mixed_precision=True,
     pipeline=VanillaPipelineConfig(
         datamanager=VanillaDataManagerConfig(
             dataparser=NerfstudioDataParserConfig(),
-            train_num_rays_per_batch=4096,
+            train_num_rays_per_batch=8192,
             eval_num_rays_per_batch=4096,
             camera_optimizer=CameraOptimizerConfig(
                 mode="SO3xR3",
                 optimizer=RAdamOptimizerConfig(lr=6e-4, eps=1e-8, weight_decay=1e-3),
             ),
         ),
         model=NerfactoModelConfig(
             eval_num_rays_per_chunk=1 << 15,
             num_nerf_samples_per_ray=128,
             num_proposal_samples_per_ray=(512, 256),
             hidden_dim=128,
             hidden_dim_color=128,
-            hidden_dim_transient=128,
-            max_res=3000,
+            appearance_embed_dim=128,
+            base_res=32,
+            max_res=4096,
+            proposal_weights_anneal_max_num_iters=5000,
+            log2_hashmap_size=21,
+        ),
+    ),
+    optimizers={
+        "proposal_networks": {
+            "optimizer": RAdamOptimizerConfig(lr=1e-2, eps=1e-15),
+            "scheduler": None,
+        },
+        "fields": {
+            "optimizer": RAdamOptimizerConfig(lr=1e-2, eps=1e-15),
+            "scheduler": ExponentialDecaySchedulerConfig(lr_final=1e-4, max_steps=50000),
+        },
+    },
+    viewer=ViewerConfig(num_rays_per_chunk=1 << 15),
+    vis="viewer",
+)
+method_configs["nerfacto-huge"] = TrainerConfig(
+    method_name="nerfacto",
+    steps_per_eval_batch=500,
+    steps_per_save=2000,
+    max_num_iterations=100000,
+    mixed_precision=True,
+    pipeline=VanillaPipelineConfig(
+        datamanager=VanillaDataManagerConfig(
+            dataparser=NerfstudioDataParserConfig(),
+            train_num_rays_per_batch=16384,
+            eval_num_rays_per_batch=4096,
+            camera_optimizer=CameraOptimizerConfig(
+                mode="SO3xR3",
+                optimizer=RAdamOptimizerConfig(lr=6e-4, eps=1e-8, weight_decay=1e-3),
+                scheduler=ExponentialDecaySchedulerConfig(lr_final=6e-5, max_steps=50000),
+            ),
+        ),
+        model=NerfactoModelConfig(
+            eval_num_rays_per_chunk=1 << 15,
+            num_nerf_samples_per_ray=64,
+            num_proposal_samples_per_ray=(512, 512),
+            proposal_net_args_list=[
+                {"hidden_dim": 16, "log2_hashmap_size": 17, "num_levels": 5, "max_res": 512, "use_linear": False},
+                {"hidden_dim": 16, "log2_hashmap_size": 17, "num_levels": 7, "max_res": 2048, "use_linear": False},
+            ],
+            hidden_dim=256,
+            hidden_dim_color=256,
+            appearance_embed_dim=32,
+            features_per_level=4,
+            base_res=32,
+            max_res=8192,
             proposal_weights_anneal_max_num_iters=5000,
             log2_hashmap_size=21,
         ),
     ),
     optimizers={
         "proposal_networks": {
             "optimizer": RAdamOptimizerConfig(lr=1e-2, eps=1e-15),
             "scheduler": None,
         },
         "fields": {
             "optimizer": RAdamOptimizerConfig(lr=1e-2, eps=1e-15),
-            "scheduler": ExponentialDecaySchedulerConfig(lr_final=1e-4, max_steps=100000),
+            "scheduler": ExponentialDecaySchedulerConfig(lr_final=1e-4, max_steps=50000),
         },
     },
     viewer=ViewerConfig(num_rays_per_chunk=1 << 15),
     vis="viewer",
 )
 
 method_configs["depth-nerfacto"] = TrainerConfig(
@@ -442,74 +484,56 @@
             "scheduler": None,
         },
     },
     viewer=ViewerConfig(num_rays_per_chunk=1 << 15),
     vis="viewer",
 )
 
-method_configs["nerfplayer-nerfacto"] = TrainerConfig(
-    method_name="nerfplayer-nerfacto",
-    steps_per_eval_batch=500,
-    steps_per_save=2000,
+method_configs["generfacto"] = TrainerConfig(
+    method_name="generfacto",
+    experiment_name="",
+    steps_per_eval_batch=50,
+    steps_per_eval_image=50,
+    steps_per_save=200,
     max_num_iterations=30000,
     mixed_precision=True,
     pipeline=VanillaPipelineConfig(
-        datamanager=VanillaDataManagerConfig(
-            _target=VanillaDataManager[DepthDataset],
-            dataparser=DycheckDataParserConfig(),
-            train_num_rays_per_batch=4096,
-            eval_num_rays_per_batch=4096,
-            camera_optimizer=CameraOptimizerConfig(
-                mode="SO3xR3", optimizer=AdamOptimizerConfig(lr=6e-4, eps=1e-8, weight_decay=1e-2)
-            ),
+        datamanager=RandomCamerasDataManagerConfig(
+            horizontal_rotation_warmup=3000,
+        ),
+        model=GenerfactoModelConfig(
+            eval_num_rays_per_chunk=1 << 15,
+            distortion_loss_mult=1.0,
+            interlevel_loss_mult=100.0,
+            max_res=256,
+            sphere_collider=True,
+            initialize_density=True,
+            taper_range=(0, 2000),
+            random_background=True,
+            proposal_warmup=2000,
+            proposal_update_every=0,
+            proposal_weights_anneal_max_num_iters=2000,
+            start_lambertian_training=500,
+            start_normals_training=2000,
+            opacity_loss_mult=0.001,
+            positional_prompting="discrete",
+            guidance_scale=25,
         ),
-        model=NerfplayerNerfactoModelConfig(eval_num_rays_per_chunk=1 << 15),
     ),
     optimizers={
         "proposal_networks": {
-            "optimizer": AdamOptimizerConfig(lr=1e-2, eps=1e-15),
+            "optimizer": AdamOptimizerConfig(lr=1e-3, eps=1e-15),
             "scheduler": None,
         },
         "fields": {
-            "optimizer": AdamOptimizerConfig(lr=1e-2, eps=1e-15),
+            "optimizer": AdamOptimizerConfig(lr=5e-4, eps=1e-15),
             "scheduler": None,
         },
     },
-    viewer=ViewerConfig(num_rays_per_chunk=1 << 15),
-    vis="viewer",
-)
-
-method_configs["nerfplayer-ngp"] = TrainerConfig(
-    method_name="nerfplayer-ngp",
-    steps_per_eval_batch=500,
-    steps_per_save=2000,
-    max_num_iterations=30000,
-    mixed_precision=True,
-    pipeline=DynamicBatchPipelineConfig(
-        datamanager=VanillaDataManagerConfig(
-            _target=VanillaDataManager[DepthDataset],
-            dataparser=DycheckDataParserConfig(),
-            train_num_rays_per_batch=8192,
-        ),
-        model=NerfplayerNGPModelConfig(
-            eval_num_rays_per_chunk=8192,
-            grid_levels=1,
-            alpha_thre=0.0,
-            render_step_size=0.001,
-            disable_scene_contraction=True,
-            near_plane=0.01,
-        ),
-    ),
-    optimizers={
-        "fields": {
-            "optimizer": AdamOptimizerConfig(lr=1e-2, eps=1e-15),
-            "scheduler": None,
-        }
-    },
-    viewer=ViewerConfig(num_rays_per_chunk=64000),
+    viewer=ViewerConfig(),
     vis="viewer",
 )
 
 method_configs["neus"] = TrainerConfig(
     method_name="neus",
     steps_per_eval_image=500,
     steps_per_eval_batch=5000,
@@ -558,15 +582,15 @@
             train_num_rays_per_batch=2048,
             eval_num_rays_per_batch=2048,
             camera_optimizer=CameraOptimizerConfig(
                 mode="SO3xR3", optimizer=AdamOptimizerConfig(lr=6e-4, eps=1e-8, weight_decay=1e-2)
             ),
         ),
         model=NeuSFactoModelConfig(
-            # proposal network allows for signifanctly smaller sdf/color network
+            # proposal network allows for significantly smaller sdf/color network
             sdf_field=SDFFieldConfig(
                 use_grid_feature=True,
                 num_layers=2,
                 num_layers_color=2,
                 hidden_dim=256,
                 bias=0.5,
                 beta_init=0.8,
```

### Comparing `nerfstudio-0.3.1/nerfstudio/data/__init__.py` & `nerfstudio-0.3.2/nerfstudio/data/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/data/datamanagers/__init__.py` & `nerfstudio-0.3.2/nerfstudio/data/datamanagers/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/data/datamanagers/base_datamanager.py` & `nerfstudio-0.3.2/nerfstudio/data/datamanagers/base_datamanager.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,27 +16,29 @@
 Datamanager.
 """
 
 from __future__ import annotations
 
 import functools
 from abc import abstractmethod
+from collections import defaultdict
 from dataclasses import dataclass, field
 from pathlib import Path
 from typing import (
     Any,
     Callable,
     Dict,
     Generic,
     List,
     Literal,
     Optional,
     Tuple,
     Type,
     Union,
+    cast,
 )
 
 import torch
 from torch import nn
 from torch.nn import Parameter
 from torch.utils.data.distributed import DistributedSampler
 from typing_extensions import TypeVar
@@ -70,26 +72,32 @@
     """Default collate function for the cached dataloader.
     Args:
         batch: Batch of samples from the dataset.
     Returns:
         Collated batch.
     """
     images = []
-    masks = []
+    imgdata_lists = defaultdict(list)
     for data in batch:
         image = data.pop("image")
-        mask = data.pop("mask", None)
         images.append(image)
-        if mask is not None:
-            masks.append(mask)
+        topop = []
+        for key, val in data.items():
+            if isinstance(val, torch.Tensor):
+                # if the value has same height and width as the image, assume that it should be collated accordingly.
+                if len(val.shape) >= 2 and val.shape[:2] == image.shape[:2]:
+                    imgdata_lists[key].append(val)
+                    topop.append(key)
+        # now that iteration is complete, the image data items can be removed from the batch
+        for key in topop:
+            del data[key]
 
     new_batch = nerfstudio_collate(batch)
     new_batch["image"] = images
-    if masks:
-        new_batch["mask"] = masks
+    new_batch.update(imgdata_lists)
 
     return new_batch
 
 
 @dataclass
 class DataManagerConfig(InstantiateConfig):
     """Configuration for data manager instantiation; DataManager is in charge of keeping the train/eval dataparsers;
@@ -99,14 +107,16 @@
 
     _target: Type = field(default_factory=lambda: DataManager)
     """Target class to instantiate."""
     data: Optional[Path] = None
     """Source of data, may not be used by all models."""
     camera_optimizer: Optional[CameraOptimizerConfig] = None
     """Specifies the camera pose optimizer used during training. Helpful if poses are noisy."""
+    masks_on_gpu: Optional[bool] = None
+    """Process masks on GPU for speed at the expense of memory, if True."""
 
 
 class DataManager(nn.Module):
     """Generic data manager's abstract class
 
     This version of the data manager is designed be a monolithic way to load data and latents,
     especially since this may contain learnable parameters which need to be shared across the train
@@ -235,39 +245,39 @@
     def next_train(self, step: int) -> Tuple[RayBundle, Dict]:
         """Returns the next batch of data from the train data manager.
 
         Args:
             step: the step number of the eval image to retrieve
         Returns:
             A tuple of the ray bundle for the image, and a dictionary of additional batch information
-            such as the groudtruth image.
+            such as the groundtruth image.
         """
         raise NotImplementedError
 
     @abstractmethod
     def next_eval(self, step: int) -> Tuple[RayBundle, Dict]:
         """Returns the next batch of data from the eval data manager.
 
         Args:
             step: the step number of the eval image to retrieve
         Returns:
             A tuple of the ray bundle for the image, and a dictionary of additional batch information
-            such as the groudtruth image.
+            such as the groundtruth image.
         """
         raise NotImplementedError
 
     @abstractmethod
     def next_eval_image(self, step: int) -> Tuple[int, RayBundle, Dict]:
-        """Retreive the next eval image.
+        """Retrieve the next eval image.
 
         Args:
             step: the step number of the eval image to retrieve
         Returns:
             A tuple of the step number, the ray bundle for the image, and a dictionary of
-            additional batch information such as the groudtruth image.
+            additional batch information such as the groundtruth image.
         """
         raise NotImplementedError
 
     @abstractmethod
     def get_train_rays_per_batch(self) -> int:
         """Returns the number of rays per batch for training."""
         raise NotImplementedError
@@ -320,15 +330,15 @@
     """When not evaluating on all images, number of iterations before picking
     new images. If -1, never pick new images."""
     eval_image_indices: Optional[Tuple[int, ...]] = (0,)
     """Specifies the image indices to use during eval; if None, uses all."""
     camera_optimizer: CameraOptimizerConfig = CameraOptimizerConfig()
     """Specifies the camera pose optimizer used during training. Helpful if poses are noisy, such as for data from
     Record3D."""
-    collate_fn: Callable[[Any], Any] = nerfstudio_collate
+    collate_fn: Callable[[Any], Any] = cast(Any, staticmethod(nerfstudio_collate))
     """Specifies the collate function to use for the train and eval dataloaders."""
     camera_res_scale_factor: float = 1.0
     """The scale factor for scaling spatial data such as images, mask, semantics
     along with relevant information about camera intrinsics
     """
     patch_size: int = 1
     """Size of patch to sample from. If >1, patch-based sampling will be used."""
@@ -376,19 +386,24 @@
         self.test_split = "test" if test_mode in ["test", "inference"] else "val"
         self.dataparser_config = self.config.dataparser
         if self.config.data is not None:
             self.config.dataparser.data = Path(self.config.data)
         else:
             self.config.data = self.config.dataparser.data
         self.dataparser = self.dataparser_config.setup()
+        if test_mode == "inference":
+            self.dataparser.downscale_factor = 1  # Avoid opening images
         self.includes_time = self.dataparser.includes_time
-        self.train_dataparser_outputs = self.dataparser.get_dataparser_outputs(split="train")
+        self.train_dataparser_outputs: DataparserOutputs = self.dataparser.get_dataparser_outputs(split="train")
 
         self.train_dataset = self.create_train_dataset()
         self.eval_dataset = self.create_eval_dataset()
+        self.exclude_batch_keys_from_device = self.train_dataset.exclude_batch_keys_from_device
+        if self.config.masks_on_gpu is True:
+            self.exclude_batch_keys_from_device.remove("mask")
 
         if self.train_dataparser_outputs is not None:
             cameras = self.train_dataparser_outputs.cameras
             if len(cameras) > 1:
                 for i in range(1, len(cameras)):
                     if cameras[0].width != cameras[i].width or cameras[0].height != cameras[i].height:
                         CONSOLE.print("Variable resolution, using variable_res_collate")
@@ -440,14 +455,15 @@
             self.train_dataset,
             num_images_to_sample_from=self.config.train_num_images_to_sample_from,
             num_times_to_repeat_images=self.config.train_num_times_to_repeat_images,
             device=self.device,
             num_workers=self.world_size * 4,
             pin_memory=True,
             collate_fn=self.config.collate_fn,
+            exclude_batch_keys_from_device=self.exclude_batch_keys_from_device,
         )
         self.iter_train_image_dataloader = iter(self.train_image_dataloader)
         self.train_pixel_sampler = self._get_pixel_sampler(self.train_dataset, self.config.train_num_rays_per_batch)
         self.train_camera_optimizer = self.config.camera_optimizer.setup(
             num_cameras=self.train_dataset.cameras.size, device=self.device
         )
         self.train_ray_generator = RayGenerator(
@@ -463,14 +479,15 @@
             self.eval_dataset,
             num_images_to_sample_from=self.config.eval_num_images_to_sample_from,
             num_times_to_repeat_images=self.config.eval_num_times_to_repeat_images,
             device=self.device,
             num_workers=self.world_size * 4,
             pin_memory=True,
             collate_fn=self.config.collate_fn,
+            exclude_batch_keys_from_device=self.exclude_batch_keys_from_device,
         )
         self.iter_eval_image_dataloader = iter(self.eval_image_dataloader)
         self.eval_pixel_sampler = self._get_pixel_sampler(self.eval_dataset, self.config.eval_num_rays_per_batch)
         self.eval_camera_optimizer = self.config.camera_optimizer.setup(
             num_cameras=self.eval_dataset.cameras.size, device=self.device
         )
         self.eval_ray_generator = RayGenerator(
```

### Comparing `nerfstudio-0.3.1/nerfstudio/data/dataparsers/__init__.py` & `nerfstudio-0.3.2/nerfstudio/data/dataparsers/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/data/dataparsers/arkitscenes_dataparser.py` & `nerfstudio-0.3.2/nerfstudio/data/dataparsers/arkitscenes_dataparser.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
     return (ts, Rt)
 
 
 @dataclass
 class ARKitScenesDataParserConfig(DataParserConfig):
     """ARKitScenes dataset config.
     ARKitScenes dataset (http://github.com/apple/ARKitScenes) is a large-scale 3D dataset of indoor scenes.
-    This dataparser uses 3D deteciton subset of the ARKitScenes dataset.
+    This dataparser uses 3D detection subset of the ARKitScenes dataset.
     """
 
     _target: Type = field(default_factory=lambda: ARKitScenes)
     """target class to instantiate"""
     data: Path = Path("data/ARKitScenes/3dod/Validation/41069021")
     """Path to ARKitScenes folder with densely extracted scenes."""
     scale_factor: float = 1.0
```

### Comparing `nerfstudio-0.3.1/nerfstudio/data/dataparsers/base_dataparser.py` & `nerfstudio-0.3.2/nerfstudio/data/dataparsers/base_dataparser.py`

 * *Files 9% similar despite different names*

```diff
@@ -137,34 +137,36 @@
     includes_time: bool = False
 
     def __init__(self, config: DataParserConfig):
         super().__init__()
         self.config = config
 
     @abstractmethod
-    def _generate_dataparser_outputs(self, split: str = "train") -> DataparserOutputs:
+    def _generate_dataparser_outputs(self, split: str = "train", **kwargs: Optional[Dict]) -> DataparserOutputs:
         """Abstract method that returns the dataparser outputs for the given split.
 
         Args:
             split: Which dataset split to generate (train/test).
+            kwargs: kwargs for generating dataparser outputs.
 
         Returns:
             DataparserOutputs containing data for the specified dataset and split
         """
 
-    def get_dataparser_outputs(self, split: str = "train") -> DataparserOutputs:
+    def get_dataparser_outputs(self, split: str = "train", **kwargs: Optional[Dict]) -> DataparserOutputs:
         """Returns the dataparser outputs for the given split.
 
         Args:
             split: Which dataset split to generate (train/test).
+            kwargs: kwargs for generating dataparser outputs.
 
         Returns:
             DataparserOutputs containing data for the specified dataset and split
         """
-        dataparser_outputs = self._generate_dataparser_outputs(split)
+        dataparser_outputs = self._generate_dataparser_outputs(split, **kwargs)
         return dataparser_outputs
 
 
 def transform_poses_to_original_space(
     poses: Float[Tensor, "num_poses 3 4"],
     applied_transform: Float[Tensor, "3 4"],
     applied_scale: float,
```

### Comparing `nerfstudio-0.3.1/nerfstudio/data/dataparsers/blender_dataparser.py` & `nerfstudio-0.3.2/nerfstudio/data/dataparsers/blender_dataparser.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/data/dataparsers/dnerf_dataparser.py` & `nerfstudio-0.3.2/nerfstudio/data/dataparsers/dnerf_dataparser.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/data/dataparsers/dycheck_dataparser.py` & `nerfstudio-0.3.2/nerfstudio/data/dataparsers/dycheck_dataparser.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/data/dataparsers/instant_ngp_dataparser.py` & `nerfstudio-0.3.2/nerfstudio/data/dataparsers/instant_ngp_dataparser.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,15 @@
         num_skipped_image_filenames = 0
         for frame in meta["frames"]:
             fname = data_dir / Path(frame["file_path"])
             # search for png file
             if not fname.exists():
                 fname = data_dir / Path(frame["file_path"] + ".png")
             if not fname.exists():
-                CONSOLE.log(f"couldnt find {fname} image")
+                CONSOLE.log(f"couldn't find {fname} image")
                 num_skipped_image_filenames += 1
             else:
                 if "w" not in meta:
                     img_0 = imageio.imread(fname)
                     h, w = img_0.shape[:2]
                     meta["w"] = w
                     if "h" in meta:
```

### Comparing `nerfstudio-0.3.1/nerfstudio/data/dataparsers/minimal_dataparser.py` & `nerfstudio-0.3.2/nerfstudio/data/dataparsers/minimal_dataparser.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/data/dataparsers/nerfosr_dataparser.py` & `nerfstudio-0.3.2/nerfstudio/data/dataparsers/nerfosr_dataparser.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/data/dataparsers/nerfstudio_dataparser.py` & `nerfstudio-0.3.2/nerfstudio/data/dataparsers/nerfstudio_dataparser.py`

 * *Files 5% similar despite different names*

```diff
@@ -81,15 +81,14 @@
             meta = load_from_json(self.config.data / "transforms.json")
             data_dir = self.config.data
 
         image_filenames = []
         mask_filenames = []
         depth_filenames = []
         poses = []
-        num_skipped_image_filenames = 0
 
         fx_fixed = "fl_x" in meta
         fy_fixed = "fl_y" in meta
         cx_fixed = "cx" in meta
         cy_fixed = "cy" in meta
         height_fixed = "h" in meta
         width_fixed = "w" in meta
@@ -105,17 +104,14 @@
         height = []
         width = []
         distort = []
 
         for frame in meta["frames"]:
             filepath = Path(frame["file_path"])
             fname = self._get_fname(filepath, data_dir)
-            if not fname.exists():
-                num_skipped_image_filenames += 1
-                continue
 
             if not fx_fixed:
                 assert "fl_x" in frame, "fx not specified in frame"
                 fx.append(float(frame["fl_x"]))
             if not fy_fixed:
                 assert "fl_y" in frame, "fy not specified in frame"
                 fy.append(float(frame["fl_y"]))
@@ -155,22 +151,14 @@
                 mask_filenames.append(mask_fname)
 
             if "depth_file_path" in frame:
                 depth_filepath = Path(frame["depth_file_path"])
                 depth_fname = self._get_fname(depth_filepath, data_dir, downsample_folder_prefix="depths_")
                 depth_filenames.append(depth_fname)
 
-        if num_skipped_image_filenames >= 0:
-            CONSOLE.log(f"Skipping {num_skipped_image_filenames} files in dataset split {split}.")
-        assert (
-            len(image_filenames) != 0
-        ), """
-        No image files found. 
-        You should check the file_paths in the transforms.json file to make sure they are correct.
-        """
         assert len(mask_filenames) == 0 or (
             len(mask_filenames) == len(image_filenames)
         ), """
         Different number of image and mask filenames.
         You should check that mask_path is specified for every frame (or zero frames) in transforms.json.
         """
         assert len(depth_filenames) == 0 or (
```

### Comparing `nerfstudio-0.3.1/nerfstudio/data/dataparsers/nuscenes_dataparser.py` & `nerfstudio-0.3.2/nerfstudio/data/dataparsers/nuscenes_dataparser.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/data/dataparsers/phototourism_dataparser.py` & `nerfstudio-0.3.2/nerfstudio/data/dataparsers/phototourism_dataparser.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/data/dataparsers/scannet_dataparser.py` & `nerfstudio-0.3.2/nerfstudio/data/dataparsers/scannet_dataparser.py`

 * *Files 3% similar despite different names*

```diff
@@ -85,18 +85,18 @@
         h, w, _ = first_img.shape
 
         image_filenames, depth_filenames, intrinsics, poses = [], [], [], []
 
         K = np.loadtxt(self.config.data / "intrinsic" / "intrinsic_color.txt")
         for img, depth, pose in zip(img_dir_sorted, depth_dir_sorted, pose_dir_sorted):
             pose = np.loadtxt(pose)
-            pose[0:3, 1:3] *= -1
-            pose = pose[np.array([1, 0, 2, 3]), :]
-            pose[2, :] *= -1
-
+            pose = np.array(pose).reshape(4, 4)
+            pose[:3, 1] *= -1
+            pose[:3, 2] *= -1
+            pose = torch.from_numpy(pose).float()
             # We cannot accept files directly, as some of the poses are invalid
             if np.isinf(pose).any():
                 continue
 
             poses.append(pose)
             intrinsics.append(K)
             image_filenames.append(img)
```

### Comparing `nerfstudio-0.3.1/nerfstudio/data/dataparsers/sdfstudio_dataparser.py` & `nerfstudio-0.3.2/nerfstudio/data/dataparsers/sdfstudio_dataparser.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/data/dataparsers/sitcoms3d_dataparser.py` & `nerfstudio-0.3.2/nerfstudio/data/dataparsers/sitcoms3d_dataparser.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/data/datasets/__init__.py` & `nerfstudio-0.3.2/nerfstudio/data/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/data/datasets/base_dataset.py` & `nerfstudio-0.3.2/nerfstudio/data/datasets/base_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,15 @@
     """Dataset that returns images.
 
     Args:
         dataparser_outputs: description of where and how to read input images.
         scale_factor: The scaling factor for the dataparser outputs
     """
 
+    exclude_batch_keys_from_device: List[str] = ["image", "mask"]
     cameras: Cameras
 
     def __init__(self, dataparser_outputs: DataparserOutputs, scale_factor: float = 1.0):
         super().__init__()
         self._dataparser_outputs = dataparser_outputs
         self.scale_factor = scale_factor
         self.scene_box = deepcopy(dataparser_outputs.scene_box)
```

### Comparing `nerfstudio-0.3.1/nerfstudio/data/datasets/depth_dataset.py` & `nerfstudio-0.3.2/nerfstudio/data/datasets/depth_dataset.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,14 +27,16 @@
     """Dataset that returns images and depths.
 
     Args:
         dataparser_outputs: description of where and how to read input images.
         scale_factor: The scaling factor for the dataparser outputs.
     """
 
+    exclude_batch_keys_from_device = InputDataset.exclude_batch_keys_from_device + ["depth_image"]
+
     def __init__(self, dataparser_outputs: DataparserOutputs, scale_factor: float = 1.0):
         super().__init__(dataparser_outputs, scale_factor)
         assert (
             "depth_filenames" in dataparser_outputs.metadata.keys()
             and dataparser_outputs.metadata["depth_filenames"] is not None
         )
         self.depth_filenames = self.metadata["depth_filenames"]
```

### Comparing `nerfstudio-0.3.1/nerfstudio/data/datasets/sdf_dataset.py` & `nerfstudio-0.3.2/nerfstudio/data/datasets/sdf_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,16 @@
     """Dataset that returns images and depths.
 
     Args:
         dataparser_outputs: description of where and how to read input images.
         scale_factor: The scaling factor for the dataparser outputs.
     """
 
+    exclude_batch_keys_from_device = InputDataset.exclude_batch_keys_from_device + ["depth", "normal"]
+
     def __init__(self, dataparser_outputs: DataparserOutputs, scale_factor: float = 1.0):
         super().__init__(dataparser_outputs, scale_factor)
 
         # can be none if monoprior not included
         self.depth_filenames = self.metadata["depth_filenames"]
         self.normal_filenames = self.metadata["normal_filenames"]
         self.camera_to_worlds = self.metadata["camera_to_worlds"]
```

### Comparing `nerfstudio-0.3.1/nerfstudio/data/datasets/semantic_dataset.py` & `nerfstudio-0.3.2/nerfstudio/data/datasets/semantic_dataset.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,14 +28,16 @@
 class SemanticDataset(InputDataset):
     """Dataset that returns images and semantics and masks.
 
     Args:
         dataparser_outputs: description of where and how to read input images.
     """
 
+    exclude_batch_keys_from_device = InputDataset.exclude_batch_keys_from_device + ["mask", "semantics"]
+
     def __init__(self, dataparser_outputs: DataparserOutputs, scale_factor: float = 1.0):
         super().__init__(dataparser_outputs, scale_factor)
         assert "semantics" in dataparser_outputs.metadata.keys() and isinstance(self.metadata["semantics"], Semantics)
         self.semantics = self.metadata["semantics"]
         self.mask_indices = torch.tensor(
             [self.semantics.classes.index(mask_class) for mask_class in self.semantics.mask_classes]
         ).view(1, 1, -1)
```

### Comparing `nerfstudio-0.3.1/nerfstudio/data/pixel_samplers.py` & `nerfstudio-0.3.2/nerfstudio/data/pixel_samplers.py`

 * *Files 1% similar despite different names*

```diff
@@ -257,15 +257,15 @@
 
     def __init__(self, num_rays_per_batch: int, keep_full_image: bool = False, **kwargs) -> None:
         self.patch_size = kwargs["patch_size"]
         num_rays = (num_rays_per_batch // (self.patch_size**2)) * (self.patch_size**2)
         super().__init__(num_rays, keep_full_image, **kwargs)
 
     def set_num_rays_per_batch(self, num_rays_per_batch: int):
-        """Set the number of rays to sample per batch. Overrided to deal with patch-based sampling.
+        """Set the number of rays to sample per batch. Overridden to deal with patch-based sampling.
 
         Args:
             num_rays_per_batch: number of rays to sample per batch
         """
         self.num_rays_per_batch = (num_rays_per_batch // (self.patch_size**2)) * (self.patch_size**2)
 
     # overrides base method
```

### Comparing `nerfstudio-0.3.1/nerfstudio/data/scene_box.py` & `nerfstudio-0.3.2/nerfstudio/data/scene_box.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/data/utils/__init__.py` & `nerfstudio-0.3.2/nerfstudio/data/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/data/utils/colmap_parsing_utils.py` & `nerfstudio-0.3.2/nerfstudio/data/utils/colmap_parsing_utils.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/data/utils/data_utils.py` & `nerfstudio-0.3.2/nerfstudio/data/utils/data_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
         filepath: Path to depth image.
         height: Target depth image height.
         width: Target depth image width.
         scale_factor: Factor by which to scale depth image.
         interpolation: Depth value interpolation for resizing.
 
     Returns:
-        Depth image torch tensor with shape [width, height, 1].
+        Depth image torch tensor with shape [height, width, 1].
     """
     if filepath.suffix == ".npy":
         image = np.load(filepath) * scale_factor
         image = cv2.resize(image, (width, height), interpolation=interpolation)
     else:
         image = cv2.imread(str(filepath.absolute()), cv2.IMREAD_ANYDEPTH)
         image = image.astype(np.float64) * scale_factor
```

### Comparing `nerfstudio-0.3.1/nerfstudio/data/utils/dataloaders.py` & `nerfstudio-0.3.2/nerfstudio/data/utils/dataloaders.py`

 * *Files 15% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 """
 
 # for multithreading
 import concurrent.futures
 import multiprocessing
 import random
 from abc import abstractmethod
-from typing import Any, Callable, Dict, Optional, Sized, Tuple, Union
+from typing import Any, Callable, Dict, List, Optional, Sized, Tuple, Union
 
 import torch
 from rich.progress import track
 from torch.utils.data import Dataset
 from torch.utils.data.dataloader import DataLoader
 
 from nerfstudio.cameras.cameras import Cameras
@@ -51,26 +51,30 @@
     def __init__(
         self,
         dataset: Dataset,
         num_images_to_sample_from: int = -1,
         num_times_to_repeat_images: int = -1,
         device: Union[torch.device, str] = "cpu",
         collate_fn: Callable[[Any], Any] = nerfstudio_collate,
+        exclude_batch_keys_from_device: Optional[List[str]] = None,
         **kwargs,
     ):
+        if exclude_batch_keys_from_device is None:
+            exclude_batch_keys_from_device = ["image"]
         self.dataset = dataset
         assert isinstance(self.dataset, Sized)
 
         super().__init__(dataset=dataset, **kwargs)  # This will set self.dataset
         self.num_times_to_repeat_images = num_times_to_repeat_images
         self.cache_all_images = (num_images_to_sample_from == -1) or (num_images_to_sample_from >= len(self.dataset))
         self.num_images_to_sample_from = len(self.dataset) if self.cache_all_images else num_images_to_sample_from
         self.device = device
         self.collate_fn = collate_fn
         self.num_workers = kwargs.get("num_workers", 0)
+        self.exclude_batch_keys_from_device = exclude_batch_keys_from_device
 
         self.num_repeated = self.num_times_to_repeat_images  # starting value
         self.first_time = True
 
         self.cached_collated_batch = None
         if self.cache_all_images:
             CONSOLE.print(f"Caching all {len(self.dataset)} images.")
@@ -114,15 +118,17 @@
 
         return batch_list
 
     def _get_collated_batch(self):
         """Returns a collated batch."""
         batch_list = self._get_batch_list()
         collated_batch = self.collate_fn(batch_list)
-        collated_batch = get_dict_to_torch(collated_batch, device=self.device, exclude=["image"])
+        collated_batch = get_dict_to_torch(
+            collated_batch, device=self.device, exclude=self.exclude_batch_keys_from_device
+        )
         return collated_batch
 
     def __iter__(self):
         while True:
             if self.cache_all_images:
                 collated_batch = self.cached_collated_batch
             elif self.first_time or (
```

### Comparing `nerfstudio-0.3.1/nerfstudio/data/utils/nerfstudio_collate.py` & `nerfstudio-0.3.2/nerfstudio/data/utils/nerfstudio_collate.py`

 * *Files 8% similar despite different names*

```diff
@@ -158,14 +158,21 @@
         # If no batch dimension exists, then we need to stack everything and create a batch dimension on 0th dim
         if elem.shape == ():
             op = torch.stack
         # If batch dimension exists, then we need to concatenate along the 0th dimension
         else:
             op = torch.cat
 
+        # Create metadata dictionary
+        metadata_keys = batch[0].metadata.keys()
+        assert all(
+            (cam.metadata.keys() == metadata_keys for cam in batch)
+        ), "All cameras must have the same metadata keys."
+        metadata = {key: op([cam.metadata[key] for cam in batch], dim=0) for key in metadata_keys}
+
         return Cameras(
             op([cameras.camera_to_worlds for cameras in batch], dim=0),
             op([cameras.fx for cameras in batch], dim=0),
             op([cameras.fy for cameras in batch], dim=0),
             op([cameras.cx for cameras in batch], dim=0),
             op([cameras.cy for cameras in batch], dim=0),
             height=op([cameras.height for cameras in batch], dim=0),
@@ -180,14 +187,15 @@
                 dim=0,
             ),
             camera_type=op([cameras.camera_type for cameras in batch], dim=0),
             times=torch.stack(
                 [cameras.times if cameras.times is not None else -torch.ones_like(cameras.times) for cameras in batch],
                 dim=0,
             ),
+            metadata=metadata,
         )
 
     for type_key in extra_mappings:
         if isinstance(elem, type_key):
             return extra_mappings[type_key](batch)
 
     raise TypeError(NERFSTUDIO_COLLATE_ERR_MSG_FORMAT.format(elem_type))
```

### Comparing `nerfstudio-0.3.1/nerfstudio/engine/__init__.py` & `nerfstudio-0.3.2/nerfstudio/engine/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/engine/callbacks.py` & `nerfstudio-0.3.2/nerfstudio/engine/callbacks.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 
 
 class TrainingCallbackLocation(Enum):
     """Enum for specifying where the training callback should be run."""
 
     BEFORE_TRAIN_ITERATION = auto()
     AFTER_TRAIN_ITERATION = auto()
+    AFTER_TRAIN = auto()
 
 
 class TrainingCallback:
     """Callback class used during training.
     The function 'func' with 'args' and 'kwargs' will be called every 'update_every_num_iters' training iterations,
     including at iteration 0. The function is called after the training iteration.
 
@@ -93,14 +94,16 @@
         """
         if self.update_every_num_iters is not None:
             if step % self.update_every_num_iters == 0:
                 self.func(*self.args, **self.kwargs, step=step)
         elif self.iters is not None:
             if step in self.iters:
                 self.func(*self.args, **self.kwargs, step=step)
+        else:
+            self.func(*self.args, **self.kwargs, step=step)
 
     def run_callback_at_location(self, step: int, location: TrainingCallbackLocation) -> None:
         """Runs the callback if it's supposed to be run at the given location.
 
         Args:
             step: current iteration step
             location: when to run callback (before/after iteration)
```

### Comparing `nerfstudio-0.3.1/nerfstudio/engine/optimizers.py` & `nerfstudio-0.3.2/nerfstudio/engine/optimizers.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/engine/schedulers.py` & `nerfstudio-0.3.2/nerfstudio/engine/schedulers.py`

 * *Files 0% similar despite different names*

```diff
@@ -118,15 +118,15 @@
             lr_final = lr_init
         else:
             lr_final = self.config.lr_final
 
         def func(step):
             if step < self.config.warmup_steps:
                 if self.config.ramp == "cosine":
-                    lr = self.config.lr_pre_warmup + (1 - self.config.lr_pre_warmup) * np.sin(
+                    lr = self.config.lr_pre_warmup + (lr_init - self.config.lr_pre_warmup) * np.sin(
                         0.5 * np.pi * np.clip(step / self.config.warmup_steps, 0, 1)
                     )
                 else:
                     lr = (
                         self.config.lr_pre_warmup
                         + (lr_init - self.config.lr_pre_warmup) * step / self.config.warmup_steps
                     )
```

### Comparing `nerfstudio-0.3.1/nerfstudio/engine/trainer.py` & `nerfstudio-0.3.2/nerfstudio/engine/trainer.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,31 +29,25 @@
 import torch
 from rich import box, style
 from rich.panel import Panel
 from rich.table import Table
 from torch.cuda.amp.grad_scaler import GradScaler
 
 from nerfstudio.configs.experiment_config import ExperimentConfig
-from nerfstudio.engine.callbacks import (
-    TrainingCallback,
-    TrainingCallbackAttributes,
-    TrainingCallbackLocation,
-)
+from nerfstudio.data.datamanagers.base_datamanager import VanillaDataManager
+from nerfstudio.engine.callbacks import TrainingCallback, TrainingCallbackAttributes, TrainingCallbackLocation
 from nerfstudio.engine.optimizers import Optimizers
 from nerfstudio.pipelines.base_pipeline import VanillaPipeline
 from nerfstudio.utils import profiler, writer
-from nerfstudio.utils.decorators import (
-    check_eval_enabled,
-    check_main_thread,
-    check_viewer_enabled,
-)
+from nerfstudio.utils.decorators import check_eval_enabled, check_main_thread, check_viewer_enabled
 from nerfstudio.utils.misc import step_check
 from nerfstudio.utils.rich_utils import CONSOLE
 from nerfstudio.utils.writer import EventName, TimeWriter
 from nerfstudio.viewer.server.viewer_state import ViewerState
+from nerfstudio.viewer_beta.viewer import Viewer as ViewerBetaState
 
 TRAIN_INTERATION_OUTPUT = Tuple[torch.Tensor, Dict[str, torch.Tensor], Dict[str, torch.Tensor]]
 TORCH_DEVICE = str
 
 
 @dataclass
 class TrainerConfig(ExperimentConfig):
@@ -84,14 +78,16 @@
     """Optionally specify model step to load from; if none, will find most recent model in load_dir."""
     load_config: Optional[Path] = None
     """Path to config YAML file."""
     load_checkpoint: Optional[Path] = None
     """Path to checkpoint file."""
     log_gradients: bool = False
     """Optionally log gradients during training"""
+    gradient_accumulation_steps: int = 1
+    """Number of steps to accumulate gradients over."""
 
 
 class Trainer:
     """Trainer class
 
     Args:
         config: The configuration object.
@@ -114,18 +110,21 @@
     callbacks: List[TrainingCallback]
 
     def __init__(self, config: TrainerConfig, local_rank: int = 0, world_size: int = 1) -> None:
         self.train_lock = Lock()
         self.config = config
         self.local_rank = local_rank
         self.world_size = world_size
-        self.device: TORCH_DEVICE = "cpu" if world_size == 0 else f"cuda:{local_rank}"
+        self.device: TORCH_DEVICE = config.machine.device_type
+        if self.device == "cuda":
+            self.device += f":{local_rank}"
         self.mixed_precision: bool = self.config.mixed_precision
         self.use_grad_scaler: bool = self.mixed_precision or self.config.use_grad_scaler
         self.training_state: Literal["training", "paused", "completed"] = "training"
+        self.gradient_accumulation_steps: int = self.config.gradient_accumulation_steps
 
         if self.device == "cpu":
             self.mixed_precision = False
             CONSOLE.print("Mixed precision is disabled for CPU training.")
         self._start_step: int = 0
         # optimizers
         self.grad_scaler = GradScaler(enabled=self.use_grad_scaler)
@@ -143,15 +142,19 @@
         Args:
             test_mode:
                 'val': loads train/val datasets into memory
                 'test': loads train/test datasets into memory
                 'inference': does not load any dataset into memory
         """
         self.pipeline = self.config.pipeline.setup(
-            device=self.device, test_mode=test_mode, world_size=self.world_size, local_rank=self.local_rank
+            device=self.device,
+            test_mode=test_mode,
+            world_size=self.world_size,
+            local_rank=self.local_rank,
+            grad_scaler=self.grad_scaler,
         )
         self.optimizers = self.setup_optimizers()
 
         # set up viewer if enabled
         viewer_log_path = self.base_dir / self.config.viewer.relative_log_filename
         self.viewer_state, banner_messages = None, None
         if self.config.is_viewer_enabled() and self.local_rank == 0:
@@ -163,14 +166,24 @@
                 log_filename=viewer_log_path,
                 datapath=datapath,
                 pipeline=self.pipeline,
                 trainer=self,
                 train_lock=self.train_lock,
             )
             banner_messages = [f"Viewer at: {self.viewer_state.viewer_url}"]
+        if self.config.is_viewer_beta_enabled() and self.local_rank == 0:
+            self.viewer_state = ViewerBetaState(
+                self.config.viewer,
+                log_filename=viewer_log_path,
+                datapath=self.base_dir,
+                pipeline=self.pipeline,
+                trainer=self,
+                train_lock=self.train_lock,
+            )
+            banner_messages = [f"Viewer Beta at: {self.viewer_state.viewer_url}"]
         self._check_viewer_warnings()
 
         self._load_checkpoint()
 
         self.callbacks = self.pipeline.get_training_callbacks(
             TrainingCallbackAttributes(
                 optimizers=self.optimizers,
@@ -211,17 +224,19 @@
             }
         return Optimizers(optimizer_config, param_groups)
 
     def train(self) -> None:
         """Train the model."""
         assert self.pipeline.datamanager.train_dataset is not None, "Missing DatsetInputs"
 
-        self.pipeline.datamanager.train_dataparser_outputs.save_dataparser_transform(
-            self.base_dir / "dataparser_transforms.json"
-        )
+        # don't want to call save_dataparser_transform if pipeline's datamanager does not have a dataparser
+        if isinstance(self.pipeline.datamanager, VanillaDataManager):
+            self.pipeline.datamanager.train_dataparser_outputs.save_dataparser_transform(
+                self.base_dir / "dataparser_transforms.json"
+            )
 
         self._init_viewer_state()
         with TimeWriter(writer, EventName.TOTAL_TRAIN_TIME):
             num_iterations = self.config.max_num_iterations
             step = 0
             for step in range(self._start_step, self._start_step + num_iterations):
                 while self.training_state == "paused":
@@ -293,22 +308,26 @@
             box=box.MINIMAL,
             title_style=style.Style(bold=True),
         )
         table.add_row("Config File", str(self.config.get_base_dir() / "config.yml"))
         table.add_row("Checkpoint Directory", str(self.checkpoint_dir))
         CONSOLE.print(Panel(table, title="[bold][green]:tada: Training Finished :tada:[/bold]", expand=False))
 
+        # after train end callbacks
+        for callback in self.callbacks:
+            callback.run_callback_at_location(step=step, location=TrainingCallbackLocation.AFTER_TRAIN)
+
         if not self.config.viewer.quit_on_train_completion:
             self._train_complete_viewer()
 
     @check_main_thread
     def _check_viewer_warnings(self) -> None:
         """Helper to print out any warnings regarding the way the viewer/loggers are enabled"""
         if (
-            self.config.is_viewer_enabled()
+            (self.config.is_viewer_enabled() or self.config.is_viewer_beta_enabled())
             and not self.config.is_tensorboard_enabled()
             and not self.config.is_wandb_enabled()
         ):
             string: str = (
                 "[NOTE] Not running eval iterations since only viewer is enabled.\n"
                 "Use [yellow]--vis {wandb, tensorboard, viewer+wandb, viewer+tensorboard}[/yellow] to run with eval."
             )
@@ -437,40 +456,44 @@
 
         Args:
             step: Current training step.
         """
 
         self.optimizers.zero_grad_all()
         cpu_or_cuda_str: str = self.device.split(":")[0]
-
-        with torch.autocast(device_type=cpu_or_cuda_str, enabled=self.mixed_precision):
-            _, loss_dict, metrics_dict = self.pipeline.get_train_loss_dict(step=step)
-            loss = functools.reduce(torch.add, loss_dict.values())
-        self.grad_scaler.scale(loss).backward()  # type: ignore
+        assert (
+            self.gradient_accumulation_steps > 0
+        ), f"gradient_accumulation_steps must be > 0, not {self.gradient_accumulation_steps}"
+        for _ in range(self.gradient_accumulation_steps):
+            with torch.autocast(device_type=cpu_or_cuda_str, enabled=self.mixed_precision):
+                _, loss_dict, metrics_dict = self.pipeline.get_train_loss_dict(step=step)
+                loss = functools.reduce(torch.add, loss_dict.values())
+                loss /= self.gradient_accumulation_steps
+            self.grad_scaler.scale(loss).backward()  # type: ignore
         self.optimizers.optimizer_scaler_step_all(self.grad_scaler)
 
         if self.config.log_gradients:
             total_grad = 0
             for tag, value in self.pipeline.model.named_parameters():
                 assert tag != "Total"
                 if value.grad is not None:
                     grad = value.grad.norm()
-                    metrics_dict[f"Gradients/{tag}"] = grad
+                    metrics_dict[f"Gradients/{tag}"] = grad  # type: ignore
                     total_grad += grad
 
-            metrics_dict["Gradients/Total"] = cast(torch.Tensor, total_grad)
+            metrics_dict["Gradients/Total"] = cast(torch.Tensor, total_grad)  # type: ignore
 
         scale = self.grad_scaler.get_scale()
         self.grad_scaler.update()
         # If the gradient scaler is decreased, no optimization step is performed so we should not step the scheduler.
         if scale <= self.grad_scaler.get_scale():
             self.optimizers.scheduler_step_all(step)
 
         # Merging loss and metrics dict into a single output.
-        return loss, loss_dict, metrics_dict
+        return loss, loss_dict, metrics_dict  # type: ignore
 
     @check_eval_enabled
     @profiler.time_function
     def eval_iteration(self, step: int) -> None:
         """Run one iteration with different batch/image/all image evaluations depending on step size.
 
         Args:
```

### Comparing `nerfstudio-0.3.1/nerfstudio/exporter/__init__.py` & `nerfstudio-0.3.2/nerfstudio/exporter/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/exporter/exporter_utils.py` & `nerfstudio-0.3.2/nerfstudio/exporter/exporter_utils.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/exporter/marching_cubes.py` & `nerfstudio-0.3.2/nerfstudio/exporter/marching_cubes.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/exporter/texture_utils.py` & `nerfstudio-0.3.2/nerfstudio/exporter/texture_utils.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/exporter/tsdf_utils.py` & `nerfstudio-0.3.2/nerfstudio/exporter/tsdf_utils.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/field_components/__init__.py` & `nerfstudio-0.3.2/nerfstudio/field_components/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/field_components/activations.py` & `nerfstudio-0.3.2/nerfstudio/field_components/activations.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/field_components/base_field_component.py` & `nerfstudio-0.3.2/nerfstudio/field_components/base_field_component.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/field_components/embedding.py` & `nerfstudio-0.3.2/nerfstudio/field_components/embedding.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/field_components/encodings.py` & `nerfstudio-0.3.2/nerfstudio/field_components/encodings.py`

 * *Files 3% similar despite different names*

```diff
@@ -105,32 +105,50 @@
         num_frequencies: Number of encoded frequencies per axis
         min_freq_exp: Minimum frequency exponent
         max_freq_exp: Maximum frequency exponent
         include_input: Append the input coordinate to the encoding
     """
 
     def __init__(
-        self, in_dim: int, num_frequencies: int, min_freq_exp: float, max_freq_exp: float, include_input: bool = False
+        self,
+        in_dim: int,
+        num_frequencies: int,
+        min_freq_exp: float,
+        max_freq_exp: float,
+        include_input: bool = False,
+        implementation: Literal["tcnn", "torch"] = "torch",
     ) -> None:
         super().__init__(in_dim)
 
         self.num_frequencies = num_frequencies
         self.min_freq = min_freq_exp
         self.max_freq = max_freq_exp
         self.include_input = include_input
 
+        self.tcnn_encoding = None
+        if implementation == "tcnn" and not TCNN_EXISTS:
+            print_tcnn_speed_warning("NeRFEncoding")
+        elif implementation == "tcnn":
+            encoding_config = {"otype": "Frequency", "n_frequencies": num_frequencies}
+            assert min_freq_exp == 0, "tcnn only supports min_freq_exp = 0"
+            assert max_freq_exp == num_frequencies - 1, "tcnn only supports max_freq_exp = num_frequencies - 1"
+            self.tcnn_encoding = tcnn.Encoding(
+                n_input_dims=in_dim,
+                encoding_config=encoding_config,
+            )
+
     def get_out_dim(self) -> int:
         if self.in_dim is None:
             raise ValueError("Input dimension has not been set")
         out_dim = self.in_dim * self.num_frequencies * 2
         if self.include_input:
             out_dim += self.in_dim
         return out_dim
 
-    def forward(
+    def pytorch_fwd(
         self,
         in_tensor: Float[Tensor, "*bs input_dim"],
         covs: Optional[Float[Tensor, "*bs input_dim input_dim"]] = None,
     ) -> Float[Tensor, "*bs output_dim"]:
         """Calculates NeRF encoding. If covariances are provided the encodings will be integrated as proposed
             in mip-NeRF.
 
@@ -154,14 +172,21 @@
                 torch.cat([scaled_inputs, scaled_inputs + torch.pi / 2.0], dim=-1), torch.cat(2 * [input_var], dim=-1)
             )
 
         if self.include_input:
             encoded_inputs = torch.cat([encoded_inputs, in_tensor], dim=-1)
         return encoded_inputs
 
+    def forward(
+        self, in_tensor: Float[Tensor, "*bs input_dim"], covs: Optional[Float[Tensor, "*bs input_dim input_dim"]] = None
+    ) -> Float[Tensor, "*bs output_dim"]:
+        if self.tcnn_encoding is not None:
+            return self.tcnn_encoding(in_tensor)
+        return self.pytorch_fwd(in_tensor, covs)
+
 
 class RFFEncoding(Encoding):
     """Random Fourier Feature encoding. Supports integrated encodings.
 
     Args:
         in_dim: Input dimension of tensor
         num_frequencies: Number of encoding frequencies
@@ -235,15 +260,15 @@
         self,
         num_levels: int = 16,
         min_res: int = 16,
         max_res: int = 1024,
         log2_hashmap_size: int = 19,
         features_per_level: int = 2,
         hash_init_scale: float = 0.001,
-        implementation: Literal["tcnn", "torch"] = "tcnn",
+        implementation: Literal["tcnn", "torch"] = "torch",
         interpolation: Optional[Literal["Nearest", "Linear", "Smoothstep"]] = None,
     ) -> None:
         super().__init__(in_dim=3)
         self.num_levels = num_levels
         self.features_per_level = features_per_level
         self.log2_hashmap_size = log2_hashmap_size
         self.hash_table_size = 2**log2_hashmap_size
@@ -254,15 +279,15 @@
 
         self.hash_offset = levels * self.hash_table_size
         self.hash_table = torch.rand(size=(self.hash_table_size * num_levels, features_per_level)) * 2 - 1
         self.hash_table *= hash_init_scale
         self.hash_table = nn.Parameter(self.hash_table)
 
         self.tcnn_encoding = None
-        if not TCNN_EXISTS and implementation == "tcnn":
+        if implementation == "tcnn" and not TCNN_EXISTS:
             print_tcnn_speed_warning("HashEncoding")
         elif implementation == "tcnn":
             encoding_config = {
                 "otype": "HashGrid",
                 "n_levels": self.num_levels,
                 "n_features_per_level": self.features_per_level,
                 "log2_hashmap_size": self.log2_hashmap_size,
@@ -273,15 +298,15 @@
                 encoding_config["interpolation"] = interpolation
 
             self.tcnn_encoding = tcnn.Encoding(
                 n_input_dims=3,
                 encoding_config=encoding_config,
             )
 
-        if not TCNN_EXISTS or self.tcnn_encoding is None:
+        if self.tcnn_encoding is None:
             assert (
                 interpolation is None or interpolation == "Linear"
             ), f"interpolation '{interpolation}' is not supported for torch encoding backend"
 
     def get_out_dim(self) -> int:
         return self.num_levels * self.features_per_level
 
@@ -344,15 +369,15 @@
         encoded_value = f0312 * offset[..., 2:3] + f4756 * (
             1 - offset[..., 2:3]
         )  # [..., num_levels, features_per_level]
 
         return torch.flatten(encoded_value, start_dim=-2, end_dim=-1)  # [..., num_levels * features_per_level]
 
     def forward(self, in_tensor: Float[Tensor, "*bs input_dim"]) -> Float[Tensor, "*bs output_dim"]:
-        if TCNN_EXISTS and self.tcnn_encoding is not None:
+        if self.tcnn_encoding is not None:
             return self.tcnn_encoding(in_tensor)
         return self.pytorch_fwd(in_tensor)
 
 
 class TensorCPEncoding(Encoding):
     """Learned CANDECOMP/PARFAC (CP) decomposition encoding used in TensoRF
 
@@ -643,21 +668,40 @@
 class SHEncoding(Encoding):
     """Spherical harmonic encoding
 
     Args:
         levels: Number of spherical harmonic levels to encode.
     """
 
-    def __init__(self, levels: int = 4) -> None:
+    def __init__(self, levels: int = 4, implementation: Literal["tcnn", "torch"] = "torch") -> None:
         super().__init__(in_dim=3)
 
         if levels <= 0 or levels > 4:
             raise ValueError(f"Spherical harmonic encoding only supports 1 to 4 levels, requested {levels}")
 
         self.levels = levels
 
+        self.tcnn_encoding = None
+        if implementation == "tcnn" and not TCNN_EXISTS:
+            print_tcnn_speed_warning("SHEncoding")
+        elif implementation == "tcnn":
+            encoding_config = {
+                "otype": "SphericalHarmonics",
+                "degree": levels,
+            }
+            self.tcnn_encoding = tcnn.Encoding(
+                n_input_dims=3,
+                encoding_config=encoding_config,
+            )
+
     def get_out_dim(self) -> int:
         return self.levels**2
 
     @torch.no_grad()
-    def forward(self, in_tensor: Float[Tensor, "*bs input_dim"]) -> Float[Tensor, "*bs output_dim"]:
+    def pytorch_fwd(self, in_tensor: Float[Tensor, "*bs input_dim"]) -> Float[Tensor, "*bs output_dim"]:
+        """Forward pass using pytorch. Significantly slower than TCNN implementation."""
         return components_from_spherical_harmonics(levels=self.levels, directions=in_tensor)
+
+    def forward(self, in_tensor: Float[Tensor, "*bs input_dim"]) -> Float[Tensor, "*bs output_dim"]:
+        if self.tcnn_encoding is not None:
+            return self.tcnn_encoding(in_tensor)
+        return self.pytorch_fwd(in_tensor)
```

### Comparing `nerfstudio-0.3.1/nerfstudio/field_components/field_heads.py` & `nerfstudio-0.3.2/nerfstudio/field_components/field_heads.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 
     RGB = "rgb"
     SH = "sh"
     DENSITY = "density"
     NORMALS = "normals"
     PRED_NORMALS = "pred_normals"
     UNCERTAINTY = "uncertainty"
+    BACKGROUND_RGB = "background_rgb"
     TRANSIENT_RGB = "transient_rgb"
     TRANSIENT_DENSITY = "transient_density"
     SEMANTICS = "semantics"
     SDF = "sdf"
     ALPHA = "alpha"
     GRADIENT = "gradient"
```

### Comparing `nerfstudio-0.3.1/nerfstudio/field_components/mlp.py` & `nerfstudio-0.3.2/nerfstudio/field_components/temporal_distortions.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,91 +8,85 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""
-Multi Layer Perceptron
-"""
-from typing import Optional, Set, Tuple
+"""Space distortions which occur as a function of time."""
+
+import abc
+from enum import Enum
+from typing import Any, Dict, Tuple
 
 import torch
 from jaxtyping import Float
 from torch import Tensor, nn
 
-from nerfstudio.field_components.base_field_component import FieldComponent
+from nerfstudio.field_components.encodings import Encoding, NeRFEncoding
+from nerfstudio.field_components.mlp import MLP
+
+
+class TemporalDistortion(nn.Module):
+    """Apply spatial distortions as a function of time"""
+
+    @abc.abstractmethod
+    def forward(self, positions: Float[Tensor, "*bs 3"], times: Float[Tensor, "*bs 1"]) -> Float[Tensor, "*bs 3"]:
+        """
+        Args:
+            positions: Samples to translate as a function of time
+            times: times for each sample
+
+        Returns:
+            Translated positions.
+        """
+
+
+class TemporalDistortionKind(Enum):
+    """Possible temporal distortion names"""
+
+    DNERF = "dnerf"
 
+    def to_temporal_distortion(self, config: Dict[str, Any]) -> TemporalDistortion:
+        """Converts this kind to a temporal distortion"""
+        if self == TemporalDistortionKind.DNERF:
+            return DNeRFDistortion(**config)
+        raise NotImplementedError(f"Unknown temporal distortion kind {self}")
 
-class MLP(FieldComponent):
-    """Multilayer perceptron
 
+class DNeRFDistortion(TemporalDistortion):
+    """Optimizable temporal deformation using an MLP.
     Args:
-        in_dim: Input layer dimension
-        num_layers: Number of network layers
-        layer_width: Width of each MLP layer
-        out_dim: Output layer dimension. Uses layer_width if None.
-        activation: intermediate layer activation function.
-        out_activation: output activation function.
+        position_encoding: An encoding for the XYZ of distortion
+        temporal_encoding: An encoding for the time of distortion
+        mlp_num_layers: Number of layers in distortion MLP
+        mlp_layer_width: Size of hidden layer for the MLP
+        skip_connections: Number of layers for skip connections in the MLP
     """
 
     def __init__(
         self,
-        in_dim: int,
-        num_layers: int,
-        layer_width: int,
-        out_dim: Optional[int] = None,
-        skip_connections: Optional[Tuple[int]] = None,
-        activation: Optional[nn.Module] = nn.ReLU(),
-        out_activation: Optional[nn.Module] = None,
+        position_encoding: Encoding = NeRFEncoding(
+            in_dim=3, num_frequencies=10, min_freq_exp=0.0, max_freq_exp=8.0, include_input=True
+        ),
+        temporal_encoding: Encoding = NeRFEncoding(
+            in_dim=1, num_frequencies=10, min_freq_exp=0.0, max_freq_exp=8.0, include_input=True
+        ),
+        mlp_num_layers: int = 4,
+        mlp_layer_width: int = 256,
+        skip_connections: Tuple[int] = (4,),
     ) -> None:
         super().__init__()
-        self.in_dim = in_dim
-        assert self.in_dim > 0
-        self.out_dim = out_dim if out_dim is not None else layer_width
-        self.num_layers = num_layers
-        self.layer_width = layer_width
-        self.skip_connections = skip_connections
-        self._skip_connections: Set[int] = set(skip_connections) if skip_connections else set()
-        self.activation = activation
-        self.out_activation = out_activation
-        self.net = None
-        self.build_nn_modules()
-
-    def build_nn_modules(self) -> None:
-        """Initialize multi-layer perceptron."""
-        layers = []
-        if self.num_layers == 1:
-            layers.append(nn.Linear(self.in_dim, self.out_dim))
-        else:
-            for i in range(self.num_layers - 1):
-                if i == 0:
-                    assert i not in self._skip_connections, "Skip connection at layer 0 doesn't make sense."
-                    layers.append(nn.Linear(self.in_dim, self.layer_width))
-                elif i in self._skip_connections:
-                    layers.append(nn.Linear(self.layer_width + self.in_dim, self.layer_width))
-                else:
-                    layers.append(nn.Linear(self.layer_width, self.layer_width))
-            layers.append(nn.Linear(self.layer_width, self.out_dim))
-        self.layers = nn.ModuleList(layers)
-
-    def forward(self, in_tensor: Float[Tensor, "*bs in_dim"]) -> Float[Tensor, "*bs out_dim"]:
-        """Process input with a multilayer perceptron.
-
-        Args:
-            in_tensor: Network input
-
-        Returns:
-            MLP network output
-        """
-        x = in_tensor
-        for i, layer in enumerate(self.layers):
-            # as checked in `build_nn_modules`, 0 should not be in `_skip_connections`
-            if i in self._skip_connections:
-                x = torch.cat([in_tensor, x], -1)
-            x = layer(x)
-            if self.activation is not None and i < len(self.layers) - 1:
-                x = self.activation(x)
-        if self.out_activation is not None:
-            x = self.out_activation(x)
-        return x
+        self.position_encoding = position_encoding
+        self.temporal_encoding = temporal_encoding
+        self.mlp_deform = MLP(
+            in_dim=self.position_encoding.get_out_dim() + self.temporal_encoding.get_out_dim(),
+            out_dim=3,
+            num_layers=mlp_num_layers,
+            layer_width=mlp_layer_width,
+            skip_connections=skip_connections,
+        )
+
+    def forward(self, positions: Float[Tensor, "*bs 3"], times: Float[Tensor, "*bs 1"]) -> Float[Tensor, "*bs 3"]:
+        p = self.position_encoding(positions)
+        t = self.temporal_encoding(times)
+        return self.mlp_deform(torch.cat([p, t], dim=-1))
```

### Comparing `nerfstudio-0.3.1/nerfstudio/field_components/spatial_distortions.py` & `nerfstudio-0.3.2/nerfstudio/field_components/spatial_distortions.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/field_components/temporal_grid.py` & `nerfstudio-0.3.2/nerfstudio/fields/sdf_field.py`

 * *Files 27% similar despite different names*

```diff
@@ -8,356 +8,457 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Implements the temporal grid used by NeRFPlayer (https://arxiv.org/abs/2210.15947).
-A time conditioned sliding window is applied on the feature channels, so
-that the feature vectors become time-aware.
-(A large) Part of the code are adapted from (@ashawkey) https://github.com/ashawkey/torch-ngp/
 """
-from typing import Optional
+Field for SDF based model, rather then estimating density to generate a surface,
+a signed distance function (SDF) for surface representation is used to help with extracting high fidelity surfaces
+"""
+
+from dataclasses import dataclass, field
+from typing import Dict, Literal, Optional, Type
 
 import numpy as np
 import torch
-from jaxtyping import Float, Int
+import torch.nn.functional as F
+from jaxtyping import Float
 from torch import Tensor, nn
-from torch.autograd import Function
-from torch.cuda.amp import custom_bwd, custom_fwd
+from torch.nn.parameter import Parameter
 
-import nerfstudio.field_components.cuda as _C
+from nerfstudio.cameras.rays import RaySamples
+from nerfstudio.field_components.embedding import Embedding
+from nerfstudio.field_components.encodings import NeRFEncoding
+from nerfstudio.field_components.field_heads import FieldHeadNames
+from nerfstudio.field_components.spatial_distortions import SpatialDistortion
+from nerfstudio.fields.base_field import Field, FieldConfig
+
+try:
+    import tinycudann as tcnn
+except ModuleNotFoundError:
+    # tinycudann module doesn't exist
+    pass
 
 
-class TemporalGridEncodeFunc(Function):
-    """Class for autograd in pytorch."""
+class LearnedVariance(nn.Module):
+    """Variance network in NeuS
 
-    @staticmethod
-    @custom_fwd
-    def forward(
-        ctx,
-        inputs: Float[Tensor, "bs input_dim"],
-        temporal_row_index: Float[Tensor, "bs temporal_index_dim"],
-        embeddings: Float[Tensor, "table_size embed_dim"],
-        offsets: Int[Tensor, "num_levels_plus_1"],
-        per_level_scale: float,
-        base_resolution: int,
-        calc_grad_inputs: bool = False,
-        gridtype: int = 0,
-        align_corners: bool = False,
-    ) -> Float[Tensor, "bs output_dim"]:
-        """Call forward and interpolate the feature from embeddings
+    Args:
+        init_val: initial value in NeuS variance network
+    """
 
-        Args:
-            inputs: the input coords
-            temporal_row_index: the input index of channels for doing the interpolation
-            embeddings: the saved (hashing) table for the feature grid (of the full sequence)
-            offsets: offsets for each level in the multilevel table, used for locating in cuda kernels
-            per_level_scale: scale parameter for the table; same as InstantNGP
-            base_resolution: base resolution for the table; same as InstantNGP
-            calc_grad_inputs: bool indicator for calculating gradients on the inputs
-            gridtype: 0 == hash, 1 == tiled; tiled is a baseline in InstantNGP (not random collision)
-            align_corners: same as other interpolation operators
-        """
+    variance: Tensor
 
-        inputs = inputs.contiguous()
-        temporal_row_index = temporal_row_index.contiguous()
+    def __init__(self, init_val):
+        super().__init__()
+        self.register_parameter("variance", nn.Parameter(init_val * torch.ones(1), requires_grad=True))
 
-        B, D = inputs.shape  # batch size, coord dim
-        L = offsets.shape[0] - 1  # level
-        grid_channel = embeddings.shape[1]  # embedding dim for each level
-        C = temporal_row_index.shape[1] // 4  # output embedding dim for each level
-        S = np.log2(per_level_scale)  # resolution multiplier at each level, apply log2 for later CUDA exp2f
-        H = base_resolution  # base resolution
-
-        # torch.half used by torch-ngp, but we disable it
-        # (could be of negative impact on the performance? not sure, but feel free to inform me and help improve it!)
-        # # manually handle autocast (only use half precision embeddings, inputs must be float for enough precision)
-        # # if C % 2 != 0, force float, since half for atomicAdd is very slow.
-        # if torch.is_autocast_enabled() and C % 2 == 0:
-        #     embeddings = embeddings.to(torch.half)
+    def forward(self, x: Float[Tensor, "1"]) -> Float[Tensor, "1"]:
+        """Returns current variance value"""
+        return torch.ones([len(x), 1], device=x.device) * torch.exp(self.variance * 10.0)
+
+    def get_variance(self) -> Float[Tensor, "1"]:
+        """return current variance value"""
+        return torch.exp(self.variance * 10.0).clip(1e-6, 1e6)
+
+
+@dataclass
+class SDFFieldConfig(FieldConfig):
+    """SDF Field Config"""
+
+    _target: Type = field(default_factory=lambda: SDFField)
+    num_layers: int = 8
+    """Number of layers for geometric network"""
+    hidden_dim: int = 256
+    """Number of hidden dimension of geometric network"""
+    geo_feat_dim: int = 256
+    """Dimension of geometric feature"""
+    num_layers_color: int = 4
+    """Number of layers for color network"""
+    hidden_dim_color: int = 256
+    """Number of hidden dimension of color network"""
+    appearance_embedding_dim: int = 32
+    """Dimension of appearance embedding"""
+    use_appearance_embedding: bool = False
+    """Whether to use appearance embedding"""
+    bias: float = 0.8
+    """Sphere size of geometric initialization"""
+    geometric_init: bool = True
+    """Whether to use geometric initialization"""
+    inside_outside: bool = True
+    """Whether to revert signed distance value, set to True for indoor scene"""
+    weight_norm: bool = True
+    """Whether to use weight norm for linear layer"""
+    use_grid_feature: bool = False
+    """Whether to use multi-resolution feature grids"""
+    divide_factor: float = 2.0
+    """Normalization factor for multi-resolution grids"""
+    beta_init: float = 0.1
+    """Init learnable beta value for transformation of sdf to density"""
+    encoding_type: Literal["hash", "periodic", "tensorf_vm"] = "hash"
+    num_levels = 16
+    """Number of encoding levels"""
+    max_res = 2048
+    """Maximum resolution of the encoding"""
+    base_res = 16
+    """Base resolution of the encoding"""
+    log2_hashmap_size = 19
+    """Size of the hash map"""
+    features_per_level = 2
+    """Number of features per encoding level"""
+    use_hash = True
+    """Whether to use hash encoding"""
+    smoothstep = True
+    """Whether to use the smoothstep function"""
 
-        # L first, optimize cache for cuda kernel, but needs an extra permute later
-        outputs = torch.empty(L, B, C, device=inputs.device, dtype=embeddings.dtype)
 
-        if calc_grad_inputs:
-            dy_dx = torch.empty(B, L * D * C, device=inputs.device, dtype=embeddings.dtype)
-        else:
-            dy_dx = None
+class SDFField(Field):
+    """
+    A field for Signed Distance Functions (SDF).
+
+    Args:
+        config: The configuration for the SDF field.
+        aabb: An axis-aligned bounding box for the SDF field.
+        num_images: The number of images for embedding appearance.
+        use_average_appearance_embedding: Whether to use average appearance embedding. Defaults to False.
+        spatial_distortion: The spatial distortion. Defaults to None.
+    """
+
+    config: SDFFieldConfig
 
-        _C.temporal_grid_encode_forward(
-            inputs,
-            temporal_row_index,
-            embeddings,
-            offsets,
-            outputs,
-            B,
-            D,
-            grid_channel,
-            C,
-            L,
-            S,
-            H,
-            dy_dx,
-            gridtype,
-            align_corners,
+    def __init__(
+        self,
+        config: SDFFieldConfig,
+        aabb: Float[Tensor, "2 3"],
+        num_images: int,
+        use_average_appearance_embedding: bool = False,
+        spatial_distortion: Optional[SpatialDistortion] = None,
+    ) -> None:
+        super().__init__()
+        self.config = config
+
+        self.aabb = Parameter(aabb, requires_grad=False)
+
+        self.spatial_distortion = spatial_distortion
+        self.num_images = num_images
+
+        self.embedding_appearance = Embedding(self.num_images, self.config.appearance_embedding_dim)
+        self.use_average_appearance_embedding = use_average_appearance_embedding
+        self.use_grid_feature = self.config.use_grid_feature
+        self.divide_factor = self.config.divide_factor
+
+        growth_factor = np.exp((np.log(config.max_res) - np.log(config.base_res)) / (config.num_levels - 1))
+
+        if self.config.encoding_type == "hash":
+            # feature encoding
+            self.encoding = tcnn.Encoding(
+                n_input_dims=3,
+                encoding_config={
+                    "otype": "HashGrid" if config.use_hash else "DenseGrid",
+                    "n_levels": config.num_levels,
+                    "n_features_per_level": config.features_per_level,
+                    "log2_hashmap_size": config.log2_hashmap_size,
+                    "base_resolution": config.base_res,
+                    "per_level_scale": growth_factor,
+                    "interpolation": "Smoothstep" if config.smoothstep else "Linear",
+                },
+            )
+
+        # we concat inputs position ourselves
+        self.position_encoding = NeRFEncoding(
+            in_dim=3, num_frequencies=6, min_freq_exp=0.0, max_freq_exp=5.0, include_input=False
         )
 
-        # permute back to [B, L * C]
-        outputs = outputs.permute(1, 0, 2).reshape(B, L * C)
+        self.direction_encoding = NeRFEncoding(
+            in_dim=3, num_frequencies=4, min_freq_exp=0.0, max_freq_exp=3.0, include_input=True
+        )
 
-        ctx.save_for_backward(inputs, temporal_row_index, embeddings, offsets, dy_dx)
-        ctx.dims = [B, D, grid_channel, C, L, S, H, gridtype]
-        ctx.align_corners = align_corners
+        # initialize geometric network
+        self.initialize_geo_layers()
 
-        return outputs
+        # deviation_network to compute alpha from sdf from NeuS
+        self.deviation_network = LearnedVariance(init_val=self.config.beta_init)
+
+        # color network
+        dims = [self.config.hidden_dim_color for _ in range(self.config.num_layers_color)]
+        # point, view_direction, normal, feature, embedding
+        in_dim = (
+            3
+            + self.direction_encoding.get_out_dim()
+            + 3
+            + self.config.geo_feat_dim
+            + self.embedding_appearance.get_out_dim()
+        )
+        dims = [in_dim] + dims + [3]
+        self.num_layers_color = len(dims)
 
-    @staticmethod
-    @custom_bwd
-    def backward(ctx, grad):
-        inputs, temporal_row_index, embeddings, offsets, dy_dx = ctx.saved_tensors
-        B, D, grid_channel, C, L, S, H, gridtype = ctx.dims
-        align_corners = ctx.align_corners
+        for layer in range(0, self.num_layers_color - 1):
+            out_dim = dims[layer + 1]
+            lin = nn.Linear(dims[layer], out_dim)
 
-        # grad: [B, L * C] --> [L, B, C]
-        grad = grad.view(B, L, C).permute(1, 0, 2).contiguous()
+            if self.config.weight_norm:
+                lin = nn.utils.weight_norm(lin)
+            setattr(self, "clin" + str(layer), lin)
 
-        grad_embeddings = torch.zeros_like(embeddings).contiguous()
+        self.softplus = nn.Softplus(beta=100)
+        self.relu = nn.ReLU()
+        self.sigmoid = torch.nn.Sigmoid()
 
-        if dy_dx is not None:
-            grad_inputs = torch.zeros_like(inputs, dtype=embeddings.dtype)
+        self._cos_anneal_ratio = 1.0
+
+        if self.use_grid_feature:
+            assert self.spatial_distortion is not None, "spatial distortion must be provided when using grid feature"
+
+    def initialize_geo_layers(self) -> None:
+        """
+        Initialize layers for geometric network (sdf)
+        """
+        # MLP with geometric initialization
+        dims = [self.config.hidden_dim for _ in range(self.config.num_layers)]
+        in_dim = 3 + self.position_encoding.get_out_dim() + self.encoding.n_output_dims
+        dims = [in_dim] + dims + [1 + self.config.geo_feat_dim]
+        self.num_layers = len(dims)
+        self.skip_in = [4]
+
+        for layer in range(0, self.num_layers - 1):
+            if layer + 1 in self.skip_in:
+                out_dim = dims[layer + 1] - dims[0]
+            else:
+                out_dim = dims[layer + 1]
+
+            lin = nn.Linear(dims[layer], out_dim)
+
+            if self.config.geometric_init:
+                if layer == self.num_layers - 2:
+                    if not self.config.inside_outside:
+                        torch.nn.init.normal_(lin.weight, mean=np.sqrt(np.pi) / np.sqrt(dims[layer]), std=0.0001)
+                        torch.nn.init.constant_(lin.bias, -self.config.bias)
+                    else:
+                        torch.nn.init.normal_(lin.weight, mean=-np.sqrt(np.pi) / np.sqrt(dims[layer]), std=0.0001)
+                        torch.nn.init.constant_(lin.bias, self.config.bias)
+                elif layer == 0:
+                    torch.nn.init.constant_(lin.bias, 0.0)
+                    torch.nn.init.constant_(lin.weight[:, 3:], 0.0)
+                    torch.nn.init.normal_(lin.weight[:, :3], 0.0, np.sqrt(2) / np.sqrt(out_dim))
+                elif layer in self.skip_in:
+                    torch.nn.init.constant_(lin.bias, 0.0)
+                    torch.nn.init.normal_(lin.weight, 0.0, np.sqrt(2) / np.sqrt(out_dim))
+                    torch.nn.init.constant_(lin.weight[:, -(dims[0] - 3) :], 0.0)
+                else:
+                    torch.nn.init.constant_(lin.bias, 0.0)
+                    torch.nn.init.normal_(lin.weight, 0.0, np.sqrt(2) / np.sqrt(out_dim))
+
+            if self.config.weight_norm:
+                lin = nn.utils.weight_norm(lin)
+            setattr(self, "glin" + str(layer), lin)
+
+    def set_cos_anneal_ratio(self, anneal: float) -> None:
+        """Set the anneal value for the proposal network."""
+        self._cos_anneal_ratio = anneal
+
+    def forward_geonetwork(self, inputs: Float[Tensor, "*batch 3"]) -> Float[Tensor, "*batch geo_features+1"]:
+        """forward the geonetwork"""
+        if self.use_grid_feature:
+            assert self.spatial_distortion is not None, "spatial distortion must be provided when using grid feature"
+            positions = self.spatial_distortion(inputs)
+            # map range [-2, 2] to [0, 1]
+            positions = (positions + 2.0) / 4.0
+            feature = self.encoding(positions)
         else:
-            grad_inputs = None
+            feature = torch.zeros_like(inputs[:, :1].repeat(1, self.encoding.n_output_dims))
 
-        _C.temporal_grid_encode_backward(
-            grad,
-            inputs,
-            temporal_row_index,
-            embeddings,
-            offsets,
-            grad_embeddings,
-            B,
-            D,
-            grid_channel,
-            C,
-            L,
-            S,
-            H,
-            dy_dx,
-            grad_inputs,
-            gridtype,
-            align_corners,
-        )
+        pe = self.position_encoding(inputs)
 
-        if grad_inputs is not None:
-            grad_inputs = grad_inputs.to(inputs.dtype)
+        inputs = torch.cat((inputs, pe, feature), dim=-1)
 
-        return grad_inputs, None, grad_embeddings, None, None, None, None, None, None
+        # Pass through layers
+        outputs = inputs
 
+        for layer in range(0, self.num_layers - 1):
+            lin = getattr(self, "glin" + str(layer))
 
-class TemporalGridEncoder(nn.Module):
-    """Class for temporal grid encoding.
-    This class extends the grid encoding (from InstantNGP) by allowing the output time-dependent feature channels.
-    For example, for time 0 the interpolation uses channels [0,1], then for time 1 channels [2,1] are used.
-    This operation can be viewed as applying a time-dependent sliding window on the feature channels.
+            if layer in self.skip_in:
+                outputs = torch.cat([outputs, inputs], 1) / np.sqrt(2)
 
-    Args:
-        temporal_dim: the dimension of temporal modeling; a higher dim indicates a higher freq on the time axis
-        input_dim: the dimension of input coords
-        num_levels: number of levels for multi-scale hashing; same as InstantNGP
-        level_dim: the dim of output feature vector for each level; same as InstantNGP
-        per_level_scale: scale factor; same as InstantNGP
-        base_resolution: base resolution for the table; same as InstantNGP
-        log2_hashmap_size: the size of the table; same as InstantNGP
-        desired_resolution: desired resolution at the last level; same as InstantNGP
-        gridtype: "tiled" or "hash"
-        align_corners: same as other interpolation operators
-    """
+            outputs = lin(outputs)
 
-    sampling_index: Tensor
-    index_a_mask: Tensor
-    index_b_mask: Tensor
-    index_list: Tensor
+            if layer < self.num_layers - 2:
+                outputs = self.softplus(outputs)
+        return outputs
 
-    def __init__(
+    # TODO: fix ... in shape annotations.
+    def get_sdf(self, ray_samples: RaySamples) -> Float[Tensor, "num_samples ... 1"]:
+        """predict the sdf value for ray samples"""
+        positions = ray_samples.frustums.get_start_positions()
+        positions_flat = positions.view(-1, 3)
+        hidden_output = self.forward_geonetwork(positions_flat).view(*ray_samples.frustums.shape, -1)
+        sdf, _ = torch.split(hidden_output, [1, self.config.geo_feat_dim], dim=-1)
+        return sdf
+
+    def get_alpha(
         self,
-        temporal_dim: int = 64,
-        input_dim: int = 3,
-        num_levels: int = 16,
-        level_dim: int = 2,
-        per_level_scale: float = 2.0,
-        base_resolution: int = 16,
-        log2_hashmap_size: int = 19,
-        desired_resolution: Optional[int] = None,
-        gridtype: str = "hash",
-        align_corners: bool = False,
-    ) -> None:
-        super().__init__()
+        ray_samples: RaySamples,
+        sdf: Optional[Float[Tensor, "num_samples ... 1"]] = None,
+        gradients: Optional[Float[Tensor, "num_samples ... 1"]] = None,
+    ) -> Float[Tensor, "num_samples ... 1"]:
+        """compute alpha from sdf as in NeuS"""
+        if sdf is None or gradients is None:
+            inputs = ray_samples.frustums.get_start_positions()
+            inputs.requires_grad_(True)
+            with torch.enable_grad():
+                hidden_output = self.forward_geonetwork(inputs)
+                sdf, _ = torch.split(hidden_output, [1, self.config.geo_feat_dim], dim=-1)
+            d_output = torch.ones_like(sdf, requires_grad=False, device=sdf.device)
+            gradients = torch.autograd.grad(
+                outputs=sdf,
+                inputs=inputs,
+                grad_outputs=d_output,
+                create_graph=True,
+                retain_graph=True,
+                only_inputs=True,
+            )[0]
+
+        inv_s = self.deviation_network.get_variance()  # Single parameter
+
+        true_cos = (ray_samples.frustums.directions * gradients).sum(-1, keepdim=True)
+
+        # anneal as NeuS
+        cos_anneal_ratio = self._cos_anneal_ratio
+
+        # "cos_anneal_ratio" grows from 0 to 1 in the beginning training iterations. The anneal strategy below makes
+        # the cos value "not dead" at the beginning training iterations, for better convergence.
+        iter_cos = -(
+            F.relu(-true_cos * 0.5 + 0.5) * (1.0 - cos_anneal_ratio) + F.relu(-true_cos) * cos_anneal_ratio
+        )  # always non-positive
+
+        # Estimate signed distances at section points
+        estimated_next_sdf = sdf + iter_cos * ray_samples.deltas * 0.5
+        estimated_prev_sdf = sdf - iter_cos * ray_samples.deltas * 0.5
+
+        prev_cdf = torch.sigmoid(estimated_prev_sdf * inv_s)
+        next_cdf = torch.sigmoid(estimated_next_sdf * inv_s)
+
+        p = prev_cdf - next_cdf
+        c = prev_cdf
 
-        # the finest resolution desired at the last level, if provided, overridee per_level_scale
-        if desired_resolution is not None:
-            per_level_scale = np.exp2(np.log2(desired_resolution / base_resolution) / (num_levels - 1))
-
-        self.temporal_dim = temporal_dim
-        self.input_dim = input_dim  # coord dims, 2 or 3
-        self.num_levels = num_levels  # num levels, each level multiply resolution by 2
-        self.level_dim = level_dim  # encode channels per level
-        self.per_level_scale = per_level_scale  # multiply resolution by this scale at each level.
-        self.log2_hashmap_size = log2_hashmap_size
-        self.base_resolution = base_resolution
-        self.output_dim = num_levels * level_dim
-        self.gridtype = gridtype
-        _gridtype_to_id = {"hash": 0, "tiled": 1}
-        self.gridtype_id = _gridtype_to_id[gridtype]  # "tiled" or "hash"
-        self.align_corners = align_corners
-
-        # allocate parameters
-        offsets = []
-        offset = 0
-        self.max_params = 2**log2_hashmap_size
-        for i in range(num_levels):
-            resolution = int(np.ceil(base_resolution * per_level_scale**i))
-            params_in_level = min(
-                self.max_params, (resolution if align_corners else resolution + 1) ** input_dim
-            )  # limit max number
-            params_in_level = int(np.ceil(params_in_level / 8) * 8)  # make divisible
-            offsets.append(offset)
-            offset += params_in_level
-        offsets.append(offset)
-        offsets = torch.from_numpy(np.array(offsets, dtype=np.int32))
-        self.register_buffer("offsets", offsets)
-        self.n_params = offsets[-1] * level_dim
-        self.embeddings = nn.Parameter(torch.empty(offset, level_dim + temporal_dim))
-        self.init_parameters()
-
-    def init_parameters(self) -> None:
-        """Initialize the parameters:
-        1. Uniform initialization of the embeddings
-        2. Temporal interpolation index initialization:
-            For each temporal dim, we initialize a interpolation candidate.
-            For example, if temporal dim 0, we use channels [0,1,2,3], then for temporal dim 1,
-            we use channels [4,1,2,3]. After that, temporal dim 2, we use channels [4,5,2,3].
-            This is for the alignment of the channels. I.e., each temporal dim should differ
-            on only one channel, otherwise moving from one temporal dim to the next one is not
-            that consistent.
-            To associate time w.r.t. temporal dim, we evenly distribute time into the temporal dims.
-            That is, if we have 16 temporal dims, then the 16th channel combinations is the time 1.
-            (Time should be within 0 and 1.) Given a time, we first look up which temporal dim should
-            be used. And then compute the linear combination weights.
-            For implementing it, a table for all possible channel combination are used. Each row in
-            the table is the candidate feature channels, and means we move from one temporal dim to
-            the next one. For example, the first row will use feature channels [0,1,2,3,4]. Each row
-            is of length `num_of_output_channel*4`. The expanding param 4 is for saving the combination
-            weights and channels. The first row will be [?,0,?,1, 1,2,0,0, 1,3,0,0, 1,4,0,0]. Each
-            4 tuple means
-                `[weight_for_channel_A, index_for_channel_A, weight_for_channel_B, index_for_channel_B]`
-            If `weight_for_channel_A` is 1, then there is no interpolation on this channel.
-        """
-        std = 1e-4
-        self.embeddings.data.uniform_(-std, std)
-        # generate sampling index
-        temporal_grid_rows = self.temporal_dim
-        index_init = [0, self.level_dim] + list(range(1, self.level_dim))
-        permute_base = list(range(2, self.level_dim + 1))
-        last_entry = 0  # insert into ith place
-        permute_init = permute_base[:last_entry] + [0] + permute_base[last_entry:]
-        index_list = [torch.as_tensor(index_init, dtype=torch.long)]
-        permute_list = [torch.as_tensor(permute_init, dtype=torch.long)]
-
-        # converts a list of channel candidates into sampling row
-        def to_sampling_index(index, permute, last_entry):
-            row = index[permute]
-            row = torch.stack([torch.ones_like(row), row, torch.zeros_like(row), torch.zeros_like(row)], 1)
-            row = row.reshape([-1])
-            mask_a = torch.zeros_like(row).bool()
-            mask_b = torch.zeros_like(row).bool()
-            row[last_entry * 4 + 3] = index[1]
-            mask_a[last_entry * 4] = 1
-            mask_b[last_entry * 4 + 2] = 1
-            return row, mask_a, mask_b
-
-        row, mask_a, mask_b = to_sampling_index(index_list[0], permute_list[0], last_entry)
-        sampling_index = [row]
-        index_a_mask, index_b_mask = [mask_a], [mask_b]
-        # iterate on all temporal grid to get all rows
-        for _ in range(1, temporal_grid_rows - 1):
-            # the following lines are a little confusing...
-            # the basic idea is to keep a buffer and then move to the next channel
-            last_entry += 1
-            if last_entry >= self.level_dim:
-                last_entry = 0
-            last_index_max = index_list[-1].max().item()
-            last_index_min = index_list[-1].min().item()
-            tem_permute_list = permute_list[-1].clone()  # for rearrange
-            tem_permute_list[tem_permute_list == 0] += 1
-            prev = index_list[-1][1:][tem_permute_list - 1].tolist()
-            prev.pop(last_entry)
-            new_index = [last_index_min + 1, last_index_max + 1] + prev
-            new_index = torch.as_tensor(new_index, dtype=torch.long)
-            new_permute = permute_base[:last_entry] + [0] + permute_base[last_entry:]
-            new_permute = torch.as_tensor(new_permute, dtype=torch.long)
-            index_list.append(torch.as_tensor(new_index, dtype=torch.long))
-            permute_list.append(torch.as_tensor(new_permute, dtype=torch.long))
-            row, mask_a, mask_b = to_sampling_index(index_list[-1], permute_list[-1], last_entry)
-            sampling_index.append(row)
-            index_a_mask.append(mask_a)
-            index_b_mask.append(mask_b)
-        self.register_buffer("index_list", torch.stack(index_list))
-        self.register_buffer("sampling_index", torch.stack(sampling_index))
-        # index_a_mask and index_b_mask are for inserting the combination weights
-        self.register_buffer("index_a_mask", torch.stack(index_a_mask))
-        self.register_buffer("index_b_mask", torch.stack(index_b_mask))
-
-    def __repr__(self) -> str:
-        """For debug and logging purpose."""
-        return (
-            f"GridEncoder: input_dim={self.input_dim} num_levels={self.num_levels} "
-            f"level_dim={self.level_dim} resolution={self.base_resolution} -> "
-            f"{int(round(self.base_resolution * self.per_level_scale ** (self.num_levels - 1)))} "
-            f"per_level_scale={self.per_level_scale:.4f} params={tuple(self.embeddings.shape)} "
-            f"gridtype={self.gridtype} align_corners={self.align_corners}"
+        alpha = ((p + 1e-5) / (c + 1e-5)).clip(0.0, 1.0)
+
+        return alpha
+
+    def get_density(self, ray_samples: RaySamples):
+        raise NotImplementedError
+
+    def get_colors(
+        self,
+        points: Float[Tensor, "*batch 3"],
+        directions: Float[Tensor, "*batch 3"],
+        normals: Float[Tensor, "*batch 3"],
+        geo_features: Float[Tensor, "*batch geo_feat_dim"],
+        camera_indices: Tensor,
+    ) -> Float[Tensor, "*batch 3"]:
+        """compute colors"""
+        d = self.direction_encoding(directions)
+
+        # appearance
+        if self.training:
+            embedded_appearance = self.embedding_appearance(camera_indices)
+            # set it to zero if don't use it
+            if not self.config.use_appearance_embedding:
+                embedded_appearance = torch.zeros_like(embedded_appearance)
+        else:
+            if self.use_average_appearance_embedding:
+                embedded_appearance = torch.ones(
+                    (*directions.shape[:-1], self.config.appearance_embedding_dim), device=directions.device
+                ) * self.embedding_appearance.mean(dim=0)
+            else:
+                embedded_appearance = torch.zeros(
+                    (*directions.shape[:-1], self.config.appearance_embedding_dim), device=directions.device
+                )
+
+        hidden_input = torch.cat(
+            [
+                points,
+                d,
+                normals,
+                geo_features.view(-1, self.config.geo_feat_dim),
+                embedded_appearance.view(-1, self.config.appearance_embedding_dim),
+            ],
+            dim=-1,
         )
 
-    def get_temporal_index(self, time: Float[Tensor, "bs"]) -> Float[Tensor, "bs temporal_index_dim"]:
-        """Convert the time into sampling index lists."""
-        row_idx_value = time * (len(self.sampling_index) - 1)
-        row_idx = row_idx_value.long()
-        row_idx[time == 1] = len(self.sampling_index) - 1
-        temporal_row_index = self.sampling_index[row_idx].float()
-        mask_a = self.index_a_mask[row_idx]
-        mask_b = self.index_b_mask[row_idx]
-        temporal_row_index[mask_a] = row_idx + 1 - row_idx_value
-        temporal_row_index[mask_b] = row_idx_value - row_idx
-        return temporal_row_index
+        for layer in range(0, self.num_layers_color - 1):
+            lin = getattr(self, "clin" + str(layer))
 
-    def forward(
-        self, xyz: Float[Tensor, "bs input_dim"], time: Float[Tensor, "bs 1"]
-    ) -> Float[Tensor, "bs output_dim"]:
-        """Forward and sampling feature vectors from the embedding.
+            hidden_input = lin(hidden_input)
 
-        Args:
-            xyz: input coords, should be in [0,1]
-            time: input time, should be in [0,1] with shape [bs, 1]
-        """
-        outputs = TemporalGridEncodeFunc.apply(
-            xyz,
-            self.get_temporal_index(time[:, 0].float()),
-            self.embeddings,
-            self.offsets,
-            self.per_level_scale,
-            self.base_resolution,
-            xyz.requires_grad,
-            self.gridtype_id,
-            self.align_corners,
+            if layer < self.num_layers_color - 2:
+                hidden_input = self.relu(hidden_input)
+
+        rgb = self.sigmoid(hidden_input)
+
+        return rgb
+
+    def get_outputs(
+        self,
+        ray_samples: RaySamples,
+        density_embedding: Optional[Tensor] = None,
+        return_alphas: bool = False,
+    ) -> Dict[FieldHeadNames, Tensor]:
+        """compute output of ray samples"""
+        if ray_samples.camera_indices is None:
+            raise AttributeError("Camera indices are not provided.")
+
+        outputs = {}
+
+        camera_indices = ray_samples.camera_indices.squeeze()
+
+        inputs = ray_samples.frustums.get_start_positions()
+        inputs = inputs.view(-1, 3)
+
+        directions = ray_samples.frustums.directions
+        directions_flat = directions.reshape(-1, 3)
+
+        inputs.requires_grad_(True)
+        with torch.enable_grad():
+            hidden_output = self.forward_geonetwork(inputs)
+            sdf, geo_feature = torch.split(hidden_output, [1, self.config.geo_feat_dim], dim=-1)
+        d_output = torch.ones_like(sdf, requires_grad=False, device=sdf.device)
+        gradients = torch.autograd.grad(
+            outputs=sdf, inputs=inputs, grad_outputs=d_output, create_graph=True, retain_graph=True, only_inputs=True
+        )[0]
+
+        rgb = self.get_colors(inputs, directions_flat, gradients, geo_feature, camera_indices)
+
+        rgb = rgb.view(*ray_samples.frustums.directions.shape[:-1], -1)
+        sdf = sdf.view(*ray_samples.frustums.directions.shape[:-1], -1)
+        gradients = gradients.view(*ray_samples.frustums.directions.shape[:-1], -1)
+        normals = torch.nn.functional.normalize(gradients, p=2, dim=-1)
+
+        outputs.update(
+            {
+                FieldHeadNames.RGB: rgb,
+                FieldHeadNames.SDF: sdf,
+                FieldHeadNames.NORMALS: normals,
+                FieldHeadNames.GRADIENT: gradients,
+            }
         )
-        assert isinstance(outputs, Tensor)
+
+        if return_alphas:
+            alphas = self.get_alpha(ray_samples, sdf, gradients)
+            outputs.update({FieldHeadNames.ALPHA: alphas})
+
         return outputs
 
-    def get_temporal_tv_loss(self) -> Float[Tensor, ""]:
-        """Apply TV loss on the temporal channels.
-        Sample a random channel combination (i.e., row for the combination table),
-        and then compute loss on it.
+    def forward(
+        self, ray_samples: RaySamples, compute_normals: bool = False, return_alphas: bool = False
+    ) -> Dict[FieldHeadNames, Tensor]:
+        """Evaluates the field at points along the ray.
+
+        Args:
+            ray_samples: Samples to evaluate field on.
+            compute normals: not currently used in this implementation.
+            return_alphas: Whether to return alpha values
         """
-        row_idx = torch.randint(0, len(self.index_list), [1])
-        feat_idx = self.index_list[row_idx]
-        return (self.embeddings[:, feat_idx[0]] - self.embeddings[:, feat_idx[1]]).abs().mean()
+        field_outputs = self.get_outputs(ray_samples, return_alphas=return_alphas)
+        return field_outputs
```

### Comparing `nerfstudio-0.3.1/nerfstudio/fields/__init__.py` & `nerfstudio-0.3.2/nerfstudio/fields/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/fields/base_field.py` & `nerfstudio-0.3.2/nerfstudio/fields/base_field.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/fields/density_fields.py` & `nerfstudio-0.3.2/nerfstudio/fields/density_fields.py`

 * *Files 26% similar despite different names*

```diff
@@ -13,32 +13,27 @@
 # limitations under the License.
 
 """
 Proposal network field.
 """
 
 
-from typing import Optional, Tuple
+from typing import Literal, Optional, Tuple
 
-import numpy as np
 import torch
-from torch import Tensor
+from torch import Tensor, nn
 
 from nerfstudio.cameras.rays import RaySamples
 from nerfstudio.data.scene_box import SceneBox
 from nerfstudio.field_components.activations import trunc_exp
+from nerfstudio.field_components.encodings import HashEncoding
+from nerfstudio.field_components.mlp import MLP
 from nerfstudio.field_components.spatial_distortions import SpatialDistortion
 from nerfstudio.fields.base_field import Field
 
-try:
-    import tinycudann as tcnn
-except ImportError:
-    # tinycudann module doesn't exist
-    pass
-
 
 class HashMLPDensityField(Field):
     """A lightweight density field module.
 
     Args:
         aabb: parameters of scene aabb bounds
         num_layers: number of hidden layers
@@ -57,53 +52,47 @@
         spatial_distortion: Optional[SpatialDistortion] = None,
         use_linear: bool = False,
         num_levels: int = 8,
         max_res: int = 1024,
         base_res: int = 16,
         log2_hashmap_size: int = 18,
         features_per_level: int = 2,
+        implementation: Literal["tcnn", "torch"] = "torch",
     ) -> None:
         super().__init__()
         self.register_buffer("aabb", aabb)
         self.spatial_distortion = spatial_distortion
         self.use_linear = use_linear
-        growth_factor = np.exp((np.log(max_res) - np.log(base_res)) / (num_levels - 1))
 
         self.register_buffer("max_res", torch.tensor(max_res))
         self.register_buffer("num_levels", torch.tensor(num_levels))
         self.register_buffer("log2_hashmap_size", torch.tensor(log2_hashmap_size))
 
-        config = {
-            "encoding": {
-                "otype": "HashGrid",
-                "n_levels": num_levels,
-                "n_features_per_level": features_per_level,
-                "log2_hashmap_size": log2_hashmap_size,
-                "base_resolution": base_res,
-                "per_level_scale": growth_factor,
-            },
-            "network": {
-                "otype": "FullyFusedMLP",
-                "activation": "ReLU",
-                "output_activation": "None",
-                "n_neurons": hidden_dim,
-                "n_hidden_layers": num_layers - 1,
-            },
-        }
+        self.encoding = HashEncoding(
+            num_levels=num_levels,
+            min_res=base_res,
+            max_res=max_res,
+            log2_hashmap_size=log2_hashmap_size,
+            features_per_level=features_per_level,
+            implementation=implementation,
+        )
 
         if not self.use_linear:
-            self.mlp_base = tcnn.NetworkWithInputEncoding(
-                n_input_dims=3,
-                n_output_dims=1,
-                encoding_config=config["encoding"],
-                network_config=config["network"],
+            network = MLP(
+                in_dim=self.encoding.get_out_dim(),
+                num_layers=num_layers,
+                layer_width=hidden_dim,
+                out_dim=1,
+                activation=nn.ReLU(),
+                out_activation=None,
+                implementation=implementation,
             )
+            self.mlp_base = torch.nn.Sequential(self.encoding, network)
         else:
-            self.encoding = tcnn.Encoding(n_input_dims=3, encoding_config=config["encoding"])
-            self.linear = torch.nn.Linear(self.encoding.n_output_dims, 1)
+            self.linear = torch.nn.Linear(self.encoding.get_out_dim(), 1)
 
     def get_density(self, ray_samples: RaySamples) -> Tuple[Tensor, None]:
         if self.spatial_distortion is not None:
             positions = self.spatial_distortion(ray_samples.frustums.get_positions())
             positions = (positions + 2.0) / 4.0
         else:
             positions = SceneBox.get_normalized_positions(ray_samples.frustums.get_positions(), self.aabb)
```

### Comparing `nerfstudio-0.3.1/nerfstudio/fields/instant_ngp_field.py` & `nerfstudio-0.3.2/nerfstudio/fields/instant_ngp_field.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,14 +56,15 @@
         use_appearance_embedding: whether to use appearance embedding
         num_images: number of images, required if use_appearance_embedding is True
         appearance_embedding_dim: dimension of appearance embedding
         contraction_type: type of contraction
         num_levels: number of levels of the hashmap for the base mlp
         log2_hashmap_size: size of the hashmap for the base mlp
         max_res: maximum resolution of the hashmap for the base mlp
+        mode: which implementation to use for the field
     """
 
     def __init__(
         self,
         aabb: Tensor,
         num_layers: int = 2,
         hidden_dim: int = 64,
```

### Comparing `nerfstudio-0.3.1/nerfstudio/fields/nerfacto_field.py` & `nerfstudio-0.3.2/nerfstudio/fields/nerfacto_field.py`

 * *Files 25% similar despite different names*

```diff
@@ -13,52 +13,38 @@
 # limitations under the License.
 
 """
 Field for compound nerf model, adds scene contraction and image embeddings to instant ngp
 """
 
 
-from typing import Dict, Optional, Tuple, Type
+from typing import Dict, Literal, Optional, Tuple
 
-import numpy as np
 import torch
 from torch import Tensor, nn
-from torch.nn.parameter import Parameter
 
 from nerfstudio.cameras.rays import RaySamples
 from nerfstudio.data.scene_box import SceneBox
 from nerfstudio.field_components.activations import trunc_exp
 from nerfstudio.field_components.embedding import Embedding
-from nerfstudio.field_components.encodings import Encoding, HashEncoding, SHEncoding
+from nerfstudio.field_components.encodings import HashEncoding, NeRFEncoding, SHEncoding
 from nerfstudio.field_components.field_heads import (
-    DensityFieldHead,
-    FieldHead,
     FieldHeadNames,
     PredNormalsFieldHead,
-    RGBFieldHead,
     SemanticFieldHead,
     TransientDensityFieldHead,
     TransientRGBFieldHead,
     UncertaintyFieldHead,
 )
 from nerfstudio.field_components.mlp import MLP
-from nerfstudio.field_components.spatial_distortions import (
-    SceneContraction,
-    SpatialDistortion,
-)
+from nerfstudio.field_components.spatial_distortions import SpatialDistortion
 from nerfstudio.fields.base_field import Field, shift_directions_for_tcnn
 
-try:
-    import tinycudann as tcnn
-except ModuleNotFoundError:
-    # tinycudann module doesn't exist
-    pass
-
 
-class TCNNNerfactoField(Field):
+class NerfactoField(Field):
     """Compound Field that uses TCNN
 
     Args:
         aabb: parameters of scene aabb bounds
         num_images: number of images in the dataset
         num_layers: number of hidden layers
         hidden_dim: dimension of hidden layers
@@ -86,29 +72,32 @@
         self,
         aabb: Tensor,
         num_images: int,
         num_layers: int = 2,
         hidden_dim: int = 64,
         geo_feat_dim: int = 15,
         num_levels: int = 16,
+        base_res: int = 16,
         max_res: int = 2048,
         log2_hashmap_size: int = 19,
         num_layers_color: int = 3,
         num_layers_transient: int = 2,
+        features_per_level: int = 2,
         hidden_dim_color: int = 64,
         hidden_dim_transient: int = 64,
         appearance_embedding_dim: int = 32,
         transient_embedding_dim: int = 16,
         use_transient_embedding: bool = False,
         use_semantics: bool = False,
         num_semantic_classes: int = 100,
         pass_semantic_gradients: bool = False,
         use_pred_normals: bool = False,
         use_average_appearance_embedding: bool = False,
         spatial_distortion: Optional[SpatialDistortion] = None,
+        implementation: Literal["tcnn", "torch"] = "tcnn",
     ) -> None:
         super().__init__()
 
         self.register_buffer("aabb", aabb)
         self.geo_feat_dim = geo_feat_dim
 
         self.register_buffer("max_res", torch.tensor(max_res))
@@ -120,113 +109,97 @@
         self.appearance_embedding_dim = appearance_embedding_dim
         self.embedding_appearance = Embedding(self.num_images, self.appearance_embedding_dim)
         self.use_average_appearance_embedding = use_average_appearance_embedding
         self.use_transient_embedding = use_transient_embedding
         self.use_semantics = use_semantics
         self.use_pred_normals = use_pred_normals
         self.pass_semantic_gradients = pass_semantic_gradients
+        self.base_res = base_res
 
-        base_res: int = 16
-        features_per_level: int = 2
-        growth_factor = np.exp((np.log(max_res) - np.log(base_res)) / (num_levels - 1))
-
-        self.direction_encoding = tcnn.Encoding(
-            n_input_dims=3,
-            encoding_config={
-                "otype": "SphericalHarmonics",
-                "degree": 4,
-            },
+        self.direction_encoding = SHEncoding(
+            levels=4,
+            implementation=implementation,
         )
 
-        self.position_encoding = tcnn.Encoding(
-            n_input_dims=3,
-            encoding_config={"otype": "Frequency", "n_frequencies": 2},
+        self.position_encoding = NeRFEncoding(
+            in_dim=3, num_frequencies=2, min_freq_exp=0, max_freq_exp=2 - 1, implementation=implementation
         )
 
-        self.mlp_base = tcnn.NetworkWithInputEncoding(
-            n_input_dims=3,
-            n_output_dims=1 + self.geo_feat_dim,
-            encoding_config={
-                "otype": "HashGrid",
-                "n_levels": num_levels,
-                "n_features_per_level": features_per_level,
-                "log2_hashmap_size": log2_hashmap_size,
-                "base_resolution": base_res,
-                "per_level_scale": growth_factor,
-            },
-            network_config={
-                "otype": "FullyFusedMLP",
-                "activation": "ReLU",
-                "output_activation": "None",
-                "n_neurons": hidden_dim,
-                "n_hidden_layers": num_layers - 1,
-            },
+        self.mlp_base_grid = HashEncoding(
+            num_levels=num_levels,
+            min_res=base_res,
+            max_res=max_res,
+            log2_hashmap_size=log2_hashmap_size,
+            features_per_level=features_per_level,
+            implementation=implementation,
         )
+        self.mlp_base_mlp = MLP(
+            in_dim=self.mlp_base_grid.get_out_dim(),
+            num_layers=num_layers,
+            layer_width=hidden_dim,
+            out_dim=1 + self.geo_feat_dim,
+            activation=nn.ReLU(),
+            out_activation=None,
+            implementation=implementation,
+        )
+        self.mlp_base = torch.nn.Sequential(self.mlp_base_grid, self.mlp_base_mlp)
 
         # transients
         if self.use_transient_embedding:
             self.transient_embedding_dim = transient_embedding_dim
             self.embedding_transient = Embedding(self.num_images, self.transient_embedding_dim)
-            self.mlp_transient = tcnn.Network(
-                n_input_dims=self.geo_feat_dim + self.transient_embedding_dim,
-                n_output_dims=hidden_dim_transient,
-                network_config={
-                    "otype": "FullyFusedMLP",
-                    "activation": "ReLU",
-                    "output_activation": "None",
-                    "n_neurons": hidden_dim_transient,
-                    "n_hidden_layers": num_layers_transient - 1,
-                },
+            self.mlp_transient = MLP(
+                in_dim=self.geo_feat_dim + self.transient_embedding_dim,
+                num_layers=num_layers_transient,
+                layer_width=hidden_dim_transient,
+                out_dim=hidden_dim_transient,
+                activation=nn.ReLU(),
+                out_activation=None,
+                implementation=implementation,
             )
-            self.field_head_transient_uncertainty = UncertaintyFieldHead(in_dim=self.mlp_transient.n_output_dims)
-            self.field_head_transient_rgb = TransientRGBFieldHead(in_dim=self.mlp_transient.n_output_dims)
-            self.field_head_transient_density = TransientDensityFieldHead(in_dim=self.mlp_transient.n_output_dims)
+            self.field_head_transient_uncertainty = UncertaintyFieldHead(in_dim=self.mlp_transient.get_out_dim())
+            self.field_head_transient_rgb = TransientRGBFieldHead(in_dim=self.mlp_transient.get_out_dim())
+            self.field_head_transient_density = TransientDensityFieldHead(in_dim=self.mlp_transient.get_out_dim())
 
         # semantics
         if self.use_semantics:
-            self.mlp_semantics = tcnn.Network(
-                n_input_dims=self.geo_feat_dim,
-                n_output_dims=hidden_dim_transient,
-                network_config={
-                    "otype": "FullyFusedMLP",
-                    "activation": "ReLU",
-                    "output_activation": "None",
-                    "n_neurons": 64,
-                    "n_hidden_layers": 1,
-                },
+            self.mlp_semantics = MLP(
+                in_dim=self.geo_feat_dim,
+                num_layers=2,
+                layer_width=64,
+                out_dim=hidden_dim_transient,
+                activation=nn.ReLU(),
+                out_activation=None,
+                implementation=implementation,
             )
             self.field_head_semantics = SemanticFieldHead(
-                in_dim=self.mlp_semantics.n_output_dims, num_classes=num_semantic_classes
+                in_dim=self.mlp_semantics.get_out_dim(), num_classes=num_semantic_classes
             )
 
         # predicted normals
         if self.use_pred_normals:
-            self.mlp_pred_normals = tcnn.Network(
-                n_input_dims=self.geo_feat_dim + self.position_encoding.n_output_dims,
-                n_output_dims=hidden_dim_transient,
-                network_config={
-                    "otype": "FullyFusedMLP",
-                    "activation": "ReLU",
-                    "output_activation": "None",
-                    "n_neurons": 64,
-                    "n_hidden_layers": 2,
-                },
+            self.mlp_pred_normals = MLP(
+                in_dim=self.geo_feat_dim + self.position_encoding.get_out_dim(),
+                num_layers=3,
+                layer_width=64,
+                out_dim=hidden_dim_transient,
+                activation=nn.ReLU(),
+                out_activation=None,
+                implementation=implementation,
             )
-            self.field_head_pred_normals = PredNormalsFieldHead(in_dim=self.mlp_pred_normals.n_output_dims)
+            self.field_head_pred_normals = PredNormalsFieldHead(in_dim=self.mlp_pred_normals.get_out_dim())
 
-        self.mlp_head = tcnn.Network(
-            n_input_dims=self.direction_encoding.n_output_dims + self.geo_feat_dim + self.appearance_embedding_dim,
-            n_output_dims=3,
-            network_config={
-                "otype": "FullyFusedMLP",
-                "activation": "ReLU",
-                "output_activation": "Sigmoid",
-                "n_neurons": hidden_dim_color,
-                "n_hidden_layers": num_layers_color - 1,
-            },
+        self.mlp_head = MLP(
+            in_dim=self.direction_encoding.get_out_dim() + self.geo_feat_dim + self.appearance_embedding_dim,
+            num_layers=num_layers_color,
+            layer_width=hidden_dim_color,
+            out_dim=3,
+            activation=nn.ReLU(),
+            out_activation=nn.Sigmoid(),
+            implementation=implementation,
         )
 
     def get_density(self, ray_samples: RaySamples) -> Tuple[Tensor, Tensor]:
         """Computes and returns the densities."""
         if self.spatial_distortion is not None:
             positions = ray_samples.frustums.get_positions()
             positions = self.spatial_distortion(positions)
@@ -320,106 +293,7 @@
             ],
             dim=-1,
         )
         rgb = self.mlp_head(h).view(*outputs_shape, -1).to(directions)
         outputs.update({FieldHeadNames.RGB: rgb})
 
         return outputs
-
-
-class TorchNerfactoField(Field):
-    """
-    PyTorch implementation of the compound field.
-    """
-
-    def __init__(
-        self,
-        aabb: Tensor,
-        num_images: int,
-        position_encoding: Encoding = HashEncoding(),
-        direction_encoding: Encoding = SHEncoding(),
-        base_mlp_num_layers: int = 3,
-        base_mlp_layer_width: int = 64,
-        head_mlp_num_layers: int = 2,
-        head_mlp_layer_width: int = 32,
-        appearance_embedding_dim: int = 40,
-        skip_connections: Tuple = (4,),
-        field_heads: Tuple[FieldHead] = (RGBFieldHead(),),
-        spatial_distortion: SpatialDistortion = SceneContraction(),
-    ) -> None:
-        super().__init__()
-        self.aabb = Parameter(aabb, requires_grad=False)
-        self.spatial_distortion = spatial_distortion
-        self.num_images = num_images
-        self.appearance_embedding_dim = appearance_embedding_dim
-        self.embedding_appearance = Embedding(self.num_images, self.appearance_embedding_dim)
-
-        self.position_encoding = position_encoding
-        self.direction_encoding = direction_encoding
-
-        self.mlp_base = MLP(
-            in_dim=self.position_encoding.get_out_dim(),
-            num_layers=base_mlp_num_layers,
-            layer_width=base_mlp_layer_width,
-            skip_connections=skip_connections,
-            out_activation=nn.ReLU(),
-        )
-
-        self.mlp_head = MLP(
-            in_dim=self.mlp_base.get_out_dim() + self.direction_encoding.get_out_dim() + self.appearance_embedding_dim,
-            num_layers=head_mlp_num_layers,
-            layer_width=head_mlp_layer_width,
-            out_activation=nn.ReLU(),
-        )
-
-        self.field_output_density = DensityFieldHead(in_dim=self.mlp_base.get_out_dim())
-        self.field_heads = nn.ModuleList(field_heads)
-        for field_head in self.field_heads:
-            field_head.set_in_dim(self.mlp_head.get_out_dim())  # type: ignore
-
-    def get_density(self, ray_samples: RaySamples) -> Tuple[Tensor, Tensor]:
-        if self.spatial_distortion is not None:
-            positions = ray_samples.frustums.get_positions()
-            positions = self.spatial_distortion(positions)
-        else:
-            positions = ray_samples.frustums.get_positions()
-        encoded_xyz = self.position_encoding(positions.view(-1, 3)).to(torch.float32)
-        base_mlp_out = self.mlp_base(encoded_xyz).view(*ray_samples.frustums.shape, -1)
-        density = self.field_output_density(base_mlp_out)
-        return density, base_mlp_out
-
-    def get_outputs(
-        self, ray_samples: RaySamples, density_embedding: Optional[Tensor] = None
-    ) -> Dict[FieldHeadNames, Tensor]:
-        outputs_shape = ray_samples.frustums.directions.shape[:-1]
-
-        if ray_samples.camera_indices is None:
-            raise AttributeError("Camera indices are not provided.")
-        camera_indices = ray_samples.camera_indices.squeeze()
-        if self.training:
-            embedded_appearance = self.embedding_appearance(camera_indices)
-        else:
-            embedded_appearance = torch.zeros(
-                (*outputs_shape, self.appearance_embedding_dim),
-                device=ray_samples.frustums.directions.device,
-            )
-
-        outputs = {}
-        for field_head in self.field_heads:
-            directions = shift_directions_for_tcnn(ray_samples.frustums.directions)
-            directions_flat = directions.view(-1, 3)
-            encoded_dir = self.direction_encoding(directions_flat)
-            mlp_out = self.mlp_head(
-                torch.cat(
-                    [
-                        encoded_dir.view(-1, self.direction_encoding.get_out_dim()),
-                        density_embedding.view(-1, self.mlp_base.get_out_dim()),  # type:ignore
-                        embedded_appearance.view(-1, self.appearance_embedding_dim),
-                    ],
-                    dim=-1,  # type:ignore
-                )
-            )
-            outputs[field_head.field_head_name] = field_head(mlp_out).view(*outputs_shape, -1).to(directions)
-        return outputs
-
-
-field_implementation_to_class: Dict[str, Type[Field]] = {"tcnn": TCNNNerfactoField, "torch": TorchNerfactoField}
```

### Comparing `nerfstudio-0.3.1/nerfstudio/fields/nerfplayer_ngp_field.py` & `nerfstudio-0.3.2/nerfstudio/models/neus_facto.py`

 * *Files 27% similar despite different names*

```diff
@@ -9,235 +9,218 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
-NeRFPlayer (https://arxiv.org/abs/2210.15947) field implementations with InstantNGP backbone
+Implementation of NeuS similar to nerfacto where proposal sampler is used.
+Based on SDFStudio https://github.com/autonomousvision/sdfstudio/
 """
 
+from __future__ import annotations
 
-from typing import Dict, Optional, Tuple
+from dataclasses import dataclass, field
+from typing import Any, Dict, List, Optional, Tuple, Type
 
+import numpy as np
 import torch
-from jaxtyping import Float
-from torch import Tensor
-from torch.nn.parameter import Parameter
-
-from nerfstudio.cameras.rays import Frustums, RaySamples
-from nerfstudio.data.scene_box import SceneBox
-from nerfstudio.field_components.activations import trunc_exp
-from nerfstudio.field_components.embedding import Embedding
+from torch.nn import Parameter
+
+from nerfstudio.cameras.rays import RayBundle
+from nerfstudio.engine.callbacks import (
+    TrainingCallback,
+    TrainingCallbackAttributes,
+    TrainingCallbackLocation,
+)
 from nerfstudio.field_components.field_heads import FieldHeadNames
-from nerfstudio.field_components.spatial_distortions import (
-    SceneContraction,
-    SpatialDistortion,
+from nerfstudio.fields.density_fields import HashMLPDensityField
+from nerfstudio.model_components.losses import interlevel_loss
+from nerfstudio.model_components.ray_samplers import (
+    ProposalNetworkSampler,
+    UniformSampler,
 )
-from nerfstudio.field_components.temporal_grid import TemporalGridEncoder
-from nerfstudio.fields.base_field import Field, shift_directions_for_tcnn
+from nerfstudio.models.neus import NeuSModel, NeuSModelConfig
+from nerfstudio.utils import colormaps
+
+
+@dataclass
+class NeuSFactoModelConfig(NeuSModelConfig):
+    """NeusFacto Model Config"""
+
+    _target: Type = field(default_factory=lambda: NeuSFactoModel)
+    num_proposal_samples_per_ray: Tuple[int, ...] = (256, 96)
+    """Number of samples per ray for the proposal network."""
+    num_neus_samples_per_ray: int = 48
+    """Number of samples per ray for the nerf network."""
+    proposal_update_every: int = 5
+    """Sample every n steps after the warmup"""
+    proposal_warmup: int = 5000
+    """Scales n from 1 to proposal_update_every over this many steps"""
+    num_proposal_iterations: int = 2
+    """Number of proposal network iterations."""
+    use_same_proposal_network: bool = False
+    """Use the same proposal network. Otherwise use different ones."""
+    proposal_net_args_list: List[Dict] = field(
+        default_factory=lambda: [
+            {"hidden_dim": 16, "log2_hashmap_size": 17, "num_levels": 5, "max_res": 64},
+            {"hidden_dim": 16, "log2_hashmap_size": 17, "num_levels": 5, "max_res": 256},
+        ]
+    )
+    """Arguments for the proposal density fields."""
+    interlevel_loss_mult: float = 1.0
+    """Proposal loss multiplier."""
+    use_proposal_weight_anneal: bool = True
+    """Whether to use proposal weight annealing."""
+    proposal_weights_anneal_slope: float = 10.0
+    """Slope of the annealing function for the proposal weights."""
+    proposal_weights_anneal_max_num_iters: int = 1000
+    """Max num iterations for the annealing function."""
+    use_single_jitter: bool = True
+    """Whether use single jitter or not for the proposal networks."""
 
-try:
-    import tinycudann as tcnn
-except ModuleNotFoundError:
-    # tinycudann module doesn't exist
-    pass
 
+class NeuSFactoModel(NeuSModel):
+    """NeuSFactoModel extends NeuSModel for a more efficient sampling strategy.
 
-class NerfplayerNGPField(Field):
-    """NeRFPlayer (https://arxiv.org/abs/2210.15947) field with InstantNGP backbone.
+    The model improves the rendering speed and quality by incorporating a learning-based
+    proposal distribution to guide the sampling process.(similar to mipnerf-360)
 
     Args:
-        aabb: parameters of scene aabb bounds
-        temporal_dim: the dimension of temporal axis, a higher dimension indicates a higher temporal frequency
-            please refer to the implementation of TemporalGridEncoder for more details
-        num_levels: the number of multi-resolution levels; same as InstantNGP
-        features_per_level: the dim of output feature vector for each level; same as InstantNGP
-        log2_hashmap_size: the size of the table; same as InstantNGP
-        base_resolution: base resolution for the table; same as InstantNGP
-        num_layers: number of hidden layers (occupancy decoder network after sampling)
-        hidden_dim: dimension of hidden layers (occupancy decoder network after sampling)
-        geo_feat_dim: output geo feat dimensions
-        num_layers_color: number of hidden layers for color network
-        hidden_dim_color: dimension of hidden layers for color network
-        use_appearance_embedding: whether to use appearance embedding
-        disable_viewing_dependent: if true, disable the viewing dependent effect (no viewing direction as inputs)
-            Sometimes we need to disable viewing dependent effects in a dynamic scene, because there is
-            ambiguity between being dynamic and viewing dependent effects. For example, the shadow of the camera
-            should be a dynamic effect, but may be reconstructed as viewing dependent effects.
-        num_images: number of images, requried if use_appearance_embedding is True
-        appearance_embedding_dim: dimension of appearance embedding
-        contraction_type: type of contraction
+        config: NeuS configuration to instantiate model
     """
 
-    def __init__(
-        self,
-        aabb: Tensor,
-        temporal_dim: int = 16,
-        num_levels: int = 16,
-        features_per_level: int = 2,
-        log2_hashmap_size: int = 19,
-        base_resolution: int = 16,
-        num_layers: int = 2,
-        hidden_dim: int = 64,
-        geo_feat_dim: int = 15,
-        num_layers_color: int = 3,
-        hidden_dim_color: int = 64,
-        use_appearance_embedding: bool = False,
-        disable_viewing_dependent: bool = False,
-        num_images: Optional[int] = None,
-        appearance_embedding_dim: int = 32,
-        spatial_distortion: Optional[SpatialDistortion] = SceneContraction(),
-    ) -> None:
-        super().__init__()
-
-        self.aabb = Parameter(aabb, requires_grad=False)
-        self.geo_feat_dim = geo_feat_dim
-        self.spatial_distortion = spatial_distortion
-
-        self.use_appearance_embedding = use_appearance_embedding
-        if use_appearance_embedding:
-            assert num_images is not None
-            self.appearance_embedding_dim = appearance_embedding_dim
-            self.appearance_embedding = Embedding(num_images, appearance_embedding_dim)
-
-        self.direction_encoding = tcnn.Encoding(
-            n_input_dims=3,
-            encoding_config={
-                "otype": "SphericalHarmonics",
-                "degree": 4,
-            },
-        )
+    config: NeuSFactoModelConfig
 
-        self.mlp_base = TemporalGridEncoder(
-            input_dim=3,
-            temporal_dim=temporal_dim,
-            num_levels=num_levels,
-            level_dim=features_per_level,
-            base_resolution=base_resolution,
-            log2_hashmap_size=log2_hashmap_size,
-            desired_resolution=int(1024 * (self.aabb.max() - self.aabb.min())),
-        )
-        self.mlp_base_decode = tcnn.Network(
-            n_input_dims=num_levels * features_per_level,
-            n_output_dims=1 + self.geo_feat_dim,
-            network_config={
-                "otype": "FullyFusedMLP",
-                "activation": "ReLU",
-                "output_activation": "None",
-                "n_neurons": hidden_dim,
-                "n_hidden_layers": num_layers - 1,
-            },
-        )
+    def populate_modules(self):
+        """Instantiate modules and fields, including proposal networks."""
+        super().populate_modules()
+
+        self.density_fns = []
+        num_prop_nets = self.config.num_proposal_iterations
+        # Build the proposal network(s)
+        self.proposal_networks = torch.nn.ModuleList()
+        if self.config.use_same_proposal_network:
+            assert len(self.config.proposal_net_args_list) == 1, "Only one proposal network is allowed."
+            prop_net_args = self.config.proposal_net_args_list[0]
+            network = HashMLPDensityField(
+                self.scene_box.aabb, spatial_distortion=self.scene_contraction, **prop_net_args
+            )
+            self.proposal_networks.append(network)
+            self.density_fns.extend([network.density_fn for _ in range(num_prop_nets)])
+        else:
+            for i in range(num_prop_nets):
+                prop_net_args = self.config.proposal_net_args_list[min(i, len(self.config.proposal_net_args_list) - 1)]
+                network = HashMLPDensityField(
+                    self.scene_box.aabb,
+                    spatial_distortion=self.scene_contraction,
+                    **prop_net_args,
+                )
+                self.proposal_networks.append(network)
+            self.density_fns.extend([network.density_fn for network in self.proposal_networks])
 
-        in_dim = self.direction_encoding.n_output_dims + self.geo_feat_dim
-        if disable_viewing_dependent:
-            in_dim = self.geo_feat_dim
-            self.direction_encoding = None
-        if self.use_appearance_embedding:
-            in_dim += self.appearance_embedding_dim
-        self.mlp_head = tcnn.Network(
-            n_input_dims=in_dim,
-            n_output_dims=3,
-            network_config={
-                "otype": "FullyFusedMLP",
-                "activation": "ReLU",
-                "output_activation": "Sigmoid",
-                "n_neurons": hidden_dim_color,
-                "n_hidden_layers": num_layers_color - 1,
-            },
+        # update proposal network every iterations
+        def update_schedule(_):
+            return -1
+
+        initial_sampler = UniformSampler(single_jitter=self.config.use_single_jitter)
+        self.proposal_sampler = ProposalNetworkSampler(
+            num_nerf_samples_per_ray=self.config.num_neus_samples_per_ray,
+            num_proposal_samples_per_ray=self.config.num_proposal_samples_per_ray,
+            num_proposal_network_iterations=self.config.num_proposal_iterations,
+            single_jitter=self.config.use_single_jitter,
+            update_sched=update_schedule,
+            initial_sampler=initial_sampler,
         )
 
-    def get_density(self, ray_samples: RaySamples) -> Tuple[Tensor, Tensor]:
-        if self.spatial_distortion is not None:
-            positions = ray_samples.frustums.get_positions()
-            positions = self.spatial_distortion(positions)
-            positions = (positions + 2.0) / 4.0
-        else:
-            positions = SceneBox.get_normalized_positions(ray_samples.frustums.get_positions(), self.aabb)
-        # Make sure the tcnn gets inputs between 0 and 1.
-        selector = ((positions > 0.0) & (positions < 1.0)).all(dim=-1)
-        positions = positions * selector[..., None]
-        positions_flat = positions.view(-1, 3)
-        assert ray_samples.times is not None, "Time should be included in the input for NeRFPlayer"
-        times_flat = ray_samples.times.view(-1, 1)
-
-        h = self.mlp_base(positions_flat, times_flat)
-        h = self.mlp_base_decode(h).view(*ray_samples.frustums.shape, -1)
-        density_before_activation, base_mlp_out = torch.split(h, [1, self.geo_feat_dim], dim=-1)
-
-        # Rectifying the density with an exponential is much more stable than a ReLU or
-        # softplus, because it enables high post-activation (float32) density outputs
-        # from smaller internal (float16) parameters.
-        density = trunc_exp(density_before_activation.to(positions))
-        density = density * selector[..., None]
-        return density, base_mlp_out
-
-    def get_outputs(
-        self, ray_samples: RaySamples, density_embedding: Optional[Tensor] = None
-    ) -> Dict[FieldHeadNames, Tensor]:
-        assert density_embedding is not None
-        directions = shift_directions_for_tcnn(ray_samples.frustums.directions)
-        directions_flat = directions.view(-1, 3)
-
-        if self.direction_encoding is not None:
-            d = self.direction_encoding(directions_flat)
-            h = torch.cat([d, density_embedding.view(-1, self.geo_feat_dim)], dim=-1)
-        else:
-            # viewing direction is disabled
-            h = density_embedding.view(-1, self.geo_feat_dim)
-
-        if self.use_appearance_embedding:
-            if ray_samples.camera_indices is None:
-                raise AttributeError("Camera indices are not provided.")
-            camera_indices = ray_samples.camera_indices.squeeze()
-            if self.training:
-                embedded_appearance = self.appearance_embedding(camera_indices)
-            else:
-                embedded_appearance = torch.zeros(
-                    (*directions.shape[:-1], self.appearance_embedding_dim), device=directions.device
+    def get_param_groups(self) -> Dict[str, List[Parameter]]:
+        """Return a dictionary with the parameters of the proposal networks."""
+        param_groups = super().get_param_groups()
+        param_groups["proposal_networks"] = list(self.proposal_networks.parameters())
+        return param_groups
+
+    def get_training_callbacks(
+        self, training_callback_attributes: TrainingCallbackAttributes
+    ) -> List[TrainingCallback]:
+        callbacks = super().get_training_callbacks(training_callback_attributes)
+
+        if self.config.use_proposal_weight_anneal:
+            # anneal the weights of the proposal network before doing PDF sampling
+            N = self.config.proposal_weights_anneal_max_num_iters
+
+            def set_anneal(step: int):
+                # https://arxiv.org/pdf/2111.12077.pdf eq. 18
+                train_frac = np.clip(step / N, 0, 1)
+
+                def bias(x, b):
+                    return b * x / ((b - 1) * x + 1)
+
+                anneal = bias(train_frac, self.config.proposal_weights_anneal_slope)
+                self.proposal_sampler.set_anneal(anneal)
+
+            callbacks.append(
+                TrainingCallback(
+                    where_to_run=[TrainingCallbackLocation.BEFORE_TRAIN_ITERATION],
+                    update_every_num_iters=1,
+                    func=set_anneal,
                 )
-            h = torch.cat([h, embedded_appearance.view(-1, self.appearance_embedding_dim)], dim=-1)
+            )
+            callbacks.append(
+                TrainingCallback(
+                    where_to_run=[TrainingCallbackLocation.AFTER_TRAIN_ITERATION],
+                    update_every_num_iters=1,
+                    func=self.proposal_sampler.step_cb,
+                )
+            )
+
+        return callbacks
 
-        rgb = self.mlp_head(h).view(*ray_samples.frustums.directions.shape[:-1], -1).to(directions)
-        return {FieldHeadNames.RGB: rgb}
+    def sample_and_forward_field(self, ray_bundle: RayBundle) -> Dict[str, Any]:
+        """Sample rays using proposal networks and compute the corresponding field outputs."""
+        ray_samples, weights_list, ray_samples_list = self.proposal_sampler(ray_bundle, density_fns=self.density_fns)
 
-    def density_fn(
-        self, positions: Float[Tensor, "*bs 3"], times: Optional[Float[Tensor, "*bs 1"]] = None
-    ) -> Float[Tensor, "*bs 1"]:
-        """Returns only the density. Used primarily with the density grid.
-        Overwrite this function since density is time dependent now.
-
-        Args:
-            positions: the origin of the samples/frustums
-            times: the time of each position
-        """
-        ray_samples = RaySamples(
-            frustums=Frustums(
-                origins=positions,
-                directions=torch.ones_like(positions),
-                starts=torch.zeros_like(positions[..., :1]),
-                ends=torch.zeros_like(positions[..., :1]),
-                pixel_area=torch.ones_like(positions[..., :1]),
-            ),
-            times=times,
+        field_outputs = self.field(ray_samples, return_alphas=True)
+        weights, transmittance = ray_samples.get_weights_and_transmittance_from_alphas(
+            field_outputs[FieldHeadNames.ALPHA]
         )
-        density, _ = self.get_density(ray_samples)
-        return density
+        bg_transmittance = transmittance[:, -1, :]
+
+        weights_list.append(weights)
+        ray_samples_list.append(ray_samples)
+
+        samples_and_field_outputs = {
+            "ray_samples": ray_samples,
+            "field_outputs": field_outputs,
+            "weights": weights,
+            "bg_transmittance": bg_transmittance,
+            "weights_list": weights_list,
+            "ray_samples_list": ray_samples_list,
+        }
+        return samples_and_field_outputs
+
+    def get_loss_dict(
+        self, outputs: Dict[str, Any], batch: Dict[str, Any], metrics_dict: Optional[Dict[str, Any]] = None
+    ) -> Dict[str, Any]:
+        """Compute the loss dictionary, including interlevel loss for proposal networks."""
+        loss_dict = super().get_loss_dict(outputs, batch, metrics_dict)
+
+        if self.training:
+            loss_dict["interlevel_loss"] = self.config.interlevel_loss_mult * interlevel_loss(
+                outputs["weights_list"], outputs["ray_samples_list"]
+            )
+
+        return loss_dict
+
+    def get_image_metrics_and_images(
+        self, outputs: Dict[str, Any], batch: Dict[str, Any]
+    ) -> Tuple[Dict[str, float], Dict[str, torch.Tensor]]:
+        """Compute image metrics and images, including the proposal depth for each iteration."""
+        metrics_dict, images_dict = super().get_image_metrics_and_images(outputs, batch)
+        for i in range(self.config.num_proposal_iterations):
+            key = f"prop_depth_{i}"
+            prop_depth_i = colormaps.apply_depth_colormap(
+                outputs[key],
+                accumulation=outputs["accumulation"],
+            )
+            images_dict[key] = prop_depth_i
 
-    def get_opacity(self, positions: Float[Tensor, "*bs 3"], step_size, time_intervals=10) -> Float[Tensor, "*bs 1"]:
-        """Returns the opacity for a position and time. Used primarily by the occupancy grid.
-        This will return the maximum opacity of the points in the space in a dynamic sequence.
-
-        Args:
-            positions: the positions to evaluate the opacity at.
-            step_size: the step size to use for the opacity evaluation.
-            time_intervals: sample density on N time stamps
-        """
-        # TODO: Converting opacity by time intervals is slow, and may lead to temporal artifacts.
-        #       (Maybe random sample time and EMA?)
-        opacity = []
-        for t in range(0, time_intervals):
-            density = self.density_fn(positions, t / (time_intervals - 1) * torch.ones_like(positions)[..., [0]])
-            opacity.append(density * step_size)
-        opacity = torch.stack(opacity, dim=0).max(dim=0).values
-        return opacity
+        return metrics_dict, images_dict
```

### Comparing `nerfstudio-0.3.1/nerfstudio/fields/nerfw_field.py` & `nerfstudio-0.3.2/nerfstudio/fields/nerfw_field.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/fields/sdf_field.py` & `nerfstudio-0.3.2/nerfstudio/models/nerfacto.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,456 +9,381 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
-Field for SDF based model, rather then estimating density to generate a surface,
-a signed distance function (SDF) for surface representation is used to help with extracting high fidelity surfaces
+NeRF implementation that combines many recent advancements.
 """
 
+from __future__ import annotations
+
 from dataclasses import dataclass, field
-from typing import Dict, Literal, Optional, Type
+from typing import Dict, List, Literal, Tuple, Type
 
 import numpy as np
 import torch
-import torch.nn.functional as F
-from jaxtyping import Float
-from torch import Tensor, nn
-from torch.nn.parameter import Parameter
-
-from nerfstudio.cameras.rays import RaySamples
-from nerfstudio.field_components.embedding import Embedding
-from nerfstudio.field_components.encodings import NeRFEncoding
-from nerfstudio.field_components.field_heads import FieldHeadNames
-from nerfstudio.field_components.spatial_distortions import SpatialDistortion
-from nerfstudio.fields.base_field import Field, FieldConfig
-
-try:
-    import tinycudann as tcnn
-except ModuleNotFoundError:
-    # tinycudann module doesn't exist
-    pass
-
-
-class LearnedVariance(nn.Module):
-    """Variance network in NeuS
+from torch.nn import Parameter
+from torchmetrics import PeakSignalNoiseRatio
+from torchmetrics.functional import structural_similarity_index_measure
+from torchmetrics.image.lpip import LearnedPerceptualImagePatchSimilarity
 
-    Args:
-        init_val: initial value in NeuS variance network
-    """
-
-    variance: Tensor
-
-    def __init__(self, init_val):
-        super().__init__()
-        self.register_parameter("variance", nn.Parameter(init_val * torch.ones(1), requires_grad=True))
-
-    def forward(self, x: Float[Tensor, "1"]) -> Float[Tensor, "1"]:
-        """Returns current variance value"""
-        return torch.ones([len(x), 1], device=x.device) * torch.exp(self.variance * 10.0)
-
-    def get_variance(self) -> Float[Tensor, "1"]:
-        """return current variance value"""
-        return torch.exp(self.variance * 10.0).clip(1e-6, 1e6)
+from nerfstudio.cameras.rays import RayBundle, RaySamples
+from nerfstudio.engine.callbacks import TrainingCallback, TrainingCallbackAttributes, TrainingCallbackLocation
+from nerfstudio.field_components.field_heads import FieldHeadNames
+from nerfstudio.field_components.spatial_distortions import SceneContraction
+from nerfstudio.fields.density_fields import HashMLPDensityField
+from nerfstudio.fields.nerfacto_field import NerfactoField
+from nerfstudio.model_components.losses import (
+    MSELoss,
+    distortion_loss,
+    interlevel_loss,
+    orientation_loss,
+    pred_normal_loss,
+    scale_gradients_by_distance_squared,
+)
+from nerfstudio.model_components.ray_samplers import ProposalNetworkSampler, UniformSampler
+from nerfstudio.model_components.renderers import AccumulationRenderer, DepthRenderer, NormalsRenderer, RGBRenderer
+from nerfstudio.model_components.scene_colliders import NearFarCollider
+from nerfstudio.model_components.shaders import NormalsShader
+from nerfstudio.models.base_model import Model, ModelConfig
+from nerfstudio.utils import colormaps
 
 
 @dataclass
-class SDFFieldConfig(FieldConfig):
-    """SDF Field Config"""
+class NerfactoModelConfig(ModelConfig):
+    """Nerfacto Model Config"""
 
-    _target: Type = field(default_factory=lambda: SDFField)
-    num_layers: int = 8
-    """Number of layers for geometric network"""
-    hidden_dim: int = 256
-    """Number of hidden dimension of geometric network"""
-    geo_feat_dim: int = 256
-    """Dimension of geometric feature"""
-    num_layers_color: int = 4
-    """Number of layers for color network"""
-    hidden_dim_color: int = 256
-    """Number of hidden dimension of color network"""
-    appearance_embedding_dim: int = 32
-    """Dimension of appearance embedding"""
-    use_appearance_embedding: bool = False
-    """Whether to use appearance embedding"""
-    bias: float = 0.8
-    """Sphere size of geometric initialization"""
-    geometric_init: bool = True
-    """Whether to use geometric initialization"""
-    inside_outside: bool = True
-    """Whether to revert signed distance value, set to True for indoor scene"""
-    weight_norm: bool = True
-    """Whether to use weight norm for linear layer"""
-    use_grid_feature: bool = False
-    """Whether to use multi-resolution feature grids"""
-    divide_factor: float = 2.0
-    """Normalization factor for multi-resolution grids"""
-    beta_init: float = 0.1
-    """Init learnable beta value for transformation of sdf to density"""
-    encoding_type: Literal["hash", "periodic", "tensorf_vm"] = "hash"
-    num_levels = 16
-    """Number of encoding levels"""
-    max_res = 2048
-    """Maximum resolution of the encoding"""
-    base_res = 16
-    """Base resolution of the encoding"""
-    log2_hashmap_size = 19
-    """Size of the hash map"""
-    features_per_level = 2
-    """Number of features per encoding level"""
-    use_hash = True
-    """Whether to use hash encoding"""
-    smoothstep = True
-    """Whether to use the smoothstep function"""
+    _target: Type = field(default_factory=lambda: NerfactoModel)
+    near_plane: float = 0.05
+    """How far along the ray to start sampling."""
+    far_plane: float = 1000.0
+    """How far along the ray to stop sampling."""
+    background_color: Literal["random", "last_sample", "black", "white"] = "last_sample"
+    """Whether to randomize the background color."""
+    hidden_dim: int = 64
+    """Dimension of hidden layers"""
+    hidden_dim_color: int = 64
+    """Dimension of hidden layers for color network"""
+    hidden_dim_transient: int = 64
+    """Dimension of hidden layers for transient network"""
+    num_levels: int = 16
+    """Number of levels of the hashmap for the base mlp."""
+    base_res: int = 16
+    """Resolution of the base grid for the hasgrid."""
+    max_res: int = 2048
+    """Maximum resolution of the hashmap for the base mlp."""
+    log2_hashmap_size: int = 19
+    """Size of the hashmap for the base mlp"""
+    features_per_level: int = 2
+    """How many hashgrid features per level"""
+    num_proposal_samples_per_ray: Tuple[int, ...] = (256, 96)
+    """Number of samples per ray for each proposal network."""
+    num_nerf_samples_per_ray: int = 48
+    """Number of samples per ray for the nerf network."""
+    proposal_update_every: int = 5
+    """Sample every n steps after the warmup"""
+    proposal_warmup: int = 5000
+    """Scales n from 1 to proposal_update_every over this many steps"""
+    num_proposal_iterations: int = 2
+    """Number of proposal network iterations."""
+    use_same_proposal_network: bool = False
+    """Use the same proposal network. Otherwise use different ones."""
+    proposal_net_args_list: List[Dict] = field(
+        default_factory=lambda: [
+            {"hidden_dim": 16, "log2_hashmap_size": 17, "num_levels": 5, "max_res": 128, "use_linear": False},
+            {"hidden_dim": 16, "log2_hashmap_size": 17, "num_levels": 5, "max_res": 256, "use_linear": False},
+        ]
+    )
+    """Arguments for the proposal density fields."""
+    proposal_initial_sampler: Literal["piecewise", "uniform"] = "piecewise"
+    """Initial sampler for the proposal network. Piecewise is preferred for unbounded scenes."""
+    interlevel_loss_mult: float = 1.0
+    """Proposal loss multiplier."""
+    distortion_loss_mult: float = 0.002
+    """Distortion loss multiplier."""
+    orientation_loss_mult: float = 0.0001
+    """Orientation loss multiplier on computed normals."""
+    pred_normal_loss_mult: float = 0.001
+    """Predicted normal loss multiplier."""
+    use_proposal_weight_anneal: bool = True
+    """Whether to use proposal weight annealing."""
+    use_average_appearance_embedding: bool = True
+    """Whether to use average appearance embedding or zeros for inference."""
+    proposal_weights_anneal_slope: float = 10.0
+    """Slope of the annealing function for the proposal weights."""
+    proposal_weights_anneal_max_num_iters: int = 1000
+    """Max num iterations for the annealing function."""
+    use_single_jitter: bool = True
+    """Whether use single jitter or not for the proposal networks."""
+    predict_normals: bool = False
+    """Whether to predict normals or not."""
+    disable_scene_contraction: bool = False
+    """Whether to disable scene contraction or not."""
+    use_gradient_scaling: bool = False
+    """Use gradient scaler where the gradients are lower for points closer to the camera."""
+    implementation: Literal["tcnn", "torch"] = "tcnn"
+    """Which implementation to use for the model."""
+    appearance_embed_dim: int = 32
+    """Dimension of the appearance embedding."""
 
 
-class SDFField(Field):
-    """
-    A field for Signed Distance Functions (SDF).
+class NerfactoModel(Model):
+    """Nerfacto model
 
     Args:
-        config: The configuration for the SDF field.
-        aabb: An axis-aligned bounding box for the SDF field.
-        num_images: The number of images for embedding appearance.
-        use_average_appearance_embedding: Whether to use average appearance embedding. Defaults to False.
-        spatial_distortion: The spatial distortion. Defaults to None.
+        config: Nerfacto configuration to instantiate model
     """
 
-    config: SDFFieldConfig
+    config: NerfactoModelConfig
 
-    def __init__(
-        self,
-        config: SDFFieldConfig,
-        aabb: Float[Tensor, "2 3"],
-        num_images: int,
-        use_average_appearance_embedding: bool = False,
-        spatial_distortion: Optional[SpatialDistortion] = None,
-    ) -> None:
-        super().__init__()
-        self.config = config
-
-        self.aabb = Parameter(aabb, requires_grad=False)
-
-        self.spatial_distortion = spatial_distortion
-        self.num_images = num_images
-
-        self.embedding_appearance = Embedding(self.num_images, self.config.appearance_embedding_dim)
-        self.use_average_appearance_embedding = use_average_appearance_embedding
-        self.use_grid_feature = self.config.use_grid_feature
-        self.divide_factor = self.config.divide_factor
-
-        growth_factor = np.exp((np.log(config.max_res) - np.log(config.base_res)) / (config.num_levels - 1))
-
-        if self.config.encoding_type == "hash":
-            # feature encoding
-            self.encoding = tcnn.Encoding(
-                n_input_dims=3,
-                encoding_config={
-                    "otype": "HashGrid" if config.use_hash else "DenseGrid",
-                    "n_levels": config.num_levels,
-                    "n_features_per_level": config.features_per_level,
-                    "log2_hashmap_size": config.log2_hashmap_size,
-                    "base_resolution": config.base_res,
-                    "per_level_scale": growth_factor,
-                    "interpolation": "Smoothstep" if config.smoothstep else "Linear",
-                },
-            )
+    def populate_modules(self):
+        """Set the fields and modules."""
+        super().populate_modules()
 
-        # we concat inputs position ourselves
-        self.position_encoding = NeRFEncoding(
-            in_dim=3, num_frequencies=6, min_freq_exp=0.0, max_freq_exp=5.0, include_input=False
-        )
+        if self.config.disable_scene_contraction:
+            scene_contraction = None
+        else:
+            scene_contraction = SceneContraction(order=float("inf"))
 
-        self.direction_encoding = NeRFEncoding(
-            in_dim=3, num_frequencies=4, min_freq_exp=0.0, max_freq_exp=3.0, include_input=True
+        # Fields
+        self.field = NerfactoField(
+            self.scene_box.aabb,
+            hidden_dim=self.config.hidden_dim,
+            num_levels=self.config.num_levels,
+            max_res=self.config.max_res,
+            log2_hashmap_size=self.config.log2_hashmap_size,
+            hidden_dim_color=self.config.hidden_dim_color,
+            hidden_dim_transient=self.config.hidden_dim_transient,
+            spatial_distortion=scene_contraction,
+            num_images=self.num_train_data,
+            use_pred_normals=self.config.predict_normals,
+            use_average_appearance_embedding=self.config.use_average_appearance_embedding,
+            appearance_embedding_dim=self.config.appearance_embed_dim,
+            implementation=self.config.implementation,
         )
 
-        # initialize geometric network
-        self.initialize_geo_layers()
+        self.density_fns = []
+        num_prop_nets = self.config.num_proposal_iterations
+        # Build the proposal network(s)
+        self.proposal_networks = torch.nn.ModuleList()
+        if self.config.use_same_proposal_network:
+            assert len(self.config.proposal_net_args_list) == 1, "Only one proposal network is allowed."
+            prop_net_args = self.config.proposal_net_args_list[0]
+            network = HashMLPDensityField(
+                self.scene_box.aabb,
+                spatial_distortion=scene_contraction,
+                **prop_net_args,
+                implementation=self.config.implementation,
+            )
+            self.proposal_networks.append(network)
+            self.density_fns.extend([network.density_fn for _ in range(num_prop_nets)])
+        else:
+            for i in range(num_prop_nets):
+                prop_net_args = self.config.proposal_net_args_list[min(i, len(self.config.proposal_net_args_list) - 1)]
+                network = HashMLPDensityField(
+                    self.scene_box.aabb,
+                    spatial_distortion=scene_contraction,
+                    **prop_net_args,
+                    implementation=self.config.implementation,
+                )
+                self.proposal_networks.append(network)
+            self.density_fns.extend([network.density_fn for network in self.proposal_networks])
 
-        # deviation_network to compute alpha from sdf from NeuS
-        self.deviation_network = LearnedVariance(init_val=self.config.beta_init)
+        # Samplers
+        def update_schedule(step):
+            return np.clip(
+                np.interp(step, [0, self.config.proposal_warmup], [0, self.config.proposal_update_every]),
+                1,
+                self.config.proposal_update_every,
+            )
 
-        # color network
-        dims = [self.config.hidden_dim_color for _ in range(self.config.num_layers_color)]
-        # point, view_direction, normal, feature, embedding
-        in_dim = (
-            3
-            + self.direction_encoding.get_out_dim()
-            + 3
-            + self.config.geo_feat_dim
-            + self.embedding_appearance.get_out_dim()
+        # Change proposal network initial sampler if uniform
+        initial_sampler = None  # None is for piecewise as default (see ProposalNetworkSampler)
+        if self.config.proposal_initial_sampler == "uniform":
+            initial_sampler = UniformSampler(single_jitter=self.config.use_single_jitter)
+
+        self.proposal_sampler = ProposalNetworkSampler(
+            num_nerf_samples_per_ray=self.config.num_nerf_samples_per_ray,
+            num_proposal_samples_per_ray=self.config.num_proposal_samples_per_ray,
+            num_proposal_network_iterations=self.config.num_proposal_iterations,
+            single_jitter=self.config.use_single_jitter,
+            update_sched=update_schedule,
+            initial_sampler=initial_sampler,
         )
-        dims = [in_dim] + dims + [3]
-        self.num_layers_color = len(dims)
-
-        for layer in range(0, self.num_layers_color - 1):
-            out_dim = dims[layer + 1]
-            lin = nn.Linear(dims[layer], out_dim)
-
-            if self.config.weight_norm:
-                lin = nn.utils.weight_norm(lin)
-            setattr(self, "clin" + str(layer), lin)
-
-        self.softplus = nn.Softplus(beta=100)
-        self.relu = nn.ReLU()
-        self.sigmoid = torch.nn.Sigmoid()
-
-        self._cos_anneal_ratio = 1.0
-
-        if self.use_grid_feature:
-            assert self.spatial_distortion is not None, "spatial distortion must be provided when using grid feature"
-
-    def initialize_geo_layers(self) -> None:
-        """
-        Initialize layers for geometric network (sdf)
-        """
-        # MLP with geometric initialization
-        dims = [self.config.hidden_dim for _ in range(self.config.num_layers)]
-        in_dim = 3 + self.position_encoding.get_out_dim() + self.encoding.n_output_dims
-        dims = [in_dim] + dims + [1 + self.config.geo_feat_dim]
-        self.num_layers = len(dims)
-        self.skip_in = [4]
-
-        for layer in range(0, self.num_layers - 1):
-            if layer + 1 in self.skip_in:
-                out_dim = dims[layer + 1] - dims[0]
-            else:
-                out_dim = dims[layer + 1]
-
-            lin = nn.Linear(dims[layer], out_dim)
-
-            if self.config.geometric_init:
-                if layer == self.num_layers - 2:
-                    if not self.config.inside_outside:
-                        torch.nn.init.normal_(lin.weight, mean=np.sqrt(np.pi) / np.sqrt(dims[layer]), std=0.0001)
-                        torch.nn.init.constant_(lin.bias, -self.config.bias)
-                    else:
-                        torch.nn.init.normal_(lin.weight, mean=-np.sqrt(np.pi) / np.sqrt(dims[layer]), std=0.0001)
-                        torch.nn.init.constant_(lin.bias, self.config.bias)
-                elif layer == 0:
-                    torch.nn.init.constant_(lin.bias, 0.0)
-                    torch.nn.init.constant_(lin.weight[:, 3:], 0.0)
-                    torch.nn.init.normal_(lin.weight[:, :3], 0.0, np.sqrt(2) / np.sqrt(out_dim))
-                elif layer in self.skip_in:
-                    torch.nn.init.constant_(lin.bias, 0.0)
-                    torch.nn.init.normal_(lin.weight, 0.0, np.sqrt(2) / np.sqrt(out_dim))
-                    torch.nn.init.constant_(lin.weight[:, -(dims[0] - 3) :], 0.0)
-                else:
-                    torch.nn.init.constant_(lin.bias, 0.0)
-                    torch.nn.init.normal_(lin.weight, 0.0, np.sqrt(2) / np.sqrt(out_dim))
-
-            if self.config.weight_norm:
-                lin = nn.utils.weight_norm(lin)
-            setattr(self, "glin" + str(layer), lin)
-
-    def set_cos_anneal_ratio(self, anneal: float) -> None:
-        """Set the anneal value for the proposal network."""
-        self._cos_anneal_ratio = anneal
-
-    def forward_geonetwork(self, inputs: Float[Tensor, "*batch 3"]) -> Float[Tensor, "*batch geo_features+1"]:
-        """forward the geonetwork"""
-        if self.use_grid_feature:
-            assert self.spatial_distortion is not None, "spatial distortion must be provided when using grid feature"
-            positions = self.spatial_distortion(inputs)
-            # map range [-2, 2] to [0, 1]
-            positions = (positions + 2.0) / 4.0
-            feature = self.encoding(positions)
-        else:
-            feature = torch.zeros_like(inputs[:, :1].repeat(1, self.encoding.n_output_dims))
 
-        pe = self.position_encoding(inputs)
+        # Collider
+        self.collider = NearFarCollider(near_plane=self.config.near_plane, far_plane=self.config.far_plane)
 
-        inputs = torch.cat((inputs, pe, feature), dim=-1)
+        # renderers
+        self.renderer_rgb = RGBRenderer(background_color=self.config.background_color)
+        self.renderer_accumulation = AccumulationRenderer()
+        self.renderer_depth = DepthRenderer()
+        self.renderer_normals = NormalsRenderer()
+
+        # shaders
+        self.normals_shader = NormalsShader()
+
+        # losses
+        self.rgb_loss = MSELoss()
+
+        # metrics
+        self.psnr = PeakSignalNoiseRatio(data_range=1.0)
+        self.ssim = structural_similarity_index_measure
+        self.lpips = LearnedPerceptualImagePatchSimilarity(normalize=True)
+
+    def get_param_groups(self) -> Dict[str, List[Parameter]]:
+        param_groups = {}
+        param_groups["proposal_networks"] = list(self.proposal_networks.parameters())
+        param_groups["fields"] = list(self.field.parameters())
+        return param_groups
+
+    def get_training_callbacks(
+        self, training_callback_attributes: TrainingCallbackAttributes
+    ) -> List[TrainingCallback]:
+        callbacks = []
+        if self.config.use_proposal_weight_anneal:
+            # anneal the weights of the proposal network before doing PDF sampling
+            N = self.config.proposal_weights_anneal_max_num_iters
+
+            def set_anneal(step):
+                # https://arxiv.org/pdf/2111.12077.pdf eq. 18
+                train_frac = np.clip(step / N, 0, 1)
+
+                def bias(x, b):
+                    return b * x / ((b - 1) * x + 1)
+
+                anneal = bias(train_frac, self.config.proposal_weights_anneal_slope)
+                self.proposal_sampler.set_anneal(anneal)
+
+            callbacks.append(
+                TrainingCallback(
+                    where_to_run=[TrainingCallbackLocation.BEFORE_TRAIN_ITERATION],
+                    update_every_num_iters=1,
+                    func=set_anneal,
+                )
+            )
+            callbacks.append(
+                TrainingCallback(
+                    where_to_run=[TrainingCallbackLocation.AFTER_TRAIN_ITERATION],
+                    update_every_num_iters=1,
+                    func=self.proposal_sampler.step_cb,
+                )
+            )
+        return callbacks
 
-        # Pass through layers
-        outputs = inputs
+    def get_outputs(self, ray_bundle: RayBundle):
+        ray_samples: RaySamples
+        ray_samples, weights_list, ray_samples_list = self.proposal_sampler(ray_bundle, density_fns=self.density_fns)
+        field_outputs = self.field.forward(ray_samples, compute_normals=self.config.predict_normals)
+        if self.config.use_gradient_scaling:
+            field_outputs = scale_gradients_by_distance_squared(field_outputs, ray_samples)
+
+        weights = ray_samples.get_weights(field_outputs[FieldHeadNames.DENSITY])
+        weights_list.append(weights)
+        ray_samples_list.append(ray_samples)
+
+        rgb = self.renderer_rgb(rgb=field_outputs[FieldHeadNames.RGB], weights=weights)
+        depth = self.renderer_depth(weights=weights, ray_samples=ray_samples)
+        accumulation = self.renderer_accumulation(weights=weights)
+
+        outputs = {
+            "rgb": rgb,
+            "accumulation": accumulation,
+            "depth": depth,
+        }
+
+        if self.config.predict_normals:
+            normals = self.renderer_normals(normals=field_outputs[FieldHeadNames.NORMALS], weights=weights)
+            pred_normals = self.renderer_normals(field_outputs[FieldHeadNames.PRED_NORMALS], weights=weights)
+            outputs["normals"] = self.normals_shader(normals)
+            outputs["pred_normals"] = self.normals_shader(pred_normals)
+        # These use a lot of GPU memory, so we avoid storing them for eval.
+        if self.training:
+            outputs["weights_list"] = weights_list
+            outputs["ray_samples_list"] = ray_samples_list
 
-        for layer in range(0, self.num_layers - 1):
-            lin = getattr(self, "glin" + str(layer))
+        if self.training and self.config.predict_normals:
+            outputs["rendered_orientation_loss"] = orientation_loss(
+                weights.detach(), field_outputs[FieldHeadNames.NORMALS], ray_bundle.directions
+            )
 
-            if layer in self.skip_in:
-                outputs = torch.cat([outputs, inputs], 1) / np.sqrt(2)
+            outputs["rendered_pred_normal_loss"] = pred_normal_loss(
+                weights.detach(),
+                field_outputs[FieldHeadNames.NORMALS].detach(),
+                field_outputs[FieldHeadNames.PRED_NORMALS],
+            )
 
-            outputs = lin(outputs)
+        for i in range(self.config.num_proposal_iterations):
+            outputs[f"prop_depth_{i}"] = self.renderer_depth(weights=weights_list[i], ray_samples=ray_samples_list[i])
 
-            if layer < self.num_layers - 2:
-                outputs = self.softplus(outputs)
         return outputs
 
-    # TODO: fix ... in shape annotations.
-    def get_sdf(self, ray_samples: RaySamples) -> Float[Tensor, "num_samples ... 1"]:
-        """predict the sdf value for ray samples"""
-        positions = ray_samples.frustums.get_start_positions()
-        positions_flat = positions.view(-1, 3)
-        hidden_output = self.forward_geonetwork(positions_flat).view(*ray_samples.frustums.shape, -1)
-        sdf, _ = torch.split(hidden_output, [1, self.config.geo_feat_dim], dim=-1)
-        return sdf
-
-    def get_alpha(
-        self,
-        ray_samples: RaySamples,
-        sdf: Optional[Float[Tensor, "num_samples ... 1"]] = None,
-        gradients: Optional[Float[Tensor, "num_samples ... 1"]] = None,
-    ) -> Float[Tensor, "num_samples ... 1"]:
-        """compute alpha from sdf as in NeuS"""
-        if sdf is None or gradients is None:
-            inputs = ray_samples.frustums.get_start_positions()
-            inputs.requires_grad_(True)
-            with torch.enable_grad():
-                hidden_output = self.forward_geonetwork(inputs)
-                sdf, _ = torch.split(hidden_output, [1, self.config.geo_feat_dim], dim=-1)
-            d_output = torch.ones_like(sdf, requires_grad=False, device=sdf.device)
-            gradients = torch.autograd.grad(
-                outputs=sdf,
-                inputs=inputs,
-                grad_outputs=d_output,
-                create_graph=True,
-                retain_graph=True,
-                only_inputs=True,
-            )[0]
-
-        inv_s = self.deviation_network.get_variance()  # Single parameter
-
-        true_cos = (ray_samples.frustums.directions * gradients).sum(-1, keepdim=True)
-
-        # anneal as NeuS
-        cos_anneal_ratio = self._cos_anneal_ratio
-
-        # "cos_anneal_ratio" grows from 0 to 1 in the beginning training iterations. The anneal strategy below makes
-        # the cos value "not dead" at the beginning training iterations, for better convergence.
-        iter_cos = -(
-            F.relu(-true_cos * 0.5 + 0.5) * (1.0 - cos_anneal_ratio) + F.relu(-true_cos) * cos_anneal_ratio
-        )  # always non-positive
-
-        # Estimate signed distances at section points
-        estimated_next_sdf = sdf + iter_cos * ray_samples.deltas * 0.5
-        estimated_prev_sdf = sdf - iter_cos * ray_samples.deltas * 0.5
-
-        prev_cdf = torch.sigmoid(estimated_prev_sdf * inv_s)
-        next_cdf = torch.sigmoid(estimated_next_sdf * inv_s)
-
-        p = prev_cdf - next_cdf
-        c = prev_cdf
-
-        alpha = ((p + 1e-5) / (c + 1e-5)).clip(0.0, 1.0)
-
-        return alpha
-
-    def get_density(self, ray_samples: RaySamples):
-        raise NotImplementedError
-
-    def get_colors(
-        self,
-        points: Float[Tensor, "*batch 3"],
-        directions: Float[Tensor, "*batch 3"],
-        normals: Float[Tensor, "*batch 3"],
-        geo_features: Float[Tensor, "*batch geo_feat_dim"],
-        camera_indices: Tensor,
-    ) -> Float[Tensor, "*batch 3"]:
-        """compute colors"""
-        d = self.direction_encoding(directions)
+    def get_metrics_dict(self, outputs, batch):
+        metrics_dict = {}
+        image = batch["image"].to(self.device)
+        metrics_dict["psnr"] = self.psnr(outputs["rgb"], image)
+        if self.training:
+            metrics_dict["distortion"] = distortion_loss(outputs["weights_list"], outputs["ray_samples_list"])
+        return metrics_dict
 
-        # appearance
+    def get_loss_dict(self, outputs, batch, metrics_dict=None):
+        loss_dict = {}
+        image = batch["image"].to(self.device)
+        loss_dict["rgb_loss"] = self.rgb_loss(image, outputs["rgb"])
         if self.training:
-            embedded_appearance = self.embedding_appearance(camera_indices)
-            # set it to zero if don't use it
-            if not self.config.use_appearance_embedding:
-                embedded_appearance = torch.zeros_like(embedded_appearance)
-        else:
-            if self.use_average_appearance_embedding:
-                embedded_appearance = torch.ones(
-                    (*directions.shape[:-1], self.config.appearance_embedding_dim), device=directions.device
-                ) * self.embedding_appearance.mean(dim=0)
-            else:
-                embedded_appearance = torch.zeros(
-                    (*directions.shape[:-1], self.config.appearance_embedding_dim), device=directions.device
+            loss_dict["interlevel_loss"] = self.config.interlevel_loss_mult * interlevel_loss(
+                outputs["weights_list"], outputs["ray_samples_list"]
+            )
+            assert metrics_dict is not None and "distortion" in metrics_dict
+            loss_dict["distortion_loss"] = self.config.distortion_loss_mult * metrics_dict["distortion"]
+            if self.config.predict_normals:
+                # orientation loss for computed normals
+                loss_dict["orientation_loss"] = self.config.orientation_loss_mult * torch.mean(
+                    outputs["rendered_orientation_loss"]
                 )
 
-        hidden_input = torch.cat(
-            [
-                points,
-                d,
-                normals,
-                geo_features.view(-1, self.config.geo_feat_dim),
-                embedded_appearance.view(-1, self.config.appearance_embedding_dim),
-            ],
-            dim=-1,
-        )
-
-        for layer in range(0, self.num_layers_color - 1):
-            lin = getattr(self, "clin" + str(layer))
-
-            hidden_input = lin(hidden_input)
-
-            if layer < self.num_layers_color - 2:
-                hidden_input = self.relu(hidden_input)
+                # ground truth supervision for normals
+                loss_dict["pred_normal_loss"] = self.config.pred_normal_loss_mult * torch.mean(
+                    outputs["rendered_pred_normal_loss"]
+                )
+        return loss_dict
 
-        rgb = self.sigmoid(hidden_input)
-
-        return rgb
-
-    def get_outputs(
-        self,
-        ray_samples: RaySamples,
-        density_embedding: Optional[Tensor] = None,
-        return_alphas: bool = False,
-    ) -> Dict[FieldHeadNames, Tensor]:
-        """compute output of ray samples"""
-        if ray_samples.camera_indices is None:
-            raise AttributeError("Camera indices are not provided.")
-
-        outputs = {}
-
-        camera_indices = ray_samples.camera_indices.squeeze()
-
-        inputs = ray_samples.frustums.get_start_positions()
-        inputs = inputs.view(-1, 3)
-
-        directions = ray_samples.frustums.directions
-        directions_flat = directions.reshape(-1, 3)
-
-        inputs.requires_grad_(True)
-        with torch.enable_grad():
-            hidden_output = self.forward_geonetwork(inputs)
-            sdf, geo_feature = torch.split(hidden_output, [1, self.config.geo_feat_dim], dim=-1)
-        d_output = torch.ones_like(sdf, requires_grad=False, device=sdf.device)
-        gradients = torch.autograd.grad(
-            outputs=sdf, inputs=inputs, grad_outputs=d_output, create_graph=True, retain_graph=True, only_inputs=True
-        )[0]
-
-        rgb = self.get_colors(inputs, directions_flat, gradients, geo_feature, camera_indices)
-
-        rgb = rgb.view(*ray_samples.frustums.directions.shape[:-1], -1)
-        sdf = sdf.view(*ray_samples.frustums.directions.shape[:-1], -1)
-        gradients = gradients.view(*ray_samples.frustums.directions.shape[:-1], -1)
-        normals = torch.nn.functional.normalize(gradients, p=2, dim=-1)
-
-        outputs.update(
-            {
-                FieldHeadNames.RGB: rgb,
-                FieldHeadNames.SDF: sdf,
-                FieldHeadNames.NORMALS: normals,
-                FieldHeadNames.GRADIENT: gradients,
-            }
+    def get_image_metrics_and_images(
+        self, outputs: Dict[str, torch.Tensor], batch: Dict[str, torch.Tensor]
+    ) -> Tuple[Dict[str, float], Dict[str, torch.Tensor]]:
+        image = batch["image"].to(self.device)
+        rgb = outputs["rgb"]
+        acc = colormaps.apply_colormap(outputs["accumulation"])
+        depth = colormaps.apply_depth_colormap(
+            outputs["depth"],
+            accumulation=outputs["accumulation"],
         )
 
-        if return_alphas:
-            alphas = self.get_alpha(ray_samples, sdf, gradients)
-            outputs.update({FieldHeadNames.ALPHA: alphas})
-
-        return outputs
+        combined_rgb = torch.cat([image, rgb], dim=1)
+        combined_acc = torch.cat([acc], dim=1)
+        combined_depth = torch.cat([depth], dim=1)
+
+        # Switch images from [H, W, C] to [1, C, H, W] for metrics computations
+        image = torch.moveaxis(image, -1, 0)[None, ...]
+        rgb = torch.moveaxis(rgb, -1, 0)[None, ...]
+
+        psnr = self.psnr(image, rgb)
+        ssim = self.ssim(image, rgb)
+        lpips = self.lpips(image, rgb)
+
+        # all of these metrics will be logged as scalars
+        metrics_dict = {"psnr": float(psnr.item()), "ssim": float(ssim)}  # type: ignore
+        metrics_dict["lpips"] = float(lpips)
+
+        images_dict = {"img": combined_rgb, "accumulation": combined_acc, "depth": combined_depth}
+
+        for i in range(self.config.num_proposal_iterations):
+            key = f"prop_depth_{i}"
+            prop_depth_i = colormaps.apply_depth_colormap(
+                outputs[key],
+                accumulation=outputs["accumulation"],
+            )
+            images_dict[key] = prop_depth_i
 
-    def forward(
-        self, ray_samples: RaySamples, compute_normals: bool = False, return_alphas: bool = False
-    ) -> Dict[FieldHeadNames, Tensor]:
-        """Evaluates the field at points along the ray.
-
-        Args:
-            ray_samples: Samples to evaluate field on.
-            compute normals: not currently used in this implementation.
-            return_alphas: Whether to return alpha values
-        """
-        field_outputs = self.get_outputs(ray_samples, return_alphas=return_alphas)
-        return field_outputs
+        return metrics_dict, images_dict
```

### Comparing `nerfstudio-0.3.1/nerfstudio/fields/semantic_nerf_field.py` & `nerfstudio-0.3.2/nerfstudio/fields/semantic_nerf_field.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/fields/tensorf_field.py` & `nerfstudio-0.3.2/nerfstudio/fields/tensorf_field.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/fields/vanilla_nerf_field.py` & `nerfstudio-0.3.2/nerfstudio/fields/vanilla_nerf_field.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/generative/__init__.py` & `nerfstudio-0.3.2/nerfstudio/generative/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/generative/stable_diffusion.py` & `nerfstudio-0.3.2/nerfstudio/generative/stable_diffusion.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,78 +12,46 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Stable Diffusion helpers"""
 
 # Modified from https://github.com/ashawkey/stable-dreamfusion/blob/main/nerf/sd.py
 
-import sys
-from dataclasses import dataclass
 from pathlib import Path
-from typing import List, Optional, Union, cast
+from typing import List, Optional, Union
+from nerfstudio.utils.rich_utils import CONSOLE
 
 import mediapy
 import numpy as np
 import torch
 import torch.nn.functional as F
 import tyro
 from jaxtyping import Float
 from torch import Tensor, nn
-from torch.cuda.amp import custom_bwd, custom_fwd
 from torch.cuda.amp.grad_scaler import GradScaler
 
-from nerfstudio.utils.rich_utils import CONSOLE
+from nerfstudio.generative.utils import CatchMissingPackages
+
 
 try:
-    from diffusers import PNDMScheduler, StableDiffusionPipeline
-    from transformers import logging
+    from diffusers import PNDMScheduler, StableDiffusionPipeline, DiffusionPipeline
 
 except ImportError:
-    CONSOLE.print("[bold red]Missing Stable Diffusion packages.")
-    CONSOLE.print(r"Install using [yellow]pip install nerfstudio\[gen][/yellow]")
-    CONSOLE.print(r"or [yellow]pip install -e .\[gen][/yellow] if installing from source.")
-    sys.exit(1)
+    PNDMScheduler = StableDiffusionPipeline = CatchMissingPackages()
+
 
-logging.set_verbosity_error()
 IMG_DIM = 512
 CONST_SCALE = 0.18215
 SD_IDENTIFIERS = {
     "1-5": "runwayml/stable-diffusion-v1-5",
     "2-0": "stabilityai/stable-diffusion-2-base",
     "2-1": "stabilityai/stable-diffusion-2-1-base",
 }
 
 
-@dataclass
-class UNet2DConditionOutput:
-    """Class to hold traced model"""
-
-    sample: torch.FloatTensor
-
-
-class _SDSGradient(torch.autograd.Function):
-    """Custom gradient function for SDS loss. Since it is already computed, we can just return it."""
-
-    @staticmethod
-    @custom_fwd
-    def forward(ctx, input_tensor, gt_grad):
-        del input_tensor
-        ctx.save_for_backward(gt_grad)
-        # Return magniture of gradient, not the actual loss.
-        return torch.mean(gt_grad**2) ** 0.5
-
-    @staticmethod
-    @custom_bwd
-    def backward(ctx, grad):
-        del grad
-        (gt_grad,) = ctx.saved_tensors
-        batch_size = len(gt_grad)
-        return gt_grad / batch_size, None
-
-
 class StableDiffusion(nn.Module):
     """Stable Diffusion implementation
     Args:
         device: device to use
         num_train_timesteps: number of training timesteps
     """
 
@@ -102,15 +70,16 @@
             beta_schedule="scaled_linear",
             num_train_timesteps=self.num_train_timesteps,
         )
         self.alphas = self.scheduler.alphas_cumprod.to(self.device)  # type: ignore
 
         sd_id = SD_IDENTIFIERS[version]
         pipe = StableDiffusionPipeline.from_pretrained(sd_id, torch_dtype=torch.float16)
-        assert isinstance(pipe, StableDiffusionPipeline)
+
+        assert isinstance(pipe, DiffusionPipeline)  # and hasattr(pipe, "to")
         pipe = pipe.to(self.device)
 
         pipe.enable_attention_slicing()
 
         self.unet = pipe.unet
         self.unet.to(memory_format=torch.channels_last)
 
@@ -168,15 +137,15 @@
             text_embeddings: Text embeddings
             image: Rendered image
             guidance_scale: How much to weigh the guidance
             grad_scaler: Grad scaler
         Returns:
             The loss
         """
-        image = F.interpolate(image, (IMG_DIM, IMG_DIM), mode="bilinear")
+        image = F.interpolate(image, (IMG_DIM, IMG_DIM), mode="bilinear").to(torch.float16)
         t = torch.randint(self.min_step, self.max_step + 1, [1], dtype=torch.long, device=self.device)
         latents = self.imgs_to_latent(image)
 
         # predict the noise residual with unet, NO grad!
         with torch.no_grad():
             # add noise
             noise = torch.randn_like(latents)
@@ -191,17 +160,16 @@
 
         # w(t), sigma_t^2
         w = 1 - self.alphas[t]
 
         grad = w * (noise_pred - noise)
         grad = torch.nan_to_num(grad)
 
-        if grad_scaler is not None:
-            latents = grad_scaler.scale(latents)
-        loss = cast(Tensor, _SDSGradient.apply(latents, grad))
+        target = (latents - grad).detach()
+        loss = 0.5 * F.mse_loss(latents, target, reduction="sum") / latents.shape[0]
 
         return loss
 
     def produce_latents(
         self,
         text_embeddings: Float[Tensor, "N max_length embed_dim"],
         height: int = IMG_DIM,
@@ -220,15 +188,16 @@
             latents: Latents to start with
         Returns:
             Latents
         """
 
         if latents is None:
             latents = torch.randn(
-                (text_embeddings.shape[0] // 2, self.unet.in_channels, height // 8, width // 8), device=self.device
+                (text_embeddings.shape[0] // 2, self.unet.config.in_channels, height // 8, width // 8),
+                device=self.device,
             )
 
         self.scheduler.set_timesteps(num_inference_steps)  # type: ignore
 
         with torch.autocast("cuda"):
             for t in self.scheduler.timesteps:  # type: ignore
                 assert latents is not None
@@ -243,14 +212,15 @@
 
                 # perform guidance
                 noise_pred_uncond, noise_pred_text = noise_pred.chunk(2)
                 noise_pred = noise_pred_text + guidance_scale * (noise_pred_text - noise_pred_uncond)
 
                 # compute the previous noisy sample x_t -> x_t-1
                 latents = self.scheduler.step(noise_pred, t, latents)["prev_sample"]  # type: ignore
+        assert isinstance(latents, Tensor)
         return latents
 
     def latents_to_img(self, latents: Float[Tensor, "BS 4 H W"]) -> Float[Tensor, "BS 3 H W"]:
         """Convert latents to images
         Args:
             latents: Latents to convert
         Returns:
```

### Comparing `nerfstudio-0.3.1/nerfstudio/model_components/__init__.py` & `nerfstudio-0.3.2/nerfstudio/model_components/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/model_components/losses.py` & `nerfstudio-0.3.2/nerfstudio/model_components/losses.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,17 +73,17 @@
     cy1_hi = torch.take_along_dim(cy1[..., 1:], idx_hi, dim=-1)
     y0_outer = cy1_hi - cy1_lo
 
     return y0_outer
 
 
 def lossfun_outer(
-    t: Float[Tensor, "*batch num_samples+1"],
+    t: Float[Tensor, "*batch num_samples_1"],
     w: Float[Tensor, "*batch num_samples"],
-    t_env: Float[Tensor, "*batch num_samples+1"],
+    t_env: Float[Tensor, "*batch num_samples_1"],
     w_env: Float[Tensor, "*batch num_samples"],
 ):
     """
     https://github.com/kakaobrain/NeRF-Factory/blob/f61bb8744a5cb4820a4d968fb3bfbed777550f4a/src/model/mipnerf360/helper.py#L136
     https://github.com/google-research/multinerf/blob/b02228160d3179300c7d499dca28cb9ca3677f32/internal/stepfun.py#L80
 
     Args:
@@ -538,15 +538,16 @@
     @staticmethod
     def backward(ctx, output_grad, grad_scaling):
         (scaling,) = ctx.saved_tensors
         return output_grad * scaling, grad_scaling
 
 
 def scale_gradients_by_distance_squared(
-    field_outputs: Dict[FieldHeadNames, torch.Tensor], ray_samples: RaySamples
+    field_outputs: Dict[FieldHeadNames, torch.Tensor],
+    ray_samples: RaySamples,
 ) -> Dict[FieldHeadNames, torch.Tensor]:
     """
     Scale gradients by the ray distance to the pixel
     as suggested in `Radiance Field Gradient Scaling for Unbiased Near-Camera Training` paper
 
     Note: The scaling is applied on the interval of [0, 1] along the ray!
```

### Comparing `nerfstudio-0.3.1/nerfstudio/model_components/ray_generators.py` & `nerfstudio-0.3.2/nerfstudio/model_components/ray_generators.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/model_components/ray_samplers.py` & `nerfstudio-0.3.2/nerfstudio/model_components/ray_samplers.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 
 """
 Collection of sampling strategies
 """
 
 from abc import abstractmethod
-from typing import Callable, List, Optional, Protocol, Tuple, Union
+from typing import Any, Callable, List, Optional, Protocol, Tuple, Union
 
 import torch
 from jaxtyping import Float
 from nerfacc import OccGridEstimator
 from torch import Tensor, nn
 
 from nerfstudio.cameras.rays import Frustums, RayBundle, RaySamples
@@ -38,18 +38,18 @@
         self,
         num_samples: Optional[int] = None,
     ) -> None:
         super().__init__()
         self.num_samples = num_samples
 
     @abstractmethod
-    def generate_ray_samples(self) -> RaySamples:
+    def generate_ray_samples(self) -> Any:
         """Generate Ray Samples"""
 
-    def forward(self, *args, **kwargs) -> RaySamples:
+    def forward(self, *args, **kwargs) -> Any:
         """Generate ray samples"""
         return self.generate_ray_samples(*args, **kwargs)
 
 
 class SpacedSampler(Sampler):
     """Sample points according to a function.
```

### Comparing `nerfstudio-0.3.1/nerfstudio/model_components/renderers.py` & `nerfstudio-0.3.2/nerfstudio/model_components/renderers.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/model_components/scene_colliders.py` & `nerfstudio-0.3.2/nerfstudio/model_components/scene_colliders.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 
 import torch
 from jaxtyping import Float
 from torch import Tensor, nn
 
 from nerfstudio.cameras.rays import RayBundle
 from nerfstudio.data.scene_box import SceneBox
-from nerfstudio.utils.misc import torch_compile
 
 
 class SceneCollider(nn.Module):
     """Module for setting near and far values for rays."""
 
     def __init__(self, **kwargs) -> None:
         self.kwargs = kwargs
@@ -105,15 +104,14 @@
         aabb = self.scene_box.aabb
         nears, fars = self._intersect_with_aabb(ray_bundle.origins, ray_bundle.directions, aabb)
         ray_bundle.nears = nears[..., None]
         ray_bundle.fars = fars[..., None]
         return ray_bundle
 
 
-@torch_compile(dynamic=True, mode="reduce-overhead")
 def _intersect_with_sphere(
     rays_o: torch.Tensor, rays_d: torch.Tensor, center: torch.Tensor, radius: float = 1.0, near_plane: float = 0.0
 ):
     a = (rays_d * rays_d).sum(dim=-1, keepdim=True)
     b = 2 * (rays_o - center) * rays_d
     b = b.sum(dim=-1, keepdim=True)
     c = (rays_o - center) * (rays_o - center)
@@ -133,15 +131,15 @@
 
 
 class SphereCollider(SceneCollider):
     """Module for colliding rays with the scene box to compute near and far values.
 
     Args:
         center: center of sphere to intersect [3]
-        redius: radius of sphere to intersect
+        radius: radius of sphere to intersect
         near_plane: near plane to clamp to
     """
 
     def __init__(self, center: torch.Tensor, radius: float, near_plane: float = 0.0, **kwargs) -> None:
         super().__init__(**kwargs)
         self.center = center
         self.radius = radius
```

### Comparing `nerfstudio-0.3.1/nerfstudio/model_components/shaders.py` & `nerfstudio-0.3.2/nerfstudio/model_components/shaders.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/models/__init__.py` & `nerfstudio-0.3.2/nerfstudio/models/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/models/base_model.py` & `nerfstudio-0.3.2/nerfstudio/models/base_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 """
 
 from __future__ import annotations
 
 from abc import abstractmethod
 from collections import defaultdict
 from dataclasses import dataclass, field
-from typing import Any, Dict, List, Optional, Tuple, Type
+from typing import Any, Dict, List, Optional, Tuple, Type, Union
 
 import torch
 from torch import nn
 from torch.nn import Parameter
 
 from nerfstudio.cameras.rays import RayBundle
 from nerfstudio.configs.base_config import InstantiateConfig
@@ -46,14 +46,16 @@
     """Whether to create a scene collider to filter rays."""
     collider_params: Optional[Dict[str, float]] = to_immutable_dict({"near_plane": 2.0, "far_plane": 6.0})
     """parameters to instantiate scene collider with"""
     loss_coefficients: Dict[str, float] = to_immutable_dict({"rgb_loss_coarse": 1.0, "rgb_loss_fine": 1.0})
     """parameters to instantiate density field with"""
     eval_num_rays_per_chunk: int = 4096
     """specifies number of rays per chunk during eval"""
+    prompt: Optional[str] = None
+    """A prompt to be used in text to NeRF models"""
 
 
 class Model(nn.Module):
     """Model class
     Where everything (Fields, Optimizers, Samplers, Visualization, etc) is linked together. This should be
     subclassed for custom NeRF model.
 
@@ -111,26 +113,26 @@
         """Obtain the parameter groups for the optimizers
 
         Returns:
             Mapping of different parameter groups
         """
 
     @abstractmethod
-    def get_outputs(self, ray_bundle: RayBundle) -> Dict[str, torch.Tensor]:
+    def get_outputs(self, ray_bundle: RayBundle) -> Dict[str, Union[torch.Tensor, List]]:
         """Takes in a Ray Bundle and returns a dictionary of outputs.
 
         Args:
             ray_bundle: Input bundle of rays. This raybundle should have all the
             needed information to compute the outputs.
 
         Returns:
             Outputs of model. (ie. rendered colors)
         """
 
-    def forward(self, ray_bundle: RayBundle) -> Dict[str, torch.Tensor]:
+    def forward(self, ray_bundle: RayBundle) -> Dict[str, Union[torch.Tensor, List]]:
         """Run forward starting with a ray bundle. This outputs different things depending on the configuration
         of the model and whether or not the batch is provided (whether or not we are training basically)
 
         Args:
             ray_bundle: containing all the information needed to render that ray latents included
         """
```

### Comparing `nerfstudio-0.3.1/nerfstudio/models/base_surface_model.py` & `nerfstudio-0.3.2/nerfstudio/models/base_surface_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 from torchmetrics.functional import structural_similarity_index_measure
 from torchmetrics.image.lpip import LearnedPerceptualImagePatchSimilarity
 
 from nerfstudio.cameras.rays import RayBundle
 from nerfstudio.field_components.encodings import NeRFEncoding
 from nerfstudio.field_components.field_heads import FieldHeadNames
 from nerfstudio.field_components.spatial_distortions import SceneContraction
-from nerfstudio.fields.nerfacto_field import TCNNNerfactoField
+from nerfstudio.fields.nerfacto_field import NerfactoField
 from nerfstudio.fields.sdf_field import SDFFieldConfig
 from nerfstudio.fields.vanilla_nerf_field import NeRFField
 from nerfstudio.model_components.losses import (
     L1Loss,
     MSELoss,
     ScaleAndShiftInvariantLoss,
     monosdf_normal_loss,
@@ -80,17 +80,17 @@
     mono_depth_loss_mult: float = 0.0
     """Monocular depth consistency loss multiplier."""
     sdf_field: SDFFieldConfig = SDFFieldConfig()
     """Config for SDF Field"""
     background_model: Literal["grid", "mlp", "none"] = "mlp"
     """background models"""
     num_samples_outside: int = 32
-    """Number of samples outside the bounding sphere for backgound"""
+    """Number of samples outside the bounding sphere for background"""
     periodic_tvl_mult: float = 0.0
-    """Total variational loss mutliplier"""
+    """Total variational loss multiplier"""
     overwrite_near_far_plane: bool = False
     """whether to use near and far collider from command line"""
 
 
 class SurfaceModel(Model):
     """Base surface model
 
@@ -120,15 +120,15 @@
 
         # command line near and far has highest priority
         if self.config.overwrite_near_far_plane:
             self.collider = NearFarCollider(near_plane=self.config.near_plane, far_plane=self.config.far_plane)
 
         # background model
         if self.config.background_model == "grid":
-            self.field_background = TCNNNerfactoField(
+            self.field_background = NerfactoField(
                 self.scene_box.aabb,
                 spatial_distortion=self.scene_contraction,
                 num_images=self.num_train_data,
                 use_average_appearance_embedding=self.config.use_average_appearance_embedding,
             )
         elif self.config.background_model == "mlp":
             position_encoding = NeRFEncoding(
@@ -239,15 +239,15 @@
             field_outputs_bg = self.field_background(ray_samples_bg)
             weights_bg = ray_samples_bg.get_weights(field_outputs_bg[FieldHeadNames.DENSITY])
 
             rgb_bg = self.renderer_rgb(rgb=field_outputs_bg[FieldHeadNames.RGB], weights=weights_bg)
             depth_bg = self.renderer_depth(weights=weights_bg, ray_samples=ray_samples_bg)
             accumulation_bg = self.renderer_accumulation(weights=weights_bg)
 
-            # merge background color to forgound color
+            # merge background color to foregound color
             rgb = rgb + bg_transmittance * rgb_bg
 
             bg_outputs = {
                 "bg_rgb": rgb_bg,
                 "bg_accumulation": accumulation_bg,
                 "bg_depth": depth_bg,
                 "bg_weights": weights_bg,
```

### Comparing `nerfstudio-0.3.1/nerfstudio/models/depth_nerfacto.py` & `nerfstudio-0.3.2/nerfstudio/models/depth_nerfacto.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,15 +103,15 @@
         return loss_dict
 
     def get_image_metrics_and_images(
         self, outputs: Dict[str, torch.Tensor], batch: Dict[str, torch.Tensor]
     ) -> Tuple[Dict[str, float], Dict[str, torch.Tensor]]:
         """Appends ground truth depth to the depth image."""
         metrics, images = super().get_image_metrics_and_images(outputs, batch)
-        ground_truth_depth = batch["depth_image"]
+        ground_truth_depth = batch["depth_image"].to(self.device)
         if not self.config.is_euclidean_depth:
             ground_truth_depth = ground_truth_depth * outputs["directions_norm"]
 
         ground_truth_depth_colormap = colormaps.apply_depth_colormap(ground_truth_depth)
         predicted_depth_colormap = colormaps.apply_depth_colormap(
             outputs["depth"],
             accumulation=outputs["accumulation"],
```

### Comparing `nerfstudio-0.3.1/nerfstudio/models/instant_ngp.py` & `nerfstudio-0.3.2/nerfstudio/models/instant_ngp.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 from nerfstudio.engine.callbacks import (
     TrainingCallback,
     TrainingCallbackAttributes,
     TrainingCallbackLocation,
 )
 from nerfstudio.field_components.field_heads import FieldHeadNames
 from nerfstudio.field_components.spatial_distortions import SceneContraction
-from nerfstudio.fields.nerfacto_field import TCNNNerfactoField
+from nerfstudio.fields.nerfacto_field import NerfactoField
 from nerfstudio.model_components.losses import MSELoss
 from nerfstudio.model_components.ray_samplers import VolumetricSampler
 from nerfstudio.model_components.renderers import (
     AccumulationRenderer,
     DepthRenderer,
     RGBRenderer,
 )
@@ -90,29 +90,29 @@
     """Instant NGP model
 
     Args:
         config: instant NGP configuration to instantiate model
     """
 
     config: InstantNGPModelConfig
-    field: TCNNNerfactoField
+    field: NerfactoField
 
     def __init__(self, config: InstantNGPModelConfig, **kwargs) -> None:
         super().__init__(config=config, **kwargs)
 
     def populate_modules(self):
         """Set the fields and modules."""
         super().populate_modules()
 
         if self.config.disable_scene_contraction:
             scene_contraction = None
         else:
             scene_contraction = SceneContraction(order=float("inf"))
 
-        self.field = TCNNNerfactoField(
+        self.field = NerfactoField(
             aabb=self.scene_box.aabb,
             num_images=self.num_train_data,
             log2_hashmap_size=self.config.log2_hashmap_size,
             max_res=self.config.max_res,
             spatial_distortion=scene_contraction,
         )
```

### Comparing `nerfstudio-0.3.1/nerfstudio/models/mipnerf.py` & `nerfstudio-0.3.2/nerfstudio/models/mipnerf.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/models/nerfacto.py` & `nerfstudio-0.3.2/nerfstudio/models/tensorf.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,377 +9,355 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
-NeRF implementation that combines many recent advancements.
+TensorRF implementation.
 """
 
 from __future__ import annotations
 
 from dataclasses import dataclass, field
-from typing import Dict, List, Literal, Tuple, Type
+from typing import Dict, List, Literal, Tuple, Type, cast
 
 import numpy as np
 import torch
 from torch.nn import Parameter
 from torchmetrics import PeakSignalNoiseRatio
 from torchmetrics.functional import structural_similarity_index_measure
 from torchmetrics.image.lpip import LearnedPerceptualImagePatchSimilarity
 
-from nerfstudio.cameras.rays import RayBundle, RaySamples
+from nerfstudio.cameras.rays import RayBundle
+from nerfstudio.configs.config_utils import to_immutable_dict
 from nerfstudio.engine.callbacks import (
     TrainingCallback,
     TrainingCallbackAttributes,
     TrainingCallbackLocation,
 )
-from nerfstudio.field_components.field_heads import FieldHeadNames
-from nerfstudio.field_components.spatial_distortions import SceneContraction
-from nerfstudio.fields.density_fields import HashMLPDensityField
-from nerfstudio.fields.nerfacto_field import TCNNNerfactoField
-from nerfstudio.model_components.losses import (
-    MSELoss,
-    distortion_loss,
-    interlevel_loss,
-    orientation_loss,
-    pred_normal_loss,
-    scale_gradients_by_distance_squared,
-)
-from nerfstudio.model_components.ray_samplers import (
-    ProposalNetworkSampler,
-    UniformSampler,
+from nerfstudio.field_components.encodings import (
+    NeRFEncoding,
+    TensorCPEncoding,
+    TensorVMEncoding,
+    TriplaneEncoding,
 )
+from nerfstudio.field_components.field_heads import FieldHeadNames
+from nerfstudio.fields.tensorf_field import TensoRFField
+from nerfstudio.model_components.losses import MSELoss, tv_loss
+from nerfstudio.model_components.ray_samplers import PDFSampler, UniformSampler
 from nerfstudio.model_components.renderers import (
     AccumulationRenderer,
     DepthRenderer,
-    NormalsRenderer,
     RGBRenderer,
 )
-from nerfstudio.model_components.scene_colliders import NearFarCollider
-from nerfstudio.model_components.shaders import NormalsShader
+from nerfstudio.model_components.scene_colliders import AABBBoxCollider
 from nerfstudio.models.base_model import Model, ModelConfig
-from nerfstudio.utils import colormaps
+from nerfstudio.utils import colormaps, colors, misc
 
 
 @dataclass
-class NerfactoModelConfig(ModelConfig):
-    """Nerfacto Model Config"""
+class TensoRFModelConfig(ModelConfig):
+    """TensoRF model config"""
 
-    _target: Type = field(default_factory=lambda: NerfactoModel)
-    near_plane: float = 0.05
-    """How far along the ray to start sampling."""
-    far_plane: float = 1000.0
-    """How far along the ray to stop sampling."""
-    background_color: Literal["random", "last_sample", "black", "white"] = "last_sample"
-    """Whether to randomize the background color."""
-    hidden_dim: int = 64
-    """Dimension of hidden layers"""
-    hidden_dim_color: int = 64
-    """Dimension of hidden layers for color network"""
-    hidden_dim_transient: int = 64
-    """Dimension of hidden layers for transient network"""
-    num_levels: int = 16
-    """Number of levels of the hashmap for the base mlp."""
-    max_res: int = 2048
-    """Maximum resolution of the hashmap for the base mlp."""
-    log2_hashmap_size: int = 19
-    """Size of the hashmap for the base mlp"""
-    num_proposal_samples_per_ray: Tuple[int, ...] = (256, 96)
-    """Number of samples per ray for each proposal network."""
-    num_nerf_samples_per_ray: int = 48
-    """Number of samples per ray for the nerf network."""
-    proposal_update_every: int = 5
-    """Sample every n steps after the warmup"""
-    proposal_warmup: int = 5000
-    """Scales n from 1 to proposal_update_every over this many steps"""
-    num_proposal_iterations: int = 2
-    """Number of proposal network iterations."""
-    use_same_proposal_network: bool = False
-    """Use the same proposal network. Otherwise use different ones."""
-    proposal_net_args_list: List[Dict] = field(
-        default_factory=lambda: [
-            {"hidden_dim": 16, "log2_hashmap_size": 17, "num_levels": 5, "max_res": 128, "use_linear": False},
-            {"hidden_dim": 16, "log2_hashmap_size": 17, "num_levels": 5, "max_res": 256, "use_linear": False},
-        ]
+    _target: Type = field(default_factory=lambda: TensoRFModel)
+    """target class to instantiate"""
+    init_resolution: int = 128
+    """initial render resolution"""
+    final_resolution: int = 300
+    """final render resolution"""
+    upsampling_iters: Tuple[int, ...] = (2000, 3000, 4000, 5500, 7000)
+    """specifies a list of iteration step numbers to perform upsampling"""
+    loss_coefficients: Dict[str, float] = to_immutable_dict(
+        {
+            "rgb_loss": 1.0,
+            "tv_reg_density": 1e-3,
+            "tv_reg_color": 1e-4,
+            "l1_reg": 5e-4,
+        }
     )
-    """Arguments for the proposal density fields."""
-    proposal_initial_sampler: Literal["piecewise", "uniform"] = "piecewise"
-    """Initial sampler for the proposal network. Piecewise is preferred for unbounded scenes."""
-    interlevel_loss_mult: float = 1.0
-    """Proposal loss multiplier."""
-    distortion_loss_mult: float = 0.002
-    """Distortion loss multiplier."""
-    orientation_loss_mult: float = 0.0001
-    """Orientation loss multiplier on computed normals."""
-    pred_normal_loss_mult: float = 0.001
-    """Predicted normal loss multiplier."""
-    use_proposal_weight_anneal: bool = True
-    """Whether to use proposal weight annealing."""
-    use_average_appearance_embedding: bool = True
-    """Whether to use average appearance embedding or zeros for inference."""
-    proposal_weights_anneal_slope: float = 10.0
-    """Slope of the annealing function for the proposal weights."""
-    proposal_weights_anneal_max_num_iters: int = 1000
-    """Max num iterations for the annealing function."""
-    use_single_jitter: bool = True
-    """Whether use single jitter or not for the proposal networks."""
-    predict_normals: bool = False
-    """Whether to predict normals or not."""
-    disable_scene_contraction: bool = False
-    """Whether to disable scene contraction or not."""
-    use_gradient_scaling: bool = False
-    """Use gradient scaler where the gradients are lower for points closer to the camera."""
+    """Loss specific weights."""
+    num_samples: int = 50
+    """Number of samples in field evaluation"""
+    num_uniform_samples: int = 200
+    """Number of samples in density evaluation"""
+    num_den_components: int = 16
+    """Number of components in density encoding"""
+    num_color_components: int = 48
+    """Number of components in color encoding"""
+    appearance_dim: int = 27
+    """Number of channels for color encoding"""
+    tensorf_encoding: Literal["triplane", "vm", "cp"] = "vm"
+    regularization: Literal["none", "l1", "tv"] = "l1"
+    """Regularization method used in tensorf paper"""
 
 
-class NerfactoModel(Model):
-    """Nerfacto model
+class TensoRFModel(Model):
+    """TensoRF Model
 
     Args:
-        config: Nerfacto configuration to instantiate model
+        config: TensoRF configuration to instantiate model
     """
 
-    config: NerfactoModelConfig
-
-    def populate_modules(self):
-        """Set the fields and modules."""
-        super().populate_modules()
-
-        if self.config.disable_scene_contraction:
-            scene_contraction = None
-        else:
-            scene_contraction = SceneContraction(order=float("inf"))
+    config: TensoRFModelConfig
 
-        # Fields
-        self.field = TCNNNerfactoField(
-            self.scene_box.aabb,
-            hidden_dim=self.config.hidden_dim,
-            num_levels=self.config.num_levels,
-            max_res=self.config.max_res,
-            log2_hashmap_size=self.config.log2_hashmap_size,
-            hidden_dim_color=self.config.hidden_dim_color,
-            hidden_dim_transient=self.config.hidden_dim_transient,
-            spatial_distortion=scene_contraction,
-            num_images=self.num_train_data,
-            use_pred_normals=self.config.predict_normals,
-            use_average_appearance_embedding=self.config.use_average_appearance_embedding,
+    def __init__(
+        self,
+        config: TensoRFModelConfig,
+        **kwargs,
+    ) -> None:
+        self.init_resolution = config.init_resolution
+        self.upsampling_iters = config.upsampling_iters
+        self.num_den_components = config.num_den_components
+        self.num_color_components = config.num_color_components
+        self.appearance_dim = config.appearance_dim
+        self.upsampling_steps = (
+            np.round(
+                np.exp(
+                    np.linspace(
+                        np.log(config.init_resolution),
+                        np.log(config.final_resolution),
+                        len(config.upsampling_iters) + 1,
+                    )
+                )
+            )
+            .astype("int")
+            .tolist()[1:]
         )
+        super().__init__(config=config, **kwargs)
 
-        self.density_fns = []
-        num_prop_nets = self.config.num_proposal_iterations
-        # Build the proposal network(s)
-        self.proposal_networks = torch.nn.ModuleList()
-        if self.config.use_same_proposal_network:
-            assert len(self.config.proposal_net_args_list) == 1, "Only one proposal network is allowed."
-            prop_net_args = self.config.proposal_net_args_list[0]
-            network = HashMLPDensityField(self.scene_box.aabb, spatial_distortion=scene_contraction, **prop_net_args)
-            self.proposal_networks.append(network)
-            self.density_fns.extend([network.density_fn for _ in range(num_prop_nets)])
-        else:
-            for i in range(num_prop_nets):
-                prop_net_args = self.config.proposal_net_args_list[min(i, len(self.config.proposal_net_args_list) - 1)]
-                network = HashMLPDensityField(
-                    self.scene_box.aabb,
-                    spatial_distortion=scene_contraction,
-                    **prop_net_args,
+    def get_training_callbacks(
+        self, training_callback_attributes: TrainingCallbackAttributes
+    ) -> List[TrainingCallback]:
+        # the callback that we want to run every X iterations after the training iteration
+        def reinitialize_optimizer(self, training_callback_attributes: TrainingCallbackAttributes, step: int):
+            assert training_callback_attributes.optimizers is not None
+            assert training_callback_attributes.pipeline is not None
+            index = self.upsampling_iters.index(step)
+            resolution = self.upsampling_steps[index]
+
+            # upsample the position and direction grids
+            self.field.density_encoding.upsample_grid(resolution)
+            self.field.color_encoding.upsample_grid(resolution)
+
+            # reinitialize the encodings optimizer
+            optimizers_config = training_callback_attributes.optimizers.config
+            enc = training_callback_attributes.pipeline.get_param_groups()["encodings"]
+            lr_init = optimizers_config["encodings"]["optimizer"].lr
+
+            training_callback_attributes.optimizers.optimizers["encodings"] = optimizers_config["encodings"][
+                "optimizer"
+            ].setup(params=enc)
+            if optimizers_config["encodings"]["scheduler"]:
+                training_callback_attributes.optimizers.schedulers["encodings"] = (
+                    optimizers_config["encodings"]["scheduler"]
+                    .setup()
+                    .get_scheduler(
+                        optimizer=training_callback_attributes.optimizers.optimizers["encodings"], lr_init=lr_init
+                    )
                 )
-                self.proposal_networks.append(network)
-            self.density_fns.extend([network.density_fn for network in self.proposal_networks])
 
-        # Samplers
-        def update_schedule(step):
-            return np.clip(
-                np.interp(step, [0, self.config.proposal_warmup], [0, self.config.proposal_update_every]),
-                1,
-                self.config.proposal_update_every,
+        callbacks = [
+            TrainingCallback(
+                where_to_run=[TrainingCallbackLocation.AFTER_TRAIN_ITERATION],
+                iters=self.upsampling_iters,
+                func=reinitialize_optimizer,
+                args=[self, training_callback_attributes],
+            )
+        ]
+        return callbacks
+
+    def update_to_step(self, step: int) -> None:
+        if step < self.upsampling_iters[0]:
+            return
+
+        new_iters = list(self.upsampling_iters) + [step + 1]
+        new_iters.sort()
+
+        index = new_iters.index(step + 1)
+        new_grid_resolution = self.upsampling_steps[index - 1]
+
+        self.field.density_encoding.upsample_grid(new_grid_resolution)  # type: ignore
+        self.field.color_encoding.upsample_grid(new_grid_resolution)  # type: ignore
+
+    def populate_modules(self):
+        """Set the fields and modules"""
+        super().populate_modules()
+
+        # setting up fields
+        if self.config.tensorf_encoding == "vm":
+            density_encoding = TensorVMEncoding(
+                resolution=self.init_resolution,
+                num_components=self.num_den_components,
+            )
+            color_encoding = TensorVMEncoding(
+                resolution=self.init_resolution,
+                num_components=self.num_color_components,
+            )
+        elif self.config.tensorf_encoding == "cp":
+            density_encoding = TensorCPEncoding(
+                resolution=self.init_resolution,
+                num_components=self.num_den_components,
+            )
+            color_encoding = TensorCPEncoding(
+                resolution=self.init_resolution,
+                num_components=self.num_color_components,
+            )
+        elif self.config.tensorf_encoding == "triplane":
+            density_encoding = TriplaneEncoding(
+                resolution=self.init_resolution,
+                num_components=self.num_den_components,
             )
+            color_encoding = TriplaneEncoding(
+                resolution=self.init_resolution,
+                num_components=self.num_color_components,
+            )
+        else:
+            raise ValueError(f"Encoding {self.config.tensorf_encoding} not supported")
 
-        # Change proposal network initial sampler if uniform
-        initial_sampler = None  # None is for piecewise as default (see ProposalNetworkSampler)
-        if self.config.proposal_initial_sampler == "uniform":
-            initial_sampler = UniformSampler(single_jitter=self.config.use_single_jitter)
-
-        self.proposal_sampler = ProposalNetworkSampler(
-            num_nerf_samples_per_ray=self.config.num_nerf_samples_per_ray,
-            num_proposal_samples_per_ray=self.config.num_proposal_samples_per_ray,
-            num_proposal_network_iterations=self.config.num_proposal_iterations,
-            single_jitter=self.config.use_single_jitter,
-            update_sched=update_schedule,
-            initial_sampler=initial_sampler,
+        feature_encoding = NeRFEncoding(in_dim=self.appearance_dim, num_frequencies=2, min_freq_exp=0, max_freq_exp=2)
+        direction_encoding = NeRFEncoding(in_dim=3, num_frequencies=2, min_freq_exp=0, max_freq_exp=2)
+
+        self.field = TensoRFField(
+            self.scene_box.aabb,
+            feature_encoding=feature_encoding,
+            direction_encoding=direction_encoding,
+            density_encoding=density_encoding,
+            color_encoding=color_encoding,
+            appearance_dim=self.appearance_dim,
+            head_mlp_num_layers=2,
+            head_mlp_layer_width=128,
+            use_sh=False,
         )
 
-        # Collider
-        self.collider = NearFarCollider(near_plane=self.config.near_plane, far_plane=self.config.far_plane)
+        # samplers
+        self.sampler_uniform = UniformSampler(num_samples=self.config.num_uniform_samples, single_jitter=True)
+        self.sampler_pdf = PDFSampler(num_samples=self.config.num_samples, single_jitter=True, include_original=False)
 
         # renderers
-        self.renderer_rgb = RGBRenderer(background_color=self.config.background_color)
+        self.renderer_rgb = RGBRenderer(background_color=colors.WHITE)
         self.renderer_accumulation = AccumulationRenderer()
         self.renderer_depth = DepthRenderer()
-        self.renderer_normals = NormalsRenderer()
-
-        # shaders
-        self.normals_shader = NormalsShader()
 
         # losses
         self.rgb_loss = MSELoss()
 
         # metrics
         self.psnr = PeakSignalNoiseRatio(data_range=1.0)
         self.ssim = structural_similarity_index_measure
         self.lpips = LearnedPerceptualImagePatchSimilarity(normalize=True)
 
+        # colliders
+        if self.config.enable_collider:
+            self.collider = AABBBoxCollider(scene_box=self.scene_box)
+
+        # regularizations
+        if self.config.tensorf_encoding == "cp" and self.config.regularization == "tv":
+            raise RuntimeError("TV reg not supported for CP decomposition")
+
     def get_param_groups(self) -> Dict[str, List[Parameter]]:
         param_groups = {}
-        param_groups["proposal_networks"] = list(self.proposal_networks.parameters())
-        param_groups["fields"] = list(self.field.parameters())
-        return param_groups
 
-    def get_training_callbacks(
-        self, training_callback_attributes: TrainingCallbackAttributes
-    ) -> List[TrainingCallback]:
-        callbacks = []
-        if self.config.use_proposal_weight_anneal:
-            # anneal the weights of the proposal network before doing PDF sampling
-            N = self.config.proposal_weights_anneal_max_num_iters
-
-            def set_anneal(step):
-                # https://arxiv.org/pdf/2111.12077.pdf eq. 18
-                train_frac = np.clip(step / N, 0, 1)
-
-                def bias(x, b):
-                    return b * x / ((b - 1) * x + 1)
-
-                anneal = bias(train_frac, self.config.proposal_weights_anneal_slope)
-                self.proposal_sampler.set_anneal(anneal)
-
-            callbacks.append(
-                TrainingCallback(
-                    where_to_run=[TrainingCallbackLocation.BEFORE_TRAIN_ITERATION],
-                    update_every_num_iters=1,
-                    func=set_anneal,
-                )
-            )
-            callbacks.append(
-                TrainingCallback(
-                    where_to_run=[TrainingCallbackLocation.AFTER_TRAIN_ITERATION],
-                    update_every_num_iters=1,
-                    func=self.proposal_sampler.step_cb,
-                )
-            )
-        return callbacks
+        param_groups["fields"] = (
+            list(self.field.mlp_head.parameters())
+            + list(self.field.B.parameters())
+            + list(self.field.field_output_rgb.parameters())
+        )
+        param_groups["encodings"] = list(self.field.color_encoding.parameters()) + list(
+            self.field.density_encoding.parameters()
+        )
+
+        return param_groups
 
     def get_outputs(self, ray_bundle: RayBundle):
-        ray_samples: RaySamples
-        ray_samples, weights_list, ray_samples_list = self.proposal_sampler(ray_bundle, density_fns=self.density_fns)
-        field_outputs = self.field.forward(ray_samples, compute_normals=self.config.predict_normals)
-        if self.config.use_gradient_scaling:
-            field_outputs = scale_gradients_by_distance_squared(field_outputs, ray_samples)
-
-        weights = ray_samples.get_weights(field_outputs[FieldHeadNames.DENSITY])
-        weights_list.append(weights)
-        ray_samples_list.append(ray_samples)
-
-        rgb = self.renderer_rgb(rgb=field_outputs[FieldHeadNames.RGB], weights=weights)
-        depth = self.renderer_depth(weights=weights, ray_samples=ray_samples)
-        accumulation = self.renderer_accumulation(weights=weights)
-
-        outputs = {
-            "rgb": rgb,
-            "accumulation": accumulation,
-            "depth": depth,
-        }
+        # uniform sampling
+        ray_samples_uniform = self.sampler_uniform(ray_bundle)
+        dens = self.field.get_density(ray_samples_uniform)
+        weights = ray_samples_uniform.get_weights(dens)
+        coarse_accumulation = self.renderer_accumulation(weights)
+        acc_mask = torch.where(coarse_accumulation < 0.0001, False, True).reshape(-1)
+
+        # pdf sampling
+        ray_samples_pdf = self.sampler_pdf(ray_bundle, ray_samples_uniform, weights)
+
+        # fine field:
+        field_outputs_fine = self.field.forward(
+            ray_samples_pdf, mask=acc_mask, bg_color=colors.WHITE.to(weights.device)
+        )
 
-        if self.config.predict_normals:
-            normals = self.renderer_normals(normals=field_outputs[FieldHeadNames.NORMALS], weights=weights)
-            pred_normals = self.renderer_normals(field_outputs[FieldHeadNames.PRED_NORMALS], weights=weights)
-            outputs["normals"] = self.normals_shader(normals)
-            outputs["pred_normals"] = self.normals_shader(pred_normals)
-        # These use a lot of GPU memory, so we avoid storing them for eval.
-        if self.training:
-            outputs["weights_list"] = weights_list
-            outputs["ray_samples_list"] = ray_samples_list
-
-        if self.training and self.config.predict_normals:
-            outputs["rendered_orientation_loss"] = orientation_loss(
-                weights.detach(), field_outputs[FieldHeadNames.NORMALS], ray_bundle.directions
-            )
+        weights_fine = ray_samples_pdf.get_weights(field_outputs_fine[FieldHeadNames.DENSITY])
 
-            outputs["rendered_pred_normal_loss"] = pred_normal_loss(
-                weights.detach(),
-                field_outputs[FieldHeadNames.NORMALS].detach(),
-                field_outputs[FieldHeadNames.PRED_NORMALS],
-            )
+        accumulation = self.renderer_accumulation(weights_fine)
+        depth = self.renderer_depth(weights_fine, ray_samples_pdf)
+
+        rgb = self.renderer_rgb(
+            rgb=field_outputs_fine[FieldHeadNames.RGB],
+            weights=weights_fine,
+        )
 
-        for i in range(self.config.num_proposal_iterations):
-            outputs[f"prop_depth_{i}"] = self.renderer_depth(weights=weights_list[i], ray_samples=ray_samples_list[i])
+        rgb = torch.where(accumulation < 0, colors.WHITE.to(rgb.device), rgb)
+        accumulation = torch.clamp(accumulation, min=0)
 
+        outputs = {"rgb": rgb, "accumulation": accumulation, "depth": depth}
         return outputs
 
-    def get_metrics_dict(self, outputs, batch):
-        metrics_dict = {}
-        image = batch["image"].to(self.device)
-        metrics_dict["psnr"] = self.psnr(outputs["rgb"], image)
-        if self.training:
-            metrics_dict["distortion"] = distortion_loss(outputs["weights_list"], outputs["ray_samples_list"])
-        return metrics_dict
-
-    def get_loss_dict(self, outputs, batch, metrics_dict=None):
-        loss_dict = {}
-        image = batch["image"].to(self.device)
-        loss_dict["rgb_loss"] = self.rgb_loss(image, outputs["rgb"])
-        if self.training:
-            loss_dict["interlevel_loss"] = self.config.interlevel_loss_mult * interlevel_loss(
-                outputs["weights_list"], outputs["ray_samples_list"]
-            )
-            assert metrics_dict is not None and "distortion" in metrics_dict
-            loss_dict["distortion_loss"] = self.config.distortion_loss_mult * metrics_dict["distortion"]
-            if self.config.predict_normals:
-                # orientation loss for computed normals
-                loss_dict["orientation_loss"] = self.config.orientation_loss_mult * torch.mean(
-                    outputs["rendered_orientation_loss"]
-                )
+    def get_loss_dict(self, outputs, batch, metrics_dict=None) -> Dict[str, torch.Tensor]:
+        # Scaling metrics by coefficients to create the losses.
+        device = outputs["rgb"].device
+        image = batch["image"].to(device)
+
+        rgb_loss = self.rgb_loss(image, outputs["rgb"])
+
+        loss_dict = {"rgb_loss": rgb_loss}
+
+        if self.config.regularization == "l1":
+            l1_parameters = []
+            for parameter in self.field.density_encoding.parameters():
+                l1_parameters.append(parameter.view(-1))
+            loss_dict["l1_reg"] = torch.abs(torch.cat(l1_parameters)).mean()
+        elif self.config.regularization == "tv":
+            density_plane_coef = self.field.density_encoding.plane_coef
+            color_plane_coef = self.field.color_encoding.plane_coef
+            assert isinstance(color_plane_coef, torch.Tensor) and isinstance(
+                density_plane_coef, torch.Tensor
+            ), "TV reg only supported for TensoRF encoding types with plane_coef attribute"
+            loss_dict["tv_reg_density"] = tv_loss(density_plane_coef)
+            loss_dict["tv_reg_color"] = tv_loss(color_plane_coef)
+        elif self.config.regularization == "none":
+            pass
+        else:
+            raise ValueError(f"Regularization {self.config.regularization} not supported")
 
-                # ground truth supervision for normals
-                loss_dict["pred_normal_loss"] = self.config.pred_normal_loss_mult * torch.mean(
-                    outputs["rendered_pred_normal_loss"]
-                )
+        loss_dict = misc.scale_dict(loss_dict, self.config.loss_coefficients)
         return loss_dict
 
     def get_image_metrics_and_images(
         self, outputs: Dict[str, torch.Tensor], batch: Dict[str, torch.Tensor]
     ) -> Tuple[Dict[str, float], Dict[str, torch.Tensor]]:
-        image = batch["image"].to(self.device)
+        image = batch["image"].to(outputs["rgb"].device)
         rgb = outputs["rgb"]
         acc = colormaps.apply_colormap(outputs["accumulation"])
+        assert self.config.collider_params is not None
         depth = colormaps.apply_depth_colormap(
             outputs["depth"],
             accumulation=outputs["accumulation"],
+            near_plane=self.config.collider_params["near_plane"],
+            far_plane=self.config.collider_params["far_plane"],
         )
 
         combined_rgb = torch.cat([image, rgb], dim=1)
-        combined_acc = torch.cat([acc], dim=1)
-        combined_depth = torch.cat([depth], dim=1)
 
         # Switch images from [H, W, C] to [1, C, H, W] for metrics computations
         image = torch.moveaxis(image, -1, 0)[None, ...]
         rgb = torch.moveaxis(rgb, -1, 0)[None, ...]
 
         psnr = self.psnr(image, rgb)
-        ssim = self.ssim(image, rgb)
+        ssim = cast(torch.Tensor, self.ssim(image, rgb))
         lpips = self.lpips(image, rgb)
 
-        # all of these metrics will be logged as scalars
-        metrics_dict = {"psnr": float(psnr.item()), "ssim": float(ssim)}  # type: ignore
-        metrics_dict["lpips"] = float(lpips)
-
-        images_dict = {"img": combined_rgb, "accumulation": combined_acc, "depth": combined_depth}
-
-        for i in range(self.config.num_proposal_iterations):
-            key = f"prop_depth_{i}"
-            prop_depth_i = colormaps.apply_depth_colormap(
-                outputs[key],
-                accumulation=outputs["accumulation"],
-            )
-            images_dict[key] = prop_depth_i
-
+        metrics_dict = {
+            "psnr": float(psnr.item()),
+            "ssim": float(ssim.item()),
+            "lpips": float(lpips.item()),
+        }
+        images_dict = {"img": combined_rgb, "accumulation": acc, "depth": depth}
         return metrics_dict, images_dict
```

### Comparing `nerfstudio-0.3.1/nerfstudio/models/nerfplayer_nerfacto.py` & `nerfstudio-0.3.2/nerfstudio/data/datamanagers/random_cameras_datamanager.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,265 +1,315 @@
-# Copyright 2022 the Regents of the University of California, Nerfstudio Team and contributors. All rights reserved.
+# Copyright 2022 The Nerfstudio Team. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
-NeRFPlayer (https://arxiv.org/abs/2210.15947) implementation with nerfacto backbone.
+Data manager without input images, only random camera poses
 """
 
 from __future__ import annotations
 
-import functools
+import sys
 from dataclasses import dataclass, field
-from typing import Dict, List, Literal, Sequence, Type, cast
+from typing import Dict, List, Tuple, Type, Union
 
-import numpy as np
 import torch
-from torchmetrics import PeakSignalNoiseRatio
-from torchmetrics.functional import structural_similarity_index_measure
-from torchmetrics.image.lpip import LearnedPerceptualImagePatchSimilarity
+from rich.progress import Console
+from torch.nn import Parameter
+from torch import Tensor
+from typing_extensions import Literal
 
+from nerfstudio.cameras.cameras import Cameras
 from nerfstudio.cameras.rays import RayBundle
-from nerfstudio.field_components.field_heads import FieldHeadNames
-from nerfstudio.field_components.spatial_distortions import SceneContraction
-from nerfstudio.fields.nerfplayer_nerfacto_field import (
-    NerfplayerNerfactoField,
-    TemporalHashMLPDensityField,
-)
-from nerfstudio.model_components.losses import (
-    MSELoss,
-    interlevel_loss,
-    orientation_loss,
-    pred_normal_loss,
-)
-from nerfstudio.model_components.ray_samplers import ProposalNetworkSampler
-from nerfstudio.model_components.renderers import (
-    AccumulationRenderer,
-    DepthRenderer,
-    NormalsRenderer,
-    RGBRenderer,
-)
-from nerfstudio.model_components.scene_colliders import NearFarCollider
-from nerfstudio.model_components.shaders import NormalsShader
-from nerfstudio.models.base_model import Model
-from nerfstudio.models.nerfacto import NerfactoModel, NerfactoModelConfig
+from nerfstudio.configs.config_utils import to_immutable_dict
+from nerfstudio.data.datamanagers.base_datamanager import DataManager, DataManagerConfig
+from nerfstudio.data.datasets.base_dataset import InputDataset
+from nerfstudio.data.scene_box import SceneBox
+from nerfstudio.data.utils.dataloaders import RandIndicesEvalDataloader
+
+CONSOLE = Console(width=120)
+
+
+class TrivialDataset(InputDataset):
+    """A trivial dataset with blank images for the viewer"""
+
+    # pylint: disable=super-init-not-called
+    def __init__(self, cameras: Cameras):
+        self.size = cameras.size
+        self.cameras = cameras
+        self.alpha_color = None
+        self.scene_box = SceneBox(torch.Tensor([[-1, -1, -1], [1, 1, 1]]))
+        self.mask_filenames = None
+        self.metadata = to_immutable_dict({})
+
+    def __len__(self):
+        return self.size
+
+    def __getitem__(self, index: int) -> Dict:
+        return {
+            "image": torch.cat([torch.ones(128, 256, 3), torch.zeros(128, 256, 3)], dim=0),
+            "image_idx": index,
+        }
 
 
-@dataclass
-class NerfplayerNerfactoModelConfig(NerfactoModelConfig):
-    """Nerfplayer Model Config with Nerfacto backbone"""
+def random_train_pose(
+    size: int,
+    resolution: int,
+    device: Union[torch.device, str],
+    radius_mean: float = 1.0,
+    radius_std: float = 0.1,
+    central_rotation_range: Tuple[float, float] = (0, 360),
+    vertical_rotation_range: Tuple[float, float] = (-90, 0),
+    focal_range: Tuple[float, float] = (0.75, 1.35),
+    jitter_std: float = 0.01,
+    center: Tuple[float, float, float] = (0, 0, 0),
+) -> Tuple[Cameras, Tensor, Tensor]:
+    """generate random poses from an orbit camera
+    Args:
+        size: batch size of generated poses.
+        device: where to allocate the output.
+        radius_mean: mean radius of the orbit camera.
+        radius_std: standard deviation of the radius of the orbit camera.
+        central_rotation_range: amount that we rotate around the center of the object
+        vertical_rotation_range: amount that we allow the cameras to pan up and down from horizontal
+        focal_range: focal length range
+        jitter_std: standard deviation of the jitter added to the camera position
+        center: center of the object
+    Return:
+        poses: [size, 4, 4]
+    """
+
+    vertical_rotation_range = (
+        vertical_rotation_range[0] + 90,
+        vertical_rotation_range[1] + 90,
+    )
+    # This is the uniform sample on the part of the sphere we care about where 0 = 0 degrees and 1 = 360 degrees
+    sampled_uniform = (
+        torch.rand(size) * (vertical_rotation_range[1] - vertical_rotation_range[0]) + vertical_rotation_range[0]
+    ) / 180
+    vertical_rotation = torch.arccos(1 - 2 * sampled_uniform)
+    central_rotation = torch.deg2rad(
+        torch.rand(size) * (central_rotation_range[1] - central_rotation_range[0]) + central_rotation_range[0]
+    )
+
+    c_cos = torch.cos(central_rotation)
+    c_sin = torch.sin(central_rotation)
+    v_cos = torch.cos(vertical_rotation)
+    v_sin = torch.sin(vertical_rotation)
+    zeros = torch.zeros_like(central_rotation)
+    ones = torch.ones_like(central_rotation)
+
+    rot_z = torch.stack(
+        [
+            torch.stack([c_cos, -c_sin, zeros], dim=-1),
+            torch.stack([c_sin, c_cos, zeros], dim=-1),
+            torch.stack([zeros, zeros, ones], dim=-1),
+        ],
+        dim=-2,
+    )
+
+    rot_x = torch.stack(
+        [
+            torch.stack([ones, zeros, zeros], dim=-1),
+            torch.stack([zeros, v_cos, -v_sin], dim=-1),
+            torch.stack([zeros, v_sin, v_cos], dim=-1),
+        ],
+        dim=-2,
+    )
 
-    _target: Type = field(default_factory=lambda: NerfplayerNerfactoModel)
-    near_plane: float = 0.05
-    """How far along the ray to start sampling."""
-    far_plane: float = 1000.0
-    """How far along the ray to stop sampling."""
-    background_color: Literal["random", "last_sample", "black", "white"] = "random"
-    """Whether to randomize the background color. (Random is reported to be better on DyCheck.)"""
-    num_levels: int = 16
-    """Hashing grid parameter."""
-    features_per_level: int = 2
-    """Hashing grid parameter."""
-    log2_hashmap_size: int = 18
-    """Hashing grid parameter."""
-    temporal_dim: int = 32
-    """Hashing grid parameter. A higher temporal dim means a higher temporal frequency."""
-    proposal_net_args_list: List[Dict] = field(
-        default_factory=lambda: [
-            {"hidden_dim": 16, "temporal_dim": 32, "log2_hashmap_size": 17, "num_levels": 5, "max_res": 64},
-            {"hidden_dim": 16, "temporal_dim": 32, "log2_hashmap_size": 17, "num_levels": 5, "max_res": 256},
-        ]
+    # Default directions are facing in the -z direction, so origins should face opposite way
+    origins = torch.stack([torch.tensor([0, 0, 1])] * size, dim=0)
+    origins = (origins * radius_mean) + (origins * (torch.randn((origins.shape)) * radius_std))
+    R = torch.bmm(rot_z, rot_x)  # Want to have Rx @ Ry @ origin
+    t = (
+        torch.bmm(R, origins.unsqueeze(-1))
+        + torch.randn((size, 3, 1)) * jitter_std
+        + torch.tensor(center)[None, :, None]
     )
-    """Arguments for the proposal density fields."""
-    distortion_loss_mult: float = 1e-2
-    """Distortion loss multiplier."""
-    temporal_tv_weight: float = 1
-    """Temporal TV balancing weight for feature channels."""
-    depth_weight: float = 1e-1
-    """depth loss balancing weight for feature channels."""
+    camera_to_worlds = torch.cat([R, t], dim=-1)
 
+    focals = torch.rand(size) * (focal_range[1] - focal_range[0]) + focal_range[0]
 
-class NerfplayerNerfactoModel(NerfactoModel):
-    """Nerfplayer model with Nerfacto backbone.
+    cameras = Cameras(
+        camera_to_worlds=camera_to_worlds,
+        fx=focals * resolution,
+        fy=focals * resolution,
+        cx=resolution / 2,
+        cy=resolution / 2,
+    ).to(device)
+
+    return cameras, torch.rad2deg(vertical_rotation), torch.rad2deg(central_rotation)
+
+
+@dataclass
+class RandomCamerasDataManagerConfig(DataManagerConfig):
+    """Configuration for data manager that does not load from a dataset. Instead, it generates random poses."""
+
+    _target: Type = field(default_factory=lambda: RandomCamerasDataManager)
+    train_resolution: int = 64
+    """Training resolution"""
+    eval_resolution: int = 64
+    """Evaluation resolution"""
+    num_eval_angles: int = 256
+    """Number of evaluation angles"""
+    train_images_per_batch: int = 1
+    """Number of images per batch for training"""
+    eval_images_per_batch: int = 1
+    """Number of images per batch for evaluation"""
+    radius_mean: float = 2.5
+    """Mean radius of camera orbit"""
+    radius_std: float = 0.1
+    """Std of radius of camera orbit"""
+    focal_range: Tuple[float, float] = (0.7, 1.35)
+    """Range of focal length"""
+    vertical_rotation_range: Tuple[float, float] = (-90, 0)
+    """Range of vertical rotation"""
+    jitter_std: float = 0.05
+    """Std of camera direction jitter, so we don't just point the cameras towards the center every time"""
+    center: Tuple[float, float, float] = (0, 0, 0)
+    """Center coordinate of the camera sphere"""
+    horizontal_rotation_warmup: int = 0
+    """How many steps until the full horizontal rotation range is used"""
+
+
+class RandomCamerasDataManager(DataManager):  # pylint: disable=abstract-method
+    """Basic stored data manager implementation.
+
+    This is pretty much a port over from our old dataloading utilities, and is a little jank
+    under the hood. We may clean this up a little bit under the hood with more standard dataloading
+    components that can be strung together, but it can be just used as a black box for now since
+    only the constructor is likely to change in the future, or maybe passing in step number to the
+    next_train and next_eval functions.
 
     Args:
-        config: Nerfplayer configuration to instantiate model
+        config: the DataManagerConfig used to instantiate class
     """
 
-    config: NerfplayerNerfactoModelConfig
+    config: RandomCamerasDataManagerConfig
 
-    def populate_modules(self):
-        """Set the fields and modules."""
-        Model.populate_modules(self)
-
-        scene_contraction = SceneContraction(order=float("inf"))
-
-        # Fields
-        self.field = NerfplayerNerfactoField(
-            self.scene_box.aabb,
-            temporal_dim=self.config.temporal_dim,
-            num_levels=self.config.num_levels,
-            features_per_level=self.config.features_per_level,
-            log2_hashmap_size=self.config.log2_hashmap_size,
-            spatial_distortion=scene_contraction,
-            num_images=self.num_train_data,
-            use_pred_normals=self.config.predict_normals,
-            use_average_appearance_embedding=self.config.use_average_appearance_embedding,
+    # pylint: disable=super-init-not-called
+    def __init__(
+        self,
+        config: RandomCamerasDataManagerConfig,
+        device: Union[torch.device, str] = "cpu",
+        test_mode: Literal["test", "val", "inference"] = "val",
+        world_size: int = 1,
+        local_rank: int = 0,
+        **kwargs,  # pylint: disable=unused-argument
+    ):
+        self.config = config
+        self.device = device
+        self.world_size = world_size
+        self.local_rank = local_rank
+        self.sampler = None
+        self.test_mode = test_mode
+        self.test_split = "test" if test_mode in ["test", "inference"] else "val"
+
+        if self.config.data is not None:
+            CONSOLE.print("[red] --data should not be used with the RandomCamerasDataManager[/red]")
+            sys.exit(1)
+
+        cameras, _, _ = random_train_pose(
+            self.config.num_eval_angles,
+            self.config.eval_resolution,
+            device=self.device,
+            radius_mean=self.config.radius_mean,
+            radius_std=self.config.radius_std,
+            focal_range=self.config.focal_range,
+            central_rotation_range=(-180, 180),
+            vertical_rotation_range=self.config.vertical_rotation_range,
+            jitter_std=self.config.jitter_std,
+            center=self.config.center,
         )
 
-        self.density_fns = []
-        num_prop_nets = self.config.num_proposal_iterations
+        self.train_dataset = TrivialDataset(cameras)
+        self.eval_dataset = TrivialDataset(cameras)
 
-        # Build the proposal network(s)
-        proposal_networks: List[TemporalHashMLPDensityField] = []
-        if self.config.use_same_proposal_network:
-            assert len(self.config.proposal_net_args_list) == 1, "Only one proposal network is allowed."
-            prop_net_args = self.config.proposal_net_args_list[0]
-            network = TemporalHashMLPDensityField(
-                self.scene_box.aabb, spatial_distortion=scene_contraction, **prop_net_args
-            )
-            proposal_networks.append(network)
-            self.density_fns.extend([network.density_fn for _ in range(num_prop_nets)])
-        else:
-            for i in range(num_prop_nets):
-                prop_net_args = self.config.proposal_net_args_list[min(i, len(self.config.proposal_net_args_list) - 1)]
-                network = TemporalHashMLPDensityField(
-                    self.scene_box.aabb,
-                    spatial_distortion=scene_contraction,
-                    **prop_net_args,
-                )
-                proposal_networks.append(network)
-            self.density_fns.extend([network.density_fn for network in proposal_networks])
-        self.proposal_networks = cast(Sequence[TemporalHashMLPDensityField], torch.nn.ModuleList(proposal_networks))
-
-        # Samplers
-        def update_schedule(step):
-            return np.clip(
-                np.interp(step, [0, self.config.proposal_warmup], [0, self.config.proposal_update_every]),
-                1,
-                self.config.proposal_update_every,
-            )
-
-        self.proposal_sampler = ProposalNetworkSampler(
-            num_nerf_samples_per_ray=self.config.num_nerf_samples_per_ray,
-            num_proposal_samples_per_ray=self.config.num_proposal_samples_per_ray,
-            num_proposal_network_iterations=self.config.num_proposal_iterations,
-            single_jitter=self.config.use_single_jitter,
-            update_sched=update_schedule,
+        self.eval_dataloader = RandIndicesEvalDataloader(
+            input_dataset=self.eval_dataset,
+            device=self.device,
+            num_workers=self.world_size * 4,
         )
 
-        # Collider
-        self.collider = NearFarCollider(near_plane=self.config.near_plane, far_plane=self.config.far_plane)
+        # pylint: disable=non-parent-init-called
+        DataManager.__init__(self)
 
-        # renderers
-        self.renderer_rgb = RGBRenderer(background_color=self.config.background_color)
-        self.renderer_accumulation = AccumulationRenderer()
-        self.renderer_depth = DepthRenderer(method="expected")  # for depth loss
-        self.renderer_normals = NormalsRenderer()
-
-        # shaders
-        self.normals_shader = NormalsShader()
-
-        # losses
-        self.rgb_loss = MSELoss()
-
-        # metrics
-        self.psnr = PeakSignalNoiseRatio(data_range=1.0)
-        self.ssim = structural_similarity_index_measure
-        self.lpips = LearnedPerceptualImagePatchSimilarity(normalize=True)
-        self.temporal_distortion = True  # for viewer
-
-    def get_outputs(self, ray_bundle: RayBundle):
-        assert ray_bundle.times is not None, "Time not provided."
-        ray_samples, weights_list, ray_samples_list = self.proposal_sampler(
-            ray_bundle, density_fns=[functools.partial(f, times=ray_bundle.times) for f in self.density_fns]
+    def next_train(self, step: int) -> Tuple[RayBundle, Dict]:
+        """Returns the next batch of data from the train dataloader."""
+
+        self.train_count += 1
+        horizontal_range = min((step / max(1, self.config.horizontal_rotation_warmup)), 1) * 180
+
+        cameras, vertical_rotation, central_rotation = random_train_pose(
+            self.config.train_images_per_batch,
+            self.config.train_resolution,
+            device=self.device,
+            radius_mean=self.config.radius_mean,
+            radius_std=self.config.radius_std,
+            focal_range=self.config.focal_range,
+            vertical_rotation_range=self.config.vertical_rotation_range,
+            jitter_std=self.config.jitter_std,
+            center=self.config.center,
+            central_rotation_range=(-horizontal_range, horizontal_range),
         )
-        field_outputs = self.field(ray_samples, compute_normals=self.config.predict_normals)
-        weights = ray_samples.get_weights(field_outputs[FieldHeadNames.DENSITY])
-        weights_list.append(weights)
-        ray_samples_list.append(ray_samples)
-
-        rgb = self.renderer_rgb(rgb=field_outputs[FieldHeadNames.RGB], weights=weights)
-        depth = self.renderer_depth(weights=weights, ray_samples=ray_samples)
-        accumulation = self.renderer_accumulation(weights=weights)
-
-        outputs = {
-            "rgb": rgb,
-            "accumulation": accumulation,
-            "depth": depth,
+        ray_bundle = cameras.generate_rays(torch.tensor(list(range(self.config.train_images_per_batch)))).flatten()
+
+        return ray_bundle, {
+            "vertical": vertical_rotation,
+            "central": central_rotation,
+            "initialization": True,
         }
 
-        if self.config.predict_normals:
-            outputs["normals"] = self.normals_shader(
-                self.renderer_normals(normals=field_outputs[FieldHeadNames.NORMALS], weights=weights)
-            )
-            outputs["pred_normals"] = self.normals_shader(
-                self.renderer_normals(field_outputs[FieldHeadNames.PRED_NORMALS], weights=weights)
-            )
-
-        # These use a lot of GPU memory, so we avoid storing them for eval.
-        if self.training:
-            outputs["weights_list"] = weights_list
-            outputs["ray_samples_list"] = ray_samples_list
-
-        if self.training and self.config.predict_normals:
-            outputs["rendered_orientation_loss"] = orientation_loss(
-                weights.detach(), field_outputs[FieldHeadNames.NORMALS], ray_bundle.directions
-            )
-
-            outputs["rendered_pred_normal_loss"] = pred_normal_loss(
-                weights.detach(),
-                field_outputs[FieldHeadNames.NORMALS].detach(),
-                field_outputs[FieldHeadNames.PRED_NORMALS],
-            )
-
-        for i in range(self.config.num_proposal_iterations):
-            outputs[f"prop_depth_{i}"] = self.renderer_depth(weights=weights_list[i], ray_samples=ray_samples_list[i])
-
-        return outputs
-
-    def get_loss_dict(self, outputs, batch, metrics_dict=None):
-        loss_dict = {}
-        image = batch["image"].to(self.device)
-        loss_dict["rgb_loss"] = self.rgb_loss(image, outputs["rgb"])
-        if self.training:
-            loss_dict["interlevel_loss"] = self.config.interlevel_loss_mult * interlevel_loss(
-                outputs["weights_list"], outputs["ray_samples_list"]
-            )
-            assert metrics_dict is not None and "distortion" in metrics_dict
-            loss_dict["distortion_loss"] = self.config.distortion_loss_mult * metrics_dict["distortion"]
-            if self.config.predict_normals:
-                # orientation loss for computed normals
-                loss_dict["orientation_loss"] = self.config.orientation_loss_mult * torch.mean(
-                    outputs["rendered_orientation_loss"]
-                )
-
-                # ground truth supervision for normals
-                loss_dict["pred_normal_loss"] = self.config.pred_normal_loss_mult * torch.mean(
-                    outputs["rendered_pred_normal_loss"]
-                )
-            if "depth_image" in batch.keys() and self.config.depth_weight > 0:
-                mask = (batch["depth_image"] != 0).view([-1])
-                loss_dict["depth_loss"] = 0
-
-                def compute_depth_loss(x):
-                    return self.config.depth_weight * (x - batch["depth_image"][mask]).pow(2).mean()
-
-                loss_dict["depth_loss"] = compute_depth_loss(outputs["depth"][mask])
-                for i in range(self.config.num_proposal_iterations):
-                    loss_dict["depth_loss"] += compute_depth_loss(outputs[f"prop_depth_{i}"][mask])
-            if self.config.temporal_tv_weight > 0:
-                loss_dict["temporal_tv_loss"] = self.field.mlp_base.get_temporal_tv_loss()
-                for net in self.proposal_networks:
-                    loss_dict["temporal_tv_loss"] += net.encoding.get_temporal_tv_loss()
-                loss_dict["temporal_tv_loss"] *= self.config.temporal_tv_weight
-        return loss_dict
+    def next_eval(self, step: int) -> Tuple[RayBundle, Dict]:
+        """Returns the next batch of data from the eval dataloader."""
+        self.eval_count += 1
+
+        cameras, vertical_rotation, central_rotation = random_train_pose(
+            self.config.eval_images_per_batch,
+            self.config.eval_resolution,
+            device=self.device,
+            radius_mean=self.config.radius_mean,
+            radius_std=self.config.radius_std,
+            focal_range=self.config.focal_range,
+            vertical_rotation_range=self.config.vertical_rotation_range,
+            jitter_std=self.config.jitter_std,
+            center=self.config.center,
+        )
+        ray_bundle = cameras.generate_rays(
+            torch.tensor([[i] for i in range(self.config.train_images_per_batch)])
+        ).flatten()
+
+        return ray_bundle, {"vertical": vertical_rotation, "central": central_rotation}
+
+    def next_eval_image(self, step: int) -> Tuple[int, RayBundle, Dict]:
+        for camera_ray_bundle, batch in self.eval_dataloader:
+            assert camera_ray_bundle.camera_indices is not None
+            image_idx = int(camera_ray_bundle.camera_indices[0, 0, 0])
+            return image_idx, camera_ray_bundle, batch
+        raise ValueError("No more eval images")
+
+    def get_train_rays_per_batch(self) -> int:
+        return self.config.train_resolution**2
+
+    def get_eval_rays_per_batch(self) -> int:
+        return self.config.eval_resolution**2
+
+    def get_param_groups(
+        self,
+    ) -> Dict[str, List[Parameter]]:  # pylint: disable=no-self-use
+        """Get the param groups for the data manager.
+        Returns:
+            A list of dictionaries containing the data manager's param groups.
+        """
+        param_groups = {}
+
+        return param_groups
```

### Comparing `nerfstudio-0.3.1/nerfstudio/models/neus.py` & `nerfstudio-0.3.2/nerfstudio/models/neus.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/models/semantic_nerfw.py` & `nerfstudio-0.3.2/nerfstudio/models/semantic_nerfw.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     TrainingCallback,
     TrainingCallbackAttributes,
     TrainingCallbackLocation,
 )
 from nerfstudio.field_components.field_heads import FieldHeadNames
 from nerfstudio.field_components.spatial_distortions import SceneContraction
 from nerfstudio.fields.density_fields import HashMLPDensityField
-from nerfstudio.fields.nerfacto_field import TCNNNerfactoField
+from nerfstudio.fields.nerfacto_field import NerfactoField
 from nerfstudio.model_components.losses import MSELoss, distortion_loss, interlevel_loss
 from nerfstudio.model_components.ray_samplers import ProposalNetworkSampler
 from nerfstudio.model_components.renderers import (
     AccumulationRenderer,
     DepthRenderer,
     RGBRenderer,
     SemanticRenderer,
@@ -86,15 +86,15 @@
 
         scene_contraction = SceneContraction(order=float("inf"))
 
         if self.config.use_transient_embedding:
             raise ValueError("Transient embedding is not fully working for semantic nerf-w.")
 
         # Fields
-        self.field = TCNNNerfactoField(
+        self.field = NerfactoField(
             self.scene_box.aabb,
             num_levels=self.config.num_levels,
             max_res=self.config.max_res,
             log2_hashmap_size=self.config.log2_hashmap_size,
             spatial_distortion=scene_contraction,
             num_images=self.num_train_data,
             use_average_appearance_embedding=self.config.use_average_appearance_embedding,
@@ -250,15 +250,15 @@
             loss_dict["density_loss"] = 0.01 * outputs["density_transient"].mean()
             loss_dict["rgb_loss"] = (((image - outputs["rgb"]) ** 2).sum(-1) / (betas[..., 0] ** 2)).mean()
         else:
             loss_dict["rgb_loss"] = self.rgb_loss(image, outputs["rgb"])
 
         # semantic loss
         loss_dict["semantics_loss"] = self.config.semantic_loss_weight * self.cross_entropy_loss(
-            outputs["semantics"], batch["semantics"][..., 0].long()
+            outputs["semantics"], batch["semantics"][..., 0].long().to(self.device)
         )
         return loss_dict
 
     def get_image_metrics_and_images(
         self, outputs: Dict[str, torch.Tensor], batch: Dict[str, torch.Tensor]
     ) -> Tuple[Dict[str, float], Dict[str, torch.Tensor]]:
         image = batch["image"].to(self.device)
@@ -297,10 +297,10 @@
             images_dict[key] = prop_depth_i
 
         # semantics
         semantic_labels = torch.argmax(torch.nn.functional.softmax(outputs["semantics"], dim=-1), dim=-1)
         images_dict["semantics_colormap"] = self.colormap.to(self.device)[semantic_labels]
 
         # valid mask
-        images_dict["mask"] = batch["mask"].repeat(1, 1, 3)
+        images_dict["mask"] = batch["mask"].repeat(1, 1, 3).to(self.device)
 
         return metrics_dict, images_dict
```

### Comparing `nerfstudio-0.3.1/nerfstudio/models/vanilla_nerf.py` & `nerfstudio-0.3.2/nerfstudio/models/vanilla_nerf.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/pipelines/__init__.py` & `nerfstudio-0.3.2/nerfstudio/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/pipelines/base_pipeline.py` & `nerfstudio-0.3.2/nerfstudio/pipelines/base_pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,20 +31,21 @@
     Progress,
     TextColumn,
     TimeElapsedColumn,
 )
 from torch import nn
 from torch.nn import Parameter
 from torch.nn.parallel import DistributedDataParallel as DDP
+from torch.cuda.amp.grad_scaler import GradScaler
 
 from nerfstudio.configs import base_config as cfg
 from nerfstudio.data.datamanagers.base_datamanager import (
     DataManager,
+    DataManagerConfig,
     VanillaDataManager,
-    VanillaDataManagerConfig,
 )
 from nerfstudio.engine.callbacks import TrainingCallback, TrainingCallbackAttributes
 from nerfstudio.models.base_model import Model, ModelConfig
 from nerfstudio.utils import profiler
 
 
 def module_wrapper(ddp_or_model: Union[DDP, Model]) -> Model:
@@ -200,15 +201,15 @@
 
 @dataclass
 class VanillaPipelineConfig(cfg.InstantiateConfig):
     """Configuration for pipeline instantiation"""
 
     _target: Type = field(default_factory=lambda: VanillaPipeline)
     """target class to instantiate"""
-    datamanager: VanillaDataManagerConfig = VanillaDataManagerConfig()
+    datamanager: DataManagerConfig = DataManagerConfig()
     """specifies the datamanager config"""
     model: ModelConfig = ModelConfig()
     """specifies the model config"""
 
 
 class VanillaPipeline(Pipeline):
     """The pipeline class for the vanilla nerf setup of multiple cameras for one or a few scenes.
@@ -218,42 +219,46 @@
         device: location to place model and data
         test_mode:
             'val': loads train/val datasets into memory
             'test': loads train/test dataset into memory
             'inference': does not load any dataset into memory
         world_size: total number of machines available
         local_rank: rank of current machine
+        grad_scaler: gradient scaler used in the trainer
 
     Attributes:
         datamanager: The data manager that will be used
         model: The model that will be used
     """
 
     def __init__(
         self,
         config: VanillaPipelineConfig,
         device: str,
         test_mode: Literal["test", "val", "inference"] = "val",
         world_size: int = 1,
         local_rank: int = 0,
+        grad_scaler: Optional[GradScaler] = None,
     ):
         super().__init__()
         self.config = config
         self.test_mode = test_mode
-        self.datamanager: VanillaDataManager = config.datamanager.setup(
+        self.datamanager: DataManager = config.datamanager.setup(
             device=device, test_mode=test_mode, world_size=world_size, local_rank=local_rank
         )
         self.datamanager.to(device)
         # TODO(ethan): get rid of scene_bounds from the model
         assert self.datamanager.train_dataset is not None, "Missing input dataset"
 
         self._model = config.model.setup(
             scene_box=self.datamanager.train_dataset.scene_box,
             num_train_data=len(self.datamanager.train_dataset),
             metadata=self.datamanager.train_dataset.metadata,
+            device=device,
+            grad_scaler=grad_scaler,
         )
         self.model.to(device)
 
         self.world_size = world_size
         if world_size > 1:
             self._model = typing.cast(Model, DDP(self._model, device_ids=[local_rank], find_unused_parameters=True))
             dist.barrier(device_ids=[local_rank])
@@ -338,14 +343,15 @@
         """Iterate over all the images in the eval dataset and get the average.
 
         Returns:
             metrics_dict: dictionary of metrics
         """
         self.eval()
         metrics_dict_list = []
+        assert isinstance(self.datamanager, VanillaDataManager)
         num_images = len(self.datamanager.fixed_indices_eval_dataloader)
         with Progress(
             TextColumn("[progress.description]{task.description}"),
             BarColumn(),
             TimeElapsedColumn(),
             MofNCompleteColumn(),
             transient=True,
```

### Comparing `nerfstudio-0.3.1/nerfstudio/pipelines/dynamic_batch.py` & `nerfstudio-0.3.2/nerfstudio/pipelines/dynamic_batch.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,17 +13,18 @@
 # limitations under the License.
 
 """
 A pipeline that dynamically chooses the number of rays to sample.
 """
 
 from dataclasses import dataclass, field
-from typing import Literal, Type
+from typing import Literal, Type, Optional
 
 import torch
+from torch.cuda.amp.grad_scaler import GradScaler
 
 from nerfstudio.data.datamanagers.base_datamanager import VanillaDataManager
 from nerfstudio.pipelines.base_pipeline import VanillaPipeline, VanillaPipelineConfig
 
 
 @dataclass
 class DynamicBatchPipelineConfig(VanillaPipelineConfig):
@@ -46,14 +47,15 @@
     def __init__(
         self,
         config: DynamicBatchPipelineConfig,
         device: str,
         test_mode: Literal["test", "val", "inference"] = "val",
         world_size: int = 1,
         local_rank: int = 0,
+        grad_scaler: Optional[GradScaler] = None,
     ):
         super().__init__(config, device, test_mode, world_size, local_rank)
         assert isinstance(
             self.datamanager, VanillaDataManager
         ), "DynamicBatchPipeline only works with VanillaDataManager."
 
         self.dynamic_num_rays_per_batch = self.config.target_num_samples // self.config.max_num_samples_per_ray
```

### Comparing `nerfstudio-0.3.1/nerfstudio/plugins/__init__.py` & `nerfstudio-0.3.2/nerfstudio/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/plugins/registry.py` & `nerfstudio-0.3.2/nerfstudio/plugins/registry.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/plugins/registry_dataparser.py` & `nerfstudio-0.3.2/nerfstudio/plugins/registry_dataparser.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/plugins/types.py` & `nerfstudio-0.3.2/nerfstudio/plugins/types.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/process_data/__init__.py` & `nerfstudio-0.3.2/nerfstudio/process_data/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/process_data/base_converter_to_nerfstudio_dataset.py` & `nerfstudio-0.3.2/nerfstudio/process_data/base_converter_to_nerfstudio_dataset.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/process_data/colmap_converter_to_nerfstudio_dataset.py` & `nerfstudio-0.3.2/nerfstudio/process_data/colmap_converter_to_nerfstudio_dataset.py`

 * *Files 5% similar despite different names*

```diff
@@ -185,17 +185,23 @@
         ) = process_data_utils.find_tool_feature_matcher_combination(
             self.sfm_tool, self.feature_type, self.matcher_type
         )
         # check that sfm_tool is hloc if using refine_pixsfm
         if self.refine_pixsfm:
             assert sfm_tool == "hloc", "refine_pixsfm only works with sfm_tool hloc"
 
+        # set the image_dir if didn't copy
+        if self.skip_image_processing:
+            image_dir = self.data
+        else:
+            image_dir = self.image_dir
+
         if sfm_tool == "colmap":
             colmap_utils.run_colmap(
-                image_dir=self.image_dir,
+                image_dir=image_dir,
                 colmap_dir=self.absolute_colmap_path,
                 camera_model=CAMERA_MODELS[self.camera_type],
                 camera_mask_path=mask_path,
                 gpu=self.gpu,
                 verbose=self.verbose,
                 matching_method=self.matching_method,
                 colmap_cmd=self.colmap_cmd,
@@ -204,15 +210,15 @@
             if mask_path is not None:
                 raise RuntimeError("Cannot use a mask with hloc. Please remove the cropping options " "and try again.")
 
             assert feature_type is not None
             assert matcher_type is not None
             assert matcher_type != "NN"  # Only used for colmap.
             hloc_utils.run_hloc(
-                image_dir=self.image_dir,
+                image_dir=image_dir,
                 colmap_dir=self.absolute_colmap_path,
                 camera_model=CAMERA_MODELS[self.camera_type],
                 verbose=self.verbose,
                 matching_method=self.matching_method,
                 feature_type=feature_type,
                 matcher_type=matcher_type,
                 refine_pixsfm=self.refine_pixsfm,
```

### Comparing `nerfstudio-0.3.1/nerfstudio/process_data/colmap_utils.py` & `nerfstudio-0.3.2/nerfstudio/process_data/colmap_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -601,32 +601,32 @@
             output_path = output_dir / "debug_depth" / out_name
             output_path.parent.mkdir(parents=True, exist_ok=True)
             cv2.imwrite(str(output_path), debug.astype(np.uint8))  # type: ignore
 
     return image_id_to_depth_path
 
 
-def get_matching_summary(num_intial_frames: int, num_matched_frames: int) -> str:
+def get_matching_summary(num_initial_frames: int, num_matched_frames: int) -> str:
     """Returns a summary of the matching results.
 
     Args:
-        num_intial_frames: The number of initial frames.
+        num_initial_frames: The number of initial frames.
         num_matched_frames: The number of matched frames.
 
     Returns:
         A summary of the matching results.
     """
-    match_ratio = num_matched_frames / num_intial_frames
+    match_ratio = num_matched_frames / num_initial_frames
     if match_ratio == 1:
         return "[bold green]COLMAP found poses for all images, CONGRATS!"
     if match_ratio < 0.4:
-        result = f"[bold red]COLMAP only found poses for {num_matched_frames / num_intial_frames * 100:.2f}%"
+        result = f"[bold red]COLMAP only found poses for {num_matched_frames / num_initial_frames * 100:.2f}%"
         result += " of the images. This is low.\nThis can be caused by a variety of reasons,"
         result += " such poor scene coverage, blurry images, or large exposure changes."
         return result
     if match_ratio < 0.8:
-        result = f"[bold yellow]COLMAP only found poses for {num_matched_frames / num_intial_frames * 100:.2f}%"
+        result = f"[bold yellow]COLMAP only found poses for {num_matched_frames / num_initial_frames * 100:.2f}%"
         result += " of the images.\nThis isn't great, but may be ok."
         result += "\nMissing poses can be caused by a variety of reasons, such poor scene coverage, blurry images,"
         result += " or large exposure changes."
         return result
-    return f"[bold green]COLMAP found poses for {num_matched_frames / num_intial_frames * 100:.2f}% of the images."
+    return f"[bold green]COLMAP found poses for {num_matched_frames / num_initial_frames * 100:.2f}% of the images."
```

### Comparing `nerfstudio-0.3.1/nerfstudio/process_data/equirect_utils.py` & `nerfstudio-0.3.2/nerfstudio/process_data/equirect_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -195,15 +195,15 @@
                     cv2.imwrite(f"{output_dir}/{i[:-4]}_{count}.jpg", pers_image)
                     count += 1
 
     return output_dir
 
 
 def compute_resolution_from_equirect(image_dir: Path, num_images: int) -> Tuple[int, int]:
-    """Compute the resolution of the persepctive projections of equirectangular images
+    """Compute the resolution of the perspective projections of equirectangular images
        from the heuristic: num_image * res**2 = orig_height * orig_width.
 
     Args:
         image_dir: The directory containing the equirectangular images.
     returns:
         The target resolution of the perspective projections.
     """
```

### Comparing `nerfstudio-0.3.1/nerfstudio/process_data/hloc_utils.py` & `nerfstudio-0.3.2/nerfstudio/process_data/hloc_utils.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/process_data/images_to_nerfstudio_dataset.py` & `nerfstudio-0.3.2/nerfstudio/process_data/images_to_nerfstudio_dataset.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/process_data/metashape_utils.py` & `nerfstudio-0.3.2/nerfstudio/process_data/metashape_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,16 @@
     ]
     if not calibrated_sensors:
         raise ValueError("No calibrated sensor found in Metashape XML")
     sensor_type = [s.get("type") for s in calibrated_sensors]
     if sensor_type.count(sensor_type[0]) != len(sensor_type):
         raise ValueError(
             "All Metashape sensors do not have the same sensor type. "
-            "nerfstudio does not support per-frame camera_model."
+            "nerfstudio does not support per-frame camera_model types."
+            "Only one camera type can be used: frame, fisheye or spherical (perspective, fisheye or equirectangular)"
         )
     data = {}
     if sensor_type[0] == "frame":
         data["camera_model"] = CAMERA_MODELS["perspective"].value
     elif sensor_type[0] == "fisheye":
         data["camera_model"] = CAMERA_MODELS["fisheye"].value
     elif sensor_type[0] == "spherical":
```

### Comparing `nerfstudio-0.3.1/nerfstudio/process_data/polycam_utils.py` & `nerfstudio-0.3.2/nerfstudio/process_data/polycam_utils.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/process_data/process_data_utils.py` & `nerfstudio-0.3.2/nerfstudio/process_data/process_data_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Helper utils for processing data into the nerfstudio format."""
 
 import math
-import os
 import shutil
 import sys
 from enum import Enum
 from pathlib import Path
 from typing import List, Literal, Optional, OrderedDict, Tuple, Union
 
 import cv2
@@ -191,25 +190,30 @@
         verbose: If True, print extra logging.
     Returns:
         A list of the copied image Paths.
     """
 
     # Remove original directory only if we provide a proper image folder path
     if image_dir.is_dir() and len(image_paths):
-        shutil.rmtree(image_dir, ignore_errors=True)
+        # check that output directory is not the same as input directory
+        if image_dir != image_paths[0].parent:
+            shutil.rmtree(image_dir, ignore_errors=True)
         image_dir.mkdir(exist_ok=True, parents=True)
 
     copied_image_paths = []
 
     # Images should be 1-indexed for the rest of the pipeline.
     for idx, image_path in enumerate(image_paths):
         if verbose:
             CONSOLE.log(f"Copying image {idx + 1} of {len(image_paths)}...")
         copied_image_path = image_dir / f"frame_{idx + 1:05d}{image_path.suffix}"
-        shutil.copy(image_path, copied_image_path)
+        try:
+            shutil.copy(image_path, copied_image_path)
+        except shutil.SameFileError:
+            pass
         copied_image_paths.append(copied_image_path)
 
     if crop_border_pixels is not None:
         file_type = image_paths[0].suffix
         filename = f"frame_%05d{file_type}"
         crop = f"crop=iw-{crop_border_pixels*2}:ih-{crop_border_pixels*2}"
         ffmpeg_cmd = f'ffmpeg -y -noautorotate -i "{image_dir / filename}" -q:v 2 -vf {crop} "{image_dir / filename}"'
@@ -339,19 +343,16 @@
     with status(msg="[bold yellow]Downscaling images...", spinner="growVertical", verbose=verbose):
         downscale_factors = [2**i for i in range(num_downscales + 1)[1:]]
         for downscale_factor in downscale_factors:
             assert downscale_factor > 1
             assert isinstance(downscale_factor, int)
             downscale_dir = image_dir.parent / f"{folder_name}_{downscale_factor}"
             downscale_dir.mkdir(parents=True, exist_ok=True)
-            # Using %05d ffmpeg commands appears to be unreliable (skips images), so use scandir.
-            files = os.scandir(image_dir)
-            for f in files:
-                if f.is_dir():
-                    continue
+            # Using %05d ffmpeg commands appears to be unreliable (skips images).
+            for f in list_images(image_dir):
                 filename = f.name
                 nn_flag = "" if not nearest_neighbor else ":flags=neighbor"
                 ffmpeg_cmd = [
                     f'ffmpeg -y -noautorotate -i "{image_dir / filename}" ',
                     f"-q:v 2 -vf scale=iw/{downscale_factor}:ih/{downscale_factor}{nn_flag} ",
                     f'"{downscale_dir / filename}"',
                 ]
```

### Comparing `nerfstudio-0.3.1/nerfstudio/process_data/realitycapture_utils.py` & `nerfstudio-0.3.2/nerfstudio/process_data/realitycapture_utils.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/process_data/record3d_utils.py` & `nerfstudio-0.3.2/nerfstudio/process_data/record3d_utils.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/process_data/video_to_nerfstudio_dataset.py` & `nerfstudio-0.3.2/nerfstudio/process_data/video_to_nerfstudio_dataset.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/scripts/__init__.py` & `nerfstudio-0.3.2/nerfstudio/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/scripts/blender/__init__.py` & `nerfstudio-0.3.2/nerfstudio/scripts/blender/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/scripts/blender/nerfstudio_blender.py` & `nerfstudio-0.3.2/nerfstudio/scripts/blender/nerfstudio_blender.py`

 * *Files 1% similar despite different names*

```diff
@@ -240,15 +240,15 @@
     # cam_obj = None # the render camera is the active camera
     nerf_bg_mesh = None  # the background NeRF as a mesh
 
     fov_list = []  # list of FOV at each frame
     transformed_camera_path_mat = []  # final transformed world matrix of the camera at each frame
     input_json = None
 
-    def read_camera_coodinates(self):
+    def read_camera_coordinates(self):
         """Read the camera coordinates (world matrix and fov) from the json camera path."""
 
         json_cam_path = self.input_json["camera_path"]
         self.fov_list = []
         self.transformed_camera_path_mat = []
 
         keyframe_counter = 0
@@ -329,15 +329,15 @@
 
         # open the json file
         full_abs_file_path = bpy.path.abspath(file_path_ns_json)
         with open(full_abs_file_path, encoding="utf8") as json_ns_file:
             self.input_json = json.load(json_ns_file)
 
         # call methods to read cam path and create camera
-        self.read_camera_coodinates()
+        self.read_camera_coordinates()
         self.generate_camera()
 
         return {"FINISHED"}
 
 
 # --- Blender UI Panel --- #
```

### Comparing `nerfstudio-0.3.1/nerfstudio/scripts/completions/__init__.py` & `nerfstudio-0.3.2/nerfstudio/scripts/completions/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/scripts/completions/install.py` & `nerfstudio-0.3.2/nerfstudio/scripts/completions/install.py`

 * *Files 0% similar despite different names*

```diff
@@ -391,15 +391,15 @@
                 CONSOLE.log(f":heavy_check_mark: No existing completions at: {target_dir}.")
     elif mode == "install":
         _generate_completions_files(completions_dir, scripts_dir, shells_supported, shells_found)
     else:
         assert_never(mode)
 
     if conda_path is not None:
-        # In conda environment we add the completitions activation scripts.
+        # In conda environment we add the completions activation scripts.
         commands = _get_all_entry_points()
         _update_conda_scripts(commands, completions_dir, mode)
     else:
         # Install or uninstall from bashrc/zshrc.
         for shell in shells_found:
             _update_rc(completions_dir, mode, shell)
```

### Comparing `nerfstudio-0.3.1/nerfstudio/scripts/completions/setup.zsh` & `nerfstudio-0.3.2/nerfstudio/scripts/completions/setup.zsh`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/scripts/datasets/process_nuscenes_masks.py` & `nerfstudio-0.3.2/nerfstudio/scripts/datasets/process_nuscenes_masks.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/scripts/docs/__init__.py` & `nerfstudio-0.3.2/nerfstudio/scripts/docs/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/scripts/docs/add_nb_tags.py` & `nerfstudio-0.3.2/nerfstudio/scripts/docs/add_nb_tags.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/scripts/docs/build_docs.py` & `nerfstudio-0.3.2/nerfstudio/scripts/docs/build_docs.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/scripts/downloads/__init__.py` & `nerfstudio-0.3.2/nerfstudio/scripts/downloads/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/scripts/downloads/download_data.py` & `nerfstudio-0.3.2/nerfstudio/scripts/downloads/download_data.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/scripts/eval.py` & `nerfstudio-0.3.2/nerfstudio/scripts/eval.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/scripts/exporter.py` & `nerfstudio-0.3.2/nerfstudio/scripts/exporter.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,24 +55,56 @@
 
     load_config: Path
     """Path to the config YAML file."""
     output_dir: Path
     """Path to the output directory."""
 
 
+def validate_pipeline(normal_method: str, normal_output_name: str, pipeline: Pipeline) -> None:
+    """Check that the pipeline is valid for this exporter.
+
+    Args:
+        normal_method: Method to estimate normals with. Either "open3d" or "model_output".
+        normal_output_name: Name of the normal output.
+        pipeline: Pipeline to evaluate with.
+    """
+    if normal_method == "model_output":
+        CONSOLE.print("Checking that the pipeline has a normal output.")
+        origins = torch.zeros((1, 3), device=pipeline.device)
+        directions = torch.ones_like(origins)
+        pixel_area = torch.ones_like(origins[..., :1])
+        camera_indices = torch.zeros_like(origins[..., :1])
+        ray_bundle = RayBundle(
+            origins=origins, directions=directions, pixel_area=pixel_area, camera_indices=camera_indices
+        )
+        outputs = pipeline.model(ray_bundle)
+        if normal_output_name not in outputs:
+            CONSOLE.print(f"[bold yellow]Warning: Normal output '{normal_output_name}' not found in pipeline outputs.")
+            CONSOLE.print(f"Available outputs: {list(outputs.keys())}")
+            CONSOLE.print(
+                "[bold yellow]Warning: Please train a model with normals "
+                "(e.g., nerfacto with predicted normals turned on)."
+            )
+            CONSOLE.print("[bold yellow]Warning: Or change --normal-method")
+            CONSOLE.print("[bold yellow]Exiting early.")
+            sys.exit(1)
+
+
 @dataclass
 class ExportPointCloud(Exporter):
     """Export NeRF as a point cloud."""
 
     num_points: int = 1000000
     """Number of points to generate. May result in less if outlier removal is used."""
     remove_outliers: bool = True
     """Remove outliers from the point cloud."""
-    estimate_normals: bool = False
-    """Estimate normals for the point cloud."""
+    normal_method: Literal["open3d", "model_output"] = "model_output"
+    """Method to estimate normals with."""
+    normal_output_name: str = "normals"
+    """Name of the normal output."""
     depth_output_name: str = "depth"
     """Name of the depth output."""
     rgb_output_name: str = "rgb"
     """Name of the RGB output."""
     use_bounding_box: bool = True
     """Only query points within the bounding box"""
     bounding_box_min: Tuple[float, float, float] = (-1, -1, -1)
@@ -88,27 +120,32 @@
         """Export point cloud."""
 
         if not self.output_dir.exists():
             self.output_dir.mkdir(parents=True)
 
         _, pipeline, _, _ = eval_setup(self.load_config)
 
+        validate_pipeline(self.normal_method, self.normal_output_name, pipeline)
+
         # Increase the batchsize to speed up the evaluation.
         assert isinstance(pipeline.datamanager, VanillaDataManager)
         assert pipeline.datamanager.train_pixel_sampler is not None
         pipeline.datamanager.train_pixel_sampler.num_rays_per_batch = self.num_rays_per_batch
 
+        # Whether the normals should be estimated based on the point cloud.
+        estimate_normals = self.normal_method == "open3d"
+
         pcd = generate_point_cloud(
             pipeline=pipeline,
             num_points=self.num_points,
             remove_outliers=self.remove_outliers,
-            estimate_normals=self.estimate_normals,
+            estimate_normals=estimate_normals,
             rgb_output_name=self.rgb_output_name,
             depth_output_name=self.depth_output_name,
-            normal_output_name=None,
+            normal_output_name=self.normal_output_name if self.normal_method == "model_output" else None,
             use_bounding_box=self.use_bounding_box,
             bounding_box_min=self.bounding_box_min,
             bounding_box_max=self.bounding_box_max,
             std_ratio=self.std_ratio,
         )
         torch.cuda.empty_cache()
 
@@ -233,47 +270,23 @@
     num_pixels_per_side: int = 2048
     """If using xatlas for unwrapping, the pixels per side of the texture image."""
     target_num_faces: Optional[int] = 50000
     """Target number of faces for the mesh to texture."""
     std_ratio: float = 10.0
     """Threshold based on STD of the average distances across the point cloud to remove outliers."""
 
-    def validate_pipeline(self, pipeline: Pipeline) -> None:
-        """Check that the pipeline is valid for this exporter."""
-        if self.normal_method == "model_output":
-            CONSOLE.print("Checking that the pipeline has a normal output.")
-            origins = torch.zeros((1, 3), device=pipeline.device)
-            directions = torch.ones_like(origins)
-            pixel_area = torch.ones_like(origins[..., :1])
-            camera_indices = torch.zeros_like(origins[..., :1])
-            ray_bundle = RayBundle(
-                origins=origins, directions=directions, pixel_area=pixel_area, camera_indices=camera_indices
-            )
-            outputs = pipeline.model(ray_bundle)
-            if self.normal_output_name not in outputs:
-                CONSOLE.print(
-                    f"[bold yellow]Warning: Normal output '{self.normal_output_name}' not found in pipeline outputs."
-                )
-                CONSOLE.print(f"Available outputs: {list(outputs.keys())}")
-                CONSOLE.print(
-                    "[bold yellow]Warning: Please train a model with normals "
-                    "(e.g., nerfacto with predicted normals turned on)."
-                )
-                CONSOLE.print("[bold yellow]Warning: Or change --normal-method")
-                CONSOLE.print("[bold yellow]Exiting early.")
-                sys.exit(1)
-
     def main(self) -> None:
         """Export mesh"""
 
         if not self.output_dir.exists():
             self.output_dir.mkdir(parents=True)
 
         _, pipeline, _, _ = eval_setup(self.load_config)
-        self.validate_pipeline(pipeline)
+
+        validate_pipeline(self.normal_method, self.normal_output_name, pipeline)
 
         # Increase the batchsize to speed up the evaluation.
         assert isinstance(pipeline.datamanager, VanillaDataManager)
         assert pipeline.datamanager.train_pixel_sampler is not None
         pipeline.datamanager.train_pixel_sampler.num_rays_per_batch = self.num_rays_per_batch
 
         # Whether the normals should be estimated based on the point cloud.
@@ -366,15 +379,15 @@
 
         CONSOLE.print("Extracting mesh with marching cubes... which may take a while")
 
         assert (
             self.resolution % 512 == 0
         ), f"""resolution must be divisible by 512, got {self.resolution}.
         This is important because the algorithm uses a multi-resolution approach
-        to evaluate the SDF where the mimimum resolution is 512."""
+        to evaluate the SDF where the minimum resolution is 512."""
 
         # Extract mesh using marching cubes for sdf at a multi-scale resolution.
         multi_res_mesh = generate_mesh_with_multires_marching_cubes(
             geometry_callable_field=lambda x: cast(SDFField, pipeline.model.field)
             .forward_geonetwork(x)[:, 0]
             .contiguous(),
             resolution=self.resolution,
```

### Comparing `nerfstudio-0.3.1/nerfstudio/scripts/github/__init__.py` & `nerfstudio-0.3.2/nerfstudio/scripts/github/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/scripts/github/run_actions.py` & `nerfstudio-0.3.2/nerfstudio/scripts/github/run_actions.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/scripts/process_data.py` & `nerfstudio-0.3.2/nerfstudio/scripts/process_data.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/scripts/render.py` & `nerfstudio-0.3.2/nerfstudio/scripts/render.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 render.py
 """
 from __future__ import annotations
 
 import json
 import os
 import struct
+import shutil
 import sys
 from contextlib import ExitStack
 from dataclasses import dataclass, field
 from pathlib import Path
 from typing import Any, Dict, List, Literal, Optional, Union
 
 import mediapy as media
@@ -55,14 +56,15 @@
 from nerfstudio.data.datamanagers.base_datamanager import VanillaDataManager
 from nerfstudio.data.scene_box import SceneBox
 from nerfstudio.model_components import renderers
 from nerfstudio.pipelines.base_pipeline import Pipeline
 from nerfstudio.utils import colormaps, install_checks
 from nerfstudio.utils.eval_utils import eval_setup
 from nerfstudio.utils.rich_utils import CONSOLE, ItersPerSecColumn
+from nerfstudio.utils.scripts import run_command
 
 
 def _render_trajectory_video(
     pipeline: Pipeline,
     cameras: Cameras,
     output_filename: Path,
     rendered_output_names: List[str],
@@ -338,28 +340,89 @@
 
         with open(self.camera_path_filename, "r", encoding="utf-8") as f:
             camera_path = json.load(f)
         seconds = camera_path["seconds"]
         crop_data = get_crop_from_json(camera_path)
         camera_path = get_path_from_json(camera_path)
 
+        if camera_path.camera_type[0] == CameraType.OMNIDIRECTIONALSTEREO_L.value:
+            # temp folder for writing left and right view renders
+            temp_folder_path = self.output_path.parent / (self.output_path.stem + "_temp")
+
+            Path(temp_folder_path).mkdir(parents=True, exist_ok=True)
+            left_eye_path = temp_folder_path / "ods_render_Left.mp4"
+
+            self.output_path = left_eye_path
+
+            CONSOLE.print("[bold green]:goggles: Omni-directional Stereo VR :goggles:")
+            CONSOLE.print("Rendering left eye view")
+
+        # add mp4 suffix to video output if none is specified
+        if self.output_format == "video" and str(self.output_path.suffix) == "":
+            self.output_path = self.output_path.with_suffix(".mp4")
+
         _render_trajectory_video(
             pipeline,
             camera_path,
             output_filename=self.output_path,
             rendered_output_names=self.rendered_output_names,
             rendered_resolution_scaling_factor=1.0 / self.downscale_factor,
             crop_data=crop_data,
             seconds=seconds,
             output_format=self.output_format,
             image_format=self.image_format,
             jpeg_quality=self.jpeg_quality,
             colormap_options=self.colormap_options,
         )
 
+        if camera_path.camera_type[0] == CameraType.OMNIDIRECTIONALSTEREO_L.value:
+            # declare paths for left and right renders
+
+            left_eye_path = self.output_path
+            right_eye_path = left_eye_path.parent / "ods_render_Right.mp4"
+
+            self.output_path = right_eye_path
+            camera_path.camera_type[0] = CameraType.OMNIDIRECTIONALSTEREO_R.value
+
+            CONSOLE.print("Rendering right eye view")
+            _render_trajectory_video(
+                pipeline,
+                camera_path,
+                output_filename=self.output_path,
+                rendered_output_names=self.rendered_output_names,
+                rendered_resolution_scaling_factor=1.0 / self.downscale_factor,
+                crop_data=crop_data,
+                seconds=seconds,
+                output_format=self.output_format,
+                image_format=self.image_format,
+                jpeg_quality=self.jpeg_quality,
+                colormap_options=self.colormap_options,
+            )
+
+            # stack the left and right eye renders for final output
+            self.output_path = Path(str(left_eye_path.parent)[:-5] + ".mp4")
+            ffmpeg_ods_command = ""
+            if self.output_format == "video":
+                ffmpeg_ods_command = f'ffmpeg -y -i "{left_eye_path}" -i "{right_eye_path}" -filter_complex "[0:v]pad=iw:2*ih[int];[int][1:v]overlay=0:h" -c:v libx264 -crf 23 -preset veryfast "{self.output_path}"'
+                run_command(ffmpeg_ods_command, verbose=False)
+            if self.output_format == "images":
+                # create a folder for the stacked renders
+                self.output_path = Path(str(left_eye_path.parent)[:-5])
+                self.output_path.mkdir(parents=True, exist_ok=True)
+                if self.image_format == "png":
+                    ffmpeg_ods_command = f'ffmpeg -y -pattern_type glob -i "{str(left_eye_path.with_suffix("") / "*.png")}"  -pattern_type glob -i "{str(right_eye_path.with_suffix("") / "*.png")}" -filter_complex vstack -start_number 0 "{str(self.output_path)+"//%05d.png"}"'
+                elif self.image_format == "jpeg":
+                    ffmpeg_ods_command = f'ffmpeg -y -pattern_type glob -i "{str(left_eye_path.with_suffix("") / "*.jpg")}"  -pattern_type glob -i "{str(right_eye_path.with_suffix("") / "*.jpg")}" -filter_complex vstack -start_number 0 "{str(self.output_path)+"//%05d.jpg"}"'
+                run_command(ffmpeg_ods_command, verbose=False)
+
+            # remove the temp files directory
+            if str(left_eye_path.parent)[-5:] == "_temp":
+                shutil.rmtree(left_eye_path.parent, ignore_errors=True)
+            CONSOLE.print("[bold green]Final ODS Render Complete")
+
 
 @dataclass
 class RenderInterpolated(BaseRender):
     """Render a trajectory that interpolates between training or eval dataset images."""
 
     rendered_output_names: List[str] = field(default_factory=lambda: ["rgb"])
     """Name of the renderer outputs to use. rgb, depth, etc. concatenates them along y axis"""
```

### Comparing `nerfstudio-0.3.1/nerfstudio/scripts/texture.py` & `nerfstudio-0.3.2/nerfstudio/scripts/texture.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/scripts/train.py` & `nerfstudio-0.3.2/nerfstudio/scripts/train.py`

 * *Files 15% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
 from __future__ import annotations
 
 import random
 import socket
 import traceback
 from datetime import timedelta
-from typing import Any, Callable, Optional
+from typing import Any, Callable, Literal, Optional
 
 import numpy as np
 import torch
 import torch.distributed as dist
 import torch.multiprocessing as mp
 import tyro
 import yaml
@@ -100,91 +100,95 @@
     trainer.train()
 
 
 def _distributed_worker(
     local_rank: int,
     main_func: Callable,
     world_size: int,
-    num_gpus_per_machine: int,
+    num_devices_per_machine: int,
     machine_rank: int,
     dist_url: str,
     config: TrainerConfig,
     timeout: timedelta = DEFAULT_TIMEOUT,
+    device_type: Literal["cpu", "cuda", "mps"] = "cuda",
 ) -> Any:
     """Spawned distributed worker that handles the initialization of process group and handles the
        training process on multiple processes.
 
     Args:
         local_rank: Current rank of process.
         main_func: Function that will be called by the distributed workers.
         world_size: Total number of gpus available.
-        num_gpus_per_machine: Number of GPUs per machine.
+        num_devices_per_machine: Number of GPUs per machine.
         machine_rank: Rank of this machine.
         dist_url: URL to connect to for distributed jobs, including protocol
             E.g., "tcp://127.0.0.1:8686".
             It can be set to "auto" to automatically select a free port on localhost.
         config: TrainerConfig specifying training regimen.
         timeout: Timeout of the distributed workers.
 
     Raises:
         e: Exception in initializing the process group
 
     Returns:
         Any: TODO: determine the return type
     """
     assert torch.cuda.is_available(), "cuda is not available. Please check your installation."
-    global_rank = machine_rank * num_gpus_per_machine + local_rank
+    global_rank = machine_rank * num_devices_per_machine + local_rank
 
     dist.init_process_group(
-        backend="nccl",
+        backend="nccl" if device_type == "cuda" else "gloo",
         init_method=dist_url,
         world_size=world_size,
         rank=global_rank,
         timeout=timeout,
     )
     assert comms.LOCAL_PROCESS_GROUP is None
-    num_machines = world_size // num_gpus_per_machine
+    num_machines = world_size // num_devices_per_machine
     for i in range(num_machines):
-        ranks_on_i = list(range(i * num_gpus_per_machine, (i + 1) * num_gpus_per_machine))
+        ranks_on_i = list(range(i * num_devices_per_machine, (i + 1) * num_devices_per_machine))
         pg = dist.new_group(ranks_on_i)
         if i == machine_rank:
             comms.LOCAL_PROCESS_GROUP = pg
 
-    assert num_gpus_per_machine <= torch.cuda.device_count()
+    assert num_devices_per_machine <= torch.cuda.device_count()
     output = main_func(local_rank, world_size, config, global_rank)
     comms.synchronize()
     dist.destroy_process_group()
     return output
 
 
 def launch(
     main_func: Callable,
-    num_gpus_per_machine: int,
+    num_devices_per_machine: int,
     num_machines: int = 1,
     machine_rank: int = 0,
     dist_url: str = "auto",
     config: Optional[TrainerConfig] = None,
     timeout: timedelta = DEFAULT_TIMEOUT,
+    device_type: Literal["cpu", "cuda", "mps"] = "cuda",
 ) -> None:
     """Function that spawns multiple processes to call on main_func
 
     Args:
         main_func (Callable): function that will be called by the distributed workers
-        num_gpus_per_machine (int): number of GPUs per machine
+        num_devices_per_machine (int): number of GPUs per machine
         num_machines (int, optional): total number of machines
         machine_rank (int, optional): rank of this machine.
         dist_url (str, optional): url to connect to for distributed jobs.
         config (TrainerConfig, optional): config file specifying training regimen.
         timeout (timedelta, optional): timeout of the distributed workers.
+        device_type: type of device to use for training.
     """
     assert config is not None
-    world_size = num_machines * num_gpus_per_machine
-    if world_size <= 1:
-        # world_size=0 uses one CPU in one process.
-        # world_size=1 uses one GPU in one process.
+    world_size = num_machines * num_devices_per_machine
+    if world_size == 0:
+        raise ValueError("world_size cannot be 0")
+    elif world_size == 1:
+        # uses one process
         try:
             main_func(local_rank=0, world_size=world_size, config=config)
         except KeyboardInterrupt:
             # print the stack trace
             CONSOLE.print(traceback.format_exc())
         finally:
             profiler.flush_profiler(config.logging)
@@ -195,25 +199,17 @@
             port = _find_free_port()
             dist_url = f"tcp://127.0.0.1:{port}"
         if num_machines > 1 and dist_url.startswith("file://"):
             CONSOLE.log("file:// is not a reliable init_method in multi-machine jobs. Prefer tcp://")
 
         process_context = mp.spawn(
             _distributed_worker,
-            nprocs=num_gpus_per_machine,
+            nprocs=num_devices_per_machine,
             join=False,
-            args=(
-                main_func,
-                world_size,
-                num_gpus_per_machine,
-                machine_rank,
-                dist_url,
-                config,
-                timeout,
-            ),
+            args=(main_func, world_size, num_devices_per_machine, machine_rank, dist_url, config, timeout, device_type),
         )
         # process_context won't be None because join=False, so it's okay to assert this
         # for Pylance reasons
         assert process_context is not None
         try:
             process_context.join()
         except KeyboardInterrupt:
@@ -231,25 +227,30 @@
     """Main function."""
 
     config.set_timestamp()
     if config.data:
         CONSOLE.log("Using --data alias for --data.pipeline.datamanager.data")
         config.pipeline.datamanager.data = config.data
 
+    if config.prompt:
+        CONSOLE.log("Using --prompt alias for --data.pipeline.model.prompt")
+        config.pipeline.model.prompt = config.prompt
+
     if config.load_config:
         CONSOLE.log(f"Loading pre-set config from: {config.load_config}")
         config = yaml.load(config.load_config.read_text(), Loader=yaml.Loader)
 
     # print and save config
     config.print_to_terminal()
     config.save_config()
 
     launch(
         main_func=train_loop,
-        num_gpus_per_machine=config.machine.num_gpus,
+        num_devices_per_machine=config.machine.num_devices,
+        device_type=config.machine.device_type,
         num_machines=config.machine.num_machines,
         machine_rank=config.machine.machine_rank,
         dist_url=config.machine.dist_url,
         config=config,
     )
```

### Comparing `nerfstudio-0.3.1/nerfstudio/scripts/viewer/__init__.py` & `nerfstudio-0.3.2/nerfstudio/scripts/viewer/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/scripts/viewer/run_viewer.py` & `nerfstudio-0.3.2/nerfstudio/scripts/viewer/run_viewer.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/scripts/viewer/sync_viser_message_defs.py` & `nerfstudio-0.3.2/nerfstudio/scripts/viewer/sync_viser_message_defs.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/utils/__init__.py` & `nerfstudio-0.3.2/nerfstudio/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/utils/colormaps.py` & `nerfstudio-0.3.2/nerfstudio/utils/colormaps.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import matplotlib
 import torch
 from jaxtyping import Bool, Float
 from torch import Tensor
 
 from nerfstudio.utils import colors
 
-Colormaps = Literal["default", "turbo", "viridis", "magma", "inferno", "cividis", "pca"]
+Colormaps = Literal["default", "turbo", "viridis", "magma", "inferno", "cividis", "gray", "pca"]
 
 
 @dataclass(frozen=True)
 class ColormapOptions:
     """Options for colormap"""
 
     colormap: Colormaps = "default"
@@ -100,14 +100,16 @@
     Returns:
         Tensor: Colored image with colors in [0, 1]
     """
     if colormap == "default":
         colormap = "turbo"
 
     image = torch.nan_to_num(image, 0)
+    if colormap == "gray":
+        return image.repeat(1, 1, 3)
     image_long = (image * 255).long()
     image_long_min = torch.min(image_long)
     image_long_max = torch.max(image_long)
     assert image_long_min >= 0, f"the min value is {image_long_min}"
     assert image_long_max <= 255, f"the max value is {image_long_max}"
     return torch.tensor(matplotlib.colormaps[colormap].colors, device=image.device)[image_long[..., 0]]
```

### Comparing `nerfstudio-0.3.1/nerfstudio/utils/colors.py` & `nerfstudio-0.3.2/nerfstudio/utils/colors.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/utils/comms.py` & `nerfstudio-0.3.2/nerfstudio/utils/comms.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/utils/decorators.py` & `nerfstudio-0.3.2/nerfstudio/utils/decorators.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,19 +46,19 @@
             ret = func(self, *args, **kwargs)
         return ret
 
     return wrapper
 
 
 def check_viewer_enabled(func: Callable) -> Callable:
-    """Decorator: check if viewer is enabled and only run on main process"""
+    """Decorator: check if the viewer or beta viewer is enabled and only run on main process"""
 
     def wrapper(self, *args, **kwargs):
         ret = None
-        if self.config.is_viewer_enabled() and comms.is_main_process():
+        if (self.config.is_viewer_enabled() or self.config.is_viewer_beta_enabled()) and comms.is_main_process():
             ret = func(self, *args, **kwargs)
         return ret
 
     return wrapper
 
 
 def check_eval_enabled(func: Callable) -> Callable:
```

### Comparing `nerfstudio-0.3.1/nerfstudio/utils/eval_utils.py` & `nerfstudio-0.3.2/nerfstudio/utils/eval_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 import sys
 from pathlib import Path
 from typing import Literal, Optional, Tuple
 
 import torch
 import yaml
 
+from nerfstudio.configs.method_configs import all_methods
 from nerfstudio.data.datamanagers.base_datamanager import VanillaDataManagerConfig
 from nerfstudio.engine.trainer import TrainerConfig
 from nerfstudio.pipelines.base_pipeline import Pipeline
 from nerfstudio.utils.rich_utils import CONSOLE
 
 
 def eval_load_checkpoint(config: TrainerConfig, pipeline: Pipeline) -> Tuple[Path, int]:
@@ -83,14 +84,15 @@
     Returns:
         Loaded config, pipeline module, corresponding checkpoint, and step
     """
     # load save config
     config = yaml.load(config_path.read_text(), Loader=yaml.Loader)
     assert isinstance(config, TrainerConfig)
 
+    config.pipeline.datamanager._target = all_methods[config.method_name].pipeline.datamanager._target
     if eval_num_rays_per_chunk:
         config.pipeline.model.eval_num_rays_per_chunk = eval_num_rays_per_chunk
 
     # load checkpoints from wherever they were saved
     # TODO: expose the ability to choose an arbitrary checkpoint
     config.load_dir = config.get_checkpoint_dir()
     if isinstance(config.pipeline.datamanager, VanillaDataManagerConfig):
```

### Comparing `nerfstudio-0.3.1/nerfstudio/utils/install_checks.py` & `nerfstudio-0.3.2/nerfstudio/utils/install_checks.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/utils/io.py` & `nerfstudio-0.3.2/nerfstudio/utils/io.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/utils/math.py` & `nerfstudio-0.3.2/nerfstudio/utils/math.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,20 +76,20 @@
         components[..., 15] = 0.5900435899266435 * x * (xx - 3 * yy)
 
     # l4
     if levels > 4:
         components[..., 16] = 2.5033429417967046 * x * y * (xx - yy)
         components[..., 17] = 1.7701307697799304 * y * z * (3 * xx - yy)
         components[..., 18] = 0.9461746957575601 * x * y * (7 * zz - 1)
-        components[..., 19] = 0.6690465435572892 * y * (7 * zz - 3)
+        components[..., 19] = 0.6690465435572892 * y * z * (7 * zz - 3)
         components[..., 20] = 0.10578554691520431 * (35 * zz * zz - 30 * zz + 3)
         components[..., 21] = 0.6690465435572892 * x * z * (7 * zz - 3)
         components[..., 22] = 0.47308734787878004 * (xx - yy) * (7 * zz - 1)
         components[..., 23] = 1.7701307697799304 * x * z * (xx - 3 * yy)
-        components[..., 24] = 0.4425326924449826 * (xx * (xx - 3 * yy) - yy * (3 * xx - yy))
+        components[..., 24] = 0.6258357354491761 * (xx * (xx - 3 * yy) - yy * (3 * xx - yy))
 
     return components
 
 
 @dataclass
 class Gaussians:
     """Stores Gaussians
```

### Comparing `nerfstudio-0.3.1/nerfstudio/utils/misc.py` & `nerfstudio-0.3.2/nerfstudio/utils/misc.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 """
 Miscellaneous helper code.
 """
 
 
 import platform
 from typing import Any, Callable, Dict, List, Optional, TypeVar, Union
+import warnings
 
 import torch
 
 T = TypeVar("T")
 TKey = TypeVar("TKey")
 
 
@@ -163,15 +164,21 @@
 
 def torch_compile(*args, **kwargs):
     """
     Safe torch.compile with backward compatibility for PyTorch 1.x
     """
     if not hasattr(torch, "compile"):
         # Backward compatibility for PyTorch 1.x
+        warnings.warn(
+            "PyTorch 1.x will no longer be supported by Nerstudio. Please upgrade to PyTorch 2.x.", DeprecationWarning
+        )
         return torch.jit.script
     elif platform.system() == "Windows":
         # torch.compile is not supported on Windows
         # https://github.com/orgs/pytorch/projects/27
         # TODO: @jkulhanek, remove this once torch.compile is supported on Windows
+        warnings.warn(
+            "Windows does not yet support torch.compile and the performance will be affected.", RuntimeWarning
+        )
         return lambda x: x
     else:
         return torch.compile(*args, **kwargs)
```

### Comparing `nerfstudio-0.3.1/nerfstudio/utils/plotly_utils.py` & `nerfstudio-0.3.2/nerfstudio/utils/plotly_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
 Visualization code for plotly.
 The function use prefix conventions in the following way:
     - 'get_*' functions (e.g., 'get_camera_frustums')
-        return data that can be ploted with plotly
+        return data that can be plotted with plotly
     - 'vis_*' functions (e.g., 'vis_camera_rays')
         return 'go.Figure' objects which are the plots. Go Figure! :')
 """
 
 from typing import Any, List, Optional, Union
 
 import numpy as np
```

### Comparing `nerfstudio-0.3.1/nerfstudio/utils/poses.py` & `nerfstudio-0.3.2/nerfstudio/utils/poses.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/utils/printing.py` & `nerfstudio-0.3.2/nerfstudio/utils/printing.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,18 +15,18 @@
 """A collection of common strings and print statements used throughout the codebase."""
 
 from math import floor, log
 
 from nerfstudio.utils.rich_utils import CONSOLE
 
 
-def print_tcnn_speed_warning(method_name: str):
+def print_tcnn_speed_warning(module_name: str):
     """Prints a warning about the speed of the TCNN."""
     CONSOLE.line()
-    CONSOLE.print(f"[bold yellow]WARNING: Using a slow implementation of {method_name}. ")
+    CONSOLE.print(f"[bold yellow]WARNING: Using a slow implementation for the {module_name} module. ")
     CONSOLE.print(
         "[bold yellow]:person_running: :person_running: "
         + "Install tcnn for speedups :person_running: :person_running:"
     )
     CONSOLE.print("[yellow]pip install git+https://github.com/NVlabs/tiny-cuda-nn/#subdirectory=bindings/torch")
     CONSOLE.line()
```

### Comparing `nerfstudio-0.3.1/nerfstudio/utils/profiler.py` & `nerfstudio-0.3.2/nerfstudio/utils/profiler.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/utils/rich_utils.py` & `nerfstudio-0.3.2/nerfstudio/utils/rich_utils.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/utils/scripts.py` & `nerfstudio-0.3.2/nerfstudio/utils/scripts.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/utils/tensor_dataclass.py` & `nerfstudio-0.3.2/nerfstudio/utils/tensor_dataclass.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/utils/writer.py` & `nerfstudio-0.3.2/nerfstudio/utils/writer.py`

 * *Files 1% similar despite different names*

```diff
@@ -316,15 +316,15 @@
 
     def write_config(self, name: str, config_dict: Dict[str, Any], step: int):
         """Function that writes out the config to wandb
 
         Args:
             config: config dictionary to write out
         """
-        wandb.config.update(config_dict)
+        wandb.config.update(config_dict, allow_val_change=True)
 
 
 @decorate_all([check_main_thread])
 class TensorboardWriter(Writer):
     """Tensorboard Writer Class"""
 
     def __init__(self, log_dir: Path):
```

### Comparing `nerfstudio-0.3.1/nerfstudio/viewer/__init__.py` & `nerfstudio-0.3.2/nerfstudio/viewer/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/viewer/app/package.json` & `nerfstudio-0.3.2/nerfstudio/viewer/app/package.json`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/viewer/app/run_deploy.py` & `nerfstudio-0.3.2/nerfstudio/viewer/app/run_deploy.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/viewer/app/src/themes/leva_theme.json` & `nerfstudio-0.3.2/nerfstudio/viewer/app/src/themes/leva_theme.json`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/viewer/server/__init__.py` & `nerfstudio-0.3.2/nerfstudio/viewer/server/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/viewer/server/control_panel.py` & `nerfstudio-0.3.2/nerfstudio/viewer/server/control_panel.py`

 * *Files 0% similar despite different names*

```diff
@@ -357,11 +357,11 @@
     Returns:
         a list of available colormap options
     """
     colormap_options: List[Colormaps] = []
     if dimensions == 3:
         colormap_options = ["default"]
     if dimensions == 1 and dtype == torch.float:
-        colormap_options = [c for c in list(get_args(Colormaps)) if c != "default"]
+        colormap_options = [c for c in list(get_args(Colormaps)) if c not in ("default", "pca")]
     if dimensions > 3:
         colormap_options = ["pca"]
     return colormap_options
```

### Comparing `nerfstudio-0.3.1/nerfstudio/viewer/server/gui_utils.py` & `nerfstudio-0.3.2/nerfstudio/viewer/server/gui_utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-""" Utilites for generating custom gui elements in the viewer """
+""" Utilities for generating custom gui elements in the viewer """
 
 from __future__ import annotations
 
 from typing import Any, List, Tuple
 
 from torch import nn
 
@@ -56,12 +56,16 @@
     for k, v in obj_props:
         if k[0] == "_":
             continue
         new_tree_stub = f"{tree_stub}/{k}"
         if isinstance(v, type_check):
             add(ret, new_tree_stub, v)
         elif isinstance(v, nn.Module):
+            if v is obj:
+                # some nn.Modules might contain infinite references, e.g. consider foo = nn.Module(), foo.bar = foo
+                # to stop infinite recursion, we skip such attributes
+                continue
             lower_rets = parse_object(v, type_check, new_tree_stub)
             # check that the values aren't already in the tree
             for ts, o in lower_rets:
                 add(ret, ts, o)
     return ret
```

### Comparing `nerfstudio-0.3.1/nerfstudio/viewer/server/path.py` & `nerfstudio-0.3.2/nerfstudio/viewer/server/path.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/viewer/server/render_state_machine.py` & `nerfstudio-0.3.2/nerfstudio/viewer/server/render_state_machine.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,24 +94,24 @@
             #  1. we are in low_moving state
             #  2. the current next_action is move, static, or rerender
             return
         elif self.next_action == "rerender":
             # never overwrite rerenders
             pass
         else:
-            #  monimal use case, just set the next action
+            #  minimal use case, just set the next action
             self.next_action = action
 
         # handle interrupt logic
         if self.state == "high" and self.next_action.action in ("move", "rerender"):
             self.interrupt_render_flag = True
         self.render_trigger.set()
 
     def _render_img(self, cam_msg: CameraMessage):
-        """Takes the current camera, generates rays, and renders the iamge
+        """Takes the current camera, generates rays, and renders the image
 
         Args:
             cam_msg: the camera message to render
         """
 
         # initialize the camera ray bundle
         viewer_utils.update_render_aabb(
@@ -234,15 +234,15 @@
             quality=self.viewer.config.jpeg_quality,
         )
 
     def _calculate_image_res(self, aspect_ratio: float) -> Tuple[int, int]:
         """Calculate the maximum image height that can be rendered in the time budget
 
         Args:
-            apect_ratio: the aspect ratio of the current view
+            aspect_ratio: the aspect ratio of the current view
         Returns:
             image_height: the maximum image height that can be rendered in the time budget
             image_width: the maximum image width that can be rendered in the time budget
         """
         max_res = self.viewer.control_panel.max_res
         if self.state == "high":
             # high res is always static
```

### Comparing `nerfstudio-0.3.1/nerfstudio/viewer/server/state/node.py` & `nerfstudio-0.3.2/nerfstudio/viewer/server/state/node.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/viewer/server/state/state_node.py` & `nerfstudio-0.3.2/nerfstudio/viewer/server/state/state_node.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/viewer/server/utils.py` & `nerfstudio-0.3.2/nerfstudio/viewer/server/utils.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/viewer/server/viewer_elements.py` & `nerfstudio-0.3.2/nerfstudio/viewer/server/viewer_elements.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/viewer/server/viewer_state.py` & `nerfstudio-0.3.2/nerfstudio/viewer/server/viewer_state.py`

 * *Files 0% similar despite different names*

```diff
@@ -328,15 +328,15 @@
             camera_to_worlds=camera_to_world[None, ...],
             times=torch.tensor([self.control_panel.time], dtype=torch.float32),
         )
         camera = camera.to(self.get_model().device)
         return camera
 
     def _pick_drawn_image_idxs(self, total_num: int) -> list[int]:
-        """Determine indicies of images to display in viewer.
+        """Determine indices of images to display in viewer.
 
         Args:
             total_num: total number of training images.
 
         Returns:
             List of indices from [0, total_num-1].
         """
```

### Comparing `nerfstudio-0.3.1/nerfstudio/viewer/server/viewer_utils.py` & `nerfstudio-0.3.2/nerfstudio/viewer/server/viewer_utils.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/viewer/viser/__init__.py` & `nerfstudio-0.3.2/nerfstudio/viewer/viser/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,14 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-""" Viser is used for the nerfstudio viewr backend """
+""" Viser is used for the nerfstudio viewer backend """
 
 
 from .message_api import GuiHandle as GuiHandle
 from .message_api import GuiSelectHandle as GuiSelectHandle
 from .messages import NerfstudioMessage as NerfstudioMessage
 from .server import ViserServer as ViserServer
```

### Comparing `nerfstudio-0.3.1/nerfstudio/viewer/viser/gui.py` & `nerfstudio-0.3.2/nerfstudio/viewer/viser/gui.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio/viewer/viser/message_api.py` & `nerfstudio-0.3.2/nerfstudio/viewer/viser/message_api.py`

 * *Files identical despite different names*

```diff
@@ -120,15 +120,15 @@
 TLiteralString = TypeVar("TLiteralString", bound=LiteralString)
 
 
 class MessageApi(abc.ABC):
     """Interface for all commands we can use to send messages over a websocket connection.
 
     Should be implemented by both our global server object (for broadcasting) and by
-    invidividual clients."""
+    individual clients."""
 
     def __init__(self) -> None:
         self._handle_state_from_gui_name: Dict[str, _GuiHandleState[Any]] = {}
         self._gui_folder_labels: List[str] = []
 
     @abc.abstractmethod
     def _queue(self, message: messages.NerfstudioMessage) -> None:
```

### Comparing `nerfstudio-0.3.1/nerfstudio/viewer/viser/messages.py` & `nerfstudio-0.3.2/nerfstudio/viewer/viser/messages.py`

 * *Files 1% similar despite different names*

```diff
@@ -182,18 +182,18 @@
     @override
     def redundancy_key(self) -> str:
         return f"{type(self).__name__}_{self.idx}"
 
 
 @dataclasses.dataclass
 class TrainingStateMessage(NerfstudioMessage):
-    """Wheather the scene is in training mode or not."""
+    """Whether the scene is in training mode or not."""
 
     training_state: Literal["training", "paused", "completed"]
-    """True if the model is currently trianing, False otherwise"""
+    """True if the model is currently training, False otherwise"""
 
 
 @dataclasses.dataclass
 class CameraPathPayloadMessage(NerfstudioMessage):
     """Camera path"""
 
     camera_path_filename: str
```

### Comparing `nerfstudio-0.3.1/nerfstudio/viewer/viser/server.py` & `nerfstudio-0.3.2/nerfstudio/viewer/viser/server.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio.egg-info/PKG-INFO` & `nerfstudio-0.3.2/nerfstudio.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nerfstudio
-Version: 0.3.1
+Version: 0.3.2
 Summary: All-in-one repository for state-of-the-art NeRFs
 License: Apache 2.0
 Project-URL: Documentation, https://docs.nerf.studio
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
@@ -306,21 +306,25 @@
 # Citation
 
 You can find a paper writeup of the framework on [arXiv](https://arxiv.org/abs/2302.04264).
 
 If you use this library or find the documentation useful for your research, please consider citing:
 
 ```
-@article{nerfstudio,
-    author = {Tancik, Matthew and Weber, Ethan and Ng, Evonne and Li, Ruilong and Yi,
-            Brent and Kerr, Justin and Wang, Terrance and Kristoffersen, Alexander and Austin,
-            Jake and Salahi, Kamyar and Ahuja, Abhik and McAllister, David and Kanazawa, Angjoo},
-    title = {Nerfstudio: A Modular Framework for Neural Radiance Field Development},
-    journal = {arXiv preprint arXiv:2302.04264},
-    year = {2023},
+@inproceedings{nerfstudio,
+	title        = {Nerfstudio: A Modular Framework for Neural Radiance Field Development},
+	author       = {
+		Tancik, Matthew and Weber, Ethan and Ng, Evonne and Li, Ruilong and Yi, Brent
+		and Kerr, Justin and Wang, Terrance and Kristoffersen, Alexander and Austin,
+		Jake and Salahi, Kamyar and Ahuja, Abhik and McAllister, David and Kanazawa,
+		Angjoo
+	},
+	year         = 2023,
+	booktitle    = {ACM SIGGRAPH 2023 Conference Proceedings},
+	series       = {SIGGRAPH '23}
 }
 ```
 
 # Contributors
 
 <a href="https://github.com/nerfstudio-project/nerfstudio/graphs/contributors">
   <img src="https://contrib.rocks/image?repo=nerfstudio-project/nerfstudio" />
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nerfstudio Version: 0.3.1 Summary: All-in-one
+Metadata-Version: 2.1 Name: nerfstudio Version: 0.3.2 Summary: All-in-one
 repository for state-of-the-art NeRFs License: Apache 2.0 Project-URL:
 Documentation, https://docs.nerf.studio Classifier: Development Status :: 3 -
 Alpha Classifier: Programming Language :: Python Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown Provides-Extra: gen Provides-Extra: dev
 Provides-Extra: docs License-File: LICENSE
  [https://img.shields.io/badge/Join-Discord-blue.svg]  [Documentation_Status]
         [PyPI_version]  [Test_Status] [Viewer_build_Status]  [License]
@@ -185,14 +185,15 @@
 on the Blender dataset - :iphone: Full pipeline support (w/ Colmap, Polycam, or
 Record3D) for going from a video on your phone to a full 3D render. # Built On
 [tyro_logo] - Easy-to-use config system - Developed by [Brent Yi](https://
 brentyi.com/) [tyro_logo] - Library for accelerating NeRF renders - Developed
 by [Ruilong Li](https://www.liruilong.cn/) # Citation You can find a paper
 writeup of the framework on [arXiv](https://arxiv.org/abs/2302.04264). If you
 use this library or find the documentation useful for your research, please
-consider citing: ``` @article{nerfstudio, author = {Tancik, Matthew and Weber,
-Ethan and Ng, Evonne and Li, Ruilong and Yi, Brent and Kerr, Justin and Wang,
-Terrance and Kristoffersen, Alexander and Austin, Jake and Salahi, Kamyar and
-Ahuja, Abhik and McAllister, David and Kanazawa, Angjoo}, title = {Nerfstudio:
-A Modular Framework for Neural Radiance Field Development}, journal = {arXiv
-preprint arXiv:2302.04264}, year = {2023}, } ``` # Contributors [https://
-contrib.rocks/image?repo=nerfstudio-project/nerfstudio]
+consider citing: ``` @inproceedings{nerfstudio, title = {Nerfstudio: A Modular
+Framework for Neural Radiance Field Development}, author = { Tancik, Matthew
+and Weber, Ethan and Ng, Evonne and Li, Ruilong and Yi, Brent and Kerr, Justin
+and Wang, Terrance and Kristoffersen, Alexander and Austin, Jake and Salahi,
+Kamyar and Ahuja, Abhik and McAllister, David and Kanazawa, Angjoo }, year =
+2023, booktitle = {ACM SIGGRAPH 2023 Conference Proceedings}, series =
+{SIGGRAPH '23} } ``` # Contributors [https://contrib.rocks/
+image?repo=nerfstudio-project/nerfstudio]
```

### Comparing `nerfstudio-0.3.1/nerfstudio.egg-info/SOURCES.txt` & `nerfstudio-0.3.2/nerfstudio.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 nerfstudio/configs/external_methods.py
 nerfstudio/configs/method_configs.py
 nerfstudio/data/__init__.py
 nerfstudio/data/pixel_samplers.py
 nerfstudio/data/scene_box.py
 nerfstudio/data/datamanagers/__init__.py
 nerfstudio/data/datamanagers/base_datamanager.py
+nerfstudio/data/datamanagers/random_cameras_datamanager.py
 nerfstudio/data/dataparsers/__init__.py
 nerfstudio/data/dataparsers/arkitscenes_dataparser.py
 nerfstudio/data/dataparsers/base_dataparser.py
 nerfstudio/data/dataparsers/blender_dataparser.py
 nerfstudio/data/dataparsers/dnerf_dataparser.py
 nerfstudio/data/dataparsers/dycheck_dataparser.py
 nerfstudio/data/dataparsers/instant_ngp_dataparser.py
@@ -68,49 +69,45 @@
 nerfstudio/field_components/base_field_component.py
 nerfstudio/field_components/embedding.py
 nerfstudio/field_components/encodings.py
 nerfstudio/field_components/field_heads.py
 nerfstudio/field_components/mlp.py
 nerfstudio/field_components/spatial_distortions.py
 nerfstudio/field_components/temporal_distortions.py
-nerfstudio/field_components/temporal_grid.py
-nerfstudio/field_components/cuda/__init__.py
-nerfstudio/field_components/cuda/_backend.py
-nerfstudio/field_components/cuda/csrc/pybind.cu
-nerfstudio/field_components/cuda/csrc/temporal_gridencoder.cu
 nerfstudio/fields/__init__.py
 nerfstudio/fields/base_field.py
 nerfstudio/fields/density_fields.py
+nerfstudio/fields/generfacto_field.py
 nerfstudio/fields/instant_ngp_field.py
 nerfstudio/fields/nerfacto_field.py
-nerfstudio/fields/nerfplayer_nerfacto_field.py
-nerfstudio/fields/nerfplayer_ngp_field.py
 nerfstudio/fields/nerfw_field.py
 nerfstudio/fields/sdf_field.py
 nerfstudio/fields/semantic_nerf_field.py
 nerfstudio/fields/tensorf_field.py
 nerfstudio/fields/vanilla_nerf_field.py
 nerfstudio/generative/__init__.py
+nerfstudio/generative/deepfloyd.py
+nerfstudio/generative/positional_text_embeddings.py
 nerfstudio/generative/stable_diffusion.py
+nerfstudio/generative/utils.py
 nerfstudio/model_components/__init__.py
 nerfstudio/model_components/losses.py
 nerfstudio/model_components/ray_generators.py
 nerfstudio/model_components/ray_samplers.py
 nerfstudio/model_components/renderers.py
 nerfstudio/model_components/scene_colliders.py
 nerfstudio/model_components/shaders.py
 nerfstudio/models/__init__.py
 nerfstudio/models/base_model.py
 nerfstudio/models/base_surface_model.py
 nerfstudio/models/depth_nerfacto.py
+nerfstudio/models/generfacto.py
 nerfstudio/models/instant_ngp.py
 nerfstudio/models/mipnerf.py
 nerfstudio/models/nerfacto.py
-nerfstudio/models/nerfplayer_nerfacto.py
-nerfstudio/models/nerfplayer_ngp.py
 nerfstudio/models/neus.py
 nerfstudio/models/neus_facto.py
 nerfstudio/models/semantic_nerfw.py
 nerfstudio/models/tensorf.py
 nerfstudio/models/vanilla_nerf.py
 nerfstudio/pipelines/__init__.py
 nerfstudio/pipelines/base_pipeline.py
@@ -192,8 +189,14 @@
 nerfstudio/viewer/server/state/node.py
 nerfstudio/viewer/server/state/state_node.py
 nerfstudio/viewer/viser/__init__.py
 nerfstudio/viewer/viser/gui.py
 nerfstudio/viewer/viser/message_api.py
 nerfstudio/viewer/viser/messages.py
 nerfstudio/viewer/viser/server.py
+nerfstudio/viewer_beta/__init__.py
+nerfstudio/viewer_beta/control_panel.py
+nerfstudio/viewer_beta/render_state_machine.py
+nerfstudio/viewer_beta/utils.py
+nerfstudio/viewer_beta/viewer.py
+nerfstudio/viewer_beta/viewer_elements.py
 tests/test_train.py
```

### Comparing `nerfstudio-0.3.1/nerfstudio.egg-info/entry_points.txt` & `nerfstudio-0.3.2/nerfstudio.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.3.1/nerfstudio.egg-info/requires.txt` & `nerfstudio-0.3.2/nerfstudio.egg-info/requires.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 appdirs>=1.4
 av>=9.2.0
 cryptography>=38
-tyro>=0.3.31
+tyro>=0.5.3
 gdown>=4.6.0
 ninja>=1.10
 h5py>=2.9.0
 imageio>=2.21.1
 ipywidgets>=7.6
 jaxtyping>=0.2.15
 jupyterlab>=3.3.4
@@ -28,15 +28,15 @@
 rich>=12.5.1
 scikit-image>=0.19.3
 tensorboard>=2.13.0
 torch>=1.13.1
 torchvision>=0.14.1
 torchmetrics[image]>=0.9.3
 typing_extensions>=4.4.0
-viser>=0.0.5
+viser>=0.0.12
 nuscenes-devkit>=1.1.1
 wandb>=0.13.3
 xatlas
 trimesh>=3.20.2
 
 [:python_version < "3.10"]
 importlib-metadata>=6.0.0
@@ -45,15 +45,15 @@
 black[jupyter]==23.3.0
 pre-commit==3.3.2
 pytest==7.1.2
 pytest-xdist==2.5.0
 typeguard==2.13.3
 ruff==0.0.267
 sshconf==0.2.5
-pycolmap==0.3.0
+pycolmap>=0.3.0
 diffusers==0.16.1
 opencv-stubs==0.0.7
 transformers==4.29.2
 pyright==1.1.308
 
 [docs]
 furo==2022.09.29
@@ -68,7 +68,10 @@
 sphinx-copybutton==0.5.0
 sphinx-design==0.2.0
 sphinxext-opengraph==0.6.3
 
 [gen]
 diffusers==0.16.1
 transformers==4.29.2
+accelerate==0.19.0
+bitsandbytes==0.39.0
+sentencepiece==0.1.99
```

### Comparing `nerfstudio-0.3.1/pyproject.toml` & `nerfstudio-0.3.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nerfstudio"
-version = "0.3.1"
+version = "0.3.2"
 description = "All-in-one repository for state-of-the-art NeRFs"
 readme = "README.md"
 license = { text="Apache 2.0"}
 requires-python = ">=3.8.0"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python",
 ]
 dependencies = [
     "appdirs>=1.4",
     "av>=9.2.0",
     "cryptography>=38",
-    "tyro>=0.3.31",
+    "tyro>=0.5.3",
     "gdown>=4.6.0",
     "ninja>=1.10",
     "h5py>=2.9.0",
     "imageio>=2.21.1",
     'importlib-metadata>=6.0.0; python_version < "3.10"',
     "ipywidgets>=7.6",
     "jaxtyping>=0.2.15",
@@ -47,15 +47,15 @@
     "rich>=12.5.1",
     "scikit-image>=0.19.3",
     "tensorboard>=2.13.0",
     "torch>=1.13.1",
     "torchvision>=0.14.1",
     "torchmetrics[image]>=0.9.3",
     "typing_extensions>=4.4.0",
-    "viser>=0.0.5",
+    "viser>=0.0.12",
     "nuscenes-devkit>=1.1.1",
     "wandb>=0.13.3",
     "xatlas",
     "trimesh>=3.20.2"
 ]
 
 [project.urls]
@@ -64,27 +64,30 @@
 
 [project.optional-dependencies]
 
 # Generative related dependencies
 gen = [
     "diffusers==0.16.1",
     "transformers==4.29.2",
+    "accelerate==0.19.0",
+    "bitsandbytes==0.39.0",
+    "sentencepiece==0.1.99",
 ]
 
 
 # Development packages
 dev = [
     "black[jupyter]==23.3.0",
     "pre-commit==3.3.2",
     "pytest==7.1.2",
     "pytest-xdist==2.5.0",
     "typeguard==2.13.3",
     "ruff==0.0.267",
     "sshconf==0.2.5",
-    "pycolmap==0.3.0",
+    "pycolmap>=0.3.0",  # NOTE: pycolmap==0.3.0 is not available on newer python versions
     "diffusers==0.16.1",
     "opencv-stubs==0.0.7",
     "transformers==4.29.2",
     "pyright==1.1.308",
 ]
 
 # Documentation related packages
```

### Comparing `nerfstudio-0.3.1/tests/test_train.py` & `nerfstudio-0.3.2/tests/test_train.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,29 +16,31 @@
 from nerfstudio.scripts.train import train_loop
 
 BLACKLIST = [
     "base",
     "semantic-nerfw",
     "instant-ngp",
     "instant-ngp-bounded",
-    "nerfacto",
     "nerfacto-big",
     "volinga",
     "phototourism",
     "depth-nerfacto",
-    "nerfplayer-ngp",
-    "nerfplayer-nerfacto",
     "neus",
+    "generfacto",
     "neus-facto",
 ]
 
 
 def set_reduced_config(config: TrainerConfig):
     """Reducing the config settings to speedup test"""
-    config.machine.num_gpus = 0
+    config.machine.device_type = "cpu"
+    if hasattr(config.pipeline.model, "implementation"):
+        setattr(config.pipeline.model, "implementation", "torch")
+    config.mixed_precision = False
+    config.use_grad_scaler = False
     config.max_num_iterations = 2
     # reduce dataset factors; set dataset to test
     config.pipeline.datamanager.dataparser = BlenderDataParserConfig(data=Path("tests/data/lego_test"))
     config.pipeline.datamanager.train_num_images_to_sample_from = 1
     config.pipeline.datamanager.train_num_rays_per_batch = 4
 
     # use tensorboard logging instead of wandb
```

