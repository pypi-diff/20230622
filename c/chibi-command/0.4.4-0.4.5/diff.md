# Comparing `tmp/chibi_command-0.4.4.tar.gz` & `tmp/chibi_command-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chibi_command-0.4.4.tar", last modified: Thu Jun 22 04:15:34 2023, max compression
+gzip compressed data, was "chibi_command-0.4.5.tar", last modified: Thu Jun 22 04:19:02 2023, max compression
```

## Comparing `chibi_command-0.4.4.tar` & `chibi_command-0.4.5.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2023-06-22 04:15:34.136103 chibi_command-0.4.4/
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      150 2020-02-22 02:37:10.000000 chibi_command-0.4.4/AUTHORS.rst
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     3598 2020-02-22 02:37:10.000000 chibi_command-0.4.4/CONTRIBUTING.rst
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       89 2020-02-22 02:37:10.000000 chibi_command-0.4.4/HISTORY.rst
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      470 2020-02-22 02:37:10.000000 chibi_command-0.4.4/LICENSE
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      262 2020-02-22 02:37:10.000000 chibi_command-0.4.4/MANIFEST.in
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1525 2023-06-22 04:15:34.136103 chibi_command-0.4.4/PKG-INFO
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      889 2020-02-22 02:37:10.000000 chibi_command-0.4.4/README.rst
-drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2023-06-22 04:15:34.136103 chibi_command-0.4.4/chibi_command/
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     5502 2023-06-22 04:15:31.000000 chibi_command-0.4.4/chibi_command/__init__.py
-drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2023-06-22 04:15:34.136103 chibi_command-0.4.4/chibi_command/centos/
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      145 2021-09-17 00:55:39.000000 chibi_command-0.4.4/chibi_command/centos/__init__.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1528 2023-04-14 20:17:15.000000 chibi_command-0.4.4/chibi_command/centos/dnf.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     3788 2021-10-28 23:36:56.000000 chibi_command-0.4.4/chibi_command/centos/iptable.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     2132 2021-09-17 00:55:32.000000 chibi_command-0.4.4/chibi_command/centos/yum.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      398 2019-09-09 16:26:47.000000 chibi_command-0.4.4/chibi_command/db.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      186 2019-10-02 15:07:59.000000 chibi_command-0.4.4/chibi_command/dd.py
-drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2023-06-22 04:15:34.136103 chibi_command-0.4.4/chibi_command/disk/
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        0 2019-12-24 07:17:23.000000 chibi_command-0.4.4/chibi_command/disk/__init__.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1057 2020-02-22 02:34:14.000000 chibi_command-0.4.4/chibi_command/disk/dd.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      176 2020-04-05 20:30:23.000000 chibi_command-0.4.4/chibi_command/disk/format.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      223 2020-04-05 21:53:54.000000 chibi_command-0.4.4/chibi_command/disk/mount.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      451 2020-03-02 15:15:53.000000 chibi_command-0.4.4/chibi_command/echo.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      124 2019-08-16 20:41:47.000000 chibi_command-0.4.4/chibi_command/ffmpeg.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1957 2023-06-22 04:10:44.000000 chibi_command-0.4.4/chibi_command/file.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     3051 2023-06-22 04:14:40.000000 chibi_command-0.4.4/chibi_command/git.py
-drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2023-06-22 04:15:34.136103 chibi_command-0.4.4/chibi_command/image/
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        0 2019-09-03 15:04:53.000000 chibi_command-0.4.4/chibi_command/image/__init__.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      973 2019-09-03 15:15:41.000000 chibi_command-0.4.4/chibi_command/image/convert.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1427 2020-03-10 23:37:01.000000 chibi_command-0.4.4/chibi_command/image/qr.py
-drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2023-06-22 04:15:34.136103 chibi_command-0.4.4/chibi_command/lxc/
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       63 2022-01-14 21:07:02.000000 chibi_command-0.4.4/chibi_command/lxc/__init__.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      569 2022-01-14 22:56:18.000000 chibi_command-0.4.4/chibi_command/lxc/delegate.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     2753 2022-01-14 22:47:34.000000 chibi_command-0.4.4/chibi_command/lxc/lxc.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      509 2019-12-24 15:20:08.000000 chibi_command-0.4.4/chibi_command/mpd.py
-drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2023-06-22 04:15:34.136103 chibi_command-0.4.4/chibi_command/network/
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       57 2020-03-02 15:17:31.000000 chibi_command-0.4.4/chibi_command/network/__init__.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      702 2021-06-22 05:36:13.000000 chibi_command-0.4.4/chibi_command/network/ifconfig.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     2850 2021-06-22 20:27:11.000000 chibi_command-0.4.4/chibi_command/network/interfaces.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      742 2021-06-22 19:27:10.000000 chibi_command-0.4.4/chibi_command/network/iwconfig.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      460 2020-10-21 09:00:09.000000 chibi_command-0.4.4/chibi_command/network/nmap.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1918 2020-01-08 04:55:57.000000 chibi_command-0.4.4/chibi_command/network/nmcli.py
-drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2023-06-22 04:15:34.136103 chibi_command-0.4.4/chibi_command/nix/
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      132 2021-03-29 04:54:05.000000 chibi_command-0.4.4/chibi_command/nix/__init__.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      393 2021-03-29 04:56:19.000000 chibi_command-0.4.4/chibi_command/nix/locale.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     2309 2022-01-23 23:53:11.000000 chibi_command-0.4.4/chibi_command/nix/systemd.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1139 2022-01-24 00:00:33.000000 chibi_command-0.4.4/chibi_command/nix/systemd_run.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      943 2020-03-05 03:47:09.000000 chibi_command-0.4.4/chibi_command/nix/user.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      763 2021-03-29 04:59:39.000000 chibi_command-0.4.4/chibi_command/qr.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      796 2019-12-24 15:25:42.000000 chibi_command-0.4.4/chibi_command/rabbitmq.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      240 2019-12-24 15:28:53.000000 chibi_command-0.4.4/chibi_command/rpm.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     2124 2023-06-16 15:51:24.000000 chibi_command-0.4.4/chibi_command/rsync.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      405 2021-09-16 23:19:35.000000 chibi_command-0.4.4/chibi_command/sysctl.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     4938 2022-03-24 21:23:12.000000 chibi_command-0.4.4/chibi_command/wmctrl.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      758 2020-03-02 15:17:03.000000 chibi_command-0.4.4/chibi_command/xfce4.py
-drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2023-06-22 04:15:34.136103 chibi_command-0.4.4/chibi_command.egg-info/
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1525 2023-06-22 04:15:34.000000 chibi_command-0.4.4/chibi_command.egg-info/PKG-INFO
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     2110 2023-06-22 04:15:34.000000 chibi_command-0.4.4/chibi_command.egg-info/SOURCES.txt
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        1 2023-06-22 04:15:34.000000 chibi_command-0.4.4/chibi_command.egg-info/dependency_links.txt
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        1 2023-06-22 04:15:34.000000 chibi_command-0.4.4/chibi_command.egg-info/not-zip-safe
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       43 2023-06-22 04:15:34.000000 chibi_command-0.4.4/chibi_command.egg-info/requires.txt
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       14 2023-06-22 04:15:34.000000 chibi_command-0.4.4/chibi_command.egg-info/top_level.txt
-drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2023-06-22 04:15:34.136103 chibi_command-0.4.4/docs/
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      614 2020-02-22 02:37:10.000000 chibi_command-0.4.4/docs/Makefile
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       28 2020-02-22 02:37:10.000000 chibi_command-0.4.4/docs/authors.rst
--rwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)     4872 2020-02-22 02:37:10.000000 chibi_command-0.4.4/docs/conf.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       33 2020-02-22 02:37:10.000000 chibi_command-0.4.4/docs/contributing.rst
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       28 2020-02-22 02:37:10.000000 chibi_command-0.4.4/docs/history.rst
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      310 2020-02-22 02:37:10.000000 chibi_command-0.4.4/docs/index.rst
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1158 2020-02-22 02:37:10.000000 chibi_command-0.4.4/docs/installation.rst
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      775 2020-02-22 02:37:10.000000 chibi_command-0.4.4/docs/make.bat
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       27 2020-02-22 02:37:10.000000 chibi_command-0.4.4/docs/readme.rst
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       81 2020-02-22 02:37:10.000000 chibi_command-0.4.4/docs/usage.rst
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      451 2023-06-22 04:15:34.136103 chibi_command-0.4.4/setup.cfg
--rwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)     1095 2023-06-22 04:15:31.000000 chibi_command-0.4.4/setup.py
-drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2023-06-22 04:15:34.136103 chibi_command-0.4.4/tests/
--rwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2018-06-27 08:43:08.000000 chibi_command-0.4.4/tests/__init__.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     2639 2021-10-28 23:37:46.000000 chibi_command-0.4.4/tests/centos.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     3014 2022-01-23 23:33:44.000000 chibi_command-0.4.4/tests/command.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      888 2022-01-23 21:58:14.000000 chibi_command-0.4.4/tests/command_result.py
-drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2023-06-22 04:15:34.136103 chibi_command-0.4.4/tests/disk/
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        0 2020-02-09 22:05:59.000000 chibi_command-0.4.4/tests/disk/__init__.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      854 2020-03-05 03:19:52.000000 chibi_command-0.4.4/tests/disk/dd.py
-drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2023-06-22 04:15:34.136103 chibi_command-0.4.4/tests/echo/
--rwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2018-06-27 08:43:08.000000 chibi_command-0.4.4/tests/echo/__init__.py
--rwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)     1489 2019-09-09 15:53:10.000000 chibi_command-0.4.4/tests/echo/test_echo.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      659 2023-06-12 10:48:40.000000 chibi_command-0.4.4/tests/file.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     2080 2021-12-09 17:56:18.000000 chibi_command-0.4.4/tests/git.py
-drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2023-06-22 04:15:34.136103 chibi_command-0.4.4/tests/image/
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        0 2019-09-03 15:17:47.000000 chibi_command-0.4.4/tests/image/__init__.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       73 2019-09-03 16:47:29.000000 chibi_command-0.4.4/tests/image/convert.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     5052 2022-01-23 22:26:47.000000 chibi_command-0.4.4/tests/lxc.py
-drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2023-06-22 04:15:34.136103 chibi_command-0.4.4/tests/network/
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        0 2019-12-24 15:36:50.000000 chibi_command-0.4.4/tests/network/__init__.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      441 2021-06-22 05:36:27.000000 chibi_command-0.4.4/tests/network/ifconfig.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     2314 2021-06-22 20:26:55.000000 chibi_command-0.4.4/tests/network/interface.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      483 2021-06-22 19:27:41.000000 chibi_command-0.4.4/tests/network/iwconfig.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1305 2020-01-08 04:56:58.000000 chibi_command-0.4.4/tests/network/nmcli.py
-drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2023-06-22 04:15:34.136103 chibi_command-0.4.4/tests/nix/
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        0 2020-03-05 03:38:01.000000 chibi_command-0.4.4/tests/nix/__init__.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      296 2021-03-29 04:56:15.000000 chibi_command-0.4.4/tests/nix/locale.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1626 2022-01-23 23:31:52.000000 chibi_command-0.4.4/tests/nix/systemd.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      805 2022-01-14 23:15:07.000000 chibi_command-0.4.4/tests/nix/systemd_run.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      538 2020-03-05 03:42:36.000000 chibi_command-0.4.4/tests/nix/user.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      948 2020-04-07 22:27:40.000000 chibi_command-0.4.4/tests/rsync.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      560 2021-09-16 23:21:23.000000 chibi_command-0.4.4/tests/sysctl.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     2805 2022-03-24 21:23:46.000000 chibi_command-0.4.4/tests/wmctrl.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1976 2019-10-31 18:00:07.000000 chibi_command-0.4.4/tests/xfce4.py
+drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2023-06-22 04:19:02.762766 chibi_command-0.4.5/
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      150 2020-02-22 02:37:10.000000 chibi_command-0.4.5/AUTHORS.rst
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     3598 2020-02-22 02:37:10.000000 chibi_command-0.4.5/CONTRIBUTING.rst
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       89 2020-02-22 02:37:10.000000 chibi_command-0.4.5/HISTORY.rst
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      470 2020-02-22 02:37:10.000000 chibi_command-0.4.5/LICENSE
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      262 2020-02-22 02:37:10.000000 chibi_command-0.4.5/MANIFEST.in
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1525 2023-06-22 04:19:02.762766 chibi_command-0.4.5/PKG-INFO
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      889 2020-02-22 02:37:10.000000 chibi_command-0.4.5/README.rst
+drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2023-06-22 04:19:02.762766 chibi_command-0.4.5/chibi_command/
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     5502 2023-06-22 04:19:00.000000 chibi_command-0.4.5/chibi_command/__init__.py
+drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2023-06-22 04:19:02.762766 chibi_command-0.4.5/chibi_command/centos/
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      145 2021-09-17 00:55:39.000000 chibi_command-0.4.5/chibi_command/centos/__init__.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1528 2023-04-14 20:17:15.000000 chibi_command-0.4.5/chibi_command/centos/dnf.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     3788 2021-10-28 23:36:56.000000 chibi_command-0.4.5/chibi_command/centos/iptable.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     2132 2021-09-17 00:55:32.000000 chibi_command-0.4.5/chibi_command/centos/yum.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      398 2019-09-09 16:26:47.000000 chibi_command-0.4.5/chibi_command/db.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      186 2019-10-02 15:07:59.000000 chibi_command-0.4.5/chibi_command/dd.py
+drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2023-06-22 04:19:02.762766 chibi_command-0.4.5/chibi_command/disk/
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        0 2019-12-24 07:17:23.000000 chibi_command-0.4.5/chibi_command/disk/__init__.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1057 2020-02-22 02:34:14.000000 chibi_command-0.4.5/chibi_command/disk/dd.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      176 2020-04-05 20:30:23.000000 chibi_command-0.4.5/chibi_command/disk/format.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      223 2020-04-05 21:53:54.000000 chibi_command-0.4.5/chibi_command/disk/mount.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      451 2020-03-02 15:15:53.000000 chibi_command-0.4.5/chibi_command/echo.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      124 2019-08-16 20:41:47.000000 chibi_command-0.4.5/chibi_command/ffmpeg.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1957 2023-06-22 04:10:44.000000 chibi_command-0.4.5/chibi_command/file.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     3344 2023-06-22 04:18:24.000000 chibi_command-0.4.5/chibi_command/git.py
+drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2023-06-22 04:19:02.762766 chibi_command-0.4.5/chibi_command/image/
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        0 2019-09-03 15:04:53.000000 chibi_command-0.4.5/chibi_command/image/__init__.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      973 2019-09-03 15:15:41.000000 chibi_command-0.4.5/chibi_command/image/convert.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1427 2020-03-10 23:37:01.000000 chibi_command-0.4.5/chibi_command/image/qr.py
+drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2023-06-22 04:19:02.762766 chibi_command-0.4.5/chibi_command/lxc/
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       63 2022-01-14 21:07:02.000000 chibi_command-0.4.5/chibi_command/lxc/__init__.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      569 2022-01-14 22:56:18.000000 chibi_command-0.4.5/chibi_command/lxc/delegate.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     2753 2022-01-14 22:47:34.000000 chibi_command-0.4.5/chibi_command/lxc/lxc.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      509 2019-12-24 15:20:08.000000 chibi_command-0.4.5/chibi_command/mpd.py
+drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2023-06-22 04:19:02.762766 chibi_command-0.4.5/chibi_command/network/
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       57 2020-03-02 15:17:31.000000 chibi_command-0.4.5/chibi_command/network/__init__.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      702 2021-06-22 05:36:13.000000 chibi_command-0.4.5/chibi_command/network/ifconfig.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     2850 2021-06-22 20:27:11.000000 chibi_command-0.4.5/chibi_command/network/interfaces.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      742 2021-06-22 19:27:10.000000 chibi_command-0.4.5/chibi_command/network/iwconfig.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      460 2020-10-21 09:00:09.000000 chibi_command-0.4.5/chibi_command/network/nmap.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1918 2020-01-08 04:55:57.000000 chibi_command-0.4.5/chibi_command/network/nmcli.py
+drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2023-06-22 04:19:02.762766 chibi_command-0.4.5/chibi_command/nix/
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      132 2021-03-29 04:54:05.000000 chibi_command-0.4.5/chibi_command/nix/__init__.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      393 2021-03-29 04:56:19.000000 chibi_command-0.4.5/chibi_command/nix/locale.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     2309 2022-01-23 23:53:11.000000 chibi_command-0.4.5/chibi_command/nix/systemd.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1139 2022-01-24 00:00:33.000000 chibi_command-0.4.5/chibi_command/nix/systemd_run.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      943 2020-03-05 03:47:09.000000 chibi_command-0.4.5/chibi_command/nix/user.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      763 2021-03-29 04:59:39.000000 chibi_command-0.4.5/chibi_command/qr.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      796 2019-12-24 15:25:42.000000 chibi_command-0.4.5/chibi_command/rabbitmq.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      240 2019-12-24 15:28:53.000000 chibi_command-0.4.5/chibi_command/rpm.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     2124 2023-06-16 15:51:24.000000 chibi_command-0.4.5/chibi_command/rsync.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      405 2021-09-16 23:19:35.000000 chibi_command-0.4.5/chibi_command/sysctl.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     4938 2022-03-24 21:23:12.000000 chibi_command-0.4.5/chibi_command/wmctrl.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      758 2020-03-02 15:17:03.000000 chibi_command-0.4.5/chibi_command/xfce4.py
+drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2023-06-22 04:19:02.762766 chibi_command-0.4.5/chibi_command.egg-info/
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1525 2023-06-22 04:19:02.000000 chibi_command-0.4.5/chibi_command.egg-info/PKG-INFO
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     2110 2023-06-22 04:19:02.000000 chibi_command-0.4.5/chibi_command.egg-info/SOURCES.txt
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        1 2023-06-22 04:19:02.000000 chibi_command-0.4.5/chibi_command.egg-info/dependency_links.txt
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        1 2023-06-22 04:19:02.000000 chibi_command-0.4.5/chibi_command.egg-info/not-zip-safe
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       43 2023-06-22 04:19:02.000000 chibi_command-0.4.5/chibi_command.egg-info/requires.txt
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       14 2023-06-22 04:19:02.000000 chibi_command-0.4.5/chibi_command.egg-info/top_level.txt
+drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2023-06-22 04:19:02.762766 chibi_command-0.4.5/docs/
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      614 2020-02-22 02:37:10.000000 chibi_command-0.4.5/docs/Makefile
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       28 2020-02-22 02:37:10.000000 chibi_command-0.4.5/docs/authors.rst
+-rwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)     4872 2020-02-22 02:37:10.000000 chibi_command-0.4.5/docs/conf.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       33 2020-02-22 02:37:10.000000 chibi_command-0.4.5/docs/contributing.rst
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       28 2020-02-22 02:37:10.000000 chibi_command-0.4.5/docs/history.rst
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      310 2020-02-22 02:37:10.000000 chibi_command-0.4.5/docs/index.rst
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1158 2020-02-22 02:37:10.000000 chibi_command-0.4.5/docs/installation.rst
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      775 2020-02-22 02:37:10.000000 chibi_command-0.4.5/docs/make.bat
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       27 2020-02-22 02:37:10.000000 chibi_command-0.4.5/docs/readme.rst
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       81 2020-02-22 02:37:10.000000 chibi_command-0.4.5/docs/usage.rst
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      451 2023-06-22 04:19:02.762766 chibi_command-0.4.5/setup.cfg
+-rwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)     1095 2023-06-22 04:19:00.000000 chibi_command-0.4.5/setup.py
+drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2023-06-22 04:19:02.762766 chibi_command-0.4.5/tests/
+-rwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2018-06-27 08:43:08.000000 chibi_command-0.4.5/tests/__init__.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     2639 2021-10-28 23:37:46.000000 chibi_command-0.4.5/tests/centos.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     3014 2022-01-23 23:33:44.000000 chibi_command-0.4.5/tests/command.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      888 2022-01-23 21:58:14.000000 chibi_command-0.4.5/tests/command_result.py
+drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2023-06-22 04:19:02.762766 chibi_command-0.4.5/tests/disk/
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        0 2020-02-09 22:05:59.000000 chibi_command-0.4.5/tests/disk/__init__.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      854 2020-03-05 03:19:52.000000 chibi_command-0.4.5/tests/disk/dd.py
+drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2023-06-22 04:19:02.762766 chibi_command-0.4.5/tests/echo/
+-rwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2018-06-27 08:43:08.000000 chibi_command-0.4.5/tests/echo/__init__.py
+-rwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)     1489 2019-09-09 15:53:10.000000 chibi_command-0.4.5/tests/echo/test_echo.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      659 2023-06-12 10:48:40.000000 chibi_command-0.4.5/tests/file.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     2080 2021-12-09 17:56:18.000000 chibi_command-0.4.5/tests/git.py
+drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2023-06-22 04:19:02.762766 chibi_command-0.4.5/tests/image/
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        0 2019-09-03 15:17:47.000000 chibi_command-0.4.5/tests/image/__init__.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       73 2019-09-03 16:47:29.000000 chibi_command-0.4.5/tests/image/convert.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     5052 2022-01-23 22:26:47.000000 chibi_command-0.4.5/tests/lxc.py
+drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2023-06-22 04:19:02.762766 chibi_command-0.4.5/tests/network/
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        0 2019-12-24 15:36:50.000000 chibi_command-0.4.5/tests/network/__init__.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      441 2021-06-22 05:36:27.000000 chibi_command-0.4.5/tests/network/ifconfig.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     2314 2021-06-22 20:26:55.000000 chibi_command-0.4.5/tests/network/interface.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      483 2021-06-22 19:27:41.000000 chibi_command-0.4.5/tests/network/iwconfig.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1305 2020-01-08 04:56:58.000000 chibi_command-0.4.5/tests/network/nmcli.py
+drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2023-06-22 04:19:02.762766 chibi_command-0.4.5/tests/nix/
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        0 2020-03-05 03:38:01.000000 chibi_command-0.4.5/tests/nix/__init__.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      296 2021-03-29 04:56:15.000000 chibi_command-0.4.5/tests/nix/locale.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1626 2022-01-23 23:31:52.000000 chibi_command-0.4.5/tests/nix/systemd.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      805 2022-01-14 23:15:07.000000 chibi_command-0.4.5/tests/nix/systemd_run.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      538 2020-03-05 03:42:36.000000 chibi_command-0.4.5/tests/nix/user.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      948 2020-04-07 22:27:40.000000 chibi_command-0.4.5/tests/rsync.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      560 2021-09-16 23:21:23.000000 chibi_command-0.4.5/tests/sysctl.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     2805 2022-03-24 21:23:46.000000 chibi_command-0.4.5/tests/wmctrl.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1976 2019-10-31 18:00:07.000000 chibi_command-0.4.5/tests/xfce4.py
```

### Comparing `chibi_command-0.4.4/CONTRIBUTING.rst` & `chibi_command-0.4.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `chibi_command-0.4.4/PKG-INFO` & `chibi_command-0.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chibi_command
-Version: 0.4.4
+Version: 0.4.5
 Summary: run terminal commands
 Home-page: https://github.com/dem4ply/chibi_command
 Author: Dem4ply
 Author-email: dem4ply@gmail.com
 License: WTFPL
 Keywords: chibi_command
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `chibi_command-0.4.4/README.rst` & `chibi_command-0.4.5/README.rst`

 * *Files identical despite different names*

### Comparing `chibi_command-0.4.4/chibi_command/__init__.py` & `chibi_command-0.4.5/chibi_command/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from subprocess import Popen, PIPE
 import json
 import itertools
 import logging
 
 __author__ = """dem4ply"""
 __email__ = 'dem4ply@gmail.com'
