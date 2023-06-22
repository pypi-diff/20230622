# Comparing `tmp/pyxy3d-0.1.2.tar.gz` & `tmp/pyxy3d-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxy3d-0.1.2.tar", max compression
+gzip compressed data, was "pyxy3d-0.1.3.tar", max compression
```

## Comparing `pyxy3d-0.1.2.tar` & `pyxy3d-0.1.3.tar`

### file list

```diff
@@ -1,233 +1,233 @@
--rw-r--r--   0        0        0    35190 2023-06-14 20:19:57.480906 pyxy3d-0.1.2/LICENSE.md
--rw-r--r--   0        0        0      922 2023-06-22 12:45:57.541839 pyxy3d-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2644 2023-06-21 22:25:18.660194 pyxy3d-0.1.2/pyxy3d/__init__.py
--rw-r--r--   0        0        0      934 2023-06-12 22:15:42.388447 pyxy3d-0.1.2/pyxy3d/__main__.py
--rw-r--r--   0        0        0     7201 2023-04-16 14:08:55.358491 pyxy3d-0.1.2/pyxy3d/calibration/__pycache__/charuco.cpython-310.pyc
--rw-r--r--   0        0        0     7111 2023-04-13 18:16:32.164621 pyxy3d-0.1.2/pyxy3d/calibration/__pycache__/charuco.cpython-38.pyc
--rw-r--r--   0        0        0     3147 2023-04-13 14:11:35.706111 pyxy3d-0.1.2/pyxy3d/calibration/__pycache__/corner_tracker.cpython-38.pyc
--rw-r--r--   0        0        0     1525 2023-04-13 21:33:14.966692 pyxy3d-0.1.2/pyxy3d/calibration/__pycache__/draw_charuco.cpython-310.pyc
--rw-r--r--   0        0        0     1517 2023-03-16 18:37:10.539737 pyxy3d-0.1.2/pyxy3d/calibration/__pycache__/draw_charuco.cpython-38.pyc
--rw-r--r--   0        0        0     7208 2023-06-12 18:45:04.367154 pyxy3d-0.1.2/pyxy3d/calibration/__pycache__/monocalibrator.cpython-310.pyc
--rw-r--r--   0        0        0     7083 2023-04-13 18:16:59.718066 pyxy3d-0.1.2/pyxy3d/calibration/__pycache__/monocalibrator.cpython-38.pyc
--rw-r--r--   0        0        0    11365 2023-03-16 18:37:11.887671 pyxy3d-0.1.2/pyxy3d/calibration/__pycache__/omnicalibrator.cpython-38.pyc
--rw-r--r--   0        0        0     7979 2023-06-08 18:19:03.652989 pyxy3d-0.1.2/pyxy3d/calibration/__pycache__/stereocalibrator.cpython-310.pyc
--rw-r--r--   0        0        0     7845 2023-04-13 14:31:07.431535 pyxy3d-0.1.2/pyxy3d/calibration/__pycache__/stereocalibrator.cpython-38.pyc
--rw-r--r--   0        0        0     7001 2023-06-12 12:22:25.787593 pyxy3d-0.1.2/pyxy3d/calibration/capture_volume/__pycache__/capture_volume.cpython-310.pyc
--rw-r--r--   0        0        0     8147 2023-04-11 10:38:21.551689 pyxy3d-0.1.2/pyxy3d/calibration/capture_volume/__pycache__/capture_volume.cpython-38.pyc
--rw-r--r--   0        0        0     3205 2023-05-02 22:08:30.018323 pyxy3d-0.1.2/pyxy3d/calibration/capture_volume/__pycache__/point_estimates.cpython-310.pyc
--rw-r--r--   0        0        0     3651 2023-04-09 20:26:50.741740 pyxy3d-0.1.2/pyxy3d/calibration/capture_volume/__pycache__/point_estimates.cpython-38.pyc
--rw-r--r--   0        0        0     9626 2023-05-22 14:59:39.828020 pyxy3d-0.1.2/pyxy3d/calibration/capture_volume/__pycache__/quality_controller.cpython-310.pyc
--rw-r--r--   0        0        0     9567 2023-04-13 18:47:12.691013 pyxy3d-0.1.2/pyxy3d/calibration/capture_volume/__pycache__/quality_controller.cpython-38.pyc
--rw-r--r--   0        0        0     7294 2023-05-22 14:59:39.817019 pyxy3d-0.1.2/pyxy3d/calibration/capture_volume/__pycache__/set_origin_functions.cpython-310.pyc
--rw-r--r--   0        0        0     7172 2023-04-06 11:06:35.216555 pyxy3d-0.1.2/pyxy3d/calibration/capture_volume/__pycache__/set_origin_functions.cpython-38.pyc
--rw-r--r--   0        0        0    10148 2023-06-12 12:14:10.017140 pyxy3d-0.1.2/pyxy3d/calibration/capture_volume/capture_volume.py
--rw-r--r--   0        0        0  1505952 2023-03-13 23:46:36.934749 pyxy3d-0.1.2/pyxy3d/calibration/capture_volume/capture_volume_stage_1.pkl
--rw-r--r--   0        0        0     2813 2023-04-13 21:41:08.181971 pyxy3d-0.1.2/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_point_estimates.cpython-310.pyc
--rw-r--r--   0        0        0     2825 2023-03-16 18:37:13.420982 pyxy3d-0.1.2/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_point_estimates.cpython-38.pyc
--rw-r--r--   0        0        0     2938 2023-04-16 14:08:57.590539 pyxy3d-0.1.2/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_stereotriangulated_table.cpython-310.pyc
--rw-r--r--   0        0        0     2963 2023-04-13 14:11:34.686199 pyxy3d-0.1.2/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_stereotriangulated_table.cpython-38.pyc
--rw-r--r--   0        0        0     3898 2023-03-16 18:13:11.445058 pyxy3d-0.1.2/pyxy3d/calibration/capture_volume/helper_functions/get_point_estimates.py
--rw-r--r--   0        0        0     4680 2023-04-16 12:58:12.386690 pyxy3d-0.1.2/pyxy3d/calibration/capture_volume/helper_functions/get_stereotriangulated_table.py
--rw-r--r--   0        0        0     3631 2023-05-02 22:08:10.575286 pyxy3d-0.1.2/pyxy3d/calibration/capture_volume/point_estimates.py
--rw-r--r--   0        0        0    15888 2023-05-22 13:44:00.083689 pyxy3d-0.1.2/pyxy3d/calibration/capture_volume/quality_controller.py
--rw-r--r--   0        0        0     1766 2023-03-16 18:13:11.448058 pyxy3d-0.1.2/pyxy3d/calibration/capture_volume/seaborn_summaries.py
--rw-r--r--   0        0        0    10868 2023-05-22 13:44:00.084688 pyxy3d-0.1.2/pyxy3d/calibration/capture_volume/set_origin_functions.py
--rw-r--r--   0        0        0     9510 2023-04-16 12:58:12.392689 pyxy3d-0.1.2/pyxy3d/calibration/charuco.py
--rw-r--r--   0        0        0     1685 2023-03-16 18:13:11.451057 pyxy3d-0.1.2/pyxy3d/calibration/draw_charuco.py
--rw-r--r--   0        0        0     9886 2023-06-12 16:49:05.518131 pyxy3d-0.1.2/pyxy3d/calibration/monocalibrator.py
--rw-r--r--   0        0        0    12385 2023-06-08 18:18:45.456813 pyxy3d-0.1.2/pyxy3d/calibration/stereocalibrator.py
--rw-r--r--   0        0        0     7119 2023-05-22 16:42:44.186443 pyxy3d-0.1.2/pyxy3d/cameras/__pycache__/camera.cpython-310.pyc
--rw-r--r--   0        0        0     7171 2023-04-12 14:56:03.753093 pyxy3d-0.1.2/pyxy3d/cameras/__pycache__/camera.cpython-38.pyc
--rw-r--r--   0        0        0     6788 2023-06-10 20:39:00.834305 pyxy3d-0.1.2/pyxy3d/cameras/__pycache__/camera_array.cpython-310.pyc
--rw-r--r--   0        0        0     6811 2023-04-09 20:26:50.029740 pyxy3d-0.1.2/pyxy3d/cameras/__pycache__/camera_array.cpython-38.pyc
--rw-r--r--   0        0        0     9199 2023-05-02 22:08:30.006322 pyxy3d-0.1.2/pyxy3d/cameras/__pycache__/camera_array_initializer.cpython-310.pyc
--rw-r--r--   0        0        0     9153 2023-04-06 11:06:35.358553 pyxy3d-0.1.2/pyxy3d/cameras/__pycache__/camera_array_initializer.cpython-38.pyc
--rw-r--r--   0        0        0     3161 2023-04-13 21:33:14.970692 pyxy3d-0.1.2/pyxy3d/cameras/__pycache__/data_packets.cpython-310.pyc
--rw-r--r--   0        0        0     3147 2023-04-13 17:33:55.370369 pyxy3d-0.1.2/pyxy3d/cameras/__pycache__/data_packets.cpython-38.pyc
--rw-r--r--   0        0        0     8085 2023-06-10 20:05:09.584549 pyxy3d-0.1.2/pyxy3d/cameras/__pycache__/live_stream.cpython-310.pyc
--rw-r--r--   0        0        0     8585 2023-04-13 17:33:56.274500 pyxy3d-0.1.2/pyxy3d/cameras/__pycache__/live_stream.cpython-38.pyc
--rw-r--r--   0        0        0     9900 2023-06-22 12:39:44.642763 pyxy3d-0.1.2/pyxy3d/cameras/__pycache__/synchronizer.cpython-310.pyc
--rw-r--r--   0        0        0    11042 2023-04-13 18:30:26.417813 pyxy3d-0.1.2/pyxy3d/cameras/__pycache__/synchronizer.cpython-38.pyc
--rw-r--r--   0        0        0    10631 2023-05-22 16:41:37.293000 pyxy3d-0.1.2/pyxy3d/cameras/camera.py
--rw-r--r--   0        0        0     7710 2023-06-10 20:38:54.275345 pyxy3d-0.1.2/pyxy3d/cameras/camera_array.py
--rw-r--r--   0        0        0    12868 2023-05-02 22:08:10.579286 pyxy3d-0.1.2/pyxy3d/cameras/camera_array_initializer.py
--rw-r--r--   0        0        0    11935 2023-06-10 20:04:58.799532 pyxy3d-0.1.2/pyxy3d/cameras/live_stream.py
--rw-r--r--   0        0        0    13543 2023-06-15 18:45:15.726954 pyxy3d-0.1.2/pyxy3d/cameras/synchronizer.py
--rw-r--r--   0        0        0    13040 2023-06-12 12:14:10.019141 pyxy3d-0.1.2/pyxy3d/configurator.py
--rw-r--r--   0        0        0     7036 2023-05-18 21:56:09.817280 pyxy3d-0.1.2/pyxy3d/export.py
--rw-r--r--   0        0        0     3538 2023-06-12 18:45:08.762112 pyxy3d-0.1.2/pyxy3d/gui/__pycache__/calibrate_capture_volume_widget.cpython-310.pyc
--rw-r--r--   0        0        0     5691 2023-06-22 12:39:42.763393 pyxy3d-0.1.2/pyxy3d/gui/__pycache__/calibration_widget.cpython-310.pyc
--rw-r--r--   0        0        0     8693 2023-05-06 16:11:05.603259 pyxy3d-0.1.2/pyxy3d/gui/__pycache__/calibration_wizard.cpython-310.pyc
--rw-r--r--   0        0        0     7124 2023-06-08 18:19:04.615289 pyxy3d-0.1.2/pyxy3d/gui/__pycache__/charuco_widget.cpython-310.pyc
--rw-r--r--   0        0        0     8558 2023-06-22 12:39:48.156709 pyxy3d-0.1.2/pyxy3d/gui/__pycache__/extrinsic_calibration_widget.cpython-310.pyc
--rw-r--r--   0        0        0     2110 2023-05-29 12:41:08.382954 pyxy3d-0.1.2/pyxy3d/gui/__pycache__/log_widget.cpython-310.pyc
--rw-r--r--   0        0        0     8811 2023-05-02 22:10:09.955994 pyxy3d-0.1.2/pyxy3d/gui/__pycache__/main.cpython-310.pyc
--rw-r--r--   0        0        0     8445 2023-04-12 14:19:14.529651 pyxy3d-0.1.2/pyxy3d/gui/__pycache__/main.cpython-38.pyc
--rw-r--r--   0        0        0    11710 2023-06-22 12:39:49.307577 pyxy3d-0.1.2/pyxy3d/gui/__pycache__/main_widget.cpython-310.pyc
--rw-r--r--   0        0        0     2664 2023-06-08 18:19:04.619290 pyxy3d-0.1.2/pyxy3d/gui/__pycache__/navigation_bars.cpython-310.pyc
--rw-r--r--   0        0        0     2468 2023-06-02 00:29:24.448977 pyxy3d-0.1.2/pyxy3d/gui/__pycache__/playback_widget.cpython-310.pyc
--rw-r--r--   0        0        0     9611 2023-06-10 20:31:20.063896 pyxy3d-0.1.2/pyxy3d/gui/__pycache__/post_processing_widget.cpython-310.pyc
--rw-r--r--   0        0        0     1176 2023-05-29 13:25:02.424999 pyxy3d-0.1.2/pyxy3d/gui/__pycache__/progress_dialog.cpython-310.pyc
--rw-r--r--   0        0        0     2649 2023-05-22 15:00:23.510630 pyxy3d-0.1.2/pyxy3d/gui/__pycache__/qt_logger.cpython-310.pyc
--rw-r--r--   0        0        0     2623 2023-04-06 18:40:19.597418 pyxy3d-0.1.2/pyxy3d/gui/__pycache__/qt_logger.cpython-38.pyc
--rw-r--r--   0        0        0    11942 2023-06-22 12:39:49.300575 pyxy3d-0.1.2/pyxy3d/gui/__pycache__/recording_widget.cpython-310.pyc
--rw-r--r--   0        0        0     8798 2023-04-12 14:17:47.475386 pyxy3d-0.1.2/pyxy3d/gui/__pycache__/recording_widget.cpython-38.pyc
--rw-r--r--   0        0        0     2641 2023-04-13 21:41:10.861210 pyxy3d-0.1.2/pyxy3d/gui/__pycache__/widgets.cpython-310.pyc
--rw-r--r--   0        0        0     2969 2023-04-06 18:40:19.600418 pyxy3d-0.1.2/pyxy3d/gui/__pycache__/widgets.cpython-38.pyc
--rw-r--r--   0        0        0     6864 2023-05-29 12:41:07.242642 pyxy3d-0.1.2/pyxy3d/gui/__pycache__/wizard_charuco.cpython-310.pyc
--rw-r--r--   0        0        0     6979 2023-04-06 18:40:19.594417 pyxy3d-0.1.2/pyxy3d/gui/__pycache__/wizard_charuco.cpython-38.pyc
--rw-r--r--   0        0        0     4851 2023-05-02 13:40:54.299559 pyxy3d-0.1.2/pyxy3d/gui/__pycache__/wizard_directory.cpython-310.pyc
--rw-r--r--   0        0        0     4903 2023-04-06 18:40:19.608417 pyxy3d-0.1.2/pyxy3d/gui/__pycache__/wizard_directory.cpython-38.pyc
--rw-r--r--   0        0        0     4052 2023-06-12 16:49:05.519131 pyxy3d-0.1.2/pyxy3d/gui/calibrate_capture_volume_widget.py
--rw-r--r--   0        0        0     7459 2023-06-15 18:45:15.727954 pyxy3d-0.1.2/pyxy3d/gui/calibration_widget.py
--rw-r--r--   0        0        0    13085 2023-06-02 16:06:24.614359 pyxy3d-0.1.2/pyxy3d/gui/camera_config/__pycache__/camera_config_dialogue.cpython-310.pyc
--rw-r--r--   0        0        0    13777 2023-03-29 13:33:28.389797 pyxy3d-0.1.2/pyxy3d/gui/camera_config/__pycache__/camera_config_dialogue.cpython-38.pyc
--rw-r--r--   0        0        0     3658 2023-06-10 20:05:11.213579 pyxy3d-0.1.2/pyxy3d/gui/camera_config/__pycache__/camera_summary_widget.cpython-310.pyc
--rw-r--r--   0        0        0     4748 2023-06-01 14:22:06.839277 pyxy3d-0.1.2/pyxy3d/gui/camera_config/__pycache__/camera_tabs.cpython-310.pyc
--rw-r--r--   0        0        0     3850 2023-03-20 23:10:53.097964 pyxy3d-0.1.2/pyxy3d/gui/camera_config/__pycache__/camera_tabs.cpython-38.pyc
--rw-r--r--   0        0        0     3155 2023-06-02 14:30:41.590277 pyxy3d-0.1.2/pyxy3d/gui/camera_config/__pycache__/frame_emitter.cpython-310.pyc
--rw-r--r--   0        0        0     2704 2023-03-16 18:37:13.513000 pyxy3d-0.1.2/pyxy3d/gui/camera_config/__pycache__/frame_emitter.cpython-38.pyc
--rw-r--r--   0        0        0     3619 2023-06-10 20:39:01.831691 pyxy3d-0.1.2/pyxy3d/gui/camera_config/__pycache__/intrinsic_calibration_widget.cpython-310.pyc
--rw-r--r--   0        0        0    17771 2023-06-02 15:39:41.317656 pyxy3d-0.1.2/pyxy3d/gui/camera_config/camera_config_dialogue.py
--rw-r--r--   0        0        0     5794 2023-06-10 20:04:49.727607 pyxy3d-0.1.2/pyxy3d/gui/camera_config/camera_summary_widget.py
--rw-r--r--   0        0        0     3893 2023-06-02 00:28:42.145417 pyxy3d-0.1.2/pyxy3d/gui/camera_config/frame_emitter.py
--rw-r--r--   0        0        0     3760 2023-06-10 20:38:54.278346 pyxy3d-0.1.2/pyxy3d/gui/camera_config/intrinsic_calibration_widget.py
--rw-r--r--   0        0        0    11157 2023-06-08 18:18:45.460813 pyxy3d-0.1.2/pyxy3d/gui/charuco_widget.py
--rw-r--r--   0        0        0    10800 2023-06-15 18:45:15.728953 pyxy3d-0.1.2/pyxy3d/gui/extrinsic_calibration_widget.py
--rw-r--r--   0        0        0     7468 2023-06-01 18:24:14.049008 pyxy3d-0.1.2/pyxy3d/gui/frame_builders/__pycache__/extrinsic_calibration_widget.cpython-310.pyc
--rw-r--r--   0        0        0     9143 2023-03-16 18:37:13.553998 pyxy3d-0.1.2/pyxy3d/gui/frame_builders/__pycache__/omni_frame_builder.cpython-38.pyc
--rw-r--r--   0        0        0     5691 2023-03-16 18:37:13.539983 pyxy3d-0.1.2/pyxy3d/gui/frame_builders/__pycache__/omni_frame_widget.cpython-38.pyc
--rw-r--r--   0        0        0     9669 2023-06-22 12:39:48.162709 pyxy3d-0.1.2/pyxy3d/gui/frame_builders/__pycache__/paired_frame_builder.cpython-310.pyc
--rw-r--r--   0        0        0     9881 2023-06-01 18:24:14.063003 pyxy3d-0.1.2/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_builder.cpython-310.pyc
--rw-r--r--   0        0        0    11456 2023-04-13 17:55:04.283828 pyxy3d-0.1.2/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_builder.cpython-38.pyc
--rw-r--r--   0        0        0     7359 2023-06-01 14:22:06.856278 pyxy3d-0.1.2/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_widget.cpython-310.pyc
--rw-r--r--   0        0        0     7148 2023-04-13 18:41:31.149308 pyxy3d-0.1.2/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_widget.cpython-38.pyc
--rw-r--r--   0        0        0    13851 2023-06-15 18:45:15.729953 pyxy3d-0.1.2/pyxy3d/gui/frame_builders/paired_frame_builder.py
--rw-r--r--   0        0        0    19878 2023-04-07 19:40:35.259432 pyxy3d-0.1.2/pyxy3d/gui/icons/pyxy_logo.svg
--rw-r--r--   0        0        0      941 2023-03-16 18:13:11.463060 pyxy3d-0.1.2/pyxy3d/gui/icons/rotate-camera-left.svg
--rw-r--r--   0        0        0      944 2023-03-16 18:13:11.464059 pyxy3d-0.1.2/pyxy3d/gui/icons/rotate-camera-right.svg
--rw-r--r--   0        0        0     2460 2023-05-28 21:21:33.674553 pyxy3d-0.1.2/pyxy3d/gui/log_widget.py
--rw-r--r--   0        0        0    16047 2023-06-15 18:45:15.731956 pyxy3d-0.1.2/pyxy3d/gui/main_widget.py
--rw-r--r--   0        0        0     3292 2023-06-08 18:18:45.464814 pyxy3d-0.1.2/pyxy3d/gui/navigation_bars.py
--rw-r--r--   0        0        0     1988 2023-06-02 00:28:42.150417 pyxy3d-0.1.2/pyxy3d/gui/playback_widget.py
--rw-r--r--   0        0        0    11310 2023-06-10 20:29:24.686837 pyxy3d-0.1.2/pyxy3d/gui/post_processing_widget.py
--rw-r--r--   0        0        0      950 2023-05-28 21:21:33.677553 pyxy3d-0.1.2/pyxy3d/gui/progress_dialog.py
--rw-r--r--   0        0        0    14740 2023-06-15 18:45:15.732954 pyxy3d-0.1.2/pyxy3d/gui/recording_widget.py
--rw-r--r--   0        0        0     6275 2023-05-13 12:35:31.914917 pyxy3d-0.1.2/pyxy3d/gui/vizualize/__pycache__/camera_mesh.cpython-310.pyc
--rw-r--r--   0        0        0     6278 2023-04-10 15:11:26.319020 pyxy3d-0.1.2/pyxy3d/gui/vizualize/__pycache__/camera_mesh.cpython-38.pyc
--rw-r--r--   0        0        0     3198 2023-03-27 01:11:02.734179 pyxy3d-0.1.2/pyxy3d/gui/vizualize/__pycache__/capture_volume_dialog.cpython-38.pyc
--rw-r--r--   0        0        0     5013 2023-04-08 17:08:48.219160 pyxy3d-0.1.2/pyxy3d/gui/vizualize/__pycache__/capture_volume_visualizer.cpython-38.pyc
--rw-r--r--   0        0        0     5850 2023-04-08 17:08:47.292159 pyxy3d-0.1.2/pyxy3d/gui/vizualize/__pycache__/capture_volume_widget.cpython-38.pyc
--rw-r--r--   0        0        0     4920 2023-06-12 12:22:29.640003 pyxy3d-0.1.2/pyxy3d/gui/vizualize/__pycache__/playback_triangulation_widget.cpython-310.pyc
--rw-r--r--   0        0        0     4522 2023-04-16 14:08:58.474682 pyxy3d-0.1.2/pyxy3d/gui/vizualize/__pycache__/realtime_triangulation_widget.cpython-310.pyc
--rw-r--r--   0        0        0     2999 2023-06-08 18:19:05.638538 pyxy3d-0.1.2/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_visualizer.cpython-310.pyc
--rw-r--r--   0        0        0     3506 2023-04-10 15:11:26.253010 pyxy3d-0.1.2/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_visualizer.cpython-38.pyc
--rw-r--r--   0        0        0     5838 2023-06-12 12:22:27.405313 pyxy3d-0.1.2/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_widget.cpython-310.pyc
--rw-r--r--   0        0        0     5615 2023-04-13 18:47:41.885491 pyxy3d-0.1.2/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_widget.cpython-38.pyc
--rw-r--r--   0        0        0     3404 2023-06-08 18:18:45.466812 pyxy3d-0.1.2/pyxy3d/gui/vizualize/calibration/capture_volume_visualizer.py
--rw-r--r--   0        0        0     6843 2023-06-12 12:14:10.025140 pyxy3d-0.1.2/pyxy3d/gui/vizualize/calibration/capture_volume_widget.py
--rw-r--r--   0        0        0     9146 2023-05-12 22:51:00.876793 pyxy3d-0.1.2/pyxy3d/gui/vizualize/camera_mesh.py
--rw-r--r--   0        0        0     5054 2023-06-12 12:14:10.027140 pyxy3d-0.1.2/pyxy3d/gui/vizualize/playback_triangulation_widget.py
--rw-r--r--   0        0        0     5450 2023-05-22 13:44:00.101687 pyxy3d-0.1.2/pyxy3d/gui/vizualize/realtime_triangulation_widget.py
--rw-r--r--   0        0        0     1135 2023-05-18 17:09:55.119648 pyxy3d-0.1.2/pyxy3d/helper.py
--rw-r--r--   0        0        0     6646 2023-06-15 00:37:58.434754 pyxy3d-0.1.2/pyxy3d/interface.py
--rw-r--r--   0        0        0     3111 2023-06-01 14:21:56.756810 pyxy3d-0.1.2/pyxy3d/logger.py
--rw-r--r--   0        0        0     7100 2023-06-12 12:14:10.028141 pyxy3d-0.1.2/pyxy3d/post_processor.py
--rw-r--r--   0        0        0     8482 2023-05-29 13:25:01.175649 pyxy3d-0.1.2/pyxy3d/recording/__pycache__/recorded_stream.cpython-310.pyc
--rw-r--r--   0        0        0     7603 2023-04-13 17:33:56.707496 pyxy3d-0.1.2/pyxy3d/recording/__pycache__/recorded_stream.cpython-38.pyc
--rw-r--r--   0        0        0     5928 2023-06-12 12:22:27.383610 pyxy3d-0.1.2/pyxy3d/recording/__pycache__/video_recorder.cpython-310.pyc
--rw-r--r--   0        0        0     5376 2023-04-13 14:11:36.908257 pyxy3d-0.1.2/pyxy3d/recording/__pycache__/video_recorder.cpython-38.pyc
--rw-r--r--   0        0        0    11830 2023-05-28 21:21:33.684552 pyxy3d-0.1.2/pyxy3d/recording/recorded_stream.py
--rw-r--r--   0        0        0     8730 2023-06-12 12:14:10.029141 pyxy3d-0.1.2/pyxy3d/recording/video_recorder.py
--rw-r--r--   0        0        0     2818 2023-06-05 20:04:19.162433 pyxy3d-0.1.2/pyxy3d/session/__pycache__/get_stage.cpython-310.pyc
--rw-r--r--   0        0        0    16304 2023-06-22 12:39:42.776391 pyxy3d-0.1.2/pyxy3d/session/__pycache__/session.cpython-310.pyc
--rw-r--r--   0        0        0    21437 2023-06-15 18:45:15.733955 pyxy3d-0.1.2/pyxy3d/session/session.py
--rw-r--r--   0        0        0        0 2023-04-16 12:58:12.408688 pyxy3d-0.1.2/pyxy3d/trackers/__init__.py
--rw-r--r--   0        0        0      153 2023-04-16 14:08:55.370508 pyxy3d-0.1.2/pyxy3d/trackers/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     3955 2023-05-13 12:35:24.878771 pyxy3d-0.1.2/pyxy3d/trackers/__pycache__/charuco_tracker.cpython-310.pyc
--rw-r--r--   0        0        0     3531 2023-05-13 12:35:26.254677 pyxy3d-0.1.2/pyxy3d/trackers/__pycache__/hand_tracker.cpython-310.pyc
--rw-r--r--   0        0        0     1123 2023-05-13 12:35:28.030304 pyxy3d-0.1.2/pyxy3d/trackers/__pycache__/helper.cpython-310.pyc
--rw-r--r--   0        0        0     6774 2023-05-18 18:02:52.161100 pyxy3d-0.1.2/pyxy3d/trackers/__pycache__/holistic_opensim_tracker.cpython-310.pyc
--rw-r--r--   0        0        0     6262 2023-05-13 12:35:28.041314 pyxy3d-0.1.2/pyxy3d/trackers/__pycache__/holistic_tracker.cpython-310.pyc
--rw-r--r--   0        0        0     3797 2023-05-13 12:35:28.036311 pyxy3d-0.1.2/pyxy3d/trackers/__pycache__/pose_tracker.cpython-310.pyc
--rw-r--r--   0        0        0     3515 2023-05-12 22:32:19.505484 pyxy3d-0.1.2/pyxy3d/trackers/__pycache__/threaded_hand_tracker.cpython-310.pyc
--rw-r--r--   0        0        0     1017 2023-05-18 18:02:48.968666 pyxy3d-0.1.2/pyxy3d/trackers/__pycache__/tracker_enum.cpython-310.pyc
--rw-r--r--   0        0        0     5004 2023-05-12 22:51:00.882792 pyxy3d-0.1.2/pyxy3d/trackers/charuco_tracker.py
--rw-r--r--   0        0        0     4651 2023-05-12 22:51:00.883791 pyxy3d-0.1.2/pyxy3d/trackers/hand_tracker.py
--rw-r--r--   0        0        0     1330 2023-05-12 22:51:00.884792 pyxy3d-0.1.2/pyxy3d/trackers/helper.py
--rw-r--r--   0        0        0    10677 2023-05-18 17:09:55.120646 pyxy3d-0.1.2/pyxy3d/trackers/holistic_opensim_tracker.py
--rw-r--r--   0        0        0     9419 2023-05-12 22:51:00.885792 pyxy3d-0.1.2/pyxy3d/trackers/holistic_tracker.py
--rw-r--r--   0        0        0     4239 2023-05-12 22:51:00.885792 pyxy3d-0.1.2/pyxy3d/trackers/pose_tracker.py
--rw-r--r--   0        0        0      669 2023-05-18 17:09:55.121648 pyxy3d-0.1.2/pyxy3d/trackers/tracker_enum.py
--rw-r--r--   0        0        0     5629 2023-04-16 14:08:57.598538 pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/array_stereo_triangulator.cpython-310.pyc
--rw-r--r--   0        0        0     5656 2023-04-13 17:33:55.945379 pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/array_stereo_triangulator.cpython-38.pyc
--rw-r--r--   0        0        0      564 2023-04-24 13:44:16.864821 pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/helper.cpython-310.pyc
--rw-r--r--   0        0        0     5809 2023-05-03 19:22:07.093614 pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/real_time_triangulator.cpython-310.pyc
--rw-r--r--   0        0        0     4640 2023-04-11 11:20:24.830020 pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/real_time_triangulator.cpython-38.pyc
--rw-r--r--   0        0        0   277847 2023-04-17 18:50:37.938076 pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-135.py310.1.nbc
--rw-r--r--   0        0        0   278178 2023-04-17 18:47:53.733008 pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-135.py310.2.nbc
--rw-r--r--   0        0        0     1853 2023-04-17 18:50:37.934076 pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-135.py310.nbi
--rw-r--r--   0        0        0   278065 2023-04-15 22:26:29.919720 pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py310.1.nbc
--rw-r--r--   0        0        0     1795 2023-04-15 22:26:29.916718 pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py310.nbi
--rw-r--r--   0        0        0   277525 2023-04-13 14:11:54.518242 pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py38.1.nbc
--rw-r--r--   0        0        0     1794 2023-04-13 14:11:54.515242 pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py38.nbi
--rw-r--r--   0        0        0   277847 2023-04-15 16:24:55.484079 pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-138.py310.1.nbc
--rw-r--r--   0        0        0     1853 2023-04-15 16:24:55.480077 pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-138.py310.nbi
--rw-r--r--   0        0        0   277847 2023-04-15 21:02:04.894614 pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-139.py310.1.nbc
--rw-r--r--   0        0        0     1853 2023-04-15 21:02:04.889631 pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-139.py310.nbi
--rw-r--r--   0        0        0   277790 2023-04-09 20:05:59.716347 pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-86.py38.1.nbc
--rw-r--r--   0        0        0     1793 2023-04-09 20:05:59.712345 pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-86.py38.nbi
--rw-r--r--   0        0        0   277795 2023-04-09 20:08:37.404028 pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-88.py38.1.nbc
--rw-r--r--   0        0        0     1793 2023-04-09 20:08:37.400042 pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-88.py38.nbi
--rw-r--r--   0        0        0    80840 2023-04-17 18:50:25.192073 pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/real_time_triangulator.unique_with_counts-118.py310.1.nbc
--rw-r--r--   0        0        0     1278 2023-04-17 18:50:25.189073 pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/real_time_triangulator.unique_with_counts-118.py310.nbi
--rw-r--r--   0        0        0     4903 2023-04-16 14:08:57.603539 pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/stereo_points_builder.cpython-310.pyc
--rw-r--r--   0        0        0     4910 2023-04-13 17:33:55.950369 pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/stereo_points_builder.cpython-38.pyc
--rw-r--r--   0        0        0     5522 2023-06-08 19:16:30.042145 pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.cpython-310.pyc
--rw-r--r--   0        0        0   277993 2023-06-10 20:35:53.847895 pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.1.nbc
--rw-r--r--   0        0        0   278337 2023-06-10 20:36:00.364127 pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.2.nbc
--rw-r--r--   0        0        0   275198 2023-06-10 20:36:15.587107 pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.3.nbc
--rw-r--r--   0        0        0     3826 2023-06-10 20:36:15.585108 pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.nbi
--rw-r--r--   0        0        0   274936 2023-05-07 17:31:11.859065 pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-170.py310.1.nbc
--rw-r--r--   0        0        0     1819 2023-05-07 17:31:11.856057 pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-170.py310.nbi
--rw-r--r--   0        0        0   280483 2023-05-11 20:37:44.633248 pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-186.py310.1.nbc
--rw-r--r--   0        0        0     1855 2023-05-11 20:37:44.630243 pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-186.py310.nbi
--rw-r--r--   0        0        0   277957 2023-05-11 19:51:33.032983 pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.1.nbc
--rw-r--r--   0        0        0   278013 2023-05-11 17:55:35.449169 pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.2.nbc
--rw-r--r--   0        0        0   278357 2023-05-11 17:56:15.957610 pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.3.nbc
--rw-r--r--   0        0        0     1855 2023-05-11 19:51:33.028983 pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.nbi
--rw-r--r--   0        0        0   277977 2023-05-11 20:58:46.910959 pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.1.nbc
--rw-r--r--   0        0        0   274956 2023-05-11 22:29:46.557422 pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.2.nbc
--rw-r--r--   0        0        0   280725 2023-05-12 22:34:01.184507 pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.3.nbc
--rw-r--r--   0        0        0     3913 2023-05-12 22:34:01.181521 pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.nbi
--rw-r--r--   0        0        0   274956 2023-05-13 12:36:45.045739 pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.1.nbc
--rw-r--r--   0        0        0   277993 2023-05-14 17:03:11.852980 pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.2.nbc
--rw-r--r--   0        0        0   278337 2023-05-14 17:03:18.755882 pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.3.nbc
--rw-r--r--   0        0        0     3855 2023-05-14 17:03:18.752878 pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.nbi
--rw-r--r--   0        0        0   278215 2023-05-12 22:36:41.576195 pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-195.py310.1.nbc
--rw-r--r--   0        0        0     1797 2023-05-12 22:36:41.573185 pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-195.py310.nbi
--rw-r--r--   0        0        0    80914 2023-06-10 20:35:46.176596 pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-152.py310.1.nbc
--rw-r--r--   0        0        0    77589 2023-06-10 20:36:11.729164 pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-152.py310.2.nbc
--rw-r--r--   0        0        0     2292 2023-06-10 20:36:11.727174 pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-152.py310.nbi
--rw-r--r--   0        0        0    77589 2023-05-10 14:04:48.307277 pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-153.py310.1.nbc
--rw-r--r--   0        0        0    80894 2023-05-09 20:10:40.338051 pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-153.py310.2.nbc
--rw-r--r--   0        0        0     1280 2023-05-10 14:04:48.305276 pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-153.py310.nbi
--rw-r--r--   0        0        0    80894 2023-05-11 20:37:03.860602 pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-170.py310.1.nbc
--rw-r--r--   0        0        0     1280 2023-05-11 20:37:03.857602 pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-170.py310.nbi
--rw-r--r--   0        0        0    80894 2023-05-11 19:51:22.690984 pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-172.py310.1.nbc
--rw-r--r--   0        0        0    80894 2023-05-11 17:55:29.550170 pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-172.py310.2.nbc
--rw-r--r--   0        0        0     1280 2023-05-11 19:51:22.687981 pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-172.py310.nbi
--rw-r--r--   0        0        0    80894 2023-05-11 20:58:36.790966 pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-173.py310.1.nbc
--rw-r--r--   0        0        0    77589 2023-05-11 22:29:37.429700 pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-173.py310.2.nbc
--rw-r--r--   0        0        0     2321 2023-05-11 22:29:37.426700 pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-173.py310.nbi
--rw-r--r--   0        0        0    77589 2023-05-13 12:36:36.027208 pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-178.py310.1.nbc
--rw-r--r--   0        0        0    80894 2023-05-14 17:03:04.107988 pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-178.py310.2.nbc
--rw-r--r--   0        0        0     2292 2023-05-14 17:03:04.102988 pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-178.py310.nbi
--rw-r--r--   0        0        0    80894 2023-05-12 22:36:32.819436 pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-179.py310.1.nbc
--rw-r--r--   0        0        0     1280 2023-05-12 22:36:32.816430 pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-179.py310.nbi
--rw-r--r--   0        0        0     5598 2023-04-04 19:53:34.784759 pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/triangulator.cpython-38.pyc
--rw-r--r--   0        0        0     8778 2023-04-16 12:58:12.413689 pyxy3d-0.1.2/pyxy3d/triangulate/array_stereo_triangulator.py
--rw-r--r--   0        0        0     5762 2023-04-16 12:58:12.416688 pyxy3d-0.1.2/pyxy3d/triangulate/stereo_points_builder.py
--rw-r--r--   0        0        0     7616 2023-06-08 19:15:56.173904 pyxy3d-0.1.2/pyxy3d/triangulate/sync_packet_triangulator.py
--rw-r--r--   0        0        0     6742 2023-06-22 12:20:08.052238 pyxy3d-0.1.2/README.md
--rw-r--r--   0        0        0     7560 1970-01-01 00:00:00.000000 pyxy3d-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    35190 2023-06-14 20:19:57.480906 pyxy3d-0.1.3/LICENSE.md
+-rw-r--r--   0        0        0      922 2023-06-22 13:04:36.844499 pyxy3d-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2644 2023-06-21 22:25:18.660194 pyxy3d-0.1.3/pyxy3d/__init__.py
+-rw-r--r--   0        0        0      934 2023-06-12 22:15:42.388447 pyxy3d-0.1.3/pyxy3d/__main__.py
+-rw-r--r--   0        0        0     7201 2023-04-16 14:08:55.358491 pyxy3d-0.1.3/pyxy3d/calibration/__pycache__/charuco.cpython-310.pyc
+-rw-r--r--   0        0        0     7111 2023-04-13 18:16:32.164621 pyxy3d-0.1.3/pyxy3d/calibration/__pycache__/charuco.cpython-38.pyc
+-rw-r--r--   0        0        0     3147 2023-04-13 14:11:35.706111 pyxy3d-0.1.3/pyxy3d/calibration/__pycache__/corner_tracker.cpython-38.pyc
+-rw-r--r--   0        0        0     1525 2023-04-13 21:33:14.966692 pyxy3d-0.1.3/pyxy3d/calibration/__pycache__/draw_charuco.cpython-310.pyc
+-rw-r--r--   0        0        0     1517 2023-03-16 18:37:10.539737 pyxy3d-0.1.3/pyxy3d/calibration/__pycache__/draw_charuco.cpython-38.pyc
+-rw-r--r--   0        0        0     7208 2023-06-12 18:45:04.367154 pyxy3d-0.1.3/pyxy3d/calibration/__pycache__/monocalibrator.cpython-310.pyc
+-rw-r--r--   0        0        0     7083 2023-04-13 18:16:59.718066 pyxy3d-0.1.3/pyxy3d/calibration/__pycache__/monocalibrator.cpython-38.pyc
+-rw-r--r--   0        0        0    11365 2023-03-16 18:37:11.887671 pyxy3d-0.1.3/pyxy3d/calibration/__pycache__/omnicalibrator.cpython-38.pyc
+-rw-r--r--   0        0        0     7979 2023-06-08 18:19:03.652989 pyxy3d-0.1.3/pyxy3d/calibration/__pycache__/stereocalibrator.cpython-310.pyc
+-rw-r--r--   0        0        0     7845 2023-04-13 14:31:07.431535 pyxy3d-0.1.3/pyxy3d/calibration/__pycache__/stereocalibrator.cpython-38.pyc
+-rw-r--r--   0        0        0     7001 2023-06-12 12:22:25.787593 pyxy3d-0.1.3/pyxy3d/calibration/capture_volume/__pycache__/capture_volume.cpython-310.pyc
+-rw-r--r--   0        0        0     8147 2023-04-11 10:38:21.551689 pyxy3d-0.1.3/pyxy3d/calibration/capture_volume/__pycache__/capture_volume.cpython-38.pyc
+-rw-r--r--   0        0        0     3205 2023-05-02 22:08:30.018323 pyxy3d-0.1.3/pyxy3d/calibration/capture_volume/__pycache__/point_estimates.cpython-310.pyc
+-rw-r--r--   0        0        0     3651 2023-04-09 20:26:50.741740 pyxy3d-0.1.3/pyxy3d/calibration/capture_volume/__pycache__/point_estimates.cpython-38.pyc
+-rw-r--r--   0        0        0     9626 2023-05-22 14:59:39.828020 pyxy3d-0.1.3/pyxy3d/calibration/capture_volume/__pycache__/quality_controller.cpython-310.pyc
+-rw-r--r--   0        0        0     9567 2023-04-13 18:47:12.691013 pyxy3d-0.1.3/pyxy3d/calibration/capture_volume/__pycache__/quality_controller.cpython-38.pyc
+-rw-r--r--   0        0        0     7294 2023-05-22 14:59:39.817019 pyxy3d-0.1.3/pyxy3d/calibration/capture_volume/__pycache__/set_origin_functions.cpython-310.pyc
+-rw-r--r--   0        0        0     7172 2023-04-06 11:06:35.216555 pyxy3d-0.1.3/pyxy3d/calibration/capture_volume/__pycache__/set_origin_functions.cpython-38.pyc
+-rw-r--r--   0        0        0    10148 2023-06-12 12:14:10.017140 pyxy3d-0.1.3/pyxy3d/calibration/capture_volume/capture_volume.py
+-rw-r--r--   0        0        0  1505952 2023-03-13 23:46:36.934749 pyxy3d-0.1.3/pyxy3d/calibration/capture_volume/capture_volume_stage_1.pkl
+-rw-r--r--   0        0        0     2813 2023-04-13 21:41:08.181971 pyxy3d-0.1.3/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_point_estimates.cpython-310.pyc
+-rw-r--r--   0        0        0     2825 2023-03-16 18:37:13.420982 pyxy3d-0.1.3/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_point_estimates.cpython-38.pyc
+-rw-r--r--   0        0        0     2938 2023-04-16 14:08:57.590539 pyxy3d-0.1.3/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_stereotriangulated_table.cpython-310.pyc
+-rw-r--r--   0        0        0     2963 2023-04-13 14:11:34.686199 pyxy3d-0.1.3/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_stereotriangulated_table.cpython-38.pyc
+-rw-r--r--   0        0        0     3898 2023-03-16 18:13:11.445058 pyxy3d-0.1.3/pyxy3d/calibration/capture_volume/helper_functions/get_point_estimates.py
+-rw-r--r--   0        0        0     4680 2023-04-16 12:58:12.386690 pyxy3d-0.1.3/pyxy3d/calibration/capture_volume/helper_functions/get_stereotriangulated_table.py
+-rw-r--r--   0        0        0     3631 2023-05-02 22:08:10.575286 pyxy3d-0.1.3/pyxy3d/calibration/capture_volume/point_estimates.py
+-rw-r--r--   0        0        0    15888 2023-05-22 13:44:00.083689 pyxy3d-0.1.3/pyxy3d/calibration/capture_volume/quality_controller.py
+-rw-r--r--   0        0        0     1766 2023-03-16 18:13:11.448058 pyxy3d-0.1.3/pyxy3d/calibration/capture_volume/seaborn_summaries.py
+-rw-r--r--   0        0        0    10868 2023-05-22 13:44:00.084688 pyxy3d-0.1.3/pyxy3d/calibration/capture_volume/set_origin_functions.py
+-rw-r--r--   0        0        0     9510 2023-04-16 12:58:12.392689 pyxy3d-0.1.3/pyxy3d/calibration/charuco.py
+-rw-r--r--   0        0        0     1685 2023-03-16 18:13:11.451057 pyxy3d-0.1.3/pyxy3d/calibration/draw_charuco.py
+-rw-r--r--   0        0        0     9886 2023-06-12 16:49:05.518131 pyxy3d-0.1.3/pyxy3d/calibration/monocalibrator.py
+-rw-r--r--   0        0        0    12385 2023-06-08 18:18:45.456813 pyxy3d-0.1.3/pyxy3d/calibration/stereocalibrator.py
+-rw-r--r--   0        0        0     7119 2023-05-22 16:42:44.186443 pyxy3d-0.1.3/pyxy3d/cameras/__pycache__/camera.cpython-310.pyc
+-rw-r--r--   0        0        0     7171 2023-04-12 14:56:03.753093 pyxy3d-0.1.3/pyxy3d/cameras/__pycache__/camera.cpython-38.pyc
+-rw-r--r--   0        0        0     6788 2023-06-10 20:39:00.834305 pyxy3d-0.1.3/pyxy3d/cameras/__pycache__/camera_array.cpython-310.pyc
+-rw-r--r--   0        0        0     6811 2023-04-09 20:26:50.029740 pyxy3d-0.1.3/pyxy3d/cameras/__pycache__/camera_array.cpython-38.pyc
+-rw-r--r--   0        0        0     9199 2023-05-02 22:08:30.006322 pyxy3d-0.1.3/pyxy3d/cameras/__pycache__/camera_array_initializer.cpython-310.pyc
+-rw-r--r--   0        0        0     9153 2023-04-06 11:06:35.358553 pyxy3d-0.1.3/pyxy3d/cameras/__pycache__/camera_array_initializer.cpython-38.pyc
+-rw-r--r--   0        0        0     3161 2023-04-13 21:33:14.970692 pyxy3d-0.1.3/pyxy3d/cameras/__pycache__/data_packets.cpython-310.pyc
+-rw-r--r--   0        0        0     3147 2023-04-13 17:33:55.370369 pyxy3d-0.1.3/pyxy3d/cameras/__pycache__/data_packets.cpython-38.pyc
+-rw-r--r--   0        0        0     8085 2023-06-10 20:05:09.584549 pyxy3d-0.1.3/pyxy3d/cameras/__pycache__/live_stream.cpython-310.pyc
+-rw-r--r--   0        0        0     8585 2023-04-13 17:33:56.274500 pyxy3d-0.1.3/pyxy3d/cameras/__pycache__/live_stream.cpython-38.pyc
+-rw-r--r--   0        0        0     9900 2023-06-22 12:39:44.642763 pyxy3d-0.1.3/pyxy3d/cameras/__pycache__/synchronizer.cpython-310.pyc
+-rw-r--r--   0        0        0    11042 2023-04-13 18:30:26.417813 pyxy3d-0.1.3/pyxy3d/cameras/__pycache__/synchronizer.cpython-38.pyc
+-rw-r--r--   0        0        0    10631 2023-05-22 16:41:37.293000 pyxy3d-0.1.3/pyxy3d/cameras/camera.py
+-rw-r--r--   0        0        0     7710 2023-06-10 20:38:54.275345 pyxy3d-0.1.3/pyxy3d/cameras/camera_array.py
+-rw-r--r--   0        0        0    12868 2023-05-02 22:08:10.579286 pyxy3d-0.1.3/pyxy3d/cameras/camera_array_initializer.py
+-rw-r--r--   0        0        0    11935 2023-06-10 20:04:58.799532 pyxy3d-0.1.3/pyxy3d/cameras/live_stream.py
+-rw-r--r--   0        0        0    13543 2023-06-15 18:45:15.726954 pyxy3d-0.1.3/pyxy3d/cameras/synchronizer.py
+-rw-r--r--   0        0        0    13040 2023-06-12 12:14:10.019141 pyxy3d-0.1.3/pyxy3d/configurator.py
+-rw-r--r--   0        0        0     7036 2023-05-18 21:56:09.817280 pyxy3d-0.1.3/pyxy3d/export.py
+-rw-r--r--   0        0        0     3538 2023-06-12 18:45:08.762112 pyxy3d-0.1.3/pyxy3d/gui/__pycache__/calibrate_capture_volume_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     5691 2023-06-22 12:39:42.763393 pyxy3d-0.1.3/pyxy3d/gui/__pycache__/calibration_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     8693 2023-05-06 16:11:05.603259 pyxy3d-0.1.3/pyxy3d/gui/__pycache__/calibration_wizard.cpython-310.pyc
+-rw-r--r--   0        0        0     7124 2023-06-08 18:19:04.615289 pyxy3d-0.1.3/pyxy3d/gui/__pycache__/charuco_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     8558 2023-06-22 12:39:48.156709 pyxy3d-0.1.3/pyxy3d/gui/__pycache__/extrinsic_calibration_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     2110 2023-05-29 12:41:08.382954 pyxy3d-0.1.3/pyxy3d/gui/__pycache__/log_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     8811 2023-05-02 22:10:09.955994 pyxy3d-0.1.3/pyxy3d/gui/__pycache__/main.cpython-310.pyc
+-rw-r--r--   0        0        0     8445 2023-04-12 14:19:14.529651 pyxy3d-0.1.3/pyxy3d/gui/__pycache__/main.cpython-38.pyc
+-rw-r--r--   0        0        0    11710 2023-06-22 12:39:49.307577 pyxy3d-0.1.3/pyxy3d/gui/__pycache__/main_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     2664 2023-06-08 18:19:04.619290 pyxy3d-0.1.3/pyxy3d/gui/__pycache__/navigation_bars.cpython-310.pyc
+-rw-r--r--   0        0        0     2468 2023-06-02 00:29:24.448977 pyxy3d-0.1.3/pyxy3d/gui/__pycache__/playback_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     9611 2023-06-10 20:31:20.063896 pyxy3d-0.1.3/pyxy3d/gui/__pycache__/post_processing_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     1176 2023-05-29 13:25:02.424999 pyxy3d-0.1.3/pyxy3d/gui/__pycache__/progress_dialog.cpython-310.pyc
+-rw-r--r--   0        0        0     2649 2023-05-22 15:00:23.510630 pyxy3d-0.1.3/pyxy3d/gui/__pycache__/qt_logger.cpython-310.pyc
+-rw-r--r--   0        0        0     2623 2023-04-06 18:40:19.597418 pyxy3d-0.1.3/pyxy3d/gui/__pycache__/qt_logger.cpython-38.pyc
+-rw-r--r--   0        0        0    11942 2023-06-22 12:39:49.300575 pyxy3d-0.1.3/pyxy3d/gui/__pycache__/recording_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     8798 2023-04-12 14:17:47.475386 pyxy3d-0.1.3/pyxy3d/gui/__pycache__/recording_widget.cpython-38.pyc
+-rw-r--r--   0        0        0     2641 2023-04-13 21:41:10.861210 pyxy3d-0.1.3/pyxy3d/gui/__pycache__/widgets.cpython-310.pyc
+-rw-r--r--   0        0        0     2969 2023-04-06 18:40:19.600418 pyxy3d-0.1.3/pyxy3d/gui/__pycache__/widgets.cpython-38.pyc
+-rw-r--r--   0        0        0     6864 2023-05-29 12:41:07.242642 pyxy3d-0.1.3/pyxy3d/gui/__pycache__/wizard_charuco.cpython-310.pyc
+-rw-r--r--   0        0        0     6979 2023-04-06 18:40:19.594417 pyxy3d-0.1.3/pyxy3d/gui/__pycache__/wizard_charuco.cpython-38.pyc
+-rw-r--r--   0        0        0     4851 2023-05-02 13:40:54.299559 pyxy3d-0.1.3/pyxy3d/gui/__pycache__/wizard_directory.cpython-310.pyc
+-rw-r--r--   0        0        0     4903 2023-04-06 18:40:19.608417 pyxy3d-0.1.3/pyxy3d/gui/__pycache__/wizard_directory.cpython-38.pyc
+-rw-r--r--   0        0        0     4052 2023-06-12 16:49:05.519131 pyxy3d-0.1.3/pyxy3d/gui/calibrate_capture_volume_widget.py
+-rw-r--r--   0        0        0     7459 2023-06-15 18:45:15.727954 pyxy3d-0.1.3/pyxy3d/gui/calibration_widget.py
+-rw-r--r--   0        0        0    13085 2023-06-02 16:06:24.614359 pyxy3d-0.1.3/pyxy3d/gui/camera_config/__pycache__/camera_config_dialogue.cpython-310.pyc
+-rw-r--r--   0        0        0    13777 2023-03-29 13:33:28.389797 pyxy3d-0.1.3/pyxy3d/gui/camera_config/__pycache__/camera_config_dialogue.cpython-38.pyc
+-rw-r--r--   0        0        0     3658 2023-06-10 20:05:11.213579 pyxy3d-0.1.3/pyxy3d/gui/camera_config/__pycache__/camera_summary_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     4748 2023-06-01 14:22:06.839277 pyxy3d-0.1.3/pyxy3d/gui/camera_config/__pycache__/camera_tabs.cpython-310.pyc
+-rw-r--r--   0        0        0     3850 2023-03-20 23:10:53.097964 pyxy3d-0.1.3/pyxy3d/gui/camera_config/__pycache__/camera_tabs.cpython-38.pyc
+-rw-r--r--   0        0        0     3155 2023-06-02 14:30:41.590277 pyxy3d-0.1.3/pyxy3d/gui/camera_config/__pycache__/frame_emitter.cpython-310.pyc
+-rw-r--r--   0        0        0     2704 2023-03-16 18:37:13.513000 pyxy3d-0.1.3/pyxy3d/gui/camera_config/__pycache__/frame_emitter.cpython-38.pyc
+-rw-r--r--   0        0        0     3619 2023-06-10 20:39:01.831691 pyxy3d-0.1.3/pyxy3d/gui/camera_config/__pycache__/intrinsic_calibration_widget.cpython-310.pyc
+-rw-r--r--   0        0        0    17771 2023-06-02 15:39:41.317656 pyxy3d-0.1.3/pyxy3d/gui/camera_config/camera_config_dialogue.py
+-rw-r--r--   0        0        0     5794 2023-06-10 20:04:49.727607 pyxy3d-0.1.3/pyxy3d/gui/camera_config/camera_summary_widget.py
+-rw-r--r--   0        0        0     3893 2023-06-02 00:28:42.145417 pyxy3d-0.1.3/pyxy3d/gui/camera_config/frame_emitter.py
+-rw-r--r--   0        0        0     3760 2023-06-10 20:38:54.278346 pyxy3d-0.1.3/pyxy3d/gui/camera_config/intrinsic_calibration_widget.py
+-rw-r--r--   0        0        0    11157 2023-06-08 18:18:45.460813 pyxy3d-0.1.3/pyxy3d/gui/charuco_widget.py
+-rw-r--r--   0        0        0    10800 2023-06-15 18:45:15.728953 pyxy3d-0.1.3/pyxy3d/gui/extrinsic_calibration_widget.py
+-rw-r--r--   0        0        0     7468 2023-06-01 18:24:14.049008 pyxy3d-0.1.3/pyxy3d/gui/frame_builders/__pycache__/extrinsic_calibration_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     9143 2023-03-16 18:37:13.553998 pyxy3d-0.1.3/pyxy3d/gui/frame_builders/__pycache__/omni_frame_builder.cpython-38.pyc
+-rw-r--r--   0        0        0     5691 2023-03-16 18:37:13.539983 pyxy3d-0.1.3/pyxy3d/gui/frame_builders/__pycache__/omni_frame_widget.cpython-38.pyc
+-rw-r--r--   0        0        0     9669 2023-06-22 12:39:48.162709 pyxy3d-0.1.3/pyxy3d/gui/frame_builders/__pycache__/paired_frame_builder.cpython-310.pyc
+-rw-r--r--   0        0        0     9881 2023-06-01 18:24:14.063003 pyxy3d-0.1.3/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_builder.cpython-310.pyc
+-rw-r--r--   0        0        0    11456 2023-04-13 17:55:04.283828 pyxy3d-0.1.3/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_builder.cpython-38.pyc
+-rw-r--r--   0        0        0     7359 2023-06-01 14:22:06.856278 pyxy3d-0.1.3/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     7148 2023-04-13 18:41:31.149308 pyxy3d-0.1.3/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_widget.cpython-38.pyc
+-rw-r--r--   0        0        0    13851 2023-06-15 18:45:15.729953 pyxy3d-0.1.3/pyxy3d/gui/frame_builders/paired_frame_builder.py
+-rw-r--r--   0        0        0    19878 2023-04-07 19:40:35.259432 pyxy3d-0.1.3/pyxy3d/gui/icons/pyxy_logo.svg
+-rw-r--r--   0        0        0      941 2023-03-16 18:13:11.463060 pyxy3d-0.1.3/pyxy3d/gui/icons/rotate-camera-left.svg
+-rw-r--r--   0        0        0      944 2023-03-16 18:13:11.464059 pyxy3d-0.1.3/pyxy3d/gui/icons/rotate-camera-right.svg
+-rw-r--r--   0        0        0     2460 2023-05-28 21:21:33.674553 pyxy3d-0.1.3/pyxy3d/gui/log_widget.py
+-rw-r--r--   0        0        0    16047 2023-06-15 18:45:15.731956 pyxy3d-0.1.3/pyxy3d/gui/main_widget.py
+-rw-r--r--   0        0        0     3292 2023-06-08 18:18:45.464814 pyxy3d-0.1.3/pyxy3d/gui/navigation_bars.py
+-rw-r--r--   0        0        0     1988 2023-06-02 00:28:42.150417 pyxy3d-0.1.3/pyxy3d/gui/playback_widget.py
+-rw-r--r--   0        0        0    11310 2023-06-10 20:29:24.686837 pyxy3d-0.1.3/pyxy3d/gui/post_processing_widget.py
+-rw-r--r--   0        0        0      950 2023-05-28 21:21:33.677553 pyxy3d-0.1.3/pyxy3d/gui/progress_dialog.py
+-rw-r--r--   0        0        0    14740 2023-06-15 18:45:15.732954 pyxy3d-0.1.3/pyxy3d/gui/recording_widget.py
+-rw-r--r--   0        0        0     6275 2023-05-13 12:35:31.914917 pyxy3d-0.1.3/pyxy3d/gui/vizualize/__pycache__/camera_mesh.cpython-310.pyc
+-rw-r--r--   0        0        0     6278 2023-04-10 15:11:26.319020 pyxy3d-0.1.3/pyxy3d/gui/vizualize/__pycache__/camera_mesh.cpython-38.pyc
+-rw-r--r--   0        0        0     3198 2023-03-27 01:11:02.734179 pyxy3d-0.1.3/pyxy3d/gui/vizualize/__pycache__/capture_volume_dialog.cpython-38.pyc
+-rw-r--r--   0        0        0     5013 2023-04-08 17:08:48.219160 pyxy3d-0.1.3/pyxy3d/gui/vizualize/__pycache__/capture_volume_visualizer.cpython-38.pyc
+-rw-r--r--   0        0        0     5850 2023-04-08 17:08:47.292159 pyxy3d-0.1.3/pyxy3d/gui/vizualize/__pycache__/capture_volume_widget.cpython-38.pyc
+-rw-r--r--   0        0        0     4920 2023-06-12 12:22:29.640003 pyxy3d-0.1.3/pyxy3d/gui/vizualize/__pycache__/playback_triangulation_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     4522 2023-04-16 14:08:58.474682 pyxy3d-0.1.3/pyxy3d/gui/vizualize/__pycache__/realtime_triangulation_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     2999 2023-06-08 18:19:05.638538 pyxy3d-0.1.3/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_visualizer.cpython-310.pyc
+-rw-r--r--   0        0        0     3506 2023-04-10 15:11:26.253010 pyxy3d-0.1.3/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_visualizer.cpython-38.pyc
+-rw-r--r--   0        0        0     5838 2023-06-12 12:22:27.405313 pyxy3d-0.1.3/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     5615 2023-04-13 18:47:41.885491 pyxy3d-0.1.3/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_widget.cpython-38.pyc
+-rw-r--r--   0        0        0     3404 2023-06-08 18:18:45.466812 pyxy3d-0.1.3/pyxy3d/gui/vizualize/calibration/capture_volume_visualizer.py
+-rw-r--r--   0        0        0     6843 2023-06-12 12:14:10.025140 pyxy3d-0.1.3/pyxy3d/gui/vizualize/calibration/capture_volume_widget.py
+-rw-r--r--   0        0        0     9146 2023-05-12 22:51:00.876793 pyxy3d-0.1.3/pyxy3d/gui/vizualize/camera_mesh.py
+-rw-r--r--   0        0        0     5054 2023-06-12 12:14:10.027140 pyxy3d-0.1.3/pyxy3d/gui/vizualize/playback_triangulation_widget.py
+-rw-r--r--   0        0        0     5450 2023-05-22 13:44:00.101687 pyxy3d-0.1.3/pyxy3d/gui/vizualize/realtime_triangulation_widget.py
+-rw-r--r--   0        0        0     1135 2023-05-18 17:09:55.119648 pyxy3d-0.1.3/pyxy3d/helper.py
+-rw-r--r--   0        0        0     6646 2023-06-15 00:37:58.434754 pyxy3d-0.1.3/pyxy3d/interface.py
+-rw-r--r--   0        0        0     3111 2023-06-01 14:21:56.756810 pyxy3d-0.1.3/pyxy3d/logger.py
+-rw-r--r--   0        0        0     7100 2023-06-12 12:14:10.028141 pyxy3d-0.1.3/pyxy3d/post_processor.py
+-rw-r--r--   0        0        0     8482 2023-05-29 13:25:01.175649 pyxy3d-0.1.3/pyxy3d/recording/__pycache__/recorded_stream.cpython-310.pyc
+-rw-r--r--   0        0        0     7603 2023-04-13 17:33:56.707496 pyxy3d-0.1.3/pyxy3d/recording/__pycache__/recorded_stream.cpython-38.pyc
+-rw-r--r--   0        0        0     5928 2023-06-12 12:22:27.383610 pyxy3d-0.1.3/pyxy3d/recording/__pycache__/video_recorder.cpython-310.pyc
+-rw-r--r--   0        0        0     5376 2023-04-13 14:11:36.908257 pyxy3d-0.1.3/pyxy3d/recording/__pycache__/video_recorder.cpython-38.pyc
+-rw-r--r--   0        0        0    11830 2023-05-28 21:21:33.684552 pyxy3d-0.1.3/pyxy3d/recording/recorded_stream.py
+-rw-r--r--   0        0        0     8730 2023-06-12 12:14:10.029141 pyxy3d-0.1.3/pyxy3d/recording/video_recorder.py
+-rw-r--r--   0        0        0     2818 2023-06-05 20:04:19.162433 pyxy3d-0.1.3/pyxy3d/session/__pycache__/get_stage.cpython-310.pyc
+-rw-r--r--   0        0        0    16304 2023-06-22 12:39:42.776391 pyxy3d-0.1.3/pyxy3d/session/__pycache__/session.cpython-310.pyc
+-rw-r--r--   0        0        0    21437 2023-06-15 18:45:15.733955 pyxy3d-0.1.3/pyxy3d/session/session.py
+-rw-r--r--   0        0        0        0 2023-04-16 12:58:12.408688 pyxy3d-0.1.3/pyxy3d/trackers/__init__.py
+-rw-r--r--   0        0        0      153 2023-04-16 14:08:55.370508 pyxy3d-0.1.3/pyxy3d/trackers/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3955 2023-05-13 12:35:24.878771 pyxy3d-0.1.3/pyxy3d/trackers/__pycache__/charuco_tracker.cpython-310.pyc
+-rw-r--r--   0        0        0     3531 2023-05-13 12:35:26.254677 pyxy3d-0.1.3/pyxy3d/trackers/__pycache__/hand_tracker.cpython-310.pyc
+-rw-r--r--   0        0        0     1123 2023-05-13 12:35:28.030304 pyxy3d-0.1.3/pyxy3d/trackers/__pycache__/helper.cpython-310.pyc
+-rw-r--r--   0        0        0     6774 2023-05-18 18:02:52.161100 pyxy3d-0.1.3/pyxy3d/trackers/__pycache__/holistic_opensim_tracker.cpython-310.pyc
+-rw-r--r--   0        0        0     6262 2023-05-13 12:35:28.041314 pyxy3d-0.1.3/pyxy3d/trackers/__pycache__/holistic_tracker.cpython-310.pyc
+-rw-r--r--   0        0        0     3797 2023-05-13 12:35:28.036311 pyxy3d-0.1.3/pyxy3d/trackers/__pycache__/pose_tracker.cpython-310.pyc
+-rw-r--r--   0        0        0     3515 2023-05-12 22:32:19.505484 pyxy3d-0.1.3/pyxy3d/trackers/__pycache__/threaded_hand_tracker.cpython-310.pyc
+-rw-r--r--   0        0        0     1017 2023-05-18 18:02:48.968666 pyxy3d-0.1.3/pyxy3d/trackers/__pycache__/tracker_enum.cpython-310.pyc
+-rw-r--r--   0        0        0     5004 2023-05-12 22:51:00.882792 pyxy3d-0.1.3/pyxy3d/trackers/charuco_tracker.py
+-rw-r--r--   0        0        0     4651 2023-05-12 22:51:00.883791 pyxy3d-0.1.3/pyxy3d/trackers/hand_tracker.py
+-rw-r--r--   0        0        0     1330 2023-05-12 22:51:00.884792 pyxy3d-0.1.3/pyxy3d/trackers/helper.py
+-rw-r--r--   0        0        0    10677 2023-05-18 17:09:55.120646 pyxy3d-0.1.3/pyxy3d/trackers/holistic_opensim_tracker.py
+-rw-r--r--   0        0        0     9419 2023-05-12 22:51:00.885792 pyxy3d-0.1.3/pyxy3d/trackers/holistic_tracker.py
+-rw-r--r--   0        0        0     4239 2023-05-12 22:51:00.885792 pyxy3d-0.1.3/pyxy3d/trackers/pose_tracker.py
+-rw-r--r--   0        0        0      669 2023-05-18 17:09:55.121648 pyxy3d-0.1.3/pyxy3d/trackers/tracker_enum.py
+-rw-r--r--   0        0        0     5629 2023-04-16 14:08:57.598538 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/array_stereo_triangulator.cpython-310.pyc
+-rw-r--r--   0        0        0     5656 2023-04-13 17:33:55.945379 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/array_stereo_triangulator.cpython-38.pyc
+-rw-r--r--   0        0        0      564 2023-04-24 13:44:16.864821 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/helper.cpython-310.pyc
+-rw-r--r--   0        0        0     5809 2023-05-03 19:22:07.093614 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/real_time_triangulator.cpython-310.pyc
+-rw-r--r--   0        0        0     4640 2023-04-11 11:20:24.830020 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/real_time_triangulator.cpython-38.pyc
+-rw-r--r--   0        0        0   277847 2023-04-17 18:50:37.938076 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-135.py310.1.nbc
+-rw-r--r--   0        0        0   278178 2023-04-17 18:47:53.733008 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-135.py310.2.nbc
+-rw-r--r--   0        0        0     1853 2023-04-17 18:50:37.934076 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-135.py310.nbi
+-rw-r--r--   0        0        0   278065 2023-04-15 22:26:29.919720 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py310.1.nbc
+-rw-r--r--   0        0        0     1795 2023-04-15 22:26:29.916718 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py310.nbi
+-rw-r--r--   0        0        0   277525 2023-04-13 14:11:54.518242 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py38.1.nbc
+-rw-r--r--   0        0        0     1794 2023-04-13 14:11:54.515242 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py38.nbi
+-rw-r--r--   0        0        0   277847 2023-04-15 16:24:55.484079 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-138.py310.1.nbc
+-rw-r--r--   0        0        0     1853 2023-04-15 16:24:55.480077 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-138.py310.nbi
+-rw-r--r--   0        0        0   277847 2023-04-15 21:02:04.894614 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-139.py310.1.nbc
+-rw-r--r--   0        0        0     1853 2023-04-15 21:02:04.889631 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-139.py310.nbi
+-rw-r--r--   0        0        0   277790 2023-04-09 20:05:59.716347 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-86.py38.1.nbc
+-rw-r--r--   0        0        0     1793 2023-04-09 20:05:59.712345 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-86.py38.nbi
+-rw-r--r--   0        0        0   277795 2023-04-09 20:08:37.404028 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-88.py38.1.nbc
+-rw-r--r--   0        0        0     1793 2023-04-09 20:08:37.400042 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-88.py38.nbi
+-rw-r--r--   0        0        0    80840 2023-04-17 18:50:25.192073 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/real_time_triangulator.unique_with_counts-118.py310.1.nbc
+-rw-r--r--   0        0        0     1278 2023-04-17 18:50:25.189073 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/real_time_triangulator.unique_with_counts-118.py310.nbi
+-rw-r--r--   0        0        0     4903 2023-04-16 14:08:57.603539 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/stereo_points_builder.cpython-310.pyc
+-rw-r--r--   0        0        0     4910 2023-04-13 17:33:55.950369 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/stereo_points_builder.cpython-38.pyc
+-rw-r--r--   0        0        0     5522 2023-06-08 19:16:30.042145 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.cpython-310.pyc
+-rw-r--r--   0        0        0   277993 2023-06-10 20:35:53.847895 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.1.nbc
+-rw-r--r--   0        0        0   278337 2023-06-10 20:36:00.364127 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.2.nbc
+-rw-r--r--   0        0        0   275198 2023-06-10 20:36:15.587107 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.3.nbc
+-rw-r--r--   0        0        0     3826 2023-06-10 20:36:15.585108 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.nbi
+-rw-r--r--   0        0        0   274936 2023-05-07 17:31:11.859065 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-170.py310.1.nbc
+-rw-r--r--   0        0        0     1819 2023-05-07 17:31:11.856057 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-170.py310.nbi
+-rw-r--r--   0        0        0   280483 2023-05-11 20:37:44.633248 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-186.py310.1.nbc
+-rw-r--r--   0        0        0     1855 2023-05-11 20:37:44.630243 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-186.py310.nbi
+-rw-r--r--   0        0        0   277957 2023-05-11 19:51:33.032983 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.1.nbc
+-rw-r--r--   0        0        0   278013 2023-05-11 17:55:35.449169 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.2.nbc
+-rw-r--r--   0        0        0   278357 2023-05-11 17:56:15.957610 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.3.nbc
+-rw-r--r--   0        0        0     1855 2023-05-11 19:51:33.028983 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.nbi
+-rw-r--r--   0        0        0   277977 2023-05-11 20:58:46.910959 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.1.nbc
+-rw-r--r--   0        0        0   274956 2023-05-11 22:29:46.557422 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.2.nbc
+-rw-r--r--   0        0        0   280725 2023-05-12 22:34:01.184507 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.3.nbc
+-rw-r--r--   0        0        0     3913 2023-05-12 22:34:01.181521 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.nbi
+-rw-r--r--   0        0        0   274956 2023-05-13 12:36:45.045739 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.1.nbc
+-rw-r--r--   0        0        0   277993 2023-05-14 17:03:11.852980 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.2.nbc
+-rw-r--r--   0        0        0   278337 2023-05-14 17:03:18.755882 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.3.nbc
+-rw-r--r--   0        0        0     3855 2023-05-14 17:03:18.752878 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.nbi
+-rw-r--r--   0        0        0   278215 2023-05-12 22:36:41.576195 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-195.py310.1.nbc
+-rw-r--r--   0        0        0     1797 2023-05-12 22:36:41.573185 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-195.py310.nbi
+-rw-r--r--   0        0        0    80914 2023-06-10 20:35:46.176596 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-152.py310.1.nbc
+-rw-r--r--   0        0        0    77589 2023-06-10 20:36:11.729164 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-152.py310.2.nbc
+-rw-r--r--   0        0        0     2292 2023-06-10 20:36:11.727174 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-152.py310.nbi
+-rw-r--r--   0        0        0    77589 2023-05-10 14:04:48.307277 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-153.py310.1.nbc
+-rw-r--r--   0        0        0    80894 2023-05-09 20:10:40.338051 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-153.py310.2.nbc
+-rw-r--r--   0        0        0     1280 2023-05-10 14:04:48.305276 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-153.py310.nbi
+-rw-r--r--   0        0        0    80894 2023-05-11 20:37:03.860602 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-170.py310.1.nbc
+-rw-r--r--   0        0        0     1280 2023-05-11 20:37:03.857602 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-170.py310.nbi
+-rw-r--r--   0        0        0    80894 2023-05-11 19:51:22.690984 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-172.py310.1.nbc
+-rw-r--r--   0        0        0    80894 2023-05-11 17:55:29.550170 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-172.py310.2.nbc
+-rw-r--r--   0        0        0     1280 2023-05-11 19:51:22.687981 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-172.py310.nbi
+-rw-r--r--   0        0        0    80894 2023-05-11 20:58:36.790966 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-173.py310.1.nbc
+-rw-r--r--   0        0        0    77589 2023-05-11 22:29:37.429700 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-173.py310.2.nbc
+-rw-r--r--   0        0        0     2321 2023-05-11 22:29:37.426700 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-173.py310.nbi
+-rw-r--r--   0        0        0    77589 2023-05-13 12:36:36.027208 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-178.py310.1.nbc
+-rw-r--r--   0        0        0    80894 2023-05-14 17:03:04.107988 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-178.py310.2.nbc
+-rw-r--r--   0        0        0     2292 2023-05-14 17:03:04.102988 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-178.py310.nbi
+-rw-r--r--   0        0        0    80894 2023-05-12 22:36:32.819436 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-179.py310.1.nbc
+-rw-r--r--   0        0        0     1280 2023-05-12 22:36:32.816430 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-179.py310.nbi
+-rw-r--r--   0        0        0     5598 2023-04-04 19:53:34.784759 pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/triangulator.cpython-38.pyc
+-rw-r--r--   0        0        0     8778 2023-04-16 12:58:12.413689 pyxy3d-0.1.3/pyxy3d/triangulate/array_stereo_triangulator.py
+-rw-r--r--   0        0        0     5762 2023-04-16 12:58:12.416688 pyxy3d-0.1.3/pyxy3d/triangulate/stereo_points_builder.py
+-rw-r--r--   0        0        0     7616 2023-06-08 19:15:56.173904 pyxy3d-0.1.3/pyxy3d/triangulate/sync_packet_triangulator.py
+-rw-r--r--   0        0        0     6742 2023-06-22 12:20:08.052238 pyxy3d-0.1.3/README.md
+-rw-r--r--   0        0        0     7560 1970-01-01 00:00:00.000000 pyxy3d-0.1.3/PKG-INFO
```

### Comparing `pyxy3d-0.1.2/LICENSE.md` & `pyxy3d-0.1.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyproject.toml` & `pyxy3d-0.1.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyxy3d"
-version = "0.1.2"
+version = "0.1.3"
 description = "A package for calibrating standard webcams to enable 3d motion tracking"
 authors = ["Mac Prible <prible@gmail.com>"]
 license = "AGPL-3.0-only"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10, <3.12"
