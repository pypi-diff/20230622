# Comparing `tmp/gaitmap_mad-2.2.0.tar.gz` & `tmp/gaitmap_mad-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gaitmap_mad-2.2.0.tar", max compression
+gzip compressed data, was "gaitmap_mad-2.2.1.tar", max compression
```

## Comparing `gaitmap_mad-2.2.0.tar` & `gaitmap_mad-2.2.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0      734 2023-06-07 10:17:51.589924 gaitmap_mad-2.2.0/LICENSE
--rw-r--r--   0        0        0      597 2023-06-07 10:17:51.589924 gaitmap_mad-2.2.0/README.md
--rw-r--r--   0        0        0      481 2023-06-07 10:17:51.589924 gaitmap_mad-2.2.0/gaitmap_mad/__init__.py
--rw-r--r--   0        0        0      441 2023-06-07 10:17:51.589924 gaitmap_mad-2.2.0/gaitmap_mad/event_detection/__init__.py
--rw-r--r--   0        0        0     6013 2023-06-07 10:17:51.589924 gaitmap_mad-2.2.0/gaitmap_mad/event_detection/_filtered_rampp_event_detection.py
--rw-r--r--   0        0        0    14317 2023-06-07 10:17:51.589924 gaitmap_mad-2.2.0/gaitmap_mad/event_detection/_rampp_event_detection.py
--rw-r--r--   0        0        0      340 2023-06-07 10:17:51.589924 gaitmap_mad-2.2.0/gaitmap_mad/gait_detection/__init__.py
--rw-r--r--   0        0        0    24779 2023-06-07 10:17:51.589924 gaitmap_mad-2.2.0/gaitmap_mad/gait_detection/_ullrich_gait_sequence_detection.py
--rw-r--r--   0        0        0      117 2023-06-07 10:17:51.589924 gaitmap_mad-2.2.0/gaitmap_mad/preprocessing/__init__.py
--rw-r--r--   0        0        0      234 2023-06-07 10:17:51.589924 gaitmap_mad-2.2.0/gaitmap_mad/preprocessing/sensor_alignment/__init__.py
--rw-r--r--   0        0        0    12666 2023-06-07 10:17:51.589924 gaitmap_mad-2.2.0/gaitmap_mad/preprocessing/sensor_alignment/_forward_direction_alignment.py
--rw-r--r--   0        0        0     1114 2023-06-07 10:17:51.589924 gaitmap_mad-2.2.0/gaitmap_mad/stride_segmentation/__init__.py
--rw-r--r--   0        0        0      813 2023-06-07 10:17:51.589924 gaitmap_mad-2.2.0/gaitmap_mad/stride_segmentation/dtw/__init__.py
--rw-r--r--   0        0        0    15170 2023-06-07 10:17:51.589924 gaitmap_mad-2.2.0/gaitmap_mad/stride_segmentation/dtw/_barth_dtw.py
--rw-r--r--   0        0        0    36773 2023-06-07 10:17:51.589924 gaitmap_mad-2.2.0/gaitmap_mad/stride_segmentation/dtw/_base_dtw.py
--rw-r--r--   0        0        0     8568 2023-06-07 10:17:51.589924 gaitmap_mad-2.2.0/gaitmap_mad/stride_segmentation/dtw/_constrained_barth_dtw.py
--rw-r--r--   0        0        0      436 2023-06-07 10:17:51.589924 gaitmap_mad-2.2.0/gaitmap_mad/stride_segmentation/dtw/_dtw_templates/__init__.py
--rw-r--r--   0        0        0     7513 2023-06-07 10:17:51.589924 gaitmap_mad-2.2.0/gaitmap_mad/stride_segmentation/dtw/_dtw_templates/barth_original_template.csv
--rw-r--r--   0        0        0    15956 2023-06-07 10:17:51.589924 gaitmap_mad-2.2.0/gaitmap_mad/stride_segmentation/dtw/_dtw_templates/templates.py
--rw-r--r--   0        0        0     3589 2023-06-07 10:17:51.589924 gaitmap_mad-2.2.0/gaitmap_mad/stride_segmentation/dtw/_vendored_tslearn.py
--rw-r--r--   0        0        0     1182 2023-06-07 10:17:51.589924 gaitmap_mad-2.2.0/gaitmap_mad/stride_segmentation/hmm/__init__.py
--rw-r--r--   0        0        0    10922 2023-06-07 10:17:51.589924 gaitmap_mad-2.2.0/gaitmap_mad/stride_segmentation/hmm/_hmm_feature_transform.py
--rw-r--r--   0        0        0    12026 2023-06-07 10:17:51.593924 gaitmap_mad-2.2.0/gaitmap_mad/stride_segmentation/hmm/_hmm_stride_segmentation.py
--rw-r--r--   0        0        0        0 2023-06-07 10:17:51.593924 gaitmap_mad-2.2.0/gaitmap_mad/stride_segmentation/hmm/_pre_trained_models/__init__.py
--rw-r--r--   0        0        0   397824 2023-06-07 10:17:51.593924 gaitmap_mad-2.2.0/gaitmap_mad/stride_segmentation/hmm/_pre_trained_models/fallriskpd_at_lab_model.json
--rw-r--r--   0        0        0    27197 2023-06-07 10:17:51.593924 gaitmap_mad-2.2.0/gaitmap_mad/stride_segmentation/hmm/_segmentation_model.py
--rw-r--r--   0        0        0    19087 2023-06-07 10:17:51.593924 gaitmap_mad-2.2.0/gaitmap_mad/stride_segmentation/hmm/_simple_model.py
--rw-r--r--   0        0        0    26902 2023-06-07 10:17:51.593924 gaitmap_mad-2.2.0/gaitmap_mad/stride_segmentation/hmm/_utils.py
--rw-r--r--   0        0        0      265 2023-06-07 10:17:51.593924 gaitmap_mad-2.2.0/gaitmap_mad/trajectory_reconstruction/__init__.py
--rw-r--r--   0        0        0      263 2023-06-07 10:17:51.593924 gaitmap_mad-2.2.0/gaitmap_mad/trajectory_reconstruction/position_methods/__init__.py
--rw-r--r--   0        0        0     9877 2023-06-07 10:17:51.593924 gaitmap_mad-2.2.0/gaitmap_mad/trajectory_reconstruction/position_methods/_piece_wise_linear_dedrifted_integration.py
--rw-r--r--   0        0        0      589 2023-06-07 10:17:51.593924 gaitmap_mad-2.2.0/pyproject.toml
--rw-r--r--   0        0        0     1295 1970-01-01 00:00:00.000000 gaitmap_mad-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0      734 2023-06-22 07:52:46.365652 gaitmap_mad-2.2.1/LICENSE
+-rw-r--r--   0        0        0      597 2023-06-22 07:52:46.365652 gaitmap_mad-2.2.1/README.md
+-rw-r--r--   0        0        0      481 2023-06-22 07:52:46.365652 gaitmap_mad-2.2.1/gaitmap_mad/__init__.py
+-rw-r--r--   0        0        0      441 2023-06-22 07:52:46.365652 gaitmap_mad-2.2.1/gaitmap_mad/event_detection/__init__.py
+-rw-r--r--   0        0        0     6013 2023-06-22 07:52:46.369652 gaitmap_mad-2.2.1/gaitmap_mad/event_detection/_filtered_rampp_event_detection.py
+-rw-r--r--   0        0        0    14317 2023-06-22 07:52:46.369652 gaitmap_mad-2.2.1/gaitmap_mad/event_detection/_rampp_event_detection.py
+-rw-r--r--   0        0        0      340 2023-06-22 07:52:46.369652 gaitmap_mad-2.2.1/gaitmap_mad/gait_detection/__init__.py
+-rw-r--r--   0        0        0    24779 2023-06-22 07:52:46.369652 gaitmap_mad-2.2.1/gaitmap_mad/gait_detection/_ullrich_gait_sequence_detection.py
+-rw-r--r--   0        0        0      117 2023-06-22 07:52:46.369652 gaitmap_mad-2.2.1/gaitmap_mad/preprocessing/__init__.py
+-rw-r--r--   0        0        0      234 2023-06-22 07:52:46.369652 gaitmap_mad-2.2.1/gaitmap_mad/preprocessing/sensor_alignment/__init__.py
+-rw-r--r--   0        0        0    12666 2023-06-22 07:52:46.369652 gaitmap_mad-2.2.1/gaitmap_mad/preprocessing/sensor_alignment/_forward_direction_alignment.py
+-rw-r--r--   0        0        0     1114 2023-06-22 07:52:46.369652 gaitmap_mad-2.2.1/gaitmap_mad/stride_segmentation/__init__.py
+-rw-r--r--   0        0        0      813 2023-06-22 07:52:46.369652 gaitmap_mad-2.2.1/gaitmap_mad/stride_segmentation/dtw/__init__.py
+-rw-r--r--   0        0        0    15216 2023-06-22 07:52:46.369652 gaitmap_mad-2.2.1/gaitmap_mad/stride_segmentation/dtw/_barth_dtw.py
+-rw-r--r--   0        0        0    36773 2023-06-22 07:52:46.369652 gaitmap_mad-2.2.1/gaitmap_mad/stride_segmentation/dtw/_base_dtw.py
+-rw-r--r--   0        0        0     8809 2023-06-22 07:52:46.369652 gaitmap_mad-2.2.1/gaitmap_mad/stride_segmentation/dtw/_constrained_barth_dtw.py
+-rw-r--r--   0        0        0      436 2023-06-22 07:52:46.369652 gaitmap_mad-2.2.1/gaitmap_mad/stride_segmentation/dtw/_dtw_templates/__init__.py
+-rw-r--r--   0        0        0     7513 2023-06-22 07:52:46.369652 gaitmap_mad-2.2.1/gaitmap_mad/stride_segmentation/dtw/_dtw_templates/barth_original_template.csv
+-rw-r--r--   0        0        0    15956 2023-06-22 07:52:46.369652 gaitmap_mad-2.2.1/gaitmap_mad/stride_segmentation/dtw/_dtw_templates/templates.py
+-rw-r--r--   0        0        0     3589 2023-06-22 07:52:46.369652 gaitmap_mad-2.2.1/gaitmap_mad/stride_segmentation/dtw/_vendored_tslearn.py
+-rw-r--r--   0        0        0     1184 2023-06-22 07:52:46.369652 gaitmap_mad-2.2.1/gaitmap_mad/stride_segmentation/hmm/__init__.py
+-rw-r--r--   0        0        0    10922 2023-06-22 07:52:46.369652 gaitmap_mad-2.2.1/gaitmap_mad/stride_segmentation/hmm/_hmm_feature_transform.py
+-rw-r--r--   0        0        0    12589 2023-06-22 07:52:46.369652 gaitmap_mad-2.2.1/gaitmap_mad/stride_segmentation/hmm/_hmm_stride_segmentation.py
+-rw-r--r--   0        0        0        0 2023-06-22 07:52:46.369652 gaitmap_mad-2.2.1/gaitmap_mad/stride_segmentation/hmm/_pre_trained_models/__init__.py
+-rw-r--r--   0        0        0   397824 2023-06-22 07:52:46.369652 gaitmap_mad-2.2.1/gaitmap_mad/stride_segmentation/hmm/_pre_trained_models/fallriskpd_at_lab_model.json
+-rw-r--r--   0        0        0    27197 2023-06-22 07:52:46.369652 gaitmap_mad-2.2.1/gaitmap_mad/stride_segmentation/hmm/_segmentation_model.py
+-rw-r--r--   0        0        0    19087 2023-06-22 07:52:46.369652 gaitmap_mad-2.2.1/gaitmap_mad/stride_segmentation/hmm/_simple_model.py
+-rw-r--r--   0        0        0    26902 2023-06-22 07:52:46.369652 gaitmap_mad-2.2.1/gaitmap_mad/stride_segmentation/hmm/_utils.py
+-rw-r--r--   0        0        0      265 2023-06-22 07:52:46.369652 gaitmap_mad-2.2.1/gaitmap_mad/trajectory_reconstruction/__init__.py
+-rw-r--r--   0        0        0      263 2023-06-22 07:52:46.369652 gaitmap_mad-2.2.1/gaitmap_mad/trajectory_reconstruction/position_methods/__init__.py
+-rw-r--r--   0        0        0    10862 2023-06-22 07:52:46.369652 gaitmap_mad-2.2.1/gaitmap_mad/trajectory_reconstruction/position_methods/_piece_wise_linear_dedrifted_integration.py
+-rw-r--r--   0        0        0      589 2023-06-22 07:52:46.369652 gaitmap_mad-2.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1295 1970-01-01 00:00:00.000000 gaitmap_mad-2.2.1/PKG-INFO
```

### Comparing `gaitmap_mad-2.2.0/LICENSE` & `gaitmap_mad-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gaitmap_mad-2.2.0/README.md` & `gaitmap_mad-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `gaitmap_mad-2.2.0/gaitmap_mad/event_detection/_filtered_rampp_event_detection.py` & `gaitmap_mad-2.2.1/gaitmap_mad/event_detection/_filtered_rampp_event_detection.py`

 * *Files identical despite different names*

