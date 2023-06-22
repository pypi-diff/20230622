# Comparing `tmp/geoh5py-0.8.0a2.tar.gz` & `tmp/geoh5py-0.8.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geoh5py-0.8.0a2.tar", max compression
+gzip compressed data, was "geoh5py-0.8.0a3.tar", max compression
```

## Comparing `geoh5py-0.8.0a2.tar` & `geoh5py-0.8.0a3.tar`

### file list

```diff
@@ -1,88 +1,89 @@
--rw-r--r--   0        0        0      841 2023-05-23 20:32:29.218825 geoh5py-0.8.0a2/geoh5py/__init__.py
--rw-r--r--   0        0        0     1486 2023-01-19 16:31:21.807961 geoh5py-0.8.0a2/geoh5py/data/__init__.py
--rw-r--r--   0        0        0     1311 2023-01-19 16:31:21.808963 geoh5py-0.8.0a2/geoh5py/data/blob_data.py
--rw-r--r--   0        0        0     3948 2023-03-23 18:19:17.279345 geoh5py-0.8.0a2/geoh5py/data/color_map.py
--rw-r--r--   0        0        0     8158 2023-05-19 15:54:32.029195 geoh5py-0.8.0a2/geoh5py/data/data.py
--rw-r--r--   0        0        0     1138 2023-01-19 16:31:21.812966 geoh5py-0.8.0a2/geoh5py/data/data_association_enum.py
--rw-r--r--   0        0        0     9612 2023-02-16 17:03:47.933513 geoh5py-0.8.0a2/geoh5py/data/data_type.py
--rw-r--r--   0        0        0     1138 2023-01-19 16:31:21.814488 geoh5py-0.8.0a2/geoh5py/data/data_unit.py
--rw-r--r--   0        0        0     1340 2023-02-07 15:33:21.371480 geoh5py-0.8.0a2/geoh5py/data/datetime_data.py
--rw-r--r--   0        0        0     3690 2023-05-23 20:32:29.220547 geoh5py-0.8.0a2/geoh5py/data/filename_data.py
--rw-r--r--   0        0        0     1218 2023-01-19 16:31:21.818527 geoh5py-0.8.0a2/geoh5py/data/float_data.py
--rw-r--r--   0        0        0     1625 2023-01-19 16:31:21.819552 geoh5py-0.8.0a2/geoh5py/data/geometric_data_constants.py
--rw-r--r--   0        0        0     2415 2023-05-19 15:54:32.031196 geoh5py-0.8.0a2/geoh5py/data/integer_data.py
--rw-r--r--   0        0        0     3473 2023-05-19 15:54:32.032196 geoh5py-0.8.0a2/geoh5py/data/numeric_data.py
--rw-r--r--   0        0        0     1103 2023-01-19 16:31:21.823165 geoh5py-0.8.0a2/geoh5py/data/primitive_type_enum.py
--rw-r--r--   0        0        0     1649 2023-01-19 16:31:21.824214 geoh5py-0.8.0a2/geoh5py/data/reference_value_map.py
--rw-r--r--   0        0        0     1531 2023-01-19 16:31:21.825276 geoh5py-0.8.0a2/geoh5py/data/referenced_data.py
--rw-r--r--   0        0        0     4445 2023-05-19 15:54:32.033195 geoh5py-0.8.0a2/geoh5py/data/text_data.py
--rw-r--r--   0        0        0     1571 2023-01-19 16:31:21.826284 geoh5py-0.8.0a2/geoh5py/data/unknown_data.py
--rw-r--r--   0        0        0     1587 2023-01-19 16:31:21.827538 geoh5py-0.8.0a2/geoh5py/groups/__init__.py
--rw-r--r--   0        0        0     1495 2023-01-19 16:31:21.828547 geoh5py-0.8.0a2/geoh5py/groups/container_group.py
--rw-r--r--   0        0        0     1449 2023-01-19 16:31:21.829603 geoh5py-0.8.0a2/geoh5py/groups/custom_group.py
--rw-r--r--   0        0        0     1851 2023-02-16 17:03:47.936515 geoh5py-0.8.0a2/geoh5py/groups/drillhole_group.py
--rw-r--r--   0        0        0     1498 2023-01-19 16:31:21.833020 geoh5py-0.8.0a2/geoh5py/groups/giftools_group.py
--rw-r--r--   0        0        0     6311 2023-03-27 17:21:08.995642 geoh5py-0.8.0a2/geoh5py/groups/group.py
--rw-r--r--   0        0        0     3698 2023-05-19 15:54:32.034195 geoh5py-0.8.0a2/geoh5py/groups/group_type.py
--rw-r--r--   0        0        0     7362 2023-05-23 20:32:29.222736 geoh5py-0.8.0a2/geoh5py/groups/integrator_group.py
--rw-r--r--   0        0        0     1349 2023-05-23 20:32:29.225255 geoh5py-0.8.0a2/geoh5py/groups/maps_group.py
--rw-r--r--   0        0        0     1468 2023-01-19 16:31:21.839544 geoh5py-0.8.0a2/geoh5py/groups/notype_group.py
--rw-r--r--   0        0        0     4449 2023-02-16 17:03:47.938518 geoh5py-0.8.0a2/geoh5py/groups/property_group.py
--rw-r--r--   0        0        0     1593 2023-01-19 16:31:21.841554 geoh5py-0.8.0a2/geoh5py/groups/root_group.py
--rw-r--r--   0        0        0     2107 2023-05-19 15:54:32.035199 geoh5py-0.8.0a2/geoh5py/groups/simpeg_group.py
--rw-r--r--   0        0        0     1376 2023-05-23 20:32:29.226255 geoh5py-0.8.0a2/geoh5py/groups/survey_group.py
--rw-r--r--   0        0        0      866 2023-01-19 16:31:21.863215 geoh5py-0.8.0a2/geoh5py/io/__init__.py
--rw-r--r--   0        0        0    17088 2023-02-16 17:03:47.939518 geoh5py-0.8.0a2/geoh5py/io/h5_reader.py
--rw-r--r--   0        0        0    32435 2023-05-19 15:54:32.036194 geoh5py-0.8.0a2/geoh5py/io/h5_writer.py
--rw-r--r--   0        0        0     2223 2023-05-15 22:45:01.215418 geoh5py-0.8.0a2/geoh5py/objects/__init__.py
--rw-r--r--   0        0        0     9496 2023-05-19 15:54:32.037194 geoh5py-0.8.0a2/geoh5py/objects/block_model.py
--rw-r--r--   0        0        0     7803 2023-05-19 15:54:32.039194 geoh5py-0.8.0a2/geoh5py/objects/cell_object.py
--rw-r--r--   0        0        0     6283 2023-05-19 15:54:32.040193 geoh5py-0.8.0a2/geoh5py/objects/curve.py
--rw-r--r--   0        0        0     5129 2023-05-19 15:54:32.041196 geoh5py-0.8.0a2/geoh5py/objects/drape_model.py
--rw-r--r--   0        0        0    25527 2023-05-19 15:54:32.042194 geoh5py-0.8.0a2/geoh5py/objects/drillhole.py
--rw-r--r--   0        0        0    19521 2023-05-23 20:32:29.228772 geoh5py-0.8.0a2/geoh5py/objects/geo_image.py
--rw-r--r--   0        0        0    14068 2023-05-19 15:54:32.045197 geoh5py-0.8.0a2/geoh5py/objects/grid2d.py
--rw-r--r--   0        0        0     4775 2023-05-19 15:54:32.046194 geoh5py-0.8.0a2/geoh5py/objects/grid_object.py
--rw-r--r--   0        0        0     1957 2023-05-23 20:32:29.230772 geoh5py-0.8.0a2/geoh5py/objects/integrator.py
--rw-r--r--   0        0        0     2977 2023-03-23 18:19:17.298881 geoh5py-0.8.0a2/geoh5py/objects/label.py
--rw-r--r--   0        0        0     2890 2023-03-23 18:19:17.302902 geoh5py-0.8.0a2/geoh5py/objects/notype_object.py
--rw-r--r--   0        0        0    17763 2023-05-19 15:54:32.048200 geoh5py-0.8.0a2/geoh5py/objects/object_base.py
--rw-r--r--   0        0        0     2748 2023-05-19 15:54:32.049219 geoh5py-0.8.0a2/geoh5py/objects/object_type.py
--rw-r--r--   0        0        0    13349 2023-05-19 15:54:32.050215 geoh5py-0.8.0a2/geoh5py/objects/octree.py
--rw-r--r--   0        0        0     5410 2023-05-19 15:54:32.051194 geoh5py-0.8.0a2/geoh5py/objects/points.py
--rw-r--r--   0        0        0     2588 2023-05-19 15:54:32.052205 geoh5py-0.8.0a2/geoh5py/objects/surface.py
--rw-r--r--   0        0        0      747 2023-01-19 16:31:21.887120 geoh5py-0.8.0a2/geoh5py/objects/surveys/__init__.py
--rw-r--r--   0        0        0    14570 2023-05-19 15:54:32.054194 geoh5py-0.8.0a2/geoh5py/objects/surveys/direct_current.py
--rw-r--r--   0        0        0      747 2023-01-19 16:31:21.889161 geoh5py-0.8.0a2/geoh5py/objects/surveys/electromagnetics/__init__.py
--rw-r--r--   0        0        0     3660 2023-05-15 22:45:01.218421 geoh5py-0.8.0a2/geoh5py/objects/surveys/electromagnetics/airborne_fem.py
--rw-r--r--   0        0        0     3629 2023-05-15 22:45:01.219419 geoh5py-0.8.0a2/geoh5py/objects/surveys/electromagnetics/airborne_tem.py
--rw-r--r--   0        0        0    35608 2023-05-19 15:54:32.055195 geoh5py-0.8.0a2/geoh5py/objects/surveys/electromagnetics/base.py
--rw-r--r--   0        0        0     6925 2023-05-15 22:45:01.221455 geoh5py-0.8.0a2/geoh5py/objects/surveys/electromagnetics/ground_fem.py
--rw-r--r--   0        0        0     7019 2023-05-15 22:45:01.222420 geoh5py-0.8.0a2/geoh5py/objects/surveys/electromagnetics/ground_tem.py
--rw-r--r--   0        0        0     2615 2023-05-15 22:45:01.223419 geoh5py-0.8.0a2/geoh5py/objects/surveys/electromagnetics/magnetotellurics.py
--rw-r--r--   0        0        0     6636 2023-05-19 15:54:32.057196 geoh5py-0.8.0a2/geoh5py/objects/surveys/electromagnetics/tipper.py
--rw-r--r--   0        0        0     1247 2023-01-19 16:31:21.895750 geoh5py-0.8.0a2/geoh5py/objects/surveys/magnetics.py
--rw-r--r--   0        0        0        0 2023-03-17 04:10:56.051740 geoh5py-0.8.0a2/geoh5py/py.typed
--rw-r--r--   0        0        0     1015 2023-01-19 16:31:21.897759 geoh5py-0.8.0a2/geoh5py/shared/__init__.py
--rw-r--r--   0        0        0    37812 2023-05-19 15:54:32.058200 geoh5py-0.8.0a2/geoh5py/shared/concatenation.py
--rw-r--r--   0        0        0      937 2023-02-06 21:13:48.440256 geoh5py-0.8.0a2/geoh5py/shared/conversion/__init__.py
--rw-r--r--   0        0        0     4287 2023-05-19 15:54:32.060201 geoh5py-0.8.0a2/geoh5py/shared/conversion/base.py
--rw-r--r--   0        0        0     7599 2023-02-06 21:13:48.440256 geoh5py-0.8.0a2/geoh5py/shared/conversion/geo_image.py
--rw-r--r--   0        0        0     8083 2023-03-14 13:51:22.342790 geoh5py-0.8.0a2/geoh5py/shared/conversion/grid2d.py
--rw-r--r--   0        0        0    16884 2023-05-23 20:32:29.232772 geoh5py-0.8.0a2/geoh5py/shared/entity.py
--rw-r--r--   0        0        0     4275 2023-02-16 17:03:47.959277 geoh5py-0.8.0a2/geoh5py/shared/entity_type.py
--rw-r--r--   0        0        0     5732 2023-03-14 13:51:22.344785 geoh5py-0.8.0a2/geoh5py/shared/exceptions.py
--rw-r--r--   0        0        0    15205 2023-05-19 15:54:32.062638 geoh5py-0.8.0a2/geoh5py/shared/utils.py
--rw-r--r--   0        0        0     8969 2023-05-23 20:32:29.234775 geoh5py-0.8.0a2/geoh5py/shared/validators.py
--rw-r--r--   0        0        0     2647 2023-01-19 16:31:21.906283 geoh5py-0.8.0a2/geoh5py/shared/weakref_utils.py
--rw-r--r--   0        0        0      921 2023-01-19 16:31:21.907291 geoh5py-0.8.0a2/geoh5py/ui_json/__init__.py
--rw-r--r--   0        0        0     2980 2023-05-23 20:32:29.236772 geoh5py-0.8.0a2/geoh5py/ui_json/constants.py
--rw-r--r--   0        0        0    18369 2023-05-23 20:32:29.238776 geoh5py-0.8.0a2/geoh5py/ui_json/input_file.py
--rw-r--r--   0        0        0    11946 2023-05-15 22:45:01.229425 geoh5py-0.8.0a2/geoh5py/ui_json/templates.py
--rw-r--r--   0        0        0    11110 2023-05-23 20:32:29.240784 geoh5py-0.8.0a2/geoh5py/ui_json/utils.py
--rw-r--r--   0        0        0    10777 2023-05-15 22:45:01.231421 geoh5py-0.8.0a2/geoh5py/ui_json/validation.py
--rw-r--r--   0        0        0      852 2023-01-19 16:31:21.913295 geoh5py-0.8.0a2/geoh5py/workspace/__init__.py
--rw-r--r--   0        0        0    42575 2023-05-23 20:32:29.242774 geoh5py-0.8.0a2/geoh5py/workspace/workspace.py
--rw-r--r--   0        0        0     2111 2023-01-19 16:31:21.916738 geoh5py-0.8.0a2/package.rst
--rw-r--r--   0        0        0     2501 2023-05-23 20:32:29.249771 geoh5py-0.8.0a2/pyproject.toml
--rw-r--r--   0        0        0     3419 1970-01-01 00:00:00.000000 geoh5py-0.8.0a2/PKG-INFO
+-rw-r--r--   0        0        0      841 2023-06-22 20:51:16.615969 geoh5py-0.8.0a3/geoh5py/__init__.py
+-rw-r--r--   0        0        0     1535 2023-06-22 20:37:45.966145 geoh5py-0.8.0a3/geoh5py/data/__init__.py
+-rw-r--r--   0        0        0     1311 2023-01-27 16:07:08.405036 geoh5py-0.8.0a3/geoh5py/data/blob_data.py
+-rw-r--r--   0        0        0     3948 2023-05-16 13:39:30.019323 geoh5py-0.8.0a3/geoh5py/data/color_map.py
+-rw-r--r--   0        0        0     8319 2023-06-22 20:37:45.967146 geoh5py-0.8.0a3/geoh5py/data/data.py
+-rw-r--r--   0        0        0     1138 2023-01-27 16:07:08.407026 geoh5py-0.8.0a3/geoh5py/data/data_association_enum.py
+-rw-r--r--   0        0        0     9612 2023-05-16 13:39:30.020323 geoh5py-0.8.0a3/geoh5py/data/data_type.py
+-rw-r--r--   0        0        0     1138 2023-01-27 16:07:08.408028 geoh5py-0.8.0a3/geoh5py/data/data_unit.py
+-rw-r--r--   0        0        0     1340 2023-05-16 13:39:30.020323 geoh5py-0.8.0a3/geoh5py/data/datetime_data.py
+-rw-r--r--   0        0        0     3690 2023-06-22 20:36:07.203044 geoh5py-0.8.0a3/geoh5py/data/filename_data.py
+-rw-r--r--   0        0        0     1218 2023-01-27 16:07:08.410027 geoh5py-0.8.0a3/geoh5py/data/float_data.py
+-rw-r--r--   0        0        0     1625 2023-01-27 16:07:08.411061 geoh5py-0.8.0a3/geoh5py/data/geometric_data_constants.py
+-rw-r--r--   0        0        0     2415 2023-01-27 16:07:08.412062 geoh5py-0.8.0a3/geoh5py/data/integer_data.py
+-rw-r--r--   0        0        0     3473 2023-06-22 20:36:07.204033 geoh5py-0.8.0a3/geoh5py/data/numeric_data.py
+-rw-r--r--   0        0        0     1103 2023-01-27 16:07:08.413026 geoh5py-0.8.0a3/geoh5py/data/primitive_type_enum.py
+-rw-r--r--   0        0        0     1649 2023-01-27 16:07:08.413026 geoh5py-0.8.0a3/geoh5py/data/reference_value_map.py
+-rw-r--r--   0        0        0     1531 2023-01-27 16:07:08.414026 geoh5py-0.8.0a3/geoh5py/data/referenced_data.py
+-rw-r--r--   0        0        0     4445 2023-05-16 13:39:30.022336 geoh5py-0.8.0a3/geoh5py/data/text_data.py
+-rw-r--r--   0        0        0     1571 2023-01-27 16:07:08.415027 geoh5py-0.8.0a3/geoh5py/data/unknown_data.py
+-rw-r--r--   0        0        0     4590 2023-06-22 20:37:45.967146 geoh5py-0.8.0a3/geoh5py/data/visual_parameters.py
+-rw-r--r--   0        0        0     1587 2023-01-27 16:07:08.416026 geoh5py-0.8.0a3/geoh5py/groups/__init__.py
+-rw-r--r--   0        0        0     1495 2023-01-27 16:07:08.416026 geoh5py-0.8.0a3/geoh5py/groups/container_group.py
+-rw-r--r--   0        0        0     1449 2023-01-27 16:07:08.416026 geoh5py-0.8.0a3/geoh5py/groups/custom_group.py
+-rw-r--r--   0        0        0     1851 2023-05-16 13:39:30.023336 geoh5py-0.8.0a3/geoh5py/groups/drillhole_group.py
+-rw-r--r--   0        0        0     1498 2023-01-27 16:07:08.417027 geoh5py-0.8.0a3/geoh5py/groups/giftools_group.py
+-rw-r--r--   0        0        0     6311 2023-05-16 13:39:30.023336 geoh5py-0.8.0a3/geoh5py/groups/group.py
+-rw-r--r--   0        0        0     3698 2023-01-27 16:07:08.418027 geoh5py-0.8.0a3/geoh5py/groups/group_type.py
+-rw-r--r--   0        0        0     7362 2023-06-22 20:36:07.204033 geoh5py-0.8.0a3/geoh5py/groups/integrator_group.py
+-rw-r--r--   0        0        0     1349 2023-06-22 20:36:07.204033 geoh5py-0.8.0a3/geoh5py/groups/maps_group.py
+-rw-r--r--   0        0        0     1468 2023-01-27 16:07:08.420026 geoh5py-0.8.0a3/geoh5py/groups/notype_group.py
+-rw-r--r--   0        0        0     4449 2023-05-16 13:39:30.024337 geoh5py-0.8.0a3/geoh5py/groups/property_group.py
+-rw-r--r--   0        0        0     1593 2023-01-27 16:07:08.421026 geoh5py-0.8.0a3/geoh5py/groups/root_group.py
+-rw-r--r--   0        0        0     2107 2023-06-22 20:36:07.204033 geoh5py-0.8.0a3/geoh5py/groups/simpeg_group.py
+-rw-r--r--   0        0        0     1376 2023-06-22 20:36:07.204033 geoh5py-0.8.0a3/geoh5py/groups/survey_group.py
+-rw-r--r--   0        0        0      866 2023-01-27 16:07:08.429046 geoh5py-0.8.0a3/geoh5py/io/__init__.py
+-rw-r--r--   0        0        0    17088 2023-05-16 13:39:30.025336 geoh5py-0.8.0a3/geoh5py/io/h5_reader.py
+-rw-r--r--   0        0        0    32422 2023-06-22 20:37:45.967146 geoh5py-0.8.0a3/geoh5py/io/h5_writer.py
+-rw-r--r--   0        0        0     2223 2023-06-22 20:36:07.204033 geoh5py-0.8.0a3/geoh5py/objects/__init__.py
+-rw-r--r--   0        0        0     9496 2023-05-16 13:39:30.026336 geoh5py-0.8.0a3/geoh5py/objects/block_model.py
+-rw-r--r--   0        0        0     7803 2023-05-16 13:39:30.026336 geoh5py-0.8.0a3/geoh5py/objects/cell_object.py
+-rw-r--r--   0        0        0     6283 2023-05-16 13:39:30.027335 geoh5py-0.8.0a3/geoh5py/objects/curve.py
+-rw-r--r--   0        0        0     5129 2023-05-16 13:39:30.027335 geoh5py-0.8.0a3/geoh5py/objects/drape_model.py
+-rw-r--r--   0        0        0    25527 2023-05-16 13:39:30.028335 geoh5py-0.8.0a3/geoh5py/objects/drillhole.py
+-rw-r--r--   0        0        0    19521 2023-06-22 20:36:07.204033 geoh5py-0.8.0a3/geoh5py/objects/geo_image.py
+-rw-r--r--   0        0        0    14068 2023-06-22 20:36:07.204033 geoh5py-0.8.0a3/geoh5py/objects/grid2d.py
+-rw-r--r--   0        0        0     4775 2023-05-16 13:39:30.030336 geoh5py-0.8.0a3/geoh5py/objects/grid_object.py
+-rw-r--r--   0        0        0     1957 2023-06-22 20:36:07.204033 geoh5py-0.8.0a3/geoh5py/objects/integrator.py
+-rw-r--r--   0        0        0     2977 2023-05-16 13:39:30.031335 geoh5py-0.8.0a3/geoh5py/objects/label.py
+-rw-r--r--   0        0        0     2890 2023-05-16 13:39:30.031335 geoh5py-0.8.0a3/geoh5py/objects/notype_object.py
+-rw-r--r--   0        0        0    19243 2023-06-22 20:37:45.968145 geoh5py-0.8.0a3/geoh5py/objects/object_base.py
+-rw-r--r--   0        0        0     2748 2023-01-27 16:07:08.438024 geoh5py-0.8.0a3/geoh5py/objects/object_type.py
+-rw-r--r--   0        0        0    13349 2023-05-16 13:39:30.032335 geoh5py-0.8.0a3/geoh5py/objects/octree.py
+-rw-r--r--   0        0        0     5410 2023-05-16 13:39:30.032335 geoh5py-0.8.0a3/geoh5py/objects/points.py
+-rw-r--r--   0        0        0     2588 2023-05-16 13:39:30.033336 geoh5py-0.8.0a3/geoh5py/objects/surface.py
+-rw-r--r--   0        0        0      747 2023-01-27 16:07:08.440024 geoh5py-0.8.0a3/geoh5py/objects/surveys/__init__.py
+-rw-r--r--   0        0        0    14570 2023-05-16 13:39:30.033336 geoh5py-0.8.0a3/geoh5py/objects/surveys/direct_current.py
+-rw-r--r--   0        0        0      747 2023-01-27 16:07:08.441024 geoh5py-0.8.0a3/geoh5py/objects/surveys/electromagnetics/__init__.py
+-rw-r--r--   0        0        0     3660 2023-06-22 20:36:07.204033 geoh5py-0.8.0a3/geoh5py/objects/surveys/electromagnetics/airborne_fem.py
+-rw-r--r--   0        0        0     3629 2023-06-22 20:36:07.204033 geoh5py-0.8.0a3/geoh5py/objects/surveys/electromagnetics/airborne_tem.py
+-rw-r--r--   0        0        0    35454 2023-06-22 20:37:45.969152 geoh5py-0.8.0a3/geoh5py/objects/surveys/electromagnetics/base.py
+-rw-r--r--   0        0        0     6925 2023-06-22 20:36:07.211568 geoh5py-0.8.0a3/geoh5py/objects/surveys/electromagnetics/ground_fem.py
+-rw-r--r--   0        0        0     7019 2023-06-22 20:36:07.212080 geoh5py-0.8.0a3/geoh5py/objects/surveys/electromagnetics/ground_tem.py
+-rw-r--r--   0        0        0     2615 2023-06-22 20:36:07.212080 geoh5py-0.8.0a3/geoh5py/objects/surveys/electromagnetics/magnetotellurics.py
+-rw-r--r--   0        0        0     6636 2023-06-22 20:36:07.212080 geoh5py-0.8.0a3/geoh5py/objects/surveys/electromagnetics/tipper.py
+-rw-r--r--   0        0        0     1247 2023-01-27 16:07:08.443024 geoh5py-0.8.0a3/geoh5py/objects/surveys/magnetics.py
+-rw-r--r--   0        0        0        0 2023-05-16 13:39:30.036442 geoh5py-0.8.0a3/geoh5py/py.typed
+-rw-r--r--   0        0        0     1015 2023-01-27 16:07:08.444702 geoh5py-0.8.0a3/geoh5py/shared/__init__.py
+-rw-r--r--   0        0        0    37812 2023-05-16 13:39:30.037925 geoh5py-0.8.0a3/geoh5py/shared/concatenation.py
+-rw-r--r--   0        0        0      937 2023-01-27 16:07:08.446085 geoh5py-0.8.0a3/geoh5py/shared/conversion/__init__.py
+-rw-r--r--   0        0        0     4287 2023-01-27 16:07:08.446085 geoh5py-0.8.0a3/geoh5py/shared/conversion/base.py
+-rw-r--r--   0        0        0     7599 2023-01-27 16:07:08.446085 geoh5py-0.8.0a3/geoh5py/shared/conversion/geo_image.py
+-rw-r--r--   0        0        0     8083 2023-05-16 13:39:30.038443 geoh5py-0.8.0a3/geoh5py/shared/conversion/grid2d.py
+-rw-r--r--   0        0        0    16876 2023-06-22 20:37:45.969152 geoh5py-0.8.0a3/geoh5py/shared/entity.py
+-rw-r--r--   0        0        0     4275 2023-05-16 13:39:30.038443 geoh5py-0.8.0a3/geoh5py/shared/entity_type.py
+-rw-r--r--   0        0        0     5732 2023-05-16 13:39:30.039442 geoh5py-0.8.0a3/geoh5py/shared/exceptions.py
+-rw-r--r--   0        0        0    15323 2023-06-22 20:37:45.969152 geoh5py-0.8.0a3/geoh5py/shared/utils.py
+-rw-r--r--   0        0        0     9023 2023-06-22 20:36:07.213513 geoh5py-0.8.0a3/geoh5py/shared/validators.py
+-rw-r--r--   0        0        0     2647 2023-01-27 16:07:08.451084 geoh5py-0.8.0a3/geoh5py/shared/weakref_utils.py
+-rw-r--r--   0        0        0      921 2023-01-27 16:07:08.452070 geoh5py-0.8.0a3/geoh5py/ui_json/__init__.py
+-rw-r--r--   0        0        0     2980 2023-06-22 20:36:07.213513 geoh5py-0.8.0a3/geoh5py/ui_json/constants.py
+-rw-r--r--   0        0        0    18044 2023-06-22 20:36:07.213513 geoh5py-0.8.0a3/geoh5py/ui_json/input_file.py
+-rw-r--r--   0        0        0    11946 2023-06-22 20:36:07.213513 geoh5py-0.8.0a3/geoh5py/ui_json/templates.py
+-rw-r--r--   0        0        0    11117 2023-06-22 20:37:45.970146 geoh5py-0.8.0a3/geoh5py/ui_json/utils.py
+-rw-r--r--   0        0        0    10777 2023-06-22 20:36:07.213513 geoh5py-0.8.0a3/geoh5py/ui_json/validation.py
+-rw-r--r--   0        0        0      852 2023-01-27 16:07:08.455078 geoh5py-0.8.0a3/geoh5py/workspace/__init__.py
+-rw-r--r--   0        0        0    46010 2023-06-22 20:37:45.971145 geoh5py-0.8.0a3/geoh5py/workspace/workspace.py
+-rw-r--r--   0        0        0     2111 2023-01-27 16:07:08.456070 geoh5py-0.8.0a3/package.rst
+-rw-r--r--   0        0        0     2218 2023-06-22 20:51:16.620983 geoh5py-0.8.0a3/pyproject.toml
+-rw-r--r--   0        0        0     3419 1970-01-01 00:00:00.000000 geoh5py-0.8.0a3/PKG-INFO
```

### Comparing `geoh5py-0.8.0a2/geoh5py/__init__.py` & `geoh5py-0.8.0a3/geoh5py/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,10 +13,10 @@
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with geoh5py.  If not, see <https://www.gnu.org/licenses/>.
 
 # flake8: noqa
 
