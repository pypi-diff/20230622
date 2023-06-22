# Comparing `tmp/pin-pink-0.9.0.tar.gz` & `tmp/pin-pink-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pin-pink-0.9.0.tar", last modified: Wed Mar 15 15:18:41 2023, max compression
+gzip compressed data, was "pin-pink-1.0.0.tar", last modified: Thu Jun 22 12:28:57 2023, max compression
```

## Comparing `pin-pink-0.9.0.tar` & `pin-pink-1.0.0.tar`

### file list

```diff
@@ -1,66 +1,74 @@
--rw-r--r--   0        0        0     2651 2023-01-16 16:18:53.687730 pin-pink-0.9.0/.github/workflows/main.yml
--rw-r--r--   0        0        0       77 2022-03-29 17:10:57.272648 pin-pink-0.9.0/.gitignore
--rw-r--r--   0        0        0     4202 2023-03-15 15:17:39.664479 pin-pink-0.9.0/CHANGELOG.md
--rw-r--r--   0        0        0     2179 2023-02-28 10:12:07.208660 pin-pink-0.9.0/CONTRIBUTING.md
--rw-r--r--   0        0        0    11357 2022-03-17 19:43:10.215116 pin-pink-0.9.0/LICENSE
--rw-r--r--   0        0        0     7614 2023-02-20 10:04:19.588236 pin-pink-0.9.0/README.md
--rw-r--r--   0        0        0     1174 2023-02-28 10:12:07.212659 pin-pink-0.9.0/doc/Makefile
--rw-r--r--   0        0        0     9828 2023-02-28 10:53:36.903715 pin-pink-0.9.0/doc/src/conf.py
--rw-r--r--   0        0        0      968 2022-03-04 11:43:18.830659 pin-pink-0.9.0/doc/src/css/custom.css
--rw-r--r--   0        0        0      459 2023-01-18 10:53:20.570424 pin-pink-0.9.0/doc/src/developer-notes.rst
--rw-r--r--   0        0        0    16030 2022-06-09 08:51:10.698591 pin-pink-0.9.0/doc/src/images/apple-touch-icon-180x180.png
--rw-r--r--   0        0        0     1013 2022-06-09 08:51:10.698591 pin-pink-0.9.0/doc/src/images/favicon-16x16.png
--rw-r--r--   0        0        0     1766 2022-06-09 08:51:10.698591 pin-pink-0.9.0/doc/src/images/favicon-32x32.png
--rw-r--r--   0        0        0    18638 2022-06-09 08:51:10.698591 pin-pink-0.9.0/doc/src/images/pink-round-corners-140x140.png
--rw-r--r--   0        0        0     1074 2023-02-28 10:12:07.212659 pin-pink-0.9.0/doc/src/index.rst
--rw-r--r--   0        0        0      685 2023-01-30 15:14:07.609694 pin-pink-0.9.0/doc/src/installation.rst
--rw-r--r--   0        0        0     1930 2023-01-16 16:18:53.687730 pin-pink-0.9.0/doc/src/introduction.rst
--rw-r--r--   0        0        0      844 2023-02-13 15:06:54.714801 pin-pink-0.9.0/doc/src/inverse-kinematics.rst
--rw-r--r--   0        0        0      189 2023-02-28 10:12:07.212659 pin-pink-0.9.0/doc/src/joint-limits.rst
--rw-r--r--   0        0        0      631 2023-02-22 16:16:17.624447 pin-pink-0.9.0/doc/src/references.rst
--rw-r--r--   0        0        0      546 2023-03-15 15:13:51.505077 pin-pink-0.9.0/doc/src/tasks.rst
--rw-r--r--   0        0        0     3194 2023-02-13 15:06:54.714801 pin-pink-0.9.0/examples/arm_kinova_gen2.py
--rw-r--r--   0        0        0     3236 2023-02-13 15:06:54.714801 pin-pink-0.9.0/examples/arm_ur3.py
--rw-r--r--   0        0        0     3053 2023-02-13 15:06:54.714801 pin-pink-0.9.0/examples/double_pendulum.py
--rw-r--r--   0        0        0     5285 2023-03-15 15:13:51.505077 pin-pink-0.9.0/examples/humanoid_draco3.py
--rw-r--r--   0        0        0     4516 2023-02-13 15:06:54.714801 pin-pink-0.9.0/examples/humanoid_jvrc.py
--rw-r--r--   0        0        0     3982 2023-02-13 15:06:54.714801 pin-pink-0.9.0/examples/humanoid_sigmaban.py
--rw-r--r--   0        0        0     1303 2023-01-30 15:14:07.609694 pin-pink-0.9.0/examples/load_custom_urdf.py
--rw-r--r--   0        0        0     3322 2023-01-30 15:14:07.609694 pin-pink-0.9.0/examples/meshcat_shapes.py
--rw-r--r--   0        0        0     3041 2023-02-13 15:06:54.714801 pin-pink-0.9.0/examples/omnidirectional_wheeled_robot.py
--rw-r--r--   0        0        0     4719 2023-01-16 16:18:53.687730 pin-pink-0.9.0/examples/robots/double_pendulum.urdf
--rw-r--r--   0        0        0     2425 2023-02-13 15:05:40.152104 pin-pink-0.9.0/examples/robots/omnidirectional_wheeled_robot.urdf
--rw-r--r--   0        0        0     3932 2023-02-13 15:06:54.714801 pin-pink-0.9.0/examples/visualize_in_meshcat.py
--rw-r--r--   0        0        0     3755 2023-02-13 15:06:54.714801 pin-pink-0.9.0/examples/visualize_in_yourdfpy.py
--rw-r--r--   0        0        0     3875 2023-02-13 15:06:54.714801 pin-pink-0.9.0/examples/wheeled_biped_upkie.py
--rw-r--r--   0        0        0      994 2023-03-15 15:17:32.616621 pin-pink-0.9.0/pink/__init__.py
--rw-r--r--   0        0        0     2644 2023-02-28 10:12:07.212659 pin-pink-0.9.0/pink/bounded_tangent.py
--rw-r--r--   0        0        0     7422 2023-02-28 10:12:07.216659 pin-pink-0.9.0/pink/configuration.py
--rw-r--r--   0        0        0     1971 2023-03-15 14:58:57.683088 pin-pink-0.9.0/pink/exceptions.py
--rw-r--r--   0        0        0     3251 2023-02-28 10:12:07.216659 pin-pink-0.9.0/pink/limits.py
--rw-r--r--   0        0        0     6145 2023-02-28 10:12:07.216659 pin-pink-0.9.0/pink/solve_ik.py
--rw-r--r--   0        0        0     1069 2023-03-15 15:13:51.505077 pin-pink-0.9.0/pink/tasks/__init__.py
--rw-r--r--   0        0        0    10897 2023-02-28 10:53:36.903715 pin-pink-0.9.0/pink/tasks/body_task.py
--rw-r--r--   0        0        0      926 2023-03-15 15:13:51.509077 pin-pink-0.9.0/pink/tasks/exceptions.py
--rw-r--r--   0        0        0     1919 2023-03-15 15:13:51.509077 pin-pink-0.9.0/pink/tasks/joint_coupling_task.py
--rw-r--r--   0        0        0     5955 2023-03-15 15:13:51.509077 pin-pink-0.9.0/pink/tasks/linear_holonomic_task.py
--rw-r--r--   0        0        0     5318 2023-02-20 10:04:19.588236 pin-pink-0.9.0/pink/tasks/posture_task.py
--rw-r--r--   0        0        0     4431 2023-02-20 10:04:19.588236 pin-pink-0.9.0/pink/tasks/task.py
--rw-r--r--   0        0        0     3575 2023-01-30 15:14:07.609694 pin-pink-0.9.0/pink/tasks/utils.py
--rw-r--r--   0        0        0     3629 2023-03-15 15:13:51.509077 pin-pink-0.9.0/pink/utils.py
--rw-r--r--   0        0        0     1128 2023-01-30 15:13:45.733252 pin-pink-0.9.0/pink/visualization.py
--rw-r--r--   0        0        0     1725 2023-01-30 15:14:07.609694 pin-pink-0.9.0/pyproject.toml
--rw-r--r--   0        0        0      705 2023-02-28 10:12:07.220660 pin-pink-0.9.0/tests/__init__.py
--rw-r--r--   0        0        0     8713 2023-02-28 10:12:07.220660 pin-pink-0.9.0/tests/test_body_task.py
--rw-r--r--   0        0        0     2422 2023-02-28 10:12:07.220660 pin-pink-0.9.0/tests/test_bounded_tangent.py
--rw-r--r--   0        0        0    14718 2023-02-28 10:12:07.220660 pin-pink-0.9.0/tests/test_configuration.py
--rw-r--r--   0        0        0     2660 2023-02-28 10:12:07.224660 pin-pink-0.9.0/tests/test_jacobians.py
--rw-r--r--   0        0        0     2997 2023-03-15 15:13:51.509077 pin-pink-0.9.0/tests/test_joint_coupling_task.py
--rw-r--r--   0        0        0     4148 2023-02-28 10:12:07.224660 pin-pink-0.9.0/tests/test_limits.py
--rw-r--r--   0        0        0     4706 2023-03-15 15:13:51.509077 pin-pink-0.9.0/tests/test_linear_holonomic_task.py
--rw-r--r--   0        0        0     4331 2023-02-28 10:12:07.224660 pin-pink-0.9.0/tests/test_posture_task.py
--rw-r--r--   0        0        0    11941 2023-02-28 10:12:07.224660 pin-pink-0.9.0/tests/test_solve_ik.py
--rw-r--r--   0        0        0     1073 2023-02-28 10:12:07.224660 pin-pink-0.9.0/tests/test_task.py
--rw-r--r--   0        0        0     1771 2023-02-28 10:12:07.228659 pin-pink-0.9.0/tests/test_utils.py
--rw-r--r--   0        0        0     1389 2023-03-15 15:13:51.509077 pin-pink-0.9.0/tox.ini
--rw-r--r--   0        0        0     8957 1970-01-01 00:00:00.000000 pin-pink-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     2644 2023-06-07 13:23:17.782466 pin-pink-1.0.0/.github/workflows/main.yml
+-rw-r--r--   0        0        0       77 2022-03-29 17:10:57.272648 pin-pink-1.0.0/.gitignore
+-rw-r--r--   0        0        0     5258 2023-06-22 12:27:44.585977 pin-pink-1.0.0/CHANGELOG.md
+-rw-r--r--   0        0        0     2166 2023-03-30 16:37:52.168295 pin-pink-1.0.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0    11357 2022-03-17 19:43:10.215116 pin-pink-1.0.0/LICENSE
+-rw-r--r--   0        0        0     7607 2023-06-22 07:44:05.245981 pin-pink-1.0.0/README.md
+-rw-r--r--   0        0        0     1079 2023-03-30 16:37:52.168295 pin-pink-1.0.0/doc/Makefile
+-rw-r--r--   0        0        0     9857 2023-06-12 18:00:20.904883 pin-pink-1.0.0/doc/src/conf.py
+-rw-r--r--   0        0        0      968 2022-03-04 11:43:18.830659 pin-pink-1.0.0/doc/src/css/custom.css
+-rw-r--r--   0        0        0      459 2023-01-18 10:53:20.570424 pin-pink-1.0.0/doc/src/developer-notes.rst
+-rw-r--r--   0        0        0    16030 2022-06-09 08:51:10.698591 pin-pink-1.0.0/doc/src/images/apple-touch-icon-180x180.png
+-rw-r--r--   0        0        0     1013 2022-06-09 08:51:10.698591 pin-pink-1.0.0/doc/src/images/favicon-16x16.png
+-rw-r--r--   0        0        0     1766 2022-06-09 08:51:10.698591 pin-pink-1.0.0/doc/src/images/favicon-32x32.png
+-rw-r--r--   0        0        0    18638 2022-06-09 08:51:10.698591 pin-pink-1.0.0/doc/src/images/pink-round-corners-140x140.png
+-rw-r--r--   0        0        0     1056 2023-03-30 16:37:52.168295 pin-pink-1.0.0/doc/src/index.rst
+-rw-r--r--   0        0        0      685 2023-04-28 12:38:34.208866 pin-pink-1.0.0/doc/src/installation.rst
+-rw-r--r--   0        0        0     1930 2023-01-16 16:18:53.687730 pin-pink-1.0.0/doc/src/introduction.rst
+-rw-r--r--   0        0        0      844 2023-02-13 15:06:54.714801 pin-pink-1.0.0/doc/src/inverse-kinematics.rst
+-rw-r--r--   0        0        0      354 2023-03-30 16:37:52.168295 pin-pink-1.0.0/doc/src/limits.rst
+-rw-r--r--   0        0        0      632 2023-04-26 13:53:46.353447 pin-pink-1.0.0/doc/src/references.rst
+-rw-r--r--   0        0        0      547 2023-04-26 13:53:46.353447 pin-pink-1.0.0/doc/src/tasks.rst
+-rw-r--r--   0        0        0     1499 2023-06-22 12:02:36.710584 pin-pink-1.0.0/examples/README.md
+-rw-r--r--   0        0        0     3197 2023-04-26 13:53:46.353447 pin-pink-1.0.0/examples/arm_kinova_gen2.py
+-rw-r--r--   0        0        0     3239 2023-04-26 13:53:46.353447 pin-pink-1.0.0/examples/arm_ur3.py
+-rw-r--r--   0        0        0     3239 2023-06-12 18:00:20.904883 pin-pink-1.0.0/examples/arm_ur5.py
+-rw-r--r--   0        0        0     3056 2023-04-26 13:53:46.353447 pin-pink-1.0.0/examples/double_pendulum.py
+-rw-r--r--   0        0        0     1847 2023-04-26 13:53:46.353447 pin-pink-1.0.0/examples/end_effector_to_target.py
+-rw-r--r--   0        0        0     7426 2023-05-10 18:07:15.716641 pin-pink-1.0.0/examples/flying_dual_arm_ur3.py
+-rw-r--r--   0        0        0     5385 2023-06-22 07:44:05.245981 pin-pink-1.0.0/examples/humanoid_draco3.py
+-rw-r--r--   0        0        0     4526 2023-04-26 13:53:46.353447 pin-pink-1.0.0/examples/humanoid_jvrc.py
+-rw-r--r--   0        0        0     3990 2023-04-26 13:53:46.353447 pin-pink-1.0.0/examples/humanoid_sigmaban.py
+-rw-r--r--   0        0        0     1303 2023-01-30 15:14:07.609694 pin-pink-1.0.0/examples/load_custom_urdf.py
+-rw-r--r--   0        0        0     3327 2023-04-26 13:53:46.353447 pin-pink-1.0.0/examples/meshcat_shapes.py
+-rw-r--r--   0        0        0     3044 2023-04-26 13:53:46.353447 pin-pink-1.0.0/examples/mobile_omni_wheeled_robot.py
+-rw-r--r--   0        0        0     3922 2023-04-26 13:53:46.353447 pin-pink-1.0.0/examples/mobile_stretch.py
+-rw-r--r--   0        0        0     4719 2023-01-16 16:18:53.687730 pin-pink-1.0.0/examples/robots/double_pendulum.urdf
+-rw-r--r--   0        0        0     2425 2023-02-13 15:05:40.152104 pin-pink-1.0.0/examples/robots/omnidirectional_wheeled_robot.urdf
+-rw-r--r--   0        0        0     3938 2023-04-26 13:53:46.353447 pin-pink-1.0.0/examples/visualize_in_meshcat.py
+-rw-r--r--   0        0        0     3762 2023-04-26 13:53:46.353447 pin-pink-1.0.0/examples/visualize_in_yourdfpy.py
+-rw-r--r--   0        0        0     3880 2023-04-26 13:53:46.353447 pin-pink-1.0.0/examples/wheeled_biped_upkie.py
+-rw-r--r--   0        0        0      994 2023-06-22 12:27:56.457780 pin-pink-1.0.0/pink/__init__.py
+-rw-r--r--   0        0        0     7554 2023-04-26 13:53:46.353447 pin-pink-1.0.0/pink/configuration.py
+-rw-r--r--   0        0        0     1971 2023-06-21 12:13:46.184563 pin-pink-1.0.0/pink/exceptions.py
+-rw-r--r--   0        0        0      846 2023-03-30 16:37:52.168295 pin-pink-1.0.0/pink/limits/__init__.py
+-rw-r--r--   0        0        0     4430 2023-06-21 09:13:40.430862 pin-pink-1.0.0/pink/limits/configuration_limit.py
+-rw-r--r--   0        0        0     1599 2023-06-21 09:13:38.138898 pin-pink-1.0.0/pink/limits/limit.py
+-rw-r--r--   0        0        0     3385 2023-06-21 09:13:36.118930 pin-pink-1.0.0/pink/limits/velocity_limit.py
+-rw-r--r--   0        0        0     6369 2023-03-30 16:37:52.168295 pin-pink-1.0.0/pink/solve_ik.py
+-rw-r--r--   0        0        0     1072 2023-04-26 13:54:16.824556 pin-pink-1.0.0/pink/tasks/__init__.py
+-rw-r--r--   0        0        0     1031 2023-06-22 07:44:05.245981 pin-pink-1.0.0/pink/tasks/exceptions.py
+-rw-r--r--   0        0        0     9047 2023-06-22 07:44:05.245981 pin-pink-1.0.0/pink/tasks/frame_task.py
+-rw-r--r--   0        0        0     3128 2023-06-22 07:44:05.245981 pin-pink-1.0.0/pink/tasks/joint_coupling_task.py
+-rw-r--r--   0        0        0     8129 2023-06-22 07:44:05.245981 pin-pink-1.0.0/pink/tasks/linear_holonomic_task.py
+-rw-r--r--   0        0        0     4409 2023-06-22 07:44:05.245981 pin-pink-1.0.0/pink/tasks/posture_task.py
+-rw-r--r--   0        0        0     7215 2023-06-22 07:44:05.245981 pin-pink-1.0.0/pink/tasks/task.py
+-rw-r--r--   0        0        0     3575 2023-06-21 09:13:28.223056 pin-pink-1.0.0/pink/tasks/utils.py
+-rw-r--r--   0        0        0     3477 2023-03-30 16:37:52.168295 pin-pink-1.0.0/pink/utils.py
+-rw-r--r--   0        0        0     1128 2023-01-30 15:13:45.733252 pin-pink-1.0.0/pink/visualization.py
+-rw-r--r--   0        0        0     1680 2023-06-07 13:23:17.786466 pin-pink-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      703 2023-06-21 12:26:39.223950 pin-pink-1.0.0/tests/__init__.py
+-rw-r--r--   0        0        0    14799 2023-06-21 12:26:42.284127 pin-pink-1.0.0/tests/test_configuration.py
+-rw-r--r--   0        0        0     4203 2023-06-21 12:26:40.888046 pin-pink-1.0.0/tests/test_configuration_limit.py
+-rw-r--r--   0        0        0    10351 2023-06-22 07:44:05.245981 pin-pink-1.0.0/tests/test_frame_task.py
+-rw-r--r--   0        0        0     2680 2023-06-21 12:26:45.152290 pin-pink-1.0.0/tests/test_jacobians.py
+-rw-r--r--   0        0        0     2934 2023-06-22 07:44:05.245981 pin-pink-1.0.0/tests/test_joint_coupling_task.py
+-rw-r--r--   0        0        0     3571 2023-06-21 12:26:47.892446 pin-pink-1.0.0/tests/test_limits.py
+-rw-r--r--   0        0        0     5089 2023-06-22 07:44:05.245981 pin-pink-1.0.0/tests/test_linear_holonomic_task.py
+-rw-r--r--   0        0        0     4349 2023-06-22 07:44:05.245981 pin-pink-1.0.0/tests/test_posture_task.py
+-rw-r--r--   0        0        0    11922 2023-06-22 07:44:05.245981 pin-pink-1.0.0/tests/test_solve_ik.py
+-rw-r--r--   0        0        0     1082 2023-06-21 12:27:00.169128 pin-pink-1.0.0/tests/test_task.py
+-rw-r--r--   0        0        0     2276 2023-06-21 12:27:01.609206 pin-pink-1.0.0/tests/test_utils.py
+-rw-r--r--   0        0        0     1872 2023-06-21 12:27:03.069285 pin-pink-1.0.0/tests/test_velocity_limit.py
+-rw-r--r--   0        0        0     1371 2023-06-07 13:23:17.786466 pin-pink-1.0.0/tox.ini
+-rw-r--r--   0        0        0     8900 1970-01-01 00:00:00.000000 pin-pink-1.0.0/PKG-INFO
```

### Comparing `pin-pink-0.9.0/.github/workflows/main.yml` & `pin-pink-1.0.0/.github/workflows/main.yml`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     test:
         name: "Test ${{ matrix.os }} with python-${{ matrix.python-version }}"
         runs-on: ${{ matrix.os }}
 
         strategy:
             matrix:
                 os: [ubuntu-latest, macos-latest]
-                python-version: ["3.7", "3.8", "3.9", "3.10"]
+                python-version: ["3.8", "3.9", "3.10"]
 
         steps:
             - name: "Checkout sources"
               uses: actions/checkout@v3
 
             - name: "Set up Python ${{ matrix.python-version }}"
               uses: actions/setup-python@v4
```