### Comparing `gaitmap_mad-2.2.0/gaitmap_mad/event_detection/_rampp_event_detection.py` & `gaitmap_mad-2.2.1/gaitmap_mad/event_detection/_rampp_event_detection.py`

 * *Files identical despite different names*

### Comparing `gaitmap_mad-2.2.0/gaitmap_mad/gait_detection/_ullrich_gait_sequence_detection.py` & `gaitmap_mad-2.2.1/gaitmap_mad/gait_detection/_ullrich_gait_sequence_detection.py`

 * *Files identical despite different names*

### Comparing `gaitmap_mad-2.2.0/gaitmap_mad/preprocessing/sensor_alignment/_forward_direction_alignment.py` & `gaitmap_mad-2.2.1/gaitmap_mad/preprocessing/sensor_alignment/_forward_direction_alignment.py`

 * *Files identical despite different names*

### Comparing `gaitmap_mad-2.2.0/gaitmap_mad/stride_segmentation/__init__.py` & `gaitmap_mad-2.2.1/gaitmap_mad/stride_segmentation/__init__.py`

 * *Files identical despite different names*

### Comparing `gaitmap_mad-2.2.0/gaitmap_mad/stride_segmentation/dtw/__init__.py` & `gaitmap_mad-2.2.1/gaitmap_mad/stride_segmentation/dtw/__init__.py`

 * *Files identical despite different names*