-__version__ = "0.8.0-alpha.2"
+__version__ = "0.8.0-alpha.3"
 
 from geoh5py.workspace import Workspace
```

### Comparing `geoh5py-0.8.0a2/geoh5py/data/__init__.py` & `geoh5py-0.8.0a3/geoh5py/data/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,7 +30,8 @@
 from .integer_data import IntegerData
 from .numeric_data import NumericData
 from .primitive_type_enum import PrimitiveTypeEnum
 from .reference_value_map import ReferenceValueMap
 from .referenced_data import ReferencedData
 from .text_data import CommentsData, MultiTextData, TextData
 from .unknown_data import UnknownData
+from .visual_parameters import VisualParameters
```

### Comparing `geoh5py-0.8.0a2/geoh5py/data/blob_data.py` & `geoh5py-0.8.0a3/geoh5py/data/blob_data.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a2/geoh5py/data/color_map.py` & `geoh5py-0.8.0a3/geoh5py/data/color_map.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a2/geoh5py/data/data.py` & `geoh5py-0.8.0a3/geoh5py/data/data.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,16 +42,23 @@
         self,
         data_type: DataType,
         **kwargs,
     ):
         self._association = None
         self._on_file = False
         self._modifiable = True
-        assert data_type is not None
-        assert data_type.primitive_type == self.primitive_type()
+
+        if (
+            not isinstance(data_type, DataType)
+            or data_type.primitive_type != self.primitive_type()
+        ):
+            raise TypeError(
+                "Input 'data_type' must be a DataType object of primitive_type 'TEXT'."
+            )
+
         self.entity_type = data_type
         self._values = None
 
         super().__init__(**kwargs)
 
         if self.entity_type.name == "Entity":
             self.entity_type.name = self.name