-__version__ = '0.4.4'
+__version__ = '0.4.5'
 
 logger = logging.getLogger( 'chibi.command' )
 
 
 class Command_result:
     def __init__( self, result, error, return_code ):
         self.result = result
```

### Comparing `chibi_command-0.4.4/chibi_command/centos/dnf.py` & `chibi_command-0.4.5/chibi_command/centos/dnf.py`

 * *Files identical despite different names*

### Comparing `chibi_command-0.4.4/chibi_command/centos/iptable.py` & `chibi_command-0.4.5/chibi_command/centos/iptable.py`

 * *Files identical despite different names*

### Comparing `chibi_command-0.4.4/chibi_command/centos/yum.py` & `chibi_command-0.4.5/chibi_command/centos/yum.py`

 * *Files identical despite different names*

### Comparing `chibi_command-0.4.4/chibi_command/disk/dd.py` & `chibi_command-0.4.5/chibi_command/disk/dd.py`

 * *Files identical despite different names*

### Comparing `chibi_command-0.4.4/chibi_command/file.py` & `chibi_command-0.4.5/chibi_command/file.py`

 * *Files identical despite different names*

### Comparing `chibi_command-0.4.4/chibi_command/git.py` & `chibi_command-0.4.5/chibi_command/git.py`

 * *Files 4% similar despite different names*

```diff
@@ -96,8 +96,16 @@
             if src:
                 command = cls(
                     f'--git-dir={src}/.git', f'--work-tree={src}',
                     'checkout', '--track', branch, **kw )
             else:
                 command = cls( 'checkout', '--track', branch, **kw )
             return command.run()
