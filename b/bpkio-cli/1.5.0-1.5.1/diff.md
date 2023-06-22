# Comparing `tmp/bpkio_cli-1.5.0.tar.gz` & `tmp/bpkio_cli-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bpkio_cli-1.5.0.tar", max compression
+gzip compressed data, was "bpkio_cli-1.5.1.tar", max compression
```

## Comparing `bpkio_cli-1.5.0.tar` & `bpkio_cli-1.5.1.tar`

### file list

```diff
@@ -1,68 +1,68 @@
--rw-r--r--   0        0        0        0 2023-06-05 14:52:28.912688 bpkio_cli-1.5.0/README.md
--rw-r--r--   0        0        0       22 2023-06-09 15:48:20.061591 bpkio_cli-1.5.0/bpkio_cli/__init__.py
--rw-r--r--   0        0        0     3880 2023-06-09 12:59:30.590598 bpkio_cli-1.5.0/bpkio_cli/app.py
--rw-r--r--   0        0        0       91 2023-06-05 14:52:28.913801 bpkio_cli-1.5.0/bpkio_cli/click_mods/__init__.py
--rw-r--r--   0        0        0      771 2023-06-05 14:52:28.914515 bpkio_cli-1.5.0/bpkio_cli/click_mods/default_last_command.py
--rw-r--r--   0        0        0     5244 2023-06-08 08:20:08.800756 bpkio_cli-1.5.0/bpkio_cli/click_mods/group_rest_resource.py
--rw-r--r--   0        0        0     1747 2023-06-05 14:52:28.915564 bpkio_cli-1.5.0/bpkio_cli/click_mods/option_eat_all.py
--rw-r--r--   0        0        0      599 2023-06-05 14:52:28.916268 bpkio_cli-1.5.0/bpkio_cli/click_options/__init__.py
--rw-r--r--   0        0        0      848 2023-06-05 14:52:28.916749 bpkio_cli-1.5.0/bpkio_cli/click_options/admin.py
--rw-r--r--   0        0        0      355 2023-06-05 14:52:28.917214 bpkio_cli-1.5.0/bpkio_cli/click_options/json.py
--rw-r--r--   0        0        0      958 2023-06-05 14:52:28.917874 bpkio_cli-1.5.0/bpkio_cli/click_options/list.py
--rw-r--r--   0        0        0      933 2023-06-05 14:52:28.918220 bpkio_cli-1.5.0/bpkio_cli/click_options/poll.py
--rw-r--r--   0        0        0      845 2023-06-07 15:41:46.996440 bpkio_cli-1.5.0/bpkio_cli/click_options/read.py
--rw-r--r--   0        0        0     1183 2023-06-05 14:52:28.919379 bpkio_cli-1.5.0/bpkio_cli/click_options/search.py
--rw-r--r--   0        0        0      445 2023-06-05 14:52:28.919891 bpkio_cli-1.5.0/bpkio_cli/click_options/table.py
--rw-r--r--   0        0        0     1735 2023-06-09 15:29:17.087943 bpkio_cli-1.5.0/bpkio_cli/click_options/urls.py
--rw-r--r--   0        0        0      656 2023-06-05 14:52:28.920820 bpkio_cli-1.5.0/bpkio_cli/commands/__init__.py
--rw-r--r--   0        0        0      751 2023-06-07 16:02:26.119276 bpkio_cli-1.5.0/bpkio_cli/commands/addons.py
--rw-r--r--   0        0        0     5246 2023-06-07 15:41:46.996745 bpkio_cli-1.5.0/bpkio_cli/commands/configure.py
--rw-r--r--   0        0        0     1766 2023-06-07 15:41:46.997118 bpkio_cli-1.5.0/bpkio_cli/commands/consumption.py
--rw-r--r--   0        0        0     4379 2023-06-07 15:41:46.997928 bpkio_cli-1.5.0/bpkio_cli/commands/creators/ad_insertion.py
--rw-r--r--   0        0        0     7921 2023-06-07 15:41:46.998681 bpkio_cli-1.5.0/bpkio_cli/commands/creators/sources.py
--rw-r--r--   0        0        0     4055 2023-06-07 15:41:46.999059 bpkio_cli-1.5.0/bpkio_cli/commands/creators/virtual_channel.py
--rw-r--r--   0        0        0     8949 2023-06-09 12:53:03.155944 bpkio_cli-1.5.0/bpkio_cli/commands/creators/virtual_channel_populate.py
--rw-r--r--   0        0        0      761 2023-06-05 14:52:28.924009 bpkio_cli-1.5.0/bpkio_cli/commands/hello.py
--rw-r--r--   0        0        0     1251 2023-06-05 14:52:28.924268 bpkio_cli-1.5.0/bpkio_cli/commands/memory.py
--rw-r--r--   0        0        0     3444 2023-06-07 15:41:46.999728 bpkio_cli-1.5.0/bpkio_cli/commands/package.py
--rw-r--r--   0        0        0    10214 2023-06-08 07:15:15.683549 bpkio_cli-1.5.0/bpkio_cli/commands/profiles.py
--rw-r--r--   0        0        0     2700 2023-06-05 14:52:28.925148 bpkio_cli-1.5.0/bpkio_cli/commands/recorder.py
--rw-r--r--   0        0        0     3669 2023-06-05 14:52:28.925467 bpkio_cli-1.5.0/bpkio_cli/commands/services.py
--rw-r--r--   0        0        0     5728 2023-06-07 15:41:47.000514 bpkio_cli-1.5.0/bpkio_cli/commands/sources.py
--rw-r--r--   0        0        0    19372 2023-06-09 14:37:07.787776 bpkio_cli-1.5.0/bpkio_cli/commands/template_crud.py
--rw-r--r--   0        0        0     7306 2023-06-05 14:52:28.926463 bpkio_cli-1.5.0/bpkio_cli/commands/template_crud_slots.py
--rw-r--r--   0        0        0      332 2023-06-05 14:52:28.926844 bpkio_cli-1.5.0/bpkio_cli/commands/tenants.py
--rw-r--r--   0        0        0     5799 2023-06-09 15:31:03.604764 bpkio_cli-1.5.0/bpkio_cli/commands/url.py
--rw-r--r--   0        0        0      359 2023-06-05 14:52:28.927398 bpkio_cli-1.5.0/bpkio_cli/commands/users.py
--rw-r--r--   0        0        0     1036 2023-06-05 14:52:28.927822 bpkio_cli-1.5.0/bpkio_cli/core/app_context.py
--rw-r--r--   0        0        0     4556 2023-06-09 14:54:47.502096 bpkio_cli-1.5.0/bpkio_cli/core/config_provider.py
--rw-r--r--   0        0        0      283 2023-06-09 10:01:38.442641 bpkio_cli-1.5.0/bpkio_cli/core/exceptions.py
--rw-r--r--   0        0        0     2714 2023-06-09 11:12:30.963265 bpkio_cli-1.5.0/bpkio_cli/core/initialize.py
--rw-r--r--   0        0        0     1718 2023-06-05 14:52:28.929630 bpkio_cli-1.5.0/bpkio_cli/core/logger.py
--rw-r--r--   0        0        0     8332 2023-06-07 15:41:47.001439 bpkio_cli-1.5.0/bpkio_cli/core/packager.py
--rw-r--r--   0        0        0     9526 2023-06-09 15:34:00.255674 bpkio_cli-1.5.0/bpkio_cli/core/resource_recorder.py
--rw-r--r--   0        0        0     2204 2023-06-05 14:52:28.930943 bpkio_cli-1.5.0/bpkio_cli/core/resource_trail.py
--rw-r--r--   0        0        0     5128 2023-06-05 14:52:28.931598 bpkio_cli-1.5.0/bpkio_cli/core/response_handler.py
--rw-r--r--   0        0        0     1234 2023-06-05 14:52:28.931905 bpkio_cli-1.5.0/bpkio_cli/core/session_recorder.py
--rw-r--r--   0        0        0      395 2023-06-05 14:52:28.932292 bpkio_cli-1.5.0/bpkio_cli/utils/__init__.py
--rw-r--r--   0        0        0     2288 2023-06-05 14:52:28.932584 bpkio_cli-1.5.0/bpkio_cli/utils/arrays.py
--rw-r--r--   0        0        0     1358 2023-06-05 14:52:28.932885 bpkio_cli-1.5.0/bpkio_cli/utils/datetimes.py
--rw-r--r--   0        0        0     1828 2023-06-05 14:52:28.933224 bpkio_cli-1.5.0/bpkio_cli/utils/editor.py
--rw-r--r--   0        0        0      494 2023-06-07 15:41:47.002131 bpkio_cli-1.5.0/bpkio_cli/utils/inquirer.py
--rw-r--r--   0        0        0      136 2023-06-05 14:52:28.933905 bpkio_cli-1.5.0/bpkio_cli/utils/json.py
--rw-r--r--   0        0        0      567 2023-06-05 14:52:28.934214 bpkio_cli-1.5.0/bpkio_cli/utils/profile_maker.py
--rw-r--r--   0        0        0    14499 2023-06-09 15:31:09.893672 bpkio_cli-1.5.0/bpkio_cli/utils/url_builders.py
--rw-r--r--   0        0        0      861 2023-06-05 14:52:28.934866 bpkio_cli-1.5.0/bpkio_cli/utils/urls.py
--rw-r--r--   0        0        0     1034 2023-06-05 14:52:28.935214 bpkio_cli-1.5.0/bpkio_cli/writers/breadcrumbs.py
--rw-r--r--   0        0        0     1667 2023-06-07 15:41:47.003003 bpkio_cli-1.5.0/bpkio_cli/writers/colorizer.py
--rw-r--r--   0        0        0     5213 2023-06-09 10:05:20.541841 bpkio_cli-1.5.0/bpkio_cli/writers/content_display.py
--rw-r--r--   0        0        0      840 2023-06-05 14:52:28.936348 bpkio_cli-1.5.0/bpkio_cli/writers/diff.py
--rw-r--r--   0        0        0      751 2023-06-07 15:41:47.003793 bpkio_cli-1.5.0/bpkio_cli/writers/formatter.py
--rw-r--r--   0        0        0     5729 2023-06-09 10:04:01.517494 bpkio_cli-1.5.0/bpkio_cli/writers/hls_formatter.py
--rw-r--r--   0        0        0      714 2023-06-05 14:52:28.938409 bpkio_cli-1.5.0/bpkio_cli/writers/json_formatter.py
--rw-r--r--   0        0        0     1658 2023-06-09 14:52:25.540620 bpkio_cli-1.5.0/bpkio_cli/writers/players.py
--rw-r--r--   0        0        0     1631 2023-06-07 15:41:47.004793 bpkio_cli-1.5.0/bpkio_cli/writers/scte35.py
--rw-r--r--   0        0        0     1865 2023-06-05 14:52:28.939530 bpkio_cli-1.5.0/bpkio_cli/writers/tables.py
--rw-r--r--   0        0        0     5741 2023-06-09 10:03:51.584951 bpkio_cli-1.5.0/bpkio_cli/writers/xml_formatter.py
--rw-r--r--   0        0        0     1242 2023-06-09 15:48:20.060601 bpkio_cli-1.5.0/pyproject.toml
--rw-r--r--   0        0        0      972 1970-01-01 00:00:00.000000 bpkio_cli-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-05 14:52:28.912688 bpkio_cli-1.5.1/README.md
+-rw-r--r--   0        0        0       22 2023-06-22 10:44:02.485942 bpkio_cli-1.5.1/bpkio_cli/__init__.py
+-rw-r--r--   0        0        0     3929 2023-06-14 20:37:39.202656 bpkio_cli-1.5.1/bpkio_cli/app.py
+-rw-r--r--   0        0        0       91 2023-06-05 14:52:28.913801 bpkio_cli-1.5.1/bpkio_cli/click_mods/__init__.py
+-rw-r--r--   0        0        0      771 2023-06-05 14:52:28.914515 bpkio_cli-1.5.1/bpkio_cli/click_mods/default_last_command.py
+-rw-r--r--   0        0        0     5244 2023-06-08 08:20:08.800756 bpkio_cli-1.5.1/bpkio_cli/click_mods/group_rest_resource.py
+-rw-r--r--   0        0        0     1747 2023-06-05 14:52:28.915564 bpkio_cli-1.5.1/bpkio_cli/click_mods/option_eat_all.py
+-rw-r--r--   0        0        0      599 2023-06-05 14:52:28.916268 bpkio_cli-1.5.1/bpkio_cli/click_options/__init__.py
+-rw-r--r--   0        0        0      848 2023-06-05 14:52:28.916749 bpkio_cli-1.5.1/bpkio_cli/click_options/admin.py
+-rw-r--r--   0        0        0      355 2023-06-05 14:52:28.917214 bpkio_cli-1.5.1/bpkio_cli/click_options/json.py
+-rw-r--r--   0        0        0      958 2023-06-05 14:52:28.917874 bpkio_cli-1.5.1/bpkio_cli/click_options/list.py
+-rw-r--r--   0        0        0      933 2023-06-05 14:52:28.918220 bpkio_cli-1.5.1/bpkio_cli/click_options/poll.py
+-rw-r--r--   0        0        0      971 2023-06-14 20:16:02.846190 bpkio_cli-1.5.1/bpkio_cli/click_options/read.py
+-rw-r--r--   0        0        0     1183 2023-06-05 14:52:28.919379 bpkio_cli-1.5.1/bpkio_cli/click_options/search.py
+-rw-r--r--   0        0        0      445 2023-06-05 14:52:28.919891 bpkio_cli-1.5.1/bpkio_cli/click_options/table.py
+-rw-r--r--   0        0        0     1948 2023-06-14 20:13:13.594461 bpkio_cli-1.5.1/bpkio_cli/click_options/urls.py
+-rw-r--r--   0        0        0      656 2023-06-05 14:52:28.920820 bpkio_cli-1.5.1/bpkio_cli/commands/__init__.py
+-rw-r--r--   0        0        0      751 2023-06-07 16:02:26.119276 bpkio_cli-1.5.1/bpkio_cli/commands/addons.py
+-rw-r--r--   0        0        0     5246 2023-06-07 15:41:46.996745 bpkio_cli-1.5.1/bpkio_cli/commands/configure.py
+-rw-r--r--   0        0        0     1766 2023-06-07 15:41:46.997118 bpkio_cli-1.5.1/bpkio_cli/commands/consumption.py
+-rw-r--r--   0        0        0     4379 2023-06-07 15:41:46.997928 bpkio_cli-1.5.1/bpkio_cli/commands/creators/ad_insertion.py
+-rw-r--r--   0        0        0     7938 2023-06-14 20:04:47.510803 bpkio_cli-1.5.1/bpkio_cli/commands/creators/sources.py
+-rw-r--r--   0        0        0     4055 2023-06-07 15:41:46.999059 bpkio_cli-1.5.1/bpkio_cli/commands/creators/virtual_channel.py
+-rw-r--r--   0        0        0     8949 2023-06-09 12:53:03.155944 bpkio_cli-1.5.1/bpkio_cli/commands/creators/virtual_channel_populate.py
+-rw-r--r--   0        0        0      761 2023-06-05 14:52:28.924009 bpkio_cli-1.5.1/bpkio_cli/commands/hello.py
+-rw-r--r--   0        0        0     1251 2023-06-05 14:52:28.924268 bpkio_cli-1.5.1/bpkio_cli/commands/memory.py
+-rw-r--r--   0        0        0     3444 2023-06-07 15:41:46.999728 bpkio_cli-1.5.1/bpkio_cli/commands/package.py
+-rw-r--r--   0        0        0    10222 2023-06-22 10:43:19.457867 bpkio_cli-1.5.1/bpkio_cli/commands/profiles.py
+-rw-r--r--   0        0        0     2700 2023-06-05 14:52:28.925148 bpkio_cli-1.5.1/bpkio_cli/commands/recorder.py
+-rw-r--r--   0        0        0     3669 2023-06-05 14:52:28.925467 bpkio_cli-1.5.1/bpkio_cli/commands/services.py
+-rw-r--r--   0        0        0     5728 2023-06-07 15:41:47.000514 bpkio_cli-1.5.1/bpkio_cli/commands/sources.py
+-rw-r--r--   0        0        0    19382 2023-06-16 10:17:46.372444 bpkio_cli-1.5.1/bpkio_cli/commands/template_crud.py
+-rw-r--r--   0        0        0     7306 2023-06-05 14:52:28.926463 bpkio_cli-1.5.1/bpkio_cli/commands/template_crud_slots.py
+-rw-r--r--   0        0        0      332 2023-06-05 14:52:28.926844 bpkio_cli-1.5.1/bpkio_cli/commands/tenants.py
+-rw-r--r--   0        0        0     5799 2023-06-09 15:31:03.604764 bpkio_cli-1.5.1/bpkio_cli/commands/url.py
+-rw-r--r--   0        0        0      359 2023-06-05 14:52:28.927398 bpkio_cli-1.5.1/bpkio_cli/commands/users.py
+-rw-r--r--   0        0        0     1036 2023-06-05 14:52:28.927822 bpkio_cli-1.5.1/bpkio_cli/core/app_context.py
+-rw-r--r--   0        0        0     4556 2023-06-09 14:54:47.502096 bpkio_cli-1.5.1/bpkio_cli/core/config_provider.py
+-rw-r--r--   0        0        0      283 2023-06-09 10:01:38.442641 bpkio_cli-1.5.1/bpkio_cli/core/exceptions.py
+-rw-r--r--   0        0        0     2714 2023-06-09 11:12:30.963265 bpkio_cli-1.5.1/bpkio_cli/core/initialize.py
+-rw-r--r--   0        0        0     1718 2023-06-05 14:52:28.929630 bpkio_cli-1.5.1/bpkio_cli/core/logger.py
+-rw-r--r--   0        0        0     8332 2023-06-07 15:41:47.001439 bpkio_cli-1.5.1/bpkio_cli/core/packager.py
+-rw-r--r--   0        0        0     9526 2023-06-09 15:34:00.255674 bpkio_cli-1.5.1/bpkio_cli/core/resource_recorder.py
+-rw-r--r--   0        0        0     2204 2023-06-05 14:52:28.930943 bpkio_cli-1.5.1/bpkio_cli/core/resource_trail.py
+-rw-r--r--   0        0        0     5128 2023-06-05 14:52:28.931598 bpkio_cli-1.5.1/bpkio_cli/core/response_handler.py
+-rw-r--r--   0        0        0     1234 2023-06-05 14:52:28.931905 bpkio_cli-1.5.1/bpkio_cli/core/session_recorder.py
+-rw-r--r--   0        0        0      395 2023-06-05 14:52:28.932292 bpkio_cli-1.5.1/bpkio_cli/utils/__init__.py
+-rw-r--r--   0        0        0     2288 2023-06-05 14:52:28.932584 bpkio_cli-1.5.1/bpkio_cli/utils/arrays.py
+-rw-r--r--   0        0        0     1358 2023-06-05 14:52:28.932885 bpkio_cli-1.5.1/bpkio_cli/utils/datetimes.py
+-rw-r--r--   0        0        0     1828 2023-06-05 14:52:28.933224 bpkio_cli-1.5.1/bpkio_cli/utils/editor.py
+-rw-r--r--   0        0        0      494 2023-06-07 15:41:47.002131 bpkio_cli-1.5.1/bpkio_cli/utils/inquirer.py
+-rw-r--r--   0        0        0      136 2023-06-05 14:52:28.933905 bpkio_cli-1.5.1/bpkio_cli/utils/json.py
+-rw-r--r--   0        0        0      567 2023-06-05 14:52:28.934214 bpkio_cli-1.5.1/bpkio_cli/utils/profile_maker.py
+-rw-r--r--   0        0        0    14628 2023-06-14 20:04:47.517297 bpkio_cli-1.5.1/bpkio_cli/utils/url_builders.py
+-rw-r--r--   0        0        0      861 2023-06-05 14:52:28.934866 bpkio_cli-1.5.1/bpkio_cli/utils/urls.py
+-rw-r--r--   0        0        0     1034 2023-06-05 14:52:28.935214 bpkio_cli-1.5.1/bpkio_cli/writers/breadcrumbs.py
+-rw-r--r--   0        0        0     1667 2023-06-07 15:41:47.003003 bpkio_cli-1.5.1/bpkio_cli/writers/colorizer.py
+-rw-r--r--   0        0        0     5213 2023-06-09 10:05:20.541841 bpkio_cli-1.5.1/bpkio_cli/writers/content_display.py
+-rw-r--r--   0        0        0      840 2023-06-05 14:52:28.936348 bpkio_cli-1.5.1/bpkio_cli/writers/diff.py
+-rw-r--r--   0        0        0      751 2023-06-07 15:41:47.003793 bpkio_cli-1.5.1/bpkio_cli/writers/formatter.py
+-rw-r--r--   0        0        0     5729 2023-06-09 10:04:01.517494 bpkio_cli-1.5.1/bpkio_cli/writers/hls_formatter.py
+-rw-r--r--   0        0        0      714 2023-06-05 14:52:28.938409 bpkio_cli-1.5.1/bpkio_cli/writers/json_formatter.py
+-rw-r--r--   0        0        0     1658 2023-06-09 14:52:25.540620 bpkio_cli-1.5.1/bpkio_cli/writers/players.py
+-rw-r--r--   0        0        0     1631 2023-06-07 15:41:47.004793 bpkio_cli-1.5.1/bpkio_cli/writers/scte35.py
+-rw-r--r--   0        0        0     1865 2023-06-05 14:52:28.939530 bpkio_cli-1.5.1/bpkio_cli/writers/tables.py
+-rw-r--r--   0        0        0     5741 2023-06-09 10:03:51.584951 bpkio_cli-1.5.1/bpkio_cli/writers/xml_formatter.py
+-rw-r--r--   0        0        0     1242 2023-06-22 10:44:02.485077 bpkio_cli-1.5.1/pyproject.toml
+-rw-r--r--   0        0        0      972 1970-01-01 00:00:00.000000 bpkio_cli-1.5.1/PKG-INFO
```

### Comparing `bpkio_cli-1.5.0/bpkio_cli/app.py` & `bpkio_cli-1.5.1/bpkio_cli/app.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # from __future__ import absolute_import
 
 import logging
 
 import click
 import cloup