@@ -116,15 +123,15 @@
     def extent(self) -> np.ndarray | None:
         """
         Geography bounding box of the parent object.
 
         :return: shape(2, 3) Bounding box defined by the bottom South-West and
             top North-East coordinates.
         """
-        return self.parent.extent
+        return None
 
     @property
     def n_values(self) -> int | None:
         """
         :obj:`int`: Number of expected data values based on
         :obj:`~geoh5py.data.data.Data.association`
         """
```

### Comparing `geoh5py-0.8.0a2/geoh5py/data/data_association_enum.py` & `geoh5py-0.8.0a3/geoh5py/data/data_association_enum.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a2/geoh5py/data/data_type.py` & `geoh5py-0.8.0a3/geoh5py/data/data_type.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a2/geoh5py/data/data_unit.py` & `geoh5py-0.8.0a3/geoh5py/data/data_unit.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a2/geoh5py/data/datetime_data.py` & `geoh5py-0.8.0a3/geoh5py/data/datetime_data.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a2/geoh5py/data/filename_data.py` & `geoh5py-0.8.0a3/geoh5py/data/filename_data.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a2/geoh5py/data/float_data.py` & `geoh5py-0.8.0a3/geoh5py/data/float_data.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a2/geoh5py/data/geometric_data_constants.py` & `geoh5py-0.8.0a3/geoh5py/data/geometric_data_constants.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a2/geoh5py/data/integer_data.py` & `geoh5py-0.8.0a3/geoh5py/data/integer_data.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a2/geoh5py/data/numeric_data.py` & `geoh5py-0.8.0a3/geoh5py/data/numeric_data.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a2/geoh5py/data/primitive_type_enum.py` & `geoh5py-0.8.0a3/geoh5py/data/primitive_type_enum.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a2/geoh5py/data/reference_value_map.py` & `geoh5py-0.8.0a3/geoh5py/data/reference_value_map.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a2/geoh5py/data/referenced_data.py` & `geoh5py-0.8.0a3/geoh5py/data/referenced_data.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a2/geoh5py/data/text_data.py` & `geoh5py-0.8.0a3/geoh5py/data/text_data.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a2/geoh5py/data/unknown_data.py` & `geoh5py-0.8.0a3/geoh5py/data/unknown_data.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a2/geoh5py/groups/__init__.py` & `geoh5py-0.8.0a3/geoh5py/groups/__init__.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a2/geoh5py/groups/container_group.py` & `geoh5py-0.8.0a3/geoh5py/groups/container_group.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a2/geoh5py/groups/custom_group.py` & `geoh5py-0.8.0a3/geoh5py/groups/custom_group.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a2/geoh5py/groups/drillhole_group.py` & `geoh5py-0.8.0a3/geoh5py/groups/drillhole_group.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a2/geoh5py/groups/giftools_group.py` & `geoh5py-0.8.0a3/geoh5py/groups/giftools_group.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a2/geoh5py/groups/group.py` & `geoh5py-0.8.0a3/geoh5py/groups/group.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a2/geoh5py/groups/group_type.py` & `geoh5py-0.8.0a3/geoh5py/groups/group_type.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a2/geoh5py/groups/integrator_group.py` & `geoh5py-0.8.0a3/geoh5py/groups/integrator_group.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a2/geoh5py/groups/maps_group.py` & `geoh5py-0.8.0a3/geoh5py/groups/maps_group.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a2/geoh5py/groups/notype_group.py` & `geoh5py-0.8.0a3/geoh5py/groups/notype_group.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a2/geoh5py/groups/property_group.py` & `geoh5py-0.8.0a3/geoh5py/groups/property_group.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a2/geoh5py/groups/root_group.py` & `geoh5py-0.8.0a3/geoh5py/groups/root_group.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a2/geoh5py/groups/simpeg_group.py` & `geoh5py-0.8.0a3/geoh5py/groups/simpeg_group.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a2/geoh5py/groups/survey_group.py` & `geoh5py-0.8.0a3/geoh5py/groups/survey_group.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a2/geoh5py/io/__init__.py` & `geoh5py-0.8.0a3/geoh5py/io/__init__.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a2/geoh5py/io/h5_reader.py` & `geoh5py-0.8.0a3/geoh5py/io/h5_reader.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a2/geoh5py/io/h5_writer.py` & `geoh5py-0.8.0a3/geoh5py/io/h5_writer.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     """
     Writing class to a geoh5 file.
     """
 
     str_type = h5py.special_dtype(vlen=str)
 
     @classmethod