### Comparing `gaitmap_mad-2.2.0/gaitmap_mad/stride_segmentation/dtw/_barth_dtw.py` & `gaitmap_mad-2.2.1/gaitmap_mad/stride_segmentation/dtw/_barth_dtw.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,16 @@
 
     BarthDtw uses a manually created template of an IMU stride to find multiple occurrences of similar signals in a
     continuous data stream.
     The method is not limited to a single sensor-axis or sensor, but can use any number of dimensions of the provided
     input signal simultaneously.
     For more details refer to the `Notes` section.
 
+    This method was first published in [1]_.
+
     Parameters
     ----------
     template
         The template used for matching.
         The required data type and shape depends on the use case.
         For more details see :class:`~gaitmap.stride_segmentation.BaseDtw`.
         By default, the :class:`~gaitmap.stride_segmentation.BarthOriginalTemplate` is used
```

### Comparing `gaitmap_mad-2.2.0/gaitmap_mad/stride_segmentation/dtw/_base_dtw.py` & `gaitmap_mad-2.2.1/gaitmap_mad/stride_segmentation/dtw/_base_dtw.py`

 * *Files identical despite different names*

### Comparing `gaitmap_mad-2.2.0/gaitmap_mad/stride_segmentation/dtw/_constrained_barth_dtw.py` & `gaitmap_mad-2.2.1/gaitmap_mad/stride_segmentation/dtw/_constrained_barth_dtw.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,16 @@
     template and the signal by default.
     This help to prevent issues, where only the region from TC to IC is mapped as the entire stride.
     For more information on this see the :ref:`example <example_constrained_barth_stride_segmentation>`.
 
     This exists as a separate class, so that users are aware, they are using a different method that might impact
     their results.
 