+from cloup.formatting.sep import Hline, RowSepIf, multiline_rows_are_at_least
 
 import bpkio_cli.commands as commands
 from bpkio_cli.click_mods.default_last_command import DefaultLastCommandGroup
 from bpkio_cli.commands.configure import init
-from bpkio_cli.core.config_provider import ConfigProvider
 from bpkio_cli.core.initialize import initialize
 from bpkio_cli.core.logger import (
     get_child_logger,
     get_level_names,
     set_console_logging_level,
 )
 from bpkio_cli.writers.breadcrumbs import display_tenant_info
@@ -20,15 +20,17 @@
 logger = get_child_logger("cli")
 
 LOG_LEVEL = None
 LOG_SDK = False
 
 
 SETTINGS = cloup.Context.settings(
-    formatter_settings=cloup.HelpFormatter.settings(theme=cloup.HelpTheme.dark())
+    formatter_settings=cloup.HelpFormatter.settings(
+        theme=cloup.HelpTheme.dark(), max_width=120
+    )
 )
 
 
 @cloup.group(
     show_subcommand_aliases=True, context_settings=SETTINGS, cls=DefaultLastCommandGroup
 )
 @click.version_option(
```

### Comparing `bpkio_cli-1.5.0/bpkio_cli/click_mods/default_last_command.py` & `bpkio_cli-1.5.1/bpkio_cli/click_mods/default_last_command.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.5.0/bpkio_cli/click_mods/group_rest_resource.py` & `bpkio_cli-1.5.1/bpkio_cli/click_mods/group_rest_resource.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.5.0/bpkio_cli/click_mods/option_eat_all.py` & `bpkio_cli-1.5.1/bpkio_cli/click_mods/option_eat_all.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.5.0/bpkio_cli/click_options/__init__.py` & `bpkio_cli-1.5.1/bpkio_cli/click_options/__init__.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.5.0/bpkio_cli/click_options/admin.py` & `bpkio_cli-1.5.1/bpkio_cli/click_options/admin.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.5.0/bpkio_cli/click_options/list.py` & `bpkio_cli-1.5.1/bpkio_cli/click_options/list.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.5.0/bpkio_cli/click_options/poll.py` & `bpkio_cli-1.5.1/bpkio_cli/click_options/poll.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.5.0/bpkio_cli/click_options/read.py` & `bpkio_cli-1.5.1/bpkio_cli/click_options/read.py`

 * *Files 25% similar despite different names*

```diff
@@ -8,25 +8,25 @@
     @click.option(
         "--raw",
         is_flag=True,
         type=bool,
         default=False,
         help="Get the raw content, unchanged",
     )
-    @click.option(
-        "--top", type=int, default=0, help="Only display the first N lines"
-    )
-    @click.option(
-        "--tail", type=int, default=0, help="Only display the last N lines"
-    )
+    @click.option("--top", type=int, default=0, help="Only display the first N lines")
+    @click.option("--tail", type=int, default=0, help="Only display the last N lines")
     @click.option(
         "--pager/--no-pager",
         type=bool,
         is_flag=True,
         default=None,
-        help="Display through a pager (to allow scrolling). If the flag is not set, a pager will automatically be used if the content is too long to fit on screen",
+        help="Display through a pager (to allow scrolling). "
+        + "If the flag is not set, a pager will automatically be used if the content "
+        + "is too long to fit on screen. "
+        + "In the pager, use keyboard shortcuts to navigate and search; "
+        + "type `h` for help on available shortcuts"
     )
     @functools.wraps(fn)
     def wrapper(*args, **kwargs):
         return fn(*args, **kwargs)
 
     return wrapper
```

### Comparing `bpkio_cli-1.5.0/bpkio_cli/click_options/search.py` & `bpkio_cli-1.5.1/bpkio_cli/click_options/search.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.5.0/bpkio_cli/click_options/urls.py` & `bpkio_cli-1.5.1/bpkio_cli/click_options/urls.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,20 @@
 # Common parameters for READ and POLL
 def url_options(fn):
     @click.option(
         "-s",
         "--sub",
         type=int,
         default=None,
-        help="For HLS, read a sub-playlist (by index - as given by the `read ID --table` option with the main playlist)",
+        is_flag=False,
+        flag_value="1",
+        help="For formats that contain links to child / related payloads, "
+        + "read a child instead (by index - as listed by the `read --table` command) "
+        + "Leave empty defaults to the first one. "
+        + "This option is primarily for use with HLS and VMAP formats.",
     )
     @click.option(
         "-u",
         "--url",
         type=str,
         default=None,
         help="Full URL of URL sub-path (for asset catalogs) to fetch",
```

### Comparing `bpkio_cli-1.5.0/bpkio_cli/commands/__init__.py` & `bpkio_cli-1.5.1/bpkio_cli/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.5.0/bpkio_cli/commands/addons.py` & `bpkio_cli-1.5.1/bpkio_cli/commands/addons.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.5.0/bpkio_cli/commands/configure.py` & `bpkio_cli-1.5.1/bpkio_cli/commands/configure.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.5.0/bpkio_cli/commands/consumption.py` & `bpkio_cli-1.5.1/bpkio_cli/commands/consumption.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.5.0/bpkio_cli/commands/creators/ad_insertion.py` & `bpkio_cli-1.5.1/bpkio_cli/commands/creators/ad_insertion.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.5.0/bpkio_cli/commands/creators/sources.py` & `bpkio_cli-1.5.1/bpkio_cli/commands/creators/sources.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,15 +123,15 @@
     parts = url.split("?")
 
     if len(parts) == 1:
         parts.append("")
 
     queries = parts[1]
 
-    if assist:
+    if len(queries) and assist:
         updated_queries = []
         for p in queries.split("&"):
             (k, val) = p.split("=")
             original_val = val
 
             # Suggest replacement for query parameters
             treatment = inquirer.fuzzy(
```

### Comparing `bpkio_cli-1.5.0/bpkio_cli/commands/creators/virtual_channel.py` & `bpkio_cli-1.5.1/bpkio_cli/commands/creators/virtual_channel.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.5.0/bpkio_cli/commands/creators/virtual_channel_populate.py` & `bpkio_cli-1.5.1/bpkio_cli/commands/creators/virtual_channel_populate.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.5.0/bpkio_cli/commands/hello.py` & `bpkio_cli-1.5.1/bpkio_cli/commands/hello.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.5.0/bpkio_cli/commands/memory.py` & `bpkio_cli-1.5.1/bpkio_cli/commands/memory.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.5.0/bpkio_cli/commands/package.py` & `bpkio_cli-1.5.1/bpkio_cli/commands/package.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.5.0/bpkio_cli/commands/profiles.py` & `bpkio_cli-1.5.1/bpkio_cli/commands/profiles.py`

 * *Files 0% similar despite different names*

```diff
@@ -259,15 +259,15 @@
 
     out_profile = create_profile_as_admin(tpro, tenant)
 
     obj.response_handler.treat_single_resource(out_profile)
 
 
 # --- UPDATE Command
-@cloup.command(aliases=["put"], help="[ADMIN] Update a Transcoding Profile")
+@cloup.command(aliases=["put", "edit"], help="[ADMIN] Update a Transcoding Profile")
 @click.option(
     "-c",
     "--content",
     "content_only",
     is_flag=True,
     default=False,
     help="Update the content of the profile, as a JSON payload",
```

### Comparing `bpkio_cli-1.5.0/bpkio_cli/commands/recorder.py` & `bpkio_cli-1.5.1/bpkio_cli/commands/recorder.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.5.0/bpkio_cli/commands/services.py` & `bpkio_cli-1.5.1/bpkio_cli/commands/services.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.5.0/bpkio_cli/commands/sources.py` & `bpkio_cli-1.5.1/bpkio_cli/commands/sources.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.5.0/bpkio_cli/commands/template_crud.py` & `bpkio_cli-1.5.1/bpkio_cli/commands/template_crud.py`

 * *Files 0% similar despite different names*

```diff
@@ -118,16 +118,16 @@
         resource_class=resource_class,
     )
     @cloup.argument(
         "id",
         metavar=f"<{name.replace('-', '_')}_id>",
         help=(
             f"The identifier of the {resource_title} to work with. "
-            f"Leave empty for commands operating on a list of {resource_title}s."
-            "You can use $ and @ notation to refer to previously selected resources"
+            f"Leave empty for commands operating on a list of {resource_title}s. "
+            "You can use $ and @ notation to refer to previously selected resources."
         ),
     )
     @click.pass_context
     @SessionRecorder.do_not_record
     def resource_group(ctx, id):
         if id:
             resource = retrieve_resource(id)
@@ -222,15 +222,15 @@
 
         # remove from cache
         ctx.obj.cache.remove(resource)
 
         click.secho(f"Resource {resource.id} deleted", fg="green")
 
     # --- UPDATE Command
-    @cloup.command(aliases=["put"], help=f"Update a {resource_title}")
+    @cloup.command(aliases=["put", "edit"], help=f"Update a {resource_title}")
     @click.pass_context
     def update(ctx):
         resource = retrieve_resource()
         resource_id = resource.id
 
         # remap to an input model
         resource = mappings.to_input_model(resource)
```

### Comparing `bpkio_cli-1.5.0/bpkio_cli/commands/template_crud_slots.py` & `bpkio_cli-1.5.1/bpkio_cli/commands/template_crud_slots.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.5.0/bpkio_cli/commands/url.py` & `bpkio_cli-1.5.1/bpkio_cli/commands/url.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.5.0/bpkio_cli/core/app_context.py` & `bpkio_cli-1.5.1/bpkio_cli/core/app_context.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.5.0/bpkio_cli/core/config_provider.py` & `bpkio_cli-1.5.1/bpkio_cli/core/config_provider.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.5.0/bpkio_cli/core/initialize.py` & `bpkio_cli-1.5.1/bpkio_cli/core/initialize.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.5.0/bpkio_cli/core/logger.py` & `bpkio_cli-1.5.1/bpkio_cli/core/logger.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.5.0/bpkio_cli/core/packager.py` & `bpkio_cli-1.5.1/bpkio_cli/core/packager.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.5.0/bpkio_cli/core/resource_recorder.py` & `bpkio_cli-1.5.1/bpkio_cli/core/resource_recorder.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.5.0/bpkio_cli/core/resource_trail.py` & `bpkio_cli-1.5.1/bpkio_cli/core/resource_trail.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.5.0/bpkio_cli/core/response_handler.py` & `bpkio_cli-1.5.1/bpkio_cli/core/response_handler.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.5.0/bpkio_cli/core/session_recorder.py` & `bpkio_cli-1.5.1/bpkio_cli/core/session_recorder.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.5.0/bpkio_cli/utils/arrays.py` & `bpkio_cli-1.5.1/bpkio_cli/utils/arrays.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.5.0/bpkio_cli/utils/datetimes.py` & `bpkio_cli-1.5.1/bpkio_cli/utils/datetimes.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.5.0/bpkio_cli/utils/editor.py` & `bpkio_cli-1.5.1/bpkio_cli/utils/editor.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.5.0/bpkio_cli/utils/profile_maker.py` & `bpkio_cli-1.5.1/bpkio_cli/utils/profile_maker.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.5.0/bpkio_cli/utils/url_builders.py` & `bpkio_cli-1.5.1/bpkio_cli/utils/url_builders.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,15 +158,18 @@
                 k = (parts[0],)
                 val = "=".join(parts[1:])
 
             if val.startswith("$arg_"):
                 input_param = val.replace("$arg_", "")
                 # determine output param name
                 if for_service:
-                    param_to_fill = input_param
+                    if input_param in ["serviceid", "sessionid"]:
+                        continue
+                    else:
+                        param_to_fill = input_param
                 else:
                     param_to_fill = k
 
                 cached_values = metadata_cache.get_metadata(adserver, input_param)
 
                 if k in existing_params:
                     cached_values.insert(0, existing_params[k])
```

### Comparing `bpkio_cli-1.5.0/bpkio_cli/utils/urls.py` & `bpkio_cli-1.5.1/bpkio_cli/utils/urls.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.5.0/bpkio_cli/writers/breadcrumbs.py` & `bpkio_cli-1.5.1/bpkio_cli/writers/breadcrumbs.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.5.0/bpkio_cli/writers/colorizer.py` & `bpkio_cli-1.5.1/bpkio_cli/writers/colorizer.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.5.0/bpkio_cli/writers/content_display.py` & `bpkio_cli-1.5.1/bpkio_cli/writers/content_display.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.5.0/bpkio_cli/writers/diff.py` & `bpkio_cli-1.5.1/bpkio_cli/writers/diff.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.5.0/bpkio_cli/writers/formatter.py` & `bpkio_cli-1.5.1/bpkio_cli/writers/formatter.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.5.0/bpkio_cli/writers/hls_formatter.py` & `bpkio_cli-1.5.1/bpkio_cli/writers/hls_formatter.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.5.0/bpkio_cli/writers/json_formatter.py` & `bpkio_cli-1.5.1/bpkio_cli/writers/json_formatter.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.5.0/bpkio_cli/writers/players.py` & `bpkio_cli-1.5.1/bpkio_cli/writers/players.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.5.0/bpkio_cli/writers/scte35.py` & `bpkio_cli-1.5.1/bpkio_cli/writers/scte35.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.5.0/bpkio_cli/writers/tables.py` & `bpkio_cli-1.5.1/bpkio_cli/writers/tables.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.5.0/bpkio_cli/writers/xml_formatter.py` & `bpkio_cli-1.5.1/bpkio_cli/writers/xml_formatter.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.5.0/pyproject.toml` & `bpkio_cli-1.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bpkio-cli"
-version = "1.5.0"
+version = "1.5.1"
 description = "A command line interface to the broadpeak.io APIs, with additional helpers"
 authors = ["Fabre Lambeau <fabre.lambeau@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "bpkio_cli" }]
 
 [tool.poetry-dynamic-versioning]
 enable = true
```

### Comparing `bpkio_cli-1.5.0/PKG-INFO` & `bpkio_cli-1.5.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bpkio-cli
-Version: 1.5.0
+Version: 1.5.1
 Summary: A command line interface to the broadpeak.io APIs, with additional helpers
 Author: Fabre Lambeau
 Author-email: fabre.lambeau@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