-    def create_geoh5(
+    def init_geoh5(
         cls,
         file: str | h5py.File,
         workspace: workspace.Workspace,
     ):
         """
         Add the geoh5 core structure.
 
@@ -206,31 +206,30 @@
     def save_entity(
         cls,
         file: str | h5py.File,
         entity,
         add_children: bool = True,
     ) -> h5py.Group:
         """
-        Write an :obj:`~geoh5py.shared.entity.Entity` to geoh5 with its
-        :obj:`~geoh5py.shared.entity.Entity.children`.
+        Save a :obj:`~geoh5py.shared.entity.Entity` to geoh5 with its
+        :obj:`~geoh5py.shared.entity.Entity.children` recursively.
 
         :param file: Name or handle to a geoh5 file.
         :param entity: Target :obj:`~geoh5py.shared.entity.Entity`.
         :param add_children: Add :obj:`~geoh5py.shared.entity.Entity.children`.
         """
         with fetch_h5_handle(file, mode="r+") as h5file:
             new_entity = H5Writer.write_entity(h5file, entity)
 
-            if add_children:
+            if add_children and not isinstance(entity, Concatenator):
                 # Write children entities and add to current parent
                 for child in entity.children:
-                    H5Writer.write_entity(h5file, child)
-                    H5Writer.write_to_parent(h5file, child, recursively=False)
+                    H5Writer.save_entity(h5file, child)
 
-            H5Writer.write_to_parent(h5file, entity)
+            H5Writer.write_to_parent(h5file, entity, recursively=False)
 
         return new_entity
 
     @classmethod
     def update_concatenated_field(
         cls, file: str | h5py.File, entity, attribute: str, channel: str
     ) -> None:
```

### Comparing `geoh5py-0.8.0a2/geoh5py/objects/__init__.py` & `geoh5py-0.8.0a3/geoh5py/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a2/geoh5py/objects/block_model.py` & `geoh5py-0.8.0a3/geoh5py/objects/block_model.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a2/geoh5py/objects/cell_object.py` & `geoh5py-0.8.0a3/geoh5py/objects/cell_object.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a2/geoh5py/objects/curve.py` & `geoh5py-0.8.0a3/geoh5py/objects/curve.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a2/geoh5py/objects/drape_model.py` & `geoh5py-0.8.0a3/geoh5py/objects/drape_model.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a2/geoh5py/objects/drillhole.py` & `geoh5py-0.8.0a3/geoh5py/objects/drillhole.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a2/geoh5py/objects/geo_image.py` & `geoh5py-0.8.0a3/geoh5py/objects/geo_image.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a2/geoh5py/objects/grid2d.py` & `geoh5py-0.8.0a3/geoh5py/objects/grid2d.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a2/geoh5py/objects/grid_object.py` & `geoh5py-0.8.0a3/geoh5py/objects/grid_object.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a2/geoh5py/objects/integrator.py` & `geoh5py-0.8.0a3/geoh5py/objects/integrator.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a2/geoh5py/objects/label.py` & `geoh5py-0.8.0a3/geoh5py/objects/label.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a2/geoh5py/objects/notype_object.py` & `geoh5py-0.8.0a3/geoh5py/objects/notype_object.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a2/geoh5py/objects/object_base.py` & `geoh5py-0.8.0a3/geoh5py/objects/object_base.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 import uuid
 from abc import abstractmethod
 from datetime import datetime
 from typing import TYPE_CHECKING
 
 import numpy as np
 
-from ..data import CommentsData, Data
+from ..data import CommentsData, Data, VisualParameters
 from ..data.data_association_enum import DataAssociationEnum
 from ..data.primitive_type_enum import PrimitiveTypeEnum
 from ..groups import PropertyGroup
 from ..shared import Entity
 from ..shared.conversion import BaseConversion
 from ..shared.utils import clear_array_attributes
 from .object_type import ObjectType
@@ -53,14 +53,15 @@
     def __init__(self, object_type: ObjectType, **kwargs):
         assert object_type is not None
         self._comments = None
         self._entity_type = object_type
         self._last_focus = "None"
         self._property_groups: list[PropertyGroup] | None = None
         # self._clipping_ids: list[uuid.UUID] = []
+        self._visual_parameters: VisualParameters | None = None
 
         if not any(key for key in kwargs if key in ["name", "Name"]):
             kwargs["name"] = type(self).__name__
 
         super().__init__(**kwargs)
 
         if self.entity_type.name == "Entity":
@@ -521,7 +522,49 @@
                     entity_type = {"primitive_type": "TEXT"}
                 else:
                     raise NotImplementedError(
                         "Only add_data values of type FLOAT, INTEGER and TEXT have been implemented"
                     )
 
         return entity_type
+
+    def add_default_visual_parameters(self):
+        """
+        Add default visual parameters to the object.
+        """
+        if self.visual_parameters is not None:
+            raise UserWarning("Visual parameters already exist.")
+
+        self.workspace.create_entity(  # type: ignore
+            Data,
+            save_on_creation=True,
+            **{
+                "entity": {
+                    "name": "Visual Parameters",
+                    "parent": self,
+                    "association": "OBJECT",
+                },
+                "entity_type": {"name": "XmlData", "primitive_type": "TEXT"},
+            },
+        )
+
+        return self._visual_parameters
+
+    @property
+    def visual_parameters(self) -> VisualParameters | None:
+        """
+        Access the visual parameters of the object.
+        """
+        if self._visual_parameters is None:
+            for child in self.children:
+                if isinstance(child, VisualParameters):
+                    self._visual_parameters = child
+                    break
+
+        return self._visual_parameters
+
+    @visual_parameters.setter
+    def visual_parameters(self, value: VisualParameters):
+        if not isinstance(value, VisualParameters):
+            raise TypeError("visual_parameters must be a VisualParameters object.")
+
+        self._visual_parameters = value
```

### Comparing `geoh5py-0.8.0a2/geoh5py/objects/object_type.py` & `geoh5py-0.8.0a3/geoh5py/objects/object_type.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a2/geoh5py/objects/octree.py` & `geoh5py-0.8.0a3/geoh5py/objects/octree.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a2/geoh5py/objects/points.py` & `geoh5py-0.8.0a3/geoh5py/objects/points.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a2/geoh5py/objects/surface.py` & `geoh5py-0.8.0a3/geoh5py/objects/surface.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a2/geoh5py/objects/surveys/__init__.py` & `geoh5py-0.8.0a3/geoh5py/objects/surveys/__init__.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a2/geoh5py/objects/surveys/direct_current.py` & `geoh5py-0.8.0a3/geoh5py/objects/surveys/direct_current.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a2/geoh5py/objects/surveys/electromagnetics/__init__.py` & `geoh5py-0.8.0a3/geoh5py/objects/surveys/electromagnetics/__init__.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a2/geoh5py/objects/surveys/electromagnetics/airborne_fem.py` & `geoh5py-0.8.0a3/geoh5py/objects/surveys/electromagnetics/airborne_fem.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a2/geoh5py/objects/surveys/electromagnetics/airborne_tem.py` & `geoh5py-0.8.0a3/geoh5py/objects/surveys/electromagnetics/airborne_tem.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a2/geoh5py/objects/surveys/electromagnetics/base.py` & `geoh5py-0.8.0a3/geoh5py/objects/surveys/electromagnetics/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -579,15 +579,15 @@
             "_metadata",
             "_receivers",
             "_transmitters",
             "_base_stations",
             "_tx_id_property",
         ]
         kwargs["omit_list"] = omit_list
-        metadata = self.metadata.copy()
+
         new_entity = super().copy(
             parent=parent,
             clear_cache=clear_cache,
             copy_children=copy_children,
             mask=mask,
             cell_mask=cell_mask,
             apply_to_complement=False,
@@ -605,15 +605,14 @@
                     cell_mask = mask
                 else:
                     cell_mask = np.all(mask[self.cells], axis=1)
             else:
                 cell_mask = np.ones(self.tx_id_property.values.shape[0], dtype=bool)
 
             new_entity.tx_id_property = self.tx_id_property.values[cell_mask]
-        metadata["EM Dataset"][new_entity.type] = new_entity.uid
 
         if (
             new_entity.tx_id_property is not None
             and self.complement is not None
             and self.complement.tx_id_property is not None
             and self.complement.tx_id_property.values is not None
             and self.complement.vertices is not None
@@ -648,15 +647,14 @@
                 tx_ids = self.complement.tx_id_property.values[cell_mask]
 
             base_object = (
                 self.base_transmitter_type  # pylint: disable=no-member
                 if isinstance(self, self.default_receiver_type)
                 else self.base_receiver_type  # pylint: disable=no-member
             )
-
             new_complement = super(base_object, self.complement).copy(
                 parent=parent,
                 omit_list=omit_list,
                 copy_children=copy_children,
                 clear_cache=clear_cache,
                 mask=mask,
             )
@@ -702,19 +700,17 @@
 
     @property
     def tx_id_property(self) -> ReferencedData | None:
         """
         Default channel units for time or frequency defined on the child class.
         """
         if self._tx_id_property is None:
-            if "Tx ID property" in self.metadata["EM Dataset"]:
-                data = self.get_data(self.metadata["EM Dataset"]["Tx ID property"])
-
-                if any(data) and isinstance(data[0], ReferencedData):
-                    self._tx_id_property = data[0]
+            data = self.get_data("Transmitter ID")
+            if any(data) and isinstance(data[0], ReferencedData):
+                self._tx_id_property = data[0]
 
         return self._tx_id_property
 
     @tx_id_property.setter
     def tx_id_property(self, value: uuid.UUID | ReferencedData | np.ndarray | None):
         if isinstance(value, uuid.UUID):
             value = self.get_data(value)[0]
@@ -734,29 +730,31 @@
                     "primitive_type": "REFERENCED",
                     "value_map": value_map,
                 }
 
             value = self.add_data(
                 {
                     "Transmitter ID": {
-                        "values": value,
+                        "values": value.astype(np.int32),
                         "entity_type": entity_type,
                         "type": "referenced",
                     }
                 }
             )
 
         if not isinstance(value, (ReferencedData, type(None))):
             raise TypeError(
                 "Input value for 'tx_id_property' should be of type uuid.UUID, "
                 "ReferencedData, np.ndarray or None.)"
             )
 
         self._tx_id_property = value
-        self.edit_metadata({"Tx ID property": getattr(value, "uid", None)})
+
+        if self.type == "Receivers":
+            self.edit_metadata({"Tx ID property": getattr(value, "uid", None)})
 
 
 class AirborneEMSurvey(BaseEMSurvey, Curve):
     __INPUT_TYPE = ["Rx", "Tx", "Tx and Rx"]
     _PROPERTY_MAP = {
         "crossline_offset": "Crossline offset",
         "inline_offset": "Inline offset",
```

### Comparing `geoh5py-0.8.0a2/geoh5py/objects/surveys/electromagnetics/ground_fem.py` & `geoh5py-0.8.0a3/geoh5py/objects/surveys/electromagnetics/ground_fem.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a2/geoh5py/objects/surveys/electromagnetics/ground_tem.py` & `geoh5py-0.8.0a3/geoh5py/objects/surveys/electromagnetics/ground_tem.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a2/geoh5py/objects/surveys/electromagnetics/magnetotellurics.py` & `geoh5py-0.8.0a3/geoh5py/objects/surveys/electromagnetics/magnetotellurics.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a2/geoh5py/objects/surveys/electromagnetics/tipper.py` & `geoh5py-0.8.0a3/geoh5py/objects/surveys/electromagnetics/tipper.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a2/geoh5py/objects/surveys/magnetics.py` & `geoh5py-0.8.0a3/geoh5py/objects/surveys/magnetics.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a2/geoh5py/shared/__init__.py` & `geoh5py-0.8.0a3/geoh5py/shared/__init__.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a2/geoh5py/shared/concatenation.py` & `geoh5py-0.8.0a3/geoh5py/shared/concatenation.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a2/geoh5py/shared/conversion/__init__.py` & `geoh5py-0.8.0a3/geoh5py/shared/conversion/__init__.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a2/geoh5py/shared/conversion/base.py` & `geoh5py-0.8.0a3/geoh5py/shared/conversion/base.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a2/geoh5py/shared/conversion/geo_image.py` & `geoh5py-0.8.0a3/geoh5py/shared/conversion/geo_image.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a2/geoh5py/shared/conversion/grid2d.py` & `geoh5py-0.8.0a3/geoh5py/shared/conversion/grid2d.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a2/geoh5py/shared/entity.py` & `geoh5py-0.8.0a3/geoh5py/shared/entity.py`

 * *Files 0% similar despite different names*

```diff
@@ -177,17 +177,17 @@
         self, extent: np.ndarray, inverse: bool = False
     ) -> np.ndarray | None:
         """
         Get a mask array from coordinate extent.
 
         :param extent: Bounding box extent coordinates defined by either:
             - obj:`numpy.ndarray` of shape (2, 3)
-                3D coordinate: [[west, south, bottom], [east, north, top]]
+            3D coordinate: [[west, south, bottom], [east, north, top]]
             - obj:`numpy.ndarray` of shape (2, 2)
-                Horizontal coordinates: [[west, south], [east, north]].
+            Horizontal coordinates: [[west, south], [east, north]].
         :param inverse: Return the complement of the mask extent. Default to False
 
         :return: Array of bool defining the vertices or cell centers
             within the mask extent, or None if no intersection.
         """
 
     @classmethod
```

### Comparing `geoh5py-0.8.0a2/geoh5py/shared/entity_type.py` & `geoh5py-0.8.0a3/geoh5py/shared/entity_type.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a2/geoh5py/shared/exceptions.py` & `geoh5py-0.8.0a3/geoh5py/shared/exceptions.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a2/geoh5py/shared/utils.py` & `geoh5py-0.8.0a3/geoh5py/shared/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 #  along with geoh5py.  If not, see <https://www.gnu.org/licenses/>.
 
 from __future__ import annotations
 
 import warnings
 from abc import ABC
 from contextlib import contextmanager
+from io import BytesIO
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Callable
 from uuid import UUID
 
 import h5py
 import numpy as np
 
@@ -165,27 +166,30 @@
 def clear_array_attributes(entity: Entity, recursive: bool = False):
     """
     Clear all stashed values of attributes from an entity to free up memory.
 
     :param entity: Entity to clear attributes from.
     :param recursive: Clear attributes from children entities.
     """
+    if isinstance(entity.workspace.h5file, BytesIO):
+        return
+
     for attribute in ["vertices", "cells", "values", "prisms", "layers"]:
         if hasattr(entity, attribute):
             setattr(entity, f"_{attribute}", None)
 
     if recursive:
         for child in entity.children:
             clear_array_attributes(child, recursive=recursive)
 
 
 def compare_entities(
     object_a, object_b, ignore: list | None = None, decimal: int = 6
 ) -> None:
-    ignore_list = ["_workspace", "_children"]
+    ignore_list = ["_workspace", "_children", "_visual_parameters"]
     if ignore is not None:
         for item in ignore:
             ignore_list.append(item)
 
     for attr in object_a.__dict__.keys():
         if attr in ignore_list:
             continue
```

### Comparing `geoh5py-0.8.0a2/geoh5py/shared/validators.py` & `geoh5py-0.8.0a3/geoh5py/shared/validators.py`

 * *Files 3% similar despite different names*

```diff
@@ -231,15 +231,15 @@
         """
         if isinstance(valid, type):
             valid = [valid]
 
         if not isinstance(valid, list):
             raise TypeError("Input `valid` options must be a type or list of types.")
 
-        if not iterable(value):
+        if not iterable(value) or (isinstance(value, list) and list in tuple(valid)):
             value = (value,)
 
         for val in value:
             if not isinstance(val, tuple(valid)):
                 valid_names = [t.__name__ for t in valid if hasattr(t, "__name__")]
                 type_name = type(val).__name__
```

### Comparing `geoh5py-0.8.0a2/geoh5py/shared/weakref_utils.py` & `geoh5py-0.8.0a3/geoh5py/shared/weakref_utils.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a2/geoh5py/ui_json/__init__.py` & `geoh5py-0.8.0a3/geoh5py/ui_json/__init__.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a2/geoh5py/ui_json/constants.py` & `geoh5py-0.8.0a3/geoh5py/ui_json/constants.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a2/geoh5py/ui_json/input_file.py` & `geoh5py-0.8.0a3/geoh5py/ui_json/input_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,14 @@
     uuid2entity,
 )
 from .constants import base_validations, ui_validations
 from .utils import (
     container_group2name,
     flatten,
     inf2str,
-    list2str,
     none2str,
     path2workspace,
     set_enabled,
     str2inf,
     str2none,
     workspace2path,
 )