+        else:
+            if src:
+                command = cls(
+                    f'--git-dir={src}/.git', f'--work-tree={src}',
+                    'checkout', **kw )
+            else:
+                raise NotImplementedError(
+                    f"branch={branch}, src={src}, kw={kw}" )
         raise NotImplementedError( f"branch={branch}, src={src}, kw={kw}" )
```

### Comparing `chibi_command-0.4.4/chibi_command/image/convert.py` & `chibi_command-0.4.5/chibi_command/image/convert.py`

 * *Files identical despite different names*

### Comparing `chibi_command-0.4.4/chibi_command/image/qr.py` & `chibi_command-0.4.5/chibi_command/image/qr.py`

 * *Files identical despite different names*

### Comparing `chibi_command-0.4.4/chibi_command/lxc/delegate.py` & `chibi_command-0.4.5/chibi_command/lxc/delegate.py`

 * *Files identical despite different names*

### Comparing `chibi_command-0.4.4/chibi_command/lxc/lxc.py` & `chibi_command-0.4.5/chibi_command/lxc/lxc.py`

 * *Files identical despite different names*

### Comparing `chibi_command-0.4.4/chibi_command/network/ifconfig.py` & `chibi_command-0.4.5/chibi_command/network/ifconfig.py`

 * *Files identical despite different names*

### Comparing `chibi_command-0.4.4/chibi_command/network/interfaces.py` & `chibi_command-0.4.5/chibi_command/network/interfaces.py`

 * *Files identical despite different names*

### Comparing `chibi_command-0.4.4/chibi_command/network/iwconfig.py` & `chibi_command-0.4.5/chibi_command/network/iwconfig.py`

 * *Files identical despite different names*

### Comparing `chibi_command-0.4.4/chibi_command/network/nmcli.py` & `chibi_command-0.4.5/chibi_command/network/nmcli.py`

 * *Files identical despite different names*

### Comparing `chibi_command-0.4.4/chibi_command/nix/systemd.py` & `chibi_command-0.4.5/chibi_command/nix/systemd.py`

 * *Files identical despite different names*

### Comparing `chibi_command-0.4.4/chibi_command/nix/systemd_run.py` & `chibi_command-0.4.5/chibi_command/nix/systemd_run.py`

 * *Files identical despite different names*

### Comparing `chibi_command-0.4.4/chibi_command/nix/user.py` & `chibi_command-0.4.5/chibi_command/nix/user.py`

 * *Files identical despite different names*

### Comparing `chibi_command-0.4.4/chibi_command/qr.py` & `chibi_command-0.4.5/chibi_command/qr.py`

 * *Files identical despite different names*

### Comparing `chibi_command-0.4.4/chibi_command/rabbitmq.py` & `chibi_command-0.4.5/chibi_command/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `chibi_command-0.4.4/chibi_command/rsync.py` & `chibi_command-0.4.5/chibi_command/rsync.py`

 * *Files identical despite different names*