+    This method is based on [1]_ and the modification of the constrained warping path is inspired by [2]_.
+
     Parameters
     ----------
     template
         The template used for matching.
         The required data type and shape depends on the use case.
         For more details see :class:`~gaitmap.stride_segmentation.BaseDtw`.
         By default, the :class:`~gaitmap.stride_segmentation.BarthOriginalTemplate` is used
@@ -116,14 +118,17 @@
 
     Notes
     -----
     .. [1] Barth, J., Oberndorfer, C., Kugler, P., Schuldhaus, D., Winkler, J., Klucken, J., & Eskofier, B. (2013).
        Subsequence dynamic time warping as a method for robust step segmentation using gyroscope signals of daily life
        activities. Proceedings of the Annual International Conference of the IEEE Engineering in Medicine and Biology
        Society, EMBS, 6744-6747. https://doi.org/10.1109/EMBC.2013.6611104
+    .. [2] M. Müller, Fundamentals of Music Processing - Using Python and Jupyter Notebooks, 2nd ed. Springer Verlag,
+       2021.
+
 
     See Also
     --------
     gaitmap.stride_segmentation.BarthDtw: For all details on the method
 
     """
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `gaitmap_mad-2.2.0/gaitmap_mad/stride_segmentation/dtw/_dtw_templates/barth_original_template.csv` & `gaitmap_mad-2.2.1/gaitmap_mad/stride_segmentation/dtw/_dtw_templates/barth_original_template.csv`

 * *Files identical despite different names*

### Comparing `gaitmap_mad-2.2.0/gaitmap_mad/stride_segmentation/dtw/_dtw_templates/templates.py` & `gaitmap_mad-2.2.1/gaitmap_mad/stride_segmentation/dtw/_dtw_templates/templates.py`

 * *Files identical despite different names*

### Comparing `gaitmap_mad-2.2.0/gaitmap_mad/stride_segmentation/dtw/_vendored_tslearn.py` & `gaitmap_mad-2.2.1/gaitmap_mad/stride_segmentation/dtw/_vendored_tslearn.py`

 * *Files identical despite different names*

### Comparing `gaitmap_mad-2.2.0/gaitmap_mad/stride_segmentation/hmm/__init__.py` & `gaitmap_mad-2.2.1/gaitmap_mad/stride_segmentation/hmm/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,17 +11,17 @@
     PreTrainedRothSegmentationModel,
 )
 from gaitmap_mad.stride_segmentation.hmm._segmentation_model import BaseSegmentationHmm, RothSegmentationHmm
 from gaitmap_mad.stride_segmentation.hmm._simple_model import SimpleHmm
 
 if multiprocessing.parent_process() is None:
     warnings.warn(
-        "The hmm support in gaitmap is still quite experimental and you might run into some rough edges."
+        "The hmm support in gaitmap is still quite experimental and you might run into some rough edges. "
         "If you encounter any issues, please report them on github. "
-        "Also expect the API to change in the future."
+        "Also expect the API to change in the future. "
         "Monitor the changelog before upgrading to newer versions when using HMMs.",
         UserWarning,
     )
 
 __all__ = [
     "RothHmmFeatureTransformer",
     "HmmStrideSegmentation",
```

### Comparing `gaitmap_mad-2.2.0/gaitmap_mad/stride_segmentation/hmm/_hmm_feature_transform.py` & `gaitmap_mad-2.2.1/gaitmap_mad/stride_segmentation/hmm/_hmm_feature_transform.py`

 * *Files identical despite different names*

### Comparing `gaitmap_mad-2.2.0/gaitmap_mad/stride_segmentation/hmm/_hmm_stride_segmentation.py` & `gaitmap_mad-2.2.1/gaitmap_mad/stride_segmentation/hmm/_hmm_stride_segmentation.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,14 +58,16 @@
     As long as it is a valid subclass of BaseSegmentationHmm, it can be used here.
     On top of the segmentation, this class implements a postprocessing step that snaps the minima in the raw signals
     and contains convenience methods that ensure that outputs conform to the expected gaitmap formats.
 
     Note, that this class only supports prediction.
     To train your own HMM, use the `self_optimize` method on the model that you were planning to use here.
 
+    This is based on the work of Roth et al. 2021 [1]_ and the implementation is using done with `pomegranate` [2]_.
+
     Parameters
     ----------
     model
         The HMM class need a valid pre-trained model to segment strides
     snap_to_min_win_ms
         The size of the window in seconds used to search local minima during the post processing of the stride borders.
         If this is set to None, this postprocessing step is skipped.
@@ -104,14 +106,20 @@
     -----
     Post Processing
         This algorithm uses an optional post-processing step that "snaps" the stride borders to the closest local
         minimum in the raw data.
         However, this assumes that the start and the end of each match is marked by a clear minimum in one axis of the
         raw data.
 
+    .. [1] Roth, N., Küderle, A., Ullrich, M. et al. Hidden Markov Model based stride segmentation on unsupervised
+       free-living gait data in Parkinson`s disease patients. J NeuroEngineering Rehabil 18, 93 (2021).
+       https://doi.org/10.1186/s12984-021-00883-7
+    .. [2] J. Schreiber, “Pomegranate: Fast and flexible probabilistic modeling in python,” Journal of Machine Learning
+       Research, vol. 18, no. 164, pp. 1-6, 2018.
+
     """
 
     snap_to_min_win_ms: Optional[float]
     snap_to_min_axis: str
     model: BaseSegmentationHmmT
 
     data: Union[np.ndarray, SensorData]