@@ -442,27 +441,20 @@
     @staticmethod
     def stringify(var: dict[str, Any]) -> dict[str, Any]:
         """
         Convert inf, none, and list types to strings within a dictionary
 
         :param var: Dictionary containing ui.json keys, values, fields
 
-        :return: Dictionary with inf, none and list types converted to string
+        :return: Dictionary with inf and none types converted to string
             representations in json format.
         """
         for key, value in var.items():
-            exclude = ["choiceList", "meshType", "dataType", "groupType", "association"]
-            mappers = (
-                [list2str, inf2str, as_str_if_uuid, none2str]
-                if key not in exclude
-                else [inf2str, as_str_if_uuid, none2str]
-            )
-            var[key] = dict_mapper(
-                value, mappers, omit={ex: [list2str] for ex in exclude}
-            )
+            mappers = [inf2str, as_str_if_uuid, none2str]
+            var[key] = dict_mapper(value, mappers)
 
         return var
 
     @classmethod
     def numify(cls, ui_json: dict[str, Any]) -> dict[str, Any]:
         """
         Convert inf, none and list strings to numerical types within a dictionary
```

### Comparing `geoh5py-0.8.0a2/geoh5py/ui_json/templates.py` & `geoh5py-0.8.0a3/geoh5py/ui_json/templates.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a2/geoh5py/ui_json/utils.py` & `geoh5py-0.8.0a3/geoh5py/ui_json/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -332,15 +332,15 @@
     directory_path = Path(directory)
     working_path = directory_path / ".working"
     working_path.mkdir(exist_ok=True)
 
     temp_geoh5 = f"temp{time():.3f}.geoh5"
 
     with fetch_active_workspace(entity.workspace, mode="r"):
-        with Workspace(working_path / temp_geoh5) as w_s:
+        with Workspace.create(working_path / temp_geoh5) as w_s:
             entity.copy(parent=w_s, copy_children=copy_children)
 
     shutil.move(
         working_path / temp_geoh5,
         directory_path / temp_geoh5,
     )
```

### Comparing `geoh5py-0.8.0a2/geoh5py/ui_json/validation.py` & `geoh5py-0.8.0a3/geoh5py/ui_json/validation.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a2/geoh5py/workspace/__init__.py` & `geoh5py-0.8.0a3/geoh5py/workspace/__init__.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a2/geoh5py/workspace/workspace.py` & `geoh5py-0.8.0a3/geoh5py/workspace/workspace.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,33 +16,36 @@
 #  along with geoh5py.  If not, see <https://www.gnu.org/licenses/>.
 
 # pylint: disable=too-many-lines, too-many-public-methods, too-many-arguments, too-many-locals
 
 from __future__ import annotations
 
 import inspect
-import io
 import shutil
 import subprocess
 import tempfile
 import uuid
 import warnings
 import weakref
 from contextlib import AbstractContextManager, contextmanager
 from gc import collect
+from getpass import getuser
+from io import BytesIO
 from pathlib import Path
 from subprocess import CalledProcessError
 from typing import TYPE_CHECKING, ClassVar, cast
 from weakref import ReferenceType
 
 import h5py
 import numpy as np
 
 from .. import data, groups, objects
 from ..data import CommentsData, Data, DataType
+from ..data.text_data import TextData
+from ..data.visual_parameters import VisualParameters
 from ..groups import (
     CustomGroup,
     DrillholeGroup,
     Group,
     IntegratorDrillholeGroup,
     PropertyGroup,
     RootGroup,
@@ -70,64 +73,68 @@
     from ..groups import group
     from ..objects import object_base
     from ..shared import EntityType
 
 
 class Workspace(AbstractContextManager):
     """