@@ -12,15 +12,15 @@
 PyQt6 = "^6.4.0"
 pandas = "^1.5.0"
 scipy = "^1.10.1"
 pyqtgraph = "^0.13.2"
 PyOpenGL = "^3.1.6"
 toml = "^0.10.2"
 numba = "^0.56.4"
-mediapipe = "0.10.0"
+mediapipe = "0.10.1"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 pytest = "^7.3.0"
 ipykernel = "^6.22.0"
 pymdown-extensions = ">=9.11,<11.0"
 mkdocs-material = "^9.1.6"
```

### Comparing `pyxy3d-0.1.2/pyxy3d/__init__.py` & `pyxy3d-0.1.3/pyxy3d/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/__main__.py` & `pyxy3d-0.1.3/pyxy3d/__main__.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/calibration/__pycache__/charuco.cpython-310.pyc` & `pyxy3d-0.1.3/pyxy3d/calibration/__pycache__/charuco.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/calibration/__pycache__/charuco.cpython-38.pyc` & `pyxy3d-0.1.3/pyxy3d/calibration/__pycache__/charuco.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/calibration/__pycache__/corner_tracker.cpython-38.pyc` & `pyxy3d-0.1.3/pyxy3d/calibration/__pycache__/corner_tracker.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/calibration/__pycache__/draw_charuco.cpython-310.pyc` & `pyxy3d-0.1.3/pyxy3d/calibration/__pycache__/draw_charuco.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/calibration/__pycache__/draw_charuco.cpython-38.pyc` & `pyxy3d-0.1.3/pyxy3d/calibration/__pycache__/draw_charuco.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/calibration/__pycache__/monocalibrator.cpython-310.pyc` & `pyxy3d-0.1.3/pyxy3d/calibration/__pycache__/monocalibrator.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/calibration/__pycache__/monocalibrator.cpython-38.pyc` & `pyxy3d-0.1.3/pyxy3d/calibration/__pycache__/monocalibrator.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/calibration/__pycache__/omnicalibrator.cpython-38.pyc` & `pyxy3d-0.1.3/pyxy3d/calibration/__pycache__/omnicalibrator.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/calibration/__pycache__/stereocalibrator.cpython-310.pyc` & `pyxy3d-0.1.3/pyxy3d/calibration/__pycache__/stereocalibrator.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/calibration/__pycache__/stereocalibrator.cpython-38.pyc` & `pyxy3d-0.1.3/pyxy3d/calibration/__pycache__/stereocalibrator.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/calibration/capture_volume/__pycache__/capture_volume.cpython-310.pyc` & `pyxy3d-0.1.3/pyxy3d/calibration/capture_volume/__pycache__/capture_volume.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/calibration/capture_volume/__pycache__/capture_volume.cpython-38.pyc` & `pyxy3d-0.1.3/pyxy3d/calibration/capture_volume/__pycache__/capture_volume.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/calibration/capture_volume/__pycache__/point_estimates.cpython-310.pyc` & `pyxy3d-0.1.3/pyxy3d/calibration/capture_volume/__pycache__/point_estimates.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/calibration/capture_volume/__pycache__/point_estimates.cpython-38.pyc` & `pyxy3d-0.1.3/pyxy3d/calibration/capture_volume/__pycache__/point_estimates.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/calibration/capture_volume/__pycache__/quality_controller.cpython-310.pyc` & `pyxy3d-0.1.3/pyxy3d/calibration/capture_volume/__pycache__/quality_controller.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/calibration/capture_volume/__pycache__/quality_controller.cpython-38.pyc` & `pyxy3d-0.1.3/pyxy3d/calibration/capture_volume/__pycache__/quality_controller.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/calibration/capture_volume/__pycache__/set_origin_functions.cpython-310.pyc` & `pyxy3d-0.1.3/pyxy3d/calibration/capture_volume/__pycache__/set_origin_functions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/calibration/capture_volume/__pycache__/set_origin_functions.cpython-38.pyc` & `pyxy3d-0.1.3/pyxy3d/calibration/capture_volume/__pycache__/set_origin_functions.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/calibration/capture_volume/capture_volume.py` & `pyxy3d-0.1.3/pyxy3d/calibration/capture_volume/capture_volume.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/calibration/capture_volume/capture_volume_stage_1.pkl` & `pyxy3d-0.1.3/pyxy3d/calibration/capture_volume/capture_volume_stage_1.pkl`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_point_estimates.cpython-310.pyc` & `pyxy3d-0.1.3/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_point_estimates.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_point_estimates.cpython-38.pyc` & `pyxy3d-0.1.3/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_point_estimates.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_stereotriangulated_table.cpython-310.pyc` & `pyxy3d-0.1.3/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_stereotriangulated_table.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_stereotriangulated_table.cpython-38.pyc` & `pyxy3d-0.1.3/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_stereotriangulated_table.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/calibration/capture_volume/helper_functions/get_point_estimates.py` & `pyxy3d-0.1.3/pyxy3d/calibration/capture_volume/helper_functions/get_point_estimates.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/calibration/capture_volume/helper_functions/get_stereotriangulated_table.py` & `pyxy3d-0.1.3/pyxy3d/calibration/capture_volume/helper_functions/get_stereotriangulated_table.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/calibration/capture_volume/point_estimates.py` & `pyxy3d-0.1.3/pyxy3d/calibration/capture_volume/point_estimates.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/calibration/capture_volume/quality_controller.py` & `pyxy3d-0.1.3/pyxy3d/calibration/capture_volume/quality_controller.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/calibration/capture_volume/seaborn_summaries.py` & `pyxy3d-0.1.3/pyxy3d/calibration/capture_volume/seaborn_summaries.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/calibration/capture_volume/set_origin_functions.py` & `pyxy3d-0.1.3/pyxy3d/calibration/capture_volume/set_origin_functions.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/calibration/charuco.py` & `pyxy3d-0.1.3/pyxy3d/calibration/charuco.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/calibration/draw_charuco.py` & `pyxy3d-0.1.3/pyxy3d/calibration/draw_charuco.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/calibration/monocalibrator.py` & `pyxy3d-0.1.3/pyxy3d/calibration/monocalibrator.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/calibration/stereocalibrator.py` & `pyxy3d-0.1.3/pyxy3d/calibration/stereocalibrator.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/cameras/__pycache__/camera.cpython-310.pyc` & `pyxy3d-0.1.3/pyxy3d/cameras/__pycache__/camera.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/cameras/__pycache__/camera.cpython-38.pyc` & `pyxy3d-0.1.3/pyxy3d/cameras/__pycache__/camera.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/cameras/__pycache__/camera_array.cpython-310.pyc` & `pyxy3d-0.1.3/pyxy3d/cameras/__pycache__/camera_array.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/cameras/__pycache__/camera_array.cpython-38.pyc` & `pyxy3d-0.1.3/pyxy3d/cameras/__pycache__/camera_array.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/cameras/__pycache__/camera_array_initializer.cpython-310.pyc` & `pyxy3d-0.1.3/pyxy3d/cameras/__pycache__/camera_array_initializer.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/cameras/__pycache__/camera_array_initializer.cpython-38.pyc` & `pyxy3d-0.1.3/pyxy3d/cameras/__pycache__/camera_array_initializer.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/cameras/__pycache__/data_packets.cpython-310.pyc` & `pyxy3d-0.1.3/pyxy3d/cameras/__pycache__/data_packets.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/cameras/__pycache__/data_packets.cpython-38.pyc` & `pyxy3d-0.1.3/pyxy3d/cameras/__pycache__/data_packets.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/cameras/__pycache__/live_stream.cpython-310.pyc` & `pyxy3d-0.1.3/pyxy3d/cameras/__pycache__/live_stream.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/cameras/__pycache__/live_stream.cpython-38.pyc` & `pyxy3d-0.1.3/pyxy3d/cameras/__pycache__/live_stream.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/cameras/__pycache__/synchronizer.cpython-310.pyc` & `pyxy3d-0.1.3/pyxy3d/cameras/__pycache__/synchronizer.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/cameras/__pycache__/synchronizer.cpython-38.pyc` & `pyxy3d-0.1.3/pyxy3d/cameras/__pycache__/synchronizer.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/cameras/camera.py` & `pyxy3d-0.1.3/pyxy3d/cameras/camera.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/cameras/camera_array.py` & `pyxy3d-0.1.3/pyxy3d/cameras/camera_array.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/cameras/camera_array_initializer.py` & `pyxy3d-0.1.3/pyxy3d/cameras/camera_array_initializer.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/cameras/live_stream.py` & `pyxy3d-0.1.3/pyxy3d/cameras/live_stream.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/cameras/synchronizer.py` & `pyxy3d-0.1.3/pyxy3d/cameras/synchronizer.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/configurator.py` & `pyxy3d-0.1.3/pyxy3d/configurator.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/export.py` & `pyxy3d-0.1.3/pyxy3d/export.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/gui/__pycache__/calibrate_capture_volume_widget.cpython-310.pyc` & `pyxy3d-0.1.3/pyxy3d/gui/__pycache__/calibrate_capture_volume_widget.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/gui/__pycache__/calibration_widget.cpython-310.pyc` & `pyxy3d-0.1.3/pyxy3d/gui/__pycache__/calibration_widget.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/gui/__pycache__/calibration_wizard.cpython-310.pyc` & `pyxy3d-0.1.3/pyxy3d/gui/__pycache__/calibration_wizard.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/gui/__pycache__/charuco_widget.cpython-310.pyc` & `pyxy3d-0.1.3/pyxy3d/gui/__pycache__/charuco_widget.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/gui/__pycache__/extrinsic_calibration_widget.cpython-310.pyc` & `pyxy3d-0.1.3/pyxy3d/gui/__pycache__/extrinsic_calibration_widget.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/gui/__pycache__/log_widget.cpython-310.pyc` & `pyxy3d-0.1.3/pyxy3d/gui/__pycache__/log_widget.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/gui/__pycache__/main.cpython-310.pyc` & `pyxy3d-0.1.3/pyxy3d/gui/__pycache__/main.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/gui/__pycache__/main.cpython-38.pyc` & `pyxy3d-0.1.3/pyxy3d/gui/__pycache__/main.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/gui/__pycache__/main_widget.cpython-310.pyc` & `pyxy3d-0.1.3/pyxy3d/gui/__pycache__/main_widget.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/gui/__pycache__/navigation_bars.cpython-310.pyc` & `pyxy3d-0.1.3/pyxy3d/gui/__pycache__/navigation_bars.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/gui/__pycache__/playback_widget.cpython-310.pyc` & `pyxy3d-0.1.3/pyxy3d/gui/__pycache__/playback_widget.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/gui/__pycache__/post_processing_widget.cpython-310.pyc` & `pyxy3d-0.1.3/pyxy3d/gui/__pycache__/post_processing_widget.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/gui/__pycache__/progress_dialog.cpython-310.pyc` & `pyxy3d-0.1.3/pyxy3d/gui/__pycache__/progress_dialog.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/gui/__pycache__/qt_logger.cpython-310.pyc` & `pyxy3d-0.1.3/pyxy3d/gui/__pycache__/qt_logger.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/gui/__pycache__/qt_logger.cpython-38.pyc` & `pyxy3d-0.1.3/pyxy3d/gui/__pycache__/qt_logger.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/gui/__pycache__/recording_widget.cpython-310.pyc` & `pyxy3d-0.1.3/pyxy3d/gui/__pycache__/recording_widget.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/gui/__pycache__/recording_widget.cpython-38.pyc` & `pyxy3d-0.1.3/pyxy3d/gui/__pycache__/recording_widget.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/gui/__pycache__/widgets.cpython-310.pyc` & `pyxy3d-0.1.3/pyxy3d/gui/__pycache__/widgets.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/gui/__pycache__/widgets.cpython-38.pyc` & `pyxy3d-0.1.3/pyxy3d/gui/__pycache__/widgets.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/gui/__pycache__/wizard_charuco.cpython-310.pyc` & `pyxy3d-0.1.3/pyxy3d/gui/__pycache__/wizard_charuco.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/gui/__pycache__/wizard_charuco.cpython-38.pyc` & `pyxy3d-0.1.3/pyxy3d/gui/__pycache__/wizard_charuco.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/gui/__pycache__/wizard_directory.cpython-310.pyc` & `pyxy3d-0.1.3/pyxy3d/gui/__pycache__/wizard_directory.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/gui/__pycache__/wizard_directory.cpython-38.pyc` & `pyxy3d-0.1.3/pyxy3d/gui/__pycache__/wizard_directory.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/gui/calibrate_capture_volume_widget.py` & `pyxy3d-0.1.3/pyxy3d/gui/calibrate_capture_volume_widget.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/gui/calibration_widget.py` & `pyxy3d-0.1.3/pyxy3d/gui/calibration_widget.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/gui/camera_config/__pycache__/camera_config_dialogue.cpython-310.pyc` & `pyxy3d-0.1.3/pyxy3d/gui/camera_config/__pycache__/camera_config_dialogue.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/gui/camera_config/__pycache__/camera_config_dialogue.cpython-38.pyc` & `pyxy3d-0.1.3/pyxy3d/gui/camera_config/__pycache__/camera_config_dialogue.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/gui/camera_config/__pycache__/camera_summary_widget.cpython-310.pyc` & `pyxy3d-0.1.3/pyxy3d/gui/camera_config/__pycache__/camera_summary_widget.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/gui/camera_config/__pycache__/camera_tabs.cpython-310.pyc` & `pyxy3d-0.1.3/pyxy3d/gui/camera_config/__pycache__/camera_tabs.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/gui/camera_config/__pycache__/camera_tabs.cpython-38.pyc` & `pyxy3d-0.1.3/pyxy3d/gui/camera_config/__pycache__/camera_tabs.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/gui/camera_config/__pycache__/frame_emitter.cpython-310.pyc` & `pyxy3d-0.1.3/pyxy3d/gui/camera_config/__pycache__/frame_emitter.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/gui/camera_config/__pycache__/frame_emitter.cpython-38.pyc` & `pyxy3d-0.1.3/pyxy3d/gui/camera_config/__pycache__/frame_emitter.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/gui/camera_config/__pycache__/intrinsic_calibration_widget.cpython-310.pyc` & `pyxy3d-0.1.3/pyxy3d/gui/camera_config/__pycache__/intrinsic_calibration_widget.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/gui/camera_config/camera_config_dialogue.py` & `pyxy3d-0.1.3/pyxy3d/gui/camera_config/camera_config_dialogue.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/gui/camera_config/camera_summary_widget.py` & `pyxy3d-0.1.3/pyxy3d/gui/camera_config/camera_summary_widget.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/gui/camera_config/frame_emitter.py` & `pyxy3d-0.1.3/pyxy3d/gui/camera_config/frame_emitter.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/gui/camera_config/intrinsic_calibration_widget.py` & `pyxy3d-0.1.3/pyxy3d/gui/camera_config/intrinsic_calibration_widget.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/gui/charuco_widget.py` & `pyxy3d-0.1.3/pyxy3d/gui/charuco_widget.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/gui/extrinsic_calibration_widget.py` & `pyxy3d-0.1.3/pyxy3d/gui/extrinsic_calibration_widget.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/gui/frame_builders/__pycache__/extrinsic_calibration_widget.cpython-310.pyc` & `pyxy3d-0.1.3/pyxy3d/gui/frame_builders/__pycache__/extrinsic_calibration_widget.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/gui/frame_builders/__pycache__/omni_frame_builder.cpython-38.pyc` & `pyxy3d-0.1.3/pyxy3d/gui/frame_builders/__pycache__/omni_frame_builder.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/gui/frame_builders/__pycache__/omni_frame_widget.cpython-38.pyc` & `pyxy3d-0.1.3/pyxy3d/gui/frame_builders/__pycache__/omni_frame_widget.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/gui/frame_builders/__pycache__/paired_frame_builder.cpython-310.pyc` & `pyxy3d-0.1.3/pyxy3d/gui/frame_builders/__pycache__/paired_frame_builder.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_builder.cpython-310.pyc` & `pyxy3d-0.1.3/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_builder.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_builder.cpython-38.pyc` & `pyxy3d-0.1.3/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_builder.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_widget.cpython-310.pyc` & `pyxy3d-0.1.3/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_widget.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_widget.cpython-38.pyc` & `pyxy3d-0.1.3/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_widget.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/gui/frame_builders/paired_frame_builder.py` & `pyxy3d-0.1.3/pyxy3d/gui/frame_builders/paired_frame_builder.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/gui/icons/pyxy_logo.svg` & `pyxy3d-0.1.3/pyxy3d/gui/icons/pyxy_logo.svg`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/gui/icons/rotate-camera-left.svg` & `pyxy3d-0.1.3/pyxy3d/gui/icons/rotate-camera-left.svg`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/gui/icons/rotate-camera-right.svg` & `pyxy3d-0.1.3/pyxy3d/gui/icons/rotate-camera-right.svg`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/gui/log_widget.py` & `pyxy3d-0.1.3/pyxy3d/gui/log_widget.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/gui/main_widget.py` & `pyxy3d-0.1.3/pyxy3d/gui/main_widget.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/gui/navigation_bars.py` & `pyxy3d-0.1.3/pyxy3d/gui/navigation_bars.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/gui/playback_widget.py` & `pyxy3d-0.1.3/pyxy3d/gui/playback_widget.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/gui/post_processing_widget.py` & `pyxy3d-0.1.3/pyxy3d/gui/post_processing_widget.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/gui/progress_dialog.py` & `pyxy3d-0.1.3/pyxy3d/gui/progress_dialog.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/gui/recording_widget.py` & `pyxy3d-0.1.3/pyxy3d/gui/recording_widget.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/gui/vizualize/__pycache__/camera_mesh.cpython-310.pyc` & `pyxy3d-0.1.3/pyxy3d/gui/vizualize/__pycache__/camera_mesh.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/gui/vizualize/__pycache__/camera_mesh.cpython-38.pyc` & `pyxy3d-0.1.3/pyxy3d/gui/vizualize/__pycache__/camera_mesh.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/gui/vizualize/__pycache__/capture_volume_dialog.cpython-38.pyc` & `pyxy3d-0.1.3/pyxy3d/gui/vizualize/__pycache__/capture_volume_dialog.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/gui/vizualize/__pycache__/capture_volume_visualizer.cpython-38.pyc` & `pyxy3d-0.1.3/pyxy3d/gui/vizualize/__pycache__/capture_volume_visualizer.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/gui/vizualize/__pycache__/capture_volume_widget.cpython-38.pyc` & `pyxy3d-0.1.3/pyxy3d/gui/vizualize/__pycache__/capture_volume_widget.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/gui/vizualize/__pycache__/playback_triangulation_widget.cpython-310.pyc` & `pyxy3d-0.1.3/pyxy3d/gui/vizualize/__pycache__/playback_triangulation_widget.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/gui/vizualize/__pycache__/realtime_triangulation_widget.cpython-310.pyc` & `pyxy3d-0.1.3/pyxy3d/gui/vizualize/__pycache__/realtime_triangulation_widget.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_visualizer.cpython-310.pyc` & `pyxy3d-0.1.3/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_visualizer.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_visualizer.cpython-38.pyc` & `pyxy3d-0.1.3/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_visualizer.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_widget.cpython-310.pyc` & `pyxy3d-0.1.3/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_widget.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_widget.cpython-38.pyc` & `pyxy3d-0.1.3/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_widget.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/gui/vizualize/calibration/capture_volume_visualizer.py` & `pyxy3d-0.1.3/pyxy3d/gui/vizualize/calibration/capture_volume_visualizer.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/gui/vizualize/calibration/capture_volume_widget.py` & `pyxy3d-0.1.3/pyxy3d/gui/vizualize/calibration/capture_volume_widget.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/gui/vizualize/camera_mesh.py` & `pyxy3d-0.1.3/pyxy3d/gui/vizualize/camera_mesh.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/gui/vizualize/playback_triangulation_widget.py` & `pyxy3d-0.1.3/pyxy3d/gui/vizualize/playback_triangulation_widget.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/gui/vizualize/realtime_triangulation_widget.py` & `pyxy3d-0.1.3/pyxy3d/gui/vizualize/realtime_triangulation_widget.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/helper.py` & `pyxy3d-0.1.3/pyxy3d/helper.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/interface.py` & `pyxy3d-0.1.3/pyxy3d/interface.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/logger.py` & `pyxy3d-0.1.3/pyxy3d/logger.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/post_processor.py` & `pyxy3d-0.1.3/pyxy3d/post_processor.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/recording/__pycache__/recorded_stream.cpython-310.pyc` & `pyxy3d-0.1.3/pyxy3d/recording/__pycache__/recorded_stream.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/recording/__pycache__/recorded_stream.cpython-38.pyc` & `pyxy3d-0.1.3/pyxy3d/recording/__pycache__/recorded_stream.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/recording/__pycache__/video_recorder.cpython-310.pyc` & `pyxy3d-0.1.3/pyxy3d/recording/__pycache__/video_recorder.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/recording/__pycache__/video_recorder.cpython-38.pyc` & `pyxy3d-0.1.3/pyxy3d/recording/__pycache__/video_recorder.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/recording/recorded_stream.py` & `pyxy3d-0.1.3/pyxy3d/recording/recorded_stream.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/recording/video_recorder.py` & `pyxy3d-0.1.3/pyxy3d/recording/video_recorder.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/session/__pycache__/get_stage.cpython-310.pyc` & `pyxy3d-0.1.3/pyxy3d/session/__pycache__/get_stage.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/session/__pycache__/session.cpython-310.pyc` & `pyxy3d-0.1.3/pyxy3d/session/__pycache__/session.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/session/session.py` & `pyxy3d-0.1.3/pyxy3d/session/session.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/trackers/__pycache__/charuco_tracker.cpython-310.pyc` & `pyxy3d-0.1.3/pyxy3d/trackers/__pycache__/charuco_tracker.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/trackers/__pycache__/hand_tracker.cpython-310.pyc` & `pyxy3d-0.1.3/pyxy3d/trackers/__pycache__/hand_tracker.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/trackers/__pycache__/helper.cpython-310.pyc` & `pyxy3d-0.1.3/pyxy3d/trackers/__pycache__/helper.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/trackers/__pycache__/holistic_opensim_tracker.cpython-310.pyc` & `pyxy3d-0.1.3/pyxy3d/trackers/__pycache__/holistic_opensim_tracker.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/trackers/__pycache__/holistic_tracker.cpython-310.pyc` & `pyxy3d-0.1.3/pyxy3d/trackers/__pycache__/holistic_tracker.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/trackers/__pycache__/pose_tracker.cpython-310.pyc` & `pyxy3d-0.1.3/pyxy3d/trackers/__pycache__/pose_tracker.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/trackers/__pycache__/threaded_hand_tracker.cpython-310.pyc` & `pyxy3d-0.1.3/pyxy3d/trackers/__pycache__/threaded_hand_tracker.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/trackers/__pycache__/tracker_enum.cpython-310.pyc` & `pyxy3d-0.1.3/pyxy3d/trackers/__pycache__/tracker_enum.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/trackers/charuco_tracker.py` & `pyxy3d-0.1.3/pyxy3d/trackers/charuco_tracker.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/trackers/hand_tracker.py` & `pyxy3d-0.1.3/pyxy3d/trackers/hand_tracker.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/trackers/helper.py` & `pyxy3d-0.1.3/pyxy3d/trackers/helper.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/trackers/holistic_opensim_tracker.py` & `pyxy3d-0.1.3/pyxy3d/trackers/holistic_opensim_tracker.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/trackers/holistic_tracker.py` & `pyxy3d-0.1.3/pyxy3d/trackers/holistic_tracker.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/trackers/pose_tracker.py` & `pyxy3d-0.1.3/pyxy3d/trackers/pose_tracker.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/trackers/tracker_enum.py` & `pyxy3d-0.1.3/pyxy3d/trackers/tracker_enum.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/array_stereo_triangulator.cpython-310.pyc` & `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/array_stereo_triangulator.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/array_stereo_triangulator.cpython-38.pyc` & `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/array_stereo_triangulator.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/helper.cpython-310.pyc` & `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/helper.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/real_time_triangulator.cpython-310.pyc` & `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/real_time_triangulator.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/real_time_triangulator.cpython-38.pyc` & `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/real_time_triangulator.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-135.py310.1.nbc` & `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-135.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-135.py310.2.nbc` & `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-135.py310.2.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-135.py310.nbi` & `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-135.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py310.1.nbc` & `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py310.nbi` & `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py38.1.nbc` & `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py38.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py38.nbi` & `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py38.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-138.py310.1.nbc` & `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-138.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-138.py310.nbi` & `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-138.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-139.py310.1.nbc` & `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-139.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-139.py310.nbi` & `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-139.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-86.py38.1.nbc` & `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-86.py38.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-86.py38.nbi` & `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-86.py38.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-88.py38.1.nbc` & `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-88.py38.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-88.py38.nbi` & `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-88.py38.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/real_time_triangulator.unique_with_counts-118.py310.1.nbc` & `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/real_time_triangulator.unique_with_counts-118.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/real_time_triangulator.unique_with_counts-118.py310.nbi` & `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/real_time_triangulator.unique_with_counts-118.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/stereo_points_builder.cpython-310.pyc` & `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/stereo_points_builder.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/stereo_points_builder.cpython-38.pyc` & `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/stereo_points_builder.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.cpython-310.pyc` & `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.1.nbc` & `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.2.nbc` & `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.2.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.3.nbc` & `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.3.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.nbi` & `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-170.py310.1.nbc` & `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-170.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-170.py310.nbi` & `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-170.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-186.py310.1.nbc` & `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-186.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-186.py310.nbi` & `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-186.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.1.nbc` & `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.2.nbc` & `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.2.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.3.nbc` & `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.3.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.nbi` & `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.1.nbc` & `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.2.nbc` & `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.2.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.3.nbc` & `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.3.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.nbi` & `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.1.nbc` & `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.2.nbc` & `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.2.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.3.nbc` & `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.3.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.nbi` & `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-195.py310.1.nbc` & `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-195.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-195.py310.nbi` & `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-195.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-152.py310.1.nbc` & `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-152.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-152.py310.2.nbc` & `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-152.py310.2.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-152.py310.nbi` & `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-152.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-153.py310.1.nbc` & `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-153.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-153.py310.2.nbc` & `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-153.py310.2.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-153.py310.nbi` & `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-153.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-170.py310.1.nbc` & `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-170.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-170.py310.nbi` & `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-170.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-172.py310.1.nbc` & `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-172.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-172.py310.2.nbc` & `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-172.py310.2.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-172.py310.nbi` & `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-172.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-173.py310.1.nbc` & `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-173.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-173.py310.2.nbc` & `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-173.py310.2.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-173.py310.nbi` & `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-173.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-178.py310.1.nbc` & `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-178.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-178.py310.2.nbc` & `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-178.py310.2.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-178.py310.nbi` & `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-178.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-179.py310.1.nbc` & `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-179.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-179.py310.nbi` & `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-179.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/triangulate/__pycache__/triangulator.cpython-38.pyc` & `pyxy3d-0.1.3/pyxy3d/triangulate/__pycache__/triangulator.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/triangulate/array_stereo_triangulator.py` & `pyxy3d-0.1.3/pyxy3d/triangulate/array_stereo_triangulator.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/triangulate/stereo_points_builder.py` & `pyxy3d-0.1.3/pyxy3d/triangulate/stereo_points_builder.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/pyxy3d/triangulate/sync_packet_triangulator.py` & `pyxy3d-0.1.3/pyxy3d/triangulate/sync_packet_triangulator.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/README.md` & `pyxy3d-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.2/PKG-INFO` & `pyxy3d-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: pyxy3d
-Version: 0.1.2
+Version: 0.1.3
 Summary: A package for calibrating standard webcams to enable 3d motion tracking
 License: AGPL-3.0-only
 Author: Mac Prible
 Author-email: prible@gmail.com
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyOpenGL (>=3.1.6,<4.0.0)
 Requires-Dist: PyQt6 (>=6.4.0,<7.0.0)
-Requires-Dist: mediapipe (==0.10.0)
+Requires-Dist: mediapipe (==0.10.1)
 Requires-Dist: numba (>=0.56.4,<0.57.0)
 Requires-Dist: opencv-contrib-python (>=4.7,<5.0)
 Requires-Dist: pandas (>=1.5.0,<2.0.0)
 Requires-Dist: pyqtgraph (>=0.13.2,<0.14.0)
 Requires-Dist: scipy (>=1.10.1,<2.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Project-URL: repository, https://github.com/mprib/pyxy3d
```