```

### Comparing `gaitmap_mad-2.2.0/gaitmap_mad/stride_segmentation/hmm/_pre_trained_models/fallriskpd_at_lab_model.json` & `gaitmap_mad-2.2.1/gaitmap_mad/stride_segmentation/hmm/_pre_trained_models/fallriskpd_at_lab_model.json`

 * *Files identical despite different names*

### Comparing `gaitmap_mad-2.2.0/gaitmap_mad/stride_segmentation/hmm/_segmentation_model.py` & `gaitmap_mad-2.2.1/gaitmap_mad/stride_segmentation/hmm/_segmentation_model.py`

 * *Files identical despite different names*

### Comparing `gaitmap_mad-2.2.0/gaitmap_mad/stride_segmentation/hmm/_simple_model.py` & `gaitmap_mad-2.2.1/gaitmap_mad/stride_segmentation/hmm/_simple_model.py`

 * *Files identical despite different names*

### Comparing `gaitmap_mad-2.2.0/gaitmap_mad/stride_segmentation/hmm/_utils.py` & `gaitmap_mad-2.2.1/gaitmap_mad/stride_segmentation/hmm/_utils.py`

 * *Files identical despite different names*

### Comparing `gaitmap_mad-2.2.0/gaitmap_mad/trajectory_reconstruction/position_methods/_piece_wise_linear_dedrifted_integration.py` & `gaitmap_mad-2.2.1/gaitmap_mad/trajectory_reconstruction/position_methods/_piece_wise_linear_dedrifted_integration.py`

 * *Files 9% similar despite different names*

```diff
@@ -34,14 +34,16 @@
     mid-stances
     as ZUPTS during regular walking.
 
     Further drift correction is applied using a level-assumption (i.e. we assume that the sensor starts and ends its
     movement at the same z-position/height between zupt regions).
     If this assumption is not true for your usecase, you can disable it using the `level_assumption` parameter.
 
