# Comparing `tmp/gaitmap-2.2.0.tar.gz` & `tmp/gaitmap-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gaitmap-2.2.0.tar", max compression
+gzip compressed data, was "gaitmap-2.2.1.tar", max compression
```

## Comparing `gaitmap-2.2.0.tar` & `gaitmap-2.2.1.tar`

### file list

```diff
@@ -1,67 +1,67 @@
--rw-r--r--   0        0        0     2032 2023-06-07 10:17:53.763523 gaitmap-2.2.0/LICENSE
--rw-r--r--   0        0        0     8913 2023-06-07 10:17:53.763523 gaitmap-2.2.0/README.md
--rw-r--r--   0        0        0       69 2023-06-07 10:17:53.839528 gaitmap-2.2.0/gaitmap/__init__.py
--rw-r--r--   0        0        0      164 2023-06-07 10:17:53.839528 gaitmap-2.2.0/gaitmap/_event_detection_common/__init__.py
--rw-r--r--   0        0        0     7213 2023-06-07 10:17:53.839528 gaitmap-2.2.0/gaitmap/_event_detection_common/_event_detection_mixin.py
--rw-r--r--   0        0        0    12216 2023-06-07 10:17:53.839528 gaitmap-2.2.0/gaitmap/base.py
--rw-r--r--   0        0        0     1316 2023-06-07 10:17:53.839528 gaitmap-2.2.0/gaitmap/data_transform/__init__.py
--rw-r--r--   0        0        0    15931 2023-06-07 10:17:53.839528 gaitmap-2.2.0/gaitmap/data_transform/_base.py
--rw-r--r--   0        0        0    12004 2023-06-07 10:17:53.839528 gaitmap-2.2.0/gaitmap/data_transform/_feature_transform.py
--rw-r--r--   0        0        0     3969 2023-06-07 10:17:53.839528 gaitmap-2.2.0/gaitmap/data_transform/_filter.py
--rw-r--r--   0        0        0    15524 2023-06-07 10:17:53.839528 gaitmap-2.2.0/gaitmap/data_transform/_scaler.py
--rw-r--r--   0        0        0      765 2023-06-07 10:17:53.839528 gaitmap-2.2.0/gaitmap/evaluation_utils/__init__.py
--rw-r--r--   0        0        0     6326 2023-06-07 10:17:53.839528 gaitmap-2.2.0/gaitmap/evaluation_utils/event_detection.py
--rw-r--r--   0        0        0    28925 2023-06-07 10:17:53.839528 gaitmap-2.2.0/gaitmap/evaluation_utils/parameter_errors.py
--rw-r--r--   0        0        0    11515 2023-06-07 10:17:53.839528 gaitmap-2.2.0/gaitmap/evaluation_utils/scores.py
--rw-r--r--   0        0        0    22255 2023-06-07 10:17:53.839528 gaitmap-2.2.0/gaitmap/evaluation_utils/stride_segmentation.py
--rw-r--r--   0        0        0      702 2023-06-07 10:17:53.839528 gaitmap-2.2.0/gaitmap/event_detection/__init__.py
--rw-r--r--   0        0        0    19385 2023-06-07 10:17:53.839528 gaitmap-2.2.0/gaitmap/event_detection/_herzer_event_detection.py
--rw-r--r--   0        0        0     6735 2023-06-07 10:17:53.839528 gaitmap-2.2.0/gaitmap/example_data.py
--rw-r--r--   0        0        0      542 2023-06-07 10:17:53.839528 gaitmap-2.2.0/gaitmap/gait_detection/__init__.py
--rw-r--r--   0        0        0      350 2023-06-07 10:17:53.839528 gaitmap-2.2.0/gaitmap/parameters/__init__.py
--rw-r--r--   0        0        0    21721 2023-06-07 10:17:53.839528 gaitmap-2.2.0/gaitmap/parameters/_spatial_parameters.py
--rw-r--r--   0        0        0     7432 2023-06-07 10:17:53.839528 gaitmap-2.2.0/gaitmap/parameters/_temporal_parameters.py
--rw-r--r--   0        0        0      287 2023-06-07 10:17:53.839528 gaitmap-2.2.0/gaitmap/preprocessing/__init__.py
--rw-r--r--   0        0        0      785 2023-06-07 10:17:53.839528 gaitmap-2.2.0/gaitmap/preprocessing/sensor_alignment/__init__.py
--rw-r--r--   0        0        0     5094 2023-06-07 10:17:53.839528 gaitmap-2.2.0/gaitmap/preprocessing/sensor_alignment/_gravity_alignment.py
--rw-r--r--   0        0        0     3940 2023-06-07 10:17:53.839528 gaitmap-2.2.0/gaitmap/preprocessing/sensor_alignment/_mulisensor_alignment.py
--rw-r--r--   0        0        0     6322 2023-06-07 10:17:53.839528 gaitmap-2.2.0/gaitmap/preprocessing/sensor_alignment/_pca_alignment.py
--rw-r--r--   0        0        0     1732 2023-06-07 10:17:53.839528 gaitmap-2.2.0/gaitmap/stride_segmentation/__init__.py
--rw-r--r--   0        0        0    14875 2023-06-07 10:17:53.843528 gaitmap-2.2.0/gaitmap/stride_segmentation/_roi_stride_segmentation.py
--rw-r--r--   0        0        0     2713 2023-06-07 10:17:53.843528 gaitmap-2.2.0/gaitmap/stride_segmentation/_utils.py
--rw-r--r--   0        0        0     1181 2023-06-07 10:17:53.843528 gaitmap-2.2.0/gaitmap/stride_segmentation/hmm.py
--rw-r--r--   0        0        0     1029 2023-06-07 10:17:53.843528 gaitmap-2.2.0/gaitmap/trajectory_reconstruction/__init__.py
--rw-r--r--   0        0        0    21419 2023-06-07 10:17:53.843528 gaitmap-2.2.0/gaitmap/trajectory_reconstruction/_region_level_trajectory.py
--rw-r--r--   0        0        0     9438 2023-06-07 10:17:53.843528 gaitmap-2.2.0/gaitmap/trajectory_reconstruction/_stride_level_trajectory.py
--rw-r--r--   0        0        0    10746 2023-06-07 10:17:53.843528 gaitmap-2.2.0/gaitmap/trajectory_reconstruction/_trajectory_wrapper.py
--rw-r--r--   0        0        0      317 2023-06-07 10:17:53.843528 gaitmap-2.2.0/gaitmap/trajectory_reconstruction/orientation_methods/__init__.py
--rw-r--r--   0        0        0     8096 2023-06-07 10:17:53.843528 gaitmap-2.2.0/gaitmap/trajectory_reconstruction/orientation_methods/_madgwick.py
--rw-r--r--   0        0        0     4858 2023-06-07 10:17:53.843528 gaitmap-2.2.0/gaitmap/trajectory_reconstruction/orientation_methods/_simple_gyro_integration.py
--rw-r--r--   0        0        0      618 2023-06-07 10:17:53.843528 gaitmap-2.2.0/gaitmap/trajectory_reconstruction/position_methods/__init__.py
--rw-r--r--   0        0        0     7458 2023-06-07 10:17:53.843528 gaitmap-2.2.0/gaitmap/trajectory_reconstruction/position_methods/_forward_backwards_integration.py
--rw-r--r--   0        0        0      243 2023-06-07 10:17:53.843528 gaitmap-2.2.0/gaitmap/trajectory_reconstruction/trajectory_methods/__init__.py
--rw-r--r--   0        0        0    13664 2023-06-07 10:17:53.843528 gaitmap-2.2.0/gaitmap/trajectory_reconstruction/trajectory_methods/_kalman_numba_funcs.py
--rw-r--r--   0        0        0    16637 2023-06-07 10:17:53.843528 gaitmap-2.2.0/gaitmap/trajectory_reconstruction/trajectory_methods/_rts_kalman.py
--rw-r--r--   0        0        0       41 2023-06-07 10:17:53.843528 gaitmap-2.2.0/gaitmap/utils/__init__.py
--rw-r--r--   0        0        0     1857 2023-06-07 10:17:53.843528 gaitmap-2.2.0/gaitmap/utils/_algo_helper.py
--rw-r--r--   0        0        0     4695 2023-06-07 10:17:53.843528 gaitmap-2.2.0/gaitmap/utils/_datatype_validation_helper.py
--rw-r--r--   0        0        0     1020 2023-06-07 10:17:53.843528 gaitmap-2.2.0/gaitmap/utils/_gaitmap_mad.py
--rw-r--r--   0        0        0      381 2023-06-07 10:17:53.843528 gaitmap-2.2.0/gaitmap/utils/_types.py
--rw-r--r--   0        0        0    17992 2023-06-07 10:17:53.843528 gaitmap-2.2.0/gaitmap/utils/array_handling.py
--rw-r--r--   0        0        0     2555 2023-06-07 10:17:53.843528 gaitmap-2.2.0/gaitmap/utils/consts.py
--rw-r--r--   0        0        0     6284 2023-06-07 10:17:53.843528 gaitmap-2.2.0/gaitmap/utils/coordinate_conversion.py
--rw-r--r--   0        0        0    48845 2023-06-07 10:17:53.843528 gaitmap-2.2.0/gaitmap/utils/datatype_helper.py
--rw-r--r--   0        0        0     1089 2023-06-07 10:17:53.843528 gaitmap-2.2.0/gaitmap/utils/exceptions.py
--rw-r--r--   0        0        0     1865 2023-06-07 10:17:53.843528 gaitmap-2.2.0/gaitmap/utils/fast_quaternion_math.py
--rw-r--r--   0        0        0    18908 2023-06-07 10:17:53.843528 gaitmap-2.2.0/gaitmap/utils/rotations.py
--rw-r--r--   0        0        0     2372 2023-06-07 10:17:53.843528 gaitmap-2.2.0/gaitmap/utils/signal_processing.py
--rw-r--r--   0        0        0    14377 2023-06-07 10:17:53.843528 gaitmap-2.2.0/gaitmap/utils/static_moment_detection.py
--rw-r--r--   0        0        0     8512 2023-06-07 10:17:53.843528 gaitmap-2.2.0/gaitmap/utils/stride_list_conversion.py
--rw-r--r--   0        0        0     4115 2023-06-07 10:17:53.843528 gaitmap-2.2.0/gaitmap/utils/vector_math.py
--rw-r--r--   0        0        0      670 2023-06-07 10:17:53.843528 gaitmap-2.2.0/gaitmap/zupt_detection/__init__.py
--rw-r--r--   0        0        0     1582 2023-06-07 10:17:53.843528 gaitmap-2.2.0/gaitmap/zupt_detection/_base.py
--rw-r--r--   0        0        0     3068 2023-06-07 10:17:53.843528 gaitmap-2.2.0/gaitmap/zupt_detection/_combo_zupt_detector.py
--rw-r--r--   0        0        0    21964 2023-06-07 10:17:53.843528 gaitmap-2.2.0/gaitmap/zupt_detection/_moving_window_zupt_detector.py
--rw-r--r--   0        0        0     4897 2023-06-07 10:17:53.843528 gaitmap-2.2.0/gaitmap/zupt_detection/_stride_event_zupt_detector.py
--rw-r--r--   0        0        0     5175 2023-06-07 10:17:53.851529 gaitmap-2.2.0/pyproject.toml
--rw-r--r--   0        0        0    10246 1970-01-01 00:00:00.000000 gaitmap-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0     2032 2023-06-22 07:52:47.189214 gaitmap-2.2.1/LICENSE
+-rw-r--r--   0        0        0    10679 2023-06-22 07:52:47.189214 gaitmap-2.2.1/README.md
+-rw-r--r--   0        0        0       69 2023-06-22 07:52:47.261214 gaitmap-2.2.1/gaitmap/__init__.py
+-rw-r--r--   0        0        0      164 2023-06-22 07:52:47.261214 gaitmap-2.2.1/gaitmap/_event_detection_common/__init__.py
+-rw-r--r--   0        0        0     7510 2023-06-22 07:52:47.261214 gaitmap-2.2.1/gaitmap/_event_detection_common/_event_detection_mixin.py
+-rw-r--r--   0        0        0    12216 2023-06-22 07:52:47.261214 gaitmap-2.2.1/gaitmap/base.py
+-rw-r--r--   0        0        0     1316 2023-06-22 07:52:47.261214 gaitmap-2.2.1/gaitmap/data_transform/__init__.py
+-rw-r--r--   0        0        0    15931 2023-06-22 07:52:47.261214 gaitmap-2.2.1/gaitmap/data_transform/_base.py
+-rw-r--r--   0        0        0    12004 2023-06-22 07:52:47.261214 gaitmap-2.2.1/gaitmap/data_transform/_feature_transform.py
+-rw-r--r--   0        0        0     3969 2023-06-22 07:52:47.261214 gaitmap-2.2.1/gaitmap/data_transform/_filter.py
+-rw-r--r--   0        0        0    15524 2023-06-22 07:52:47.261214 gaitmap-2.2.1/gaitmap/data_transform/_scaler.py
+-rw-r--r--   0        0        0      765 2023-06-22 07:52:47.261214 gaitmap-2.2.1/gaitmap/evaluation_utils/__init__.py
+-rw-r--r--   0        0        0     6326 2023-06-22 07:52:47.261214 gaitmap-2.2.1/gaitmap/evaluation_utils/event_detection.py
+-rw-r--r--   0        0        0    28925 2023-06-22 07:52:47.261214 gaitmap-2.2.1/gaitmap/evaluation_utils/parameter_errors.py
+-rw-r--r--   0        0        0    11515 2023-06-22 07:52:47.261214 gaitmap-2.2.1/gaitmap/evaluation_utils/scores.py
+-rw-r--r--   0        0        0    22255 2023-06-22 07:52:47.261214 gaitmap-2.2.1/gaitmap/evaluation_utils/stride_segmentation.py
+-rw-r--r--   0        0        0      702 2023-06-22 07:52:47.261214 gaitmap-2.2.1/gaitmap/event_detection/__init__.py
+-rw-r--r--   0        0        0    19385 2023-06-22 07:52:47.261214 gaitmap-2.2.1/gaitmap/event_detection/_herzer_event_detection.py
+-rw-r--r--   0        0        0     6727 2023-06-22 07:52:47.261214 gaitmap-2.2.1/gaitmap/example_data.py
+-rw-r--r--   0        0        0      542 2023-06-22 07:52:47.261214 gaitmap-2.2.1/gaitmap/gait_detection/__init__.py
+-rw-r--r--   0        0        0      350 2023-06-22 07:52:47.261214 gaitmap-2.2.1/gaitmap/parameters/__init__.py
+-rw-r--r--   0        0        0    21722 2023-06-22 07:52:47.261214 gaitmap-2.2.1/gaitmap/parameters/_spatial_parameters.py
+-rw-r--r--   0        0        0     7836 2023-06-22 07:52:47.261214 gaitmap-2.2.1/gaitmap/parameters/_temporal_parameters.py
+-rw-r--r--   0        0        0      287 2023-06-22 07:52:47.261214 gaitmap-2.2.1/gaitmap/preprocessing/__init__.py
+-rw-r--r--   0        0        0      785 2023-06-22 07:52:47.261214 gaitmap-2.2.1/gaitmap/preprocessing/sensor_alignment/__init__.py
+-rw-r--r--   0        0        0     5094 2023-06-22 07:52:47.261214 gaitmap-2.2.1/gaitmap/preprocessing/sensor_alignment/_gravity_alignment.py
+-rw-r--r--   0        0        0     3940 2023-06-22 07:52:47.261214 gaitmap-2.2.1/gaitmap/preprocessing/sensor_alignment/_mulisensor_alignment.py
+-rw-r--r--   0        0        0     6635 2023-06-22 07:52:47.261214 gaitmap-2.2.1/gaitmap/preprocessing/sensor_alignment/_pca_alignment.py
+-rw-r--r--   0        0        0     1732 2023-06-22 07:52:47.261214 gaitmap-2.2.1/gaitmap/stride_segmentation/__init__.py
+-rw-r--r--   0        0        0    14875 2023-06-22 07:52:47.261214 gaitmap-2.2.1/gaitmap/stride_segmentation/_roi_stride_segmentation.py
+-rw-r--r--   0        0        0     2713 2023-06-22 07:52:47.261214 gaitmap-2.2.1/gaitmap/stride_segmentation/_utils.py
+-rw-r--r--   0        0        0     1181 2023-06-22 07:52:47.261214 gaitmap-2.2.1/gaitmap/stride_segmentation/hmm.py
+-rw-r--r--   0        0        0     1029 2023-06-22 07:52:47.261214 gaitmap-2.2.1/gaitmap/trajectory_reconstruction/__init__.py
+-rw-r--r--   0        0        0    21419 2023-06-22 07:52:47.261214 gaitmap-2.2.1/gaitmap/trajectory_reconstruction/_region_level_trajectory.py
+-rw-r--r--   0        0        0     9438 2023-06-22 07:52:47.261214 gaitmap-2.2.1/gaitmap/trajectory_reconstruction/_stride_level_trajectory.py
+-rw-r--r--   0        0        0    10746 2023-06-22 07:52:47.261214 gaitmap-2.2.1/gaitmap/trajectory_reconstruction/_trajectory_wrapper.py
+-rw-r--r--   0        0        0      317 2023-06-22 07:52:47.261214 gaitmap-2.2.1/gaitmap/trajectory_reconstruction/orientation_methods/__init__.py
+-rw-r--r--   0        0        0     8096 2023-06-22 07:52:47.261214 gaitmap-2.2.1/gaitmap/trajectory_reconstruction/orientation_methods/_madgwick.py
+-rw-r--r--   0        0        0     4858 2023-06-22 07:52:47.261214 gaitmap-2.2.1/gaitmap/trajectory_reconstruction/orientation_methods/_simple_gyro_integration.py
+-rw-r--r--   0        0        0      618 2023-06-22 07:52:47.261214 gaitmap-2.2.1/gaitmap/trajectory_reconstruction/position_methods/__init__.py
+-rw-r--r--   0        0        0     7841 2023-06-22 07:52:47.265214 gaitmap-2.2.1/gaitmap/trajectory_reconstruction/position_methods/_forward_backwards_integration.py
+-rw-r--r--   0        0        0      243 2023-06-22 07:52:47.265214 gaitmap-2.2.1/gaitmap/trajectory_reconstruction/trajectory_methods/__init__.py
+-rw-r--r--   0        0        0    13664 2023-06-22 07:52:47.265214 gaitmap-2.2.1/gaitmap/trajectory_reconstruction/trajectory_methods/_kalman_numba_funcs.py
+-rw-r--r--   0        0        0    16637 2023-06-22 07:52:47.265214 gaitmap-2.2.1/gaitmap/trajectory_reconstruction/trajectory_methods/_rts_kalman.py
+-rw-r--r--   0        0        0       41 2023-06-22 07:52:47.265214 gaitmap-2.2.1/gaitmap/utils/__init__.py
+-rw-r--r--   0        0        0     1857 2023-06-22 07:52:47.265214 gaitmap-2.2.1/gaitmap/utils/_algo_helper.py
+-rw-r--r--   0        0        0     4695 2023-06-22 07:52:47.265214 gaitmap-2.2.1/gaitmap/utils/_datatype_validation_helper.py
+-rw-r--r--   0        0        0     1195 2023-06-22 07:52:47.265214 gaitmap-2.2.1/gaitmap/utils/_gaitmap_mad.py
+-rw-r--r--   0        0        0      381 2023-06-22 07:52:47.265214 gaitmap-2.2.1/gaitmap/utils/_types.py
+-rw-r--r--   0        0        0    17992 2023-06-22 07:52:47.265214 gaitmap-2.2.1/gaitmap/utils/array_handling.py
+-rw-r--r--   0        0        0     2555 2023-06-22 07:52:47.265214 gaitmap-2.2.1/gaitmap/utils/consts.py
+-rw-r--r--   0        0        0     6284 2023-06-22 07:52:47.265214 gaitmap-2.2.1/gaitmap/utils/coordinate_conversion.py
+-rw-r--r--   0        0        0    48845 2023-06-22 07:52:47.265214 gaitmap-2.2.1/gaitmap/utils/datatype_helper.py
+-rw-r--r--   0        0        0     1089 2023-06-22 07:52:47.265214 gaitmap-2.2.1/gaitmap/utils/exceptions.py
+-rw-r--r--   0        0        0     1865 2023-06-22 07:52:47.265214 gaitmap-2.2.1/gaitmap/utils/fast_quaternion_math.py
+-rw-r--r--   0        0        0    18908 2023-06-22 07:52:47.265214 gaitmap-2.2.1/gaitmap/utils/rotations.py
+-rw-r--r--   0        0        0     2372 2023-06-22 07:52:47.265214 gaitmap-2.2.1/gaitmap/utils/signal_processing.py
+-rw-r--r--   0        0        0    14377 2023-06-22 07:52:47.265214 gaitmap-2.2.1/gaitmap/utils/static_moment_detection.py
+-rw-r--r--   0        0        0     8512 2023-06-22 07:52:47.265214 gaitmap-2.2.1/gaitmap/utils/stride_list_conversion.py
+-rw-r--r--   0        0        0     4115 2023-06-22 07:52:47.265214 gaitmap-2.2.1/gaitmap/utils/vector_math.py
+-rw-r--r--   0        0        0      670 2023-06-22 07:52:47.265214 gaitmap-2.2.1/gaitmap/zupt_detection/__init__.py
+-rw-r--r--   0        0        0     1582 2023-06-22 07:52:47.265214 gaitmap-2.2.1/gaitmap/zupt_detection/_base.py
+-rw-r--r--   0        0        0     3068 2023-06-22 07:52:47.265214 gaitmap-2.2.1/gaitmap/zupt_detection/_combo_zupt_detector.py
+-rw-r--r--   0        0        0    21964 2023-06-22 07:52:47.265214 gaitmap-2.2.1/gaitmap/zupt_detection/_moving_window_zupt_detector.py
+-rw-r--r--   0        0        0     4897 2023-06-22 07:52:47.265214 gaitmap-2.2.1/gaitmap/zupt_detection/_stride_event_zupt_detector.py
+-rw-r--r--   0        0        0     5175 2023-06-22 07:52:47.269214 gaitmap-2.2.1/pyproject.toml
+-rw-r--r--   0        0        0    12012 1970-01-01 00:00:00.000000 gaitmap-2.2.1/PKG-INFO
```

### Comparing `gaitmap-2.2.0/LICENSE` & `gaitmap-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.0/README.md` & `gaitmap-2.2.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -10,47 +10,60 @@
 # gaitmap - The Gait and Movement Analysis Package
 
 *gaitmap* provides a set of algorithms to analyze your IMU movement data (with a focus on foot-worn IMUs) without 
 getting into your way.
 
 - 💻 [20+ Algorithms](https://gaitmap.readthedocs.io/en/latest/modules/index.html) from 17+ publications
 - 📚 Extensive [documentation](https://gaitmap.readthedocs.io/en/latest/)
-- 📝 Build to be [easily extensible](https://gaitmap.readthedocs.io/en/latest/source/user_guide/create_own_algorithm.html)
+- 📝 Build to be [easily extendable](https://gaitmap.readthedocs.io/en/latest/source/user_guide/create_own_algorithm.html)
 - ⚙️ Familiar API inspired by scikit-learn
 - 🤝 Interoperable with the other libraries from the gaitmap ecosystem ([gaitmap-dataset](https://github.com/mad-lab-fau/gaitmap-datasets), [tpcp](https://github.com/mad-lab-fau/tpcp), ...)
 
 **Documentation:** [gaitmap.readthedocs.io](https://gaitmap.readthedocs.io/en/latest/)<br>
-**Learn More about the gaitmap ecosystem:** TODO: Website Link
+**Learn More about the gaitmap ecosystem:** Coming soon!
 
 ## Installation
 
-Gaitmap is split into two packages: `gaitmap` and `gaitmap_mad` ([Learn more](https://gaitmap.readthedocs.io/en/latest/source/user_guide/gaitmap_mad.html).
-To get access to all available algorithms, you need to install both packages.
+Gaitmap is split into two packages: `gaitmap` and `gaitmap_mad` ([Learn more](https://gaitmap.readthedocs.io/en/latest/source/user_guide/gaitmap_mad.html)).
+To get access to all available algorithms, you need to install both packages:
 
-```
+```bash
 pip install gaitmap gaitmap_mad --upgrade
 ```
 
 Both packages are always released together and have the same version number.
 We don't recommend mixing different versions of `gaitmap` and `gaitmap_mad`.
 
 **Note:** gaitmap-mad is published under a AGPL-3.0 license, while gaitmap is published under a MIT license.
 Please, check the [License](#license) section below for more details.
 
 In case you are sure that AGPL-3.0 is compatible with your project, you can install `gaitmap_mad` without any downsides.
 Otherwise, just install `gaitmap` and check the API-docu page of the individual algorithms if they are available in
 `gaitmap` only.
 
+### Installing from Github
+
+If you want to install the latest version from Github, you can use the following command:
+
+```bash
+# For gaitmap
+pip install "git+https://github.com/mad-lab-fau/gaitmap.git" --upgrade
+# For gaitmap_mad
+pip install "git+https://github.com/mad-lab-fau/gaitmap.git#subdirectory=gaitmap_mad"
+```
+
+Note, that we don't guarantee that the latest version on Github is stable.
+
 ### Enabling specific features
 
 #### Hidden Markov Models
 
 To use the HMM (anything imported from `gaitmap.stride_segmentation.hmm`) based algorithms make sure you install `gaitmap` with the `hmm` extra.
 
-```
+```bash
 pip install gaitmap_mad "gaitmap[hmm]" --upgrade
 ```
 This installs the `pomegranate` package, which is the basis for the HMM implementation.
 Note, that we only support the `pomegranate` version `>=0.14.2,<=0.14.6` and that `pomegrante` is not compatible with 
 Python 3.10.
 
 We are working on upgrading to a newer version of `pomegranate`, but this is not a priority at the moment.
@@ -65,17 +78,18 @@
 ## Working with Algorithms
 
 *gaitmap* is designed to be a toolbox and not a single algorithm.
 This means, that you are expected to pick and use individual algorithms.
 
 To get started with *gaitmap* we recommend to follow these steps:
 
-1. Understand the common datatypes we use: [Common Datatypes](https://gaitmap.readthedocs.io/en/latest/source/user_guide/datatypes.html), [Coordinate Systems](https://gaitmap.readthedocs.io/en/latest/source/user_guide/coordinate_systems.html)
-2. Learn how to prepare your own data (or play around with example data): TODO 
-3. Check the API docs and examples for available algorithms: [API Docs](https://gaitmap.readthedocs.io/en/latest/modules/index.html), [Examples](https://gaitmap.readthedocs.io/en/latest/auto_examples/index.html)
+1. Have a look at our example to get an understanding of what *gaitmap* can do: [Example](https://gaitmap.readthedocs.io/en/latest/auto_examples/index.html)
+2. Understand the common datatypes we use: [Common Datatypes](https://gaitmap.readthedocs.io/en/latest/source/user_guide/datatypes.html), [Coordinate Systems](https://gaitmap.readthedocs.io/en/latest/source/user_guide/coordinate_systems.html)
+3. Learn how to prepare your own data (or play around with example data): [Prepare Data](https://gaitmap.readthedocs.io/en/latest/source/user_guide/prepare_data.html) 
+4. Check the API docs and examples for available algorithms: [API Docs](https://gaitmap.readthedocs.io/en/latest/modules/index.html), [Examples](https://gaitmap.readthedocs.io/en/latest/auto_examples/index.html)
 
 Each algorithm is implemented as a class, which is initialized with the required parameters.
 In many cases the default parameters are sufficient, but to get the best results on your data, you should adapt them.
 
 ```python
 from gaitmap.stride_segmentation import BarthDtw
 
@@ -101,24 +115,40 @@
 dtw_warping_path = stride_segmenter.paths_
 ```
 
 To build a full gait analysis pipeline you can combine multiple algorithms ([Example](https://gaitmap.readthedocs.io/en/latest/auto_examples/full_pipelines/mad_gait_pipeline.html#sphx-glr-auto-examples-full-pipelines-mad-gait-pipeline-py)).
 You can even substitute your own algorithms ([Guide](https://gaitmap.readthedocs.io/en/latest/source/user_guide/create_own_algorithm.html)) or use the provided tooling to validate
 and optimize your algorithms using tpcp ([General Guide](https://tpcp.readthedocs.io/en/latest/guides/index.html#optimization-and-validation), [Example](https://gaitmap.readthedocs.io/en/latest/auto_examples/datasets_and_pipelines/gridsearch.html#sphx-glr-auto-examples-datasets-and-pipelines-gridsearch-py)).
 
+## Contributing
+
+**We want to hear from you (and we want your algorithms)!**
+
+👍 We are always happy to receive feedback and contributions.
+If you run into any issues or have any questions, please open an [issue on Github](https://github.com/mad-lab-fau/gaitmap/issues)
+or start a [discussions](https://github.com/mad-lab-fau/gaitmap/discussions/).
+
+📚 If you are using *gaitmap* in your research or project, we would love to hear about it and link your work here! The [show and tell section](https://github.com/mad-lab-fau/gaitmap/discussions/categories/show-and-tell)
+in the discussions is a great place for this.
+
+💻 And most importantly, we want your algorithms!
+If you have an algorithm that you think would be a good fit for *gaitmap*, open an issue, and we can discuss how to integrate it.
+We are happy to help you with the integration process.
+Even if you are not confident in your Python skills, we can discuss ways to get your algorithm into *gaitmap*.
+
+For all these topics check out our [contributing guide](https://gaitmap.readthedocs.io/en/latest/source/user_guide/contributing.html) for more details.
+
 ## Citation
 
 If you use *gaitmap* in your research we would appreciate a citation.
 This helps us to justify the time we invest in the development and maintenance of the library.
 
 We currently prepare a paper to describe the *gaitmap* library in detail.
 Until then, please simply cite the repository.
 
-
-
 If you use a specific algorithm please also make sure you cite the original paper of the algorithm!
 We recommend the following citation style:
 
 *We used the algorithm proposed by Author et al. [paper-citation], implemented by the Gaitmap package [gaitmap-citation].*
 
 ## License
```

### Comparing `gaitmap-2.2.0/gaitmap/_event_detection_common/_event_detection_mixin.py` & `gaitmap-2.2.1/gaitmap/_event_detection_common/_event_detection_mixin.py`

 * *Files 4% similar despite different names*

```diff
@@ -91,16 +91,14 @@
                     data[sensor],
                     stride_list[sensor],
                     detect_kwargs=detect_kwargs,
                     memory=self.memory,
                 )
             results = invert_result_dictionary(results_dict)
 
-        # do not set min_vel_event_list_ if consistency is not enforced as it would be completely scrambeled
-        # and can not be used for anything anyway
         if not self.enforce_consistency:
             results.pop("min_vel_event_list", None)
         set_params_from_dict(self, results, result_formatting=True)
         return self
 
     def _detect_single_dataset(
         self,
@@ -139,25 +137,31 @@
 
         if self.enforce_consistency:
             # check for consistency, remove inconsistent strides
             segmented_event_list, _ = enforce_stride_list_consistency(
                 segmented_event_list, stride_type="segmented", check_stride_list=False
             )
 
-        if "min_vel" not in events:
+        if "min_vel" not in events or self.enforce_consistency is False:
+            # do not set min_vel_event_list_ if consistency is not enforced as it would be completely scrambled
+            # and can not be used for anything anyway
             return {"segmented_event_list": segmented_event_list}
 
         # convert to min_vel event list
         min_vel_event_list, _ = _segmented_stride_list_to_min_vel_single_sensor(
             segmented_event_list, target_stride_type="min_vel"
         )
 
         output_order = [c for c in ["start", "end", "ic", "tc", "min_vel", "pre_ic"] if c in min_vel_event_list.columns]
 
-        min_vel_event_list = min_vel_event_list[output_order]
+        # We enforce consistency again here, as a valid segmented stride list does not necessarily result in a valid
+        # min_vel stride list
+        min_vel_event_list, _ = enforce_stride_list_consistency(
+            min_vel_event_list[output_order], stride_type="min_vel", check_stride_list=False
+        )
 
         return {"min_vel_event_list": min_vel_event_list, "segmented_event_list": segmented_event_list}
 
     def _select_all_event_detection_method(self) -> Callable:
         """Select the function to calculate the all events.
 
         This is separate method to make it easy to overwrite by a subclass.
```

### Comparing `gaitmap-2.2.0/gaitmap/base.py` & `gaitmap-2.2.1/gaitmap/base.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.0/gaitmap/data_transform/__init__.py` & `gaitmap-2.2.1/gaitmap/data_transform/__init__.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.0/gaitmap/data_transform/_base.py` & `gaitmap-2.2.1/gaitmap/data_transform/_base.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.0/gaitmap/data_transform/_feature_transform.py` & `gaitmap-2.2.1/gaitmap/data_transform/_feature_transform.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.0/gaitmap/data_transform/_filter.py` & `gaitmap-2.2.1/gaitmap/data_transform/_filter.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.0/gaitmap/data_transform/_scaler.py` & `gaitmap-2.2.1/gaitmap/data_transform/_scaler.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.0/gaitmap/evaluation_utils/__init__.py` & `gaitmap-2.2.1/gaitmap/evaluation_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.0/gaitmap/evaluation_utils/event_detection.py` & `gaitmap-2.2.1/gaitmap/evaluation_utils/event_detection.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.0/gaitmap/evaluation_utils/parameter_errors.py` & `gaitmap-2.2.1/gaitmap/evaluation_utils/parameter_errors.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.0/gaitmap/evaluation_utils/scores.py` & `gaitmap-2.2.1/gaitmap/evaluation_utils/scores.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.0/gaitmap/evaluation_utils/stride_segmentation.py` & `gaitmap-2.2.1/gaitmap/evaluation_utils/stride_segmentation.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.0/gaitmap/event_detection/__init__.py` & `gaitmap-2.2.1/gaitmap/event_detection/__init__.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.0/gaitmap/event_detection/_herzer_event_detection.py` & `gaitmap-2.2.1/gaitmap/event_detection/_herzer_event_detection.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.0/gaitmap/example_data.py` & `gaitmap-2.2.1/gaitmap/example_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,17 +9,15 @@
 
 from pathlib import Path
 
 import pandas as pd
 
 LOCAL_EXAMPLE_PATH = Path(__file__).parent.parent / "example_data/"
 PC_EXAMPLE_PATH = Path.home() / ".gaitmap_data/"
-GITHUB_FOLDER_PATH = (
-    "https://github.com/mad-lab-fau/gaitmap/tree/master/example_data/{}"
-)
+GITHUB_FOLDER_PATH = "https://github.com/mad-lab-fau/gaitmap/tree/master/example_data/{}"
 
 
 def _is_manual_installed() -> bool:
     return (LOCAL_EXAMPLE_PATH / "__init__.py").is_file()
 
 
 def _get_data(filename: str) -> str:
```

### Comparing `gaitmap-2.2.0/gaitmap/gait_detection/__init__.py` & `gaitmap-2.2.1/gaitmap/gait_detection/__init__.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.0/gaitmap/parameters/_spatial_parameters.py` & `gaitmap-2.2.1/gaitmap/parameters/_spatial_parameters.py`

 * *Files 0% similar despite different names*

```diff
@@ -124,15 +124,15 @@
        (pp. 5424-5427). IEEE.
     .. [2] Rampp, A., Barth, J., Schülein, S., Gaßmann, K. G., Klucken, J., & Eskofier, B. M. (2014).
        Inertial sensor-based stride parameter calculation from gait sequences in geriatric patients.
        IEEE transactions on biomedical engineering, 62(4), 1089-1097.
 
     Examples
     --------
-    This method requires the output of a event detection method and a full trajectory reconstruction
+    This method requires the output of an event detection method and a full trajectory reconstruction
     (orientation and position) as input.
 
     >>> stride_list = ...  # from event detection
     >>> positions = ...  # from position estimation
     >>> orientations = ...  # from orientation estimation
     >>> spatial_paras = SpatialParameterCalculation()
     >>> spatial_paras = spatial_paras.calculate(
```

### Comparing `gaitmap-2.2.0/gaitmap/parameters/_temporal_parameters.py` & `gaitmap-2.2.1/gaitmap/parameters/_temporal_parameters.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 Self = TypeVar("Self", bound="TemporalParameterCalculation")
 
 
 class TemporalParameterCalculation(BaseTemporalParameterCalculation):
     """Calculat temporal parameters of strides based on detected gait events.
 
     For details on the individual parameters see the Notes section.
+    Calculations are based on [1]_.
 
     Parameters
     ----------
     expected_stride_type
         The expected stride type of the stride list.
         This changes how the temporal parameters are calculated.
         This can either be "min_vel" or "ic".
@@ -56,14 +57,19 @@
         For a `min_vel`-stride this is the time between "tc" and "ic"
         For a `ic`-stride this is the time between "tc" and "end".
     stance_time [s]
         The stance time is the time the foot is on the ground.
         Hence, it is the time from a ic to the next tc.
         For both stride types this is calculated as stride_time - swing_time.
 
+    .. [1] A. Rampp, J. Barth, S. Schuelein, K.-G. Gassmann, J. Klucken, and B. M. Eskofier, “Inertial Sensor-Based
+       Stride Parameter Calculation From Gait Sequences in Geriatric Patients,” IEEE Transactions on Biomedical
+       Engineering, vol. 62, no. 4, pp. 1089-1097, Apr. 2015. [Online].
+       Available: http://ieeexplore.ieee.org/document/6949634/
+
     Examples
     --------
     This method requires the output of a event detection method as input.
 
     >>> stride_list = ... #  from event detection
     >>> temporal_paras = TemporalParameterCalculation()
     >>> temporal_paras = temporal_paras.calculate(stride_event_list=stride_list, sampling_rate_hz=204.8)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `gaitmap-2.2.0/gaitmap/preprocessing/sensor_alignment/__init__.py` & `gaitmap-2.2.1/gaitmap/preprocessing/sensor_alignment/__init__.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.0/gaitmap/preprocessing/sensor_alignment/_gravity_alignment.py` & `gaitmap-2.2.1/gaitmap/preprocessing/sensor_alignment/_gravity_alignment.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.0/gaitmap/preprocessing/sensor_alignment/_mulisensor_alignment.py` & `gaitmap-2.2.1/gaitmap/preprocessing/sensor_alignment/_mulisensor_alignment.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.0/gaitmap/preprocessing/sensor_alignment/_pca_alignment.py` & `gaitmap-2.2.1/gaitmap/preprocessing/sensor_alignment/_pca_alignment.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,14 +71,16 @@
     The Principle Component Analysis (PCA) can be used to determin the coordinate plane where the main movement
     component is located, which corresponds to the main component of the PCA after fitting to the provided data. This
     is typically intended to align one axis of the sensor frame to the foot medio-lateral axis. The ML-axis is therefore
     assumed to correspond to the principle component with the highest explained variance within the 2D projection
     ("birds eye view") of the X-Y sensor frame. To ensure a 2D problem the dataset should be aligned roughly to gravity
     beforhand so we can assume a fixed z-axis of [0,0,1] and solve the alignment as a pure heading issue.
 
+    This approach is inspired by [1]_
+
     Parameters
     ----------
     target_axis
         axis to which the main component found by the pca analysis will be aligned e.g. "y"
     pca_plane_axis
         list of axis names which span the 2D-plane where the pca will be performed e.g. ("gyr_x","gyr_y"). Note: the
         order of the axis defining the pca plane will influence also your target axis! So best keep a x-y order.
@@ -110,14 +112,18 @@
     ...
 
     Notes
     -----
     The PCA is sign invariant this means only an alignment to the medio-lateral plane will be performend! An additional
     180deg flip of the coordinate system might be still necessary after the PCA alignment!
 
+    .. [1] W. Kong, S. Sessa, M. Zecca, and A. Takanishi, “Anatomical Calibration through Post-Processing of Standard
+           Motion Tests Data,” Sensors, vol. 16, no. 12, p. 2011, Dec. 2016. [Online]. Available:
+           https://www.mdpi.com/1424-8220/16/12/2011
+
 
     See Also
     --------
     sklearn.decomposition.PCA: Details on the used PCA implementation for this method.
     gaitmap.preprocessing.sensor_alignment.ForwardDirectionSignAlignment: Alignment of the forward direction after
                                                                           PCA Alignment
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `gaitmap-2.2.0/gaitmap/stride_segmentation/__init__.py` & `gaitmap-2.2.1/gaitmap/stride_segmentation/__init__.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.0/gaitmap/stride_segmentation/_roi_stride_segmentation.py` & `gaitmap-2.2.1/gaitmap/stride_segmentation/_roi_stride_segmentation.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.0/gaitmap/stride_segmentation/_utils.py` & `gaitmap-2.2.1/gaitmap/stride_segmentation/_utils.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.0/gaitmap/stride_segmentation/hmm.py` & `gaitmap-2.2.1/gaitmap/stride_segmentation/hmm.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.0/gaitmap/trajectory_reconstruction/__init__.py` & `gaitmap-2.2.1/gaitmap/trajectory_reconstruction/__init__.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.0/gaitmap/trajectory_reconstruction/_region_level_trajectory.py` & `gaitmap-2.2.1/gaitmap/trajectory_reconstruction/_region_level_trajectory.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.0/gaitmap/trajectory_reconstruction/_stride_level_trajectory.py` & `gaitmap-2.2.1/gaitmap/trajectory_reconstruction/_stride_level_trajectory.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.0/gaitmap/trajectory_reconstruction/_trajectory_wrapper.py` & `gaitmap-2.2.1/gaitmap/trajectory_reconstruction/_trajectory_wrapper.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.0/gaitmap/trajectory_reconstruction/orientation_methods/_madgwick.py` & `gaitmap-2.2.1/gaitmap/trajectory_reconstruction/orientation_methods/_madgwick.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.0/gaitmap/trajectory_reconstruction/orientation_methods/_simple_gyro_integration.py` & `gaitmap-2.2.1/gaitmap/trajectory_reconstruction/orientation_methods/_simple_gyro_integration.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.0/gaitmap/trajectory_reconstruction/position_methods/__init__.py` & `gaitmap-2.2.1/gaitmap/trajectory_reconstruction/position_methods/__init__.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.0/gaitmap/trajectory_reconstruction/position_methods/_forward_backwards_integration.py` & `gaitmap-2.2.1/gaitmap/trajectory_reconstruction/position_methods/_forward_backwards_integration.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     This means we assume no movement (zero velocity and zero acceleration except gravity) at the beginning and end of
     the signal.
 
     Further drift correction is applied using a level-assumption (i.e. we assume that the sensor starts and ends its
     movement at the same z-position/height).
     If this assumption is not true for your usecase, you can disable it using the `level_assumption` parameter.
 
-    Implementation based on the paper by Hannink et al. [1]_.
+    Implementation based on the paper by Hannink et al. [1]_ and Zok et al. [2]_.
 
     Parameters
     ----------
     turning_point
         The point at which the sigmoid weighting function has a value of 0.5 and therefore forward and backward
         integrals are weighted 50/50. Specified as percentage of the signal length (0.0 < turning_point <= 1.0).
     steepness
@@ -62,14 +62,18 @@
         The sampling rate of the data.
 
     Notes
     -----
     .. [1] Hannink, J., Ollenschläger, M., Kluge, F., Roth, N., Klucken, J., and Eskofier, B. M. 2017. Benchmarking Foot
        Trajectory Estimation Methods for Mobile Gait Analysis. Sensors (Basel, Switzerland) 17, 9.
        https://doi.org/10.3390/s17091940
+    .. [2] M. Zok, C. Mazz`a, and U. Della Croce, “Total body centre of mass displacement estimated using ground
+       reactions during transitory motor tasks: Application to step ascent,” Medical Engineering & Physics, vol. 26,
+       no. 9, pp. 791-798, Nov. 2004. [Online]. Available:
+       https://linkinghub.elsevier.com/retrieve/pii/S1350453304001195
 
     Examples
     --------
     Your data must be a pd.DataFrame with at least columns defined by :obj:`~gaitmap.utils.consts.SF_ACC`.
     Remember, that this method does not transform your data into another coordinate frame, but just integrates it.
     If you want to use this method to calculate e.g. a stride length, make sure to cenvert your data into the global
     frame using any of the implemented orientation estimation methods.
```

### Comparing `gaitmap-2.2.0/gaitmap/trajectory_reconstruction/trajectory_methods/_kalman_numba_funcs.py` & `gaitmap-2.2.1/gaitmap/trajectory_reconstruction/trajectory_methods/_kalman_numba_funcs.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.0/gaitmap/trajectory_reconstruction/trajectory_methods/_rts_kalman.py` & `gaitmap-2.2.1/gaitmap/trajectory_reconstruction/trajectory_methods/_rts_kalman.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.0/gaitmap/utils/_algo_helper.py` & `gaitmap-2.2.1/gaitmap/utils/_algo_helper.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.0/gaitmap/utils/_datatype_validation_helper.py` & `gaitmap-2.2.1/gaitmap/utils/_datatype_validation_helper.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.0/gaitmap/utils/_gaitmap_mad.py` & `gaitmap-2.2.1/gaitmap/utils/_gaitmap_mad.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,17 @@
 def patch_gaitmap_mad_import(_gaitmap_mad_modules, current_module_name):
     """Check if the gaitmap_mad module is available and return a patched getattr method if not."""
     if find_spec("gaitmap_mad"):
         import gaitmap_mad  # pylint: disable=import-outside-toplevel
 
         assert (gm_version := gaitmap_mad.__version__) == (g_version := gaitmap.__version__), (
             "We only support using the exact same version of `gaitmap` and `gaitmap_mad`. "
-            f"Currently you have the versions `gaitmap`: v{g_version} and `gaitmap_mad`: v{gm_version}."
+            f"Currently you have the versions `gaitmap`: v{g_version} and `gaitmap_mad`: v{gm_version}. "
+            "Update the `gaitmap` and `gaitmap_mad` packages to the same version (likely you just forgot to update "
+            "`gaitmap_mad` when you updated `gaitmap`)."
         )
         return None
     from gaitmap.utils.exceptions import GaitmapMadImportError  # pylint: disable=import-outside-toplevel
 
     def new_getattr(name: str):
         if name in _gaitmap_mad_modules:
             raise GaitmapMadImportError(name, current_module_name)
```

### Comparing `gaitmap-2.2.0/gaitmap/utils/array_handling.py` & `gaitmap-2.2.1/gaitmap/utils/array_handling.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.0/gaitmap/utils/consts.py` & `gaitmap-2.2.1/gaitmap/utils/consts.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.0/gaitmap/utils/coordinate_conversion.py` & `gaitmap-2.2.1/gaitmap/utils/coordinate_conversion.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.0/gaitmap/utils/datatype_helper.py` & `gaitmap-2.2.1/gaitmap/utils/datatype_helper.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.0/gaitmap/utils/exceptions.py` & `gaitmap-2.2.1/gaitmap/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.0/gaitmap/utils/fast_quaternion_math.py` & `gaitmap-2.2.1/gaitmap/utils/fast_quaternion_math.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.0/gaitmap/utils/rotations.py` & `gaitmap-2.2.1/gaitmap/utils/rotations.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.0/gaitmap/utils/signal_processing.py` & `gaitmap-2.2.1/gaitmap/utils/signal_processing.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.0/gaitmap/utils/static_moment_detection.py` & `gaitmap-2.2.1/gaitmap/utils/static_moment_detection.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.0/gaitmap/utils/stride_list_conversion.py` & `gaitmap-2.2.1/gaitmap/utils/stride_list_conversion.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.0/gaitmap/utils/vector_math.py` & `gaitmap-2.2.1/gaitmap/utils/vector_math.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.0/gaitmap/zupt_detection/__init__.py` & `gaitmap-2.2.1/gaitmap/zupt_detection/__init__.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.0/gaitmap/zupt_detection/_base.py` & `gaitmap-2.2.1/gaitmap/zupt_detection/_base.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.0/gaitmap/zupt_detection/_combo_zupt_detector.py` & `gaitmap-2.2.1/gaitmap/zupt_detection/_combo_zupt_detector.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.0/gaitmap/zupt_detection/_moving_window_zupt_detector.py` & `gaitmap-2.2.1/gaitmap/zupt_detection/_moving_window_zupt_detector.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.0/gaitmap/zupt_detection/_stride_event_zupt_detector.py` & `gaitmap-2.2.1/gaitmap/zupt_detection/_stride_event_zupt_detector.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.0/pyproject.toml` & `gaitmap-2.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gaitmap"
-version = "2.2.0"
+version = "2.2.1"
 description = "The Gait and Movement Analysis Package - Your definite guide to reliable IMU based human movement analysis."
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/mad-lab-fau/gaitmap"
 repository = "https://github.com/mad-lab-fau/gaitmap"
 authors = [
     "Arne Küderle <arne.kuederle@fau.de>",
```

### Comparing `gaitmap-2.2.0/PKG-INFO` & `gaitmap-2.2.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaitmap
-Version: 2.2.0
+Version: 2.2.1
 Summary: The Gait and Movement Analysis Package - Your definite guide to reliable IMU based human movement analysis.
 Home-page: https://github.com/mad-lab-fau/gaitmap
 License: MIT
 Author: Arne Küderle
 Author-email: arne.kuederle@fau.de
 Requires-Python: >=3.8.0,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -42,47 +42,60 @@
 # gaitmap - The Gait and Movement Analysis Package
 
 *gaitmap* provides a set of algorithms to analyze your IMU movement data (with a focus on foot-worn IMUs) without 
 getting into your way.
 
 - 💻 [20+ Algorithms](https://gaitmap.readthedocs.io/en/latest/modules/index.html) from 17+ publications
 - 📚 Extensive [documentation](https://gaitmap.readthedocs.io/en/latest/)
-- 📝 Build to be [easily extensible](https://gaitmap.readthedocs.io/en/latest/source/user_guide/create_own_algorithm.html)
+- 📝 Build to be [easily extendable](https://gaitmap.readthedocs.io/en/latest/source/user_guide/create_own_algorithm.html)
 - ⚙️ Familiar API inspired by scikit-learn
 - 🤝 Interoperable with the other libraries from the gaitmap ecosystem ([gaitmap-dataset](https://github.com/mad-lab-fau/gaitmap-datasets), [tpcp](https://github.com/mad-lab-fau/tpcp), ...)
 
 **Documentation:** [gaitmap.readthedocs.io](https://gaitmap.readthedocs.io/en/latest/)<br>
-**Learn More about the gaitmap ecosystem:** TODO: Website Link
+**Learn More about the gaitmap ecosystem:** Coming soon!
 
 ## Installation
 
-Gaitmap is split into two packages: `gaitmap` and `gaitmap_mad` ([Learn more](https://gaitmap.readthedocs.io/en/latest/source/user_guide/gaitmap_mad.html).
-To get access to all available algorithms, you need to install both packages.
+Gaitmap is split into two packages: `gaitmap` and `gaitmap_mad` ([Learn more](https://gaitmap.readthedocs.io/en/latest/source/user_guide/gaitmap_mad.html)).
+To get access to all available algorithms, you need to install both packages:
 
-```
+```bash
 pip install gaitmap gaitmap_mad --upgrade
 ```
 
 Both packages are always released together and have the same version number.
 We don't recommend mixing different versions of `gaitmap` and `gaitmap_mad`.
 
 **Note:** gaitmap-mad is published under a AGPL-3.0 license, while gaitmap is published under a MIT license.
 Please, check the [License](#license) section below for more details.
 
 In case you are sure that AGPL-3.0 is compatible with your project, you can install `gaitmap_mad` without any downsides.
 Otherwise, just install `gaitmap` and check the API-docu page of the individual algorithms if they are available in
 `gaitmap` only.
 
+### Installing from Github
+
+If you want to install the latest version from Github, you can use the following command:
+
+```bash
+# For gaitmap
+pip install "git+https://github.com/mad-lab-fau/gaitmap.git" --upgrade
+# For gaitmap_mad
+pip install "git+https://github.com/mad-lab-fau/gaitmap.git#subdirectory=gaitmap_mad"
+```
+
+Note, that we don't guarantee that the latest version on Github is stable.
+
 ### Enabling specific features
 
 #### Hidden Markov Models
 
 To use the HMM (anything imported from `gaitmap.stride_segmentation.hmm`) based algorithms make sure you install `gaitmap` with the `hmm` extra.
 
-```
+```bash
 pip install gaitmap_mad "gaitmap[hmm]" --upgrade
 ```
 This installs the `pomegranate` package, which is the basis for the HMM implementation.
 Note, that we only support the `pomegranate` version `>=0.14.2,<=0.14.6` and that `pomegrante` is not compatible with 
 Python 3.10.
 
 We are working on upgrading to a newer version of `pomegranate`, but this is not a priority at the moment.
@@ -97,17 +110,18 @@
 ## Working with Algorithms
 
 *gaitmap* is designed to be a toolbox and not a single algorithm.
 This means, that you are expected to pick and use individual algorithms.
 
 To get started with *gaitmap* we recommend to follow these steps:
 
-1. Understand the common datatypes we use: [Common Datatypes](https://gaitmap.readthedocs.io/en/latest/source/user_guide/datatypes.html), [Coordinate Systems](https://gaitmap.readthedocs.io/en/latest/source/user_guide/coordinate_systems.html)
-2. Learn how to prepare your own data (or play around with example data): TODO 
-3. Check the API docs and examples for available algorithms: [API Docs](https://gaitmap.readthedocs.io/en/latest/modules/index.html), [Examples](https://gaitmap.readthedocs.io/en/latest/auto_examples/index.html)
+1. Have a look at our example to get an understanding of what *gaitmap* can do: [Example](https://gaitmap.readthedocs.io/en/latest/auto_examples/index.html)
+2. Understand the common datatypes we use: [Common Datatypes](https://gaitmap.readthedocs.io/en/latest/source/user_guide/datatypes.html), [Coordinate Systems](https://gaitmap.readthedocs.io/en/latest/source/user_guide/coordinate_systems.html)
+3. Learn how to prepare your own data (or play around with example data): [Prepare Data](https://gaitmap.readthedocs.io/en/latest/source/user_guide/prepare_data.html) 
+4. Check the API docs and examples for available algorithms: [API Docs](https://gaitmap.readthedocs.io/en/latest/modules/index.html), [Examples](https://gaitmap.readthedocs.io/en/latest/auto_examples/index.html)
 
 Each algorithm is implemented as a class, which is initialized with the required parameters.
 In many cases the default parameters are sufficient, but to get the best results on your data, you should adapt them.
 
 ```python
 from gaitmap.stride_segmentation import BarthDtw
 
@@ -133,24 +147,40 @@
 dtw_warping_path = stride_segmenter.paths_
 ```
 
 To build a full gait analysis pipeline you can combine multiple algorithms ([Example](https://gaitmap.readthedocs.io/en/latest/auto_examples/full_pipelines/mad_gait_pipeline.html#sphx-glr-auto-examples-full-pipelines-mad-gait-pipeline-py)).
 You can even substitute your own algorithms ([Guide](https://gaitmap.readthedocs.io/en/latest/source/user_guide/create_own_algorithm.html)) or use the provided tooling to validate
 and optimize your algorithms using tpcp ([General Guide](https://tpcp.readthedocs.io/en/latest/guides/index.html#optimization-and-validation), [Example](https://gaitmap.readthedocs.io/en/latest/auto_examples/datasets_and_pipelines/gridsearch.html#sphx-glr-auto-examples-datasets-and-pipelines-gridsearch-py)).
 
+## Contributing
+
+**We want to hear from you (and we want your algorithms)!**
+
+👍 We are always happy to receive feedback and contributions.
+If you run into any issues or have any questions, please open an [issue on Github](https://github.com/mad-lab-fau/gaitmap/issues)
+or start a [discussions](https://github.com/mad-lab-fau/gaitmap/discussions/).
+
+📚 If you are using *gaitmap* in your research or project, we would love to hear about it and link your work here! The [show and tell section](https://github.com/mad-lab-fau/gaitmap/discussions/categories/show-and-tell)
+in the discussions is a great place for this.
+
+💻 And most importantly, we want your algorithms!
+If you have an algorithm that you think would be a good fit for *gaitmap*, open an issue, and we can discuss how to integrate it.
+We are happy to help you with the integration process.
+Even if you are not confident in your Python skills, we can discuss ways to get your algorithm into *gaitmap*.
+
+For all these topics check out our [contributing guide](https://gaitmap.readthedocs.io/en/latest/source/user_guide/contributing.html) for more details.
+
 ## Citation
 
 If you use *gaitmap* in your research we would appreciate a citation.
 This helps us to justify the time we invest in the development and maintenance of the library.
 
 We currently prepare a paper to describe the *gaitmap* library in detail.
 Until then, please simply cite the repository.
 
-
-
 If you use a specific algorithm please also make sure you cite the original paper of the algorithm!
 We recommend the following citation style:
 
 *We used the algorithm proposed by Author et al. [paper-citation], implemented by the Gaitmap package [gaitmap-citation].*
 
 ## License
```

