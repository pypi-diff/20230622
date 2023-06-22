# Comparing `tmp/raya-3.5.0.dev0.tar.gz` & `tmp/raya-3.5.1.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raya-3.5.0.dev0.tar", last modified: Thu Jun  8 01:58:14 2023, max compression
+gzip compressed data, was "raya-3.5.1.dev0.tar", last modified: Thu Jun 22 18:50:07 2023, max compression
```

## Comparing `raya-3.5.0.dev0.tar` & `raya-3.5.1.dev0.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2023-06-08 01:58:14.440130 raya-3.5.0.dev0/
--rw-rw-r--   0 prod      (1001) prod      (1001)      568 2023-06-08 01:58:14.440130 raya-3.5.0.dev0/PKG-INFO
--rw-rw-r--   0 prod      (1001) prod      (1001)      150 2023-06-07 02:42:34.000000 raya-3.5.0.dev0/README.md
--rw-rw-r--   0 prod      (1001) prod      (1001)      103 2023-06-07 02:42:34.000000 raya-3.5.0.dev0/pyproject.toml
--rw-rw-r--   0 prod      (1001) prod      (1001)       38 2023-06-08 01:58:14.440130 raya-3.5.0.dev0/setup.cfg
--rw-rw-r--   0 prod      (1001) prod      (1001)     2752 2023-06-08 01:58:14.000000 raya-3.5.0.dev0/setup.py
-drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2023-06-08 01:58:14.436130 raya-3.5.0.dev0/src/
-drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2023-06-08 01:58:14.436130 raya-3.5.0.dev0/src/raya/
--rw-rw-r--   0 prod      (1001) prod      (1001)       38 2023-06-07 02:42:34.000000 raya-3.5.0.dev0/src/raya/__init__.py
--rw-rw-r--   0 prod      (1001) prod      (1001)       25 2023-06-08 01:58:04.000000 raya-3.5.0.dev0/src/raya/_version.py
--rw-rw-r--   0 prod      (1001) prod      (1001)     3183 2023-06-08 01:58:13.000000 raya-3.5.0.dev0/src/raya/application_base.py
--rw-rw-r--   0 prod      (1001) prod      (1001)      664 2023-06-08 01:58:13.000000 raya-3.5.0.dev0/src/raya/constants.py
-drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2023-06-08 01:58:14.436130 raya-3.5.0.dev0/src/raya/controllers/
--rw-rw-r--   0 prod      (1001) prod      (1001)        0 2023-06-07 02:42:34.000000 raya-3.5.0.dev0/src/raya/controllers/__init__.py
--rw-rw-r--   0 prod      (1001) prod      (1001)      260 2023-06-08 01:58:14.000000 raya-3.5.0.dev0/src/raya/controllers/analytics_controller.py
--rw-rw-r--   0 prod      (1001) prod      (1001)    25655 2023-06-08 01:58:14.000000 raya-3.5.0.dev0/src/raya/controllers/arms_controller.py
--rw-rw-r--   0 prod      (1001) prod      (1001)      952 2023-06-08 01:58:13.000000 raya-3.5.0.dev0/src/raya/controllers/base_controller.py
--rw-rw-r--   0 prod      (1001) prod      (1001)       90 2023-06-08 01:58:13.000000 raya-3.5.0.dev0/src/raya/controllers/base_pseudo_controller.py
--rw-rw-r--   0 prod      (1001) prod      (1001)     1289 2023-06-08 01:58:13.000000 raya-3.5.0.dev0/src/raya/controllers/cameras_controller.py
--rw-rw-r--   0 prod      (1001) prod      (1001)      425 2023-06-08 01:58:13.000000 raya-3.5.0.dev0/src/raya/controllers/communication_controller.py
--rw-rw-r--   0 prod      (1001) prod      (1001)     2934 2023-06-08 01:58:13.000000 raya-3.5.0.dev0/src/raya/controllers/cv_controller.py
--rw-rw-r--   0 prod      (1001) prod      (1001)     1387 2023-06-08 01:58:13.000000 raya-3.5.0.dev0/src/raya/controllers/fleet_controller.py
--rw-rw-r--   0 prod      (1001) prod      (1001)      523 2023-06-08 01:58:13.000000 raya-3.5.0.dev0/src/raya/controllers/grasping_controller.py
--rw-rw-r--   0 prod      (1001) prod      (1001)      924 2023-06-08 01:58:13.000000 raya-3.5.0.dev0/src/raya/controllers/interactions_controller.py
--rw-rw-r--   0 prod      (1001) prod      (1001)     1298 2023-06-08 01:58:13.000000 raya-3.5.0.dev0/src/raya/controllers/leds_controller.py
--rw-rw-r--   0 prod      (1001) prod      (1001)     1171 2023-06-08 01:58:13.000000 raya-3.5.0.dev0/src/raya/controllers/lidar_controller.py
--rw-rw-r--   0 prod      (1001) prod      (1001)     3127 2023-06-08 01:58:13.000000 raya-3.5.0.dev0/src/raya/controllers/manipulation_controller.py
--rw-rw-r--   0 prod      (1001) prod      (1001)     2436 2023-06-08 01:58:13.000000 raya-3.5.0.dev0/src/raya/controllers/motion_controller.py
--rw-rw-r--   0 prod      (1001) prod      (1001)     7148 2023-06-08 01:58:13.000000 raya-3.5.0.dev0/src/raya/controllers/navigation_controller.py
--rw-rw-r--   0 prod      (1001) prod      (1001)     1367 2023-06-08 01:58:13.000000 raya-3.5.0.dev0/src/raya/controllers/sensors_controller.py
--rw-rw-r--   0 prod      (1001) prod      (1001)      808 2023-06-08 01:58:14.000000 raya-3.5.0.dev0/src/raya/controllers/skills_controller.py
--rw-rw-r--   0 prod      (1001) prod      (1001)     2590 2023-06-08 01:58:13.000000 raya-3.5.0.dev0/src/raya/controllers/sound_controller.py
--rw-rw-r--   0 prod      (1001) prod      (1001)     8614 2023-06-08 01:58:14.000000 raya-3.5.0.dev0/src/raya/controllers/ui_controller.py
--rw-rw-r--   0 prod      (1001) prod      (1001)       59 2023-06-08 01:58:13.000000 raya-3.5.0.dev0/src/raya/entry_point.py
--rw-rw-r--   0 prod      (1001) prod      (1001)     4876 2023-06-08 01:58:13.000000 raya-3.5.0.dev0/src/raya/enumerations.py
--rw-rw-r--   0 prod      (1001) prod      (1001)    14002 2023-06-08 01:58:13.000000 raya-3.5.0.dev0/src/raya/exceptions.py
--rw-rw-r--   0 prod      (1001) prod      (1001)     6639 2023-06-08 01:58:13.000000 raya-3.5.0.dev0/src/raya/exceptions_handler.py
-drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2023-06-08 01:58:14.436130 raya-3.5.0.dev0/src/raya/handlers/
--rw-rw-r--   0 prod      (1001) prod      (1001)        0 2023-06-07 02:42:34.000000 raya-3.5.0.dev0/src/raya/handlers/__init__.py
-drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2023-06-08 01:58:14.436130 raya-3.5.0.dev0/src/raya/handlers/cv/
--rw-rw-r--   0 prod      (1001) prod      (1001)        0 2023-06-07 02:42:34.000000 raya-3.5.0.dev0/src/raya/handlers/cv/__init__.py
-drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2023-06-08 01:58:14.436130 raya-3.5.0.dev0/src/raya/handlers/cv/classifiers/
--rw-rw-r--   0 prod      (1001) prod      (1001)        0 2023-06-08 01:23:36.000000 raya-3.5.0.dev0/src/raya/handlers/cv/classifiers/__init__.py
--rw-rw-r--   0 prod      (1001) prod      (1001)     1211 2023-06-08 01:58:13.000000 raya-3.5.0.dev0/src/raya/handlers/cv/classifiers/classifier_handler.py
--rw-rw-r--   0 prod      (1001) prod      (1001)      802 2023-06-08 01:58:13.000000 raya-3.5.0.dev0/src/raya/handlers/cv/classifiers/objects_classifier_handler.py
-drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2023-06-08 01:58:14.436130 raya-3.5.0.dev0/src/raya/handlers/cv/detectors/
--rw-rw-r--   0 prod      (1001) prod      (1001)        0 2023-06-08 01:23:36.000000 raya-3.5.0.dev0/src/raya/handlers/cv/detectors/__init__.py
--rw-rw-r--   0 prod      (1001) prod      (1001)     1168 2023-06-08 01:58:13.000000 raya-3.5.0.dev0/src/raya/handlers/cv/detectors/detector_handler.py
--rw-rw-r--   0 prod      (1001) prod      (1001)      312 2023-06-08 01:58:13.000000 raya-3.5.0.dev0/src/raya/handlers/cv/detectors/faces_detector_handler.py
--rw-rw-r--   0 prod      (1001) prod      (1001)      792 2023-06-08 01:58:13.000000 raya-3.5.0.dev0/src/raya/handlers/cv/detectors/objects_detector_handler.py
--rw-rw-r--   0 prod      (1001) prod      (1001)      713 2023-06-08 01:58:13.000000 raya-3.5.0.dev0/src/raya/handlers/cv/detectors/tags_detector_handler.py
-drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2023-06-08 01:58:14.436130 raya-3.5.0.dev0/src/raya/handlers/cv/estimators/
--rw-rw-r--   0 prod      (1001) prod      (1001)        0 2023-06-08 01:23:36.000000 raya-3.5.0.dev0/src/raya/handlers/cv/estimators/__init__.py
--rw-rw-r--   0 prod      (1001) prod      (1001)     1069 2023-06-08 01:58:13.000000 raya-3.5.0.dev0/src/raya/handlers/cv/estimators/estimator_handler.py
--rw-rw-r--   0 prod      (1001) prod      (1001)      316 2023-06-08 01:58:13.000000 raya-3.5.0.dev0/src/raya/handlers/cv/estimators/hand_estimator_handler.py
--rw-rw-r--   0 prod      (1001) prod      (1001)      197 2023-06-08 01:58:13.000000 raya-3.5.0.dev0/src/raya/handlers/cv/model_handler.py
-drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2023-06-08 01:58:14.436130 raya-3.5.0.dev0/src/raya/handlers/cv/recognizers/
--rw-rw-r--   0 prod      (1001) prod      (1001)        0 2023-06-08 01:23:36.000000 raya-3.5.0.dev0/src/raya/handlers/cv/recognizers/__init__.py
--rw-rw-r--   0 prod      (1001) prod      (1001)      843 2023-06-08 01:58:13.000000 raya-3.5.0.dev0/src/raya/handlers/cv/recognizers/faces_recognizer_handler.py
--rw-rw-r--   0 prod      (1001) prod      (1001)     1190 2023-06-08 01:58:13.000000 raya-3.5.0.dev0/src/raya/handlers/cv/recognizers/recognizer_handler.py
-drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2023-06-08 01:58:14.436130 raya-3.5.0.dev0/src/raya/handlers/cv/segmentators/
--rw-rw-r--   0 prod      (1001) prod      (1001)        0 2023-06-08 01:23:36.000000 raya-3.5.0.dev0/src/raya/handlers/cv/segmentators/__init__.py
--rw-rw-r--   0 prod      (1001) prod      (1001)      807 2023-06-08 01:58:13.000000 raya-3.5.0.dev0/src/raya/handlers/cv/segmentators/objects_segmentator_handler.py
--rw-rw-r--   0 prod      (1001) prod      (1001)      796 2023-06-08 01:58:13.000000 raya-3.5.0.dev0/src/raya/handlers/cv/segmentators/planes_segmentator_handler.py
--rw-rw-r--   0 prod      (1001) prod      (1001)     1201 2023-06-08 01:58:13.000000 raya-3.5.0.dev0/src/raya/handlers/cv/segmentators/segmentator_handler.py
-drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2023-06-08 01:58:14.436130 raya-3.5.0.dev0/src/raya/handlers/general/
--rw-rw-r--   0 prod      (1001) prod      (1001)        0 2023-06-07 02:42:34.000000 raya-3.5.0.dev0/src/raya/handlers/general/__init__.py
--rw-rw-r--   0 prod      (1001) prod      (1001)      330 2023-06-08 01:58:13.000000 raya-3.5.0.dev0/src/raya/handlers/general/callback_handler.py
-drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2023-06-08 01:58:14.436130 raya-3.5.0.dev0/src/raya/listeners/
--rw-rw-r--   0 prod      (1001) prod      (1001)        0 2023-06-07 02:42:34.000000 raya-3.5.0.dev0/src/raya/listeners/__init__.py
--rw-rw-r--   0 prod      (1001) prod      (1001)       77 2023-06-08 01:58:13.000000 raya-3.5.0.dev0/src/raya/listeners/lidar_listeners.py
--rw-rw-r--   0 prod      (1001) prod      (1001)      160 2023-06-08 01:58:13.000000 raya-3.5.0.dev0/src/raya/listeners/sensors_listeners.py
--rw-rw-r--   0 prod      (1001) prod      (1001)      408 2023-06-08 01:58:13.000000 raya-3.5.0.dev0/src/raya/logger.py
--rw-rw-r--   0 prod      (1001) prod      (1001)     2055 2023-06-08 01:58:13.000000 raya-3.5.0.dev0/src/raya/raya_interface.py
--rw-rw-r--   0 prod      (1001) prod      (1001)      257 2023-06-08 01:58:13.000000 raya-3.5.0.dev0/src/raya/standalone_handler.py
-drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2023-06-08 01:58:14.436130 raya-3.5.0.dev0/src/raya/tools/
--rw-rw-r--   0 prod      (1001) prod      (1001)        0 2023-06-07 02:42:34.000000 raya-3.5.0.dev0/src/raya/tools/__init__.py
--rw-rw-r--   0 prod      (1001) prod      (1001)      399 2023-06-08 01:58:13.000000 raya-3.5.0.dev0/src/raya/tools/filesystem.py
--rw-rw-r--   0 prod      (1001) prod      (1001)      984 2023-06-08 01:58:13.000000 raya-3.5.0.dev0/src/raya/tools/fsm.py
--rw-rw-r--   0 prod      (1001) prod      (1001)      294 2023-06-08 01:58:13.000000 raya-3.5.0.dev0/src/raya/tools/image.py
-drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2023-06-08 01:58:14.436130 raya-3.5.0.dev0/src/raya.egg-info/
--rw-rw-r--   0 prod      (1001) prod      (1001)      568 2023-06-08 01:58:14.000000 raya-3.5.0.dev0/src/raya.egg-info/PKG-INFO
--rw-rw-r--   0 prod      (1001) prod      (1001)     2656 2023-06-08 01:58:14.000000 raya-3.5.0.dev0/src/raya.egg-info/SOURCES.txt
--rw-rw-r--   0 prod      (1001) prod      (1001)        1 2023-06-08 01:58:14.000000 raya-3.5.0.dev0/src/raya.egg-info/dependency_links.txt
--rw-rw-r--   0 prod      (1001) prod      (1001)        5 2023-06-08 01:58:14.000000 raya-3.5.0.dev0/src/raya.egg-info/top_level.txt
+drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2023-06-22 18:50:07.383708 raya-3.5.1.dev0/
+-rw-rw-r--   0 prod      (1001) prod      (1001)      568 2023-06-22 18:50:07.383708 raya-3.5.1.dev0/PKG-INFO
+-rw-rw-r--   0 prod      (1001) prod      (1001)      150 2023-06-07 02:42:34.000000 raya-3.5.1.dev0/README.md
+-rw-rw-r--   0 prod      (1001) prod      (1001)      103 2023-06-07 02:42:34.000000 raya-3.5.1.dev0/pyproject.toml
+-rw-rw-r--   0 prod      (1001) prod      (1001)       38 2023-06-22 18:50:07.383708 raya-3.5.1.dev0/setup.cfg
+-rw-rw-r--   0 prod      (1001) prod      (1001)     2752 2023-06-22 18:50:07.000000 raya-3.5.1.dev0/setup.py
+drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2023-06-22 18:50:07.379708 raya-3.5.1.dev0/src/
+drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2023-06-22 18:50:07.379708 raya-3.5.1.dev0/src/raya/
+-rw-rw-r--   0 prod      (1001) prod      (1001)       38 2023-06-07 02:42:34.000000 raya-3.5.1.dev0/src/raya/__init__.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)       25 2023-06-22 18:49:57.000000 raya-3.5.1.dev0/src/raya/_version.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     3183 2023-06-22 18:50:05.000000 raya-3.5.1.dev0/src/raya/application_base.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      664 2023-06-22 18:50:05.000000 raya-3.5.1.dev0/src/raya/constants.py
+drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2023-06-22 18:50:07.379708 raya-3.5.1.dev0/src/raya/controllers/
+-rw-rw-r--   0 prod      (1001) prod      (1001)        0 2023-06-07 02:42:34.000000 raya-3.5.1.dev0/src/raya/controllers/__init__.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      260 2023-06-22 18:50:07.000000 raya-3.5.1.dev0/src/raya/controllers/analytics_controller.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)    25655 2023-06-22 18:50:06.000000 raya-3.5.1.dev0/src/raya/controllers/arms_controller.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      952 2023-06-22 18:50:06.000000 raya-3.5.1.dev0/src/raya/controllers/base_controller.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)       90 2023-06-22 18:50:06.000000 raya-3.5.1.dev0/src/raya/controllers/base_pseudo_controller.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     1289 2023-06-22 18:50:06.000000 raya-3.5.1.dev0/src/raya/controllers/cameras_controller.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      425 2023-06-22 18:50:06.000000 raya-3.5.1.dev0/src/raya/controllers/communication_controller.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     2934 2023-06-22 18:50:06.000000 raya-3.5.1.dev0/src/raya/controllers/cv_controller.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     1387 2023-06-22 18:50:06.000000 raya-3.5.1.dev0/src/raya/controllers/fleet_controller.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      523 2023-06-22 18:50:06.000000 raya-3.5.1.dev0/src/raya/controllers/grasping_controller.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      924 2023-06-22 18:50:06.000000 raya-3.5.1.dev0/src/raya/controllers/interactions_controller.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     1298 2023-06-22 18:50:06.000000 raya-3.5.1.dev0/src/raya/controllers/leds_controller.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     1171 2023-06-22 18:50:06.000000 raya-3.5.1.dev0/src/raya/controllers/lidar_controller.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     3127 2023-06-22 18:50:06.000000 raya-3.5.1.dev0/src/raya/controllers/manipulation_controller.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     2436 2023-06-22 18:50:06.000000 raya-3.5.1.dev0/src/raya/controllers/motion_controller.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     7148 2023-06-22 18:50:06.000000 raya-3.5.1.dev0/src/raya/controllers/navigation_controller.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     1367 2023-06-22 18:50:06.000000 raya-3.5.1.dev0/src/raya/controllers/sensors_controller.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      808 2023-06-22 18:50:07.000000 raya-3.5.1.dev0/src/raya/controllers/skills_controller.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     2590 2023-06-22 18:50:06.000000 raya-3.5.1.dev0/src/raya/controllers/sound_controller.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     8614 2023-06-22 18:50:07.000000 raya-3.5.1.dev0/src/raya/controllers/ui_controller.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)       59 2023-06-22 18:50:05.000000 raya-3.5.1.dev0/src/raya/entry_point.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     4876 2023-06-22 18:50:05.000000 raya-3.5.1.dev0/src/raya/enumerations.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)    14002 2023-06-22 18:50:06.000000 raya-3.5.1.dev0/src/raya/exceptions.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     6639 2023-06-22 18:50:05.000000 raya-3.5.1.dev0/src/raya/exceptions_handler.py
+drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2023-06-22 18:50:07.379708 raya-3.5.1.dev0/src/raya/handlers/
+-rw-rw-r--   0 prod      (1001) prod      (1001)        0 2023-06-07 02:42:34.000000 raya-3.5.1.dev0/src/raya/handlers/__init__.py
+drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2023-06-22 18:50:07.379708 raya-3.5.1.dev0/src/raya/handlers/cv/
+-rw-rw-r--   0 prod      (1001) prod      (1001)        0 2023-06-07 02:42:34.000000 raya-3.5.1.dev0/src/raya/handlers/cv/__init__.py
+drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2023-06-22 18:50:07.383708 raya-3.5.1.dev0/src/raya/handlers/cv/classifiers/
+-rw-rw-r--   0 prod      (1001) prod      (1001)        0 2023-06-08 01:23:36.000000 raya-3.5.1.dev0/src/raya/handlers/cv/classifiers/__init__.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     1211 2023-06-22 18:50:06.000000 raya-3.5.1.dev0/src/raya/handlers/cv/classifiers/classifier_handler.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      802 2023-06-22 18:50:06.000000 raya-3.5.1.dev0/src/raya/handlers/cv/classifiers/objects_classifier_handler.py
+drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2023-06-22 18:50:07.383708 raya-3.5.1.dev0/src/raya/handlers/cv/detectors/
+-rw-rw-r--   0 prod      (1001) prod      (1001)        0 2023-06-08 01:23:36.000000 raya-3.5.1.dev0/src/raya/handlers/cv/detectors/__init__.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     1168 2023-06-22 18:50:06.000000 raya-3.5.1.dev0/src/raya/handlers/cv/detectors/detector_handler.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      312 2023-06-22 18:50:06.000000 raya-3.5.1.dev0/src/raya/handlers/cv/detectors/faces_detector_handler.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      792 2023-06-22 18:50:06.000000 raya-3.5.1.dev0/src/raya/handlers/cv/detectors/objects_detector_handler.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      713 2023-06-22 18:50:06.000000 raya-3.5.1.dev0/src/raya/handlers/cv/detectors/tags_detector_handler.py
+drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2023-06-22 18:50:07.383708 raya-3.5.1.dev0/src/raya/handlers/cv/estimators/
+-rw-rw-r--   0 prod      (1001) prod      (1001)        0 2023-06-08 01:23:36.000000 raya-3.5.1.dev0/src/raya/handlers/cv/estimators/__init__.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     1069 2023-06-22 18:50:06.000000 raya-3.5.1.dev0/src/raya/handlers/cv/estimators/estimator_handler.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      316 2023-06-22 18:50:06.000000 raya-3.5.1.dev0/src/raya/handlers/cv/estimators/hand_estimator_handler.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      197 2023-06-22 18:50:06.000000 raya-3.5.1.dev0/src/raya/handlers/cv/model_handler.py
+drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2023-06-22 18:50:07.383708 raya-3.5.1.dev0/src/raya/handlers/cv/recognizers/
+-rw-rw-r--   0 prod      (1001) prod      (1001)        0 2023-06-08 01:23:36.000000 raya-3.5.1.dev0/src/raya/handlers/cv/recognizers/__init__.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      843 2023-06-22 18:50:06.000000 raya-3.5.1.dev0/src/raya/handlers/cv/recognizers/faces_recognizer_handler.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     1190 2023-06-22 18:50:06.000000 raya-3.5.1.dev0/src/raya/handlers/cv/recognizers/recognizer_handler.py
+drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2023-06-22 18:50:07.383708 raya-3.5.1.dev0/src/raya/handlers/cv/segmentators/
+-rw-rw-r--   0 prod      (1001) prod      (1001)        0 2023-06-08 01:23:36.000000 raya-3.5.1.dev0/src/raya/handlers/cv/segmentators/__init__.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      807 2023-06-22 18:50:06.000000 raya-3.5.1.dev0/src/raya/handlers/cv/segmentators/objects_segmentator_handler.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      796 2023-06-22 18:50:06.000000 raya-3.5.1.dev0/src/raya/handlers/cv/segmentators/planes_segmentator_handler.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     1201 2023-06-22 18:50:06.000000 raya-3.5.1.dev0/src/raya/handlers/cv/segmentators/segmentator_handler.py
+drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2023-06-22 18:50:07.383708 raya-3.5.1.dev0/src/raya/handlers/general/
+-rw-rw-r--   0 prod      (1001) prod      (1001)        0 2023-06-07 02:42:34.000000 raya-3.5.1.dev0/src/raya/handlers/general/__init__.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      330 2023-06-22 18:50:06.000000 raya-3.5.1.dev0/src/raya/handlers/general/callback_handler.py
+drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2023-06-22 18:50:07.383708 raya-3.5.1.dev0/src/raya/listeners/
+-rw-rw-r--   0 prod      (1001) prod      (1001)        0 2023-06-07 02:42:34.000000 raya-3.5.1.dev0/src/raya/listeners/__init__.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)       77 2023-06-22 18:50:06.000000 raya-3.5.1.dev0/src/raya/listeners/lidar_listeners.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      160 2023-06-22 18:50:06.000000 raya-3.5.1.dev0/src/raya/listeners/sensors_listeners.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      408 2023-06-22 18:50:05.000000 raya-3.5.1.dev0/src/raya/logger.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     2055 2023-06-22 18:50:05.000000 raya-3.5.1.dev0/src/raya/raya_interface.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      257 2023-06-22 18:50:05.000000 raya-3.5.1.dev0/src/raya/standalone_handler.py
+drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2023-06-22 18:50:07.383708 raya-3.5.1.dev0/src/raya/tools/
+-rw-rw-r--   0 prod      (1001) prod      (1001)        0 2023-06-07 02:42:34.000000 raya-3.5.1.dev0/src/raya/tools/__init__.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      399 2023-06-22 18:50:06.000000 raya-3.5.1.dev0/src/raya/tools/filesystem.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      984 2023-06-22 18:50:06.000000 raya-3.5.1.dev0/src/raya/tools/fsm.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      294 2023-06-22 18:50:06.000000 raya-3.5.1.dev0/src/raya/tools/image.py
+drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2023-06-22 18:50:07.379708 raya-3.5.1.dev0/src/raya.egg-info/
+-rw-rw-r--   0 prod      (1001) prod      (1001)      568 2023-06-22 18:50:07.000000 raya-3.5.1.dev0/src/raya.egg-info/PKG-INFO
+-rw-rw-r--   0 prod      (1001) prod      (1001)     2656 2023-06-22 18:50:07.000000 raya-3.5.1.dev0/src/raya.egg-info/SOURCES.txt
+-rw-rw-r--   0 prod      (1001) prod      (1001)        1 2023-06-22 18:50:07.000000 raya-3.5.1.dev0/src/raya.egg-info/dependency_links.txt
+-rw-rw-r--   0 prod      (1001) prod      (1001)        5 2023-06-22 18:50:07.000000 raya-3.5.1.dev0/src/raya.egg-info/top_level.txt
```

### Comparing `raya-3.5.0.dev0/PKG-INFO` & `raya-3.5.1.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raya
-Version: 3.5.0.dev0
+Version: 3.5.1.dev0
 Summary: Unlimited Robotics - Ra-Ya Python Library
 Home-page: https://documentation.unlimited-robotics.com/
 Author: Unlimited Robotics
 Author-email: camilo@unlimited-robotics.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Description: UNKNOWN