-    The Workspace class manages all Entities created or imported from the *geoh5* structure.
+    The Workspace class manages all Entities created or imported from the
+    *geoh5* structure.
 
     The basic requirements needed to create a Workspace are:
 
-    :param geoh5: File name of the target *geoh5* file.
-        A new project is created if the target file cannot by found on disk.
+    :param h5file: Path to the *geoh5* file or :obj:`oi.BytesIO` representation
+        of a geoh5 structure.
+    :param contributors: List of contributors to the project.
+    :param distance_unit: Distance unit used in the project.
+    :param ga_version: Version of the *geoh5* file format.
+    :param mode: Mode in which the *geoh5* file is opened.
+    :param name: Name of the project.
+    :param repack: Repack the *geoh5* file after closing.
+    :param version: Version of the project.
     """
 
     _active_ref: ClassVar[ReferenceType[Workspace]] | type(None) = type(None)  # type: ignore
 
     _attribute_map = {
         "Contributors": "contributors",
         "Distance unit": "distance_unit",
         "GA Version": "ga_version",
         "Version": "version",
     }
 
     def __init__(
-        self, h5file: str | Path | io.BytesIO = "Analyst.geoh5", mode="a", **kwargs
+        self,
+        h5file: str | Path | BytesIO | None = None,
+        contributors: tuple[str] = (getuser(),),
+        distance_unit: str = "meter",
+        ga_version: str = "1",
+        mode="r+",
+        name: str = "GEOSCIENCE",
+        repack: bool = False,
+        version: float = 2.1,
     ):
-        self._contributors = np.asarray(
-            ["UserName"], dtype=h5py.special_dtype(vlen=str)
+        self._data: dict[uuid.UUID, ReferenceType[data.Data]] = {}
+        self._distance_unit: str = distance_unit
+        self._contributors: list[str] = np.asarray(
+            contributors, dtype=h5py.special_dtype(vlen=str)
         )
-        self._root: Entity | None = None
-        self._repack: bool = False
-        self._mode = mode
-        self._distance_unit = "meter"
-        self._ga_version = "1"
-        self._version = 2.1
-        self._name = "GEOSCIENCE"
-        self._types: dict[uuid.UUID, ReferenceType[EntityType]] = {}
+        self._ga_version: str = ga_version
+        self._geoh5: h5py.File | bool = False
         self._groups: dict[uuid.UUID, ReferenceType[group.Group]] = {}
+        self._h5file: str | Path | BytesIO | None = None
+        self._mode: str = mode
+        self._name: str = name
         self._objects: dict[uuid.UUID, ReferenceType[object_base.ObjectBase]] = {}
-        self._data: dict[uuid.UUID, ReferenceType[data.Data]] = {}
-        self._geoh5: h5py.File | bool = False
-        self.h5file: str | Path | io.BytesIO = h5file
-
-        for attr, item in kwargs.items():
-            if attr in self._attribute_map:
-                attr = self._attribute_map[attr]
-
-            if getattr(self, attr, None) is None:
-                warnings.warn(
-                    f"Argument {attr} with value {item} is not a valid attribute of workspace. "
-                    f"Argument ignored.",
-                    UserWarning,
-                )
-            else:
-                setattr(self, attr, item)
+        self._repack: bool = repack
+        self._root: Entity | None = None
+        self._types: dict[uuid.UUID, ReferenceType[EntityType]] = {}
+        self._version: float = version
 
+        self.h5file = h5file
         self.open()
 
     def activate(self):
         """Makes this workspace the active one.
 
         In case the workspace gets deleted, Workspace.active() safely returns None.
         """
@@ -183,25 +190,29 @@
                 if isinstance(entity, Concatenator) and self.repack:
                     self.update_attribute(entity, "concatenated_attributes")
 
             self._io_call(H5Writer.save_entity, self.root, add_children=True, mode="r+")
 
         self.geoh5.close()
         self._data = {}
-        if self.repack and not isinstance(self.h5file, io.BytesIO):
-            temp_file = Path(tempfile.gettempdir()) / Path(self.h5file).name
+        if (
+            self.repack
+            and not isinstance(self._h5file, BytesIO)
+            and self._h5file is not None
+        ):
+            temp_file = Path(tempfile.gettempdir()) / Path(self._h5file).name
             try:
                 subprocess.run(
-                    f'h5repack --native "{self.h5file}" "{temp_file}"',
+                    f'h5repack --native "{self._h5file}" "{temp_file}"',
                     check=True,
                     shell=True,
                     stdout=subprocess.DEVNULL,
                 )
-                Path(self.h5file).unlink()
-                shutil.move(temp_file, self.h5file)
+                Path(self._h5file).unlink()
+                shutil.move(temp_file, self._h5file)
             except CalledProcessError:
                 pass
 
             self.repack = False
 
     @property
     def contributors(self) -> np.ndarray:
@@ -231,15 +242,22 @@
         :param clear_cache: Clear array attributes after copy.
         :param kwargs: Additional keyword arguments passed to the copy constructor.
 
         :return: The Entity registered to the workspace.
         """
         entity_kwargs = get_attributes(
             entity,
-            omit_list=["_uid", "_entity_type", "_on_file", "_centroids", "_extent"]
+            omit_list=[
+                "_uid",
+                "_entity_type",
+                "_on_file",
+                "_centroids",
+                "_extent",
+                "_visual_parameters",
+            ]
             + list(omit_list),
             attributes={"uid": None, "parent": None},
         )
 
         if entity_kwargs is None:
             return None
 