### Comparing `pin-pink-0.9.0/CHANGELOG.md` & `pin-pink-1.0.0/CHANGELOG.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,57 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
+## [1.0.0] 2-23/06/22
+
+### Added
+
+- Example: UR5 arm
+- Example: flying dual-arm with UR3
+- General linear holonomic task (thanks to @ymontmarin)
+
+### Changed
+
+- Cost vector is now defined for all tasks
+- Drop support for Python 3.7
+- Levenberg-Marquardt damping is now defined for all tasks
+- Update joint-coupling task to derive from general linear holonomic task
+
+### Fixed
+
+- Example: Draco 3 numerical stability
+
+## [0.11.0] - 2023/05/01
+
+### Added
+
+- Example: Stretch RE1
+
+### Changed
+
+- Handle all frames, including non-body frames (thanks to @proyan)
+- Rename ``BodyTask`` to ``FrameTask``
+
+## [0.10.0] - 2023/03/30
+
+### Added
+
+- Base class ``Limit`` for configuration and velocity limits
+- In-place integration of a velocity from a configuration
+- Unit tests for configuration limits
+- Unit tests for velocity limits
+
+### Changed
+
+- Add ``pink.limits`` submodule
+- Configuration and velocity limits are now stacked rather than pre-reduced
+- Move configuration limit to ``ConfigurationLimit`` class
+- Move velocity limit to ``VelocityLimit`` class
+
 ## [0.9.0] - 2023/03/15
 
 ### Added
 
 - Example: Draco 3 humanoid by @shbang91
 - Joint-coupling task by @shbang91
 - Linear holonomic task by @shbang91