### Comparing `chibi_command-0.4.4/chibi_command/wmctrl.py` & `chibi_command-0.4.5/chibi_command/wmctrl.py`

 * *Files identical despite different names*

### Comparing `chibi_command-0.4.4/chibi_command/xfce4.py` & `chibi_command-0.4.5/chibi_command/xfce4.py`

 * *Files identical despite different names*

### Comparing `chibi_command-0.4.4/chibi_command.egg-info/PKG-INFO` & `chibi_command-0.4.5/chibi_command.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chibi-command
-Version: 0.4.4
+Version: 0.4.5
 Summary: run terminal commands
 Home-page: https://github.com/dem4ply/chibi_command
 Author: Dem4ply
 Author-email: dem4ply@gmail.com
 License: WTFPL
 Keywords: chibi_command
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `chibi_command-0.4.4/chibi_command.egg-info/SOURCES.txt` & `chibi_command-0.4.5/chibi_command.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chibi_command-0.4.4/docs/Makefile` & `chibi_command-0.4.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `chibi_command-0.4.4/docs/conf.py` & `chibi_command-0.4.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `chibi_command-0.4.4/docs/installation.rst` & `chibi_command-0.4.5/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `chibi_command-0.4.4/docs/make.bat` & `chibi_command-0.4.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `chibi_command-0.4.4/setup.py` & `chibi_command-0.4.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,10 +29,10 @@
     license="WTFPL",
     long_description=readme + '\n\n' + history,
     include_package_data=True,
     keywords='chibi_command',
     name='chibi_command',
     packages=find_packages(include=['chibi_command', 'chibi_command.*']),
     url='https://github.com/dem4ply/chibi_command',
-    version='0.4.4',
+    version='0.4.5',
     zip_safe=False,
 )
```