@@ -296,14 +314,19 @@
                     "association": prop_group.association,
                     "name": prop_group.name,
                     "property_group_type": prop_group.property_group_type,
                 }
             )
             new_group.properties = [data_map[uid] for uid in prop_group.properties]
 
+    @classmethod
+    def create(cls, path: str | Path, **kwargs) -> Workspace:
+        """Create a named blank workspace and save to disk."""
+        return cls(**kwargs).save(path)
+
     def create_from_concatenation(self, attributes):
         if "Name" in attributes:
             attributes["Name"] = attributes["Name"].replace("\u2044", "/")
 
         if "Object Type ID" in attributes:
             recovered_entity = self.create_entity(
                 ObjectBase,
@@ -370,14 +393,20 @@
                     continue
 
                 if self.version > 1.0 and isinstance(
                     entity_kwargs["parent"], ConcatenatedObject
                 ):
                     member = type(name + "Concatenated", (ConcatenatedData, member), {})
 
+                if member is TextData and any(
+                    isinstance(val, str) and "Visual Parameters" == val
+                    for val in entity_kwargs.values()
+                ):
+                    member = VisualParameters
+
                 created_entity = member(data_type, **entity_kwargs)
                 return created_entity
 
         return None
 
     def create_entity(
         self,
@@ -398,29 +427,32 @@
 
         if entity_class is not RootGroup and (
             "parent" not in entity_kwargs or entity_kwargs["parent"] is None
         ):
             entity_kwargs["parent"] = self.root
 
         created_entity: Data | Group | ObjectBase | None = None
-        if entity_class is Data or entity_class is None:
+        if entity_class is None or issubclass(entity_class, Data):
             created_entity = self.create_data(Data, entity_kwargs, entity_type_kwargs)
 
+            if isinstance(created_entity, VisualParameters):
+                entity_kwargs["parent"].visual_parameters = created_entity
+
         elif entity_class is RootGroup:
             created_entity = RootGroup(
                 RootGroup.find_or_create_type(self, **entity_type_kwargs),
                 **entity_kwargs,
             )
 
         elif issubclass(entity_class, (Group, ObjectBase)):
             created_entity = self.create_object_or_group(
                 entity_class, entity_kwargs, entity_type_kwargs
             )
 
-        if created_entity is not None and save_on_creation:
+        if created_entity is not None and save_on_creation and self.h5file is not None:
             self.save_entity(created_entity)
 
         return created_entity
 
     def create_object_or_group(
         self, entity_class, entity_kwargs: dict, entity_type_kwargs: dict
     ) -> Group | ObjectBase | None:
@@ -830,15 +862,16 @@
         Deprecate method finalize
 
         :param file: :obj:`h5py.File` or name of the target geoh5 file
         """
         warnings.warn(
             "The 'finalize' method will be deprecated in future versions of geoh5py in"
             " favor of `workspace.close()`. "
-            "Please update your code to suppress this warning."
+            "Please update your code to suppress this warning.",
+            DeprecationWarning,
         )
         self.close()
 
     def find_data(self, data_uid: uuid.UUID) -> Entity | None:
         """
         Find an existing and active Data entity.
         """
@@ -923,33 +956,65 @@
         """
         if not self._geoh5:
             raise Geoh5FileClosedError
 
         return self._geoh5
 
     @property
-    def h5file(self) -> str | Path | io.BytesIO:
+    def h5file(self) -> str | Path | BytesIO | None:
         """
-        :str: Target *geoh5* file name with path.
+        Target *geoh5* file name with path or BytesIO object representation.
+
+        On :func:`geoh5py.workspace.Workspace.save`, the BytesIO representation
+        gets replaced by a Path to a file on disk.
         """
         return self._h5file
 
     @h5file.setter
-    def h5file(self, file: str | Path | io.BytesIO):
-        if isinstance(file, (str, Path)):
-            if Path(file).suffix != ".geoh5":
-                raise ValueError("Input 'h5file' file must have a 'geoh5' extension.")
-        elif not isinstance(file, io.BytesIO):
+    def h5file(self, file: str | Path | BytesIO | None):
+        if self._h5file is not None:
+            raise ValueError(
+                "The 'h5file' attribute cannot be changed once it has been set."
+            )
+
+        if not isinstance(file, (str, Path, BytesIO, type(None))):
             raise ValueError(
                 "The 'h5file' attribute must be a str, "
-                "pathlib.Path or bytes to the target geoh5 file. "
+                "pathlib.Path to the target geoh5 file or BytesIO. "
                 f"Provided {file} of type({type(file)})"
             )
 
-        self._h5file = file
+        if isinstance(file, type(None)) or (
+            isinstance(file, (str, Path)) and not Path(file).is_file()
+        ):
+            self._h5file = BytesIO()
+            self._geoh5 = h5py.File(self.h5file, "a")
+
+            with self._geoh5:
+                self._root = self.create_entity(RootGroup, save_on_creation=False)
+                H5Writer.init_geoh5(self.geoh5, self)
+
+        elif isinstance(file, BytesIO):
+            self._h5file = file
+
+        if isinstance(file, (str, Path)):
+            if Path(file).suffix != ".geoh5":
+                raise ValueError("Input 'h5file' file must have a 'geoh5' extension.")
+
+            if not Path(file).is_file():
+                warnings.warn(
+                    "From version 0.8.0, the 'h5file' attribute must be a string "
+                    "or path to an existing file, or user must call the 'create' "
+                    "method. We will attempt to create the file for you, but this "
+                    "behaviour will be removed in future releases.",
+                    DeprecationWarning,
+                )
+                self.save(file)
+            else:
+                self._h5file = file
 
     @property
     def list_data_name(self) -> dict[uuid.UUID, str]:
         """
         :obj:`dict` of :obj:`uuid.UUID` keys and name values for all registered Data.
         """
         data_name = {}
@@ -1061,32 +1126,27 @@
             warnings.warn(f"Workspace already opened in mode {self._geoh5.mode}.")
             return self
 
         if mode is None:
             mode = self._mode
 
         try:
-            self._geoh5 = h5py.File(self._h5file, mode)
+            self._geoh5 = h5py.File(self.h5file, mode)
         except OSError:
-            mode = "r"
-            self._geoh5 = h5py.File(self._h5file, mode)
+            self._geoh5 = h5py.File(self.h5file, "r")
 
         self._data = {}
         self._objects = {}
         self._groups = {}
         self._types = {}
 
-        try:
-            proj_attributes = self._io_call(H5Reader.fetch_project_attributes, mode="r")
-
-            for key, attr in proj_attributes.items():
-                setattr(self, self._attribute_map[key], attr)
+        proj_attributes = self._io_call(H5Reader.fetch_project_attributes, mode="r")
 
-        except FileNotFoundError:
-            self._io_call(H5Writer.create_geoh5, self, mode="a")
+        for key, attr in proj_attributes.items():
+            setattr(self, self._attribute_map[key], attr)
 
         self.fetch_or_create_root()
 
         return self
 
     def _register_type(self, entity_type: EntityType):
         weakref_utils.insert_once(self._types, entity_type.uid, entity_type)
@@ -1114,14 +1174,36 @@
         """
         return self._repack
 
     @repack.setter
     def repack(self, value: bool):
         self._repack = value
 
+    def save(self, filepath: str | Path) -> Workspace:
+        """
+        Save the workspace to disk.
+        """
+        if self._geoh5 is not None:
+            self.close()
+
+        filepath = Path(filepath)
+
+        if filepath.suffix != ".geoh5":
+            raise ValueError("Input 'h5file' file must have a 'geoh5' extension.")
+
+        if isinstance(self.h5file, BytesIO):
+            with open(filepath, "wb") as file:
+                file.write(self.h5file.getbuffer())
+
+            self._h5file = filepath
+
+        self.open()
+
+        return self
+
     def save_entity(
         self,
         entity: Entity,
         add_children: bool = True,
     ) -> None:
         """
         Save or update an entity to geoh5.
@@ -1218,25 +1300,37 @@
         return self
 
     def _io_call(self, fun, *args, mode="r", **kwargs):
         """
         Run a H5Writer or H5Reader function with validation of target geoh5
         """
         try:
+            if self._geoh5 is None:
+                return None
+
             if mode in ["r+", "a"] and self.geoh5.mode == "r":
                 raise UserWarning(
                     f"Error performing {fun}. "
                     "Attempting to write to a geoh5 file in read-only mode. "
                     "Consider closing the workspace (Geoscience ANALYST) and "
                     "re-opening in mode='r+'."
                 )
 
             return fun(self.geoh5, *args, **kwargs)
 
         except Geoh5FileClosedError as error:
+            if not Path(str(self.h5file)).is_file() and not isinstance(
+                self.h5file, BytesIO
+            ):
+                raise FileNotFoundError(
+                    f"Error performing {fun}. "
+                    "The geoh5 file does not exist."
+                    r"Consider creating the geoh5 with Workspace().save('PATH\*.geoh5)'"
+                ) from error
+
             raise Geoh5FileClosedError(
                 f"Error executing {fun}. "
                 + "Consider re-opening with `Workspace.open()' "
                 "or used within a context manager."
             ) from error
 
     def __exit__(self, exc_type, exc_value, traceback):
```

### Comparing `geoh5py-0.8.0a2/package.rst` & `geoh5py-0.8.0a3/package.rst`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a2/pyproject.toml` & `geoh5py-0.8.0a3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "geoh5py"
-version = "0.8.0-alpha.2"
+version = "0.8.0-alpha.3"
 license = "LGPL-3.0-or-later"
 description = "Python API for geoh5, an open file format for geoscientific data"
 authors = ["Mira Geoscience <support@mirageoscience.com>"]
 repository = "https://github.com/MiraGeoscience/geoh5py"
 documentation = "https://geoh5py.readthedocs.io/en/latest/"
 homepage = "https://mirageoscience.com"
 readme = "package.rst"
@@ -25,35 +25,27 @@
 [tool.poetry.dependencies]
 python = "^3.8,<3.11"
 Pillow = ">=8.0.1,<10.0.0"
 h5py = "^3.2.1"
 numpy = "!=1.19.4, ~1.23.5"
 
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
 lockfile = "^0.12.2"
-poetry-publish = {git = "https://github.com/MiraGeoscience/poetry-publish.git", rev = "pending_fixes"}
 pylint = "*"
 pytest = "*"
 pytest-cov = "*"
 scipy = "^1.4.1"
 sphinx = "^3.0"
 sphinx-autodoc-typehints = "^1.10"
 sphinx-rtd-theme = "^0.4.3"
 tomli = "*"
 
 [tool.poetry.extras]
 
-[tool.poetry.scripts]
-publish = 'devtools.publish:publish'
-
-[tool.dephell.main]
-from = {format = "poetry", path = "pyproject.toml"}
-to = {format = "setuppy", path = "setup.py"}
-
 [tool.isort]
 # settings for compatibility between ``isort`` and ``black`` formatting
 multi_line_output = 3
 include_trailing_comma = true
 force_grid_wrap = 0
 use_parentheses = true
 line_length = 88
```

### Comparing `geoh5py-0.8.0a2/PKG-INFO` & `geoh5py-0.8.0a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geoh5py
-Version: 0.8.0a2
+Version: 0.8.0a3
 Summary: Python API for geoh5, an open file format for geoscientific data
 Home-page: https://mirageoscience.com
 License: LGPL-3.0-or-later
 Keywords: geology,geophysics,data,interoperability
 Author: Mira Geoscience
 Author-email: support@mirageoscience.com
 Requires-Python: >=3.8,<3.11
```