```

### Comparing `raya-3.5.0.dev0/setup.py` & `raya-3.5.1.dev0/setup.py`

 * *Files identical despite different names*

### Comparing `raya-3.5.0.dev0/src/raya/application_base.py` & `raya-3.5.1.dev0/src/raya/application_base.py`

 * *Files identical despite different names*

### Comparing `raya-3.5.0.dev0/src/raya/constants.py` & `raya-3.5.1.dev0/src/raya/constants.py`

 * *Files identical despite different names*

### Comparing `raya-3.5.0.dev0/src/raya/controllers/arms_controller.py` & `raya-3.5.1.dev0/src/raya/controllers/arms_controller.py`

 * *Files identical despite different names*

### Comparing `raya-3.5.0.dev0/src/raya/controllers/base_controller.py` & `raya-3.5.1.dev0/src/raya/controllers/base_controller.py`

 * *Files identical despite different names*

### Comparing `raya-3.5.0.dev0/src/raya/controllers/cameras_controller.py` & `raya-3.5.1.dev0/src/raya/controllers/cameras_controller.py`

 * *Files identical despite different names*

### Comparing `raya-3.5.0.dev0/src/raya/controllers/cv_controller.py` & `raya-3.5.1.dev0/src/raya/controllers/cv_controller.py`

 * *Files identical despite different names*

### Comparing `raya-3.5.0.dev0/src/raya/controllers/fleet_controller.py` & `raya-3.5.1.dev0/src/raya/controllers/fleet_controller.py`

 * *Files identical despite different names*

### Comparing `raya-3.5.0.dev0/src/raya/controllers/grasping_controller.py` & `raya-3.5.1.dev0/src/raya/controllers/grasping_controller.py`

 * *Files identical despite different names*

### Comparing `raya-3.5.0.dev0/src/raya/controllers/interactions_controller.py` & `raya-3.5.1.dev0/src/raya/controllers/interactions_controller.py`

 * *Files identical despite different names*

### Comparing `raya-3.5.0.dev0/src/raya/controllers/leds_controller.py` & `raya-3.5.1.dev0/src/raya/controllers/leds_controller.py`

 * *Files identical despite different names*

### Comparing `raya-3.5.0.dev0/src/raya/controllers/lidar_controller.py` & `raya-3.5.1.dev0/src/raya/controllers/lidar_controller.py`

 * *Files identical despite different names*

### Comparing `raya-3.5.0.dev0/src/raya/controllers/manipulation_controller.py` & `raya-3.5.1.dev0/src/raya/controllers/manipulation_controller.py`

 * *Files identical despite different names*

### Comparing `raya-3.5.0.dev0/src/raya/controllers/motion_controller.py` & `raya-3.5.1.dev0/src/raya/controllers/motion_controller.py`

 * *Files identical despite different names*

### Comparing `raya-3.5.0.dev0/src/raya/controllers/navigation_controller.py` & `raya-3.5.1.dev0/src/raya/controllers/navigation_controller.py`

 * *Files identical despite different names*

### Comparing `raya-3.5.0.dev0/src/raya/controllers/sensors_controller.py` & `raya-3.5.1.dev0/src/raya/controllers/sensors_controller.py`

 * *Files identical despite different names*

### Comparing `raya-3.5.0.dev0/src/raya/controllers/skills_controller.py` & `raya-3.5.1.dev0/src/raya/controllers/skills_controller.py`

 * *Files identical despite different names*

### Comparing `raya-3.5.0.dev0/src/raya/controllers/sound_controller.py` & `raya-3.5.1.dev0/src/raya/controllers/sound_controller.py`

 * *Files identical despite different names*

### Comparing `raya-3.5.0.dev0/src/raya/controllers/ui_controller.py` & `raya-3.5.1.dev0/src/raya/controllers/ui_controller.py`

 * *Files identical despite different names*

### Comparing `raya-3.5.0.dev0/src/raya/enumerations.py` & `raya-3.5.1.dev0/src/raya/enumerations.py`

 * *Files identical despite different names*

### Comparing `raya-3.5.0.dev0/src/raya/exceptions.py` & `raya-3.5.1.dev0/src/raya/exceptions.py`

 * *Files identical despite different names*

### Comparing `raya-3.5.0.dev0/src/raya/exceptions_handler.py` & `raya-3.5.1.dev0/src/raya/exceptions_handler.py`

 * *Files identical despite different names*

### Comparing `raya-3.5.0.dev0/src/raya/handlers/cv/classifiers/classifier_handler.py` & `raya-3.5.1.dev0/src/raya/handlers/cv/classifiers/classifier_handler.py`

 * *Files identical despite different names*

### Comparing `raya-3.5.0.dev0/src/raya/handlers/cv/classifiers/objects_classifier_handler.py` & `raya-3.5.1.dev0/src/raya/handlers/cv/classifiers/objects_classifier_handler.py`

 * *Files identical despite different names*

### Comparing `raya-3.5.0.dev0/src/raya/handlers/cv/detectors/detector_handler.py` & `raya-3.5.1.dev0/src/raya/handlers/cv/detectors/detector_handler.py`

 * *Files identical despite different names*

### Comparing `raya-3.5.0.dev0/src/raya/handlers/cv/detectors/objects_detector_handler.py` & `raya-3.5.1.dev0/src/raya/handlers/cv/detectors/objects_detector_handler.py`

 * *Files identical despite different names*

### Comparing `raya-3.5.0.dev0/src/raya/handlers/cv/detectors/tags_detector_handler.py` & `raya-3.5.1.dev0/src/raya/handlers/cv/detectors/tags_detector_handler.py`

 * *Files identical despite different names*

### Comparing `raya-3.5.0.dev0/src/raya/handlers/cv/estimators/estimator_handler.py` & `raya-3.5.1.dev0/src/raya/handlers/cv/estimators/estimator_handler.py`

 * *Files identical despite different names*

### Comparing `raya-3.5.0.dev0/src/raya/handlers/cv/recognizers/faces_recognizer_handler.py` & `raya-3.5.1.dev0/src/raya/handlers/cv/recognizers/faces_recognizer_handler.py`

 * *Files identical despite different names*

### Comparing `raya-3.5.0.dev0/src/raya/handlers/cv/recognizers/recognizer_handler.py` & `raya-3.5.1.dev0/src/raya/handlers/cv/recognizers/recognizer_handler.py`

 * *Files identical despite different names*

### Comparing `raya-3.5.0.dev0/src/raya/handlers/cv/segmentators/objects_segmentator_handler.py` & `raya-3.5.1.dev0/src/raya/handlers/cv/segmentators/objects_segmentator_handler.py`

 * *Files identical despite different names*

### Comparing `raya-3.5.0.dev0/src/raya/handlers/cv/segmentators/planes_segmentator_handler.py` & `raya-3.5.1.dev0/src/raya/handlers/cv/segmentators/planes_segmentator_handler.py`

 * *Files identical despite different names*

### Comparing `raya-3.5.0.dev0/src/raya/handlers/cv/segmentators/segmentator_handler.py` & `raya-3.5.1.dev0/src/raya/handlers/cv/segmentators/segmentator_handler.py`

 * *Files identical despite different names*

### Comparing `raya-3.5.0.dev0/src/raya/raya_interface.py` & `raya-3.5.1.dev0/src/raya/raya_interface.py`

 * *Files identical despite different names*

### Comparing `raya-3.5.0.dev0/src/raya/tools/fsm.py` & `raya-3.5.1.dev0/src/raya/tools/fsm.py`

 * *Files identical despite different names*

### Comparing `raya-3.5.0.dev0/src/raya.egg-info/PKG-INFO` & `raya-3.5.1.dev0/src/raya.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raya
-Version: 3.5.0.dev0
+Version: 3.5.1.dev0
 Summary: Unlimited Robotics - Ra-Ya Python Library
 Home-page: https://documentation.unlimited-robotics.com/
 Author: Unlimited Robotics
 Author-email: camilo@unlimited-robotics.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Description: UNKNOWN
```

### Comparing `raya-3.5.0.dev0/src/raya.egg-info/SOURCES.txt` & `raya-3.5.1.dev0/src/raya.egg-info/SOURCES.txt`

 * *Files identical despite different names*