### Comparing `chibi_command-0.4.4/tests/centos.py` & `chibi_command-0.4.5/tests/centos.py`

 * *Files identical despite different names*

### Comparing `chibi_command-0.4.4/tests/command.py` & `chibi_command-0.4.5/tests/command.py`

 * *Files identical despite different names*

### Comparing `chibi_command-0.4.4/tests/command_result.py` & `chibi_command-0.4.5/tests/command_result.py`

 * *Files identical despite different names*

### Comparing `chibi_command-0.4.4/tests/disk/dd.py` & `chibi_command-0.4.5/tests/disk/dd.py`

 * *Files identical despite different names*

### Comparing `chibi_command-0.4.4/tests/echo/test_echo.py` & `chibi_command-0.4.5/tests/echo/test_echo.py`

 * *Files identical despite different names*

### Comparing `chibi_command-0.4.4/tests/file.py` & `chibi_command-0.4.5/tests/file.py`

 * *Files identical despite different names*

### Comparing `chibi_command-0.4.4/tests/git.py` & `chibi_command-0.4.5/tests/git.py`

 * *Files identical despite different names*

### Comparing `chibi_command-0.4.4/tests/lxc.py` & `chibi_command-0.4.5/tests/lxc.py`

 * *Files identical despite different names*

### Comparing `chibi_command-0.4.4/tests/network/interface.py` & `chibi_command-0.4.5/tests/network/interface.py`

 * *Files identical despite different names*