```

### Comparing `pin-pink-0.9.0/CONTRIBUTING.md` & `pin-pink-1.0.0/CONTRIBUTING.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # 👷 Contributing
 
 This project's goal is to make it easy to do inverse kinematics on all kinds of robot models. All contributions are welcome, for example here are some ways to help:
 
 - Try out the [examples](examples) and report any issue
 - Propose improvements or ask questions about the [documentation](https://tasts-robots.org/doc/pink/)
-- Pick something you want to do with one of the many [robot descriptions](https://github.com/robot-descriptions/awesome-robot-descriptions), and write a new example for it
+- Pick something you want to do with one of the many [robot descriptions](https://github.com/robot-descriptions/robot_descriptions.py) and write a new example
 - Find a use case that is not covered and write a unit test for it
 - Benchmark the performance of the following design choice depending on the number and types of tasks:
     - The current ``Configuration`` interface, which does ``pin.computeJointJacobians`` + ``pin.getFrameJacobian``
     - The alternative using only ``pin.computeFrameJacobian``
 
 There are also a number of tasks from Pymanoid that are not in Pink yet. If you happen to need one of them for your application, check out the reference implementation and add it to Pink:
```

### Comparing `pin-pink-0.9.0/LICENSE` & `pin-pink-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pin-pink-0.9.0/README.md` & `pin-pink-1.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 # Pink
 
 <img src="https://user-images.githubusercontent.com/1189580/172797197-9aa46561-cfaa-4046-bd60-f681d85b055d.png" align="right" height=140>
 
 [![Build](https://img.shields.io/github/actions/workflow/status/tasts-robots/pink/main.yml?branch=master)](https://github.com/tasts-robots/pink/actions)
 [![Coverage](https://coveralls.io/repos/github/tasts-robots/pink/badge.svg?branch=master)](https://coveralls.io/github/tasts-robots/pink?branch=master)
-[![Documentation](https://img.shields.io/badge/docs-online-brightgreen?style=flat)](https://tasts-robots.org/doc/pink/)
+[![Documentation](https://img.shields.io/badge/docs-online-brightgreen?logo=read-the-docs&style=flat)](https://tasts-robots.org/doc/pink/)
 [![PyPI version](https://img.shields.io/pypi/v/pin-pink)](https://pypi.org/project/pin-pink/)
 
 **P**ython **in**verse **k**inematics for articulated robot models, based on [Pinocchio](https://github.com/stack-of-tasks/pinocchio).
 
 ## Installation
 
 ```console
 pip install pin-pink
 ```
 
-On Raspberry Pi, you will need to install [from source](https://tasts-robots.org/doc/pink/installation.html#from-source).
-
 ## Usage
 
 Pink solves differential inverse kinematics by [weighted tasks](https://scaron.info/robot-locomotion/inverse-kinematics.html). A task is defined by a *residual* function $e(q)$ of the robot configuration $q \in \mathcal{C}$ to be driven to zero. For instance, putting a foot position $p_{foot}(q)$ at a given target $p_{foot}^{\star}$ can be described by the position residual:
 
 $$
 e(q) = p_{foot}^{\star} - p_{foot}(q)
 $$
@@ -43,28 +41,28 @@
 Pink provides an API to describe the problem as tasks with targets, and automatically build and solve the underlying quadratic program.
 
 ### Task costs
 
 Here is the example of a biped robot that controls the position and orientation of its base, left and right contact frames. A fourth "posture" task, giving a preferred angle for each joint, is added for regularization:
 
 ```python
-from pink.tasks import BodyTask, PostureTask
+from pink.tasks import FrameTask, PostureTask
 
 tasks = {
-    "base": BodyTask(
+    "base": FrameTask(
         "base",
         position_cost=1.0,              # [cost] / [m]
         orientation_cost=1.0,           # [cost] / [rad]
     ),
-    "left_contact": BodyTask(
+    "left_contact": FrameTask(
         "left_contact",
         position_cost=[0.1, 0.0, 0.1],  # [cost] / [m]
         orientation_cost=0.0,           # [cost] / [rad]
     ),
-    "right_contact": BodyTask(
+    "right_contact": FrameTask(
         "right_contact",
         position_cost=[0.1, 0.0, 0.1],  # [cost] / [m]
         orientation_cost=0.0,           # [cost] / [rad]
     ),
     "posture": PostureTask(
         cost=1e-3,                      # [cost] / [rad]
     ),
@@ -90,16 +88,16 @@
 ```python
 import pink
 from robot_descriptions.loaders.pinocchio import load_robot_description
 
 robot = load_robot_description("upkie_description")
 configuration = pink.Configuration(robot.model, robot.data, robot.q0)
 for body, task in tasks.items():
-    if type(task) is BodyTask:
-        task.set_target(configuration.get_transform_body_to_world(body))
+    if type(task) is FrameTask:
+        task.set_target(configuration.get_transform_frame_to_world(body))
 ```
 
 A task can be added to the inverse kinematics once both its cost and target (if applicable) are defined.
 
 ### Differential inverse kinematics
 
 Pink solves differential inverse kinematics, meaning it outputs a velocity that steers the robot towards achieving all tasks at best. If we keep integrating that velocity, and task targets don't change over time, we will converge to a stationary configuration:
@@ -123,16 +121,16 @@
 * [Visualization in MeshCat](https://github.com/tasts-robots/pink/blob/master/examples/visualize_in_meshcat.py)
 * [Visualization in yourdfpy](https://github.com/tasts-robots/pink/blob/master/examples/visualize_in_yourdfpy.py)
 
 Pink works with all kinds of robot morphologies:
 
 * Arms: [Kinova Gen2](https://github.com/tasts-robots/pink/blob/master/examples/arm_kinova_gen2.py), [UR3](https://github.com/tasts-robots/pink/blob/master/examples/arm_ur3.py)
 * Humanoids: [JVRC-1](https://github.com/tasts-robots/pink/blob/master/examples/humanoid_jvrc.py), [SigmaBan](https://github.com/tasts-robots/pink/blob/master/examples/humanoid_sigmaban.py)
+* Mobile base: [Omnidirectional robot](https://github.com/tasts-robots/pink/blob/master/examples/mobile_omni_wheeled_robot.py), [Stretch R1](https://github.com/tasts-robots/pink/blob/master/examples/mobile_stretch.py)
 * Wheeled biped: [Upkie](https://github.com/tasts-robots/pink/blob/master/examples/wheeled_biped_upkie.py)
-* Wheeled: [Omnidirectional robot](https://github.com/tasts-robots/pink/blob/master/examples/omnidirectional_wheeled_robot.py)
 
 Check out the [examples](https://github.com/tasts-robots/pink/tree/master/examples) folder for more.
 
 ## How can I help?
 
 Install the library and use it! Report bugs in the [issue tracker](https://github.com/tasts-robots/pink/issues). If you are a developer with some robotics experience looking to hack on open source, check out the [contribution guidelines](CONTRIBUTING.md).
```

### Comparing `pin-pink-0.9.0/doc/Makefile` & `pin-pink-1.0.0/doc/Makefile`

 * *Files 10% similar despite different names*

```diff
@@ -16,20 +16,18 @@
 
 # You can set these variables from the command line.
 SPHINXOPTS    = -W
 SPHINXBUILD   = sphinx-build
 SOURCEDIR     = src
 BUILDDIR      = build
 ONLINEDIR     = tasts-robots.org:public_html/doc/pink
-PDFFILE       = pink.pdf
 
 .PHONY: help Makefile upload
 
 help:
 	@$(SPHINXBUILD) -M help "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS)
 
 %: Makefile
 	@$(SPHINXBUILD) -M $@ "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS)
 
-upload: clean html latexpdf
-	cp $(BUILDDIR)/latex/$(PDFFILE) $(BUILDDIR)/html/$(PDFFILE)
+upload: clean html
 	rsync -auvz --delete-after $(BUILDDIR)/html/ $(ONLINEDIR)/
```

### Comparing `pin-pink-0.9.0/doc/src/conf.py` & `pin-pink-1.0.0/doc/src/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,17 @@
 # The full version, including alpha/beta/rc tags.
 release = None  # read from __init__.py
 
 # Read version info directly from the module's __init__.py
 init_path = join(dirname(dirname(dirname(str(abspath(__file__))))), "pink")
 with open(f"{init_path}/__init__.py", "r") as fh:
     for line in fh:
-        match = re.match('__version__ = "((\\d.\\d).\\d)[a-z0-9\\-]*".*', line)
+        match = re.match(
+            '__version__ = "((\\d+\\.\\d+)\\.\\d+)[a-z0-9\\-]*".*', line
+        )
         if match is not None:
             release = match.group(1)
             version = match.group(2)
             break
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
```

### Comparing `pin-pink-0.9.0/doc/src/css/custom.css` & `pin-pink-1.0.0/doc/src/css/custom.css`

 * *Files identical despite different names*

### Comparing `pin-pink-0.9.0/doc/src/images/apple-touch-icon-180x180.png` & `pin-pink-1.0.0/doc/src/images/apple-touch-icon-180x180.png`

 * *Files identical despite different names*

### Comparing `pin-pink-0.9.0/doc/src/images/favicon-16x16.png` & `pin-pink-1.0.0/doc/src/images/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `pin-pink-0.9.0/doc/src/images/favicon-32x32.png` & `pin-pink-1.0.0/doc/src/images/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `pin-pink-0.9.0/doc/src/images/pink-round-corners-140x140.png` & `pin-pink-1.0.0/doc/src/images/pink-round-corners-140x140.png`

 * *Files identical despite different names*

### Comparing `pin-pink-0.9.0/doc/src/index.rst` & `pin-pink-1.0.0/doc/src/index.rst`

 * *Files 10% similar despite different names*

```diff
@@ -9,21 +9,21 @@
 .. image:: images/pink-round-corners-140x140.png
    :height: 140px
    :alt: alternate text
    :align: right
 
 **P**\ ython **in**\ verse **k**\ inematics for articulated robot models, based on `Pinocchio <https://github.com/stack-of-tasks/pinocchio>`_.
 
-Inverse kinematics in Pink is defined by weighted :ref:`tasks <Tasks>` and :ref:`joint limits <Joint limits>`. The library adds a :ref:`configuration <Configuration>` type to Pinocchio, a configuration being a robot model and data to which forward kinematics have been applied. Given a configuration, tasks and a time step, :func:`pink.solve_ik.solve_ik` computes joint velocities that steer the model towards fulfilling all tasks at best.
+Inverse kinematics in Pink is defined by weighted :ref:`tasks <Tasks>` and :ref:`limits <Limits>`. The library adds a :ref:`configuration <Configuration>` type to Pinocchio, a configuration being a robot model and data to which forward kinematics have been applied. Given a configuration, tasks and a time step, :func:`pink.solve_ik.solve_ik` computes joint velocities that steer the model towards fulfilling all tasks at best.
 
 .. toctree::
     :maxdepth: 1
 
     installation.rst
     introduction.rst
     tasks.rst
-    joint-limits.rst
+    limits.rst
     inverse-kinematics.rst
     developer-notes.rst
     references.rst
 
 You can also download this documentation as a `PDF document <pink.pdf>`_.
```

### Comparing `pin-pink-0.9.0/doc/src/installation.rst` & `pin-pink-1.0.0/doc/src/installation.rst`

 * *Files identical despite different names*

### Comparing `pin-pink-0.9.0/doc/src/introduction.rst` & `pin-pink-1.0.0/doc/src/introduction.rst`

 * *Files identical despite different names*

### Comparing `pin-pink-0.9.0/doc/src/inverse-kinematics.rst` & `pin-pink-1.0.0/doc/src/inverse-kinematics.rst`

 * *Files identical despite different names*

### Comparing `pin-pink-0.9.0/doc/src/references.rst` & `pin-pink-1.0.0/doc/src/references.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 :github_url: https://github.com/tasts-robots/pink/tree/master/doc/src/references.rst
 
 **********
 References
 **********
 
-.. [BodyTaskJacobian] `Jacobian of a kinematic task and derivatives on manifolds <https://scaron.info/robotics/jacobian-of-a-kinematic-task-and-derivatives-on-manifolds.html>`_. S. Caron. 2023.
+.. [FrameTaskJacobian] `Jacobian of a kinematic task and derivatives on manifolds <https://scaron.info/robotics/jacobian-of-a-kinematic-task-and-derivatives-on-manifolds.html>`_. S. Caron. 2023.
 
 .. [MLT] `A micro Lie theory for state estimation in robotics <https://arxiv.org/abs/1812.01537>`_. J. Solà, J. Deray, D. Atchuthan. 2018.
 
 .. [Sugihara2011] *Solvability-Unconcerned Inverse Kinematics by the Levenberg-Marquardt Method*. T. Sugihara. IEEE transactions on robotics, 2011, vol. 27, no 5, p. 984-991.
```

### Comparing `pin-pink-0.9.0/doc/src/tasks.rst` & `pin-pink-1.0.0/doc/src/tasks.rst`

 * *Files 24% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 .. automodule:: pink.tasks.task
     :members:
 
 Body task
 =========
 
-.. automodule:: pink.tasks.body_task
+.. automodule:: pink.tasks.frame_task
     :members:
 
 Joint coupling task
 ===================
 
 .. automodule:: pink.tasks.joint_coupling_task
     :members:
```

### Comparing `pin-pink-0.9.0/examples/arm_kinova_gen2.py` & `pin-pink-1.0.0/examples/arm_kinova_gen2.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import meshcat_shapes
 import numpy as np
 import qpsolvers
 from loop_rate_limiters import RateLimiter
 
 import pink
 from pink import solve_ik
-from pink.tasks import BodyTask, PostureTask
+from pink.tasks import FrameTask, PostureTask
 from pink.utils import custom_configuration_vector
 from pink.visualization import start_meshcat_visualizer
 
 try:
     from robot_descriptions.loaders.pinocchio import load_robot_description
 except ModuleNotFoundError:
     raise ModuleNotFoundError(
@@ -37,15 +37,15 @@
     )
 
 
 if __name__ == "__main__":
     robot = load_robot_description("gen2_description", root_joint=None)
     viz = start_meshcat_visualizer(robot)
 
-    end_effector_task = BodyTask(
+    end_effector_task = FrameTask(
         "j2s6s200_end_effector",
         position_cost=1.0,  # [cost] / [m]
         orientation_cost=1.0,  # [cost] / [rad]
     )
 
     posture_task = PostureTask(
         cost=1e-3,  # [cost] / [rad]
@@ -81,15 +81,15 @@
         end_effector_target = end_effector_task.transform_target_to_world
         end_effector_target.translation[1] = 0.8 + 0.1 * np.sin(2.0 * t)
         end_effector_target.translation[2] = 0.2
 
         # Update visualization frames
         viewer["end_effector_target"].set_transform(end_effector_target.np)
         viewer["end_effector"].set_transform(
-            configuration.get_transform_body_to_world(
+            configuration.get_transform_frame_to_world(
                 end_effector_task.body
             ).np
         )
 
         # Compute velocity and integrate it into next configuration
         velocity = solve_ik(configuration, tasks, dt, solver=solver)
         configuration.integrate_inplace(velocity, dt)
```

### Comparing `pin-pink-0.9.0/examples/arm_ur3.py` & `pin-pink-1.0.0/examples/arm_ur3.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import meshcat_shapes
 import numpy as np
 import qpsolvers
 from loop_rate_limiters import RateLimiter
 
 import pink
 from pink import solve_ik
-from pink.tasks import BodyTask, PostureTask
+from pink.tasks import FrameTask, PostureTask
 from pink.utils import custom_configuration_vector
 from pink.visualization import start_meshcat_visualizer
 
 try:
     from robot_descriptions.loaders.pinocchio import load_robot_description
 except ModuleNotFoundError:
     raise ModuleNotFoundError(
@@ -37,15 +37,15 @@
     )
 
 
 if __name__ == "__main__":
     robot = load_robot_description("ur3_description", root_joint=None)
     viz = start_meshcat_visualizer(robot)
 
-    end_effector_task = BodyTask(
+    end_effector_task = FrameTask(
         "ee_link",
         position_cost=1.0,  # [cost] / [m]
         orientation_cost=1.0,  # [cost] / [rad]
         lm_damping=1.0,  # tuned for this setup
     )
 
     posture_task = PostureTask(
@@ -82,15 +82,15 @@
         end_effector_target = end_effector_task.transform_target_to_world
         end_effector_target.translation[1] = 0.5 + 0.1 * np.sin(2.0 * t)
         end_effector_target.translation[2] = 0.2
 
         # Update visualization frames
         viewer["end_effector_target"].set_transform(end_effector_target.np)
         viewer["end_effector"].set_transform(
-            configuration.get_transform_body_to_world(
+            configuration.get_transform_frame_to_world(
                 end_effector_task.body
             ).np
         )
 
         # Compute velocity and integrate it into next configuration
         velocity = solve_ik(configuration, tasks, dt, solver=solver)
         configuration.integrate_inplace(velocity, dt)
```

### Comparing `pin-pink-0.9.0/examples/double_pendulum.py` & `pin-pink-1.0.0/examples/double_pendulum.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 import numpy as np
 import pinocchio as pin
 import qpsolvers
 from loop_rate_limiters import RateLimiter
 
 import pink
 from pink import solve_ik
-from pink.tasks import BodyTask, PostureTask
+from pink.tasks import FrameTask, PostureTask
 from pink.visualization import start_meshcat_visualizer
 
 if __name__ == "__main__":
 
     # Load robot description
     urdf_path = os.path.join(
         os.path.dirname(__file__),
@@ -48,15 +48,15 @@
     viz = start_meshcat_visualizer(robot)
     viewer = viz.viewer
     meshcat_shapes.frame(viewer["target_frame"], opacity=0.5)
     meshcat_shapes.frame(viewer["tip_frame"], opacity=1.0)
 
     # Define tasks
     tasks = {
-        "tip": BodyTask(
+        "tip": FrameTask(
             "link3",
             position_cost=1.0,  # [cost] / [m]
             orientation_cost=1e-3,  # [cost] / [rad]
         ),
         "posture": PostureTask(
             cost=1e-2,  # [cost] / [rad]
         ),
@@ -83,15 +83,15 @@
         # Update task targets
         T = tasks["tip"].transform_target_to_world
         T.translation[1] = 0.1 * np.sin(t)
 
         # Update visualizer frames
         viewer["target_frame"].set_transform(T.np)
         viewer["tip_frame"].set_transform(
-            configuration.get_transform_body_to_world(tasks["tip"].body).np
+            configuration.get_transform_frame_to_world(tasks["tip"].body).np
         )
 
         # Compute velocity and integrate it into next configuration
         velocity = solve_ik(configuration, tasks.values(), dt, solver=solver)
         configuration.integrate_inplace(velocity, dt)
 
         # Visualize result at fixed FPS
```

### Comparing `pin-pink-0.9.0/examples/humanoid_draco3.py` & `pin-pink-1.0.0/examples/humanoid_draco3.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,32 +13,23 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """DRACO 3 humanoid standing on two feet and reaching with a hand."""
 
-import os
-import sys
-
-import meshcat_shapes
 import numpy as np
 import pinocchio as pin
 import qpsolvers
 from loop_rate_limiters import RateLimiter
 
-cwd = os.getcwd()
-sys.path.append(cwd)
+import meshcat_shapes
 import pink
 from pink import solve_ik
-from pink.tasks import (
-    BodyTask,
-    JointCouplingTask,
-    PostureTask,
-)
+from pink.tasks import FrameTask, JointCouplingTask, PostureTask
 
 try:
     from robot_descriptions.loaders.pinocchio import load_robot_description
 except ModuleNotFoundError:
     raise ModuleNotFoundError(
         "Examples need robot_descriptions, "
         "try `pip install robot_descriptions`"
@@ -87,79 +78,95 @@
     viz.loadViewerModel()
 
     # Set initial robot configuration
     configuration = pink.Configuration(robot.model, robot.data, robot.q0)
     viz.display(configuration.q)
 
     # Tasks initialization for IK
-    left_foot_task = BodyTask(
-        "l_foot_contact", position_cost=1.0, orientation_cost=1.0
-    )
-    pelvis_task = BodyTask(
-        "torso_com_link", position_cost=1.0, orientation_cost=0.0
-    )
-    right_foot_task = BodyTask(
-        "r_foot_contact", position_cost=1.0, orientation_cost=1.0
-    )
-    right_wrist_task = BodyTask(
-        "r_hand_contact", position_cost=4.0, orientation_cost=4.0
+    left_foot_task = FrameTask(
+        "l_foot_contact",
+        position_cost=1.0,
+        orientation_cost=1.0,
+    )
+    pelvis_task = FrameTask(
+        "torso_com_link",
+        position_cost=1.0,
+        orientation_cost=0.0,
+    )
+    right_foot_task = FrameTask(
+        "r_foot_contact",
+        position_cost=1.0,
+        orientation_cost=1.0,
+    )
+    right_wrist_task = FrameTask(
+        "r_hand_contact",
+        position_cost=4.0,
+        orientation_cost=4.0,
     )
     posture_task = PostureTask(
         cost=1e-1,  # [cost] / [rad]
     )
 
     # Joint coupling task
     r_knee_holonomic_task = JointCouplingTask(
-        ["r_knee_fe_jp", "r_knee_fe_jd"], [1.0, -1.0], 100.0, configuration
+        ["r_knee_fe_jp", "r_knee_fe_jd"],
+        [1.0, -1.0],
+        100.0,
+        configuration,
+        lm_damping=1e-7,
     )
     l_knee_holonomic_task = JointCouplingTask(
-        ["l_knee_fe_jp", "l_knee_fe_jd"], [1.0, -1.0], 100.0, configuration
+        ["l_knee_fe_jp", "l_knee_fe_jd"],
+        [1.0, -1.0],
+        100.0,
+        configuration,
+        lm_damping=1e-7,
     )
 
     tasks = [
         left_foot_task,
         pelvis_task,
         right_foot_task,
         right_wrist_task,
         posture_task,
         l_knee_holonomic_task,
         r_knee_holonomic_task,
     ]
 
     # Task target specifications
-    pelvis_pose = configuration.get_transform_body_to_world(
+    pelvis_pose = configuration.get_transform_frame_to_world(
         "torso_com_link"
     ).copy()
     pelvis_pose.translation[0] += 0.05
     pelvis_task.set_target(pelvis_pose)
 
     transform_l_ankle_target_to_init = pin.SE3(
         np.eye(3), np.array([0.1, 0.0, 0.0])
     )
     transform_r_ankle_target_to_init = pin.SE3(
         np.eye(3), np.array([-0.1, 0.0, 0.0])
     )
 
     left_foot_task.set_target(
-        configuration.get_transform_body_to_world("l_foot_contact")
+        configuration.get_transform_frame_to_world("l_foot_contact")
         * transform_l_ankle_target_to_init
     )
     right_foot_task.set_target(
-        configuration.get_transform_body_to_world("r_foot_contact")
+        configuration.get_transform_frame_to_world("r_foot_contact")
         * transform_r_ankle_target_to_init
     )
 
     pelvis_task.set_target(
-        configuration.get_transform_body_to_world("torso_com_link")
+        configuration.get_transform_frame_to_world("torso_com_link")
     )
 
     posture_task.set_target_from_configuration(configuration)
 
     right_wrist_pose = WavingPose(
-        configuration.get_transform_body_to_world("r_hand_contact")
+        configuration.get_transform_frame_to_world("r_hand_contact")
     )
 
     wrist_frame = viz.viewer["right_wrist_pose"]
     meshcat_shapes.frame(wrist_frame)
 
     # Select QP solver
     solver = qpsolvers.available_solvers[0]
```

### Comparing `pin-pink-0.9.0/examples/humanoid_jvrc.py` & `pin-pink-1.0.0/examples/humanoid_jvrc.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import numpy as np
 import pinocchio as pin
 import qpsolvers
 from loop_rate_limiters import RateLimiter
 
 import pink
 from pink import solve_ik
-from pink.tasks import BodyTask
+from pink.tasks import FrameTask
 
 try:
     from robot_descriptions.loaders.pinocchio import load_robot_description
 except ModuleNotFoundError:
     raise ModuleNotFoundError(
         "Examples need robot_descriptions, "
         "try `pip install robot_descriptions`"
@@ -74,53 +74,53 @@
     robot.setVisualizer(viz, init=False)
     viz.initViewer(open=True)
     viz.loadViewerModel()
 
     configuration = pink.Configuration(robot.model, robot.data, robot.q0)
     viz.display(configuration.q)
 
-    left_foot_task = BodyTask(
+    left_foot_task = FrameTask(
         "l_ankle", position_cost=1.0, orientation_cost=3.0
     )
-    pelvis_task = BodyTask("PELVIS_S", position_cost=1.0, orientation_cost=0.0)
-    right_foot_task = BodyTask(
+    pelvis_task = FrameTask("PELVIS_S", position_cost=1.0, orientation_cost=0.0)
+    right_foot_task = FrameTask(
         "r_ankle", position_cost=1.0, orientation_cost=3.0
     )
-    right_wrist_task = BodyTask(
+    right_wrist_task = FrameTask(
         "r_wrist", position_cost=1.0, orientation_cost=3.0
     )
     tasks = [left_foot_task, pelvis_task, right_foot_task, right_wrist_task]
 
-    pelvis_pose = configuration.get_transform_body_to_world("PELVIS_S").copy()
+    pelvis_pose = configuration.get_transform_frame_to_world("PELVIS_S").copy()
     pelvis_pose.translation[0] += 0.05
     meshcat_shapes.frame(viz.viewer["pelvis_pose"])
     viz.viewer["pelvis_pose"].set_transform(pelvis_pose.np)
     pelvis_task.set_target(pelvis_pose)
 
     transform_l_ankle_target_to_init = pin.SE3(
         np.eye(3), np.array([0.1, 0.0, 0.0])
     )
     transform_r_ankle_target_to_init = pin.SE3(
         np.eye(3), np.array([-0.1, 0.0, 0.0])
     )
 
     left_foot_task.set_target(
-        configuration.get_transform_body_to_world("l_ankle")
+        configuration.get_transform_frame_to_world("l_ankle")
         * transform_l_ankle_target_to_init
     )
     right_foot_task.set_target(
-        configuration.get_transform_body_to_world("r_ankle")
+        configuration.get_transform_frame_to_world("r_ankle")
         * transform_r_ankle_target_to_init
     )
     pelvis_task.set_target(
-        configuration.get_transform_body_to_world("PELVIS_S")
+        configuration.get_transform_frame_to_world("PELVIS_S")
     )
 
     right_wrist_pose = WavingPose(
-        configuration.get_transform_body_to_world("r_wrist")
+        configuration.get_transform_frame_to_world("r_wrist")
     )
 
     wrist_frame = viz.viewer["right_wrist_pose"]
     meshcat_shapes.frame(wrist_frame)
 
     # Select QP solver
     solver = qpsolvers.available_solvers[0]
```

### Comparing `pin-pink-0.9.0/examples/humanoid_sigmaban.py` & `pin-pink-1.0.0/examples/humanoid_sigmaban.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import numpy as np
 import pinocchio as pin
 import qpsolvers
 from loop_rate_limiters import RateLimiter
 
 import pink
 from pink import solve_ik
-from pink.tasks import BodyTask, PostureTask
+from pink.tasks import FrameTask, PostureTask
 
 try:
     from robot_descriptions.loaders.pinocchio import load_robot_description
 except ModuleNotFoundError:
     raise ModuleNotFoundError(
         "Examples need robot_descriptions, "
         "try `pip install robot_descriptions`"
@@ -47,55 +47,55 @@
     viz.initViewer(open=True)
     viz.loadViewerModel()
 
     configuration = pink.Configuration(robot.model, robot.data, robot.q0)
     viz.display(configuration.q)
     viewer = viz.viewer
 
-    left_foot_task = BodyTask(
+    left_foot_task = FrameTask(
         "left_foot_tip",
         position_cost=1.0,
         orientation_cost=1.0,
     )
-    torso_task = BodyTask(
+    torso_task = FrameTask(
         "torso",
         position_cost=1.0,
         orientation_cost=1.0,
     )
-    right_foot_task = BodyTask(
+    right_foot_task = FrameTask(
         "right_foot_tip",
         position_cost=1.0,
         orientation_cost=1.0,
     )
     posture_task = PostureTask(
         cost=1e-2,  # [cost] / [rad]
     )
     tasks = [left_foot_task, torso_task, right_foot_task, posture_task]
 
-    torso_pose = configuration.get_transform_body_to_world("torso").copy()
+    torso_pose = configuration.get_transform_frame_to_world("torso").copy()
     # torso_pose.translation[0] += 0.05
     torso_task.set_target(torso_pose)
     posture_task.set_target_from_configuration(configuration)
 
     transform_left_foot_tip_target_to_init = pin.SE3(
         np.eye(3), np.array([0.0, 0.03, 0.0])
     )
     transform_right_foot_tip_target_to_init = pin.SE3(
         np.eye(3), np.array([0.0, -0.03, 0.0])
     )
 
     left_foot_task.set_target(
-        configuration.get_transform_body_to_world("left_foot_tip")
+        configuration.get_transform_frame_to_world("left_foot_tip")
         * transform_left_foot_tip_target_to_init
     )
     right_foot_task.set_target(
-        configuration.get_transform_body_to_world("right_foot_tip")
+        configuration.get_transform_frame_to_world("right_foot_tip")
         * transform_right_foot_tip_target_to_init
     )
-    torso_task.set_target(configuration.get_transform_body_to_world("torso"))
+    torso_task.set_target(configuration.get_transform_frame_to_world("torso"))
 
     # Display targets
     meshcat_shapes.frame(viewer["left_foot_target"], opacity=0.5)
     meshcat_shapes.frame(viewer["right_foot_target"], opacity=0.5)
     meshcat_shapes.frame(viewer["torso_target"], opacity=0.5)
     viewer["left_foot_target"].set_transform(
         left_foot_task.transform_target_to_world.np
```

### Comparing `pin-pink-0.9.0/examples/load_custom_urdf.py` & `pin-pink-1.0.0/examples/load_custom_urdf.py`

 * *Files identical despite different names*

### Comparing `pin-pink-0.9.0/examples/meshcat_shapes.py` & `pin-pink-1.0.0/examples/meshcat_shapes.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,27 +43,27 @@
     Note:
         As per the de-facto standard (Blender, OpenRAVE, RViz, ...), the
         x-axis is red, the y-axis is green and the z-axis is blue.
     """
     direction_names = ["x", "y", "z"]
     colors = [0xFF0000, 0x00FF00, 0x0000FF]
     rotation_axes = [[0, 0, 1], [0, 1, 0], [1, 0, 0]]
-    position_cylinder_in_body = 0.5 * length * np.eye(3)
+    position_cylinder_in_frame = 0.5 * length * np.eye(3)
     for i in range(3):
         dir_name = direction_names[i]
         material = meshcat.geometry.MeshLambertMaterial(
             color=colors[i], opacity=opacity
         )
-        transform_cylinder_to_body = meshcat.transformations.rotation_matrix(
+        transform_cylinder_to_frame = meshcat.transformations.rotation_matrix(
             np.pi / 2, rotation_axes[i]
         )
-        transform_cylinder_to_body[0:3, 3] = position_cylinder_in_body[i]
+        transform_cylinder_to_frame[0:3, 3] = position_cylinder_in_frame[i]
         cylinder = meshcat.geometry.Cylinder(length, thickness)
         handle[dir_name].set_object(cylinder, material)
-        handle[dir_name].set_transform(transform_cylinder_to_body)
+        handle[dir_name].set_transform(transform_cylinder_to_frame)
 
 
 def frame(
     handle: meshcat.Visualizer,
     axis_length: float = 0.1,
     axis_thickness: float = 0.005,
     opacity: float = 1.0,
```

### Comparing `pin-pink-0.9.0/examples/omnidirectional_wheeled_robot.py` & `pin-pink-1.0.0/examples/mobile_omni_wheeled_robot.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 import numpy as np
 import pinocchio as pin
 import qpsolvers
 from loop_rate_limiters import RateLimiter
 
 import pink
 from pink import solve_ik
-from pink.tasks import BodyTask
+from pink.tasks import FrameTask
 from pink.visualization import start_meshcat_visualizer
 
 if __name__ == "__main__":
 
     # Load robot description
     urdf_path = os.path.join(
         os.path.dirname(__file__),
@@ -50,15 +50,15 @@
     # Initialize visualizer
     viz = start_meshcat_visualizer(robot)
     viewer = viz.viewer
     meshcat_shapes.frame(viewer["target_frame"], opacity=0.5)
     meshcat_shapes.frame(viewer["tip_frame"], opacity=1.0)
 
     # Define tasks
-    base_task = BodyTask(
+    base_task = FrameTask(
         "base",
         position_cost=1.0,  # [cost] / [m]
         orientation_cost=1e-5,  # [cost] / [rad]
     )
     base_task.gain = 0.22  # slow things down
     tasks = [base_task]
 
@@ -82,15 +82,15 @@
         T = base_task.transform_target_to_world
         T.translation[0] = 0.2 * jumpy
         T.rotation = pin.utils.rpyToMatrix(0.0, 0.0, np.pi * jumpy)
 
         # Update visualizer frames
         viewer["target_frame"].set_transform(T.np)
         viewer["tip_frame"].set_transform(
-            configuration.get_transform_body_to_world(base_task.body).np
+            configuration.get_transform_frame_to_world(base_task.body).np
         )
 
         # Compute velocity and integrate it into next configuration
         velocity = solve_ik(configuration, tasks, dt, solver=solver)
         configuration.integrate_inplace(velocity, dt)
 
         # Visualize result at fixed FPS
```

### Comparing `pin-pink-0.9.0/examples/robots/double_pendulum.urdf` & `pin-pink-1.0.0/examples/robots/double_pendulum.urdf`

 * *Files identical despite different names*

### Comparing `pin-pink-0.9.0/examples/robots/omnidirectional_wheeled_robot.urdf` & `pin-pink-1.0.0/examples/robots/omnidirectional_wheeled_robot.urdf`

 * *Files identical despite different names*

### Comparing `pin-pink-0.9.0/examples/visualize_in_meshcat.py` & `pin-pink-1.0.0/examples/visualize_in_meshcat.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import numpy as np
 import pinocchio as pin
 import qpsolvers
 from loop_rate_limiters import RateLimiter
 
 import pink
 from pink import solve_ik
-from pink.tasks import BodyTask, PostureTask
+from pink.tasks import FrameTask, PostureTask
 from pink.utils import custom_configuration_vector
 from pink.visualization import start_meshcat_visualizer
 
 try:
     from robot_descriptions.loaders.pinocchio import load_robot_description
 except ModuleNotFoundError:
     raise ModuleNotFoundError(
@@ -41,25 +41,25 @@
 if __name__ == "__main__":
     robot = load_robot_description(
         "upkie_description", root_joint=pin.JointModelFreeFlyer()
     )
     viz = start_meshcat_visualizer(robot)
 
     tasks = {
-        "base": BodyTask(
+        "base": FrameTask(
             "base",
             position_cost=1.0,  # [cost] / [m]
             orientation_cost=1.0,  # [cost] / [rad]
         ),
-        "left_contact": BodyTask(
+        "left_contact": FrameTask(
             "left_contact",
             position_cost=[0.1, 0.0, 0.1],  # [cost] / [m]
             orientation_cost=0.0,  # [cost] / [rad]
         ),
-        "right_contact": BodyTask(
+        "right_contact": FrameTask(
             "right_contact",
             position_cost=[0.1, 0.0, 0.1],  # [cost] / [m]
             orientation_cost=0.0,  # [cost] / [rad]
         ),
         "posture": PostureTask(
             cost=1e-3,  # [cost] / [rad]
         ),
@@ -67,15 +67,15 @@
 
     tasks["posture"].set_target(
         custom_configuration_vector(robot, left_knee=0.2, right_knee=-0.2)
     )
 
     configuration = pink.Configuration(robot.model, robot.data, robot.q0)
     for body, task in tasks.items():
-        if type(task) is BodyTask:
+        if type(task) is FrameTask:
             task.set_target_from_configuration(configuration)
     viz.display(configuration.q)
 
     left_contact_target = tasks["left_contact"].transform_target_to_world
     right_contact_target = tasks["right_contact"].transform_target_to_world
 
     viewer = viz.viewer
@@ -98,15 +98,15 @@
         right_contact_target.translation[2] += 0.1 * np.sin(t) * dt
 
         # Update visualization frames
         viewer["left_contact_target"].set_transform(left_contact_target.np)
         viewer["right_contact_target"].set_transform(right_contact_target.np)
         for body in ["left_contact", "right_contact"]:
             viewer[body].set_transform(
-                configuration.get_transform_body_to_world(body).np
+                configuration.get_transform_frame_to_world(body).np
             )
 
         # Compute velocity and integrate it into next configuration
         velocity = solve_ik(configuration, tasks.values(), dt, solver=solver)
         configuration.integrate_inplace(velocity, dt)
 
         # Visualize result at fixed FPS
```

### Comparing `pin-pink-0.9.0/examples/visualize_in_yourdfpy.py` & `pin-pink-1.0.0/examples/visualize_in_yourdfpy.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import pinocchio as pin
 import qpsolvers
 import yourdfpy
 from loop_rate_limiters import RateLimiter
 
 import pink
 from pink import solve_ik
-from pink.tasks import BodyTask, PostureTask
+from pink.tasks import FrameTask, PostureTask
 from pink.utils import custom_configuration_vector
 
 try:
     from robot_descriptions import upkie_description
     from robot_descriptions.loaders.pinocchio import load_robot_description
 except ModuleNotFoundError:
     raise ModuleNotFoundError(
@@ -40,47 +40,47 @@
 
 if __name__ == "__main__":
     robot = load_robot_description(
         "upkie_description", root_joint=pin.JointModelFreeFlyer()
     )
 
     tasks = {
-        "base": BodyTask(
+        "base": FrameTask(
             "base",
             position_cost=1.0,  # [cost] / [m]
             orientation_cost=1.0,  # [cost] / [rad]
         ),
-        "left_contact": BodyTask(
+        "left_contact": FrameTask(
             "left_contact",
             position_cost=[0.1, 0.0, 0.1],  # [cost] / [m]
             orientation_cost=0.0,  # [cost] / [rad]
         ),
-        "right_contact": BodyTask(
+        "right_contact": FrameTask(
             "right_contact",
             position_cost=[0.1, 0.0, 0.1],  # [cost] / [m]
             orientation_cost=0.0,  # [cost] / [rad]
         ),
         "posture": PostureTask(
             cost=1e-3,  # [cost] / [rad]
         ),
     }
 
     configuration = pink.Configuration(robot.model, robot.data, robot.q0)
     for body, task in tasks.items():
-        if type(task) is BodyTask:
+        if type(task) is FrameTask:
             task.set_target_from_configuration(configuration)
 
     tasks["posture"].set_target(
         custom_configuration_vector(robot, left_knee=0.2, right_knee=-0.2)
     )
 
-    left_contact_target = configuration.get_transform_body_to_world(
+    left_contact_target = configuration.get_transform_frame_to_world(
         "left_contact"
     )
-    right_contact_target = configuration.get_transform_body_to_world(
+    right_contact_target = configuration.get_transform_frame_to_world(
         "right_contact"
     )
 
     # Select QP solver
     solver = qpsolvers.available_solvers[0]
     if "quadprog" in qpsolvers.available_solvers:
         solver = "quadprog"
```

### Comparing `pin-pink-0.9.0/examples/wheeled_biped_upkie.py` & `pin-pink-1.0.0/examples/wheeled_biped_upkie.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import meshcat_shapes
 import numpy as np
 import qpsolvers
 from loop_rate_limiters import RateLimiter
 
 import pink
 from pink import solve_ik
-from pink.tasks import BodyTask, PostureTask
+from pink.tasks import FrameTask, PostureTask
 from pink.utils import custom_configuration_vector
 from pink.visualization import start_meshcat_visualizer
 
 try:
     from robot_descriptions.loaders.pinocchio import load_robot_description
 except ModuleNotFoundError:
     raise ModuleNotFoundError(
@@ -41,35 +41,35 @@
     full_robot = load_robot_description("upkie_description", root_joint=None)
     robot = full_robot.buildReducedRobot(
         list_of_joints_to_lock=["left_wheel", "right_wheel"]
     )
     viz = start_meshcat_visualizer(robot)
 
     tasks = {
-        "left_contact": BodyTask(
+        "left_contact": FrameTask(
             "left_contact",
             position_cost=[0.1, 0.0, 0.1],  # [cost] / [m]
             orientation_cost=0.0,  # [cost] / [rad]
         ),
-        "right_contact": BodyTask(
+        "right_contact": FrameTask(
             "right_contact",
             position_cost=[0.1, 0.0, 0.1],  # [cost] / [m]
             orientation_cost=0.0,  # [cost] / [rad]
         ),
         "posture": PostureTask(
             cost=1e-3,  # [cost] / [rad]
         ),
     }
 
     q_ref = custom_configuration_vector(
         robot, left_hip=-0.2, left_knee=0.4, right_hip=0.2, right_knee=-0.4
     )
     configuration = pink.Configuration(robot.model, robot.data, q_ref)
     for body, task in tasks.items():
-        if type(task) is BodyTask:
+        if type(task) is FrameTask:
             task.set_target_from_configuration(configuration)
     tasks["posture"].set_target(q_ref)
     viz.display(configuration.q)
 
     left_contact_target = tasks["left_contact"].transform_target_to_world
     right_contact_target = tasks["right_contact"].transform_target_to_world
 
@@ -93,15 +93,15 @@
         right_contact_target.translation[2] += 0.1 * np.sin(t) * dt
 
         # Update visualization frames
         viewer["left_contact_target"].set_transform(left_contact_target.np)
         viewer["right_contact_target"].set_transform(right_contact_target.np)
         for body in ["left_contact", "right_contact"]:
             viewer[body].set_transform(
-                configuration.get_transform_body_to_world(body).np
+                configuration.get_transform_frame_to_world(body).np
             )
 
         # Compute velocity and integrate it into next configuration
         velocity = solve_ik(configuration, tasks.values(), dt, solver=solver)
         configuration.integrate_inplace(velocity, dt)
 
         # Visualize result at fixed FPS
```

### Comparing `pin-pink-0.9.0/pink/__init__.py` & `pin-pink-1.0.0/pink/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 """Python inverse kinematics for your robot model based on Pinocchio."""
 
 from .configuration import Configuration
 from .solve_ik import build_ik, solve_ik
 from .tasks import Task
 from .utils import custom_configuration_vector
 
-__version__ = "0.9.0"
+__version__ = "1.0.0"
 
 __all__ = [
     "Configuration",
     "build_ik",
     "custom_configuration_vector",
     "solve_ik",
     "Task",
```

### Comparing `pin-pink-0.9.0/pink/bounded_tangent.py` & `pin-pink-1.0.0/pink/limits/velocity_limit.py`

 * *Files 21% similar despite different names*

```diff
@@ -12,79 +12,99 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Subset of bounded joints associated with a robot model."""
+"""Subset of velocity-limited joints in a robot model."""
 
-from typing import List, Optional
+from typing import List, Optional, Tuple
 
 import numpy as np
 import pinocchio as pin
 
-from .utils import VectorSpace
+from .limit import Limit
 
 
-class BoundedTangent(VectorSpace):
-    """Subspace of the tangent space restricted to bounded joints.
+class VelocityLimit(Limit):
+    """Subset of velocity-limited joints in a robot model.
 
     Attributes:
-        nv: Dimension of the full tangent space.
+        indices: Tangent indices corresponding to velocity-limited joints.
+        joints: List of velocity-limited joints.
+        model: Robot model.
+        projection_matrix: Projection from tangent space to subspace with
+            velocity-limited joints.
     """
 
     indices: np.ndarray
     joints: list
-    nv: int
+    model: pin.Model
     projection_matrix: Optional[np.ndarray]
-    velocity_limit: Optional[np.ndarray]
 
     def __init__(self, model: pin.Model):
-        """Bounded joints in a robot model.
+        """Initialize bounded tangent of a model.
 
         Args:
             model: robot model.
-
-        Returns:
-            List of bounded joints.
         """
-        has_configuration_limit = np.logical_and(
-            model.upperPositionLimit < 1e20,
-            model.upperPositionLimit > model.lowerPositionLimit + 1e-10,
+        has_velocity_limit = np.logical_and(
+            model.velocityLimit < 1e20,
+            model.velocityLimit > 1e-10,
         )
 
         joints = [
             joint
             for joint in model.joints
-            if joint.idx_q >= 0
-            and has_configuration_limit[
-                slice(joint.idx_q, joint.idx_q + joint.nq)
+            if joint.idx_v >= 0
+            and has_velocity_limit[
+                slice(joint.idx_v, joint.idx_v + joint.nv)
             ].all()
         ]
 
         index_list: List[int] = []
         for joint in joints:
             index_list.extend(range(joint.idx_v, joint.idx_v + joint.nv))
         indices = np.array(index_list)
         indices.setflags(write=False)
 
         dim = len(indices)
-        super().__init__(dim)
         projection_matrix = np.eye(model.nv)[indices] if dim > 0 else None
 
         self.indices = indices
         self.joints = joints
-        self.nv = model.nv
+        self.model = model
         self.projection_matrix = projection_matrix
-        self.velocity_limit = (
-            model.velocityLimit[indices] if len(joints) > 0 else None
-        )
 
-    def project(self, v: np.ndarray) -> np.ndarray:
-        """Project a tangent vector to the bounded tangent subspace.
+    def compute_qp_inequalities(
+        self,
+        q: np.ndarray,
+        dt: float,
+    ) -> Optional[Tuple[np.ndarray, np.ndarray]]:
+        r"""Compute the configuration-dependent velocity limits.
+
+        Those limits are defined by:
+
+        .. math::
+
+            -\mathrm{d}t v_{max} \leq \Delta q \leq \mathrm{d}t v_{max}
+
+        where :math:`v_{max} \in {\cal T}` is the robot's velocity limit
+        vector and :math:`\Delta q \in T_q({\cal C})` is the displacement
+        computed by the inverse kinematics.
 
         Args:
-            v: Vector from the original space.
+            q: Robot configuration.
+            dt: Integration timestep in [s].
+
+        Returns:
+            Pair :math:`(G, h)` representing the inequality constraint as
+            :math:`G \Delta q \leq h`, or ``None`` if there is no limit.
         """
-        assert v.shape == (self.nv,), "Dimension mismatch"
-        return v[self.indices]
+        if self.projection_matrix is None:  # no joint (thus checked for mypy)
+            return None
+
+        v_max = self.model.velocityLimit[self.indices]
+        G = np.vstack([self.projection_matrix, -self.projection_matrix])
+        h = np.hstack([dt * v_max, dt * v_max])
+        return G, h
```

### Comparing `pin-pink-0.9.0/pink/configuration.py` & `pin-pink-1.0.0/pink/configuration.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,16 +23,16 @@
 transforms and frame Jacobians used for IK can be queried from the robot's
 data.
 """
 
 import numpy as np
 import pinocchio as pin
 
-from .bounded_tangent import BoundedTangent
 from .exceptions import BodyNotFound, NotWithinConfigurationLimits
+from .limits import ConfigurationLimit, VelocityLimit
 from .utils import VectorSpace, get_root_joint_dim
 
 
 class Configuration:
     """Type indicating that configuration-dependent quantities are available.
 
     In Pink, this type enables access to frame transforms and frame Jacobians.
@@ -85,16 +85,18 @@
             Configurations copy data and run forward kinematics by default so
             that they are less error-prone for newcomers. You can avoid copies
             or forward kinematics (e.g. if it is already computed by the
             caller) using constructor parameters.
         """
         if not hasattr(model, "tangent"):
             model.tangent = VectorSpace(model.nv)
-        if not hasattr(model, "bounded_tangent"):
-            model.bounded_tangent = BoundedTangent(model)
+        if not hasattr(model, "configuration_limit"):
+            model.configuration_limit = ConfigurationLimit(model)
+        if not hasattr(model, "velocity_limit"):
+            model.velocity_limit = VelocityLimit(model)
         q_readonly = q.copy()
         q_readonly.setflags(write=False)
         self.data = data.copy() if copy_data else data
         self.model = model
         self.q = q_readonly
         self.tangent = model.tangent
         #
@@ -126,15 +128,15 @@
                 raise NotWithinConfigurationLimits(
                     i,
                     self.q[i],
                     q_min[i],
                     q_max[i],
                 )
 
-    def get_body_jacobian(self, body: str) -> np.ndarray:
+    def get_frame_jacobian(self, body: str) -> np.ndarray:
         r"""Compute the Jacobian matrix of the body velocity.
 
         This matrix :math:`{}_B J_{WB}` is related to the body velocity
         :math:`{}_B v_{WB}` by:
 
         .. math::
 
@@ -152,37 +154,37 @@
 
         - ``q[0:3]``: position in [m] of the floating base in the inertial
           frame, formatted as :math:`[p_x, p_y, p_z]`.
         - ``q[3:7]``: unit quaternion for the orientation of the floating base
           in the inertial frame, formatted as :math:`[q_x, q_y, q_z, q_w]`.
         - ``q[7:]``: joint angles in [rad].
         """
-        if not self.model.existBodyName(body):
+        if not self.model.existFrame(body):
             raise BodyNotFound(f"body {body} does not exist")
-        body_id = self.model.getBodyId(body)
+        frame_id = self.model.getFrameId(body)
         J: np.ndarray = pin.getFrameJacobian(
-            self.model, self.data, body_id, pin.ReferenceFrame.LOCAL
+            self.model, self.data, frame_id, pin.ReferenceFrame.LOCAL
         )
         return J
 
-    def get_transform_body_to_world(self, body: str) -> pin.SE3:
+    def get_transform_frame_to_world(self, body: str) -> pin.SE3:
         """Get the pose of a body frame in the current configuration.
 
         Args:
             body: Body frame name, typically the link name from the URDF.
 
         Returns:
             Current transform from body frame to world frame.
 
         Raises:
             KeyError: if the body name is not found in the robot model.
         """
-        body_id = self.model.getBodyId(body)
+        frame_id = self.model.getFrameId(body)
         try:
-            return self.data.oMf[body_id].copy()
+            return self.data.oMf[frame_id].copy()
         except IndexError as index_error:
             raise KeyError(
                 f'Body "{body}" not found in robot model'
             ) from index_error
 
     def integrate(self, velocity, dt) -> np.ndarray:
         """Integrate a velocity starting from the current configuration.
```

### Comparing `pin-pink-0.9.0/pink/exceptions.py` & `pin-pink-1.0.0/pink/exceptions.py`

 * *Files identical despite different names*

### Comparing `pin-pink-0.9.0/pink/solve_ik.py` & `pin-pink-1.0.0/pink/solve_ik.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 
 from typing import Iterable, Optional, Tuple
 
 import numpy as np
 import qpsolvers
 
 from .configuration import Configuration
-from .limits import compute_velocity_limits
 from .tasks import Task
 
 
 def __compute_qp_objective(
     configuration: Configuration, tasks: Iterable[Task], damping: float
 ) -> Tuple[np.ndarray, np.ndarray]:
     r"""Compute the QP objective function.
@@ -60,39 +59,47 @@
         H_task, c_task = task.compute_qp_objective(configuration)
         H += H_task
         c += c_task
     return (H, c)
 
 
 def __compute_qp_inequalities(
-    configuration, dt
+    configuration,
+    dt: float,
 ) -> Tuple[Optional[np.ndarray], Optional[np.ndarray]]:
-    """Compute inequality constraints for the quadratic program.
+    r"""Compute inequality constraints for the quadratic program.
 
     Args:
         configuration: Robot configuration to read kinematics from.
         dt: Integration timestep in [s].
 
     Returns:
-        Pair :math:`(G, h)` of inequality matrix and vector.
+        Pair :math:`(G, h)` of inequality matrix and vector representing the
+        inequality :math:`G \Delta q \leq h`, or ``(None, None)`` if there is
+        no inequality.
 
     Notes:
         We trim comparisons to infinity (equivalently: big floats) because some
         solvers don't support it. See for instance
         https://github.com/tasts-robots/pink/issues/10.
     """
-    v_max, v_min = compute_velocity_limits(configuration, dt)
-    if v_max is None or v_min is None:
+    configuration_limit = configuration.model.configuration_limit
+    velocity_limit = configuration.model.velocity_limit
+    q = configuration.q
+
+    G_list = []
+    h_list = []
+    for limit in (configuration_limit, velocity_limit):
+        matvec = limit.compute_qp_inequalities(q, dt)
+        if matvec is not None:
+            G_list.append(matvec[0])
+            h_list.append(matvec[1])
+    if not G_list:
         return None, None
-
-    bounded_tangent = configuration.model.bounded_tangent
-    bounded_proj = bounded_tangent.projection_matrix
-    G = np.vstack([bounded_proj, -bounded_proj])
-    h = np.hstack([dt * v_max, -dt * v_min])
-    return G, h
+    return np.vstack(G_list), np.hstack(h_list)
 
 
 def build_ik(
     configuration: Configuration,
     tasks: Iterable[Task],
     dt: float,
     damping: float = 1e-12,
```

### Comparing `pin-pink-0.9.0/pink/tasks/__init__.py` & `pin-pink-1.0.0/pink/tasks/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,23 +13,23 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Kinematic tasks."""
 
-from .body_task import BodyTask
 from .exceptions import TargetNotSet, TaskJacobianNotSet
+from .frame_task import FrameTask
 from .joint_coupling_task import JointCouplingTask
 from .linear_holonomic_task import LinearHolonomicTask
 from .posture_task import PostureTask
 from .task import Task
 
 __all__ = [
-    "BodyTask",
+    "FrameTask",
     "TargetNotSet",
     "TaskJacobianNotSet",
     "JointCouplingTask",
     "LinearHolonomicTask",
     "PostureTask",
     "Task",
 ]
```

### Comparing `pin-pink-0.9.0/pink/tasks/body_task.py` & `pin-pink-1.0.0/pink/tasks/frame_task.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,66 +13,52 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Body task implementation."""
 
-from typing import Optional, Sequence, Tuple, Union
+from typing import Optional, Sequence, Union
 
 import numpy as np
 import pinocchio as pin
 
 from ..configuration import Configuration
-from .exceptions import TargetNotSet
+from .exceptions import TargetNotSet, TaskDefinitionError
 from .task import Task
 from .utils import body_minus
 
 
-class BodyTask(Task):
+class FrameTask(Task):
     r"""Regulate the pose of a robot body in the world frame.
 
     Attributes:
         body: Body frame name, typically the link name from the URDF.
-        cost: 6D vector that specifies how much each coordinate (in the local
-            body frame) contributes to the cost. Position costs come first
-            (Pinocchio spatial vector convention) and are in
-            :math:`[\mathrm{cost}] / [\mathrm{m}]`, where the the unit of
-            :math:`[\mathrm{cost}]` up to the user. They are followed by
-            orientation costs in :math:`[\mathrm{cost}] / [\mathrm{rad}]`.
-            Set a cost to zero to disable the task along a coordinate (no cost
-            no effect).
-        lm_damping: Unitless scale of the Levenberg-Marquardt (only when
-            the error is large) regularization term, which helps when
-            targets are unfeasible. Increase this value if the task is too
-            jerky under unfeasible targets, but beware that a larger
-            damping slows down the task.
         transform_target_to_world: Target pose for the body frame.
 
-    Costs are designed so that position/orientation costs can be compared
-    between tasks. For example, if task 1 has a position cost of 1.0 and task 2
-    a position cost of 0.1, then a 1 [cm] error in task 1 costs as much as a 10
-    [cm] error in task 2.
+    Costs are designed so that errors with varying SI units, here position and
+    orientation displacements, can be cast to homogeneous values. For example,
+    if task "foo" has a position cost of 1.0 and task "bar" a position cost of
+    0.1, then a 1 [cm] error in task "foo" costs as much as a 10 [cm] error in
+    task "bar".
 
     Note:
         Dimensionally, the 6D cost vector is a (normalized) force screw and our
         objective function is a (normalized) energy.
     """
 
     body: str
-    cost: np.ndarray
-    lm_damping: float
     transform_target_to_world: Optional[pin.SE3]
 
     def __init__(
         self,
         body: str,
         position_cost: Union[float, Sequence[float]],
         orientation_cost: Union[float, Sequence[float]],
-        lm_damping: float = 1e-6,
+        lm_damping: float = 0.0,
     ) -> None:
         r"""Define a new body task.
 
         Args:
             body: Name of the body frame to move to the target pose.
             position_cost: Contribution of position errors to the normalized
                 cost, in :math:`[\mathrm{cost}] / [\mathrm{m}]`. If this is a
@@ -81,55 +67,68 @@
             orientation_cost: Contribution of orientation errors to the
                 normalized cost, in :math:`[\mathrm{cost}] / [\mathrm{rad}]`.
                 If this is a vector, the cost is anisotropic and each
                 coordinate corresponds to an axis in the local body frame.
             lm_damping: Levenberg-Marquardt damping (see class attributes). The
                 default value is conservatively low.
         """
+        to_be_updated_cost = np.ones(6)  # updated below
+        super().__init__(cost=to_be_updated_cost, lm_damping=lm_damping)
         self.body = body
-        self.cost = np.ones(6)
         self.lm_damping = lm_damping
         self.transform_target_to_world = None
         #
         self.set_position_cost(position_cost)
         self.set_orientation_cost(orientation_cost)
 
     def set_position_cost(
-        self, position_cost: Union[float, Sequence[float]]
+        self, position_cost: Union[float, Sequence[float], np.ndarray]
     ) -> None:
         r"""Set a new cost for all 3D position coordinates.
 
         Args:
             position_cost: Contribution of position errors to the normalized
                 cost, in :math:`[\mathrm{cost}] / [\mathrm{m}]`. If this is a
                 vector, the cost is anisotropic and each coordinate corresponds
                 to an axis in the local body frame.
         """
         if isinstance(position_cost, float):
             assert position_cost >= 0.0
         else:  # not isinstance(position_cost, float)
             assert all(cost >= 0.0 for cost in position_cost)
-        self.cost[0:3] = position_cost
+        if isinstance(self.cost, np.ndarray):
+            self.cost[0:3] = position_cost
+        else:  # self.cost is not a vector
+            raise TaskDefinitionError(
+                "Frame task cost should be a vector, "
+                f"currently cost={self.cost}"
+            )
 
     def set_orientation_cost(
-        self, orientation_cost: Union[float, Sequence[float]]
+        self, orientation_cost: Union[float, Sequence[float], np.ndarray]
     ) -> None:
         r"""Set a new cost for all 3D orientation coordinates.
 
         Args:
             orientation_cost: Contribution of orientation errors to the
                 normalized cost, in :math:`[\mathrm{cost}] / [\mathrm{rad}]`.
                 If this is a vector, the cost is anisotropic and each
                 coordinate corresponds to an axis in the local body frame.
         """
         if isinstance(orientation_cost, float):
             assert orientation_cost >= 0.0
         else:  # not isinstance(orientation_cost, float)
             assert all(cost >= 0.0 for cost in orientation_cost)
-        self.cost[3:6] = orientation_cost
+        if isinstance(self.cost, np.ndarray):
+            self.cost[3:6] = orientation_cost
+        else:  # self.cost is not a vector
+            raise TaskDefinitionError(
+                "Frame task cost should be a vector, "
+                f"currently cost={self.cost}"
+            )
 
     def set_target(
         self,
         transform_target_to_world: pin.SE3,
     ) -> None:
         """Set task target pose in the world frame.
 
@@ -143,15 +142,15 @@
         self, configuration: Configuration
     ) -> None:
         """Set task target pose from a robot configuration.
 
         Args:
             configuration: Robot configuration.
         """
-        self.set_target(configuration.get_transform_body_to_world(self.body))
+        self.set_target(configuration.get_transform_frame_to_world(self.body))
 
     def compute_error(self, configuration: Configuration) -> np.ndarray:
         r"""Compute body task error.
 
         Mathematically this error is a twist :math:`e(q) \in se(3)` expressed
         in the local frame (i.e., it is a bodytwist ). We map it to
         :math:`\mathbb{R}^6` using Pinocchio's convention (linear coordinates
@@ -175,104 +174,67 @@
             configuration: Robot configuration :math:`q`.
 
         Returns:
             Body task error :math:`e(q)`.
         """
         if self.transform_target_to_world is None:
             raise TargetNotSet(f"no target set for body {self.body}")
-        transform_body_to_world = configuration.get_transform_body_to_world(
+        transform_frame_to_world = configuration.get_transform_frame_to_world(
             self.body
         )
-        error_in_body: np.ndarray = body_minus(
+        error_in_frame: np.ndarray = body_minus(
             self.transform_target_to_world,
-            transform_body_to_world,
+            transform_frame_to_world,
         )
-        return error_in_body
+        return error_in_frame
 
     def compute_jacobian(self, configuration: Configuration) -> np.ndarray:
         r"""Compute the body task Jacobian.
 
         The task Jacobian :math:`J(q) \in \mathbb{R}^{6 \times n_v}` appears in
         the task dynamics:
 
         .. math::
 
             J(q) \Delta q = \alpha e(q)
 
         The derivation of the formula for this Jacobian is detailed in
-        [BodyTaskJacobian]_. See also :func:`Task.compute_jacobian` for more
+        [FrameTaskJacobian]_. See also :func:`Task.compute_jacobian` for more
         context on task Jacobians.
 
         Args:
             configuration: Robot configuration :math:`q`.
 
         Returns:
             Pair :math:`(J, \alpha e)` of Jacobian matrix and error vector,
             both expressed in the body frame.
         """
-        jacobian_in_body = configuration.get_body_jacobian(self.body)
+        jacobian_in_frame = configuration.get_frame_jacobian(self.body)
 
         # TODO(scaron): fix sign of error and box minus
         if self.transform_target_to_world is None:
             raise TargetNotSet(f"no target set for body {self.body}")
-        transform_body_to_world = configuration.get_transform_body_to_world(
+        transform_frame_to_world = configuration.get_transform_frame_to_world(
             self.body
         )
-        transform_body_to_target = (
-            self.transform_target_to_world.inverse() * transform_body_to_world
+        transform_frame_to_target = (
+            self.transform_target_to_world.inverse() * transform_frame_to_world
         )
-        J = pin.Jlog6(transform_body_to_target) @ jacobian_in_body
+        J = pin.Jlog6(transform_frame_to_target) @ jacobian_in_frame
         return J
 
-    def compute_qp_objective(
-        self, configuration: Configuration
-    ) -> Tuple[np.ndarray, np.ndarray]:
-        r"""Compute the matrix-vector pair :math:`(H, c)` of the QP objective.
-
-        This pair is such that the contribution of the task to the QP objective
-        of the IK is:
-
-        .. math::
-
-            \| J \Delta q - \alpha e \|_{W}^2
-            = \frac{1}{2} \Delta q^T H \Delta q + c^T q
-
-        The weight matrix :math:`W \in \mathbb{R}^{6 \times 6}` combines
-        position and orientation costs. The unit of the overall contribution is
-        :math:`[\mathrm{cost}]^2`. The configuration displacement
-        :math:`\Delta q` is the output of inverse kinematics (we divide it by
-        :math:`\Delta t` to get a commanded velocity).
-
-        Args:
-            configuration: Robot configuration :math:`q`.
-
-        Returns:
-            Pair :math:`(H(q), c(q))` of Hessian matrix and linear vector of
-            the QP objective.
-
-        See Also:
-            Levenberg-Marquardt damping is described in [Sugihara2011]_. The
-            dimensional analysis in this class is our own.
-        """
-        jacobian = self.compute_jacobian(configuration)
-        gain_error = self.gain * self.compute_error(configuration)
-        weight = np.diag(self.cost)  # [cost] * [twist]^{-1}
-        weighted_jacobian = weight @ jacobian  # [cost]
-        weighted_error = weight @ gain_error  # [cost]
-        mu = self.lm_damping * weighted_error @ weighted_error  # [cost]^2
-        eye_tg = configuration.tangent.eye
-        # Our Levenberg-Marquardt damping `mu * eye_tg` is isotropic in the
-        # robot's tangent space. If it helps we can add a tangent-space scaling
-        # to damp the floating base differently from joint angular velocities.
-        H = weighted_jacobian.T @ weighted_jacobian + mu * eye_tg
-        c = -weighted_error.T @ weighted_jacobian
-        return (H, c)
-
     def __repr__(self):
         """Human-readable representation of the task."""
+        orientation_cost = (
+            self.cost if isinstance(self.cost, float) else self.cost[3:6]
+        )
+        position_cost = (
+            self.cost if isinstance(self.cost, float) else self.cost[0:3]
+        )
         return (
-            f"BodyTask({self.body}, "
+            "FrameTask("
+            f"body={self.body}, "
             f"gain={self.gain}, "
-            f"orientation_cost={self.cost[3:6]}, "
-            f"position_cost={self.cost[0:3]}, "
-            f"target={self.transform_target_to_world})"
+            f"orientation_cost={orientation_cost}, "
+            f"position_cost={position_cost}, "
+            f"transform_target_to_world={self.transform_target_to_world})"
         )
```

### Comparing `pin-pink-0.9.0/pink/tasks/exceptions.py` & `pin-pink-1.0.0/pink/tasks/exceptions.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,9 +20,13 @@
 from ..exceptions import PinkError
 
 
 class TargetNotSet(PinkError):
     """Exception raised when attempting to compute with an unset target."""
 
 
+class TaskDefinitionError(PinkError):
+    """Exception raised when a task definition is ill-formed."""
+
+
 class TaskJacobianNotSet(PinkError):
     """Exception raised when attempting to compute without a task Jacobian."""
```

### Comparing `pin-pink-0.9.0/pink/tasks/linear_holonomic_task.py` & `pin-pink-1.0.0/pink/tasks/task.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,64 +11,75 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Linear holonomic task :math:`A q = b`."""
+"""All kinematic tasks derive from the :class:`Task` base class.
 
-from typing import Sequence, Tuple, Union
+The formalism used in this implementation is written down in `this note on
+task-based inverse kinematics
+<https://scaron.info/robotics/inverse-kinematics.html>`_. As of February 2022
+it hasn't been updated with the proper dimensional analysis, but the core
+concepts and notations are there.
+"""
+
+import abc
+from typing import Optional, Sequence, Tuple, Union
 
 import numpy as np
 
 from ..configuration import Configuration
-from .exceptions import TaskJacobianNotSet
-from .task import Task
 
 
-class LinearHolonomicTask(Task):
-    r"""Linear holonomic task :math:`A q = 0`.
+class Task(abc.ABC):
+    r"""Abstract base class for kinematic tasks.
 
     Attributes:
-        A: matrix that defines the task:
-
-            .. math::
-                e(q) = A q
-                \dot{e}(q) := A \dot{q}
-
-            where :math: `e(q) \in \mathbb{R}^{k}` is the quantity that the
-            task aims to drive to zero (:math:`k` is the dimension of the
-            task).
-        cost: joint angular error cost in
-            :math:`[\mathrm{cost}] / [\mathrm{rad}]`.
-
-    Note:
-        A linear holonomic task is typically used for a robot
-        that has mechanical constraint (e.g., closed loop kinematics).
-        Floating base coordinates are not affected by this task.
+        cost: cost vector with the same dimension as the error of the task. Its
+            units depends on the error as well.
+        gain: Task gain :math:`\alpha \in [0, 1]` for additional low-pass
+            filtering. Defaults to 1.0 (no filtering) for dead-beat control.
+        lm_damping: Unitless scale of the Levenberg-Marquardt (only when
+            the error is large) regularization term, which helps when
+            targets are unfeasible. Increase this value if the task is too
+            jerky under unfeasible targets, but beware that a larger
+            damping slows down the task.
     """
 
-    A: np.ndarray
-    cost: Union[float, Sequence[float]]
+    cost: Optional[Union[float, Sequence[float], np.ndarray]]
+    gain: float
+    lm_damping: float
 
     def __init__(
-        self, A: np.ndarray, cost: Union[float, Sequence[float]]
-    ) -> None:
+        self,
+        cost: Optional[Union[float, Sequence[float], np.ndarray]] = None,
+        gain: float = 1.0,
+        lm_damping: float = 0.0,
+    ):
         r"""Create task.
 
         Args:
-            A: Jacobian matrix of the task.
-            cost: joint angular error cost in
-                :math:`[\mathrm{cost}] / [\mathrm{rad}]`.
+            cost: cost vector with the same dimension as the error of the task.
+                Its units depends on the error as well.
+            gain: Task gain :math:`\alpha \in [0, 1]` for additional low-pass
+                filtering. Defaults to 1.0 (no filtering) for dead-beat
+                control.
+            lm_damping: Unitless scale of the Levenberg-Marquardt (only when
+                the error is large) regularization term, which helps when
+                targets are unfeasible. Increase this value if the task is too
+                jerky under unfeasible targets, but beware that too large a
+                damping can slow down the task.
         """
-        assert A.shape[0] == 1 if isinstance(cost, float) else len(cost)
-        self.A = A
         self.cost = cost
+        self.gain = gain
+        self.lm_damping = lm_damping
 
+    @abc.abstractmethod
     def compute_error(self, configuration: Configuration) -> np.ndarray:
         r"""Compute the task error function.
 
         The error function :math:`e(q) \in \mathbb{R}^{k}` is the quantity that
         the task aims to drive to zero (:math:`k` is the dimension of the
         task). It appears in the first-order task dynamics:
 
@@ -87,20 +98,16 @@
 
         Args:
             configuration: Robot configuration :math:`q`.
 
         Returns:
             Task error vector :math:`e(q)`.
         """
-        if self.A.shape[1] != configuration.model.nv:
-            raise TaskJacobianNotSet(
-                "task Jacobian dimension is not set properly"
-            )
-        return np.zeros(self.A.shape[0])
 
+    @abc.abstractmethod
     def compute_jacobian(self, configuration: Configuration) -> np.ndarray:
         r"""Compute the task Jacobian at a given configuration.
 
         The task Jacobian :math:`J(q) \in \mathbb{R}^{k \times n_v}` appears in
         the first-order task dynamics:
 
         .. math::
@@ -115,54 +122,70 @@
 
         Args:
             configuration: Robot configuration :math:`q`.
 
         Returns:
             Task Jacobian :math:`J(q)`.
         """
-        if self.A.shape[1] != configuration.model.nv:
-            raise TaskJacobianNotSet(
-                "task Jacobian dimension is not set properly"
-            )
-        return self.A
 
     def compute_qp_objective(
         self, configuration: Configuration
     ) -> Tuple[np.ndarray, np.ndarray]:
         r"""Compute the matrix-vector pair :math:`(H, c)` of the QP objective.
 
         This pair is such that the contribution of the task to the QP objective
         of the IK is:
 
         .. math::
 
-            \| J \Delta q - \alpha e \|_{W}^2
-            = \frac{1}{2} \Delta q^T H \Delta q + c^T q
+            \| J \Delta q - \alpha e \|_{W}^2 = \frac{1}{2} \Delta q^T H
+            \Delta q + c^T q
 
-        The weight matrix :math:`W \in \mathbb{R}^{n \times n}` weighs and
+        The weight matrix :math:`W \in \mathbb{R}^{k \times k}` weighs and
         normalizes task coordinates to the same unit. The unit of the overall
-        contribution is :math:`[\mathrm{cost}]^2`. The configuration
-        displacement :math:`\Delta q` is the output of inverse kinematics (we
-        divide it by :math:`\Delta t` to get a commanded velocity).
+        contribution is [cost]^2. The configuration displacement :math:`\Delta
+        q` is the output of inverse kinematics (we divide it by :math:`\Delta
+        t` to get a commanded velocity).
 
         Args:
-            configuration: Robot configuration.
+            configuration: Robot configuration :math:`q`.
 
         Returns:
-            Pair :math:`(H)` of Hessian matrix of the QP objective.
+            Pair :math:`(H(q), c(q))` of Hessian matrix and linear vector of
+            the QP objective.
+
+        See Also:
+            Levenberg-Marquardt damping is described in [Sugihara2011]_. The
+            dimensional analysis in this class is our own.
         """
         jacobian = self.compute_jacobian(configuration)
         gain_error = self.gain * self.compute_error(configuration)
-        weight = np.diag(
-            [self.cost] * jacobian.shape[0]
-            if isinstance(self.cost, float)
-            else self.cost
+
+        weight = (
+            np.eye(jacobian.shape[0])
+            if self.cost is None
+            else np.diag(
+                [self.cost] * jacobian.shape[0]
+                if isinstance(self.cost, float)
+                else self.cost
+            )
         )
-        weighted_jacobian = np.dot(weight, jacobian)  # [cost]
-        weighted_error = np.dot(weight, gain_error)  # [cost]
-        H = weighted_jacobian.T @ weighted_jacobian
+
+        weighted_jacobian = weight @ jacobian  # [cost]
+        weighted_error = weight @ gain_error  # [cost]
+        mu = self.lm_damping * weighted_error @ weighted_error  # [cost]^2
+        eye_tg = configuration.tangent.eye
+        # Our Levenberg-Marquardt damping `mu * eye_tg` is isotropic in the
+        # robot's tangent space. If it helps we can add a tangent-space scaling
+        # to damp the floating base differently from joint angular velocities.
+        H = weighted_jacobian.T @ weighted_jacobian + mu * eye_tg
         c = -weighted_error.T @ weighted_jacobian
         return (H, c)
 
     def __repr__(self):
         """Human-readable representation of the task."""
-        return f"LinearHolonomicTask(cost={self.cost}, gain={self.gain})"
+        return (
+            f"Task("
+            f"cost={self.cost}, "
+            f"gain={self.gain}, "
+            f"lm_damping={self.lm_damping})"
+        )
```

### Comparing `pin-pink-0.9.0/pink/tasks/posture_task.py` & `pin-pink-1.0.0/pink/tasks/posture_task.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Posture task implementation."""
 
-from typing import Optional, Tuple
+from typing import Optional
 
 import numpy as np
 import pinocchio as pin
 
 from ..configuration import Configuration
 from ..utils import get_root_joint_dim
 from .exceptions import TargetNotSet
@@ -31,39 +31,41 @@
 class PostureTask(Task):
     r"""Regulate joint angles to a desired posture.
 
     A posture is a vector of actuated joint angles. Floating base coordinates
     are not affected by this task.
 
     Attributes:
-        cost: joint angular error cost in
-            :math:`[\mathrm{cost}] / [\mathrm{rad}]`.
         target_q: Target vector in the configuration space.
 
     A posture task is typically used for regularization as it has a steady
     rank. For instance, when Upkie's legs are stretched and the Jacobian of its
     contact frames become singular, the posture task will drive the knees
     toward a preferred orientation.
     """
 
-    cost: float
     target_q: Optional[np.ndarray]
 
-    def __init__(self, cost: float) -> None:
+    def __init__(self, cost: float, lm_damping: float = 0.0) -> None:
         r"""Create task.
 
         Args:
-            cost: joint angular error cost in
-                :math:`[\mathrm{cost}] / [\mathrm{rad}]`.
+            cost: value used to cast joint angle differences to a homogeneous
+                cost, in :math:`[\mathrm{cost}] / [\mathrm{rad}]`.
+            lm_damping: Unitless scale of the Levenberg-Marquardt (only when
+                the error is large) regularization term, which helps when
+                targets are unfeasible. Increase this value if the task is too
+                jerky under unfeasible targets, but beware that too large a
+                damping can slow down the task.
 
         Note:
             We assume that the first seven coordinates of the configuration are
             for the floating base.
         """
-        self.cost = cost
+        super().__init__(cost=cost, lm_damping=lm_damping)
         self.target_q = None
 
     def set_target(self, target_q: np.ndarray) -> None:
         """Set target posture.
 
         Args:
             target_q: Target vector in the configuration space.
@@ -118,44 +120,15 @@
             Posture task Jacobian :math:`J(q)`.
         """
         if self.target_q is None:
             raise TargetNotSet("no posture target")
         _, nv = get_root_joint_dim(configuration.model)
         return configuration.tangent.eye[nv:, :]
 
-    def compute_qp_objective(
-        self, configuration: Configuration
-    ) -> Tuple[np.ndarray, np.ndarray]:
-        r"""Compute the matrix-vector pair :math:`(H, c)` of the QP objective.
-
-        This pair is such that the contribution of the task to the QP objective
-        of the IK is:
-
-        .. math::
-
-            \| J \Delta q - \alpha e \|_{W}^2
-            = \frac{1}{2} \Delta q^T H \Delta q + c^T q
-
-        The weight matrix :math:`W \in \mathbb{R}^{n \times n}` weighs and
-        normalizes task coordinates to the same unit. The unit of the overall
-        contribution is :math:`[\mathrm{cost}]^2`. The configuration
-        displacement :math:`\Delta q` is the output of inverse kinematics (we
-        divide it by :math:`\Delta t` to get a commanded velocity).
-
-        Args:
-            configuration: Robot configuration.
-
-        Returns:
-            Pair :math:`(H, c)` of Hessian matrix and linear vector of the QP
-            objective.
-        """
-        jacobian = self.compute_jacobian(configuration)
-        gain_error = self.gain * self.compute_error(configuration)
-        weighted_jacobian = self.cost * jacobian  # [cost]
-        weighted_error = self.cost * gain_error  # [cost]
-        H = weighted_jacobian.T @ weighted_jacobian
-        c = -weighted_error.T @ weighted_jacobian
-        return (H, c)
-
     def __repr__(self):
         """Human-readable representation of the task."""
-        return f"PostureTask(cost={self.cost}, gain={self.gain})"
+        return (
+            "PostureTask("
+            f"cost={self.cost}, "
+            f"gain={self.gain}, "
+            f"lm_damping={self.lm_damping})"
+        )
```

### Comparing `pin-pink-0.9.0/pink/tasks/utils.py` & `pin-pink-1.0.0/pink/tasks/utils.py`

 * *Files identical despite different names*

### Comparing `pin-pink-0.9.0/pink/utils.py` & `pin-pink-1.0.0/pink/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -80,15 +80,14 @@
         f"cannot find the joint index corresponding to joint {joint_name}"
     )
 
 
 class VectorSpace:
     """Wrapper to refer to a vector space and its characteristic matrices."""
 
-    __dim: int
     __eye: np.ndarray
     __ones: np.ndarray
     __zeros: np.ndarray
 
     def __init__(self, dim: int):
         """Create new vector space description.
 
@@ -97,25 +96,19 @@
         """
         eye = np.eye(dim)
         ones = np.ones(dim)
         zeros = np.zeros(dim)
         eye.setflags(write=False)
         ones.setflags(write=False)
         zeros.setflags(write=False)
-        self.__dim = dim
         self.__eye = eye
         self.__ones = ones
         self.__zeros = zeros
 
     @property
-    def dim(self) -> int:
-        """Dimension of the vector space."""
-        return self.__dim
-
-    @property
     def eye(self) -> np.ndarray:
         """Identity matrix from and to the vector space."""
         return self.__eye
 
     @property
     def ones(self) -> np.ndarray:
         """Vector full of ones, dimension of the space."""
```

### Comparing `pin-pink-0.9.0/pink/visualization.py` & `pin-pink-1.0.0/pink/visualization.py`

 * *Files identical despite different names*

### Comparing `pin-pink-0.9.0/pyproject.toml` & `pin-pink-1.0.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -8,31 +8,30 @@
 authors = [
     {name = "Stéphane Caron", email = "stephane.caron@normalesup.org"},
 ]
 maintainers = [
     {name = "Stéphane Caron", email = "stephane.caron@normalesup.org"},
 ]
 dynamic = ['version', 'description']
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Framework :: Robot Framework :: Library",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Topic :: Scientific/Engineering",
 ]
 dependencies = [
     "loop-rate-limiters >=0.1.0",
-    "numpy >=1.20.0",
+    "numpy >=1.19.0",
     "pin >=2.6.3",
     "qpsolvers >=2.5.0",
     "quadprog >=0.1.11",
 ]
 keywords = ["inverse", "kinematics", "pinocchio"]
 
 [project.urls]
```

### Comparing `pin-pink-0.9.0/tests/__init__.py` & `pin-pink-1.0.0/tests/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,10 +11,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""
-This file makes sure Python treats the test directory as a package.
-"""
+"""This file makes sure Python treats the test directory as a package."""
```

### Comparing `pin-pink-0.9.0/tests/test_body_task.py` & `pin-pink-1.0.0/tests/test_frame_task.py`

 * *Files 24% similar despite different names*

```diff
@@ -21,114 +21,129 @@
 
 import numpy as np
 import pinocchio as pin
 from qpsolvers import solve_qp
 from robot_descriptions.loaders.pinocchio import load_robot_description
 
 from pink import Configuration
-from pink.tasks import BodyTask, TargetNotSet
+from pink.tasks import FrameTask, TargetNotSet
+from pink.tasks.exceptions import TaskDefinitionError
 
 
-class TestBodyTask(unittest.TestCase):
-
-    """
-    Test consistency of the body task.
+class TestFrameTask(unittest.TestCase):
+    """Test consistency of the body task.
 
     Note:
         This fixture only tests the task itself. Integration tests with the IK
         are carried out in :class:`TestSolveIK`.
     """
 
     def setUp(self):
         """Prepare test fixture."""
         robot = load_robot_description(
             "jvrc_description", root_joint=pin.JointModelFreeFlyer()
         )
+        frame_name = "ee_frame"
+        joint_name = robot.model.names[-1]
+        parent_joint = robot.model.getJointId(joint_name)
+        parent_frame = robot.model.getFrameId(joint_name)
+        placement = pin.SE3.Identity()
+        robot.model.addFrame(
+            pin.Frame(
+                frame_name,
+                parent_joint,
+                parent_frame,
+                placement,
+                pin.FrameType.OP_FRAME,
+            )
+        )
+        robot.data = pin.Data(robot.model)
         self.configuration = Configuration(robot.model, robot.data, robot.q0)
 
     def test_set_target_from_configuration(self):
-        task = BodyTask("l_ankle", position_cost=1.0, orientation_cost=0.1)
+        """Read target after setting it to a known value."""
+        task = FrameTask("l_ankle", position_cost=1.0, orientation_cost=0.1)
         task.set_target_from_configuration(self.configuration)
         transform_ankle_to_world = (
-            self.configuration.get_transform_body_to_world("l_ankle")
+            self.configuration.get_transform_frame_to_world("l_ankle")
         )
         self.assertTrue(
             np.allclose(
                 transform_ankle_to_world, task.transform_target_to_world
             )
         )
 
     def test_task_repr(self):
         """String representation reports the task gain, costs and target."""
-        earflap_task = BodyTask(
+        earflap_task = FrameTask(
             "earflap", position_cost=1.0, orientation_cost=0.1
         )
         self.assertTrue("gain=" in repr(earflap_task))
         self.assertTrue("cost=" in repr(earflap_task))
-        self.assertTrue("target=" in repr(earflap_task))
+        self.assertTrue("transform_target_to_world=" in repr(earflap_task))
 
     def test_target_not_set(self):
         """Raise an exception when the target is not set."""
-        task = BodyTask("l_ankle", position_cost=1.0, orientation_cost=0.1)
+        task = FrameTask("l_ankle", position_cost=1.0, orientation_cost=0.1)
         with self.assertRaises(TargetNotSet):
             task.compute_error(self.configuration)
         with self.assertRaises(TargetNotSet):
             task.compute_jacobian(self.configuration)
 
     def test_target_set_properly(self):
         """Return target properly once it's set."""
-        task = BodyTask("l_ankle", position_cost=1.0, orientation_cost=0.1)
-        T = self.configuration.get_transform_body_to_world("l_ankle")
+        task = FrameTask("l_ankle", position_cost=1.0, orientation_cost=0.1)
+        T = self.configuration.get_transform_frame_to_world("l_ankle")
         task.set_target(T)
         self.assertIsNotNone(task.transform_target_to_world)
         if task.transform_target_to_world is not None:  # help mypy
             self.assertTrue(
                 np.allclose(
                     T.homogeneous,
                     task.transform_target_to_world.homogeneous,
                 )
             )
 
     def test_target_is_a_copy(self):
         """Target is saved as a copy, not a reference to the original."""
-        task = BodyTask("l_ankle", position_cost=1.0, orientation_cost=0.1)
-        target = self.configuration.get_transform_body_to_world("l_ankle")
+        task = FrameTask("l_ankle", position_cost=1.0, orientation_cost=0.1)
+        target = self.configuration.get_transform_frame_to_world("l_ankle")
         task.set_target(target)
         y = target.translation[1]
         target.translation[1] += 12.0
         if task.transform_target_to_world is not None:  # help mypy
             self.assertAlmostEqual(
                 task.transform_target_to_world.translation[1], y
             )
             self.assertNotAlmostEqual(
                 task.transform_target_to_world.translation[1],
                 target.translation[1],
             )
 
     def test_zero_error_when_target_at_body(self):
         """Error is zero when the target and body are at the same location."""
-        task = BodyTask("r_ankle", position_cost=1.0, orientation_cost=0.1)
-        target = self.configuration.get_transform_body_to_world("r_ankle")
+        task = FrameTask("r_ankle", position_cost=1.0, orientation_cost=0.1)
+        target = self.configuration.get_transform_frame_to_world("r_ankle")
         task.set_target(target)  # error == 0
         J = task.compute_jacobian(self.configuration)
         e = task.compute_error(self.configuration)
         self.assertTrue(
-            np.allclose(J, self.configuration.get_body_jacobian("r_ankle"))
+            np.allclose(J, self.configuration.get_frame_jacobian("r_ankle"))
         )
         self.assertLess(np.linalg.norm(e), 1e-10)
 
     def test_unit_cost_qp_objective(self):
         """Unit cost means the QP objective is exactly (J^T J, -e^T J)."""
-        task = BodyTask("r_wrist", position_cost=1.0, orientation_cost=0.1)
-        transform_target_to_body = pin.SE3(
+        task = FrameTask("r_wrist", position_cost=1.0, orientation_cost=0.1)
+        transform_target_to_frame = pin.SE3(
             np.eye(3), np.array([0.0, 0.01, 0.0])
         )
         target = (
-            self.configuration.get_transform_body_to_world("r_wrist")
-            * transform_target_to_body
+            self.configuration.get_transform_frame_to_world("r_wrist")
+            * transform_target_to_frame
         )
         task.set_target(target)
         J = task.compute_jacobian(self.configuration)
         e = task.compute_error(self.configuration)
         task.set_position_cost(1.0)
         task.set_orientation_cost(1.0)
         task.lm_damping = 0.0
@@ -138,21 +153,21 @@
 
     def test_zero_costs_same_as_disabling_lines(self):
         """Setting a position or orientation cost to zero.
 
         A zero yields the same QP objective as disabling the corresponding
         Jacobian and error coordinates.
         """
-        task = BodyTask("l_wrist", position_cost=1.0, orientation_cost=0.1)
-        transform_target_to_body = pin.SE3(
+        task = FrameTask("l_wrist", position_cost=1.0, orientation_cost=0.1)
+        transform_target_to_frame = pin.SE3(
             np.eye(3), np.array([0.1, 0.02, 0.01])
         )
         target = (
-            self.configuration.get_transform_body_to_world("l_wrist")
-            * transform_target_to_body
+            self.configuration.get_transform_frame_to_world("l_wrist")
+            * transform_target_to_frame
         )
         task.set_target(target)
         J = task.compute_jacobian(self.configuration)
         e = task.compute_error(self.configuration)
         qd = np.random.random(J.shape[1:])
         test_cases = {
             "position_only": (1.0, 0.0, slice(0, 3)),
@@ -174,38 +189,59 @@
             c_check = -e[indexes].T @ J[indexes]
             cost = qd.T @ H @ qd + c @ qd
             cost_check = qd.T @ H_check @ qd + c_check @ qd
             self.assertAlmostEqual(cost, cost_check)
 
     def test_lm_damping_has_no_effect_at_target(self):
         """Levenberg-Marquardt damping has no effect when the error is zero."""
-        task = BodyTask("l_wrist", position_cost=1.0, orientation_cost=0.1)
-        target = self.configuration.get_transform_body_to_world("l_wrist")
+        task = FrameTask("l_wrist", position_cost=1.0, orientation_cost=0.1)
+        target = self.configuration.get_transform_frame_to_world("l_wrist")
         task.set_target(target)
         task.lm_damping = 1e-8
         H_1, c_1 = task.compute_qp_objective(self.configuration)
         task.lm_damping = 1e-4
         H_2, c_2 = task.compute_qp_objective(self.configuration)
         self.assertTrue(np.allclose(H_1, H_2))
         self.assertTrue(np.allclose(c_1, c_2))
 
     def test_lm_damping_has_effect_under_error(self):
         """Levenberg-Marquardt damping is indeed a damping.
 
         That is, unless the task is fulfilled, it reduces velocities.
         """
-        task = BodyTask("r_wrist", position_cost=1.0, orientation_cost=0.1)
-        transform_target_to_body = pin.SE3(
+        task = FrameTask("r_wrist", position_cost=1.0, orientation_cost=0.1)
+        transform_target_to_frame = pin.SE3(
             np.eye(3), np.array([0.0, 2.0, 0.0])
         )
         target = (
-            self.configuration.get_transform_body_to_world("r_wrist")
-            * transform_target_to_body
+            self.configuration.get_transform_frame_to_world("r_wrist")
+            * transform_target_to_frame
         )
         task.set_target(target)
         task.lm_damping = 1e-8
         H_1, c_1 = task.compute_qp_objective(self.configuration)
         task.lm_damping = 1e-4
         H_2, c_2 = task.compute_qp_objective(self.configuration)
         qd_1 = solve_qp(H_1, c_1, solver="quadprog")  # H_1 p.s.d. (LM damping)
         qd_2 = solve_qp(H_2, c_2, solver="quadprog")  # idem for H_2
         self.assertGreater(np.linalg.norm(qd_2 - qd_1), 1e-6)
+
+    def test_task_on_user_added_op_frame(self):
+        """Error is zero when the target and body are at the same location."""
+        task = FrameTask("ee_frame", [1.0, 1.0, 1.0], [1.0, 1.0, 1.0])
+        target = self.configuration.get_transform_frame_to_world("ee_frame")
+        task.set_target(target)  # error == 0
+        J = task.compute_jacobian(self.configuration)
+        e = task.compute_error(self.configuration)
+        self.assertTrue(
+            np.allclose(J, self.configuration.get_frame_jacobian("ee_frame"))
+        )
+        self.assertLess(np.linalg.norm(e), 1e-10)
+
+    def test_inconsistent_cost(self):
+        """Exception when the cost is not a vector any more."""
+        task = FrameTask("ee_frame", [1.0, 1.0, 1.0], [1.0, 1.0, 1.0])
+        task.cost = 42.0
+        with self.assertRaises(TaskDefinitionError):
+            task.set_position_cost(1.0)
+        with self.assertRaises(TaskDefinitionError):
+            task.set_orientation_cost(1.0)
```

### Comparing `pin-pink-0.9.0/tests/test_configuration.py` & `pin-pink-1.0.0/tests/test_configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,16 @@
 from robot_descriptions.loaders.pinocchio import load_robot_description
 
 from pink import Configuration
 from pink.exceptions import BodyNotFound, NotWithinConfigurationLimits
 
 
 class TestConfiguration(unittest.TestCase):
+    """Test configuration type."""
+
     def test_constructor(self):
         """Constructing a configuration computes Jacobians."""
         robot = load_robot_description(
             "jvrc_description", root_joint=pin.JointModelFreeFlyer()
         )
         robot.data.J.fill(42.0)
         configuration = Configuration(robot.model, robot.data, robot.q0)
@@ -389,15 +391,15 @@
 
     def test_transform_found(self):
         """Return the pose of an existing robot body."""
         robot = load_robot_description(
             "jvrc_description", root_joint=pin.JointModelFreeFlyer()
         )
         configuration = Configuration(robot.model, robot.data, robot.q0)
-        transform_pelvis_to_world = configuration.get_transform_body_to_world(
+        transform_pelvis_to_world = configuration.get_transform_frame_to_world(
             "PELVIS_S"
         )
         self.assertTrue(
             np.allclose(
                 transform_pelvis_to_world.np[3, :],
                 np.array([0.0, 0.0, 0.0, 1.0]),
             )
@@ -406,15 +408,15 @@
     def test_transform_not_found(self):
         """Raise an error when the request robot body is not found."""
         robot = load_robot_description(
             "jvrc_description", root_joint=pin.JointModelFreeFlyer()
         )
         configuration = Configuration(robot.model, robot.data, robot.q0)
         with self.assertRaises(KeyError):
-            configuration.get_transform_body_to_world("foo")
+            configuration.get_transform_frame_to_world("foo")
 
     def test_check_limits(self):
         """Raise an error if and only if a joint limit is exceened."""
         robot = load_robot_description(
             "jvrc_description", root_joint=pin.JointModelFreeFlyer()
         )
         q = robot.q0
@@ -461,22 +463,23 @@
         robot = load_robot_description(
             "jvrc_description", root_joint=pin.JointModelFreeFlyer()
         )
         configuration = Configuration(robot.model, robot.data, robot.q0)
         self.assertAlmostEqual(np.sum(configuration.tangent.zeros), 0.0)
         self.assertEqual(len(configuration.tangent.zeros), robot.model.nv)
 
-    def test_body_jacobian_not_found(self):
+    def test_frame_jacobian_not_found(self):
         """Querying a body that does not exist raises a ValueError."""
         robot = load_robot_description(
             "jvrc_description", root_joint=pin.JointModelFreeFlyer()
         )
         configuration = Configuration(robot.model, robot.data, robot.q0)
         with self.assertRaises(BodyNotFound):
-            configuration.get_body_jacobian("does_not_exist")
+            configuration.get_frame_jacobian("does_not_exist")
 
     def test_get_integrate_inplace(self):
+        """Test in-place integration."""
         robot = load_robot_description("sigmaban_description", root_joint=None)
         configuration = Configuration(robot.model, robot.data, robot.q0)
         velocity = robot.model.tangent.ones
         configuration.integrate_inplace(velocity, dt=1e-3)
         self.assertGreater(np.linalg.norm(configuration.q - robot.q0), 2e-3)
```

### Comparing `pin-pink-0.9.0/tests/test_joint_coupling_task.py` & `pin-pink-1.0.0/tests/test_joint_coupling_task.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,43 +41,42 @@
             "draco3_description", root_joint=pin.JointModelFreeFlyer()
         )
         self.configuration = Configuration(robot.model, robot.data, robot.q0)
 
     def test_task_repr(self):
         """String representation reports the task gain, costs and target."""
         task = JointCouplingTask(
-            joint_name_list=["r_knee_fe_jp", "r_knee_fe_jd"],
+            joint_names=["r_knee_fe_jp", "r_knee_fe_jd"],
             ratios=[1.0, -1.0],
             cost=1.0,
             configuration=self.configuration,
         )
         self.assertTrue("cost=" in repr(task))
         self.assertTrue("gain=" in repr(task))
 
     def test_unit_cost_qp_objective(self):
         """A unit cost vector means the QP objective is (J^T J, -e^T J)."""
         task = JointCouplingTask(
-            joint_name_list=["r_knee_fe_jp", "r_knee_fe_jd"],
+            joint_names=["r_knee_fe_jp", "r_knee_fe_jd"],
             ratios=[1.0, -1.0],
             cost=1.0,
             configuration=self.configuration,
         )
         e = task.compute_error(self.configuration)
         J = task.compute_jacobian(self.configuration)
         H, c = task.compute_qp_objective(self.configuration)
         self.assertTrue(np.allclose(J.T @ J, H))
         self.assertTrue(np.allclose(-e.T @ J, c))
 
     def test_zero_cost_same_as_disabling_task(self):
         """The task has no effect when its cost is zero."""
         task = JointCouplingTask(
-            joint_name_list=["r_knee_fe_jp", "r_knee_fe_jd"],
+            joint_names=["r_knee_fe_jp", "r_knee_fe_jd"],
             ratios=[1.0, -1.0],
             cost=0.0,
             configuration=self.configuration,
         )
         J = task.compute_jacobian(self.configuration)
-        e = task.compute_error(self.configuration)
         H, c = task.compute_qp_objective(self.configuration)
         qd = np.random.random(J.shape[1:])
         cost = qd.T @ H @ qd + c @ qd
         self.assertAlmostEqual(cost, 0.0)
```

### Comparing `pin-pink-0.9.0/tests/test_linear_holonomic_task.py` & `pin-pink-1.0.0/tests/test_linear_holonomic_task.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 
 import numpy as np
 import pinocchio as pin
 from robot_descriptions.loaders.pinocchio import load_robot_description
 
 from pink import Configuration
 from pink.tasks import LinearHolonomicTask, TaskJacobianNotSet
+from pink.tasks.exceptions import TaskDefinitionError
 from pink.utils import get_joint_idx
 
 
 class TestLinearHolonomicTask(unittest.TestCase):
     """Test consistency of the linear holonomic task.
 
     Note:
@@ -39,33 +40,38 @@
     def setUp(self):
         """Prepare test fixture."""
         robot = load_robot_description(
             "draco3_description", root_joint=pin.JointModelFreeFlyer()
         )
         self.configuration = Configuration(robot.model, robot.data, robot.q0)
 
+    def test_inconsistent_definition(self):
+        """Exception when the task is not defined properly."""
+        with self.assertRaises(TaskDefinitionError):
+            LinearHolonomicTask(A=np.ones((3, 4)), b=np.ones(5), q_0=None)
+
     def test_task_repr(self):
         """String representation reports the task gain, costs and target."""
         A = np.zeros((1, self.configuration.model.nv))
         _, r_knee_fe_jp_v_idx = get_joint_idx(
             self.configuration.model, "r_knee_fe_jp"
         )
         _, r_knee_fe_jd_v_idx = get_joint_idx(
             self.configuration.model, "r_knee_fe_jd"
         )
         A[:, r_knee_fe_jp_v_idx] = 1.0
         A[:, r_knee_fe_jd_v_idx] = -1.0
-        task = LinearHolonomicTask(A=A, cost=1.0)
+        task = LinearHolonomicTask(A=A, b=np.zeros(1), q_0=None, cost=1.0)
         self.assertTrue("cost=" in repr(task))
         self.assertTrue("gain=" in repr(task))
 
     def test_jacobian_not_set_properly(self):
         """Raise an exception when the task Jacobian is not set properly."""
         A = np.zeros((1, self.configuration.model.nq))
-        task = LinearHolonomicTask(A=A, cost=1.0)
+        task = LinearHolonomicTask(A=A, b=np.zeros(1), q_0=None, cost=1.0)
         with self.assertRaises(TaskJacobianNotSet):
             task.compute_error(self.configuration)
         with self.assertRaises(TaskJacobianNotSet):
             task.compute_jacobian(self.configuration)
 
     def test_unit_cost_qp_objective(self):
         """A unit cost vector means the QP objective is (J^T J, -e^T J)."""
@@ -82,15 +88,17 @@
             self.configuration.model, "l_knee_fe_jp"
         )
         _, l_knee_fe_jd_v_idx = get_joint_idx(
             self.configuration.model, "l_knee_fe_jd"
         )
         A[:, l_knee_fe_jp_v_idx] = 1.0
         A[:, l_knee_fe_jd_v_idx] = -1.0
-        task = LinearHolonomicTask(A=A, cost=[1.0, 1.0])
+        task = LinearHolonomicTask(
+            A=A, b=np.zeros(2), q_0=None, cost=[1.0, 1.0]
+        )
         e = task.compute_error(self.configuration)
         J = task.compute_jacobian(self.configuration)
         H, c = task.compute_qp_objective(self.configuration)
         self.assertTrue(np.allclose(J.T @ J, H))
         self.assertTrue(np.allclose(-e.T @ J, c))
 
     def test_zero_cost_same_as_disabling_task(self):
@@ -108,14 +116,15 @@
             self.configuration.model, "l_knee_fe_jp"
         )
         _, l_knee_fe_jd_v_idx = get_joint_idx(
             self.configuration.model, "l_knee_fe_jd"
         )
         A[:, l_knee_fe_jp_v_idx] = 1.0
         A[:, l_knee_fe_jd_v_idx] = -1.0
-        task = LinearHolonomicTask(A=A, cost=[0.0, 0.0])
+        task = LinearHolonomicTask(
+            A=A, b=np.zeros(2), q_0=None, cost=[0.0, 0.0]
+        )
         J = task.compute_jacobian(self.configuration)
-        e = task.compute_error(self.configuration)
         H, c = task.compute_qp_objective(self.configuration)
         qd = np.random.random(J.shape[1:])
         cost = qd.T @ H @ qd + c @ qd
         self.assertAlmostEqual(cost, 0.0)
```

### Comparing `pin-pink-0.9.0/tests/test_posture_task.py` & `pin-pink-1.0.0/tests/test_posture_task.py`

 * *Files 13% similar despite different names*

```diff
@@ -53,14 +53,15 @@
         task = PostureTask(cost=1.0)
         with self.assertRaises(TargetNotSet):
             task.compute_error(self.configuration)
         with self.assertRaises(TargetNotSet):
             task.compute_jacobian(self.configuration)
 
     def test_set_target_from_configuration(self):
+        """Check that target is set from its configuration value."""
         task = PostureTask(cost=1.0)
         task.set_target_from_configuration(self.configuration)
         self.assertTrue(np.allclose(self.configuration.q, task.target_q))
 
     def test_target_set_properly(self):
         """Return target properly once it's set."""
         task = PostureTask(cost=1.0)
@@ -102,12 +103,11 @@
 
     def test_zero_cost_same_as_disabling_task(self):
         """The task has no effect when its cost is zero."""
         task = PostureTask(cost=0.0)
         q = self.configuration.q
         task.set_target(q)
         J = task.compute_jacobian(self.configuration)
-        e = task.compute_error(self.configuration)
         H, c = task.compute_qp_objective(self.configuration)
         qd = np.random.random(J.shape[1:])
         cost = qd.T @ H @ qd + c @ qd
         self.assertAlmostEqual(cost, 0.0)
```

### Comparing `pin-pink-0.9.0/tests/test_solve_ik.py` & `pin-pink-1.0.0/tests/test_solve_ik.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,19 +23,18 @@
 import pinocchio as pin
 import qpsolvers
 from numpy.linalg import norm
 from robot_descriptions.loaders.pinocchio import load_robot_description
 
 from pink import Configuration, build_ik, solve_ik
 from pink.exceptions import NotWithinConfigurationLimits
-from pink.tasks import BodyTask
+from pink.tasks import FrameTask
 
 
 class TestSolveIK(unittest.TestCase):
-
     """Test fixture for the solve_ik function."""
 
     def test_checks_configuration_limits(self):
         """IK checks for configuration limits."""
         robot = load_robot_description(
             "upkie_description", root_joint=pin.JointModelFreeFlyer()
         )
@@ -69,33 +68,33 @@
 
     def test_single_task_fulfilled(self):
         """Velocity is zero when the only task is already fulfilled."""
         robot = load_robot_description(
             "upkie_description", root_joint=pin.JointModelFreeFlyer()
         )
         configuration = Configuration(robot.model, robot.data, robot.q0)
-        task = BodyTask(
+        task = FrameTask(
             "left_contact", position_cost=1.0, orientation_cost=1.0
         )
         task.set_target(
-            configuration.get_transform_body_to_world("left_contact")
+            configuration.get_transform_frame_to_world("left_contact")
         )
         velocity = solve_ik(configuration, [task], dt=5e-3, solver="quadprog")
         self.assertTrue(np.allclose(velocity, 0.0))
 
     def test_single_task_convergence(self):
         """Integrating velocities makes a task converge to its target."""
         robot = load_robot_description(
             "upkie_description", root_joint=pin.JointModelFreeFlyer()
         )
         configuration = Configuration(robot.model, robot.data, robot.q0)
-        task = BodyTask(
+        task = FrameTask(
             "left_contact", position_cost=1.0, orientation_cost=1.0
         )
-        transform_init_to_world = configuration.get_transform_body_to_world(
+        transform_init_to_world = configuration.get_transform_frame_to_world(
             "left_contact"
         )
         transform_target_to_init = pin.SE3(
             np.eye(3), np.array([0.0, 0.0, 0.1])
         )
         transform_target_to_world = (
             transform_init_to_world * transform_target_to_init
@@ -104,17 +103,17 @@
         dt = 5e-3  # [s]
         velocity = solve_ik(configuration, [task], dt, solver="quadprog")
 
         # Initially we are nowhere near the target and moving
         self.assertFalse(np.allclose(velocity, 0.0))
         self.assertAlmostEqual(norm(task.compute_error(configuration)), 0.1)
         self.assertFalse(
-            configuration.get_transform_body_to_world("left_contact").isApprox(
-                transform_target_to_world, prec=1e-4
-            )
+            configuration.get_transform_frame_to_world(
+                "left_contact"
+            ).isApprox(transform_target_to_world, prec=1e-4)
         )
 
         last_error = 1e6
         for nb_steps in range(42):
             error = norm(task.compute_error(configuration))
             if error < 1e-6 and np.allclose(velocity, 0.0):
                 break
@@ -124,30 +123,30 @@
             configuration = Configuration(robot.model, robot.data, q)
             velocity = solve_ik(configuration, [task], dt, solver="quadprog")
 
         # After nb_steps we are at the target and not moving
         self.assertTrue(np.allclose(velocity, 0.0))
         self.assertAlmostEqual(norm(task.compute_error(configuration)), 0.0)
         self.assertTrue(
-            configuration.get_transform_body_to_world("left_contact").isApprox(
-                transform_target_to_world, prec=1e-8
-            )
+            configuration.get_transform_frame_to_world(
+                "left_contact"
+            ).isApprox(transform_target_to_world, prec=1e-8)
         )
         self.assertLess(nb_steps, 3)
 
     def test_single_task_translation(self):
         """Translating a target yields a pure linear velocity."""
         robot = load_robot_description(
             "upkie_description", root_joint=pin.JointModelFreeFlyer()
         )
         configuration = Configuration(robot.model, robot.data, robot.q0)
-        contact_task = BodyTask(
+        contact_task = FrameTask(
             "right_contact", position_cost=1.0, orientation_cost=1.0
         )
-        transform_target_to_world = configuration.get_transform_body_to_world(
+        transform_target_to_world = configuration.get_transform_frame_to_world(
             "right_contact"
         ).copy()
         self.assertTrue(
             np.allclose(transform_target_to_world.rotation, np.eye(3)),
             "default orientation should be aligned with the world frame",
         )
         transform_target_to_world.translation[1] -= 0.1
@@ -156,15 +155,15 @@
         velocity = solve_ik(
             configuration,
             [contact_task],
             dt=1e-3,
             damping=1e-12,
             solver="quadprog",
         )
-        jacobian_contact_in_contact = configuration.get_body_jacobian(
+        jacobian_contact_in_contact = configuration.get_frame_jacobian(
             "right_contact"
         )
         velocity_contact_in_contact = jacobian_contact_in_contact @ velocity
         linear_velocity_contact_in_contact = velocity_contact_in_contact[0:3]
         angular_velocity_contact_in_contact = velocity_contact_in_contact[3:6]
         self.assertTrue(np.allclose(angular_velocity_contact_in_contact, 0.0))
         self.assertAlmostEqual(linear_velocity_contact_in_contact[0], 0.0)
@@ -173,117 +172,114 @@
 
     def test_three_tasks_fulfilled(self):
         """No motion when all targets are reached."""
         robot = load_robot_description(
             "jvrc_description", root_joint=pin.JointModelFreeFlyer()
         )
         configuration = Configuration(robot.model, robot.data, robot.q0)
-        left_ankle_task = BodyTask(
+        left_ankle_task = FrameTask(
             "l_ankle", position_cost=1.0, orientation_cost=3.0
         )
-        right_ankle_task = BodyTask(
+        right_ankle_task = FrameTask(
             "r_ankle", position_cost=1.0, orientation_cost=3.0
         )
-        pelvis_task = BodyTask(
+        pelvis_task = FrameTask(
             "PELVIS_S", position_cost=1.0, orientation_cost=3.0
         )
 
         left_ankle_task.set_target(
-            configuration.get_transform_body_to_world("l_ankle")
+            configuration.get_transform_frame_to_world("l_ankle")
         )
         right_ankle_task.set_target(
-            configuration.get_transform_body_to_world("r_ankle")
+            configuration.get_transform_frame_to_world("r_ankle")
         )
         pelvis_task.set_target(
-            configuration.get_transform_body_to_world("PELVIS_S")
+            configuration.get_transform_frame_to_world("PELVIS_S")
         )
 
         tasks = [pelvis_task, left_ankle_task, right_ankle_task]
         velocity = solve_ik(configuration, tasks, dt=5e-3, solver="quadprog")
         self.assertTrue(np.allclose(velocity, 0.0))
 
     def test_three_tasks_convergence(self):
         """Three simultaneously feasible tasks on the JVRC model converge."""
         robot = load_robot_description(
             "jvrc_description", root_joint=pin.JointModelFreeFlyer()
         )
         configuration = Configuration(robot.model, robot.data, robot.q0)
 
         # Define tasks
-        left_ankle_task = BodyTask(
+        left_ankle_task = FrameTask(
             "l_ankle", position_cost=1.0, orientation_cost=3.0
         )
-        right_ankle_task = BodyTask(
+        right_ankle_task = FrameTask(
             "r_ankle", position_cost=1.0, orientation_cost=3.0
         )
-        pelvis_task = BodyTask(
+        pelvis_task = FrameTask(
             "PELVIS_S", position_cost=1.0, orientation_cost=0.0
         )
         tasks = [pelvis_task, left_ankle_task, right_ankle_task]
 
         # Set task targets
         transform_l_ankle_target_to_init = pin.SE3(
             np.eye(3), np.array([0.1, 0.0, 0.0])
         )
         transform_r_ankle_target_to_init = pin.SE3(
             np.eye(3), np.array([-0.1, 0.0, 0.0])
         )
         left_ankle_task.set_target(
-            configuration.get_transform_body_to_world("l_ankle")
+            configuration.get_transform_frame_to_world("l_ankle")
             * transform_l_ankle_target_to_init
         )
         right_ankle_task.set_target(
-            configuration.get_transform_body_to_world("r_ankle")
+            configuration.get_transform_frame_to_world("r_ankle")
             * transform_r_ankle_target_to_init
         )
         pelvis_task.set_target(
-            configuration.get_transform_body_to_world("PELVIS_S")
+            configuration.get_transform_frame_to_world("PELVIS_S")
         )
 
         # Run IK in closed loop
         dt = 4e-3  # [s]
         for nb_iter in range(42):
             velocity = solve_ik(configuration, tasks, dt, solver="quadprog")
             if norm(velocity) < 1e-10:
                 break
             q = configuration.integrate(velocity, dt)
             configuration = Configuration(robot.model, robot.data, q)
         self.assertLess(nb_iter, 42)
         self.assertLess(norm(velocity), 1e-10)
         self.assertLess(
-            max(
-                norm(task.compute_error(configuration))
-                for task in tasks
-            ),
+            max(norm(task.compute_error(configuration)) for task in tasks),
             0.5,
         )
 
     def get_jvrc_problem(self):
         """Get an IK problem with three tasks on a humanoid model."""
         robot = load_robot_description(
             "jvrc_description", root_joint=pin.JointModelFreeFlyer()
         )
         configuration = Configuration(robot.model, robot.data, robot.q0)
-        left_ankle_task = BodyTask(
+        left_ankle_task = FrameTask(
             "l_ankle", position_cost=1.0, orientation_cost=3.0
         )
-        right_ankle_task = BodyTask(
+        right_ankle_task = FrameTask(
             "r_ankle", position_cost=1.0, orientation_cost=3.0
         )
-        pelvis_task = BodyTask(
+        pelvis_task = FrameTask(
             "PELVIS_S", position_cost=1.0, orientation_cost=3.0
         )
         left_ankle_task.set_target(
-            configuration.get_transform_body_to_world("l_ankle")
+            configuration.get_transform_frame_to_world("l_ankle")
         )
         right_ankle_task.set_target(
-            configuration.get_transform_body_to_world("r_ankle")
+            configuration.get_transform_frame_to_world("r_ankle")
         )
         pelvis_task.set_target(
-            configuration.get_transform_body_to_world("PELVIS_S")
+            configuration.get_transform_frame_to_world("PELVIS_S")
         )
         tasks = [pelvis_task, left_ankle_task, right_ankle_task]
         dt = 5e-3
         return configuration, tasks, dt
 
     @staticmethod
     def get_solver_test(solver: str):
```

### Comparing `pin-pink-0.9.0/tests/test_task.py` & `pin-pink-1.0.0/tests/test_task.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,29 +11,25 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""
-Test base class for kinematic tasks.
-"""
+"""Test base class for kinematic tasks."""
 
 import unittest
 
 from pink.tasks import Task
 
 
 class TestTask(unittest.TestCase):
+    """Test abstract base class for tasks."""
+
     def setUp(self):
-        """
-        Prepare test fixture.
-        """
+        """Prepare test fixture."""
         Task.__abstractmethods__ = set()  # allow instantiation
 
     def test_task_repr(self):
-        """
-        String representation reports the task gain.
-        """
+        """String representation reports the task gain."""
         task = Task()
         self.assertTrue("gain=" in repr(task))
```

### Comparing `pin-pink-0.9.0/tests/test_utils.py` & `pin-pink-1.0.0/tests/test_utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -18,20 +18,23 @@
 
 """Test fixture for other library features."""
 
 import unittest
 
 import numpy as np
 import pinocchio as pin
-from pink.tasks.utils import body_minus, spatial_minus
-from pink.utils import custom_configuration_vector
 from robot_descriptions.loaders.pinocchio import load_robot_description
 
+from pink.tasks.utils import body_minus, spatial_minus
+from pink.utils import VectorSpace, custom_configuration_vector
+
 
 class TestUtils(unittest.TestCase):
+    """Test utility classes and functions."""
+
     def test_custom_configuration_vector(self):
         """Check a custom configuration vector for Upkie.
 
         Assumes the left and right knees have joint indices respectively 8 and
         11 in the configuration vector.
         """
         robot = load_robot_description(
@@ -43,7 +46,18 @@
 
     def test_minus(self):
         """Test Lie minus operators."""
         X = pin.SE3.Random()
         Y = pin.SE3.Random()
         self.assertTrue(np.allclose(Y, X * pin.exp6(body_minus(Y, X))))
         self.assertTrue(np.allclose(Y, pin.exp6(spatial_minus(Y, X)) * X))
+
+    def test_vector_space(self):
+        """Check dimensions of regular tangent space."""
+        robot = load_robot_description(
+            "upkie_description", root_joint=pin.JointModelFreeFlyer()
+        )
+        nv = robot.model.nv
+        tangent = VectorSpace(robot.model.nv)
+        self.assertEqual(tangent.eye.shape, (nv, nv))
+        self.assertEqual(tangent.ones.shape, (nv,))
+        self.assertEqual(tangent.zeros.shape, (nv,))
```

### Comparing `pin-pink-0.9.0/tox.ini` & `pin-pink-1.0.0/tox.ini`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 [tox]
 isolated_build = True
-envlist = py{37, 38, 39, 310}
+envlist = py{38, 39, 310}
 
 [gh-actions]
 python =
-    3.7: py37
     3.8: py38
     3.9: py39
     3.10: py310
 
 [testenv]
 deps =
     numpy
```

### Comparing `pin-pink-0.9.0/PKG-INFO` & `pin-pink-1.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,56 +1,53 @@
 Metadata-Version: 2.1
 Name: pin-pink
-Version: 0.9.0
+Version: 1.0.0
 Summary: Python inverse kinematics for your robot model based on Pinocchio.
 Keywords: inverse,kinematics,pinocchio
 Author-email: Stéphane Caron <stephane.caron@normalesup.org>
 Maintainer-email: Stéphane Caron <stephane.caron@normalesup.org>
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Robot Framework :: Library
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering
 Requires-Dist: loop-rate-limiters >=0.1.0
-Requires-Dist: numpy >=1.20.0
+Requires-Dist: numpy >=1.19.0
 Requires-Dist: pin >=2.6.3
 Requires-Dist: qpsolvers >=2.5.0
 Requires-Dist: quadprog >=0.1.11
 Project-URL: Changelog, https://github.com/tasts-robots/pink/blob/master/CHANGELOG.md
 Project-URL: Documentation, https://tasts-robots.org/doc/pink/
 Project-URL: Source, https://github.com/tasts-robots/pink
 Project-URL: Tracker, https://github.com/tasts-robots/pink/issues
 
 # Pink
 
 <img src="https://user-images.githubusercontent.com/1189580/172797197-9aa46561-cfaa-4046-bd60-f681d85b055d.png" align="right" height=140>
 
 [![Build](https://img.shields.io/github/actions/workflow/status/tasts-robots/pink/main.yml?branch=master)](https://github.com/tasts-robots/pink/actions)
 [![Coverage](https://coveralls.io/repos/github/tasts-robots/pink/badge.svg?branch=master)](https://coveralls.io/github/tasts-robots/pink?branch=master)
-[![Documentation](https://img.shields.io/badge/docs-online-brightgreen?style=flat)](https://tasts-robots.org/doc/pink/)
+[![Documentation](https://img.shields.io/badge/docs-online-brightgreen?logo=read-the-docs&style=flat)](https://tasts-robots.org/doc/pink/)
 [![PyPI version](https://img.shields.io/pypi/v/pin-pink)](https://pypi.org/project/pin-pink/)
 
 **P**ython **in**verse **k**inematics for articulated robot models, based on [Pinocchio](https://github.com/stack-of-tasks/pinocchio).
 
 ## Installation
 
 ```console
 pip install pin-pink
 ```
 
-On Raspberry Pi, you will need to install [from source](https://tasts-robots.org/doc/pink/installation.html#from-source).
-
 ## Usage
 
 Pink solves differential inverse kinematics by [weighted tasks](https://scaron.info/robot-locomotion/inverse-kinematics.html). A task is defined by a *residual* function $e(q)$ of the robot configuration $q \in \mathcal{C}$ to be driven to zero. For instance, putting a foot position $p_{foot}(q)$ at a given target $p_{foot}^{\star}$ can be described by the position residual:
 
 $$
 e(q) = p_{foot}^{\star} - p_{foot}(q)
 $$
@@ -73,28 +70,28 @@
 Pink provides an API to describe the problem as tasks with targets, and automatically build and solve the underlying quadratic program.
 
 ### Task costs
 
 Here is the example of a biped robot that controls the position and orientation of its base, left and right contact frames. A fourth "posture" task, giving a preferred angle for each joint, is added for regularization:
 
 ```python
-from pink.tasks import BodyTask, PostureTask
+from pink.tasks import FrameTask, PostureTask
 
 tasks = {
-    "base": BodyTask(
+    "base": FrameTask(
         "base",
         position_cost=1.0,              # [cost] / [m]
         orientation_cost=1.0,           # [cost] / [rad]
     ),
-    "left_contact": BodyTask(
+    "left_contact": FrameTask(
         "left_contact",
         position_cost=[0.1, 0.0, 0.1],  # [cost] / [m]
         orientation_cost=0.0,           # [cost] / [rad]
     ),
-    "right_contact": BodyTask(
+    "right_contact": FrameTask(
         "right_contact",
         position_cost=[0.1, 0.0, 0.1],  # [cost] / [m]
         orientation_cost=0.0,           # [cost] / [rad]
     ),
     "posture": PostureTask(
         cost=1e-3,                      # [cost] / [rad]
     ),
@@ -120,16 +117,16 @@
 ```python
 import pink
 from robot_descriptions.loaders.pinocchio import load_robot_description
 
 robot = load_robot_description("upkie_description")
 configuration = pink.Configuration(robot.model, robot.data, robot.q0)
 for body, task in tasks.items():
-    if type(task) is BodyTask:
-        task.set_target(configuration.get_transform_body_to_world(body))
+    if type(task) is FrameTask:
+        task.set_target(configuration.get_transform_frame_to_world(body))
 ```
 
 A task can be added to the inverse kinematics once both its cost and target (if applicable) are defined.
 
 ### Differential inverse kinematics
 
 Pink solves differential inverse kinematics, meaning it outputs a velocity that steers the robot towards achieving all tasks at best. If we keep integrating that velocity, and task targets don't change over time, we will converge to a stationary configuration:
@@ -153,16 +150,16 @@
 * [Visualization in MeshCat](https://github.com/tasts-robots/pink/blob/master/examples/visualize_in_meshcat.py)
 * [Visualization in yourdfpy](https://github.com/tasts-robots/pink/blob/master/examples/visualize_in_yourdfpy.py)
 
 Pink works with all kinds of robot morphologies:
 
 * Arms: [Kinova Gen2](https://github.com/tasts-robots/pink/blob/master/examples/arm_kinova_gen2.py), [UR3](https://github.com/tasts-robots/pink/blob/master/examples/arm_ur3.py)
 * Humanoids: [JVRC-1](https://github.com/tasts-robots/pink/blob/master/examples/humanoid_jvrc.py), [SigmaBan](https://github.com/tasts-robots/pink/blob/master/examples/humanoid_sigmaban.py)
+* Mobile base: [Omnidirectional robot](https://github.com/tasts-robots/pink/blob/master/examples/mobile_omni_wheeled_robot.py), [Stretch R1](https://github.com/tasts-robots/pink/blob/master/examples/mobile_stretch.py)
 * Wheeled biped: [Upkie](https://github.com/tasts-robots/pink/blob/master/examples/wheeled_biped_upkie.py)
-* Wheeled: [Omnidirectional robot](https://github.com/tasts-robots/pink/blob/master/examples/omnidirectional_wheeled_robot.py)
 
 Check out the [examples](https://github.com/tasts-robots/pink/tree/master/examples) folder for more.
 
 ## How can I help?
 
 Install the library and use it! Report bugs in the [issue tracker](https://github.com/tasts-robots/pink/issues). If you are a developer with some robotics experience looking to hack on open source, check out the [contribution guidelines](CONTRIBUTING.md).
```