+    This approach is inspired by [1]_,[2]_, and [3]_.
+
     Parameters
     ----------
     zupt_detector
         An instance of a valid Zupt detector that will be used to find ZUPTs.
     level_assumption
         If True, it is assumed that the stride starts and ends at z=0 and dedrifting in that direction is applied
         accordingly.
@@ -102,14 +104,25 @@
     fit applied to one region to the start of the next region with a straight line.
     For the first value in the sequence, we always assume a velocity of 0 and for the last value we take the final
     uncorrected velocity value.
     This multi linear baseline is than substracted from the velocity to correct it.
 
     The same process is repeated for the z-position in case `level_walking=True`.
 
+    .. [1] Hannink, J., Ollenschläger, M., Kluge, F., Roth, N., Klucken, J., and Eskofier, B. M. 2017. Benchmarking Foot
+       Trajectory Estimation Methods for Mobile Gait Analysis. Sensors (Basel, Switzerland) 17, 9.
+       https://doi.org/10.3390/s17091940
+    .. [2] M. Zok, C. Mazz`a, and U. Della Croce, “Total body centre of mass displacement estimated using ground
+       reactions during transitory motor tasks: Application to step ascent,” Medical Engineering & Physics, vol. 26,
+       no. 9, pp. 791-798, Nov. 2004. [Online]. Available:
+       https://linkinghub.elsevier.com/retrieve/pii/S1350453304001195
+    .. [3] N. Kitagawa and N. Ogihara, “Estimation of foot trajectory during human walking by a wearable inertial
+       measurement unit mounted to the foot,” Gait & Posture, vol. 45, pp. 110-114, Mar. 2016. [Online].
+       Available: https://linkinghub.elsevier.com/retrieve/pii/S0966636216000151
+
     See Also
     --------
     gaitmap.trajectory_reconstruction: Other implemented algorithms for orientation and position estimation
     gaitmap.utils.static_moment_detection: Static moment detector used for estimating zupt updates.
 
     """
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `gaitmap_mad-2.2.0/pyproject.toml` & `gaitmap_mad-2.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gaitmap_mad"
-version = "2.2.0"
+version = "2.2.1"
 description = "Specific algorithm implementaions by the mad_lab"
 license = "AGPL-3.0"
 readme = "README.md"
 homepage = "https://github.com/mad-lab-fau/gaitmap"
 repository = "https://github.com/mad-lab-fau/gaitmap"
 authors = [
     "Arne Küderle <arne.kuederle@fau.de>",
```

### Comparing `gaitmap_mad-2.2.0/PKG-INFO` & `gaitmap_mad-2.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaitmap-mad
-Version: 2.2.0
+Version: 2.2.1
 Summary: Specific algorithm implementaions by the mad_lab
 Home-page: https://github.com/mad-lab-fau/gaitmap
 License: AGPL-3.0
 Author: Arne Küderle
 Author-email: arne.kuederle@fau.de
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