### Comparing `chibi_command-0.4.4/tests/network/nmcli.py` & `chibi_command-0.4.5/tests/network/nmcli.py`

 * *Files identical despite different names*

### Comparing `chibi_command-0.4.4/tests/nix/systemd.py` & `chibi_command-0.4.5/tests/nix/systemd.py`

 * *Files identical despite different names*

### Comparing `chibi_command-0.4.4/tests/nix/systemd_run.py` & `chibi_command-0.4.5/tests/nix/systemd_run.py`

 * *Files identical despite different names*

### Comparing `chibi_command-0.4.4/tests/nix/user.py` & `chibi_command-0.4.5/tests/nix/user.py`

 * *Files identical despite different names*

### Comparing `chibi_command-0.4.4/tests/rsync.py` & `chibi_command-0.4.5/tests/rsync.py`

 * *Files identical despite different names*

### Comparing `chibi_command-0.4.4/tests/sysctl.py` & `chibi_command-0.4.5/tests/sysctl.py`

 * *Files identical despite different names*

### Comparing `chibi_command-0.4.4/tests/wmctrl.py` & `chibi_command-0.4.5/tests/wmctrl.py`

 * *Files identical despite different names*

### Comparing `chibi_command-0.4.4/tests/xfce4.py` & `chibi_command-0.4.5/tests/xfce4.py`

 * *Files identical despite different names*

