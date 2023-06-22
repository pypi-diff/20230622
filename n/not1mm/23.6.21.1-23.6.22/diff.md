# Comparing `tmp/not1mm-23.6.21.1.tar.gz` & `tmp/not1mm-23.6.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "not1mm-23.6.21.1.tar", last modified: Wed Jun 21 20:55:27 2023, max compression
+gzip compressed data, was "not1mm-23.6.22.tar", last modified: Thu Jun 22 21:25:07 2023, max compression
```

## Comparing `not1mm-23.6.21.1.tar` & `not1mm-23.6.22.tar`

### file list

```diff
@@ -1,142 +1,142 @@
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-21 20:55:27.985357 not1mm-23.6.21.1/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35149 2022-05-05 15:15:13.000000 not1mm-23.6.21.1/LICENSE
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    23206 2023-06-21 20:55:27.985357 not1mm-23.6.21.1/PKG-INFO
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    22458 2023-06-21 19:46:29.000000 not1mm-23.6.21.1/README.md
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-21 20:55:27.874356 not1mm-23.6.21.1/not1mm/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2022-11-03 15:04:39.000000 not1mm-23.6.21.1/not1mm/__init__.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    95077 2023-06-21 20:50:27.000000 not1mm-23.6.21.1/not1mm/__main__.py
--rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)    25525 2023-06-01 00:41:28.000000 not1mm-23.6.21.1/not1mm/bandmap.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-21 20:55:27.938356 not1mm-23.6.21.1/not1mm/data/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   203952 2023-01-27 16:44:51.000000 not1mm-23.6.21.1/not1mm/data/JetBrainsMono-Regular.ttf
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   635340 2023-06-17 01:32:08.000000 not1mm-23.6.21.1/not1mm/data/MASTER.SCP
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2067 2023-05-18 23:48:17.000000 not1mm-23.6.21.1/not1mm/data/about.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      224 2023-04-18 03:49:58.000000 not1mm-23.6.21.1/not1mm/data/alpha bravo charlie delta.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     5246 2023-05-01 15:41:16.000000 not1mm-23.6.21.1/not1mm/data/bandmap.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      387 2023-03-15 16:56:38.000000 not1mm-23.6.21.1/not1mm/data/check.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    41522 2023-05-23 20:03:51.000000 not1mm-23.6.21.1/not1mm/data/configuration.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    89307 2023-03-07 17:30:38.000000 not1mm-23.6.21.1/not1mm/data/contests.sql
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)  7127932 2023-06-21 20:52:19.000000 not1mm-23.6.21.1/not1mm/data/cty.json
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      451 2023-04-11 19:54:10.000000 not1mm-23.6.21.1/not1mm/data/cwmacros.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      116 2023-06-20 14:51:41.000000 not1mm-23.6.21.1/not1mm/data/donors.html
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    19280 2023-03-20 20:22:09.000000 not1mm-23.6.21.1/not1mm/data/editcontact.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2273 2023-02-21 14:39:24.000000 not1mm-23.6.21.1/not1mm/data/editmacro.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      474 2023-02-10 02:42:18.000000 not1mm-23.6.21.1/not1mm/data/greendot.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      205 2023-02-09 20:47:40.000000 not1mm-23.6.21.1/not1mm/data/k6gte-not1mm.desktop
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4010 2023-02-09 20:45:38.000000 not1mm-23.6.21.1/not1mm/data/k6gte.not1mm-128.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1108 2023-02-09 20:45:03.000000 not1mm-23.6.21.1/not1mm/data/k6gte.not1mm-32.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2152 2023-02-09 20:45:22.000000 not1mm-23.6.21.1/not1mm/data/k6gte.not1mm-64.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      970 2023-03-23 20:14:51.000000 not1mm-23.6.21.1/not1mm/data/logwindow.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    44985 2023-06-21 19:42:00.000000 not1mm-23.6.21.1/not1mm/data/main.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    17963 2023-05-05 12:59:56.000000 not1mm-23.6.21.1/not1mm/data/new_contest.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    20129 2023-06-17 01:47:05.000000 not1mm-23.6.21.1/not1mm/data/not1mm.html
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2018 2023-02-12 17:56:36.000000 not1mm-23.6.21.1/not1mm/data/opon.ui
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-21 20:55:27.970357 not1mm-23.6.21.1/not1mm/data/phonetics/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    42590 2023-04-21 20:24:24.000000 not1mm-23.6.21.1/not1mm/data/phonetics/0.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    30248 2023-04-21 20:25:33.000000 not1mm-23.6.21.1/not1mm/data/phonetics/1.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    29584 2023-04-21 20:27:16.000000 not1mm-23.6.21.1/not1mm/data/phonetics/2.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    32072 2023-04-21 20:29:07.000000 not1mm-23.6.21.1/not1mm/data/phonetics/3.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43052 2023-04-21 20:29:49.000000 not1mm-23.6.21.1/not1mm/data/phonetics/4.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    51976 2023-04-21 21:46:26.000000 not1mm-23.6.21.1/not1mm/data/phonetics/5.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    58634 2023-04-21 21:08:45.000000 not1mm-23.6.21.1/not1mm/data/phonetics/6.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    49154 2023-04-21 21:10:50.000000 not1mm-23.6.21.1/not1mm/data/phonetics/7.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    32842 2023-04-21 21:13:51.000000 not1mm-23.6.21.1/not1mm/data/phonetics/73.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35636 2023-04-21 21:11:40.000000 not1mm-23.6.21.1/not1mm/data/phonetics/8.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    39592 2023-04-21 21:12:32.000000 not1mm-23.6.21.1/not1mm/data/phonetics/9.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46800 2023-04-21 21:14:36.000000 not1mm-23.6.21.1/not1mm/data/phonetics/a.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    44594 2023-04-21 21:15:20.000000 not1mm-23.6.21.1/not1mm/data/phonetics/again.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    40976 2023-04-21 21:16:10.000000 not1mm-23.6.21.1/not1mm/data/phonetics/b.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46746 2023-04-21 21:17:07.000000 not1mm-23.6.21.1/not1mm/data/phonetics/c.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    62558 2023-04-21 13:38:05.000000 not1mm-23.6.21.1/not1mm/data/phonetics/contest.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    92498 2023-04-21 21:17:54.000000 not1mm-23.6.21.1/not1mm/data/phonetics/cq.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    52524 2023-04-21 21:18:24.000000 not1mm-23.6.21.1/not1mm/data/phonetics/d.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    45700 2023-04-21 21:19:02.000000 not1mm-23.6.21.1/not1mm/data/phonetics/e.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    53438 2023-04-21 21:19:38.000000 not1mm-23.6.21.1/not1mm/data/phonetics/f.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    42766 2023-04-21 21:20:18.000000 not1mm-23.6.21.1/not1mm/data/phonetics/g.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    50040 2023-04-21 21:21:03.000000 not1mm-23.6.21.1/not1mm/data/phonetics/h.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46372 2023-04-21 21:23:33.000000 not1mm-23.6.21.1/not1mm/data/phonetics/i.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43434 2023-04-21 21:24:12.000000 not1mm-23.6.21.1/not1mm/data/phonetics/j.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    49066 2023-04-21 21:24:57.000000 not1mm-23.6.21.1/not1mm/data/phonetics/k.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   185562 2023-04-21 21:25:43.000000 not1mm-23.6.21.1/not1mm/data/phonetics/k6gte.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43154 2023-04-21 21:26:21.000000 not1mm-23.6.21.1/not1mm/data/phonetics/l.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    54352 2023-04-21 21:27:07.000000 not1mm-23.6.21.1/not1mm/data/phonetics/m.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56798 2023-04-21 21:27:57.000000 not1mm-23.6.21.1/not1mm/data/phonetics/mynumber.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    52204 2023-04-21 21:28:42.000000 not1mm-23.6.21.1/not1mm/data/phonetics/n.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   154544 2023-04-21 21:29:54.000000 not1mm-23.6.21.1/not1mm/data/phonetics/nil.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    47440 2023-04-21 21:30:37.000000 not1mm-23.6.21.1/not1mm/data/phonetics/o.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    38300 2023-04-21 21:31:22.000000 not1mm-23.6.21.1/not1mm/data/phonetics/p.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    55288 2023-04-21 21:31:58.000000 not1mm-23.6.21.1/not1mm/data/phonetics/q.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    47432 2023-04-21 21:32:39.000000 not1mm-23.6.21.1/not1mm/data/phonetics/r.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46122 2023-04-21 21:33:20.000000 not1mm-23.6.21.1/not1mm/data/phonetics/roger.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    60698 2023-04-21 21:33:59.000000 not1mm-23.6.21.1/not1mm/data/phonetics/s.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    70424 2023-04-17 20:43:04.000000 not1mm-23.6.21.1/not1mm/data/phonetics/space.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    58196 2023-04-21 21:35:28.000000 not1mm-23.6.21.1/not1mm/data/phonetics/t.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56320 2023-04-21 21:36:54.000000 not1mm-23.6.21.1/not1mm/data/phonetics/thankyou.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    94980 2023-04-21 21:37:27.000000 not1mm-23.6.21.1/not1mm/data/phonetics/thankyouqrz.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    65922 2023-04-21 21:38:05.000000 not1mm-23.6.21.1/not1mm/data/phonetics/u.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    50142 2023-04-21 21:38:37.000000 not1mm-23.6.21.1/not1mm/data/phonetics/v.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    37638 2023-04-21 21:39:21.000000 not1mm-23.6.21.1/not1mm/data/phonetics/w.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    61870 2023-04-21 21:40:02.000000 not1mm-23.6.21.1/not1mm/data/phonetics/x.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56524 2023-04-21 21:40:40.000000 not1mm-23.6.21.1/not1mm/data/phonetics/y.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46510 2023-04-21 21:41:22.000000 not1mm-23.6.21.1/not1mm/data/phonetics/yourcall.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    51768 2023-04-21 21:41:59.000000 not1mm-23.6.21.1/not1mm/data/phonetics/z.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1600 2023-04-03 14:20:44.000000 not1mm-23.6.21.1/not1mm/data/pickcontest.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      565 2023-02-10 02:42:40.000000 not1mm-23.6.21.1/not1mm/data/reddot.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35566 2023-04-15 16:43:11.000000 not1mm-23.6.21.1/not1mm/data/settings.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      470 2023-04-18 18:00:45.000000 not1mm-23.6.21.1/not1mm/data/ssbmacros.txt
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-21 20:55:27.976357 not1mm-23.6.21.1/not1mm/lib/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2022-11-03 15:04:39.000000 not1mm-23.6.21.1/not1mm/lib/__init__.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      379 2023-04-10 20:24:21.000000 not1mm-23.6.21.1/not1mm/lib/about.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    15676 2023-05-22 20:40:03.000000 not1mm-23.6.21.1/not1mm/lib/cat_interface.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3123 2023-05-11 20:24:55.000000 not1mm-23.6.21.1/not1mm/lib/cwinterface.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    34356 2023-05-24 20:24:28.000000 not1mm-23.6.21.1/not1mm/lib/database.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      357 2023-03-20 13:17:21.000000 not1mm-23.6.21.1/not1mm/lib/edit_contact.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      559 2023-03-06 17:59:31.000000 not1mm-23.6.21.1/not1mm/lib/edit_macro.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      363 2023-03-06 18:02:53.000000 not1mm-23.6.21.1/not1mm/lib/edit_opon.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1973 2023-04-11 17:58:02.000000 not1mm-23.6.21.1/not1mm/lib/edit_station.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     8760 2023-04-05 20:29:02.000000 not1mm-23.6.21.1/not1mm/lib/ham_utility.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13916 2023-03-07 18:49:31.000000 not1mm-23.6.21.1/not1mm/lib/lookup.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1761 2023-05-12 16:20:09.000000 not1mm-23.6.21.1/not1mm/lib/multicast.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     5713 2023-05-24 14:24:14.000000 not1mm-23.6.21.1/not1mm/lib/n1mm.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      354 2023-03-28 20:21:24.000000 not1mm-23.6.21.1/not1mm/lib/new_contest.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      363 2023-03-31 21:22:27.000000 not1mm-23.6.21.1/not1mm/lib/select_contest.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     6885 2023-05-23 19:07:39.000000 not1mm-23.6.21.1/not1mm/lib/settings.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       47 2023-06-21 19:45:17.000000 not1mm-23.6.21.1/not1mm/lib/version.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1286 2023-05-19 19:40:38.000000 not1mm-23.6.21.1/not1mm/lib/versiontest.py
--rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)    33732 2023-05-30 16:14:11.000000 not1mm-23.6.21.1/not1mm/logwindow.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-21 20:55:27.982357 not1mm-23.6.21.1/not1mm/plugins/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13883 2023-05-29 18:30:11.000000 not1mm-23.6.21.1/not1mm/plugins/10_10_fall_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13888 2023-05-29 18:30:48.000000 not1mm-23.6.21.1/not1mm/plugins/10_10_spring_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13895 2023-05-29 18:31:29.000000 not1mm-23.6.21.1/not1mm/plugins/10_10_summer_phone.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13898 2023-05-29 18:31:57.000000 not1mm-23.6.21.1/not1mm/plugins/10_10_winter_phone.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2023-02-20 21:20:03.000000 not1mm-23.6.21.1/not1mm/plugins/__init__.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14684 2023-05-29 18:32:51.000000 not1mm-23.6.21.1/not1mm/plugins/arrl_dx_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14687 2023-05-29 18:33:05.000000 not1mm-23.6.21.1/not1mm/plugins/arrl_dx_ssb.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13125 2023-05-29 18:33:21.000000 not1mm-23.6.21.1/not1mm/plugins/arrl_field_day.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2860 2023-05-05 16:10:11.000000 not1mm-23.6.21.1/not1mm/plugins/arrl_rtty_ru.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    16077 2023-05-29 18:33:47.000000 not1mm-23.6.21.1/not1mm/plugins/arrl_ss_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    16082 2023-05-29 18:34:01.000000 not1mm-23.6.21.1/not1mm/plugins/arrl_ss_phone.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    15301 2023-05-29 18:25:56.000000 not1mm-23.6.21.1/not1mm/plugins/cq_wpx_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    15323 2023-05-29 18:34:21.000000 not1mm-23.6.21.1/not1mm/plugins/cq_wpx_ssb.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14031 2023-05-29 18:34:36.000000 not1mm-23.6.21.1/not1mm/plugins/cq_ww_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14035 2023-05-29 18:34:53.000000 not1mm-23.6.21.1/not1mm/plugins/cq_ww_ssb.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14890 2023-05-29 18:35:16.000000 not1mm-23.6.21.1/not1mm/plugins/cwt.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     7453 2023-05-05 16:10:58.000000 not1mm-23.6.21.1/not1mm/plugins/general_logging.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13854 2023-05-05 16:10:55.000000 not1mm-23.6.21.1/not1mm/plugins/jidx_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13855 2023-05-05 16:10:48.000000 not1mm-23.6.21.1/not1mm/plugins/jidx_ph.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3121 2023-05-05 16:11:15.000000 not1mm-23.6.21.1/not1mm/plugins/winter_field_day.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-21 20:55:27.984357 not1mm-23.6.21.1/not1mm/testing/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2083 2023-05-19 23:10:32.000000 not1mm-23.6.21.1/not1mm/testing/fakeflrig.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1658 2023-05-19 17:23:54.000000 not1mm-23.6.21.1/not1mm/testing/flrigclient.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1099 2023-05-24 18:38:16.000000 not1mm-23.6.21.1/not1mm/testing/n1mm_listener.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1660 2023-05-14 06:26:14.000000 not1mm-23.6.21.1/not1mm/testing/test.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-21 20:55:27.884356 not1mm-23.6.21.1/not1mm.egg-info/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    23206 2023-06-21 20:55:27.000000 not1mm-23.6.21.1/not1mm.egg-info/PKG-INFO
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3581 2023-06-21 20:55:27.000000 not1mm-23.6.21.1/not1mm.egg-info/SOURCES.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        1 2023-06-21 20:55:27.000000 not1mm-23.6.21.1/not1mm.egg-info/dependency_links.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       47 2023-06-21 20:55:27.000000 not1mm-23.6.21.1/not1mm.egg-info/entry_points.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       92 2023-06-21 20:55:27.000000 not1mm-23.6.21.1/not1mm.egg-info/requires.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       33 2023-06-21 20:55:27.000000 not1mm-23.6.21.1/not1mm.egg-info/top_level.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1274 2023-06-21 20:54:10.000000 not1mm-23.6.21.1/pyproject.toml
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       38 2023-06-21 20:55:27.985357 not1mm-23.6.21.1/setup.cfg
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-21 20:55:27.984357 not1mm-23.6.21.1/testing/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      176 2023-05-31 20:52:45.000000 not1mm-23.6.21.1/testing/test.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-22 21:25:07.033548 not1mm-23.6.22/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35149 2022-05-05 15:15:13.000000 not1mm-23.6.22/LICENSE
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    23204 2023-06-22 21:25:07.032548 not1mm-23.6.22/PKG-INFO
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    22458 2023-06-21 19:46:29.000000 not1mm-23.6.22/README.md
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-22 21:25:06.787546 not1mm-23.6.22/not1mm/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2022-11-03 15:04:39.000000 not1mm-23.6.22/not1mm/__init__.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    95150 2023-06-21 21:06:11.000000 not1mm-23.6.22/not1mm/__main__.py
+-rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)    25525 2023-06-01 00:41:28.000000 not1mm-23.6.22/not1mm/bandmap.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-22 21:25:06.887546 not1mm-23.6.22/not1mm/data/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   203952 2023-01-27 16:44:51.000000 not1mm-23.6.22/not1mm/data/JetBrainsMono-Regular.ttf
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   635340 2023-06-17 01:32:08.000000 not1mm-23.6.22/not1mm/data/MASTER.SCP
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2067 2023-05-18 23:48:17.000000 not1mm-23.6.22/not1mm/data/about.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      224 2023-04-18 03:49:58.000000 not1mm-23.6.22/not1mm/data/alpha bravo charlie delta.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     5246 2023-05-01 15:41:16.000000 not1mm-23.6.22/not1mm/data/bandmap.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      387 2023-03-15 16:56:38.000000 not1mm-23.6.22/not1mm/data/check.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    41522 2023-05-23 20:03:51.000000 not1mm-23.6.22/not1mm/data/configuration.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    89307 2023-03-07 17:30:38.000000 not1mm-23.6.22/not1mm/data/contests.sql
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)  7127932 2023-06-21 20:52:19.000000 not1mm-23.6.22/not1mm/data/cty.json
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      451 2023-04-11 19:54:10.000000 not1mm-23.6.22/not1mm/data/cwmacros.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      116 2023-06-20 14:51:41.000000 not1mm-23.6.22/not1mm/data/donors.html
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    19280 2023-03-20 20:22:09.000000 not1mm-23.6.22/not1mm/data/editcontact.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2273 2023-02-21 14:39:24.000000 not1mm-23.6.22/not1mm/data/editmacro.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      474 2023-02-10 02:42:18.000000 not1mm-23.6.22/not1mm/data/greendot.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      205 2023-02-09 20:47:40.000000 not1mm-23.6.22/not1mm/data/k6gte-not1mm.desktop
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4010 2023-02-09 20:45:38.000000 not1mm-23.6.22/not1mm/data/k6gte.not1mm-128.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1108 2023-02-09 20:45:03.000000 not1mm-23.6.22/not1mm/data/k6gte.not1mm-32.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2152 2023-02-09 20:45:22.000000 not1mm-23.6.22/not1mm/data/k6gte.not1mm-64.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      970 2023-03-23 20:14:51.000000 not1mm-23.6.22/not1mm/data/logwindow.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    44985 2023-06-21 19:42:00.000000 not1mm-23.6.22/not1mm/data/main.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    17963 2023-05-05 12:59:56.000000 not1mm-23.6.22/not1mm/data/new_contest.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    20129 2023-06-17 01:47:05.000000 not1mm-23.6.22/not1mm/data/not1mm.html
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2018 2023-02-12 17:56:36.000000 not1mm-23.6.22/not1mm/data/opon.ui
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-22 21:25:07.004548 not1mm-23.6.22/not1mm/data/phonetics/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    42590 2023-04-21 20:24:24.000000 not1mm-23.6.22/not1mm/data/phonetics/0.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    30248 2023-04-21 20:25:33.000000 not1mm-23.6.22/not1mm/data/phonetics/1.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    29584 2023-04-21 20:27:16.000000 not1mm-23.6.22/not1mm/data/phonetics/2.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    32072 2023-04-21 20:29:07.000000 not1mm-23.6.22/not1mm/data/phonetics/3.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43052 2023-04-21 20:29:49.000000 not1mm-23.6.22/not1mm/data/phonetics/4.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    51976 2023-04-21 21:46:26.000000 not1mm-23.6.22/not1mm/data/phonetics/5.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    58634 2023-04-21 21:08:45.000000 not1mm-23.6.22/not1mm/data/phonetics/6.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    49154 2023-04-21 21:10:50.000000 not1mm-23.6.22/not1mm/data/phonetics/7.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    32842 2023-04-21 21:13:51.000000 not1mm-23.6.22/not1mm/data/phonetics/73.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35636 2023-04-21 21:11:40.000000 not1mm-23.6.22/not1mm/data/phonetics/8.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    39592 2023-04-21 21:12:32.000000 not1mm-23.6.22/not1mm/data/phonetics/9.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46800 2023-04-21 21:14:36.000000 not1mm-23.6.22/not1mm/data/phonetics/a.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    44594 2023-04-21 21:15:20.000000 not1mm-23.6.22/not1mm/data/phonetics/again.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    40976 2023-04-21 21:16:10.000000 not1mm-23.6.22/not1mm/data/phonetics/b.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46746 2023-04-21 21:17:07.000000 not1mm-23.6.22/not1mm/data/phonetics/c.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    62558 2023-04-21 13:38:05.000000 not1mm-23.6.22/not1mm/data/phonetics/contest.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    92498 2023-04-21 21:17:54.000000 not1mm-23.6.22/not1mm/data/phonetics/cq.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    52524 2023-04-21 21:18:24.000000 not1mm-23.6.22/not1mm/data/phonetics/d.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    45700 2023-04-21 21:19:02.000000 not1mm-23.6.22/not1mm/data/phonetics/e.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    53438 2023-04-21 21:19:38.000000 not1mm-23.6.22/not1mm/data/phonetics/f.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    42766 2023-04-21 21:20:18.000000 not1mm-23.6.22/not1mm/data/phonetics/g.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    50040 2023-04-21 21:21:03.000000 not1mm-23.6.22/not1mm/data/phonetics/h.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46372 2023-04-21 21:23:33.000000 not1mm-23.6.22/not1mm/data/phonetics/i.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43434 2023-04-21 21:24:12.000000 not1mm-23.6.22/not1mm/data/phonetics/j.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    49066 2023-04-21 21:24:57.000000 not1mm-23.6.22/not1mm/data/phonetics/k.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   185562 2023-04-21 21:25:43.000000 not1mm-23.6.22/not1mm/data/phonetics/k6gte.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43154 2023-04-21 21:26:21.000000 not1mm-23.6.22/not1mm/data/phonetics/l.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    54352 2023-04-21 21:27:07.000000 not1mm-23.6.22/not1mm/data/phonetics/m.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56798 2023-04-21 21:27:57.000000 not1mm-23.6.22/not1mm/data/phonetics/mynumber.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    52204 2023-04-21 21:28:42.000000 not1mm-23.6.22/not1mm/data/phonetics/n.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   154544 2023-04-21 21:29:54.000000 not1mm-23.6.22/not1mm/data/phonetics/nil.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    47440 2023-04-21 21:30:37.000000 not1mm-23.6.22/not1mm/data/phonetics/o.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    38300 2023-04-21 21:31:22.000000 not1mm-23.6.22/not1mm/data/phonetics/p.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    55288 2023-04-21 21:31:58.000000 not1mm-23.6.22/not1mm/data/phonetics/q.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    47432 2023-04-21 21:32:39.000000 not1mm-23.6.22/not1mm/data/phonetics/r.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46122 2023-04-21 21:33:20.000000 not1mm-23.6.22/not1mm/data/phonetics/roger.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    60698 2023-04-21 21:33:59.000000 not1mm-23.6.22/not1mm/data/phonetics/s.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    70424 2023-04-17 20:43:04.000000 not1mm-23.6.22/not1mm/data/phonetics/space.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    58196 2023-04-21 21:35:28.000000 not1mm-23.6.22/not1mm/data/phonetics/t.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56320 2023-04-21 21:36:54.000000 not1mm-23.6.22/not1mm/data/phonetics/thankyou.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    94980 2023-04-21 21:37:27.000000 not1mm-23.6.22/not1mm/data/phonetics/thankyouqrz.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    65922 2023-04-21 21:38:05.000000 not1mm-23.6.22/not1mm/data/phonetics/u.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    50142 2023-04-21 21:38:37.000000 not1mm-23.6.22/not1mm/data/phonetics/v.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    37638 2023-04-21 21:39:21.000000 not1mm-23.6.22/not1mm/data/phonetics/w.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    61870 2023-04-21 21:40:02.000000 not1mm-23.6.22/not1mm/data/phonetics/x.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56524 2023-04-21 21:40:40.000000 not1mm-23.6.22/not1mm/data/phonetics/y.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46510 2023-04-21 21:41:22.000000 not1mm-23.6.22/not1mm/data/phonetics/yourcall.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    51768 2023-04-21 21:41:59.000000 not1mm-23.6.22/not1mm/data/phonetics/z.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1600 2023-04-03 14:20:44.000000 not1mm-23.6.22/not1mm/data/pickcontest.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      565 2023-02-10 02:42:40.000000 not1mm-23.6.22/not1mm/data/reddot.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35566 2023-04-15 16:43:11.000000 not1mm-23.6.22/not1mm/data/settings.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      470 2023-04-18 18:00:45.000000 not1mm-23.6.22/not1mm/data/ssbmacros.txt
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-22 21:25:07.019548 not1mm-23.6.22/not1mm/lib/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2022-11-03 15:04:39.000000 not1mm-23.6.22/not1mm/lib/__init__.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      379 2023-04-10 20:24:21.000000 not1mm-23.6.22/not1mm/lib/about.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    15676 2023-05-22 20:40:03.000000 not1mm-23.6.22/not1mm/lib/cat_interface.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3123 2023-05-11 20:24:55.000000 not1mm-23.6.22/not1mm/lib/cwinterface.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    34356 2023-05-24 20:24:28.000000 not1mm-23.6.22/not1mm/lib/database.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      357 2023-03-20 13:17:21.000000 not1mm-23.6.22/not1mm/lib/edit_contact.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      559 2023-03-06 17:59:31.000000 not1mm-23.6.22/not1mm/lib/edit_macro.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      363 2023-03-06 18:02:53.000000 not1mm-23.6.22/not1mm/lib/edit_opon.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1973 2023-04-11 17:58:02.000000 not1mm-23.6.22/not1mm/lib/edit_station.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     8760 2023-04-05 20:29:02.000000 not1mm-23.6.22/not1mm/lib/ham_utility.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13916 2023-03-07 18:49:31.000000 not1mm-23.6.22/not1mm/lib/lookup.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1761 2023-05-12 16:20:09.000000 not1mm-23.6.22/not1mm/lib/multicast.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     5713 2023-05-24 14:24:14.000000 not1mm-23.6.22/not1mm/lib/n1mm.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      354 2023-03-28 20:21:24.000000 not1mm-23.6.22/not1mm/lib/new_contest.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      363 2023-03-31 21:22:27.000000 not1mm-23.6.22/not1mm/lib/select_contest.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     6885 2023-05-23 19:07:39.000000 not1mm-23.6.22/not1mm/lib/settings.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       47 2023-06-22 21:23:09.000000 not1mm-23.6.22/not1mm/lib/version.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1286 2023-05-19 19:40:38.000000 not1mm-23.6.22/not1mm/lib/versiontest.py
+-rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)    33732 2023-05-30 16:14:11.000000 not1mm-23.6.22/not1mm/logwindow.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-22 21:25:07.029548 not1mm-23.6.22/not1mm/plugins/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13883 2023-05-29 18:30:11.000000 not1mm-23.6.22/not1mm/plugins/10_10_fall_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13888 2023-05-29 18:30:48.000000 not1mm-23.6.22/not1mm/plugins/10_10_spring_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13895 2023-05-29 18:31:29.000000 not1mm-23.6.22/not1mm/plugins/10_10_summer_phone.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13898 2023-05-29 18:31:57.000000 not1mm-23.6.22/not1mm/plugins/10_10_winter_phone.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2023-02-20 21:20:03.000000 not1mm-23.6.22/not1mm/plugins/__init__.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14684 2023-05-29 18:32:51.000000 not1mm-23.6.22/not1mm/plugins/arrl_dx_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14687 2023-05-29 18:33:05.000000 not1mm-23.6.22/not1mm/plugins/arrl_dx_ssb.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13125 2023-05-29 18:33:21.000000 not1mm-23.6.22/not1mm/plugins/arrl_field_day.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2860 2023-05-05 16:10:11.000000 not1mm-23.6.22/not1mm/plugins/arrl_rtty_ru.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    16077 2023-05-29 18:33:47.000000 not1mm-23.6.22/not1mm/plugins/arrl_ss_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    16082 2023-05-29 18:34:01.000000 not1mm-23.6.22/not1mm/plugins/arrl_ss_phone.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    15301 2023-05-29 18:25:56.000000 not1mm-23.6.22/not1mm/plugins/cq_wpx_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    15323 2023-05-29 18:34:21.000000 not1mm-23.6.22/not1mm/plugins/cq_wpx_ssb.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14031 2023-05-29 18:34:36.000000 not1mm-23.6.22/not1mm/plugins/cq_ww_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14035 2023-05-29 18:34:53.000000 not1mm-23.6.22/not1mm/plugins/cq_ww_ssb.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14890 2023-05-29 18:35:16.000000 not1mm-23.6.22/not1mm/plugins/cwt.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     7453 2023-05-05 16:10:58.000000 not1mm-23.6.22/not1mm/plugins/general_logging.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13854 2023-05-05 16:10:55.000000 not1mm-23.6.22/not1mm/plugins/jidx_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13855 2023-05-05 16:10:48.000000 not1mm-23.6.22/not1mm/plugins/jidx_ph.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3121 2023-05-05 16:11:15.000000 not1mm-23.6.22/not1mm/plugins/winter_field_day.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-22 21:25:07.031548 not1mm-23.6.22/not1mm/testing/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2083 2023-05-19 23:10:32.000000 not1mm-23.6.22/not1mm/testing/fakeflrig.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1658 2023-05-19 17:23:54.000000 not1mm-23.6.22/not1mm/testing/flrigclient.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1099 2023-05-24 18:38:16.000000 not1mm-23.6.22/not1mm/testing/n1mm_listener.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1660 2023-05-14 06:26:14.000000 not1mm-23.6.22/not1mm/testing/test.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-22 21:25:06.792545 not1mm-23.6.22/not1mm.egg-info/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    23204 2023-06-22 21:25:06.000000 not1mm-23.6.22/not1mm.egg-info/PKG-INFO
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3581 2023-06-22 21:25:06.000000 not1mm-23.6.22/not1mm.egg-info/SOURCES.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        1 2023-06-22 21:25:06.000000 not1mm-23.6.22/not1mm.egg-info/dependency_links.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       47 2023-06-22 21:25:06.000000 not1mm-23.6.22/not1mm.egg-info/entry_points.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       92 2023-06-22 21:25:06.000000 not1mm-23.6.22/not1mm.egg-info/requires.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       33 2023-06-22 21:25:06.000000 not1mm-23.6.22/not1mm.egg-info/top_level.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1272 2023-06-22 21:23:21.000000 not1mm-23.6.22/pyproject.toml
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       38 2023-06-22 21:25:07.033548 not1mm-23.6.22/setup.cfg
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-22 21:25:07.032548 not1mm-23.6.22/testing/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      176 2023-05-31 20:52:45.000000 not1mm-23.6.22/testing/test.py
```

### Comparing `not1mm-23.6.21.1/LICENSE` & `not1mm-23.6.22/LICENSE`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/PKG-INFO` & `not1mm-23.6.22/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: not1mm
-Version: 23.6.21.1
+Version: 23.6.22
 Summary: NOT1MM Logger
 Author-email: Michael Bridak <michael.bridak@gmail.com>
 Project-URL: Homepage, https://github.com/mbridak/not1mm
 Project-URL: Bug Tracker, https://github.com/mbridak/not1mm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `not1mm-23.6.21.1/README.md` & `not1mm-23.6.22/README.md`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/__main__.py` & `not1mm-23.6.22/not1mm/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,29 +7,29 @@
 00000060: 6265 722c 206e 6f2d 6d65 6d62 6572 2c20  ber, no-member, 
 00000070: 696e 7661 6c69 642d 6e61 6d65 2c20 746f  invalid-name, to
 00000080: 6f2d 6d61 6e79 2d6c 696e 6573 2c20 6e6f  o-many-lines, no
 00000090: 2d6e 616d 652d 696e 2d6d 6f64 756c 650a  -name-in-module.
 000000a0: 0a69 6d70 6f72 7420 6461 7465 7469 6d65  .import datetime
 000000b0: 2061 7320 6474 0a69 6d70 6f72 7420 696d   as dt.import im
 000000c0: 706f 7274 6c69 620a 696d 706f 7274 206c  portlib.import l
-000000d0: 6f67 6769 6e67 0a69 6d70 6f72 7420 6f73  ogging.import os
-000000e0: 0a69 6d70 6f72 7420 706b 6775 7469 6c0a  .import pkgutil.
-000000f0: 696d 706f 7274 2070 6c61 7466 6f72 6d0a  import platform.
-00000100: 696d 706f 7274 2072 650a 696d 706f 7274  import re.import
-00000110: 2073 6f63 6b65 740a 696d 706f 7274 2073   socket.import s
-00000120: 7562 7072 6f63 6573 730a 696d 706f 7274  ubprocess.import
-00000130: 2073 7973 0a69 6d70 6f72 7420 7468 7265   sys.import thre
-00000140: 6164 696e 670a 696d 706f 7274 2074 696d  ading.import tim
-00000150: 650a 696d 706f 7274 2075 7569 640a 6672  e.import uuid.fr
-00000160: 6f6d 2064 6174 6574 696d 6520 696d 706f  om datetime impo
-00000170: 7274 2064 6174 6574 696d 650a 6672 6f6d  rt datetime.from
-00000180: 206a 736f 6e20 696d 706f 7274 204a 534f   json import JSO
-00000190: 4e44 6563 6f64 6545 7272 6f72 2c20 6475  NDecodeError, du
-000001a0: 6d70 732c 206c 6f61 6473 0a69 6d70 6f72  mps, loads.impor
-000001b0: 7420 6c6f 6361 6c65 0a66 726f 6d20 7061  t locale.from pa
+000000d0: 6f63 616c 650a 696d 706f 7274 206c 6f67  ocale.import log
+000000e0: 6769 6e67 0a69 6d70 6f72 7420 6f73 0a69  ging.import os.i
+000000f0: 6d70 6f72 7420 706b 6775 7469 6c0a 696d  mport pkgutil.im
+00000100: 706f 7274 2070 6c61 7466 6f72 6d0a 696d  port platform.im
+00000110: 706f 7274 2072 650a 696d 706f 7274 2073  port re.import s
+00000120: 6f63 6b65 740a 696d 706f 7274 2073 7562  ocket.import sub
+00000130: 7072 6f63 6573 730a 696d 706f 7274 2073  process.import s
+00000140: 7973 0a69 6d70 6f72 7420 7468 7265 6164  ys.import thread
+00000150: 696e 670a 696d 706f 7274 2074 696d 650a  ing.import time.
+00000160: 696d 706f 7274 2075 7569 640a 6672 6f6d  import uuid.from
+00000170: 2064 6174 6574 696d 6520 696d 706f 7274   datetime import
+00000180: 2064 6174 6574 696d 650a 6672 6f6d 206a   datetime.from j
+00000190: 736f 6e20 696d 706f 7274 204a 534f 4e44  son import JSOND
+000001a0: 6563 6f64 6545 7272 6f72 2c20 6475 6d70  ecodeError, dump
+000001b0: 732c 206c 6f61 6473 0a66 726f 6d20 7061  s, loads.from pa
 000001c0: 7468 6c69 6220 696d 706f 7274 2050 6174  thlib import Pat
 000001d0: 680a 6672 6f6d 2073 6875 7469 6c20 696d  h.from shutil im
 000001e0: 706f 7274 2063 6f70 7966 696c 650a 0a69  port copyfile..i
 000001f0: 6d70 6f72 7420 6e6f 7463 7479 7061 7273  mport notctypars
 00000200: 6572 0a69 6d70 6f72 7420 7073 7574 696c  er.import psutil
 00000210: 0a69 6d70 6f72 7420 7265 7175 6573 7473  .import requests
 00000220: 0a69 6d70 6f72 7420 736f 756e 6464 6576  .import sounddev
@@ -62,5882 +62,5886 @@
 000003d0: 726f 6d20 6e6f 7431 6d6d 2e6c 6962 2e65  rom not1mm.lib.e
 000003e0: 6469 745f 6f70 6f6e 2069 6d70 6f72 7420  dit_opon import 
 000003f0: 4f70 4f6e 0a66 726f 6d20 6e6f 7431 6d6d  OpOn.from not1mm
 00000400: 2e6c 6962 2e65 6469 745f 7374 6174 696f  .lib.edit_statio
 00000410: 6e20 696d 706f 7274 2045 6469 7453 7461  n import EditSta
 00000420: 7469 6f6e 0a66 726f 6d20 6e6f 7431 6d6d  tion.from not1mm
 00000430: 2e6c 6962 2e68 616d 5f75 7469 6c69 7479  .lib.ham_utility
-00000440: 2069 6d70 6f72 7420 280a 2020 2020 6265   import (.    be
-00000450: 6172 696e 672c 0a20 2020 2062 6561 7269  aring,.    beari
-00000460: 6e67 5f77 6974 685f 6c61 746c 6f6e 2c0a  ng_with_latlon,.
-00000470: 2020 2020 6361 6c63 756c 6174 655f 7770      calculate_wp
-00000480: 785f 7072 6566 6978 2c0a 2020 2020 6469  x_prefix,.    di
-00000490: 7374 616e 6365 2c0a 2020 2020 6469 7374  stance,.    dist
-000004a0: 616e 6365 5f77 6974 685f 6c61 746c 6f6e  ance_with_latlon
-000004b0: 2c0a 2020 2020 6765 745f 6c6f 6767 6564  ,.    get_logged
-000004c0: 5f62 616e 642c 0a20 2020 2067 6574 6261  _band,.    getba
-000004d0: 6e64 2c0a 2020 2020 7265 6369 7072 6f63  nd,.    reciproc
-000004e0: 6f6c 2c0a 290a 6672 6f6d 206e 6f74 316d  ol,.).from not1m
-000004f0: 6d2e 6c69 622e 6c6f 6f6b 7570 2069 6d70  m.lib.lookup imp
-00000500: 6f72 7420 4861 6d44 426c 6f6f 6b75 702c  ort HamDBlookup,
-00000510: 2048 616d 5154 482c 2051 525a 6c6f 6f6b   HamQTH, QRZlook
-00000520: 7570 0a66 726f 6d20 6e6f 7431 6d6d 2e6c  up.from not1mm.l
-00000530: 6962 2e6d 756c 7469 6361 7374 2069 6d70  ib.multicast imp
-00000540: 6f72 7420 4d75 6c74 6963 6173 740a 6672  ort Multicast.fr
-00000550: 6f6d 206e 6f74 316d 6d2e 6c69 622e 6e31  om not1mm.lib.n1
-00000560: 6d6d 2069 6d70 6f72 7420 4e31 4d4d 0a66  mm import N1MM.f
-00000570: 726f 6d20 6e6f 7431 6d6d 2e6c 6962 2e6e  rom not1mm.lib.n
-00000580: 6577 5f63 6f6e 7465 7374 2069 6d70 6f72  ew_contest impor
-00000590: 7420 4e65 7743 6f6e 7465 7374 0a66 726f  t NewContest.fro
-000005a0: 6d20 6e6f 7431 6d6d 2e6c 6962 2e73 656c  m not1mm.lib.sel
-000005b0: 6563 745f 636f 6e74 6573 7420 696d 706f  ect_contest impo
-000005c0: 7274 2053 656c 6563 7443 6f6e 7465 7374  rt SelectContest
-000005d0: 0a66 726f 6d20 6e6f 7431 6d6d 2e6c 6962  .from not1mm.lib
-000005e0: 2e73 6574 7469 6e67 7320 696d 706f 7274  .settings import
-000005f0: 2053 6574 7469 6e67 730a 6672 6f6d 206e   Settings.from n
-00000600: 6f74 316d 6d2e 6c69 622e 7665 7273 696f  ot1mm.lib.versio
-00000610: 6e20 696d 706f 7274 205f 5f76 6572 7369  n import __versi
-00000620: 6f6e 5f5f 0a66 726f 6d20 6e6f 7431 6d6d  on__.from not1mm
-00000630: 2e6c 6962 2e76 6572 7369 6f6e 7465 7374  .lib.versiontest
-00000640: 2069 6d70 6f72 7420 5665 7273 696f 6e54   import VersionT
-00000650: 6573 740a 0a23 2066 726f 6d20 786d 6c72  est..# from xmlr
-00000660: 7063 2e63 6c69 656e 7420 696d 706f 7274  pc.client import
-00000670: 2045 7272 6f72 2c20 5365 7276 6572 5072   Error, ServerPr
-00000680: 6f78 790a 0a0a 2320 6773 6574 7469 6e67  oxy...# gsetting
-00000690: 7320 6765 7420 6f72 672e 676e 6f6d 652e  s get org.gnome.
-000006a0: 6465 736b 746f 702e 696e 7465 7266 6163  desktop.interfac
-000006b0: 6520 636f 6c6f 722d 7363 6865 6d65 0a23  e color-scheme.#
-000006c0: 206f 732e 656e 7669 726f 6e5b 2251 545f   os.environ["QT_
-000006d0: 5150 415f 504c 4154 464f 524d 225d 203d  QPA_PLATFORM"] =
-000006e0: 2022 7761 796c 616e 6422 0a23 2063 6420   "wayland".# cd 
-000006f0: 3d20 6f73 2e65 6e76 6972 6f6e 2e67 6574  = os.environ.get
-00000700: 2822 5844 475f 4355 5252 454e 545f 4445  ("XDG_CURRENT_DE
-00000710: 534b 544f 5022 2c20 4661 6c73 6529 0a23  SKTOP", False).#
-00000720: 2069 6620 2247 4e4f 4d45 2220 696e 2063   if "GNOME" in c
-00000730: 6420 6f72 2022 556e 6974 7922 2069 6e20  d or "Unity" in 
-00000740: 6364 3a0a 2320 2020 2020 6f73 2e65 6e76  cd:.#     os.env
-00000750: 6972 6f6e 5b22 5154 5f51 5041 5f50 4c41  iron["QT_QPA_PLA
-00000760: 5446 4f52 4d54 4845 4d45 225d 203d 2022  TFORMTHEME"] = "
-00000770: 676e 6f6d 6522 0a23 2020 2020 206f 732e  gnome".#     os.
-00000780: 656e 7669 726f 6e5b 2251 545f 5354 594c  environ["QT_STYL
-00000790: 455f 4f56 4552 5249 4445 225d 203d 2022  E_OVERRIDE"] = "
-000007a0: 4164 7761 6974 612d 4461 726b 220a 0a0a  Adwaita-Dark"...
-000007b0: 2320 7072 696e 7428 6622 4c41 4e47 3a20  # print(f"LANG: 
-000007c0: 7b6f 732e 656e 7669 726f 6e2e 6765 7428  {os.environ.get(
-000007d0: 274c 414e 4727 297d 2229 0a23 2070 7269  'LANG')}").# pri
-000007e0: 6e74 2866 224c 435f 5449 4d45 3a20 7b6f  nt(f"LC_TIME: {o
-000007f0: 732e 656e 7669 726f 6e2e 6765 7428 274c  s.environ.get('L
-00000800: 435f 5449 4d45 2729 7d22 290a 0a0a 6c6f  C_TIME')}")...lo
-00000810: 6164 6572 203d 2070 6b67 7574 696c 2e67  ader = pkgutil.g
-00000820: 6574 5f6c 6f61 6465 7228 226e 6f74 316d  et_loader("not1m
-00000830: 6d22 290a 574f 524b 494e 475f 5041 5448  m").WORKING_PATH
-00000840: 203d 206f 732e 7061 7468 2e64 6972 6e61   = os.path.dirna
-00000850: 6d65 286c 6f61 6465 722e 6765 745f 6669  me(loader.get_fi
-00000860: 6c65 6e61 6d65 2829 290a 0a4d 4153 5445  lename())..MASTE
-00000870: 525f 5343 505f 5552 4c20 3d20 2268 7474  R_SCP_URL = "htt
-00000880: 7073 3a2f 2f77 7777 2e73 7570 6572 6368  ps://www.superch
-00000890: 6563 6b70 6172 7469 616c 2e63 6f6d 2f4d  eckpartial.com/M
-000008a0: 4153 5445 522e 5343 5022 0a0a 4441 5441  ASTER.SCP"..DATA
-000008b0: 5f50 4154 4820 3d20 6f73 2e65 6e76 6972  _PATH = os.envir
-000008c0: 6f6e 2e67 6574 2822 5844 475f 4441 5441  on.get("XDG_DATA
-000008d0: 5f48 4f4d 4522 2c20 7374 7228 5061 7468  _HOME", str(Path
-000008e0: 2e68 6f6d 6528 2920 2f20 222e 6c6f 6361  .home() / ".loca
-000008f0: 6c22 202f 2022 7368 6172 6522 2929 0a44  l" / "share")).D
-00000900: 4154 415f 5041 5448 202b 3d20 222f 6e6f  ATA_PATH += "/no
-00000910: 7431 6d6d 220a 0a74 7279 3a0a 2020 2020  t1mm"..try:.    
-00000920: 6f73 2e6d 6b64 6972 2844 4154 415f 5041  os.mkdir(DATA_PA
-00000930: 5448 290a 6578 6365 7074 2046 696c 6545  TH).except FileE
-00000940: 7869 7374 7345 7272 6f72 3a0a 2020 2020  xistsError:.    
-00000950: 2e2e 2e0a 0a43 4f4e 4649 475f 5041 5448  .....CONFIG_PATH
-00000960: 203d 206f 732e 656e 7669 726f 6e2e 6765   = os.environ.ge
-00000970: 7428 2258 4447 5f43 4f4e 4649 475f 484f  t("XDG_CONFIG_HO
-00000980: 4d45 222c 2073 7472 2850 6174 682e 686f  ME", str(Path.ho
-00000990: 6d65 2829 202f 2022 2e63 6f6e 6669 6722  me() / ".config"
-000009a0: 2929 0a43 4f4e 4649 475f 5041 5448 202b  )).CONFIG_PATH +
-000009b0: 3d20 222f 6e6f 7431 6d6d 220a 0a74 7279  = "/not1mm"..try
-000009c0: 3a0a 2020 2020 6f73 2e6d 6b64 6972 2843  :.    os.mkdir(C
-000009d0: 4f4e 4649 475f 5041 5448 290a 6578 6365  ONFIG_PATH).exce
-000009e0: 7074 2046 696c 6545 7869 7374 7345 7272  pt FileExistsErr
-000009f0: 6f72 3a0a 2020 2020 2e2e 2e0a 0a0a 4354  or:.    ......CT
-00000a00: 5946 494c 4520 3d20 7b7d 0a0a 7769 7468  YFILE = {}..with
-00000a10: 206f 7065 6e28 574f 524b 494e 475f 5041   open(WORKING_PA
-00000a20: 5448 202b 2022 2f64 6174 612f 6374 792e  TH + "/data/cty.
-00000a30: 6a73 6f6e 222c 2022 7274 222c 2065 6e63  json", "rt", enc
-00000a40: 6f64 696e 673d 2275 7466 2d38 2229 2061  oding="utf-8") a
-00000a50: 7320 635f 6669 6c65 3a0a 2020 2020 4354  s c_file:.    CT
-00000a60: 5946 494c 4520 3d20 6c6f 6164 7328 635f  YFILE = loads(c_
-00000a70: 6669 6c65 2e72 6561 6428 2929 0a0a 706f  file.read())..po
-00000a80: 6c6c 5f74 696d 6520 3d20 6461 7465 7469  ll_time = dateti
-00000a90: 6d65 2e6e 6f77 2829 0a0a 0a64 6566 2063  me.now()...def c
-00000aa0: 6865 636b 5f70 726f 6365 7373 286e 616d  heck_process(nam
-00000ab0: 653a 2073 7472 2920 2d3e 2062 6f6f 6c3a  e: str) -> bool:
-00000ac0: 0a20 2020 2022 2222 4368 6563 6b73 2074  .    """Checks t
-00000ad0: 6f20 7365 6520 6966 2074 6865 206e 616d  o see if the nam
-00000ae0: 6520 6f66 2074 6865 2070 726f 6772 616d  e of the program
-00000af0: 2069 7320 696e 2074 6865 2061 6374 6976   is in the activ
-00000b00: 6520 7072 6f63 6573 7320 6c69 7374 2e0a  e process list..
-00000b10: 0a20 2020 2050 6172 616d 6574 6572 730a  .    Parameters.
-00000b20: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
-00000b30: 2020 206e 616d 6520 3a20 7374 720a 0a20     name : str.. 
-00000b40: 2020 2052 6574 7572 6e73 0a20 2020 202d     Returns.    -
-00000b50: 2d2d 2d2d 2d2d 0a20 2020 2042 6f6f 6c0a  ------.    Bool.
-00000b60: 2020 2020 2222 220a 2020 2020 666f 7220      """.    for 
-00000b70: 7072 6f63 2069 6e20 7073 7574 696c 2e70  proc in psutil.p
-00000b80: 726f 6365 7373 5f69 7465 7228 293a 0a20  rocess_iter():. 
-00000b90: 2020 2020 2020 2069 6620 6c65 6e28 7072         if len(pr
-00000ba0: 6f63 2e63 6d64 6c69 6e65 2829 2920 3d3d  oc.cmdline()) ==
-00000bb0: 2032 3a0a 2020 2020 2020 2020 2020 2020   2:.            
-00000bc0: 6966 206e 616d 6520 696e 2070 726f 632e  if name in proc.
-00000bd0: 636d 646c 696e 6528 295b 315d 3a0a 2020  cmdline()[1]:.  
-00000be0: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00000bf0: 7475 726e 2054 7275 650a 2020 2020 7265  turn True.    re
-00000c00: 7475 726e 2046 616c 7365 0a0a 0a23 2064  turn False...# d
-00000c10: 6566 2063 7479 5f6c 6f6f 6b75 7028 6361  ef cty_lookup(ca
-00000c20: 6c6c 7369 676e 3a20 7374 7229 3a0a 2320  llsign: str):.# 
-00000c30: 2020 2020 2222 224c 6f6f 6b75 7020 6361      """Lookup ca
-00000c40: 6c6c 7369 676e 2069 6e20 6374 792e 6461  llsign in cty.da
-00000c50: 7420 6669 6c65 2e0a 0a23 2020 2020 2050  t file...#     P
-00000c60: 6172 616d 6574 6572 730a 2320 2020 2020  arameters.#     
-00000c70: 2d2d 2d2d 2d2d 2d2d 2d2d 0a23 2020 2020  ----------.#    
-00000c80: 2063 616c 6c73 6967 6e20 3a20 7374 720a   callsign : str.
-00000c90: 0a23 2020 2020 2052 6574 7572 6e73 0a23  .#     Returns.#
-00000ca0: 2020 2020 202d 2d2d 2d2d 2d2d 0a23 2020       -------.#  
-00000cb0: 2020 2072 6573 756c 743a 206c 6973 740a     result: list.
-00000cc0: 2320 2020 2020 2222 220a 2320 2020 2020  #     """.#     
-00000cd0: 6361 6c6c 7369 676e 203d 2063 616c 6c73  callsign = calls
-00000ce0: 6967 6e2e 7570 7065 7228 290a 2320 2020  ign.upper().#   
-00000cf0: 2020 666f 7220 636f 756e 7420 696e 2072    for count in r
-00000d00: 6576 6572 7365 6428 7261 6e67 6528 6c65  eversed(range(le
-00000d10: 6e28 6361 6c6c 7369 676e 2929 293a 0a23  n(callsign))):.#
-00000d20: 2020 2020 2020 2020 2073 6561 7263 6869           searchi
-00000d30: 7465 6d20 3d20 6361 6c6c 7369 676e 5b3a  tem = callsign[:
-00000d40: 2063 6f75 6e74 202b 2031 5d0a 2320 2020   count + 1].#   
-00000d50: 2020 2020 2020 7265 7375 6c74 203d 207b        result = {
-00000d60: 6b65 793a 2076 616c 2066 6f72 206b 6579  key: val for key
-00000d70: 2c20 7661 6c20 696e 2043 5459 4649 4c45  , val in CTYFILE
-00000d80: 2e69 7465 6d73 2829 2069 6620 6b65 7920  .items() if key 
-00000d90: 3d3d 2073 6561 7263 6869 7465 6d7d 0a23  == searchitem}.#
-00000da0: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
-00000db0: 7265 7375 6c74 3a0a 2320 2020 2020 2020  result:.#       
-00000dc0: 2020 2020 2020 636f 6e74 696e 7565 0a23        continue.#
-00000dd0: 2020 2020 2020 2020 2069 6620 7265 7375           if resu
-00000de0: 6c74 2e67 6574 2873 6561 7263 6869 7465  lt.get(searchite
-00000df0: 6d29 2e67 6574 2822 6578 6163 745f 6d61  m).get("exact_ma
-00000e00: 7463 6822 293a 0a23 2020 2020 2020 2020  tch"):.#        
-00000e10: 2020 2020 2069 6620 7365 6172 6368 6974       if searchit
-00000e20: 656d 203d 3d20 6361 6c6c 7369 676e 3a0a  em == callsign:.
-00000e30: 2320 2020 2020 2020 2020 2020 2020 2020  #               
-00000e40: 2020 7265 7475 726e 2072 6573 756c 740a    return result.
-00000e50: 2320 2020 2020 2020 2020 2020 2020 636f  #             co
-00000e60: 6e74 696e 7565 0a23 2020 2020 2020 2020  ntinue.#        
-00000e70: 2072 6574 7572 6e20 7265 7375 6c74 0a0a   return result..
-00000e80: 0a63 6c61 7373 204d 6169 6e57 696e 646f  .class MainWindo
-00000e90: 7728 5174 5769 6467 6574 732e 514d 6169  w(QtWidgets.QMai
-00000ea0: 6e57 696e 646f 7729 3a0a 2020 2020 2222  nWindow):.    ""
-00000eb0: 220a 2020 2020 5468 6520 6d61 696e 2077  ".    The main w
-00000ec0: 696e 646f 770a 2020 2020 2222 220a 0a20  indow.    """.. 
-00000ed0: 2020 2070 7265 665f 7265 6620 3d20 7b0a     pref_ref = {.
-00000ee0: 2020 2020 2020 2020 2273 6f75 6e64 6465          "soundde
-00000ef0: 7669 6365 223a 2022 6465 6661 756c 7422  vice": "default"
-00000f00: 2c0a 2020 2020 2020 2020 2275 7365 7172  ,.        "useqr
-00000f10: 7a22 3a20 4661 6c73 652c 0a20 2020 2020  z": False,.     
-00000f20: 2020 2022 6c6f 6f6b 7570 7573 6572 6e61     "lookupuserna
-00000f30: 6d65 223a 2022 7573 6572 6e61 6d65 222c  me": "username",
-00000f40: 0a20 2020 2020 2020 2022 6c6f 6f6b 7570  .        "lookup
-00000f50: 7061 7373 776f 7264 223a 2022 7061 7373  password": "pass
-00000f60: 776f 7264 222c 0a20 2020 2020 2020 2022  word",.        "
-00000f70: 7275 6e5f 7374 6174 6522 3a20 5472 7565  run_state": True
-00000f80: 2c0a 2020 2020 2020 2020 2263 6f6d 6d61  ,.        "comma
-00000f90: 6e64 5f62 7574 746f 6e73 223a 2046 616c  nd_buttons": Fal
-00000fa0: 7365 2c0a 2020 2020 2020 2020 2263 775f  se,.        "cw_
-00000fb0: 6d61 6372 6f73 223a 2054 7275 652c 0a20  macros": True,. 
-00000fc0: 2020 2020 2020 2022 6261 6e64 735f 6d6f         "bands_mo
-00000fd0: 6465 7322 3a20 5472 7565 2c0a 2020 2020  des": True,.    
-00000fe0: 2020 2020 2277 696e 646f 775f 6865 6967      "window_heig
-00000ff0: 6874 223a 2032 3030 2c0a 2020 2020 2020  ht": 200,.      
-00001000: 2020 2277 696e 646f 775f 7769 6474 6822    "window_width"
-00001010: 3a20 3630 302c 0a20 2020 2020 2020 2022  : 600,.        "
-00001020: 7769 6e64 6f77 5f78 223a 2031 3230 2c0a  window_x": 120,.
-00001030: 2020 2020 2020 2020 2277 696e 646f 775f          "window_
-00001040: 7922 3a20 3132 302c 0a20 2020 2020 2020  y": 120,.       
-00001050: 2022 6375 7272 656e 745f 6461 7461 6261   "current_databa
-00001060: 7365 223a 2022 6861 6d2e 6462 222c 0a20  se": "ham.db",. 
-00001070: 2020 2020 2020 2022 636f 6e74 6573 7422         "contest"
-00001080: 3a20 2222 2c0a 2020 2020 2020 2020 226d  : "",.        "m
-00001090: 756c 7469 6361 7374 5f67 726f 7570 223a  ulticast_group":
-000010a0: 2022 3233 392e 312e 312e 3122 2c0a 2020   "239.1.1.1",.  
-000010b0: 2020 2020 2020 226d 756c 7469 6361 7374        "multicast
-000010c0: 5f70 6f72 7422 3a20 3232 3339 2c0a 2020  _port": 2239,.  
-000010d0: 2020 2020 2020 2269 6e74 6572 6661 6365        "interface
-000010e0: 5f69 7022 3a20 2230 2e30 2e30 2e30 222c  _ip": "0.0.0.0",
-000010f0: 0a20 2020 2020 2020 2022 7365 6e64 5f6e  .        "send_n
-00001100: 316d 6d5f 7061 636b 6574 7322 3a20 4661  1mm_packets": Fa
-00001110: 6c73 652c 0a20 2020 2020 2020 2022 6e31  lse,.        "n1
-00001120: 6d6d 5f73 7461 7469 6f6e 5f6e 616d 6522  mm_station_name"
-00001130: 3a20 2232 304d 2043 5720 5465 6e74 222c  : "20M CW Tent",
-00001140: 0a20 2020 2020 2020 2022 6e31 6d6d 5f6f  .        "n1mm_o
-00001150: 7065 7261 746f 7222 3a20 2242 6572 6e69  perator": "Berni
-00001160: 6522 2c0a 2020 2020 2020 2020 226e 316d  e",.        "n1m
-00001170: 6d5f 7261 6469 6f70 6f72 7422 3a20 2231  m_radioport": "1
-00001180: 3237 2e30 2e30 2e31 3a31 3230 3630 222c  27.0.0.1:12060",
-00001190: 0a20 2020 2020 2020 2022 6e31 6d6d 5f63  .        "n1mm_c
-000011a0: 6f6e 7461 6374 706f 7274 223a 2022 3132  ontactport": "12
-000011b0: 372e 302e 302e 313a 3132 3036 3022 2c0a  7.0.0.1:12060",.
-000011c0: 2020 2020 2020 2020 226e 316d 6d5f 6c6f          "n1mm_lo
-000011d0: 6f6b 7570 706f 7274 223a 2022 3132 372e  okupport": "127.
-000011e0: 302e 302e 313a 3132 3036 3022 2c0a 2020  0.0.1:12060",.  
-000011f0: 2020 2020 2020 226e 316d 6d5f 7363 6f72        "n1mm_scor
-00001200: 6570 6f72 7422 3a20 2231 3237 2e30 2e30  eport": "127.0.0
-00001210: 2e31 3a31 3230 3630 222c 0a20 2020 2020  .1:12060",.     
-00001220: 2020 2022 7573 6568 616d 6462 223a 2046     "usehamdb": F
-00001230: 616c 7365 2c0a 2020 2020 2020 2020 2275  alse,.        "u
-00001240: 7365 6861 6d71 7468 223a 2046 616c 7365  sehamqth": False
-00001250: 2c0a 2020 2020 2020 2020 2263 6c6f 7564  ,.        "cloud
-00001260: 6c6f 6722 3a20 4661 6c73 652c 0a20 2020  log": False,.   
-00001270: 2020 2020 2022 636c 6f75 646c 6f67 6170       "cloudlogap
-00001280: 6922 3a20 2222 2c0a 2020 2020 2020 2020  i": "",.        
-00001290: 2263 6c6f 7564 6c6f 6775 726c 223a 2022  "cloudlogurl": "
-000012a0: 222c 0a20 2020 2020 2020 2022 4341 545f  ",.        "CAT_
-000012b0: 6970 223a 2022 3132 372e 302e 302e 3122  ip": "127.0.0.1"
-000012c0: 2c0a 2020 2020 2020 2020 2275 7365 7269  ,.        "useri
-000012d0: 6763 746c 6422 3a20 4661 6c73 652c 0a20  gctld": False,. 
-000012e0: 2020 2020 2020 2022 7573 6566 6c72 6967         "useflrig
-000012f0: 223a 2046 616c 7365 2c0a 2020 2020 2020  ": False,.      
-00001300: 2020 2263 7769 7022 3a20 2231 3237 2e30    "cwip": "127.0
-00001310: 2e30 2e31 222c 0a20 2020 2020 2020 2022  .0.1",.        "
-00001320: 6377 706f 7274 223a 2036 3738 392c 0a20  cwport": 6789,. 
-00001330: 2020 2020 2020 2022 6377 7479 7065 223a         "cwtype":
-00001340: 2030 2c0a 2020 2020 2020 2020 2275 7365   0,.        "use
-00001350: 7365 7276 6572 223a 2046 616c 7365 2c0a  server": False,.
-00001360: 2020 2020 2020 2020 2243 4154 5f70 6f72          "CAT_por
-00001370: 7422 3a20 3435 3332 2c0a 2020 2020 2020  t": 4532,.      
-00001380: 2020 2263 6c75 7374 6572 5f73 6572 7665    "cluster_serve
-00001390: 7222 3a20 2264 7863 2e6e 6337 6a2e 636f  r": "dxc.nc7j.co
-000013a0: 6d22 2c0a 2020 2020 2020 2020 2263 6c75  m",.        "clu
-000013b0: 7374 6572 5f70 6f72 7422 3a20 3733 3733  ster_port": 7373
-000013c0: 2c0a 2020 2020 2020 2020 2263 6c75 7374  ,.        "clust
-000013d0: 6572 5f66 696c 7465 7222 3a20 2253 6574  er_filter": "Set
-000013e0: 2044 5820 4669 6c74 6572 2053 706f 7474   DX Filter Spott
-000013f0: 6572 436f 6e74 3d4e 4122 2c0a 2020 2020  erCont=NA",.    
-00001400: 2020 2020 2263 6c75 7374 6572 5f6d 6f64      "cluster_mod
-00001410: 6522 3a20 224f 5045 4e22 2c0a 2020 2020  e": "OPEN",.    
-00001420: 7d0a 2020 2020 6170 7073 7461 7274 6564  }.    appstarted
-00001430: 203d 2046 616c 7365 0a20 2020 2063 6f6e   = False.    con
-00001440: 7461 6374 203d 207b 7d0a 2020 2020 636f  tact = {}.    co
-00001450: 6e74 6573 7420 3d20 4e6f 6e65 0a20 2020  ntest = None.   
-00001460: 2063 6f6e 7465 7374 5f73 6574 7469 6e67   contest_setting
-00001470: 7320 3d20 7b7d 0a20 2020 2070 7265 6620  s = {}.    pref 
-00001480: 3d20 4e6f 6e65 0a20 2020 2073 7461 7469  = None.    stati
-00001490: 6f6e 203d 207b 7d0a 2020 2020 6375 7272  on = {}.    curr
-000014a0: 656e 745f 6f70 203d 2022 220a 2020 2020  ent_op = "".    
-000014b0: 6375 7272 656e 745f 6d6f 6465 203d 2022  current_mode = "
-000014c0: 220a 2020 2020 6375 7272 656e 745f 6261  ".    current_ba
-000014d0: 6e64 203d 2022 220a 2020 2020 6465 6661  nd = "".    defa
-000014e0: 756c 745f 7273 7420 3d20 2235 3922 0a20  ult_rst = "59". 
-000014f0: 2020 2063 7720 3d20 4e6f 6e65 0a20 2020     cw = None.   
-00001500: 206c 6f6f 6b5f 7570 203d 204e 6f6e 650a   look_up = None.
-00001510: 2020 2020 7275 6e5f 7374 6174 6520 3d20      run_state = 
-00001520: 4661 6c73 650a 2020 2020 666b 6579 7320  False.    fkeys 
-00001530: 3d20 7b7d 0a20 2020 2061 626f 7574 5f64  = {}.    about_d
-00001540: 6961 6c6f 6720 3d20 4e6f 6e65 0a20 2020  ialog = None.   
-00001550: 2071 727a 5f64 6961 6c6f 6720 3d20 4e6f   qrz_dialog = No
-00001560: 6e65 0a20 2020 2073 6574 7469 6e67 735f  ne.    settings_
-00001570: 6469 616c 6f67 203d 204e 6f6e 650a 2020  dialog = None.  
-00001580: 2020 6564 6974 5f6d 6163 726f 5f64 6961    edit_macro_dia
-00001590: 6c6f 6720 3d20 4e6f 6e65 0a20 2020 2063  log = None.    c
-000015a0: 6f6e 7465 7374 5f64 6961 6c6f 6720 3d20  ontest_dialog = 
-000015b0: 4e6f 6e65 0a20 2020 2063 6f6e 6669 6775  None.    configu
-000015c0: 7261 7469 6f6e 5f64 6961 6c6f 6720 3d20  ration_dialog = 
-000015d0: 4e6f 6e65 0a20 2020 206f 706f 6e5f 6469  None.    opon_di
-000015e0: 616c 6f67 203d 204e 6f6e 650a 2020 2020  alog = None.    
-000015f0: 6462 6e61 6d65 203d 2044 4154 415f 5041  dbname = DATA_PA
-00001600: 5448 202b 2022 2f68 616d 2e64 6222 0a20  TH + "/ham.db". 
-00001610: 2020 2072 6164 696f 5f73 7461 7465 203d     radio_state =
-00001620: 207b 7d0a 2020 2020 7269 675f 636f 6e74   {}.    rig_cont
-00001630: 726f 6c20 3d20 4e6f 6e65 0a20 2020 206d  rol = None.    m
-00001640: 756c 7469 6361 7374 5f67 726f 7570 203d  ulticast_group =
-00001650: 204e 6f6e 650a 2020 2020 6d75 6c74 6963   None.    multic
-00001660: 6173 745f 706f 7274 203d 204e 6f6e 650a  ast_port = None.
-00001670: 2020 2020 696e 7465 7266 6163 655f 6970      interface_ip
-00001680: 203d 204e 6f6e 650a 2020 2020 7269 675f   = None.    rig_
-00001690: 636f 6e74 726f 6c20 3d20 4e6f 6e65 0a0a  control = None..
-000016a0: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
-000016b0: 2873 656c 662c 202a 6172 6773 2c20 2a2a  (self, *args, **
-000016c0: 6b77 6172 6773 293a 0a20 2020 2020 2020  kwargs):.       
-000016d0: 2073 7570 6572 2829 2e5f 5f69 6e69 745f   super().__init_
-000016e0: 5f28 2a61 7267 732c 202a 2a6b 7761 7267  _(*args, **kwarg
-000016f0: 7329 0a20 2020 2020 2020 206c 6f67 6765  s).        logge
-00001700: 722e 696e 666f 2822 4d61 696e 5769 6e64  r.info("MainWind
-00001710: 6f77 3a20 5f5f 696e 6974 5f5f 2229 0a20  ow: __init__"). 
-00001720: 2020 2020 2020 2064 6174 615f 7061 7468         data_path
-00001730: 203d 2057 4f52 4b49 4e47 5f50 4154 4820   = WORKING_PATH 
-00001740: 2b20 222f 6461 7461 2f6d 6169 6e2e 7569  + "/data/main.ui
-00001750: 220a 2020 2020 2020 2020 7569 632e 6c6f  ".        uic.lo
-00001760: 6164 5569 2864 6174 615f 7061 7468 2c20  adUi(data_path, 
-00001770: 7365 6c66 290a 2020 2020 2020 2020 7365  self).        se
-00001780: 6c66 2e6c 6566 7464 6f74 2e68 6964 6528  lf.leftdot.hide(
-00001790: 290a 2020 2020 2020 2020 7365 6c66 2e72  ).        self.r
-000017a0: 6967 6874 646f 742e 6869 6465 2829 0a20  ightdot.hide(). 
-000017b0: 2020 2020 2020 2073 656c 662e 6e31 6d6d         self.n1mm
-000017c0: 203d 204e 314d 4d28 290a 2020 2020 2020   = N1MM().      
-000017d0: 2020 7365 6c66 2e6e 6578 745f 6669 656c    self.next_fiel
-000017e0: 6420 3d20 7365 6c66 2e6f 7468 6572 5f32  d = self.other_2
-000017f0: 0a20 2020 2020 2020 2073 656c 662e 6475  .        self.du
-00001800: 7065 5f69 6e64 6963 6174 6f72 2e68 6964  pe_indicator.hid
-00001810: 6528 290a 2020 2020 2020 2020 7365 6c66  e().        self
-00001820: 2e63 775f 7370 6565 642e 7661 6c75 6543  .cw_speed.valueC
-00001830: 6861 6e67 6564 2e63 6f6e 6e65 6374 2873  hanged.connect(s
-00001840: 656c 662e 6377 7370 6565 645f 7370 696e  elf.cwspeed_spin
-00001850: 626f 785f 6368 616e 6765 6429 0a0a 2020  box_changed)..  
-00001860: 2020 2020 2020 7365 6c66 2e61 6374 696f        self.actio
-00001870: 6e43 575f 4d61 6372 6f73 2e74 7269 6767  nCW_Macros.trigg
-00001880: 6572 6564 2e63 6f6e 6e65 6374 2873 656c  ered.connect(sel
-00001890: 662e 6377 5f6d 6163 726f 735f 7374 6174  f.cw_macros_stat
-000018a0: 655f 6368 616e 6765 6429 0a20 2020 2020  e_changed).     
-000018b0: 2020 2073 656c 662e 6163 7469 6f6e 436f     self.actionCo
-000018c0: 6d6d 616e 645f 4275 7474 6f6e 732e 7472  mmand_Buttons.tr
-000018d0: 6967 6765 7265 642e 636f 6e6e 6563 7428  iggered.connect(
-000018e0: 7365 6c66 2e63 6f6d 6d61 6e64 5f62 7574  self.command_but
-000018f0: 746f 6e73 5f73 7461 7465 5f63 6861 6e67  tons_state_chang
-00001900: 6529 0a20 2020 2020 2020 2073 656c 662e  e).        self.
-00001910: 6163 7469 6f6e 4c6f 675f 5769 6e64 6f77  actionLog_Window
-00001920: 2e74 7269 6767 6572 6564 2e63 6f6e 6e65  .triggered.conne
-00001930: 6374 2873 656c 662e 6c61 756e 6368 5f6c  ct(self.launch_l
-00001940: 6f67 5f77 696e 646f 7729 0a20 2020 2020  og_window).     
-00001950: 2020 2073 656c 662e 6163 7469 6f6e 4261     self.actionBa
-00001960: 6e64 6d61 702e 7472 6967 6765 7265 642e  ndmap.triggered.
-00001970: 636f 6e6e 6563 7428 7365 6c66 2e6c 6175  connect(self.lau
-00001980: 6e63 685f 6261 6e64 6d61 705f 7769 6e64  nch_bandmap_wind
+00000440: 2069 6d70 6f72 7420 2862 6561 7269 6e67   import (bearing
+00000450: 2c20 6265 6172 696e 675f 7769 7468 5f6c  , bearing_with_l
+00000460: 6174 6c6f 6e2c 0a20 2020 2020 2020 2020  atlon,.         
+00000470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000480: 2020 2020 2020 2020 2020 2063 616c 6375             calcu
+00000490: 6c61 7465 5f77 7078 5f70 7265 6669 782c  late_wpx_prefix,
+000004a0: 2064 6973 7461 6e63 652c 0a20 2020 2020   distance,.     
+000004b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000004c0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+000004d0: 6973 7461 6e63 655f 7769 7468 5f6c 6174  istance_with_lat
+000004e0: 6c6f 6e2c 2067 6574 5f6c 6f67 6765 645f  lon, get_logged_
+000004f0: 6261 6e64 2c0a 2020 2020 2020 2020 2020  band,.          
+00000500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000510: 2020 2020 2020 2020 2020 6765 7462 616e            getban
+00000520: 642c 2072 6563 6970 726f 636f 6c29 0a66  d, reciprocol).f
+00000530: 726f 6d20 6e6f 7431 6d6d 2e6c 6962 2e6c  rom not1mm.lib.l
+00000540: 6f6f 6b75 7020 696d 706f 7274 2048 616d  ookup import Ham
+00000550: 4442 6c6f 6f6b 7570 2c20 4861 6d51 5448  DBlookup, HamQTH
+00000560: 2c20 5152 5a6c 6f6f 6b75 700a 6672 6f6d  , QRZlookup.from
+00000570: 206e 6f74 316d 6d2e 6c69 622e 6d75 6c74   not1mm.lib.mult
+00000580: 6963 6173 7420 696d 706f 7274 204d 756c  icast import Mul
+00000590: 7469 6361 7374 0a66 726f 6d20 6e6f 7431  ticast.from not1
+000005a0: 6d6d 2e6c 6962 2e6e 316d 6d20 696d 706f  mm.lib.n1mm impo
+000005b0: 7274 204e 314d 4d0a 6672 6f6d 206e 6f74  rt N1MM.from not
+000005c0: 316d 6d2e 6c69 622e 6e65 775f 636f 6e74  1mm.lib.new_cont
+000005d0: 6573 7420 696d 706f 7274 204e 6577 436f  est import NewCo
+000005e0: 6e74 6573 740a 6672 6f6d 206e 6f74 316d  ntest.from not1m
+000005f0: 6d2e 6c69 622e 7365 6c65 6374 5f63 6f6e  m.lib.select_con
+00000600: 7465 7374 2069 6d70 6f72 7420 5365 6c65  test import Sele
+00000610: 6374 436f 6e74 6573 740a 6672 6f6d 206e  ctContest.from n
+00000620: 6f74 316d 6d2e 6c69 622e 7365 7474 696e  ot1mm.lib.settin
+00000630: 6773 2069 6d70 6f72 7420 5365 7474 696e  gs import Settin
+00000640: 6773 0a66 726f 6d20 6e6f 7431 6d6d 2e6c  gs.from not1mm.l
+00000650: 6962 2e76 6572 7369 6f6e 2069 6d70 6f72  ib.version impor
+00000660: 7420 5f5f 7665 7273 696f 6e5f 5f0a 6672  t __version__.fr
+00000670: 6f6d 206e 6f74 316d 6d2e 6c69 622e 7665  om not1mm.lib.ve
+00000680: 7273 696f 6e74 6573 7420 696d 706f 7274  rsiontest import
+00000690: 2056 6572 7369 6f6e 5465 7374 0a0a 2320   VersionTest..# 
+000006a0: 6672 6f6d 2078 6d6c 7270 632e 636c 6965  from xmlrpc.clie
+000006b0: 6e74 2069 6d70 6f72 7420 4572 726f 722c  nt import Error,
+000006c0: 2053 6572 7665 7250 726f 7879 0a0a 0a23   ServerProxy...#
+000006d0: 2067 7365 7474 696e 6773 2067 6574 206f   gsettings get o
+000006e0: 7267 2e67 6e6f 6d65 2e64 6573 6b74 6f70  rg.gnome.desktop
+000006f0: 2e69 6e74 6572 6661 6365 2063 6f6c 6f72  .interface color
+00000700: 2d73 6368 656d 650a 2320 6f73 2e65 6e76  -scheme.# os.env
+00000710: 6972 6f6e 5b22 5154 5f51 5041 5f50 4c41  iron["QT_QPA_PLA
+00000720: 5446 4f52 4d22 5d20 3d20 2277 6179 6c61  TFORM"] = "wayla
+00000730: 6e64 220a 2320 6364 203d 206f 732e 656e  nd".# cd = os.en
+00000740: 7669 726f 6e2e 6765 7428 2258 4447 5f43  viron.get("XDG_C
+00000750: 5552 5245 4e54 5f44 4553 4b54 4f50 222c  URRENT_DESKTOP",
+00000760: 2046 616c 7365 290a 2320 6966 2022 474e   False).# if "GN
+00000770: 4f4d 4522 2069 6e20 6364 206f 7220 2255  OME" in cd or "U
+00000780: 6e69 7479 2220 696e 2063 643a 0a23 2020  nity" in cd:.#  
+00000790: 2020 206f 732e 656e 7669 726f 6e5b 2251     os.environ["Q
+000007a0: 545f 5150 415f 504c 4154 464f 524d 5448  T_QPA_PLATFORMTH
+000007b0: 454d 4522 5d20 3d20 2267 6e6f 6d65 220a  EME"] = "gnome".
+000007c0: 2320 2020 2020 6f73 2e65 6e76 6972 6f6e  #     os.environ
+000007d0: 5b22 5154 5f53 5459 4c45 5f4f 5645 5252  ["QT_STYLE_OVERR
+000007e0: 4944 4522 5d20 3d20 2241 6477 6169 7461  IDE"] = "Adwaita
+000007f0: 2d44 6172 6b22 0a0a 0a23 2070 7269 6e74  -Dark"...# print
+00000800: 2866 224c 414e 473a 207b 6f73 2e65 6e76  (f"LANG: {os.env
+00000810: 6972 6f6e 2e67 6574 2827 4c41 4e47 2729  iron.get('LANG')
+00000820: 7d22 290a 2320 7072 696e 7428 6622 4c43  }").# print(f"LC
+00000830: 5f54 494d 453a 207b 6f73 2e65 6e76 6972  _TIME: {os.envir
+00000840: 6f6e 2e67 6574 2827 4c43 5f54 494d 4527  on.get('LC_TIME'
+00000850: 297d 2229 0a0a 0a6c 6f61 6465 7220 3d20  )}")...loader = 
+00000860: 706b 6775 7469 6c2e 6765 745f 6c6f 6164  pkgutil.get_load
+00000870: 6572 2822 6e6f 7431 6d6d 2229 0a57 4f52  er("not1mm").WOR
+00000880: 4b49 4e47 5f50 4154 4820 3d20 6f73 2e70  KING_PATH = os.p
+00000890: 6174 682e 6469 726e 616d 6528 6c6f 6164  ath.dirname(load
+000008a0: 6572 2e67 6574 5f66 696c 656e 616d 6528  er.get_filename(
+000008b0: 2929 0a0a 4d41 5354 4552 5f53 4350 5f55  ))..MASTER_SCP_U
+000008c0: 524c 203d 2022 6874 7470 733a 2f2f 7777  RL = "https://ww
+000008d0: 772e 7375 7065 7263 6865 636b 7061 7274  w.supercheckpart
+000008e0: 6961 6c2e 636f 6d2f 4d41 5354 4552 2e53  ial.com/MASTER.S
+000008f0: 4350 220a 0a44 4154 415f 5041 5448 203d  CP"..DATA_PATH =
+00000900: 206f 732e 656e 7669 726f 6e2e 6765 7428   os.environ.get(
+00000910: 2258 4447 5f44 4154 415f 484f 4d45 222c  "XDG_DATA_HOME",
+00000920: 2073 7472 2850 6174 682e 686f 6d65 2829   str(Path.home()
+00000930: 202f 2022 2e6c 6f63 616c 2220 2f20 2273   / ".local" / "s
+00000940: 6861 7265 2229 290a 4441 5441 5f50 4154  hare")).DATA_PAT
+00000950: 4820 2b3d 2022 2f6e 6f74 316d 6d22 0a0a  H += "/not1mm"..
+00000960: 7472 793a 0a20 2020 206f 732e 6d6b 6469  try:.    os.mkdi
+00000970: 7228 4441 5441 5f50 4154 4829 0a65 7863  r(DATA_PATH).exc
+00000980: 6570 7420 4669 6c65 4578 6973 7473 4572  ept FileExistsEr
+00000990: 726f 723a 0a20 2020 202e 2e2e 0a0a 434f  ror:.    .....CO
+000009a0: 4e46 4947 5f50 4154 4820 3d20 6f73 2e65  NFIG_PATH = os.e
+000009b0: 6e76 6972 6f6e 2e67 6574 2822 5844 475f  nviron.get("XDG_
+000009c0: 434f 4e46 4947 5f48 4f4d 4522 2c20 7374  CONFIG_HOME", st
+000009d0: 7228 5061 7468 2e68 6f6d 6528 2920 2f20  r(Path.home() / 
+000009e0: 222e 636f 6e66 6967 2229 290a 434f 4e46  ".config")).CONF
+000009f0: 4947 5f50 4154 4820 2b3d 2022 2f6e 6f74  IG_PATH += "/not
+00000a00: 316d 6d22 0a0a 7472 793a 0a20 2020 206f  1mm"..try:.    o
+00000a10: 732e 6d6b 6469 7228 434f 4e46 4947 5f50  s.mkdir(CONFIG_P
+00000a20: 4154 4829 0a65 7863 6570 7420 4669 6c65  ATH).except File
+00000a30: 4578 6973 7473 4572 726f 723a 0a20 2020  ExistsError:.   
+00000a40: 202e 2e2e 0a0a 0a43 5459 4649 4c45 203d   ......CTYFILE =
+00000a50: 207b 7d0a 0a77 6974 6820 6f70 656e 2857   {}..with open(W
+00000a60: 4f52 4b49 4e47 5f50 4154 4820 2b20 222f  ORKING_PATH + "/
+00000a70: 6461 7461 2f63 7479 2e6a 736f 6e22 2c20  data/cty.json", 
+00000a80: 2272 7422 2c20 656e 636f 6469 6e67 3d22  "rt", encoding="
+00000a90: 7574 662d 3822 2920 6173 2063 5f66 696c  utf-8") as c_fil
+00000aa0: 653a 0a20 2020 2043 5459 4649 4c45 203d  e:.    CTYFILE =
+00000ab0: 206c 6f61 6473 2863 5f66 696c 652e 7265   loads(c_file.re
+00000ac0: 6164 2829 290a 0a70 6f6c 6c5f 7469 6d65  ad())..poll_time
+00000ad0: 203d 2064 6174 6574 696d 652e 6e6f 7728   = datetime.now(
+00000ae0: 290a 0a0a 6465 6620 6368 6563 6b5f 7072  )...def check_pr
+00000af0: 6f63 6573 7328 6e61 6d65 3a20 7374 7229  ocess(name: str)
+00000b00: 202d 3e20 626f 6f6c 3a0a 2020 2020 2222   -> bool:.    ""
+00000b10: 2243 6865 636b 7320 746f 2073 6565 2069  "Checks to see i
+00000b20: 6620 7468 6520 6e61 6d65 206f 6620 7468  f the name of th
+00000b30: 6520 7072 6f67 7261 6d20 6973 2069 6e20  e program is in 
+00000b40: 7468 6520 6163 7469 7665 2070 726f 6365  the active proce
+00000b50: 7373 206c 6973 742e 0a0a 2020 2020 5061  ss list...    Pa
+00000b60: 7261 6d65 7465 7273 0a20 2020 202d 2d2d  rameters.    ---
+00000b70: 2d2d 2d2d 2d2d 2d0a 2020 2020 6e61 6d65  -------.    name
+00000b80: 203a 2073 7472 0a0a 2020 2020 5265 7475   : str..    Retu
+00000b90: 726e 730a 2020 2020 2d2d 2d2d 2d2d 2d0a  rns.    -------.
+00000ba0: 2020 2020 426f 6f6c 0a20 2020 2022 2222      Bool.    """
+00000bb0: 0a20 2020 2066 6f72 2070 726f 6320 696e  .    for proc in
+00000bc0: 2070 7375 7469 6c2e 7072 6f63 6573 735f   psutil.process_
+00000bd0: 6974 6572 2829 3a0a 2020 2020 2020 2020  iter():.        
+00000be0: 6966 206c 656e 2870 726f 632e 636d 646c  if len(proc.cmdl
+00000bf0: 696e 6528 2929 203d 3d20 323a 0a20 2020  ine()) == 2:.   
+00000c00: 2020 2020 2020 2020 2069 6620 6e61 6d65           if name
+00000c10: 2069 6e20 7072 6f63 2e63 6d64 6c69 6e65   in proc.cmdline
+00000c20: 2829 5b31 5d3a 0a20 2020 2020 2020 2020  ()[1]:.         
+00000c30: 2020 2020 2020 2072 6574 7572 6e20 5472         return Tr
+00000c40: 7565 0a20 2020 2072 6574 7572 6e20 4661  ue.    return Fa
+00000c50: 6c73 650a 0a0a 2320 6465 6620 6374 795f  lse...# def cty_
+00000c60: 6c6f 6f6b 7570 2863 616c 6c73 6967 6e3a  lookup(callsign:
+00000c70: 2073 7472 293a 0a23 2020 2020 2022 2222   str):.#     """
+00000c80: 4c6f 6f6b 7570 2063 616c 6c73 6967 6e20  Lookup callsign 
+00000c90: 696e 2063 7479 2e64 6174 2066 696c 652e  in cty.dat file.
+00000ca0: 0a0a 2320 2020 2020 5061 7261 6d65 7465  ..#     Paramete
+00000cb0: 7273 0a23 2020 2020 202d 2d2d 2d2d 2d2d  rs.#     -------
+00000cc0: 2d2d 2d0a 2320 2020 2020 6361 6c6c 7369  ---.#     callsi
+00000cd0: 676e 203a 2073 7472 0a0a 2320 2020 2020  gn : str..#     
+00000ce0: 5265 7475 726e 730a 2320 2020 2020 2d2d  Returns.#     --
+00000cf0: 2d2d 2d2d 2d0a 2320 2020 2020 7265 7375  -----.#     resu
+00000d00: 6c74 3a20 6c69 7374 0a23 2020 2020 2022  lt: list.#     "
+00000d10: 2222 0a23 2020 2020 2063 616c 6c73 6967  "".#     callsig
+00000d20: 6e20 3d20 6361 6c6c 7369 676e 2e75 7070  n = callsign.upp
+00000d30: 6572 2829 0a23 2020 2020 2066 6f72 2063  er().#     for c
+00000d40: 6f75 6e74 2069 6e20 7265 7665 7273 6564  ount in reversed
+00000d50: 2872 616e 6765 286c 656e 2863 616c 6c73  (range(len(calls
+00000d60: 6967 6e29 2929 3a0a 2320 2020 2020 2020  ign))):.#       
+00000d70: 2020 7365 6172 6368 6974 656d 203d 2063    searchitem = c
+00000d80: 616c 6c73 6967 6e5b 3a20 636f 756e 7420  allsign[: count 
+00000d90: 2b20 315d 0a23 2020 2020 2020 2020 2072  + 1].#         r
+00000da0: 6573 756c 7420 3d20 7b6b 6579 3a20 7661  esult = {key: va
+00000db0: 6c20 666f 7220 6b65 792c 2076 616c 2069  l for key, val i
+00000dc0: 6e20 4354 5946 494c 452e 6974 656d 7328  n CTYFILE.items(
+00000dd0: 2920 6966 206b 6579 203d 3d20 7365 6172  ) if key == sear
+00000de0: 6368 6974 656d 7d0a 2320 2020 2020 2020  chitem}.#       
+00000df0: 2020 6966 206e 6f74 2072 6573 756c 743a    if not result:
+00000e00: 0a23 2020 2020 2020 2020 2020 2020 2063  .#             c
+00000e10: 6f6e 7469 6e75 650a 2320 2020 2020 2020  ontinue.#       
+00000e20: 2020 6966 2072 6573 756c 742e 6765 7428    if result.get(
+00000e30: 7365 6172 6368 6974 656d 292e 6765 7428  searchitem).get(
+00000e40: 2265 7861 6374 5f6d 6174 6368 2229 3a0a  "exact_match"):.
+00000e50: 2320 2020 2020 2020 2020 2020 2020 6966  #             if
+00000e60: 2073 6561 7263 6869 7465 6d20 3d3d 2063   searchitem == c
+00000e70: 616c 6c73 6967 6e3a 0a23 2020 2020 2020  allsign:.#      
+00000e80: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00000e90: 6e20 7265 7375 6c74 0a23 2020 2020 2020  n result.#      
+00000ea0: 2020 2020 2020 2063 6f6e 7469 6e75 650a         continue.
+00000eb0: 2320 2020 2020 2020 2020 7265 7475 726e  #         return
+00000ec0: 2072 6573 756c 740a 0a0a 636c 6173 7320   result...class 
+00000ed0: 4d61 696e 5769 6e64 6f77 2851 7457 6964  MainWindow(QtWid
+00000ee0: 6765 7473 2e51 4d61 696e 5769 6e64 6f77  gets.QMainWindow
+00000ef0: 293a 0a20 2020 2022 2222 0a20 2020 2054  ):.    """.    T
+00000f00: 6865 206d 6169 6e20 7769 6e64 6f77 0a20  he main window. 
+00000f10: 2020 2022 2222 0a0a 2020 2020 7072 6566     """..    pref
+00000f20: 5f72 6566 203d 207b 0a20 2020 2020 2020  _ref = {.       
+00000f30: 2022 736f 756e 6464 6576 6963 6522 3a20   "sounddevice": 
+00000f40: 2264 6566 6175 6c74 222c 0a20 2020 2020  "default",.     
+00000f50: 2020 2022 7573 6571 727a 223a 2046 616c     "useqrz": Fal
+00000f60: 7365 2c0a 2020 2020 2020 2020 226c 6f6f  se,.        "loo
+00000f70: 6b75 7075 7365 726e 616d 6522 3a20 2275  kupusername": "u
+00000f80: 7365 726e 616d 6522 2c0a 2020 2020 2020  sername",.      
+00000f90: 2020 226c 6f6f 6b75 7070 6173 7377 6f72    "lookuppasswor
+00000fa0: 6422 3a20 2270 6173 7377 6f72 6422 2c0a  d": "password",.
+00000fb0: 2020 2020 2020 2020 2272 756e 5f73 7461          "run_sta
+00000fc0: 7465 223a 2054 7275 652c 0a20 2020 2020  te": True,.     
+00000fd0: 2020 2022 636f 6d6d 616e 645f 6275 7474     "command_butt
+00000fe0: 6f6e 7322 3a20 4661 6c73 652c 0a20 2020  ons": False,.   
+00000ff0: 2020 2020 2022 6377 5f6d 6163 726f 7322       "cw_macros"
+00001000: 3a20 5472 7565 2c0a 2020 2020 2020 2020  : True,.        
+00001010: 2262 616e 6473 5f6d 6f64 6573 223a 2054  "bands_modes": T
+00001020: 7275 652c 0a20 2020 2020 2020 2022 7769  rue,.        "wi
+00001030: 6e64 6f77 5f68 6569 6768 7422 3a20 3230  ndow_height": 20
+00001040: 302c 0a20 2020 2020 2020 2022 7769 6e64  0,.        "wind
+00001050: 6f77 5f77 6964 7468 223a 2036 3030 2c0a  ow_width": 600,.
+00001060: 2020 2020 2020 2020 2277 696e 646f 775f          "window_
+00001070: 7822 3a20 3132 302c 0a20 2020 2020 2020  x": 120,.       
+00001080: 2022 7769 6e64 6f77 5f79 223a 2031 3230   "window_y": 120
+00001090: 2c0a 2020 2020 2020 2020 2263 7572 7265  ,.        "curre
+000010a0: 6e74 5f64 6174 6162 6173 6522 3a20 2268  nt_database": "h
+000010b0: 616d 2e64 6222 2c0a 2020 2020 2020 2020  am.db",.        
+000010c0: 2263 6f6e 7465 7374 223a 2022 222c 0a20  "contest": "",. 
+000010d0: 2020 2020 2020 2022 6d75 6c74 6963 6173         "multicas
+000010e0: 745f 6772 6f75 7022 3a20 2232 3339 2e31  t_group": "239.1
+000010f0: 2e31 2e31 222c 0a20 2020 2020 2020 2022  .1.1",.        "
+00001100: 6d75 6c74 6963 6173 745f 706f 7274 223a  multicast_port":
+00001110: 2032 3233 392c 0a20 2020 2020 2020 2022   2239,.        "
+00001120: 696e 7465 7266 6163 655f 6970 223a 2022  interface_ip": "
+00001130: 302e 302e 302e 3022 2c0a 2020 2020 2020  0.0.0.0",.      
+00001140: 2020 2273 656e 645f 6e31 6d6d 5f70 6163    "send_n1mm_pac
+00001150: 6b65 7473 223a 2046 616c 7365 2c0a 2020  kets": False,.  
+00001160: 2020 2020 2020 226e 316d 6d5f 7374 6174        "n1mm_stat
+00001170: 696f 6e5f 6e61 6d65 223a 2022 3230 4d20  ion_name": "20M 
+00001180: 4357 2054 656e 7422 2c0a 2020 2020 2020  CW Tent",.      
+00001190: 2020 226e 316d 6d5f 6f70 6572 6174 6f72    "n1mm_operator
+000011a0: 223a 2022 4265 726e 6965 222c 0a20 2020  ": "Bernie",.   
+000011b0: 2020 2020 2022 6e31 6d6d 5f72 6164 696f       "n1mm_radio
+000011c0: 706f 7274 223a 2022 3132 372e 302e 302e  port": "127.0.0.
+000011d0: 313a 3132 3036 3022 2c0a 2020 2020 2020  1:12060",.      
+000011e0: 2020 226e 316d 6d5f 636f 6e74 6163 7470    "n1mm_contactp
+000011f0: 6f72 7422 3a20 2231 3237 2e30 2e30 2e31  ort": "127.0.0.1
+00001200: 3a31 3230 3630 222c 0a20 2020 2020 2020  :12060",.       
+00001210: 2022 6e31 6d6d 5f6c 6f6f 6b75 7070 6f72   "n1mm_lookuppor
+00001220: 7422 3a20 2231 3237 2e30 2e30 2e31 3a31  t": "127.0.0.1:1
+00001230: 3230 3630 222c 0a20 2020 2020 2020 2022  2060",.        "
+00001240: 6e31 6d6d 5f73 636f 7265 706f 7274 223a  n1mm_scoreport":
+00001250: 2022 3132 372e 302e 302e 313a 3132 3036   "127.0.0.1:1206
+00001260: 3022 2c0a 2020 2020 2020 2020 2275 7365  0",.        "use
+00001270: 6861 6d64 6222 3a20 4661 6c73 652c 0a20  hamdb": False,. 
+00001280: 2020 2020 2020 2022 7573 6568 616d 7174         "usehamqt
+00001290: 6822 3a20 4661 6c73 652c 0a20 2020 2020  h": False,.     
+000012a0: 2020 2022 636c 6f75 646c 6f67 223a 2046     "cloudlog": F
+000012b0: 616c 7365 2c0a 2020 2020 2020 2020 2263  alse,.        "c
+000012c0: 6c6f 7564 6c6f 6761 7069 223a 2022 222c  loudlogapi": "",
+000012d0: 0a20 2020 2020 2020 2022 636c 6f75 646c  .        "cloudl
+000012e0: 6f67 7572 6c22 3a20 2222 2c0a 2020 2020  ogurl": "",.    
+000012f0: 2020 2020 2243 4154 5f69 7022 3a20 2231      "CAT_ip": "1
+00001300: 3237 2e30 2e30 2e31 222c 0a20 2020 2020  27.0.0.1",.     
+00001310: 2020 2022 7573 6572 6967 6374 6c64 223a     "userigctld":
+00001320: 2046 616c 7365 2c0a 2020 2020 2020 2020   False,.        
+00001330: 2275 7365 666c 7269 6722 3a20 4661 6c73  "useflrig": Fals
+00001340: 652c 0a20 2020 2020 2020 2022 6377 6970  e,.        "cwip
+00001350: 223a 2022 3132 372e 302e 302e 3122 2c0a  ": "127.0.0.1",.
+00001360: 2020 2020 2020 2020 2263 7770 6f72 7422          "cwport"
+00001370: 3a20 3637 3839 2c0a 2020 2020 2020 2020  : 6789,.        
+00001380: 2263 7774 7970 6522 3a20 302c 0a20 2020  "cwtype": 0,.   
+00001390: 2020 2020 2022 7573 6573 6572 7665 7222       "useserver"
+000013a0: 3a20 4661 6c73 652c 0a20 2020 2020 2020  : False,.       
+000013b0: 2022 4341 545f 706f 7274 223a 2034 3533   "CAT_port": 453
+000013c0: 322c 0a20 2020 2020 2020 2022 636c 7573  2,.        "clus
+000013d0: 7465 725f 7365 7276 6572 223a 2022 6478  ter_server": "dx
+000013e0: 632e 6e63 376a 2e63 6f6d 222c 0a20 2020  c.nc7j.com",.   
+000013f0: 2020 2020 2022 636c 7573 7465 725f 706f       "cluster_po
+00001400: 7274 223a 2037 3337 332c 0a20 2020 2020  rt": 7373,.     
+00001410: 2020 2022 636c 7573 7465 725f 6669 6c74     "cluster_filt
+00001420: 6572 223a 2022 5365 7420 4458 2046 696c  er": "Set DX Fil
+00001430: 7465 7220 5370 6f74 7465 7243 6f6e 743d  ter SpotterCont=
+00001440: 4e41 222c 0a20 2020 2020 2020 2022 636c  NA",.        "cl
+00001450: 7573 7465 725f 6d6f 6465 223a 2022 4f50  uster_mode": "OP
+00001460: 454e 222c 0a20 2020 207d 0a20 2020 2061  EN",.    }.    a
+00001470: 7070 7374 6172 7465 6420 3d20 4661 6c73  ppstarted = Fals
+00001480: 650a 2020 2020 636f 6e74 6163 7420 3d20  e.    contact = 
+00001490: 7b7d 0a20 2020 2063 6f6e 7465 7374 203d  {}.    contest =
+000014a0: 204e 6f6e 650a 2020 2020 636f 6e74 6573   None.    contes
+000014b0: 745f 7365 7474 696e 6773 203d 207b 7d0a  t_settings = {}.
+000014c0: 2020 2020 7072 6566 203d 204e 6f6e 650a      pref = None.
+000014d0: 2020 2020 7374 6174 696f 6e20 3d20 7b7d      station = {}
+000014e0: 0a20 2020 2063 7572 7265 6e74 5f6f 7020  .    current_op 
+000014f0: 3d20 2222 0a20 2020 2063 7572 7265 6e74  = "".    current
+00001500: 5f6d 6f64 6520 3d20 2222 0a20 2020 2063  _mode = "".    c
+00001510: 7572 7265 6e74 5f62 616e 6420 3d20 2222  urrent_band = ""
+00001520: 0a20 2020 2064 6566 6175 6c74 5f72 7374  .    default_rst
+00001530: 203d 2022 3539 220a 2020 2020 6377 203d   = "59".    cw =
+00001540: 204e 6f6e 650a 2020 2020 6c6f 6f6b 5f75   None.    look_u
+00001550: 7020 3d20 4e6f 6e65 0a20 2020 2072 756e  p = None.    run
+00001560: 5f73 7461 7465 203d 2046 616c 7365 0a20  _state = False. 
+00001570: 2020 2066 6b65 7973 203d 207b 7d0a 2020     fkeys = {}.  
+00001580: 2020 6162 6f75 745f 6469 616c 6f67 203d    about_dialog =
+00001590: 204e 6f6e 650a 2020 2020 7172 7a5f 6469   None.    qrz_di
+000015a0: 616c 6f67 203d 204e 6f6e 650a 2020 2020  alog = None.    
+000015b0: 7365 7474 696e 6773 5f64 6961 6c6f 6720  settings_dialog 
+000015c0: 3d20 4e6f 6e65 0a20 2020 2065 6469 745f  = None.    edit_
+000015d0: 6d61 6372 6f5f 6469 616c 6f67 203d 204e  macro_dialog = N
+000015e0: 6f6e 650a 2020 2020 636f 6e74 6573 745f  one.    contest_
+000015f0: 6469 616c 6f67 203d 204e 6f6e 650a 2020  dialog = None.  
+00001600: 2020 636f 6e66 6967 7572 6174 696f 6e5f    configuration_
+00001610: 6469 616c 6f67 203d 204e 6f6e 650a 2020  dialog = None.  
+00001620: 2020 6f70 6f6e 5f64 6961 6c6f 6720 3d20    opon_dialog = 
+00001630: 4e6f 6e65 0a20 2020 2064 626e 616d 6520  None.    dbname 
+00001640: 3d20 4441 5441 5f50 4154 4820 2b20 222f  = DATA_PATH + "/
+00001650: 6861 6d2e 6462 220a 2020 2020 7261 6469  ham.db".    radi
+00001660: 6f5f 7374 6174 6520 3d20 7b7d 0a20 2020  o_state = {}.   
+00001670: 2072 6967 5f63 6f6e 7472 6f6c 203d 204e   rig_control = N
+00001680: 6f6e 650a 2020 2020 6d75 6c74 6963 6173  one.    multicas
+00001690: 745f 6772 6f75 7020 3d20 4e6f 6e65 0a20  t_group = None. 
+000016a0: 2020 206d 756c 7469 6361 7374 5f70 6f72     multicast_por
+000016b0: 7420 3d20 4e6f 6e65 0a20 2020 2069 6e74  t = None.    int
+000016c0: 6572 6661 6365 5f69 7020 3d20 4e6f 6e65  erface_ip = None
+000016d0: 0a20 2020 2072 6967 5f63 6f6e 7472 6f6c  .    rig_control
+000016e0: 203d 204e 6f6e 650a 0a20 2020 2064 6566   = None..    def
+000016f0: 205f 5f69 6e69 745f 5f28 7365 6c66 2c20   __init__(self, 
+00001700: 2a61 7267 732c 202a 2a6b 7761 7267 7329  *args, **kwargs)
+00001710: 3a0a 2020 2020 2020 2020 7375 7065 7228  :.        super(
+00001720: 292e 5f5f 696e 6974 5f5f 282a 6172 6773  ).__init__(*args
+00001730: 2c20 2a2a 6b77 6172 6773 290a 2020 2020  , **kwargs).    
+00001740: 2020 2020 6c6f 6767 6572 2e69 6e66 6f28      logger.info(
+00001750: 224d 6169 6e57 696e 646f 773a 205f 5f69  "MainWindow: __i
+00001760: 6e69 745f 5f22 290a 2020 2020 2020 2020  nit__").        
+00001770: 6461 7461 5f70 6174 6820 3d20 574f 524b  data_path = WORK
+00001780: 494e 475f 5041 5448 202b 2022 2f64 6174  ING_PATH + "/dat
+00001790: 612f 6d61 696e 2e75 6922 0a20 2020 2020  a/main.ui".     
+000017a0: 2020 2075 6963 2e6c 6f61 6455 6928 6461     uic.loadUi(da
+000017b0: 7461 5f70 6174 682c 2073 656c 6629 0a20  ta_path, self). 
+000017c0: 2020 2020 2020 2073 656c 662e 6c65 6674         self.left
+000017d0: 646f 742e 6869 6465 2829 0a20 2020 2020  dot.hide().     
+000017e0: 2020 2073 656c 662e 7269 6768 7464 6f74     self.rightdot
+000017f0: 2e68 6964 6528 290a 2020 2020 2020 2020  .hide().        
+00001800: 7365 6c66 2e6e 316d 6d20 3d20 4e31 4d4d  self.n1mm = N1MM
+00001810: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
+00001820: 6e65 7874 5f66 6965 6c64 203d 2073 656c  next_field = sel
+00001830: 662e 6f74 6865 725f 320a 2020 2020 2020  f.other_2.      
+00001840: 2020 7365 6c66 2e64 7570 655f 696e 6469    self.dupe_indi
+00001850: 6361 746f 722e 6869 6465 2829 0a20 2020  cator.hide().   
+00001860: 2020 2020 2073 656c 662e 6377 5f73 7065       self.cw_spe
+00001870: 6564 2e76 616c 7565 4368 616e 6765 642e  ed.valueChanged.
+00001880: 636f 6e6e 6563 7428 7365 6c66 2e63 7773  connect(self.cws
+00001890: 7065 6564 5f73 7069 6e62 6f78 5f63 6861  peed_spinbox_cha
+000018a0: 6e67 6564 290a 0a20 2020 2020 2020 2073  nged)..        s
+000018b0: 656c 662e 6163 7469 6f6e 4357 5f4d 6163  elf.actionCW_Mac
+000018c0: 726f 732e 7472 6967 6765 7265 642e 636f  ros.triggered.co
+000018d0: 6e6e 6563 7428 7365 6c66 2e63 775f 6d61  nnect(self.cw_ma
+000018e0: 6372 6f73 5f73 7461 7465 5f63 6861 6e67  cros_state_chang
+000018f0: 6564 290a 2020 2020 2020 2020 7365 6c66  ed).        self
+00001900: 2e61 6374 696f 6e43 6f6d 6d61 6e64 5f42  .actionCommand_B
+00001910: 7574 746f 6e73 2e74 7269 6767 6572 6564  uttons.triggered
+00001920: 2e63 6f6e 6e65 6374 2873 656c 662e 636f  .connect(self.co
+00001930: 6d6d 616e 645f 6275 7474 6f6e 735f 7374  mmand_buttons_st
+00001940: 6174 655f 6368 616e 6765 290a 2020 2020  ate_change).    
+00001950: 2020 2020 7365 6c66 2e61 6374 696f 6e4c      self.actionL
+00001960: 6f67 5f57 696e 646f 772e 7472 6967 6765  og_Window.trigge
+00001970: 7265 642e 636f 6e6e 6563 7428 7365 6c66  red.connect(self
+00001980: 2e6c 6175 6e63 685f 6c6f 675f 7769 6e64  .launch_log_wind
 00001990: 6f77 290a 2020 2020 2020 2020 7365 6c66  ow).        self
-000019a0: 2e61 6374 696f 6e52 6563 616c 6375 6c61  .actionRecalcula
-000019b0: 7465 5f4d 756c 7473 2e74 7269 6767 6572  te_Mults.trigger
-000019c0: 6564 2e63 6f6e 6e65 6374 2873 656c 662e  ed.connect(self.
-000019d0: 7265 6361 6c63 756c 6174 655f 6d75 6c74  recalculate_mult
-000019e0: 7329 0a0a 2020 2020 2020 2020 7365 6c66  s)..        self
-000019f0: 2e61 6374 696f 6e47 656e 6572 6174 655f  .actionGenerate_
-00001a00: 4361 6272 696c 6c6f 2e74 7269 6767 6572  Cabrillo.trigger
-00001a10: 6564 2e63 6f6e 6e65 6374 2873 656c 662e  ed.connect(self.
-00001a20: 6765 6e65 7261 7465 5f63 6162 7269 6c6c  generate_cabrill
-00001a30: 6f29 0a20 2020 2020 2020 2073 656c 662e  o).        self.
-00001a40: 6163 7469 6f6e 4765 6e65 7261 7465 5f41  actionGenerate_A
-00001a50: 4449 462e 7472 6967 6765 7265 642e 636f  DIF.triggered.co
-00001a60: 6e6e 6563 7428 7365 6c66 2e67 656e 6572  nnect(self.gener
-00001a70: 6174 655f 6164 6966 290a 0a20 2020 2020  ate_adif)..     
-00001a80: 2020 2073 656c 662e 6163 7469 6f6e 436f     self.actionCo
-00001a90: 6e66 6967 7572 6174 696f 6e5f 5365 7474  nfiguration_Sett
-00001aa0: 696e 6773 2e74 7269 6767 6572 6564 2e63  ings.triggered.c
-00001ab0: 6f6e 6e65 6374 280a 2020 2020 2020 2020  onnect(.        
-00001ac0: 2020 2020 7365 6c66 2e65 6469 745f 636f      self.edit_co
-00001ad0: 6e66 6967 7572 6174 696f 6e5f 7365 7474  nfiguration_sett
-00001ae0: 696e 6773 0a20 2020 2020 2020 2029 0a20  ings.        ). 
-00001af0: 2020 2020 2020 2073 656c 662e 6163 7469         self.acti
-00001b00: 6f6e 5374 6174 696f 6e53 6574 7469 6e67  onStationSetting
-00001b10: 732e 7472 6967 6765 7265 642e 636f 6e6e  s.triggered.conn
-00001b20: 6563 7428 7365 6c66 2e65 6469 745f 7374  ect(self.edit_st
-00001b30: 6174 696f 6e5f 7365 7474 696e 6773 290a  ation_settings).
-00001b40: 0a20 2020 2020 2020 2073 656c 662e 6163  .        self.ac
-00001b50: 7469 6f6e 4e65 775f 436f 6e74 6573 742e  tionNew_Contest.
-00001b60: 7472 6967 6765 7265 642e 636f 6e6e 6563  triggered.connec
-00001b70: 7428 7365 6c66 2e6e 6577 5f63 6f6e 7465  t(self.new_conte
-00001b80: 7374 5f64 6961 6c6f 6729 0a20 2020 2020  st_dialog).     
-00001b90: 2020 2073 656c 662e 6163 7469 6f6e 4f70     self.actionOp
-00001ba0: 656e 5f43 6f6e 7465 7374 2e74 7269 6767  en_Contest.trigg
-00001bb0: 6572 6564 2e63 6f6e 6e65 6374 2873 656c  ered.connect(sel
-00001bc0: 662e 6f70 656e 5f63 6f6e 7465 7374 290a  f.open_contest).
-00001bd0: 2020 2020 2020 2020 7365 6c66 2e61 6374          self.act
-00001be0: 696f 6e45 6469 745f 4375 7272 656e 745f  ionEdit_Current_
-00001bf0: 436f 6e74 6573 742e 7472 6967 6765 7265  Contest.triggere
-00001c00: 642e 636f 6e6e 6563 7428 7365 6c66 2e65  d.connect(self.e
-00001c10: 6469 745f 636f 6e74 6573 7429 0a0a 2020  dit_contest)..  
-00001c20: 2020 2020 2020 7365 6c66 2e61 6374 696f        self.actio
-00001c30: 6e4e 6577 5f44 6174 6162 6173 652e 7472  nNew_Database.tr
-00001c40: 6967 6765 7265 642e 636f 6e6e 6563 7428  iggered.connect(
-00001c50: 7365 6c66 2e6e 6577 5f64 6174 6162 6173  self.new_databas
-00001c60: 6529 0a20 2020 2020 2020 2073 656c 662e  e).        self.
-00001c70: 6163 7469 6f6e 4f70 656e 5f44 6174 6162  actionOpen_Datab
-00001c80: 6173 652e 7472 6967 6765 7265 642e 636f  ase.triggered.co
-00001c90: 6e6e 6563 7428 7365 6c66 2e6f 7065 6e5f  nnect(self.open_
-00001ca0: 6461 7461 6261 7365 290a 0a20 2020 2020  database)..     
-00001cb0: 2020 2073 656c 662e 6163 7469 6f6e 4564     self.actionEd
-00001cc0: 6974 5f4d 6163 726f 732e 7472 6967 6765  it_Macros.trigge
-00001cd0: 7265 642e 636f 6e6e 6563 7428 7365 6c66  red.connect(self
-00001ce0: 2e65 6469 745f 6377 5f6d 6163 726f 7329  .edit_cw_macros)
-00001cf0: 0a0a 2020 2020 2020 2020 7365 6c66 2e61  ..        self.a
-00001d00: 6374 696f 6e41 626f 7574 2e74 7269 6767  ctionAbout.trigg
-00001d10: 6572 6564 2e63 6f6e 6e65 6374 2873 656c  ered.connect(sel
-00001d20: 662e 7368 6f77 5f61 626f 7574 5f64 6961  f.show_about_dia
-00001d30: 6c6f 6729 0a20 2020 2020 2020 2073 656c  log).        sel
-00001d40: 662e 6163 7469 6f6e 486f 744b 6579 732e  f.actionHotKeys.
-00001d50: 7472 6967 6765 7265 642e 636f 6e6e 6563  triggered.connec
-00001d60: 7428 7365 6c66 2e73 686f 775f 6b65 795f  t(self.show_key_
-00001d70: 6865 6c70 290a 2020 2020 2020 2020 7365  help).        se
-00001d80: 6c66 2e61 6374 696f 6e48 656c 702e 7472  lf.actionHelp.tr
-00001d90: 6967 6765 7265 642e 636f 6e6e 6563 7428  iggered.connect(
-00001da0: 7365 6c66 2e73 686f 775f 6865 6c70 5f64  self.show_help_d
-00001db0: 6961 6c6f 6729 0a20 2020 2020 2020 2073  ialog).        s
-00001dc0: 656c 662e 6163 7469 6f6e 5570 6461 7465  elf.actionUpdate
-00001dd0: 5f43 5459 2e74 7269 6767 6572 6564 2e63  _CTY.triggered.c
-00001de0: 6f6e 6e65 6374 2873 656c 662e 6368 6563  onnect(self.chec
-00001df0: 6b5f 666f 725f 6e65 775f 6374 7929 0a20  k_for_new_cty). 
-00001e00: 2020 2020 2020 2073 656c 662e 6163 7469         self.acti
-00001e10: 6f6e 5570 6461 7465 5f4d 4153 5445 525f  onUpdate_MASTER_
-00001e20: 5343 502e 7472 6967 6765 7265 642e 636f  SCP.triggered.co
-00001e30: 6e6e 6563 7428 7365 6c66 2e75 7064 6174  nnect(self.updat
-00001e40: 655f 6d61 7374 6572 7363 7029 0a20 2020  e_masterscp).   
-00001e50: 2020 2020 2073 656c 662e 6163 7469 6f6e       self.action
-00001e60: 5175 6974 2e74 7269 6767 6572 6564 2e63  Quit.triggered.c
-00001e70: 6f6e 6e65 6374 2873 656c 662e 7175 6974  onnect(self.quit
-00001e80: 5f61 7070 290a 0a20 2020 2020 2020 2073  _app)..        s
-00001e90: 656c 662e 7261 6469 6f42 7574 746f 6e5f  elf.radioButton_
-00001ea0: 7275 6e2e 636c 6963 6b65 642e 636f 6e6e  run.clicked.conn
-00001eb0: 6563 7428 7365 6c66 2e72 756e 5f73 705f  ect(self.run_sp_
-00001ec0: 6275 7474 6f6e 735f 636c 6963 6b65 6429  buttons_clicked)
-00001ed0: 0a20 2020 2020 2020 2073 656c 662e 7261  .        self.ra
-00001ee0: 6469 6f42 7574 746f 6e5f 7370 2e63 6c69  dioButton_sp.cli
+000019a0: 2e61 6374 696f 6e42 616e 646d 6170 2e74  .actionBandmap.t
+000019b0: 7269 6767 6572 6564 2e63 6f6e 6e65 6374  riggered.connect
+000019c0: 2873 656c 662e 6c61 756e 6368 5f62 616e  (self.launch_ban
+000019d0: 646d 6170 5f77 696e 646f 7729 0a20 2020  dmap_window).   
+000019e0: 2020 2020 2073 656c 662e 6163 7469 6f6e       self.action
+000019f0: 5265 6361 6c63 756c 6174 655f 4d75 6c74  Recalculate_Mult
+00001a00: 732e 7472 6967 6765 7265 642e 636f 6e6e  s.triggered.conn
+00001a10: 6563 7428 7365 6c66 2e72 6563 616c 6375  ect(self.recalcu
+00001a20: 6c61 7465 5f6d 756c 7473 290a 0a20 2020  late_mults)..   
+00001a30: 2020 2020 2073 656c 662e 6163 7469 6f6e       self.action
+00001a40: 4765 6e65 7261 7465 5f43 6162 7269 6c6c  Generate_Cabrill
+00001a50: 6f2e 7472 6967 6765 7265 642e 636f 6e6e  o.triggered.conn
+00001a60: 6563 7428 7365 6c66 2e67 656e 6572 6174  ect(self.generat
+00001a70: 655f 6361 6272 696c 6c6f 290a 2020 2020  e_cabrillo).    
+00001a80: 2020 2020 7365 6c66 2e61 6374 696f 6e47      self.actionG
+00001a90: 656e 6572 6174 655f 4144 4946 2e74 7269  enerate_ADIF.tri
+00001aa0: 6767 6572 6564 2e63 6f6e 6e65 6374 2873  ggered.connect(s
+00001ab0: 656c 662e 6765 6e65 7261 7465 5f61 6469  elf.generate_adi
+00001ac0: 6629 0a0a 2020 2020 2020 2020 7365 6c66  f)..        self
+00001ad0: 2e61 6374 696f 6e43 6f6e 6669 6775 7261  .actionConfigura
+00001ae0: 7469 6f6e 5f53 6574 7469 6e67 732e 7472  tion_Settings.tr
+00001af0: 6967 6765 7265 642e 636f 6e6e 6563 7428  iggered.connect(
+00001b00: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00001b10: 662e 6564 6974 5f63 6f6e 6669 6775 7261  f.edit_configura
+00001b20: 7469 6f6e 5f73 6574 7469 6e67 730a 2020  tion_settings.  
+00001b30: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00001b40: 7365 6c66 2e61 6374 696f 6e53 7461 7469  self.actionStati
+00001b50: 6f6e 5365 7474 696e 6773 2e74 7269 6767  onSettings.trigg
+00001b60: 6572 6564 2e63 6f6e 6e65 6374 2873 656c  ered.connect(sel
+00001b70: 662e 6564 6974 5f73 7461 7469 6f6e 5f73  f.edit_station_s
+00001b80: 6574 7469 6e67 7329 0a0a 2020 2020 2020  ettings)..      
+00001b90: 2020 7365 6c66 2e61 6374 696f 6e4e 6577    self.actionNew
+00001ba0: 5f43 6f6e 7465 7374 2e74 7269 6767 6572  _Contest.trigger
+00001bb0: 6564 2e63 6f6e 6e65 6374 2873 656c 662e  ed.connect(self.
+00001bc0: 6e65 775f 636f 6e74 6573 745f 6469 616c  new_contest_dial
+00001bd0: 6f67 290a 2020 2020 2020 2020 7365 6c66  og).        self
+00001be0: 2e61 6374 696f 6e4f 7065 6e5f 436f 6e74  .actionOpen_Cont
+00001bf0: 6573 742e 7472 6967 6765 7265 642e 636f  est.triggered.co
+00001c00: 6e6e 6563 7428 7365 6c66 2e6f 7065 6e5f  nnect(self.open_
+00001c10: 636f 6e74 6573 7429 0a20 2020 2020 2020  contest).       
+00001c20: 2073 656c 662e 6163 7469 6f6e 4564 6974   self.actionEdit
+00001c30: 5f43 7572 7265 6e74 5f43 6f6e 7465 7374  _Current_Contest
+00001c40: 2e74 7269 6767 6572 6564 2e63 6f6e 6e65  .triggered.conne
+00001c50: 6374 2873 656c 662e 6564 6974 5f63 6f6e  ct(self.edit_con
+00001c60: 7465 7374 290a 0a20 2020 2020 2020 2073  test)..        s
+00001c70: 656c 662e 6163 7469 6f6e 4e65 775f 4461  elf.actionNew_Da
+00001c80: 7461 6261 7365 2e74 7269 6767 6572 6564  tabase.triggered
+00001c90: 2e63 6f6e 6e65 6374 2873 656c 662e 6e65  .connect(self.ne
+00001ca0: 775f 6461 7461 6261 7365 290a 2020 2020  w_database).    
+00001cb0: 2020 2020 7365 6c66 2e61 6374 696f 6e4f      self.actionO
+00001cc0: 7065 6e5f 4461 7461 6261 7365 2e74 7269  pen_Database.tri
+00001cd0: 6767 6572 6564 2e63 6f6e 6e65 6374 2873  ggered.connect(s
+00001ce0: 656c 662e 6f70 656e 5f64 6174 6162 6173  elf.open_databas
+00001cf0: 6529 0a0a 2020 2020 2020 2020 7365 6c66  e)..        self
+00001d00: 2e61 6374 696f 6e45 6469 745f 4d61 6372  .actionEdit_Macr
+00001d10: 6f73 2e74 7269 6767 6572 6564 2e63 6f6e  os.triggered.con
+00001d20: 6e65 6374 2873 656c 662e 6564 6974 5f63  nect(self.edit_c
+00001d30: 775f 6d61 6372 6f73 290a 0a20 2020 2020  w_macros)..     
+00001d40: 2020 2073 656c 662e 6163 7469 6f6e 4162     self.actionAb
+00001d50: 6f75 742e 7472 6967 6765 7265 642e 636f  out.triggered.co
+00001d60: 6e6e 6563 7428 7365 6c66 2e73 686f 775f  nnect(self.show_
+00001d70: 6162 6f75 745f 6469 616c 6f67 290a 2020  about_dialog).  
+00001d80: 2020 2020 2020 7365 6c66 2e61 6374 696f        self.actio
+00001d90: 6e48 6f74 4b65 7973 2e74 7269 6767 6572  nHotKeys.trigger
+00001da0: 6564 2e63 6f6e 6e65 6374 2873 656c 662e  ed.connect(self.
+00001db0: 7368 6f77 5f6b 6579 5f68 656c 7029 0a20  show_key_help). 
+00001dc0: 2020 2020 2020 2073 656c 662e 6163 7469         self.acti
+00001dd0: 6f6e 4865 6c70 2e74 7269 6767 6572 6564  onHelp.triggered
+00001de0: 2e63 6f6e 6e65 6374 2873 656c 662e 7368  .connect(self.sh
+00001df0: 6f77 5f68 656c 705f 6469 616c 6f67 290a  ow_help_dialog).
+00001e00: 2020 2020 2020 2020 7365 6c66 2e61 6374          self.act
+00001e10: 696f 6e55 7064 6174 655f 4354 592e 7472  ionUpdate_CTY.tr
+00001e20: 6967 6765 7265 642e 636f 6e6e 6563 7428  iggered.connect(
+00001e30: 7365 6c66 2e63 6865 636b 5f66 6f72 5f6e  self.check_for_n
+00001e40: 6577 5f63 7479 290a 2020 2020 2020 2020  ew_cty).        
+00001e50: 7365 6c66 2e61 6374 696f 6e55 7064 6174  self.actionUpdat
+00001e60: 655f 4d41 5354 4552 5f53 4350 2e74 7269  e_MASTER_SCP.tri
+00001e70: 6767 6572 6564 2e63 6f6e 6e65 6374 2873  ggered.connect(s
+00001e80: 656c 662e 7570 6461 7465 5f6d 6173 7465  elf.update_maste
+00001e90: 7273 6370 290a 2020 2020 2020 2020 7365  rscp).        se
+00001ea0: 6c66 2e61 6374 696f 6e51 7569 742e 7472  lf.actionQuit.tr
+00001eb0: 6967 6765 7265 642e 636f 6e6e 6563 7428  iggered.connect(
+00001ec0: 7365 6c66 2e71 7569 745f 6170 7029 0a0a  self.quit_app)..
+00001ed0: 2020 2020 2020 2020 7365 6c66 2e72 6164          self.rad
+00001ee0: 696f 4275 7474 6f6e 5f72 756e 2e63 6c69  ioButton_run.cli
 00001ef0: 636b 6564 2e63 6f6e 6e65 6374 2873 656c  cked.connect(sel
 00001f00: 662e 7275 6e5f 7370 5f62 7574 746f 6e73  f.run_sp_buttons
 00001f10: 5f63 6c69 636b 6564 290a 2020 2020 2020  _clicked).      
-00001f20: 2020 7365 6c66 2e73 636f 7265 2e73 6574    self.score.set
-00001f30: 5465 7874 2822 3022 290a 2020 2020 2020  Text("0").      
-00001f40: 2020 7365 6c66 2e63 616c 6c73 6967 6e2e    self.callsign.
-00001f50: 7465 7874 4564 6974 6564 2e63 6f6e 6e65  textEdited.conne
-00001f60: 6374 2873 656c 662e 6361 6c6c 7369 676e  ct(self.callsign
-00001f70: 5f63 6861 6e67 6564 290a 2020 2020 2020  _changed).      
-00001f80: 2020 7365 6c66 2e63 616c 6c73 6967 6e2e    self.callsign.
-00001f90: 7265 7475 726e 5072 6573 7365 642e 636f  returnPressed.co
-00001fa0: 6e6e 6563 7428 7365 6c66 2e73 6176 655f  nnect(self.save_
-00001fb0: 636f 6e74 6163 7429 0a20 2020 2020 2020  contact).       
-00001fc0: 2073 656c 662e 7365 6e74 2e72 6574 7572   self.sent.retur
-00001fd0: 6e50 7265 7373 6564 2e63 6f6e 6e65 6374  nPressed.connect
-00001fe0: 2873 656c 662e 7361 7665 5f63 6f6e 7461  (self.save_conta
-00001ff0: 6374 290a 2020 2020 2020 2020 7365 6c66  ct).        self
-00002000: 2e72 6563 6569 7665 2e72 6574 7572 6e50  .receive.returnP
-00002010: 7265 7373 6564 2e63 6f6e 6e65 6374 2873  ressed.connect(s
-00002020: 656c 662e 7361 7665 5f63 6f6e 7461 6374  elf.save_contact
-00002030: 290a 2020 2020 2020 2020 7365 6c66 2e6f  ).        self.o
-00002040: 7468 6572 5f31 2e72 6574 7572 6e50 7265  ther_1.returnPre
-00002050: 7373 6564 2e63 6f6e 6e65 6374 2873 656c  ssed.connect(sel
-00002060: 662e 7361 7665 5f63 6f6e 7461 6374 290a  f.save_contact).
-00002070: 2020 2020 2020 2020 7365 6c66 2e6f 7468          self.oth
-00002080: 6572 5f32 2e72 6574 7572 6e50 7265 7373  er_2.returnPress
-00002090: 6564 2e63 6f6e 6e65 6374 2873 656c 662e  ed.connect(self.
-000020a0: 7361 7665 5f63 6f6e 7461 6374 290a 2020  save_contact).  
-000020b0: 2020 2020 2020 7365 6c66 2e6f 7468 6572        self.other
-000020c0: 5f32 2e74 6578 7445 6469 7465 642e 636f  _2.textEdited.co
-000020d0: 6e6e 6563 7428 7365 6c66 2e6f 7468 6572  nnect(self.other
-000020e0: 5f32 5f63 6861 6e67 6564 290a 0a20 2020  _2_changed)..   
-000020f0: 2020 2020 2073 656c 662e 7365 6e74 2e73       self.sent.s
-00002100: 6574 5465 7874 2822 3539 2229 0a20 2020  etText("59").   
-00002110: 2020 2020 2073 656c 662e 7265 6365 6976       self.receiv
-00002120: 652e 7365 7454 6578 7428 2235 3922 290a  e.setText("59").
-00002130: 2020 2020 2020 2020 6963 6f6e 5f70 6174          icon_pat
-00002140: 6820 3d20 574f 524b 494e 475f 5041 5448  h = WORKING_PATH
-00002150: 202b 2022 2f64 6174 612f 220a 2020 2020   + "/data/".    
-00002160: 2020 2020 7365 6c66 2e67 7265 656e 646f      self.greendo
-00002170: 7420 3d20 5174 4775 692e 5150 6978 6d61  t = QtGui.QPixma
-00002180: 7028 6963 6f6e 5f70 6174 6820 2b20 2267  p(icon_path + "g
-00002190: 7265 656e 646f 742e 706e 6722 290a 2020  reendot.png").  
-000021a0: 2020 2020 2020 7365 6c66 2e72 6564 646f        self.reddo
-000021b0: 7420 3d20 5174 4775 692e 5150 6978 6d61  t = QtGui.QPixma
-000021c0: 7028 6963 6f6e 5f70 6174 6820 2b20 2272  p(icon_path + "r
-000021d0: 6564 646f 742e 706e 6722 290a 2020 2020  eddot.png").    
-000021e0: 2020 2020 7365 6c66 2e6c 6566 7464 6f74      self.leftdot
-000021f0: 2e73 6574 5069 786d 6170 2873 656c 662e  .setPixmap(self.
-00002200: 6772 6565 6e64 6f74 290a 2020 2020 2020  greendot).      
-00002210: 2020 7365 6c66 2e72 6967 6874 646f 742e    self.rightdot.
-00002220: 7365 7450 6978 6d61 7028 7365 6c66 2e72  setPixmap(self.r
-00002230: 6564 646f 7429 0a0a 2020 2020 2020 2020  eddot)..        
-00002240: 7365 6c66 2e46 312e 7365 7443 6f6e 7465  self.F1.setConte
-00002250: 7874 4d65 6e75 506f 6c69 6379 2851 7443  xtMenuPolicy(QtC
-00002260: 6f72 652e 5174 2e43 7573 746f 6d43 6f6e  ore.Qt.CustomCon
-00002270: 7465 7874 4d65 6e75 290a 2020 2020 2020  textMenu).      
-00002280: 2020 7365 6c66 2e46 312e 6375 7374 6f6d    self.F1.custom
-00002290: 436f 6e74 6578 744d 656e 7552 6571 7565  ContextMenuReque
-000022a0: 7374 6564 2e63 6f6e 6e65 6374 2873 656c  sted.connect(sel
-000022b0: 662e 6564 6974 5f46 3129 0a20 2020 2020  f.edit_F1).     
-000022c0: 2020 2073 656c 662e 4631 2e63 6c69 636b     self.F1.click
-000022d0: 6564 2e63 6f6e 6e65 6374 2873 656c 662e  ed.connect(self.
-000022e0: 7365 6e64 6631 290a 2020 2020 2020 2020  sendf1).        
-000022f0: 7365 6c66 2e46 322e 7365 7443 6f6e 7465  self.F2.setConte
-00002300: 7874 4d65 6e75 506f 6c69 6379 2851 7443  xtMenuPolicy(QtC
-00002310: 6f72 652e 5174 2e43 7573 746f 6d43 6f6e  ore.Qt.CustomCon
-00002320: 7465 7874 4d65 6e75 290a 2020 2020 2020  textMenu).      
-00002330: 2020 7365 6c66 2e46 322e 6375 7374 6f6d    self.F2.custom
-00002340: 436f 6e74 6578 744d 656e 7552 6571 7565  ContextMenuReque
-00002350: 7374 6564 2e63 6f6e 6e65 6374 2873 656c  sted.connect(sel
-00002360: 662e 6564 6974 5f46 3229 0a20 2020 2020  f.edit_F2).     
-00002370: 2020 2073 656c 662e 4632 2e63 6c69 636b     self.F2.click
-00002380: 6564 2e63 6f6e 6e65 6374 2873 656c 662e  ed.connect(self.
-00002390: 7365 6e64 6632 290a 2020 2020 2020 2020  sendf2).        
-000023a0: 7365 6c66 2e46 332e 7365 7443 6f6e 7465  self.F3.setConte
-000023b0: 7874 4d65 6e75 506f 6c69 6379 2851 7443  xtMenuPolicy(QtC
-000023c0: 6f72 652e 5174 2e43 7573 746f 6d43 6f6e  ore.Qt.CustomCon
-000023d0: 7465 7874 4d65 6e75 290a 2020 2020 2020  textMenu).      
-000023e0: 2020 7365 6c66 2e46 332e 6375 7374 6f6d    self.F3.custom
-000023f0: 436f 6e74 6578 744d 656e 7552 6571 7565  ContextMenuReque
-00002400: 7374 6564 2e63 6f6e 6e65 6374 2873 656c  sted.connect(sel
-00002410: 662e 6564 6974 5f46 3329 0a20 2020 2020  f.edit_F3).     
-00002420: 2020 2073 656c 662e 4633 2e63 6c69 636b     self.F3.click
-00002430: 6564 2e63 6f6e 6e65 6374 2873 656c 662e  ed.connect(self.
-00002440: 7365 6e64 6633 290a 2020 2020 2020 2020  sendf3).        
-00002450: 7365 6c66 2e46 342e 7365 7443 6f6e 7465  self.F4.setConte
-00002460: 7874 4d65 6e75 506f 6c69 6379 2851 7443  xtMenuPolicy(QtC
-00002470: 6f72 652e 5174 2e43 7573 746f 6d43 6f6e  ore.Qt.CustomCon
-00002480: 7465 7874 4d65 6e75 290a 2020 2020 2020  textMenu).      
-00002490: 2020 7365 6c66 2e46 342e 6375 7374 6f6d    self.F4.custom
-000024a0: 436f 6e74 6578 744d 656e 7552 6571 7565  ContextMenuReque
-000024b0: 7374 6564 2e63 6f6e 6e65 6374 2873 656c  sted.connect(sel
-000024c0: 662e 6564 6974 5f46 3429 0a20 2020 2020  f.edit_F4).     
-000024d0: 2020 2073 656c 662e 4634 2e63 6c69 636b     self.F4.click
-000024e0: 6564 2e63 6f6e 6e65 6374 2873 656c 662e  ed.connect(self.
-000024f0: 7365 6e64 6634 290a 2020 2020 2020 2020  sendf4).        
-00002500: 7365 6c66 2e46 352e 7365 7443 6f6e 7465  self.F5.setConte
-00002510: 7874 4d65 6e75 506f 6c69 6379 2851 7443  xtMenuPolicy(QtC
-00002520: 6f72 652e 5174 2e43 7573 746f 6d43 6f6e  ore.Qt.CustomCon
-00002530: 7465 7874 4d65 6e75 290a 2020 2020 2020  textMenu).      
-00002540: 2020 7365 6c66 2e46 352e 6375 7374 6f6d    self.F5.custom
-00002550: 436f 6e74 6578 744d 656e 7552 6571 7565  ContextMenuReque
-00002560: 7374 6564 2e63 6f6e 6e65 6374 2873 656c  sted.connect(sel
-00002570: 662e 6564 6974 5f46 3529 0a20 2020 2020  f.edit_F5).     
-00002580: 2020 2073 656c 662e 4635 2e63 6c69 636b     self.F5.click
-00002590: 6564 2e63 6f6e 6e65 6374 2873 656c 662e  ed.connect(self.
-000025a0: 7365 6e64 6635 290a 2020 2020 2020 2020  sendf5).        
-000025b0: 7365 6c66 2e46 362e 7365 7443 6f6e 7465  self.F6.setConte
-000025c0: 7874 4d65 6e75 506f 6c69 6379 2851 7443  xtMenuPolicy(QtC
-000025d0: 6f72 652e 5174 2e43 7573 746f 6d43 6f6e  ore.Qt.CustomCon
-000025e0: 7465 7874 4d65 6e75 290a 2020 2020 2020  textMenu).      
-000025f0: 2020 7365 6c66 2e46 362e 6375 7374 6f6d    self.F6.custom
-00002600: 436f 6e74 6578 744d 656e 7552 6571 7565  ContextMenuReque
-00002610: 7374 6564 2e63 6f6e 6e65 6374 2873 656c  sted.connect(sel
-00002620: 662e 6564 6974 5f46 3629 0a20 2020 2020  f.edit_F6).     
-00002630: 2020 2073 656c 662e 4636 2e63 6c69 636b     self.F6.click
-00002640: 6564 2e63 6f6e 6e65 6374 2873 656c 662e  ed.connect(self.
-00002650: 7365 6e64 6636 290a 2020 2020 2020 2020  sendf6).        
-00002660: 7365 6c66 2e46 372e 7365 7443 6f6e 7465  self.F7.setConte
-00002670: 7874 4d65 6e75 506f 6c69 6379 2851 7443  xtMenuPolicy(QtC
-00002680: 6f72 652e 5174 2e43 7573 746f 6d43 6f6e  ore.Qt.CustomCon
-00002690: 7465 7874 4d65 6e75 290a 2020 2020 2020  textMenu).      
-000026a0: 2020 7365 6c66 2e46 372e 6375 7374 6f6d    self.F7.custom
-000026b0: 436f 6e74 6578 744d 656e 7552 6571 7565  ContextMenuReque
-000026c0: 7374 6564 2e63 6f6e 6e65 6374 2873 656c  sted.connect(sel
-000026d0: 662e 6564 6974 5f46 3729 0a20 2020 2020  f.edit_F7).     
-000026e0: 2020 2073 656c 662e 4637 2e63 6c69 636b     self.F7.click
-000026f0: 6564 2e63 6f6e 6e65 6374 2873 656c 662e  ed.connect(self.
-00002700: 7365 6e64 6637 290a 2020 2020 2020 2020  sendf7).        
-00002710: 7365 6c66 2e46 382e 7365 7443 6f6e 7465  self.F8.setConte
-00002720: 7874 4d65 6e75 506f 6c69 6379 2851 7443  xtMenuPolicy(QtC
-00002730: 6f72 652e 5174 2e43 7573 746f 6d43 6f6e  ore.Qt.CustomCon
-00002740: 7465 7874 4d65 6e75 290a 2020 2020 2020  textMenu).      
-00002750: 2020 7365 6c66 2e46 382e 6375 7374 6f6d    self.F8.custom
-00002760: 436f 6e74 6578 744d 656e 7552 6571 7565  ContextMenuReque
-00002770: 7374 6564 2e63 6f6e 6e65 6374 2873 656c  sted.connect(sel
-00002780: 662e 6564 6974 5f46 3829 0a20 2020 2020  f.edit_F8).     
-00002790: 2020 2073 656c 662e 4638 2e63 6c69 636b     self.F8.click
-000027a0: 6564 2e63 6f6e 6e65 6374 2873 656c 662e  ed.connect(self.
-000027b0: 7365 6e64 6638 290a 2020 2020 2020 2020  sendf8).        
-000027c0: 7365 6c66 2e46 392e 7365 7443 6f6e 7465  self.F9.setConte
-000027d0: 7874 4d65 6e75 506f 6c69 6379 2851 7443  xtMenuPolicy(QtC
-000027e0: 6f72 652e 5174 2e43 7573 746f 6d43 6f6e  ore.Qt.CustomCon
-000027f0: 7465 7874 4d65 6e75 290a 2020 2020 2020  textMenu).      
-00002800: 2020 7365 6c66 2e46 392e 6375 7374 6f6d    self.F9.custom
-00002810: 436f 6e74 6578 744d 656e 7552 6571 7565  ContextMenuReque
-00002820: 7374 6564 2e63 6f6e 6e65 6374 2873 656c  sted.connect(sel
-00002830: 662e 6564 6974 5f46 3929 0a20 2020 2020  f.edit_F9).     
-00002840: 2020 2073 656c 662e 4639 2e63 6c69 636b     self.F9.click
-00002850: 6564 2e63 6f6e 6e65 6374 2873 656c 662e  ed.connect(self.
-00002860: 7365 6e64 6639 290a 2020 2020 2020 2020  sendf9).        
-00002870: 7365 6c66 2e46 3130 2e73 6574 436f 6e74  self.F10.setCont
-00002880: 6578 744d 656e 7550 6f6c 6963 7928 5174  extMenuPolicy(Qt
-00002890: 436f 7265 2e51 742e 4375 7374 6f6d 436f  Core.Qt.CustomCo
-000028a0: 6e74 6578 744d 656e 7529 0a20 2020 2020  ntextMenu).     
-000028b0: 2020 2073 656c 662e 4631 302e 6375 7374     self.F10.cust
-000028c0: 6f6d 436f 6e74 6578 744d 656e 7552 6571  omContextMenuReq
-000028d0: 7565 7374 6564 2e63 6f6e 6e65 6374 2873  uested.connect(s
-000028e0: 656c 662e 6564 6974 5f46 3130 290a 2020  elf.edit_F10).  
-000028f0: 2020 2020 2020 7365 6c66 2e46 3130 2e63        self.F10.c
-00002900: 6c69 636b 6564 2e63 6f6e 6e65 6374 2873  licked.connect(s
-00002910: 656c 662e 7365 6e64 6631 3029 0a20 2020  elf.sendf10).   
-00002920: 2020 2020 2073 656c 662e 4631 312e 7365       self.F11.se
-00002930: 7443 6f6e 7465 7874 4d65 6e75 506f 6c69  tContextMenuPoli
-00002940: 6379 2851 7443 6f72 652e 5174 2e43 7573  cy(QtCore.Qt.Cus
-00002950: 746f 6d43 6f6e 7465 7874 4d65 6e75 290a  tomContextMenu).
-00002960: 2020 2020 2020 2020 7365 6c66 2e46 3131          self.F11
-00002970: 2e63 7573 746f 6d43 6f6e 7465 7874 4d65  .customContextMe
-00002980: 6e75 5265 7175 6573 7465 642e 636f 6e6e  nuRequested.conn
-00002990: 6563 7428 7365 6c66 2e65 6469 745f 4631  ect(self.edit_F1
-000029a0: 3129 0a20 2020 2020 2020 2073 656c 662e  1).        self.
-000029b0: 4631 312e 636c 6963 6b65 642e 636f 6e6e  F11.clicked.conn
-000029c0: 6563 7428 7365 6c66 2e73 656e 6466 3131  ect(self.sendf11
-000029d0: 290a 2020 2020 2020 2020 7365 6c66 2e46  ).        self.F
-000029e0: 3132 2e73 6574 436f 6e74 6578 744d 656e  12.setContextMen
-000029f0: 7550 6f6c 6963 7928 5174 436f 7265 2e51  uPolicy(QtCore.Q
-00002a00: 742e 4375 7374 6f6d 436f 6e74 6578 744d  t.CustomContextM
-00002a10: 656e 7529 0a20 2020 2020 2020 2073 656c  enu).        sel
-00002a20: 662e 4631 322e 6375 7374 6f6d 436f 6e74  f.F12.customCont
-00002a30: 6578 744d 656e 7552 6571 7565 7374 6564  extMenuRequested
-00002a40: 2e63 6f6e 6e65 6374 2873 656c 662e 6564  .connect(self.ed
-00002a50: 6974 5f46 3132 290a 2020 2020 2020 2020  it_F12).        
-00002a60: 7365 6c66 2e46 3132 2e63 6c69 636b 6564  self.F12.clicked
-00002a70: 2e63 6f6e 6e65 6374 2873 656c 662e 7365  .connect(self.se
-00002a80: 6e64 6631 3229 0a0a 2020 2020 2020 2020  ndf12)..        
-00002a90: 7365 6c66 2e72 6561 6470 7265 6665 7265  self.readprefere
-00002aa0: 6e63 6573 2829 0a20 2020 2020 2020 2073  nces().        s
-00002ab0: 656c 662e 6462 6e61 6d65 203d 2044 4154  elf.dbname = DAT
-00002ac0: 415f 5041 5448 202b 2022 2f22 202b 2073  A_PATH + "/" + s
-00002ad0: 656c 662e 7072 6566 2e67 6574 2822 6375  elf.pref.get("cu
-00002ae0: 7272 656e 745f 6461 7461 6261 7365 222c  rrent_database",
-00002af0: 2022 6861 6d2e 6462 2229 0a20 2020 2020   "ham.db").     
-00002b00: 2020 2073 656c 662e 6461 7461 6261 7365     self.database
-00002b10: 203d 2044 6174 6142 6173 6528 7365 6c66   = DataBase(self
-00002b20: 2e64 626e 616d 652c 2057 4f52 4b49 4e47  .dbname, WORKING
-00002b30: 5f50 4154 4829 0a20 2020 2020 2020 2073  _PATH).        s
-00002b40: 656c 662e 7374 6174 696f 6e20 3d20 7365  elf.station = se
-00002b50: 6c66 2e64 6174 6162 6173 652e 6665 7463  lf.database.fetc
-00002b60: 685f 7374 6174 696f 6e28 290a 2020 2020  h_station().    
-00002b70: 2020 2020 6966 2073 656c 662e 7374 6174      if self.stat
-00002b80: 696f 6e20 6973 204e 6f6e 653a 0a20 2020  ion is None:.   
-00002b90: 2020 2020 2020 2020 2073 656c 662e 7374           self.st
-00002ba0: 6174 696f 6e20 3d20 7b7d 0a20 2020 2020  ation = {}.     
-00002bb0: 2020 2020 2020 2073 656c 662e 6564 6974         self.edit
-00002bc0: 5f73 7461 7469 6f6e 5f73 6574 7469 6e67  _station_setting
-00002bd0: 7328 290a 2020 2020 2020 2020 2020 2020  s().            
-00002be0: 7365 6c66 2e73 7461 7469 6f6e 203d 2073  self.station = s
-00002bf0: 656c 662e 6461 7461 6261 7365 2e66 6574  elf.database.fet
-00002c00: 6368 5f73 7461 7469 6f6e 2829 0a20 2020  ch_station().   
-00002c10: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
-00002c20: 2e73 7461 7469 6f6e 2069 7320 4e6f 6e65  .station is None
-00002c30: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00002c40: 2020 7365 6c66 2e73 7461 7469 6f6e 203d    self.station =
-00002c50: 207b 7d0a 2020 2020 2020 2020 7365 6c66   {}.        self
-00002c60: 2e63 6f6e 7461 6374 203d 2073 656c 662e  .contact = self.
-00002c70: 6461 7461 6261 7365 2e65 6d70 7479 5f63  database.empty_c
-00002c80: 6f6e 7461 6374 0a20 2020 2020 2020 2073  ontact.        s
-00002c90: 656c 662e 6375 7272 656e 745f 6f70 203d  elf.current_op =
-00002ca0: 2073 656c 662e 7374 6174 696f 6e2e 6765   self.station.ge
-00002cb0: 7428 2243 616c 6c22 2c20 2222 290a 2020  t("Call", "").  
-00002cc0: 2020 2020 2020 7365 6c66 2e6d 616b 655f        self.make_
-00002cd0: 6f70 5f64 6972 2829 0a20 2020 2020 2020  op_dir().       
-00002ce0: 2073 656c 662e 7265 6164 5f63 775f 6d61   self.read_cw_ma
-00002cf0: 6372 6f73 2829 0a20 2020 2020 2020 2073  cros().        s
-00002d00: 656c 662e 636c 6561 7269 6e70 7574 7328  elf.clearinputs(
-00002d10: 290a 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00002d20: 6261 6e64 5f69 6e64 6963 6174 6f72 735f  band_indicators_
-00002d30: 6377 203d 207b 0a20 2020 2020 2020 2020  cw = {.         
-00002d40: 2020 2022 3136 3022 3a20 7365 6c66 2e63     "160": self.c
-00002d50: 775f 6261 6e64 5f31 3630 2c0a 2020 2020  w_band_160,.    
-00002d60: 2020 2020 2020 2020 2238 3022 3a20 7365          "80": se
-00002d70: 6c66 2e63 775f 6261 6e64 5f38 302c 0a20  lf.cw_band_80,. 
-00002d80: 2020 2020 2020 2020 2020 2022 3430 223a             "40":
-00002d90: 2073 656c 662e 6377 5f62 616e 645f 3430   self.cw_band_40
-00002da0: 2c0a 2020 2020 2020 2020 2020 2020 2232  ,.            "2
-00002db0: 3022 3a20 7365 6c66 2e63 775f 6261 6e64  0": self.cw_band
-00002dc0: 5f32 302c 0a20 2020 2020 2020 2020 2020  _20,.           
-00002dd0: 2022 3135 223a 2073 656c 662e 6377 5f62   "15": self.cw_b
-00002de0: 616e 645f 3135 2c0a 2020 2020 2020 2020  and_15,.        
-00002df0: 2020 2020 2231 3022 3a20 7365 6c66 2e63      "10": self.c
-00002e00: 775f 6261 6e64 5f31 302c 0a20 2020 2020  w_band_10,.     
-00002e10: 2020 207d 0a0a 2020 2020 2020 2020 7365     }..        se
-00002e20: 6c66 2e62 616e 645f 696e 6469 6361 746f  lf.band_indicato
-00002e30: 7273 5f73 7362 203d 207b 0a20 2020 2020  rs_ssb = {.     
-00002e40: 2020 2020 2020 2022 3136 3022 3a20 7365         "160": se
-00002e50: 6c66 2e73 7362 5f62 616e 645f 3136 302c  lf.ssb_band_160,
-00002e60: 0a20 2020 2020 2020 2020 2020 2022 3830  .            "80
-00002e70: 223a 2073 656c 662e 7373 625f 6261 6e64  ": self.ssb_band
-00002e80: 5f38 302c 0a20 2020 2020 2020 2020 2020  _80,.           
-00002e90: 2022 3430 223a 2073 656c 662e 7373 625f   "40": self.ssb_
-00002ea0: 6261 6e64 5f34 302c 0a20 2020 2020 2020  band_40,.       
-00002eb0: 2020 2020 2022 3230 223a 2073 656c 662e       "20": self.
-00002ec0: 7373 625f 6261 6e64 5f32 302c 0a20 2020  ssb_band_20,.   
-00002ed0: 2020 2020 2020 2020 2022 3135 223a 2073           "15": s
-00002ee0: 656c 662e 7373 625f 6261 6e64 5f31 352c  elf.ssb_band_15,
-00002ef0: 0a20 2020 2020 2020 2020 2020 2022 3130  .            "10
-00002f00: 223a 2073 656c 662e 7373 625f 6261 6e64  ": self.ssb_band
-00002f10: 5f31 302c 0a20 2020 2020 2020 207d 0a0a  _10,.        }..
-00002f20: 2020 2020 2020 2020 7365 6c66 2e62 616e          self.ban
-00002f30: 645f 696e 6469 6361 746f 7273 5f72 7474  d_indicators_rtt
-00002f40: 7920 3d20 7b0a 2020 2020 2020 2020 2020  y = {.          
-00002f50: 2020 2231 3630 223a 2073 656c 662e 7274    "160": self.rt
-00002f60: 7479 5f62 616e 645f 3136 302c 0a20 2020  ty_band_160,.   
-00002f70: 2020 2020 2020 2020 2022 3830 223a 2073           "80": s
-00002f80: 656c 662e 7274 7479 5f62 616e 645f 3830  elf.rtty_band_80
-00002f90: 2c0a 2020 2020 2020 2020 2020 2020 2234  ,.            "4
-00002fa0: 3022 3a20 7365 6c66 2e72 7474 795f 6261  0": self.rtty_ba
-00002fb0: 6e64 5f34 302c 0a20 2020 2020 2020 2020  nd_40,.         
-00002fc0: 2020 2022 3230 223a 2073 656c 662e 7274     "20": self.rt
-00002fd0: 7479 5f62 616e 645f 3230 2c0a 2020 2020  ty_band_20,.    
-00002fe0: 2020 2020 2020 2020 2231 3522 3a20 7365          "15": se
-00002ff0: 6c66 2e72 7474 795f 6261 6e64 5f31 352c  lf.rtty_band_15,
-00003000: 0a20 2020 2020 2020 2020 2020 2022 3130  .            "10
-00003010: 223a 2073 656c 662e 7274 7479 5f62 616e  ": self.rtty_ban
-00003020: 645f 3130 2c0a 2020 2020 2020 2020 7d0a  d_10,.        }.
-00003030: 0a20 2020 2020 2020 2073 656c 662e 616c  .        self.al
-00003040: 6c5f 6d6f 6465 5f69 6e64 6963 6174 6f72  l_mode_indicator
-00003050: 7320 3d20 7b0a 2020 2020 2020 2020 2020  s = {.          
-00003060: 2020 2243 5722 3a20 7365 6c66 2e62 616e    "CW": self.ban
-00003070: 645f 696e 6469 6361 746f 7273 5f63 772c  d_indicators_cw,
-00003080: 0a20 2020 2020 2020 2020 2020 2022 5353  .            "SS
-00003090: 4222 3a20 7365 6c66 2e62 616e 645f 696e  B": self.band_in
-000030a0: 6469 6361 746f 7273 5f73 7362 2c0a 2020  dicators_ssb,.  
-000030b0: 2020 2020 2020 2020 2020 2252 5454 5922            "RTTY"
-000030c0: 3a20 7365 6c66 2e62 616e 645f 696e 6469  : self.band_indi
-000030d0: 6361 746f 7273 5f72 7474 792c 0a20 2020  cators_rtty,.   
-000030e0: 2020 2020 207d 0a0a 2020 2020 2020 2020       }..        
-000030f0: 6966 2073 656c 662e 7072 6566 2e67 6574  if self.pref.get
-00003100: 2822 636f 6e74 6573 7422 293a 0a20 2020  ("contest"):.   
-00003110: 2020 2020 2020 2020 2073 656c 662e 6c6f           self.lo
-00003120: 6164 5f63 6f6e 7465 7374 2829 0a0a 2020  ad_contest()..  
-00003130: 2020 2020 2020 6966 2056 6572 7369 6f6e        if Version
-00003140: 5465 7374 285f 5f76 6572 7369 6f6e 5f5f  Test(__version__
-00003150: 292e 7465 7374 2829 3a0a 2020 2020 2020  ).test():.      
-00003160: 2020 2020 2020 7365 6c66 2e73 686f 775f        self.show_
-00003170: 6d65 7373 6167 655f 626f 7828 0a20 2020  message_box(.   
-00003180: 2020 2020 2020 2020 2020 2020 2022 5468               "Th
-00003190: 6572 6520 6973 2061 206e 6577 6572 2076  ere is a newer v
-000031a0: 6572 7369 6f6e 206f 6620 6e6f 7431 6d6d  ersion of not1mm
-000031b0: 2061 7661 696c 6162 6c65 2e5c 6e22 0a20   available.\n". 
-000031c0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-000031d0: 596f 7520 6361 6e20 7564 6174 6520 746f  You can udate to
-000031e0: 2074 6865 2063 7572 7265 6e74 2076 6572   the current ver
-000031f0: 7369 6f6e 2062 7920 7573 696e 673a 5c6e  sion by using:\n
-00003200: 7069 7020 696e 7374 616c 6c20 2d55 206e  pip install -U n
-00003210: 6f74 316d 6d22 0a20 2020 2020 2020 2020  ot1mm".         
-00003220: 2020 2029 0a0a 2020 2020 6465 6620 7175     )..    def qu
-00003230: 6974 5f61 7070 2873 656c 6629 3a0a 2020  it_app(self):.  
-00003240: 2020 2020 2020 2222 2264 6f63 2222 220a        """doc""".
-00003250: 2020 2020 2020 2020 6170 702e 7175 6974          app.quit
-00003260: 2829 0a0a 2020 2020 4073 7461 7469 636d  ()..    @staticm
-00003270: 6574 686f 640a 2020 2020 6465 6620 6368  ethod.    def ch
-00003280: 6563 6b5f 7072 6f63 6573 7328 6e61 6d65  eck_process(name
-00003290: 3a20 7374 7229 202d 3e20 626f 6f6c 3a0a  : str) -> bool:.
-000032a0: 2020 2020 2020 2020 2222 2263 6865 636b          """check
-000032b0: 7320 746f 2073 6565 2069 6620 7072 6f67  s to see if prog
-000032c0: 7261 6d20 6f66 206e 616d 6520 6973 2069  ram of name is i
-000032d0: 6e20 7468 6520 6163 7469 7665 2070 726f  n the active pro
-000032e0: 6365 7373 206c 6973 7422 2222 0a20 2020  cess list""".   
-000032f0: 2020 2020 2066 6f72 2070 726f 6320 696e       for proc in
-00003300: 2070 7375 7469 6c2e 7072 6f63 6573 735f   psutil.process_
-00003310: 6974 6572 2829 3a0a 2020 2020 2020 2020  iter():.        
-00003320: 2020 2020 6966 2062 6f6f 6c28 7265 2e6d      if bool(re.m
-00003330: 6174 6368 286e 616d 652c 2070 726f 632e  atch(name, proc.
-00003340: 6e61 6d65 2829 2e6c 6f77 6572 2829 2929  name().lower()))
-00003350: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00003360: 2020 7265 7475 726e 2054 7275 650a 2020    return True.  
-00003370: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
-00003380: 7365 0a0a 2020 2020 6465 6620 7368 6f77  se..    def show
-00003390: 5f6d 6573 7361 6765 5f62 6f78 2873 656c  _message_box(sel
-000033a0: 662c 206d 6573 7361 6765 3a20 7374 7229  f, message: str)
-000033b0: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
-000033c0: 2020 2222 2264 6f63 2222 220a 2020 2020    """doc""".    
-000033d0: 2020 2020 6d65 7373 6167 655f 626f 7820      message_box 
-000033e0: 3d20 5174 5769 6467 6574 732e 514d 6573  = QtWidgets.QMes
-000033f0: 7361 6765 426f 7828 290a 2020 2020 2020  sageBox().      
-00003400: 2020 6d65 7373 6167 655f 626f 782e 7365    message_box.se
-00003410: 7449 636f 6e28 5174 5769 6467 6574 732e  tIcon(QtWidgets.
-00003420: 514d 6573 7361 6765 426f 782e 496e 666f  QMessageBox.Info
-00003430: 726d 6174 696f 6e29 0a20 2020 2020 2020  rmation).       
-00003440: 206d 6573 7361 6765 5f62 6f78 2e73 6574   message_box.set
-00003450: 5465 7874 286d 6573 7361 6765 290a 2020  Text(message).  
-00003460: 2020 2020 2020 6d65 7373 6167 655f 626f        message_bo
-00003470: 782e 7365 7457 696e 646f 7754 6974 6c65  x.setWindowTitle
-00003480: 2822 496e 666f 726d 6174 696f 6e22 290a  ("Information").
-00003490: 2020 2020 2020 2020 6d65 7373 6167 655f          message_
-000034a0: 626f 782e 7365 7453 7461 6e64 6172 6442  box.setStandardB
-000034b0: 7574 746f 6e73 2851 7457 6964 6765 7473  uttons(QtWidgets
-000034c0: 2e51 4d65 7373 6167 6542 6f78 2e4f 6b29  .QMessageBox.Ok)
-000034d0: 0a20 2020 2020 2020 205f 203d 206d 6573  .        _ = mes
-000034e0: 7361 6765 5f62 6f78 2e65 7865 635f 2829  sage_box.exec_()
-000034f0: 0a0a 2020 2020 6465 6620 7368 6f77 5f61  ..    def show_a
-00003500: 626f 7574 5f64 6961 6c6f 6728 7365 6c66  bout_dialog(self
-00003510: 293a 0a20 2020 2020 2020 2022 2222 5368  ):.        """Sh
-00003520: 6f77 2061 626f 7574 2064 6961 6c6f 6722  ow about dialog"
-00003530: 2222 0a20 2020 2020 2020 2073 656c 662e  "".        self.
-00003540: 6162 6f75 745f 6469 616c 6f67 203d 2041  about_dialog = A
-00003550: 626f 7574 2857 4f52 4b49 4e47 5f50 4154  bout(WORKING_PAT
-00003560: 4829 0a20 2020 2020 2020 2073 656c 662e  H).        self.
-00003570: 6162 6f75 745f 6469 616c 6f67 2e64 6f6e  about_dialog.don
-00003580: 6f72 732e 7365 7453 6f75 7263 6528 0a20  ors.setSource(. 
-00003590: 2020 2020 2020 2020 2020 2051 7443 6f72             QtCor
-000035a0: 652e 5155 726c 2e66 726f 6d4c 6f63 616c  e.QUrl.fromLocal
-000035b0: 4669 6c65 2857 4f52 4b49 4e47 5f50 4154  File(WORKING_PAT
-000035c0: 4820 2b20 222f 6461 7461 2f64 6f6e 6f72  H + "/data/donor
-000035d0: 732e 6874 6d6c 2229 0a20 2020 2020 2020  s.html").       
-000035e0: 2029 0a20 2020 2020 2020 2073 656c 662e   ).        self.
-000035f0: 6162 6f75 745f 6469 616c 6f67 2e6f 7065  about_dialog.ope
-00003600: 6e28 290a 0a20 2020 2064 6566 2073 686f  n()..    def sho
-00003610: 775f 6865 6c70 5f64 6961 6c6f 6728 7365  w_help_dialog(se
-00003620: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
-00003630: 5368 6f77 2061 626f 7574 2064 6961 6c6f  Show about dialo
-00003640: 6722 2222 0a20 2020 2020 2020 2073 656c  g""".        sel
-00003650: 662e 6162 6f75 745f 6469 616c 6f67 203d  f.about_dialog =
-00003660: 2041 626f 7574 2857 4f52 4b49 4e47 5f50   About(WORKING_P
-00003670: 4154 4829 0a20 2020 2020 2020 2073 656c  ATH).        sel
-00003680: 662e 6162 6f75 745f 6469 616c 6f67 2e73  f.about_dialog.s
-00003690: 6574 5769 6e64 6f77 5469 746c 6528 2248  etWindowTitle("H
-000036a0: 656c 7022 290a 2020 2020 2020 2020 7365  elp").        se
-000036b0: 6c66 2e61 626f 7574 5f64 6961 6c6f 672e  lf.about_dialog.
-000036c0: 7365 7447 656f 6d65 7472 7928 302c 2030  setGeometry(0, 0
-000036d0: 2c20 3830 302c 2036 3030 290a 2020 2020  , 800, 600).    
-000036e0: 2020 2020 7365 6c66 2e61 626f 7574 5f64      self.about_d
-000036f0: 6961 6c6f 672e 646f 6e6f 7273 2e73 6574  ialog.donors.set
-00003700: 536f 7572 6365 280a 2020 2020 2020 2020  Source(.        
-00003710: 2020 2020 5174 436f 7265 2e51 5572 6c2e      QtCore.QUrl.
-00003720: 6672 6f6d 4c6f 6361 6c46 696c 6528 574f  fromLocalFile(WO
-00003730: 524b 494e 475f 5041 5448 202b 2022 2f64  RKING_PATH + "/d
-00003740: 6174 612f 6e6f 7431 6d6d 2e68 746d 6c22  ata/not1mm.html"
-00003750: 290a 2020 2020 2020 2020 290a 2020 2020  ).        ).    
-00003760: 2020 2020 7365 6c66 2e61 626f 7574 5f64      self.about_d
-00003770: 6961 6c6f 672e 6f70 656e 2829 0a0a 2020  ialog.open()..  
-00003780: 2020 6465 6620 7570 6461 7465 5f6d 6173    def update_mas
-00003790: 7465 7273 6370 2873 656c 6629 202d 3e20  terscp(self) -> 
-000037a0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
-000037b0: 2255 7064 6174 6520 7468 6520 4d41 5354  "Update the MAST
-000037c0: 4552 2e53 4350 2066 696c 652e 0a20 2020  ER.SCP file..   
-000037d0: 2020 2020 202d 2052 6574 7572 6e73 2054       - Returns T
-000037e0: 7275 6520 6966 2073 7563 6365 7373 6675  rue if successfu
-000037f0: 6c0a 2020 2020 2020 2020 2d20 4f74 6865  l.        - Othe
-00003800: 7277 6973 6520 4661 6c73 650a 2020 2020  rwise False.    
-00003810: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00003820: 7769 7468 2072 6571 7565 7374 732e 5365  with requests.Se
-00003830: 7373 696f 6e28 2920 6173 2073 6573 7369  ssion() as sessi
-00003840: 6f6e 3a0a 2020 2020 2020 2020 2020 2020  on:.            
-00003850: 7468 655f 7265 7175 6573 7420 3d20 7365  the_request = se
-00003860: 7373 696f 6e2e 6765 7428 4d41 5354 4552  ssion.get(MASTER
-00003870: 5f53 4350 5f55 524c 290a 2020 2020 2020  _SCP_URL).      
-00003880: 2020 2020 2020 6966 2074 6865 5f72 6571        if the_req
-00003890: 7565 7374 2e73 7461 7475 735f 636f 6465  uest.status_code
-000038a0: 203d 3d20 3230 303a 0a20 2020 2020 2020   == 200:.       
-000038b0: 2020 2020 2020 2020 2077 6974 6820 6f70           with op
-000038c0: 656e 2857 4f52 4b49 4e47 5f50 4154 4820  en(WORKING_PATH 
-000038d0: 2b20 222f 6461 7461 2f4d 4153 5445 522e  + "/data/MASTER.
-000038e0: 5343 5022 2c20 2277 622b 2229 2061 7320  SCP", "wb+") as 
-000038f0: 6669 6c65 3a0a 2020 2020 2020 2020 2020  file:.          
-00003900: 2020 2020 2020 2020 2020 6669 6c65 2e77            file.w
-00003910: 7269 7465 2874 6865 5f72 6571 7565 7374  rite(the_request
-00003920: 2e63 6f6e 7465 6e74 290a 2020 2020 2020  .content).      
-00003930: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
-00003940: 686f 775f 6d65 7373 6167 655f 626f 7828  how_message_box(
-00003950: 224d 4153 5445 522e 5343 5020 6669 6c65  "MASTER.SCP file
-00003960: 2075 7064 6174 6564 2e22 290a 2020 2020   updated.").    
-00003970: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00003980: 726e 0a20 2020 2020 2020 2073 656c 662e  rn.        self.
-00003990: 7368 6f77 5f6d 6573 7361 6765 5f62 6f78  show_message_box
-000039a0: 2822 4d41 5354 4552 2e53 4350 2063 6f75  ("MASTER.SCP cou
-000039b0: 6c64 206e 6f74 2062 6520 7570 6461 7465  ld not be update
-000039c0: 642e 2229 0a0a 2020 2020 6465 6620 6564  d.")..    def ed
-000039d0: 6974 5f63 6f6e 6669 6775 7261 7469 6f6e  it_configuration
-000039e0: 5f73 6574 7469 6e67 7328 7365 6c66 293a  _settings(self):
-000039f0: 0a20 2020 2020 2020 2022 2222 436f 6e66  .        """Conf
-00003a00: 6967 7572 6174 696f 6e20 5365 7474 696e  iguration Settin
-00003a10: 6773 2077 6173 2063 6c69 636b 6564 2222  gs was clicked""
-00003a20: 220a 2020 2020 2020 2020 7365 6c66 2e63  ".        self.c
-00003a30: 6f6e 6669 6775 7261 7469 6f6e 5f64 6961  onfiguration_dia
-00003a40: 6c6f 6720 3d20 5365 7474 696e 6773 2857  log = Settings(W
-00003a50: 4f52 4b49 4e47 5f50 4154 482c 2043 4f4e  ORKING_PATH, CON
-00003a60: 4649 475f 5041 5448 2c20 7365 6c66 2e70  FIG_PATH, self.p
-00003a70: 7265 6629 0a20 2020 2020 2020 2073 656c  ref).        sel
-00003a80: 662e 636f 6e66 6967 7572 6174 696f 6e5f  f.configuration_
-00003a90: 6469 616c 6f67 2e75 7365 6861 6d64 625f  dialog.usehamdb_
-00003aa0: 7261 6469 6f42 7574 746f 6e2e 6869 6465  radioButton.hide
-00003ab0: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
-00003ac0: 636f 6e66 6967 7572 6174 696f 6e5f 6469  configuration_di
-00003ad0: 616c 6f67 2e73 686f 7728 290a 2020 2020  alog.show().    
-00003ae0: 2020 2020 7365 6c66 2e63 6f6e 6669 6775      self.configu
-00003af0: 7261 7469 6f6e 5f64 6961 6c6f 672e 6163  ration_dialog.ac
-00003b00: 6365 7074 6564 2e63 6f6e 6e65 6374 2873  cepted.connect(s
-00003b10: 656c 662e 6564 6974 5f63 6f6e 6669 6775  elf.edit_configu
-00003b20: 7261 7469 6f6e 5f72 6574 7572 6e29 0a0a  ration_return)..
-00003b30: 2020 2020 6465 6620 6564 6974 5f63 6f6e      def edit_con
-00003b40: 6669 6775 7261 7469 6f6e 5f72 6574 7572  figuration_retur
-00003b50: 6e28 7365 6c66 293a 0a20 2020 2020 2020  n(self):.       
-00003b60: 2022 2222 5265 7475 726e 7320 6865 7265   """Returns here
-00003b70: 2077 6865 6e20 636f 6e66 6967 7572 6174   when configurat
-00003b80: 696f 6e20 6469 616c 6f67 2063 6c6f 7365  ion dialog close
-00003b90: 6420 7769 7468 206f 6b61 792e 2222 220a  d with okay.""".
-00003ba0: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
-00003bb0: 6669 6775 7261 7469 6f6e 5f64 6961 6c6f  figuration_dialo
-00003bc0: 672e 7361 7665 5f63 6861 6e67 6573 2829  g.save_changes()
-00003bd0: 0a20 2020 2020 2020 2073 656c 662e 7772  .        self.wr
-00003be0: 6974 655f 7072 6566 6572 656e 6365 2829  ite_preference()
-00003bf0: 0a20 2020 2020 2020 206c 6f67 6765 722e  .        logger.
-00003c00: 6465 6275 6728 2225 7322 2c20 6622 7b73  debug("%s", f"{s
-00003c10: 656c 662e 7072 6566 7d22 290a 2020 2020  elf.pref}").    
-00003c20: 2020 2020 7365 6c66 2e72 6561 6470 7265      self.readpre
-00003c30: 6665 7265 6e63 6573 2829 0a0a 2020 2020  ferences()..    
-00003c40: 6465 6620 6e65 775f 6461 7461 6261 7365  def new_database
-00003c50: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00003c60: 2222 2243 7265 6174 6520 6e65 7720 6461  """Create new da
-00003c70: 7461 6261 7365 2e22 2222 0a20 2020 2020  tabase.""".     
-00003c80: 2020 2066 696c 656e 616d 6520 3d20 7365     filename = se
-00003c90: 6c66 2e66 696c 6570 6963 6b65 7228 226e  lf.filepicker("n
-00003ca0: 6577 2229 0a20 2020 2020 2020 2069 6620  ew").        if 
-00003cb0: 6669 6c65 6e61 6d65 3a0a 2020 2020 2020  filename:.      
-00003cc0: 2020 2020 2020 6966 2066 696c 656e 616d        if filenam
-00003cd0: 655b 2d33 3a5d 2021 3d20 222e 6462 223a  e[-3:] != ".db":
-00003ce0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003cf0: 2066 696c 656e 616d 6520 2b3d 2022 2e64   filename += ".d
-00003d00: 6222 0a20 2020 2020 2020 2020 2020 2073  b".            s
-00003d10: 656c 662e 7072 6566 5b22 6375 7272 656e  elf.pref["curren
-00003d20: 745f 6461 7461 6261 7365 225d 203d 2066  t_database"] = f
-00003d30: 696c 656e 616d 652e 7370 6c69 7428 222f  ilename.split("/
-00003d40: 2229 5b2d 313a 5d5b 305d 0a20 2020 2020  ")[-1:][0].     
-00003d50: 2020 2020 2020 2073 656c 662e 7772 6974         self.writ
-00003d60: 655f 7072 6566 6572 656e 6365 2829 0a20  e_preference(). 
-00003d70: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00003d80: 6462 6e61 6d65 203d 2044 4154 415f 5041  dbname = DATA_PA
-00003d90: 5448 202b 2022 2f22 202b 2073 656c 662e  TH + "/" + self.
-00003da0: 7072 6566 2e67 6574 2822 6375 7272 656e  pref.get("curren
-00003db0: 745f 6461 7461 6261 7365 222c 2022 6861  t_database", "ha
-00003dc0: 6d2e 6462 2229 0a20 2020 2020 2020 2020  m.db").         
-00003dd0: 2020 2073 656c 662e 6461 7461 6261 7365     self.database
-00003de0: 203d 2044 6174 6142 6173 6528 7365 6c66   = DataBase(self
-00003df0: 2e64 626e 616d 652c 2057 4f52 4b49 4e47  .dbname, WORKING
-00003e00: 5f50 4154 4829 0a20 2020 2020 2020 2020  _PATH).         
-00003e10: 2020 2073 656c 662e 636f 6e74 6163 7420     self.contact 
-00003e20: 3d20 7365 6c66 2e64 6174 6162 6173 652e  = self.database.
-00003e30: 656d 7074 795f 636f 6e74 6163 740a 2020  empty_contact.  
-00003e40: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
-00003e50: 7461 7469 6f6e 203d 2073 656c 662e 6461  tation = self.da
-00003e60: 7461 6261 7365 2e66 6574 6368 5f73 7461  tabase.fetch_sta
-00003e70: 7469 6f6e 2829 0a20 2020 2020 2020 2020  tion().         
-00003e80: 2020 2069 6620 7365 6c66 2e73 7461 7469     if self.stati
-00003e90: 6f6e 2069 7320 4e6f 6e65 3a0a 2020 2020  on is None:.    
-00003ea0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00003eb0: 2e73 7461 7469 6f6e 203d 207b 7d0a 2020  .station = {}.  
-00003ec0: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-00003ed0: 7572 7265 6e74 5f6f 7020 3d20 7365 6c66  urrent_op = self
-00003ee0: 2e73 7461 7469 6f6e 2e67 6574 2822 4361  .station.get("Ca
-00003ef0: 6c6c 222c 2022 2229 0a20 2020 2020 2020  ll", "").       
-00003f00: 2020 2020 2073 656c 662e 6d61 6b65 5f6f       self.make_o
-00003f10: 705f 6469 7228 290a 2020 2020 2020 2020  p_dir().        
-00003f20: 2020 2020 636d 6420 3d20 7b7d 0a20 2020      cmd = {}.   
-00003f30: 2020 2020 2020 2020 2063 6d64 5b22 636d           cmd["cm
-00003f40: 6422 5d20 3d20 224e 4557 4442 220a 2020  d"] = "NEWDB".  
-00003f50: 2020 2020 2020 2020 2020 636d 645b 2273            cmd["s
-00003f60: 7461 7469 6f6e 225d 203d 2070 6c61 7466  tation"] = platf
-00003f70: 6f72 6d2e 6e6f 6465 2829 0a20 2020 2020  orm.node().     
-00003f80: 2020 2020 2020 2073 656c 662e 6d75 6c74         self.mult
-00003f90: 6963 6173 745f 696e 7465 7266 6163 652e  icast_interface.
-00003fa0: 7365 6e64 5f61 735f 6a73 6f6e 2863 6d64  send_as_json(cmd
-00003fb0: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-00003fc0: 6c66 2e63 6c65 6172 696e 7075 7473 2829  lf.clearinputs()
-00003fd0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00003fe0: 662e 6564 6974 5f73 7461 7469 6f6e 5f73  f.edit_station_s
-00003ff0: 6574 7469 6e67 7328 290a 0a20 2020 2064  ettings()..    d
-00004000: 6566 206f 7065 6e5f 6461 7461 6261 7365  ef open_database
-00004010: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00004020: 2222 224f 7065 6e20 6578 6973 7469 6e67  """Open existing
-00004030: 2064 6174 6162 6173 652e 2222 220a 2020   database.""".  
-00004040: 2020 2020 2020 6669 6c65 6e61 6d65 203d        filename =
-00004050: 2073 656c 662e 6669 6c65 7069 636b 6572   self.filepicker
-00004060: 2822 6f70 656e 2229 0a20 2020 2020 2020  ("open").       
-00004070: 2069 6620 6669 6c65 6e61 6d65 3a0a 2020   if filename:.  
-00004080: 2020 2020 2020 2020 2020 7365 6c66 2e70            self.p
-00004090: 7265 665b 2263 7572 7265 6e74 5f64 6174  ref["current_dat
-000040a0: 6162 6173 6522 5d20 3d20 6669 6c65 6e61  abase"] = filena
-000040b0: 6d65 2e73 706c 6974 2822 2f22 295b 2d31  me.split("/")[-1
-000040c0: 3a5d 5b30 5d0a 2020 2020 2020 2020 2020  :][0].          
-000040d0: 2020 7365 6c66 2e77 7269 7465 5f70 7265    self.write_pre
-000040e0: 6665 7265 6e63 6528 290a 2020 2020 2020  ference().      
-000040f0: 2020 2020 2020 7365 6c66 2e64 626e 616d        self.dbnam
-00004100: 6520 3d20 4441 5441 5f50 4154 4820 2b20  e = DATA_PATH + 
-00004110: 222f 2220 2b20 7365 6c66 2e70 7265 662e  "/" + self.pref.
-00004120: 6765 7428 2263 7572 7265 6e74 5f64 6174  get("current_dat
-00004130: 6162 6173 6522 2c20 2268 616d 2e64 6222  abase", "ham.db"
-00004140: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-00004150: 6c66 2e64 6174 6162 6173 6520 3d20 4461  lf.database = Da
-00004160: 7461 4261 7365 2873 656c 662e 6462 6e61  taBase(self.dbna
-00004170: 6d65 2c20 574f 524b 494e 475f 5041 5448  me, WORKING_PATH
-00004180: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-00004190: 6c66 2e63 6f6e 7461 6374 203d 2073 656c  lf.contact = sel
-000041a0: 662e 6461 7461 6261 7365 2e65 6d70 7479  f.database.empty
-000041b0: 5f63 6f6e 7461 6374 0a20 2020 2020 2020  _contact.       
-000041c0: 2020 2020 2073 656c 662e 7374 6174 696f       self.statio
-000041d0: 6e20 3d20 7365 6c66 2e64 6174 6162 6173  n = self.databas
-000041e0: 652e 6665 7463 685f 7374 6174 696f 6e28  e.fetch_station(
-000041f0: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
-00004200: 2073 656c 662e 7374 6174 696f 6e20 6973   self.station is
-00004210: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00004220: 2020 2020 2020 2073 656c 662e 7374 6174         self.stat
-00004230: 696f 6e20 3d20 7b7d 0a20 2020 2020 2020  ion = {}.       
-00004240: 2020 2020 2069 6620 7365 6c66 2e73 7461       if self.sta
-00004250: 7469 6f6e 2e67 6574 2822 4361 6c6c 222c  tion.get("Call",
-00004260: 2022 2229 203d 3d20 2222 3a0a 2020 2020   "") == "":.    
-00004270: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00004280: 2e65 6469 745f 7374 6174 696f 6e5f 7365  .edit_station_se
-00004290: 7474 696e 6773 2829 0a20 2020 2020 2020  ttings().       
-000042a0: 2020 2020 2073 656c 662e 6375 7272 656e       self.curren
-000042b0: 745f 6f70 203d 2073 656c 662e 7374 6174  t_op = self.stat
-000042c0: 696f 6e2e 6765 7428 2243 616c 6c22 2c20  ion.get("Call", 
-000042d0: 2222 290a 2020 2020 2020 2020 2020 2020  "").            
-000042e0: 7365 6c66 2e6d 616b 655f 6f70 5f64 6972  self.make_op_dir
-000042f0: 2829 0a20 2020 2020 2020 2020 2020 2063  ().            c
-00004300: 6d64 203d 207b 7d0a 2020 2020 2020 2020  md = {}.        
-00004310: 2020 2020 636d 645b 2263 6d64 225d 203d      cmd["cmd"] =
-00004320: 2022 4e45 5744 4222 0a20 2020 2020 2020   "NEWDB".       
-00004330: 2020 2020 2063 6d64 5b22 7374 6174 696f       cmd["statio
-00004340: 6e22 5d20 3d20 706c 6174 666f 726d 2e6e  n"] = platform.n
-00004350: 6f64 6528 290a 2020 2020 2020 2020 2020  ode().          
-00004360: 2020 7365 6c66 2e6d 756c 7469 6361 7374    self.multicast
-00004370: 5f69 6e74 6572 6661 6365 2e73 656e 645f  _interface.send_
-00004380: 6173 5f6a 736f 6e28 636d 6429 0a20 2020  as_json(cmd).   
-00004390: 2020 2020 2020 2020 2073 656c 662e 636c           self.cl
-000043a0: 6561 7269 6e70 7574 7328 290a 0a20 2020  earinputs()..   
-000043b0: 2064 6566 206e 6577 5f63 6f6e 7465 7374   def new_contest
-000043c0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-000043d0: 2222 2243 7265 6174 6520 6e65 7720 636f  """Create new co
-000043e0: 6e74 6573 7420 696e 2065 7869 7374 696e  ntest in existin
-000043f0: 6720 6461 7461 6261 7365 2e22 2222 0a0a  g database."""..
-00004400: 2020 2020 6465 6620 6f70 656e 5f63 6f6e      def open_con
-00004410: 7465 7374 2873 656c 6629 3a0a 2020 2020  test(self):.    
-00004420: 2020 2020 2222 2253 7769 7463 6820 746f      """Switch to
-00004430: 2061 2064 6966 6665 7265 6e74 2065 7869   a different exi
-00004440: 7374 696e 6720 636f 6e74 6573 7420 696e  sting contest in
-00004450: 2065 7869 7374 696e 6720 6461 7461 6261   existing databa
-00004460: 7365 2e22 2222 0a20 2020 2020 2020 206c  se.""".        l
-00004470: 6f67 6765 722e 6465 6275 6728 224f 7065  ogger.debug("Ope
-00004480: 6e20 436f 6e74 6573 7420 7365 6c65 6374  n Contest select
-00004490: 6564 2229 0a20 2020 2020 2020 2063 6f6e  ed").        con
-000044a0: 7465 7374 7320 3d20 7365 6c66 2e64 6174  tests = self.dat
-000044b0: 6162 6173 652e 6665 7463 685f 616c 6c5f  abase.fetch_all_
-000044c0: 636f 6e74 6573 7473 2829 0a20 2020 2020  contests().     
-000044d0: 2020 206c 6f67 6765 722e 6465 6275 6728     logger.debug(
-000044e0: 2225 7322 2c20 6622 7b63 6f6e 7465 7374  "%s", f"{contest
-000044f0: 737d 2229 0a0a 2020 2020 2020 2020 6966  s}")..        if
-00004500: 2063 6f6e 7465 7374 733a 0a20 2020 2020   contests:.     
-00004510: 2020 2020 2020 2073 656c 662e 636f 6e74         self.cont
-00004520: 6573 745f 6469 616c 6f67 203d 2053 656c  est_dialog = Sel
-00004530: 6563 7443 6f6e 7465 7374 2857 4f52 4b49  ectContest(WORKI
-00004540: 4e47 5f50 4154 4829 0a20 2020 2020 2020  NG_PATH).       
-00004550: 2020 2020 2073 656c 662e 636f 6e74 6573       self.contes
-00004560: 745f 6469 616c 6f67 2e63 6f6e 7465 7374  t_dialog.contest
-00004570: 5f6c 6973 742e 7365 7452 6f77 436f 756e  _list.setRowCoun
-00004580: 7428 3029 0a20 2020 2020 2020 2020 2020  t(0).           
-00004590: 2073 656c 662e 636f 6e74 6573 745f 6469   self.contest_di
-000045a0: 616c 6f67 2e63 6f6e 7465 7374 5f6c 6973  alog.contest_lis
-000045b0: 742e 7365 7443 6f6c 756d 6e43 6f75 6e74  t.setColumnCount
-000045c0: 2834 290a 2020 2020 2020 2020 2020 2020  (4).            
-000045d0: 7365 6c66 2e63 6f6e 7465 7374 5f64 6961  self.contest_dia
-000045e0: 6c6f 672e 636f 6e74 6573 745f 6c69 7374  log.contest_list
-000045f0: 2e76 6572 7469 6361 6c48 6561 6465 7228  .verticalHeader(
-00004600: 292e 7365 7456 6973 6962 6c65 2846 616c  ).setVisible(Fal
-00004610: 7365 290a 2020 2020 2020 2020 2020 2020  se).            
-00004620: 7365 6c66 2e63 6f6e 7465 7374 5f64 6961  self.contest_dia
-00004630: 6c6f 672e 636f 6e74 6573 745f 6c69 7374  log.contest_list
-00004640: 2e73 6574 436f 6c75 6d6e 5769 6474 6828  .setColumnWidth(
-00004650: 312c 2032 3030 290a 2020 2020 2020 2020  1, 200).        
-00004660: 2020 2020 7365 6c66 2e63 6f6e 7465 7374      self.contest
-00004670: 5f64 6961 6c6f 672e 636f 6e74 6573 745f  _dialog.contest_
-00004680: 6c69 7374 2e73 6574 436f 6c75 6d6e 5769  list.setColumnWi
-00004690: 6474 6828 322c 2032 3030 290a 2020 2020  dth(2, 200).    
-000046a0: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
-000046b0: 7465 7374 5f64 6961 6c6f 672e 636f 6e74  test_dialog.cont
-000046c0: 6573 745f 6c69 7374 2e73 6574 486f 7269  est_list.setHori
-000046d0: 7a6f 6e74 616c 4865 6164 6572 4974 656d  zontalHeaderItem
-000046e0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-000046f0: 2020 302c 2051 7457 6964 6765 7473 2e51    0, QtWidgets.Q
-00004700: 5461 626c 6557 6964 6765 7449 7465 6d28  TableWidgetItem(
-00004710: 2243 6f6e 7465 7374 204e 7222 290a 2020  "Contest Nr").  
-00004720: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-00004730: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
-00004740: 7465 7374 5f64 6961 6c6f 672e 636f 6e74  test_dialog.cont
-00004750: 6573 745f 6c69 7374 2e73 6574 486f 7269  est_list.setHori
-00004760: 7a6f 6e74 616c 4865 6164 6572 4974 656d  zontalHeaderItem
-00004770: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00004780: 2020 312c 2051 7457 6964 6765 7473 2e51    1, QtWidgets.Q
-00004790: 5461 626c 6557 6964 6765 7449 7465 6d28  TableWidgetItem(
-000047a0: 2243 6f6e 7465 7374 204e 616d 6522 290a  "Contest Name").
-000047b0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-000047c0: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-000047d0: 6f6e 7465 7374 5f64 6961 6c6f 672e 636f  ontest_dialog.co
-000047e0: 6e74 6573 745f 6c69 7374 2e73 6574 486f  ntest_list.setHo
-000047f0: 7269 7a6f 6e74 616c 4865 6164 6572 4974  rizontalHeaderIt
-00004800: 656d 280a 2020 2020 2020 2020 2020 2020  em(.            
-00004810: 2020 2020 322c 2051 7457 6964 6765 7473      2, QtWidgets
-00004820: 2e51 5461 626c 6557 6964 6765 7449 7465  .QTableWidgetIte
-00004830: 6d28 2243 6f6e 7465 7374 2053 7461 7274  m("Contest Start
-00004840: 2229 0a20 2020 2020 2020 2020 2020 2029  ").            )
-00004850: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00004860: 662e 636f 6e74 6573 745f 6469 616c 6f67  f.contest_dialog
-00004870: 2e63 6f6e 7465 7374 5f6c 6973 742e 7365  .contest_list.se
-00004880: 7448 6f72 697a 6f6e 7461 6c48 6561 6465  tHorizontalHeade
-00004890: 7249 7465 6d28 0a20 2020 2020 2020 2020  rItem(.         
-000048a0: 2020 2020 2020 2033 2c20 5174 5769 6467         3, QtWidg
-000048b0: 6574 732e 5154 6162 6c65 5769 6467 6574  ets.QTableWidget
-000048c0: 4974 656d 2822 4e6f 7420 5549 7365 6422  Item("Not UIsed"
-000048d0: 290a 2020 2020 2020 2020 2020 2020 290a  ).            ).
-000048e0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000048f0: 2e63 6f6e 7465 7374 5f64 6961 6c6f 672e  .contest_dialog.
-00004900: 636f 6e74 6573 745f 6c69 7374 2e73 6574  contest_list.set
-00004910: 436f 6c75 6d6e 4869 6464 656e 2830 2c20  ColumnHidden(0, 
-00004920: 5472 7565 290a 2020 2020 2020 2020 2020  True).          
-00004930: 2020 7365 6c66 2e63 6f6e 7465 7374 5f64    self.contest_d
-00004940: 6961 6c6f 672e 636f 6e74 6573 745f 6c69  ialog.contest_li
-00004950: 7374 2e73 6574 436f 6c75 6d6e 4869 6464  st.setColumnHidd
-00004960: 656e 2833 2c20 5472 7565 290a 2020 2020  en(3, True).    
-00004970: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
-00004980: 7465 7374 5f64 6961 6c6f 672e 6163 6365  test_dialog.acce
-00004990: 7074 6564 2e63 6f6e 6e65 6374 2873 656c  pted.connect(sel
-000049a0: 662e 6f70 656e 5f63 6f6e 7465 7374 5f72  f.open_contest_r
-000049b0: 6574 7572 6e29 0a20 2020 2020 2020 2020  eturn).         
-000049c0: 2020 2066 6f72 2063 6f6e 7465 7374 2069     for contest i
-000049d0: 6e20 636f 6e74 6573 7473 3a0a 2020 2020  n contests:.    
-000049e0: 2020 2020 2020 2020 2020 2020 6e75 6d62              numb
-000049f0: 6572 5f6f 665f 726f 7773 203d 2073 656c  er_of_rows = sel
-00004a00: 662e 636f 6e74 6573 745f 6469 616c 6f67  f.contest_dialog
-00004a10: 2e63 6f6e 7465 7374 5f6c 6973 742e 726f  .contest_list.ro
-00004a20: 7743 6f75 6e74 2829 0a20 2020 2020 2020  wCount().       
-00004a30: 2020 2020 2020 2020 2073 656c 662e 636f           self.co
-00004a40: 6e74 6573 745f 6469 616c 6f67 2e63 6f6e  ntest_dialog.con
-00004a50: 7465 7374 5f6c 6973 742e 696e 7365 7274  test_list.insert
-00004a60: 526f 7728 6e75 6d62 6572 5f6f 665f 726f  Row(number_of_ro
-00004a70: 7773 290a 2020 2020 2020 2020 2020 2020  ws).            
-00004a80: 2020 2020 636f 6e74 6573 745f 6964 203d      contest_id =
-00004a90: 2073 7472 2863 6f6e 7465 7374 2e67 6574   str(contest.get
-00004aa0: 2822 436f 6e74 6573 7449 4422 2c20 3129  ("ContestID", 1)
-00004ab0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00004ac0: 2020 636f 6e74 6573 745f 6e61 6d65 203d    contest_name =
-00004ad0: 2063 6f6e 7465 7374 2e67 6574 2822 436f   contest.get("Co
-00004ae0: 6e74 6573 744e 616d 6522 2c20 3129 0a20  ntestName", 1). 
-00004af0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00004b00: 7461 7274 5f64 6174 6520 3d20 636f 6e74  tart_date = cont
-00004b10: 6573 742e 6765 7428 2253 7461 7274 4461  est.get("StartDa
-00004b20: 7465 222c 2031 290a 2020 2020 2020 2020  te", 1).        
-00004b30: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
-00004b40: 7465 7374 5f64 6961 6c6f 672e 636f 6e74  test_dialog.cont
-00004b50: 6573 745f 6c69 7374 2e73 6574 4974 656d  est_list.setItem
-00004b60: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00004b70: 2020 2020 2020 6e75 6d62 6572 5f6f 665f        number_of_
-00004b80: 726f 7773 2c20 302c 2051 7457 6964 6765  rows, 0, QtWidge
-00004b90: 7473 2e51 5461 626c 6557 6964 6765 7449  ts.QTableWidgetI
-00004ba0: 7465 6d28 636f 6e74 6573 745f 6964 290a  tem(contest_id).
-00004bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004bc0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00004bd0: 2020 7365 6c66 2e63 6f6e 7465 7374 5f64    self.contest_d
-00004be0: 6961 6c6f 672e 636f 6e74 6573 745f 6c69  ialog.contest_li
-00004bf0: 7374 2e73 6574 4974 656d 280a 2020 2020  st.setItem(.    
-00004c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004c10: 6e75 6d62 6572 5f6f 665f 726f 7773 2c20  number_of_rows, 
-00004c20: 312c 2051 7457 6964 6765 7473 2e51 5461  1, QtWidgets.QTa
-00004c30: 626c 6557 6964 6765 7449 7465 6d28 636f  bleWidgetItem(co
-00004c40: 6e74 6573 745f 6e61 6d65 290a 2020 2020  ntest_name).    
-00004c50: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-00004c60: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00004c70: 6c66 2e63 6f6e 7465 7374 5f64 6961 6c6f  lf.contest_dialo
-00004c80: 672e 636f 6e74 6573 745f 6c69 7374 2e73  g.contest_list.s
-00004c90: 6574 4974 656d 280a 2020 2020 2020 2020  etItem(.        
-00004ca0: 2020 2020 2020 2020 2020 2020 6e75 6d62              numb
-00004cb0: 6572 5f6f 665f 726f 7773 2c20 322c 2051  er_of_rows, 2, Q
-00004cc0: 7457 6964 6765 7473 2e51 5461 626c 6557  tWidgets.QTableW
-00004cd0: 6964 6765 7449 7465 6d28 7374 6172 745f  idgetItem(start_
-00004ce0: 6461 7465 290a 2020 2020 2020 2020 2020  date).          
-00004cf0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00004d00: 7365 6c66 2e63 6f6e 7465 7374 5f64 6961  self.contest_dia
-00004d10: 6c6f 672e 7368 6f77 2829 0a0a 2020 2020  log.show()..    
-00004d20: 6465 6620 6f70 656e 5f63 6f6e 7465 7374  def open_contest
-00004d30: 5f72 6574 7572 6e28 7365 6c66 293a 0a20  _return(self):. 
-00004d40: 2020 2020 2020 2022 2222 4361 6c6c 6564         """Called
-00004d50: 2062 7920 6f70 656e 5f63 6f6e 7465 7374   by open_contest
-00004d60: 2222 220a 2020 2020 2020 2020 7365 6c65  """.        sele
-00004d70: 6374 6564 5f72 6f77 203d 2073 656c 662e  cted_row = self.
-00004d80: 636f 6e74 6573 745f 6469 616c 6f67 2e63  contest_dialog.c
-00004d90: 6f6e 7465 7374 5f6c 6973 742e 6375 7272  ontest_list.curr
-00004da0: 656e 7452 6f77 2829 0a20 2020 2020 2020  entRow().       
-00004db0: 2063 6f6e 7465 7374 203d 2073 656c 662e   contest = self.
-00004dc0: 636f 6e74 6573 745f 6469 616c 6f67 2e63  contest_dialog.c
-00004dd0: 6f6e 7465 7374 5f6c 6973 742e 6974 656d  ontest_list.item
-00004de0: 2873 656c 6563 7465 645f 726f 772c 2030  (selected_row, 0
-00004df0: 292e 7465 7874 2829 0a20 2020 2020 2020  ).text().       
-00004e00: 2073 656c 662e 7072 6566 5b22 636f 6e74   self.pref["cont
-00004e10: 6573 7422 5d20 3d20 636f 6e74 6573 740a  est"] = contest.
-00004e20: 2020 2020 2020 2020 7365 6c66 2e77 7269          self.wri
-00004e30: 7465 5f70 7265 6665 7265 6e63 6528 290a  te_preference().
-00004e40: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
-00004e50: 6562 7567 2822 5365 6c65 6374 6564 2063  ebug("Selected c
-00004e60: 6f6e 7465 7374 3a20 2573 222c 2066 227b  ontest: %s", f"{
-00004e70: 636f 6e74 6573 747d 2229 0a20 2020 2020  contest}").     
-00004e80: 2020 2073 656c 662e 6c6f 6164 5f63 6f6e     self.load_con
-00004e90: 7465 7374 2829 0a0a 2020 2020 6465 6620  test()..    def 
-00004ea0: 7265 6669 6c6c 5f64 726f 7064 6f77 6e28  refill_dropdown(
-00004eb0: 7365 6c66 2c20 7461 7267 6574 2c20 736f  self, target, so
-00004ec0: 7572 6365 293a 0a20 2020 2020 2020 2022  urce):.        "
-00004ed0: 2222 5265 6669 6c6c 2051 436f 6d62 6f62  ""Refill QCombob
-00004ee0: 6f78 2077 6964 6765 7420 7769 7468 2076  ox widget with v
-00004ef0: 616c 7565 2e22 2222 0a20 2020 2020 2020  alue.""".       
-00004f00: 2069 6e64 6578 203d 2074 6172 6765 742e   index = target.
-00004f10: 6669 6e64 5465 7874 2873 6f75 7263 6529  findText(source)
-00004f20: 0a20 2020 2020 2020 2074 6172 6765 742e  .        target.
-00004f30: 7365 7443 7572 7265 6e74 496e 6465 7828  setCurrentIndex(
-00004f40: 696e 6465 7829 0a0a 2020 2020 6465 6620  index)..    def 
-00004f50: 6564 6974 5f63 6f6e 7465 7374 2873 656c  edit_contest(sel
-00004f60: 6629 3a0a 2020 2020 2020 2020 2222 2245  f):.        """E
-00004f70: 6469 7420 7468 6520 6375 7272 656e 7420  dit the current 
-00004f80: 636f 6e74 6573 7422 2222 0a20 2020 2020  contest""".     
-00004f90: 2020 206c 6f67 6765 722e 6465 6275 6728     logger.debug(
-00004fa0: 2245 6469 7420 636f 6e74 6573 7420 4469  "Edit contest Di
-00004fb0: 616c 6f67 2229 0a20 2020 2020 2020 2069  alog").        i
-00004fc0: 6620 7365 6c66 2e63 6f6e 7465 7374 2069  f self.contest i
-00004fd0: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
-00004fe0: 2020 2020 7365 6c66 2e73 686f 775f 6d65      self.show_me
-00004ff0: 7373 6167 655f 626f 7828 2259 6f75 2068  ssage_box("You h
-00005000: 6176 6520 6e6f 2063 6f6e 7465 7374 2064  ave no contest d
-00005010: 6566 696e 6564 2e22 290a 2020 2020 2020  efined.").      
-00005020: 2020 2020 2020 7265 7475 726e 0a20 2020        return.   
-00005030: 2020 2020 2069 6620 7365 6c66 2e63 6f6e       if self.con
-00005040: 7465 7374 5f73 6574 7469 6e67 7320 6973  test_settings is
-00005050: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00005060: 2020 2072 6574 7572 6e0a 2020 2020 2020     return.      
-00005070: 2020 7365 6c66 2e63 6f6e 7465 7374 5f64    self.contest_d
-00005080: 6961 6c6f 6720 3d20 4e65 7743 6f6e 7465  ialog = NewConte
-00005090: 7374 2857 4f52 4b49 4e47 5f50 4154 4829  st(WORKING_PATH)
-000050a0: 0a20 2020 2020 2020 2073 656c 662e 636f  .        self.co
-000050b0: 6e74 6573 745f 6469 616c 6f67 2e73 6574  ntest_dialog.set
-000050c0: 5769 6e64 6f77 5469 746c 6528 2245 6469  WindowTitle("Edi
-000050d0: 7420 436f 6e74 6573 7422 290a 2020 2020  t Contest").    
-000050e0: 2020 2020 7365 6c66 2e63 6f6e 7465 7374      self.contest
-000050f0: 5f64 6961 6c6f 672e 7469 746c 652e 7365  _dialog.title.se
-00005100: 7454 6578 7428 2222 290a 2020 2020 2020  tText("").      
-00005110: 2020 7365 6c66 2e63 6f6e 7465 7374 5f64    self.contest_d
-00005120: 6961 6c6f 672e 6163 6365 7074 6564 2e63  ialog.accepted.c
-00005130: 6f6e 6e65 6374 2873 656c 662e 7361 7665  onnect(self.save
-00005140: 5f65 6469 7465 645f 636f 6e74 6573 7429  _edited_contest)
-00005150: 0a20 2020 2020 2020 2076 616c 7565 203d  .        value =
-00005160: 2073 656c 662e 636f 6e74 6573 745f 7365   self.contest_se
-00005170: 7474 696e 6773 2e67 6574 2822 436f 6e74  ttings.get("Cont
-00005180: 6573 744e 616d 6522 292e 7570 7065 7228  estName").upper(
-00005190: 292e 7265 706c 6163 6528 225f 222c 2022  ).replace("_", "
-000051a0: 2022 290a 2020 2020 2020 2020 6966 2076   ").        if v
-000051b0: 616c 7565 203d 3d20 2247 454e 4552 414c  alue == "GENERAL
-000051c0: 204c 4f47 4749 4e47 223a 0a20 2020 2020   LOGGING":.     
-000051d0: 2020 2020 2020 2076 616c 7565 203d 2022         value = "
-000051e0: 4765 6e65 7261 6c20 4c6f 6767 696e 6722  General Logging"
-000051f0: 0a20 2020 2020 2020 2073 656c 662e 7265  .        self.re
-00005200: 6669 6c6c 5f64 726f 7064 6f77 6e28 7365  fill_dropdown(se
-00005210: 6c66 2e63 6f6e 7465 7374 5f64 6961 6c6f  lf.contest_dialo
-00005220: 672e 636f 6e74 6573 742c 2076 616c 7565  g.contest, value
-00005230: 290a 2020 2020 2020 2020 7661 6c75 6520  ).        value 
-00005240: 3d20 7365 6c66 2e63 6f6e 7465 7374 5f73  = self.contest_s
-00005250: 6574 7469 6e67 732e 6765 7428 224f 7065  ettings.get("Ope
-00005260: 7261 746f 7243 6174 6567 6f72 7922 290a  ratorCategory").
-00005270: 2020 2020 2020 2020 7365 6c66 2e72 6566          self.ref
-00005280: 696c 6c5f 6472 6f70 646f 776e 2873 656c  ill_dropdown(sel
-00005290: 662e 636f 6e74 6573 745f 6469 616c 6f67  f.contest_dialog
-000052a0: 2e6f 7065 7261 746f 725f 636c 6173 732c  .operator_class,
-000052b0: 2076 616c 7565 290a 2020 2020 2020 2020   value).        
-000052c0: 7661 6c75 6520 3d20 7365 6c66 2e63 6f6e  value = self.con
-000052d0: 7465 7374 5f73 6574 7469 6e67 732e 6765  test_settings.ge
-000052e0: 7428 2242 616e 6443 6174 6567 6f72 7922  t("BandCategory"
-000052f0: 290a 2020 2020 2020 2020 7365 6c66 2e72  ).        self.r
-00005300: 6566 696c 6c5f 6472 6f70 646f 776e 2873  efill_dropdown(s
-00005310: 656c 662e 636f 6e74 6573 745f 6469 616c  elf.contest_dial
-00005320: 6f67 2e62 616e 642c 2076 616c 7565 290a  og.band, value).
-00005330: 2020 2020 2020 2020 7661 6c75 6520 3d20          value = 
-00005340: 7365 6c66 2e63 6f6e 7465 7374 5f73 6574  self.contest_set
-00005350: 7469 6e67 732e 6765 7428 2250 6f77 6572  tings.get("Power
-00005360: 4361 7465 676f 7279 2229 0a20 2020 2020  Category").     
-00005370: 2020 2073 656c 662e 7265 6669 6c6c 5f64     self.refill_d
-00005380: 726f 7064 6f77 6e28 7365 6c66 2e63 6f6e  ropdown(self.con
-00005390: 7465 7374 5f64 6961 6c6f 672e 706f 7765  test_dialog.powe
-000053a0: 722c 2076 616c 7565 290a 2020 2020 2020  r, value).      
-000053b0: 2020 7661 6c75 6520 3d20 7365 6c66 2e63    value = self.c
-000053c0: 6f6e 7465 7374 5f73 6574 7469 6e67 732e  ontest_settings.
-000053d0: 6765 7428 224d 6f64 6543 6174 6567 6f72  get("ModeCategor
-000053e0: 7922 290a 2020 2020 2020 2020 7365 6c66  y").        self
-000053f0: 2e72 6566 696c 6c5f 6472 6f70 646f 776e  .refill_dropdown
-00005400: 2873 656c 662e 636f 6e74 6573 745f 6469  (self.contest_di
-00005410: 616c 6f67 2e6d 6f64 652c 2076 616c 7565  alog.mode, value
-00005420: 290a 2020 2020 2020 2020 7661 6c75 6520  ).        value 
-00005430: 3d20 7365 6c66 2e63 6f6e 7465 7374 5f73  = self.contest_s
-00005440: 6574 7469 6e67 732e 6765 7428 224f 7665  ettings.get("Ove
-00005450: 726c 6179 4361 7465 676f 7279 2229 0a20  rlayCategory"). 
-00005460: 2020 2020 2020 2073 656c 662e 7265 6669         self.refi
-00005470: 6c6c 5f64 726f 7064 6f77 6e28 7365 6c66  ll_dropdown(self
-00005480: 2e63 6f6e 7465 7374 5f64 6961 6c6f 672e  .contest_dialog.
-00005490: 6f76 6572 6c61 792c 2076 616c 7565 290a  overlay, value).
-000054a0: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
-000054b0: 7465 7374 5f64 6961 6c6f 672e 6f70 6572  test_dialog.oper
-000054c0: 6174 6f72 732e 7365 7454 6578 7428 7365  ators.setText(se
-000054d0: 6c66 2e63 6f6e 7465 7374 5f73 6574 7469  lf.contest_setti
-000054e0: 6e67 732e 6765 7428 224f 7065 7261 746f  ngs.get("Operato
-000054f0: 7273 2229 290a 2020 2020 2020 2020 7365  rs")).        se
-00005500: 6c66 2e63 6f6e 7465 7374 5f64 6961 6c6f  lf.contest_dialo
-00005510: 672e 736f 6170 626f 782e 7365 7450 6c61  g.soapbox.setPla
-00005520: 696e 5465 7874 2873 656c 662e 636f 6e74  inText(self.cont
-00005530: 6573 745f 7365 7474 696e 6773 2e67 6574  est_settings.get
-00005540: 2822 536f 6170 626f 7822 2929 0a20 2020  ("Soapbox")).   
-00005550: 2020 2020 2073 656c 662e 636f 6e74 6573       self.contes
-00005560: 745f 6469 616c 6f67 2e65 7863 6861 6e67  t_dialog.exchang
-00005570: 652e 7365 7454 6578 7428 7365 6c66 2e63  e.setText(self.c
-00005580: 6f6e 7465 7374 5f73 6574 7469 6e67 732e  ontest_settings.
-00005590: 6765 7428 2253 656e 7445 7863 6861 6e67  get("SentExchang
-000055a0: 6522 2929 0a20 2020 2020 2020 2076 616c  e")).        val
-000055b0: 7565 203d 2073 656c 662e 636f 6e74 6573  ue = self.contes
-000055c0: 745f 7365 7474 696e 6773 2e67 6574 2822  t_settings.get("
-000055d0: 5374 6174 696f 6e43 6174 6567 6f72 7922  StationCategory"
-000055e0: 290a 2020 2020 2020 2020 7365 6c66 2e72  ).        self.r
-000055f0: 6566 696c 6c5f 6472 6f70 646f 776e 2873  efill_dropdown(s
-00005600: 656c 662e 636f 6e74 6573 745f 6469 616c  elf.contest_dial
-00005610: 6f67 2e73 7461 7469 6f6e 2c20 7661 6c75  og.station, valu
-00005620: 6529 0a20 2020 2020 2020 2076 616c 7565  e).        value
-00005630: 203d 2073 656c 662e 636f 6e74 6573 745f   = self.contest_
-00005640: 7365 7474 696e 6773 2e67 6574 2822 4173  settings.get("As
-00005650: 7369 7374 6564 4361 7465 676f 7279 2229  sistedCategory")
-00005660: 0a20 2020 2020 2020 2073 656c 662e 7265  .        self.re
-00005670: 6669 6c6c 5f64 726f 7064 6f77 6e28 7365  fill_dropdown(se
-00005680: 6c66 2e63 6f6e 7465 7374 5f64 6961 6c6f  lf.contest_dialo
-00005690: 672e 6173 7369 7374 6564 2c20 7661 6c75  g.assisted, valu
-000056a0: 6529 0a20 2020 2020 2020 2076 616c 7565  e).        value
-000056b0: 203d 2073 656c 662e 636f 6e74 6573 745f   = self.contest_
-000056c0: 7365 7474 696e 6773 2e67 6574 2822 5472  settings.get("Tr
-000056d0: 616e 736d 6974 7465 7243 6174 6567 6f72  ansmitterCategor
-000056e0: 7922 290a 2020 2020 2020 2020 7365 6c66  y").        self
-000056f0: 2e72 6566 696c 6c5f 6472 6f70 646f 776e  .refill_dropdown
-00005700: 2873 656c 662e 636f 6e74 6573 745f 6469  (self.contest_di
-00005710: 616c 6f67 2e74 7261 6e73 6d69 7474 6572  alog.transmitter
-00005720: 2c20 7661 6c75 6529 0a20 2020 2020 2020  , value).       
-00005730: 2076 616c 7565 203d 2073 656c 662e 636f   value = self.co
-00005740: 6e74 6573 745f 7365 7474 696e 6773 2e67  ntest_settings.g
-00005750: 6574 2822 5374 6172 7444 6174 6522 290a  et("StartDate").
-00005760: 2020 2020 2020 2020 7468 655f 6461 7465          the_date
-00005770: 2c20 7468 655f 7469 6d65 203d 2076 616c  , the_time = val
-00005780: 7565 2e73 706c 6974 2829 0a20 2020 2020  ue.split().     
-00005790: 2020 2073 656c 662e 636f 6e74 6573 745f     self.contest_
-000057a0: 6469 616c 6f67 2e64 6174 6554 696d 6545  dialog.dateTimeE
-000057b0: 6469 742e 7365 7444 6174 6528 0a20 2020  dit.setDate(.   
-000057c0: 2020 2020 2020 2020 2051 7443 6f72 652e           QtCore.
-000057d0: 5144 6174 652e 6672 6f6d 5374 7269 6e67  QDate.fromString
-000057e0: 2874 6865 5f64 6174 652c 2022 7979 7979  (the_date, "yyyy
-000057f0: 2d4d 4d2d 6464 2229 0a20 2020 2020 2020  -MM-dd").       
-00005800: 2029 0a20 2020 2020 2020 2073 656c 662e   ).        self.
-00005810: 636f 6e74 6573 745f 6469 616c 6f67 2e64  contest_dialog.d
-00005820: 6174 6554 696d 6545 6469 742e 7365 7443  ateTimeEdit.setC
-00005830: 616c 656e 6461 7250 6f70 7570 2854 7275  alendarPopup(Tru
-00005840: 6529 0a20 2020 2020 2020 2073 656c 662e  e).        self.
-00005850: 636f 6e74 6573 745f 6469 616c 6f67 2e64  contest_dialog.d
-00005860: 6174 6554 696d 6545 6469 742e 7365 7454  ateTimeEdit.setT
-00005870: 696d 6528 0a20 2020 2020 2020 2020 2020  ime(.           
-00005880: 2051 7443 6f72 652e 5154 696d 652e 6672   QtCore.QTime.fr
-00005890: 6f6d 5374 7269 6e67 2874 6865 5f74 696d  omString(the_tim
-000058a0: 652c 2022 6868 3a6d 6d3a 7373 2229 0a20  e, "hh:mm:ss"). 
-000058b0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-000058c0: 2073 656c 662e 636f 6e74 6573 745f 6469   self.contest_di
-000058d0: 616c 6f67 2e6f 7065 6e28 290a 0a20 2020  alog.open()..   
-000058e0: 2064 6566 2073 6176 655f 6564 6974 6564   def save_edited
-000058f0: 5f63 6f6e 7465 7374 2873 656c 6629 3a0a  _contest(self):.
-00005900: 2020 2020 2020 2020 2222 2253 6176 6520          """Save 
-00005910: 7468 6520 6564 6974 6564 2063 6f6e 7465  the edited conte
-00005920: 7374 2222 220a 2020 2020 2020 2020 636f  st""".        co
-00005930: 6e74 6573 7420 3d20 7b7d 0a20 2020 2020  ntest = {}.     
-00005940: 2020 2063 6f6e 7465 7374 5b22 436f 6e74     contest["Cont
-00005950: 6573 744e 616d 6522 5d20 3d20 280a 2020  estName"] = (.  
-00005960: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-00005970: 6f6e 7465 7374 5f64 6961 6c6f 672e 636f  ontest_dialog.co
-00005980: 6e74 6573 742e 6375 7272 656e 7454 6578  ntest.currentTex
-00005990: 7428 292e 6c6f 7765 7228 292e 7265 706c  t().lower().repl
-000059a0: 6163 6528 2220 222c 2022 5f22 290a 2020  ace(" ", "_").  
-000059b0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-000059c0: 636f 6e74 6573 745b 2253 7461 7274 4461  contest["StartDa
-000059d0: 7465 225d 203d 2073 656c 662e 636f 6e74  te"] = self.cont
-000059e0: 6573 745f 6469 616c 6f67 2e64 6174 6554  est_dialog.dateT
-000059f0: 696d 6545 6469 742e 6461 7465 5469 6d65  imeEdit.dateTime
-00005a00: 2829 2e74 6f53 7472 696e 6728 0a20 2020  ().toString(.   
-00005a10: 2020 2020 2020 2020 2022 7979 7979 2d4d           "yyyy-M
-00005a20: 4d2d 6464 2068 683a 6d6d 3a73 7322 0a20  M-dd hh:mm:ss". 
-00005a30: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00005a40: 2063 6f6e 7465 7374 5b22 4f70 6572 6174   contest["Operat
-00005a50: 6f72 4361 7465 676f 7279 225d 203d 2073  orCategory"] = s
-00005a60: 656c 662e 636f 6e74 6573 745f 6469 616c  elf.contest_dial
-00005a70: 6f67 2e6f 7065 7261 746f 725f 636c 6173  og.operator_clas
-00005a80: 732e 6375 7272 656e 7454 6578 7428 290a  s.currentText().
-00005a90: 2020 2020 2020 2020 636f 6e74 6573 745b          contest[
-00005aa0: 2242 616e 6443 6174 6567 6f72 7922 5d20  "BandCategory"] 
-00005ab0: 3d20 7365 6c66 2e63 6f6e 7465 7374 5f64  = self.contest_d
-00005ac0: 6961 6c6f 672e 6261 6e64 2e63 7572 7265  ialog.band.curre
+00001f20: 2020 7365 6c66 2e72 6164 696f 4275 7474    self.radioButt
+00001f30: 6f6e 5f73 702e 636c 6963 6b65 642e 636f  on_sp.clicked.co
+00001f40: 6e6e 6563 7428 7365 6c66 2e72 756e 5f73  nnect(self.run_s
+00001f50: 705f 6275 7474 6f6e 735f 636c 6963 6b65  p_buttons_clicke
+00001f60: 6429 0a20 2020 2020 2020 2073 656c 662e  d).        self.
+00001f70: 7363 6f72 652e 7365 7454 6578 7428 2230  score.setText("0
+00001f80: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
+00001f90: 6361 6c6c 7369 676e 2e74 6578 7445 6469  callsign.textEdi
+00001fa0: 7465 642e 636f 6e6e 6563 7428 7365 6c66  ted.connect(self
+00001fb0: 2e63 616c 6c73 6967 6e5f 6368 616e 6765  .callsign_change
+00001fc0: 6429 0a20 2020 2020 2020 2073 656c 662e  d).        self.
+00001fd0: 6361 6c6c 7369 676e 2e72 6574 7572 6e50  callsign.returnP
+00001fe0: 7265 7373 6564 2e63 6f6e 6e65 6374 2873  ressed.connect(s
+00001ff0: 656c 662e 7361 7665 5f63 6f6e 7461 6374  elf.save_contact
+00002000: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
+00002010: 656e 742e 7265 7475 726e 5072 6573 7365  ent.returnPresse
+00002020: 642e 636f 6e6e 6563 7428 7365 6c66 2e73  d.connect(self.s
+00002030: 6176 655f 636f 6e74 6163 7429 0a20 2020  ave_contact).   
+00002040: 2020 2020 2073 656c 662e 7265 6365 6976       self.receiv
+00002050: 652e 7265 7475 726e 5072 6573 7365 642e  e.returnPressed.
+00002060: 636f 6e6e 6563 7428 7365 6c66 2e73 6176  connect(self.sav
+00002070: 655f 636f 6e74 6163 7429 0a20 2020 2020  e_contact).     
+00002080: 2020 2073 656c 662e 6f74 6865 725f 312e     self.other_1.
+00002090: 7265 7475 726e 5072 6573 7365 642e 636f  returnPressed.co
+000020a0: 6e6e 6563 7428 7365 6c66 2e73 6176 655f  nnect(self.save_
+000020b0: 636f 6e74 6163 7429 0a20 2020 2020 2020  contact).       
+000020c0: 2073 656c 662e 6f74 6865 725f 322e 7265   self.other_2.re
+000020d0: 7475 726e 5072 6573 7365 642e 636f 6e6e  turnPressed.conn
+000020e0: 6563 7428 7365 6c66 2e73 6176 655f 636f  ect(self.save_co
+000020f0: 6e74 6163 7429 0a20 2020 2020 2020 2073  ntact).        s
+00002100: 656c 662e 6f74 6865 725f 322e 7465 7874  elf.other_2.text
+00002110: 4564 6974 6564 2e63 6f6e 6e65 6374 2873  Edited.connect(s
+00002120: 656c 662e 6f74 6865 725f 325f 6368 616e  elf.other_2_chan
+00002130: 6765 6429 0a0a 2020 2020 2020 2020 7365  ged)..        se
+00002140: 6c66 2e73 656e 742e 7365 7454 6578 7428  lf.sent.setText(
+00002150: 2235 3922 290a 2020 2020 2020 2020 7365  "59").        se
+00002160: 6c66 2e72 6563 6569 7665 2e73 6574 5465  lf.receive.setTe
+00002170: 7874 2822 3539 2229 0a20 2020 2020 2020  xt("59").       
+00002180: 2069 636f 6e5f 7061 7468 203d 2057 4f52   icon_path = WOR
+00002190: 4b49 4e47 5f50 4154 4820 2b20 222f 6461  KING_PATH + "/da
+000021a0: 7461 2f22 0a20 2020 2020 2020 2073 656c  ta/".        sel
+000021b0: 662e 6772 6565 6e64 6f74 203d 2051 7447  f.greendot = QtG
+000021c0: 7569 2e51 5069 786d 6170 2869 636f 6e5f  ui.QPixmap(icon_
+000021d0: 7061 7468 202b 2022 6772 6565 6e64 6f74  path + "greendot
+000021e0: 2e70 6e67 2229 0a20 2020 2020 2020 2073  .png").        s
+000021f0: 656c 662e 7265 6464 6f74 203d 2051 7447  elf.reddot = QtG
+00002200: 7569 2e51 5069 786d 6170 2869 636f 6e5f  ui.QPixmap(icon_
+00002210: 7061 7468 202b 2022 7265 6464 6f74 2e70  path + "reddot.p
+00002220: 6e67 2229 0a20 2020 2020 2020 2073 656c  ng").        sel
+00002230: 662e 6c65 6674 646f 742e 7365 7450 6978  f.leftdot.setPix
+00002240: 6d61 7028 7365 6c66 2e67 7265 656e 646f  map(self.greendo
+00002250: 7429 0a20 2020 2020 2020 2073 656c 662e  t).        self.
+00002260: 7269 6768 7464 6f74 2e73 6574 5069 786d  rightdot.setPixm
+00002270: 6170 2873 656c 662e 7265 6464 6f74 290a  ap(self.reddot).
+00002280: 0a20 2020 2020 2020 2073 656c 662e 4631  .        self.F1
+00002290: 2e73 6574 436f 6e74 6578 744d 656e 7550  .setContextMenuP
+000022a0: 6f6c 6963 7928 5174 436f 7265 2e51 742e  olicy(QtCore.Qt.
+000022b0: 4375 7374 6f6d 436f 6e74 6578 744d 656e  CustomContextMen
+000022c0: 7529 0a20 2020 2020 2020 2073 656c 662e  u).        self.
+000022d0: 4631 2e63 7573 746f 6d43 6f6e 7465 7874  F1.customContext
+000022e0: 4d65 6e75 5265 7175 6573 7465 642e 636f  MenuRequested.co
+000022f0: 6e6e 6563 7428 7365 6c66 2e65 6469 745f  nnect(self.edit_
+00002300: 4631 290a 2020 2020 2020 2020 7365 6c66  F1).        self
+00002310: 2e46 312e 636c 6963 6b65 642e 636f 6e6e  .F1.clicked.conn
+00002320: 6563 7428 7365 6c66 2e73 656e 6466 3129  ect(self.sendf1)
+00002330: 0a20 2020 2020 2020 2073 656c 662e 4632  .        self.F2
+00002340: 2e73 6574 436f 6e74 6578 744d 656e 7550  .setContextMenuP
+00002350: 6f6c 6963 7928 5174 436f 7265 2e51 742e  olicy(QtCore.Qt.
+00002360: 4375 7374 6f6d 436f 6e74 6578 744d 656e  CustomContextMen
+00002370: 7529 0a20 2020 2020 2020 2073 656c 662e  u).        self.
+00002380: 4632 2e63 7573 746f 6d43 6f6e 7465 7874  F2.customContext
+00002390: 4d65 6e75 5265 7175 6573 7465 642e 636f  MenuRequested.co
+000023a0: 6e6e 6563 7428 7365 6c66 2e65 6469 745f  nnect(self.edit_
+000023b0: 4632 290a 2020 2020 2020 2020 7365 6c66  F2).        self
+000023c0: 2e46 322e 636c 6963 6b65 642e 636f 6e6e  .F2.clicked.conn
+000023d0: 6563 7428 7365 6c66 2e73 656e 6466 3229  ect(self.sendf2)
+000023e0: 0a20 2020 2020 2020 2073 656c 662e 4633  .        self.F3
+000023f0: 2e73 6574 436f 6e74 6578 744d 656e 7550  .setContextMenuP
+00002400: 6f6c 6963 7928 5174 436f 7265 2e51 742e  olicy(QtCore.Qt.
+00002410: 4375 7374 6f6d 436f 6e74 6578 744d 656e  CustomContextMen
+00002420: 7529 0a20 2020 2020 2020 2073 656c 662e  u).        self.
+00002430: 4633 2e63 7573 746f 6d43 6f6e 7465 7874  F3.customContext
+00002440: 4d65 6e75 5265 7175 6573 7465 642e 636f  MenuRequested.co
+00002450: 6e6e 6563 7428 7365 6c66 2e65 6469 745f  nnect(self.edit_
+00002460: 4633 290a 2020 2020 2020 2020 7365 6c66  F3).        self
+00002470: 2e46 332e 636c 6963 6b65 642e 636f 6e6e  .F3.clicked.conn
+00002480: 6563 7428 7365 6c66 2e73 656e 6466 3329  ect(self.sendf3)
+00002490: 0a20 2020 2020 2020 2073 656c 662e 4634  .        self.F4
+000024a0: 2e73 6574 436f 6e74 6578 744d 656e 7550  .setContextMenuP
+000024b0: 6f6c 6963 7928 5174 436f 7265 2e51 742e  olicy(QtCore.Qt.
+000024c0: 4375 7374 6f6d 436f 6e74 6578 744d 656e  CustomContextMen
+000024d0: 7529 0a20 2020 2020 2020 2073 656c 662e  u).        self.
+000024e0: 4634 2e63 7573 746f 6d43 6f6e 7465 7874  F4.customContext
+000024f0: 4d65 6e75 5265 7175 6573 7465 642e 636f  MenuRequested.co
+00002500: 6e6e 6563 7428 7365 6c66 2e65 6469 745f  nnect(self.edit_
+00002510: 4634 290a 2020 2020 2020 2020 7365 6c66  F4).        self
+00002520: 2e46 342e 636c 6963 6b65 642e 636f 6e6e  .F4.clicked.conn
+00002530: 6563 7428 7365 6c66 2e73 656e 6466 3429  ect(self.sendf4)
+00002540: 0a20 2020 2020 2020 2073 656c 662e 4635  .        self.F5
+00002550: 2e73 6574 436f 6e74 6578 744d 656e 7550  .setContextMenuP
+00002560: 6f6c 6963 7928 5174 436f 7265 2e51 742e  olicy(QtCore.Qt.
+00002570: 4375 7374 6f6d 436f 6e74 6578 744d 656e  CustomContextMen
+00002580: 7529 0a20 2020 2020 2020 2073 656c 662e  u).        self.
+00002590: 4635 2e63 7573 746f 6d43 6f6e 7465 7874  F5.customContext
+000025a0: 4d65 6e75 5265 7175 6573 7465 642e 636f  MenuRequested.co
+000025b0: 6e6e 6563 7428 7365 6c66 2e65 6469 745f  nnect(self.edit_
+000025c0: 4635 290a 2020 2020 2020 2020 7365 6c66  F5).        self
+000025d0: 2e46 352e 636c 6963 6b65 642e 636f 6e6e  .F5.clicked.conn
+000025e0: 6563 7428 7365 6c66 2e73 656e 6466 3529  ect(self.sendf5)
+000025f0: 0a20 2020 2020 2020 2073 656c 662e 4636  .        self.F6
+00002600: 2e73 6574 436f 6e74 6578 744d 656e 7550  .setContextMenuP
+00002610: 6f6c 6963 7928 5174 436f 7265 2e51 742e  olicy(QtCore.Qt.
+00002620: 4375 7374 6f6d 436f 6e74 6578 744d 656e  CustomContextMen
+00002630: 7529 0a20 2020 2020 2020 2073 656c 662e  u).        self.
+00002640: 4636 2e63 7573 746f 6d43 6f6e 7465 7874  F6.customContext
+00002650: 4d65 6e75 5265 7175 6573 7465 642e 636f  MenuRequested.co
+00002660: 6e6e 6563 7428 7365 6c66 2e65 6469 745f  nnect(self.edit_
+00002670: 4636 290a 2020 2020 2020 2020 7365 6c66  F6).        self
+00002680: 2e46 362e 636c 6963 6b65 642e 636f 6e6e  .F6.clicked.conn
+00002690: 6563 7428 7365 6c66 2e73 656e 6466 3629  ect(self.sendf6)
+000026a0: 0a20 2020 2020 2020 2073 656c 662e 4637  .        self.F7
+000026b0: 2e73 6574 436f 6e74 6578 744d 656e 7550  .setContextMenuP
+000026c0: 6f6c 6963 7928 5174 436f 7265 2e51 742e  olicy(QtCore.Qt.
+000026d0: 4375 7374 6f6d 436f 6e74 6578 744d 656e  CustomContextMen
+000026e0: 7529 0a20 2020 2020 2020 2073 656c 662e  u).        self.
+000026f0: 4637 2e63 7573 746f 6d43 6f6e 7465 7874  F7.customContext
+00002700: 4d65 6e75 5265 7175 6573 7465 642e 636f  MenuRequested.co
+00002710: 6e6e 6563 7428 7365 6c66 2e65 6469 745f  nnect(self.edit_
+00002720: 4637 290a 2020 2020 2020 2020 7365 6c66  F7).        self
+00002730: 2e46 372e 636c 6963 6b65 642e 636f 6e6e  .F7.clicked.conn
+00002740: 6563 7428 7365 6c66 2e73 656e 6466 3729  ect(self.sendf7)
+00002750: 0a20 2020 2020 2020 2073 656c 662e 4638  .        self.F8
+00002760: 2e73 6574 436f 6e74 6578 744d 656e 7550  .setContextMenuP
+00002770: 6f6c 6963 7928 5174 436f 7265 2e51 742e  olicy(QtCore.Qt.
+00002780: 4375 7374 6f6d 436f 6e74 6578 744d 656e  CustomContextMen
+00002790: 7529 0a20 2020 2020 2020 2073 656c 662e  u).        self.
+000027a0: 4638 2e63 7573 746f 6d43 6f6e 7465 7874  F8.customContext
+000027b0: 4d65 6e75 5265 7175 6573 7465 642e 636f  MenuRequested.co
+000027c0: 6e6e 6563 7428 7365 6c66 2e65 6469 745f  nnect(self.edit_
+000027d0: 4638 290a 2020 2020 2020 2020 7365 6c66  F8).        self
+000027e0: 2e46 382e 636c 6963 6b65 642e 636f 6e6e  .F8.clicked.conn
+000027f0: 6563 7428 7365 6c66 2e73 656e 6466 3829  ect(self.sendf8)
+00002800: 0a20 2020 2020 2020 2073 656c 662e 4639  .        self.F9
+00002810: 2e73 6574 436f 6e74 6578 744d 656e 7550  .setContextMenuP
+00002820: 6f6c 6963 7928 5174 436f 7265 2e51 742e  olicy(QtCore.Qt.
+00002830: 4375 7374 6f6d 436f 6e74 6578 744d 656e  CustomContextMen
+00002840: 7529 0a20 2020 2020 2020 2073 656c 662e  u).        self.
+00002850: 4639 2e63 7573 746f 6d43 6f6e 7465 7874  F9.customContext
+00002860: 4d65 6e75 5265 7175 6573 7465 642e 636f  MenuRequested.co
+00002870: 6e6e 6563 7428 7365 6c66 2e65 6469 745f  nnect(self.edit_
+00002880: 4639 290a 2020 2020 2020 2020 7365 6c66  F9).        self
+00002890: 2e46 392e 636c 6963 6b65 642e 636f 6e6e  .F9.clicked.conn
+000028a0: 6563 7428 7365 6c66 2e73 656e 6466 3929  ect(self.sendf9)
+000028b0: 0a20 2020 2020 2020 2073 656c 662e 4631  .        self.F1
+000028c0: 302e 7365 7443 6f6e 7465 7874 4d65 6e75  0.setContextMenu
+000028d0: 506f 6c69 6379 2851 7443 6f72 652e 5174  Policy(QtCore.Qt
+000028e0: 2e43 7573 746f 6d43 6f6e 7465 7874 4d65  .CustomContextMe
+000028f0: 6e75 290a 2020 2020 2020 2020 7365 6c66  nu).        self
+00002900: 2e46 3130 2e63 7573 746f 6d43 6f6e 7465  .F10.customConte
+00002910: 7874 4d65 6e75 5265 7175 6573 7465 642e  xtMenuRequested.
+00002920: 636f 6e6e 6563 7428 7365 6c66 2e65 6469  connect(self.edi
+00002930: 745f 4631 3029 0a20 2020 2020 2020 2073  t_F10).        s
+00002940: 656c 662e 4631 302e 636c 6963 6b65 642e  elf.F10.clicked.
+00002950: 636f 6e6e 6563 7428 7365 6c66 2e73 656e  connect(self.sen
+00002960: 6466 3130 290a 2020 2020 2020 2020 7365  df10).        se
+00002970: 6c66 2e46 3131 2e73 6574 436f 6e74 6578  lf.F11.setContex
+00002980: 744d 656e 7550 6f6c 6963 7928 5174 436f  tMenuPolicy(QtCo
+00002990: 7265 2e51 742e 4375 7374 6f6d 436f 6e74  re.Qt.CustomCont
+000029a0: 6578 744d 656e 7529 0a20 2020 2020 2020  extMenu).       
+000029b0: 2073 656c 662e 4631 312e 6375 7374 6f6d   self.F11.custom
+000029c0: 436f 6e74 6578 744d 656e 7552 6571 7565  ContextMenuReque
+000029d0: 7374 6564 2e63 6f6e 6e65 6374 2873 656c  sted.connect(sel
+000029e0: 662e 6564 6974 5f46 3131 290a 2020 2020  f.edit_F11).    
+000029f0: 2020 2020 7365 6c66 2e46 3131 2e63 6c69      self.F11.cli
+00002a00: 636b 6564 2e63 6f6e 6e65 6374 2873 656c  cked.connect(sel
+00002a10: 662e 7365 6e64 6631 3129 0a20 2020 2020  f.sendf11).     
+00002a20: 2020 2073 656c 662e 4631 322e 7365 7443     self.F12.setC
+00002a30: 6f6e 7465 7874 4d65 6e75 506f 6c69 6379  ontextMenuPolicy
+00002a40: 2851 7443 6f72 652e 5174 2e43 7573 746f  (QtCore.Qt.Custo
+00002a50: 6d43 6f6e 7465 7874 4d65 6e75 290a 2020  mContextMenu).  
+00002a60: 2020 2020 2020 7365 6c66 2e46 3132 2e63        self.F12.c
+00002a70: 7573 746f 6d43 6f6e 7465 7874 4d65 6e75  ustomContextMenu
+00002a80: 5265 7175 6573 7465 642e 636f 6e6e 6563  Requested.connec
+00002a90: 7428 7365 6c66 2e65 6469 745f 4631 3229  t(self.edit_F12)
+00002aa0: 0a20 2020 2020 2020 2073 656c 662e 4631  .        self.F1
+00002ab0: 322e 636c 6963 6b65 642e 636f 6e6e 6563  2.clicked.connec
+00002ac0: 7428 7365 6c66 2e73 656e 6466 3132 290a  t(self.sendf12).
+00002ad0: 0a20 2020 2020 2020 2073 656c 662e 7265  .        self.re
+00002ae0: 6164 7072 6566 6572 656e 6365 7328 290a  adpreferences().
+00002af0: 2020 2020 2020 2020 7365 6c66 2e64 626e          self.dbn
+00002b00: 616d 6520 3d20 4441 5441 5f50 4154 4820  ame = DATA_PATH 
+00002b10: 2b20 222f 2220 2b20 7365 6c66 2e70 7265  + "/" + self.pre
+00002b20: 662e 6765 7428 2263 7572 7265 6e74 5f64  f.get("current_d
+00002b30: 6174 6162 6173 6522 2c20 2268 616d 2e64  atabase", "ham.d
+00002b40: 6222 290a 2020 2020 2020 2020 7365 6c66  b").        self
+00002b50: 2e64 6174 6162 6173 6520 3d20 4461 7461  .database = Data
+00002b60: 4261 7365 2873 656c 662e 6462 6e61 6d65  Base(self.dbname
+00002b70: 2c20 574f 524b 494e 475f 5041 5448 290a  , WORKING_PATH).
+00002b80: 2020 2020 2020 2020 7365 6c66 2e73 7461          self.sta
+00002b90: 7469 6f6e 203d 2073 656c 662e 6461 7461  tion = self.data
+00002ba0: 6261 7365 2e66 6574 6368 5f73 7461 7469  base.fetch_stati
+00002bb0: 6f6e 2829 0a20 2020 2020 2020 2069 6620  on().        if 
+00002bc0: 7365 6c66 2e73 7461 7469 6f6e 2069 7320  self.station is 
+00002bd0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00002be0: 2020 7365 6c66 2e73 7461 7469 6f6e 203d    self.station =
+00002bf0: 207b 7d0a 2020 2020 2020 2020 2020 2020   {}.            
+00002c00: 7365 6c66 2e65 6469 745f 7374 6174 696f  self.edit_statio
+00002c10: 6e5f 7365 7474 696e 6773 2829 0a20 2020  n_settings().   
+00002c20: 2020 2020 2020 2020 2073 656c 662e 7374           self.st
+00002c30: 6174 696f 6e20 3d20 7365 6c66 2e64 6174  ation = self.dat
+00002c40: 6162 6173 652e 6665 7463 685f 7374 6174  abase.fetch_stat
+00002c50: 696f 6e28 290a 2020 2020 2020 2020 2020  ion().          
+00002c60: 2020 6966 2073 656c 662e 7374 6174 696f    if self.statio
+00002c70: 6e20 6973 204e 6f6e 653a 0a20 2020 2020  n is None:.     
+00002c80: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00002c90: 7374 6174 696f 6e20 3d20 7b7d 0a20 2020  station = {}.   
+00002ca0: 2020 2020 2073 656c 662e 636f 6e74 6163       self.contac
+00002cb0: 7420 3d20 7365 6c66 2e64 6174 6162 6173  t = self.databas
+00002cc0: 652e 656d 7074 795f 636f 6e74 6163 740a  e.empty_contact.
+00002cd0: 2020 2020 2020 2020 7365 6c66 2e63 7572          self.cur
+00002ce0: 7265 6e74 5f6f 7020 3d20 7365 6c66 2e73  rent_op = self.s
+00002cf0: 7461 7469 6f6e 2e67 6574 2822 4361 6c6c  tation.get("Call
+00002d00: 222c 2022 2229 0a20 2020 2020 2020 2073  ", "").        s
+00002d10: 656c 662e 6d61 6b65 5f6f 705f 6469 7228  elf.make_op_dir(
+00002d20: 290a 2020 2020 2020 2020 7365 6c66 2e72  ).        self.r
+00002d30: 6561 645f 6377 5f6d 6163 726f 7328 290a  ead_cw_macros().
+00002d40: 2020 2020 2020 2020 7365 6c66 2e63 6c65          self.cle
+00002d50: 6172 696e 7075 7473 2829 0a0a 2020 2020  arinputs()..    
+00002d60: 2020 2020 7365 6c66 2e62 616e 645f 696e      self.band_in
+00002d70: 6469 6361 746f 7273 5f63 7720 3d20 7b0a  dicators_cw = {.
+00002d80: 2020 2020 2020 2020 2020 2020 2231 3630              "160
+00002d90: 223a 2073 656c 662e 6377 5f62 616e 645f  ": self.cw_band_
+00002da0: 3136 302c 0a20 2020 2020 2020 2020 2020  160,.           
+00002db0: 2022 3830 223a 2073 656c 662e 6377 5f62   "80": self.cw_b
+00002dc0: 616e 645f 3830 2c0a 2020 2020 2020 2020  and_80,.        
+00002dd0: 2020 2020 2234 3022 3a20 7365 6c66 2e63      "40": self.c
+00002de0: 775f 6261 6e64 5f34 302c 0a20 2020 2020  w_band_40,.     
+00002df0: 2020 2020 2020 2022 3230 223a 2073 656c         "20": sel
+00002e00: 662e 6377 5f62 616e 645f 3230 2c0a 2020  f.cw_band_20,.  
+00002e10: 2020 2020 2020 2020 2020 2231 3522 3a20            "15": 
+00002e20: 7365 6c66 2e63 775f 6261 6e64 5f31 352c  self.cw_band_15,
+00002e30: 0a20 2020 2020 2020 2020 2020 2022 3130  .            "10
+00002e40: 223a 2073 656c 662e 6377 5f62 616e 645f  ": self.cw_band_
+00002e50: 3130 2c0a 2020 2020 2020 2020 7d0a 0a20  10,.        }.. 
+00002e60: 2020 2020 2020 2073 656c 662e 6261 6e64         self.band
+00002e70: 5f69 6e64 6963 6174 6f72 735f 7373 6220  _indicators_ssb 
+00002e80: 3d20 7b0a 2020 2020 2020 2020 2020 2020  = {.            
+00002e90: 2231 3630 223a 2073 656c 662e 7373 625f  "160": self.ssb_
+00002ea0: 6261 6e64 5f31 3630 2c0a 2020 2020 2020  band_160,.      
+00002eb0: 2020 2020 2020 2238 3022 3a20 7365 6c66        "80": self
+00002ec0: 2e73 7362 5f62 616e 645f 3830 2c0a 2020  .ssb_band_80,.  
+00002ed0: 2020 2020 2020 2020 2020 2234 3022 3a20            "40": 
+00002ee0: 7365 6c66 2e73 7362 5f62 616e 645f 3430  self.ssb_band_40
+00002ef0: 2c0a 2020 2020 2020 2020 2020 2020 2232  ,.            "2
+00002f00: 3022 3a20 7365 6c66 2e73 7362 5f62 616e  0": self.ssb_ban
+00002f10: 645f 3230 2c0a 2020 2020 2020 2020 2020  d_20,.          
+00002f20: 2020 2231 3522 3a20 7365 6c66 2e73 7362    "15": self.ssb
+00002f30: 5f62 616e 645f 3135 2c0a 2020 2020 2020  _band_15,.      
+00002f40: 2020 2020 2020 2231 3022 3a20 7365 6c66        "10": self
+00002f50: 2e73 7362 5f62 616e 645f 3130 2c0a 2020  .ssb_band_10,.  
+00002f60: 2020 2020 2020 7d0a 0a20 2020 2020 2020        }..       
+00002f70: 2073 656c 662e 6261 6e64 5f69 6e64 6963   self.band_indic
+00002f80: 6174 6f72 735f 7274 7479 203d 207b 0a20  ators_rtty = {. 
+00002f90: 2020 2020 2020 2020 2020 2022 3136 3022             "160"
+00002fa0: 3a20 7365 6c66 2e72 7474 795f 6261 6e64  : self.rtty_band
+00002fb0: 5f31 3630 2c0a 2020 2020 2020 2020 2020  _160,.          
+00002fc0: 2020 2238 3022 3a20 7365 6c66 2e72 7474    "80": self.rtt
+00002fd0: 795f 6261 6e64 5f38 302c 0a20 2020 2020  y_band_80,.     
+00002fe0: 2020 2020 2020 2022 3430 223a 2073 656c         "40": sel
+00002ff0: 662e 7274 7479 5f62 616e 645f 3430 2c0a  f.rtty_band_40,.
+00003000: 2020 2020 2020 2020 2020 2020 2232 3022              "20"
+00003010: 3a20 7365 6c66 2e72 7474 795f 6261 6e64  : self.rtty_band
+00003020: 5f32 302c 0a20 2020 2020 2020 2020 2020  _20,.           
+00003030: 2022 3135 223a 2073 656c 662e 7274 7479   "15": self.rtty
+00003040: 5f62 616e 645f 3135 2c0a 2020 2020 2020  _band_15,.      
+00003050: 2020 2020 2020 2231 3022 3a20 7365 6c66        "10": self
+00003060: 2e72 7474 795f 6261 6e64 5f31 302c 0a20  .rtty_band_10,. 
+00003070: 2020 2020 2020 207d 0a0a 2020 2020 2020         }..      
+00003080: 2020 7365 6c66 2e61 6c6c 5f6d 6f64 655f    self.all_mode_
+00003090: 696e 6469 6361 746f 7273 203d 207b 0a20  indicators = {. 
+000030a0: 2020 2020 2020 2020 2020 2022 4357 223a             "CW":
+000030b0: 2073 656c 662e 6261 6e64 5f69 6e64 6963   self.band_indic
+000030c0: 6174 6f72 735f 6377 2c0a 2020 2020 2020  ators_cw,.      
+000030d0: 2020 2020 2020 2253 5342 223a 2073 656c        "SSB": sel
+000030e0: 662e 6261 6e64 5f69 6e64 6963 6174 6f72  f.band_indicator
+000030f0: 735f 7373 622c 0a20 2020 2020 2020 2020  s_ssb,.         
+00003100: 2020 2022 5254 5459 223a 2073 656c 662e     "RTTY": self.
+00003110: 6261 6e64 5f69 6e64 6963 6174 6f72 735f  band_indicators_
+00003120: 7274 7479 2c0a 2020 2020 2020 2020 7d0a  rtty,.        }.
+00003130: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00003140: 2e70 7265 662e 6765 7428 2263 6f6e 7465  .pref.get("conte
+00003150: 7374 2229 3a0a 2020 2020 2020 2020 2020  st"):.          
+00003160: 2020 7365 6c66 2e6c 6f61 645f 636f 6e74    self.load_cont
+00003170: 6573 7428 290a 0a20 2020 2020 2020 2069  est()..        i
+00003180: 6620 5665 7273 696f 6e54 6573 7428 5f5f  f VersionTest(__
+00003190: 7665 7273 696f 6e5f 5f29 2e74 6573 7428  version__).test(
+000031a0: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
+000031b0: 656c 662e 7368 6f77 5f6d 6573 7361 6765  elf.show_message
+000031c0: 5f62 6f78 280a 2020 2020 2020 2020 2020  _box(.          
+000031d0: 2020 2020 2020 2254 6865 7265 2069 7320        "There is 
+000031e0: 6120 6e65 7765 7220 7665 7273 696f 6e20  a newer version 
+000031f0: 6f66 206e 6f74 316d 6d20 6176 6169 6c61  of not1mm availa
+00003200: 626c 652e 5c6e 220a 2020 2020 2020 2020  ble.\n".        
+00003210: 2020 2020 2020 2020 2259 6f75 2063 616e          "You can
+00003220: 2075 6461 7465 2074 6f20 7468 6520 6375   udate to the cu
+00003230: 7272 656e 7420 7665 7273 696f 6e20 6279  rrent version by
+00003240: 2075 7369 6e67 3a5c 6e70 6970 2069 6e73   using:\npip ins
+00003250: 7461 6c6c 202d 5520 6e6f 7431 6d6d 220a  tall -U not1mm".
+00003260: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
+00003270: 2020 2064 6566 2071 7569 745f 6170 7028     def quit_app(
+00003280: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
+00003290: 2222 646f 6322 2222 0a20 2020 2020 2020  ""doc""".       
+000032a0: 2061 7070 2e71 7569 7428 290a 0a20 2020   app.quit()..   
+000032b0: 2040 7374 6174 6963 6d65 7468 6f64 0a20   @staticmethod. 
+000032c0: 2020 2064 6566 2063 6865 636b 5f70 726f     def check_pro
+000032d0: 6365 7373 286e 616d 653a 2073 7472 2920  cess(name: str) 
+000032e0: 2d3e 2062 6f6f 6c3a 0a20 2020 2020 2020  -> bool:.       
+000032f0: 2022 2222 6368 6563 6b73 2074 6f20 7365   """checks to se
+00003300: 6520 6966 2070 726f 6772 616d 206f 6620  e if program of 
+00003310: 6e61 6d65 2069 7320 696e 2074 6865 2061  name is in the a
+00003320: 6374 6976 6520 7072 6f63 6573 7320 6c69  ctive process li
+00003330: 7374 2222 220a 2020 2020 2020 2020 666f  st""".        fo
+00003340: 7220 7072 6f63 2069 6e20 7073 7574 696c  r proc in psutil
+00003350: 2e70 726f 6365 7373 5f69 7465 7228 293a  .process_iter():
+00003360: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00003370: 626f 6f6c 2872 652e 6d61 7463 6828 6e61  bool(re.match(na
+00003380: 6d65 2c20 7072 6f63 2e6e 616d 6528 292e  me, proc.name().
+00003390: 6c6f 7765 7228 2929 293a 0a20 2020 2020  lower())):.     
+000033a0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+000033b0: 6e20 5472 7565 0a20 2020 2020 2020 2072  n True.        r
+000033c0: 6574 7572 6e20 4661 6c73 650a 0a20 2020  eturn False..   
+000033d0: 2064 6566 2073 686f 775f 6d65 7373 6167   def show_messag
+000033e0: 655f 626f 7828 7365 6c66 2c20 6d65 7373  e_box(self, mess
+000033f0: 6167 653a 2073 7472 2920 2d3e 204e 6f6e  age: str) -> Non
+00003400: 653a 0a20 2020 2020 2020 2022 2222 646f  e:.        """do
+00003410: 6322 2222 0a20 2020 2020 2020 206d 6573  c""".        mes
+00003420: 7361 6765 5f62 6f78 203d 2051 7457 6964  sage_box = QtWid
+00003430: 6765 7473 2e51 4d65 7373 6167 6542 6f78  gets.QMessageBox
+00003440: 2829 0a20 2020 2020 2020 206d 6573 7361  ().        messa
+00003450: 6765 5f62 6f78 2e73 6574 4963 6f6e 2851  ge_box.setIcon(Q
+00003460: 7457 6964 6765 7473 2e51 4d65 7373 6167  tWidgets.QMessag
+00003470: 6542 6f78 2e49 6e66 6f72 6d61 7469 6f6e  eBox.Information
+00003480: 290a 2020 2020 2020 2020 6d65 7373 6167  ).        messag
+00003490: 655f 626f 782e 7365 7454 6578 7428 6d65  e_box.setText(me
+000034a0: 7373 6167 6529 0a20 2020 2020 2020 206d  ssage).        m
+000034b0: 6573 7361 6765 5f62 6f78 2e73 6574 5769  essage_box.setWi
+000034c0: 6e64 6f77 5469 746c 6528 2249 6e66 6f72  ndowTitle("Infor
+000034d0: 6d61 7469 6f6e 2229 0a20 2020 2020 2020  mation").       
+000034e0: 206d 6573 7361 6765 5f62 6f78 2e73 6574   message_box.set
+000034f0: 5374 616e 6461 7264 4275 7474 6f6e 7328  StandardButtons(
+00003500: 5174 5769 6467 6574 732e 514d 6573 7361  QtWidgets.QMessa
+00003510: 6765 426f 782e 4f6b 290a 2020 2020 2020  geBox.Ok).      
+00003520: 2020 5f20 3d20 6d65 7373 6167 655f 626f    _ = message_bo
+00003530: 782e 6578 6563 5f28 290a 0a20 2020 2064  x.exec_()..    d
+00003540: 6566 2073 686f 775f 6162 6f75 745f 6469  ef show_about_di
+00003550: 616c 6f67 2873 656c 6629 3a0a 2020 2020  alog(self):.    
+00003560: 2020 2020 2222 2253 686f 7720 6162 6f75      """Show abou
+00003570: 7420 6469 616c 6f67 2222 220a 2020 2020  t dialog""".    
+00003580: 2020 2020 7365 6c66 2e61 626f 7574 5f64      self.about_d
+00003590: 6961 6c6f 6720 3d20 4162 6f75 7428 574f  ialog = About(WO
+000035a0: 524b 494e 475f 5041 5448 290a 2020 2020  RKING_PATH).    
+000035b0: 2020 2020 7365 6c66 2e61 626f 7574 5f64      self.about_d
+000035c0: 6961 6c6f 672e 646f 6e6f 7273 2e73 6574  ialog.donors.set
+000035d0: 536f 7572 6365 280a 2020 2020 2020 2020  Source(.        
+000035e0: 2020 2020 5174 436f 7265 2e51 5572 6c2e      QtCore.QUrl.
+000035f0: 6672 6f6d 4c6f 6361 6c46 696c 6528 574f  fromLocalFile(WO
+00003600: 524b 494e 475f 5041 5448 202b 2022 2f64  RKING_PATH + "/d
+00003610: 6174 612f 646f 6e6f 7273 2e68 746d 6c22  ata/donors.html"
+00003620: 290a 2020 2020 2020 2020 290a 2020 2020  ).        ).    
+00003630: 2020 2020 7365 6c66 2e61 626f 7574 5f64      self.about_d
+00003640: 6961 6c6f 672e 6f70 656e 2829 0a0a 2020  ialog.open()..  
+00003650: 2020 6465 6620 7368 6f77 5f68 656c 705f    def show_help_
+00003660: 6469 616c 6f67 2873 656c 6629 3a0a 2020  dialog(self):.  
+00003670: 2020 2020 2020 2222 2253 686f 7720 6162        """Show ab
+00003680: 6f75 7420 6469 616c 6f67 2222 220a 2020  out dialog""".  
+00003690: 2020 2020 2020 7365 6c66 2e61 626f 7574        self.about
+000036a0: 5f64 6961 6c6f 6720 3d20 4162 6f75 7428  _dialog = About(
+000036b0: 574f 524b 494e 475f 5041 5448 290a 2020  WORKING_PATH).  
+000036c0: 2020 2020 2020 7365 6c66 2e61 626f 7574        self.about
+000036d0: 5f64 6961 6c6f 672e 7365 7457 696e 646f  _dialog.setWindo
+000036e0: 7754 6974 6c65 2822 4865 6c70 2229 0a20  wTitle("Help"). 
+000036f0: 2020 2020 2020 2073 656c 662e 6162 6f75         self.abou
+00003700: 745f 6469 616c 6f67 2e73 6574 4765 6f6d  t_dialog.setGeom
+00003710: 6574 7279 2830 2c20 302c 2038 3030 2c20  etry(0, 0, 800, 
+00003720: 3630 3029 0a20 2020 2020 2020 2073 656c  600).        sel
+00003730: 662e 6162 6f75 745f 6469 616c 6f67 2e64  f.about_dialog.d
+00003740: 6f6e 6f72 732e 7365 7453 6f75 7263 6528  onors.setSource(
+00003750: 0a20 2020 2020 2020 2020 2020 2051 7443  .            QtC
+00003760: 6f72 652e 5155 726c 2e66 726f 6d4c 6f63  ore.QUrl.fromLoc
+00003770: 616c 4669 6c65 2857 4f52 4b49 4e47 5f50  alFile(WORKING_P
+00003780: 4154 4820 2b20 222f 6461 7461 2f6e 6f74  ATH + "/data/not
+00003790: 316d 6d2e 6874 6d6c 2229 0a20 2020 2020  1mm.html").     
+000037a0: 2020 2029 0a20 2020 2020 2020 2073 656c     ).        sel
+000037b0: 662e 6162 6f75 745f 6469 616c 6f67 2e6f  f.about_dialog.o
+000037c0: 7065 6e28 290a 0a20 2020 2064 6566 2075  pen()..    def u
+000037d0: 7064 6174 655f 6d61 7374 6572 7363 7028  pdate_masterscp(
+000037e0: 7365 6c66 2920 2d3e 204e 6f6e 653a 0a20  self) -> None:. 
+000037f0: 2020 2020 2020 2022 2222 5570 6461 7465         """Update
+00003800: 2074 6865 204d 4153 5445 522e 5343 5020   the MASTER.SCP 
+00003810: 6669 6c65 2e0a 2020 2020 2020 2020 2d20  file..        - 
+00003820: 5265 7475 726e 7320 5472 7565 2069 6620  Returns True if 
+00003830: 7375 6363 6573 7366 756c 0a20 2020 2020  successful.     
+00003840: 2020 202d 204f 7468 6572 7769 7365 2046     - Otherwise F
+00003850: 616c 7365 0a20 2020 2020 2020 2022 2222  alse.        """
+00003860: 0a20 2020 2020 2020 2077 6974 6820 7265  .        with re
+00003870: 7175 6573 7473 2e53 6573 7369 6f6e 2829  quests.Session()
+00003880: 2061 7320 7365 7373 696f 6e3a 0a20 2020   as session:.   
+00003890: 2020 2020 2020 2020 2074 6865 5f72 6571           the_req
+000038a0: 7565 7374 203d 2073 6573 7369 6f6e 2e67  uest = session.g
+000038b0: 6574 284d 4153 5445 525f 5343 505f 5552  et(MASTER_SCP_UR
+000038c0: 4c29 0a20 2020 2020 2020 2020 2020 2069  L).            i
+000038d0: 6620 7468 655f 7265 7175 6573 742e 7374  f the_request.st
+000038e0: 6174 7573 5f63 6f64 6520 3d3d 2032 3030  atus_code == 200
+000038f0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00003900: 2020 7769 7468 206f 7065 6e28 574f 524b    with open(WORK
+00003910: 494e 475f 5041 5448 202b 2022 2f64 6174  ING_PATH + "/dat
+00003920: 612f 4d41 5354 4552 2e53 4350 222c 2022  a/MASTER.SCP", "
+00003930: 7762 2b22 2920 6173 2066 696c 653a 0a20  wb+") as file:. 
+00003940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003950: 2020 2066 696c 652e 7772 6974 6528 7468     file.write(th
+00003960: 655f 7265 7175 6573 742e 636f 6e74 656e  e_request.conten
+00003970: 7429 0a20 2020 2020 2020 2020 2020 2020  t).             
+00003980: 2020 2073 656c 662e 7368 6f77 5f6d 6573     self.show_mes
+00003990: 7361 6765 5f62 6f78 2822 4d41 5354 4552  sage_box("MASTER
+000039a0: 2e53 4350 2066 696c 6520 7570 6461 7465  .SCP file update
+000039b0: 642e 2229 0a20 2020 2020 2020 2020 2020  d.").           
+000039c0: 2020 2020 2072 6574 7572 6e0a 2020 2020       return.    
+000039d0: 2020 2020 7365 6c66 2e73 686f 775f 6d65      self.show_me
+000039e0: 7373 6167 655f 626f 7828 224d 4153 5445  ssage_box("MASTE
+000039f0: 522e 5343 5020 636f 756c 6420 6e6f 7420  R.SCP could not 
+00003a00: 6265 2075 7064 6174 6564 2e22 290a 0a20  be updated.").. 
+00003a10: 2020 2064 6566 2065 6469 745f 636f 6e66     def edit_conf
+00003a20: 6967 7572 6174 696f 6e5f 7365 7474 696e  iguration_settin
+00003a30: 6773 2873 656c 6629 3a0a 2020 2020 2020  gs(self):.      
+00003a40: 2020 2222 2243 6f6e 6669 6775 7261 7469    """Configurati
+00003a50: 6f6e 2053 6574 7469 6e67 7320 7761 7320  on Settings was 
+00003a60: 636c 6963 6b65 6422 2222 0a20 2020 2020  clicked""".     
+00003a70: 2020 2073 656c 662e 636f 6e66 6967 7572     self.configur
+00003a80: 6174 696f 6e5f 6469 616c 6f67 203d 2053  ation_dialog = S
+00003a90: 6574 7469 6e67 7328 574f 524b 494e 475f  ettings(WORKING_
+00003aa0: 5041 5448 2c20 434f 4e46 4947 5f50 4154  PATH, CONFIG_PAT
+00003ab0: 482c 2073 656c 662e 7072 6566 290a 2020  H, self.pref).  
+00003ac0: 2020 2020 2020 7365 6c66 2e63 6f6e 6669        self.confi
+00003ad0: 6775 7261 7469 6f6e 5f64 6961 6c6f 672e  guration_dialog.
+00003ae0: 7573 6568 616d 6462 5f72 6164 696f 4275  usehamdb_radioBu
+00003af0: 7474 6f6e 2e68 6964 6528 290a 2020 2020  tton.hide().    
+00003b00: 2020 2020 7365 6c66 2e63 6f6e 6669 6775      self.configu
+00003b10: 7261 7469 6f6e 5f64 6961 6c6f 672e 7368  ration_dialog.sh
+00003b20: 6f77 2829 0a20 2020 2020 2020 2073 656c  ow().        sel
+00003b30: 662e 636f 6e66 6967 7572 6174 696f 6e5f  f.configuration_
+00003b40: 6469 616c 6f67 2e61 6363 6570 7465 642e  dialog.accepted.
+00003b50: 636f 6e6e 6563 7428 7365 6c66 2e65 6469  connect(self.edi
+00003b60: 745f 636f 6e66 6967 7572 6174 696f 6e5f  t_configuration_
+00003b70: 7265 7475 726e 290a 0a20 2020 2064 6566  return)..    def
+00003b80: 2065 6469 745f 636f 6e66 6967 7572 6174   edit_configurat
+00003b90: 696f 6e5f 7265 7475 726e 2873 656c 6629  ion_return(self)
+00003ba0: 3a0a 2020 2020 2020 2020 2222 2252 6574  :.        """Ret
+00003bb0: 7572 6e73 2068 6572 6520 7768 656e 2063  urns here when c
+00003bc0: 6f6e 6669 6775 7261 7469 6f6e 2064 6961  onfiguration dia
+00003bd0: 6c6f 6720 636c 6f73 6564 2077 6974 6820  log closed with 
+00003be0: 6f6b 6179 2e22 2222 0a20 2020 2020 2020  okay.""".       
+00003bf0: 2073 656c 662e 636f 6e66 6967 7572 6174   self.configurat
+00003c00: 696f 6e5f 6469 616c 6f67 2e73 6176 655f  ion_dialog.save_
+00003c10: 6368 616e 6765 7328 290a 2020 2020 2020  changes().      
+00003c20: 2020 7365 6c66 2e77 7269 7465 5f70 7265    self.write_pre
+00003c30: 6665 7265 6e63 6528 290a 2020 2020 2020  ference().      
+00003c40: 2020 6c6f 6767 6572 2e64 6562 7567 2822    logger.debug("
+00003c50: 2573 222c 2066 227b 7365 6c66 2e70 7265  %s", f"{self.pre
+00003c60: 667d 2229 0a20 2020 2020 2020 2073 656c  f}").        sel
+00003c70: 662e 7265 6164 7072 6566 6572 656e 6365  f.readpreference
+00003c80: 7328 290a 0a20 2020 2064 6566 206e 6577  s()..    def new
+00003c90: 5f64 6174 6162 6173 6528 7365 6c66 293a  _database(self):
+00003ca0: 0a20 2020 2020 2020 2022 2222 4372 6561  .        """Crea
+00003cb0: 7465 206e 6577 2064 6174 6162 6173 652e  te new database.
+00003cc0: 2222 220a 2020 2020 2020 2020 6669 6c65  """.        file
+00003cd0: 6e61 6d65 203d 2073 656c 662e 6669 6c65  name = self.file
+00003ce0: 7069 636b 6572 2822 6e65 7722 290a 2020  picker("new").  
+00003cf0: 2020 2020 2020 6966 2066 696c 656e 616d        if filenam
+00003d00: 653a 0a20 2020 2020 2020 2020 2020 2069  e:.            i
+00003d10: 6620 6669 6c65 6e61 6d65 5b2d 333a 5d20  f filename[-3:] 
+00003d20: 213d 2022 2e64 6222 3a0a 2020 2020 2020  != ".db":.      
+00003d30: 2020 2020 2020 2020 2020 6669 6c65 6e61            filena
+00003d40: 6d65 202b 3d20 222e 6462 220a 2020 2020  me += ".db".    
+00003d50: 2020 2020 2020 2020 7365 6c66 2e70 7265          self.pre
+00003d60: 665b 2263 7572 7265 6e74 5f64 6174 6162  f["current_datab
+00003d70: 6173 6522 5d20 3d20 6669 6c65 6e61 6d65  ase"] = filename
+00003d80: 2e73 706c 6974 2822 2f22 295b 2d31 3a5d  .split("/")[-1:]
+00003d90: 5b30 5d0a 2020 2020 2020 2020 2020 2020  [0].            
+00003da0: 7365 6c66 2e77 7269 7465 5f70 7265 6665  self.write_prefe
+00003db0: 7265 6e63 6528 290a 2020 2020 2020 2020  rence().        
+00003dc0: 2020 2020 7365 6c66 2e64 626e 616d 6520      self.dbname 
+00003dd0: 3d20 4441 5441 5f50 4154 4820 2b20 222f  = DATA_PATH + "/
+00003de0: 2220 2b20 7365 6c66 2e70 7265 662e 6765  " + self.pref.ge
+00003df0: 7428 2263 7572 7265 6e74 5f64 6174 6162  t("current_datab
+00003e00: 6173 6522 2c20 2268 616d 2e64 6222 290a  ase", "ham.db").
+00003e10: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00003e20: 2e64 6174 6162 6173 6520 3d20 4461 7461  .database = Data
+00003e30: 4261 7365 2873 656c 662e 6462 6e61 6d65  Base(self.dbname
+00003e40: 2c20 574f 524b 494e 475f 5041 5448 290a  , WORKING_PATH).
+00003e50: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00003e60: 2e63 6f6e 7461 6374 203d 2073 656c 662e  .contact = self.
+00003e70: 6461 7461 6261 7365 2e65 6d70 7479 5f63  database.empty_c
+00003e80: 6f6e 7461 6374 0a20 2020 2020 2020 2020  ontact.         
+00003e90: 2020 2073 656c 662e 7374 6174 696f 6e20     self.station 
+00003ea0: 3d20 7365 6c66 2e64 6174 6162 6173 652e  = self.database.
+00003eb0: 6665 7463 685f 7374 6174 696f 6e28 290a  fetch_station().
+00003ec0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+00003ed0: 656c 662e 7374 6174 696f 6e20 6973 204e  elf.station is N
+00003ee0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00003ef0: 2020 2020 2073 656c 662e 7374 6174 696f       self.statio
+00003f00: 6e20 3d20 7b7d 0a20 2020 2020 2020 2020  n = {}.         
+00003f10: 2020 2073 656c 662e 6375 7272 656e 745f     self.current_
+00003f20: 6f70 203d 2073 656c 662e 7374 6174 696f  op = self.statio
+00003f30: 6e2e 6765 7428 2243 616c 6c22 2c20 2222  n.get("Call", ""
+00003f40: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
+00003f50: 6c66 2e6d 616b 655f 6f70 5f64 6972 2829  lf.make_op_dir()
+00003f60: 0a20 2020 2020 2020 2020 2020 2063 6d64  .            cmd
+00003f70: 203d 207b 7d0a 2020 2020 2020 2020 2020   = {}.          
+00003f80: 2020 636d 645b 2263 6d64 225d 203d 2022    cmd["cmd"] = "
+00003f90: 4e45 5744 4222 0a20 2020 2020 2020 2020  NEWDB".         
+00003fa0: 2020 2063 6d64 5b22 7374 6174 696f 6e22     cmd["station"
+00003fb0: 5d20 3d20 706c 6174 666f 726d 2e6e 6f64  ] = platform.nod
+00003fc0: 6528 290a 2020 2020 2020 2020 2020 2020  e().            
+00003fd0: 7365 6c66 2e6d 756c 7469 6361 7374 5f69  self.multicast_i
+00003fe0: 6e74 6572 6661 6365 2e73 656e 645f 6173  nterface.send_as
+00003ff0: 5f6a 736f 6e28 636d 6429 0a20 2020 2020  _json(cmd).     
+00004000: 2020 2020 2020 2073 656c 662e 636c 6561         self.clea
+00004010: 7269 6e70 7574 7328 290a 2020 2020 2020  rinputs().      
+00004020: 2020 2020 2020 7365 6c66 2e65 6469 745f        self.edit_
+00004030: 7374 6174 696f 6e5f 7365 7474 696e 6773  station_settings
+00004040: 2829 0a0a 2020 2020 6465 6620 6f70 656e  ()..    def open
+00004050: 5f64 6174 6162 6173 6528 7365 6c66 293a  _database(self):
+00004060: 0a20 2020 2020 2020 2022 2222 4f70 656e  .        """Open
+00004070: 2065 7869 7374 696e 6720 6461 7461 6261   existing databa
+00004080: 7365 2e22 2222 0a20 2020 2020 2020 2066  se.""".        f
+00004090: 696c 656e 616d 6520 3d20 7365 6c66 2e66  ilename = self.f
+000040a0: 696c 6570 6963 6b65 7228 226f 7065 6e22  ilepicker("open"
+000040b0: 290a 2020 2020 2020 2020 6966 2066 696c  ).        if fil
+000040c0: 656e 616d 653a 0a20 2020 2020 2020 2020  ename:.         
+000040d0: 2020 2073 656c 662e 7072 6566 5b22 6375     self.pref["cu
+000040e0: 7272 656e 745f 6461 7461 6261 7365 225d  rrent_database"]
+000040f0: 203d 2066 696c 656e 616d 652e 7370 6c69   = filename.spli
+00004100: 7428 222f 2229 5b2d 313a 5d5b 305d 0a20  t("/")[-1:][0]. 
+00004110: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00004120: 7772 6974 655f 7072 6566 6572 656e 6365  write_preference
+00004130: 2829 0a20 2020 2020 2020 2020 2020 2073  ().            s
+00004140: 656c 662e 6462 6e61 6d65 203d 2044 4154  elf.dbname = DAT
+00004150: 415f 5041 5448 202b 2022 2f22 202b 2073  A_PATH + "/" + s
+00004160: 656c 662e 7072 6566 2e67 6574 2822 6375  elf.pref.get("cu
+00004170: 7272 656e 745f 6461 7461 6261 7365 222c  rrent_database",
+00004180: 2022 6861 6d2e 6462 2229 0a20 2020 2020   "ham.db").     
+00004190: 2020 2020 2020 2073 656c 662e 6461 7461         self.data
+000041a0: 6261 7365 203d 2044 6174 6142 6173 6528  base = DataBase(
+000041b0: 7365 6c66 2e64 626e 616d 652c 2057 4f52  self.dbname, WOR
+000041c0: 4b49 4e47 5f50 4154 4829 0a20 2020 2020  KING_PATH).     
+000041d0: 2020 2020 2020 2073 656c 662e 636f 6e74         self.cont
+000041e0: 6163 7420 3d20 7365 6c66 2e64 6174 6162  act = self.datab
+000041f0: 6173 652e 656d 7074 795f 636f 6e74 6163  ase.empty_contac
+00004200: 740a 2020 2020 2020 2020 2020 2020 7365  t.            se
+00004210: 6c66 2e73 7461 7469 6f6e 203d 2073 656c  lf.station = sel
+00004220: 662e 6461 7461 6261 7365 2e66 6574 6368  f.database.fetch
+00004230: 5f73 7461 7469 6f6e 2829 0a20 2020 2020  _station().     
+00004240: 2020 2020 2020 2069 6620 7365 6c66 2e73         if self.s
+00004250: 7461 7469 6f6e 2069 7320 4e6f 6e65 3a0a  tation is None:.
+00004260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004270: 7365 6c66 2e73 7461 7469 6f6e 203d 207b  self.station = {
+00004280: 7d0a 2020 2020 2020 2020 2020 2020 6966  }.            if
+00004290: 2073 656c 662e 7374 6174 696f 6e2e 6765   self.station.ge
+000042a0: 7428 2243 616c 6c22 2c20 2222 2920 3d3d  t("Call", "") ==
+000042b0: 2022 223a 0a20 2020 2020 2020 2020 2020   "":.           
+000042c0: 2020 2020 2073 656c 662e 6564 6974 5f73       self.edit_s
+000042d0: 7461 7469 6f6e 5f73 6574 7469 6e67 7328  tation_settings(
+000042e0: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
+000042f0: 6c66 2e63 7572 7265 6e74 5f6f 7020 3d20  lf.current_op = 
+00004300: 7365 6c66 2e73 7461 7469 6f6e 2e67 6574  self.station.get
+00004310: 2822 4361 6c6c 222c 2022 2229 0a20 2020  ("Call", "").   
+00004320: 2020 2020 2020 2020 2073 656c 662e 6d61           self.ma
+00004330: 6b65 5f6f 705f 6469 7228 290a 2020 2020  ke_op_dir().    
+00004340: 2020 2020 2020 2020 636d 6420 3d20 7b7d          cmd = {}
+00004350: 0a20 2020 2020 2020 2020 2020 2063 6d64  .            cmd
+00004360: 5b22 636d 6422 5d20 3d20 224e 4557 4442  ["cmd"] = "NEWDB
+00004370: 220a 2020 2020 2020 2020 2020 2020 636d  ".            cm
+00004380: 645b 2273 7461 7469 6f6e 225d 203d 2070  d["station"] = p
+00004390: 6c61 7466 6f72 6d2e 6e6f 6465 2829 0a20  latform.node(). 
+000043a0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000043b0: 6d75 6c74 6963 6173 745f 696e 7465 7266  multicast_interf
+000043c0: 6163 652e 7365 6e64 5f61 735f 6a73 6f6e  ace.send_as_json
+000043d0: 2863 6d64 290a 2020 2020 2020 2020 2020  (cmd).          
+000043e0: 2020 7365 6c66 2e63 6c65 6172 696e 7075    self.clearinpu
+000043f0: 7473 2829 0a0a 2020 2020 6465 6620 6e65  ts()..    def ne
+00004400: 775f 636f 6e74 6573 7428 7365 6c66 293a  w_contest(self):
+00004410: 0a20 2020 2020 2020 2022 2222 4372 6561  .        """Crea
+00004420: 7465 206e 6577 2063 6f6e 7465 7374 2069  te new contest i
+00004430: 6e20 6578 6973 7469 6e67 2064 6174 6162  n existing datab
+00004440: 6173 652e 2222 220a 0a20 2020 2064 6566  ase."""..    def
+00004450: 206f 7065 6e5f 636f 6e74 6573 7428 7365   open_contest(se
+00004460: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
+00004470: 5377 6974 6368 2074 6f20 6120 6469 6666  Switch to a diff
+00004480: 6572 656e 7420 6578 6973 7469 6e67 2063  erent existing c
+00004490: 6f6e 7465 7374 2069 6e20 6578 6973 7469  ontest in existi
+000044a0: 6e67 2064 6174 6162 6173 652e 2222 220a  ng database.""".
+000044b0: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
+000044c0: 6562 7567 2822 4f70 656e 2043 6f6e 7465  ebug("Open Conte
+000044d0: 7374 2073 656c 6563 7465 6422 290a 2020  st selected").  
+000044e0: 2020 2020 2020 636f 6e74 6573 7473 203d        contests =
+000044f0: 2073 656c 662e 6461 7461 6261 7365 2e66   self.database.f
+00004500: 6574 6368 5f61 6c6c 5f63 6f6e 7465 7374  etch_all_contest
+00004510: 7328 290a 2020 2020 2020 2020 6c6f 6767  s().        logg
+00004520: 6572 2e64 6562 7567 2822 2573 222c 2066  er.debug("%s", f
+00004530: 227b 636f 6e74 6573 7473 7d22 290a 0a20  "{contests}").. 
+00004540: 2020 2020 2020 2069 6620 636f 6e74 6573         if contes
+00004550: 7473 3a0a 2020 2020 2020 2020 2020 2020  ts:.            
+00004560: 7365 6c66 2e63 6f6e 7465 7374 5f64 6961  self.contest_dia
+00004570: 6c6f 6720 3d20 5365 6c65 6374 436f 6e74  log = SelectCont
+00004580: 6573 7428 574f 524b 494e 475f 5041 5448  est(WORKING_PATH
+00004590: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
+000045a0: 6c66 2e63 6f6e 7465 7374 5f64 6961 6c6f  lf.contest_dialo
+000045b0: 672e 636f 6e74 6573 745f 6c69 7374 2e73  g.contest_list.s
+000045c0: 6574 526f 7743 6f75 6e74 2830 290a 2020  etRowCount(0).  
+000045d0: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+000045e0: 6f6e 7465 7374 5f64 6961 6c6f 672e 636f  ontest_dialog.co
+000045f0: 6e74 6573 745f 6c69 7374 2e73 6574 436f  ntest_list.setCo
+00004600: 6c75 6d6e 436f 756e 7428 3429 0a20 2020  lumnCount(4).   
+00004610: 2020 2020 2020 2020 2073 656c 662e 636f           self.co
+00004620: 6e74 6573 745f 6469 616c 6f67 2e63 6f6e  ntest_dialog.con
+00004630: 7465 7374 5f6c 6973 742e 7665 7274 6963  test_list.vertic
+00004640: 616c 4865 6164 6572 2829 2e73 6574 5669  alHeader().setVi
+00004650: 7369 626c 6528 4661 6c73 6529 0a20 2020  sible(False).   
+00004660: 2020 2020 2020 2020 2073 656c 662e 636f           self.co
+00004670: 6e74 6573 745f 6469 616c 6f67 2e63 6f6e  ntest_dialog.con
+00004680: 7465 7374 5f6c 6973 742e 7365 7443 6f6c  test_list.setCol
+00004690: 756d 6e57 6964 7468 2831 2c20 3230 3029  umnWidth(1, 200)
+000046a0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+000046b0: 662e 636f 6e74 6573 745f 6469 616c 6f67  f.contest_dialog
+000046c0: 2e63 6f6e 7465 7374 5f6c 6973 742e 7365  .contest_list.se
+000046d0: 7443 6f6c 756d 6e57 6964 7468 2832 2c20  tColumnWidth(2, 
+000046e0: 3230 3029 0a20 2020 2020 2020 2020 2020  200).           
+000046f0: 2073 656c 662e 636f 6e74 6573 745f 6469   self.contest_di
+00004700: 616c 6f67 2e63 6f6e 7465 7374 5f6c 6973  alog.contest_lis
+00004710: 742e 7365 7448 6f72 697a 6f6e 7461 6c48  t.setHorizontalH
+00004720: 6561 6465 7249 7465 6d28 0a20 2020 2020  eaderItem(.     
+00004730: 2020 2020 2020 2020 2020 2030 2c20 5174             0, Qt
+00004740: 5769 6467 6574 732e 5154 6162 6c65 5769  Widgets.QTableWi
+00004750: 6467 6574 4974 656d 2822 436f 6e74 6573  dgetItem("Contes
+00004760: 7420 4e72 2229 0a20 2020 2020 2020 2020  t Nr").         
+00004770: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+00004780: 2073 656c 662e 636f 6e74 6573 745f 6469   self.contest_di
+00004790: 616c 6f67 2e63 6f6e 7465 7374 5f6c 6973  alog.contest_lis
+000047a0: 742e 7365 7448 6f72 697a 6f6e 7461 6c48  t.setHorizontalH
+000047b0: 6561 6465 7249 7465 6d28 0a20 2020 2020  eaderItem(.     
+000047c0: 2020 2020 2020 2020 2020 2031 2c20 5174             1, Qt
+000047d0: 5769 6467 6574 732e 5154 6162 6c65 5769  Widgets.QTableWi
+000047e0: 6467 6574 4974 656d 2822 436f 6e74 6573  dgetItem("Contes
+000047f0: 7420 4e61 6d65 2229 0a20 2020 2020 2020  t Name").       
+00004800: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+00004810: 2020 2073 656c 662e 636f 6e74 6573 745f     self.contest_
+00004820: 6469 616c 6f67 2e63 6f6e 7465 7374 5f6c  dialog.contest_l
+00004830: 6973 742e 7365 7448 6f72 697a 6f6e 7461  ist.setHorizonta
+00004840: 6c48 6561 6465 7249 7465 6d28 0a20 2020  lHeaderItem(.   
+00004850: 2020 2020 2020 2020 2020 2020 2032 2c20               2, 
+00004860: 5174 5769 6467 6574 732e 5154 6162 6c65  QtWidgets.QTable
+00004870: 5769 6467 6574 4974 656d 2822 436f 6e74  WidgetItem("Cont
+00004880: 6573 7420 5374 6172 7422 290a 2020 2020  est Start").    
+00004890: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+000048a0: 2020 2020 2020 7365 6c66 2e63 6f6e 7465        self.conte
+000048b0: 7374 5f64 6961 6c6f 672e 636f 6e74 6573  st_dialog.contes
+000048c0: 745f 6c69 7374 2e73 6574 486f 7269 7a6f  t_list.setHorizo
+000048d0: 6e74 616c 4865 6164 6572 4974 656d 280a  ntalHeaderItem(.
+000048e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000048f0: 332c 2051 7457 6964 6765 7473 2e51 5461  3, QtWidgets.QTa
+00004900: 626c 6557 6964 6765 7449 7465 6d28 224e  bleWidgetItem("N
+00004910: 6f74 2055 4973 6564 2229 0a20 2020 2020  ot UIsed").     
+00004920: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00004930: 2020 2020 2073 656c 662e 636f 6e74 6573       self.contes
+00004940: 745f 6469 616c 6f67 2e63 6f6e 7465 7374  t_dialog.contest
+00004950: 5f6c 6973 742e 7365 7443 6f6c 756d 6e48  _list.setColumnH
+00004960: 6964 6465 6e28 302c 2054 7275 6529 0a20  idden(0, True). 
+00004970: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00004980: 636f 6e74 6573 745f 6469 616c 6f67 2e63  contest_dialog.c
+00004990: 6f6e 7465 7374 5f6c 6973 742e 7365 7443  ontest_list.setC
+000049a0: 6f6c 756d 6e48 6964 6465 6e28 332c 2054  olumnHidden(3, T
+000049b0: 7275 6529 0a20 2020 2020 2020 2020 2020  rue).           
+000049c0: 2073 656c 662e 636f 6e74 6573 745f 6469   self.contest_di
+000049d0: 616c 6f67 2e61 6363 6570 7465 642e 636f  alog.accepted.co
+000049e0: 6e6e 6563 7428 7365 6c66 2e6f 7065 6e5f  nnect(self.open_
+000049f0: 636f 6e74 6573 745f 7265 7475 726e 290a  contest_return).
+00004a00: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00004a10: 636f 6e74 6573 7420 696e 2063 6f6e 7465  contest in conte
+00004a20: 7374 733a 0a20 2020 2020 2020 2020 2020  sts:.           
+00004a30: 2020 2020 206e 756d 6265 725f 6f66 5f72       number_of_r
+00004a40: 6f77 7320 3d20 7365 6c66 2e63 6f6e 7465  ows = self.conte
+00004a50: 7374 5f64 6961 6c6f 672e 636f 6e74 6573  st_dialog.contes
+00004a60: 745f 6c69 7374 2e72 6f77 436f 756e 7428  t_list.rowCount(
+00004a70: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00004a80: 2020 7365 6c66 2e63 6f6e 7465 7374 5f64    self.contest_d
+00004a90: 6961 6c6f 672e 636f 6e74 6573 745f 6c69  ialog.contest_li
+00004aa0: 7374 2e69 6e73 6572 7452 6f77 286e 756d  st.insertRow(num
+00004ab0: 6265 725f 6f66 5f72 6f77 7329 0a20 2020  ber_of_rows).   
+00004ac0: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
+00004ad0: 7465 7374 5f69 6420 3d20 7374 7228 636f  test_id = str(co
+00004ae0: 6e74 6573 742e 6765 7428 2243 6f6e 7465  ntest.get("Conte
+00004af0: 7374 4944 222c 2031 2929 0a20 2020 2020  stID", 1)).     
+00004b00: 2020 2020 2020 2020 2020 2063 6f6e 7465             conte
+00004b10: 7374 5f6e 616d 6520 3d20 636f 6e74 6573  st_name = contes
+00004b20: 742e 6765 7428 2243 6f6e 7465 7374 4e61  t.get("ContestNa
+00004b30: 6d65 222c 2031 290a 2020 2020 2020 2020  me", 1).        
+00004b40: 2020 2020 2020 2020 7374 6172 745f 6461          start_da
+00004b50: 7465 203d 2063 6f6e 7465 7374 2e67 6574  te = contest.get
+00004b60: 2822 5374 6172 7444 6174 6522 2c20 3129  ("StartDate", 1)
+00004b70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004b80: 2073 656c 662e 636f 6e74 6573 745f 6469   self.contest_di
+00004b90: 616c 6f67 2e63 6f6e 7465 7374 5f6c 6973  alog.contest_lis
+00004ba0: 742e 7365 7449 7465 6d28 0a20 2020 2020  t.setItem(.     
+00004bb0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+00004bc0: 756d 6265 725f 6f66 5f72 6f77 732c 2030  umber_of_rows, 0
+00004bd0: 2c20 5174 5769 6467 6574 732e 5154 6162  , QtWidgets.QTab
+00004be0: 6c65 5769 6467 6574 4974 656d 2863 6f6e  leWidgetItem(con
+00004bf0: 7465 7374 5f69 6429 0a20 2020 2020 2020  test_id).       
+00004c00: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+00004c10: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00004c20: 636f 6e74 6573 745f 6469 616c 6f67 2e63  contest_dialog.c
+00004c30: 6f6e 7465 7374 5f6c 6973 742e 7365 7449  ontest_list.setI
+00004c40: 7465 6d28 0a20 2020 2020 2020 2020 2020  tem(.           
+00004c50: 2020 2020 2020 2020 206e 756d 6265 725f           number_
+00004c60: 6f66 5f72 6f77 732c 2031 2c20 5174 5769  of_rows, 1, QtWi
+00004c70: 6467 6574 732e 5154 6162 6c65 5769 6467  dgets.QTableWidg
+00004c80: 6574 4974 656d 2863 6f6e 7465 7374 5f6e  etItem(contest_n
+00004c90: 616d 6529 0a20 2020 2020 2020 2020 2020  ame).           
+00004ca0: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+00004cb0: 2020 2020 2020 2073 656c 662e 636f 6e74         self.cont
+00004cc0: 6573 745f 6469 616c 6f67 2e63 6f6e 7465  est_dialog.conte
+00004cd0: 7374 5f6c 6973 742e 7365 7449 7465 6d28  st_list.setItem(
+00004ce0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004cf0: 2020 2020 206e 756d 6265 725f 6f66 5f72       number_of_r
+00004d00: 6f77 732c 2032 2c20 5174 5769 6467 6574  ows, 2, QtWidget
+00004d10: 732e 5154 6162 6c65 5769 6467 6574 4974  s.QTableWidgetIt
+00004d20: 656d 2873 7461 7274 5f64 6174 6529 0a20  em(start_date). 
+00004d30: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00004d40: 0a20 2020 2020 2020 2073 656c 662e 636f  .        self.co
+00004d50: 6e74 6573 745f 6469 616c 6f67 2e73 686f  ntest_dialog.sho
+00004d60: 7728 290a 0a20 2020 2064 6566 206f 7065  w()..    def ope
+00004d70: 6e5f 636f 6e74 6573 745f 7265 7475 726e  n_contest_return
+00004d80: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00004d90: 2222 2243 616c 6c65 6420 6279 206f 7065  """Called by ope
+00004da0: 6e5f 636f 6e74 6573 7422 2222 0a20 2020  n_contest""".   
+00004db0: 2020 2020 2073 656c 6563 7465 645f 726f       selected_ro
+00004dc0: 7720 3d20 7365 6c66 2e63 6f6e 7465 7374  w = self.contest
+00004dd0: 5f64 6961 6c6f 672e 636f 6e74 6573 745f  _dialog.contest_
+00004de0: 6c69 7374 2e63 7572 7265 6e74 526f 7728  list.currentRow(
+00004df0: 290a 2020 2020 2020 2020 636f 6e74 6573  ).        contes
+00004e00: 7420 3d20 7365 6c66 2e63 6f6e 7465 7374  t = self.contest
+00004e10: 5f64 6961 6c6f 672e 636f 6e74 6573 745f  _dialog.contest_
+00004e20: 6c69 7374 2e69 7465 6d28 7365 6c65 6374  list.item(select
+00004e30: 6564 5f72 6f77 2c20 3029 2e74 6578 7428  ed_row, 0).text(
+00004e40: 290a 2020 2020 2020 2020 7365 6c66 2e70  ).        self.p
+00004e50: 7265 665b 2263 6f6e 7465 7374 225d 203d  ref["contest"] =
+00004e60: 2063 6f6e 7465 7374 0a20 2020 2020 2020   contest.       
+00004e70: 2073 656c 662e 7772 6974 655f 7072 6566   self.write_pref
+00004e80: 6572 656e 6365 2829 0a20 2020 2020 2020  erence().       
+00004e90: 206c 6f67 6765 722e 6465 6275 6728 2253   logger.debug("S
+00004ea0: 656c 6563 7465 6420 636f 6e74 6573 743a  elected contest:
+00004eb0: 2025 7322 2c20 6622 7b63 6f6e 7465 7374   %s", f"{contest
+00004ec0: 7d22 290a 2020 2020 2020 2020 7365 6c66  }").        self
+00004ed0: 2e6c 6f61 645f 636f 6e74 6573 7428 290a  .load_contest().
+00004ee0: 0a20 2020 2064 6566 2072 6566 696c 6c5f  .    def refill_
+00004ef0: 6472 6f70 646f 776e 2873 656c 662c 2074  dropdown(self, t
+00004f00: 6172 6765 742c 2073 6f75 7263 6529 3a0a  arget, source):.
+00004f10: 2020 2020 2020 2020 2222 2252 6566 696c          """Refil
+00004f20: 6c20 5143 6f6d 626f 626f 7820 7769 6467  l QCombobox widg
+00004f30: 6574 2077 6974 6820 7661 6c75 652e 2222  et with value.""
+00004f40: 220a 2020 2020 2020 2020 696e 6465 7820  ".        index 
+00004f50: 3d20 7461 7267 6574 2e66 696e 6454 6578  = target.findTex
+00004f60: 7428 736f 7572 6365 290a 2020 2020 2020  t(source).      
+00004f70: 2020 7461 7267 6574 2e73 6574 4375 7272    target.setCurr
+00004f80: 656e 7449 6e64 6578 2869 6e64 6578 290a  entIndex(index).
+00004f90: 0a20 2020 2064 6566 2065 6469 745f 636f  .    def edit_co
+00004fa0: 6e74 6573 7428 7365 6c66 293a 0a20 2020  ntest(self):.   
+00004fb0: 2020 2020 2022 2222 4564 6974 2074 6865       """Edit the
+00004fc0: 2063 7572 7265 6e74 2063 6f6e 7465 7374   current contest
+00004fd0: 2222 220a 2020 2020 2020 2020 6c6f 6767  """.        logg
+00004fe0: 6572 2e64 6562 7567 2822 4564 6974 2063  er.debug("Edit c
+00004ff0: 6f6e 7465 7374 2044 6961 6c6f 6722 290a  ontest Dialog").
+00005000: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00005010: 636f 6e74 6573 7420 6973 204e 6f6e 653a  contest is None:
+00005020: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00005030: 662e 7368 6f77 5f6d 6573 7361 6765 5f62  f.show_message_b
+00005040: 6f78 2822 596f 7520 6861 7665 206e 6f20  ox("You have no 
+00005050: 636f 6e74 6573 7420 6465 6669 6e65 642e  contest defined.
+00005060: 2229 0a20 2020 2020 2020 2020 2020 2072  ").            r
+00005070: 6574 7572 6e0a 2020 2020 2020 2020 6966  eturn.        if
+00005080: 2073 656c 662e 636f 6e74 6573 745f 7365   self.contest_se
+00005090: 7474 696e 6773 2069 7320 4e6f 6e65 3a0a  ttings is None:.
+000050a0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+000050b0: 726e 0a20 2020 2020 2020 2073 656c 662e  rn.        self.
+000050c0: 636f 6e74 6573 745f 6469 616c 6f67 203d  contest_dialog =
+000050d0: 204e 6577 436f 6e74 6573 7428 574f 524b   NewContest(WORK
+000050e0: 494e 475f 5041 5448 290a 2020 2020 2020  ING_PATH).      
+000050f0: 2020 7365 6c66 2e63 6f6e 7465 7374 5f64    self.contest_d
+00005100: 6961 6c6f 672e 7365 7457 696e 646f 7754  ialog.setWindowT
+00005110: 6974 6c65 2822 4564 6974 2043 6f6e 7465  itle("Edit Conte
+00005120: 7374 2229 0a20 2020 2020 2020 2073 656c  st").        sel
+00005130: 662e 636f 6e74 6573 745f 6469 616c 6f67  f.contest_dialog
+00005140: 2e74 6974 6c65 2e73 6574 5465 7874 2822  .title.setText("
+00005150: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
+00005160: 636f 6e74 6573 745f 6469 616c 6f67 2e61  contest_dialog.a
+00005170: 6363 6570 7465 642e 636f 6e6e 6563 7428  ccepted.connect(
+00005180: 7365 6c66 2e73 6176 655f 6564 6974 6564  self.save_edited
+00005190: 5f63 6f6e 7465 7374 290a 2020 2020 2020  _contest).      
+000051a0: 2020 7661 6c75 6520 3d20 7365 6c66 2e63    value = self.c
+000051b0: 6f6e 7465 7374 5f73 6574 7469 6e67 732e  ontest_settings.
+000051c0: 6765 7428 2243 6f6e 7465 7374 4e61 6d65  get("ContestName
+000051d0: 2229 2e75 7070 6572 2829 2e72 6570 6c61  ").upper().repla
+000051e0: 6365 2822 5f22 2c20 2220 2229 0a20 2020  ce("_", " ").   
+000051f0: 2020 2020 2069 6620 7661 6c75 6520 3d3d       if value ==
+00005200: 2022 4745 4e45 5241 4c20 4c4f 4747 494e   "GENERAL LOGGIN
+00005210: 4722 3a0a 2020 2020 2020 2020 2020 2020  G":.            
+00005220: 7661 6c75 6520 3d20 2247 656e 6572 616c  value = "General
+00005230: 204c 6f67 6769 6e67 220a 2020 2020 2020   Logging".      
+00005240: 2020 7365 6c66 2e72 6566 696c 6c5f 6472    self.refill_dr
+00005250: 6f70 646f 776e 2873 656c 662e 636f 6e74  opdown(self.cont
+00005260: 6573 745f 6469 616c 6f67 2e63 6f6e 7465  est_dialog.conte
+00005270: 7374 2c20 7661 6c75 6529 0a20 2020 2020  st, value).     
+00005280: 2020 2076 616c 7565 203d 2073 656c 662e     value = self.
+00005290: 636f 6e74 6573 745f 7365 7474 696e 6773  contest_settings
+000052a0: 2e67 6574 2822 4f70 6572 6174 6f72 4361  .get("OperatorCa
+000052b0: 7465 676f 7279 2229 0a20 2020 2020 2020  tegory").       
+000052c0: 2073 656c 662e 7265 6669 6c6c 5f64 726f   self.refill_dro
+000052d0: 7064 6f77 6e28 7365 6c66 2e63 6f6e 7465  pdown(self.conte
+000052e0: 7374 5f64 6961 6c6f 672e 6f70 6572 6174  st_dialog.operat
+000052f0: 6f72 5f63 6c61 7373 2c20 7661 6c75 6529  or_class, value)
+00005300: 0a20 2020 2020 2020 2076 616c 7565 203d  .        value =
+00005310: 2073 656c 662e 636f 6e74 6573 745f 7365   self.contest_se
+00005320: 7474 696e 6773 2e67 6574 2822 4261 6e64  ttings.get("Band
+00005330: 4361 7465 676f 7279 2229 0a20 2020 2020  Category").     
+00005340: 2020 2073 656c 662e 7265 6669 6c6c 5f64     self.refill_d
+00005350: 726f 7064 6f77 6e28 7365 6c66 2e63 6f6e  ropdown(self.con
+00005360: 7465 7374 5f64 6961 6c6f 672e 6261 6e64  test_dialog.band
+00005370: 2c20 7661 6c75 6529 0a20 2020 2020 2020  , value).       
+00005380: 2076 616c 7565 203d 2073 656c 662e 636f   value = self.co
+00005390: 6e74 6573 745f 7365 7474 696e 6773 2e67  ntest_settings.g
+000053a0: 6574 2822 506f 7765 7243 6174 6567 6f72  et("PowerCategor
+000053b0: 7922 290a 2020 2020 2020 2020 7365 6c66  y").        self
+000053c0: 2e72 6566 696c 6c5f 6472 6f70 646f 776e  .refill_dropdown
+000053d0: 2873 656c 662e 636f 6e74 6573 745f 6469  (self.contest_di
+000053e0: 616c 6f67 2e70 6f77 6572 2c20 7661 6c75  alog.power, valu
+000053f0: 6529 0a20 2020 2020 2020 2076 616c 7565  e).        value
+00005400: 203d 2073 656c 662e 636f 6e74 6573 745f   = self.contest_
+00005410: 7365 7474 696e 6773 2e67 6574 2822 4d6f  settings.get("Mo
+00005420: 6465 4361 7465 676f 7279 2229 0a20 2020  deCategory").   
+00005430: 2020 2020 2073 656c 662e 7265 6669 6c6c       self.refill
+00005440: 5f64 726f 7064 6f77 6e28 7365 6c66 2e63  _dropdown(self.c
+00005450: 6f6e 7465 7374 5f64 6961 6c6f 672e 6d6f  ontest_dialog.mo
+00005460: 6465 2c20 7661 6c75 6529 0a20 2020 2020  de, value).     
+00005470: 2020 2076 616c 7565 203d 2073 656c 662e     value = self.
+00005480: 636f 6e74 6573 745f 7365 7474 696e 6773  contest_settings
+00005490: 2e67 6574 2822 4f76 6572 6c61 7943 6174  .get("OverlayCat
+000054a0: 6567 6f72 7922 290a 2020 2020 2020 2020  egory").        
+000054b0: 7365 6c66 2e72 6566 696c 6c5f 6472 6f70  self.refill_drop
+000054c0: 646f 776e 2873 656c 662e 636f 6e74 6573  down(self.contes
+000054d0: 745f 6469 616c 6f67 2e6f 7665 726c 6179  t_dialog.overlay
+000054e0: 2c20 7661 6c75 6529 0a20 2020 2020 2020  , value).       
+000054f0: 2073 656c 662e 636f 6e74 6573 745f 6469   self.contest_di
+00005500: 616c 6f67 2e6f 7065 7261 746f 7273 2e73  alog.operators.s
+00005510: 6574 5465 7874 2873 656c 662e 636f 6e74  etText(self.cont
+00005520: 6573 745f 7365 7474 696e 6773 2e67 6574  est_settings.get
+00005530: 2822 4f70 6572 6174 6f72 7322 2929 0a20  ("Operators")). 
+00005540: 2020 2020 2020 2073 656c 662e 636f 6e74         self.cont
+00005550: 6573 745f 6469 616c 6f67 2e73 6f61 7062  est_dialog.soapb
+00005560: 6f78 2e73 6574 506c 6169 6e54 6578 7428  ox.setPlainText(
+00005570: 7365 6c66 2e63 6f6e 7465 7374 5f73 6574  self.contest_set
+00005580: 7469 6e67 732e 6765 7428 2253 6f61 7062  tings.get("Soapb
+00005590: 6f78 2229 290a 2020 2020 2020 2020 7365  ox")).        se
+000055a0: 6c66 2e63 6f6e 7465 7374 5f64 6961 6c6f  lf.contest_dialo
+000055b0: 672e 6578 6368 616e 6765 2e73 6574 5465  g.exchange.setTe
+000055c0: 7874 2873 656c 662e 636f 6e74 6573 745f  xt(self.contest_
+000055d0: 7365 7474 696e 6773 2e67 6574 2822 5365  settings.get("Se
+000055e0: 6e74 4578 6368 616e 6765 2229 290a 2020  ntExchange")).  
+000055f0: 2020 2020 2020 7661 6c75 6520 3d20 7365        value = se
+00005600: 6c66 2e63 6f6e 7465 7374 5f73 6574 7469  lf.contest_setti
+00005610: 6e67 732e 6765 7428 2253 7461 7469 6f6e  ngs.get("Station
+00005620: 4361 7465 676f 7279 2229 0a20 2020 2020  Category").     
+00005630: 2020 2073 656c 662e 7265 6669 6c6c 5f64     self.refill_d
+00005640: 726f 7064 6f77 6e28 7365 6c66 2e63 6f6e  ropdown(self.con
+00005650: 7465 7374 5f64 6961 6c6f 672e 7374 6174  test_dialog.stat
+00005660: 696f 6e2c 2076 616c 7565 290a 2020 2020  ion, value).    
+00005670: 2020 2020 7661 6c75 6520 3d20 7365 6c66      value = self
+00005680: 2e63 6f6e 7465 7374 5f73 6574 7469 6e67  .contest_setting
+00005690: 732e 6765 7428 2241 7373 6973 7465 6443  s.get("AssistedC
+000056a0: 6174 6567 6f72 7922 290a 2020 2020 2020  ategory").      
+000056b0: 2020 7365 6c66 2e72 6566 696c 6c5f 6472    self.refill_dr
+000056c0: 6f70 646f 776e 2873 656c 662e 636f 6e74  opdown(self.cont
+000056d0: 6573 745f 6469 616c 6f67 2e61 7373 6973  est_dialog.assis
+000056e0: 7465 642c 2076 616c 7565 290a 2020 2020  ted, value).    
+000056f0: 2020 2020 7661 6c75 6520 3d20 7365 6c66      value = self
+00005700: 2e63 6f6e 7465 7374 5f73 6574 7469 6e67  .contest_setting
+00005710: 732e 6765 7428 2254 7261 6e73 6d69 7474  s.get("Transmitt
+00005720: 6572 4361 7465 676f 7279 2229 0a20 2020  erCategory").   
+00005730: 2020 2020 2073 656c 662e 7265 6669 6c6c       self.refill
+00005740: 5f64 726f 7064 6f77 6e28 7365 6c66 2e63  _dropdown(self.c
+00005750: 6f6e 7465 7374 5f64 6961 6c6f 672e 7472  ontest_dialog.tr
+00005760: 616e 736d 6974 7465 722c 2076 616c 7565  ansmitter, value
+00005770: 290a 2020 2020 2020 2020 7661 6c75 6520  ).        value 
+00005780: 3d20 7365 6c66 2e63 6f6e 7465 7374 5f73  = self.contest_s
+00005790: 6574 7469 6e67 732e 6765 7428 2253 7461  ettings.get("Sta
+000057a0: 7274 4461 7465 2229 0a20 2020 2020 2020  rtDate").       
+000057b0: 2074 6865 5f64 6174 652c 2074 6865 5f74   the_date, the_t
+000057c0: 696d 6520 3d20 7661 6c75 652e 7370 6c69  ime = value.spli
+000057d0: 7428 290a 2020 2020 2020 2020 7365 6c66  t().        self
+000057e0: 2e63 6f6e 7465 7374 5f64 6961 6c6f 672e  .contest_dialog.
+000057f0: 6461 7465 5469 6d65 4564 6974 2e73 6574  dateTimeEdit.set
+00005800: 4461 7465 280a 2020 2020 2020 2020 2020  Date(.          
+00005810: 2020 5174 436f 7265 2e51 4461 7465 2e66    QtCore.QDate.f
+00005820: 726f 6d53 7472 696e 6728 7468 655f 6461  romString(the_da
+00005830: 7465 2c20 2279 7979 792d 4d4d 2d64 6422  te, "yyyy-MM-dd"
+00005840: 290a 2020 2020 2020 2020 290a 2020 2020  ).        ).    
+00005850: 2020 2020 7365 6c66 2e63 6f6e 7465 7374      self.contest
+00005860: 5f64 6961 6c6f 672e 6461 7465 5469 6d65  _dialog.dateTime
+00005870: 4564 6974 2e73 6574 4361 6c65 6e64 6172  Edit.setCalendar
+00005880: 506f 7075 7028 5472 7565 290a 2020 2020  Popup(True).    
+00005890: 2020 2020 7365 6c66 2e63 6f6e 7465 7374      self.contest
+000058a0: 5f64 6961 6c6f 672e 6461 7465 5469 6d65  _dialog.dateTime
+000058b0: 4564 6974 2e73 6574 5469 6d65 280a 2020  Edit.setTime(.  
+000058c0: 2020 2020 2020 2020 2020 5174 436f 7265            QtCore
+000058d0: 2e51 5469 6d65 2e66 726f 6d53 7472 696e  .QTime.fromStrin
+000058e0: 6728 7468 655f 7469 6d65 2c20 2268 683a  g(the_time, "hh:
+000058f0: 6d6d 3a73 7322 290a 2020 2020 2020 2020  mm:ss").        
+00005900: 290a 2020 2020 2020 2020 7365 6c66 2e63  ).        self.c
+00005910: 6f6e 7465 7374 5f64 6961 6c6f 672e 6f70  ontest_dialog.op
+00005920: 656e 2829 0a0a 2020 2020 6465 6620 7361  en()..    def sa
+00005930: 7665 5f65 6469 7465 645f 636f 6e74 6573  ve_edited_contes
+00005940: 7428 7365 6c66 293a 0a20 2020 2020 2020  t(self):.       
+00005950: 2022 2222 5361 7665 2074 6865 2065 6469   """Save the edi
+00005960: 7465 6420 636f 6e74 6573 7422 2222 0a20  ted contest""". 
+00005970: 2020 2020 2020 2063 6f6e 7465 7374 203d         contest =
+00005980: 207b 7d0a 2020 2020 2020 2020 636f 6e74   {}.        cont
+00005990: 6573 745b 2243 6f6e 7465 7374 4e61 6d65  est["ContestName
+000059a0: 225d 203d 2028 0a20 2020 2020 2020 2020  "] = (.         
+000059b0: 2020 2073 656c 662e 636f 6e74 6573 745f     self.contest_
+000059c0: 6469 616c 6f67 2e63 6f6e 7465 7374 2e63  dialog.contest.c
+000059d0: 7572 7265 6e74 5465 7874 2829 2e6c 6f77  urrentText().low
+000059e0: 6572 2829 2e72 6570 6c61 6365 2822 2022  er().replace(" "
+000059f0: 2c20 225f 2229 0a20 2020 2020 2020 2029  , "_").        )
+00005a00: 0a20 2020 2020 2020 2063 6f6e 7465 7374  .        contest
+00005a10: 5b22 5374 6172 7444 6174 6522 5d20 3d20  ["StartDate"] = 
+00005a20: 7365 6c66 2e63 6f6e 7465 7374 5f64 6961  self.contest_dia
+00005a30: 6c6f 672e 6461 7465 5469 6d65 4564 6974  log.dateTimeEdit
+00005a40: 2e64 6174 6554 696d 6528 292e 746f 5374  .dateTime().toSt
+00005a50: 7269 6e67 280a 2020 2020 2020 2020 2020  ring(.          
+00005a60: 2020 2279 7979 792d 4d4d 2d64 6420 6868    "yyyy-MM-dd hh
+00005a70: 3a6d 6d3a 7373 220a 2020 2020 2020 2020  :mm:ss".        
+00005a80: 290a 2020 2020 2020 2020 636f 6e74 6573  ).        contes
+00005a90: 745b 224f 7065 7261 746f 7243 6174 6567  t["OperatorCateg
+00005aa0: 6f72 7922 5d20 3d20 7365 6c66 2e63 6f6e  ory"] = self.con
+00005ab0: 7465 7374 5f64 6961 6c6f 672e 6f70 6572  test_dialog.oper
+00005ac0: 6174 6f72 5f63 6c61 7373 2e63 7572 7265  ator_class.curre
 00005ad0: 6e74 5465 7874 2829 0a20 2020 2020 2020  ntText().       
-00005ae0: 2063 6f6e 7465 7374 5b22 506f 7765 7243   contest["PowerC
-00005af0: 6174 6567 6f72 7922 5d20 3d20 7365 6c66  ategory"] = self
-00005b00: 2e63 6f6e 7465 7374 5f64 6961 6c6f 672e  .contest_dialog.
-00005b10: 706f 7765 722e 6375 7272 656e 7454 6578  power.currentTex
-00005b20: 7428 290a 2020 2020 2020 2020 636f 6e74  t().        cont
-00005b30: 6573 745b 224d 6f64 6543 6174 6567 6f72  est["ModeCategor
-00005b40: 7922 5d20 3d20 7365 6c66 2e63 6f6e 7465  y"] = self.conte
-00005b50: 7374 5f64 6961 6c6f 672e 6d6f 6465 2e63  st_dialog.mode.c
+00005ae0: 2063 6f6e 7465 7374 5b22 4261 6e64 4361   contest["BandCa
+00005af0: 7465 676f 7279 225d 203d 2073 656c 662e  tegory"] = self.
+00005b00: 636f 6e74 6573 745f 6469 616c 6f67 2e62  contest_dialog.b
+00005b10: 616e 642e 6375 7272 656e 7454 6578 7428  and.currentText(
+00005b20: 290a 2020 2020 2020 2020 636f 6e74 6573  ).        contes
+00005b30: 745b 2250 6f77 6572 4361 7465 676f 7279  t["PowerCategory
+00005b40: 225d 203d 2073 656c 662e 636f 6e74 6573  "] = self.contes
+00005b50: 745f 6469 616c 6f67 2e70 6f77 6572 2e63  t_dialog.power.c
 00005b60: 7572 7265 6e74 5465 7874 2829 0a20 2020  urrentText().   
-00005b70: 2020 2020 2063 6f6e 7465 7374 5b22 4f76       contest["Ov
-00005b80: 6572 6c61 7943 6174 6567 6f72 7922 5d20  erlayCategory"] 
-00005b90: 3d20 7365 6c66 2e63 6f6e 7465 7374 5f64  = self.contest_d
-00005ba0: 6961 6c6f 672e 6f76 6572 6c61 792e 6375  ialog.overlay.cu
-00005bb0: 7272 656e 7454 6578 7428 290a 2020 2020  rrentText().    
-00005bc0: 2020 2020 636f 6e74 6573 745b 224f 7065      contest["Ope
-00005bd0: 7261 746f 7273 225d 203d 2073 656c 662e  rators"] = self.
+00005b70: 2020 2020 2063 6f6e 7465 7374 5b22 4d6f       contest["Mo
+00005b80: 6465 4361 7465 676f 7279 225d 203d 2073  deCategory"] = s
+00005b90: 656c 662e 636f 6e74 6573 745f 6469 616c  elf.contest_dial
+00005ba0: 6f67 2e6d 6f64 652e 6375 7272 656e 7454  og.mode.currentT
+00005bb0: 6578 7428 290a 2020 2020 2020 2020 636f  ext().        co
+00005bc0: 6e74 6573 745b 224f 7665 726c 6179 4361  ntest["OverlayCa
+00005bd0: 7465 676f 7279 225d 203d 2073 656c 662e  tegory"] = self.
 00005be0: 636f 6e74 6573 745f 6469 616c 6f67 2e6f  contest_dialog.o
-00005bf0: 7065 7261 746f 7273 2e74 6578 7428 290a  perators.text().
-00005c00: 2020 2020 2020 2020 636f 6e74 6573 745b          contest[
-00005c10: 2253 6f61 7062 6f78 225d 203d 2073 656c  "Soapbox"] = sel
-00005c20: 662e 636f 6e74 6573 745f 6469 616c 6f67  f.contest_dialog
-00005c30: 2e73 6f61 7062 6f78 2e74 6f50 6c61 696e  .soapbox.toPlain
-00005c40: 5465 7874 2829 0a20 2020 2020 2020 2063  Text().        c
-00005c50: 6f6e 7465 7374 5b22 5365 6e74 4578 6368  ontest["SentExch
-00005c60: 616e 6765 225d 203d 2073 656c 662e 636f  ange"] = self.co
-00005c70: 6e74 6573 745f 6469 616c 6f67 2e65 7863  ntest_dialog.exc
-00005c80: 6861 6e67 652e 7465 7874 2829 0a20 2020  hange.text().   
-00005c90: 2020 2020 2063 6f6e 7465 7374 5b22 436f       contest["Co
-00005ca0: 6e74 6573 744e 5222 5d20 3d20 7365 6c66  ntestNR"] = self
-00005cb0: 2e70 7265 662e 6765 7428 2263 6f6e 7465  .pref.get("conte
-00005cc0: 7374 222c 2031 290a 2020 2020 2020 2020  st", 1).        
-00005cd0: 636f 6e74 6573 745b 2253 7461 7469 6f6e  contest["Station
-00005ce0: 4361 7465 676f 7279 225d 203d 2073 656c  Category"] = sel
-00005cf0: 662e 636f 6e74 6573 745f 6469 616c 6f67  f.contest_dialog
-00005d00: 2e73 7461 7469 6f6e 2e63 7572 7265 6e74  .station.current
-00005d10: 5465 7874 2829 0a20 2020 2020 2020 2063  Text().        c
-00005d20: 6f6e 7465 7374 5b22 4173 7369 7374 6564  ontest["Assisted
-00005d30: 4361 7465 676f 7279 225d 203d 2073 656c  Category"] = sel
-00005d40: 662e 636f 6e74 6573 745f 6469 616c 6f67  f.contest_dialog
-00005d50: 2e61 7373 6973 7465 642e 6375 7272 656e  .assisted.curren
-00005d60: 7454 6578 7428 290a 2020 2020 2020 2020  tText().        
-00005d70: 636f 6e74 6573 745b 2254 7261 6e73 6d69  contest["Transmi
-00005d80: 7474 6572 4361 7465 676f 7279 225d 203d  tterCategory"] =
-00005d90: 2073 656c 662e 636f 6e74 6573 745f 6469   self.contest_di
-00005da0: 616c 6f67 2e74 7261 6e73 6d69 7474 6572  alog.transmitter
-00005db0: 2e63 7572 7265 6e74 5465 7874 2829 0a0a  .currentText()..
-00005dc0: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
-00005dd0: 6562 7567 2822 2573 222c 2066 227b 636f  ebug("%s", f"{co
-00005de0: 6e74 6573 747d 2229 0a20 2020 2020 2020  ntest}").       
-00005df0: 2073 656c 662e 6461 7461 6261 7365 2e75   self.database.u
-00005e00: 7064 6174 655f 636f 6e74 6573 7428 636f  pdate_contest(co
-00005e10: 6e74 6573 7429 0a20 2020 2020 2020 2073  ntest).        s
-00005e20: 656c 662e 7772 6974 655f 7072 6566 6572  elf.write_prefer
-00005e30: 656e 6365 2829 0a20 2020 2020 2020 2073  ence().        s
-00005e40: 656c 662e 6c6f 6164 5f63 6f6e 7465 7374  elf.load_contest
-00005e50: 2829 0a0a 2020 2020 6465 6620 6c6f 6164  ()..    def load
-00005e60: 5f63 6f6e 7465 7374 2873 656c 6629 3a0a  _contest(self):.
-00005e70: 2020 2020 2020 2020 2222 226c 6f61 6420          """load 
-00005e80: 6120 636f 6e74 6573 7422 2222 0a20 2020  a contest""".   
-00005e90: 2020 2020 2069 6620 7365 6c66 2e70 7265       if self.pre
-00005ea0: 662e 6765 7428 2263 6f6e 7465 7374 2229  f.get("contest")
-00005eb0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00005ec0: 6c66 2e63 6f6e 7465 7374 5f73 6574 7469  lf.contest_setti
-00005ed0: 6e67 7320 3d20 7365 6c66 2e64 6174 6162  ngs = self.datab
-00005ee0: 6173 652e 6665 7463 685f 636f 6e74 6573  ase.fetch_contes
-00005ef0: 745f 6279 5f69 6428 0a20 2020 2020 2020  t_by_id(.       
-00005f00: 2020 2020 2020 2020 2073 656c 662e 7072           self.pr
-00005f10: 6566 2e67 6574 2822 636f 6e74 6573 7422  ef.get("contest"
-00005f20: 290a 2020 2020 2020 2020 2020 2020 290a  ).            ).
-00005f30: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-00005f40: 656c 662e 636f 6e74 6573 745f 7365 7474  elf.contest_sett
-00005f50: 696e 6773 3a0a 2020 2020 2020 2020 2020  ings:.          
-00005f60: 2020 2020 2020 7365 6c66 2e64 6174 6162        self.datab
-00005f70: 6173 652e 6375 7272 656e 745f 636f 6e74  ase.current_cont
-00005f80: 6573 7420 3d20 7365 6c66 2e70 7265 662e  est = self.pref.
-00005f90: 6765 7428 2263 6f6e 7465 7374 2229 0a20  get("contest"). 
-00005fa0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00005fb0: 6620 7365 6c66 2e63 6f6e 7465 7374 5f73  f self.contest_s
-00005fc0: 6574 7469 6e67 732e 6765 7428 2243 6f6e  ettings.get("Con
-00005fd0: 7465 7374 4e61 6d65 2229 3a0a 2020 2020  testName"):.    
-00005fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005ff0: 7365 6c66 2e63 6f6e 7465 7374 203d 2064  self.contest = d
-00006000: 6f69 6d70 2873 656c 662e 636f 6e74 6573  oimp(self.contes
-00006010: 745f 7365 7474 696e 6773 2e67 6574 2822  t_settings.get("
-00006020: 436f 6e74 6573 744e 616d 6522 2929 0a20  ContestName")). 
-00006030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006040: 2020 206c 6f67 6765 722e 6465 6275 6728     logger.debug(
-00006050: 224c 6f61 6465 6420 436f 6e74 6573 7420  "Loaded Contest 
-00006060: 4e61 6d65 203d 2025 7322 2c20 7365 6c66  Name = %s", self
-00006070: 2e63 6f6e 7465 7374 2e6e 616d 6529 0a20  .contest.name). 
-00006080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006090: 2020 2073 656c 662e 7365 745f 7769 6e64     self.set_wind
-000060a0: 6f77 5f74 6974 6c65 2829 0a20 2020 2020  ow_title().     
-000060b0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000060c0: 656c 662e 636f 6e74 6573 742e 696e 6974  elf.contest.init
-000060d0: 5f63 6f6e 7465 7374 2873 656c 6629 0a20  _contest(self). 
-000060e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000060f0: 2020 2073 656c 662e 6869 6465 5f62 616e     self.hide_ban
-00006100: 645f 6d6f 6465 2873 656c 662e 636f 6e74  d_mode(self.cont
-00006110: 6573 745f 7365 7474 696e 6773 2e67 6574  est_settings.get
-00006120: 2822 4d6f 6465 4361 7465 676f 7279 222c  ("ModeCategory",
-00006130: 2022 2229 290a 2020 2020 2020 2020 2020   "")).          
-00006140: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
-00006150: 2e64 6562 7567 2822 2573 222c 2066 227b  .debug("%s", f"{
-00006160: 7365 6c66 2e63 6f6e 7465 7374 5f73 6574  self.contest_set
-00006170: 7469 6e67 737d 2229 0a20 2020 2020 2020  tings}").       
-00006180: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00006190: 7365 6c66 2e63 6f6e 7465 7374 5f73 6574  self.contest_set
-000061a0: 7469 6e67 732e 6765 7428 224d 6f64 6543  tings.get("ModeC
-000061b0: 6174 6567 6f72 7922 2c20 2222 2920 3d3d  ategory", "") ==
-000061c0: 2022 4357 223a 0a20 2020 2020 2020 2020   "CW":.         
-000061d0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000061e0: 656c 662e 7365 746d 6f64 6528 2243 5722  elf.setmode("CW"
-000061f0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00006200: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
-00006210: 6164 696f 5f73 7461 7465 5b22 6d6f 6465  adio_state["mode
-00006220: 225d 203d 2022 4357 220a 2020 2020 2020  "] = "CW".      
-00006230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006240: 2020 6966 2073 656c 662e 7269 675f 636f    if self.rig_co
-00006250: 6e74 726f 6c3a 0a20 2020 2020 2020 2020  ntrol:.         
-00006260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006270: 2020 2069 6620 7365 6c66 2e72 6967 5f63     if self.rig_c
-00006280: 6f6e 7472 6f6c 2e6f 6e6c 696e 653a 0a20  ontrol.online:. 
-00006290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000062a0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000062b0: 656c 662e 7269 675f 636f 6e74 726f 6c2e  elf.rig_control.
-000062c0: 7365 745f 6d6f 6465 2822 4357 2229 0a20  set_mode("CW"). 
-000062d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000062e0: 2020 2020 2020 2062 616e 6420 3d20 6765         band = ge
-000062f0: 7462 616e 6428 7374 7228 7365 6c66 2e72  tband(str(self.r
-00006300: 6164 696f 5f73 7461 7465 2e67 6574 2822  adio_state.get("
-00006310: 7666 6f61 222c 2022 302e 3022 2929 290a  vfoa", "0.0"))).
+00005bf0: 7665 726c 6179 2e63 7572 7265 6e74 5465  verlay.currentTe
+00005c00: 7874 2829 0a20 2020 2020 2020 2063 6f6e  xt().        con
+00005c10: 7465 7374 5b22 4f70 6572 6174 6f72 7322  test["Operators"
+00005c20: 5d20 3d20 7365 6c66 2e63 6f6e 7465 7374  ] = self.contest
+00005c30: 5f64 6961 6c6f 672e 6f70 6572 6174 6f72  _dialog.operator
+00005c40: 732e 7465 7874 2829 0a20 2020 2020 2020  s.text().       
+00005c50: 2063 6f6e 7465 7374 5b22 536f 6170 626f   contest["Soapbo
+00005c60: 7822 5d20 3d20 7365 6c66 2e63 6f6e 7465  x"] = self.conte
+00005c70: 7374 5f64 6961 6c6f 672e 736f 6170 626f  st_dialog.soapbo
+00005c80: 782e 746f 506c 6169 6e54 6578 7428 290a  x.toPlainText().
+00005c90: 2020 2020 2020 2020 636f 6e74 6573 745b          contest[
+00005ca0: 2253 656e 7445 7863 6861 6e67 6522 5d20  "SentExchange"] 
+00005cb0: 3d20 7365 6c66 2e63 6f6e 7465 7374 5f64  = self.contest_d
+00005cc0: 6961 6c6f 672e 6578 6368 616e 6765 2e74  ialog.exchange.t
+00005cd0: 6578 7428 290a 2020 2020 2020 2020 636f  ext().        co
+00005ce0: 6e74 6573 745b 2243 6f6e 7465 7374 4e52  ntest["ContestNR
+00005cf0: 225d 203d 2073 656c 662e 7072 6566 2e67  "] = self.pref.g
+00005d00: 6574 2822 636f 6e74 6573 7422 2c20 3129  et("contest", 1)
+00005d10: 0a20 2020 2020 2020 2063 6f6e 7465 7374  .        contest
+00005d20: 5b22 5374 6174 696f 6e43 6174 6567 6f72  ["StationCategor
+00005d30: 7922 5d20 3d20 7365 6c66 2e63 6f6e 7465  y"] = self.conte
+00005d40: 7374 5f64 6961 6c6f 672e 7374 6174 696f  st_dialog.statio
+00005d50: 6e2e 6375 7272 656e 7454 6578 7428 290a  n.currentText().
+00005d60: 2020 2020 2020 2020 636f 6e74 6573 745b          contest[
+00005d70: 2241 7373 6973 7465 6443 6174 6567 6f72  "AssistedCategor
+00005d80: 7922 5d20 3d20 7365 6c66 2e63 6f6e 7465  y"] = self.conte
+00005d90: 7374 5f64 6961 6c6f 672e 6173 7369 7374  st_dialog.assist
+00005da0: 6564 2e63 7572 7265 6e74 5465 7874 2829  ed.currentText()
+00005db0: 0a20 2020 2020 2020 2063 6f6e 7465 7374  .        contest
+00005dc0: 5b22 5472 616e 736d 6974 7465 7243 6174  ["TransmitterCat
+00005dd0: 6567 6f72 7922 5d20 3d20 7365 6c66 2e63  egory"] = self.c
+00005de0: 6f6e 7465 7374 5f64 6961 6c6f 672e 7472  ontest_dialog.tr
+00005df0: 616e 736d 6974 7465 722e 6375 7272 656e  ansmitter.curren
+00005e00: 7454 6578 7428 290a 0a20 2020 2020 2020  tText()..       
+00005e10: 206c 6f67 6765 722e 6465 6275 6728 2225   logger.debug("%
+00005e20: 7322 2c20 6622 7b63 6f6e 7465 7374 7d22  s", f"{contest}"
+00005e30: 290a 2020 2020 2020 2020 7365 6c66 2e64  ).        self.d
+00005e40: 6174 6162 6173 652e 7570 6461 7465 5f63  atabase.update_c
+00005e50: 6f6e 7465 7374 2863 6f6e 7465 7374 290a  ontest(contest).
+00005e60: 2020 2020 2020 2020 7365 6c66 2e77 7269          self.wri
+00005e70: 7465 5f70 7265 6665 7265 6e63 6528 290a  te_preference().
+00005e80: 2020 2020 2020 2020 7365 6c66 2e6c 6f61          self.loa
+00005e90: 645f 636f 6e74 6573 7428 290a 0a20 2020  d_contest()..   
+00005ea0: 2064 6566 206c 6f61 645f 636f 6e74 6573   def load_contes
+00005eb0: 7428 7365 6c66 293a 0a20 2020 2020 2020  t(self):.       
+00005ec0: 2022 2222 6c6f 6164 2061 2063 6f6e 7465   """load a conte
+00005ed0: 7374 2222 220a 2020 2020 2020 2020 6966  st""".        if
+00005ee0: 2073 656c 662e 7072 6566 2e67 6574 2822   self.pref.get("
+00005ef0: 636f 6e74 6573 7422 293a 0a20 2020 2020  contest"):.     
+00005f00: 2020 2020 2020 2073 656c 662e 636f 6e74         self.cont
+00005f10: 6573 745f 7365 7474 696e 6773 203d 2073  est_settings = s
+00005f20: 656c 662e 6461 7461 6261 7365 2e66 6574  elf.database.fet
+00005f30: 6368 5f63 6f6e 7465 7374 5f62 795f 6964  ch_contest_by_id
+00005f40: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00005f50: 2020 7365 6c66 2e70 7265 662e 6765 7428    self.pref.get(
+00005f60: 2263 6f6e 7465 7374 2229 0a20 2020 2020  "contest").     
+00005f70: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00005f80: 2020 2020 2069 6620 7365 6c66 2e63 6f6e       if self.con
+00005f90: 7465 7374 5f73 6574 7469 6e67 733a 0a20  test_settings:. 
+00005fa0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00005fb0: 656c 662e 6461 7461 6261 7365 2e63 7572  elf.database.cur
+00005fc0: 7265 6e74 5f63 6f6e 7465 7374 203d 2073  rent_contest = s
+00005fd0: 656c 662e 7072 6566 2e67 6574 2822 636f  elf.pref.get("co
+00005fe0: 6e74 6573 7422 290a 2020 2020 2020 2020  ntest").        
+00005ff0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00006000: 636f 6e74 6573 745f 7365 7474 696e 6773  contest_settings
+00006010: 2e67 6574 2822 436f 6e74 6573 744e 616d  .get("ContestNam
+00006020: 6522 293a 0a20 2020 2020 2020 2020 2020  e"):.           
+00006030: 2020 2020 2020 2020 2073 656c 662e 636f           self.co
+00006040: 6e74 6573 7420 3d20 646f 696d 7028 7365  ntest = doimp(se
+00006050: 6c66 2e63 6f6e 7465 7374 5f73 6574 7469  lf.contest_setti
+00006060: 6e67 732e 6765 7428 2243 6f6e 7465 7374  ngs.get("Contest
+00006070: 4e61 6d65 2229 290a 2020 2020 2020 2020  Name")).        
+00006080: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
+00006090: 6572 2e64 6562 7567 2822 4c6f 6164 6564  er.debug("Loaded
+000060a0: 2043 6f6e 7465 7374 204e 616d 6520 3d20   Contest Name = 
+000060b0: 2573 222c 2073 656c 662e 636f 6e74 6573  %s", self.contes
+000060c0: 742e 6e61 6d65 290a 2020 2020 2020 2020  t.name).        
+000060d0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000060e0: 2e73 6574 5f77 696e 646f 775f 7469 746c  .set_window_titl
+000060f0: 6528 290a 2020 2020 2020 2020 2020 2020  e().            
+00006100: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
+00006110: 7465 7374 2e69 6e69 745f 636f 6e74 6573  test.init_contes
+00006120: 7428 7365 6c66 290a 2020 2020 2020 2020  t(self).        
+00006130: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00006140: 2e68 6964 655f 6261 6e64 5f6d 6f64 6528  .hide_band_mode(
+00006150: 7365 6c66 2e63 6f6e 7465 7374 5f73 6574  self.contest_set
+00006160: 7469 6e67 732e 6765 7428 224d 6f64 6543  tings.get("ModeC
+00006170: 6174 6567 6f72 7922 2c20 2222 2929 0a20  ategory", "")). 
+00006180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006190: 2020 206c 6f67 6765 722e 6465 6275 6728     logger.debug(
+000061a0: 2225 7322 2c20 6622 7b73 656c 662e 636f  "%s", f"{self.co
+000061b0: 6e74 6573 745f 7365 7474 696e 6773 7d22  ntest_settings}"
+000061c0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+000061d0: 2020 2020 2020 6966 2073 656c 662e 636f        if self.co
+000061e0: 6e74 6573 745f 7365 7474 696e 6773 2e67  ntest_settings.g
+000061f0: 6574 2822 4d6f 6465 4361 7465 676f 7279  et("ModeCategory
+00006200: 222c 2022 2229 203d 3d20 2243 5722 3a0a  ", "") == "CW":.
+00006210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006220: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
+00006230: 6d6f 6465 2822 4357 2229 0a20 2020 2020  mode("CW").     
+00006240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006250: 2020 2073 656c 662e 7261 6469 6f5f 7374     self.radio_st
+00006260: 6174 655b 226d 6f64 6522 5d20 3d20 2243  ate["mode"] = "C
+00006270: 5722 0a20 2020 2020 2020 2020 2020 2020  W".             
+00006280: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+00006290: 6c66 2e72 6967 5f63 6f6e 7472 6f6c 3a0a  lf.rig_control:.
+000062a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000062b0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+000062c0: 656c 662e 7269 675f 636f 6e74 726f 6c2e  elf.rig_control.
+000062d0: 6f6e 6c69 6e65 3a0a 2020 2020 2020 2020  online:.        
+000062e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000062f0: 2020 2020 2020 2020 7365 6c66 2e72 6967          self.rig
+00006300: 5f63 6f6e 7472 6f6c 2e73 6574 5f6d 6f64  _control.set_mod
+00006310: 6528 2243 5722 290a 2020 2020 2020 2020  e("CW").        
 00006320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006330: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
-00006340: 5f62 616e 645f 696e 6469 6361 746f 7228  _band_indicator(
-00006350: 6261 6e64 290a 2020 2020 2020 2020 2020  band).          
-00006360: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00006370: 6c66 2e73 6574 5f77 696e 646f 775f 7469  lf.set_window_ti
-00006380: 746c 6528 290a 2020 2020 2020 2020 2020  tle().          
-00006390: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-000063a0: 662e 636f 6e74 6573 745f 7365 7474 696e  f.contest_settin
-000063b0: 6773 2e67 6574 2822 4d6f 6465 4361 7465  gs.get("ModeCate
-000063c0: 676f 7279 222c 2022 2229 203d 3d20 2253  gory", "") == "S
-000063d0: 5342 223a 0a20 2020 2020 2020 2020 2020  SB":.           
-000063e0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-000063f0: 662e 7365 746d 6f64 6528 2253 5342 2229  f.setmode("SSB")
-00006400: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006410: 2020 2020 2020 2020 2069 6620 696e 7428           if int(
-00006420: 7365 6c66 2e72 6164 696f 5f73 7461 7465  self.radio_state
-00006430: 2e67 6574 2822 7666 6f61 222c 2030 2929  .get("vfoa", 0))
-00006440: 203e 2031 3030 3030 3030 303a 0a20 2020   > 10000000:.   
+00006330: 6261 6e64 203d 2067 6574 6261 6e64 2873  band = getband(s
+00006340: 7472 2873 656c 662e 7261 6469 6f5f 7374  tr(self.radio_st
+00006350: 6174 652e 6765 7428 2276 666f 6122 2c20  ate.get("vfoa", 
+00006360: 2230 2e30 2229 2929 0a20 2020 2020 2020  "0.0"))).       
+00006370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006380: 2073 656c 662e 7365 745f 6261 6e64 5f69   self.set_band_i
+00006390: 6e64 6963 6174 6f72 2862 616e 6429 0a20  ndicator(band). 
+000063a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000063b0: 2020 2020 2020 2073 656c 662e 7365 745f         self.set_
+000063c0: 7769 6e64 6f77 5f74 6974 6c65 2829 0a20  window_title(). 
+000063d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000063e0: 2020 2069 6620 7365 6c66 2e63 6f6e 7465     if self.conte
+000063f0: 7374 5f73 6574 7469 6e67 732e 6765 7428  st_settings.get(
+00006400: 224d 6f64 6543 6174 6567 6f72 7922 2c20  "ModeCategory", 
+00006410: 2222 2920 3d3d 2022 5353 4222 3a0a 2020  "") == "SSB":.  
+00006420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006430: 2020 2020 2020 7365 6c66 2e73 6574 6d6f        self.setmo
+00006440: 6465 2822 5353 4222 290a 2020 2020 2020  de("SSB").      
 00006450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006460: 2020 2020 2020 2020 2073 656c 662e 7261           self.ra
-00006470: 6469 6f5f 7374 6174 655b 226d 6f64 6522  dio_state["mode"
-00006480: 5d20 3d20 2255 5342 220a 2020 2020 2020  ] = "USB".      
-00006490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000064a0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-000064b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000064c0: 2020 2020 7365 6c66 2e72 6164 696f 5f73      self.radio_s
-000064d0: 7461 7465 5b22 6d6f 6465 225d 203d 2022  tate["mode"] = "
-000064e0: 4c53 4222 0a20 2020 2020 2020 2020 2020  LSB".           
-000064f0: 2020 2020 2020 2020 2020 2020 2062 616e               ban
-00006500: 6420 3d20 6765 7462 616e 6428 7374 7228  d = getband(str(
-00006510: 7365 6c66 2e72 6164 696f 5f73 7461 7465  self.radio_state
-00006520: 2e67 6574 2822 7666 6f61 222c 2022 302e  .get("vfoa", "0.
-00006530: 3022 2929 290a 2020 2020 2020 2020 2020  0"))).          
-00006540: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00006550: 6c66 2e73 6574 5f62 616e 645f 696e 6469  lf.set_band_indi
-00006560: 6361 746f 7228 6261 6e64 290a 2020 2020  cator(band).    
-00006570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006580: 2020 2020 7365 6c66 2e73 6574 5f77 696e      self.set_win
-00006590: 646f 775f 7469 746c 6528 290a 2020 2020  dow_title().    
-000065a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000065b0: 2020 2020 6966 2073 656c 662e 7269 675f      if self.rig_
-000065c0: 636f 6e74 726f 6c3a 0a20 2020 2020 2020  control:.       
-000065d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000065e0: 2020 2020 2073 656c 662e 7269 675f 636f       self.rig_co
-000065f0: 6e74 726f 6c2e 7365 745f 6d6f 6465 2873  ntrol.set_mode(s
-00006600: 656c 662e 7261 6469 6f5f 7374 6174 652e  elf.radio_state.
-00006610: 6765 7428 226d 6f64 6522 2929 0a0a 2020  get("mode"))..  
-00006620: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00006630: 2068 6173 6174 7472 2873 656c 662e 636f   hasattr(self.co
-00006640: 6e74 6573 742c 2022 6d6f 6465 2229 3a0a  ntest, "mode"):.
-00006650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006660: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
-00006670: 2822 2573 222c 2066 2220 202a 2a2a 2a20  ("%s", f"  **** 
-00006680: 207b 7365 6c66 2e63 6f6e 7465 7374 7d22   {self.contest}"
-00006690: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-000066a0: 2020 2020 2020 6966 2073 656c 662e 636f        if self.co
-000066b0: 6e74 6573 742e 6d6f 6465 2069 6e20 5b22  ntest.mode in ["
-000066c0: 4357 222c 2022 424f 5448 225d 3a0a 2020  CW", "BOTH"]:.  
-000066d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000066e0: 2020 2020 2020 7365 6c66 2e63 775f 7370        self.cw_sp
-000066f0: 6565 642e 7368 6f77 2829 0a20 2020 2020  eed.show().     
-00006700: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00006710: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00006720: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00006730: 662e 6377 5f73 7065 6564 2e68 6964 6528  f.cw_speed.hide(
-00006740: 290a 0a20 2020 2020 2020 2020 2020 2020  )..             
-00006750: 2020 2063 6d64 203d 207b 7d0a 2020 2020     cmd = {}.    
-00006760: 2020 2020 2020 2020 2020 2020 636d 645b              cmd[
-00006770: 2263 6d64 225d 203d 2022 4e45 5744 4222  "cmd"] = "NEWDB"
-00006780: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006790: 2063 6d64 5b22 7374 6174 696f 6e22 5d20   cmd["station"] 
-000067a0: 3d20 706c 6174 666f 726d 2e6e 6f64 6528  = platform.node(
-000067b0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-000067c0: 2020 7365 6c66 2e6d 756c 7469 6361 7374    self.multicast
-000067d0: 5f69 6e74 6572 6661 6365 2e73 656e 645f  _interface.send_
-000067e0: 6173 5f6a 736f 6e28 636d 6429 0a20 2020  as_json(cmd).   
-000067f0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00006800: 6861 7361 7474 7228 7365 6c66 2e63 6f6e  hasattr(self.con
-00006810: 7465 7374 2c20 2263 6f6c 756d 6e73 2229  test, "columns")
-00006820: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00006830: 2020 2020 2020 636d 6420 3d20 7b7d 0a20        cmd = {}. 
-00006840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006850: 2020 2063 6d64 5b22 636d 6422 5d20 3d20     cmd["cmd"] = 
-00006860: 2253 484f 5743 4f4c 554d 4e53 220a 2020  "SHOWCOLUMNS".  
-00006870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006880: 2020 636d 645b 2273 7461 7469 6f6e 225d    cmd["station"]
-00006890: 203d 2070 6c61 7466 6f72 6d2e 6e6f 6465   = platform.node
-000068a0: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
-000068b0: 2020 2020 2020 2063 6d64 5b22 434f 4c55         cmd["COLU
-000068c0: 4d4e 5322 5d20 3d20 7365 6c66 2e63 6f6e  MNS"] = self.con
-000068d0: 7465 7374 2e63 6f6c 756d 6e73 0a20 2020  test.columns.   
-000068e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000068f0: 2073 656c 662e 6d75 6c74 6963 6173 745f   self.multicast_
-00006900: 696e 7465 7266 6163 652e 7365 6e64 5f61  interface.send_a
-00006910: 735f 6a73 6f6e 2863 6d64 290a 0a20 2020  s_json(cmd)..   
-00006920: 2064 6566 2063 6865 636b 5f66 6f72 5f6e   def check_for_n
-00006930: 6577 5f63 7479 2873 656c 6629 3a0a 2020  ew_cty(self):.  
-00006940: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00006950: 2020 4368 6563 6b73 2066 6f72 2061 206e    Checks for a n
-00006960: 6577 2063 7479 2e64 6174 2066 696c 652e  ew cty.dat file.
-00006970: 0a20 2020 2020 2020 204c 6f61 6473 2069  .        Loads i
-00006980: 7420 6966 2061 7661 696c 6162 6c65 2e0a  t if available..
-00006990: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-000069a0: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
-000069b0: 2020 2020 2063 7479 203d 206e 6f74 6374       cty = notct
-000069c0: 7970 6172 7365 722e 4269 6743 7479 2857  yparser.BigCty(W
-000069d0: 4f52 4b49 4e47 5f50 4154 4820 2b20 222f  ORKING_PATH + "/
-000069e0: 6461 7461 2f63 7479 2e6a 736f 6e22 290a  data/cty.json").
-000069f0: 2020 2020 2020 2020 2020 2020 7570 6461              upda
-00006a00: 7465 5f61 7661 696c 6162 6c65 203d 2063  te_available = c
-00006a10: 7479 2e63 6865 636b 5f75 7064 6174 6528  ty.check_update(
-00006a20: 290a 2020 2020 2020 2020 6578 6365 7074  ).        except
-00006a30: 2041 7474 7269 6275 7465 4572 726f 7220   AttributeError 
-00006a40: 6173 2074 6865 5f65 7272 6f72 3a0a 2020  as the_error:.  
-00006a50: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
-00006a60: 2e64 6562 7567 2822 6374 7920 7061 7273  .debug("cty pars
-00006a70: 6572 2072 6574 7572 6e65 6420 616e 2065  er returned an e
-00006a80: 7272 6f72 3a20 2573 222c 2074 6865 5f65  rror: %s", the_e
-00006a90: 7272 6f72 290a 2020 2020 2020 2020 2020  rror).          
-00006aa0: 2020 7265 7475 726e 0a20 2020 2020 2020    return.       
-00006ab0: 2065 7863 6570 7420 5661 6c75 6545 7272   except ValueErr
-00006ac0: 6f72 2061 7320 7468 655f 6572 726f 723a  or as the_error:
-00006ad0: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
-00006ae0: 6e74 2822 6374 7920 7061 7273 6572 2072  nt("cty parser r
-00006af0: 6574 7572 6e65 6420 616e 2065 7272 6f72  eturned an error
-00006b00: 3a20 2573 222c 2074 6865 5f65 7272 6f72  : %s", the_error
-00006b10: 290a 2020 2020 2020 2020 2020 2020 6c6f  ).            lo
-00006b20: 6767 6572 2e64 6562 7567 2822 6374 7920  gger.debug("cty 
-00006b30: 7061 7273 6572 2072 6574 7572 6e65 6420  parser returned 
-00006b40: 616e 2065 7272 6f72 3a20 2573 222c 2074  an error: %s", t
-00006b50: 6865 5f65 7272 6f72 290a 2020 2020 2020  he_error).      
-00006b60: 2020 2020 2020 7265 7475 726e 0a20 2020        return.   
-00006b70: 2020 2020 2065 7863 6570 7420 6c6f 6361       except loca
-00006b80: 6c65 2e45 7272 6f72 2061 7320 7468 655f  le.Error as the_
-00006b90: 6572 726f 723a 0a20 2020 2020 2020 2020  error:.         
-00006ba0: 2020 2070 7269 6e74 2822 6374 7920 7061     print("cty pa
-00006bb0: 7273 6572 2072 6574 7572 6e65 6420 616e  rser returned an
-00006bc0: 2065 7272 6f72 3a20 2573 222c 2074 6865   error: %s", the
-00006bd0: 5f65 7272 6f72 290a 2020 2020 2020 2020  _error).        
-00006be0: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
-00006bf0: 2822 6374 7920 7061 7273 6572 2072 6574  ("cty parser ret
-00006c00: 7572 6e65 6420 616e 2065 7272 6f72 3a20  urned an error: 
-00006c10: 2573 222c 2074 6865 5f65 7272 6f72 290a  %s", the_error).
-00006c20: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00006c30: 726e 0a20 2020 2020 2020 206c 6f67 6765  rn.        logge
-00006c40: 722e 6465 6275 6728 224e 6577 6572 2063  r.debug("Newer c
-00006c50: 7479 2066 696c 6520 6176 6169 6c61 626c  ty file availabl
-00006c60: 6520 2573 222c 2073 7472 2875 7064 6174  e %s", str(updat
-00006c70: 655f 6176 6169 6c61 626c 6529 290a 0a20  e_available)).. 
-00006c80: 2020 2020 2020 2069 6620 7570 6461 7465         if update
-00006c90: 5f61 7661 696c 6162 6c65 3a0a 2020 2020  _available:.    
-00006ca0: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
-00006cb0: 2020 2020 2020 2020 2020 2020 2075 7064               upd
-00006cc0: 6174 6564 203d 2063 7479 2e75 7064 6174  ated = cty.updat
-00006cd0: 6528 290a 2020 2020 2020 2020 2020 2020  e().            
-00006ce0: 6578 6365 7074 2052 6573 6f75 7263 6557  except ResourceW
-00006cf0: 6172 6e69 6e67 2061 7320 7468 655f 6572  arning as the_er
-00006d00: 726f 723a 0a20 2020 2020 2020 2020 2020  ror:.           
-00006d10: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
-00006d20: 6728 2263 7479 2070 6172 7365 7220 7265  g("cty parser re
-00006d30: 7475 726e 6564 2061 6e20 6572 726f 723a  turned an error:
-00006d40: 2025 7322 2c20 7468 655f 6572 726f 7229   %s", the_error)
-00006d50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006d60: 2072 6574 7572 6e0a 2020 2020 2020 2020   return.        
-00006d70: 2020 2020 6966 2075 7064 6174 6564 3a0a      if updated:.
-00006d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006d90: 6374 792e 6475 6d70 2857 4f52 4b49 4e47  cty.dump(WORKING
-00006da0: 5f50 4154 4820 2b20 222f 6461 7461 2f63  _PATH + "/data/c
-00006db0: 7479 2e6a 736f 6e22 290a 2020 2020 2020  ty.json").      
-00006dc0: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
-00006dd0: 686f 775f 6d65 7373 6167 655f 626f 7828  how_message_box(
-00006de0: 2263 7479 2066 696c 6520 7570 6461 7465  "cty file update
-00006df0: 642e 2229 0a20 2020 2020 2020 2020 2020  d.").           
-00006e00: 2020 2020 2077 6974 6820 6f70 656e 280a       with open(.
-00006e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006e20: 2020 2020 574f 524b 494e 475f 5041 5448      WORKING_PATH
-00006e30: 202b 2022 2f64 6174 612f 6374 792e 6a73   + "/data/cty.js
-00006e40: 6f6e 222c 2022 7274 222c 2065 6e63 6f64  on", "rt", encod
-00006e50: 696e 673d 2275 7466 2d38 220a 2020 2020  ing="utf-8".    
-00006e60: 2020 2020 2020 2020 2020 2020 2920 6173              ) as
-00006e70: 2063 7479 6669 6c65 3a0a 2020 2020 2020   ctyfile:.      
-00006e80: 2020 2020 2020 2020 2020 2020 2020 676c                gl
-00006e90: 6f62 616c 7328 295b 2243 5459 4649 4c45  obals()["CTYFILE
-00006ea0: 225d 203d 206c 6f61 6473 2863 7479 6669  "] = loads(ctyfi
-00006eb0: 6c65 2e72 6561 6428 2929 0a20 2020 2020  le.read()).     
-00006ec0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00006ed0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00006ee0: 662e 7368 6f77 5f6d 6573 7361 6765 5f62  f.show_message_b
-00006ef0: 6f78 2822 416e 2045 7272 6f72 206f 6363  ox("An Error occ
-00006f00: 7572 6564 2075 7064 6174 696e 6720 6669  ured updating fi
-00006f10: 6c65 2e22 290a 2020 2020 2020 2020 656c  le.").        el
-00006f20: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00006f30: 7365 6c66 2e73 686f 775f 6d65 7373 6167  self.show_messag
-00006f40: 655f 626f 7828 2243 5459 2066 696c 6520  e_box("CTY file 
-00006f50: 6973 2075 7020 746f 2064 6174 652e 2229  is up to date.")
-00006f60: 0a0a 2020 2020 6465 6620 6869 6465 5f62  ..    def hide_b
-00006f70: 616e 645f 6d6f 6465 2873 656c 662c 2074  and_mode(self, t
-00006f80: 6865 5f6d 6f64 653a 2073 7472 2920 2d3e  he_mode: str) ->
-00006f90: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
-00006fa0: 2222 6869 6465 2222 220a 2020 2020 2020  ""hide""".      
-00006fb0: 2020 6c6f 6767 6572 2e64 6562 7567 2822    logger.debug("
-00006fc0: 2573 222c 2066 227b 7468 655f 6d6f 6465  %s", f"{the_mode
-00006fd0: 7d22 290a 2020 2020 2020 2020 7365 6c66  }").        self
-00006fe0: 2e42 616e 645f 4d6f 6465 5f46 7261 6d65  .Band_Mode_Frame
-00006ff0: 5f43 572e 6869 6465 2829 0a20 2020 2020  _CW.hide().     
-00007000: 2020 2073 656c 662e 4261 6e64 5f4d 6f64     self.Band_Mod
-00007010: 655f 4672 616d 655f 5353 422e 6869 6465  e_Frame_SSB.hide
-00007020: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
-00007030: 4261 6e64 5f4d 6f64 655f 4672 616d 655f  Band_Mode_Frame_
-00007040: 5254 5459 2e68 6964 6528 290a 2020 2020  RTTY.hide().    
-00007050: 2020 2020 6d6f 6465 7320 3d20 7b0a 2020      modes = {.  
-00007060: 2020 2020 2020 2020 2020 2243 5722 3a20            "CW": 
-00007070: 2873 656c 662e 4261 6e64 5f4d 6f64 655f  (self.Band_Mode_
-00007080: 4672 616d 655f 4357 2c29 2c0a 2020 2020  Frame_CW,),.    
-00007090: 2020 2020 2020 2020 2253 5342 223a 2028          "SSB": (
-000070a0: 7365 6c66 2e42 616e 645f 4d6f 6465 5f46  self.Band_Mode_F
-000070b0: 7261 6d65 5f53 5342 2c29 2c0a 2020 2020  rame_SSB,),.    
-000070c0: 2020 2020 2020 2020 2252 5454 5922 3a20          "RTTY": 
-000070d0: 2873 656c 662e 4261 6e64 5f4d 6f64 655f  (self.Band_Mode_
-000070e0: 4672 616d 655f 5254 5459 2c29 2c0a 2020  Frame_RTTY,),.  
-000070f0: 2020 2020 2020 2020 2020 2250 534b 223a            "PSK":
-00007100: 2028 7365 6c66 2e42 616e 645f 4d6f 6465   (self.Band_Mode
-00007110: 5f46 7261 6d65 5f52 5454 592c 292c 0a20  _Frame_RTTY,),. 
-00007120: 2020 2020 2020 2020 2020 2022 5353 422b             "SSB+
-00007130: 4357 223a 2028 7365 6c66 2e42 616e 645f  CW": (self.Band_
-00007140: 4d6f 6465 5f46 7261 6d65 5f43 572c 2073  Mode_Frame_CW, s
-00007150: 656c 662e 4261 6e64 5f4d 6f64 655f 4672  elf.Band_Mode_Fr
-00007160: 616d 655f 5353 4229 2c0a 2020 2020 2020  ame_SSB),.      
-00007170: 2020 2020 2020 2242 4f54 4822 3a20 2873        "BOTH": (s
+00006460: 2020 6966 2069 6e74 2873 656c 662e 7261    if int(self.ra
+00006470: 6469 6f5f 7374 6174 652e 6765 7428 2276  dio_state.get("v
+00006480: 666f 6122 2c20 3029 2920 3e20 3130 3030  foa", 0)) > 1000
+00006490: 3030 3030 3a0a 2020 2020 2020 2020 2020  0000:.          
+000064a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000064b0: 2020 7365 6c66 2e72 6164 696f 5f73 7461    self.radio_sta
+000064c0: 7465 5b22 6d6f 6465 225d 203d 2022 5553  te["mode"] = "US
+000064d0: 4222 0a20 2020 2020 2020 2020 2020 2020  B".             
+000064e0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+000064f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006500: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00006510: 662e 7261 6469 6f5f 7374 6174 655b 226d  f.radio_state["m
+00006520: 6f64 6522 5d20 3d20 224c 5342 220a 2020  ode"] = "LSB".  
+00006530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006540: 2020 2020 2020 6261 6e64 203d 2067 6574        band = get
+00006550: 6261 6e64 2873 7472 2873 656c 662e 7261  band(str(self.ra
+00006560: 6469 6f5f 7374 6174 652e 6765 7428 2276  dio_state.get("v
+00006570: 666f 6122 2c20 2230 2e30 2229 2929 0a20  foa", "0.0"))). 
+00006580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006590: 2020 2020 2020 2073 656c 662e 7365 745f         self.set_
+000065a0: 6261 6e64 5f69 6e64 6963 6174 6f72 2862  band_indicator(b
+000065b0: 616e 6429 0a20 2020 2020 2020 2020 2020  and).           
+000065c0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+000065d0: 662e 7365 745f 7769 6e64 6f77 5f74 6974  f.set_window_tit
+000065e0: 6c65 2829 0a20 2020 2020 2020 2020 2020  le().           
+000065f0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00006600: 7365 6c66 2e72 6967 5f63 6f6e 7472 6f6c  self.rig_control
+00006610: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00006620: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00006630: 6c66 2e72 6967 5f63 6f6e 7472 6f6c 2e73  lf.rig_control.s
+00006640: 6574 5f6d 6f64 6528 7365 6c66 2e72 6164  et_mode(self.rad
+00006650: 696f 5f73 7461 7465 2e67 6574 2822 6d6f  io_state.get("mo
+00006660: 6465 2229 290a 0a20 2020 2020 2020 2020  de"))..         
+00006670: 2020 2020 2020 2069 6620 6861 7361 7474         if hasatt
+00006680: 7228 7365 6c66 2e63 6f6e 7465 7374 2c20  r(self.contest, 
+00006690: 226d 6f64 6522 293a 0a20 2020 2020 2020  "mode"):.       
+000066a0: 2020 2020 2020 2020 2020 2020 206c 6f67               log
+000066b0: 6765 722e 6465 6275 6728 2225 7322 2c20  ger.debug("%s", 
+000066c0: 6622 2020 2a2a 2a2a 2020 7b73 656c 662e  f"  ****  {self.
+000066d0: 636f 6e74 6573 747d 2229 0a20 2020 2020  contest}").     
+000066e0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+000066f0: 6620 7365 6c66 2e63 6f6e 7465 7374 2e6d  f self.contest.m
+00006700: 6f64 6520 696e 205b 2243 5722 2c20 2242  ode in ["CW", "B
+00006710: 4f54 4822 5d3a 0a20 2020 2020 2020 2020  OTH"]:.         
+00006720: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00006730: 656c 662e 6377 5f73 7065 6564 2e73 686f  elf.cw_speed.sho
+00006740: 7728 290a 2020 2020 2020 2020 2020 2020  w().            
+00006750: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00006760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006770: 2020 2020 2020 7365 6c66 2e63 775f 7370        self.cw_sp
+00006780: 6565 642e 6869 6465 2829 0a0a 2020 2020  eed.hide()..    
+00006790: 2020 2020 2020 2020 2020 2020 636d 6420              cmd 
+000067a0: 3d20 7b7d 0a20 2020 2020 2020 2020 2020  = {}.           
+000067b0: 2020 2020 2063 6d64 5b22 636d 6422 5d20       cmd["cmd"] 
+000067c0: 3d20 224e 4557 4442 220a 2020 2020 2020  = "NEWDB".      
+000067d0: 2020 2020 2020 2020 2020 636d 645b 2273            cmd["s
+000067e0: 7461 7469 6f6e 225d 203d 2070 6c61 7466  tation"] = platf
+000067f0: 6f72 6d2e 6e6f 6465 2829 0a20 2020 2020  orm.node().     
+00006800: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00006810: 6d75 6c74 6963 6173 745f 696e 7465 7266  multicast_interf
+00006820: 6163 652e 7365 6e64 5f61 735f 6a73 6f6e  ace.send_as_json
+00006830: 2863 6d64 290a 2020 2020 2020 2020 2020  (cmd).          
+00006840: 2020 2020 2020 6966 2068 6173 6174 7472        if hasattr
+00006850: 2873 656c 662e 636f 6e74 6573 742c 2022  (self.contest, "
+00006860: 636f 6c75 6d6e 7322 293a 0a20 2020 2020  columns"):.     
+00006870: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00006880: 6d64 203d 207b 7d0a 2020 2020 2020 2020  md = {}.        
+00006890: 2020 2020 2020 2020 2020 2020 636d 645b              cmd[
+000068a0: 2263 6d64 225d 203d 2022 5348 4f57 434f  "cmd"] = "SHOWCO
+000068b0: 4c55 4d4e 5322 0a20 2020 2020 2020 2020  LUMNS".         
+000068c0: 2020 2020 2020 2020 2020 2063 6d64 5b22             cmd["
+000068d0: 7374 6174 696f 6e22 5d20 3d20 706c 6174  station"] = plat
+000068e0: 666f 726d 2e6e 6f64 6528 290a 2020 2020  form.node().    
+000068f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006900: 636d 645b 2243 4f4c 554d 4e53 225d 203d  cmd["COLUMNS"] =
+00006910: 2073 656c 662e 636f 6e74 6573 742e 636f   self.contest.co
+00006920: 6c75 6d6e 730a 2020 2020 2020 2020 2020  lumns.          
+00006930: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
+00006940: 756c 7469 6361 7374 5f69 6e74 6572 6661  ulticast_interfa
+00006950: 6365 2e73 656e 645f 6173 5f6a 736f 6e28  ce.send_as_json(
+00006960: 636d 6429 0a0a 2020 2020 6465 6620 6368  cmd)..    def ch
+00006970: 6563 6b5f 666f 725f 6e65 775f 6374 7928  eck_for_new_cty(
+00006980: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
+00006990: 2222 0a20 2020 2020 2020 2043 6865 636b  "".        Check
+000069a0: 7320 666f 7220 6120 6e65 7720 6374 792e  s for a new cty.
+000069b0: 6461 7420 6669 6c65 2e0a 2020 2020 2020  dat file..      
+000069c0: 2020 4c6f 6164 7320 6974 2069 6620 6176    Loads it if av
+000069d0: 6169 6c61 626c 652e 0a20 2020 2020 2020  ailable..       
+000069e0: 2022 2222 0a20 2020 2020 2020 2074 7279   """.        try
+000069f0: 3a0a 2020 2020 2020 2020 2020 2020 6374  :.            ct
+00006a00: 7920 3d20 6e6f 7463 7479 7061 7273 6572  y = notctyparser
+00006a10: 2e42 6967 4374 7928 574f 524b 494e 475f  .BigCty(WORKING_
+00006a20: 5041 5448 202b 2022 2f64 6174 612f 6374  PATH + "/data/ct
+00006a30: 792e 6a73 6f6e 2229 0a20 2020 2020 2020  y.json").       
+00006a40: 2020 2020 2075 7064 6174 655f 6176 6169       update_avai
+00006a50: 6c61 626c 6520 3d20 6374 792e 6368 6563  lable = cty.chec
+00006a60: 6b5f 7570 6461 7465 2829 0a20 2020 2020  k_update().     
+00006a70: 2020 2065 7863 6570 7420 4174 7472 6962     except Attrib
+00006a80: 7574 6545 7272 6f72 2061 7320 7468 655f  uteError as the_
+00006a90: 6572 726f 723a 0a20 2020 2020 2020 2020  error:.         
+00006aa0: 2020 206c 6f67 6765 722e 6465 6275 6728     logger.debug(
+00006ab0: 2263 7479 2070 6172 7365 7220 7265 7475  "cty parser retu
+00006ac0: 726e 6564 2061 6e20 6572 726f 723a 2025  rned an error: %
+00006ad0: 7322 2c20 7468 655f 6572 726f 7229 0a20  s", the_error). 
+00006ae0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00006af0: 6e0a 2020 2020 2020 2020 6578 6365 7074  n.        except
+00006b00: 2056 616c 7565 4572 726f 7220 6173 2074   ValueError as t
+00006b10: 6865 5f65 7272 6f72 3a0a 2020 2020 2020  he_error:.      
+00006b20: 2020 2020 2020 7072 696e 7428 2263 7479        print("cty
+00006b30: 2070 6172 7365 7220 7265 7475 726e 6564   parser returned
+00006b40: 2061 6e20 6572 726f 723a 2025 7322 2c20   an error: %s", 
+00006b50: 7468 655f 6572 726f 7229 0a20 2020 2020  the_error).     
+00006b60: 2020 2020 2020 206c 6f67 6765 722e 6465         logger.de
+00006b70: 6275 6728 2263 7479 2070 6172 7365 7220  bug("cty parser 
+00006b80: 7265 7475 726e 6564 2061 6e20 6572 726f  returned an erro
+00006b90: 723a 2025 7322 2c20 7468 655f 6572 726f  r: %s", the_erro
+00006ba0: 7229 0a20 2020 2020 2020 2020 2020 2072  r).            r
+00006bb0: 6574 7572 6e0a 2020 2020 2020 2020 6578  eturn.        ex
+00006bc0: 6365 7074 206c 6f63 616c 652e 4572 726f  cept locale.Erro
+00006bd0: 7220 6173 2074 6865 5f65 7272 6f72 3a0a  r as the_error:.
+00006be0: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+00006bf0: 7428 2263 7479 2070 6172 7365 7220 7265  t("cty parser re
+00006c00: 7475 726e 6564 2061 6e20 6572 726f 723a  turned an error:
+00006c10: 2025 7322 2c20 7468 655f 6572 726f 7229   %s", the_error)
+00006c20: 0a20 2020 2020 2020 2020 2020 206c 6f67  .            log
+00006c30: 6765 722e 6465 6275 6728 2263 7479 2070  ger.debug("cty p
+00006c40: 6172 7365 7220 7265 7475 726e 6564 2061  arser returned a
+00006c50: 6e20 6572 726f 723a 2025 7322 2c20 7468  n error: %s", th
+00006c60: 655f 6572 726f 7229 0a20 2020 2020 2020  e_error).       
+00006c70: 2020 2020 2072 6574 7572 6e0a 2020 2020       return.    
+00006c80: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
+00006c90: 2822 4e65 7765 7220 6374 7920 6669 6c65  ("Newer cty file
+00006ca0: 2061 7661 696c 6162 6c65 2025 7322 2c20   available %s", 
+00006cb0: 7374 7228 7570 6461 7465 5f61 7661 696c  str(update_avail
+00006cc0: 6162 6c65 2929 0a0a 2020 2020 2020 2020  able))..        
+00006cd0: 6966 2075 7064 6174 655f 6176 6169 6c61  if update_availa
+00006ce0: 626c 653a 0a20 2020 2020 2020 2020 2020  ble:.           
+00006cf0: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
+00006d00: 2020 2020 2020 7570 6461 7465 6420 3d20        updated = 
+00006d10: 6374 792e 7570 6461 7465 2829 0a20 2020  cty.update().   
+00006d20: 2020 2020 2020 2020 2065 7863 6570 7420           except 
+00006d30: 5265 736f 7572 6365 5761 726e 696e 6720  ResourceWarning 
+00006d40: 6173 2074 6865 5f65 7272 6f72 3a0a 2020  as the_error:.  
+00006d50: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
+00006d60: 6767 6572 2e64 6562 7567 2822 6374 7920  gger.debug("cty 
+00006d70: 7061 7273 6572 2072 6574 7572 6e65 6420  parser returned 
+00006d80: 616e 2065 7272 6f72 3a20 2573 222c 2074  an error: %s", t
+00006d90: 6865 5f65 7272 6f72 290a 2020 2020 2020  he_error).      
+00006da0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00006db0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00006dc0: 7570 6461 7465 643a 0a20 2020 2020 2020  updated:.       
+00006dd0: 2020 2020 2020 2020 2063 7479 2e64 756d           cty.dum
+00006de0: 7028 574f 524b 494e 475f 5041 5448 202b  p(WORKING_PATH +
+00006df0: 2022 2f64 6174 612f 6374 792e 6a73 6f6e   "/data/cty.json
+00006e00: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
+00006e10: 2020 2073 656c 662e 7368 6f77 5f6d 6573     self.show_mes
+00006e20: 7361 6765 5f62 6f78 2822 6374 7920 6669  sage_box("cty fi
+00006e30: 6c65 2075 7064 6174 6564 2e22 290a 2020  le updated.").  
+00006e40: 2020 2020 2020 2020 2020 2020 2020 7769                wi
+00006e50: 7468 206f 7065 6e28 0a20 2020 2020 2020  th open(.       
+00006e60: 2020 2020 2020 2020 2020 2020 2057 4f52               WOR
+00006e70: 4b49 4e47 5f50 4154 4820 2b20 222f 6461  KING_PATH + "/da
+00006e80: 7461 2f63 7479 2e6a 736f 6e22 2c20 2272  ta/cty.json", "r
+00006e90: 7422 2c20 656e 636f 6469 6e67 3d22 7574  t", encoding="ut
+00006ea0: 662d 3822 0a20 2020 2020 2020 2020 2020  f-8".           
+00006eb0: 2020 2020 2029 2061 7320 6374 7966 696c       ) as ctyfil
+00006ec0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00006ed0: 2020 2020 2020 2067 6c6f 6261 6c73 2829         globals()
+00006ee0: 5b22 4354 5946 494c 4522 5d20 3d20 6c6f  ["CTYFILE"] = lo
+00006ef0: 6164 7328 6374 7966 696c 652e 7265 6164  ads(ctyfile.read
+00006f00: 2829 290a 2020 2020 2020 2020 2020 2020  ()).            
+00006f10: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00006f20: 2020 2020 2020 7365 6c66 2e73 686f 775f        self.show_
+00006f30: 6d65 7373 6167 655f 626f 7828 2241 6e20  message_box("An 
+00006f40: 4572 726f 7220 6f63 6375 7265 6420 7570  Error occured up
+00006f50: 6461 7469 6e67 2066 696c 652e 2229 0a20  dating file."). 
+00006f60: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00006f70: 2020 2020 2020 2020 2073 656c 662e 7368           self.sh
+00006f80: 6f77 5f6d 6573 7361 6765 5f62 6f78 2822  ow_message_box("
+00006f90: 4354 5920 6669 6c65 2069 7320 7570 2074  CTY file is up t
+00006fa0: 6f20 6461 7465 2e22 290a 0a20 2020 2064  o date.")..    d
+00006fb0: 6566 2068 6964 655f 6261 6e64 5f6d 6f64  ef hide_band_mod
+00006fc0: 6528 7365 6c66 2c20 7468 655f 6d6f 6465  e(self, the_mode
+00006fd0: 3a20 7374 7229 202d 3e20 4e6f 6e65 3a0a  : str) -> None:.
+00006fe0: 2020 2020 2020 2020 2222 2268 6964 6522          """hide"
+00006ff0: 2222 0a20 2020 2020 2020 206c 6f67 6765  "".        logge
+00007000: 722e 6465 6275 6728 2225 7322 2c20 6622  r.debug("%s", f"
+00007010: 7b74 6865 5f6d 6f64 657d 2229 0a20 2020  {the_mode}").   
+00007020: 2020 2020 2073 656c 662e 4261 6e64 5f4d       self.Band_M
+00007030: 6f64 655f 4672 616d 655f 4357 2e68 6964  ode_Frame_CW.hid
+00007040: 6528 290a 2020 2020 2020 2020 7365 6c66  e().        self
+00007050: 2e42 616e 645f 4d6f 6465 5f46 7261 6d65  .Band_Mode_Frame
+00007060: 5f53 5342 2e68 6964 6528 290a 2020 2020  _SSB.hide().    
+00007070: 2020 2020 7365 6c66 2e42 616e 645f 4d6f      self.Band_Mo
+00007080: 6465 5f46 7261 6d65 5f52 5454 592e 6869  de_Frame_RTTY.hi
+00007090: 6465 2829 0a20 2020 2020 2020 206d 6f64  de().        mod
+000070a0: 6573 203d 207b 0a20 2020 2020 2020 2020  es = {.         
+000070b0: 2020 2022 4357 223a 2028 7365 6c66 2e42     "CW": (self.B
+000070c0: 616e 645f 4d6f 6465 5f46 7261 6d65 5f43  and_Mode_Frame_C
+000070d0: 572c 292c 0a20 2020 2020 2020 2020 2020  W,),.           
+000070e0: 2022 5353 4222 3a20 2873 656c 662e 4261   "SSB": (self.Ba
+000070f0: 6e64 5f4d 6f64 655f 4672 616d 655f 5353  nd_Mode_Frame_SS
+00007100: 422c 292c 0a20 2020 2020 2020 2020 2020  B,),.           
+00007110: 2022 5254 5459 223a 2028 7365 6c66 2e42   "RTTY": (self.B
+00007120: 616e 645f 4d6f 6465 5f46 7261 6d65 5f52  and_Mode_Frame_R
+00007130: 5454 592c 292c 0a20 2020 2020 2020 2020  TTY,),.         
+00007140: 2020 2022 5053 4b22 3a20 2873 656c 662e     "PSK": (self.
+00007150: 4261 6e64 5f4d 6f64 655f 4672 616d 655f  Band_Mode_Frame_
+00007160: 5254 5459 2c29 2c0a 2020 2020 2020 2020  RTTY,),.        
+00007170: 2020 2020 2253 5342 2b43 5722 3a20 2873      "SSB+CW": (s
 00007180: 656c 662e 4261 6e64 5f4d 6f64 655f 4672  elf.Band_Mode_Fr
 00007190: 616d 655f 4357 2c20 7365 6c66 2e42 616e  ame_CW, self.Ban
 000071a0: 645f 4d6f 6465 5f46 7261 6d65 5f53 5342  d_Mode_Frame_SSB
 000071b0: 292c 0a20 2020 2020 2020 2020 2020 2022  ),.            "
-000071c0: 4449 4749 5441 4c22 3a20 2873 656c 662e  DIGITAL": (self.
-000071d0: 4261 6e64 5f4d 6f64 655f 4672 616d 655f  Band_Mode_Frame_
-000071e0: 5254 5459 2c29 2c0a 2020 2020 2020 2020  RTTY,),.        
-000071f0: 2020 2020 2253 5342 2b43 572b 4449 4749      "SSB+CW+DIGI
-00007200: 5441 4c22 3a20 280a 2020 2020 2020 2020  TAL": (.        
-00007210: 2020 2020 2020 2020 7365 6c66 2e42 616e          self.Ban
-00007220: 645f 4d6f 6465 5f46 7261 6d65 5f52 5454  d_Mode_Frame_RTT
-00007230: 592c 0a20 2020 2020 2020 2020 2020 2020  Y,.             
-00007240: 2020 2073 656c 662e 4261 6e64 5f4d 6f64     self.Band_Mod
-00007250: 655f 4672 616d 655f 4357 2c0a 2020 2020  e_Frame_CW,.    
-00007260: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00007270: 2e42 616e 645f 4d6f 6465 5f46 7261 6d65  .Band_Mode_Frame
-00007280: 5f53 5342 2c0a 2020 2020 2020 2020 2020  _SSB,.          
-00007290: 2020 292c 0a20 2020 2020 2020 2020 2020    ),.           
-000072a0: 2022 464d 223a 2028 7365 6c66 2e42 616e   "FM": (self.Ban
-000072b0: 645f 4d6f 6465 5f46 7261 6d65 5f53 5342  d_Mode_Frame_SSB
-000072c0: 2c29 2c0a 2020 2020 2020 2020 7d0a 2020  ,),.        }.  
-000072d0: 2020 2020 2020 6672 616d 6573 203d 206d        frames = m
-000072e0: 6f64 6573 2e67 6574 2874 6865 5f6d 6f64  odes.get(the_mod
-000072f0: 6529 0a20 2020 2020 2020 2069 6620 6672  e).        if fr
-00007300: 616d 6573 3a0a 2020 2020 2020 2020 2020  ames:.          
-00007310: 2020 666f 7220 6672 616d 6520 696e 2066    for frame in f
-00007320: 7261 6d65 733a 0a20 2020 2020 2020 2020  rames:.         
-00007330: 2020 2020 2020 2066 7261 6d65 2e73 686f         frame.sho
-00007340: 7728 290a 0a20 2020 2064 6566 2073 686f  w()..    def sho
-00007350: 775f 6b65 795f 6865 6c70 2873 656c 6629  w_key_help(self)
-00007360: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
-00007370: 2020 2222 2253 686f 7720 6865 6c70 2062    """Show help b
-00007380: 6f78 2066 6f72 2068 6f74 6b65 7973 2222  ox for hotkeys""
-00007390: 220a 2020 2020 2020 2020 7365 6c66 2e73  ".        self.s
-000073a0: 686f 775f 6d65 7373 6167 655f 626f 7828  how_message_box(
-000073b0: 0a20 2020 2020 2020 2020 2020 2022 5b45  .            "[E
-000073c0: 7363 5d5c 7443 6c65 6172 7320 7468 6520  sc]\tClears the 
-000073d0: 696e 7075 7420 6669 656c 6473 206f 6620  input fields of 
-000073e0: 616e 7920 7465 7874 2e5c 6e22 0a20 2020  any text.\n".   
-000073f0: 2020 2020 2020 2020 2022 5b43 5452 4c2d           "[CTRL-
-00007400: 4573 635d 5c74 5374 6f70 7320 6377 6461  Esc]\tStops cwda
-00007410: 656d 6f6e 2066 726f 6d20 7365 6e64 696e  emon from sendin
-00007420: 6720 4d6f 7273 652e 5c6e 220a 2020 2020  g Morse.\n".    
-00007430: 2020 2020 2020 2020 225b 5067 5570 5d5c          "[PgUp]\
-00007440: 7449 6e63 7265 6173 6573 2074 6865 2063  tIncreases the c
-00007450: 7720 7365 6e64 696e 6720 7370 6565 642e  w sending speed.
-00007460: 5c6e 220a 2020 2020 2020 2020 2020 2020  \n".            
-00007470: 225b 5067 446f 776e 5d5c 7444 6563 7265  "[PgDown]\tDecre
-00007480: 6173 6573 2074 6865 2063 7720 7365 6e64  ases the cw send
-00007490: 696e 6720 7370 6565 642e 5c6e 220a 2020  ing speed.\n".  
-000074a0: 2020 2020 2020 2020 2020 225b 4172 726f            "[Arro
-000074b0: 772d 5570 5d20 4a75 6d70 2074 6f20 7468  w-Up] Jump to th
-000074c0: 6520 6e65 7874 2073 706f 7420 6162 6f76  e next spot abov
-000074d0: 6520 7468 6520 6375 7272 656e 7420 5646  e the current VF
-000074e0: 4f20 6375 7273 6f72 5c6e 220a 2020 2020  O cursor\n".    
-000074f0: 2020 2020 2020 2020 225c 7469 6e20 7468          "\tin th
-00007500: 6520 6261 6e64 6d61 7020 7769 6e64 6f77  e bandmap window
-00007510: 2028 4341 5420 5265 7175 6972 6564 292e   (CAT Required).
-00007520: 5c6e 220a 2020 2020 2020 2020 2020 2020  \n".            
-00007530: 225b 4172 726f 772d 446f 776e 5d20 4a75  "[Arrow-Down] Ju
-00007540: 6d70 2074 6f20 7468 6520 6e65 7874 2073  mp to the next s
-00007550: 706f 7420 6265 6c6f 7720 7468 6520 6375  pot below the cu
-00007560: 7272 656e 745c 6e22 0a20 2020 2020 2020  rrent\n".       
-00007570: 2020 2020 2022 5c74 5646 4f20 6375 7273       "\tVFO curs
-00007580: 6f72 2069 6e20 7468 6520 6261 6e64 6d61  or in the bandma
-00007590: 7020 7769 6e64 6f77 2028 4341 5420 5265  p window (CAT Re
-000075a0: 7175 6972 6564 292e 5c6e 220a 2020 2020  quired).\n".    
-000075b0: 2020 2020 2020 2020 225b 5441 425d 5c74          "[TAB]\t
-000075c0: 4d6f 7665 2063 7572 736f 7220 746f 2074  Move cursor to t
-000075d0: 6865 2072 6967 6874 206f 6e65 2066 6965  he right one fie
-000075e0: 6c64 2e5c 6e22 0a20 2020 2020 2020 2020  ld.\n".         
-000075f0: 2020 2022 5b53 6869 6674 2d54 6162 5d5c     "[Shift-Tab]\
-00007600: 744d 6f76 6520 6375 7273 6f72 206c 6566  tMove cursor lef
-00007610: 7420 4f6e 6520 6669 656c 642e 5c6e 220a  t One field.\n".
-00007620: 2020 2020 2020 2020 2020 2020 225b 5350              "[SP
-00007630: 4143 455d 5c74 5768 656e 2069 6e20 7468  ACE]\tWhen in th
-00007640: 6520 6361 6c6c 7369 676e 2066 6965 6c64  e callsign field
-00007650: 2c20 7769 6c6c 206d 6f76 6520 7468 6520  , will move the 
-00007660: 696e 7075 7420 746f 2074 6865 5c6e 220a  input to the\n".
-00007670: 2020 2020 2020 2020 2020 2020 225c 7466              "\tf
-00007680: 6972 7374 2066 6965 6c64 206e 6565 6465  irst field neede
-00007690: 6420 666f 7220 7468 6520 6578 6368 616e  d for the exchan
-000076a0: 6765 2e5c 6e22 0a20 2020 2020 2020 2020  ge.\n".         
-000076b0: 2020 2022 5b45 6e74 6572 5d5c 7453 7562     "[Enter]\tSub
-000076c0: 6d69 7473 2074 6865 2066 6965 6c64 7320  mits the fields 
-000076d0: 746f 2074 6865 206c 6f67 2e5c 6e22 0a20  to the log.\n". 
-000076e0: 2020 2020 2020 2020 2020 2022 5b46 312d             "[F1-
-000076f0: 4631 325d 5c74 5365 6e64 2028 4357 206f  F12]\tSend (CW o
-00007700: 7220 566f 6963 6529 206d 6163 726f 732e  r Voice) macros.
-00007710: 5c6e 220a 2020 2020 2020 2020 2020 2020  \n".            
-00007720: 225b 4354 524c 2d53 5d5c 7453 706f 7420  "[CTRL-S]\tSpot 
-00007730: 4361 6c6c 7369 676e 2074 6f20 7468 6520  Callsign to the 
-00007740: 636c 7573 7465 722e 5c6e 220a 2020 2020  cluster.\n".    
-00007750: 2020 2020 2020 2020 225b 4354 524c 2d47          "[CTRL-G
-00007760: 5d5c 7454 756e 6520 746f 2061 2073 706f  ]\tTune to a spo
-00007770: 7420 6d61 7463 6869 6e67 2070 6172 7469  t matching parti
-00007780: 616c 2074 6578 7420 696e 2074 6865 2063  al text in the c
-00007790: 616c 6c73 6967 6e5c 6e22 0a20 2020 2020  allsign\n".     
-000077a0: 2020 2020 2020 2022 5c74 656e 7472 7920         "\tentry 
-000077b0: 6669 656c 6420 2843 4154 2052 6571 7569  field (CAT Requi
-000077c0: 7265 6429 2e5c 6e22 0a20 2020 2020 2020  red).\n".       
-000077d0: 2029 0a0a 2020 2020 6465 6620 6669 6c65   )..    def file
-000077e0: 7069 636b 6572 2873 656c 662c 2061 6374  picker(self, act
-000077f0: 696f 6e3a 2073 7472 2920 2d3e 2073 7472  ion: str) -> str
-00007800: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-00007810: 2020 2020 2020 4765 7420 6120 6669 6c65        Get a file
-00007820: 6e61 6d65 0a20 2020 2020 2020 2061 6374  name.        act
-00007830: 696f 6e3a 2022 6e65 7722 206f 7220 226f  ion: "new" or "o
-00007840: 7065 6e22 0a20 2020 2020 2020 2022 2222  pen".        """
-00007850: 0a20 2020 2020 2020 206f 7074 696f 6e73  .        options
-00007860: 203d 2051 4669 6c65 4469 616c 6f67 2e4f   = QFileDialog.O
-00007870: 7074 696f 6e73 2829 0a20 2020 2020 2020  ptions().       
-00007880: 206f 7074 696f 6e73 207c 3d20 5146 696c   options |= QFil
-00007890: 6544 6961 6c6f 672e 446f 6e74 5573 654e  eDialog.DontUseN
-000078a0: 6174 6976 6544 6961 6c6f 670a 2020 2020  ativeDialog.    
-000078b0: 2020 2020 6f70 7469 6f6e 7320 7c3d 2051      options |= Q
-000078c0: 4669 6c65 4469 616c 6f67 2e44 6f6e 7443  FileDialog.DontC
-000078d0: 6f6e 6669 726d 4f76 6572 7772 6974 650a  onfirmOverwrite.
-000078e0: 2020 2020 2020 2020 6966 2061 6374 696f          if actio
-000078f0: 6e20 3d3d 2022 6e65 7722 3a0a 2020 2020  n == "new":.    
-00007900: 2020 2020 2020 2020 6669 6c65 2c20 5f20          file, _ 
-00007910: 3d20 5146 696c 6544 6961 6c6f 672e 6765  = QFileDialog.ge
-00007920: 7453 6176 6546 696c 654e 616d 6528 0a20  tSaveFileName(. 
-00007930: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00007940: 656c 662c 0a20 2020 2020 2020 2020 2020  elf,.           
-00007950: 2020 2020 2022 4368 6f6f 7365 2061 2044       "Choose a D
-00007960: 6174 6162 6173 6522 2c0a 2020 2020 2020  atabase",.      
-00007970: 2020 2020 2020 2020 2020 4441 5441 5f50            DATA_P
-00007980: 4154 482c 0a20 2020 2020 2020 2020 2020  ATH,.           
-00007990: 2020 2020 2022 4461 7461 6261 7365 2028       "Database (
-000079a0: 2a2e 6462 2922 2c0a 2020 2020 2020 2020  *.db)",.        
-000079b0: 2020 2020 2020 2020 6f70 7469 6f6e 733d          options=
-000079c0: 6f70 7469 6f6e 732c 0a20 2020 2020 2020  options,.       
-000079d0: 2020 2020 2029 0a20 2020 2020 2020 2069       ).        i
-000079e0: 6620 6163 7469 6f6e 203d 3d20 226f 7065  f action == "ope
-000079f0: 6e22 3a0a 2020 2020 2020 2020 2020 2020  n":.            
-00007a00: 6669 6c65 2c20 5f20 3d20 5146 696c 6544  file, _ = QFileD
-00007a10: 6961 6c6f 672e 6765 744f 7065 6e46 696c  ialog.getOpenFil
-00007a20: 654e 616d 6528 0a20 2020 2020 2020 2020  eName(.         
-00007a30: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
-00007a40: 2020 2020 2020 2020 2020 2020 2022 4368               "Ch
-00007a50: 6f6f 7365 2061 2044 6174 6162 6173 6522  oose a Database"
-00007a60: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00007a70: 2020 4441 5441 5f50 4154 482c 0a20 2020    DATA_PATH,.   
-00007a80: 2020 2020 2020 2020 2020 2020 2022 4461               "Da
-00007a90: 7461 6261 7365 2028 2a2e 6462 2922 2c0a  tabase (*.db)",.
-00007aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ab0: 6f70 7469 6f6e 733d 6f70 7469 6f6e 732c  options=options,
-00007ac0: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
-00007ad0: 2020 2020 2020 2072 6574 7572 6e20 6669         return fi
-00007ae0: 6c65 0a0a 2020 2020 6465 6620 7265 6361  le..    def reca
-00007af0: 6c63 756c 6174 655f 6d75 6c74 7328 7365  lculate_mults(se
-00007b00: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
-00007b10: 5265 6361 6c63 756c 6174 6520 4d75 6c74  Recalculate Mult
-00007b20: 6970 6c69 6572 7322 2222 0a20 2020 2020  ipliers""".     
-00007b30: 2020 2073 656c 662e 636f 6e74 6573 742e     self.contest.
-00007b40: 7265 6361 6c63 756c 6174 655f 6d75 6c74  recalculate_mult
-00007b50: 7328 7365 6c66 290a 0a20 2020 2064 6566  s(self)..    def
-00007b60: 206c 6175 6e63 685f 6c6f 675f 7769 6e64   launch_log_wind
-00007b70: 6f77 2873 656c 6629 3a0a 2020 2020 2020  ow(self):.      
-00007b80: 2020 2222 226c 6175 6e63 6820 7468 6520    """launch the 
-00007b90: 4c6f 6720 5769 6e64 6f77 2222 220a 2020  Log Window""".  
-00007ba0: 2020 2020 2020 6966 206e 6f74 2063 6865        if not che
-00007bb0: 636b 5f70 726f 6365 7373 2822 6c6f 6777  ck_process("logw
-00007bc0: 696e 646f 772e 7079 2229 3a0a 2020 2020  indow.py"):.    
-00007bd0: 2020 2020 2020 2020 5f20 3d20 7375 6270          _ = subp
-00007be0: 726f 6365 7373 2e50 6f70 656e 285b 7379  rocess.Popen([sy
-00007bf0: 732e 6578 6563 7574 6162 6c65 2c20 574f  s.executable, WO
-00007c00: 524b 494e 475f 5041 5448 202b 2022 2f6c  RKING_PATH + "/l
-00007c10: 6f67 7769 6e64 6f77 2e70 7922 5d29 0a0a  ogwindow.py"])..
-00007c20: 2020 2020 6465 6620 6c61 756e 6368 5f62      def launch_b
-00007c30: 616e 646d 6170 5f77 696e 646f 7728 7365  andmap_window(se
-00007c40: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
-00007c50: 6c61 756e 6368 2074 6865 204c 6f67 2057  launch the Log W
-00007c60: 696e 646f 7722 2222 0a20 2020 2020 2020  indow""".       
-00007c70: 2069 6620 6e6f 7420 6368 6563 6b5f 7072   if not check_pr
-00007c80: 6f63 6573 7328 2262 616e 646d 6170 2e70  ocess("bandmap.p
-00007c90: 7922 293a 0a20 2020 2020 2020 2020 2020  y"):.           
-00007ca0: 205f 203d 2073 7562 7072 6f63 6573 732e   _ = subprocess.
-00007cb0: 506f 7065 6e28 5b73 7973 2e65 7865 6375  Popen([sys.execu
-00007cc0: 7461 626c 652c 2057 4f52 4b49 4e47 5f50  table, WORKING_P
-00007cd0: 4154 4820 2b20 222f 6261 6e64 6d61 702e  ATH + "/bandmap.
-00007ce0: 7079 225d 290a 0a20 2020 2064 6566 2063  py"])..    def c
-00007cf0: 6c65 6172 5f62 616e 645f 696e 6469 6361  lear_band_indica
-00007d00: 746f 7273 2873 656c 6629 3a0a 2020 2020  tors(self):.    
-00007d10: 2020 2020 2222 2243 6c65 6172 2074 6865      """Clear the
-00007d20: 2069 6e64 6963 6174 6f72 7322 2222 0a20   indicators""". 
-00007d30: 2020 2020 2020 2066 6f72 205f 2c20 696e         for _, in
-00007d40: 6469 6361 746f 7273 2069 6e20 7365 6c66  dicators in self
-00007d50: 2e61 6c6c 5f6d 6f64 655f 696e 6469 6361  .all_mode_indica
-00007d60: 746f 7273 2e69 7465 6d73 2829 3a0a 2020  tors.items():.  
-00007d70: 2020 2020 2020 2020 2020 666f 7220 5f2c            for _,
-00007d80: 2069 6e64 6963 6174 6f72 2069 6e20 696e   indicator in in
-00007d90: 6469 6361 746f 7273 2e69 7465 6d73 2829  dicators.items()
-00007da0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00007db0: 2020 696e 6469 6361 746f 722e 7365 7446    indicator.setF
-00007dc0: 7261 6d65 5368 6170 6528 5174 5769 6467  rameShape(QtWidg
-00007dd0: 6574 732e 5146 7261 6d65 2e4e 6f46 7261  ets.QFrame.NoFra
-00007de0: 6d65 290a 2020 2020 2020 2020 2020 2020  me).            
-00007df0: 2020 2020 696e 6469 6361 746f 722e 7365      indicator.se
-00007e00: 7453 7479 6c65 5368 6565 7428 2266 6f6e  tStyleSheet("fon
-00007e10: 742d 6661 6d69 6c79 3a20 4a65 7442 7261  t-family: JetBra
-00007e20: 696e 7320 4d6f 6e6f 3b22 290a 0a20 2020  ins Mono;")..   
-00007e30: 2064 6566 2073 6574 5f62 616e 645f 696e   def set_band_in
-00007e40: 6469 6361 746f 7228 7365 6c66 2c20 6261  dicator(self, ba
-00007e50: 6e64 3a20 7374 7229 202d 3e20 4e6f 6e65  nd: str) -> None
-00007e60: 3a0a 2020 2020 2020 2020 2222 2253 6574  :.        """Set
-00007e70: 2074 6865 2062 616e 6420 696e 6469 6361   the band indica
-00007e80: 746f 7222 2222 0a20 2020 2020 2020 2023  tor""".        #
-00007e90: 206c 6f67 6765 722e 6465 6275 6728 2225   logger.debug("%
-00007ea0: 7322 2c20 6622 6261 6e64 3a7b 6261 6e64  s", f"band:{band
-00007eb0: 7d20 6d6f 6465 3a20 7b73 656c 662e 6375  } mode: {self.cu
-00007ec0: 7272 656e 745f 6d6f 6465 7d22 290a 2020  rrent_mode}").  
-00007ed0: 2020 2020 2020 6966 2062 616e 6420 616e        if band an
-00007ee0: 6420 7365 6c66 2e63 7572 7265 6e74 5f6d  d self.current_m
-00007ef0: 6f64 653a 0a20 2020 2020 2020 2020 2020  ode:.           
-00007f00: 2073 656c 662e 636c 6561 725f 6261 6e64   self.clear_band
-00007f10: 5f69 6e64 6963 6174 6f72 7328 290a 2020  _indicators().  
-00007f20: 2020 2020 2020 2020 2020 696e 6469 6361            indica
-00007f30: 746f 7220 3d20 7365 6c66 2e61 6c6c 5f6d  tor = self.all_m
-00007f40: 6f64 655f 696e 6469 6361 746f 7273 5b73  ode_indicators[s
-00007f50: 656c 662e 6375 7272 656e 745f 6d6f 6465  elf.current_mode
-00007f60: 5d2e 6765 7428 6261 6e64 2c20 4e6f 6e65  ].get(band, None
-00007f70: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
-00007f80: 2069 6e64 6963 6174 6f72 3a0a 2020 2020   indicator:.    
-00007f90: 2020 2020 2020 2020 2020 2020 696e 6469              indi
-00007fa0: 6361 746f 722e 7365 7446 7261 6d65 5368  cator.setFrameSh
-00007fb0: 6170 6528 5174 5769 6467 6574 732e 5146  ape(QtWidgets.QF
-00007fc0: 7261 6d65 2e42 6f78 290a 2020 2020 2020  rame.Box).      
-00007fd0: 2020 2020 2020 2020 2020 696e 6469 6361            indica
-00007fe0: 746f 722e 7365 7453 7479 6c65 5368 6565  tor.setStyleShee
-00007ff0: 7428 2266 6f6e 742d 6661 6d69 6c79 3a20  t("font-family: 
-00008000: 4a65 7442 7261 696e 7320 4d6f 6e6f 3b20  JetBrains Mono; 
-00008010: 636f 6c6f 723a 2067 7265 656e 3b22 290a  color: green;").
-00008020: 0a20 2020 2064 6566 2063 6c6f 7365 4576  .    def closeEv
-00008030: 656e 7428 7365 6c66 2c20 5f65 7665 6e74  ent(self, _event
-00008040: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
-00008050: 2020 2020 2020 2057 7269 7465 2077 696e         Write win
-00008060: 646f 7720 7369 7a65 2061 6e64 2070 6f73  dow size and pos
-00008070: 6974 696f 6e20 746f 2063 6f6e 6669 6720  ition to config 
-00008080: 6669 6c65 0a20 2020 2020 2020 2022 2222  file.        """
-00008090: 0a20 2020 2020 2020 2073 656c 662e 7072  .        self.pr
-000080a0: 6566 5b22 7769 6e64 6f77 5f77 6964 7468  ef["window_width
-000080b0: 225d 203d 2073 656c 662e 7369 7a65 2829  "] = self.size()
-000080c0: 2e77 6964 7468 2829 0a20 2020 2020 2020  .width().       
-000080d0: 2073 656c 662e 7072 6566 5b22 7769 6e64   self.pref["wind
-000080e0: 6f77 5f68 6569 6768 7422 5d20 3d20 7365  ow_height"] = se
-000080f0: 6c66 2e73 697a 6528 292e 6865 6967 6874  lf.size().height
-00008100: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
-00008110: 7072 6566 5b22 7769 6e64 6f77 5f78 225d  pref["window_x"]
-00008120: 203d 2073 656c 662e 706f 7328 292e 7828   = self.pos().x(
-00008130: 290a 2020 2020 2020 2020 7365 6c66 2e70  ).        self.p
-00008140: 7265 665b 2277 696e 646f 775f 7922 5d20  ref["window_y"] 
-00008150: 3d20 7365 6c66 2e70 6f73 2829 2e79 2829  = self.pos().y()
-00008160: 0a20 2020 2020 2020 2073 656c 662e 7772  .        self.wr
-00008170: 6974 655f 7072 6566 6572 656e 6365 2829  ite_preference()
-00008180: 0a0a 2020 2020 6465 6620 6374 795f 6c6f  ..    def cty_lo
-00008190: 6f6b 7570 2873 656c 662c 2063 616c 6c73  okup(self, calls
-000081a0: 6967 6e3a 2073 7472 293a 0a20 2020 2020  ign: str):.     
-000081b0: 2020 2022 2222 4c6f 6f6b 7570 2063 616c     """Lookup cal
-000081c0: 6c73 6967 6e20 696e 2063 7479 2e64 6174  lsign in cty.dat
-000081d0: 2066 696c 652e 0a0a 2020 2020 2020 2020   file...        
-000081e0: 5061 7261 6d65 7465 7273 0a20 2020 2020  Parameters.     
-000081f0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
-00008200: 2020 2020 2020 6361 6c6c 7369 676e 203a        callsign :
-00008210: 2073 7472 0a0a 2020 2020 2020 2020 5265   str..        Re
-00008220: 7475 726e 730a 2020 2020 2020 2020 2d2d  turns.        --
-00008230: 2d2d 2d2d 2d0a 2020 2020 2020 2020 7265  -----.        re
-00008240: 7475 726e 203a 206c 6973 7420 6f66 2064  turn : list of d
-00008250: 6963 7473 0a20 2020 2020 2020 2022 2222  icts.        """
-00008260: 0a20 2020 2020 2020 2063 616c 6c73 6967  .        callsig
-00008270: 6e20 3d20 6361 6c6c 7369 676e 2e75 7070  n = callsign.upp
-00008280: 6572 2829 0a20 2020 2020 2020 2066 6f72  er().        for
-00008290: 2063 6f75 6e74 2069 6e20 7265 7665 7273   count in revers
-000082a0: 6564 2872 616e 6765 286c 656e 2863 616c  ed(range(len(cal
-000082b0: 6c73 6967 6e29 2929 3a0a 2020 2020 2020  lsign))):.      
-000082c0: 2020 2020 2020 7365 6172 6368 6974 656d        searchitem
-000082d0: 203d 2063 616c 6c73 6967 6e5b 3a20 636f   = callsign[: co
-000082e0: 756e 7420 2b20 315d 0a20 2020 2020 2020  unt + 1].       
-000082f0: 2020 2020 2072 6573 756c 7420 3d20 7b6b       result = {k
-00008300: 6579 3a20 7661 6c20 666f 7220 6b65 792c  ey: val for key,
-00008310: 2076 616c 2069 6e20 4354 5946 494c 452e   val in CTYFILE.
-00008320: 6974 656d 7328 2920 6966 206b 6579 203d  items() if key =
-00008330: 3d20 7365 6172 6368 6974 656d 7d0a 2020  = searchitem}.  
-00008340: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
-00008350: 2072 6573 756c 743a 0a20 2020 2020 2020   result:.       
-00008360: 2020 2020 2020 2020 2063 6f6e 7469 6e75           continu
-00008370: 650a 2020 2020 2020 2020 2020 2020 6966  e.            if
-00008380: 2072 6573 756c 742e 6765 7428 7365 6172   result.get(sear
-00008390: 6368 6974 656d 292e 6765 7428 2265 7861  chitem).get("exa
-000083a0: 6374 5f6d 6174 6368 2229 3a0a 2020 2020  ct_match"):.    
-000083b0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-000083c0: 6561 7263 6869 7465 6d20 3d3d 2063 616c  earchitem == cal
-000083d0: 6c73 6967 6e3a 0a20 2020 2020 2020 2020  lsign:.         
-000083e0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-000083f0: 6e20 7265 7375 6c74 0a20 2020 2020 2020  n result.       
-00008400: 2020 2020 2020 2020 2063 6f6e 7469 6e75           continu
-00008410: 650a 2020 2020 2020 2020 2020 2020 7265  e.            re
-00008420: 7475 726e 2072 6573 756c 740a 0a20 2020  turn result..   
-00008430: 2064 6566 2063 7773 7065 6564 5f73 7069   def cwspeed_spi
-00008440: 6e62 6f78 5f63 6861 6e67 6564 2873 656c  nbox_changed(sel
-00008450: 6629 3a0a 2020 2020 2020 2020 2222 2274  f):.        """t
-00008460: 7269 6767 6572 6564 2077 6865 6e20 7661  riggered when va
-00008470: 6c75 6520 6f66 2043 5720 7370 6565 6420  lue of CW speed 
-00008480: 696e 2074 6865 2073 7069 6e62 6f78 2063  in the spinbox c
-00008490: 6861 6e67 6573 2e22 2222 0a20 2020 2020  hanges.""".     
-000084a0: 2020 2069 6620 7365 6c66 2e63 7720 6973     if self.cw is
-000084b0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-000084c0: 2020 2072 6574 7572 6e0a 2020 2020 2020     return.      
-000084d0: 2020 6966 2073 656c 662e 6377 2e73 6572    if self.cw.ser
-000084e0: 7665 7274 7970 6520 3d3d 2031 3a0a 2020  vertype == 1:.  
-000084f0: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-00008500: 772e 7370 6565 6420 3d20 7365 6c66 2e63  w.speed = self.c
-00008510: 775f 7370 6565 642e 7661 6c75 6528 290a  w_speed.value().
-00008520: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00008530: 2e63 772e 7365 6e64 6377 2866 225c 7831  .cw.sendcw(f"\x1
-00008540: 6232 7b73 656c 662e 6377 2e73 7065 6564  b2{self.cw.speed
-00008550: 7d22 290a 2020 2020 2020 2020 6966 2073  }").        if s
-00008560: 656c 662e 6377 2e73 6572 7665 7274 7970  elf.cw.servertyp
-00008570: 6520 3d3d 2032 3a0a 2020 2020 2020 2020  e == 2:.        
-00008580: 2020 2020 7365 6c66 2e63 772e 7365 745f      self.cw.set_
-00008590: 7769 6e6b 6579 6572 5f73 7065 6564 2873  winkeyer_speed(s
-000085a0: 656c 662e 6377 5f73 7065 6564 2e76 616c  elf.cw_speed.val
-000085b0: 7565 2829 290a 0a20 2020 2064 6566 206b  ue())..    def k
-000085c0: 6579 5072 6573 7345 7665 6e74 2873 656c  eyPressEvent(sel
-000085d0: 662c 2065 7665 6e74 293a 2020 2320 7079  f, event):  # py
-000085e0: 6c69 6e74 3a20 6469 7361 626c 653d 696e  lint: disable=in
-000085f0: 7661 6c69 642d 6e61 6d65 0a20 2020 2020  valid-name.     
-00008600: 2020 2022 2222 5468 6973 206f 7665 7272     """This overr
-00008610: 6964 6573 2051 7420 6b65 7920 6576 656e  ides Qt key even
-00008620: 742e 2222 220a 2020 2020 2020 2020 6d6f  t.""".        mo
-00008630: 6469 6669 6572 203d 2065 7665 6e74 2e6d  difier = event.m
-00008640: 6f64 6966 6965 7273 2829 0a20 2020 2020  odifiers().     
-00008650: 2020 2069 6620 6576 656e 742e 6b65 7928     if event.key(
-00008660: 2920 3d3d 2051 742e 4b65 795f 5320 616e  ) == Qt.Key_S an
-00008670: 6420 6d6f 6469 6669 6572 203d 3d20 5174  d modifier == Qt
-00008680: 2e43 6f6e 7472 6f6c 4d6f 6469 6669 6572  .ControlModifier
-00008690: 3a0a 2020 2020 2020 2020 2020 2020 6672  :.            fr
-000086a0: 6571 203d 2073 656c 662e 7261 6469 6f5f  eq = self.radio_
-000086b0: 7374 6174 652e 6765 7428 2276 666f 6122  state.get("vfoa"
-000086c0: 290a 2020 2020 2020 2020 2020 2020 6478  ).            dx
-000086d0: 203d 2073 656c 662e 6361 6c6c 7369 676e   = self.callsign
-000086e0: 2e74 6578 7428 290a 2020 2020 2020 2020  .text().        
-000086f0: 2020 2020 6966 2066 7265 7120 616e 6420      if freq and 
-00008700: 6478 3a0a 2020 2020 2020 2020 2020 2020  dx:.            
-00008710: 2020 2020 636d 6420 3d20 7b7d 0a20 2020      cmd = {}.   
-00008720: 2020 2020 2020 2020 2020 2020 2063 6d64               cmd
-00008730: 5b22 636d 6422 5d20 3d20 2253 504f 5444  ["cmd"] = "SPOTD
-00008740: 5822 0a20 2020 2020 2020 2020 2020 2020  X".             
-00008750: 2020 2063 6d64 5b22 7374 6174 696f 6e22     cmd["station"
-00008760: 5d20 3d20 706c 6174 666f 726d 2e6e 6f64  ] = platform.nod
-00008770: 6528 290a 2020 2020 2020 2020 2020 2020  e().            
-00008780: 2020 2020 636d 645b 2264 7822 5d20 3d20      cmd["dx"] = 
-00008790: 6478 0a20 2020 2020 2020 2020 2020 2020  dx.             
-000087a0: 2020 2063 6d64 5b22 6672 6571 225d 203d     cmd["freq"] =
-000087b0: 2066 6c6f 6174 2869 6e74 2866 7265 7129   float(int(freq)
-000087c0: 202f 2031 3030 3029 0a20 2020 2020 2020   / 1000).       
-000087d0: 2020 2020 2020 2020 2073 656c 662e 6d75           self.mu
-000087e0: 6c74 6963 6173 745f 696e 7465 7266 6163  lticast_interfac
-000087f0: 652e 7365 6e64 5f61 735f 6a73 6f6e 2863  e.send_as_json(c
-00008800: 6d64 290a 2020 2020 2020 2020 2020 2020  md).            
-00008810: 7265 7475 726e 0a20 2020 2020 2020 2069  return.        i
-00008820: 6620 6576 656e 742e 6b65 7928 2920 3d3d  f event.key() ==
-00008830: 2051 742e 4b65 795f 4720 616e 6420 6d6f   Qt.Key_G and mo
-00008840: 6469 6669 6572 203d 3d20 5174 2e43 6f6e  difier == Qt.Con
-00008850: 7472 6f6c 4d6f 6469 6669 6572 3a0a 2020  trolModifier:.  
-00008860: 2020 2020 2020 2020 2020 6478 203d 2073            dx = s
-00008870: 656c 662e 6361 6c6c 7369 676e 2e74 6578  elf.callsign.tex
-00008880: 7428 290a 2020 2020 2020 2020 2020 2020  t().            
-00008890: 6966 2064 783a 0a20 2020 2020 2020 2020  if dx:.         
-000088a0: 2020 2020 2020 2063 6d64 203d 207b 7d0a         cmd = {}.
-000088b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000088c0: 636d 645b 2263 6d64 225d 203d 2022 4649  cmd["cmd"] = "FI
-000088d0: 4e44 4458 220a 2020 2020 2020 2020 2020  NDDX".          
-000088e0: 2020 2020 2020 636d 645b 2273 7461 7469        cmd["stati
-000088f0: 6f6e 225d 203d 2070 6c61 7466 6f72 6d2e  on"] = platform.
-00008900: 6e6f 6465 2829 0a20 2020 2020 2020 2020  node().         
-00008910: 2020 2020 2020 2063 6d64 5b22 6478 225d         cmd["dx"]
-00008920: 203d 2064 780a 2020 2020 2020 2020 2020   = dx.          
-00008930: 2020 2020 2020 7365 6c66 2e6d 756c 7469        self.multi
-00008940: 6361 7374 5f69 6e74 6572 6661 6365 2e73  cast_interface.s
-00008950: 656e 645f 6173 5f6a 736f 6e28 636d 6429  end_as_json(cmd)
-00008960: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00008970: 7572 6e0a 2020 2020 2020 2020 6966 2028  urn.        if (
-00008980: 0a20 2020 2020 2020 2020 2020 2065 7665  .            eve
-00008990: 6e74 2e6b 6579 2829 203d 3d20 5174 2e4b  nt.key() == Qt.K
-000089a0: 6579 2e4b 6579 5f45 7363 6170 6520 616e  ey.Key_Escape an
-000089b0: 6420 6d6f 6469 6669 6572 2021 3d20 5174  d modifier != Qt
-000089c0: 2e43 6f6e 7472 6f6c 4d6f 6469 6669 6572  .ControlModifier
-000089d0: 0a20 2020 2020 2020 2029 3a20 2023 2070  .        ):  # p
-000089e0: 796c 696e 743a 2064 6973 6162 6c65 3d6e  ylint: disable=n
-000089f0: 6f2d 6d65 6d62 6572 0a20 2020 2020 2020  o-member.       
-00008a00: 2020 2020 2073 656c 662e 636c 6561 7269       self.cleari
-00008a10: 6e70 7574 7328 290a 2020 2020 2020 2020  nputs().        
-00008a20: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
-00008a30: 2020 2069 6620 6576 656e 742e 6b65 7928     if event.key(
-00008a40: 2920 3d3d 2051 742e 4b65 792e 4b65 795f  ) == Qt.Key.Key_
-00008a50: 4573 6361 7065 2061 6e64 206d 6f64 6966  Escape and modif
-00008a60: 6965 7220 3d3d 2051 742e 436f 6e74 726f  ier == Qt.Contro
-00008a70: 6c4d 6f64 6966 6965 723a 0a20 2020 2020  lModifier:.     
-00008a80: 2020 2020 2020 2069 6620 7365 6c66 2e63         if self.c
-00008a90: 7720 6973 206e 6f74 204e 6f6e 653a 0a20  w is not None:. 
-00008aa0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00008ab0: 6620 7365 6c66 2e63 772e 7365 7276 6572  f self.cw.server
-00008ac0: 7479 7065 203d 3d20 313a 0a20 2020 2020  type == 1:.     
-00008ad0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00008ae0: 656c 662e 6377 2e73 656e 6463 7728 225c  elf.cw.sendcw("\
-00008af0: 7831 6234 2229 0a20 2020 2020 2020 2020  x1b4").         
-00008b00: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00008b10: 6e0a 2020 2020 2020 2020 6966 2065 7665  n.        if eve
-00008b20: 6e74 2e6b 6579 2829 203d 3d20 5174 2e4b  nt.key() == Qt.K
-00008b30: 6579 2e4b 6579 5f55 703a 0a20 2020 2020  ey.Key_Up:.     
-00008b40: 2020 2020 2020 2063 6d64 203d 207b 7d0a         cmd = {}.
-00008b50: 2020 2020 2020 2020 2020 2020 636d 645b              cmd[
-00008b60: 2263 6d64 225d 203d 2022 5052 4556 5350  "cmd"] = "PREVSP
-00008b70: 4f54 220a 2020 2020 2020 2020 2020 2020  OT".            
-00008b80: 636d 645b 2273 7461 7469 6f6e 225d 203d  cmd["station"] =
-00008b90: 2070 6c61 7466 6f72 6d2e 6e6f 6465 2829   platform.node()
-00008ba0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00008bb0: 662e 6d75 6c74 6963 6173 745f 696e 7465  f.multicast_inte
-00008bc0: 7266 6163 652e 7365 6e64 5f61 735f 6a73  rface.send_as_js
-00008bd0: 6f6e 2863 6d64 290a 2020 2020 2020 2020  on(cmd).        
-00008be0: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
-00008bf0: 2020 2069 6620 6576 656e 742e 6b65 7928     if event.key(
-00008c00: 2920 3d3d 2051 742e 4b65 792e 4b65 795f  ) == Qt.Key.Key_
-00008c10: 446f 776e 3a0a 2020 2020 2020 2020 2020  Down:.          
-00008c20: 2020 636d 6420 3d20 7b7d 0a20 2020 2020    cmd = {}.     
-00008c30: 2020 2020 2020 2063 6d64 5b22 636d 6422         cmd["cmd"
-00008c40: 5d20 3d20 224e 4558 5453 504f 5422 0a20  ] = "NEXTSPOT". 
-00008c50: 2020 2020 2020 2020 2020 2063 6d64 5b22             cmd["
-00008c60: 7374 6174 696f 6e22 5d20 3d20 706c 6174  station"] = plat
-00008c70: 666f 726d 2e6e 6f64 6528 290a 2020 2020  form.node().    
-00008c80: 2020 2020 2020 2020 7365 6c66 2e6d 756c          self.mul
-00008c90: 7469 6361 7374 5f69 6e74 6572 6661 6365  ticast_interface
-00008ca0: 2e73 656e 645f 6173 5f6a 736f 6e28 636d  .send_as_json(cm
-00008cb0: 6429 0a20 2020 2020 2020 2020 2020 2072  d).            r
-00008cc0: 6574 7572 6e0a 2020 2020 2020 2020 6966  eturn.        if
-00008cd0: 2065 7665 6e74 2e6b 6579 2829 203d 3d20   event.key() == 
-00008ce0: 5174 2e4b 6579 2e4b 6579 5f50 6167 6555  Qt.Key.Key_PageU
-00008cf0: 7020 616e 6420 6d6f 6469 6669 6572 2021  p and modifier !
-00008d00: 3d20 5174 2e43 6f6e 7472 6f6c 4d6f 6469  = Qt.ControlModi
-00008d10: 6669 6572 3a0a 2020 2020 2020 2020 2020  fier:.          
-00008d20: 2020 6966 2073 656c 662e 6377 2069 7320    if self.cw is 
-00008d30: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00008d40: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-00008d50: 772e 7370 6565 6420 2b3d 2031 0a20 2020  w.speed += 1.   
-00008d60: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00008d70: 662e 6377 5f73 7065 6564 2e73 6574 5661  f.cw_speed.setVa
-00008d80: 6c75 6528 7365 6c66 2e63 772e 7370 6565  lue(self.cw.spee
-00008d90: 6429 0a20 2020 2020 2020 2020 2020 2020  d).             
-00008da0: 2020 2069 6620 7365 6c66 2e63 772e 7365     if self.cw.se
-00008db0: 7276 6572 7479 7065 203d 3d20 313a 0a20  rvertype == 1:. 
-00008dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008dd0: 2020 2073 656c 662e 6377 2e73 656e 6463     self.cw.sendc
-00008de0: 7728 6622 5c78 3162 327b 7365 6c66 2e63  w(f"\x1b2{self.c
-00008df0: 772e 7370 6565 647d 2229 0a20 2020 2020  w.speed}").     
-00008e00: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-00008e10: 6c66 2e63 772e 7365 7276 6572 7479 7065  lf.cw.servertype
-00008e20: 203d 3d20 323a 0a20 2020 2020 2020 2020   == 2:.         
-00008e30: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00008e40: 6377 2e73 6574 5f77 696e 6b65 7965 725f  cw.set_winkeyer_
-00008e50: 7370 6565 6428 7365 6c66 2e63 775f 7370  speed(self.cw_sp
-00008e60: 6565 642e 7661 6c75 6528 2929 0a20 2020  eed.value()).   
-00008e70: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
-00008e80: 2020 2020 2020 2020 6966 2065 7665 6e74          if event
-00008e90: 2e6b 6579 2829 203d 3d20 5174 2e4b 6579  .key() == Qt.Key
-00008ea0: 2e4b 6579 5f50 6167 6544 6f77 6e20 616e  .Key_PageDown an
-00008eb0: 6420 6d6f 6469 6669 6572 2021 3d20 5174  d modifier != Qt
-00008ec0: 2e43 6f6e 7472 6f6c 4d6f 6469 6669 6572  .ControlModifier
-00008ed0: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
-00008ee0: 2073 656c 662e 6377 2069 7320 6e6f 7420   self.cw is not 
-00008ef0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00008f00: 2020 2020 2020 7365 6c66 2e63 772e 7370        self.cw.sp
-00008f10: 6565 6420 2d3d 2031 0a20 2020 2020 2020  eed -= 1.       
-00008f20: 2020 2020 2020 2020 2073 656c 662e 6377           self.cw
-00008f30: 5f73 7065 6564 2e73 6574 5661 6c75 6528  _speed.setValue(
-00008f40: 7365 6c66 2e63 772e 7370 6565 6429 0a20  self.cw.speed). 
-00008f50: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00008f60: 6620 7365 6c66 2e63 772e 7365 7276 6572  f self.cw.server
-00008f70: 7479 7065 203d 3d20 313a 0a20 2020 2020  type == 1:.     
-00008f80: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00008f90: 656c 662e 6377 2e73 656e 6463 7728 6622  elf.cw.sendcw(f"
-00008fa0: 5c78 3162 327b 7365 6c66 2e63 772e 7370  \x1b2{self.cw.sp
-00008fb0: 6565 647d 2229 0a20 2020 2020 2020 2020  eed}").         
-00008fc0: 2020 2020 2020 2069 6620 7365 6c66 2e63         if self.c
-00008fd0: 772e 7365 7276 6572 7479 7065 203d 3d20  w.servertype == 
-00008fe0: 323a 0a20 2020 2020 2020 2020 2020 2020  2:.             
-00008ff0: 2020 2020 2020 2073 656c 662e 6377 2e73         self.cw.s
-00009000: 6574 5f77 696e 6b65 7965 725f 7370 6565  et_winkeyer_spee
-00009010: 6428 7365 6c66 2e63 775f 7370 6565 642e  d(self.cw_speed.
-00009020: 7661 6c75 6528 2929 0a20 2020 2020 2020  value()).       
-00009030: 2020 2020 2072 6574 7572 6e0a 2020 2020       return.    
-00009040: 2020 2020 2320 6966 2065 7665 6e74 2e6b      # if event.k
-00009050: 6579 2829 203d 3d20 5174 2e4b 6579 2e4b  ey() == Qt.Key.K
-00009060: 6579 5f45 6e74 6572 3a0a 2020 2020 2020  ey_Enter:.      
-00009070: 2020 2320 2020 2020 7365 6c66 2e73 6176    #     self.sav
-00009080: 655f 636f 6e74 6163 7428 290a 2020 2020  e_contact().    
-00009090: 2020 2020 6966 2065 7665 6e74 2e6b 6579      if event.key
-000090a0: 2829 203d 3d20 5174 2e4b 6579 2e4b 6579  () == Qt.Key.Key
-000090b0: 5f54 6162 206f 7220 6576 656e 742e 6b65  _Tab or event.ke
-000090c0: 7928 2920 3d3d 2051 742e 4b65 792e 4b65  y() == Qt.Key.Ke
-000090d0: 795f 4261 636b 7461 623a 0a20 2020 2020  y_Backtab:.     
-000090e0: 2020 2020 2020 2069 6620 7365 6c66 2e73         if self.s
-000090f0: 656e 742e 6861 7346 6f63 7573 2829 3a0a  ent.hasFocus():.
-00009100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009110: 6c6f 6767 6572 2e64 6562 7567 2822 4672  logger.debug("Fr
-00009120: 6f6d 2073 656e 7422 290a 2020 2020 2020  om sent").      
-00009130: 2020 2020 2020 2020 2020 6966 206d 6f64            if mod
-00009140: 6966 6965 7220 3d3d 2051 742e 5368 6966  ifier == Qt.Shif
-00009150: 744d 6f64 6966 6965 723a 0a20 2020 2020  tModifier:.     
-00009160: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00009170: 7265 765f 7461 6220 3d20 7365 6c66 2e74  rev_tab = self.t
-00009180: 6162 5f70 7265 762e 6765 7428 7365 6c66  ab_prev.get(self
-00009190: 2e73 656e 7429 0a20 2020 2020 2020 2020  .sent).         
-000091a0: 2020 2020 2020 2020 2020 2070 7265 765f             prev_
-000091b0: 7461 622e 7365 7446 6f63 7573 2829 0a20  tab.setFocus(). 
-000091c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000091d0: 2020 2070 7265 765f 7461 622e 6465 7365     prev_tab.dese
-000091e0: 6c65 6374 2829 0a20 2020 2020 2020 2020  lect().         
-000091f0: 2020 2020 2020 2020 2020 2070 7265 765f             prev_
-00009200: 7461 622e 656e 6428 4661 6c73 6529 0a20  tab.end(False). 
-00009210: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00009220: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00009230: 2020 2020 2020 2020 206e 6578 745f 7461           next_ta
-00009240: 6220 3d20 7365 6c66 2e74 6162 5f6e 6578  b = self.tab_nex
-00009250: 742e 6765 7428 7365 6c66 2e73 656e 7429  t.get(self.sent)
-00009260: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009270: 2020 2020 206e 6578 745f 7461 622e 7365       next_tab.se
-00009280: 7446 6f63 7573 2829 0a20 2020 2020 2020  tFocus().       
-00009290: 2020 2020 2020 2020 2020 2020 206e 6578               nex
-000092a0: 745f 7461 622e 6465 7365 6c65 6374 2829  t_tab.deselect()
-000092b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000092c0: 2020 2020 206e 6578 745f 7461 622e 656e       next_tab.en
-000092d0: 6428 4661 6c73 6529 0a20 2020 2020 2020  d(False).       
-000092e0: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
-000092f0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-00009300: 656c 662e 7265 6365 6976 652e 6861 7346  elf.receive.hasF
-00009310: 6f63 7573 2829 3a0a 2020 2020 2020 2020  ocus():.        
-00009320: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
-00009330: 6562 7567 2822 4672 6f6d 2072 6563 6569  ebug("From recei
-00009340: 7665 2229 0a20 2020 2020 2020 2020 2020  ve").           
-00009350: 2020 2020 2069 6620 6d6f 6469 6669 6572       if modifier
-00009360: 203d 3d20 5174 2e53 6869 6674 4d6f 6469   == Qt.ShiftModi
-00009370: 6669 6572 3a0a 2020 2020 2020 2020 2020  fier:.          
-00009380: 2020 2020 2020 2020 2020 7072 6576 5f74            prev_t
-00009390: 6162 203d 2073 656c 662e 7461 625f 7072  ab = self.tab_pr
-000093a0: 6576 2e67 6574 2873 656c 662e 7265 6365  ev.get(self.rece
-000093b0: 6976 6529 0a20 2020 2020 2020 2020 2020  ive).           
-000093c0: 2020 2020 2020 2020 2070 7265 765f 7461           prev_ta
-000093d0: 622e 7365 7446 6f63 7573 2829 0a20 2020  b.setFocus().   
-000093e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000093f0: 2070 7265 765f 7461 622e 6465 7365 6c65   prev_tab.desele
-00009400: 6374 2829 0a20 2020 2020 2020 2020 2020  ct().           
-00009410: 2020 2020 2020 2020 2070 7265 765f 7461           prev_ta
-00009420: 622e 656e 6428 4661 6c73 6529 0a20 2020  b.end(False).   
-00009430: 2020 2020 2020 2020 2020 2020 2065 6c73               els
-00009440: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-00009450: 2020 2020 2020 206e 6578 745f 7461 6220         next_tab 
-00009460: 3d20 7365 6c66 2e74 6162 5f6e 6578 742e  = self.tab_next.
-00009470: 6765 7428 7365 6c66 2e72 6563 6569 7665  get(self.receive
-00009480: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00009490: 2020 2020 2020 6e65 7874 5f74 6162 2e73        next_tab.s
-000094a0: 6574 466f 6375 7328 290a 2020 2020 2020  etFocus().      
-000094b0: 2020 2020 2020 2020 2020 2020 2020 6e65                ne
-000094c0: 7874 5f74 6162 2e64 6573 656c 6563 7428  xt_tab.deselect(
-000094d0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-000094e0: 2020 2020 2020 6e65 7874 5f74 6162 2e65        next_tab.e
-000094f0: 6e64 2846 616c 7365 290a 2020 2020 2020  nd(False).      
-00009500: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00009510: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00009520: 7365 6c66 2e6f 7468 6572 5f31 2e68 6173  self.other_1.has
-00009530: 466f 6375 7328 293a 0a20 2020 2020 2020  Focus():.       
-00009540: 2020 2020 2020 2020 206c 6f67 6765 722e           logger.
-00009550: 6465 6275 6728 2246 726f 6d20 6f74 6865  debug("From othe
-00009560: 725f 3122 290a 2020 2020 2020 2020 2020  r_1").          
-00009570: 2020 2020 2020 6966 206d 6f64 6966 6965        if modifie
-00009580: 7220 3d3d 2051 742e 5368 6966 744d 6f64  r == Qt.ShiftMod
-00009590: 6966 6965 723a 0a20 2020 2020 2020 2020  ifier:.         
-000095a0: 2020 2020 2020 2020 2020 2070 7265 765f             prev_
-000095b0: 7461 6220 3d20 7365 6c66 2e74 6162 5f70  tab = self.tab_p
-000095c0: 7265 762e 6765 7428 7365 6c66 2e6f 7468  rev.get(self.oth
-000095d0: 6572 5f31 290a 2020 2020 2020 2020 2020  er_1).          
-000095e0: 2020 2020 2020 2020 2020 7072 6576 5f74            prev_t
-000095f0: 6162 2e73 6574 466f 6375 7328 290a 2020  ab.setFocus().  
-00009600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009610: 2020 7072 6576 5f74 6162 2e64 6573 656c    prev_tab.desel
-00009620: 6563 7428 290a 2020 2020 2020 2020 2020  ect().          
-00009630: 2020 2020 2020 2020 2020 7072 6576 5f74            prev_t
-00009640: 6162 2e65 6e64 2846 616c 7365 290a 2020  ab.end(False).  
-00009650: 2020 2020 2020 2020 2020 2020 2020 656c                el
-00009660: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00009670: 2020 2020 2020 2020 6e65 7874 5f74 6162          next_tab
-00009680: 203d 2073 656c 662e 7461 625f 6e65 7874   = self.tab_next
-00009690: 2e67 6574 2873 656c 662e 6f74 6865 725f  .get(self.other_
-000096a0: 3129 0a20 2020 2020 2020 2020 2020 2020  1).             
-000096b0: 2020 2020 2020 206e 6578 745f 7461 622e         next_tab.
-000096c0: 7365 7446 6f63 7573 2829 0a20 2020 2020  setFocus().     
-000096d0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-000096e0: 6578 745f 7461 622e 6465 7365 6c65 6374  ext_tab.deselect
-000096f0: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
-00009700: 2020 2020 2020 206e 6578 745f 7461 622e         next_tab.
-00009710: 656e 6428 4661 6c73 6529 0a20 2020 2020  end(False).     
-00009720: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00009730: 6e0a 2020 2020 2020 2020 2020 2020 6966  n.            if
-00009740: 2073 656c 662e 6f74 6865 725f 322e 6861   self.other_2.ha
-00009750: 7346 6f63 7573 2829 3a0a 2020 2020 2020  sFocus():.      
-00009760: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
-00009770: 2e64 6562 7567 2822 4672 6f6d 206f 7468  .debug("From oth
-00009780: 6572 5f32 2229 0a20 2020 2020 2020 2020  er_2").         
-00009790: 2020 2020 2020 2069 6620 6d6f 6469 6669         if modifi
-000097a0: 6572 203d 3d20 5174 2e53 6869 6674 4d6f  er == Qt.ShiftMo
-000097b0: 6469 6669 6572 3a0a 2020 2020 2020 2020  difier:.        
-000097c0: 2020 2020 2020 2020 2020 2020 7072 6576              prev
-000097d0: 5f74 6162 203d 2073 656c 662e 7461 625f  _tab = self.tab_
-000097e0: 7072 6576 2e67 6574 2873 656c 662e 6f74  prev.get(self.ot
-000097f0: 6865 725f 3229 0a20 2020 2020 2020 2020  her_2).         
-00009800: 2020 2020 2020 2020 2020 2070 7265 765f             prev_
-00009810: 7461 622e 7365 7446 6f63 7573 2829 0a20  tab.setFocus(). 
-00009820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009830: 2020 2070 7265 765f 7461 622e 6465 7365     prev_tab.dese
-00009840: 6c65 6374 2829 0a20 2020 2020 2020 2020  lect().         
-00009850: 2020 2020 2020 2020 2020 2070 7265 765f             prev_
-00009860: 7461 622e 656e 6428 4661 6c73 6529 0a20  tab.end(False). 
-00009870: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00009880: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00009890: 2020 2020 2020 2020 206e 6578 745f 7461           next_ta
-000098a0: 6220 3d20 7365 6c66 2e74 6162 5f6e 6578  b = self.tab_nex
-000098b0: 742e 6765 7428 7365 6c66 2e6f 7468 6572  t.get(self.other
-000098c0: 5f32 290a 2020 2020 2020 2020 2020 2020  _2).            
-000098d0: 2020 2020 2020 2020 6e65 7874 5f74 6162          next_tab
-000098e0: 2e73 6574 466f 6375 7328 290a 2020 2020  .setFocus().    
-000098f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009900: 6e65 7874 5f74 6162 2e64 6573 656c 6563  next_tab.deselec
-00009910: 7428 290a 2020 2020 2020 2020 2020 2020  t().            
-00009920: 2020 2020 2020 2020 6e65 7874 5f74 6162          next_tab
-00009930: 2e65 6e64 2846 616c 7365 290a 2020 2020  .end(False).    
-00009940: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00009950: 726e 0a20 2020 2020 2020 2020 2020 2069  rn.            i
-00009960: 6620 7365 6c66 2e63 616c 6c73 6967 6e2e  f self.callsign.
-00009970: 6861 7346 6f63 7573 2829 3a0a 2020 2020  hasFocus():.    
-00009980: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
-00009990: 6572 2e64 6562 7567 2822 4672 6f6d 2063  er.debug("From c
-000099a0: 616c 6c73 6967 6e22 290a 2020 2020 2020  allsign").      
-000099b0: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-000099c0: 6865 636b 5f63 616c 6c73 6967 6e28 7365  heck_callsign(se
-000099d0: 6c66 2e63 616c 6c73 6967 6e2e 7465 7874  lf.callsign.text
-000099e0: 2829 290a 2020 2020 2020 2020 2020 2020  ()).            
-000099f0: 2020 2020 6966 2073 656c 662e 6368 6563      if self.chec
-00009a00: 6b5f 6475 7065 2873 656c 662e 6361 6c6c  k_dupe(self.call
-00009a10: 7369 676e 2e74 6578 7428 2929 3a0a 2020  sign.text()):.  
-00009a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009a30: 2020 7365 6c66 2e64 7570 655f 696e 6469    self.dupe_indi
-00009a40: 6361 746f 722e 7368 6f77 2829 0a20 2020  cator.show().   
-00009a50: 2020 2020 2020 2020 2020 2020 2065 6c73               els
-00009a60: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-00009a70: 2020 2020 2020 2073 656c 662e 6475 7065         self.dupe
-00009a80: 5f69 6e64 6963 6174 6f72 2e68 6964 6528  _indicator.hide(
-00009a90: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00009aa0: 2020 6966 206d 6f64 6966 6965 7220 3d3d    if modifier ==
-00009ab0: 2051 742e 5368 6966 744d 6f64 6966 6965   Qt.ShiftModifie
-00009ac0: 723a 0a20 2020 2020 2020 2020 2020 2020  r:.             
-00009ad0: 2020 2020 2020 2070 7265 765f 7461 6220         prev_tab 
-00009ae0: 3d20 7365 6c66 2e74 6162 5f70 7265 762e  = self.tab_prev.
-00009af0: 6765 7428 7365 6c66 2e63 616c 6c73 6967  get(self.callsig
-00009b00: 6e29 0a20 2020 2020 2020 2020 2020 2020  n).             
-00009b10: 2020 2020 2020 2070 7265 765f 7461 622e         prev_tab.
-00009b20: 7365 7446 6f63 7573 2829 0a20 2020 2020  setFocus().     
-00009b30: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00009b40: 7265 765f 7461 622e 6465 7365 6c65 6374  rev_tab.deselect
-00009b50: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
-00009b60: 2020 2020 2020 2070 7265 765f 7461 622e         prev_tab.
-00009b70: 656e 6428 4661 6c73 6529 0a20 2020 2020  end(False).     
-00009b80: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-00009b90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009ba0: 2020 2020 2074 6578 7420 3d20 7365 6c66       text = self
-00009bb0: 2e63 616c 6c73 6967 6e2e 7465 7874 2829  .callsign.text()
-00009bc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009bd0: 2020 2020 2074 6578 7420 3d20 7465 7874       text = text
-00009be0: 2e75 7070 6572 2829 0a20 2020 2020 2020  .upper().       
-00009bf0: 2020 2020 2020 2020 2020 2020 205f 7468               _th
-00009c00: 6574 6872 6561 6420 3d20 7468 7265 6164  ethread = thread
-00009c10: 696e 672e 5468 7265 6164 280a 2020 2020  ing.Thread(.    
-00009c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009c30: 2020 2020 7461 7267 6574 3d73 656c 662e      target=self.
-00009c40: 6368 6563 6b5f 6361 6c6c 7369 676e 322c  check_callsign2,
-00009c50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009c60: 2020 2020 2020 2020 2061 7267 733d 2874           args=(t
-00009c70: 6578 742c 292c 0a20 2020 2020 2020 2020  ext,),.         
-00009c80: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00009c90: 6165 6d6f 6e3d 5472 7565 2c0a 2020 2020  aemon=True,.    
+000071c0: 424f 5448 223a 2028 7365 6c66 2e42 616e  BOTH": (self.Ban
+000071d0: 645f 4d6f 6465 5f46 7261 6d65 5f43 572c  d_Mode_Frame_CW,
+000071e0: 2073 656c 662e 4261 6e64 5f4d 6f64 655f   self.Band_Mode_
+000071f0: 4672 616d 655f 5353 4229 2c0a 2020 2020  Frame_SSB),.    
+00007200: 2020 2020 2020 2020 2244 4947 4954 414c          "DIGITAL
+00007210: 223a 2028 7365 6c66 2e42 616e 645f 4d6f  ": (self.Band_Mo
+00007220: 6465 5f46 7261 6d65 5f52 5454 592c 292c  de_Frame_RTTY,),
+00007230: 0a20 2020 2020 2020 2020 2020 2022 5353  .            "SS
+00007240: 422b 4357 2b44 4947 4954 414c 223a 2028  B+CW+DIGITAL": (
+00007250: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007260: 2073 656c 662e 4261 6e64 5f4d 6f64 655f   self.Band_Mode_
+00007270: 4672 616d 655f 5254 5459 2c0a 2020 2020  Frame_RTTY,.    
+00007280: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00007290: 2e42 616e 645f 4d6f 6465 5f46 7261 6d65  .Band_Mode_Frame
+000072a0: 5f43 572c 0a20 2020 2020 2020 2020 2020  _CW,.           
+000072b0: 2020 2020 2073 656c 662e 4261 6e64 5f4d       self.Band_M
+000072c0: 6f64 655f 4672 616d 655f 5353 422c 0a20  ode_Frame_SSB,. 
+000072d0: 2020 2020 2020 2020 2020 2029 2c0a 2020             ),.  
+000072e0: 2020 2020 2020 2020 2020 2246 4d22 3a20            "FM": 
+000072f0: 2873 656c 662e 4261 6e64 5f4d 6f64 655f  (self.Band_Mode_
+00007300: 4672 616d 655f 5353 422c 292c 0a20 2020  Frame_SSB,),.   
+00007310: 2020 2020 207d 0a20 2020 2020 2020 2066       }.        f
+00007320: 7261 6d65 7320 3d20 6d6f 6465 732e 6765  rames = modes.ge
+00007330: 7428 7468 655f 6d6f 6465 290a 2020 2020  t(the_mode).    
+00007340: 2020 2020 6966 2066 7261 6d65 733a 0a20      if frames:. 
+00007350: 2020 2020 2020 2020 2020 2066 6f72 2066             for f
+00007360: 7261 6d65 2069 6e20 6672 616d 6573 3a0a  rame in frames:.
+00007370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007380: 6672 616d 652e 7368 6f77 2829 0a0a 2020  frame.show()..  
+00007390: 2020 6465 6620 7368 6f77 5f6b 6579 5f68    def show_key_h
+000073a0: 656c 7028 7365 6c66 2920 2d3e 204e 6f6e  elp(self) -> Non
+000073b0: 653a 0a20 2020 2020 2020 2022 2222 5368  e:.        """Sh
+000073c0: 6f77 2068 656c 7020 626f 7820 666f 7220  ow help box for 
+000073d0: 686f 746b 6579 7322 2222 0a20 2020 2020  hotkeys""".     
+000073e0: 2020 2073 656c 662e 7368 6f77 5f6d 6573     self.show_mes
+000073f0: 7361 6765 5f62 6f78 280a 2020 2020 2020  sage_box(.      
+00007400: 2020 2020 2020 225b 4573 635d 5c74 436c        "[Esc]\tCl
+00007410: 6561 7273 2074 6865 2069 6e70 7574 2066  ears the input f
+00007420: 6965 6c64 7320 6f66 2061 6e79 2074 6578  ields of any tex
+00007430: 742e 5c6e 220a 2020 2020 2020 2020 2020  t.\n".          
+00007440: 2020 225b 4354 524c 2d45 7363 5d5c 7453    "[CTRL-Esc]\tS
+00007450: 746f 7073 2063 7764 6165 6d6f 6e20 6672  tops cwdaemon fr
+00007460: 6f6d 2073 656e 6469 6e67 204d 6f72 7365  om sending Morse
+00007470: 2e5c 6e22 0a20 2020 2020 2020 2020 2020  .\n".           
+00007480: 2022 5b50 6755 705d 5c74 496e 6372 6561   "[PgUp]\tIncrea
+00007490: 7365 7320 7468 6520 6377 2073 656e 6469  ses the cw sendi
+000074a0: 6e67 2073 7065 6564 2e5c 6e22 0a20 2020  ng speed.\n".   
+000074b0: 2020 2020 2020 2020 2022 5b50 6744 6f77           "[PgDow
+000074c0: 6e5d 5c74 4465 6372 6561 7365 7320 7468  n]\tDecreases th
+000074d0: 6520 6377 2073 656e 6469 6e67 2073 7065  e cw sending spe
+000074e0: 6564 2e5c 6e22 0a20 2020 2020 2020 2020  ed.\n".         
+000074f0: 2020 2022 5b41 7272 6f77 2d55 705d 204a     "[Arrow-Up] J
+00007500: 756d 7020 746f 2074 6865 206e 6578 7420  ump to the next 
+00007510: 7370 6f74 2061 626f 7665 2074 6865 2063  spot above the c
+00007520: 7572 7265 6e74 2056 464f 2063 7572 736f  urrent VFO curso
+00007530: 725c 6e22 0a20 2020 2020 2020 2020 2020  r\n".           
+00007540: 2022 5c74 696e 2074 6865 2062 616e 646d   "\tin the bandm
+00007550: 6170 2077 696e 646f 7720 2843 4154 2052  ap window (CAT R
+00007560: 6571 7569 7265 6429 2e5c 6e22 0a20 2020  equired).\n".   
+00007570: 2020 2020 2020 2020 2022 5b41 7272 6f77           "[Arrow
+00007580: 2d44 6f77 6e5d 204a 756d 7020 746f 2074  -Down] Jump to t
+00007590: 6865 206e 6578 7420 7370 6f74 2062 656c  he next spot bel
+000075a0: 6f77 2074 6865 2063 7572 7265 6e74 5c6e  ow the current\n
+000075b0: 220a 2020 2020 2020 2020 2020 2020 225c  ".            "\
+000075c0: 7456 464f 2063 7572 736f 7220 696e 2074  tVFO cursor in t
+000075d0: 6865 2062 616e 646d 6170 2077 696e 646f  he bandmap windo
+000075e0: 7720 2843 4154 2052 6571 7569 7265 6429  w (CAT Required)
+000075f0: 2e5c 6e22 0a20 2020 2020 2020 2020 2020  .\n".           
+00007600: 2022 5b54 4142 5d5c 744d 6f76 6520 6375   "[TAB]\tMove cu
+00007610: 7273 6f72 2074 6f20 7468 6520 7269 6768  rsor to the righ
+00007620: 7420 6f6e 6520 6669 656c 642e 5c6e 220a  t one field.\n".
+00007630: 2020 2020 2020 2020 2020 2020 225b 5368              "[Sh
+00007640: 6966 742d 5461 625d 5c74 4d6f 7665 2063  ift-Tab]\tMove c
+00007650: 7572 736f 7220 6c65 6674 204f 6e65 2066  ursor left One f
+00007660: 6965 6c64 2e5c 6e22 0a20 2020 2020 2020  ield.\n".       
+00007670: 2020 2020 2022 5b53 5041 4345 5d5c 7457       "[SPACE]\tW
+00007680: 6865 6e20 696e 2074 6865 2063 616c 6c73  hen in the calls
+00007690: 6967 6e20 6669 656c 642c 2077 696c 6c20  ign field, will 
+000076a0: 6d6f 7665 2074 6865 2069 6e70 7574 2074  move the input t
+000076b0: 6f20 7468 655c 6e22 0a20 2020 2020 2020  o the\n".       
+000076c0: 2020 2020 2022 5c74 6669 7273 7420 6669       "\tfirst fi
+000076d0: 656c 6420 6e65 6564 6564 2066 6f72 2074  eld needed for t
+000076e0: 6865 2065 7863 6861 6e67 652e 5c6e 220a  he exchange.\n".
+000076f0: 2020 2020 2020 2020 2020 2020 225b 456e              "[En
+00007700: 7465 725d 5c74 5375 626d 6974 7320 7468  ter]\tSubmits th
+00007710: 6520 6669 656c 6473 2074 6f20 7468 6520  e fields to the 
+00007720: 6c6f 672e 5c6e 220a 2020 2020 2020 2020  log.\n".        
+00007730: 2020 2020 225b 4631 2d46 3132 5d5c 7453      "[F1-F12]\tS
+00007740: 656e 6420 2843 5720 6f72 2056 6f69 6365  end (CW or Voice
+00007750: 2920 6d61 6372 6f73 2e5c 6e22 0a20 2020  ) macros.\n".   
+00007760: 2020 2020 2020 2020 2022 5b43 5452 4c2d           "[CTRL-
+00007770: 535d 5c74 5370 6f74 2043 616c 6c73 6967  S]\tSpot Callsig
+00007780: 6e20 746f 2074 6865 2063 6c75 7374 6572  n to the cluster
+00007790: 2e5c 6e22 0a20 2020 2020 2020 2020 2020  .\n".           
+000077a0: 2022 5b43 5452 4c2d 475d 5c74 5475 6e65   "[CTRL-G]\tTune
+000077b0: 2074 6f20 6120 7370 6f74 206d 6174 6368   to a spot match
+000077c0: 696e 6720 7061 7274 6961 6c20 7465 7874  ing partial text
+000077d0: 2069 6e20 7468 6520 6361 6c6c 7369 676e   in the callsign
+000077e0: 5c6e 220a 2020 2020 2020 2020 2020 2020  \n".            
+000077f0: 225c 7465 6e74 7279 2066 6965 6c64 2028  "\tentry field (
+00007800: 4341 5420 5265 7175 6972 6564 292e 5c6e  CAT Required).\n
+00007810: 220a 2020 2020 2020 2020 290a 0a20 2020  ".        )..   
+00007820: 2064 6566 2066 696c 6570 6963 6b65 7228   def filepicker(
+00007830: 7365 6c66 2c20 6163 7469 6f6e 3a20 7374  self, action: st
+00007840: 7229 202d 3e20 7374 723a 0a20 2020 2020  r) -> str:.     
+00007850: 2020 2022 2222 0a20 2020 2020 2020 2047     """.        G
+00007860: 6574 2061 2066 696c 656e 616d 650a 2020  et a filename.  
+00007870: 2020 2020 2020 6163 7469 6f6e 3a20 226e        action: "n
+00007880: 6577 2220 6f72 2022 6f70 656e 220a 2020  ew" or "open".  
+00007890: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+000078a0: 2020 6f70 7469 6f6e 7320 3d20 5146 696c    options = QFil
+000078b0: 6544 6961 6c6f 672e 4f70 7469 6f6e 7328  eDialog.Options(
+000078c0: 290a 2020 2020 2020 2020 6f70 7469 6f6e  ).        option
+000078d0: 7320 7c3d 2051 4669 6c65 4469 616c 6f67  s |= QFileDialog
+000078e0: 2e44 6f6e 7455 7365 4e61 7469 7665 4469  .DontUseNativeDi
+000078f0: 616c 6f67 0a20 2020 2020 2020 206f 7074  alog.        opt
+00007900: 696f 6e73 207c 3d20 5146 696c 6544 6961  ions |= QFileDia
+00007910: 6c6f 672e 446f 6e74 436f 6e66 6972 6d4f  log.DontConfirmO
+00007920: 7665 7277 7269 7465 0a20 2020 2020 2020  verwrite.       
+00007930: 2069 6620 6163 7469 6f6e 203d 3d20 226e   if action == "n
+00007940: 6577 223a 0a20 2020 2020 2020 2020 2020  ew":.           
+00007950: 2066 696c 652c 205f 203d 2051 4669 6c65   file, _ = QFile
+00007960: 4469 616c 6f67 2e67 6574 5361 7665 4669  Dialog.getSaveFi
+00007970: 6c65 4e61 6d65 280a 2020 2020 2020 2020  leName(.        
+00007980: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
+00007990: 2020 2020 2020 2020 2020 2020 2020 2243                "C
+000079a0: 686f 6f73 6520 6120 4461 7461 6261 7365  hoose a Database
+000079b0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+000079c0: 2020 2044 4154 415f 5041 5448 2c0a 2020     DATA_PATH,.  
+000079d0: 2020 2020 2020 2020 2020 2020 2020 2244                "D
+000079e0: 6174 6162 6173 6520 282a 2e64 6229 222c  atabase (*.db)",
+000079f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007a00: 206f 7074 696f 6e73 3d6f 7074 696f 6e73   options=options
+00007a10: 2c0a 2020 2020 2020 2020 2020 2020 290a  ,.            ).
+00007a20: 2020 2020 2020 2020 6966 2061 6374 696f          if actio
+00007a30: 6e20 3d3d 2022 6f70 656e 223a 0a20 2020  n == "open":.   
+00007a40: 2020 2020 2020 2020 2066 696c 652c 205f           file, _
+00007a50: 203d 2051 4669 6c65 4469 616c 6f67 2e67   = QFileDialog.g
+00007a60: 6574 4f70 656e 4669 6c65 4e61 6d65 280a  etOpenFileName(.
+00007a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007a80: 7365 6c66 2c0a 2020 2020 2020 2020 2020  self,.          
+00007a90: 2020 2020 2020 2243 686f 6f73 6520 6120        "Choose a 
+00007aa0: 4461 7461 6261 7365 222c 0a20 2020 2020  Database",.     
+00007ab0: 2020 2020 2020 2020 2020 2044 4154 415f             DATA_
+00007ac0: 5041 5448 2c0a 2020 2020 2020 2020 2020  PATH,.          
+00007ad0: 2020 2020 2020 2244 6174 6162 6173 6520        "Database 
+00007ae0: 282a 2e64 6229 222c 0a20 2020 2020 2020  (*.db)",.       
+00007af0: 2020 2020 2020 2020 206f 7074 696f 6e73           options
+00007b00: 3d6f 7074 696f 6e73 2c0a 2020 2020 2020  =options,.      
+00007b10: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00007b20: 7265 7475 726e 2066 696c 650a 0a20 2020  return file..   
+00007b30: 2064 6566 2072 6563 616c 6375 6c61 7465   def recalculate
+00007b40: 5f6d 756c 7473 2873 656c 6629 3a0a 2020  _mults(self):.  
+00007b50: 2020 2020 2020 2222 2252 6563 616c 6375        """Recalcu
+00007b60: 6c61 7465 204d 756c 7469 706c 6965 7273  late Multipliers
+00007b70: 2222 220a 2020 2020 2020 2020 7365 6c66  """.        self
+00007b80: 2e63 6f6e 7465 7374 2e72 6563 616c 6375  .contest.recalcu
+00007b90: 6c61 7465 5f6d 756c 7473 2873 656c 6629  late_mults(self)
+00007ba0: 0a0a 2020 2020 6465 6620 6c61 756e 6368  ..    def launch
+00007bb0: 5f6c 6f67 5f77 696e 646f 7728 7365 6c66  _log_window(self
+00007bc0: 293a 0a20 2020 2020 2020 2022 2222 6c61  ):.        """la
+00007bd0: 756e 6368 2074 6865 204c 6f67 2057 696e  unch the Log Win
+00007be0: 646f 7722 2222 0a20 2020 2020 2020 2069  dow""".        i
+00007bf0: 6620 6e6f 7420 6368 6563 6b5f 7072 6f63  f not check_proc
+00007c00: 6573 7328 226c 6f67 7769 6e64 6f77 2e70  ess("logwindow.p
+00007c10: 7922 293a 0a20 2020 2020 2020 2020 2020  y"):.           
+00007c20: 205f 203d 2073 7562 7072 6f63 6573 732e   _ = subprocess.
+00007c30: 506f 7065 6e28 5b73 7973 2e65 7865 6375  Popen([sys.execu
+00007c40: 7461 626c 652c 2057 4f52 4b49 4e47 5f50  table, WORKING_P
+00007c50: 4154 4820 2b20 222f 6c6f 6777 696e 646f  ATH + "/logwindo
+00007c60: 772e 7079 225d 290a 0a20 2020 2064 6566  w.py"])..    def
+00007c70: 206c 6175 6e63 685f 6261 6e64 6d61 705f   launch_bandmap_
+00007c80: 7769 6e64 6f77 2873 656c 6629 3a0a 2020  window(self):.  
+00007c90: 2020 2020 2020 2222 226c 6175 6e63 6820        """launch 
+00007ca0: 7468 6520 4c6f 6720 5769 6e64 6f77 2222  the Log Window""
+00007cb0: 220a 2020 2020 2020 2020 6966 206e 6f74  ".        if not
+00007cc0: 2063 6865 636b 5f70 726f 6365 7373 2822   check_process("
+00007cd0: 6261 6e64 6d61 702e 7079 2229 3a0a 2020  bandmap.py"):.  
+00007ce0: 2020 2020 2020 2020 2020 5f20 3d20 7375            _ = su
+00007cf0: 6270 726f 6365 7373 2e50 6f70 656e 285b  bprocess.Popen([
+00007d00: 7379 732e 6578 6563 7574 6162 6c65 2c20  sys.executable, 
+00007d10: 574f 524b 494e 475f 5041 5448 202b 2022  WORKING_PATH + "
+00007d20: 2f62 616e 646d 6170 2e70 7922 5d29 0a0a  /bandmap.py"])..
+00007d30: 2020 2020 6465 6620 636c 6561 725f 6261      def clear_ba
+00007d40: 6e64 5f69 6e64 6963 6174 6f72 7328 7365  nd_indicators(se
+00007d50: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
+00007d60: 436c 6561 7220 7468 6520 696e 6469 6361  Clear the indica
+00007d70: 746f 7273 2222 220a 2020 2020 2020 2020  tors""".        
+00007d80: 666f 7220 5f2c 2069 6e64 6963 6174 6f72  for _, indicator
+00007d90: 7320 696e 2073 656c 662e 616c 6c5f 6d6f  s in self.all_mo
+00007da0: 6465 5f69 6e64 6963 6174 6f72 732e 6974  de_indicators.it
+00007db0: 656d 7328 293a 0a20 2020 2020 2020 2020  ems():.         
+00007dc0: 2020 2066 6f72 205f 2c20 696e 6469 6361     for _, indica
+00007dd0: 746f 7220 696e 2069 6e64 6963 6174 6f72  tor in indicator
+00007de0: 732e 6974 656d 7328 293a 0a20 2020 2020  s.items():.     
+00007df0: 2020 2020 2020 2020 2020 2069 6e64 6963             indic
+00007e00: 6174 6f72 2e73 6574 4672 616d 6553 6861  ator.setFrameSha
+00007e10: 7065 2851 7457 6964 6765 7473 2e51 4672  pe(QtWidgets.QFr
+00007e20: 616d 652e 4e6f 4672 616d 6529 0a20 2020  ame.NoFrame).   
+00007e30: 2020 2020 2020 2020 2020 2020 2069 6e64               ind
+00007e40: 6963 6174 6f72 2e73 6574 5374 796c 6553  icator.setStyleS
+00007e50: 6865 6574 2822 666f 6e74 2d66 616d 696c  heet("font-famil
+00007e60: 793a 204a 6574 4272 6169 6e73 204d 6f6e  y: JetBrains Mon
+00007e70: 6f3b 2229 0a0a 2020 2020 6465 6620 7365  o;")..    def se
+00007e80: 745f 6261 6e64 5f69 6e64 6963 6174 6f72  t_band_indicator
+00007e90: 2873 656c 662c 2062 616e 643a 2073 7472  (self, band: str
+00007ea0: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+00007eb0: 2020 2022 2222 5365 7420 7468 6520 6261     """Set the ba
+00007ec0: 6e64 2069 6e64 6963 6174 6f72 2222 220a  nd indicator""".
+00007ed0: 2020 2020 2020 2020 2320 6c6f 6767 6572          # logger
+00007ee0: 2e64 6562 7567 2822 2573 222c 2066 2262  .debug("%s", f"b
+00007ef0: 616e 643a 7b62 616e 647d 206d 6f64 653a  and:{band} mode:
+00007f00: 207b 7365 6c66 2e63 7572 7265 6e74 5f6d   {self.current_m
+00007f10: 6f64 657d 2229 0a20 2020 2020 2020 2069  ode}").        i
+00007f20: 6620 6261 6e64 2061 6e64 2073 656c 662e  f band and self.
+00007f30: 6375 7272 656e 745f 6d6f 6465 3a0a 2020  current_mode:.  
+00007f40: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+00007f50: 6c65 6172 5f62 616e 645f 696e 6469 6361  lear_band_indica
+00007f60: 746f 7273 2829 0a20 2020 2020 2020 2020  tors().         
+00007f70: 2020 2069 6e64 6963 6174 6f72 203d 2073     indicator = s
+00007f80: 656c 662e 616c 6c5f 6d6f 6465 5f69 6e64  elf.all_mode_ind
+00007f90: 6963 6174 6f72 735b 7365 6c66 2e63 7572  icators[self.cur
+00007fa0: 7265 6e74 5f6d 6f64 655d 2e67 6574 2862  rent_mode].get(b
+00007fb0: 616e 642c 204e 6f6e 6529 0a20 2020 2020  and, None).     
+00007fc0: 2020 2020 2020 2069 6620 696e 6469 6361         if indica
+00007fd0: 746f 723a 0a20 2020 2020 2020 2020 2020  tor:.           
+00007fe0: 2020 2020 2069 6e64 6963 6174 6f72 2e73       indicator.s
+00007ff0: 6574 4672 616d 6553 6861 7065 2851 7457  etFrameShape(QtW
+00008000: 6964 6765 7473 2e51 4672 616d 652e 426f  idgets.QFrame.Bo
+00008010: 7829 0a20 2020 2020 2020 2020 2020 2020  x).             
+00008020: 2020 2069 6e64 6963 6174 6f72 2e73 6574     indicator.set
+00008030: 5374 796c 6553 6865 6574 2822 666f 6e74  StyleSheet("font
+00008040: 2d66 616d 696c 793a 204a 6574 4272 6169  -family: JetBrai
+00008050: 6e73 204d 6f6e 6f3b 2063 6f6c 6f72 3a20  ns Mono; color: 
+00008060: 6772 6565 6e3b 2229 0a0a 2020 2020 6465  green;")..    de
+00008070: 6620 636c 6f73 6545 7665 6e74 2873 656c  f closeEvent(sel
+00008080: 662c 205f 6576 656e 7429 3a0a 2020 2020  f, _event):.    
+00008090: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+000080a0: 5772 6974 6520 7769 6e64 6f77 2073 697a  Write window siz
+000080b0: 6520 616e 6420 706f 7369 7469 6f6e 2074  e and position t
+000080c0: 6f20 636f 6e66 6967 2066 696c 650a 2020  o config file.  
+000080d0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+000080e0: 2020 7365 6c66 2e70 7265 665b 2277 696e    self.pref["win
+000080f0: 646f 775f 7769 6474 6822 5d20 3d20 7365  dow_width"] = se
+00008100: 6c66 2e73 697a 6528 292e 7769 6474 6828  lf.size().width(
+00008110: 290a 2020 2020 2020 2020 7365 6c66 2e70  ).        self.p
+00008120: 7265 665b 2277 696e 646f 775f 6865 6967  ref["window_heig
+00008130: 6874 225d 203d 2073 656c 662e 7369 7a65  ht"] = self.size
+00008140: 2829 2e68 6569 6768 7428 290a 2020 2020  ().height().    
+00008150: 2020 2020 7365 6c66 2e70 7265 665b 2277      self.pref["w
+00008160: 696e 646f 775f 7822 5d20 3d20 7365 6c66  indow_x"] = self
+00008170: 2e70 6f73 2829 2e78 2829 0a20 2020 2020  .pos().x().     
+00008180: 2020 2073 656c 662e 7072 6566 5b22 7769     self.pref["wi
+00008190: 6e64 6f77 5f79 225d 203d 2073 656c 662e  ndow_y"] = self.
+000081a0: 706f 7328 292e 7928 290a 2020 2020 2020  pos().y().      
+000081b0: 2020 7365 6c66 2e77 7269 7465 5f70 7265    self.write_pre
+000081c0: 6665 7265 6e63 6528 290a 0a20 2020 2064  ference()..    d
+000081d0: 6566 2063 7479 5f6c 6f6f 6b75 7028 7365  ef cty_lookup(se
+000081e0: 6c66 2c20 6361 6c6c 7369 676e 3a20 7374  lf, callsign: st
+000081f0: 7229 3a0a 2020 2020 2020 2020 2222 224c  r):.        """L
+00008200: 6f6f 6b75 7020 6361 6c6c 7369 676e 2069  ookup callsign i
+00008210: 6e20 6374 792e 6461 7420 6669 6c65 2e0a  n cty.dat file..
+00008220: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
+00008230: 6572 730a 2020 2020 2020 2020 2d2d 2d2d  ers.        ----
+00008240: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2063  ------.        c
+00008250: 616c 6c73 6967 6e20 3a20 7374 720a 0a20  allsign : str.. 
+00008260: 2020 2020 2020 2052 6574 7572 6e73 0a20         Returns. 
+00008270: 2020 2020 2020 202d 2d2d 2d2d 2d2d 0a20         -------. 
+00008280: 2020 2020 2020 2072 6574 7572 6e20 3a20         return : 
+00008290: 6c69 7374 206f 6620 6469 6374 730a 2020  list of dicts.  
+000082a0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+000082b0: 2020 6361 6c6c 7369 676e 203d 2063 616c    callsign = cal
+000082c0: 6c73 6967 6e2e 7570 7065 7228 290a 2020  lsign.upper().  
+000082d0: 2020 2020 2020 666f 7220 636f 756e 7420        for count 
+000082e0: 696e 2072 6576 6572 7365 6428 7261 6e67  in reversed(rang
+000082f0: 6528 6c65 6e28 6361 6c6c 7369 676e 2929  e(len(callsign))
+00008300: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
+00008310: 6561 7263 6869 7465 6d20 3d20 6361 6c6c  earchitem = call
+00008320: 7369 676e 5b3a 2063 6f75 6e74 202b 2031  sign[: count + 1
+00008330: 5d0a 2020 2020 2020 2020 2020 2020 7265  ].            re
+00008340: 7375 6c74 203d 207b 6b65 793a 2076 616c  sult = {key: val
+00008350: 2066 6f72 206b 6579 2c20 7661 6c20 696e   for key, val in
+00008360: 2043 5459 4649 4c45 2e69 7465 6d73 2829   CTYFILE.items()
+00008370: 2069 6620 6b65 7920 3d3d 2073 6561 7263   if key == searc
+00008380: 6869 7465 6d7d 0a20 2020 2020 2020 2020  hitem}.         
+00008390: 2020 2069 6620 6e6f 7420 7265 7375 6c74     if not result
+000083a0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000083b0: 2020 636f 6e74 696e 7565 0a20 2020 2020    continue.     
+000083c0: 2020 2020 2020 2069 6620 7265 7375 6c74         if result
+000083d0: 2e67 6574 2873 6561 7263 6869 7465 6d29  .get(searchitem)
+000083e0: 2e67 6574 2822 6578 6163 745f 6d61 7463  .get("exact_matc
+000083f0: 6822 293a 0a20 2020 2020 2020 2020 2020  h"):.           
+00008400: 2020 2020 2069 6620 7365 6172 6368 6974       if searchit
+00008410: 656d 203d 3d20 6361 6c6c 7369 676e 3a0a  em == callsign:.
+00008420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008430: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
+00008440: 740a 2020 2020 2020 2020 2020 2020 2020  t.              
+00008450: 2020 636f 6e74 696e 7565 0a20 2020 2020    continue.     
+00008460: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
+00008470: 7375 6c74 0a0a 2020 2020 6465 6620 6377  sult..    def cw
+00008480: 7370 6565 645f 7370 696e 626f 785f 6368  speed_spinbox_ch
+00008490: 616e 6765 6428 7365 6c66 293a 0a20 2020  anged(self):.   
+000084a0: 2020 2020 2022 2222 7472 6967 6765 7265       """triggere
+000084b0: 6420 7768 656e 2076 616c 7565 206f 6620  d when value of 
+000084c0: 4357 2073 7065 6564 2069 6e20 7468 6520  CW speed in the 
+000084d0: 7370 696e 626f 7820 6368 616e 6765 732e  spinbox changes.
+000084e0: 2222 220a 2020 2020 2020 2020 6966 2073  """.        if s
+000084f0: 656c 662e 6377 2069 7320 4e6f 6e65 3a0a  elf.cw is None:.
+00008500: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00008510: 726e 0a20 2020 2020 2020 2069 6620 7365  rn.        if se
+00008520: 6c66 2e63 772e 7365 7276 6572 7479 7065  lf.cw.servertype
+00008530: 203d 3d20 313a 0a20 2020 2020 2020 2020   == 1:.         
+00008540: 2020 2073 656c 662e 6377 2e73 7065 6564     self.cw.speed
+00008550: 203d 2073 656c 662e 6377 5f73 7065 6564   = self.cw_speed
+00008560: 2e76 616c 7565 2829 0a20 2020 2020 2020  .value().       
+00008570: 2020 2020 2073 656c 662e 6377 2e73 656e       self.cw.sen
+00008580: 6463 7728 6622 5c78 3162 327b 7365 6c66  dcw(f"\x1b2{self
+00008590: 2e63 772e 7370 6565 647d 2229 0a20 2020  .cw.speed}").   
+000085a0: 2020 2020 2069 6620 7365 6c66 2e63 772e       if self.cw.
+000085b0: 7365 7276 6572 7479 7065 203d 3d20 323a  servertype == 2:
+000085c0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+000085d0: 662e 6377 2e73 6574 5f77 696e 6b65 7965  f.cw.set_winkeye
+000085e0: 725f 7370 6565 6428 7365 6c66 2e63 775f  r_speed(self.cw_
+000085f0: 7370 6565 642e 7661 6c75 6528 2929 0a0a  speed.value())..
+00008600: 2020 2020 6465 6620 6b65 7950 7265 7373      def keyPress
+00008610: 4576 656e 7428 7365 6c66 2c20 6576 656e  Event(self, even
+00008620: 7429 3a20 2023 2070 796c 696e 743a 2064  t):  # pylint: d
+00008630: 6973 6162 6c65 3d69 6e76 616c 6964 2d6e  isable=invalid-n
+00008640: 616d 650a 2020 2020 2020 2020 2222 2254  ame.        """T
+00008650: 6869 7320 6f76 6572 7269 6465 7320 5174  his overrides Qt
+00008660: 206b 6579 2065 7665 6e74 2e22 2222 0a20   key event.""". 
+00008670: 2020 2020 2020 206d 6f64 6966 6965 7220         modifier 
+00008680: 3d20 6576 656e 742e 6d6f 6469 6669 6572  = event.modifier
+00008690: 7328 290a 2020 2020 2020 2020 6966 2065  s().        if e
+000086a0: 7665 6e74 2e6b 6579 2829 203d 3d20 5174  vent.key() == Qt
+000086b0: 2e4b 6579 5f53 2061 6e64 206d 6f64 6966  .Key_S and modif
+000086c0: 6965 7220 3d3d 2051 742e 436f 6e74 726f  ier == Qt.Contro
+000086d0: 6c4d 6f64 6966 6965 723a 0a20 2020 2020  lModifier:.     
+000086e0: 2020 2020 2020 2066 7265 7120 3d20 7365         freq = se
+000086f0: 6c66 2e72 6164 696f 5f73 7461 7465 2e67  lf.radio_state.g
+00008700: 6574 2822 7666 6f61 2229 0a20 2020 2020  et("vfoa").     
+00008710: 2020 2020 2020 2064 7820 3d20 7365 6c66         dx = self
+00008720: 2e63 616c 6c73 6967 6e2e 7465 7874 2829  .callsign.text()
+00008730: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00008740: 6672 6571 2061 6e64 2064 783a 0a20 2020  freq and dx:.   
+00008750: 2020 2020 2020 2020 2020 2020 2063 6d64               cmd
+00008760: 203d 207b 7d0a 2020 2020 2020 2020 2020   = {}.          
+00008770: 2020 2020 2020 636d 645b 2263 6d64 225d        cmd["cmd"]
+00008780: 203d 2022 5350 4f54 4458 220a 2020 2020   = "SPOTDX".    
+00008790: 2020 2020 2020 2020 2020 2020 636d 645b              cmd[
+000087a0: 2273 7461 7469 6f6e 225d 203d 2070 6c61  "station"] = pla
+000087b0: 7466 6f72 6d2e 6e6f 6465 2829 0a20 2020  tform.node().   
+000087c0: 2020 2020 2020 2020 2020 2020 2063 6d64               cmd
+000087d0: 5b22 6478 225d 203d 2064 780a 2020 2020  ["dx"] = dx.    
+000087e0: 2020 2020 2020 2020 2020 2020 636d 645b              cmd[
+000087f0: 2266 7265 7122 5d20 3d20 666c 6f61 7428  "freq"] = float(
+00008800: 696e 7428 6672 6571 2920 2f20 3130 3030  int(freq) / 1000
+00008810: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00008820: 2020 7365 6c66 2e6d 756c 7469 6361 7374    self.multicast
+00008830: 5f69 6e74 6572 6661 6365 2e73 656e 645f  _interface.send_
+00008840: 6173 5f6a 736f 6e28 636d 6429 0a20 2020  as_json(cmd).   
+00008850: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
+00008860: 2020 2020 2020 2020 6966 2065 7665 6e74          if event
+00008870: 2e6b 6579 2829 203d 3d20 5174 2e4b 6579  .key() == Qt.Key
+00008880: 5f47 2061 6e64 206d 6f64 6966 6965 7220  _G and modifier 
+00008890: 3d3d 2051 742e 436f 6e74 726f 6c4d 6f64  == Qt.ControlMod
+000088a0: 6966 6965 723a 0a20 2020 2020 2020 2020  ifier:.         
+000088b0: 2020 2064 7820 3d20 7365 6c66 2e63 616c     dx = self.cal
+000088c0: 6c73 6967 6e2e 7465 7874 2829 0a20 2020  lsign.text().   
+000088d0: 2020 2020 2020 2020 2069 6620 6478 3a0a           if dx:.
+000088e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000088f0: 636d 6420 3d20 7b7d 0a20 2020 2020 2020  cmd = {}.       
+00008900: 2020 2020 2020 2020 2063 6d64 5b22 636d           cmd["cm
+00008910: 6422 5d20 3d20 2246 494e 4444 5822 0a20  d"] = "FINDDX". 
+00008920: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00008930: 6d64 5b22 7374 6174 696f 6e22 5d20 3d20  md["station"] = 
+00008940: 706c 6174 666f 726d 2e6e 6f64 6528 290a  platform.node().
+00008950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008960: 636d 645b 2264 7822 5d20 3d20 6478 0a20  cmd["dx"] = dx. 
+00008970: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00008980: 656c 662e 6d75 6c74 6963 6173 745f 696e  elf.multicast_in
+00008990: 7465 7266 6163 652e 7365 6e64 5f61 735f  terface.send_as_
+000089a0: 6a73 6f6e 2863 6d64 290a 2020 2020 2020  json(cmd).      
+000089b0: 2020 2020 2020 7265 7475 726e 0a20 2020        return.   
+000089c0: 2020 2020 2069 6620 280a 2020 2020 2020       if (.      
+000089d0: 2020 2020 2020 6576 656e 742e 6b65 7928        event.key(
+000089e0: 2920 3d3d 2051 742e 4b65 792e 4b65 795f  ) == Qt.Key.Key_
+000089f0: 4573 6361 7065 2061 6e64 206d 6f64 6966  Escape and modif
+00008a00: 6965 7220 213d 2051 742e 436f 6e74 726f  ier != Qt.Contro
+00008a10: 6c4d 6f64 6966 6965 720a 2020 2020 2020  lModifier.      
+00008a20: 2020 293a 2020 2320 7079 6c69 6e74 3a20    ):  # pylint: 
+00008a30: 6469 7361 626c 653d 6e6f 2d6d 656d 6265  disable=no-membe
+00008a40: 720a 2020 2020 2020 2020 2020 2020 7365  r.            se
+00008a50: 6c66 2e63 6c65 6172 696e 7075 7473 2829  lf.clearinputs()
+00008a60: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00008a70: 7572 6e0a 2020 2020 2020 2020 6966 2065  urn.        if e
+00008a80: 7665 6e74 2e6b 6579 2829 203d 3d20 5174  vent.key() == Qt
+00008a90: 2e4b 6579 2e4b 6579 5f45 7363 6170 6520  .Key.Key_Escape 
+00008aa0: 616e 6420 6d6f 6469 6669 6572 203d 3d20  and modifier == 
+00008ab0: 5174 2e43 6f6e 7472 6f6c 4d6f 6469 6669  Qt.ControlModifi
+00008ac0: 6572 3a0a 2020 2020 2020 2020 2020 2020  er:.            
+00008ad0: 6966 2073 656c 662e 6377 2069 7320 6e6f  if self.cw is no
+00008ae0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00008af0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00008b00: 6377 2e73 6572 7665 7274 7970 6520 3d3d  cw.servertype ==
+00008b10: 2031 3a0a 2020 2020 2020 2020 2020 2020   1:.            
+00008b20: 2020 2020 2020 2020 7365 6c66 2e63 772e          self.cw.
+00008b30: 7365 6e64 6377 2822 5c78 3162 3422 290a  sendcw("\x1b4").
+00008b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008b50: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
+00008b60: 2020 2069 6620 6576 656e 742e 6b65 7928     if event.key(
+00008b70: 2920 3d3d 2051 742e 4b65 792e 4b65 795f  ) == Qt.Key.Key_
+00008b80: 5570 3a0a 2020 2020 2020 2020 2020 2020  Up:.            
+00008b90: 636d 6420 3d20 7b7d 0a20 2020 2020 2020  cmd = {}.       
+00008ba0: 2020 2020 2063 6d64 5b22 636d 6422 5d20       cmd["cmd"] 
+00008bb0: 3d20 2250 5245 5653 504f 5422 0a20 2020  = "PREVSPOT".   
+00008bc0: 2020 2020 2020 2020 2063 6d64 5b22 7374           cmd["st
+00008bd0: 6174 696f 6e22 5d20 3d20 706c 6174 666f  ation"] = platfo
+00008be0: 726d 2e6e 6f64 6528 290a 2020 2020 2020  rm.node().      
+00008bf0: 2020 2020 2020 7365 6c66 2e6d 756c 7469        self.multi
+00008c00: 6361 7374 5f69 6e74 6572 6661 6365 2e73  cast_interface.s
+00008c10: 656e 645f 6173 5f6a 736f 6e28 636d 6429  end_as_json(cmd)
+00008c20: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00008c30: 7572 6e0a 2020 2020 2020 2020 6966 2065  urn.        if e
+00008c40: 7665 6e74 2e6b 6579 2829 203d 3d20 5174  vent.key() == Qt
+00008c50: 2e4b 6579 2e4b 6579 5f44 6f77 6e3a 0a20  .Key.Key_Down:. 
+00008c60: 2020 2020 2020 2020 2020 2063 6d64 203d             cmd =
+00008c70: 207b 7d0a 2020 2020 2020 2020 2020 2020   {}.            
+00008c80: 636d 645b 2263 6d64 225d 203d 2022 4e45  cmd["cmd"] = "NE
+00008c90: 5854 5350 4f54 220a 2020 2020 2020 2020  XTSPOT".        
+00008ca0: 2020 2020 636d 645b 2273 7461 7469 6f6e      cmd["station
+00008cb0: 225d 203d 2070 6c61 7466 6f72 6d2e 6e6f  "] = platform.no
+00008cc0: 6465 2829 0a20 2020 2020 2020 2020 2020  de().           
+00008cd0: 2073 656c 662e 6d75 6c74 6963 6173 745f   self.multicast_
+00008ce0: 696e 7465 7266 6163 652e 7365 6e64 5f61  interface.send_a
+00008cf0: 735f 6a73 6f6e 2863 6d64 290a 2020 2020  s_json(cmd).    
+00008d00: 2020 2020 2020 2020 7265 7475 726e 0a20          return. 
+00008d10: 2020 2020 2020 2069 6620 6576 656e 742e         if event.
+00008d20: 6b65 7928 2920 3d3d 2051 742e 4b65 792e  key() == Qt.Key.
+00008d30: 4b65 795f 5061 6765 5570 2061 6e64 206d  Key_PageUp and m
+00008d40: 6f64 6966 6965 7220 213d 2051 742e 436f  odifier != Qt.Co
+00008d50: 6e74 726f 6c4d 6f64 6966 6965 723a 0a20  ntrolModifier:. 
+00008d60: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+00008d70: 6c66 2e63 7720 6973 206e 6f74 204e 6f6e  lf.cw is not Non
+00008d80: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00008d90: 2020 2073 656c 662e 6377 2e73 7065 6564     self.cw.speed
+00008da0: 202b 3d20 310a 2020 2020 2020 2020 2020   += 1.          
+00008db0: 2020 2020 2020 7365 6c66 2e63 775f 7370        self.cw_sp
+00008dc0: 6565 642e 7365 7456 616c 7565 2873 656c  eed.setValue(sel
+00008dd0: 662e 6377 2e73 7065 6564 290a 2020 2020  f.cw.speed).    
+00008de0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+00008df0: 656c 662e 6377 2e73 6572 7665 7274 7970  elf.cw.servertyp
+00008e00: 6520 3d3d 2031 3a0a 2020 2020 2020 2020  e == 1:.        
+00008e10: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00008e20: 2e63 772e 7365 6e64 6377 2866 225c 7831  .cw.sendcw(f"\x1
+00008e30: 6232 7b73 656c 662e 6377 2e73 7065 6564  b2{self.cw.speed
+00008e40: 7d22 290a 2020 2020 2020 2020 2020 2020  }").            
+00008e50: 2020 2020 6966 2073 656c 662e 6377 2e73      if self.cw.s
+00008e60: 6572 7665 7274 7970 6520 3d3d 2032 3a0a  ervertype == 2:.
+00008e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008e80: 2020 2020 7365 6c66 2e63 772e 7365 745f      self.cw.set_
+00008e90: 7769 6e6b 6579 6572 5f73 7065 6564 2873  winkeyer_speed(s
+00008ea0: 656c 662e 6377 5f73 7065 6564 2e76 616c  elf.cw_speed.val
+00008eb0: 7565 2829 290a 2020 2020 2020 2020 2020  ue()).          
+00008ec0: 2020 7265 7475 726e 0a20 2020 2020 2020    return.       
+00008ed0: 2069 6620 6576 656e 742e 6b65 7928 2920   if event.key() 
+00008ee0: 3d3d 2051 742e 4b65 792e 4b65 795f 5061  == Qt.Key.Key_Pa
+00008ef0: 6765 446f 776e 2061 6e64 206d 6f64 6966  geDown and modif
+00008f00: 6965 7220 213d 2051 742e 436f 6e74 726f  ier != Qt.Contro
+00008f10: 6c4d 6f64 6966 6965 723a 0a20 2020 2020  lModifier:.     
+00008f20: 2020 2020 2020 2069 6620 7365 6c66 2e63         if self.c
+00008f30: 7720 6973 206e 6f74 204e 6f6e 653a 0a20  w is not None:. 
+00008f40: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00008f50: 656c 662e 6377 2e73 7065 6564 202d 3d20  elf.cw.speed -= 
+00008f60: 310a 2020 2020 2020 2020 2020 2020 2020  1.              
+00008f70: 2020 7365 6c66 2e63 775f 7370 6565 642e    self.cw_speed.
+00008f80: 7365 7456 616c 7565 2873 656c 662e 6377  setValue(self.cw
+00008f90: 2e73 7065 6564 290a 2020 2020 2020 2020  .speed).        
+00008fa0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00008fb0: 6377 2e73 6572 7665 7274 7970 6520 3d3d  cw.servertype ==
+00008fc0: 2031 3a0a 2020 2020 2020 2020 2020 2020   1:.            
+00008fd0: 2020 2020 2020 2020 7365 6c66 2e63 772e          self.cw.
+00008fe0: 7365 6e64 6377 2866 225c 7831 6232 7b73  sendcw(f"\x1b2{s
+00008ff0: 656c 662e 6377 2e73 7065 6564 7d22 290a  elf.cw.speed}").
+00009000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009010: 6966 2073 656c 662e 6377 2e73 6572 7665  if self.cw.serve
+00009020: 7274 7970 6520 3d3d 2032 3a0a 2020 2020  rtype == 2:.    
+00009030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009040: 7365 6c66 2e63 772e 7365 745f 7769 6e6b  self.cw.set_wink
+00009050: 6579 6572 5f73 7065 6564 2873 656c 662e  eyer_speed(self.
+00009060: 6377 5f73 7065 6564 2e76 616c 7565 2829  cw_speed.value()
+00009070: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
+00009080: 7475 726e 0a20 2020 2020 2020 2023 2069  turn.        # i
+00009090: 6620 6576 656e 742e 6b65 7928 2920 3d3d  f event.key() ==
+000090a0: 2051 742e 4b65 792e 4b65 795f 456e 7465   Qt.Key.Key_Ente
+000090b0: 723a 0a20 2020 2020 2020 2023 2020 2020  r:.        #    
+000090c0: 2073 656c 662e 7361 7665 5f63 6f6e 7461   self.save_conta
+000090d0: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
+000090e0: 6576 656e 742e 6b65 7928 2920 3d3d 2051  event.key() == Q
+000090f0: 742e 4b65 792e 4b65 795f 5461 6220 6f72  t.Key.Key_Tab or
+00009100: 2065 7665 6e74 2e6b 6579 2829 203d 3d20   event.key() == 
+00009110: 5174 2e4b 6579 2e4b 6579 5f42 6163 6b74  Qt.Key.Key_Backt
+00009120: 6162 3a0a 2020 2020 2020 2020 2020 2020  ab:.            
+00009130: 6966 2073 656c 662e 7365 6e74 2e68 6173  if self.sent.has
+00009140: 466f 6375 7328 293a 0a20 2020 2020 2020  Focus():.       
+00009150: 2020 2020 2020 2020 206c 6f67 6765 722e           logger.
+00009160: 6465 6275 6728 2246 726f 6d20 7365 6e74  debug("From sent
+00009170: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
+00009180: 2020 2069 6620 6d6f 6469 6669 6572 203d     if modifier =
+00009190: 3d20 5174 2e53 6869 6674 4d6f 6469 6669  = Qt.ShiftModifi
+000091a0: 6572 3a0a 2020 2020 2020 2020 2020 2020  er:.            
+000091b0: 2020 2020 2020 2020 7072 6576 5f74 6162          prev_tab
+000091c0: 203d 2073 656c 662e 7461 625f 7072 6576   = self.tab_prev
+000091d0: 2e67 6574 2873 656c 662e 7365 6e74 290a  .get(self.sent).
+000091e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000091f0: 2020 2020 7072 6576 5f74 6162 2e73 6574      prev_tab.set
+00009200: 466f 6375 7328 290a 2020 2020 2020 2020  Focus().        
+00009210: 2020 2020 2020 2020 2020 2020 7072 6576              prev
+00009220: 5f74 6162 2e64 6573 656c 6563 7428 290a  _tab.deselect().
+00009230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009240: 2020 2020 7072 6576 5f74 6162 2e65 6e64      prev_tab.end
+00009250: 2846 616c 7365 290a 2020 2020 2020 2020  (False).        
+00009260: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00009270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009280: 2020 6e65 7874 5f74 6162 203d 2073 656c    next_tab = sel
+00009290: 662e 7461 625f 6e65 7874 2e67 6574 2873  f.tab_next.get(s
+000092a0: 656c 662e 7365 6e74 290a 2020 2020 2020  elf.sent).      
+000092b0: 2020 2020 2020 2020 2020 2020 2020 6e65                ne
+000092c0: 7874 5f74 6162 2e73 6574 466f 6375 7328  xt_tab.setFocus(
+000092d0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+000092e0: 2020 2020 2020 6e65 7874 5f74 6162 2e64        next_tab.d
+000092f0: 6573 656c 6563 7428 290a 2020 2020 2020  eselect().      
+00009300: 2020 2020 2020 2020 2020 2020 2020 6e65                ne
+00009310: 7874 5f74 6162 2e65 6e64 2846 616c 7365  xt_tab.end(False
+00009320: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00009330: 2020 7265 7475 726e 0a20 2020 2020 2020    return.       
+00009340: 2020 2020 2069 6620 7365 6c66 2e72 6563       if self.rec
+00009350: 6569 7665 2e68 6173 466f 6375 7328 293a  eive.hasFocus():
+00009360: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009370: 206c 6f67 6765 722e 6465 6275 6728 2246   logger.debug("F
+00009380: 726f 6d20 7265 6365 6976 6522 290a 2020  rom receive").  
+00009390: 2020 2020 2020 2020 2020 2020 2020 6966                if
+000093a0: 206d 6f64 6966 6965 7220 3d3d 2051 742e   modifier == Qt.
+000093b0: 5368 6966 744d 6f64 6966 6965 723a 0a20  ShiftModifier:. 
+000093c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000093d0: 2020 2070 7265 765f 7461 6220 3d20 7365     prev_tab = se
+000093e0: 6c66 2e74 6162 5f70 7265 762e 6765 7428  lf.tab_prev.get(
+000093f0: 7365 6c66 2e72 6563 6569 7665 290a 2020  self.receive).  
+00009400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009410: 2020 7072 6576 5f74 6162 2e73 6574 466f    prev_tab.setFo
+00009420: 6375 7328 290a 2020 2020 2020 2020 2020  cus().          
+00009430: 2020 2020 2020 2020 2020 7072 6576 5f74            prev_t
+00009440: 6162 2e64 6573 656c 6563 7428 290a 2020  ab.deselect().  
+00009450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009460: 2020 7072 6576 5f74 6162 2e65 6e64 2846    prev_tab.end(F
+00009470: 616c 7365 290a 2020 2020 2020 2020 2020  alse).          
+00009480: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00009490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000094a0: 6e65 7874 5f74 6162 203d 2073 656c 662e  next_tab = self.
+000094b0: 7461 625f 6e65 7874 2e67 6574 2873 656c  tab_next.get(sel
+000094c0: 662e 7265 6365 6976 6529 0a20 2020 2020  f.receive).     
+000094d0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+000094e0: 6578 745f 7461 622e 7365 7446 6f63 7573  ext_tab.setFocus
+000094f0: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
+00009500: 2020 2020 2020 206e 6578 745f 7461 622e         next_tab.
+00009510: 6465 7365 6c65 6374 2829 0a20 2020 2020  deselect().     
+00009520: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+00009530: 6578 745f 7461 622e 656e 6428 4661 6c73  ext_tab.end(Fals
+00009540: 6529 0a20 2020 2020 2020 2020 2020 2020  e).             
+00009550: 2020 2072 6574 7572 6e0a 2020 2020 2020     return.      
+00009560: 2020 2020 2020 6966 2073 656c 662e 6f74        if self.ot
+00009570: 6865 725f 312e 6861 7346 6f63 7573 2829  her_1.hasFocus()
+00009580: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00009590: 2020 6c6f 6767 6572 2e64 6562 7567 2822    logger.debug("
+000095a0: 4672 6f6d 206f 7468 6572 5f31 2229 0a20  From other_1"). 
+000095b0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+000095c0: 6620 6d6f 6469 6669 6572 203d 3d20 5174  f modifier == Qt
+000095d0: 2e53 6869 6674 4d6f 6469 6669 6572 3a0a  .ShiftModifier:.
+000095e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000095f0: 2020 2020 7072 6576 5f74 6162 203d 2073      prev_tab = s
+00009600: 656c 662e 7461 625f 7072 6576 2e67 6574  elf.tab_prev.get
+00009610: 2873 656c 662e 6f74 6865 725f 3129 0a20  (self.other_1). 
+00009620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009630: 2020 2070 7265 765f 7461 622e 7365 7446     prev_tab.setF
+00009640: 6f63 7573 2829 0a20 2020 2020 2020 2020  ocus().         
+00009650: 2020 2020 2020 2020 2020 2070 7265 765f             prev_
+00009660: 7461 622e 6465 7365 6c65 6374 2829 0a20  tab.deselect(). 
+00009670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009680: 2020 2070 7265 765f 7461 622e 656e 6428     prev_tab.end(
+00009690: 4661 6c73 6529 0a20 2020 2020 2020 2020  False).         
+000096a0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+000096b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000096c0: 206e 6578 745f 7461 6220 3d20 7365 6c66   next_tab = self
+000096d0: 2e74 6162 5f6e 6578 742e 6765 7428 7365  .tab_next.get(se
+000096e0: 6c66 2e6f 7468 6572 5f31 290a 2020 2020  lf.other_1).    
+000096f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009700: 6e65 7874 5f74 6162 2e73 6574 466f 6375  next_tab.setFocu
+00009710: 7328 290a 2020 2020 2020 2020 2020 2020  s().            
+00009720: 2020 2020 2020 2020 6e65 7874 5f74 6162          next_tab
+00009730: 2e64 6573 656c 6563 7428 290a 2020 2020  .deselect().    
+00009740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009750: 6e65 7874 5f74 6162 2e65 6e64 2846 616c  next_tab.end(Fal
+00009760: 7365 290a 2020 2020 2020 2020 2020 2020  se).            
+00009770: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
+00009780: 2020 2020 2020 2069 6620 7365 6c66 2e6f         if self.o
+00009790: 7468 6572 5f32 2e68 6173 466f 6375 7328  ther_2.hasFocus(
+000097a0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+000097b0: 2020 206c 6f67 6765 722e 6465 6275 6728     logger.debug(
+000097c0: 2246 726f 6d20 6f74 6865 725f 3222 290a  "From other_2").
+000097d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000097e0: 6966 206d 6f64 6966 6965 7220 3d3d 2051  if modifier == Q
+000097f0: 742e 5368 6966 744d 6f64 6966 6965 723a  t.ShiftModifier:
+00009800: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009810: 2020 2020 2070 7265 765f 7461 6220 3d20       prev_tab = 
+00009820: 7365 6c66 2e74 6162 5f70 7265 762e 6765  self.tab_prev.ge
+00009830: 7428 7365 6c66 2e6f 7468 6572 5f32 290a  t(self.other_2).
+00009840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009850: 2020 2020 7072 6576 5f74 6162 2e73 6574      prev_tab.set
+00009860: 466f 6375 7328 290a 2020 2020 2020 2020  Focus().        
+00009870: 2020 2020 2020 2020 2020 2020 7072 6576              prev
+00009880: 5f74 6162 2e64 6573 656c 6563 7428 290a  _tab.deselect().
+00009890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000098a0: 2020 2020 7072 6576 5f74 6162 2e65 6e64      prev_tab.end
+000098b0: 2846 616c 7365 290a 2020 2020 2020 2020  (False).        
+000098c0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+000098d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000098e0: 2020 6e65 7874 5f74 6162 203d 2073 656c    next_tab = sel
+000098f0: 662e 7461 625f 6e65 7874 2e67 6574 2873  f.tab_next.get(s
+00009900: 656c 662e 6f74 6865 725f 3229 0a20 2020  elf.other_2).   
+00009910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009920: 206e 6578 745f 7461 622e 7365 7446 6f63   next_tab.setFoc
+00009930: 7573 2829 0a20 2020 2020 2020 2020 2020  us().           
+00009940: 2020 2020 2020 2020 206e 6578 745f 7461           next_ta
+00009950: 622e 6465 7365 6c65 6374 2829 0a20 2020  b.deselect().   
+00009960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009970: 206e 6578 745f 7461 622e 656e 6428 4661   next_tab.end(Fa
+00009980: 6c73 6529 0a20 2020 2020 2020 2020 2020  lse).           
+00009990: 2020 2020 2072 6574 7572 6e0a 2020 2020       return.    
+000099a0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+000099b0: 6361 6c6c 7369 676e 2e68 6173 466f 6375  callsign.hasFocu
+000099c0: 7328 293a 0a20 2020 2020 2020 2020 2020  s():.           
+000099d0: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
+000099e0: 6728 2246 726f 6d20 6361 6c6c 7369 676e  g("From callsign
+000099f0: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
+00009a00: 2020 2073 656c 662e 6368 6563 6b5f 6361     self.check_ca
+00009a10: 6c6c 7369 676e 2873 656c 662e 6361 6c6c  llsign(self.call
+00009a20: 7369 676e 2e74 6578 7428 2929 0a20 2020  sign.text()).   
+00009a30: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00009a40: 7365 6c66 2e63 6865 636b 5f64 7570 6528  self.check_dupe(
+00009a50: 7365 6c66 2e63 616c 6c73 6967 6e2e 7465  self.callsign.te
+00009a60: 7874 2829 293a 0a20 2020 2020 2020 2020  xt()):.         
+00009a70: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00009a80: 6475 7065 5f69 6e64 6963 6174 6f72 2e73  dupe_indicator.s
+00009a90: 686f 7728 290a 2020 2020 2020 2020 2020  how().          
+00009aa0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00009ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009ac0: 7365 6c66 2e64 7570 655f 696e 6469 6361  self.dupe_indica
+00009ad0: 746f 722e 6869 6465 2829 0a20 2020 2020  tor.hide().     
+00009ae0: 2020 2020 2020 2020 2020 2069 6620 6d6f             if mo
+00009af0: 6469 6669 6572 203d 3d20 5174 2e53 6869  difier == Qt.Shi
+00009b00: 6674 4d6f 6469 6669 6572 3a0a 2020 2020  ftModifier:.    
+00009b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009b20: 7072 6576 5f74 6162 203d 2073 656c 662e  prev_tab = self.
+00009b30: 7461 625f 7072 6576 2e67 6574 2873 656c  tab_prev.get(sel
+00009b40: 662e 6361 6c6c 7369 676e 290a 2020 2020  f.callsign).    
+00009b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009b60: 7072 6576 5f74 6162 2e73 6574 466f 6375  prev_tab.setFocu
+00009b70: 7328 290a 2020 2020 2020 2020 2020 2020  s().            
+00009b80: 2020 2020 2020 2020 7072 6576 5f74 6162          prev_tab
+00009b90: 2e64 6573 656c 6563 7428 290a 2020 2020  .deselect().    
+00009ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009bb0: 7072 6576 5f74 6162 2e65 6e64 2846 616c  prev_tab.end(Fal
+00009bc0: 7365 290a 2020 2020 2020 2020 2020 2020  se).            
+00009bd0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00009be0: 2020 2020 2020 2020 2020 2020 2020 7465                te
+00009bf0: 7874 203d 2073 656c 662e 6361 6c6c 7369  xt = self.callsi
+00009c00: 676e 2e74 6578 7428 290a 2020 2020 2020  gn.text().      
+00009c10: 2020 2020 2020 2020 2020 2020 2020 7465                te
+00009c20: 7874 203d 2074 6578 742e 7570 7065 7228  xt = text.upper(
+00009c30: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00009c40: 2020 2020 2020 5f74 6865 7468 7265 6164        _thethread
+00009c50: 203d 2074 6872 6561 6469 6e67 2e54 6872   = threading.Thr
+00009c60: 6561 6428 0a20 2020 2020 2020 2020 2020  ead(.           
+00009c70: 2020 2020 2020 2020 2020 2020 2074 6172               tar
+00009c80: 6765 743d 7365 6c66 2e63 6865 636b 5f63  get=self.check_c
+00009c90: 616c 6c73 6967 6e32 2c0a 2020 2020 2020  allsign2,.      
 00009ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009cb0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00009cc0: 2020 2020 2020 5f74 6865 7468 7265 6164        _thethread
-00009cd0: 2e73 7461 7274 2829 0a20 2020 2020 2020  .start().       
-00009ce0: 2020 2020 2020 2020 2020 2020 206e 6578               nex
-00009cf0: 745f 7461 6220 3d20 7365 6c66 2e74 6162  t_tab = self.tab
-00009d00: 5f6e 6578 742e 6765 7428 7365 6c66 2e63  _next.get(self.c
-00009d10: 616c 6c73 6967 6e29 0a20 2020 2020 2020  allsign).       
-00009d20: 2020 2020 2020 2020 2020 2020 206e 6578               nex
-00009d30: 745f 7461 622e 7365 7446 6f63 7573 2829  t_tab.setFocus()
-00009d40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009d50: 2020 2020 206e 6578 745f 7461 622e 6465       next_tab.de
-00009d60: 7365 6c65 6374 2829 0a20 2020 2020 2020  select().       
-00009d70: 2020 2020 2020 2020 2020 2020 206e 6578               nex
-00009d80: 745f 7461 622e 656e 6428 4661 6c73 6529  t_tab.end(False)
-00009d90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009da0: 2072 6574 7572 6e0a 2020 2020 2020 2020   return.        
-00009db0: 6966 2065 7665 6e74 2e6b 6579 2829 203d  if event.key() =
-00009dc0: 3d20 5174 2e4b 6579 5f46 313a 0a20 2020  = Qt.Key_F1:.   
-00009dd0: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
-00009de0: 6e64 6631 2829 0a20 2020 2020 2020 2069  ndf1().        i
-00009df0: 6620 6576 656e 742e 6b65 7928 2920 3d3d  f event.key() ==
-00009e00: 2051 742e 4b65 795f 4632 3a0a 2020 2020   Qt.Key_F2:.    
-00009e10: 2020 2020 2020 2020 7365 6c66 2e73 656e          self.sen
-00009e20: 6466 3228 290a 2020 2020 2020 2020 6966  df2().        if
-00009e30: 2065 7665 6e74 2e6b 6579 2829 203d 3d20   event.key() == 
-00009e40: 5174 2e4b 6579 5f46 333a 0a20 2020 2020  Qt.Key_F3:.     
-00009e50: 2020 2020 2020 2073 656c 662e 7365 6e64         self.send
-00009e60: 6633 2829 0a20 2020 2020 2020 2069 6620  f3().        if 
-00009e70: 6576 656e 742e 6b65 7928 2920 3d3d 2051  event.key() == Q
-00009e80: 742e 4b65 795f 4634 3a0a 2020 2020 2020  t.Key_F4:.      
-00009e90: 2020 2020 2020 7365 6c66 2e73 656e 6466        self.sendf
-00009ea0: 3428 290a 2020 2020 2020 2020 6966 2065  4().        if e
-00009eb0: 7665 6e74 2e6b 6579 2829 203d 3d20 5174  vent.key() == Qt
-00009ec0: 2e4b 6579 5f46 353a 0a20 2020 2020 2020  .Key_F5:.       
-00009ed0: 2020 2020 2073 656c 662e 7365 6e64 6635       self.sendf5
-00009ee0: 2829 0a20 2020 2020 2020 2069 6620 6576  ().        if ev
-00009ef0: 656e 742e 6b65 7928 2920 3d3d 2051 742e  ent.key() == Qt.
-00009f00: 4b65 795f 4636 3a0a 2020 2020 2020 2020  Key_F6:.        
-00009f10: 2020 2020 7365 6c66 2e73 656e 6466 3628      self.sendf6(
-00009f20: 290a 2020 2020 2020 2020 6966 2065 7665  ).        if eve
-00009f30: 6e74 2e6b 6579 2829 203d 3d20 5174 2e4b  nt.key() == Qt.K
-00009f40: 6579 5f46 373a 0a20 2020 2020 2020 2020  ey_F7:.         
-00009f50: 2020 2073 656c 662e 7365 6e64 6637 2829     self.sendf7()
-00009f60: 0a20 2020 2020 2020 2069 6620 6576 656e  .        if even
-00009f70: 742e 6b65 7928 2920 3d3d 2051 742e 4b65  t.key() == Qt.Ke
-00009f80: 795f 4638 3a0a 2020 2020 2020 2020 2020  y_F8:.          
-00009f90: 2020 7365 6c66 2e73 656e 6466 3828 290a    self.sendf8().
-00009fa0: 2020 2020 2020 2020 6966 2065 7665 6e74          if event
-00009fb0: 2e6b 6579 2829 203d 3d20 5174 2e4b 6579  .key() == Qt.Key
-00009fc0: 5f46 393a 0a20 2020 2020 2020 2020 2020  _F9:.           
-00009fd0: 2073 656c 662e 7365 6e64 6639 2829 0a20   self.sendf9(). 
-00009fe0: 2020 2020 2020 2069 6620 6576 656e 742e         if event.
-00009ff0: 6b65 7928 2920 3d3d 2051 742e 4b65 795f  key() == Qt.Key_
-0000a000: 4631 303a 0a20 2020 2020 2020 2020 2020  F10:.           
-0000a010: 2073 656c 662e 7365 6e64 6631 3028 290a   self.sendf10().
-0000a020: 2020 2020 2020 2020 6966 2065 7665 6e74          if event
-0000a030: 2e6b 6579 2829 203d 3d20 5174 2e4b 6579  .key() == Qt.Key
-0000a040: 5f46 3131 3a0a 2020 2020 2020 2020 2020  _F11:.          
-0000a050: 2020 7365 6c66 2e73 656e 6466 3131 2829    self.sendf11()
-0000a060: 0a20 2020 2020 2020 2069 6620 6576 656e  .        if even
-0000a070: 742e 6b65 7928 2920 3d3d 2051 742e 4b65  t.key() == Qt.Ke
-0000a080: 795f 4631 323a 0a20 2020 2020 2020 2020  y_F12:.         
-0000a090: 2020 2073 656c 662e 7365 6e64 6631 3228     self.sendf12(
-0000a0a0: 290a 0a20 2020 2064 6566 2073 6574 5f77  )..    def set_w
-0000a0b0: 696e 646f 775f 7469 746c 6528 7365 6c66  indow_title(self
-0000a0c0: 293a 0a20 2020 2020 2020 2022 2222 5365  ):.        """Se
-0000a0d0: 7420 7769 6e64 6f77 2074 6974 6c65 2222  t window title""
-0000a0e0: 220a 2020 2020 2020 2020 7666 6f61 203d  ".        vfoa =
-0000a0f0: 2073 656c 662e 7261 6469 6f5f 7374 6174   self.radio_stat
-0000a100: 652e 6765 7428 2276 666f 6122 2c20 2222  e.get("vfoa", ""
-0000a110: 290a 2020 2020 2020 2020 6966 2076 666f  ).        if vfo
-0000a120: 613a 0a20 2020 2020 2020 2020 2020 2076  a:.            v
-0000a130: 666f 6120 3d20 696e 7428 7666 6f61 2920  foa = int(vfoa) 
-0000a140: 2f20 3130 3030 0a20 2020 2020 2020 2065  / 1000.        e
-0000a150: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-0000a160: 2076 666f 6120 3d20 302e 300a 2020 2020   vfoa = 0.0.    
-0000a170: 2020 2020 636f 6e74 6573 745f 6e61 6d65      contest_name
-0000a180: 203d 2022 220a 2020 2020 2020 2020 6966   = "".        if
-0000a190: 2073 656c 662e 636f 6e74 6573 743a 0a20   self.contest:. 
-0000a1a0: 2020 2020 2020 2020 2020 2063 6f6e 7465             conte
-0000a1b0: 7374 5f6e 616d 6520 3d20 7365 6c66 2e63  st_name = self.c
-0000a1c0: 6f6e 7465 7374 2e6e 616d 650a 2020 2020  ontest.name.    
-0000a1d0: 2020 2020 6c69 6e65 203d 2028 0a20 2020      line = (.   
-0000a1e0: 2020 2020 2020 2020 2066 2276 666f 613a           f"vfoa:
-0000a1f0: 7b72 6f75 6e64 2876 666f 612c 3229 7d20  {round(vfoa,2)} 
-0000a200: 220a 2020 2020 2020 2020 2020 2020 6622  ".            f"
-0000a210: 6d6f 6465 3a7b 7365 6c66 2e72 6164 696f  mode:{self.radio
-0000a220: 5f73 7461 7465 2e67 6574 2827 6d6f 6465  _state.get('mode
-0000a230: 272c 2027 2729 7d20 220a 2020 2020 2020  ', '')} ".      
-0000a240: 2020 2020 2020 6622 4f50 3a7b 7365 6c66        f"OP:{self
-0000a250: 2e63 7572 7265 6e74 5f6f 707d 207b 636f  .current_op} {co
-0000a260: 6e74 6573 745f 6e61 6d65 7d20 220a 2020  ntest_name} ".  
-0000a270: 2020 2020 2020 2020 2020 6622 2d20 4e6f            f"- No
-0000a280: 7431 4d4d 2076 7b5f 5f76 6572 7369 6f6e  t1MM v{__version
-0000a290: 5f5f 7d22 0a20 2020 2020 2020 2029 0a20  __}".        ). 
-0000a2a0: 2020 2020 2020 2073 656c 662e 7365 7457         self.setW
-0000a2b0: 696e 646f 7754 6974 6c65 286c 696e 6529  indowTitle(line)
-0000a2c0: 0a0a 2020 2020 6465 6620 636c 6561 7269  ..    def cleari
-0000a2d0: 6e70 7574 7328 7365 6c66 293a 0a20 2020  nputs(self):.   
-0000a2e0: 2020 2020 2022 2222 436c 6561 7273 2074       """Clears t
-0000a2f0: 6865 2074 6578 7420 696e 7075 7420 6669  he text input fi
-0000a300: 656c 6473 2061 6e64 2073 6574 7320 666f  elds and sets fo
-0000a310: 6375 7320 746f 2063 616c 6c73 6967 6e20  cus to callsign 
-0000a320: 6669 656c 642e 2222 220a 2020 2020 2020  field.""".      
-0000a330: 2020 7365 6c66 2e64 7570 655f 696e 6469    self.dupe_indi
-0000a340: 6361 746f 722e 6869 6465 2829 0a20 2020  cator.hide().   
-0000a350: 2020 2020 2073 656c 662e 636f 6e74 6163       self.contac
-0000a360: 7420 3d20 7365 6c66 2e64 6174 6162 6173  t = self.databas
-0000a370: 652e 656d 7074 795f 636f 6e74 6163 740a  e.empty_contact.
-0000a380: 2020 2020 2020 2020 7365 6c66 2e68 6561          self.hea
-0000a390: 6469 6e67 5f64 6973 7461 6e63 652e 7365  ding_distance.se
-0000a3a0: 7454 6578 7428 2222 290a 2020 2020 2020  tText("").      
-0000a3b0: 2020 7365 6c66 2e64 785f 656e 7469 7479    self.dx_entity
-0000a3c0: 2e73 6574 5465 7874 2822 2229 0a20 2020  .setText("").   
-0000a3d0: 2020 2020 2069 6620 7365 6c66 2e63 6f6e       if self.con
-0000a3e0: 7465 7374 3a0a 2020 2020 2020 2020 2020  test:.          
-0000a3f0: 2020 6d75 6c74 7320 3d20 7365 6c66 2e63    mults = self.c
-0000a400: 6f6e 7465 7374 2e73 686f 775f 6d75 6c74  ontest.show_mult
-0000a410: 7328 7365 6c66 290a 2020 2020 2020 2020  s(self).        
-0000a420: 2020 2020 7173 6f73 203d 2073 656c 662e      qsos = self.
-0000a430: 636f 6e74 6573 742e 7368 6f77 5f71 736f  contest.show_qso
-0000a440: 2873 656c 6629 0a20 2020 2020 2020 2020  (self).         
-0000a450: 2020 206d 756c 7473 7472 696e 6720 3d20     multstring = 
-0000a460: 6622 7b71 736f 737d 2f7b 6d75 6c74 737d  f"{qsos}/{mults}
-0000a470: 220a 2020 2020 2020 2020 2020 2020 7365  ".            se
-0000a480: 6c66 2e6d 756c 7473 2e73 6574 5465 7874  lf.mults.setText
-0000a490: 286d 756c 7473 7472 696e 6729 0a20 2020  (multstring).   
-0000a4a0: 2020 2020 2020 2020 2073 636f 7265 203d           score =
-0000a4b0: 2073 656c 662e 636f 6e74 6573 742e 6361   self.contest.ca
-0000a4c0: 6c63 5f73 636f 7265 2873 656c 6629 0a20  lc_score(self). 
-0000a4d0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000a4e0: 7363 6f72 652e 7365 7454 6578 7428 7374  score.setText(st
-0000a4f0: 7228 7363 6f72 6529 290a 2020 2020 2020  r(score)).      
-0000a500: 2020 2020 2020 7365 6c66 2e63 6f6e 7465        self.conte
-0000a510: 7374 2e72 6573 6574 5f6c 6162 656c 2873  st.reset_label(s
-0000a520: 656c 6629 0a20 2020 2020 2020 2073 656c  elf).        sel
-0000a530: 662e 6361 6c6c 7369 676e 2e63 6c65 6172  f.callsign.clear
-0000a540: 2829 0a20 2020 2020 2020 2069 6620 7365  ().        if se
-0000a550: 6c66 2e63 7572 7265 6e74 5f6d 6f64 6520  lf.current_mode 
-0000a560: 3d3d 2022 4357 223a 0a20 2020 2020 2020  == "CW":.       
-0000a570: 2020 2020 2073 656c 662e 7365 6e74 2e73       self.sent.s
-0000a580: 6574 5465 7874 2822 3539 3922 290a 2020  etText("599").  
-0000a590: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
-0000a5a0: 6563 6569 7665 2e73 6574 5465 7874 2822  eceive.setText("
-0000a5b0: 3539 3922 290a 2020 2020 2020 2020 656c  599").        el
-0000a5c0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-0000a5d0: 7365 6c66 2e73 656e 742e 7365 7454 6578  self.sent.setTex
-0000a5e0: 7428 2235 3922 290a 2020 2020 2020 2020  t("59").        
-0000a5f0: 2020 2020 7365 6c66 2e72 6563 6569 7665      self.receive
-0000a600: 2e73 6574 5465 7874 2822 3539 2229 0a20  .setText("59"). 
-0000a610: 2020 2020 2020 2073 656c 662e 6f74 6865         self.othe
-0000a620: 725f 312e 636c 6561 7228 290a 2020 2020  r_1.clear().    
-0000a630: 2020 2020 7365 6c66 2e6f 7468 6572 5f32      self.other_2
-0000a640: 2e63 6c65 6172 2829 0a20 2020 2020 2020  .clear().       
-0000a650: 2073 656c 662e 6361 6c6c 7369 676e 2e73   self.callsign.s
-0000a660: 6574 466f 6375 7328 290a 2020 2020 2020  etFocus().      
-0000a670: 2020 636d 6420 3d20 7b7d 0a20 2020 2020    cmd = {}.     
-0000a680: 2020 2063 6d64 5b22 636d 6422 5d20 3d20     cmd["cmd"] = 
-0000a690: 2243 414c 4c43 4841 4e47 4544 220a 2020  "CALLCHANGED".  
-0000a6a0: 2020 2020 2020 636d 645b 2273 7461 7469        cmd["stati
-0000a6b0: 6f6e 225d 203d 2070 6c61 7466 6f72 6d2e  on"] = platform.
-0000a6c0: 6e6f 6465 2829 0a20 2020 2020 2020 2063  node().        c
-0000a6d0: 6d64 5b22 6361 6c6c 225d 203d 2022 220a  md["call"] = "".
-0000a6e0: 2020 2020 2020 2020 7365 6c66 2e6d 756c          self.mul
-0000a6f0: 7469 6361 7374 5f69 6e74 6572 6661 6365  ticast_interface
-0000a700: 2e73 656e 645f 6173 5f6a 736f 6e28 636d  .send_as_json(cm
-0000a710: 6429 0a0a 2020 2020 6465 6620 7361 7665  d)..    def save
-0000a720: 5f63 6f6e 7461 6374 2873 656c 6629 3a0a  _contact(self):.
-0000a730: 2020 2020 2020 2020 2222 2253 6176 6520          """Save 
-0000a740: 746f 2064 6222 2222 0a20 2020 2020 2020  to db""".       
-0000a750: 206c 6f67 6765 722e 6465 6275 6728 2273   logger.debug("s
-0000a760: 6176 696e 6720 636f 6e74 6163 7422 290a  aving contact").
-0000a770: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0000a780: 636f 6e74 6573 7420 6973 204e 6f6e 653a  contest is None:
-0000a790: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000a7a0: 662e 7368 6f77 5f6d 6573 7361 6765 5f62  f.show_message_b
-0000a7b0: 6f78 2822 596f 7520 6861 7665 206e 6f20  ox("You have no 
-0000a7c0: 636f 6e74 6573 7420 6465 6669 6e65 642e  contest defined.
-0000a7d0: 2229 0a20 2020 2020 2020 2020 2020 2072  ").            r
-0000a7e0: 6574 7572 6e0a 2020 2020 2020 2020 6966  eturn.        if
-0000a7f0: 206c 656e 2873 656c 662e 6361 6c6c 7369   len(self.callsi
-0000a800: 676e 2e74 6578 7428 2929 203c 2033 3a0a  gn.text()) < 3:.
-0000a810: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0000a820: 726e 0a20 2020 2020 2020 2069 6620 6e6f  rn.        if no
-0000a830: 7420 616e 7928 6368 6172 2e69 7364 6967  t any(char.isdig
-0000a840: 6974 2829 2066 6f72 2063 6861 7220 696e  it() for char in
-0000a850: 2073 656c 662e 6361 6c6c 7369 676e 2e74   self.callsign.t
-0000a860: 6578 7428 2929 3a0a 2020 2020 2020 2020  ext()):.        
-0000a870: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
-0000a880: 2020 2069 6620 6e6f 7420 616e 7928 6368     if not any(ch
-0000a890: 6172 2e69 7361 6c70 6861 2829 2066 6f72  ar.isalpha() for
-0000a8a0: 2063 6861 7220 696e 2073 656c 662e 6361   char in self.ca
-0000a8b0: 6c6c 7369 676e 2e74 6578 7428 2929 3a0a  llsign.text()):.
-0000a8c0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0000a8d0: 726e 0a0a 2020 2020 2020 2020 7365 6c66  rn..        self
-0000a8e0: 2e63 6f6e 7461 6374 5b22 5453 225d 203d  .contact["TS"] =
-0000a8f0: 2064 6174 6574 696d 652e 7574 636e 6f77   datetime.utcnow
-0000a900: 2829 2e69 736f 666f 726d 6174 2822 2022  ().isoformat(" "
-0000a910: 295b 3a31 395d 0a20 2020 2020 2020 2073  )[:19].        s
-0000a920: 656c 662e 636f 6e74 6163 745b 2243 616c  elf.contact["Cal
-0000a930: 6c22 5d20 3d20 7365 6c66 2e63 616c 6c73  l"] = self.calls
-0000a940: 6967 6e2e 7465 7874 2829 0a20 2020 2020  ign.text().     
-0000a950: 2020 2073 656c 662e 636f 6e74 6163 745b     self.contact[
-0000a960: 2246 7265 7122 5d20 3d20 726f 756e 6428  "Freq"] = round(
-0000a970: 666c 6f61 7428 7365 6c66 2e72 6164 696f  float(self.radio
-0000a980: 5f73 7461 7465 2e67 6574 2822 7666 6f61  _state.get("vfoa
-0000a990: 222c 2030 2e30 2929 202f 2031 3030 302c  ", 0.0)) / 1000,
-0000a9a0: 2032 290a 2020 2020 2020 2020 7365 6c66   2).        self
-0000a9b0: 2e63 6f6e 7461 6374 5b22 5153 5846 7265  .contact["QSXFre
-0000a9c0: 7122 5d20 3d20 726f 756e 6428 0a20 2020  q"] = round(.   
-0000a9d0: 2020 2020 2020 2020 2066 6c6f 6174 2873           float(s
-0000a9e0: 656c 662e 7261 6469 6f5f 7374 6174 652e  elf.radio_state.
-0000a9f0: 6765 7428 2276 666f 6122 2c20 302e 3029  get("vfoa", 0.0)
-0000aa00: 2920 2f20 3130 3030 2c20 320a 2020 2020  ) / 1000, 2.    
-0000aa10: 2020 2020 290a 2020 2020 2020 2020 7365      ).        se
-0000aa20: 6c66 2e63 6f6e 7461 6374 5b22 4d6f 6465  lf.contact["Mode
-0000aa30: 225d 203d 2073 656c 662e 7261 6469 6f5f  "] = self.radio_
-0000aa40: 7374 6174 652e 6765 7428 226d 6f64 6522  state.get("mode"
-0000aa50: 2c20 2222 290a 2020 2020 2020 2020 7365  , "").        se
-0000aa60: 6c66 2e63 6f6e 7461 6374 5b22 436f 6e74  lf.contact["Cont
-0000aa70: 6573 744e 616d 6522 5d20 3d20 7365 6c66  estName"] = self
-0000aa80: 2e63 6f6e 7465 7374 2e63 6162 7269 6c6c  .contest.cabrill
-0000aa90: 6f5f 6e61 6d65 0a20 2020 2020 2020 2073  o_name.        s
-0000aaa0: 656c 662e 636f 6e74 6163 745b 2243 6f6e  elf.contact["Con
-0000aab0: 7465 7374 4e52 225d 203d 2073 656c 662e  testNR"] = self.
-0000aac0: 7072 6566 2e67 6574 2822 636f 6e74 6573  pref.get("contes
-0000aad0: 7422 2c20 2230 2229 0a20 2020 2020 2020  t", "0").       
-0000aae0: 2073 656c 662e 636f 6e74 6163 745b 2253   self.contact["S
-0000aaf0: 7461 7469 6f6e 5072 6566 6978 225d 203d  tationPrefix"] =
-0000ab00: 2073 656c 662e 7374 6174 696f 6e2e 6765   self.station.ge
-0000ab10: 7428 2243 616c 6c22 2c20 2222 290a 2020  t("Call", "").  
-0000ab20: 2020 2020 2020 7365 6c66 2e63 6f6e 7461        self.conta
-0000ab30: 6374 5b22 5750 5850 7265 6669 7822 5d20  ct["WPXPrefix"] 
-0000ab40: 3d20 6361 6c63 756c 6174 655f 7770 785f  = calculate_wpx_
-0000ab50: 7072 6566 6978 2873 656c 662e 6361 6c6c  prefix(self.call
-0000ab60: 7369 676e 2e74 6578 7428 2929 0a20 2020  sign.text()).   
-0000ab70: 2020 2020 2073 656c 662e 636f 6e74 6163       self.contac
-0000ab80: 745b 2249 7352 756e 5153 4f22 5d20 3d20  t["IsRunQSO"] = 
-0000ab90: 7365 6c66 2e72 6164 696f 4275 7474 6f6e  self.radioButton
-0000aba0: 5f72 756e 2e69 7343 6865 636b 6564 2829  _run.isChecked()
-0000abb0: 0a20 2020 2020 2020 2073 656c 662e 636f  .        self.co
-0000abc0: 6e74 6163 745b 224f 7065 7261 746f 7222  ntact["Operator"
-0000abd0: 5d20 3d20 7365 6c66 2e63 7572 7265 6e74  ] = self.current
-0000abe0: 5f6f 700a 2020 2020 2020 2020 7365 6c66  _op.        self
-0000abf0: 2e63 6f6e 7461 6374 5b22 4e65 7442 696f  .contact["NetBio
-0000ac00: 734e 616d 6522 5d20 3d20 736f 636b 6574  sName"] = socket
-0000ac10: 2e67 6574 686f 7374 6e61 6d65 2829 0a20  .gethostname(). 
-0000ac20: 2020 2020 2020 2073 656c 662e 636f 6e74         self.cont
-0000ac30: 6163 745b 2249 734f 7269 6769 6e61 6c22  act["IsOriginal"
-0000ac40: 5d20 3d20 310a 2020 2020 2020 2020 7365  ] = 1.        se
-0000ac50: 6c66 2e63 6f6e 7461 6374 5b22 4944 225d  lf.contact["ID"]
-0000ac60: 203d 2075 7569 642e 7575 6964 3428 292e   = uuid.uuid4().
-0000ac70: 6865 780a 2020 2020 2020 2020 7365 6c66  hex.        self
-0000ac80: 2e63 6f6e 7465 7374 2e73 6574 5f63 6f6e  .contest.set_con
-0000ac90: 7461 6374 5f76 6172 7328 7365 6c66 290a  tact_vars(self).
-0000aca0: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
-0000acb0: 7461 6374 5b22 506f 696e 7473 225d 203d  tact["Points"] =
-0000acc0: 2073 656c 662e 636f 6e74 6573 742e 706f   self.contest.po
-0000acd0: 696e 7473 2873 656c 6629 0a20 2020 2020  ints(self).     
-0000ace0: 2020 2064 6562 7567 5f6f 7574 7075 7420     debug_output 
-0000acf0: 3d20 6622 7b73 656c 662e 636f 6e74 6163  = f"{self.contac
-0000ad00: 747d 220a 2020 2020 2020 2020 6c6f 6767  t}".        logg
-0000ad10: 6572 2e64 6562 7567 2864 6562 7567 5f6f  er.debug(debug_o
-0000ad20: 7574 7075 7429 0a0a 2020 2020 2020 2020  utput)..        
-0000ad30: 6966 2073 656c 662e 6e31 6d6d 3a0a 2020  if self.n1mm:.  
-0000ad40: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
-0000ad50: 2e64 6562 7567 2822 7061 636b 6574 7320  .debug("packets 
-0000ad60: 2573 222c 2066 227b 7365 6c66 2e6e 316d  %s", f"{self.n1m
-0000ad70: 6d2e 7365 6e64 5f63 6f6e 7461 6374 5f70  m.send_contact_p
-0000ad80: 6163 6b65 7473 7d22 290a 2020 2020 2020  ackets}").      
-0000ad90: 2020 2020 2020 6966 2073 656c 662e 6e31        if self.n1
-0000ada0: 6d6d 2e73 656e 645f 636f 6e74 6163 745f  mm.send_contact_
-0000adb0: 7061 636b 6574 733a 0a20 2020 2020 2020  packets:.       
-0000adc0: 2020 2020 2020 2020 2073 656c 662e 6e31           self.n1
-0000add0: 6d6d 2e63 6f6e 7461 6374 5f69 6e66 6f5b  mm.contact_info[
-0000ade0: 2274 696d 6573 7461 6d70 225d 203d 2073  "timestamp"] = s
-0000adf0: 656c 662e 636f 6e74 6163 745b 2254 5322  elf.contact["TS"
-0000ae00: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+00009cb0: 2020 6172 6773 3d28 7465 7874 2c29 2c0a    args=(text,),.
+00009cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009cd0: 2020 2020 2020 2020 6461 656d 6f6e 3d54          daemon=T
+00009ce0: 7275 652c 0a20 2020 2020 2020 2020 2020  rue,.           
+00009cf0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+00009d00: 2020 2020 2020 2020 2020 2020 2020 205f                 _
+00009d10: 7468 6574 6872 6561 642e 7374 6172 7428  thethread.start(
+00009d20: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00009d30: 2020 2020 2020 6e65 7874 5f74 6162 203d        next_tab =
+00009d40: 2073 656c 662e 7461 625f 6e65 7874 2e67   self.tab_next.g
+00009d50: 6574 2873 656c 662e 6361 6c6c 7369 676e  et(self.callsign
+00009d60: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00009d70: 2020 2020 2020 6e65 7874 5f74 6162 2e73        next_tab.s
+00009d80: 6574 466f 6375 7328 290a 2020 2020 2020  etFocus().      
+00009d90: 2020 2020 2020 2020 2020 2020 2020 6e65                ne
+00009da0: 7874 5f74 6162 2e64 6573 656c 6563 7428  xt_tab.deselect(
+00009db0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00009dc0: 2020 2020 2020 6e65 7874 5f74 6162 2e65        next_tab.e
+00009dd0: 6e64 2846 616c 7365 290a 2020 2020 2020  nd(False).      
+00009de0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00009df0: 0a20 2020 2020 2020 2069 6620 6576 656e  .        if even
+00009e00: 742e 6b65 7928 2920 3d3d 2051 742e 4b65  t.key() == Qt.Ke
+00009e10: 795f 4631 3a0a 2020 2020 2020 2020 2020  y_F1:.          
+00009e20: 2020 7365 6c66 2e73 656e 6466 3128 290a    self.sendf1().
+00009e30: 2020 2020 2020 2020 6966 2065 7665 6e74          if event
+00009e40: 2e6b 6579 2829 203d 3d20 5174 2e4b 6579  .key() == Qt.Key
+00009e50: 5f46 323a 0a20 2020 2020 2020 2020 2020  _F2:.           
+00009e60: 2073 656c 662e 7365 6e64 6632 2829 0a20   self.sendf2(). 
+00009e70: 2020 2020 2020 2069 6620 6576 656e 742e         if event.
+00009e80: 6b65 7928 2920 3d3d 2051 742e 4b65 795f  key() == Qt.Key_
+00009e90: 4633 3a0a 2020 2020 2020 2020 2020 2020  F3:.            
+00009ea0: 7365 6c66 2e73 656e 6466 3328 290a 2020  self.sendf3().  
+00009eb0: 2020 2020 2020 6966 2065 7665 6e74 2e6b        if event.k
+00009ec0: 6579 2829 203d 3d20 5174 2e4b 6579 5f46  ey() == Qt.Key_F
+00009ed0: 343a 0a20 2020 2020 2020 2020 2020 2073  4:.            s
+00009ee0: 656c 662e 7365 6e64 6634 2829 0a20 2020  elf.sendf4().   
+00009ef0: 2020 2020 2069 6620 6576 656e 742e 6b65       if event.ke
+00009f00: 7928 2920 3d3d 2051 742e 4b65 795f 4635  y() == Qt.Key_F5
+00009f10: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00009f20: 6c66 2e73 656e 6466 3528 290a 2020 2020  lf.sendf5().    
+00009f30: 2020 2020 6966 2065 7665 6e74 2e6b 6579      if event.key
+00009f40: 2829 203d 3d20 5174 2e4b 6579 5f46 363a  () == Qt.Key_F6:
+00009f50: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00009f60: 662e 7365 6e64 6636 2829 0a20 2020 2020  f.sendf6().     
+00009f70: 2020 2069 6620 6576 656e 742e 6b65 7928     if event.key(
+00009f80: 2920 3d3d 2051 742e 4b65 795f 4637 3a0a  ) == Qt.Key_F7:.
+00009f90: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00009fa0: 2e73 656e 6466 3728 290a 2020 2020 2020  .sendf7().      
+00009fb0: 2020 6966 2065 7665 6e74 2e6b 6579 2829    if event.key()
+00009fc0: 203d 3d20 5174 2e4b 6579 5f46 383a 0a20   == Qt.Key_F8:. 
+00009fd0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00009fe0: 7365 6e64 6638 2829 0a20 2020 2020 2020  sendf8().       
+00009ff0: 2069 6620 6576 656e 742e 6b65 7928 2920   if event.key() 
+0000a000: 3d3d 2051 742e 4b65 795f 4639 3a0a 2020  == Qt.Key_F9:.  
+0000a010: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+0000a020: 656e 6466 3928 290a 2020 2020 2020 2020  endf9().        
+0000a030: 6966 2065 7665 6e74 2e6b 6579 2829 203d  if event.key() =
+0000a040: 3d20 5174 2e4b 6579 5f46 3130 3a0a 2020  = Qt.Key_F10:.  
+0000a050: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+0000a060: 656e 6466 3130 2829 0a20 2020 2020 2020  endf10().       
+0000a070: 2069 6620 6576 656e 742e 6b65 7928 2920   if event.key() 
+0000a080: 3d3d 2051 742e 4b65 795f 4631 313a 0a20  == Qt.Key_F11:. 
+0000a090: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000a0a0: 7365 6e64 6631 3128 290a 2020 2020 2020  sendf11().      
+0000a0b0: 2020 6966 2065 7665 6e74 2e6b 6579 2829    if event.key()
+0000a0c0: 203d 3d20 5174 2e4b 6579 5f46 3132 3a0a   == Qt.Key_F12:.
+0000a0d0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000a0e0: 2e73 656e 6466 3132 2829 0a0a 2020 2020  .sendf12()..    
+0000a0f0: 6465 6620 7365 745f 7769 6e64 6f77 5f74  def set_window_t
+0000a100: 6974 6c65 2873 656c 6629 3a0a 2020 2020  itle(self):.    
+0000a110: 2020 2020 2222 2253 6574 2077 696e 646f      """Set windo
+0000a120: 7720 7469 746c 6522 2222 0a20 2020 2020  w title""".     
+0000a130: 2020 2076 666f 6120 3d20 7365 6c66 2e72     vfoa = self.r
+0000a140: 6164 696f 5f73 7461 7465 2e67 6574 2822  adio_state.get("
+0000a150: 7666 6f61 222c 2022 2229 0a20 2020 2020  vfoa", "").     
+0000a160: 2020 2069 6620 7666 6f61 3a0a 2020 2020     if vfoa:.    
+0000a170: 2020 2020 2020 2020 7666 6f61 203d 2069          vfoa = i
+0000a180: 6e74 2876 666f 6129 202f 2031 3030 300a  nt(vfoa) / 1000.
+0000a190: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+0000a1a0: 2020 2020 2020 2020 2020 7666 6f61 203d            vfoa =
+0000a1b0: 2030 2e30 0a20 2020 2020 2020 2063 6f6e   0.0.        con
+0000a1c0: 7465 7374 5f6e 616d 6520 3d20 2222 0a20  test_name = "". 
+0000a1d0: 2020 2020 2020 2069 6620 7365 6c66 2e63         if self.c
+0000a1e0: 6f6e 7465 7374 3a0a 2020 2020 2020 2020  ontest:.        
+0000a1f0: 2020 2020 636f 6e74 6573 745f 6e61 6d65      contest_name
+0000a200: 203d 2073 656c 662e 636f 6e74 6573 742e   = self.contest.
+0000a210: 6e61 6d65 0a20 2020 2020 2020 206c 696e  name.        lin
+0000a220: 6520 3d20 280a 2020 2020 2020 2020 2020  e = (.          
+0000a230: 2020 6622 7666 6f61 3a7b 726f 756e 6428    f"vfoa:{round(
+0000a240: 7666 6f61 2c32 297d 2022 0a20 2020 2020  vfoa,2)} ".     
+0000a250: 2020 2020 2020 2066 226d 6f64 653a 7b73         f"mode:{s
+0000a260: 656c 662e 7261 6469 6f5f 7374 6174 652e  elf.radio_state.
+0000a270: 6765 7428 276d 6f64 6527 2c20 2727 297d  get('mode', '')}
+0000a280: 2022 0a20 2020 2020 2020 2020 2020 2066   ".            f
+0000a290: 224f 503a 7b73 656c 662e 6375 7272 656e  "OP:{self.curren
+0000a2a0: 745f 6f70 7d20 7b63 6f6e 7465 7374 5f6e  t_op} {contest_n
+0000a2b0: 616d 657d 2022 0a20 2020 2020 2020 2020  ame} ".         
+0000a2c0: 2020 2066 222d 204e 6f74 314d 4d20 767b     f"- Not1MM v{
+0000a2d0: 5f5f 7665 7273 696f 6e5f 5f7d 220a 2020  __version__}".  
+0000a2e0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+0000a2f0: 7365 6c66 2e73 6574 5769 6e64 6f77 5469  self.setWindowTi
+0000a300: 746c 6528 6c69 6e65 290a 0a20 2020 2064  tle(line)..    d
+0000a310: 6566 2063 6c65 6172 696e 7075 7473 2873  ef clearinputs(s
+0000a320: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
+0000a330: 2243 6c65 6172 7320 7468 6520 7465 7874  "Clears the text
+0000a340: 2069 6e70 7574 2066 6965 6c64 7320 616e   input fields an
+0000a350: 6420 7365 7473 2066 6f63 7573 2074 6f20  d sets focus to 
+0000a360: 6361 6c6c 7369 676e 2066 6965 6c64 2e22  callsign field."
+0000a370: 2222 0a20 2020 2020 2020 2073 656c 662e  "".        self.
+0000a380: 6475 7065 5f69 6e64 6963 6174 6f72 2e68  dupe_indicator.h
+0000a390: 6964 6528 290a 2020 2020 2020 2020 7365  ide().        se
+0000a3a0: 6c66 2e63 6f6e 7461 6374 203d 2073 656c  lf.contact = sel
+0000a3b0: 662e 6461 7461 6261 7365 2e65 6d70 7479  f.database.empty
+0000a3c0: 5f63 6f6e 7461 6374 0a20 2020 2020 2020  _contact.       
+0000a3d0: 2073 656c 662e 6865 6164 696e 675f 6469   self.heading_di
+0000a3e0: 7374 616e 6365 2e73 6574 5465 7874 2822  stance.setText("
+0000a3f0: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
+0000a400: 6478 5f65 6e74 6974 792e 7365 7454 6578  dx_entity.setTex
+0000a410: 7428 2222 290a 2020 2020 2020 2020 6966  t("").        if
+0000a420: 2073 656c 662e 636f 6e74 6573 743a 0a20   self.contest:. 
+0000a430: 2020 2020 2020 2020 2020 206d 756c 7473             mults
+0000a440: 203d 2073 656c 662e 636f 6e74 6573 742e   = self.contest.
+0000a450: 7368 6f77 5f6d 756c 7473 2873 656c 6629  show_mults(self)
+0000a460: 0a20 2020 2020 2020 2020 2020 2071 736f  .            qso
+0000a470: 7320 3d20 7365 6c66 2e63 6f6e 7465 7374  s = self.contest
+0000a480: 2e73 686f 775f 7173 6f28 7365 6c66 290a  .show_qso(self).
+0000a490: 2020 2020 2020 2020 2020 2020 6d75 6c74              mult
+0000a4a0: 7374 7269 6e67 203d 2066 227b 7173 6f73  string = f"{qsos
+0000a4b0: 7d2f 7b6d 756c 7473 7d22 0a20 2020 2020  }/{mults}".     
+0000a4c0: 2020 2020 2020 2073 656c 662e 6d75 6c74         self.mult
+0000a4d0: 732e 7365 7454 6578 7428 6d75 6c74 7374  s.setText(multst
+0000a4e0: 7269 6e67 290a 2020 2020 2020 2020 2020  ring).          
+0000a4f0: 2020 7363 6f72 6520 3d20 7365 6c66 2e63    score = self.c
+0000a500: 6f6e 7465 7374 2e63 616c 635f 7363 6f72  ontest.calc_scor
+0000a510: 6528 7365 6c66 290a 2020 2020 2020 2020  e(self).        
+0000a520: 2020 2020 7365 6c66 2e73 636f 7265 2e73      self.score.s
+0000a530: 6574 5465 7874 2873 7472 2873 636f 7265  etText(str(score
+0000a540: 2929 0a20 2020 2020 2020 2020 2020 2073  )).            s
+0000a550: 656c 662e 636f 6e74 6573 742e 7265 7365  elf.contest.rese
+0000a560: 745f 6c61 6265 6c28 7365 6c66 290a 2020  t_label(self).  
+0000a570: 2020 2020 2020 7365 6c66 2e63 616c 6c73        self.calls
+0000a580: 6967 6e2e 636c 6561 7228 290a 2020 2020  ign.clear().    
+0000a590: 2020 2020 6966 2073 656c 662e 6375 7272      if self.curr
+0000a5a0: 656e 745f 6d6f 6465 203d 3d20 2243 5722  ent_mode == "CW"
+0000a5b0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0000a5c0: 6c66 2e73 656e 742e 7365 7454 6578 7428  lf.sent.setText(
+0000a5d0: 2235 3939 2229 0a20 2020 2020 2020 2020  "599").         
+0000a5e0: 2020 2073 656c 662e 7265 6365 6976 652e     self.receive.
+0000a5f0: 7365 7454 6578 7428 2235 3939 2229 0a20  setText("599"). 
+0000a600: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+0000a610: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
+0000a620: 6e74 2e73 6574 5465 7874 2822 3539 2229  nt.setText("59")
+0000a630: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000a640: 662e 7265 6365 6976 652e 7365 7454 6578  f.receive.setTex
+0000a650: 7428 2235 3922 290a 2020 2020 2020 2020  t("59").        
+0000a660: 7365 6c66 2e6f 7468 6572 5f31 2e63 6c65  self.other_1.cle
+0000a670: 6172 2829 0a20 2020 2020 2020 2073 656c  ar().        sel
+0000a680: 662e 6f74 6865 725f 322e 636c 6561 7228  f.other_2.clear(
+0000a690: 290a 2020 2020 2020 2020 7365 6c66 2e63  ).        self.c
+0000a6a0: 616c 6c73 6967 6e2e 7365 7446 6f63 7573  allsign.setFocus
+0000a6b0: 2829 0a20 2020 2020 2020 2063 6d64 203d  ().        cmd =
+0000a6c0: 207b 7d0a 2020 2020 2020 2020 636d 645b   {}.        cmd[
+0000a6d0: 2263 6d64 225d 203d 2022 4341 4c4c 4348  "cmd"] = "CALLCH
+0000a6e0: 414e 4745 4422 0a20 2020 2020 2020 2063  ANGED".        c
+0000a6f0: 6d64 5b22 7374 6174 696f 6e22 5d20 3d20  md["station"] = 
+0000a700: 706c 6174 666f 726d 2e6e 6f64 6528 290a  platform.node().
+0000a710: 2020 2020 2020 2020 636d 645b 2263 616c          cmd["cal
+0000a720: 6c22 5d20 3d20 2222 0a20 2020 2020 2020  l"] = "".       
+0000a730: 2073 656c 662e 6d75 6c74 6963 6173 745f   self.multicast_
+0000a740: 696e 7465 7266 6163 652e 7365 6e64 5f61  interface.send_a
+0000a750: 735f 6a73 6f6e 2863 6d64 290a 0a20 2020  s_json(cmd)..   
+0000a760: 2064 6566 2073 6176 655f 636f 6e74 6163   def save_contac
+0000a770: 7428 7365 6c66 293a 0a20 2020 2020 2020  t(self):.       
+0000a780: 2022 2222 5361 7665 2074 6f20 6462 2222   """Save to db""
+0000a790: 220a 2020 2020 2020 2020 6c6f 6767 6572  ".        logger
+0000a7a0: 2e64 6562 7567 2822 7361 7669 6e67 2063  .debug("saving c
+0000a7b0: 6f6e 7461 6374 2229 0a20 2020 2020 2020  ontact").       
+0000a7c0: 2069 6620 7365 6c66 2e63 6f6e 7465 7374   if self.contest
+0000a7d0: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
+0000a7e0: 2020 2020 2020 7365 6c66 2e73 686f 775f        self.show_
+0000a7f0: 6d65 7373 6167 655f 626f 7828 2259 6f75  message_box("You
+0000a800: 2068 6176 6520 6e6f 2063 6f6e 7465 7374   have no contest
+0000a810: 2064 6566 696e 6564 2e22 290a 2020 2020   defined.").    
+0000a820: 2020 2020 2020 2020 7265 7475 726e 0a20          return. 
+0000a830: 2020 2020 2020 2069 6620 6c65 6e28 7365         if len(se
+0000a840: 6c66 2e63 616c 6c73 6967 6e2e 7465 7874  lf.callsign.text
+0000a850: 2829 2920 3c20 333a 0a20 2020 2020 2020  ()) < 3:.       
+0000a860: 2020 2020 2072 6574 7572 6e0a 2020 2020       return.    
+0000a870: 2020 2020 6966 206e 6f74 2061 6e79 2863      if not any(c
+0000a880: 6861 722e 6973 6469 6769 7428 2920 666f  har.isdigit() fo
+0000a890: 7220 6368 6172 2069 6e20 7365 6c66 2e63  r char in self.c
+0000a8a0: 616c 6c73 6967 6e2e 7465 7874 2829 293a  allsign.text()):
+0000a8b0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+0000a8c0: 7572 6e0a 2020 2020 2020 2020 6966 206e  urn.        if n
+0000a8d0: 6f74 2061 6e79 2863 6861 722e 6973 616c  ot any(char.isal
+0000a8e0: 7068 6128 2920 666f 7220 6368 6172 2069  pha() for char i
+0000a8f0: 6e20 7365 6c66 2e63 616c 6c73 6967 6e2e  n self.callsign.
+0000a900: 7465 7874 2829 293a 0a20 2020 2020 2020  text()):.       
+0000a910: 2020 2020 2072 6574 7572 6e0a 0a20 2020       return..   
+0000a920: 2020 2020 2073 656c 662e 636f 6e74 6163       self.contac
+0000a930: 745b 2254 5322 5d20 3d20 6461 7465 7469  t["TS"] = dateti
+0000a940: 6d65 2e75 7463 6e6f 7728 292e 6973 6f66  me.utcnow().isof
+0000a950: 6f72 6d61 7428 2220 2229 5b3a 3139 5d0a  ormat(" ")[:19].
+0000a960: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
+0000a970: 7461 6374 5b22 4361 6c6c 225d 203d 2073  tact["Call"] = s
+0000a980: 656c 662e 6361 6c6c 7369 676e 2e74 6578  elf.callsign.tex
+0000a990: 7428 290a 2020 2020 2020 2020 7365 6c66  t().        self
+0000a9a0: 2e63 6f6e 7461 6374 5b22 4672 6571 225d  .contact["Freq"]
+0000a9b0: 203d 2072 6f75 6e64 2866 6c6f 6174 2873   = round(float(s
+0000a9c0: 656c 662e 7261 6469 6f5f 7374 6174 652e  elf.radio_state.
+0000a9d0: 6765 7428 2276 666f 6122 2c20 302e 3029  get("vfoa", 0.0)
+0000a9e0: 2920 2f20 3130 3030 2c20 3229 0a20 2020  ) / 1000, 2).   
+0000a9f0: 2020 2020 2073 656c 662e 636f 6e74 6163       self.contac
+0000aa00: 745b 2251 5358 4672 6571 225d 203d 2072  t["QSXFreq"] = r
+0000aa10: 6f75 6e64 280a 2020 2020 2020 2020 2020  ound(.          
+0000aa20: 2020 666c 6f61 7428 7365 6c66 2e72 6164    float(self.rad
+0000aa30: 696f 5f73 7461 7465 2e67 6574 2822 7666  io_state.get("vf
+0000aa40: 6f61 222c 2030 2e30 2929 202f 2031 3030  oa", 0.0)) / 100
+0000aa50: 302c 2032 0a20 2020 2020 2020 2029 0a20  0, 2.        ). 
+0000aa60: 2020 2020 2020 2073 656c 662e 636f 6e74         self.cont
+0000aa70: 6163 745b 224d 6f64 6522 5d20 3d20 7365  act["Mode"] = se
+0000aa80: 6c66 2e72 6164 696f 5f73 7461 7465 2e67  lf.radio_state.g
+0000aa90: 6574 2822 6d6f 6465 222c 2022 2229 0a20  et("mode", ""). 
+0000aaa0: 2020 2020 2020 2073 656c 662e 636f 6e74         self.cont
+0000aab0: 6163 745b 2243 6f6e 7465 7374 4e61 6d65  act["ContestName
+0000aac0: 225d 203d 2073 656c 662e 636f 6e74 6573  "] = self.contes
+0000aad0: 742e 6361 6272 696c 6c6f 5f6e 616d 650a  t.cabrillo_name.
+0000aae0: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
+0000aaf0: 7461 6374 5b22 436f 6e74 6573 744e 5222  tact["ContestNR"
+0000ab00: 5d20 3d20 7365 6c66 2e70 7265 662e 6765  ] = self.pref.ge
+0000ab10: 7428 2263 6f6e 7465 7374 222c 2022 3022  t("contest", "0"
+0000ab20: 290a 2020 2020 2020 2020 7365 6c66 2e63  ).        self.c
+0000ab30: 6f6e 7461 6374 5b22 5374 6174 696f 6e50  ontact["StationP
+0000ab40: 7265 6669 7822 5d20 3d20 7365 6c66 2e73  refix"] = self.s
+0000ab50: 7461 7469 6f6e 2e67 6574 2822 4361 6c6c  tation.get("Call
+0000ab60: 222c 2022 2229 0a20 2020 2020 2020 2073  ", "").        s
+0000ab70: 656c 662e 636f 6e74 6163 745b 2257 5058  elf.contact["WPX
+0000ab80: 5072 6566 6978 225d 203d 2063 616c 6375  Prefix"] = calcu
+0000ab90: 6c61 7465 5f77 7078 5f70 7265 6669 7828  late_wpx_prefix(
+0000aba0: 7365 6c66 2e63 616c 6c73 6967 6e2e 7465  self.callsign.te
+0000abb0: 7874 2829 290a 2020 2020 2020 2020 7365  xt()).        se
+0000abc0: 6c66 2e63 6f6e 7461 6374 5b22 4973 5275  lf.contact["IsRu
+0000abd0: 6e51 534f 225d 203d 2073 656c 662e 7261  nQSO"] = self.ra
+0000abe0: 6469 6f42 7574 746f 6e5f 7275 6e2e 6973  dioButton_run.is
+0000abf0: 4368 6563 6b65 6428 290a 2020 2020 2020  Checked().      
+0000ac00: 2020 7365 6c66 2e63 6f6e 7461 6374 5b22    self.contact["
+0000ac10: 4f70 6572 6174 6f72 225d 203d 2073 656c  Operator"] = sel
+0000ac20: 662e 6375 7272 656e 745f 6f70 0a20 2020  f.current_op.   
+0000ac30: 2020 2020 2073 656c 662e 636f 6e74 6163       self.contac
+0000ac40: 745b 224e 6574 4269 6f73 4e61 6d65 225d  t["NetBiosName"]
+0000ac50: 203d 2073 6f63 6b65 742e 6765 7468 6f73   = socket.gethos
+0000ac60: 746e 616d 6528 290a 2020 2020 2020 2020  tname().        
+0000ac70: 7365 6c66 2e63 6f6e 7461 6374 5b22 4973  self.contact["Is
+0000ac80: 4f72 6967 696e 616c 225d 203d 2031 0a20  Original"] = 1. 
+0000ac90: 2020 2020 2020 2073 656c 662e 636f 6e74         self.cont
+0000aca0: 6163 745b 2249 4422 5d20 3d20 7575 6964  act["ID"] = uuid
+0000acb0: 2e75 7569 6434 2829 2e68 6578 0a20 2020  .uuid4().hex.   
+0000acc0: 2020 2020 2073 656c 662e 636f 6e74 6573       self.contes
+0000acd0: 742e 7365 745f 636f 6e74 6163 745f 7661  t.set_contact_va
+0000ace0: 7273 2873 656c 6629 0a20 2020 2020 2020  rs(self).       
+0000acf0: 2073 656c 662e 636f 6e74 6163 745b 2250   self.contact["P
+0000ad00: 6f69 6e74 7322 5d20 3d20 7365 6c66 2e63  oints"] = self.c
+0000ad10: 6f6e 7465 7374 2e70 6f69 6e74 7328 7365  ontest.points(se
+0000ad20: 6c66 290a 2020 2020 2020 2020 6465 6275  lf).        debu
+0000ad30: 675f 6f75 7470 7574 203d 2066 227b 7365  g_output = f"{se
+0000ad40: 6c66 2e63 6f6e 7461 6374 7d22 0a20 2020  lf.contact}".   
+0000ad50: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
+0000ad60: 6728 6465 6275 675f 6f75 7470 7574 290a  g(debug_output).
+0000ad70: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+0000ad80: 2e6e 316d 6d3a 0a20 2020 2020 2020 2020  .n1mm:.         
+0000ad90: 2020 206c 6f67 6765 722e 6465 6275 6728     logger.debug(
+0000ada0: 2270 6163 6b65 7473 2025 7322 2c20 6622  "packets %s", f"
+0000adb0: 7b73 656c 662e 6e31 6d6d 2e73 656e 645f  {self.n1mm.send_
+0000adc0: 636f 6e74 6163 745f 7061 636b 6574 737d  contact_packets}
+0000add0: 2229 0a20 2020 2020 2020 2020 2020 2069  ").            i
+0000ade0: 6620 7365 6c66 2e6e 316d 6d2e 7365 6e64  f self.n1mm.send
+0000adf0: 5f63 6f6e 7461 6374 5f70 6163 6b65 7473  _contact_packets
+0000ae00: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
 0000ae10: 2020 7365 6c66 2e6e 316d 6d2e 636f 6e74    self.n1mm.cont
-0000ae20: 6163 745f 696e 666f 5b22 6f6c 6463 616c  act_info["oldcal
-0000ae30: 6c22 5d20 3d20 7365 6c66 2e6e 316d 6d2e  l"] = self.n1mm.
-0000ae40: 636f 6e74 6163 745f 696e 666f 5b0a 2020  contact_info[.  
-0000ae50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ae60: 2020 2263 616c 6c22 0a20 2020 2020 2020    "call".       
-0000ae70: 2020 2020 2020 2020 205d 203d 2073 656c           ] = sel
-0000ae80: 662e 636f 6e74 6163 745b 2243 616c 6c22  f.contact["Call"
-0000ae90: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
-0000aea0: 2020 7365 6c66 2e6e 316d 6d2e 636f 6e74    self.n1mm.cont
-0000aeb0: 6163 745f 696e 666f 5b22 7478 6672 6571  act_info["txfreq
-0000aec0: 225d 203d 2073 656c 662e 6e31 6d6d 2e63  "] = self.n1mm.c
-0000aed0: 6f6e 7461 6374 5f69 6e66 6f5b 0a20 2020  ontact_info[.   
-0000aee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aef0: 2022 7278 6672 6571 220a 2020 2020 2020   "rxfreq".      
-0000af00: 2020 2020 2020 2020 2020 5d20 3d20 7365            ] = se
-0000af10: 6c66 2e6e 316d 6d2e 7261 6469 6f5f 696e  lf.n1mm.radio_in
-0000af20: 666f 5b22 4672 6571 225d 0a20 2020 2020  fo["Freq"].     
-0000af30: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000af40: 6e31 6d6d 2e63 6f6e 7461 6374 5f69 6e66  n1mm.contact_inf
-0000af50: 6f5b 226d 6f64 6522 5d20 3d20 7365 6c66  o["mode"] = self
-0000af60: 2e63 6f6e 7461 6374 5b22 4d6f 6465 225d  .contact["Mode"]
-0000af70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000af80: 2073 656c 662e 6e31 6d6d 2e63 6f6e 7461   self.n1mm.conta
-0000af90: 6374 5f69 6e66 6f5b 2263 6f6e 7465 7374  ct_info["contest
-0000afa0: 6e61 6d65 225d 203d 2073 656c 662e 636f  name"] = self.co
-0000afb0: 6e74 6163 745b 0a20 2020 2020 2020 2020  ntact[.         
-0000afc0: 2020 2020 2020 2020 2020 2022 436f 6e74             "Cont
-0000afd0: 6573 744e 616d 6522 0a20 2020 2020 2020  estName".       
-0000afe0: 2020 2020 2020 2020 205d 2e72 6570 6c61           ].repla
-0000aff0: 6365 2822 2d22 2c20 2222 290a 2020 2020  ce("-", "").    
-0000b000: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000b010: 2e6e 316d 6d2e 636f 6e74 6163 745f 696e  .n1mm.contact_in
-0000b020: 666f 5b22 636f 6e74 6573 746e 7222 5d20  fo["contestnr"] 
-0000b030: 3d20 7365 6c66 2e63 6f6e 7461 6374 5b22  = self.contact["
-0000b040: 436f 6e74 6573 744e 5222 5d0a 2020 2020  ContestNR"].    
-0000b050: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000b060: 2e6e 316d 6d2e 636f 6e74 6163 745f 696e  .n1mm.contact_in
-0000b070: 666f 5b22 7374 6174 696f 6e70 7265 6669  fo["stationprefi
-0000b080: 7822 5d20 3d20 7365 6c66 2e63 6f6e 7461  x"] = self.conta
-0000b090: 6374 5b22 5374 6174 696f 6e50 7265 6669  ct["StationPrefi
-0000b0a0: 7822 5d0a 2020 2020 2020 2020 2020 2020  x"].            
-0000b0b0: 2020 2020 7365 6c66 2e6e 316d 6d2e 636f      self.n1mm.co
-0000b0c0: 6e74 6163 745f 696e 666f 5b22 7770 7870  ntact_info["wpxp
-0000b0d0: 7265 6669 7822 5d20 3d20 7365 6c66 2e63  refix"] = self.c
-0000b0e0: 6f6e 7461 6374 5b22 5750 5850 7265 6669  ontact["WPXPrefi
-0000b0f0: 7822 5d0a 2020 2020 2020 2020 2020 2020  x"].            
-0000b100: 2020 2020 7365 6c66 2e6e 316d 6d2e 636f      self.n1mm.co
-0000b110: 6e74 6163 745f 696e 666f 5b22 4973 5275  ntact_info["IsRu
-0000b120: 6e51 534f 225d 203d 2073 656c 662e 636f  nQSO"] = self.co
-0000b130: 6e74 6163 745b 2249 7352 756e 5153 4f22  ntact["IsRunQSO"
-0000b140: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
-0000b150: 2020 7365 6c66 2e6e 316d 6d2e 636f 6e74    self.n1mm.cont
-0000b160: 6163 745f 696e 666f 5b22 6f70 6572 6174  act_info["operat
-0000b170: 6f72 225d 203d 2073 656c 662e 636f 6e74  or"] = self.cont
-0000b180: 6163 745b 224f 7065 7261 746f 7222 5d0a  act["Operator"].
-0000b190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b1a0: 7365 6c66 2e6e 316d 6d2e 636f 6e74 6163  self.n1mm.contac
-0000b1b0: 745f 696e 666f 5b22 6d79 6361 6c6c 225d  t_info["mycall"]
-0000b1c0: 203d 2073 656c 662e 636f 6e74 6163 745b   = self.contact[
-0000b1d0: 224f 7065 7261 746f 7222 5d0a 2020 2020  "Operator"].    
-0000b1e0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000b1f0: 2e6e 316d 6d2e 636f 6e74 6163 745f 696e  .n1mm.contact_in
-0000b200: 666f 5b22 5374 6174 696f 6e4e 616d 6522  fo["StationName"
-0000b210: 5d20 3d20 7365 6c66 2e6e 316d 6d2e 636f  ] = self.n1mm.co
-0000b220: 6e74 6163 745f 696e 666f 5b0a 2020 2020  ntact_info[.    
-0000b230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b240: 224e 6574 4269 6f73 4e61 6d65 220a 2020  "NetBiosName".  
-0000b250: 2020 2020 2020 2020 2020 2020 2020 5d20                ] 
-0000b260: 3d20 7365 6c66 2e63 6f6e 7461 6374 5b22  = self.contact["
-0000b270: 4e65 7442 696f 734e 616d 6522 5d0a 2020  NetBiosName"].  
-0000b280: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000b290: 6c66 2e6e 316d 6d2e 636f 6e74 6163 745f  lf.n1mm.contact_
-0000b2a0: 696e 666f 5b22 4973 4f72 6967 696e 616c  info["IsOriginal
-0000b2b0: 225d 203d 2073 656c 662e 636f 6e74 6163  "] = self.contac
-0000b2c0: 745b 2249 734f 7269 6769 6e61 6c22 5d0a  t["IsOriginal"].
-0000b2d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b2e0: 7365 6c66 2e6e 316d 6d2e 636f 6e74 6163  self.n1mm.contac
-0000b2f0: 745f 696e 666f 5b22 4944 225d 203d 2073  t_info["ID"] = s
-0000b300: 656c 662e 636f 6e74 6163 745b 2249 4422  elf.contact["ID"
-0000b310: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
-0000b320: 2020 7365 6c66 2e6e 316d 6d2e 636f 6e74    self.n1mm.cont
-0000b330: 6163 745f 696e 666f 5b22 706f 696e 7473  act_info["points
-0000b340: 225d 203d 2073 656c 662e 636f 6e74 6163  "] = self.contac
-0000b350: 745b 2250 6f69 6e74 7322 5d0a 2020 2020  t["Points"].    
-0000b360: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000b370: 2e6e 316d 6d2e 636f 6e74 6163 745f 696e  .n1mm.contact_in
-0000b380: 666f 5b22 736e 7422 5d20 3d20 7365 6c66  fo["snt"] = self
-0000b390: 2e63 6f6e 7461 6374 5b22 534e 5422 5d0a  .contact["SNT"].
-0000b3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b3b0: 7365 6c66 2e6e 316d 6d2e 636f 6e74 6163  self.n1mm.contac
-0000b3c0: 745f 696e 666f 5b22 7263 7622 5d20 3d20  t_info["rcv"] = 
-0000b3d0: 7365 6c66 2e63 6f6e 7461 6374 5b22 5243  self.contact["RC
-0000b3e0: 5622 5d0a 2020 2020 2020 2020 2020 2020  V"].            
-0000b3f0: 2020 2020 7365 6c66 2e6e 316d 6d2e 636f      self.n1mm.co
-0000b400: 6e74 6163 745f 696e 666f 5b22 736e 746e  ntact_info["sntn
-0000b410: 7222 5d20 3d20 7365 6c66 2e63 6f6e 7461  r"] = self.conta
-0000b420: 6374 5b22 5365 6e74 4e72 225d 0a20 2020  ct["SentNr"].   
+0000ae20: 6163 745f 696e 666f 5b22 7469 6d65 7374  act_info["timest
+0000ae30: 616d 7022 5d20 3d20 7365 6c66 2e63 6f6e  amp"] = self.con
+0000ae40: 7461 6374 5b22 5453 225d 0a20 2020 2020  tact["TS"].     
+0000ae50: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000ae60: 6e31 6d6d 2e63 6f6e 7461 6374 5f69 6e66  n1mm.contact_inf
+0000ae70: 6f5b 226f 6c64 6361 6c6c 225d 203d 2073  o["oldcall"] = s
+0000ae80: 656c 662e 6e31 6d6d 2e63 6f6e 7461 6374  elf.n1mm.contact
+0000ae90: 5f69 6e66 6f5b 0a20 2020 2020 2020 2020  _info[.         
+0000aea0: 2020 2020 2020 2020 2020 2022 6361 6c6c             "call
+0000aeb0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+0000aec0: 2020 5d20 3d20 7365 6c66 2e63 6f6e 7461    ] = self.conta
+0000aed0: 6374 5b22 4361 6c6c 225d 0a20 2020 2020  ct["Call"].     
+0000aee0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000aef0: 6e31 6d6d 2e63 6f6e 7461 6374 5f69 6e66  n1mm.contact_inf
+0000af00: 6f5b 2274 7866 7265 7122 5d20 3d20 7365  o["txfreq"] = se
+0000af10: 6c66 2e6e 316d 6d2e 636f 6e74 6163 745f  lf.n1mm.contact_
+0000af20: 696e 666f 5b0a 2020 2020 2020 2020 2020  info[.          
+0000af30: 2020 2020 2020 2020 2020 2272 7866 7265            "rxfre
+0000af40: 7122 0a20 2020 2020 2020 2020 2020 2020  q".             
+0000af50: 2020 205d 203d 2073 656c 662e 6e31 6d6d     ] = self.n1mm
+0000af60: 2e72 6164 696f 5f69 6e66 6f5b 2246 7265  .radio_info["Fre
+0000af70: 7122 5d0a 2020 2020 2020 2020 2020 2020  q"].            
+0000af80: 2020 2020 7365 6c66 2e6e 316d 6d2e 636f      self.n1mm.co
+0000af90: 6e74 6163 745f 696e 666f 5b22 6d6f 6465  ntact_info["mode
+0000afa0: 225d 203d 2073 656c 662e 636f 6e74 6163  "] = self.contac
+0000afb0: 745b 224d 6f64 6522 5d0a 2020 2020 2020  t["Mode"].      
+0000afc0: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
+0000afd0: 316d 6d2e 636f 6e74 6163 745f 696e 666f  1mm.contact_info
+0000afe0: 5b22 636f 6e74 6573 746e 616d 6522 5d20  ["contestname"] 
+0000aff0: 3d20 7365 6c66 2e63 6f6e 7461 6374 5b0a  = self.contact[.
+0000b000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b010: 2020 2020 2243 6f6e 7465 7374 4e61 6d65      "ContestName
+0000b020: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+0000b030: 2020 5d2e 7265 706c 6163 6528 222d 222c    ].replace("-",
+0000b040: 2022 2229 0a20 2020 2020 2020 2020 2020   "").           
+0000b050: 2020 2020 2073 656c 662e 6e31 6d6d 2e63       self.n1mm.c
+0000b060: 6f6e 7461 6374 5f69 6e66 6f5b 2263 6f6e  ontact_info["con
+0000b070: 7465 7374 6e72 225d 203d 2073 656c 662e  testnr"] = self.
+0000b080: 636f 6e74 6163 745b 2243 6f6e 7465 7374  contact["Contest
+0000b090: 4e52 225d 0a20 2020 2020 2020 2020 2020  NR"].           
+0000b0a0: 2020 2020 2073 656c 662e 6e31 6d6d 2e63       self.n1mm.c
+0000b0b0: 6f6e 7461 6374 5f69 6e66 6f5b 2273 7461  ontact_info["sta
+0000b0c0: 7469 6f6e 7072 6566 6978 225d 203d 2073  tionprefix"] = s
+0000b0d0: 656c 662e 636f 6e74 6163 745b 2253 7461  elf.contact["Sta
+0000b0e0: 7469 6f6e 5072 6566 6978 225d 0a20 2020  tionPrefix"].   
+0000b0f0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000b100: 662e 6e31 6d6d 2e63 6f6e 7461 6374 5f69  f.n1mm.contact_i
+0000b110: 6e66 6f5b 2277 7078 7072 6566 6978 225d  nfo["wpxprefix"]
+0000b120: 203d 2073 656c 662e 636f 6e74 6163 745b   = self.contact[
+0000b130: 2257 5058 5072 6566 6978 225d 0a20 2020  "WPXPrefix"].   
+0000b140: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000b150: 662e 6e31 6d6d 2e63 6f6e 7461 6374 5f69  f.n1mm.contact_i
+0000b160: 6e66 6f5b 2249 7352 756e 5153 4f22 5d20  nfo["IsRunQSO"] 
+0000b170: 3d20 7365 6c66 2e63 6f6e 7461 6374 5b22  = self.contact["
+0000b180: 4973 5275 6e51 534f 225d 0a20 2020 2020  IsRunQSO"].     
+0000b190: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000b1a0: 6e31 6d6d 2e63 6f6e 7461 6374 5f69 6e66  n1mm.contact_inf
+0000b1b0: 6f5b 226f 7065 7261 746f 7222 5d20 3d20  o["operator"] = 
+0000b1c0: 7365 6c66 2e63 6f6e 7461 6374 5b22 4f70  self.contact["Op
+0000b1d0: 6572 6174 6f72 225d 0a20 2020 2020 2020  erator"].       
+0000b1e0: 2020 2020 2020 2020 2073 656c 662e 6e31           self.n1
+0000b1f0: 6d6d 2e63 6f6e 7461 6374 5f69 6e66 6f5b  mm.contact_info[
+0000b200: 226d 7963 616c 6c22 5d20 3d20 7365 6c66  "mycall"] = self
+0000b210: 2e63 6f6e 7461 6374 5b22 4f70 6572 6174  .contact["Operat
+0000b220: 6f72 225d 0a20 2020 2020 2020 2020 2020  or"].           
+0000b230: 2020 2020 2073 656c 662e 6e31 6d6d 2e63       self.n1mm.c
+0000b240: 6f6e 7461 6374 5f69 6e66 6f5b 2253 7461  ontact_info["Sta
+0000b250: 7469 6f6e 4e61 6d65 225d 203d 2073 656c  tionName"] = sel
+0000b260: 662e 6e31 6d6d 2e63 6f6e 7461 6374 5f69  f.n1mm.contact_i
+0000b270: 6e66 6f5b 0a20 2020 2020 2020 2020 2020  nfo[.           
+0000b280: 2020 2020 2020 2020 2022 4e65 7442 696f           "NetBio
+0000b290: 734e 616d 6522 0a20 2020 2020 2020 2020  sName".         
+0000b2a0: 2020 2020 2020 205d 203d 2073 656c 662e         ] = self.
+0000b2b0: 636f 6e74 6163 745b 224e 6574 4269 6f73  contact["NetBios
+0000b2c0: 4e61 6d65 225d 0a20 2020 2020 2020 2020  Name"].         
+0000b2d0: 2020 2020 2020 2073 656c 662e 6e31 6d6d         self.n1mm
+0000b2e0: 2e63 6f6e 7461 6374 5f69 6e66 6f5b 2249  .contact_info["I
+0000b2f0: 734f 7269 6769 6e61 6c22 5d20 3d20 7365  sOriginal"] = se
+0000b300: 6c66 2e63 6f6e 7461 6374 5b22 4973 4f72  lf.contact["IsOr
+0000b310: 6967 696e 616c 225d 0a20 2020 2020 2020  iginal"].       
+0000b320: 2020 2020 2020 2020 2073 656c 662e 6e31           self.n1
+0000b330: 6d6d 2e63 6f6e 7461 6374 5f69 6e66 6f5b  mm.contact_info[
+0000b340: 2249 4422 5d20 3d20 7365 6c66 2e63 6f6e  "ID"] = self.con
+0000b350: 7461 6374 5b22 4944 225d 0a20 2020 2020  tact["ID"].     
+0000b360: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000b370: 6e31 6d6d 2e63 6f6e 7461 6374 5f69 6e66  n1mm.contact_inf
+0000b380: 6f5b 2270 6f69 6e74 7322 5d20 3d20 7365  o["points"] = se
+0000b390: 6c66 2e63 6f6e 7461 6374 5b22 506f 696e  lf.contact["Poin
+0000b3a0: 7473 225d 0a20 2020 2020 2020 2020 2020  ts"].           
+0000b3b0: 2020 2020 2073 656c 662e 6e31 6d6d 2e63       self.n1mm.c
+0000b3c0: 6f6e 7461 6374 5f69 6e66 6f5b 2273 6e74  ontact_info["snt
+0000b3d0: 225d 203d 2073 656c 662e 636f 6e74 6163  "] = self.contac
+0000b3e0: 745b 2253 4e54 225d 0a20 2020 2020 2020  t["SNT"].       
+0000b3f0: 2020 2020 2020 2020 2073 656c 662e 6e31           self.n1
+0000b400: 6d6d 2e63 6f6e 7461 6374 5f69 6e66 6f5b  mm.contact_info[
+0000b410: 2272 6376 225d 203d 2073 656c 662e 636f  "rcv"] = self.co
+0000b420: 6e74 6163 745b 2252 4356 225d 0a20 2020  ntact["RCV"].   
 0000b430: 2020 2020 2020 2020 2020 2020 2073 656c               sel
 0000b440: 662e 6e31 6d6d 2e63 6f6e 7461 6374 5f69  f.n1mm.contact_i
-0000b450: 6e66 6f5b 2272 6376 6e72 225d 203d 2073  nfo["rcvnr"] = s
-0000b460: 656c 662e 636f 6e74 6163 745b 224e 5222  elf.contact["NR"
-0000b470: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
-0000b480: 2020 7365 6c66 2e6e 316d 6d2e 636f 6e74    self.n1mm.cont
-0000b490: 6163 745f 696e 666f 5b22 6973 6d75 6c74  act_info["ismult
-0000b4a0: 6970 6c69 6572 3122 5d20 3d20 7365 6c66  iplier1"] = self
-0000b4b0: 2e63 6f6e 7461 6374 2e67 6574 280a 2020  .contact.get(.  
-0000b4c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b4d0: 2020 2249 734d 756c 7469 706c 6965 7231    "IsMultiplier1
-0000b4e0: 222c 2030 0a20 2020 2020 2020 2020 2020  ", 0.           
-0000b4f0: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-0000b500: 2020 2020 2020 2073 656c 662e 6e31 6d6d         self.n1mm
-0000b510: 2e63 6f6e 7461 6374 5f69 6e66 6f5b 2269  .contact_info["i
-0000b520: 736d 756c 7469 706c 6965 7232 225d 203d  smultiplier2"] =
-0000b530: 2073 656c 662e 636f 6e74 6163 742e 6765   self.contact.ge
-0000b540: 7428 0a20 2020 2020 2020 2020 2020 2020  t(.             
-0000b550: 2020 2020 2020 2022 4973 4d75 6c74 6970         "IsMultip
-0000b560: 6c69 6572 3222 2c20 300a 2020 2020 2020  lier2", 0.      
-0000b570: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-0000b580: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000b590: 2e6e 316d 6d2e 636f 6e74 6163 745f 696e  .n1mm.contact_in
-0000b5a0: 666f 5b22 6973 6d75 6c74 6970 6c69 6572  fo["ismultiplier
-0000b5b0: 3322 5d20 3d20 7365 6c66 2e63 6f6e 7461  3"] = self.conta
-0000b5c0: 6374 2e67 6574 280a 2020 2020 2020 2020  ct.get(.        
-0000b5d0: 2020 2020 2020 2020 2020 2020 2249 734d              "IsM
-0000b5e0: 756c 7469 706c 6965 7233 222c 2022 3022  ultiplier3", "0"
-0000b5f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000b600: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
-0000b610: 2020 2073 656c 662e 6e31 6d6d 2e63 6f6e     self.n1mm.con
-0000b620: 7461 6374 5f69 6e66 6f5b 2273 6563 7469  tact_info["secti
-0000b630: 6f6e 225d 203d 2073 656c 662e 636f 6e74  on"] = self.cont
-0000b640: 6163 745b 2253 6563 7422 5d0a 2020 2020  act["Sect"].    
+0000b450: 6e66 6f5b 2273 6e74 6e72 225d 203d 2073  nfo["sntnr"] = s
+0000b460: 656c 662e 636f 6e74 6163 745b 2253 656e  elf.contact["Sen
+0000b470: 744e 7222 5d0a 2020 2020 2020 2020 2020  tNr"].          
+0000b480: 2020 2020 2020 7365 6c66 2e6e 316d 6d2e        self.n1mm.
+0000b490: 636f 6e74 6163 745f 696e 666f 5b22 7263  contact_info["rc
+0000b4a0: 766e 7222 5d20 3d20 7365 6c66 2e63 6f6e  vnr"] = self.con
+0000b4b0: 7461 6374 5b22 4e52 225d 0a20 2020 2020  tact["NR"].     
+0000b4c0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000b4d0: 6e31 6d6d 2e63 6f6e 7461 6374 5f69 6e66  n1mm.contact_inf
+0000b4e0: 6f5b 2269 736d 756c 7469 706c 6965 7231  o["ismultiplier1
+0000b4f0: 225d 203d 2073 656c 662e 636f 6e74 6163  "] = self.contac
+0000b500: 742e 6765 7428 0a20 2020 2020 2020 2020  t.get(.         
+0000b510: 2020 2020 2020 2020 2020 2022 4973 4d75             "IsMu
+0000b520: 6c74 6970 6c69 6572 3122 2c20 300a 2020  ltiplier1", 0.  
+0000b530: 2020 2020 2020 2020 2020 2020 2020 290a                ).
+0000b540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b550: 7365 6c66 2e6e 316d 6d2e 636f 6e74 6163  self.n1mm.contac
+0000b560: 745f 696e 666f 5b22 6973 6d75 6c74 6970  t_info["ismultip
+0000b570: 6c69 6572 3222 5d20 3d20 7365 6c66 2e63  lier2"] = self.c
+0000b580: 6f6e 7461 6374 2e67 6574 280a 2020 2020  ontact.get(.    
+0000b590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b5a0: 2249 734d 756c 7469 706c 6965 7232 222c  "IsMultiplier2",
+0000b5b0: 2030 0a20 2020 2020 2020 2020 2020 2020   0.             
+0000b5c0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+0000b5d0: 2020 2020 2073 656c 662e 6e31 6d6d 2e63       self.n1mm.c
+0000b5e0: 6f6e 7461 6374 5f69 6e66 6f5b 2269 736d  ontact_info["ism
+0000b5f0: 756c 7469 706c 6965 7233 225d 203d 2073  ultiplier3"] = s
+0000b600: 656c 662e 636f 6e74 6163 742e 6765 7428  elf.contact.get(
+0000b610: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b620: 2020 2020 2022 4973 4d75 6c74 6970 6c69       "IsMultipli
+0000b630: 6572 3322 2c20 2230 220a 2020 2020 2020  er3", "0".      
+0000b640: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
 0000b650: 2020 2020 2020 2020 2020 2020 7365 6c66              self
 0000b660: 2e6e 316d 6d2e 636f 6e74 6163 745f 696e  .n1mm.contact_in
-0000b670: 666f 5b22 7072 6563 225d 203d 2073 656c  fo["prec"] = sel
-0000b680: 662e 636f 6e74 6163 745b 2250 7265 6322  f.contact["Prec"
-0000b690: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
-0000b6a0: 2020 7365 6c66 2e6e 316d 6d2e 636f 6e74    self.n1mm.cont
-0000b6b0: 6163 745f 696e 666f 5b22 636b 225d 203d  act_info["ck"] =
-0000b6c0: 2073 656c 662e 636f 6e74 6163 745b 2243   self.contact["C
-0000b6d0: 4b22 5d0a 2020 2020 2020 2020 2020 2020  K"].            
-0000b6e0: 2020 2020 7365 6c66 2e6e 316d 6d2e 636f      self.n1mm.co
-0000b6f0: 6e74 6163 745f 696e 666f 5b22 7a6e 225d  ntact_info["zn"]
-0000b700: 203d 2073 656c 662e 636f 6e74 6163 745b   = self.contact[
-0000b710: 225a 4e22 5d0a 2020 2020 2020 2020 2020  "ZN"].          
-0000b720: 2020 2020 2020 7365 6c66 2e6e 316d 6d2e        self.n1mm.
-0000b730: 636f 6e74 6163 745f 696e 666f 5b22 706f  contact_info["po
-0000b740: 7765 7222 5d20 3d20 7365 6c66 2e63 6f6e  wer"] = self.con
-0000b750: 7461 6374 5b22 506f 7765 7222 5d0a 2020  tact["Power"].  
-0000b760: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000b770: 6c66 2e6e 316d 6d2e 636f 6e74 6163 745f  lf.n1mm.contact_
-0000b780: 696e 666f 5b22 6261 6e64 225d 203d 2073  info["band"] = s
-0000b790: 656c 662e 636f 6e74 6163 745b 2242 616e  elf.contact["Ban
-0000b7a0: 6422 5d0a 2020 2020 2020 2020 2020 2020  d"].            
-0000b7b0: 2020 2020 2320 7365 6c66 2e6e 316d 6d2e      # self.n1mm.
-0000b7c0: 636f 6e74 6163 745f 696e 666f 5b27 275d  contact_info['']
-0000b7d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000b7e0: 2023 2073 656c 662e 6e31 6d6d 2e63 6f6e   # self.n1mm.con
-0000b7f0: 7461 6374 5f69 6e66 6f5b 2727 5d0a 2020  tact_info[''].  
-0000b800: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-0000b810: 7365 6c66 2e6e 316d 6d2e 636f 6e74 6163  self.n1mm.contac
-0000b820: 745f 696e 666f 5b27 275d 0a20 2020 2020  t_info[''].     
-0000b830: 2020 2020 2020 2020 2020 2023 2073 656c             # sel
-0000b840: 662e 6e31 6d6d 2e63 6f6e 7461 6374 5f69  f.n1mm.contact_i
-0000b850: 6e66 6f5b 2727 5d0a 2020 2020 2020 2020  nfo[''].        
-0000b860: 2020 2020 2020 2020 2320 7365 6c66 2e6e          # self.n
-0000b870: 316d 6d2e 636f 6e74 6163 745f 696e 666f  1mm.contact_info
-0000b880: 5b27 275d 0a20 2020 2020 2020 2020 2020  [''].           
-0000b890: 2020 2020 2023 2073 656c 662e 6e31 6d6d       # self.n1mm
-0000b8a0: 2e63 6f6e 7461 6374 5f69 6e66 6f5b 2727  .contact_info[''
-0000b8b0: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
-0000b8c0: 2020 6c6f 6767 6572 2e64 6562 7567 2822    logger.debug("
-0000b8d0: 2573 222c 2066 227b 7365 6c66 2e6e 316d  %s", f"{self.n1m
-0000b8e0: 6d2e 636f 6e74 6163 745f 696e 666f 7d22  m.contact_info}"
-0000b8f0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000b900: 2020 7365 6c66 2e6e 316d 6d2e 7365 6e64    self.n1mm.send
-0000b910: 5f63 6f6e 7461 6374 5f69 6e66 6f28 290a  _contact_info().
-0000b920: 0a20 2020 2020 2020 2073 656c 662e 6461  .        self.da
-0000b930: 7461 6261 7365 2e6c 6f67 5f63 6f6e 7461  tabase.log_conta
-0000b940: 6374 2873 656c 662e 636f 6e74 6163 7429  ct(self.contact)
-0000b950: 0a20 2020 2020 2020 2073 656c 662e 636c  .        self.cl
-0000b960: 6561 7269 6e70 7574 7328 290a 2020 2020  earinputs().    
-0000b970: 2020 2020 636d 6420 3d20 7b7d 0a20 2020      cmd = {}.   
-0000b980: 2020 2020 2063 6d64 5b22 636d 6422 5d20       cmd["cmd"] 
-0000b990: 3d20 2255 5044 4154 454c 4f47 220a 2020  = "UPDATELOG".  
-0000b9a0: 2020 2020 2020 636d 645b 2273 7461 7469        cmd["stati
-0000b9b0: 6f6e 225d 203d 2070 6c61 7466 6f72 6d2e  on"] = platform.
-0000b9c0: 6e6f 6465 2829 0a20 2020 2020 2020 2073  node().        s
-0000b9d0: 656c 662e 6d75 6c74 6963 6173 745f 696e  elf.multicast_in
-0000b9e0: 7465 7266 6163 652e 7365 6e64 5f61 735f  terface.send_as_
-0000b9f0: 6a73 6f6e 2863 6d64 290a 2020 2020 2020  json(cmd).      
-0000ba00: 2020 2320 7365 6c66 2e63 6f6e 7461 6374    # self.contact
-0000ba10: 5b22 436f 6e74 6573 744e 616d 6522 5d20  ["ContestName"] 
-0000ba20: 3d20 7365 6c66 2e63 6f6e 7465 7374 2e6e  = self.contest.n
-0000ba30: 616d 650a 2020 2020 2020 2020 2320 7365  ame.        # se
-0000ba40: 6c66 2e63 6f6e 7461 6374 5b22 534e 5422  lf.contact["SNT"
-0000ba50: 5d20 3d20 7365 6c66 2e73 656e 742e 7465  ] = self.sent.te
-0000ba60: 7874 2829 0a20 2020 2020 2020 2023 2073  xt().        # s
-0000ba70: 656c 662e 636f 6e74 6163 745b 2252 4356  elf.contact["RCV
-0000ba80: 225d 203d 2073 656c 662e 7265 6365 6976  "] = self.receiv
-0000ba90: 652e 7465 7874 2829 0a20 2020 2020 2020  e.text().       
-0000baa0: 2023 2073 656c 662e 636f 6e74 6163 745b   # self.contact[
-0000bab0: 2243 6f75 6e74 7279 5072 6566 6978 225d  "CountryPrefix"]
-0000bac0: 0a20 2020 2020 2020 2023 2073 656c 662e  .        # self.
-0000bad0: 636f 6e74 6163 745b 2253 7461 7469 6f6e  contact["Station
-0000bae0: 5072 6566 6978 225d 203d 2073 656c 662e  Prefix"] = self.
-0000baf0: 7072 6566 2e67 6574 2822 6361 6c6c 7369  pref.get("callsi
-0000bb00: 676e 222c 2022 2229 0a20 2020 2020 2020  gn", "").       
-0000bb10: 2023 2073 656c 662e 636f 6e74 6163 745b   # self.contact[
-0000bb20: 2251 5448 225d 0a20 2020 2020 2020 2023  "QTH"].        #
-0000bb30: 2073 656c 662e 636f 6e74 6163 745b 224e   self.contact["N
-0000bb40: 616d 6522 5d20 3d20 7365 6c66 2e6f 7468  ame"] = self.oth
-0000bb50: 6572 5f31 2e74 6578 7428 290a 2020 2020  er_1.text().    
-0000bb60: 2020 2020 2320 7365 6c66 2e63 6f6e 7461      # self.conta
-0000bb70: 6374 5b22 436f 6d6d 656e 7422 5d20 3d20  ct["Comment"] = 
-0000bb80: 7365 6c66 2e6f 7468 6572 5f32 2e74 6578  self.other_2.tex
-0000bb90: 7428 290a 2020 2020 2020 2020 2320 7365  t().        # se
-0000bba0: 6c66 2e63 6f6e 7461 6374 5b22 4e52 225d  lf.contact["NR"]
-0000bbb0: 0a20 2020 2020 2020 2023 2073 656c 662e  .        # self.
-0000bbc0: 636f 6e74 6163 745b 2253 6563 7422 5d0a  contact["Sect"].
-0000bbd0: 2020 2020 2020 2020 2320 7365 6c66 2e63          # self.c
-0000bbe0: 6f6e 7461 6374 5b22 5072 6563 225d 0a20  ontact["Prec"]. 
-0000bbf0: 2020 2020 2020 2023 2073 656c 662e 636f         # self.co
-0000bc00: 6e74 6163 745b 2243 4b22 5d0a 2020 2020  ntact["CK"].    
-0000bc10: 2020 2020 2320 7365 6c66 2e63 6f6e 7461      # self.conta
-0000bc20: 6374 5b22 5a4e 225d 0a20 2020 2020 2020  ct["ZN"].       
-0000bc30: 2023 2073 656c 662e 636f 6e74 6163 745b   # self.contact[
-0000bc40: 2253 656e 744e 7222 5d0a 2020 2020 2020  "SentNr"].      
-0000bc50: 2020 2320 7365 6c66 2e63 6f6e 7461 6374    # self.contact
-0000bc60: 5b22 506f 696e 7473 225d 0a20 2020 2020  ["Points"].     
-0000bc70: 2020 2023 2073 656c 662e 636f 6e74 6163     # self.contac
-0000bc80: 745b 2249 734d 756c 7469 706c 6965 7231  t["IsMultiplier1
+0000b670: 666f 5b22 7365 6374 696f 6e22 5d20 3d20  fo["section"] = 
+0000b680: 7365 6c66 2e63 6f6e 7461 6374 5b22 5365  self.contact["Se
+0000b690: 6374 225d 0a20 2020 2020 2020 2020 2020  ct"].           
+0000b6a0: 2020 2020 2073 656c 662e 6e31 6d6d 2e63       self.n1mm.c
+0000b6b0: 6f6e 7461 6374 5f69 6e66 6f5b 2270 7265  ontact_info["pre
+0000b6c0: 6322 5d20 3d20 7365 6c66 2e63 6f6e 7461  c"] = self.conta
+0000b6d0: 6374 5b22 5072 6563 225d 0a20 2020 2020  ct["Prec"].     
+0000b6e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000b6f0: 6e31 6d6d 2e63 6f6e 7461 6374 5f69 6e66  n1mm.contact_inf
+0000b700: 6f5b 2263 6b22 5d20 3d20 7365 6c66 2e63  o["ck"] = self.c
+0000b710: 6f6e 7461 6374 5b22 434b 225d 0a20 2020  ontact["CK"].   
+0000b720: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000b730: 662e 6e31 6d6d 2e63 6f6e 7461 6374 5f69  f.n1mm.contact_i
+0000b740: 6e66 6f5b 227a 6e22 5d20 3d20 7365 6c66  nfo["zn"] = self
+0000b750: 2e63 6f6e 7461 6374 5b22 5a4e 225d 0a20  .contact["ZN"]. 
+0000b760: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000b770: 656c 662e 6e31 6d6d 2e63 6f6e 7461 6374  elf.n1mm.contact
+0000b780: 5f69 6e66 6f5b 2270 6f77 6572 225d 203d  _info["power"] =
+0000b790: 2073 656c 662e 636f 6e74 6163 745b 2250   self.contact["P
+0000b7a0: 6f77 6572 225d 0a20 2020 2020 2020 2020  ower"].         
+0000b7b0: 2020 2020 2020 2073 656c 662e 6e31 6d6d         self.n1mm
+0000b7c0: 2e63 6f6e 7461 6374 5f69 6e66 6f5b 2262  .contact_info["b
+0000b7d0: 616e 6422 5d20 3d20 7365 6c66 2e63 6f6e  and"] = self.con
+0000b7e0: 7461 6374 5b22 4261 6e64 225d 0a20 2020  tact["Band"].   
+0000b7f0: 2020 2020 2020 2020 2020 2020 2023 2073               # s
+0000b800: 656c 662e 6e31 6d6d 2e63 6f6e 7461 6374  elf.n1mm.contact
+0000b810: 5f69 6e66 6f5b 2727 5d0a 2020 2020 2020  _info[''].      
+0000b820: 2020 2020 2020 2020 2020 2320 7365 6c66            # self
+0000b830: 2e6e 316d 6d2e 636f 6e74 6163 745f 696e  .n1mm.contact_in
+0000b840: 666f 5b27 275d 0a20 2020 2020 2020 2020  fo[''].         
+0000b850: 2020 2020 2020 2023 2073 656c 662e 6e31         # self.n1
+0000b860: 6d6d 2e63 6f6e 7461 6374 5f69 6e66 6f5b  mm.contact_info[
+0000b870: 2727 5d0a 2020 2020 2020 2020 2020 2020  ''].            
+0000b880: 2020 2020 2320 7365 6c66 2e6e 316d 6d2e      # self.n1mm.
+0000b890: 636f 6e74 6163 745f 696e 666f 5b27 275d  contact_info['']
+0000b8a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b8b0: 2023 2073 656c 662e 6e31 6d6d 2e63 6f6e   # self.n1mm.con
+0000b8c0: 7461 6374 5f69 6e66 6f5b 2727 5d0a 2020  tact_info[''].  
+0000b8d0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+0000b8e0: 7365 6c66 2e6e 316d 6d2e 636f 6e74 6163  self.n1mm.contac
+0000b8f0: 745f 696e 666f 5b27 275d 0a20 2020 2020  t_info[''].     
+0000b900: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
+0000b910: 722e 6465 6275 6728 2225 7322 2c20 6622  r.debug("%s", f"
+0000b920: 7b73 656c 662e 6e31 6d6d 2e63 6f6e 7461  {self.n1mm.conta
+0000b930: 6374 5f69 6e66 6f7d 2229 0a20 2020 2020  ct_info}").     
+0000b940: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000b950: 6e31 6d6d 2e73 656e 645f 636f 6e74 6163  n1mm.send_contac
+0000b960: 745f 696e 666f 2829 0a0a 2020 2020 2020  t_info()..      
+0000b970: 2020 7365 6c66 2e64 6174 6162 6173 652e    self.database.
+0000b980: 6c6f 675f 636f 6e74 6163 7428 7365 6c66  log_contact(self
+0000b990: 2e63 6f6e 7461 6374 290a 2020 2020 2020  .contact).      
+0000b9a0: 2020 7365 6c66 2e63 6c65 6172 696e 7075    self.clearinpu
+0000b9b0: 7473 2829 0a20 2020 2020 2020 2063 6d64  ts().        cmd
+0000b9c0: 203d 207b 7d0a 2020 2020 2020 2020 636d   = {}.        cm
+0000b9d0: 645b 2263 6d64 225d 203d 2022 5550 4441  d["cmd"] = "UPDA
+0000b9e0: 5445 4c4f 4722 0a20 2020 2020 2020 2063  TELOG".        c
+0000b9f0: 6d64 5b22 7374 6174 696f 6e22 5d20 3d20  md["station"] = 
+0000ba00: 706c 6174 666f 726d 2e6e 6f64 6528 290a  platform.node().
+0000ba10: 2020 2020 2020 2020 7365 6c66 2e6d 756c          self.mul
+0000ba20: 7469 6361 7374 5f69 6e74 6572 6661 6365  ticast_interface
+0000ba30: 2e73 656e 645f 6173 5f6a 736f 6e28 636d  .send_as_json(cm
+0000ba40: 6429 0a20 2020 2020 2020 2023 2073 656c  d).        # sel
+0000ba50: 662e 636f 6e74 6163 745b 2243 6f6e 7465  f.contact["Conte
+0000ba60: 7374 4e61 6d65 225d 203d 2073 656c 662e  stName"] = self.
+0000ba70: 636f 6e74 6573 742e 6e61 6d65 0a20 2020  contest.name.   
+0000ba80: 2020 2020 2023 2073 656c 662e 636f 6e74       # self.cont
+0000ba90: 6163 745b 2253 4e54 225d 203d 2073 656c  act["SNT"] = sel
+0000baa0: 662e 7365 6e74 2e74 6578 7428 290a 2020  f.sent.text().  
+0000bab0: 2020 2020 2020 2320 7365 6c66 2e63 6f6e        # self.con
+0000bac0: 7461 6374 5b22 5243 5622 5d20 3d20 7365  tact["RCV"] = se
+0000bad0: 6c66 2e72 6563 6569 7665 2e74 6578 7428  lf.receive.text(
+0000bae0: 290a 2020 2020 2020 2020 2320 7365 6c66  ).        # self
+0000baf0: 2e63 6f6e 7461 6374 5b22 436f 756e 7472  .contact["Countr
+0000bb00: 7950 7265 6669 7822 5d0a 2020 2020 2020  yPrefix"].      
+0000bb10: 2020 2320 7365 6c66 2e63 6f6e 7461 6374    # self.contact
+0000bb20: 5b22 5374 6174 696f 6e50 7265 6669 7822  ["StationPrefix"
+0000bb30: 5d20 3d20 7365 6c66 2e70 7265 662e 6765  ] = self.pref.ge
+0000bb40: 7428 2263 616c 6c73 6967 6e22 2c20 2222  t("callsign", ""
+0000bb50: 290a 2020 2020 2020 2020 2320 7365 6c66  ).        # self
+0000bb60: 2e63 6f6e 7461 6374 5b22 5154 4822 5d0a  .contact["QTH"].
+0000bb70: 2020 2020 2020 2020 2320 7365 6c66 2e63          # self.c
+0000bb80: 6f6e 7461 6374 5b22 4e61 6d65 225d 203d  ontact["Name"] =
+0000bb90: 2073 656c 662e 6f74 6865 725f 312e 7465   self.other_1.te
+0000bba0: 7874 2829 0a20 2020 2020 2020 2023 2073  xt().        # s
+0000bbb0: 656c 662e 636f 6e74 6163 745b 2243 6f6d  elf.contact["Com
+0000bbc0: 6d65 6e74 225d 203d 2073 656c 662e 6f74  ment"] = self.ot
+0000bbd0: 6865 725f 322e 7465 7874 2829 0a20 2020  her_2.text().   
+0000bbe0: 2020 2020 2023 2073 656c 662e 636f 6e74       # self.cont
+0000bbf0: 6163 745b 224e 5222 5d0a 2020 2020 2020  act["NR"].      
+0000bc00: 2020 2320 7365 6c66 2e63 6f6e 7461 6374    # self.contact
+0000bc10: 5b22 5365 6374 225d 0a20 2020 2020 2020  ["Sect"].       
+0000bc20: 2023 2073 656c 662e 636f 6e74 6163 745b   # self.contact[
+0000bc30: 2250 7265 6322 5d0a 2020 2020 2020 2020  "Prec"].        
+0000bc40: 2320 7365 6c66 2e63 6f6e 7461 6374 5b22  # self.contact["
+0000bc50: 434b 225d 0a20 2020 2020 2020 2023 2073  CK"].        # s
+0000bc60: 656c 662e 636f 6e74 6163 745b 225a 4e22  elf.contact["ZN"
+0000bc70: 5d0a 2020 2020 2020 2020 2320 7365 6c66  ].        # self
+0000bc80: 2e63 6f6e 7461 6374 5b22 5365 6e74 4e72  .contact["SentNr
 0000bc90: 225d 0a20 2020 2020 2020 2023 2073 656c  "].        # sel
-0000bca0: 662e 636f 6e74 6163 745b 2249 734d 756c  f.contact["IsMul
-0000bcb0: 7469 706c 6965 7232 225d 0a20 2020 2020  tiplier2"].     
-0000bcc0: 2020 2023 2073 656c 662e 636f 6e74 6163     # self.contac
-0000bcd0: 745b 2250 6f77 6572 225d 0a20 2020 2020  t["Power"].     
-0000bce0: 2020 2023 2073 656c 662e 636f 6e74 6163     # self.contac
-0000bcf0: 745b 2242 616e 6422 5d0a 2020 2020 2020  t["Band"].      
-0000bd00: 2020 2320 7365 6c66 2e63 6f6e 7461 6374    # self.contact
-0000bd10: 5b22 5750 5850 7265 6669 7822 5d20 3d20  ["WPXPrefix"] = 
-0000bd20: 6361 6c63 756c 6174 655f 7770 785f 7072  calculate_wpx_pr
-0000bd30: 6566 6978 2873 656c 662e 6361 6c6c 7369  efix(self.callsi
-0000bd40: 676e 2e74 6578 7428 2929 0a20 2020 2020  gn.text()).     
-0000bd50: 2020 2023 2073 656c 662e 636f 6e74 6163     # self.contac
-0000bd60: 745b 2245 7863 6861 6e67 6531 225d 0a20  t["Exchange1"]. 
-0000bd70: 2020 2020 2020 2023 2073 656c 662e 636f         # self.co
-0000bd80: 6e74 6163 745b 2252 6164 696f 4e52 225d  ntact["RadioNR"]
-0000bd90: 0a20 2020 2020 2020 2023 2073 656c 662e  .        # self.
-0000bda0: 636f 6e74 6163 745b 2269 734d 756c 7469  contact["isMulti
-0000bdb0: 706c 6965 7233 225d 0a20 2020 2020 2020  plier3"].       
-0000bdc0: 2023 2073 656c 662e 636f 6e74 6163 745b   # self.contact[
-0000bdd0: 224d 6973 6354 6578 7422 5d0a 2020 2020  "MiscText"].    
-0000bde0: 2020 2020 2320 7365 6c66 2e63 6f6e 7461      # self.conta
-0000bdf0: 6374 5b22 436f 6e74 6163 7454 7970 6522  ct["ContactType"
+0000bca0: 662e 636f 6e74 6163 745b 2250 6f69 6e74  f.contact["Point
+0000bcb0: 7322 5d0a 2020 2020 2020 2020 2320 7365  s"].        # se
+0000bcc0: 6c66 2e63 6f6e 7461 6374 5b22 4973 4d75  lf.contact["IsMu
+0000bcd0: 6c74 6970 6c69 6572 3122 5d0a 2020 2020  ltiplier1"].    
+0000bce0: 2020 2020 2320 7365 6c66 2e63 6f6e 7461      # self.conta
+0000bcf0: 6374 5b22 4973 4d75 6c74 6970 6c69 6572  ct["IsMultiplier
+0000bd00: 3222 5d0a 2020 2020 2020 2020 2320 7365  2"].        # se
+0000bd10: 6c66 2e63 6f6e 7461 6374 5b22 506f 7765  lf.contact["Powe
+0000bd20: 7222 5d0a 2020 2020 2020 2020 2320 7365  r"].        # se
+0000bd30: 6c66 2e63 6f6e 7461 6374 5b22 4261 6e64  lf.contact["Band
+0000bd40: 225d 0a20 2020 2020 2020 2023 2073 656c  "].        # sel
+0000bd50: 662e 636f 6e74 6163 745b 2257 5058 5072  f.contact["WPXPr
+0000bd60: 6566 6978 225d 203d 2063 616c 6375 6c61  efix"] = calcula
+0000bd70: 7465 5f77 7078 5f70 7265 6669 7828 7365  te_wpx_prefix(se
+0000bd80: 6c66 2e63 616c 6c73 6967 6e2e 7465 7874  lf.callsign.text
+0000bd90: 2829 290a 2020 2020 2020 2020 2320 7365  ()).        # se
+0000bda0: 6c66 2e63 6f6e 7461 6374 5b22 4578 6368  lf.contact["Exch
+0000bdb0: 616e 6765 3122 5d0a 2020 2020 2020 2020  ange1"].        
+0000bdc0: 2320 7365 6c66 2e63 6f6e 7461 6374 5b22  # self.contact["
+0000bdd0: 5261 6469 6f4e 5222 5d0a 2020 2020 2020  RadioNR"].      
+0000bde0: 2020 2320 7365 6c66 2e63 6f6e 7461 6374    # self.contact
+0000bdf0: 5b22 6973 4d75 6c74 6970 6c69 6572 3322  ["isMultiplier3"
 0000be00: 5d0a 2020 2020 2020 2020 2320 7365 6c66  ].        # self
-0000be10: 2e63 6f6e 7461 6374 5b22 5275 6e31 5275  .contact["Run1Ru
-0000be20: 6e32 225d 0a20 2020 2020 2020 2023 2073  n2"].        # s
-0000be30: 656c 662e 636f 6e74 6163 745b 2247 7269  elf.contact["Gri
-0000be40: 6453 7175 6172 6522 5d0a 2020 2020 2020  dSquare"].      
-0000be50: 2020 2320 7365 6c66 2e63 6f6e 7461 6374    # self.contact
-0000be60: 5b22 436f 6e74 696e 656e 7422 5d0a 2020  ["Continent"].  
+0000be10: 2e63 6f6e 7461 6374 5b22 4d69 7363 5465  .contact["MiscTe
+0000be20: 7874 225d 0a20 2020 2020 2020 2023 2073  xt"].        # s
+0000be30: 656c 662e 636f 6e74 6163 745b 2243 6f6e  elf.contact["Con
+0000be40: 7461 6374 5479 7065 225d 0a20 2020 2020  tactType"].     
+0000be50: 2020 2023 2073 656c 662e 636f 6e74 6163     # self.contac
+0000be60: 745b 2252 756e 3152 756e 3222 5d0a 2020  t["Run1Run2"].  
 0000be70: 2020 2020 2020 2320 7365 6c66 2e63 6f6e        # self.con
-0000be80: 7461 6374 5b22 526f 7665 724c 6f63 6174  tact["RoverLocat
-0000be90: 696f 6e22 5d0a 2020 2020 2020 2020 2320  ion"].        # 
-0000bea0: 7365 6c66 2e63 6f6e 7461 6374 5b22 5261  self.contact["Ra
-0000beb0: 6469 6f49 6e74 6572 6661 6365 6422 5d0a  dioInterfaced"].
-0000bec0: 2020 2020 2020 2020 2320 7365 6c66 2e63          # self.c
-0000bed0: 6f6e 7461 6374 5b22 4e65 7477 6f72 6b65  ontact["Networke
-0000bee0: 6443 6f6d 704e 7222 5d0a 2020 2020 2020  dCompNr"].      
-0000bef0: 2020 2320 7365 6c66 2e63 6f6e 7461 6374    # self.contact
-0000bf00: 5b22 434c 4149 4d45 4451 534f 225d 0a0a  ["CLAIMEDQSO"]..
-0000bf10: 2020 2020 6465 6620 6e65 775f 636f 6e74      def new_cont
-0000bf20: 6573 745f 6469 616c 6f67 2873 656c 6629  est_dialog(self)
-0000bf30: 3a0a 2020 2020 2020 2020 2222 2253 686f  :.        """Sho
-0000bf40: 7720 6e65 7720 636f 6e74 6573 7420 6469  w new contest di
-0000bf50: 616c 6f67 2222 220a 2020 2020 2020 2020  alog""".        
-0000bf60: 6c6f 6767 6572 2e64 6562 7567 2822 4e65  logger.debug("Ne
-0000bf70: 7720 636f 6e74 6573 7420 4469 616c 6f67  w contest Dialog
-0000bf80: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
-0000bf90: 636f 6e74 6573 745f 6469 616c 6f67 203d  contest_dialog =
-0000bfa0: 204e 6577 436f 6e74 6573 7428 574f 524b   NewContest(WORK
-0000bfb0: 494e 475f 5041 5448 290a 2020 2020 2020  ING_PATH).      
-0000bfc0: 2020 7365 6c66 2e63 6f6e 7465 7374 5f64    self.contest_d
-0000bfd0: 6961 6c6f 672e 6163 6365 7074 6564 2e63  ialog.accepted.c
-0000bfe0: 6f6e 6e65 6374 2873 656c 662e 7361 7665  onnect(self.save
-0000bff0: 5f63 6f6e 7465 7374 290a 2020 2020 2020  _contest).      
-0000c000: 2020 7365 6c66 2e63 6f6e 7465 7374 5f64    self.contest_d
-0000c010: 6961 6c6f 672e 6461 7465 5469 6d65 4564  ialog.dateTimeEd
-0000c020: 6974 2e73 6574 4461 7465 2851 7443 6f72  it.setDate(QtCor
-0000c030: 652e 5144 6174 652e 6375 7272 656e 7444  e.QDate.currentD
-0000c040: 6174 6528 2929 0a20 2020 2020 2020 2073  ate()).        s
-0000c050: 656c 662e 636f 6e74 6573 745f 6469 616c  elf.contest_dial
-0000c060: 6f67 2e64 6174 6554 696d 6545 6469 742e  og.dateTimeEdit.
-0000c070: 7365 7443 616c 656e 6461 7250 6f70 7570  setCalendarPopup
-0000c080: 2854 7275 6529 0a20 2020 2020 2020 2073  (True).        s
-0000c090: 656c 662e 636f 6e74 6573 745f 6469 616c  elf.contest_dial
-0000c0a0: 6f67 2e64 6174 6554 696d 6545 6469 742e  og.dateTimeEdit.
-0000c0b0: 7365 7454 696d 6528 5174 436f 7265 2e51  setTime(QtCore.Q
-0000c0c0: 5469 6d65 2830 2c20 3029 290a 2020 2020  Time(0, 0)).    
-0000c0d0: 2020 2020 7365 6c66 2e63 6f6e 7465 7374      self.contest
-0000c0e0: 5f64 6961 6c6f 672e 706f 7765 722e 7365  _dialog.power.se
-0000c0f0: 7443 7572 7265 6e74 5465 7874 2822 4c4f  tCurrentText("LO
-0000c100: 5722 290a 2020 2020 2020 2020 7365 6c66  W").        self
-0000c110: 2e63 6f6e 7465 7374 5f64 6961 6c6f 672e  .contest_dialog.
-0000c120: 7374 6174 696f 6e2e 7365 7443 7572 7265  station.setCurre
-0000c130: 6e74 5465 7874 2822 4649 5845 4422 290a  ntText("FIXED").
-0000c140: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
-0000c150: 7465 7374 5f64 6961 6c6f 672e 6f70 656e  test_dialog.open
-0000c160: 2829 0a0a 2020 2020 6465 6620 7361 7665  ()..    def save
-0000c170: 5f63 6f6e 7465 7374 2873 656c 6629 3a0a  _contest(self):.
-0000c180: 2020 2020 2020 2020 2222 2253 6176 6520          """Save 
-0000c190: 436f 6e74 6573 7422 2222 0a20 2020 2020  Contest""".     
-0000c1a0: 2020 206e 6578 745f 6e75 6d62 6572 203d     next_number =
-0000c1b0: 2073 656c 662e 6461 7461 6261 7365 2e67   self.database.g
-0000c1c0: 6574 5f6e 6578 745f 636f 6e74 6573 745f  et_next_contest_
-0000c1d0: 6e72 2829 0a20 2020 2020 2020 2063 6f6e  nr().        con
-0000c1e0: 7465 7374 203d 207b 7d0a 2020 2020 2020  test = {}.      
-0000c1f0: 2020 636f 6e74 6573 745b 2243 6f6e 7465    contest["Conte
-0000c200: 7374 4e61 6d65 225d 203d 2028 0a20 2020  stName"] = (.   
-0000c210: 2020 2020 2020 2020 2073 656c 662e 636f           self.co
-0000c220: 6e74 6573 745f 6469 616c 6f67 2e63 6f6e  ntest_dialog.con
-0000c230: 7465 7374 2e63 7572 7265 6e74 5465 7874  test.currentText
-0000c240: 2829 2e6c 6f77 6572 2829 2e72 6570 6c61  ().lower().repla
-0000c250: 6365 2822 2022 2c20 225f 2229 0a20 2020  ce(" ", "_").   
-0000c260: 2020 2020 2029 0a20 2020 2020 2020 2063       ).        c
-0000c270: 6f6e 7465 7374 5b22 5374 6172 7444 6174  ontest["StartDat
-0000c280: 6522 5d20 3d20 7365 6c66 2e63 6f6e 7465  e"] = self.conte
-0000c290: 7374 5f64 6961 6c6f 672e 6461 7465 5469  st_dialog.dateTi
-0000c2a0: 6d65 4564 6974 2e64 6174 6554 696d 6528  meEdit.dateTime(
-0000c2b0: 292e 746f 5374 7269 6e67 280a 2020 2020  ).toString(.    
-0000c2c0: 2020 2020 2020 2020 2279 7979 792d 4d4d          "yyyy-MM
-0000c2d0: 2d64 6420 6868 3a6d 6d3a 7373 220a 2020  -dd hh:mm:ss".  
-0000c2e0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-0000c2f0: 636f 6e74 6573 745b 224f 7065 7261 746f  contest["Operato
-0000c300: 7243 6174 6567 6f72 7922 5d20 3d20 7365  rCategory"] = se
-0000c310: 6c66 2e63 6f6e 7465 7374 5f64 6961 6c6f  lf.contest_dialo
-0000c320: 672e 6f70 6572 6174 6f72 5f63 6c61 7373  g.operator_class
-0000c330: 2e63 7572 7265 6e74 5465 7874 2829 0a20  .currentText(). 
-0000c340: 2020 2020 2020 2063 6f6e 7465 7374 5b22         contest["
-0000c350: 4261 6e64 4361 7465 676f 7279 225d 203d  BandCategory"] =
-0000c360: 2073 656c 662e 636f 6e74 6573 745f 6469   self.contest_di
-0000c370: 616c 6f67 2e62 616e 642e 6375 7272 656e  alog.band.curren
+0000be80: 7461 6374 5b22 4772 6964 5371 7561 7265  tact["GridSquare
+0000be90: 225d 0a20 2020 2020 2020 2023 2073 656c  "].        # sel
+0000bea0: 662e 636f 6e74 6163 745b 2243 6f6e 7469  f.contact["Conti
+0000beb0: 6e65 6e74 225d 0a20 2020 2020 2020 2023  nent"].        #
+0000bec0: 2073 656c 662e 636f 6e74 6163 745b 2252   self.contact["R
+0000bed0: 6f76 6572 4c6f 6361 7469 6f6e 225d 0a20  overLocation"]. 
+0000bee0: 2020 2020 2020 2023 2073 656c 662e 636f         # self.co
+0000bef0: 6e74 6163 745b 2252 6164 696f 496e 7465  ntact["RadioInte
+0000bf00: 7266 6163 6564 225d 0a20 2020 2020 2020  rfaced"].       
+0000bf10: 2023 2073 656c 662e 636f 6e74 6163 745b   # self.contact[
+0000bf20: 224e 6574 776f 726b 6564 436f 6d70 4e72  "NetworkedCompNr
+0000bf30: 225d 0a20 2020 2020 2020 2023 2073 656c  "].        # sel
+0000bf40: 662e 636f 6e74 6163 745b 2243 4c41 494d  f.contact["CLAIM
+0000bf50: 4544 5153 4f22 5d0a 0a20 2020 2064 6566  EDQSO"]..    def
+0000bf60: 206e 6577 5f63 6f6e 7465 7374 5f64 6961   new_contest_dia
+0000bf70: 6c6f 6728 7365 6c66 293a 0a20 2020 2020  log(self):.     
+0000bf80: 2020 2022 2222 5368 6f77 206e 6577 2063     """Show new c
+0000bf90: 6f6e 7465 7374 2064 6961 6c6f 6722 2222  ontest dialog"""
+0000bfa0: 0a20 2020 2020 2020 206c 6f67 6765 722e  .        logger.
+0000bfb0: 6465 6275 6728 224e 6577 2063 6f6e 7465  debug("New conte
+0000bfc0: 7374 2044 6961 6c6f 6722 290a 2020 2020  st Dialog").    
+0000bfd0: 2020 2020 7365 6c66 2e63 6f6e 7465 7374      self.contest
+0000bfe0: 5f64 6961 6c6f 6720 3d20 4e65 7743 6f6e  _dialog = NewCon
+0000bff0: 7465 7374 2857 4f52 4b49 4e47 5f50 4154  test(WORKING_PAT
+0000c000: 4829 0a20 2020 2020 2020 2073 656c 662e  H).        self.
+0000c010: 636f 6e74 6573 745f 6469 616c 6f67 2e61  contest_dialog.a
+0000c020: 6363 6570 7465 642e 636f 6e6e 6563 7428  ccepted.connect(
+0000c030: 7365 6c66 2e73 6176 655f 636f 6e74 6573  self.save_contes
+0000c040: 7429 0a20 2020 2020 2020 2073 656c 662e  t).        self.
+0000c050: 636f 6e74 6573 745f 6469 616c 6f67 2e64  contest_dialog.d
+0000c060: 6174 6554 696d 6545 6469 742e 7365 7444  ateTimeEdit.setD
+0000c070: 6174 6528 5174 436f 7265 2e51 4461 7465  ate(QtCore.QDate
+0000c080: 2e63 7572 7265 6e74 4461 7465 2829 290a  .currentDate()).
+0000c090: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
+0000c0a0: 7465 7374 5f64 6961 6c6f 672e 6461 7465  test_dialog.date
+0000c0b0: 5469 6d65 4564 6974 2e73 6574 4361 6c65  TimeEdit.setCale
+0000c0c0: 6e64 6172 506f 7075 7028 5472 7565 290a  ndarPopup(True).
+0000c0d0: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
+0000c0e0: 7465 7374 5f64 6961 6c6f 672e 6461 7465  test_dialog.date
+0000c0f0: 5469 6d65 4564 6974 2e73 6574 5469 6d65  TimeEdit.setTime
+0000c100: 2851 7443 6f72 652e 5154 696d 6528 302c  (QtCore.QTime(0,
+0000c110: 2030 2929 0a20 2020 2020 2020 2073 656c   0)).        sel
+0000c120: 662e 636f 6e74 6573 745f 6469 616c 6f67  f.contest_dialog
+0000c130: 2e70 6f77 6572 2e73 6574 4375 7272 656e  .power.setCurren
+0000c140: 7454 6578 7428 224c 4f57 2229 0a20 2020  tText("LOW").   
+0000c150: 2020 2020 2073 656c 662e 636f 6e74 6573       self.contes
+0000c160: 745f 6469 616c 6f67 2e73 7461 7469 6f6e  t_dialog.station
+0000c170: 2e73 6574 4375 7272 656e 7454 6578 7428  .setCurrentText(
+0000c180: 2246 4958 4544 2229 0a20 2020 2020 2020  "FIXED").       
+0000c190: 2073 656c 662e 636f 6e74 6573 745f 6469   self.contest_di
+0000c1a0: 616c 6f67 2e6f 7065 6e28 290a 0a20 2020  alog.open()..   
+0000c1b0: 2064 6566 2073 6176 655f 636f 6e74 6573   def save_contes
+0000c1c0: 7428 7365 6c66 293a 0a20 2020 2020 2020  t(self):.       
+0000c1d0: 2022 2222 5361 7665 2043 6f6e 7465 7374   """Save Contest
+0000c1e0: 2222 220a 2020 2020 2020 2020 6e65 7874  """.        next
+0000c1f0: 5f6e 756d 6265 7220 3d20 7365 6c66 2e64  _number = self.d
+0000c200: 6174 6162 6173 652e 6765 745f 6e65 7874  atabase.get_next
+0000c210: 5f63 6f6e 7465 7374 5f6e 7228 290a 2020  _contest_nr().  
+0000c220: 2020 2020 2020 636f 6e74 6573 7420 3d20        contest = 
+0000c230: 7b7d 0a20 2020 2020 2020 2063 6f6e 7465  {}.        conte
+0000c240: 7374 5b22 436f 6e74 6573 744e 616d 6522  st["ContestName"
+0000c250: 5d20 3d20 280a 2020 2020 2020 2020 2020  ] = (.          
+0000c260: 2020 7365 6c66 2e63 6f6e 7465 7374 5f64    self.contest_d
+0000c270: 6961 6c6f 672e 636f 6e74 6573 742e 6375  ialog.contest.cu
+0000c280: 7272 656e 7454 6578 7428 292e 6c6f 7765  rrentText().lowe
+0000c290: 7228 292e 7265 706c 6163 6528 2220 222c  r().replace(" ",
+0000c2a0: 2022 5f22 290a 2020 2020 2020 2020 290a   "_").        ).
+0000c2b0: 2020 2020 2020 2020 636f 6e74 6573 745b          contest[
+0000c2c0: 2253 7461 7274 4461 7465 225d 203d 2073  "StartDate"] = s
+0000c2d0: 656c 662e 636f 6e74 6573 745f 6469 616c  elf.contest_dial
+0000c2e0: 6f67 2e64 6174 6554 696d 6545 6469 742e  og.dateTimeEdit.
+0000c2f0: 6461 7465 5469 6d65 2829 2e74 6f53 7472  dateTime().toStr
+0000c300: 696e 6728 0a20 2020 2020 2020 2020 2020  ing(.           
+0000c310: 2022 7979 7979 2d4d 4d2d 6464 2068 683a   "yyyy-MM-dd hh:
+0000c320: 6d6d 3a73 7322 0a20 2020 2020 2020 2029  mm:ss".        )
+0000c330: 0a20 2020 2020 2020 2063 6f6e 7465 7374  .        contest
+0000c340: 5b22 4f70 6572 6174 6f72 4361 7465 676f  ["OperatorCatego
+0000c350: 7279 225d 203d 2073 656c 662e 636f 6e74  ry"] = self.cont
+0000c360: 6573 745f 6469 616c 6f67 2e6f 7065 7261  est_dialog.opera
+0000c370: 746f 725f 636c 6173 732e 6375 7272 656e  tor_class.curren
 0000c380: 7454 6578 7428 290a 2020 2020 2020 2020  tText().        
-0000c390: 636f 6e74 6573 745b 2250 6f77 6572 4361  contest["PowerCa
-0000c3a0: 7465 676f 7279 225d 203d 2073 656c 662e  tegory"] = self.
-0000c3b0: 636f 6e74 6573 745f 6469 616c 6f67 2e70  contest_dialog.p
-0000c3c0: 6f77 6572 2e63 7572 7265 6e74 5465 7874  ower.currentText
-0000c3d0: 2829 0a20 2020 2020 2020 2063 6f6e 7465  ().        conte
-0000c3e0: 7374 5b22 4d6f 6465 4361 7465 676f 7279  st["ModeCategory
-0000c3f0: 225d 203d 2073 656c 662e 636f 6e74 6573  "] = self.contes
-0000c400: 745f 6469 616c 6f67 2e6d 6f64 652e 6375  t_dialog.mode.cu
+0000c390: 636f 6e74 6573 745b 2242 616e 6443 6174  contest["BandCat
+0000c3a0: 6567 6f72 7922 5d20 3d20 7365 6c66 2e63  egory"] = self.c
+0000c3b0: 6f6e 7465 7374 5f64 6961 6c6f 672e 6261  ontest_dialog.ba
+0000c3c0: 6e64 2e63 7572 7265 6e74 5465 7874 2829  nd.currentText()
+0000c3d0: 0a20 2020 2020 2020 2063 6f6e 7465 7374  .        contest
+0000c3e0: 5b22 506f 7765 7243 6174 6567 6f72 7922  ["PowerCategory"
+0000c3f0: 5d20 3d20 7365 6c66 2e63 6f6e 7465 7374  ] = self.contest
+0000c400: 5f64 6961 6c6f 672e 706f 7765 722e 6375  _dialog.power.cu
 0000c410: 7272 656e 7454 6578 7428 290a 2020 2020  rrentText().    
-0000c420: 2020 2020 636f 6e74 6573 745b 224f 7665      contest["Ove
-0000c430: 726c 6179 4361 7465 676f 7279 225d 203d  rlayCategory"] =
-0000c440: 2073 656c 662e 636f 6e74 6573 745f 6469   self.contest_di
-0000c450: 616c 6f67 2e6f 7665 726c 6179 2e63 7572  alog.overlay.cur
-0000c460: 7265 6e74 5465 7874 2829 0a20 2020 2020  rentText().     
-0000c470: 2020 2023 2063 6f6e 7465 7374 5b27 436c     # contest['Cl
-0000c480: 6169 6d65 6453 636f 7265 275d 203d 2073  aimedScore'] = s
-0000c490: 656c 662e 636f 6e74 6573 745f 6469 616c  elf.contest_dial
-0000c4a0: 6f67 2e0a 2020 2020 2020 2020 636f 6e74  og..        cont
-0000c4b0: 6573 745b 224f 7065 7261 746f 7273 225d  est["Operators"]
-0000c4c0: 203d 2073 656c 662e 636f 6e74 6573 745f   = self.contest_
-0000c4d0: 6469 616c 6f67 2e6f 7065 7261 746f 7273  dialog.operators
-0000c4e0: 2e74 6578 7428 290a 2020 2020 2020 2020  .text().        
-0000c4f0: 636f 6e74 6573 745b 2253 6f61 7062 6f78  contest["Soapbox
-0000c500: 225d 203d 2073 656c 662e 636f 6e74 6573  "] = self.contes
-0000c510: 745f 6469 616c 6f67 2e73 6f61 7062 6f78  t_dialog.soapbox
-0000c520: 2e74 6f50 6c61 696e 5465 7874 2829 0a20  .toPlainText(). 
-0000c530: 2020 2020 2020 2063 6f6e 7465 7374 5b22         contest["
-0000c540: 5365 6e74 4578 6368 616e 6765 225d 203d  SentExchange"] =
-0000c550: 2073 656c 662e 636f 6e74 6573 745f 6469   self.contest_di
-0000c560: 616c 6f67 2e65 7863 6861 6e67 652e 7465  alog.exchange.te
-0000c570: 7874 2829 0a20 2020 2020 2020 2063 6f6e  xt().        con
-0000c580: 7465 7374 5b22 436f 6e74 6573 744e 5222  test["ContestNR"
-0000c590: 5d20 3d20 6e65 7874 5f6e 756d 6265 722e  ] = next_number.
-0000c5a0: 6765 7428 2263 6f75 6e74 222c 2031 290a  get("count", 1).
-0000c5b0: 2020 2020 2020 2020 7365 6c66 2e70 7265          self.pre
-0000c5c0: 665b 2263 6f6e 7465 7374 225d 203d 206e  f["contest"] = n
-0000c5d0: 6578 745f 6e75 6d62 6572 2e67 6574 2822  ext_number.get("
-0000c5e0: 636f 756e 7422 2c20 3129 0a20 2020 2020  count", 1).     
-0000c5f0: 2020 2023 2063 6f6e 7465 7374 5b27 5375     # contest['Su
-0000c600: 6254 7970 6527 5d20 3d20 7365 6c66 2e63  bType'] = self.c
-0000c610: 6f6e 7465 7374 5f64 6961 6c6f 672e 0a20  ontest_dialog.. 
-0000c620: 2020 2020 2020 2063 6f6e 7465 7374 5b22         contest["
-0000c630: 5374 6174 696f 6e43 6174 6567 6f72 7922  StationCategory"
-0000c640: 5d20 3d20 7365 6c66 2e63 6f6e 7465 7374  ] = self.contest
-0000c650: 5f64 6961 6c6f 672e 7374 6174 696f 6e2e  _dialog.station.
-0000c660: 6375 7272 656e 7454 6578 7428 290a 2020  currentText().  
-0000c670: 2020 2020 2020 636f 6e74 6573 745b 2241        contest["A
-0000c680: 7373 6973 7465 6443 6174 6567 6f72 7922  ssistedCategory"
-0000c690: 5d20 3d20 7365 6c66 2e63 6f6e 7465 7374  ] = self.contest
-0000c6a0: 5f64 6961 6c6f 672e 6173 7369 7374 6564  _dialog.assisted
-0000c6b0: 2e63 7572 7265 6e74 5465 7874 2829 0a20  .currentText(). 
-0000c6c0: 2020 2020 2020 2063 6f6e 7465 7374 5b22         contest["
-0000c6d0: 5472 616e 736d 6974 7465 7243 6174 6567  TransmitterCateg
-0000c6e0: 6f72 7922 5d20 3d20 7365 6c66 2e63 6f6e  ory"] = self.con
-0000c6f0: 7465 7374 5f64 6961 6c6f 672e 7472 616e  test_dialog.tran
-0000c700: 736d 6974 7465 722e 6375 7272 656e 7454  smitter.currentT
-0000c710: 6578 7428 290a 2020 2020 2020 2020 2320  ext().        # 
-0000c720: 636f 6e74 6573 745b 2754 696d 6543 6174  contest['TimeCat
-0000c730: 6567 6f72 7927 5d20 3d20 7365 6c66 2e63  egory'] = self.c
-0000c740: 6f6e 7465 7374 5f64 6961 6c6f 672e 0a20  ontest_dialog.. 
-0000c750: 2020 2020 2020 206c 6f67 6765 722e 6465         logger.de
-0000c760: 6275 6728 2225 7322 2c20 6622 7b63 6f6e  bug("%s", f"{con
-0000c770: 7465 7374 7d22 290a 2020 2020 2020 2020  test}").        
-0000c780: 7365 6c66 2e64 6174 6162 6173 652e 6164  self.database.ad
-0000c790: 645f 636f 6e74 6573 7428 636f 6e74 6573  d_contest(contes
-0000c7a0: 7429 0a20 2020 2020 2020 2073 656c 662e  t).        self.
-0000c7b0: 7772 6974 655f 7072 6566 6572 656e 6365  write_preference
-0000c7c0: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
-0000c7d0: 6c6f 6164 5f63 6f6e 7465 7374 2829 0a0a  load_contest()..
-0000c7e0: 2020 2020 6465 6620 6564 6974 5f73 7461      def edit_sta
-0000c7f0: 7469 6f6e 5f73 6574 7469 6e67 7328 7365  tion_settings(se
-0000c800: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
-0000c810: 5368 6f77 2073 6574 7469 6e67 7320 6469  Show settings di
-0000c820: 616c 6f67 2222 220a 2020 2020 2020 2020  alog""".        
-0000c830: 6c6f 6767 6572 2e64 6562 7567 2822 5374  logger.debug("St
-0000c840: 6174 696f 6e20 5365 7474 696e 6773 2073  ation Settings s
-0000c850: 656c 6563 7465 6422 290a 2020 2020 2020  elected").      
-0000c860: 2020 7365 6c66 2e73 6574 7469 6e67 735f    self.settings_
-0000c870: 6469 616c 6f67 203d 2045 6469 7453 7461  dialog = EditSta
-0000c880: 7469 6f6e 2857 4f52 4b49 4e47 5f50 4154  tion(WORKING_PAT
-0000c890: 4829 0a20 2020 2020 2020 2073 656c 662e  H).        self.
-0000c8a0: 7365 7474 696e 6773 5f64 6961 6c6f 672e  settings_dialog.
-0000c8b0: 6163 6365 7074 6564 2e63 6f6e 6e65 6374  accepted.connect
-0000c8c0: 2873 656c 662e 7361 7665 5f73 6574 7469  (self.save_setti
-0000c8d0: 6e67 7329 0a20 2020 2020 2020 2073 656c  ngs).        sel
-0000c8e0: 662e 7365 7474 696e 6773 5f64 6961 6c6f  f.settings_dialo
-0000c8f0: 672e 4361 6c6c 2e73 6574 5465 7874 2873  g.Call.setText(s
-0000c900: 656c 662e 7374 6174 696f 6e2e 6765 7428  elf.station.get(
-0000c910: 2243 616c 6c22 2c20 2222 2929 0a20 2020  "Call", "")).   
-0000c920: 2020 2020 2073 656c 662e 7365 7474 696e       self.settin
-0000c930: 6773 5f64 6961 6c6f 672e 4e61 6d65 2e73  gs_dialog.Name.s
-0000c940: 6574 5465 7874 2873 656c 662e 7374 6174  etText(self.stat
-0000c950: 696f 6e2e 6765 7428 224e 616d 6522 2c20  ion.get("Name", 
-0000c960: 2222 2929 0a20 2020 2020 2020 2073 656c  "")).        sel
-0000c970: 662e 7365 7474 696e 6773 5f64 6961 6c6f  f.settings_dialo
-0000c980: 672e 4164 6472 6573 7331 2e73 6574 5465  g.Address1.setTe
-0000c990: 7874 2873 656c 662e 7374 6174 696f 6e2e  xt(self.station.
-0000c9a0: 6765 7428 2253 7472 6565 7431 222c 2022  get("Street1", "
-0000c9b0: 2229 290a 2020 2020 2020 2020 7365 6c66  ")).        self
-0000c9c0: 2e73 6574 7469 6e67 735f 6469 616c 6f67  .settings_dialog
-0000c9d0: 2e41 6464 7265 7373 322e 7365 7454 6578  .Address2.setTex
-0000c9e0: 7428 7365 6c66 2e73 7461 7469 6f6e 2e67  t(self.station.g
-0000c9f0: 6574 2822 5374 7265 6574 3222 2c20 2222  et("Street2", ""
-0000ca00: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
-0000ca10: 7365 7474 696e 6773 5f64 6961 6c6f 672e  settings_dialog.
-0000ca20: 4369 7479 2e73 6574 5465 7874 2873 656c  City.setText(sel
-0000ca30: 662e 7374 6174 696f 6e2e 6765 7428 2243  f.station.get("C
-0000ca40: 6974 7922 2c20 2222 2929 0a20 2020 2020  ity", "")).     
-0000ca50: 2020 2073 656c 662e 7365 7474 696e 6773     self.settings
-0000ca60: 5f64 6961 6c6f 672e 5374 6174 652e 7365  _dialog.State.se
+0000c420: 2020 2020 636f 6e74 6573 745b 224d 6f64      contest["Mod
+0000c430: 6543 6174 6567 6f72 7922 5d20 3d20 7365  eCategory"] = se
+0000c440: 6c66 2e63 6f6e 7465 7374 5f64 6961 6c6f  lf.contest_dialo
+0000c450: 672e 6d6f 6465 2e63 7572 7265 6e74 5465  g.mode.currentTe
+0000c460: 7874 2829 0a20 2020 2020 2020 2063 6f6e  xt().        con
+0000c470: 7465 7374 5b22 4f76 6572 6c61 7943 6174  test["OverlayCat
+0000c480: 6567 6f72 7922 5d20 3d20 7365 6c66 2e63  egory"] = self.c
+0000c490: 6f6e 7465 7374 5f64 6961 6c6f 672e 6f76  ontest_dialog.ov
+0000c4a0: 6572 6c61 792e 6375 7272 656e 7454 6578  erlay.currentTex
+0000c4b0: 7428 290a 2020 2020 2020 2020 2320 636f  t().        # co
+0000c4c0: 6e74 6573 745b 2743 6c61 696d 6564 5363  ntest['ClaimedSc
+0000c4d0: 6f72 6527 5d20 3d20 7365 6c66 2e63 6f6e  ore'] = self.con
+0000c4e0: 7465 7374 5f64 6961 6c6f 672e 0a20 2020  test_dialog..   
+0000c4f0: 2020 2020 2063 6f6e 7465 7374 5b22 4f70       contest["Op
+0000c500: 6572 6174 6f72 7322 5d20 3d20 7365 6c66  erators"] = self
+0000c510: 2e63 6f6e 7465 7374 5f64 6961 6c6f 672e  .contest_dialog.
+0000c520: 6f70 6572 6174 6f72 732e 7465 7874 2829  operators.text()
+0000c530: 0a20 2020 2020 2020 2063 6f6e 7465 7374  .        contest
+0000c540: 5b22 536f 6170 626f 7822 5d20 3d20 7365  ["Soapbox"] = se
+0000c550: 6c66 2e63 6f6e 7465 7374 5f64 6961 6c6f  lf.contest_dialo
+0000c560: 672e 736f 6170 626f 782e 746f 506c 6169  g.soapbox.toPlai
+0000c570: 6e54 6578 7428 290a 2020 2020 2020 2020  nText().        
+0000c580: 636f 6e74 6573 745b 2253 656e 7445 7863  contest["SentExc
+0000c590: 6861 6e67 6522 5d20 3d20 7365 6c66 2e63  hange"] = self.c
+0000c5a0: 6f6e 7465 7374 5f64 6961 6c6f 672e 6578  ontest_dialog.ex
+0000c5b0: 6368 616e 6765 2e74 6578 7428 290a 2020  change.text().  
+0000c5c0: 2020 2020 2020 636f 6e74 6573 745b 2243        contest["C
+0000c5d0: 6f6e 7465 7374 4e52 225d 203d 206e 6578  ontestNR"] = nex
+0000c5e0: 745f 6e75 6d62 6572 2e67 6574 2822 636f  t_number.get("co
+0000c5f0: 756e 7422 2c20 3129 0a20 2020 2020 2020  unt", 1).       
+0000c600: 2073 656c 662e 7072 6566 5b22 636f 6e74   self.pref["cont
+0000c610: 6573 7422 5d20 3d20 6e65 7874 5f6e 756d  est"] = next_num
+0000c620: 6265 722e 6765 7428 2263 6f75 6e74 222c  ber.get("count",
+0000c630: 2031 290a 2020 2020 2020 2020 2320 636f   1).        # co
+0000c640: 6e74 6573 745b 2753 7562 5479 7065 275d  ntest['SubType']
+0000c650: 203d 2073 656c 662e 636f 6e74 6573 745f   = self.contest_
+0000c660: 6469 616c 6f67 2e0a 2020 2020 2020 2020  dialog..        
+0000c670: 636f 6e74 6573 745b 2253 7461 7469 6f6e  contest["Station
+0000c680: 4361 7465 676f 7279 225d 203d 2073 656c  Category"] = sel
+0000c690: 662e 636f 6e74 6573 745f 6469 616c 6f67  f.contest_dialog
+0000c6a0: 2e73 7461 7469 6f6e 2e63 7572 7265 6e74  .station.current
+0000c6b0: 5465 7874 2829 0a20 2020 2020 2020 2063  Text().        c
+0000c6c0: 6f6e 7465 7374 5b22 4173 7369 7374 6564  ontest["Assisted
+0000c6d0: 4361 7465 676f 7279 225d 203d 2073 656c  Category"] = sel
+0000c6e0: 662e 636f 6e74 6573 745f 6469 616c 6f67  f.contest_dialog
+0000c6f0: 2e61 7373 6973 7465 642e 6375 7272 656e  .assisted.curren
+0000c700: 7454 6578 7428 290a 2020 2020 2020 2020  tText().        
+0000c710: 636f 6e74 6573 745b 2254 7261 6e73 6d69  contest["Transmi
+0000c720: 7474 6572 4361 7465 676f 7279 225d 203d  tterCategory"] =
+0000c730: 2073 656c 662e 636f 6e74 6573 745f 6469   self.contest_di
+0000c740: 616c 6f67 2e74 7261 6e73 6d69 7474 6572  alog.transmitter
+0000c750: 2e63 7572 7265 6e74 5465 7874 2829 0a20  .currentText(). 
+0000c760: 2020 2020 2020 2023 2063 6f6e 7465 7374         # contest
+0000c770: 5b27 5469 6d65 4361 7465 676f 7279 275d  ['TimeCategory']
+0000c780: 203d 2073 656c 662e 636f 6e74 6573 745f   = self.contest_
+0000c790: 6469 616c 6f67 2e0a 2020 2020 2020 2020  dialog..        
+0000c7a0: 6c6f 6767 6572 2e64 6562 7567 2822 2573  logger.debug("%s
+0000c7b0: 222c 2066 227b 636f 6e74 6573 747d 2229  ", f"{contest}")
+0000c7c0: 0a20 2020 2020 2020 2073 656c 662e 6461  .        self.da
+0000c7d0: 7461 6261 7365 2e61 6464 5f63 6f6e 7465  tabase.add_conte
+0000c7e0: 7374 2863 6f6e 7465 7374 290a 2020 2020  st(contest).    
+0000c7f0: 2020 2020 7365 6c66 2e77 7269 7465 5f70      self.write_p
+0000c800: 7265 6665 7265 6e63 6528 290a 2020 2020  reference().    
+0000c810: 2020 2020 7365 6c66 2e6c 6f61 645f 636f      self.load_co
+0000c820: 6e74 6573 7428 290a 0a20 2020 2064 6566  ntest()..    def
+0000c830: 2065 6469 745f 7374 6174 696f 6e5f 7365   edit_station_se
+0000c840: 7474 696e 6773 2873 656c 6629 3a0a 2020  ttings(self):.  
+0000c850: 2020 2020 2020 2222 2253 686f 7720 7365        """Show se
+0000c860: 7474 696e 6773 2064 6961 6c6f 6722 2222  ttings dialog"""
+0000c870: 0a20 2020 2020 2020 206c 6f67 6765 722e  .        logger.
+0000c880: 6465 6275 6728 2253 7461 7469 6f6e 2053  debug("Station S
+0000c890: 6574 7469 6e67 7320 7365 6c65 6374 6564  ettings selected
+0000c8a0: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
+0000c8b0: 7365 7474 696e 6773 5f64 6961 6c6f 6720  settings_dialog 
+0000c8c0: 3d20 4564 6974 5374 6174 696f 6e28 574f  = EditStation(WO
+0000c8d0: 524b 494e 475f 5041 5448 290a 2020 2020  RKING_PATH).    
+0000c8e0: 2020 2020 7365 6c66 2e73 6574 7469 6e67      self.setting
+0000c8f0: 735f 6469 616c 6f67 2e61 6363 6570 7465  s_dialog.accepte
+0000c900: 642e 636f 6e6e 6563 7428 7365 6c66 2e73  d.connect(self.s
+0000c910: 6176 655f 7365 7474 696e 6773 290a 2020  ave_settings).  
+0000c920: 2020 2020 2020 7365 6c66 2e73 6574 7469        self.setti
+0000c930: 6e67 735f 6469 616c 6f67 2e43 616c 6c2e  ngs_dialog.Call.
+0000c940: 7365 7454 6578 7428 7365 6c66 2e73 7461  setText(self.sta
+0000c950: 7469 6f6e 2e67 6574 2822 4361 6c6c 222c  tion.get("Call",
+0000c960: 2022 2229 290a 2020 2020 2020 2020 7365   "")).        se
+0000c970: 6c66 2e73 6574 7469 6e67 735f 6469 616c  lf.settings_dial
+0000c980: 6f67 2e4e 616d 652e 7365 7454 6578 7428  og.Name.setText(
+0000c990: 7365 6c66 2e73 7461 7469 6f6e 2e67 6574  self.station.get
+0000c9a0: 2822 4e61 6d65 222c 2022 2229 290a 2020  ("Name", "")).  
+0000c9b0: 2020 2020 2020 7365 6c66 2e73 6574 7469        self.setti
+0000c9c0: 6e67 735f 6469 616c 6f67 2e41 6464 7265  ngs_dialog.Addre
+0000c9d0: 7373 312e 7365 7454 6578 7428 7365 6c66  ss1.setText(self
+0000c9e0: 2e73 7461 7469 6f6e 2e67 6574 2822 5374  .station.get("St
+0000c9f0: 7265 6574 3122 2c20 2222 2929 0a20 2020  reet1", "")).   
+0000ca00: 2020 2020 2073 656c 662e 7365 7474 696e       self.settin
+0000ca10: 6773 5f64 6961 6c6f 672e 4164 6472 6573  gs_dialog.Addres
+0000ca20: 7332 2e73 6574 5465 7874 2873 656c 662e  s2.setText(self.
+0000ca30: 7374 6174 696f 6e2e 6765 7428 2253 7472  station.get("Str
+0000ca40: 6565 7432 222c 2022 2229 290a 2020 2020  eet2", "")).    
+0000ca50: 2020 2020 7365 6c66 2e73 6574 7469 6e67      self.setting
+0000ca60: 735f 6469 616c 6f67 2e43 6974 792e 7365  s_dialog.City.se
 0000ca70: 7454 6578 7428 7365 6c66 2e73 7461 7469  tText(self.stati
-0000ca80: 6f6e 2e67 6574 2822 5374 6174 6522 2c20  on.get("State", 
-0000ca90: 2222 2929 0a20 2020 2020 2020 2073 656c  "")).        sel
-0000caa0: 662e 7365 7474 696e 6773 5f64 6961 6c6f  f.settings_dialo
-0000cab0: 672e 5a69 702e 7365 7454 6578 7428 7365  g.Zip.setText(se
-0000cac0: 6c66 2e73 7461 7469 6f6e 2e67 6574 2822  lf.station.get("
-0000cad0: 5a69 7022 2c20 2222 2929 0a20 2020 2020  Zip", "")).     
-0000cae0: 2020 2073 656c 662e 7365 7474 696e 6773     self.settings
-0000caf0: 5f64 6961 6c6f 672e 436f 756e 7472 792e  _dialog.Country.
-0000cb00: 7365 7454 6578 7428 7365 6c66 2e73 7461  setText(self.sta
-0000cb10: 7469 6f6e 2e67 6574 2822 436f 756e 7472  tion.get("Countr
-0000cb20: 7922 2c20 2222 2929 0a20 2020 2020 2020  y", "")).       
-0000cb30: 2073 656c 662e 7365 7474 696e 6773 5f64   self.settings_d
-0000cb40: 6961 6c6f 672e 4772 6964 5371 7561 7265  ialog.GridSquare
-0000cb50: 2e73 6574 5465 7874 2873 656c 662e 7374  .setText(self.st
-0000cb60: 6174 696f 6e2e 6765 7428 2247 7269 6453  ation.get("GridS
-0000cb70: 7175 6172 6522 2c20 2222 2929 0a20 2020  quare", "")).   
-0000cb80: 2020 2020 2073 656c 662e 7365 7474 696e       self.settin
-0000cb90: 6773 5f64 6961 6c6f 672e 4351 5a6f 6e65  gs_dialog.CQZone
-0000cba0: 2e73 6574 5465 7874 2873 7472 2873 656c  .setText(str(sel
-0000cbb0: 662e 7374 6174 696f 6e2e 6765 7428 2243  f.station.get("C
-0000cbc0: 515a 6f6e 6522 2c20 2222 2929 290a 2020  QZone", ""))).  
-0000cbd0: 2020 2020 2020 7365 6c66 2e73 6574 7469        self.setti
-0000cbe0: 6e67 735f 6469 616c 6f67 2e49 5455 5a6f  ngs_dialog.ITUZo
-0000cbf0: 6e65 2e73 6574 5465 7874 2873 7472 2873  ne.setText(str(s
-0000cc00: 656c 662e 7374 6174 696f 6e2e 6765 7428  elf.station.get(
-0000cc10: 2249 4152 555a 6f6e 6522 2c20 2222 2929  "IARUZone", ""))
-0000cc20: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
-0000cc30: 6574 7469 6e67 735f 6469 616c 6f67 2e4c  ettings_dialog.L
-0000cc40: 6963 656e 7365 2e73 6574 5465 7874 2873  icense.setText(s
-0000cc50: 656c 662e 7374 6174 696f 6e2e 6765 7428  elf.station.get(
-0000cc60: 224c 6963 656e 7365 436c 6173 7322 2c20  "LicenseClass", 
-0000cc70: 2222 2929 0a20 2020 2020 2020 2073 656c  "")).        sel
-0000cc80: 662e 7365 7474 696e 6773 5f64 6961 6c6f  f.settings_dialo
-0000cc90: 672e 4c61 7469 7475 6465 2e73 6574 5465  g.Latitude.setTe
-0000cca0: 7874 2873 7472 2873 656c 662e 7374 6174  xt(str(self.stat
-0000ccb0: 696f 6e2e 6765 7428 224c 6174 6974 7564  ion.get("Latitud
-0000ccc0: 6522 2c20 2222 2929 290a 2020 2020 2020  e", ""))).      
-0000ccd0: 2020 7365 6c66 2e73 6574 7469 6e67 735f    self.settings_
-0000cce0: 6469 616c 6f67 2e4c 6f6e 6769 7475 6465  dialog.Longitude
-0000ccf0: 2e73 6574 5465 7874 2873 7472 2873 656c  .setText(str(sel
-0000cd00: 662e 7374 6174 696f 6e2e 6765 7428 224c  f.station.get("L
-0000cd10: 6f6e 6769 7475 6465 222c 2022 2229 2929  ongitude", "")))
-0000cd20: 0a20 2020 2020 2020 2073 656c 662e 7365  .        self.se
-0000cd30: 7474 696e 6773 5f64 6961 6c6f 672e 5374  ttings_dialog.St
-0000cd40: 6174 696f 6e54 5852 582e 7365 7454 6578  ationTXRX.setTex
-0000cd50: 7428 7365 6c66 2e73 7461 7469 6f6e 2e67  t(self.station.g
-0000cd60: 6574 2822 7374 6174 696f 6e74 7872 7822  et("stationtxrx"
-0000cd70: 2c20 2222 2929 0a20 2020 2020 2020 2073  , "")).        s
-0000cd80: 656c 662e 7365 7474 696e 6773 5f64 6961  elf.settings_dia
-0000cd90: 6c6f 672e 506f 7765 722e 7365 7454 6578  log.Power.setTex
-0000cda0: 7428 7365 6c66 2e73 7461 7469 6f6e 2e67  t(self.station.g
-0000cdb0: 6574 2822 5350 6f77 6522 2c20 2222 2929  et("SPowe", ""))
-0000cdc0: 0a20 2020 2020 2020 2073 656c 662e 7365  .        self.se
-0000cdd0: 7474 696e 6773 5f64 6961 6c6f 672e 416e  ttings_dialog.An
-0000cde0: 7465 6e6e 612e 7365 7454 6578 7428 7365  tenna.setText(se
-0000cdf0: 6c66 2e73 7461 7469 6f6e 2e67 6574 2822  lf.station.get("
-0000ce00: 5341 6e74 6522 2c20 2222 2929 0a20 2020  SAnte", "")).   
-0000ce10: 2020 2020 2073 656c 662e 7365 7474 696e       self.settin
-0000ce20: 6773 5f64 6961 6c6f 672e 416e 7448 6569  gs_dialog.AntHei
-0000ce30: 6768 742e 7365 7454 6578 7428 7365 6c66  ght.setText(self
-0000ce40: 2e73 7461 7469 6f6e 2e67 6574 2822 5341  .station.get("SA
-0000ce50: 6e74 4831 222c 2022 2229 290a 2020 2020  ntH1", "")).    
-0000ce60: 2020 2020 7365 6c66 2e73 6574 7469 6e67      self.setting
-0000ce70: 735f 6469 616c 6f67 2e41 534c 2e73 6574  s_dialog.ASL.set
+0000ca80: 6f6e 2e67 6574 2822 4369 7479 222c 2022  on.get("City", "
+0000ca90: 2229 290a 2020 2020 2020 2020 7365 6c66  ")).        self
+0000caa0: 2e73 6574 7469 6e67 735f 6469 616c 6f67  .settings_dialog
+0000cab0: 2e53 7461 7465 2e73 6574 5465 7874 2873  .State.setText(s
+0000cac0: 656c 662e 7374 6174 696f 6e2e 6765 7428  elf.station.get(
+0000cad0: 2253 7461 7465 222c 2022 2229 290a 2020  "State", "")).  
+0000cae0: 2020 2020 2020 7365 6c66 2e73 6574 7469        self.setti
+0000caf0: 6e67 735f 6469 616c 6f67 2e5a 6970 2e73  ngs_dialog.Zip.s
+0000cb00: 6574 5465 7874 2873 656c 662e 7374 6174  etText(self.stat
+0000cb10: 696f 6e2e 6765 7428 225a 6970 222c 2022  ion.get("Zip", "
+0000cb20: 2229 290a 2020 2020 2020 2020 7365 6c66  ")).        self
+0000cb30: 2e73 6574 7469 6e67 735f 6469 616c 6f67  .settings_dialog
+0000cb40: 2e43 6f75 6e74 7279 2e73 6574 5465 7874  .Country.setText
+0000cb50: 2873 656c 662e 7374 6174 696f 6e2e 6765  (self.station.ge
+0000cb60: 7428 2243 6f75 6e74 7279 222c 2022 2229  t("Country", "")
+0000cb70: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
+0000cb80: 6574 7469 6e67 735f 6469 616c 6f67 2e47  ettings_dialog.G
+0000cb90: 7269 6453 7175 6172 652e 7365 7454 6578  ridSquare.setTex
+0000cba0: 7428 7365 6c66 2e73 7461 7469 6f6e 2e67  t(self.station.g
+0000cbb0: 6574 2822 4772 6964 5371 7561 7265 222c  et("GridSquare",
+0000cbc0: 2022 2229 290a 2020 2020 2020 2020 7365   "")).        se
+0000cbd0: 6c66 2e73 6574 7469 6e67 735f 6469 616c  lf.settings_dial
+0000cbe0: 6f67 2e43 515a 6f6e 652e 7365 7454 6578  og.CQZone.setTex
+0000cbf0: 7428 7374 7228 7365 6c66 2e73 7461 7469  t(str(self.stati
+0000cc00: 6f6e 2e67 6574 2822 4351 5a6f 6e65 222c  on.get("CQZone",
+0000cc10: 2022 2229 2929 0a20 2020 2020 2020 2073   ""))).        s
+0000cc20: 656c 662e 7365 7474 696e 6773 5f64 6961  elf.settings_dia
+0000cc30: 6c6f 672e 4954 555a 6f6e 652e 7365 7454  log.ITUZone.setT
+0000cc40: 6578 7428 7374 7228 7365 6c66 2e73 7461  ext(str(self.sta
+0000cc50: 7469 6f6e 2e67 6574 2822 4941 5255 5a6f  tion.get("IARUZo
+0000cc60: 6e65 222c 2022 2229 2929 0a20 2020 2020  ne", ""))).     
+0000cc70: 2020 2073 656c 662e 7365 7474 696e 6773     self.settings
+0000cc80: 5f64 6961 6c6f 672e 4c69 6365 6e73 652e  _dialog.License.
+0000cc90: 7365 7454 6578 7428 7365 6c66 2e73 7461  setText(self.sta
+0000cca0: 7469 6f6e 2e67 6574 2822 4c69 6365 6e73  tion.get("Licens
+0000ccb0: 6543 6c61 7373 222c 2022 2229 290a 2020  eClass", "")).  
+0000ccc0: 2020 2020 2020 7365 6c66 2e73 6574 7469        self.setti
+0000ccd0: 6e67 735f 6469 616c 6f67 2e4c 6174 6974  ngs_dialog.Latit
+0000cce0: 7564 652e 7365 7454 6578 7428 7374 7228  ude.setText(str(
+0000ccf0: 7365 6c66 2e73 7461 7469 6f6e 2e67 6574  self.station.get
+0000cd00: 2822 4c61 7469 7475 6465 222c 2022 2229  ("Latitude", "")
+0000cd10: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
+0000cd20: 7365 7474 696e 6773 5f64 6961 6c6f 672e  settings_dialog.
+0000cd30: 4c6f 6e67 6974 7564 652e 7365 7454 6578  Longitude.setTex
+0000cd40: 7428 7374 7228 7365 6c66 2e73 7461 7469  t(str(self.stati
+0000cd50: 6f6e 2e67 6574 2822 4c6f 6e67 6974 7564  on.get("Longitud
+0000cd60: 6522 2c20 2222 2929 290a 2020 2020 2020  e", ""))).      
+0000cd70: 2020 7365 6c66 2e73 6574 7469 6e67 735f    self.settings_
+0000cd80: 6469 616c 6f67 2e53 7461 7469 6f6e 5458  dialog.StationTX
+0000cd90: 5258 2e73 6574 5465 7874 2873 656c 662e  RX.setText(self.
+0000cda0: 7374 6174 696f 6e2e 6765 7428 2273 7461  station.get("sta
+0000cdb0: 7469 6f6e 7478 7278 222c 2022 2229 290a  tiontxrx", "")).
+0000cdc0: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
+0000cdd0: 7469 6e67 735f 6469 616c 6f67 2e50 6f77  tings_dialog.Pow
+0000cde0: 6572 2e73 6574 5465 7874 2873 656c 662e  er.setText(self.
+0000cdf0: 7374 6174 696f 6e2e 6765 7428 2253 506f  station.get("SPo
+0000ce00: 7765 222c 2022 2229 290a 2020 2020 2020  we", "")).      
+0000ce10: 2020 7365 6c66 2e73 6574 7469 6e67 735f    self.settings_
+0000ce20: 6469 616c 6f67 2e41 6e74 656e 6e61 2e73  dialog.Antenna.s
+0000ce30: 6574 5465 7874 2873 656c 662e 7374 6174  etText(self.stat
+0000ce40: 696f 6e2e 6765 7428 2253 416e 7465 222c  ion.get("SAnte",
+0000ce50: 2022 2229 290a 2020 2020 2020 2020 7365   "")).        se
+0000ce60: 6c66 2e73 6574 7469 6e67 735f 6469 616c  lf.settings_dial
+0000ce70: 6f67 2e41 6e74 4865 6967 6874 2e73 6574  og.AntHeight.set
 0000ce80: 5465 7874 2873 656c 662e 7374 6174 696f  Text(self.statio
-0000ce90: 6e2e 6765 7428 2253 416e 7448 3222 2c20  n.get("SAntH2", 
+0000ce90: 6e2e 6765 7428 2253 416e 7448 3122 2c20  n.get("SAntH1", 
 0000cea0: 2222 2929 0a20 2020 2020 2020 2073 656c  "")).        sel
 0000ceb0: 662e 7365 7474 696e 6773 5f64 6961 6c6f  f.settings_dialo
-0000cec0: 672e 4152 524c 5365 6374 696f 6e2e 7365  g.ARRLSection.se
-0000ced0: 7454 6578 7428 7365 6c66 2e73 7461 7469  tText(self.stati
-0000cee0: 6f6e 2e67 6574 2822 4152 524c 5365 6374  on.get("ARRLSect
-0000cef0: 696f 6e22 2c20 2222 2929 0a20 2020 2020  ion", "")).     
-0000cf00: 2020 2073 656c 662e 7365 7474 696e 6773     self.settings
-0000cf10: 5f64 6961 6c6f 672e 526f 7665 7251 5448  _dialog.RoverQTH
-0000cf20: 2e73 6574 5465 7874 2873 656c 662e 7374  .setText(self.st
-0000cf30: 6174 696f 6e2e 6765 7428 2252 6f76 6572  ation.get("Rover
-0000cf40: 5154 4822 2c20 2222 2929 0a20 2020 2020  QTH", "")).     
-0000cf50: 2020 2073 656c 662e 7365 7474 696e 6773     self.settings
-0000cf60: 5f64 6961 6c6f 672e 436c 7562 2e73 6574  _dialog.Club.set
-0000cf70: 5465 7874 2873 656c 662e 7374 6174 696f  Text(self.statio
-0000cf80: 6e2e 6765 7428 2243 6c75 6222 2c20 2222  n.get("Club", ""
-0000cf90: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
-0000cfa0: 7365 7474 696e 6773 5f64 6961 6c6f 672e  settings_dialog.
-0000cfb0: 456d 6169 6c2e 7365 7454 6578 7428 7365  Email.setText(se
+0000cec0: 672e 4153 4c2e 7365 7454 6578 7428 7365  g.ASL.setText(se
+0000ced0: 6c66 2e73 7461 7469 6f6e 2e67 6574 2822  lf.station.get("
+0000cee0: 5341 6e74 4832 222c 2022 2229 290a 2020  SAntH2", "")).  
+0000cef0: 2020 2020 2020 7365 6c66 2e73 6574 7469        self.setti
+0000cf00: 6e67 735f 6469 616c 6f67 2e41 5252 4c53  ngs_dialog.ARRLS
+0000cf10: 6563 7469 6f6e 2e73 6574 5465 7874 2873  ection.setText(s
+0000cf20: 656c 662e 7374 6174 696f 6e2e 6765 7428  elf.station.get(
+0000cf30: 2241 5252 4c53 6563 7469 6f6e 222c 2022  "ARRLSection", "
+0000cf40: 2229 290a 2020 2020 2020 2020 7365 6c66  ")).        self
+0000cf50: 2e73 6574 7469 6e67 735f 6469 616c 6f67  .settings_dialog
+0000cf60: 2e52 6f76 6572 5154 482e 7365 7454 6578  .RoverQTH.setTex
+0000cf70: 7428 7365 6c66 2e73 7461 7469 6f6e 2e67  t(self.station.g
+0000cf80: 6574 2822 526f 7665 7251 5448 222c 2022  et("RoverQTH", "
+0000cf90: 2229 290a 2020 2020 2020 2020 7365 6c66  ")).        self
+0000cfa0: 2e73 6574 7469 6e67 735f 6469 616c 6f67  .settings_dialog
+0000cfb0: 2e43 6c75 622e 7365 7454 6578 7428 7365  .Club.setText(se
 0000cfc0: 6c66 2e73 7461 7469 6f6e 2e67 6574 2822  lf.station.get("
-0000cfd0: 456d 6169 6c22 2c20 2222 2929 0a20 2020  Email", "")).   
-0000cfe0: 2020 2020 2073 656c 662e 7365 7474 696e       self.settin
-0000cff0: 6773 5f64 6961 6c6f 672e 6f70 656e 2829  gs_dialog.open()
-0000d000: 0a0a 2020 2020 6465 6620 7361 7665 5f73  ..    def save_s
-0000d010: 6574 7469 6e67 7328 7365 6c66 293a 0a20  ettings(self):. 
-0000d020: 2020 2020 2020 2022 2222 5361 7665 2073         """Save s
-0000d030: 6574 7469 6e67 7322 2222 0a20 2020 2020  ettings""".     
-0000d040: 2020 2063 7320 3d20 7365 6c66 2e73 6574     cs = self.set
-0000d050: 7469 6e67 735f 6469 616c 6f67 2e43 616c  tings_dialog.Cal
-0000d060: 6c2e 7465 7874 2829 0a20 2020 2020 2020  l.text().       
-0000d070: 2073 656c 662e 7374 6174 696f 6e20 3d20   self.station = 
-0000d080: 7b7d 0a20 2020 2020 2020 2073 656c 662e  {}.        self.
-0000d090: 7374 6174 696f 6e5b 2243 616c 6c22 5d20  station["Call"] 
-0000d0a0: 3d20 6373 2e75 7070 6572 2829 0a20 2020  = cs.upper().   
-0000d0b0: 2020 2020 2073 656c 662e 7374 6174 696f       self.statio
-0000d0c0: 6e5b 224e 616d 6522 5d20 3d20 7365 6c66  n["Name"] = self
-0000d0d0: 2e73 6574 7469 6e67 735f 6469 616c 6f67  .settings_dialog
-0000d0e0: 2e4e 616d 652e 7465 7874 2829 2e74 6974  .Name.text().tit
-0000d0f0: 6c65 2829 0a20 2020 2020 2020 2073 656c  le().        sel
-0000d100: 662e 7374 6174 696f 6e5b 2253 7472 6565  f.station["Stree
-0000d110: 7431 225d 203d 2073 656c 662e 7365 7474  t1"] = self.sett
-0000d120: 696e 6773 5f64 6961 6c6f 672e 4164 6472  ings_dialog.Addr
-0000d130: 6573 7331 2e74 6578 7428 292e 7469 746c  ess1.text().titl
-0000d140: 6528 290a 2020 2020 2020 2020 7365 6c66  e().        self
-0000d150: 2e73 7461 7469 6f6e 5b22 5374 7265 6574  .station["Street
-0000d160: 3222 5d20 3d20 7365 6c66 2e73 6574 7469  2"] = self.setti
-0000d170: 6e67 735f 6469 616c 6f67 2e41 6464 7265  ngs_dialog.Addre
-0000d180: 7373 322e 7465 7874 2829 2e74 6974 6c65  ss2.text().title
-0000d190: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
-0000d1a0: 7374 6174 696f 6e5b 2243 6974 7922 5d20  station["City"] 
-0000d1b0: 3d20 7365 6c66 2e73 6574 7469 6e67 735f  = self.settings_
-0000d1c0: 6469 616c 6f67 2e43 6974 792e 7465 7874  dialog.City.text
-0000d1d0: 2829 2e74 6974 6c65 2829 0a20 2020 2020  ().title().     
-0000d1e0: 2020 2073 656c 662e 7374 6174 696f 6e5b     self.station[
-0000d1f0: 2253 7461 7465 225d 203d 2073 656c 662e  "State"] = self.
+0000cfd0: 436c 7562 222c 2022 2229 290a 2020 2020  Club", "")).    
+0000cfe0: 2020 2020 7365 6c66 2e73 6574 7469 6e67      self.setting
+0000cff0: 735f 6469 616c 6f67 2e45 6d61 696c 2e73  s_dialog.Email.s
+0000d000: 6574 5465 7874 2873 656c 662e 7374 6174  etText(self.stat
+0000d010: 696f 6e2e 6765 7428 2245 6d61 696c 222c  ion.get("Email",
+0000d020: 2022 2229 290a 2020 2020 2020 2020 7365   "")).        se
+0000d030: 6c66 2e73 6574 7469 6e67 735f 6469 616c  lf.settings_dial
+0000d040: 6f67 2e6f 7065 6e28 290a 0a20 2020 2064  og.open()..    d
+0000d050: 6566 2073 6176 655f 7365 7474 696e 6773  ef save_settings
+0000d060: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0000d070: 2222 2253 6176 6520 7365 7474 696e 6773  """Save settings
+0000d080: 2222 220a 2020 2020 2020 2020 6373 203d  """.        cs =
+0000d090: 2073 656c 662e 7365 7474 696e 6773 5f64   self.settings_d
+0000d0a0: 6961 6c6f 672e 4361 6c6c 2e74 6578 7428  ialog.Call.text(
+0000d0b0: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
+0000d0c0: 7461 7469 6f6e 203d 207b 7d0a 2020 2020  tation = {}.    
+0000d0d0: 2020 2020 7365 6c66 2e73 7461 7469 6f6e      self.station
+0000d0e0: 5b22 4361 6c6c 225d 203d 2063 732e 7570  ["Call"] = cs.up
+0000d0f0: 7065 7228 290a 2020 2020 2020 2020 7365  per().        se
+0000d100: 6c66 2e73 7461 7469 6f6e 5b22 4e61 6d65  lf.station["Name
+0000d110: 225d 203d 2073 656c 662e 7365 7474 696e  "] = self.settin
+0000d120: 6773 5f64 6961 6c6f 672e 4e61 6d65 2e74  gs_dialog.Name.t
+0000d130: 6578 7428 292e 7469 746c 6528 290a 2020  ext().title().  
+0000d140: 2020 2020 2020 7365 6c66 2e73 7461 7469        self.stati
+0000d150: 6f6e 5b22 5374 7265 6574 3122 5d20 3d20  on["Street1"] = 
+0000d160: 7365 6c66 2e73 6574 7469 6e67 735f 6469  self.settings_di
+0000d170: 616c 6f67 2e41 6464 7265 7373 312e 7465  alog.Address1.te
+0000d180: 7874 2829 2e74 6974 6c65 2829 0a20 2020  xt().title().   
+0000d190: 2020 2020 2073 656c 662e 7374 6174 696f       self.statio
+0000d1a0: 6e5b 2253 7472 6565 7432 225d 203d 2073  n["Street2"] = s
+0000d1b0: 656c 662e 7365 7474 696e 6773 5f64 6961  elf.settings_dia
+0000d1c0: 6c6f 672e 4164 6472 6573 7332 2e74 6578  log.Address2.tex
+0000d1d0: 7428 292e 7469 746c 6528 290a 2020 2020  t().title().    
+0000d1e0: 2020 2020 7365 6c66 2e73 7461 7469 6f6e      self.station
+0000d1f0: 5b22 4369 7479 225d 203d 2073 656c 662e  ["City"] = self.
 0000d200: 7365 7474 696e 6773 5f64 6961 6c6f 672e  settings_dialog.
-0000d210: 5374 6174 652e 7465 7874 2829 2e75 7070  State.text().upp
-0000d220: 6572 2829 0a20 2020 2020 2020 2073 656c  er().        sel
-0000d230: 662e 7374 6174 696f 6e5b 225a 6970 225d  f.station["Zip"]
-0000d240: 203d 2073 656c 662e 7365 7474 696e 6773   = self.settings
-0000d250: 5f64 6961 6c6f 672e 5a69 702e 7465 7874  _dialog.Zip.text
-0000d260: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
-0000d270: 7374 6174 696f 6e5b 2243 6f75 6e74 7279  station["Country
-0000d280: 225d 203d 2073 656c 662e 7365 7474 696e  "] = self.settin
-0000d290: 6773 5f64 6961 6c6f 672e 436f 756e 7472  gs_dialog.Countr
-0000d2a0: 792e 7465 7874 2829 2e74 6974 6c65 2829  y.text().title()
-0000d2b0: 0a20 2020 2020 2020 2073 656c 662e 7374  .        self.st
-0000d2c0: 6174 696f 6e5b 2247 7269 6453 7175 6172  ation["GridSquar
-0000d2d0: 6522 5d20 3d20 7365 6c66 2e73 6574 7469  e"] = self.setti
-0000d2e0: 6e67 735f 6469 616c 6f67 2e47 7269 6453  ngs_dialog.GridS
-0000d2f0: 7175 6172 652e 7465 7874 2829 0a20 2020  quare.text().   
-0000d300: 2020 2020 2073 656c 662e 7374 6174 696f       self.statio
-0000d310: 6e5b 2243 515a 6f6e 6522 5d20 3d20 7365  n["CQZone"] = se
-0000d320: 6c66 2e73 6574 7469 6e67 735f 6469 616c  lf.settings_dial
-0000d330: 6f67 2e43 515a 6f6e 652e 7465 7874 2829  og.CQZone.text()
-0000d340: 0a20 2020 2020 2020 2073 656c 662e 7374  .        self.st
-0000d350: 6174 696f 6e5b 2249 4152 555a 6f6e 6522  ation["IARUZone"
-0000d360: 5d20 3d20 7365 6c66 2e73 6574 7469 6e67  ] = self.setting
-0000d370: 735f 6469 616c 6f67 2e49 5455 5a6f 6e65  s_dialog.ITUZone
-0000d380: 2e74 6578 7428 290a 2020 2020 2020 2020  .text().        
-0000d390: 7365 6c66 2e73 7461 7469 6f6e 5b22 4c69  self.station["Li
-0000d3a0: 6365 6e73 6543 6c61 7373 225d 203d 2073  censeClass"] = s
-0000d3b0: 656c 662e 7365 7474 696e 6773 5f64 6961  elf.settings_dia
-0000d3c0: 6c6f 672e 4c69 6365 6e73 652e 7465 7874  log.License.text
-0000d3d0: 2829 2e74 6974 6c65 2829 0a20 2020 2020  ().title().     
-0000d3e0: 2020 2073 656c 662e 7374 6174 696f 6e5b     self.station[
-0000d3f0: 224c 6174 6974 7564 6522 5d20 3d20 7365  "Latitude"] = se
-0000d400: 6c66 2e73 6574 7469 6e67 735f 6469 616c  lf.settings_dial
-0000d410: 6f67 2e4c 6174 6974 7564 652e 7465 7874  og.Latitude.text
-0000d420: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
-0000d430: 7374 6174 696f 6e5b 224c 6f6e 6769 7475  station["Longitu
+0000d210: 4369 7479 2e74 6578 7428 292e 7469 746c  City.text().titl
+0000d220: 6528 290a 2020 2020 2020 2020 7365 6c66  e().        self
+0000d230: 2e73 7461 7469 6f6e 5b22 5374 6174 6522  .station["State"
+0000d240: 5d20 3d20 7365 6c66 2e73 6574 7469 6e67  ] = self.setting
+0000d250: 735f 6469 616c 6f67 2e53 7461 7465 2e74  s_dialog.State.t
+0000d260: 6578 7428 292e 7570 7065 7228 290a 2020  ext().upper().  
+0000d270: 2020 2020 2020 7365 6c66 2e73 7461 7469        self.stati
+0000d280: 6f6e 5b22 5a69 7022 5d20 3d20 7365 6c66  on["Zip"] = self
+0000d290: 2e73 6574 7469 6e67 735f 6469 616c 6f67  .settings_dialog
+0000d2a0: 2e5a 6970 2e74 6578 7428 290a 2020 2020  .Zip.text().    
+0000d2b0: 2020 2020 7365 6c66 2e73 7461 7469 6f6e      self.station
+0000d2c0: 5b22 436f 756e 7472 7922 5d20 3d20 7365  ["Country"] = se
+0000d2d0: 6c66 2e73 6574 7469 6e67 735f 6469 616c  lf.settings_dial
+0000d2e0: 6f67 2e43 6f75 6e74 7279 2e74 6578 7428  og.Country.text(
+0000d2f0: 292e 7469 746c 6528 290a 2020 2020 2020  ).title().      
+0000d300: 2020 7365 6c66 2e73 7461 7469 6f6e 5b22    self.station["
+0000d310: 4772 6964 5371 7561 7265 225d 203d 2073  GridSquare"] = s
+0000d320: 656c 662e 7365 7474 696e 6773 5f64 6961  elf.settings_dia
+0000d330: 6c6f 672e 4772 6964 5371 7561 7265 2e74  log.GridSquare.t
+0000d340: 6578 7428 290a 2020 2020 2020 2020 7365  ext().        se
+0000d350: 6c66 2e73 7461 7469 6f6e 5b22 4351 5a6f  lf.station["CQZo
+0000d360: 6e65 225d 203d 2073 656c 662e 7365 7474  ne"] = self.sett
+0000d370: 696e 6773 5f64 6961 6c6f 672e 4351 5a6f  ings_dialog.CQZo
+0000d380: 6e65 2e74 6578 7428 290a 2020 2020 2020  ne.text().      
+0000d390: 2020 7365 6c66 2e73 7461 7469 6f6e 5b22    self.station["
+0000d3a0: 4941 5255 5a6f 6e65 225d 203d 2073 656c  IARUZone"] = sel
+0000d3b0: 662e 7365 7474 696e 6773 5f64 6961 6c6f  f.settings_dialo
+0000d3c0: 672e 4954 555a 6f6e 652e 7465 7874 2829  g.ITUZone.text()
+0000d3d0: 0a20 2020 2020 2020 2073 656c 662e 7374  .        self.st
+0000d3e0: 6174 696f 6e5b 224c 6963 656e 7365 436c  ation["LicenseCl
+0000d3f0: 6173 7322 5d20 3d20 7365 6c66 2e73 6574  ass"] = self.set
+0000d400: 7469 6e67 735f 6469 616c 6f67 2e4c 6963  tings_dialog.Lic
+0000d410: 656e 7365 2e74 6578 7428 292e 7469 746c  ense.text().titl
+0000d420: 6528 290a 2020 2020 2020 2020 7365 6c66  e().        self
+0000d430: 2e73 7461 7469 6f6e 5b22 4c61 7469 7475  .station["Latitu
 0000d440: 6465 225d 203d 2073 656c 662e 7365 7474  de"] = self.sett
-0000d450: 696e 6773 5f64 6961 6c6f 672e 4c6f 6e67  ings_dialog.Long
-0000d460: 6974 7564 652e 7465 7874 2829 0a20 2020  itude.text().   
-0000d470: 2020 2020 2073 656c 662e 7374 6174 696f       self.statio
-0000d480: 6e5b 2253 5458 6571 225d 203d 2073 656c  n["STXeq"] = sel
-0000d490: 662e 7365 7474 696e 6773 5f64 6961 6c6f  f.settings_dialo
-0000d4a0: 672e 5374 6174 696f 6e54 5852 582e 7465  g.StationTXRX.te
-0000d4b0: 7874 2829 0a20 2020 2020 2020 2073 656c  xt().        sel
-0000d4c0: 662e 7374 6174 696f 6e5b 2253 506f 7765  f.station["SPowe
-0000d4d0: 225d 203d 2073 656c 662e 7365 7474 696e  "] = self.settin
-0000d4e0: 6773 5f64 6961 6c6f 672e 506f 7765 722e  gs_dialog.Power.
-0000d4f0: 7465 7874 2829 0a20 2020 2020 2020 2073  text().        s
-0000d500: 656c 662e 7374 6174 696f 6e5b 2253 416e  elf.station["SAn
-0000d510: 7465 225d 203d 2073 656c 662e 7365 7474  te"] = self.sett
-0000d520: 696e 6773 5f64 6961 6c6f 672e 416e 7465  ings_dialog.Ante
-0000d530: 6e6e 612e 7465 7874 2829 0a20 2020 2020  nna.text().     
-0000d540: 2020 2073 656c 662e 7374 6174 696f 6e5b     self.station[
-0000d550: 2253 416e 7448 3122 5d20 3d20 7365 6c66  "SAntH1"] = self
-0000d560: 2e73 6574 7469 6e67 735f 6469 616c 6f67  .settings_dialog
-0000d570: 2e41 6e74 4865 6967 6874 2e74 6578 7428  .AntHeight.text(
-0000d580: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
-0000d590: 7461 7469 6f6e 5b22 5341 6e74 4832 225d  tation["SAntH2"]
-0000d5a0: 203d 2073 656c 662e 7365 7474 696e 6773   = self.settings
-0000d5b0: 5f64 6961 6c6f 672e 4153 4c2e 7465 7874  _dialog.ASL.text
-0000d5c0: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
-0000d5d0: 7374 6174 696f 6e5b 2241 5252 4c53 6563  station["ARRLSec
-0000d5e0: 7469 6f6e 225d 203d 2073 656c 662e 7365  tion"] = self.se
-0000d5f0: 7474 696e 6773 5f64 6961 6c6f 672e 4152  ttings_dialog.AR
-0000d600: 524c 5365 6374 696f 6e2e 7465 7874 2829  RLSection.text()
-0000d610: 2e75 7070 6572 2829 0a20 2020 2020 2020  .upper().       
-0000d620: 2073 656c 662e 7374 6174 696f 6e5b 2252   self.station["R
-0000d630: 6f76 6572 5154 4822 5d20 3d20 7365 6c66  overQTH"] = self
-0000d640: 2e73 6574 7469 6e67 735f 6469 616c 6f67  .settings_dialog
-0000d650: 2e52 6f76 6572 5154 482e 7465 7874 2829  .RoverQTH.text()
-0000d660: 0a20 2020 2020 2020 2073 656c 662e 7374  .        self.st
-0000d670: 6174 696f 6e5b 2243 6c75 6222 5d20 3d20  ation["Club"] = 
-0000d680: 7365 6c66 2e73 6574 7469 6e67 735f 6469  self.settings_di
-0000d690: 616c 6f67 2e43 6c75 622e 7465 7874 2829  alog.Club.text()
-0000d6a0: 2e74 6974 6c65 2829 0a20 2020 2020 2020  .title().       
-0000d6b0: 2073 656c 662e 7374 6174 696f 6e5b 2245   self.station["E
-0000d6c0: 6d61 696c 225d 203d 2073 656c 662e 7365  mail"] = self.se
-0000d6d0: 7474 696e 6773 5f64 6961 6c6f 672e 456d  ttings_dialog.Em
-0000d6e0: 6169 6c2e 7465 7874 2829 0a20 2020 2020  ail.text().     
-0000d6f0: 2020 2073 656c 662e 6461 7461 6261 7365     self.database
-0000d700: 2e61 6464 5f73 7461 7469 6f6e 2873 656c  .add_station(sel
-0000d710: 662e 7374 6174 696f 6e29 0a20 2020 2020  f.station).     
-0000d720: 2020 2073 656c 662e 7365 7474 696e 6773     self.settings
-0000d730: 5f64 6961 6c6f 672e 636c 6f73 6528 290a  _dialog.close().
-0000d740: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0000d750: 6375 7272 656e 745f 6f70 203d 3d20 2222  current_op == ""
-0000d760: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-0000d770: 6c66 2e63 7572 7265 6e74 5f6f 7020 3d20  lf.current_op = 
-0000d780: 7365 6c66 2e73 7461 7469 6f6e 2e67 6574  self.station.get
-0000d790: 2822 4361 6c6c 222c 2022 2229 0a20 2020  ("Call", "").   
-0000d7a0: 2020 2020 2020 2020 2073 656c 662e 6d61           self.ma
-0000d7b0: 6b65 5f6f 705f 6469 7228 290a 2020 2020  ke_op_dir().    
-0000d7c0: 2020 2020 636f 6e74 6573 745f 636f 756e      contest_coun
-0000d7d0: 7420 3d20 7365 6c66 2e64 6174 6162 6173  t = self.databas
-0000d7e0: 652e 6665 7463 685f 616c 6c5f 636f 6e74  e.fetch_all_cont
-0000d7f0: 6573 7473 2829 0a20 2020 2020 2020 2069  ests().        i
-0000d800: 6620 6c65 6e28 636f 6e74 6573 745f 636f  f len(contest_co
-0000d810: 756e 7429 203d 3d20 303a 0a20 2020 2020  unt) == 0:.     
-0000d820: 2020 2020 2020 2073 656c 662e 6e65 775f         self.new_
-0000d830: 636f 6e74 6573 745f 6469 616c 6f67 2829  contest_dialog()
-0000d840: 0a0a 2020 2020 6465 6620 6564 6974 5f6d  ..    def edit_m
-0000d850: 6163 726f 2873 656c 662c 2066 756e 6374  acro(self, funct
-0000d860: 696f 6e5f 6b65 7929 3a0a 2020 2020 2020  ion_key):.      
-0000d870: 2020 2222 2253 686f 7720 6564 6974 206d    """Show edit m
-0000d880: 6163 726f 2064 6961 6c6f 6722 2222 0a20  acro dialog""". 
-0000d890: 2020 2020 2020 2073 656c 662e 6564 6974         self.edit
-0000d8a0: 5f6d 6163 726f 5f64 6961 6c6f 6720 3d20  _macro_dialog = 
-0000d8b0: 4564 6974 4d61 6372 6f28 6675 6e63 7469  EditMacro(functi
-0000d8c0: 6f6e 5f6b 6579 2c20 574f 524b 494e 475f  on_key, WORKING_
-0000d8d0: 5041 5448 290a 2020 2020 2020 2020 7365  PATH).        se
-0000d8e0: 6c66 2e65 6469 745f 6d61 6372 6f5f 6469  lf.edit_macro_di
-0000d8f0: 616c 6f67 2e61 6363 6570 7465 642e 636f  alog.accepted.co
-0000d900: 6e6e 6563 7428 7365 6c66 2e65 6469 7465  nnect(self.edite
-0000d910: 645f 6d61 6372 6f29 0a20 2020 2020 2020  d_macro).       
-0000d920: 2073 656c 662e 6564 6974 5f6d 6163 726f   self.edit_macro
-0000d930: 5f64 6961 6c6f 672e 6f70 656e 2829 0a0a  _dialog.open()..
-0000d940: 2020 2020 6465 6620 6564 6974 6564 5f6d      def edited_m
-0000d950: 6163 726f 2873 656c 6629 3a0a 2020 2020  acro(self):.    
-0000d960: 2020 2020 2222 2253 6176 6520 6564 6974      """Save edit
-0000d970: 6564 206d 6163 726f 2222 220a 2020 2020  ed macro""".    
-0000d980: 2020 2020 7365 6c66 2e65 6469 745f 6d61      self.edit_ma
-0000d990: 6372 6f5f 6469 616c 6f67 2e66 756e 6374  cro_dialog.funct
-0000d9a0: 696f 6e5f 6b65 792e 7365 7454 6578 7428  ion_key.setText(
-0000d9b0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000d9c0: 662e 6564 6974 5f6d 6163 726f 5f64 6961  f.edit_macro_dia
-0000d9d0: 6c6f 672e 6d61 6372 6f5f 6c61 6265 6c2e  log.macro_label.
-0000d9e0: 7465 7874 2829 0a20 2020 2020 2020 2029  text().        )
-0000d9f0: 0a20 2020 2020 2020 2073 656c 662e 6564  .        self.ed
-0000da00: 6974 5f6d 6163 726f 5f64 6961 6c6f 672e  it_macro_dialog.
-0000da10: 6675 6e63 7469 6f6e 5f6b 6579 2e73 6574  function_key.set
-0000da20: 546f 6f6c 5469 7028 0a20 2020 2020 2020  ToolTip(.       
-0000da30: 2020 2020 2073 656c 662e 6564 6974 5f6d       self.edit_m
-0000da40: 6163 726f 5f64 6961 6c6f 672e 7468 655f  acro_dialog.the_
-0000da50: 6d61 6372 6f2e 7465 7874 2829 0a20 2020  macro.text().   
-0000da60: 2020 2020 2029 0a20 2020 2020 2020 2073       ).        s
-0000da70: 656c 662e 6564 6974 5f6d 6163 726f 5f64  elf.edit_macro_d
-0000da80: 6961 6c6f 672e 636c 6f73 6528 290a 0a20  ialog.close().. 
-0000da90: 2020 2064 6566 2065 6469 745f 4631 2873     def edit_F1(s
-0000daa0: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
-0000dab0: 2273 7475 6222 2222 0a20 2020 2020 2020  "stub""".       
-0000dac0: 206c 6f67 6765 722e 6465 6275 6728 2246   logger.debug("F
-0000dad0: 3120 5269 6768 7420 436c 6963 6b65 642e  1 Right Clicked.
-0000dae0: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
-0000daf0: 6564 6974 5f6d 6163 726f 2873 656c 662e  edit_macro(self.
-0000db00: 4631 290a 0a20 2020 2064 6566 2065 6469  F1)..    def edi
-0000db10: 745f 4632 2873 656c 6629 3a0a 2020 2020  t_F2(self):.    
-0000db20: 2020 2020 2222 2273 7475 6222 2222 0a20      """stub""". 
-0000db30: 2020 2020 2020 206c 6f67 6765 722e 6465         logger.de
-0000db40: 6275 6728 2246 3220 5269 6768 7420 436c  bug("F2 Right Cl
-0000db50: 6963 6b65 642e 2229 0a20 2020 2020 2020  icked.").       
-0000db60: 2073 656c 662e 6564 6974 5f6d 6163 726f   self.edit_macro
-0000db70: 2873 656c 662e 4632 290a 0a20 2020 2064  (self.F2)..    d
-0000db80: 6566 2065 6469 745f 4633 2873 656c 6629  ef edit_F3(self)
-0000db90: 3a0a 2020 2020 2020 2020 2222 2273 7475  :.        """stu
-0000dba0: 6222 2222 0a20 2020 2020 2020 206c 6f67  b""".        log
-0000dbb0: 6765 722e 6465 6275 6728 2246 3320 5269  ger.debug("F3 Ri
-0000dbc0: 6768 7420 436c 6963 6b65 642e 2229 0a20  ght Clicked."). 
-0000dbd0: 2020 2020 2020 2073 656c 662e 6564 6974         self.edit
-0000dbe0: 5f6d 6163 726f 2873 656c 662e 4633 290a  _macro(self.F3).
-0000dbf0: 0a20 2020 2064 6566 2065 6469 745f 4634  .    def edit_F4
-0000dc00: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-0000dc10: 2222 2273 7475 6222 2222 0a20 2020 2020  """stub""".     
-0000dc20: 2020 206c 6f67 6765 722e 6465 6275 6728     logger.debug(
-0000dc30: 2246 3420 5269 6768 7420 436c 6963 6b65  "F4 Right Clicke
-0000dc40: 642e 2229 0a20 2020 2020 2020 2073 656c  d.").        sel
-0000dc50: 662e 6564 6974 5f6d 6163 726f 2873 656c  f.edit_macro(sel
-0000dc60: 662e 4634 290a 0a20 2020 2064 6566 2065  f.F4)..    def e
-0000dc70: 6469 745f 4635 2873 656c 6629 3a0a 2020  dit_F5(self):.  
-0000dc80: 2020 2020 2020 2222 2273 7475 6222 2222        """stub"""
-0000dc90: 0a20 2020 2020 2020 206c 6f67 6765 722e  .        logger.
-0000dca0: 6465 6275 6728 2246 3520 5269 6768 7420  debug("F5 Right 
-0000dcb0: 436c 6963 6b65 642e 2229 0a20 2020 2020  Clicked.").     
-0000dcc0: 2020 2073 656c 662e 6564 6974 5f6d 6163     self.edit_mac
-0000dcd0: 726f 2873 656c 662e 4635 290a 0a20 2020  ro(self.F5)..   
-0000dce0: 2064 6566 2065 6469 745f 4636 2873 656c   def edit_F6(sel
-0000dcf0: 6629 3a0a 2020 2020 2020 2020 2222 2273  f):.        """s
-0000dd00: 7475 6222 2222 0a20 2020 2020 2020 206c  tub""".        l
-0000dd10: 6f67 6765 722e 6465 6275 6728 2246 3620  ogger.debug("F6 
-0000dd20: 5269 6768 7420 436c 6963 6b65 642e 2229  Right Clicked.")
-0000dd30: 0a20 2020 2020 2020 2073 656c 662e 6564  .        self.ed
-0000dd40: 6974 5f6d 6163 726f 2873 656c 662e 4636  it_macro(self.F6
-0000dd50: 290a 0a20 2020 2064 6566 2065 6469 745f  )..    def edit_
-0000dd60: 4637 2873 656c 6629 3a0a 2020 2020 2020  F7(self):.      
-0000dd70: 2020 2222 2273 7475 6222 2222 0a20 2020    """stub""".   
-0000dd80: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
-0000dd90: 6728 2246 3720 5269 6768 7420 436c 6963  g("F7 Right Clic
-0000dda0: 6b65 642e 2229 0a20 2020 2020 2020 2073  ked.").        s
-0000ddb0: 656c 662e 6564 6974 5f6d 6163 726f 2873  elf.edit_macro(s
-0000ddc0: 656c 662e 4637 290a 0a20 2020 2064 6566  elf.F7)..    def
-0000ddd0: 2065 6469 745f 4638 2873 656c 6629 3a0a   edit_F8(self):.
-0000dde0: 2020 2020 2020 2020 2222 2273 7475 6222          """stub"
-0000ddf0: 2222 0a20 2020 2020 2020 206c 6f67 6765  "".        logge
-0000de00: 722e 6465 6275 6728 2246 3820 5269 6768  r.debug("F8 Righ
-0000de10: 7420 436c 6963 6b65 642e 2229 0a20 2020  t Clicked.").   
-0000de20: 2020 2020 2073 656c 662e 6564 6974 5f6d       self.edit_m
-0000de30: 6163 726f 2873 656c 662e 4638 290a 0a20  acro(self.F8).. 
-0000de40: 2020 2064 6566 2065 6469 745f 4639 2873     def edit_F9(s
-0000de50: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
-0000de60: 2273 7475 6222 2222 0a20 2020 2020 2020  "stub""".       
-0000de70: 206c 6f67 6765 722e 6465 6275 6728 2246   logger.debug("F
-0000de80: 3920 5269 6768 7420 436c 6963 6b65 642e  9 Right Clicked.
-0000de90: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
-0000dea0: 6564 6974 5f6d 6163 726f 2873 656c 662e  edit_macro(self.
-0000deb0: 4639 290a 0a20 2020 2064 6566 2065 6469  F9)..    def edi
-0000dec0: 745f 4631 3028 7365 6c66 293a 0a20 2020  t_F10(self):.   
-0000ded0: 2020 2020 2022 2222 7374 7562 2222 220a       """stub""".
-0000dee0: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
-0000def0: 6562 7567 2822 4631 3020 5269 6768 7420  ebug("F10 Right 
-0000df00: 436c 6963 6b65 642e 2229 0a20 2020 2020  Clicked.").     
-0000df10: 2020 2073 656c 662e 6564 6974 5f6d 6163     self.edit_mac
-0000df20: 726f 2873 656c 662e 4631 3029 0a0a 2020  ro(self.F10)..  
-0000df30: 2020 6465 6620 6564 6974 5f46 3131 2873    def edit_F11(s
-0000df40: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
-0000df50: 2273 7475 6222 2222 0a20 2020 2020 2020  "stub""".       
-0000df60: 206c 6f67 6765 722e 6465 6275 6728 2246   logger.debug("F
-0000df70: 3131 2052 6967 6874 2043 6c69 636b 6564  11 Right Clicked
-0000df80: 2e22 290a 2020 2020 2020 2020 7365 6c66  .").        self
-0000df90: 2e65 6469 745f 6d61 6372 6f28 7365 6c66  .edit_macro(self
-0000dfa0: 2e46 3131 290a 0a20 2020 2064 6566 2065  .F11)..    def e
-0000dfb0: 6469 745f 4631 3228 7365 6c66 293a 0a20  dit_F12(self):. 
-0000dfc0: 2020 2020 2020 2022 2222 7374 7562 2222         """stub""
-0000dfd0: 220a 2020 2020 2020 2020 6c6f 6767 6572  ".        logger
-0000dfe0: 2e64 6562 7567 2822 4631 3220 5269 6768  .debug("F12 Righ
-0000dff0: 7420 436c 6963 6b65 642e 2229 0a20 2020  t Clicked.").   
-0000e000: 2020 2020 2073 656c 662e 6564 6974 5f6d       self.edit_m
-0000e010: 6163 726f 2873 656c 662e 4631 3229 0a0a  acro(self.F12)..
-0000e020: 2020 2020 6465 6620 7072 6f63 6573 735f      def process_
-0000e030: 6d61 6372 6f28 7365 6c66 2c20 6d61 6372  macro(self, macr
-0000e040: 6f3a 2073 7472 2920 2d3e 2073 7472 3a0a  o: str) -> str:.
-0000e050: 2020 2020 2020 2020 2222 2250 726f 6365          """Proce
-0000e060: 7373 2043 5720 6d61 6372 6f20 7375 6273  ss CW macro subs
-0000e070: 7469 7475 7469 6f6e 7322 2222 0a20 2020  titutions""".   
-0000e080: 2020 2020 2072 6573 756c 7420 3d20 7365       result = se
-0000e090: 6c66 2e64 6174 6162 6173 652e 6765 745f  lf.database.get_
-0000e0a0: 7365 7269 616c 2829 0a20 2020 2020 2020  serial().       
-0000e0b0: 206e 6578 745f 7365 7269 616c 203d 2073   next_serial = s
-0000e0c0: 7472 2872 6573 756c 742e 6765 7428 2273  tr(result.get("s
-0000e0d0: 6572 6961 6c5f 6e72 222c 2022 3122 2929  erial_nr", "1"))
-0000e0e0: 0a20 2020 2020 2020 2069 6620 6e65 7874  .        if next
-0000e0f0: 5f73 6572 6961 6c20 3d3d 2022 4e6f 6e65  _serial == "None
-0000e100: 223a 0a20 2020 2020 2020 2020 2020 206e  ":.            n
-0000e110: 6578 745f 7365 7269 616c 203d 2022 3122  ext_serial = "1"
-0000e120: 0a20 2020 2020 2020 206d 6163 726f 203d  .        macro =
-0000e130: 206d 6163 726f 2e75 7070 6572 2829 0a20   macro.upper(). 
-0000e140: 2020 2020 2020 206d 6163 726f 203d 206d         macro = m
-0000e150: 6163 726f 2e72 6570 6c61 6365 2822 2322  acro.replace("#"
-0000e160: 2c20 6e65 7874 5f73 6572 6961 6c29 0a20  , next_serial). 
-0000e170: 2020 2020 2020 206d 6163 726f 203d 206d         macro = m
-0000e180: 6163 726f 2e72 6570 6c61 6365 2822 7b4d  acro.replace("{M
-0000e190: 5943 414c 4c7d 222c 2073 656c 662e 7374  YCALL}", self.st
-0000e1a0: 6174 696f 6e2e 6765 7428 2243 616c 6c22  ation.get("Call"
-0000e1b0: 2c20 2222 2929 0a20 2020 2020 2020 206d  , "")).        m
-0000e1c0: 6163 726f 203d 206d 6163 726f 2e72 6570  acro = macro.rep
-0000e1d0: 6c61 6365 2822 7b48 4953 4341 4c4c 7d22  lace("{HISCALL}"
-0000e1e0: 2c20 7365 6c66 2e63 616c 6c73 6967 6e2e  , self.callsign.
-0000e1f0: 7465 7874 2829 290a 2020 2020 2020 2020  text()).        
-0000e200: 6966 2073 656c 662e 7261 6469 6f5f 7374  if self.radio_st
-0000e210: 6174 652e 6765 7428 226d 6f64 6522 2920  ate.get("mode") 
-0000e220: 3d3d 2022 4357 223a 0a20 2020 2020 2020  == "CW":.       
-0000e230: 2020 2020 206d 6163 726f 203d 206d 6163       macro = mac
-0000e240: 726f 2e72 6570 6c61 6365 2822 7b53 4e54  ro.replace("{SNT
-0000e250: 7d22 2c20 7365 6c66 2e73 656e 742e 7465  }", self.sent.te
-0000e260: 7874 2829 2e72 6570 6c61 6365 2822 3922  xt().replace("9"
-0000e270: 2c20 226e 2229 290a 2020 2020 2020 2020  , "n")).        
-0000e280: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-0000e290: 2020 6d61 6372 6f20 3d20 6d61 6372 6f2e    macro = macro.
-0000e2a0: 7265 706c 6163 6528 227b 534e 547d 222c  replace("{SNT}",
-0000e2b0: 2073 656c 662e 7365 6e74 2e74 6578 7428   self.sent.text(
-0000e2c0: 2929 0a20 2020 2020 2020 206d 6163 726f  )).        macro
-0000e2d0: 203d 206d 6163 726f 2e72 6570 6c61 6365   = macro.replace
-0000e2e0: 2822 7b53 454e 544e 527d 222c 2073 656c  ("{SENTNR}", sel
-0000e2f0: 662e 6f74 6865 725f 312e 7465 7874 2829  f.other_1.text()
-0000e300: 290a 2020 2020 2020 2020 6d61 6372 6f20  ).        macro 
-0000e310: 3d20 6d61 6372 6f2e 7265 706c 6163 6528  = macro.replace(
-0000e320: 0a20 2020 2020 2020 2020 2020 2022 7b45  .            "{E
-0000e330: 5843 487d 222c 2073 656c 662e 636f 6e74  XCH}", self.cont
-0000e340: 6573 745f 7365 7474 696e 6773 2e67 6574  est_settings.get
-0000e350: 2822 5365 6e74 4578 6368 616e 6765 222c  ("SentExchange",
-0000e360: 2022 7878 7822 290a 2020 2020 2020 2020   "xxx").        
-0000e370: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-0000e380: 206d 6163 726f 0a0a 2020 2020 6465 6620   macro..    def 
-0000e390: 766f 6963 655f 7374 7269 6e67 2873 656c  voice_string(sel
-0000e3a0: 662c 2074 6865 5f73 7472 696e 673a 2073  f, the_string: s
-0000e3b0: 7472 2920 2d3e 204e 6f6e 653a 0a20 2020  tr) -> None:.   
-0000e3c0: 2020 2020 2022 2222 766f 6963 6573 2073       """voices s
-0000e3d0: 7472 696e 6720 7573 696e 6720 6e61 746f  tring using nato
-0000e3e0: 2070 686f 6e65 7469 6373 2222 220a 2020   phonetics""".  
-0000e3f0: 2020 2020 2020 6c6f 6767 6572 2e64 6562        logger.deb
-0000e400: 7567 2822 566f 6963 696e 673a 2025 7322  ug("Voicing: %s"
-0000e410: 2c20 7468 655f 7374 7269 6e67 290a 2020  , the_string).  
-0000e420: 2020 2020 2020 6f70 5f70 6174 6820 3d20        op_path = 
-0000e430: 5061 7468 2844 4154 415f 5041 5448 2920  Path(DATA_PATH) 
-0000e440: 2f20 7365 6c66 2e63 7572 7265 6e74 5f6f  / self.current_o
-0000e450: 700a 2020 2020 2020 2020 6966 2022 5b22  p.        if "["
-0000e460: 2069 6e20 7468 655f 7374 7269 6e67 3a0a   in the_string:.
-0000e470: 2020 2020 2020 2020 2020 2020 7375 625f              sub_
-0000e480: 7374 7269 6e67 203d 2074 6865 5f73 7472  string = the_str
-0000e490: 696e 672e 7374 7269 7028 225b 5d22 292e  ing.strip("[]").
-0000e4a0: 6c6f 7765 7228 290a 2020 2020 2020 2020  lower().        
-0000e4b0: 2020 2020 6669 6c65 6e61 6d65 203d 2066      filename = f
-0000e4c0: 227b 7374 7228 6f70 5f70 6174 6829 7d2f  "{str(op_path)}/
-0000e4d0: 7b73 7562 5f73 7472 696e 677d 2e77 6176  {sub_string}.wav
-0000e4e0: 220a 2020 2020 2020 2020 2020 2020 6966  ".            if
-0000e4f0: 2050 6174 6828 6669 6c65 6e61 6d65 292e   Path(filename).
-0000e500: 6973 5f66 696c 6528 293a 0a20 2020 2020  is_file():.     
-0000e510: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
-0000e520: 722e 6465 6275 6728 2256 6f69 6369 6e67  r.debug("Voicing
-0000e530: 3a20 2573 222c 2066 696c 656e 616d 6529  : %s", filename)
-0000e540: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e550: 2064 6174 612c 205f 6673 203d 2073 662e   data, _fs = sf.
-0000e560: 7265 6164 2866 696c 656e 616d 652c 2064  read(filename, d
-0000e570: 7479 7065 3d22 666c 6f61 7433 3222 290a  type="float32").
-0000e580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e590: 7365 6c66 2e70 7474 5f6f 6e28 290a 2020  self.ptt_on().  
-0000e5a0: 2020 2020 2020 2020 2020 2020 2020 7472                tr
-0000e5b0: 793a 0a20 2020 2020 2020 2020 2020 2020  y:.             
-0000e5c0: 2020 2020 2020 2073 642e 6465 6661 756c         sd.defaul
-0000e5d0: 742e 6465 7669 6365 203d 2073 656c 662e  t.device = self.
-0000e5e0: 7072 6566 2e67 6574 2822 736f 756e 6464  pref.get("soundd
-0000e5f0: 6576 6963 6522 2c20 2264 6566 6175 6c74  evice", "default
-0000e600: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
-0000e610: 2020 2020 2020 2073 642e 6465 6661 756c         sd.defaul
-0000e620: 742e 7361 6d70 6c65 7261 7465 203d 2034  t.samplerate = 4
-0000e630: 3431 3030 2e30 0a20 2020 2020 2020 2020  4100.0.         
-0000e640: 2020 2020 2020 2020 2020 2073 642e 706c             sd.pl
-0000e650: 6179 2864 6174 6129 0a20 2020 2020 2020  ay(data).       
-0000e660: 2020 2020 2020 2020 2020 2020 205f 7374               _st
-0000e670: 6174 7573 203d 2073 642e 7761 6974 2829  atus = sd.wait()
-0000e680: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e690: 2020 2020 2023 2068 7474 7073 3a2f 2f73       # https://s
-0000e6a0: 6e79 6b2e 696f 2f61 6476 6973 6f72 2f70  nyk.io/advisor/p
-0000e6b0: 7974 686f 6e2f 736f 756e 6464 6576 6963  ython/sounddevic
-0000e6c0: 652f 6675 6e63 7469 6f6e 732f 736f 756e  e/functions/soun
-0000e6d0: 6464 6576 6963 652e 506f 7274 4175 6469  ddevice.PortAudi
-0000e6e0: 6f45 7272 6f72 0a20 2020 2020 2020 2020  oError.         
-0000e6f0: 2020 2020 2020 2065 7863 6570 7420 7364         except sd
-0000e700: 2e50 6f72 7441 7564 696f 4572 726f 7220  .PortAudioError 
-0000e710: 6173 2065 7272 3a0a 2020 2020 2020 2020  as err:.        
-0000e720: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
-0000e730: 6572 2e77 6172 6e69 6e67 2822 2573 222c  er.warning("%s",
-0000e740: 2066 227b 6572 727d 2229 0a0a 2020 2020   f"{err}")..    
-0000e750: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000e760: 2e70 7474 5f6f 6666 2829 0a20 2020 2020  .ptt_off().     
-0000e770: 2020 2020 2020 2072 6574 7572 6e0a 2020         return.  
-0000e780: 2020 2020 2020 7365 6c66 2e70 7474 5f6f        self.ptt_o
-0000e790: 6e28 290a 2020 2020 2020 2020 666f 7220  n().        for 
-0000e7a0: 6c65 7474 6572 2069 6e20 7468 655f 7374  letter in the_st
-0000e7b0: 7269 6e67 2e6c 6f77 6572 2829 3a0a 2020  ring.lower():.  
-0000e7c0: 2020 2020 2020 2020 2020 6966 206c 6574            if let
-0000e7d0: 7465 7220 696e 2022 6162 6364 6566 6768  ter in "abcdefgh
-0000e7e0: 696a 6b6c 6d6e 6f70 7172 7374 7576 7778  ijklmnopqrstuvwx
-0000e7f0: 797a 2031 3233 3435 3637 3839 3022 3a0a  yz 1234567890":.
-0000e800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e810: 6966 206c 6574 7465 7220 3d3d 2022 2022  if letter == " "
-0000e820: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000e830: 2020 2020 2020 6c65 7474 6572 203d 2022        letter = "
-0000e840: 7370 6163 6522 0a20 2020 2020 2020 2020  space".         
-0000e850: 2020 2020 2020 2066 696c 656e 616d 6520         filename 
-0000e860: 3d20 6622 7b73 7472 286f 705f 7061 7468  = f"{str(op_path
-0000e870: 297d 2f7b 6c65 7474 6572 7d2e 7761 7622  )}/{letter}.wav"
-0000e880: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e890: 2069 6620 5061 7468 2866 696c 656e 616d   if Path(filenam
-0000e8a0: 6529 2e69 735f 6669 6c65 2829 3a0a 2020  e).is_file():.  
-0000e8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e8c0: 2020 6c6f 6767 6572 2e64 6562 7567 2822    logger.debug("
-0000e8d0: 566f 6963 696e 673a 2025 7322 2c20 6669  Voicing: %s", fi
-0000e8e0: 6c65 6e61 6d65 290a 2020 2020 2020 2020  lename).        
-0000e8f0: 2020 2020 2020 2020 2020 2020 6461 7461              data
-0000e900: 2c20 5f66 7320 3d20 7366 2e72 6561 6428  , _fs = sf.read(
-0000e910: 6669 6c65 6e61 6d65 2c20 6474 7970 653d  filename, dtype=
-0000e920: 2266 6c6f 6174 3332 2229 0a20 2020 2020  "float32").     
-0000e930: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-0000e940: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
-0000e950: 2020 2020 2020 2020 2020 2020 7364 2e64              sd.d
-0000e960: 6566 6175 6c74 2e64 6576 6963 6520 3d20  efault.device = 
-0000e970: 7365 6c66 2e70 7265 662e 6765 7428 2273  self.pref.get("s
-0000e980: 6f75 6e64 6465 7669 6365 222c 2022 6465  ounddevice", "de
-0000e990: 6661 756c 7422 290a 2020 2020 2020 2020  fault").        
-0000e9a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e9b0: 7364 2e64 6566 6175 6c74 2e73 616d 706c  sd.default.sampl
-0000e9c0: 6572 6174 6520 3d20 3434 3130 302e 300a  erate = 44100.0.
-0000e9d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e9e0: 2020 2020 2020 2020 7364 2e70 6c61 7928          sd.play(
-0000e9f0: 6461 7461 290a 2020 2020 2020 2020 2020  data).          
-0000ea00: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
-0000ea10: 6767 6572 2e64 6562 7567 2822 2573 222c  gger.debug("%s",
-0000ea20: 2066 227b 7364 2e77 6169 7428 297d 2229   f"{sd.wait()}")
-0000ea30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ea40: 2020 2020 2065 7863 6570 7420 7364 2e50       except sd.P
-0000ea50: 6f72 7441 7564 696f 4572 726f 7220 6173  ortAudioError as
-0000ea60: 2065 7272 3a0a 2020 2020 2020 2020 2020   err:.          
-0000ea70: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
-0000ea80: 6767 6572 2e77 6172 6e69 6e67 2822 2573  gger.warning("%s
-0000ea90: 222c 2066 227b 6572 727d 2229 0a20 2020  ", f"{err}").   
-0000eaa0: 2020 2020 2073 656c 662e 7074 745f 6f66       self.ptt_of
-0000eab0: 6628 290a 0a20 2020 2064 6566 2070 7474  f()..    def ptt
-0000eac0: 5f6f 6e28 7365 6c66 293a 0a20 2020 2020  _on(self):.     
-0000ead0: 2020 2022 2222 7475 726e 206f 6e20 7074     """turn on pt
-0000eae0: 7422 2222 0a20 2020 2020 2020 2069 6620  t""".        if 
-0000eaf0: 7365 6c66 2e72 6967 5f63 6f6e 7472 6f6c  self.rig_control
-0000eb00: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-0000eb10: 6c66 2e6c 6566 7464 6f74 2e73 6574 5069  lf.leftdot.setPi
-0000eb20: 786d 6170 2873 656c 662e 6772 6565 6e64  xmap(self.greend
-0000eb30: 6f74 290a 2020 2020 2020 2020 2020 2020  ot).            
-0000eb40: 6170 702e 7072 6f63 6573 7345 7665 6e74  app.processEvent
-0000eb50: 7328 290a 2020 2020 2020 2020 2020 2020  s().            
-0000eb60: 7365 6c66 2e72 6967 5f63 6f6e 7472 6f6c  self.rig_control
-0000eb70: 2e70 7474 5f6f 6e28 290a 0a20 2020 2064  .ptt_on()..    d
-0000eb80: 6566 2070 7474 5f6f 6666 2873 656c 6629  ef ptt_off(self)
-0000eb90: 3a0a 2020 2020 2020 2020 2222 2274 7572  :.        """tur
-0000eba0: 6e20 6f66 6620 7074 7422 2222 0a20 2020  n off ptt""".   
-0000ebb0: 2020 2020 2069 6620 7365 6c66 2e72 6967       if self.rig
-0000ebc0: 5f63 6f6e 7472 6f6c 3a0a 2020 2020 2020  _control:.      
-0000ebd0: 2020 2020 2020 7365 6c66 2e6c 6566 7464        self.leftd
-0000ebe0: 6f74 2e73 6574 5069 786d 6170 2873 656c  ot.setPixmap(sel
-0000ebf0: 662e 7265 6464 6f74 290a 2020 2020 2020  f.reddot).      
-0000ec00: 2020 2020 2020 6170 702e 7072 6f63 6573        app.proces
-0000ec10: 7345 7665 6e74 7328 290a 2020 2020 2020  sEvents().      
-0000ec20: 2020 2020 2020 7365 6c66 2e72 6967 5f63        self.rig_c
-0000ec30: 6f6e 7472 6f6c 2e70 7474 5f6f 6666 2829  ontrol.ptt_off()
-0000ec40: 0a0a 2020 2020 6465 6620 7365 6e64 6631  ..    def sendf1
-0000ec50: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-0000ec60: 2222 2273 7475 6222 2222 0a20 2020 2020  """stub""".     
-0000ec70: 2020 206c 6f67 6765 722e 6465 6275 6728     logger.debug(
-0000ec80: 2246 3120 436c 6963 6b65 6422 290a 2020  "F1 Clicked").  
-0000ec90: 2020 2020 2020 6966 2073 656c 662e 6e31        if self.n1
-0000eca0: 6d6d 3a0a 2020 2020 2020 2020 2020 2020  mm:.            
-0000ecb0: 7365 6c66 2e6e 316d 6d2e 7261 6469 6f5f  self.n1mm.radio_
-0000ecc0: 696e 666f 5b22 4675 6e63 7469 6f6e 4b65  info["FunctionKe
-0000ecd0: 7943 6170 7469 6f6e 225d 203d 2073 656c  yCaption"] = sel
-0000ece0: 662e 4631 2e74 6578 7428 290a 2020 2020  f.F1.text().    
-0000ecf0: 2020 2020 6966 2073 656c 662e 7261 6469      if self.radi
-0000ed00: 6f5f 7374 6174 652e 6765 7428 226d 6f64  o_state.get("mod
-0000ed10: 6522 2920 696e 205b 224c 5342 222c 2022  e") in ["LSB", "
-0000ed20: 5553 4222 2c20 2253 5342 225d 3a0a 2020  USB", "SSB"]:.  
-0000ed30: 2020 2020 2020 2020 2020 7365 6c66 2e76            self.v
-0000ed40: 6f69 6365 5f73 7472 696e 6728 7365 6c66  oice_string(self
-0000ed50: 2e70 726f 6365 7373 5f6d 6163 726f 2873  .process_macro(s
-0000ed60: 656c 662e 4631 2e74 6f6f 6c54 6970 2829  elf.F1.toolTip()
-0000ed70: 2929 0a20 2020 2020 2020 2020 2020 2072  )).            r
-0000ed80: 6574 7572 6e0a 2020 2020 2020 2020 6966  eturn.        if
-0000ed90: 2073 656c 662e 6377 3a0a 2020 2020 2020   self.cw:.      
-0000eda0: 2020 2020 2020 7365 6c66 2e63 772e 7365        self.cw.se
-0000edb0: 6e64 6377 2873 656c 662e 7072 6f63 6573  ndcw(self.proces
-0000edc0: 735f 6d61 6372 6f28 7365 6c66 2e46 312e  s_macro(self.F1.
-0000edd0: 746f 6f6c 5469 7028 2929 290a 0a20 2020  toolTip()))..   
-0000ede0: 2064 6566 2073 656e 6466 3228 7365 6c66   def sendf2(self
-0000edf0: 293a 0a20 2020 2020 2020 2022 2222 7374  ):.        """st
-0000ee00: 7562 2222 220a 2020 2020 2020 2020 6c6f  ub""".        lo
-0000ee10: 6767 6572 2e64 6562 7567 2822 4632 2043  gger.debug("F2 C
-0000ee20: 6c69 636b 6564 2229 0a20 2020 2020 2020  licked").       
-0000ee30: 2069 6620 7365 6c66 2e6e 316d 6d3a 0a20   if self.n1mm:. 
-0000ee40: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000ee50: 6e31 6d6d 2e72 6164 696f 5f69 6e66 6f5b  n1mm.radio_info[
-0000ee60: 2246 756e 6374 696f 6e4b 6579 4361 7074  "FunctionKeyCapt
-0000ee70: 696f 6e22 5d20 3d20 7365 6c66 2e46 322e  ion"] = self.F2.
-0000ee80: 7465 7874 2829 0a20 2020 2020 2020 2069  text().        i
-0000ee90: 6620 7365 6c66 2e72 6164 696f 5f73 7461  f self.radio_sta
-0000eea0: 7465 2e67 6574 2822 6d6f 6465 2229 2069  te.get("mode") i
-0000eeb0: 6e20 5b22 4c53 4222 2c20 2255 5342 222c  n ["LSB", "USB",
-0000eec0: 2022 5353 4222 5d3a 0a20 2020 2020 2020   "SSB"]:.       
-0000eed0: 2020 2020 2073 656c 662e 766f 6963 655f       self.voice_
-0000eee0: 7374 7269 6e67 2873 656c 662e 7072 6f63  string(self.proc
-0000eef0: 6573 735f 6d61 6372 6f28 7365 6c66 2e46  ess_macro(self.F
-0000ef00: 322e 746f 6f6c 5469 7028 2929 290a 2020  2.toolTip())).  
-0000ef10: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0000ef20: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-0000ef30: 2e63 773a 0a20 2020 2020 2020 2020 2020  .cw:.           
-0000ef40: 2073 656c 662e 6377 2e73 656e 6463 7728   self.cw.sendcw(
-0000ef50: 7365 6c66 2e70 726f 6365 7373 5f6d 6163  self.process_mac
-0000ef60: 726f 2873 656c 662e 4632 2e74 6f6f 6c54  ro(self.F2.toolT
-0000ef70: 6970 2829 2929 0a0a 2020 2020 6465 6620  ip()))..    def 
-0000ef80: 7365 6e64 6633 2873 656c 6629 3a0a 2020  sendf3(self):.  
-0000ef90: 2020 2020 2020 2222 2273 7475 6222 2222        """stub"""
-0000efa0: 0a20 2020 2020 2020 206c 6f67 6765 722e  .        logger.
-0000efb0: 6465 6275 6728 2246 3320 436c 6963 6b65  debug("F3 Clicke
-0000efc0: 6422 290a 2020 2020 2020 2020 6966 2073  d").        if s
-0000efd0: 656c 662e 6e31 6d6d 3a0a 2020 2020 2020  elf.n1mm:.      
-0000efe0: 2020 2020 2020 7365 6c66 2e6e 316d 6d2e        self.n1mm.
-0000eff0: 7261 6469 6f5f 696e 666f 5b22 4675 6e63  radio_info["Func
-0000f000: 7469 6f6e 4b65 7943 6170 7469 6f6e 225d  tionKeyCaption"]
-0000f010: 203d 2073 656c 662e 4633 2e74 6578 7428   = self.F3.text(
-0000f020: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
-0000f030: 662e 7261 6469 6f5f 7374 6174 652e 6765  f.radio_state.ge
-0000f040: 7428 226d 6f64 6522 2920 696e 205b 224c  t("mode") in ["L
-0000f050: 5342 222c 2022 5553 4222 2c20 2253 5342  SB", "USB", "SSB
-0000f060: 225d 3a0a 2020 2020 2020 2020 2020 2020  "]:.            
-0000f070: 7365 6c66 2e76 6f69 6365 5f73 7472 696e  self.voice_strin
-0000f080: 6728 7365 6c66 2e70 726f 6365 7373 5f6d  g(self.process_m
-0000f090: 6163 726f 2873 656c 662e 4633 2e74 6f6f  acro(self.F3.too
-0000f0a0: 6c54 6970 2829 2929 0a20 2020 2020 2020  lTip())).       
-0000f0b0: 2020 2020 2072 6574 7572 6e0a 2020 2020       return.    
-0000f0c0: 2020 2020 6966 2073 656c 662e 6377 3a0a      if self.cw:.
-0000f0d0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000f0e0: 2e63 772e 7365 6e64 6377 2873 656c 662e  .cw.sendcw(self.
-0000f0f0: 7072 6f63 6573 735f 6d61 6372 6f28 7365  process_macro(se
-0000f100: 6c66 2e46 332e 746f 6f6c 5469 7028 2929  lf.F3.toolTip())
-0000f110: 290a 0a20 2020 2064 6566 2073 656e 6466  )..    def sendf
-0000f120: 3428 7365 6c66 293a 0a20 2020 2020 2020  4(self):.       
-0000f130: 2022 2222 7374 7562 2222 220a 2020 2020   """stub""".    
-0000f140: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
-0000f150: 2822 4634 2043 6c69 636b 6564 2229 0a20  ("F4 Clicked"). 
-0000f160: 2020 2020 2020 2069 6620 7365 6c66 2e6e         if self.n
-0000f170: 316d 6d3a 0a20 2020 2020 2020 2020 2020  1mm:.           
-0000f180: 2073 656c 662e 6e31 6d6d 2e72 6164 696f   self.n1mm.radio
-0000f190: 5f69 6e66 6f5b 2246 756e 6374 696f 6e4b  _info["FunctionK
-0000f1a0: 6579 4361 7074 696f 6e22 5d20 3d20 7365  eyCaption"] = se
-0000f1b0: 6c66 2e46 342e 7465 7874 2829 0a20 2020  lf.F4.text().   
-0000f1c0: 2020 2020 2069 6620 7365 6c66 2e72 6164       if self.rad
-0000f1d0: 696f 5f73 7461 7465 2e67 6574 2822 6d6f  io_state.get("mo
-0000f1e0: 6465 2229 2069 6e20 5b22 4c53 4222 2c20  de") in ["LSB", 
-0000f1f0: 2255 5342 222c 2022 5353 4222 5d3a 0a20  "USB", "SSB"]:. 
-0000f200: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000f210: 766f 6963 655f 7374 7269 6e67 2873 656c  voice_string(sel
-0000f220: 662e 7072 6f63 6573 735f 6d61 6372 6f28  f.process_macro(
-0000f230: 7365 6c66 2e46 342e 746f 6f6c 5469 7028  self.F4.toolTip(
-0000f240: 2929 290a 2020 2020 2020 2020 2020 2020  ))).            
-0000f250: 7265 7475 726e 0a20 2020 2020 2020 2069  return.        i
-0000f260: 6620 7365 6c66 2e63 773a 0a20 2020 2020  f self.cw:.     
-0000f270: 2020 2020 2020 2073 656c 662e 6377 2e73         self.cw.s
-0000f280: 656e 6463 7728 7365 6c66 2e70 726f 6365  endcw(self.proce
-0000f290: 7373 5f6d 6163 726f 2873 656c 662e 4634  ss_macro(self.F4
-0000f2a0: 2e74 6f6f 6c54 6970 2829 2929 0a0a 2020  .toolTip()))..  
-0000f2b0: 2020 6465 6620 7365 6e64 6635 2873 656c    def sendf5(sel
-0000f2c0: 6629 3a0a 2020 2020 2020 2020 2222 2273  f):.        """s
-0000f2d0: 7475 6222 2222 0a20 2020 2020 2020 206c  tub""".        l
-0000f2e0: 6f67 6765 722e 6465 6275 6728 2246 3520  ogger.debug("F5 
-0000f2f0: 436c 6963 6b65 6422 290a 2020 2020 2020  Clicked").      
-0000f300: 2020 6966 2073 656c 662e 6e31 6d6d 3a0a    if self.n1mm:.
-0000f310: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000f320: 2e6e 316d 6d2e 7261 6469 6f5f 696e 666f  .n1mm.radio_info
-0000f330: 5b22 4675 6e63 7469 6f6e 4b65 7943 6170  ["FunctionKeyCap
-0000f340: 7469 6f6e 225d 203d 2073 656c 662e 4635  tion"] = self.F5
-0000f350: 2e74 6578 7428 290a 2020 2020 2020 2020  .text().        
-0000f360: 6966 2073 656c 662e 7261 6469 6f5f 7374  if self.radio_st
-0000f370: 6174 652e 6765 7428 226d 6f64 6522 2920  ate.get("mode") 
-0000f380: 696e 205b 224c 5342 222c 2022 5553 4222  in ["LSB", "USB"
-0000f390: 2c20 2253 5342 225d 3a0a 2020 2020 2020  , "SSB"]:.      
-0000f3a0: 2020 2020 2020 7365 6c66 2e76 6f69 6365        self.voice
-0000f3b0: 5f73 7472 696e 6728 7365 6c66 2e70 726f  _string(self.pro
-0000f3c0: 6365 7373 5f6d 6163 726f 2873 656c 662e  cess_macro(self.
-0000f3d0: 4635 2e74 6f6f 6c54 6970 2829 2929 0a20  F5.toolTip())). 
-0000f3e0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-0000f3f0: 6e0a 2020 2020 2020 2020 6966 2073 656c  n.        if sel
-0000f400: 662e 6377 3a0a 2020 2020 2020 2020 2020  f.cw:.          
-0000f410: 2020 7365 6c66 2e63 772e 7365 6e64 6377    self.cw.sendcw
-0000f420: 2873 656c 662e 7072 6f63 6573 735f 6d61  (self.process_ma
-0000f430: 6372 6f28 7365 6c66 2e46 352e 746f 6f6c  cro(self.F5.tool
-0000f440: 5469 7028 2929 290a 0a20 2020 2064 6566  Tip()))..    def
-0000f450: 2073 656e 6466 3628 7365 6c66 293a 0a20   sendf6(self):. 
-0000f460: 2020 2020 2020 2022 2222 7374 7562 2222         """stub""
-0000f470: 220a 2020 2020 2020 2020 6c6f 6767 6572  ".        logger
-0000f480: 2e64 6562 7567 2822 4636 2043 6c69 636b  .debug("F6 Click
-0000f490: 6564 2229 0a20 2020 2020 2020 2069 6620  ed").        if 
-0000f4a0: 7365 6c66 2e6e 316d 6d3a 0a20 2020 2020  self.n1mm:.     
-0000f4b0: 2020 2020 2020 2073 656c 662e 6e31 6d6d         self.n1mm
-0000f4c0: 2e72 6164 696f 5f69 6e66 6f5b 2246 756e  .radio_info["Fun
-0000f4d0: 6374 696f 6e4b 6579 4361 7074 696f 6e22  ctionKeyCaption"
-0000f4e0: 5d20 3d20 7365 6c66 2e46 362e 7465 7874  ] = self.F6.text
-0000f4f0: 2829 0a20 2020 2020 2020 2069 6620 7365  ().        if se
-0000f500: 6c66 2e72 6164 696f 5f73 7461 7465 2e67  lf.radio_state.g
-0000f510: 6574 2822 6d6f 6465 2229 2069 6e20 5b22  et("mode") in ["
-0000f520: 4c53 4222 2c20 2255 5342 222c 2022 5353  LSB", "USB", "SS
-0000f530: 4222 5d3a 0a20 2020 2020 2020 2020 2020  B"]:.           
-0000f540: 2073 656c 662e 766f 6963 655f 7374 7269   self.voice_stri
-0000f550: 6e67 2873 656c 662e 7072 6f63 6573 735f  ng(self.process_
-0000f560: 6d61 6372 6f28 7365 6c66 2e46 362e 746f  macro(self.F6.to
-0000f570: 6f6c 5469 7028 2929 290a 2020 2020 2020  olTip())).      
-0000f580: 2020 2020 2020 7265 7475 726e 0a20 2020        return.   
-0000f590: 2020 2020 2069 6620 7365 6c66 2e63 773a       if self.cw:
-0000f5a0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000f5b0: 662e 6377 2e73 656e 6463 7728 7365 6c66  f.cw.sendcw(self
-0000f5c0: 2e70 726f 6365 7373 5f6d 6163 726f 2873  .process_macro(s
-0000f5d0: 656c 662e 4636 2e74 6f6f 6c54 6970 2829  elf.F6.toolTip()
-0000f5e0: 2929 0a0a 2020 2020 6465 6620 7365 6e64  ))..    def send
-0000f5f0: 6637 2873 656c 6629 3a0a 2020 2020 2020  f7(self):.      
-0000f600: 2020 2222 2273 7475 6222 2222 0a20 2020    """stub""".   
-0000f610: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
-0000f620: 6728 2246 3720 436c 6963 6b65 6422 290a  g("F7 Clicked").
-0000f630: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0000f640: 6e31 6d6d 3a0a 2020 2020 2020 2020 2020  n1mm:.          
-0000f650: 2020 7365 6c66 2e6e 316d 6d2e 7261 6469    self.n1mm.radi
-0000f660: 6f5f 696e 666f 5b22 4675 6e63 7469 6f6e  o_info["Function
-0000f670: 4b65 7943 6170 7469 6f6e 225d 203d 2073  KeyCaption"] = s
-0000f680: 656c 662e 4637 2e74 6578 7428 290a 2020  elf.F7.text().  
-0000f690: 2020 2020 2020 6966 2073 656c 662e 7261        if self.ra
-0000f6a0: 6469 6f5f 7374 6174 652e 6765 7428 226d  dio_state.get("m
-0000f6b0: 6f64 6522 2920 696e 205b 224c 5342 222c  ode") in ["LSB",
-0000f6c0: 2022 5553 4222 2c20 2253 5342 225d 3a0a   "USB", "SSB"]:.
-0000f6d0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000f6e0: 2e76 6f69 6365 5f73 7472 696e 6728 7365  .voice_string(se
-0000f6f0: 6c66 2e70 726f 6365 7373 5f6d 6163 726f  lf.process_macro
-0000f700: 2873 656c 662e 4637 2e74 6f6f 6c54 6970  (self.F7.toolTip
-0000f710: 2829 2929 0a20 2020 2020 2020 2020 2020  ())).           
-0000f720: 2072 6574 7572 6e0a 2020 2020 2020 2020   return.        
-0000f730: 6966 2073 656c 662e 6377 3a0a 2020 2020  if self.cw:.    
-0000f740: 2020 2020 2020 2020 7365 6c66 2e63 772e          self.cw.
-0000f750: 7365 6e64 6377 2873 656c 662e 7072 6f63  sendcw(self.proc
-0000f760: 6573 735f 6d61 6372 6f28 7365 6c66 2e46  ess_macro(self.F
-0000f770: 372e 746f 6f6c 5469 7028 2929 290a 0a20  7.toolTip())).. 
-0000f780: 2020 2064 6566 2073 656e 6466 3828 7365     def sendf8(se
-0000f790: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
-0000f7a0: 7374 7562 2222 220a 2020 2020 2020 2020  stub""".        
-0000f7b0: 6c6f 6767 6572 2e64 6562 7567 2822 4638  logger.debug("F8
-0000f7c0: 2043 6c69 636b 6564 2229 0a20 2020 2020   Clicked").     
-0000f7d0: 2020 2069 6620 7365 6c66 2e6e 316d 6d3a     if self.n1mm:
-0000f7e0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000f7f0: 662e 6e31 6d6d 2e72 6164 696f 5f69 6e66  f.n1mm.radio_inf
-0000f800: 6f5b 2246 756e 6374 696f 6e4b 6579 4361  o["FunctionKeyCa
-0000f810: 7074 696f 6e22 5d20 3d20 7365 6c66 2e46  ption"] = self.F
-0000f820: 382e 7465 7874 2829 0a20 2020 2020 2020  8.text().       
-0000f830: 2069 6620 7365 6c66 2e72 6164 696f 5f73   if self.radio_s
-0000f840: 7461 7465 2e67 6574 2822 6d6f 6465 2229  tate.get("mode")
-0000f850: 2069 6e20 5b22 4c53 4222 2c20 2255 5342   in ["LSB", "USB
-0000f860: 222c 2022 5353 4222 5d3a 0a20 2020 2020  ", "SSB"]:.     
-0000f870: 2020 2020 2020 2073 656c 662e 766f 6963         self.voic
-0000f880: 655f 7374 7269 6e67 2873 656c 662e 7072  e_string(self.pr
-0000f890: 6f63 6573 735f 6d61 6372 6f28 7365 6c66  ocess_macro(self
-0000f8a0: 2e46 382e 746f 6f6c 5469 7028 2929 290a  .F8.toolTip())).
-0000f8b0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0000f8c0: 726e 0a20 2020 2020 2020 2069 6620 7365  rn.        if se
-0000f8d0: 6c66 2e63 773a 0a20 2020 2020 2020 2020  lf.cw:.         
-0000f8e0: 2020 2073 656c 662e 6377 2e73 656e 6463     self.cw.sendc
-0000f8f0: 7728 7365 6c66 2e70 726f 6365 7373 5f6d  w(self.process_m
-0000f900: 6163 726f 2873 656c 662e 4638 2e74 6f6f  acro(self.F8.too
-0000f910: 6c54 6970 2829 2929 0a0a 2020 2020 6465  lTip()))..    de
-0000f920: 6620 7365 6e64 6639 2873 656c 6629 3a0a  f sendf9(self):.
-0000f930: 2020 2020 2020 2020 2222 2273 7475 6222          """stub"
-0000f940: 2222 0a20 2020 2020 2020 206c 6f67 6765  "".        logge
-0000f950: 722e 6465 6275 6728 2246 3920 436c 6963  r.debug("F9 Clic
-0000f960: 6b65 6422 290a 2020 2020 2020 2020 6966  ked").        if
-0000f970: 2073 656c 662e 6e31 6d6d 3a0a 2020 2020   self.n1mm:.    
-0000f980: 2020 2020 2020 2020 7365 6c66 2e6e 316d          self.n1m
-0000f990: 6d2e 7261 6469 6f5f 696e 666f 5b22 4675  m.radio_info["Fu
-0000f9a0: 6e63 7469 6f6e 4b65 7943 6170 7469 6f6e  nctionKeyCaption
-0000f9b0: 225d 203d 2073 656c 662e 4639 2e74 6578  "] = self.F9.tex
-0000f9c0: 7428 290a 2020 2020 2020 2020 6966 2073  t().        if s
-0000f9d0: 656c 662e 7261 6469 6f5f 7374 6174 652e  elf.radio_state.
-0000f9e0: 6765 7428 226d 6f64 6522 2920 696e 205b  get("mode") in [
-0000f9f0: 224c 5342 222c 2022 5553 4222 2c20 2253  "LSB", "USB", "S
-0000fa00: 5342 225d 3a0a 2020 2020 2020 2020 2020  SB"]:.          
-0000fa10: 2020 7365 6c66 2e76 6f69 6365 5f73 7472    self.voice_str
-0000fa20: 696e 6728 7365 6c66 2e70 726f 6365 7373  ing(self.process
-0000fa30: 5f6d 6163 726f 2873 656c 662e 4639 2e74  _macro(self.F9.t
-0000fa40: 6f6f 6c54 6970 2829 2929 0a20 2020 2020  oolTip())).     
-0000fa50: 2020 2020 2020 2072 6574 7572 6e0a 2020         return.  
-0000fa60: 2020 2020 2020 6966 2073 656c 662e 6377        if self.cw
-0000fa70: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-0000fa80: 6c66 2e63 772e 7365 6e64 6377 2873 656c  lf.cw.sendcw(sel
-0000fa90: 662e 7072 6f63 6573 735f 6d61 6372 6f28  f.process_macro(
-0000faa0: 7365 6c66 2e46 392e 746f 6f6c 5469 7028  self.F9.toolTip(
-0000fab0: 2929 290a 0a20 2020 2064 6566 2073 656e  )))..    def sen
-0000fac0: 6466 3130 2873 656c 6629 3a0a 2020 2020  df10(self):.    
-0000fad0: 2020 2020 2222 2273 7475 6222 2222 0a20      """stub""". 
-0000fae0: 2020 2020 2020 206c 6f67 6765 722e 6465         logger.de
-0000faf0: 6275 6728 2246 3130 2043 6c69 636b 6564  bug("F10 Clicked
-0000fb00: 2229 0a20 2020 2020 2020 2069 6620 7365  ").        if se
-0000fb10: 6c66 2e6e 316d 6d3a 0a20 2020 2020 2020  lf.n1mm:.       
-0000fb20: 2020 2020 2073 656c 662e 6e31 6d6d 2e72       self.n1mm.r
-0000fb30: 6164 696f 5f69 6e66 6f5b 2246 756e 6374  adio_info["Funct
-0000fb40: 696f 6e4b 6579 4361 7074 696f 6e22 5d20  ionKeyCaption"] 
-0000fb50: 3d20 7365 6c66 2e46 3130 2e74 6578 7428  = self.F10.text(
-0000fb60: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
-0000fb70: 662e 7261 6469 6f5f 7374 6174 652e 6765  f.radio_state.ge
-0000fb80: 7428 226d 6f64 6522 2920 696e 205b 224c  t("mode") in ["L
-0000fb90: 5342 222c 2022 5553 4222 2c20 2253 5342  SB", "USB", "SSB
-0000fba0: 225d 3a0a 2020 2020 2020 2020 2020 2020  "]:.            
-0000fbb0: 7365 6c66 2e76 6f69 6365 5f73 7472 696e  self.voice_strin
-0000fbc0: 6728 7365 6c66 2e70 726f 6365 7373 5f6d  g(self.process_m
-0000fbd0: 6163 726f 2873 656c 662e 4631 302e 746f  acro(self.F10.to
-0000fbe0: 6f6c 5469 7028 2929 290a 2020 2020 2020  olTip())).      
-0000fbf0: 2020 2020 2020 7265 7475 726e 0a20 2020        return.   
-0000fc00: 2020 2020 2069 6620 7365 6c66 2e63 773a       if self.cw:
-0000fc10: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000fc20: 662e 6377 2e73 656e 6463 7728 7365 6c66  f.cw.sendcw(self
-0000fc30: 2e70 726f 6365 7373 5f6d 6163 726f 2873  .process_macro(s
-0000fc40: 656c 662e 4631 302e 746f 6f6c 5469 7028  elf.F10.toolTip(
-0000fc50: 2929 290a 0a20 2020 2064 6566 2073 656e  )))..    def sen
-0000fc60: 6466 3131 2873 656c 6629 3a0a 2020 2020  df11(self):.    
-0000fc70: 2020 2020 2222 2273 7475 6222 2222 0a20      """stub""". 
-0000fc80: 2020 2020 2020 206c 6f67 6765 722e 6465         logger.de
-0000fc90: 6275 6728 2246 3131 2043 6c69 636b 6564  bug("F11 Clicked
-0000fca0: 2229 0a20 2020 2020 2020 2069 6620 7365  ").        if se
-0000fcb0: 6c66 2e6e 316d 6d3a 0a20 2020 2020 2020  lf.n1mm:.       
-0000fcc0: 2020 2020 2073 656c 662e 6e31 6d6d 2e72       self.n1mm.r
-0000fcd0: 6164 696f 5f69 6e66 6f5b 2246 756e 6374  adio_info["Funct
-0000fce0: 696f 6e4b 6579 4361 7074 696f 6e22 5d20  ionKeyCaption"] 
-0000fcf0: 3d20 7365 6c66 2e46 3131 2e74 6578 7428  = self.F11.text(
-0000fd00: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
-0000fd10: 662e 7261 6469 6f5f 7374 6174 652e 6765  f.radio_state.ge
-0000fd20: 7428 226d 6f64 6522 2920 696e 205b 224c  t("mode") in ["L
-0000fd30: 5342 222c 2022 5553 4222 2c20 2253 5342  SB", "USB", "SSB
-0000fd40: 225d 3a0a 2020 2020 2020 2020 2020 2020  "]:.            
-0000fd50: 7365 6c66 2e76 6f69 6365 5f73 7472 696e  self.voice_strin
-0000fd60: 6728 7365 6c66 2e70 726f 6365 7373 5f6d  g(self.process_m
-0000fd70: 6163 726f 2873 656c 662e 4631 312e 746f  acro(self.F11.to
-0000fd80: 6f6c 5469 7028 2929 290a 2020 2020 2020  olTip())).      
-0000fd90: 2020 2020 2020 7265 7475 726e 0a20 2020        return.   
-0000fda0: 2020 2020 2069 6620 7365 6c66 2e63 773a       if self.cw:
-0000fdb0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000fdc0: 662e 6377 2e73 656e 6463 7728 7365 6c66  f.cw.sendcw(self
-0000fdd0: 2e70 726f 6365 7373 5f6d 6163 726f 2873  .process_macro(s
-0000fde0: 656c 662e 4631 312e 746f 6f6c 5469 7028  elf.F11.toolTip(
-0000fdf0: 2929 290a 0a20 2020 2064 6566 2073 656e  )))..    def sen
-0000fe00: 6466 3132 2873 656c 6629 3a0a 2020 2020  df12(self):.    
-0000fe10: 2020 2020 2222 2273 7475 6222 2222 0a20      """stub""". 
-0000fe20: 2020 2020 2020 206c 6f67 6765 722e 6465         logger.de
-0000fe30: 6275 6728 2246 3132 2043 6c69 636b 6564  bug("F12 Clicked
-0000fe40: 2229 0a20 2020 2020 2020 2069 6620 7365  ").        if se
-0000fe50: 6c66 2e6e 316d 6d3a 0a20 2020 2020 2020  lf.n1mm:.       
-0000fe60: 2020 2020 2073 656c 662e 6e31 6d6d 2e72       self.n1mm.r
-0000fe70: 6164 696f 5f69 6e66 6f5b 2246 756e 6374  adio_info["Funct
-0000fe80: 696f 6e4b 6579 4361 7074 696f 6e22 5d20  ionKeyCaption"] 
-0000fe90: 3d20 7365 6c66 2e46 3132 2e74 6578 7428  = self.F12.text(
-0000fea0: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
-0000feb0: 662e 7261 6469 6f5f 7374 6174 652e 6765  f.radio_state.ge
-0000fec0: 7428 226d 6f64 6522 2920 696e 205b 224c  t("mode") in ["L
-0000fed0: 5342 222c 2022 5553 4222 2c20 2253 5342  SB", "USB", "SSB
-0000fee0: 225d 3a0a 2020 2020 2020 2020 2020 2020  "]:.            
-0000fef0: 7365 6c66 2e76 6f69 6365 5f73 7472 696e  self.voice_strin
-0000ff00: 6728 7365 6c66 2e70 726f 6365 7373 5f6d  g(self.process_m
-0000ff10: 6163 726f 2873 656c 662e 4631 322e 746f  acro(self.F12.to
-0000ff20: 6f6c 5469 7028 2929 290a 2020 2020 2020  olTip())).      
-0000ff30: 2020 2020 2020 7265 7475 726e 0a20 2020        return.   
-0000ff40: 2020 2020 2069 6620 7365 6c66 2e63 773a       if self.cw:
-0000ff50: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000ff60: 662e 6377 2e73 656e 6463 7728 7365 6c66  f.cw.sendcw(self
-0000ff70: 2e70 726f 6365 7373 5f6d 6163 726f 2873  .process_macro(s
-0000ff80: 656c 662e 4631 322e 746f 6f6c 5469 7028  elf.F12.toolTip(
-0000ff90: 2929 290a 0a20 2020 2064 6566 2072 756e  )))..    def run
-0000ffa0: 5f73 705f 6275 7474 6f6e 735f 636c 6963  _sp_buttons_clic
-0000ffb0: 6b65 6428 7365 6c66 293a 0a20 2020 2020  ked(self):.     
-0000ffc0: 2020 2022 2222 4861 6e64 6c65 2072 756e     """Handle run
-0000ffd0: 2f73 2670 206d 6f64 6522 2222 0a20 2020  /s&p mode""".   
-0000ffe0: 2020 2020 2073 656c 662e 7072 6566 5b22       self.pref["
-0000fff0: 7275 6e5f 7374 6174 6522 5d20 3d20 7365  run_state"] = se
-00010000: 6c66 2e72 6164 696f 4275 7474 6f6e 5f72  lf.radioButton_r
-00010010: 756e 2e69 7343 6865 636b 6564 2829 0a20  un.isChecked(). 
-00010020: 2020 2020 2020 2073 656c 662e 7772 6974         self.writ
-00010030: 655f 7072 6566 6572 656e 6365 2829 0a20  e_preference(). 
-00010040: 2020 2020 2020 2073 656c 662e 7265 6164         self.read
-00010050: 5f63 775f 6d61 6372 6f73 2829 0a0a 2020  _cw_macros()..  
-00010060: 2020 6465 6620 7772 6974 655f 7072 6566    def write_pref
-00010070: 6572 656e 6365 2873 656c 6629 3a0a 2020  erence(self):.  
-00010080: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00010090: 2020 5772 6974 6520 7072 6566 6572 656e    Write preferen
-000100a0: 6365 7320 746f 206a 736f 6e20 6669 6c65  ces to json file
-000100b0: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
-000100c0: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
-000100d0: 2020 2020 2020 2077 6974 6820 6f70 656e         with open
-000100e0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-000100f0: 2020 434f 4e46 4947 5f50 4154 4820 2b20    CONFIG_PATH + 
-00010100: 222f 6e6f 7431 6d6d 2e6a 736f 6e22 2c20  "/not1mm.json", 
-00010110: 2277 7422 2c20 656e 636f 6469 6e67 3d22  "wt", encoding="
-00010120: 7574 662d 3822 0a20 2020 2020 2020 2020  utf-8".         
-00010130: 2020 2029 2061 7320 6669 6c65 5f64 6573     ) as file_des
-00010140: 6372 6970 746f 723a 0a20 2020 2020 2020  criptor:.       
-00010150: 2020 2020 2020 2020 2066 696c 655f 6465           file_de
-00010160: 7363 7269 7074 6f72 2e77 7269 7465 2864  scriptor.write(d
-00010170: 756d 7073 2873 656c 662e 7072 6566 2c20  umps(self.pref, 
-00010180: 696e 6465 6e74 3d34 2929 0a20 2020 2020  indent=4)).     
-00010190: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
-000101a0: 722e 696e 666f 2822 7772 6974 696e 673a  r.info("writing:
-000101b0: 2025 7322 2c20 7365 6c66 2e70 7265 6629   %s", self.pref)
-000101c0: 0a20 2020 2020 2020 2065 7863 6570 7420  .        except 
-000101d0: 494f 4572 726f 7220 6173 2065 7863 6570  IOError as excep
-000101e0: 7469 6f6e 3a0a 2020 2020 2020 2020 2020  tion:.          
-000101f0: 2020 6c6f 6767 6572 2e63 7269 7469 6361    logger.critica
-00010200: 6c28 2277 7269 7465 7072 6566 6572 656e  l("writepreferen
-00010210: 6365 733a 2025 7322 2c20 6578 6365 7074  ces: %s", except
-00010220: 696f 6e29 0a0a 2020 2020 6465 6620 7265  ion)..    def re
-00010230: 6164 7072 6566 6572 656e 6365 7328 7365  adpreferences(se
-00010240: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
-00010250: 0a20 2020 2020 2020 2052 6573 746f 7265  .        Restore
-00010260: 2070 7265 6665 7265 6e63 6573 2069 6620   preferences if 
-00010270: 7468 6579 2065 7869 7374 2c20 6f74 6865  they exist, othe
-00010280: 7277 6973 6520 6372 6561 7465 2073 6f6d  rwise create som
-00010290: 6520 7361 6e65 2064 6566 6175 6c74 732e  e sane defaults.
-000102a0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-000102b0: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
-000102c0: 2020 2020 2020 6966 206f 732e 7061 7468        if os.path
-000102d0: 2e65 7869 7374 7328 434f 4e46 4947 5f50  .exists(CONFIG_P
-000102e0: 4154 4820 2b20 222f 6e6f 7431 6d6d 2e6a  ATH + "/not1mm.j
-000102f0: 736f 6e22 293a 0a20 2020 2020 2020 2020  son"):.         
-00010300: 2020 2020 2020 2077 6974 6820 6f70 656e         with open
-00010310: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00010320: 2020 2020 2020 434f 4e46 4947 5f50 4154        CONFIG_PAT
-00010330: 4820 2b20 222f 6e6f 7431 6d6d 2e6a 736f  H + "/not1mm.jso
-00010340: 6e22 2c20 2272 7422 2c20 656e 636f 6469  n", "rt", encodi
-00010350: 6e67 3d22 7574 662d 3822 0a20 2020 2020  ng="utf-8".     
-00010360: 2020 2020 2020 2020 2020 2029 2061 7320             ) as 
-00010370: 6669 6c65 5f64 6573 6372 6970 746f 723a  file_descriptor:
-00010380: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010390: 2020 2020 2073 656c 662e 7072 6566 203d       self.pref =
-000103a0: 206c 6f61 6473 2866 696c 655f 6465 7363   loads(file_desc
-000103b0: 7269 7074 6f72 2e72 6561 6428 2929 0a20  riptor.read()). 
-000103c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000103d0: 2020 206c 6f67 6765 722e 696e 666f 2822     logger.info("
-000103e0: 2573 222c 2073 656c 662e 7072 6566 290a  %s", self.pref).
-000103f0: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00010400: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00010410: 2020 6c6f 6767 6572 2e69 6e66 6f28 224e    logger.info("N
-00010420: 6f20 7072 6566 6572 656e 6365 2066 696c  o preference fil
-00010430: 652e 2057 7269 7469 6e67 2070 7265 6665  e. Writing prefe
-00010440: 7265 6e63 652e 2229 0a20 2020 2020 2020  rence.").       
-00010450: 2020 2020 2020 2020 2077 6974 6820 6f70           with op
-00010460: 656e 280a 2020 2020 2020 2020 2020 2020  en(.            
-00010470: 2020 2020 2020 2020 434f 4e46 4947 5f50          CONFIG_P
-00010480: 4154 4820 2b20 222f 6e6f 7431 6d6d 2e6a  ATH + "/not1mm.j
-00010490: 736f 6e22 2c20 2277 7422 2c20 656e 636f  son", "wt", enco
-000104a0: 6469 6e67 3d22 7574 662d 3822 0a20 2020  ding="utf-8".   
-000104b0: 2020 2020 2020 2020 2020 2020 2029 2061               ) a
-000104c0: 7320 6669 6c65 5f64 6573 6372 6970 746f  s file_descripto
-000104d0: 723a 0a20 2020 2020 2020 2020 2020 2020  r:.             
-000104e0: 2020 2020 2020 2073 656c 662e 7072 6566         self.pref
-000104f0: 203d 2073 656c 662e 7072 6566 5f72 6566   = self.pref_ref
-00010500: 2e63 6f70 7928 290a 2020 2020 2020 2020  .copy().        
-00010510: 2020 2020 2020 2020 2020 2020 6669 6c65              file
-00010520: 5f64 6573 6372 6970 746f 722e 7772 6974  _descriptor.writ
-00010530: 6528 6475 6d70 7328 7365 6c66 2e70 7265  e(dumps(self.pre
-00010540: 662c 2069 6e64 656e 743d 3429 290a 2020  f, indent=4)).  
-00010550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010560: 2020 6c6f 6767 6572 2e69 6e66 6f28 2225    logger.info("%
-00010570: 7322 2c20 7365 6c66 2e70 7265 6629 0a20  s", self.pref). 
-00010580: 2020 2020 2020 2065 7863 6570 7420 494f         except IO
-00010590: 4572 726f 7220 6173 2065 7863 6570 7469  Error as excepti
-000105a0: 6f6e 3a0a 2020 2020 2020 2020 2020 2020  on:.            
-000105b0: 6c6f 6767 6572 2e63 7269 7469 6361 6c28  logger.critical(
-000105c0: 2245 7272 6f72 3a20 2573 222c 2065 7863  "Error: %s", exc
-000105d0: 6570 7469 6f6e 290a 0a20 2020 2020 2020  eption)..       
-000105e0: 2073 656c 662e 6c6f 6f6b 5f75 7020 3d20   self.look_up = 
-000105f0: 4e6f 6e65 0a20 2020 2020 2020 2069 6620  None.        if 
-00010600: 7365 6c66 2e70 7265 662e 6765 7428 2275  self.pref.get("u
-00010610: 7365 7172 7a22 293a 0a20 2020 2020 2020  seqrz"):.       
-00010620: 2020 2020 2073 656c 662e 6c6f 6f6b 5f75       self.look_u
-00010630: 7020 3d20 5152 5a6c 6f6f 6b75 7028 0a20  p = QRZlookup(. 
-00010640: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00010650: 656c 662e 7072 6566 2e67 6574 2822 6c6f  elf.pref.get("lo
-00010660: 6f6b 7570 7573 6572 6e61 6d65 2229 2c0a  okupusername"),.
-00010670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010680: 7365 6c66 2e70 7265 662e 6765 7428 226c  self.pref.get("l
-00010690: 6f6f 6b75 7070 6173 7377 6f72 6422 292c  ookuppassword"),
-000106a0: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
-000106b0: 2020 2020 2020 2023 2069 6620 7365 6c66         # if self
-000106c0: 2e70 7265 662e 6765 7428 2275 7365 6861  .pref.get("useha
-000106d0: 6d64 6222 293a 0a20 2020 2020 2020 2023  mdb"):.        #
-000106e0: 2020 2020 2073 656c 662e 6c6f 6f6b 5f75       self.look_u
-000106f0: 7020 3d20 4861 6d44 426c 6f6f 6b75 7028  p = HamDBlookup(
-00010700: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
-00010710: 662e 7072 6566 2e67 6574 2822 7573 6568  f.pref.get("useh
-00010720: 616d 7174 6822 293a 0a20 2020 2020 2020  amqth"):.       
-00010730: 2020 2020 2073 656c 662e 6c6f 6f6b 5f75       self.look_u
-00010740: 7020 3d20 4861 6d51 5448 280a 2020 2020  p = HamQTH(.    
-00010750: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00010760: 2e70 7265 662e 6765 7428 226c 6f6f 6b75  .pref.get("looku
-00010770: 7075 7365 726e 616d 6522 292c 0a20 2020  pusername"),.   
-00010780: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00010790: 662e 7072 6566 2e67 6574 2822 6c6f 6f6b  f.pref.get("look
-000107a0: 7570 7061 7373 776f 7264 2229 2c0a 2020  uppassword"),.  
-000107b0: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
-000107c0: 2020 2020 2069 6620 7365 6c66 2e70 7265       if self.pre
-000107d0: 662e 6765 7428 2272 756e 5f73 7461 7465  f.get("run_state
-000107e0: 2229 3a0a 2020 2020 2020 2020 2020 2020  "):.            
-000107f0: 7365 6c66 2e72 6164 696f 4275 7474 6f6e  self.radioButton
-00010800: 5f72 756e 2e73 6574 4368 6563 6b65 6428  _run.setChecked(
-00010810: 5472 7565 290a 2020 2020 2020 2020 656c  True).        el
-00010820: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00010830: 7365 6c66 2e72 6164 696f 4275 7474 6f6e  self.radioButton
-00010840: 5f73 702e 7365 7443 6865 636b 6564 2854  _sp.setChecked(T
-00010850: 7275 6529 0a0a 2020 2020 2020 2020 6966  rue)..        if
-00010860: 2073 656c 662e 7072 6566 2e67 6574 2822   self.pref.get("
-00010870: 636f 6d6d 616e 645f 6275 7474 6f6e 7322  command_buttons"
-00010880: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
-00010890: 656c 662e 6163 7469 6f6e 436f 6d6d 616e  elf.actionComman
-000108a0: 645f 4275 7474 6f6e 732e 7365 7443 6865  d_Buttons.setChe
-000108b0: 636b 6564 2854 7275 6529 0a20 2020 2020  cked(True).     
-000108c0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-000108d0: 2020 2020 2073 656c 662e 6163 7469 6f6e       self.action
-000108e0: 436f 6d6d 616e 645f 4275 7474 6f6e 732e  Command_Buttons.
-000108f0: 7365 7443 6865 636b 6564 2846 616c 7365  setChecked(False
-00010900: 290a 0a20 2020 2020 2020 2069 6620 7365  )..        if se
-00010910: 6c66 2e70 7265 662e 6765 7428 2263 775f  lf.pref.get("cw_
-00010920: 6d61 6372 6f73 2229 3a0a 2020 2020 2020  macros"):.      
-00010930: 2020 2020 2020 7365 6c66 2e61 6374 696f        self.actio
-00010940: 6e43 575f 4d61 6372 6f73 2e73 6574 4368  nCW_Macros.setCh
-00010950: 6563 6b65 6428 5472 7565 290a 2020 2020  ecked(True).    
-00010960: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00010970: 2020 2020 2020 7365 6c66 2e61 6374 696f        self.actio
-00010980: 6e43 575f 4d61 6372 6f73 2e73 6574 4368  nCW_Macros.setCh
-00010990: 6563 6b65 6428 4661 6c73 6529 0a0a 2020  ecked(False)..  
-000109a0: 2020 2020 2020 6966 2073 656c 662e 7072        if self.pr
-000109b0: 6566 2e67 6574 2822 6261 6e64 735f 6d6f  ef.get("bands_mo
-000109c0: 6465 7322 293a 0a20 2020 2020 2020 2020  des"):.         
-000109d0: 2020 2073 656c 662e 6163 7469 6f6e 4d6f     self.actionMo
-000109e0: 6465 5f61 6e64 5f42 616e 6473 2e73 6574  de_and_Bands.set
-000109f0: 4368 6563 6b65 6428 5472 7565 290a 2020  Checked(True).  
-00010a00: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00010a10: 2020 2020 2020 2020 7365 6c66 2e61 6374          self.act
-00010a20: 696f 6e4d 6f64 655f 616e 645f 4261 6e64  ionMode_and_Band
-00010a30: 732e 7365 7443 6865 636b 6564 2846 616c  s.setChecked(Fal
-00010a40: 7365 290a 0a20 2020 2020 2020 206d 756c  se)..        mul
-00010a50: 7469 6361 7374 5f67 726f 7570 203d 2073  ticast_group = s
-00010a60: 656c 662e 7072 6566 2e67 6574 2822 6d75  elf.pref.get("mu
-00010a70: 6c74 6963 6173 745f 6772 6f75 7022 2c20  lticast_group", 
-00010a80: 2232 3339 2e31 2e31 2e31 2229 0a20 2020  "239.1.1.1").   
-00010a90: 2020 2020 206d 756c 7469 6361 7374 5f70       multicast_p
-00010aa0: 6f72 7420 3d20 7365 6c66 2e70 7265 662e  ort = self.pref.
-00010ab0: 6765 7428 226d 756c 7469 6361 7374 5f70  get("multicast_p
-00010ac0: 6f72 7422 2c20 3232 3339 290a 2020 2020  ort", 2239).    
-00010ad0: 2020 2020 696e 7465 7266 6163 655f 6970      interface_ip
-00010ae0: 203d 2073 656c 662e 7072 6566 2e67 6574   = self.pref.get
-00010af0: 2822 696e 7465 7266 6163 655f 6970 222c  ("interface_ip",
-00010b00: 2022 302e 302e 302e 3022 290a 2020 2020   "0.0.0.0").    
-00010b10: 2020 2020 7365 6c66 2e6d 756c 7469 6361      self.multica
-00010b20: 7374 5f69 6e74 6572 6661 6365 203d 204d  st_interface = M
-00010b30: 756c 7469 6361 7374 280a 2020 2020 2020  ulticast(.      
-00010b40: 2020 2020 2020 6d75 6c74 6963 6173 745f        multicast_
-00010b50: 6772 6f75 702c 206d 756c 7469 6361 7374  group, multicast
-00010b60: 5f70 6f72 742c 2069 6e74 6572 6661 6365  _port, interface
-00010b70: 5f69 700a 2020 2020 2020 2020 290a 2020  _ip.        ).  
-00010b80: 2020 2020 2020 7365 6c66 2e6d 756c 7469        self.multi
-00010b90: 6361 7374 5f69 6e74 6572 6661 6365 2e72  cast_interface.r
-00010ba0: 6561 6479 5f72 6561 645f 636f 6e6e 6563  eady_read_connec
-00010bb0: 7428 7365 6c66 2e77 6174 6368 5f75 6470  t(self.watch_udp
-00010bc0: 290a 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00010bd0: 7269 675f 636f 6e74 726f 6c20 3d20 4e6f  rig_control = No
-00010be0: 6e65 0a0a 2020 2020 2020 2020 6966 2073  ne..        if s
-00010bf0: 656c 662e 7072 6566 2e67 6574 2822 7573  elf.pref.get("us
-00010c00: 6566 6c72 6967 222c 2046 616c 7365 293a  eflrig", False):
-00010c10: 0a20 2020 2020 2020 2020 2020 206c 6f67  .            log
-00010c20: 6765 722e 6465 6275 6728 0a20 2020 2020  ger.debug(.     
-00010c30: 2020 2020 2020 2020 2020 2022 5573 696e             "Usin
-00010c40: 6720 666c 7269 673a 2025 7322 2c0a 2020  g flrig: %s",.  
-00010c50: 2020 2020 2020 2020 2020 2020 2020 6622                f"
-00010c60: 7b73 656c 662e 7072 6566 2e67 6574 2827  {self.pref.get('
-00010c70: 4341 545f 6970 2729 7d20 7b73 656c 662e  CAT_ip')} {self.
-00010c80: 7072 6566 2e67 6574 2827 4341 545f 706f  pref.get('CAT_po
-00010c90: 7274 2729 7d22 2c0a 2020 2020 2020 2020  rt')}",.        
-00010ca0: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-00010cb0: 2020 7365 6c66 2e72 6967 5f63 6f6e 7472    self.rig_contr
-00010cc0: 6f6c 203d 2043 4154 280a 2020 2020 2020  ol = CAT(.      
-00010cd0: 2020 2020 2020 2020 2020 2266 6c72 6967            "flrig
-00010ce0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00010cf0: 2020 2073 656c 662e 7072 6566 2e67 6574     self.pref.get
-00010d00: 2822 4341 545f 6970 222c 2022 3132 372e  ("CAT_ip", "127.
-00010d10: 302e 302e 3122 292c 0a20 2020 2020 2020  0.0.1"),.       
-00010d20: 2020 2020 2020 2020 2069 6e74 2873 656c           int(sel
-00010d30: 662e 7072 6566 2e67 6574 2822 4341 545f  f.pref.get("CAT_
-00010d40: 706f 7274 222c 2031 3233 3435 2929 2c0a  port", 12345)),.
-00010d50: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-00010d60: 2020 2020 2020 6966 2073 656c 662e 7072        if self.pr
-00010d70: 6566 2e67 6574 2822 7573 6572 6967 6374  ef.get("userigct
-00010d80: 6c64 222c 2046 616c 7365 293a 0a20 2020  ld", False):.   
-00010d90: 2020 2020 2020 2020 206c 6f67 6765 722e           logger.
-00010da0: 6465 6275 6728 0a20 2020 2020 2020 2020  debug(.         
-00010db0: 2020 2020 2020 2022 5573 696e 6720 7269         "Using ri
-00010dc0: 6763 746c 643a 2025 7322 2c0a 2020 2020  gctld: %s",.    
-00010dd0: 2020 2020 2020 2020 2020 2020 6622 7b73              f"{s
-00010de0: 656c 662e 7072 6566 2e67 6574 2827 4341  elf.pref.get('CA
-00010df0: 545f 6970 2729 7d20 7b73 656c 662e 7072  T_ip')} {self.pr
-00010e00: 6566 2e67 6574 2827 4341 545f 706f 7274  ef.get('CAT_port
-00010e10: 2729 7d22 2c0a 2020 2020 2020 2020 2020  ')}",.          
-00010e20: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
-00010e30: 7365 6c66 2e72 6967 5f63 6f6e 7472 6f6c  self.rig_control
-00010e40: 203d 2043 4154 280a 2020 2020 2020 2020   = CAT(.        
-00010e50: 2020 2020 2020 2020 2272 6967 6374 6c64          "rigctld
-00010e60: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00010e70: 2020 2073 656c 662e 7072 6566 2e67 6574     self.pref.get
-00010e80: 2822 4341 545f 6970 222c 2022 3132 372e  ("CAT_ip", "127.
-00010e90: 302e 302e 3122 292c 0a20 2020 2020 2020  0.0.1"),.       
-00010ea0: 2020 2020 2020 2020 2069 6e74 2873 656c           int(sel
-00010eb0: 662e 7072 6566 2e67 6574 2822 4341 545f  f.pref.get("CAT_
-00010ec0: 706f 7274 222c 2034 3533 3229 292c 0a20  port", 4532)),. 
-00010ed0: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
-00010ee0: 2020 2020 2020 6966 2073 656c 662e 7072        if self.pr
-00010ef0: 6566 2e67 6574 2822 6377 7479 7065 222c  ef.get("cwtype",
-00010f00: 2030 2920 3d3d 2030 3a0a 2020 2020 2020   0) == 0:.      
-00010f10: 2020 2020 2020 7365 6c66 2e63 7720 3d20        self.cw = 
-00010f20: 4e6f 6e65 0a20 2020 2020 2020 2065 6c73  None.        els
-00010f30: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-00010f40: 656c 662e 6377 203d 2043 5728 0a20 2020  elf.cw = CW(.   
-00010f50: 2020 2020 2020 2020 2020 2020 2069 6e74               int
-00010f60: 2873 656c 662e 7072 6566 2e67 6574 2822  (self.pref.get("
-00010f70: 6377 7479 7065 2229 292c 0a20 2020 2020  cwtype")),.     
-00010f80: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00010f90: 7072 6566 2e67 6574 2822 6377 6970 2229  pref.get("cwip")
-00010fa0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00010fb0: 2020 696e 7428 7365 6c66 2e70 7265 662e    int(self.pref.
-00010fc0: 6765 7428 2263 7770 6f72 7422 2c20 3637  get("cwport", 67
-00010fd0: 3839 2929 2c0a 2020 2020 2020 2020 2020  89)),.          
-00010fe0: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
-00010ff0: 7365 6c66 2e63 772e 7370 6565 6420 3d20  self.cw.speed = 
-00011000: 3230 0a20 2020 2020 2020 2020 2020 2069  20.            i
-00011010: 6620 7365 6c66 2e63 772e 7365 7276 6572  f self.cw.server
-00011020: 7479 7065 203d 3d20 323a 0a20 2020 2020  type == 2:.     
-00011030: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00011040: 6377 2e73 6574 5f77 696e 6b65 7965 725f  cw.set_winkeyer_
-00011050: 7370 6565 6428 3230 290a 0a20 2020 2020  speed(20)..     
-00011060: 2020 2073 656c 662e 6e31 6d6d 203d 204e     self.n1mm = N
-00011070: 6f6e 650a 2020 2020 2020 2020 6966 2073  one.        if s
-00011080: 656c 662e 7072 6566 2e67 6574 2822 7365  elf.pref.get("se
-00011090: 6e64 5f6e 316d 6d5f 7061 636b 6574 7322  nd_n1mm_packets"
-000110a0: 2c20 4661 6c73 6529 3a0a 2020 2020 2020  , False):.      
-000110b0: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
-000110c0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000110d0: 6e31 6d6d 203d 204e 314d 4d28 0a20 2020  n1mm = N1MM(.   
-000110e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000110f0: 2073 656c 662e 7072 6566 2e67 6574 2822   self.pref.get("
-00011100: 6e31 6d6d 5f72 6164 696f 706f 7274 222c  n1mm_radioport",
-00011110: 2022 3132 372e 302e 302e 313a 3132 3036   "127.0.0.1:1206
-00011120: 3022 292c 0a20 2020 2020 2020 2020 2020  0"),.           
-00011130: 2020 2020 2020 2020 2073 656c 662e 7072           self.pr
-00011140: 6566 2e67 6574 2822 6e31 6d6d 5f63 6f6e  ef.get("n1mm_con
-00011150: 7461 6374 706f 7274 222c 2022 3132 372e  tactport", "127.
-00011160: 302e 302e 313a 3132 3036 3122 292c 0a20  0.0.1:12061"),. 
+0000d450: 696e 6773 5f64 6961 6c6f 672e 4c61 7469  ings_dialog.Lati
+0000d460: 7475 6465 2e74 6578 7428 290a 2020 2020  tude.text().    
+0000d470: 2020 2020 7365 6c66 2e73 7461 7469 6f6e      self.station
+0000d480: 5b22 4c6f 6e67 6974 7564 6522 5d20 3d20  ["Longitude"] = 
+0000d490: 7365 6c66 2e73 6574 7469 6e67 735f 6469  self.settings_di
+0000d4a0: 616c 6f67 2e4c 6f6e 6769 7475 6465 2e74  alog.Longitude.t
+0000d4b0: 6578 7428 290a 2020 2020 2020 2020 7365  ext().        se
+0000d4c0: 6c66 2e73 7461 7469 6f6e 5b22 5354 5865  lf.station["STXe
+0000d4d0: 7122 5d20 3d20 7365 6c66 2e73 6574 7469  q"] = self.setti
+0000d4e0: 6e67 735f 6469 616c 6f67 2e53 7461 7469  ngs_dialog.Stati
+0000d4f0: 6f6e 5458 5258 2e74 6578 7428 290a 2020  onTXRX.text().  
+0000d500: 2020 2020 2020 7365 6c66 2e73 7461 7469        self.stati
+0000d510: 6f6e 5b22 5350 6f77 6522 5d20 3d20 7365  on["SPowe"] = se
+0000d520: 6c66 2e73 6574 7469 6e67 735f 6469 616c  lf.settings_dial
+0000d530: 6f67 2e50 6f77 6572 2e74 6578 7428 290a  og.Power.text().
+0000d540: 2020 2020 2020 2020 7365 6c66 2e73 7461          self.sta
+0000d550: 7469 6f6e 5b22 5341 6e74 6522 5d20 3d20  tion["SAnte"] = 
+0000d560: 7365 6c66 2e73 6574 7469 6e67 735f 6469  self.settings_di
+0000d570: 616c 6f67 2e41 6e74 656e 6e61 2e74 6578  alog.Antenna.tex
+0000d580: 7428 290a 2020 2020 2020 2020 7365 6c66  t().        self
+0000d590: 2e73 7461 7469 6f6e 5b22 5341 6e74 4831  .station["SAntH1
+0000d5a0: 225d 203d 2073 656c 662e 7365 7474 696e  "] = self.settin
+0000d5b0: 6773 5f64 6961 6c6f 672e 416e 7448 6569  gs_dialog.AntHei
+0000d5c0: 6768 742e 7465 7874 2829 0a20 2020 2020  ght.text().     
+0000d5d0: 2020 2073 656c 662e 7374 6174 696f 6e5b     self.station[
+0000d5e0: 2253 416e 7448 3222 5d20 3d20 7365 6c66  "SAntH2"] = self
+0000d5f0: 2e73 6574 7469 6e67 735f 6469 616c 6f67  .settings_dialog
+0000d600: 2e41 534c 2e74 6578 7428 290a 2020 2020  .ASL.text().    
+0000d610: 2020 2020 7365 6c66 2e73 7461 7469 6f6e      self.station
+0000d620: 5b22 4152 524c 5365 6374 696f 6e22 5d20  ["ARRLSection"] 
+0000d630: 3d20 7365 6c66 2e73 6574 7469 6e67 735f  = self.settings_
+0000d640: 6469 616c 6f67 2e41 5252 4c53 6563 7469  dialog.ARRLSecti
+0000d650: 6f6e 2e74 6578 7428 292e 7570 7065 7228  on.text().upper(
+0000d660: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
+0000d670: 7461 7469 6f6e 5b22 526f 7665 7251 5448  tation["RoverQTH
+0000d680: 225d 203d 2073 656c 662e 7365 7474 696e  "] = self.settin
+0000d690: 6773 5f64 6961 6c6f 672e 526f 7665 7251  gs_dialog.RoverQ
+0000d6a0: 5448 2e74 6578 7428 290a 2020 2020 2020  TH.text().      
+0000d6b0: 2020 7365 6c66 2e73 7461 7469 6f6e 5b22    self.station["
+0000d6c0: 436c 7562 225d 203d 2073 656c 662e 7365  Club"] = self.se
+0000d6d0: 7474 696e 6773 5f64 6961 6c6f 672e 436c  ttings_dialog.Cl
+0000d6e0: 7562 2e74 6578 7428 292e 7469 746c 6528  ub.text().title(
+0000d6f0: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
+0000d700: 7461 7469 6f6e 5b22 456d 6169 6c22 5d20  tation["Email"] 
+0000d710: 3d20 7365 6c66 2e73 6574 7469 6e67 735f  = self.settings_
+0000d720: 6469 616c 6f67 2e45 6d61 696c 2e74 6578  dialog.Email.tex
+0000d730: 7428 290a 2020 2020 2020 2020 7365 6c66  t().        self
+0000d740: 2e64 6174 6162 6173 652e 6164 645f 7374  .database.add_st
+0000d750: 6174 696f 6e28 7365 6c66 2e73 7461 7469  ation(self.stati
+0000d760: 6f6e 290a 2020 2020 2020 2020 7365 6c66  on).        self
+0000d770: 2e73 6574 7469 6e67 735f 6469 616c 6f67  .settings_dialog
+0000d780: 2e63 6c6f 7365 2829 0a20 2020 2020 2020  .close().       
+0000d790: 2069 6620 7365 6c66 2e63 7572 7265 6e74   if self.current
+0000d7a0: 5f6f 7020 3d3d 2022 223a 0a20 2020 2020  _op == "":.     
+0000d7b0: 2020 2020 2020 2073 656c 662e 6375 7272         self.curr
+0000d7c0: 656e 745f 6f70 203d 2073 656c 662e 7374  ent_op = self.st
+0000d7d0: 6174 696f 6e2e 6765 7428 2243 616c 6c22  ation.get("Call"
+0000d7e0: 2c20 2222 290a 2020 2020 2020 2020 2020  , "").          
+0000d7f0: 2020 7365 6c66 2e6d 616b 655f 6f70 5f64    self.make_op_d
+0000d800: 6972 2829 0a20 2020 2020 2020 2063 6f6e  ir().        con
+0000d810: 7465 7374 5f63 6f75 6e74 203d 2073 656c  test_count = sel
+0000d820: 662e 6461 7461 6261 7365 2e66 6574 6368  f.database.fetch
+0000d830: 5f61 6c6c 5f63 6f6e 7465 7374 7328 290a  _all_contests().
+0000d840: 2020 2020 2020 2020 6966 206c 656e 2863          if len(c
+0000d850: 6f6e 7465 7374 5f63 6f75 6e74 2920 3d3d  ontest_count) ==
+0000d860: 2030 3a0a 2020 2020 2020 2020 2020 2020   0:.            
+0000d870: 7365 6c66 2e6e 6577 5f63 6f6e 7465 7374  self.new_contest
+0000d880: 5f64 6961 6c6f 6728 290a 0a20 2020 2064  _dialog()..    d
+0000d890: 6566 2065 6469 745f 6d61 6372 6f28 7365  ef edit_macro(se
+0000d8a0: 6c66 2c20 6675 6e63 7469 6f6e 5f6b 6579  lf, function_key
+0000d8b0: 293a 0a20 2020 2020 2020 2022 2222 5368  ):.        """Sh
+0000d8c0: 6f77 2065 6469 7420 6d61 6372 6f20 6469  ow edit macro di
+0000d8d0: 616c 6f67 2222 220a 2020 2020 2020 2020  alog""".        
+0000d8e0: 7365 6c66 2e65 6469 745f 6d61 6372 6f5f  self.edit_macro_
+0000d8f0: 6469 616c 6f67 203d 2045 6469 744d 6163  dialog = EditMac
+0000d900: 726f 2866 756e 6374 696f 6e5f 6b65 792c  ro(function_key,
+0000d910: 2057 4f52 4b49 4e47 5f50 4154 4829 0a20   WORKING_PATH). 
+0000d920: 2020 2020 2020 2073 656c 662e 6564 6974         self.edit
+0000d930: 5f6d 6163 726f 5f64 6961 6c6f 672e 6163  _macro_dialog.ac
+0000d940: 6365 7074 6564 2e63 6f6e 6e65 6374 2873  cepted.connect(s
+0000d950: 656c 662e 6564 6974 6564 5f6d 6163 726f  elf.edited_macro
+0000d960: 290a 2020 2020 2020 2020 7365 6c66 2e65  ).        self.e
+0000d970: 6469 745f 6d61 6372 6f5f 6469 616c 6f67  dit_macro_dialog
+0000d980: 2e6f 7065 6e28 290a 0a20 2020 2064 6566  .open()..    def
+0000d990: 2065 6469 7465 645f 6d61 6372 6f28 7365   edited_macro(se
+0000d9a0: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
+0000d9b0: 5361 7665 2065 6469 7465 6420 6d61 6372  Save edited macr
+0000d9c0: 6f22 2222 0a20 2020 2020 2020 2073 656c  o""".        sel
+0000d9d0: 662e 6564 6974 5f6d 6163 726f 5f64 6961  f.edit_macro_dia
+0000d9e0: 6c6f 672e 6675 6e63 7469 6f6e 5f6b 6579  log.function_key
+0000d9f0: 2e73 6574 5465 7874 280a 2020 2020 2020  .setText(.      
+0000da00: 2020 2020 2020 7365 6c66 2e65 6469 745f        self.edit_
+0000da10: 6d61 6372 6f5f 6469 616c 6f67 2e6d 6163  macro_dialog.mac
+0000da20: 726f 5f6c 6162 656c 2e74 6578 7428 290a  ro_label.text().
+0000da30: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+0000da40: 2020 7365 6c66 2e65 6469 745f 6d61 6372    self.edit_macr
+0000da50: 6f5f 6469 616c 6f67 2e66 756e 6374 696f  o_dialog.functio
+0000da60: 6e5f 6b65 792e 7365 7454 6f6f 6c54 6970  n_key.setToolTip
+0000da70: 280a 2020 2020 2020 2020 2020 2020 7365  (.            se
+0000da80: 6c66 2e65 6469 745f 6d61 6372 6f5f 6469  lf.edit_macro_di
+0000da90: 616c 6f67 2e74 6865 5f6d 6163 726f 2e74  alog.the_macro.t
+0000daa0: 6578 7428 290a 2020 2020 2020 2020 290a  ext().        ).
+0000dab0: 2020 2020 2020 2020 7365 6c66 2e65 6469          self.edi
+0000dac0: 745f 6d61 6372 6f5f 6469 616c 6f67 2e63  t_macro_dialog.c
+0000dad0: 6c6f 7365 2829 0a0a 2020 2020 6465 6620  lose()..    def 
+0000dae0: 6564 6974 5f46 3128 7365 6c66 293a 0a20  edit_F1(self):. 
+0000daf0: 2020 2020 2020 2022 2222 7374 7562 2222         """stub""
+0000db00: 220a 2020 2020 2020 2020 6c6f 6767 6572  ".        logger
+0000db10: 2e64 6562 7567 2822 4631 2052 6967 6874  .debug("F1 Right
+0000db20: 2043 6c69 636b 6564 2e22 290a 2020 2020   Clicked.").    
+0000db30: 2020 2020 7365 6c66 2e65 6469 745f 6d61      self.edit_ma
+0000db40: 6372 6f28 7365 6c66 2e46 3129 0a0a 2020  cro(self.F1)..  
+0000db50: 2020 6465 6620 6564 6974 5f46 3228 7365    def edit_F2(se
+0000db60: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
+0000db70: 7374 7562 2222 220a 2020 2020 2020 2020  stub""".        
+0000db80: 6c6f 6767 6572 2e64 6562 7567 2822 4632  logger.debug("F2
+0000db90: 2052 6967 6874 2043 6c69 636b 6564 2e22   Right Clicked."
+0000dba0: 290a 2020 2020 2020 2020 7365 6c66 2e65  ).        self.e
+0000dbb0: 6469 745f 6d61 6372 6f28 7365 6c66 2e46  dit_macro(self.F
+0000dbc0: 3229 0a0a 2020 2020 6465 6620 6564 6974  2)..    def edit
+0000dbd0: 5f46 3328 7365 6c66 293a 0a20 2020 2020  _F3(self):.     
+0000dbe0: 2020 2022 2222 7374 7562 2222 220a 2020     """stub""".  
+0000dbf0: 2020 2020 2020 6c6f 6767 6572 2e64 6562        logger.deb
+0000dc00: 7567 2822 4633 2052 6967 6874 2043 6c69  ug("F3 Right Cli
+0000dc10: 636b 6564 2e22 290a 2020 2020 2020 2020  cked.").        
+0000dc20: 7365 6c66 2e65 6469 745f 6d61 6372 6f28  self.edit_macro(
+0000dc30: 7365 6c66 2e46 3329 0a0a 2020 2020 6465  self.F3)..    de
+0000dc40: 6620 6564 6974 5f46 3428 7365 6c66 293a  f edit_F4(self):
+0000dc50: 0a20 2020 2020 2020 2022 2222 7374 7562  .        """stub
+0000dc60: 2222 220a 2020 2020 2020 2020 6c6f 6767  """.        logg
+0000dc70: 6572 2e64 6562 7567 2822 4634 2052 6967  er.debug("F4 Rig
+0000dc80: 6874 2043 6c69 636b 6564 2e22 290a 2020  ht Clicked.").  
+0000dc90: 2020 2020 2020 7365 6c66 2e65 6469 745f        self.edit_
+0000dca0: 6d61 6372 6f28 7365 6c66 2e46 3429 0a0a  macro(self.F4)..
+0000dcb0: 2020 2020 6465 6620 6564 6974 5f46 3528      def edit_F5(
+0000dcc0: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
+0000dcd0: 2222 7374 7562 2222 220a 2020 2020 2020  ""stub""".      
+0000dce0: 2020 6c6f 6767 6572 2e64 6562 7567 2822    logger.debug("
+0000dcf0: 4635 2052 6967 6874 2043 6c69 636b 6564  F5 Right Clicked
+0000dd00: 2e22 290a 2020 2020 2020 2020 7365 6c66  .").        self
+0000dd10: 2e65 6469 745f 6d61 6372 6f28 7365 6c66  .edit_macro(self
+0000dd20: 2e46 3529 0a0a 2020 2020 6465 6620 6564  .F5)..    def ed
+0000dd30: 6974 5f46 3628 7365 6c66 293a 0a20 2020  it_F6(self):.   
+0000dd40: 2020 2020 2022 2222 7374 7562 2222 220a       """stub""".
+0000dd50: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
+0000dd60: 6562 7567 2822 4636 2052 6967 6874 2043  ebug("F6 Right C
+0000dd70: 6c69 636b 6564 2e22 290a 2020 2020 2020  licked.").      
+0000dd80: 2020 7365 6c66 2e65 6469 745f 6d61 6372    self.edit_macr
+0000dd90: 6f28 7365 6c66 2e46 3629 0a0a 2020 2020  o(self.F6)..    
+0000dda0: 6465 6620 6564 6974 5f46 3728 7365 6c66  def edit_F7(self
+0000ddb0: 293a 0a20 2020 2020 2020 2022 2222 7374  ):.        """st
+0000ddc0: 7562 2222 220a 2020 2020 2020 2020 6c6f  ub""".        lo
+0000ddd0: 6767 6572 2e64 6562 7567 2822 4637 2052  gger.debug("F7 R
+0000dde0: 6967 6874 2043 6c69 636b 6564 2e22 290a  ight Clicked.").
+0000ddf0: 2020 2020 2020 2020 7365 6c66 2e65 6469          self.edi
+0000de00: 745f 6d61 6372 6f28 7365 6c66 2e46 3729  t_macro(self.F7)
+0000de10: 0a0a 2020 2020 6465 6620 6564 6974 5f46  ..    def edit_F
+0000de20: 3828 7365 6c66 293a 0a20 2020 2020 2020  8(self):.       
+0000de30: 2022 2222 7374 7562 2222 220a 2020 2020   """stub""".    
+0000de40: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
+0000de50: 2822 4638 2052 6967 6874 2043 6c69 636b  ("F8 Right Click
+0000de60: 6564 2e22 290a 2020 2020 2020 2020 7365  ed.").        se
+0000de70: 6c66 2e65 6469 745f 6d61 6372 6f28 7365  lf.edit_macro(se
+0000de80: 6c66 2e46 3829 0a0a 2020 2020 6465 6620  lf.F8)..    def 
+0000de90: 6564 6974 5f46 3928 7365 6c66 293a 0a20  edit_F9(self):. 
+0000dea0: 2020 2020 2020 2022 2222 7374 7562 2222         """stub""
+0000deb0: 220a 2020 2020 2020 2020 6c6f 6767 6572  ".        logger
+0000dec0: 2e64 6562 7567 2822 4639 2052 6967 6874  .debug("F9 Right
+0000ded0: 2043 6c69 636b 6564 2e22 290a 2020 2020   Clicked.").    
+0000dee0: 2020 2020 7365 6c66 2e65 6469 745f 6d61      self.edit_ma
+0000def0: 6372 6f28 7365 6c66 2e46 3929 0a0a 2020  cro(self.F9)..  
+0000df00: 2020 6465 6620 6564 6974 5f46 3130 2873    def edit_F10(s
+0000df10: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
+0000df20: 2273 7475 6222 2222 0a20 2020 2020 2020  "stub""".       
+0000df30: 206c 6f67 6765 722e 6465 6275 6728 2246   logger.debug("F
+0000df40: 3130 2052 6967 6874 2043 6c69 636b 6564  10 Right Clicked
+0000df50: 2e22 290a 2020 2020 2020 2020 7365 6c66  .").        self
+0000df60: 2e65 6469 745f 6d61 6372 6f28 7365 6c66  .edit_macro(self
+0000df70: 2e46 3130 290a 0a20 2020 2064 6566 2065  .F10)..    def e
+0000df80: 6469 745f 4631 3128 7365 6c66 293a 0a20  dit_F11(self):. 
+0000df90: 2020 2020 2020 2022 2222 7374 7562 2222         """stub""
+0000dfa0: 220a 2020 2020 2020 2020 6c6f 6767 6572  ".        logger
+0000dfb0: 2e64 6562 7567 2822 4631 3120 5269 6768  .debug("F11 Righ
+0000dfc0: 7420 436c 6963 6b65 642e 2229 0a20 2020  t Clicked.").   
+0000dfd0: 2020 2020 2073 656c 662e 6564 6974 5f6d       self.edit_m
+0000dfe0: 6163 726f 2873 656c 662e 4631 3129 0a0a  acro(self.F11)..
+0000dff0: 2020 2020 6465 6620 6564 6974 5f46 3132      def edit_F12
+0000e000: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0000e010: 2222 2273 7475 6222 2222 0a20 2020 2020  """stub""".     
+0000e020: 2020 206c 6f67 6765 722e 6465 6275 6728     logger.debug(
+0000e030: 2246 3132 2052 6967 6874 2043 6c69 636b  "F12 Right Click
+0000e040: 6564 2e22 290a 2020 2020 2020 2020 7365  ed.").        se
+0000e050: 6c66 2e65 6469 745f 6d61 6372 6f28 7365  lf.edit_macro(se
+0000e060: 6c66 2e46 3132 290a 0a20 2020 2064 6566  lf.F12)..    def
+0000e070: 2070 726f 6365 7373 5f6d 6163 726f 2873   process_macro(s
+0000e080: 656c 662c 206d 6163 726f 3a20 7374 7229  elf, macro: str)
+0000e090: 202d 3e20 7374 723a 0a20 2020 2020 2020   -> str:.       
+0000e0a0: 2022 2222 5072 6f63 6573 7320 4357 206d   """Process CW m
+0000e0b0: 6163 726f 2073 7562 7374 6974 7574 696f  acro substitutio
+0000e0c0: 6e73 2222 220a 2020 2020 2020 2020 7265  ns""".        re
+0000e0d0: 7375 6c74 203d 2073 656c 662e 6461 7461  sult = self.data
+0000e0e0: 6261 7365 2e67 6574 5f73 6572 6961 6c28  base.get_serial(
+0000e0f0: 290a 2020 2020 2020 2020 6e65 7874 5f73  ).        next_s
+0000e100: 6572 6961 6c20 3d20 7374 7228 7265 7375  erial = str(resu
+0000e110: 6c74 2e67 6574 2822 7365 7269 616c 5f6e  lt.get("serial_n
+0000e120: 7222 2c20 2231 2229 290a 2020 2020 2020  r", "1")).      
+0000e130: 2020 6966 206e 6578 745f 7365 7269 616c    if next_serial
+0000e140: 203d 3d20 224e 6f6e 6522 3a0a 2020 2020   == "None":.    
+0000e150: 2020 2020 2020 2020 6e65 7874 5f73 6572          next_ser
+0000e160: 6961 6c20 3d20 2231 220a 2020 2020 2020  ial = "1".      
+0000e170: 2020 6d61 6372 6f20 3d20 6d61 6372 6f2e    macro = macro.
+0000e180: 7570 7065 7228 290a 2020 2020 2020 2020  upper().        
+0000e190: 6d61 6372 6f20 3d20 6d61 6372 6f2e 7265  macro = macro.re
+0000e1a0: 706c 6163 6528 2223 222c 206e 6578 745f  place("#", next_
+0000e1b0: 7365 7269 616c 290a 2020 2020 2020 2020  serial).        
+0000e1c0: 6d61 6372 6f20 3d20 6d61 6372 6f2e 7265  macro = macro.re
+0000e1d0: 706c 6163 6528 227b 4d59 4341 4c4c 7d22  place("{MYCALL}"
+0000e1e0: 2c20 7365 6c66 2e73 7461 7469 6f6e 2e67  , self.station.g
+0000e1f0: 6574 2822 4361 6c6c 222c 2022 2229 290a  et("Call", "")).
+0000e200: 2020 2020 2020 2020 6d61 6372 6f20 3d20          macro = 
+0000e210: 6d61 6372 6f2e 7265 706c 6163 6528 227b  macro.replace("{
+0000e220: 4849 5343 414c 4c7d 222c 2073 656c 662e  HISCALL}", self.
+0000e230: 6361 6c6c 7369 676e 2e74 6578 7428 2929  callsign.text())
+0000e240: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+0000e250: 2e72 6164 696f 5f73 7461 7465 2e67 6574  .radio_state.get
+0000e260: 2822 6d6f 6465 2229 203d 3d20 2243 5722  ("mode") == "CW"
+0000e270: 3a0a 2020 2020 2020 2020 2020 2020 6d61  :.            ma
+0000e280: 6372 6f20 3d20 6d61 6372 6f2e 7265 706c  cro = macro.repl
+0000e290: 6163 6528 227b 534e 547d 222c 2073 656c  ace("{SNT}", sel
+0000e2a0: 662e 7365 6e74 2e74 6578 7428 292e 7265  f.sent.text().re
+0000e2b0: 706c 6163 6528 2239 222c 2022 6e22 2929  place("9", "n"))
+0000e2c0: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+0000e2d0: 2020 2020 2020 2020 2020 206d 6163 726f             macro
+0000e2e0: 203d 206d 6163 726f 2e72 6570 6c61 6365   = macro.replace
+0000e2f0: 2822 7b53 4e54 7d22 2c20 7365 6c66 2e73  ("{SNT}", self.s
+0000e300: 656e 742e 7465 7874 2829 290a 2020 2020  ent.text()).    
+0000e310: 2020 2020 6d61 6372 6f20 3d20 6d61 6372      macro = macr
+0000e320: 6f2e 7265 706c 6163 6528 227b 5345 4e54  o.replace("{SENT
+0000e330: 4e52 7d22 2c20 7365 6c66 2e6f 7468 6572  NR}", self.other
+0000e340: 5f31 2e74 6578 7428 2929 0a20 2020 2020  _1.text()).     
+0000e350: 2020 206d 6163 726f 203d 206d 6163 726f     macro = macro
+0000e360: 2e72 6570 6c61 6365 280a 2020 2020 2020  .replace(.      
+0000e370: 2020 2020 2020 227b 4558 4348 7d22 2c20        "{EXCH}", 
+0000e380: 7365 6c66 2e63 6f6e 7465 7374 5f73 6574  self.contest_set
+0000e390: 7469 6e67 732e 6765 7428 2253 656e 7445  tings.get("SentE
+0000e3a0: 7863 6861 6e67 6522 2c20 2278 7878 2229  xchange", "xxx")
+0000e3b0: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
+0000e3c0: 2020 2072 6574 7572 6e20 6d61 6372 6f0a     return macro.
+0000e3d0: 0a20 2020 2064 6566 2076 6f69 6365 5f73  .    def voice_s
+0000e3e0: 7472 696e 6728 7365 6c66 2c20 7468 655f  tring(self, the_
+0000e3f0: 7374 7269 6e67 3a20 7374 7229 202d 3e20  string: str) -> 
+0000e400: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
+0000e410: 2276 6f69 6365 7320 7374 7269 6e67 2075  "voices string u
+0000e420: 7369 6e67 206e 6174 6f20 7068 6f6e 6574  sing nato phonet
+0000e430: 6963 7322 2222 0a20 2020 2020 2020 206c  ics""".        l
+0000e440: 6f67 6765 722e 6465 6275 6728 2256 6f69  ogger.debug("Voi
+0000e450: 6369 6e67 3a20 2573 222c 2074 6865 5f73  cing: %s", the_s
+0000e460: 7472 696e 6729 0a20 2020 2020 2020 206f  tring).        o
+0000e470: 705f 7061 7468 203d 2050 6174 6828 4441  p_path = Path(DA
+0000e480: 5441 5f50 4154 4829 202f 2073 656c 662e  TA_PATH) / self.
+0000e490: 6375 7272 656e 745f 6f70 0a20 2020 2020  current_op.     
+0000e4a0: 2020 2069 6620 225b 2220 696e 2074 6865     if "[" in the
+0000e4b0: 5f73 7472 696e 673a 0a20 2020 2020 2020  _string:.       
+0000e4c0: 2020 2020 2073 7562 5f73 7472 696e 6720       sub_string 
+0000e4d0: 3d20 7468 655f 7374 7269 6e67 2e73 7472  = the_string.str
+0000e4e0: 6970 2822 5b5d 2229 2e6c 6f77 6572 2829  ip("[]").lower()
+0000e4f0: 0a20 2020 2020 2020 2020 2020 2066 696c  .            fil
+0000e500: 656e 616d 6520 3d20 6622 7b73 7472 286f  ename = f"{str(o
+0000e510: 705f 7061 7468 297d 2f7b 7375 625f 7374  p_path)}/{sub_st
+0000e520: 7269 6e67 7d2e 7761 7622 0a20 2020 2020  ring}.wav".     
+0000e530: 2020 2020 2020 2069 6620 5061 7468 2866         if Path(f
+0000e540: 696c 656e 616d 6529 2e69 735f 6669 6c65  ilename).is_file
+0000e550: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+0000e560: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
+0000e570: 2822 566f 6963 696e 673a 2025 7322 2c20  ("Voicing: %s", 
+0000e580: 6669 6c65 6e61 6d65 290a 2020 2020 2020  filename).      
+0000e590: 2020 2020 2020 2020 2020 6461 7461 2c20            data, 
+0000e5a0: 5f66 7320 3d20 7366 2e72 6561 6428 6669  _fs = sf.read(fi
+0000e5b0: 6c65 6e61 6d65 2c20 6474 7970 653d 2266  lename, dtype="f
+0000e5c0: 6c6f 6174 3332 2229 0a20 2020 2020 2020  loat32").       
+0000e5d0: 2020 2020 2020 2020 2073 656c 662e 7074           self.pt
+0000e5e0: 745f 6f6e 2829 0a20 2020 2020 2020 2020  t_on().         
+0000e5f0: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
+0000e600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e610: 7364 2e64 6566 6175 6c74 2e64 6576 6963  sd.default.devic
+0000e620: 6520 3d20 7365 6c66 2e70 7265 662e 6765  e = self.pref.ge
+0000e630: 7428 2273 6f75 6e64 6465 7669 6365 222c  t("sounddevice",
+0000e640: 2022 6465 6661 756c 7422 290a 2020 2020   "default").    
+0000e650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e660: 7364 2e64 6566 6175 6c74 2e73 616d 706c  sd.default.sampl
+0000e670: 6572 6174 6520 3d20 3434 3130 302e 300a  erate = 44100.0.
+0000e680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e690: 2020 2020 7364 2e70 6c61 7928 6461 7461      sd.play(data
+0000e6a0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000e6b0: 2020 2020 2020 5f73 7461 7475 7320 3d20        _status = 
+0000e6c0: 7364 2e77 6169 7428 290a 2020 2020 2020  sd.wait().      
+0000e6d0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+0000e6e0: 6874 7470 733a 2f2f 736e 796b 2e69 6f2f  https://snyk.io/
+0000e6f0: 6164 7669 736f 722f 7079 7468 6f6e 2f73  advisor/python/s
+0000e700: 6f75 6e64 6465 7669 6365 2f66 756e 6374  ounddevice/funct
+0000e710: 696f 6e73 2f73 6f75 6e64 6465 7669 6365  ions/sounddevice
+0000e720: 2e50 6f72 7441 7564 696f 4572 726f 720a  .PortAudioError.
+0000e730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e740: 6578 6365 7074 2073 642e 506f 7274 4175  except sd.PortAu
+0000e750: 6469 6f45 7272 6f72 2061 7320 6572 723a  dioError as err:
+0000e760: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e770: 2020 2020 206c 6f67 6765 722e 7761 726e       logger.warn
+0000e780: 696e 6728 2225 7322 2c20 6622 7b65 7272  ing("%s", f"{err
+0000e790: 7d22 290a 0a20 2020 2020 2020 2020 2020  }")..           
+0000e7a0: 2020 2020 2073 656c 662e 7074 745f 6f66       self.ptt_of
+0000e7b0: 6628 290a 2020 2020 2020 2020 2020 2020  f().            
+0000e7c0: 7265 7475 726e 0a20 2020 2020 2020 2073  return.        s
+0000e7d0: 656c 662e 7074 745f 6f6e 2829 0a20 2020  elf.ptt_on().   
+0000e7e0: 2020 2020 2066 6f72 206c 6574 7465 7220       for letter 
+0000e7f0: 696e 2074 6865 5f73 7472 696e 672e 6c6f  in the_string.lo
+0000e800: 7765 7228 293a 0a20 2020 2020 2020 2020  wer():.         
+0000e810: 2020 2069 6620 6c65 7474 6572 2069 6e20     if letter in 
+0000e820: 2261 6263 6465 6667 6869 6a6b 6c6d 6e6f  "abcdefghijklmno
+0000e830: 7071 7273 7475 7677 7879 7a20 3132 3334  pqrstuvwxyz 1234
+0000e840: 3536 3738 3930 223a 0a20 2020 2020 2020  567890":.       
+0000e850: 2020 2020 2020 2020 2069 6620 6c65 7474           if lett
+0000e860: 6572 203d 3d20 2220 223a 0a20 2020 2020  er == " ":.     
+0000e870: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+0000e880: 6574 7465 7220 3d20 2273 7061 6365 220a  etter = "space".
+0000e890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e8a0: 6669 6c65 6e61 6d65 203d 2066 227b 7374  filename = f"{st
+0000e8b0: 7228 6f70 5f70 6174 6829 7d2f 7b6c 6574  r(op_path)}/{let
+0000e8c0: 7465 727d 2e77 6176 220a 2020 2020 2020  ter}.wav".      
+0000e8d0: 2020 2020 2020 2020 2020 6966 2050 6174            if Pat
+0000e8e0: 6828 6669 6c65 6e61 6d65 292e 6973 5f66  h(filename).is_f
+0000e8f0: 696c 6528 293a 0a20 2020 2020 2020 2020  ile():.         
+0000e900: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
+0000e910: 722e 6465 6275 6728 2256 6f69 6369 6e67  r.debug("Voicing
+0000e920: 3a20 2573 222c 2066 696c 656e 616d 6529  : %s", filename)
+0000e930: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e940: 2020 2020 2064 6174 612c 205f 6673 203d       data, _fs =
+0000e950: 2073 662e 7265 6164 2866 696c 656e 616d   sf.read(filenam
+0000e960: 652c 2064 7479 7065 3d22 666c 6f61 7433  e, dtype="float3
+0000e970: 3222 290a 2020 2020 2020 2020 2020 2020  2").            
+0000e980: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
+0000e990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e9a0: 2020 2020 2073 642e 6465 6661 756c 742e       sd.default.
+0000e9b0: 6465 7669 6365 203d 2073 656c 662e 7072  device = self.pr
+0000e9c0: 6566 2e67 6574 2822 736f 756e 6464 6576  ef.get("sounddev
+0000e9d0: 6963 6522 2c20 2264 6566 6175 6c74 2229  ice", "default")
+0000e9e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e9f0: 2020 2020 2020 2020 2073 642e 6465 6661           sd.defa
+0000ea00: 756c 742e 7361 6d70 6c65 7261 7465 203d  ult.samplerate =
+0000ea10: 2034 3431 3030 2e30 0a20 2020 2020 2020   44100.0.       
+0000ea20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ea30: 2073 642e 706c 6179 2864 6174 6129 0a20   sd.play(data). 
+0000ea40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ea50: 2020 2020 2020 206c 6f67 6765 722e 6465         logger.de
+0000ea60: 6275 6728 2225 7322 2c20 6622 7b73 642e  bug("%s", f"{sd.
+0000ea70: 7761 6974 2829 7d22 290a 2020 2020 2020  wait()}").      
+0000ea80: 2020 2020 2020 2020 2020 2020 2020 6578                ex
+0000ea90: 6365 7074 2073 642e 506f 7274 4175 6469  cept sd.PortAudi
+0000eaa0: 6f45 7272 6f72 2061 7320 6572 723a 0a20  oError as err:. 
+0000eab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eac0: 2020 2020 2020 206c 6f67 6765 722e 7761         logger.wa
+0000ead0: 726e 696e 6728 2225 7322 2c20 6622 7b65  rning("%s", f"{e
+0000eae0: 7272 7d22 290a 2020 2020 2020 2020 7365  rr}").        se
+0000eaf0: 6c66 2e70 7474 5f6f 6666 2829 0a0a 2020  lf.ptt_off()..  
+0000eb00: 2020 6465 6620 7074 745f 6f6e 2873 656c    def ptt_on(sel
+0000eb10: 6629 3a0a 2020 2020 2020 2020 2222 2274  f):.        """t
+0000eb20: 7572 6e20 6f6e 2070 7474 2222 220a 2020  urn on ptt""".  
+0000eb30: 2020 2020 2020 6966 2073 656c 662e 7269        if self.ri
+0000eb40: 675f 636f 6e74 726f 6c3a 0a20 2020 2020  g_control:.     
+0000eb50: 2020 2020 2020 2073 656c 662e 6c65 6674         self.left
+0000eb60: 646f 742e 7365 7450 6978 6d61 7028 7365  dot.setPixmap(se
+0000eb70: 6c66 2e67 7265 656e 646f 7429 0a20 2020  lf.greendot).   
+0000eb80: 2020 2020 2020 2020 2061 7070 2e70 726f           app.pro
+0000eb90: 6365 7373 4576 656e 7473 2829 0a20 2020  cessEvents().   
+0000eba0: 2020 2020 2020 2020 2073 656c 662e 7269           self.ri
+0000ebb0: 675f 636f 6e74 726f 6c2e 7074 745f 6f6e  g_control.ptt_on
+0000ebc0: 2829 0a0a 2020 2020 6465 6620 7074 745f  ()..    def ptt_
+0000ebd0: 6f66 6628 7365 6c66 293a 0a20 2020 2020  off(self):.     
+0000ebe0: 2020 2022 2222 7475 726e 206f 6666 2070     """turn off p
+0000ebf0: 7474 2222 220a 2020 2020 2020 2020 6966  tt""".        if
+0000ec00: 2073 656c 662e 7269 675f 636f 6e74 726f   self.rig_contro
+0000ec10: 6c3a 0a20 2020 2020 2020 2020 2020 2073  l:.            s
+0000ec20: 656c 662e 6c65 6674 646f 742e 7365 7450  elf.leftdot.setP
+0000ec30: 6978 6d61 7028 7365 6c66 2e72 6564 646f  ixmap(self.reddo
+0000ec40: 7429 0a20 2020 2020 2020 2020 2020 2061  t).            a
+0000ec50: 7070 2e70 726f 6365 7373 4576 656e 7473  pp.processEvents
+0000ec60: 2829 0a20 2020 2020 2020 2020 2020 2073  ().            s
+0000ec70: 656c 662e 7269 675f 636f 6e74 726f 6c2e  elf.rig_control.
+0000ec80: 7074 745f 6f66 6628 290a 0a20 2020 2064  ptt_off()..    d
+0000ec90: 6566 2073 656e 6466 3128 7365 6c66 293a  ef sendf1(self):
+0000eca0: 0a20 2020 2020 2020 2022 2222 7374 7562  .        """stub
+0000ecb0: 2222 220a 2020 2020 2020 2020 6c6f 6767  """.        logg
+0000ecc0: 6572 2e64 6562 7567 2822 4631 2043 6c69  er.debug("F1 Cli
+0000ecd0: 636b 6564 2229 0a20 2020 2020 2020 2069  cked").        i
+0000ece0: 6620 7365 6c66 2e6e 316d 6d3a 0a20 2020  f self.n1mm:.   
+0000ecf0: 2020 2020 2020 2020 2073 656c 662e 6e31           self.n1
+0000ed00: 6d6d 2e72 6164 696f 5f69 6e66 6f5b 2246  mm.radio_info["F
+0000ed10: 756e 6374 696f 6e4b 6579 4361 7074 696f  unctionKeyCaptio
+0000ed20: 6e22 5d20 3d20 7365 6c66 2e46 312e 7465  n"] = self.F1.te
+0000ed30: 7874 2829 0a20 2020 2020 2020 2069 6620  xt().        if 
+0000ed40: 7365 6c66 2e72 6164 696f 5f73 7461 7465  self.radio_state
+0000ed50: 2e67 6574 2822 6d6f 6465 2229 2069 6e20  .get("mode") in 
+0000ed60: 5b22 4c53 4222 2c20 2255 5342 222c 2022  ["LSB", "USB", "
+0000ed70: 5353 4222 5d3a 0a20 2020 2020 2020 2020  SSB"]:.         
+0000ed80: 2020 2073 656c 662e 766f 6963 655f 7374     self.voice_st
+0000ed90: 7269 6e67 2873 656c 662e 7072 6f63 6573  ring(self.proces
+0000eda0: 735f 6d61 6372 6f28 7365 6c66 2e46 312e  s_macro(self.F1.
+0000edb0: 746f 6f6c 5469 7028 2929 290a 2020 2020  toolTip())).    
+0000edc0: 2020 2020 2020 2020 7265 7475 726e 0a20          return. 
+0000edd0: 2020 2020 2020 2069 6620 7365 6c66 2e63         if self.c
+0000ede0: 773a 0a20 2020 2020 2020 2020 2020 2073  w:.            s
+0000edf0: 656c 662e 6377 2e73 656e 6463 7728 7365  elf.cw.sendcw(se
+0000ee00: 6c66 2e70 726f 6365 7373 5f6d 6163 726f  lf.process_macro
+0000ee10: 2873 656c 662e 4631 2e74 6f6f 6c54 6970  (self.F1.toolTip
+0000ee20: 2829 2929 0a0a 2020 2020 6465 6620 7365  ()))..    def se
+0000ee30: 6e64 6632 2873 656c 6629 3a0a 2020 2020  ndf2(self):.    
+0000ee40: 2020 2020 2222 2273 7475 6222 2222 0a20      """stub""". 
+0000ee50: 2020 2020 2020 206c 6f67 6765 722e 6465         logger.de
+0000ee60: 6275 6728 2246 3220 436c 6963 6b65 6422  bug("F2 Clicked"
+0000ee70: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
+0000ee80: 662e 6e31 6d6d 3a0a 2020 2020 2020 2020  f.n1mm:.        
+0000ee90: 2020 2020 7365 6c66 2e6e 316d 6d2e 7261      self.n1mm.ra
+0000eea0: 6469 6f5f 696e 666f 5b22 4675 6e63 7469  dio_info["Functi
+0000eeb0: 6f6e 4b65 7943 6170 7469 6f6e 225d 203d  onKeyCaption"] =
+0000eec0: 2073 656c 662e 4632 2e74 6578 7428 290a   self.F2.text().
+0000eed0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0000eee0: 7261 6469 6f5f 7374 6174 652e 6765 7428  radio_state.get(
+0000eef0: 226d 6f64 6522 2920 696e 205b 224c 5342  "mode") in ["LSB
+0000ef00: 222c 2022 5553 4222 2c20 2253 5342 225d  ", "USB", "SSB"]
+0000ef10: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0000ef20: 6c66 2e76 6f69 6365 5f73 7472 696e 6728  lf.voice_string(
+0000ef30: 7365 6c66 2e70 726f 6365 7373 5f6d 6163  self.process_mac
+0000ef40: 726f 2873 656c 662e 4632 2e74 6f6f 6c54  ro(self.F2.toolT
+0000ef50: 6970 2829 2929 0a20 2020 2020 2020 2020  ip())).         
+0000ef60: 2020 2072 6574 7572 6e0a 2020 2020 2020     return.      
+0000ef70: 2020 6966 2073 656c 662e 6377 3a0a 2020    if self.cw:.  
+0000ef80: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+0000ef90: 772e 7365 6e64 6377 2873 656c 662e 7072  w.sendcw(self.pr
+0000efa0: 6f63 6573 735f 6d61 6372 6f28 7365 6c66  ocess_macro(self
+0000efb0: 2e46 322e 746f 6f6c 5469 7028 2929 290a  .F2.toolTip())).
+0000efc0: 0a20 2020 2064 6566 2073 656e 6466 3328  .    def sendf3(
+0000efd0: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
+0000efe0: 2222 7374 7562 2222 220a 2020 2020 2020  ""stub""".      
+0000eff0: 2020 6c6f 6767 6572 2e64 6562 7567 2822    logger.debug("
+0000f000: 4633 2043 6c69 636b 6564 2229 0a20 2020  F3 Clicked").   
+0000f010: 2020 2020 2069 6620 7365 6c66 2e6e 316d       if self.n1m
+0000f020: 6d3a 0a20 2020 2020 2020 2020 2020 2073  m:.            s
+0000f030: 656c 662e 6e31 6d6d 2e72 6164 696f 5f69  elf.n1mm.radio_i
+0000f040: 6e66 6f5b 2246 756e 6374 696f 6e4b 6579  nfo["FunctionKey
+0000f050: 4361 7074 696f 6e22 5d20 3d20 7365 6c66  Caption"] = self
+0000f060: 2e46 332e 7465 7874 2829 0a20 2020 2020  .F3.text().     
+0000f070: 2020 2069 6620 7365 6c66 2e72 6164 696f     if self.radio
+0000f080: 5f73 7461 7465 2e67 6574 2822 6d6f 6465  _state.get("mode
+0000f090: 2229 2069 6e20 5b22 4c53 4222 2c20 2255  ") in ["LSB", "U
+0000f0a0: 5342 222c 2022 5353 4222 5d3a 0a20 2020  SB", "SSB"]:.   
+0000f0b0: 2020 2020 2020 2020 2073 656c 662e 766f           self.vo
+0000f0c0: 6963 655f 7374 7269 6e67 2873 656c 662e  ice_string(self.
+0000f0d0: 7072 6f63 6573 735f 6d61 6372 6f28 7365  process_macro(se
+0000f0e0: 6c66 2e46 332e 746f 6f6c 5469 7028 2929  lf.F3.toolTip())
+0000f0f0: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
+0000f100: 7475 726e 0a20 2020 2020 2020 2069 6620  turn.        if 
+0000f110: 7365 6c66 2e63 773a 0a20 2020 2020 2020  self.cw:.       
+0000f120: 2020 2020 2073 656c 662e 6377 2e73 656e       self.cw.sen
+0000f130: 6463 7728 7365 6c66 2e70 726f 6365 7373  dcw(self.process
+0000f140: 5f6d 6163 726f 2873 656c 662e 4633 2e74  _macro(self.F3.t
+0000f150: 6f6f 6c54 6970 2829 2929 0a0a 2020 2020  oolTip()))..    
+0000f160: 6465 6620 7365 6e64 6634 2873 656c 6629  def sendf4(self)
+0000f170: 3a0a 2020 2020 2020 2020 2222 2273 7475  :.        """stu
+0000f180: 6222 2222 0a20 2020 2020 2020 206c 6f67  b""".        log
+0000f190: 6765 722e 6465 6275 6728 2246 3420 436c  ger.debug("F4 Cl
+0000f1a0: 6963 6b65 6422 290a 2020 2020 2020 2020  icked").        
+0000f1b0: 6966 2073 656c 662e 6e31 6d6d 3a0a 2020  if self.n1mm:.  
+0000f1c0: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
+0000f1d0: 316d 6d2e 7261 6469 6f5f 696e 666f 5b22  1mm.radio_info["
+0000f1e0: 4675 6e63 7469 6f6e 4b65 7943 6170 7469  FunctionKeyCapti
+0000f1f0: 6f6e 225d 203d 2073 656c 662e 4634 2e74  on"] = self.F4.t
+0000f200: 6578 7428 290a 2020 2020 2020 2020 6966  ext().        if
+0000f210: 2073 656c 662e 7261 6469 6f5f 7374 6174   self.radio_stat
+0000f220: 652e 6765 7428 226d 6f64 6522 2920 696e  e.get("mode") in
+0000f230: 205b 224c 5342 222c 2022 5553 4222 2c20   ["LSB", "USB", 
+0000f240: 2253 5342 225d 3a0a 2020 2020 2020 2020  "SSB"]:.        
+0000f250: 2020 2020 7365 6c66 2e76 6f69 6365 5f73      self.voice_s
+0000f260: 7472 696e 6728 7365 6c66 2e70 726f 6365  tring(self.proce
+0000f270: 7373 5f6d 6163 726f 2873 656c 662e 4634  ss_macro(self.F4
+0000f280: 2e74 6f6f 6c54 6970 2829 2929 0a20 2020  .toolTip())).   
+0000f290: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
+0000f2a0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0000f2b0: 6377 3a0a 2020 2020 2020 2020 2020 2020  cw:.            
+0000f2c0: 7365 6c66 2e63 772e 7365 6e64 6377 2873  self.cw.sendcw(s
+0000f2d0: 656c 662e 7072 6f63 6573 735f 6d61 6372  elf.process_macr
+0000f2e0: 6f28 7365 6c66 2e46 342e 746f 6f6c 5469  o(self.F4.toolTi
+0000f2f0: 7028 2929 290a 0a20 2020 2064 6566 2073  p()))..    def s
+0000f300: 656e 6466 3528 7365 6c66 293a 0a20 2020  endf5(self):.   
+0000f310: 2020 2020 2022 2222 7374 7562 2222 220a       """stub""".
+0000f320: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
+0000f330: 6562 7567 2822 4635 2043 6c69 636b 6564  ebug("F5 Clicked
+0000f340: 2229 0a20 2020 2020 2020 2069 6620 7365  ").        if se
+0000f350: 6c66 2e6e 316d 6d3a 0a20 2020 2020 2020  lf.n1mm:.       
+0000f360: 2020 2020 2073 656c 662e 6e31 6d6d 2e72       self.n1mm.r
+0000f370: 6164 696f 5f69 6e66 6f5b 2246 756e 6374  adio_info["Funct
+0000f380: 696f 6e4b 6579 4361 7074 696f 6e22 5d20  ionKeyCaption"] 
+0000f390: 3d20 7365 6c66 2e46 352e 7465 7874 2829  = self.F5.text()
+0000f3a0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+0000f3b0: 2e72 6164 696f 5f73 7461 7465 2e67 6574  .radio_state.get
+0000f3c0: 2822 6d6f 6465 2229 2069 6e20 5b22 4c53  ("mode") in ["LS
+0000f3d0: 4222 2c20 2255 5342 222c 2022 5353 4222  B", "USB", "SSB"
+0000f3e0: 5d3a 0a20 2020 2020 2020 2020 2020 2073  ]:.            s
+0000f3f0: 656c 662e 766f 6963 655f 7374 7269 6e67  elf.voice_string
+0000f400: 2873 656c 662e 7072 6f63 6573 735f 6d61  (self.process_ma
+0000f410: 6372 6f28 7365 6c66 2e46 352e 746f 6f6c  cro(self.F5.tool
+0000f420: 5469 7028 2929 290a 2020 2020 2020 2020  Tip())).        
+0000f430: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
+0000f440: 2020 2069 6620 7365 6c66 2e63 773a 0a20     if self.cw:. 
+0000f450: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000f460: 6377 2e73 656e 6463 7728 7365 6c66 2e70  cw.sendcw(self.p
+0000f470: 726f 6365 7373 5f6d 6163 726f 2873 656c  rocess_macro(sel
+0000f480: 662e 4635 2e74 6f6f 6c54 6970 2829 2929  f.F5.toolTip()))
+0000f490: 0a0a 2020 2020 6465 6620 7365 6e64 6636  ..    def sendf6
+0000f4a0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0000f4b0: 2222 2273 7475 6222 2222 0a20 2020 2020  """stub""".     
+0000f4c0: 2020 206c 6f67 6765 722e 6465 6275 6728     logger.debug(
+0000f4d0: 2246 3620 436c 6963 6b65 6422 290a 2020  "F6 Clicked").  
+0000f4e0: 2020 2020 2020 6966 2073 656c 662e 6e31        if self.n1
+0000f4f0: 6d6d 3a0a 2020 2020 2020 2020 2020 2020  mm:.            
+0000f500: 7365 6c66 2e6e 316d 6d2e 7261 6469 6f5f  self.n1mm.radio_
+0000f510: 696e 666f 5b22 4675 6e63 7469 6f6e 4b65  info["FunctionKe
+0000f520: 7943 6170 7469 6f6e 225d 203d 2073 656c  yCaption"] = sel
+0000f530: 662e 4636 2e74 6578 7428 290a 2020 2020  f.F6.text().    
+0000f540: 2020 2020 6966 2073 656c 662e 7261 6469      if self.radi
+0000f550: 6f5f 7374 6174 652e 6765 7428 226d 6f64  o_state.get("mod
+0000f560: 6522 2920 696e 205b 224c 5342 222c 2022  e") in ["LSB", "
+0000f570: 5553 4222 2c20 2253 5342 225d 3a0a 2020  USB", "SSB"]:.  
+0000f580: 2020 2020 2020 2020 2020 7365 6c66 2e76            self.v
+0000f590: 6f69 6365 5f73 7472 696e 6728 7365 6c66  oice_string(self
+0000f5a0: 2e70 726f 6365 7373 5f6d 6163 726f 2873  .process_macro(s
+0000f5b0: 656c 662e 4636 2e74 6f6f 6c54 6970 2829  elf.F6.toolTip()
+0000f5c0: 2929 0a20 2020 2020 2020 2020 2020 2072  )).            r
+0000f5d0: 6574 7572 6e0a 2020 2020 2020 2020 6966  eturn.        if
+0000f5e0: 2073 656c 662e 6377 3a0a 2020 2020 2020   self.cw:.      
+0000f5f0: 2020 2020 2020 7365 6c66 2e63 772e 7365        self.cw.se
+0000f600: 6e64 6377 2873 656c 662e 7072 6f63 6573  ndcw(self.proces
+0000f610: 735f 6d61 6372 6f28 7365 6c66 2e46 362e  s_macro(self.F6.
+0000f620: 746f 6f6c 5469 7028 2929 290a 0a20 2020  toolTip()))..   
+0000f630: 2064 6566 2073 656e 6466 3728 7365 6c66   def sendf7(self
+0000f640: 293a 0a20 2020 2020 2020 2022 2222 7374  ):.        """st
+0000f650: 7562 2222 220a 2020 2020 2020 2020 6c6f  ub""".        lo
+0000f660: 6767 6572 2e64 6562 7567 2822 4637 2043  gger.debug("F7 C
+0000f670: 6c69 636b 6564 2229 0a20 2020 2020 2020  licked").       
+0000f680: 2069 6620 7365 6c66 2e6e 316d 6d3a 0a20   if self.n1mm:. 
+0000f690: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000f6a0: 6e31 6d6d 2e72 6164 696f 5f69 6e66 6f5b  n1mm.radio_info[
+0000f6b0: 2246 756e 6374 696f 6e4b 6579 4361 7074  "FunctionKeyCapt
+0000f6c0: 696f 6e22 5d20 3d20 7365 6c66 2e46 372e  ion"] = self.F7.
+0000f6d0: 7465 7874 2829 0a20 2020 2020 2020 2069  text().        i
+0000f6e0: 6620 7365 6c66 2e72 6164 696f 5f73 7461  f self.radio_sta
+0000f6f0: 7465 2e67 6574 2822 6d6f 6465 2229 2069  te.get("mode") i
+0000f700: 6e20 5b22 4c53 4222 2c20 2255 5342 222c  n ["LSB", "USB",
+0000f710: 2022 5353 4222 5d3a 0a20 2020 2020 2020   "SSB"]:.       
+0000f720: 2020 2020 2073 656c 662e 766f 6963 655f       self.voice_
+0000f730: 7374 7269 6e67 2873 656c 662e 7072 6f63  string(self.proc
+0000f740: 6573 735f 6d61 6372 6f28 7365 6c66 2e46  ess_macro(self.F
+0000f750: 372e 746f 6f6c 5469 7028 2929 290a 2020  7.toolTip())).  
+0000f760: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0000f770: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+0000f780: 2e63 773a 0a20 2020 2020 2020 2020 2020  .cw:.           
+0000f790: 2073 656c 662e 6377 2e73 656e 6463 7728   self.cw.sendcw(
+0000f7a0: 7365 6c66 2e70 726f 6365 7373 5f6d 6163  self.process_mac
+0000f7b0: 726f 2873 656c 662e 4637 2e74 6f6f 6c54  ro(self.F7.toolT
+0000f7c0: 6970 2829 2929 0a0a 2020 2020 6465 6620  ip()))..    def 
+0000f7d0: 7365 6e64 6638 2873 656c 6629 3a0a 2020  sendf8(self):.  
+0000f7e0: 2020 2020 2020 2222 2273 7475 6222 2222        """stub"""
+0000f7f0: 0a20 2020 2020 2020 206c 6f67 6765 722e  .        logger.
+0000f800: 6465 6275 6728 2246 3820 436c 6963 6b65  debug("F8 Clicke
+0000f810: 6422 290a 2020 2020 2020 2020 6966 2073  d").        if s
+0000f820: 656c 662e 6e31 6d6d 3a0a 2020 2020 2020  elf.n1mm:.      
+0000f830: 2020 2020 2020 7365 6c66 2e6e 316d 6d2e        self.n1mm.
+0000f840: 7261 6469 6f5f 696e 666f 5b22 4675 6e63  radio_info["Func
+0000f850: 7469 6f6e 4b65 7943 6170 7469 6f6e 225d  tionKeyCaption"]
+0000f860: 203d 2073 656c 662e 4638 2e74 6578 7428   = self.F8.text(
+0000f870: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
+0000f880: 662e 7261 6469 6f5f 7374 6174 652e 6765  f.radio_state.ge
+0000f890: 7428 226d 6f64 6522 2920 696e 205b 224c  t("mode") in ["L
+0000f8a0: 5342 222c 2022 5553 4222 2c20 2253 5342  SB", "USB", "SSB
+0000f8b0: 225d 3a0a 2020 2020 2020 2020 2020 2020  "]:.            
+0000f8c0: 7365 6c66 2e76 6f69 6365 5f73 7472 696e  self.voice_strin
+0000f8d0: 6728 7365 6c66 2e70 726f 6365 7373 5f6d  g(self.process_m
+0000f8e0: 6163 726f 2873 656c 662e 4638 2e74 6f6f  acro(self.F8.too
+0000f8f0: 6c54 6970 2829 2929 0a20 2020 2020 2020  lTip())).       
+0000f900: 2020 2020 2072 6574 7572 6e0a 2020 2020       return.    
+0000f910: 2020 2020 6966 2073 656c 662e 6377 3a0a      if self.cw:.
+0000f920: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000f930: 2e63 772e 7365 6e64 6377 2873 656c 662e  .cw.sendcw(self.
+0000f940: 7072 6f63 6573 735f 6d61 6372 6f28 7365  process_macro(se
+0000f950: 6c66 2e46 382e 746f 6f6c 5469 7028 2929  lf.F8.toolTip())
+0000f960: 290a 0a20 2020 2064 6566 2073 656e 6466  )..    def sendf
+0000f970: 3928 7365 6c66 293a 0a20 2020 2020 2020  9(self):.       
+0000f980: 2022 2222 7374 7562 2222 220a 2020 2020   """stub""".    
+0000f990: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
+0000f9a0: 2822 4639 2043 6c69 636b 6564 2229 0a20  ("F9 Clicked"). 
+0000f9b0: 2020 2020 2020 2069 6620 7365 6c66 2e6e         if self.n
+0000f9c0: 316d 6d3a 0a20 2020 2020 2020 2020 2020  1mm:.           
+0000f9d0: 2073 656c 662e 6e31 6d6d 2e72 6164 696f   self.n1mm.radio
+0000f9e0: 5f69 6e66 6f5b 2246 756e 6374 696f 6e4b  _info["FunctionK
+0000f9f0: 6579 4361 7074 696f 6e22 5d20 3d20 7365  eyCaption"] = se
+0000fa00: 6c66 2e46 392e 7465 7874 2829 0a20 2020  lf.F9.text().   
+0000fa10: 2020 2020 2069 6620 7365 6c66 2e72 6164       if self.rad
+0000fa20: 696f 5f73 7461 7465 2e67 6574 2822 6d6f  io_state.get("mo
+0000fa30: 6465 2229 2069 6e20 5b22 4c53 4222 2c20  de") in ["LSB", 
+0000fa40: 2255 5342 222c 2022 5353 4222 5d3a 0a20  "USB", "SSB"]:. 
+0000fa50: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000fa60: 766f 6963 655f 7374 7269 6e67 2873 656c  voice_string(sel
+0000fa70: 662e 7072 6f63 6573 735f 6d61 6372 6f28  f.process_macro(
+0000fa80: 7365 6c66 2e46 392e 746f 6f6c 5469 7028  self.F9.toolTip(
+0000fa90: 2929 290a 2020 2020 2020 2020 2020 2020  ))).            
+0000faa0: 7265 7475 726e 0a20 2020 2020 2020 2069  return.        i
+0000fab0: 6620 7365 6c66 2e63 773a 0a20 2020 2020  f self.cw:.     
+0000fac0: 2020 2020 2020 2073 656c 662e 6377 2e73         self.cw.s
+0000fad0: 656e 6463 7728 7365 6c66 2e70 726f 6365  endcw(self.proce
+0000fae0: 7373 5f6d 6163 726f 2873 656c 662e 4639  ss_macro(self.F9
+0000faf0: 2e74 6f6f 6c54 6970 2829 2929 0a0a 2020  .toolTip()))..  
+0000fb00: 2020 6465 6620 7365 6e64 6631 3028 7365    def sendf10(se
+0000fb10: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
+0000fb20: 7374 7562 2222 220a 2020 2020 2020 2020  stub""".        
+0000fb30: 6c6f 6767 6572 2e64 6562 7567 2822 4631  logger.debug("F1
+0000fb40: 3020 436c 6963 6b65 6422 290a 2020 2020  0 Clicked").    
+0000fb50: 2020 2020 6966 2073 656c 662e 6e31 6d6d      if self.n1mm
+0000fb60: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0000fb70: 6c66 2e6e 316d 6d2e 7261 6469 6f5f 696e  lf.n1mm.radio_in
+0000fb80: 666f 5b22 4675 6e63 7469 6f6e 4b65 7943  fo["FunctionKeyC
+0000fb90: 6170 7469 6f6e 225d 203d 2073 656c 662e  aption"] = self.
+0000fba0: 4631 302e 7465 7874 2829 0a20 2020 2020  F10.text().     
+0000fbb0: 2020 2069 6620 7365 6c66 2e72 6164 696f     if self.radio
+0000fbc0: 5f73 7461 7465 2e67 6574 2822 6d6f 6465  _state.get("mode
+0000fbd0: 2229 2069 6e20 5b22 4c53 4222 2c20 2255  ") in ["LSB", "U
+0000fbe0: 5342 222c 2022 5353 4222 5d3a 0a20 2020  SB", "SSB"]:.   
+0000fbf0: 2020 2020 2020 2020 2073 656c 662e 766f           self.vo
+0000fc00: 6963 655f 7374 7269 6e67 2873 656c 662e  ice_string(self.
+0000fc10: 7072 6f63 6573 735f 6d61 6372 6f28 7365  process_macro(se
+0000fc20: 6c66 2e46 3130 2e74 6f6f 6c54 6970 2829  lf.F10.toolTip()
+0000fc30: 2929 0a20 2020 2020 2020 2020 2020 2072  )).            r
+0000fc40: 6574 7572 6e0a 2020 2020 2020 2020 6966  eturn.        if
+0000fc50: 2073 656c 662e 6377 3a0a 2020 2020 2020   self.cw:.      
+0000fc60: 2020 2020 2020 7365 6c66 2e63 772e 7365        self.cw.se
+0000fc70: 6e64 6377 2873 656c 662e 7072 6f63 6573  ndcw(self.proces
+0000fc80: 735f 6d61 6372 6f28 7365 6c66 2e46 3130  s_macro(self.F10
+0000fc90: 2e74 6f6f 6c54 6970 2829 2929 0a0a 2020  .toolTip()))..  
+0000fca0: 2020 6465 6620 7365 6e64 6631 3128 7365    def sendf11(se
+0000fcb0: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
+0000fcc0: 7374 7562 2222 220a 2020 2020 2020 2020  stub""".        
+0000fcd0: 6c6f 6767 6572 2e64 6562 7567 2822 4631  logger.debug("F1
+0000fce0: 3120 436c 6963 6b65 6422 290a 2020 2020  1 Clicked").    
+0000fcf0: 2020 2020 6966 2073 656c 662e 6e31 6d6d      if self.n1mm
+0000fd00: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0000fd10: 6c66 2e6e 316d 6d2e 7261 6469 6f5f 696e  lf.n1mm.radio_in
+0000fd20: 666f 5b22 4675 6e63 7469 6f6e 4b65 7943  fo["FunctionKeyC
+0000fd30: 6170 7469 6f6e 225d 203d 2073 656c 662e  aption"] = self.
+0000fd40: 4631 312e 7465 7874 2829 0a20 2020 2020  F11.text().     
+0000fd50: 2020 2069 6620 7365 6c66 2e72 6164 696f     if self.radio
+0000fd60: 5f73 7461 7465 2e67 6574 2822 6d6f 6465  _state.get("mode
+0000fd70: 2229 2069 6e20 5b22 4c53 4222 2c20 2255  ") in ["LSB", "U
+0000fd80: 5342 222c 2022 5353 4222 5d3a 0a20 2020  SB", "SSB"]:.   
+0000fd90: 2020 2020 2020 2020 2073 656c 662e 766f           self.vo
+0000fda0: 6963 655f 7374 7269 6e67 2873 656c 662e  ice_string(self.
+0000fdb0: 7072 6f63 6573 735f 6d61 6372 6f28 7365  process_macro(se
+0000fdc0: 6c66 2e46 3131 2e74 6f6f 6c54 6970 2829  lf.F11.toolTip()
+0000fdd0: 2929 0a20 2020 2020 2020 2020 2020 2072  )).            r
+0000fde0: 6574 7572 6e0a 2020 2020 2020 2020 6966  eturn.        if
+0000fdf0: 2073 656c 662e 6377 3a0a 2020 2020 2020   self.cw:.      
+0000fe00: 2020 2020 2020 7365 6c66 2e63 772e 7365        self.cw.se
+0000fe10: 6e64 6377 2873 656c 662e 7072 6f63 6573  ndcw(self.proces
+0000fe20: 735f 6d61 6372 6f28 7365 6c66 2e46 3131  s_macro(self.F11
+0000fe30: 2e74 6f6f 6c54 6970 2829 2929 0a0a 2020  .toolTip()))..  
+0000fe40: 2020 6465 6620 7365 6e64 6631 3228 7365    def sendf12(se
+0000fe50: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
+0000fe60: 7374 7562 2222 220a 2020 2020 2020 2020  stub""".        
+0000fe70: 6c6f 6767 6572 2e64 6562 7567 2822 4631  logger.debug("F1
+0000fe80: 3220 436c 6963 6b65 6422 290a 2020 2020  2 Clicked").    
+0000fe90: 2020 2020 6966 2073 656c 662e 6e31 6d6d      if self.n1mm
+0000fea0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0000feb0: 6c66 2e6e 316d 6d2e 7261 6469 6f5f 696e  lf.n1mm.radio_in
+0000fec0: 666f 5b22 4675 6e63 7469 6f6e 4b65 7943  fo["FunctionKeyC
+0000fed0: 6170 7469 6f6e 225d 203d 2073 656c 662e  aption"] = self.
+0000fee0: 4631 322e 7465 7874 2829 0a20 2020 2020  F12.text().     
+0000fef0: 2020 2069 6620 7365 6c66 2e72 6164 696f     if self.radio
+0000ff00: 5f73 7461 7465 2e67 6574 2822 6d6f 6465  _state.get("mode
+0000ff10: 2229 2069 6e20 5b22 4c53 4222 2c20 2255  ") in ["LSB", "U
+0000ff20: 5342 222c 2022 5353 4222 5d3a 0a20 2020  SB", "SSB"]:.   
+0000ff30: 2020 2020 2020 2020 2073 656c 662e 766f           self.vo
+0000ff40: 6963 655f 7374 7269 6e67 2873 656c 662e  ice_string(self.
+0000ff50: 7072 6f63 6573 735f 6d61 6372 6f28 7365  process_macro(se
+0000ff60: 6c66 2e46 3132 2e74 6f6f 6c54 6970 2829  lf.F12.toolTip()
+0000ff70: 2929 0a20 2020 2020 2020 2020 2020 2072  )).            r
+0000ff80: 6574 7572 6e0a 2020 2020 2020 2020 6966  eturn.        if
+0000ff90: 2073 656c 662e 6377 3a0a 2020 2020 2020   self.cw:.      
+0000ffa0: 2020 2020 2020 7365 6c66 2e63 772e 7365        self.cw.se
+0000ffb0: 6e64 6377 2873 656c 662e 7072 6f63 6573  ndcw(self.proces
+0000ffc0: 735f 6d61 6372 6f28 7365 6c66 2e46 3132  s_macro(self.F12
+0000ffd0: 2e74 6f6f 6c54 6970 2829 2929 0a0a 2020  .toolTip()))..  
+0000ffe0: 2020 6465 6620 7275 6e5f 7370 5f62 7574    def run_sp_but
+0000fff0: 746f 6e73 5f63 6c69 636b 6564 2873 656c  tons_clicked(sel
+00010000: 6629 3a0a 2020 2020 2020 2020 2222 2248  f):.        """H
+00010010: 616e 646c 6520 7275 6e2f 7326 7020 6d6f  andle run/s&p mo
+00010020: 6465 2222 220a 2020 2020 2020 2020 7365  de""".        se
+00010030: 6c66 2e70 7265 665b 2272 756e 5f73 7461  lf.pref["run_sta
+00010040: 7465 225d 203d 2073 656c 662e 7261 6469  te"] = self.radi
+00010050: 6f42 7574 746f 6e5f 7275 6e2e 6973 4368  oButton_run.isCh
+00010060: 6563 6b65 6428 290a 2020 2020 2020 2020  ecked().        
+00010070: 7365 6c66 2e77 7269 7465 5f70 7265 6665  self.write_prefe
+00010080: 7265 6e63 6528 290a 2020 2020 2020 2020  rence().        
+00010090: 7365 6c66 2e72 6561 645f 6377 5f6d 6163  self.read_cw_mac
+000100a0: 726f 7328 290a 0a20 2020 2064 6566 2077  ros()..    def w
+000100b0: 7269 7465 5f70 7265 6665 7265 6e63 6528  rite_preference(
+000100c0: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
+000100d0: 2222 0a20 2020 2020 2020 2057 7269 7465  "".        Write
+000100e0: 2070 7265 6665 7265 6e63 6573 2074 6f20   preferences to 
+000100f0: 6a73 6f6e 2066 696c 652e 0a20 2020 2020  json file..     
+00010100: 2020 2022 2222 0a20 2020 2020 2020 2074     """.        t
+00010110: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
+00010120: 7769 7468 206f 7065 6e28 0a20 2020 2020  with open(.     
+00010130: 2020 2020 2020 2020 2020 2043 4f4e 4649             CONFI
+00010140: 475f 5041 5448 202b 2022 2f6e 6f74 316d  G_PATH + "/not1m
+00010150: 6d2e 6a73 6f6e 222c 2022 7774 222c 2065  m.json", "wt", e
+00010160: 6e63 6f64 696e 673d 2275 7466 2d38 220a  ncoding="utf-8".
+00010170: 2020 2020 2020 2020 2020 2020 2920 6173              ) as
+00010180: 2066 696c 655f 6465 7363 7269 7074 6f72   file_descriptor
+00010190: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000101a0: 2020 6669 6c65 5f64 6573 6372 6970 746f    file_descripto
+000101b0: 722e 7772 6974 6528 6475 6d70 7328 7365  r.write(dumps(se
+000101c0: 6c66 2e70 7265 662c 2069 6e64 656e 743d  lf.pref, indent=
+000101d0: 3429 290a 2020 2020 2020 2020 2020 2020  4)).            
+000101e0: 2020 2020 6c6f 6767 6572 2e69 6e66 6f28      logger.info(
+000101f0: 2277 7269 7469 6e67 3a20 2573 222c 2073  "writing: %s", s
+00010200: 656c 662e 7072 6566 290a 2020 2020 2020  elf.pref).      
+00010210: 2020 6578 6365 7074 2049 4f45 7272 6f72    except IOError
+00010220: 2061 7320 6578 6365 7074 696f 6e3a 0a20   as exception:. 
+00010230: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
+00010240: 722e 6372 6974 6963 616c 2822 7772 6974  r.critical("writ
+00010250: 6570 7265 6665 7265 6e63 6573 3a20 2573  epreferences: %s
+00010260: 222c 2065 7863 6570 7469 6f6e 290a 0a20  ", exception).. 
+00010270: 2020 2064 6566 2072 6561 6470 7265 6665     def readprefe
+00010280: 7265 6e63 6573 2873 656c 6629 3a0a 2020  rences(self):.  
+00010290: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+000102a0: 2020 5265 7374 6f72 6520 7072 6566 6572    Restore prefer
+000102b0: 656e 6365 7320 6966 2074 6865 7920 6578  ences if they ex
+000102c0: 6973 742c 206f 7468 6572 7769 7365 2063  ist, otherwise c
+000102d0: 7265 6174 6520 736f 6d65 2073 616e 6520  reate some sane 
+000102e0: 6465 6661 756c 7473 2e0a 2020 2020 2020  defaults..      
+000102f0: 2020 2222 220a 2020 2020 2020 2020 7472    """.        tr
+00010300: 793a 0a20 2020 2020 2020 2020 2020 2069  y:.            i
+00010310: 6620 6f73 2e70 6174 682e 6578 6973 7473  f os.path.exists
+00010320: 2843 4f4e 4649 475f 5041 5448 202b 2022  (CONFIG_PATH + "
+00010330: 2f6e 6f74 316d 6d2e 6a73 6f6e 2229 3a0a  /not1mm.json"):.
+00010340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010350: 7769 7468 206f 7065 6e28 0a20 2020 2020  with open(.     
+00010360: 2020 2020 2020 2020 2020 2020 2020 2043                 C
+00010370: 4f4e 4649 475f 5041 5448 202b 2022 2f6e  ONFIG_PATH + "/n
+00010380: 6f74 316d 6d2e 6a73 6f6e 222c 2022 7274  ot1mm.json", "rt
+00010390: 222c 2065 6e63 6f64 696e 673d 2275 7466  ", encoding="utf
+000103a0: 2d38 220a 2020 2020 2020 2020 2020 2020  -8".            
+000103b0: 2020 2020 2920 6173 2066 696c 655f 6465      ) as file_de
+000103c0: 7363 7269 7074 6f72 3a0a 2020 2020 2020  scriptor:.      
+000103d0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000103e0: 6c66 2e70 7265 6620 3d20 6c6f 6164 7328  lf.pref = loads(
+000103f0: 6669 6c65 5f64 6573 6372 6970 746f 722e  file_descriptor.
+00010400: 7265 6164 2829 290a 2020 2020 2020 2020  read()).        
+00010410: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
+00010420: 6572 2e69 6e66 6f28 2225 7322 2c20 7365  er.info("%s", se
+00010430: 6c66 2e70 7265 6629 0a20 2020 2020 2020  lf.pref).       
+00010440: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00010450: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
+00010460: 722e 696e 666f 2822 4e6f 2070 7265 6665  r.info("No prefe
+00010470: 7265 6e63 6520 6669 6c65 2e20 5772 6974  rence file. Writ
+00010480: 696e 6720 7072 6566 6572 656e 6365 2e22  ing preference."
+00010490: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+000104a0: 2020 7769 7468 206f 7065 6e28 0a20 2020    with open(.   
+000104b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000104c0: 2043 4f4e 4649 475f 5041 5448 202b 2022   CONFIG_PATH + "
+000104d0: 2f6e 6f74 316d 6d2e 6a73 6f6e 222c 2022  /not1mm.json", "
+000104e0: 7774 222c 2065 6e63 6f64 696e 673d 2275  wt", encoding="u
+000104f0: 7466 2d38 220a 2020 2020 2020 2020 2020  tf-8".          
+00010500: 2020 2020 2020 2920 6173 2066 696c 655f        ) as file_
+00010510: 6465 7363 7269 7074 6f72 3a0a 2020 2020  descriptor:.    
+00010520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010530: 7365 6c66 2e70 7265 6620 3d20 7365 6c66  self.pref = self
+00010540: 2e70 7265 665f 7265 662e 636f 7079 2829  .pref_ref.copy()
+00010550: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010560: 2020 2020 2066 696c 655f 6465 7363 7269       file_descri
+00010570: 7074 6f72 2e77 7269 7465 2864 756d 7073  ptor.write(dumps
+00010580: 2873 656c 662e 7072 6566 2c20 696e 6465  (self.pref, inde
+00010590: 6e74 3d34 2929 0a20 2020 2020 2020 2020  nt=4)).         
+000105a0: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
+000105b0: 722e 696e 666f 2822 2573 222c 2073 656c  r.info("%s", sel
+000105c0: 662e 7072 6566 290a 2020 2020 2020 2020  f.pref).        
+000105d0: 6578 6365 7074 2049 4f45 7272 6f72 2061  except IOError a
+000105e0: 7320 6578 6365 7074 696f 6e3a 0a20 2020  s exception:.   
+000105f0: 2020 2020 2020 2020 206c 6f67 6765 722e           logger.
+00010600: 6372 6974 6963 616c 2822 4572 726f 723a  critical("Error:
+00010610: 2025 7322 2c20 6578 6365 7074 696f 6e29   %s", exception)
+00010620: 0a0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
+00010630: 6f6f 6b5f 7570 203d 204e 6f6e 650a 2020  ook_up = None.  
+00010640: 2020 2020 2020 6966 2073 656c 662e 7072        if self.pr
+00010650: 6566 2e67 6574 2822 7573 6571 727a 2229  ef.get("useqrz")
+00010660: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00010670: 6c66 2e6c 6f6f 6b5f 7570 203d 2051 525a  lf.look_up = QRZ
+00010680: 6c6f 6f6b 7570 280a 2020 2020 2020 2020  lookup(.        
+00010690: 2020 2020 2020 2020 7365 6c66 2e70 7265          self.pre
+000106a0: 662e 6765 7428 226c 6f6f 6b75 7075 7365  f.get("lookupuse
+000106b0: 726e 616d 6522 292c 0a20 2020 2020 2020  rname"),.       
+000106c0: 2020 2020 2020 2020 2073 656c 662e 7072           self.pr
+000106d0: 6566 2e67 6574 2822 6c6f 6f6b 7570 7061  ef.get("lookuppa
+000106e0: 7373 776f 7264 2229 2c0a 2020 2020 2020  ssword"),.      
+000106f0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00010700: 2320 6966 2073 656c 662e 7072 6566 2e67  # if self.pref.g
+00010710: 6574 2822 7573 6568 616d 6462 2229 3a0a  et("usehamdb"):.
+00010720: 2020 2020 2020 2020 2320 2020 2020 7365          #     se
+00010730: 6c66 2e6c 6f6f 6b5f 7570 203d 2048 616d  lf.look_up = Ham
+00010740: 4442 6c6f 6f6b 7570 2829 0a20 2020 2020  DBlookup().     
+00010750: 2020 2069 6620 7365 6c66 2e70 7265 662e     if self.pref.
+00010760: 6765 7428 2275 7365 6861 6d71 7468 2229  get("usehamqth")
+00010770: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00010780: 6c66 2e6c 6f6f 6b5f 7570 203d 2048 616d  lf.look_up = Ham
+00010790: 5154 4828 0a20 2020 2020 2020 2020 2020  QTH(.           
+000107a0: 2020 2020 2073 656c 662e 7072 6566 2e67       self.pref.g
+000107b0: 6574 2822 6c6f 6f6b 7570 7573 6572 6e61  et("lookupuserna
+000107c0: 6d65 2229 2c0a 2020 2020 2020 2020 2020  me"),.          
+000107d0: 2020 2020 2020 7365 6c66 2e70 7265 662e        self.pref.
+000107e0: 6765 7428 226c 6f6f 6b75 7070 6173 7377  get("lookuppassw
+000107f0: 6f72 6422 292c 0a20 2020 2020 2020 2020  ord"),.         
+00010800: 2020 2029 0a0a 2020 2020 2020 2020 6966     )..        if
+00010810: 2073 656c 662e 7072 6566 2e67 6574 2822   self.pref.get("
+00010820: 7275 6e5f 7374 6174 6522 293a 0a20 2020  run_state"):.   
+00010830: 2020 2020 2020 2020 2073 656c 662e 7261           self.ra
+00010840: 6469 6f42 7574 746f 6e5f 7275 6e2e 7365  dioButton_run.se
+00010850: 7443 6865 636b 6564 2854 7275 6529 0a20  tChecked(True). 
+00010860: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00010870: 2020 2020 2020 2020 2073 656c 662e 7261           self.ra
+00010880: 6469 6f42 7574 746f 6e5f 7370 2e73 6574  dioButton_sp.set
+00010890: 4368 6563 6b65 6428 5472 7565 290a 0a20  Checked(True).. 
+000108a0: 2020 2020 2020 2069 6620 7365 6c66 2e70         if self.p
+000108b0: 7265 662e 6765 7428 2263 6f6d 6d61 6e64  ref.get("command
+000108c0: 5f62 7574 746f 6e73 2229 3a0a 2020 2020  _buttons"):.    
+000108d0: 2020 2020 2020 2020 7365 6c66 2e61 6374          self.act
+000108e0: 696f 6e43 6f6d 6d61 6e64 5f42 7574 746f  ionCommand_Butto
+000108f0: 6e73 2e73 6574 4368 6563 6b65 6428 5472  ns.setChecked(Tr
+00010900: 7565 290a 2020 2020 2020 2020 656c 7365  ue).        else
+00010910: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00010920: 6c66 2e61 6374 696f 6e43 6f6d 6d61 6e64  lf.actionCommand
+00010930: 5f42 7574 746f 6e73 2e73 6574 4368 6563  _Buttons.setChec
+00010940: 6b65 6428 4661 6c73 6529 0a0a 2020 2020  ked(False)..    
+00010950: 2020 2020 6966 2073 656c 662e 7072 6566      if self.pref
+00010960: 2e67 6574 2822 6377 5f6d 6163 726f 7322  .get("cw_macros"
+00010970: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
+00010980: 656c 662e 6163 7469 6f6e 4357 5f4d 6163  elf.actionCW_Mac
+00010990: 726f 732e 7365 7443 6865 636b 6564 2854  ros.setChecked(T
+000109a0: 7275 6529 0a20 2020 2020 2020 2065 6c73  rue).        els
+000109b0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+000109c0: 656c 662e 6163 7469 6f6e 4357 5f4d 6163  elf.actionCW_Mac
+000109d0: 726f 732e 7365 7443 6865 636b 6564 2846  ros.setChecked(F
+000109e0: 616c 7365 290a 0a20 2020 2020 2020 2069  alse)..        i
+000109f0: 6620 7365 6c66 2e70 7265 662e 6765 7428  f self.pref.get(
+00010a00: 2262 616e 6473 5f6d 6f64 6573 2229 3a0a  "bands_modes"):.
+00010a10: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00010a20: 2e61 6374 696f 6e4d 6f64 655f 616e 645f  .actionMode_and_
+00010a30: 4261 6e64 732e 7365 7443 6865 636b 6564  Bands.setChecked
+00010a40: 2854 7275 6529 0a20 2020 2020 2020 2065  (True).        e
+00010a50: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00010a60: 2073 656c 662e 6163 7469 6f6e 4d6f 6465   self.actionMode
+00010a70: 5f61 6e64 5f42 616e 6473 2e73 6574 4368  _and_Bands.setCh
+00010a80: 6563 6b65 6428 4661 6c73 6529 0a0a 2020  ecked(False)..  
+00010a90: 2020 2020 2020 6d75 6c74 6963 6173 745f        multicast_
+00010aa0: 6772 6f75 7020 3d20 7365 6c66 2e70 7265  group = self.pre
+00010ab0: 662e 6765 7428 226d 756c 7469 6361 7374  f.get("multicast
+00010ac0: 5f67 726f 7570 222c 2022 3233 392e 312e  _group", "239.1.
+00010ad0: 312e 3122 290a 2020 2020 2020 2020 6d75  1.1").        mu
+00010ae0: 6c74 6963 6173 745f 706f 7274 203d 2073  lticast_port = s
+00010af0: 656c 662e 7072 6566 2e67 6574 2822 6d75  elf.pref.get("mu
+00010b00: 6c74 6963 6173 745f 706f 7274 222c 2032  lticast_port", 2
+00010b10: 3233 3929 0a20 2020 2020 2020 2069 6e74  239).        int
+00010b20: 6572 6661 6365 5f69 7020 3d20 7365 6c66  erface_ip = self
+00010b30: 2e70 7265 662e 6765 7428 2269 6e74 6572  .pref.get("inter
+00010b40: 6661 6365 5f69 7022 2c20 2230 2e30 2e30  face_ip", "0.0.0
+00010b50: 2e30 2229 0a20 2020 2020 2020 2073 656c  .0").        sel
+00010b60: 662e 6d75 6c74 6963 6173 745f 696e 7465  f.multicast_inte
+00010b70: 7266 6163 6520 3d20 4d75 6c74 6963 6173  rface = Multicas
+00010b80: 7428 0a20 2020 2020 2020 2020 2020 206d  t(.            m
+00010b90: 756c 7469 6361 7374 5f67 726f 7570 2c20  ulticast_group, 
+00010ba0: 6d75 6c74 6963 6173 745f 706f 7274 2c20  multicast_port, 
+00010bb0: 696e 7465 7266 6163 655f 6970 0a20 2020  interface_ip.   
+00010bc0: 2020 2020 2029 0a20 2020 2020 2020 2073       ).        s
+00010bd0: 656c 662e 6d75 6c74 6963 6173 745f 696e  elf.multicast_in
+00010be0: 7465 7266 6163 652e 7265 6164 795f 7265  terface.ready_re
+00010bf0: 6164 5f63 6f6e 6e65 6374 2873 656c 662e  ad_connect(self.
+00010c00: 7761 7463 685f 7564 7029 0a0a 2020 2020  watch_udp)..    
+00010c10: 2020 2020 7365 6c66 2e72 6967 5f63 6f6e      self.rig_con
+00010c20: 7472 6f6c 203d 204e 6f6e 650a 0a20 2020  trol = None..   
+00010c30: 2020 2020 2069 6620 7365 6c66 2e70 7265       if self.pre
+00010c40: 662e 6765 7428 2275 7365 666c 7269 6722  f.get("useflrig"
+00010c50: 2c20 4661 6c73 6529 3a0a 2020 2020 2020  , False):.      
+00010c60: 2020 2020 2020 6c6f 6767 6572 2e64 6562        logger.deb
+00010c70: 7567 280a 2020 2020 2020 2020 2020 2020  ug(.            
+00010c80: 2020 2020 2255 7369 6e67 2066 6c72 6967      "Using flrig
+00010c90: 3a20 2573 222c 0a20 2020 2020 2020 2020  : %s",.         
+00010ca0: 2020 2020 2020 2066 227b 7365 6c66 2e70         f"{self.p
+00010cb0: 7265 662e 6765 7428 2743 4154 5f69 7027  ref.get('CAT_ip'
+00010cc0: 297d 207b 7365 6c66 2e70 7265 662e 6765  )} {self.pref.ge
+00010cd0: 7428 2743 4154 5f70 6f72 7427 297d 222c  t('CAT_port')}",
+00010ce0: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
+00010cf0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00010d00: 7269 675f 636f 6e74 726f 6c20 3d20 4341  rig_control = CA
+00010d10: 5428 0a20 2020 2020 2020 2020 2020 2020  T(.             
+00010d20: 2020 2022 666c 7269 6722 2c0a 2020 2020     "flrig",.    
+00010d30: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00010d40: 2e70 7265 662e 6765 7428 2243 4154 5f69  .pref.get("CAT_i
+00010d50: 7022 2c20 2231 3237 2e30 2e30 2e31 2229  p", "127.0.0.1")
+00010d60: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00010d70: 2020 696e 7428 7365 6c66 2e70 7265 662e    int(self.pref.
+00010d80: 6765 7428 2243 4154 5f70 6f72 7422 2c20  get("CAT_port", 
+00010d90: 3132 3334 3529 292c 0a20 2020 2020 2020  12345)),.       
+00010da0: 2020 2020 2029 0a20 2020 2020 2020 2069       ).        i
+00010db0: 6620 7365 6c66 2e70 7265 662e 6765 7428  f self.pref.get(
+00010dc0: 2275 7365 7269 6763 746c 6422 2c20 4661  "userigctld", Fa
+00010dd0: 6c73 6529 3a0a 2020 2020 2020 2020 2020  lse):.          
+00010de0: 2020 6c6f 6767 6572 2e64 6562 7567 280a    logger.debug(.
+00010df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010e00: 2255 7369 6e67 2072 6967 6374 6c64 3a20  "Using rigctld: 
+00010e10: 2573 222c 0a20 2020 2020 2020 2020 2020  %s",.           
+00010e20: 2020 2020 2066 227b 7365 6c66 2e70 7265       f"{self.pre
+00010e30: 662e 6765 7428 2743 4154 5f69 7027 297d  f.get('CAT_ip')}
+00010e40: 207b 7365 6c66 2e70 7265 662e 6765 7428   {self.pref.get(
+00010e50: 2743 4154 5f70 6f72 7427 297d 222c 0a20  'CAT_port')}",. 
+00010e60: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00010e70: 2020 2020 2020 2020 2073 656c 662e 7269           self.ri
+00010e80: 675f 636f 6e74 726f 6c20 3d20 4341 5428  g_control = CAT(
+00010e90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010ea0: 2022 7269 6763 746c 6422 2c0a 2020 2020   "rigctld",.    
+00010eb0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00010ec0: 2e70 7265 662e 6765 7428 2243 4154 5f69  .pref.get("CAT_i
+00010ed0: 7022 2c20 2231 3237 2e30 2e30 2e31 2229  p", "127.0.0.1")
+00010ee0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00010ef0: 2020 696e 7428 7365 6c66 2e70 7265 662e    int(self.pref.
+00010f00: 6765 7428 2243 4154 5f70 6f72 7422 2c20  get("CAT_port", 
+00010f10: 3435 3332 2929 2c0a 2020 2020 2020 2020  4532)),.        
+00010f20: 2020 2020 290a 0a20 2020 2020 2020 2069      )..        i
+00010f30: 6620 7365 6c66 2e70 7265 662e 6765 7428  f self.pref.get(
+00010f40: 2263 7774 7970 6522 2c20 3029 203d 3d20  "cwtype", 0) == 
+00010f50: 303a 0a20 2020 2020 2020 2020 2020 2073  0:.            s
+00010f60: 656c 662e 6377 203d 204e 6f6e 650a 2020  elf.cw = None.  
+00010f70: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00010f80: 2020 2020 2020 2020 7365 6c66 2e63 7720          self.cw 
+00010f90: 3d20 4357 280a 2020 2020 2020 2020 2020  = CW(.          
+00010fa0: 2020 2020 2020 696e 7428 7365 6c66 2e70        int(self.p
+00010fb0: 7265 662e 6765 7428 2263 7774 7970 6522  ref.get("cwtype"
+00010fc0: 2929 2c0a 2020 2020 2020 2020 2020 2020  )),.            
+00010fd0: 2020 2020 7365 6c66 2e70 7265 662e 6765      self.pref.ge
+00010fe0: 7428 2263 7769 7022 292c 0a20 2020 2020  t("cwip"),.     
+00010ff0: 2020 2020 2020 2020 2020 2069 6e74 2873             int(s
+00011000: 656c 662e 7072 6566 2e67 6574 2822 6377  elf.pref.get("cw
+00011010: 706f 7274 222c 2036 3738 3929 292c 0a20  port", 6789)),. 
+00011020: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00011030: 2020 2020 2020 2020 2073 656c 662e 6377           self.cw
+00011040: 2e73 7065 6564 203d 2032 300a 2020 2020  .speed = 20.    
+00011050: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00011060: 6377 2e73 6572 7665 7274 7970 6520 3d3d  cw.servertype ==
+00011070: 2032 3a0a 2020 2020 2020 2020 2020 2020   2:.            
+00011080: 2020 2020 7365 6c66 2e63 772e 7365 745f      self.cw.set_
+00011090: 7769 6e6b 6579 6572 5f73 7065 6564 2832  winkeyer_speed(2
+000110a0: 3029 0a0a 2020 2020 2020 2020 7365 6c66  0)..        self
+000110b0: 2e6e 316d 6d20 3d20 4e6f 6e65 0a20 2020  .n1mm = None.   
+000110c0: 2020 2020 2069 6620 7365 6c66 2e70 7265       if self.pre
+000110d0: 662e 6765 7428 2273 656e 645f 6e31 6d6d  f.get("send_n1mm
+000110e0: 5f70 6163 6b65 7473 222c 2046 616c 7365  _packets", False
+000110f0: 293a 0a20 2020 2020 2020 2020 2020 2074  ):.            t
+00011100: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
+00011110: 2020 2020 7365 6c66 2e6e 316d 6d20 3d20      self.n1mm = 
+00011120: 4e31 4d4d 280a 2020 2020 2020 2020 2020  N1MM(.          
+00011130: 2020 2020 2020 2020 2020 7365 6c66 2e70            self.p
+00011140: 7265 662e 6765 7428 226e 316d 6d5f 7261  ref.get("n1mm_ra
+00011150: 6469 6f70 6f72 7422 2c20 2231 3237 2e30  dioport", "127.0
+00011160: 2e30 2e31 3a31 3230 3630 2229 2c0a 2020  .0.1:12060"),.  
 00011170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011180: 2020 2073 656c 662e 7072 6566 2e67 6574     self.pref.get
-00011190: 2822 6e31 6d6d 5f6c 6f6f 6b75 7070 6f72  ("n1mm_lookuppor
+00011180: 2020 7365 6c66 2e70 7265 662e 6765 7428    self.pref.get(
+00011190: 226e 316d 6d5f 636f 6e74 6163 7470 6f72  "n1mm_contactpor
 000111a0: 7422 2c20 2231 3237 2e30 2e30 2e31 3a31  t", "127.0.0.1:1
-000111b0: 3230 3630 2229 2c0a 2020 2020 2020 2020  2060"),.        
+000111b0: 3230 3631 2229 2c0a 2020 2020 2020 2020  2061"),.        
 000111c0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
 000111d0: 2e70 7265 662e 6765 7428 226e 316d 6d5f  .pref.get("n1mm_
-000111e0: 7363 6f72 6570 6f72 7422 2c20 2231 3237  scoreport", "127
-000111f0: 2e30 2e30 2e31 3a31 3230 3630 2229 2c0a  .0.0.1:12060"),.
-00011200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011210: 290a 2020 2020 2020 2020 2020 2020 6578  ).            ex
-00011220: 6365 7074 2056 616c 7565 4572 726f 723a  cept ValueError:
-00011230: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011240: 206c 6f67 6765 722e 7761 726e 696e 6728   logger.warning(
-00011250: 2225 7322 2c20 6622 7b56 616c 7565 4572  "%s", f"{ValueEr
-00011260: 726f 727d 2229 0a20 2020 2020 2020 2020  ror}").         
-00011270: 2020 2073 656c 662e 6e31 6d6d 2e73 656e     self.n1mm.sen
-00011280: 645f 7261 6469 6f5f 7061 636b 6574 7320  d_radio_packets 
-00011290: 3d20 7365 6c66 2e70 7265 662e 6765 7428  = self.pref.get(
-000112a0: 2273 656e 645f 6e31 6d6d 5f72 6164 696f  "send_n1mm_radio
-000112b0: 222c 2046 616c 7365 290a 2020 2020 2020  ", False).      
-000112c0: 2020 2020 2020 7365 6c66 2e6e 316d 6d2e        self.n1mm.
-000112d0: 7365 6e64 5f63 6f6e 7461 6374 5f70 6163  send_contact_pac
-000112e0: 6b65 7473 203d 2073 656c 662e 7072 6566  kets = self.pref
-000112f0: 2e67 6574 2822 7365 6e64 5f6e 316d 6d5f  .get("send_n1mm_
-00011300: 636f 6e74 6163 7422 2c20 4661 6c73 6529  contact", False)
-00011310: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00011320: 662e 6e31 6d6d 2e73 656e 645f 6c6f 6f6b  f.n1mm.send_look
-00011330: 7570 5f70 6163 6b65 7473 203d 2073 656c  up_packets = sel
-00011340: 662e 7072 6566 2e67 6574 2822 7365 6e64  f.pref.get("send
-00011350: 5f6e 316d 6d5f 6c6f 6f6b 7570 222c 2046  _n1mm_lookup", F
-00011360: 616c 7365 290a 2020 2020 2020 2020 2020  alse).          
-00011370: 2020 7365 6c66 2e6e 316d 6d2e 7365 6e64    self.n1mm.send
-00011380: 5f73 636f 7265 5f70 6163 6b65 7473 203d  _score_packets =
-00011390: 2073 656c 662e 7072 6566 2e67 6574 2822   self.pref.get("
-000113a0: 7365 6e64 5f6e 316d 6d5f 7363 6f72 6522  send_n1mm_score"
-000113b0: 2c20 4661 6c73 6529 0a20 2020 2020 2020  , False).       
-000113c0: 2020 2020 2073 656c 662e 6e31 6d6d 2e72       self.n1mm.r
-000113d0: 6164 696f 5f69 6e66 6f5b 2253 7461 7469  adio_info["Stati
-000113e0: 6f6e 4e61 6d65 225d 203d 2073 656c 662e  onName"] = self.
-000113f0: 7072 6566 2e67 6574 2822 6e31 6d6d 5f73  pref.get("n1mm_s
-00011400: 7461 7469 6f6e 5f6e 616d 6522 2c20 2222  tation_name", ""
-00011410: 290a 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00011420: 7368 6f77 5f63 6f6d 6d61 6e64 5f62 7574  show_command_but
-00011430: 746f 6e73 2829 0a20 2020 2020 2020 2073  tons().        s
-00011440: 656c 662e 7368 6f77 5f43 575f 6d61 6372  elf.show_CW_macr
-00011450: 6f73 2829 0a20 2020 2020 2020 2023 2073  os().        # s
-00011460: 656c 662e 7368 6f77 5f62 616e 645f 6d6f  elf.show_band_mo
-00011470: 6465 2829 0a0a 2020 2020 6465 6620 7761  de()..    def wa
-00011480: 7463 685f 7564 7028 7365 6c66 293a 0a20  tch_udp(self):. 
-00011490: 2020 2020 2020 2022 2222 5072 6f63 6573         """Proces
-000114a0: 7320 5544 5020 6461 7461 6772 616d 732e  s UDP datagrams.
-000114b0: 2222 220a 2020 2020 2020 2020 7768 696c  """.        whil
-000114c0: 6520 7365 6c66 2e6d 756c 7469 6361 7374  e self.multicast
-000114d0: 5f69 6e74 6572 6661 6365 2e73 6572 7665  _interface.serve
-000114e0: 725f 7564 702e 6861 7350 656e 6469 6e67  r_udp.hasPending
-000114f0: 4461 7461 6772 616d 7328 293a 0a20 2020  Datagrams():.   
-00011500: 2020 2020 2020 2020 2062 756e 646c 6520           bundle 
-00011510: 3d20 7365 6c66 2e6d 756c 7469 6361 7374  = self.multicast
-00011520: 5f69 6e74 6572 6661 6365 2e73 6572 7665  _interface.serve
-00011530: 725f 7564 702e 7265 6164 4461 7461 6772  r_udp.readDatagr
-00011540: 616d 280a 2020 2020 2020 2020 2020 2020  am(.            
-00011550: 2020 2020 7365 6c66 2e6d 756c 7469 6361      self.multica
-00011560: 7374 5f69 6e74 6572 6661 6365 2e73 6572  st_interface.ser
-00011570: 7665 725f 7564 702e 7065 6e64 696e 6744  ver_udp.pendingD
-00011580: 6174 6167 7261 6d53 697a 6528 290a 2020  atagramSize().  
-00011590: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-000115a0: 2020 2020 2020 2020 6461 7461 6772 616d          datagram
-000115b0: 2c20 5f2c 205f 203d 2062 756e 646c 650a  , _, _ = bundle.
-000115c0: 2020 2020 2020 2020 2020 2020 2320 6c6f              # lo
-000115d0: 6767 6572 2e64 6562 7567 2864 6174 6167  gger.debug(datag
-000115e0: 7261 6d2e 6465 636f 6465 2829 290a 2020  ram.decode()).  
-000115f0: 2020 2020 2020 2020 2020 6966 2064 6174            if dat
-00011600: 6167 7261 6d3a 0a20 2020 2020 2020 2020  agram:.         
-00011610: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
-00011620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011630: 2320 6465 6275 675f 696e 666f 203d 2066  # debug_info = f
-00011640: 227b 6461 7461 6772 616d 2e64 6563 6f64  "{datagram.decod
-00011650: 6528 297d 220a 2020 2020 2020 2020 2020  e()}".          
-00011660: 2020 2020 2020 2020 2020 2320 6c6f 6767            # logg
-00011670: 6572 2e64 6562 7567 2864 6562 7567 5f69  er.debug(debug_i
-00011680: 6e66 6f29 0a20 2020 2020 2020 2020 2020  nfo).           
-00011690: 2020 2020 2020 2020 206a 736f 6e5f 6461           json_da
-000116a0: 7461 203d 206c 6f61 6473 2864 6174 6167  ta = loads(datag
-000116b0: 7261 6d2e 6465 636f 6465 2829 290a 2020  ram.decode()).  
-000116c0: 2020 2020 2020 2020 2020 2020 2020 6578                ex
-000116d0: 6365 7074 2055 6e69 636f 6465 4465 636f  cept UnicodeDeco
-000116e0: 6465 4572 726f 7220 6173 2065 7272 3a0a  deError as err:.
-000116f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011700: 2020 2020 7468 655f 6572 726f 7220 3d20      the_error = 
-00011710: 6622 4e6f 7420 556e 6963 6f64 653a 207b  f"Not Unicode: {
-00011720: 6572 727d 5c6e 7b64 6174 6167 7261 6d7d  err}\n{datagram}
-00011730: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00011740: 2020 2020 2020 6c6f 6767 6572 2e77 6172        logger.war
-00011750: 6e69 6e67 2874 6865 5f65 7272 6f72 290a  ning(the_error).
-00011760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011770: 2020 2020 636f 6e74 696e 7565 0a20 2020      continue.   
-00011780: 2020 2020 2020 2020 2020 2020 2065 7863               exc
-00011790: 6570 7420 4a53 4f4e 4465 636f 6465 4572  ept JSONDecodeEr
-000117a0: 726f 7220 6173 2065 7272 3a0a 2020 2020  ror as err:.    
-000117b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000117c0: 7468 655f 6572 726f 7220 3d20 6622 4e6f  the_error = f"No
-000117d0: 7420 4a53 4f4e 3a20 7b65 7272 7d5c 6e7b  t JSON: {err}\n{
-000117e0: 6461 7461 6772 616d 7d22 0a20 2020 2020  datagram}".     
-000117f0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-00011800: 6f67 6765 722e 7761 726e 696e 6728 7468  ogger.warning(th
-00011810: 655f 6572 726f 7229 0a20 2020 2020 2020  e_error).       
-00011820: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
-00011830: 7469 6e75 650a 2020 2020 2020 2020 2020  tinue.          
-00011840: 2020 2020 2020 6966 2028 0a20 2020 2020        if (.     
-00011850: 2020 2020 2020 2020 2020 2020 2020 206a                 j
-00011860: 736f 6e5f 6461 7461 2e67 6574 2822 636d  son_data.get("cm
-00011870: 6422 2c20 2222 2920 3d3d 2022 4745 5443  d", "") == "GETC
-00011880: 4f4c 554d 4e53 220a 2020 2020 2020 2020  OLUMNS".        
-00011890: 2020 2020 2020 2020 2020 2020 616e 6420              and 
-000118a0: 6a73 6f6e 5f64 6174 612e 6765 7428 2273  json_data.get("s
-000118b0: 7461 7469 6f6e 222c 2022 2229 203d 3d20  tation", "") == 
-000118c0: 706c 6174 666f 726d 2e6e 6f64 6528 290a  platform.node().
-000118d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000118e0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-000118f0: 2020 2020 2020 2069 6620 6861 7361 7474         if hasatt
-00011900: 7228 7365 6c66 2e63 6f6e 7465 7374 2c20  r(self.contest, 
-00011910: 2263 6f6c 756d 6e73 2229 3a0a 2020 2020  "columns"):.    
-00011920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011930: 2020 2020 636d 6420 3d20 7b7d 0a20 2020      cmd = {}.   
-00011940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011950: 2020 2020 2063 6d64 5b22 636d 6422 5d20       cmd["cmd"] 
-00011960: 3d20 2253 484f 5743 4f4c 554d 4e53 220a  = "SHOWCOLUMNS".
-00011970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011980: 2020 2020 2020 2020 636d 645b 2273 7461          cmd["sta
-00011990: 7469 6f6e 225d 203d 2070 6c61 7466 6f72  tion"] = platfor
-000119a0: 6d2e 6e6f 6465 2829 0a20 2020 2020 2020  m.node().       
-000119b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000119c0: 2063 6d64 5b22 434f 4c55 4d4e 5322 5d20   cmd["COLUMNS"] 
-000119d0: 3d20 7365 6c66 2e63 6f6e 7465 7374 2e63  = self.contest.c
-000119e0: 6f6c 756d 6e73 0a20 2020 2020 2020 2020  olumns.         
-000119f0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00011a00: 656c 662e 6d75 6c74 6963 6173 745f 696e  elf.multicast_in
-00011a10: 7465 7266 6163 652e 7365 6e64 5f61 735f  terface.send_as_
-00011a20: 6a73 6f6e 2863 6d64 290a 2020 2020 2020  json(cmd).      
-00011a30: 2020 2020 2020 2020 2020 6966 2028 0a20            if (. 
-00011a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011a50: 2020 206a 736f 6e5f 6461 7461 2e67 6574     json_data.get
-00011a60: 2822 636d 6422 2c20 2222 2920 3d3d 2022  ("cmd", "") == "
-00011a70: 5455 4e45 220a 2020 2020 2020 2020 2020  TUNE".          
-00011a80: 2020 2020 2020 2020 2020 616e 6420 6a73            and js
-00011a90: 6f6e 5f64 6174 612e 6765 7428 2273 7461  on_data.get("sta
-00011aa0: 7469 6f6e 222c 2022 2229 203d 3d20 706c  tion", "") == pl
-00011ab0: 6174 666f 726d 2e6e 6f64 6528 290a 2020  atform.node().  
-00011ac0: 2020 2020 2020 2020 2020 2020 2020 293a                ):
-00011ad0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011ae0: 2020 2020 2023 2062 277b 2263 6d64 223a       # b'{"cmd":
-00011af0: 2022 5455 4e45 222c 2022 6672 6571 223a   "TUNE", "freq":
-00011b00: 2037 2e30 3233 352c 2022 7370 6f74 223a   7.0235, "spot":
-00011b10: 2022 4d4d 3044 4749 227d 270a 2020 2020   "MM0DGI"}'.    
-00011b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011b30: 7666 6f20 3d20 6a73 6f6e 5f64 6174 612e  vfo = json_data.
-00011b40: 6765 7428 2266 7265 7122 290a 2020 2020  get("freq").    
-00011b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011b60: 7666 6f20 3d20 666c 6f61 7428 7666 6f29  vfo = float(vfo)
-00011b70: 202a 2031 3030 3030 3030 0a20 2020 2020   * 1000000.     
-00011b80: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00011b90: 656c 662e 7261 6469 6f5f 7374 6174 655b  elf.radio_state[
-00011ba0: 2276 666f 6122 5d20 3d20 696e 7428 7666  "vfoa"] = int(vf
-00011bb0: 6f29 0a20 2020 2020 2020 2020 2020 2020  o).             
-00011bc0: 2020 2020 2020 2069 6620 7365 6c66 2e72         if self.r
-00011bd0: 6967 5f63 6f6e 7472 6f6c 3a0a 2020 2020  ig_control:.    
-00011be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011bf0: 2020 2020 7365 6c66 2e72 6967 5f63 6f6e      self.rig_con
-00011c00: 7472 6f6c 2e73 6574 5f76 666f 2869 6e74  trol.set_vfo(int
-00011c10: 2876 666f 2929 0a20 2020 2020 2020 2020  (vfo)).         
-00011c20: 2020 2020 2020 2020 2020 2073 706f 7420             spot 
-00011c30: 3d20 6a73 6f6e 5f64 6174 612e 6765 7428  = json_data.get(
-00011c40: 2273 706f 7422 2c20 2222 290a 2020 2020  "spot", "").    
-00011c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011c60: 7365 6c66 2e63 616c 6c73 6967 6e2e 7365  self.callsign.se
-00011c70: 7454 6578 7428 7370 6f74 290a 2020 2020  tText(spot).    
-00011c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011c90: 7365 6c66 2e63 616c 6c73 6967 6e5f 6368  self.callsign_ch
-00011ca0: 616e 6765 6428 290a 2020 2020 2020 2020  anged().        
-00011cb0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00011cc0: 2e63 616c 6c73 6967 6e2e 7365 7446 6f63  .callsign.setFoc
-00011cd0: 7573 2829 0a20 2020 2020 2020 2020 2020  us().           
-00011ce0: 2020 2020 2020 2020 2073 656c 662e 6361           self.ca
-00011cf0: 6c6c 7369 676e 2e61 6374 6976 6174 6557  llsign.activateW
-00011d00: 696e 646f 7728 290a 2020 2020 2020 2020  indow().        
-00011d10: 2020 2020 2020 2020 2020 2020 7769 6e64              wind
-00011d20: 6f77 2e72 6169 7365 5f28 290a 2020 2020  ow.raise_().    
-00011d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011d40: 2320 6667 203d 2077 696e 646f 772e 6672  # fg = window.fr
-00011d50: 616d 6547 656f 6d65 7472 7928 292e 746f  ameGeometry().to
-00011d60: 704c 6566 740a 2020 2020 2020 2020 2020  pLeft.          
-00011d70: 2020 2020 2020 2020 2020 2320 2320 5f77            # # _w
-00011d80: 6964 7468 203d 2073 656c 662e 7369 7a65  idth = self.size
-00011d90: 2829 2e77 6964 7468 2829 0a20 2020 2020  ().width().     
-00011da0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00011db0: 2023 205f 6865 6967 6874 203d 2073 656c   # _height = sel
-00011dc0: 662e 7369 7a65 2829 2e68 6569 6768 7428  f.size().height(
-00011dd0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00011de0: 2020 2020 2020 2320 2320 5f78 203d 2073        # # _x = s
-00011df0: 656c 662e 706f 7328 292e 7828 290a 2020  elf.pos().x().  
-00011e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011e10: 2020 2320 2320 5f79 203d 2073 656c 662e    # # _y = self.
-00011e20: 706f 7328 292e 7928 290a 2020 2020 2020  pos().y().      
-00011e30: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00011e40: 2320 7072 696e 7428 6622 2a2a 2a2a 2a2a  # print(f"******
-00011e50: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
-00011e60: 2a2a 2a2a 2a2a 2078 207b 5f78 7d20 7920  ****** x {_x} y 
-00011e70: 7b5f 797d 2229 0a20 2020 2020 2020 2020  {_y}").         
-00011e80: 2020 2020 2020 2020 2020 2023 2023 2077             # # w
-00011e90: 696e 646f 772e 6869 6465 2829 0a20 2020  indow.hide().   
-00011ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011eb0: 2023 2023 2077 696e 646f 772e 7368 6f77   # # window.show
-00011ec0: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
-00011ed0: 2020 2020 2020 2023 2023 2077 696e 646f         # # windo
-00011ee0: 772e 7365 7447 656f 6d65 7472 7928 302c  w.setGeometry(0,
-00011ef0: 2030 2c20 5f77 6964 7468 2c20 5f68 6569   0, _width, _hei
-00011f00: 6768 7429 0a20 2020 2020 2020 2020 2020  ght).           
-00011f10: 2020 2020 2020 2020 2023 2077 696e 646f           # windo
-00011f20: 772e 7368 6f77 2829 0a20 2020 2020 2020  w.show().       
-00011f30: 2020 2020 2020 2020 2020 2020 2023 2077               # w
-00011f40: 696e 646f 772e 6765 6f6d 6574 7279 2829  indow.geometry()
-00011f50: 2e73 6574 5828 3130 3029 0a20 2020 2020  .setX(100).     
-00011f60: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00011f70: 2077 696e 646f 772e 6765 6f6d 6574 7279   window.geometry
-00011f80: 2829 2e73 6574 5928 3130 3029 0a0a 2020  ().setY(100)..  
-00011f90: 2020 6465 6620 6377 5f6d 6163 726f 735f    def cw_macros_
-00011fa0: 7374 6174 655f 6368 616e 6765 6428 7365  state_changed(se
-00011fb0: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
-00011fc0: 4d65 6e75 2069 7465 6d20 746f 2073 686f  Menu item to sho
-00011fd0: 772f 6869 6465 206d 6163 726f 2062 7574  w/hide macro but
-00011fe0: 746f 6e73 2222 220a 2020 2020 2020 2020  tons""".        
-00011ff0: 7365 6c66 2e70 7265 665b 2263 775f 6d61  self.pref["cw_ma
-00012000: 6372 6f73 225d 203d 2073 656c 662e 6163  cros"] = self.ac
-00012010: 7469 6f6e 4357 5f4d 6163 726f 732e 6973  tionCW_Macros.is
-00012020: 4368 6563 6b65 6428 290a 2020 2020 2020  Checked().      
-00012030: 2020 7365 6c66 2e77 7269 7465 5f70 7265    self.write_pre
-00012040: 6665 7265 6e63 6528 290a 2020 2020 2020  ference().      
-00012050: 2020 7365 6c66 2e73 686f 775f 4357 5f6d    self.show_CW_m
-00012060: 6163 726f 7328 290a 0a20 2020 2064 6566  acros()..    def
-00012070: 2073 686f 775f 4357 5f6d 6163 726f 7328   show_CW_macros(
-00012080: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
-00012090: 2222 6d61 6372 6f20 6275 7474 6f6e 2073  ""macro button s
-000120a0: 7461 7465 2063 6861 6e67 6522 2222 0a20  tate change""". 
-000120b0: 2020 2020 2020 2069 6620 7365 6c66 2e70         if self.p
-000120c0: 7265 662e 6765 7428 2263 775f 6d61 6372  ref.get("cw_macr
-000120d0: 6f73 2229 3a0a 2020 2020 2020 2020 2020  os"):.          
-000120e0: 2020 7365 6c66 2e42 7574 746f 6e5f 526f    self.Button_Ro
-000120f0: 7731 2e73 686f 7728 290a 2020 2020 2020  w1.show().      
-00012100: 2020 2020 2020 7365 6c66 2e42 7574 746f        self.Butto
-00012110: 6e5f 526f 7732 2e73 686f 7728 290a 2020  n_Row2.show().  
-00012120: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00012130: 2020 2020 2020 2020 7365 6c66 2e42 7574          self.But
-00012140: 746f 6e5f 526f 7731 2e68 6964 6528 290a  ton_Row1.hide().
-00012150: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00012160: 2e42 7574 746f 6e5f 526f 7732 2e68 6964  .Button_Row2.hid
-00012170: 6528 290a 0a20 2020 2064 6566 2063 6f6d  e()..    def com
-00012180: 6d61 6e64 5f62 7574 746f 6e73 5f73 7461  mand_buttons_sta
-00012190: 7465 5f63 6861 6e67 6528 7365 6c66 293a  te_change(self):
-000121a0: 0a20 2020 2020 2020 2022 2222 4d65 6e75  .        """Menu
-000121b0: 2069 7465 6d20 746f 2073 686f 772f 6869   item to show/hi
-000121c0: 6465 2063 6f6d 6d61 6e64 2062 7574 746f  de command butto
-000121d0: 6e73 2222 220a 2020 2020 2020 2020 7365  ns""".        se
-000121e0: 6c66 2e70 7265 665b 2263 6f6d 6d61 6e64  lf.pref["command
-000121f0: 5f62 7574 746f 6e73 225d 203d 2073 656c  _buttons"] = sel
-00012200: 662e 6163 7469 6f6e 436f 6d6d 616e 645f  f.actionCommand_
-00012210: 4275 7474 6f6e 732e 6973 4368 6563 6b65  Buttons.isChecke
-00012220: 6428 290a 2020 2020 2020 2020 7365 6c66  d().        self
-00012230: 2e77 7269 7465 5f70 7265 6665 7265 6e63  .write_preferenc
-00012240: 6528 290a 2020 2020 2020 2020 7365 6c66  e().        self
-00012250: 2e73 686f 775f 636f 6d6d 616e 645f 6275  .show_command_bu
-00012260: 7474 6f6e 7328 290a 0a20 2020 2064 6566  ttons()..    def
-00012270: 2073 686f 775f 636f 6d6d 616e 645f 6275   show_command_bu
-00012280: 7474 6f6e 7328 7365 6c66 293a 0a20 2020  ttons(self):.   
-00012290: 2020 2020 2022 2222 636f 6d6d 616e 6420       """command 
-000122a0: 6275 7474 6f6e 2073 7461 7465 2063 6861  button state cha
-000122b0: 6e67 6522 2222 0a20 2020 2020 2020 2069  nge""".        i
-000122c0: 6620 7365 6c66 2e70 7265 662e 6765 7428  f self.pref.get(
-000122d0: 2263 6f6d 6d61 6e64 5f62 7574 746f 6e73  "command_buttons
-000122e0: 2229 3a0a 2020 2020 2020 2020 2020 2020  "):.            
-000122f0: 7365 6c66 2e43 6f6d 6d61 6e64 5f42 7574  self.Command_But
-00012300: 746f 6e73 2e73 686f 7728 290a 2020 2020  tons.show().    
-00012310: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00012320: 2020 2020 2020 7365 6c66 2e43 6f6d 6d61        self.Comma
-00012330: 6e64 5f42 7574 746f 6e73 2e68 6964 6528  nd_Buttons.hide(
-00012340: 290a 0a20 2020 2064 6566 2069 735f 666c  )..    def is_fl
-00012350: 6f61 7461 626c 6528 7365 6c66 2c20 6974  oatable(self, it
-00012360: 656d 3a20 7374 7229 202d 3e20 626f 6f6c  em: str) -> bool
-00012370: 3a0a 2020 2020 2020 2020 2222 2263 6865  :.        """che
-00012380: 636b 2074 6f20 7365 6520 6966 2073 7472  ck to see if str
-00012390: 696e 6720 6361 6e20 6265 2061 2066 6c6f  ing can be a flo
-000123a0: 6174 2222 220a 2020 2020 2020 2020 6966  at""".        if
-000123b0: 2069 7465 6d2e 6973 6e75 6d65 7269 6328   item.isnumeric(
-000123c0: 293a 0a20 2020 2020 2020 2020 2020 2072  ):.            r
-000123d0: 6574 7572 6e20 5472 7565 0a20 2020 2020  eturn True.     
-000123e0: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
-000123f0: 2020 2020 5f74 6573 7420 3d20 666c 6f61      _test = floa
-00012400: 7428 6974 656d 290a 2020 2020 2020 2020  t(item).        
-00012410: 6578 6365 7074 2056 616c 7565 4572 726f  except ValueErro
-00012420: 723a 0a20 2020 2020 2020 2020 2020 2072  r:.            r
-00012430: 6574 7572 6e20 4661 6c73 650a 2020 2020  eturn False.    
-00012440: 2020 2020 7265 7475 726e 2054 7275 650a      return True.
-00012450: 0a20 2020 2064 6566 206f 7468 6572 5f32  .    def other_2
-00012460: 5f63 6861 6e67 6564 2873 656c 6629 3a0a  _changed(self):.
-00012470: 2020 2020 2020 2020 2222 2243 616c 6c65          """Calle
-00012480: 6420 7768 656e 2077 6520 6e65 6564 2074  d when we need t
-00012490: 6f20 7061 7273 6520 5353 2065 7863 6861  o parse SS excha
-000124a0: 6e67 652e 2222 220a 2020 2020 2020 2020  nge.""".        
-000124b0: 6966 2073 656c 662e 636f 6e74 6573 743a  if self.contest:
-000124c0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-000124d0: 2241 5252 4c20 5377 6565 7073 7461 6b65  "ARRL Sweepstake
-000124e0: 7322 2069 6e20 7365 6c66 2e63 6f6e 7465  s" in self.conte
-000124f0: 7374 2e6e 616d 653a 0a20 2020 2020 2020  st.name:.       
-00012500: 2020 2020 2020 2020 2073 656c 662e 636f           self.co
-00012510: 6e74 6573 742e 7061 7273 655f 6578 6368  ntest.parse_exch
-00012520: 616e 6765 2873 656c 6629 0a0a 2020 2020  ange(self)..    
-00012530: 6465 6620 6361 6c6c 7369 676e 5f63 6861  def callsign_cha
-00012540: 6e67 6564 2873 656c 6629 3a0a 2020 2020  nged(self):.    
-00012550: 2020 2020 2222 2243 616c 6c65 6420 7768      """Called wh
-00012560: 656e 2074 6578 7420 696e 2074 6865 2063  en text in the c
-00012570: 616c 6c73 6967 6e20 6669 656c 6420 6861  allsign field ha
-00012580: 7320 6368 616e 6765 6422 2222 0a20 2020  s changed""".   
-00012590: 2020 2020 2074 6578 7420 3d20 7365 6c66       text = self
-000125a0: 2e63 616c 6c73 6967 6e2e 7465 7874 2829  .callsign.text()
-000125b0: 0a20 2020 2020 2020 2074 6578 7420 3d20  .        text = 
-000125c0: 7465 7874 2e75 7070 6572 2829 0a20 2020  text.upper().   
-000125d0: 2020 2020 2070 6f73 6974 696f 6e20 3d20       position = 
-000125e0: 7365 6c66 2e63 616c 6c73 6967 6e2e 6375  self.callsign.cu
-000125f0: 7273 6f72 506f 7369 7469 6f6e 2829 0a20  rsorPosition(). 
-00012600: 2020 2020 2020 2073 7472 6970 7065 645f         stripped_
-00012610: 7465 7874 203d 2074 6578 742e 7374 7269  text = text.stri
-00012620: 7028 292e 7265 706c 6163 6528 2220 222c  p().replace(" ",
-00012630: 2022 2229 0a20 2020 2020 2020 2073 656c   "").        sel
-00012640: 662e 6361 6c6c 7369 676e 2e73 6574 5465  f.callsign.setTe
-00012650: 7874 2873 7472 6970 7065 645f 7465 7874  xt(stripped_text
-00012660: 290a 2020 2020 2020 2020 7365 6c66 2e63  ).        self.c
-00012670: 616c 6c73 6967 6e2e 7365 7443 7572 736f  allsign.setCurso
-00012680: 7250 6f73 6974 696f 6e28 706f 7369 7469  rPosition(positi
-00012690: 6f6e 290a 0a20 2020 2020 2020 2069 6620  on)..        if 
-000126a0: 2220 2220 696e 2074 6578 743a 0a20 2020  " " in text:.   
-000126b0: 2020 2020 2020 2020 2069 6620 7374 7269           if stri
-000126c0: 7070 6564 5f74 6578 7420 3d3d 2022 4357  pped_text == "CW
-000126d0: 223a 0a20 2020 2020 2020 2020 2020 2020  ":.             
-000126e0: 2020 2073 656c 662e 7365 746d 6f64 6528     self.setmode(
-000126f0: 2243 5722 290a 2020 2020 2020 2020 2020  "CW").          
-00012700: 2020 2020 2020 7365 6c66 2e72 6164 696f        self.radio
-00012710: 5f73 7461 7465 5b22 6d6f 6465 225d 203d  _state["mode"] =
-00012720: 2022 4357 220a 2020 2020 2020 2020 2020   "CW".          
-00012730: 2020 2020 2020 6966 2073 656c 662e 7269        if self.ri
-00012740: 675f 636f 6e74 726f 6c3a 0a20 2020 2020  g_control:.     
-00012750: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00012760: 6620 7365 6c66 2e72 6967 5f63 6f6e 7472  f self.rig_contr
-00012770: 6f6c 2e6f 6e6c 696e 653a 0a20 2020 2020  ol.online:.     
-00012780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012790: 2020 2073 656c 662e 7269 675f 636f 6e74     self.rig_cont
-000127a0: 726f 6c2e 7365 745f 6d6f 6465 2822 4357  rol.set_mode("CW
-000127b0: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
-000127c0: 2020 2062 616e 6420 3d20 6765 7462 616e     band = getban
-000127d0: 6428 7374 7228 7365 6c66 2e72 6164 696f  d(str(self.radio
-000127e0: 5f73 7461 7465 2e67 6574 2822 7666 6f61  _state.get("vfoa
-000127f0: 222c 2022 302e 3022 2929 290a 2020 2020  ", "0.0"))).    
-00012800: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00012810: 2e73 6574 5f62 616e 645f 696e 6469 6361  .set_band_indica
-00012820: 746f 7228 6261 6e64 290a 2020 2020 2020  tor(band).      
-00012830: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
-00012840: 6574 5f77 696e 646f 775f 7469 746c 6528  et_window_title(
-00012850: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00012860: 2020 7365 6c66 2e63 6c65 6172 696e 7075    self.clearinpu
-00012870: 7473 2829 0a20 2020 2020 2020 2020 2020  ts().           
-00012880: 2020 2020 2073 656c 662e 7265 6164 5f63       self.read_c
-00012890: 775f 6d61 6372 6f73 2829 0a20 2020 2020  w_macros().     
-000128a0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-000128b0: 6e0a 2020 2020 2020 2020 2020 2020 6966  n.            if
-000128c0: 2073 7472 6970 7065 645f 7465 7874 203d   stripped_text =
-000128d0: 3d20 2252 5454 5922 3a0a 2020 2020 2020  = "RTTY":.      
-000128e0: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
-000128f0: 6574 6d6f 6465 2822 5254 5459 2229 0a20  etmode("RTTY"). 
-00012900: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00012910: 6620 7365 6c66 2e72 6967 5f63 6f6e 7472  f self.rig_contr
-00012920: 6f6c 3a0a 2020 2020 2020 2020 2020 2020  ol:.            
-00012930: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00012940: 7269 675f 636f 6e74 726f 6c2e 6f6e 6c69  rig_control.onli
-00012950: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00012960: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00012970: 2e72 6967 5f63 6f6e 7472 6f6c 2e73 6574  .rig_control.set
-00012980: 5f6d 6f64 6528 2252 5454 5922 290a 2020  _mode("RTTY").  
-00012990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000129a0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-000129b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000129c0: 7365 6c66 2e72 6164 696f 5f73 7461 7465  self.radio_state
-000129d0: 5b22 6d6f 6465 225d 203d 2022 5254 5459  ["mode"] = "RTTY
-000129e0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-000129f0: 2020 6261 6e64 203d 2067 6574 6261 6e64    band = getband
-00012a00: 2873 7472 2873 656c 662e 7261 6469 6f5f  (str(self.radio_
-00012a10: 7374 6174 652e 6765 7428 2276 666f 6122  state.get("vfoa"
-00012a20: 2c20 2230 2e30 2229 2929 0a20 2020 2020  , "0.0"))).     
-00012a30: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00012a40: 7365 745f 6261 6e64 5f69 6e64 6963 6174  set_band_indicat
-00012a50: 6f72 2862 616e 6429 0a20 2020 2020 2020  or(band).       
-00012a60: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
-00012a70: 745f 7769 6e64 6f77 5f74 6974 6c65 2829  t_window_title()
-00012a80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012a90: 2073 656c 662e 636c 6561 7269 6e70 7574   self.clearinput
-00012aa0: 7328 290a 2020 2020 2020 2020 2020 2020  s().            
-00012ab0: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
-00012ac0: 2020 2020 2020 2069 6620 7374 7269 7070         if stripp
-00012ad0: 6564 5f74 6578 7420 3d3d 2022 5353 4222  ed_text == "SSB"
-00012ae0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00012af0: 2020 7365 6c66 2e73 6574 6d6f 6465 2822    self.setmode("
-00012b00: 5353 4222 290a 2020 2020 2020 2020 2020  SSB").          
-00012b10: 2020 2020 2020 6966 2069 6e74 2873 656c        if int(sel
-00012b20: 662e 7261 6469 6f5f 7374 6174 652e 6765  f.radio_state.ge
-00012b30: 7428 2276 666f 6122 2c20 3029 2920 3e20  t("vfoa", 0)) > 
-00012b40: 3130 3030 3030 3030 3a0a 2020 2020 2020  10000000:.      
-00012b50: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00012b60: 6c66 2e72 6164 696f 5f73 7461 7465 5b22  lf.radio_state["
-00012b70: 6d6f 6465 225d 203d 2022 5553 4222 0a20  mode"] = "USB". 
-00012b80: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00012b90: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00012ba0: 2020 2020 2020 2020 2073 656c 662e 7261           self.ra
-00012bb0: 6469 6f5f 7374 6174 655b 226d 6f64 6522  dio_state["mode"
-00012bc0: 5d20 3d20 224c 5342 220a 2020 2020 2020  ] = "LSB".      
-00012bd0: 2020 2020 2020 2020 2020 6261 6e64 203d            band =
-00012be0: 2067 6574 6261 6e64 2873 7472 2873 656c   getband(str(sel
-00012bf0: 662e 7261 6469 6f5f 7374 6174 652e 6765  f.radio_state.ge
-00012c00: 7428 2276 666f 6122 2c20 2230 2e30 2229  t("vfoa", "0.0")
-00012c10: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
-00012c20: 2020 2073 656c 662e 7365 745f 6261 6e64     self.set_band
-00012c30: 5f69 6e64 6963 6174 6f72 2862 616e 6429  _indicator(band)
-00012c40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012c50: 2073 656c 662e 7365 745f 7769 6e64 6f77   self.set_window
-00012c60: 5f74 6974 6c65 2829 0a20 2020 2020 2020  _title().       
-00012c70: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
-00012c80: 2e72 6967 5f63 6f6e 7472 6f6c 3a0a 2020  .rig_control:.  
-00012c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012ca0: 2020 7365 6c66 2e72 6967 5f63 6f6e 7472    self.rig_contr
-00012cb0: 6f6c 2e73 6574 5f6d 6f64 6528 7365 6c66  ol.set_mode(self
-00012cc0: 2e72 6164 696f 5f73 7461 7465 2e67 6574  .radio_state.get
-00012cd0: 2822 6d6f 6465 2229 290a 2020 2020 2020  ("mode")).      
-00012ce0: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-00012cf0: 6c65 6172 696e 7075 7473 2829 0a20 2020  learinputs().   
-00012d00: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00012d10: 662e 7265 6164 5f63 775f 6d61 6372 6f73  f.read_cw_macros
-00012d20: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
-00012d30: 2020 2072 6574 7572 6e0a 2020 2020 2020     return.      
-00012d40: 2020 2020 2020 6966 2073 7472 6970 7065        if strippe
-00012d50: 645f 7465 7874 203d 3d20 224f 504f 4e22  d_text == "OPON"
-00012d60: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00012d70: 2020 7365 6c66 2e67 6574 5f6f 706f 6e28    self.get_opon(
-00012d80: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00012d90: 2020 7365 6c66 2e63 6c65 6172 696e 7075    self.clearinpu
-00012da0: 7473 2829 0a20 2020 2020 2020 2020 2020  ts().           
-00012db0: 2020 2020 2072 6574 7572 6e0a 2020 2020       return.    
-00012dc0: 2020 2020 2020 2020 6966 2073 7472 6970          if strip
-00012dd0: 7065 645f 7465 7874 203d 3d20 2248 454c  ped_text == "HEL
-00012de0: 5022 3a0a 2020 2020 2020 2020 2020 2020  P":.            
-00012df0: 2020 2020 7365 6c66 2e73 686f 775f 6865      self.show_he
-00012e00: 6c70 5f64 6961 6c6f 6728 290a 2020 2020  lp_dialog().    
-00012e10: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00012e20: 2e63 6c65 6172 696e 7075 7473 2829 0a20  .clearinputs(). 
-00012e30: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00012e40: 6574 7572 6e0a 2020 2020 2020 2020 2020  eturn.          
-00012e50: 2020 6966 2073 7472 6970 7065 645f 7465    if stripped_te
-00012e60: 7874 203d 3d20 2254 4553 5422 3a0a 2020  xt == "TEST":.  
-00012e70: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00012e80: 6c66 2e73 686f 775f 6d65 7373 6167 655f  lf.show_message_
-00012e90: 626f 7828 0a20 2020 2020 2020 2020 2020  box(.           
-00012ea0: 2020 2020 2020 2020 2022 5b45 7363 5d5c           "[Esc]\
-00012eb0: 7443 6c65 6172 7320 7468 6520 696e 7075  tClears the inpu
-00012ec0: 7420 6669 656c 6473 206f 6620 616e 7920  t fields of any 
-00012ed0: 7465 7874 2e5c 6e22 0a20 2020 2020 2020  text.\n".       
-00012ee0: 2020 2020 2020 2020 2020 2020 2022 5b43               "[C
-00012ef0: 5452 4c2d 4573 635d 5c74 5374 6f70 7320  TRL-Esc]\tStops 
-00012f00: 6377 6461 656d 6f6e 2066 726f 6d20 7365  cwdaemon from se
-00012f10: 6e64 696e 6720 4d6f 7273 652e 5c6e 220a  nding Morse.\n".
-00012f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012f30: 2020 2020 225b 5067 5570 5d5c 7449 6e63      "[PgUp]\tInc
-00012f40: 7265 6173 6573 2074 6865 2063 7720 7365  reases the cw se
-00012f50: 6e64 696e 6720 7370 6565 642e 5c6e 220a  nding speed.\n".
-00012f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012f70: 2020 2020 225b 5067 446f 776e 5d5c 7444      "[PgDown]\tD
-00012f80: 6563 7265 6173 6573 2074 6865 2063 7720  ecreases the cw 
-00012f90: 7365 6e64 696e 6720 7370 6565 642e 5c6e  sending speed.\n
-00012fa0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00012fb0: 2020 2020 2020 225b 4172 726f 772d 5570        "[Arrow-Up
-00012fc0: 5d20 4a75 6d70 2074 6f20 7468 6520 6e65  ] Jump to the ne
-00012fd0: 7874 2073 706f 7420 6162 6f76 6520 7468  xt spot above th
-00012fe0: 6520 6375 7272 656e 7420 5646 4f20 6375  e current VFO cu
-00012ff0: 7273 6f72 5c6e 220a 2020 2020 2020 2020  rsor\n".        
-00013000: 2020 2020 2020 2020 2020 2020 225c 7469              "\ti
-00013010: 6e20 7468 6520 6261 6e64 6d61 7020 7769  n the bandmap wi
-00013020: 6e64 6f77 2028 4341 5420 5265 7175 6972  ndow (CAT Requir
-00013030: 6564 292e 5c6e 220a 2020 2020 2020 2020  ed).\n".        
-00013040: 2020 2020 2020 2020 2020 2020 225b 4172              "[Ar
-00013050: 726f 772d 446f 776e 5d20 4a75 6d70 2074  row-Down] Jump t
-00013060: 6f20 7468 6520 6e65 7874 2073 706f 7420  o the next spot 
-00013070: 6265 6c6f 7720 7468 6520 6375 7272 656e  below the curren
-00013080: 745c 6e22 0a20 2020 2020 2020 2020 2020  t\n".           
-00013090: 2020 2020 2020 2020 2022 5c74 5646 4f20           "\tVFO 
-000130a0: 6375 7273 6f72 2069 6e20 7468 6520 6261  cursor in the ba
-000130b0: 6e64 6d61 7020 7769 6e64 6f77 2028 4341  ndmap window (CA
-000130c0: 5420 5265 7175 6972 6564 292e 5c6e 220a  T Required).\n".
+000111e0: 6c6f 6f6b 7570 706f 7274 222c 2022 3132  lookupport", "12
+000111f0: 372e 302e 302e 313a 3132 3036 3022 292c  7.0.0.1:12060"),
+00011200: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011210: 2020 2020 2073 656c 662e 7072 6566 2e67       self.pref.g
+00011220: 6574 2822 6e31 6d6d 5f73 636f 7265 706f  et("n1mm_scorepo
+00011230: 7274 222c 2022 3132 372e 302e 302e 313a  rt", "127.0.0.1:
+00011240: 3132 3036 3022 292c 0a20 2020 2020 2020  12060"),.       
+00011250: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+00011260: 2020 2020 2020 2065 7863 6570 7420 5661         except Va
+00011270: 6c75 6545 7272 6f72 3a0a 2020 2020 2020  lueError:.      
+00011280: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
+00011290: 2e77 6172 6e69 6e67 2822 2573 222c 2066  .warning("%s", f
+000112a0: 227b 5661 6c75 6545 7272 6f72 7d22 290a  "{ValueError}").
+000112b0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000112c0: 2e6e 316d 6d2e 7365 6e64 5f72 6164 696f  .n1mm.send_radio
+000112d0: 5f70 6163 6b65 7473 203d 2073 656c 662e  _packets = self.
+000112e0: 7072 6566 2e67 6574 2822 7365 6e64 5f6e  pref.get("send_n
+000112f0: 316d 6d5f 7261 6469 6f22 2c20 4661 6c73  1mm_radio", Fals
+00011300: 6529 0a20 2020 2020 2020 2020 2020 2073  e).            s
+00011310: 656c 662e 6e31 6d6d 2e73 656e 645f 636f  elf.n1mm.send_co
+00011320: 6e74 6163 745f 7061 636b 6574 7320 3d20  ntact_packets = 
+00011330: 7365 6c66 2e70 7265 662e 6765 7428 2273  self.pref.get("s
+00011340: 656e 645f 6e31 6d6d 5f63 6f6e 7461 6374  end_n1mm_contact
+00011350: 222c 2046 616c 7365 290a 2020 2020 2020  ", False).      
+00011360: 2020 2020 2020 7365 6c66 2e6e 316d 6d2e        self.n1mm.
+00011370: 7365 6e64 5f6c 6f6f 6b75 705f 7061 636b  send_lookup_pack
+00011380: 6574 7320 3d20 7365 6c66 2e70 7265 662e  ets = self.pref.
+00011390: 6765 7428 2273 656e 645f 6e31 6d6d 5f6c  get("send_n1mm_l
+000113a0: 6f6f 6b75 7022 2c20 4661 6c73 6529 0a20  ookup", False). 
+000113b0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000113c0: 6e31 6d6d 2e73 656e 645f 7363 6f72 655f  n1mm.send_score_
+000113d0: 7061 636b 6574 7320 3d20 7365 6c66 2e70  packets = self.p
+000113e0: 7265 662e 6765 7428 2273 656e 645f 6e31  ref.get("send_n1
+000113f0: 6d6d 5f73 636f 7265 222c 2046 616c 7365  mm_score", False
+00011400: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
+00011410: 6c66 2e6e 316d 6d2e 7261 6469 6f5f 696e  lf.n1mm.radio_in
+00011420: 666f 5b22 5374 6174 696f 6e4e 616d 6522  fo["StationName"
+00011430: 5d20 3d20 7365 6c66 2e70 7265 662e 6765  ] = self.pref.ge
+00011440: 7428 226e 316d 6d5f 7374 6174 696f 6e5f  t("n1mm_station_
+00011450: 6e61 6d65 222c 2022 2229 0a0a 2020 2020  name", "")..    
+00011460: 2020 2020 7365 6c66 2e73 686f 775f 636f      self.show_co
+00011470: 6d6d 616e 645f 6275 7474 6f6e 7328 290a  mmand_buttons().
+00011480: 2020 2020 2020 2020 7365 6c66 2e73 686f          self.sho
+00011490: 775f 4357 5f6d 6163 726f 7328 290a 2020  w_CW_macros().  
+000114a0: 2020 2020 2020 2320 7365 6c66 2e73 686f        # self.sho
+000114b0: 775f 6261 6e64 5f6d 6f64 6528 290a 0a20  w_band_mode().. 
+000114c0: 2020 2064 6566 2077 6174 6368 5f75 6470     def watch_udp
+000114d0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+000114e0: 2222 2250 726f 6365 7373 2055 4450 2064  """Process UDP d
+000114f0: 6174 6167 7261 6d73 2e22 2222 0a20 2020  atagrams.""".   
+00011500: 2020 2020 2077 6869 6c65 2073 656c 662e       while self.
+00011510: 6d75 6c74 6963 6173 745f 696e 7465 7266  multicast_interf
+00011520: 6163 652e 7365 7276 6572 5f75 6470 2e68  ace.server_udp.h
+00011530: 6173 5065 6e64 696e 6744 6174 6167 7261  asPendingDatagra
+00011540: 6d73 2829 3a0a 2020 2020 2020 2020 2020  ms():.          
+00011550: 2020 6275 6e64 6c65 203d 2073 656c 662e    bundle = self.
+00011560: 6d75 6c74 6963 6173 745f 696e 7465 7266  multicast_interf
+00011570: 6163 652e 7365 7276 6572 5f75 6470 2e72  ace.server_udp.r
+00011580: 6561 6444 6174 6167 7261 6d28 0a20 2020  eadDatagram(.   
+00011590: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+000115a0: 662e 6d75 6c74 6963 6173 745f 696e 7465  f.multicast_inte
+000115b0: 7266 6163 652e 7365 7276 6572 5f75 6470  rface.server_udp
+000115c0: 2e70 656e 6469 6e67 4461 7461 6772 616d  .pendingDatagram
+000115d0: 5369 7a65 2829 0a20 2020 2020 2020 2020  Size().         
+000115e0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+000115f0: 2064 6174 6167 7261 6d2c 205f 2c20 5f20   datagram, _, _ 
+00011600: 3d20 6275 6e64 6c65 0a20 2020 2020 2020  = bundle.       
+00011610: 2020 2020 2023 206c 6f67 6765 722e 6465       # logger.de
+00011620: 6275 6728 6461 7461 6772 616d 2e64 6563  bug(datagram.dec
+00011630: 6f64 6528 2929 0a20 2020 2020 2020 2020  ode()).         
+00011640: 2020 2069 6620 6461 7461 6772 616d 3a0a     if datagram:.
+00011650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011660: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
+00011670: 2020 2020 2020 2020 2023 2064 6562 7567           # debug
+00011680: 5f69 6e66 6f20 3d20 6622 7b64 6174 6167  _info = f"{datag
+00011690: 7261 6d2e 6465 636f 6465 2829 7d22 0a20  ram.decode()}". 
+000116a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000116b0: 2020 2023 206c 6f67 6765 722e 6465 6275     # logger.debu
+000116c0: 6728 6465 6275 675f 696e 666f 290a 2020  g(debug_info).  
+000116d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000116e0: 2020 6a73 6f6e 5f64 6174 6120 3d20 6c6f    json_data = lo
+000116f0: 6164 7328 6461 7461 6772 616d 2e64 6563  ads(datagram.dec
+00011700: 6f64 6528 2929 0a20 2020 2020 2020 2020  ode()).         
+00011710: 2020 2020 2020 2065 7863 6570 7420 556e         except Un
+00011720: 6963 6f64 6544 6563 6f64 6545 7272 6f72  icodeDecodeError
+00011730: 2061 7320 6572 723a 0a20 2020 2020 2020   as err:.       
+00011740: 2020 2020 2020 2020 2020 2020 2074 6865               the
+00011750: 5f65 7272 6f72 203d 2066 224e 6f74 2055  _error = f"Not U
+00011760: 6e69 636f 6465 3a20 7b65 7272 7d5c 6e7b  nicode: {err}\n{
+00011770: 6461 7461 6772 616d 7d22 0a20 2020 2020  datagram}".     
+00011780: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+00011790: 6f67 6765 722e 7761 726e 696e 6728 7468  ogger.warning(th
+000117a0: 655f 6572 726f 7229 0a20 2020 2020 2020  e_error).       
+000117b0: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
+000117c0: 7469 6e75 650a 2020 2020 2020 2020 2020  tinue.          
+000117d0: 2020 2020 2020 6578 6365 7074 204a 534f        except JSO
+000117e0: 4e44 6563 6f64 6545 7272 6f72 2061 7320  NDecodeError as 
+000117f0: 6572 723a 0a20 2020 2020 2020 2020 2020  err:.           
+00011800: 2020 2020 2020 2020 2074 6865 5f65 7272           the_err
+00011810: 6f72 203d 2066 224e 6f74 204a 534f 4e3a  or = f"Not JSON:
+00011820: 207b 6572 727d 5c6e 7b64 6174 6167 7261   {err}\n{datagra
+00011830: 6d7d 220a 2020 2020 2020 2020 2020 2020  m}".            
+00011840: 2020 2020 2020 2020 6c6f 6767 6572 2e77          logger.w
+00011850: 6172 6e69 6e67 2874 6865 5f65 7272 6f72  arning(the_error
+00011860: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00011870: 2020 2020 2020 636f 6e74 696e 7565 0a20        continue. 
+00011880: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00011890: 6620 280a 2020 2020 2020 2020 2020 2020  f (.            
+000118a0: 2020 2020 2020 2020 6a73 6f6e 5f64 6174          json_dat
+000118b0: 612e 6765 7428 2263 6d64 222c 2022 2229  a.get("cmd", "")
+000118c0: 203d 3d20 2247 4554 434f 4c55 4d4e 5322   == "GETCOLUMNS"
+000118d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000118e0: 2020 2020 2061 6e64 206a 736f 6e5f 6461       and json_da
+000118f0: 7461 2e67 6574 2822 7374 6174 696f 6e22  ta.get("station"
+00011900: 2c20 2222 2920 3d3d 2070 6c61 7466 6f72  , "") == platfor
+00011910: 6d2e 6e6f 6465 2829 0a20 2020 2020 2020  m.node().       
+00011920: 2020 2020 2020 2020 2029 3a0a 2020 2020           ):.    
+00011930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011940: 6966 2068 6173 6174 7472 2873 656c 662e  if hasattr(self.
+00011950: 636f 6e74 6573 742c 2022 636f 6c75 6d6e  contest, "column
+00011960: 7322 293a 0a20 2020 2020 2020 2020 2020  s"):.           
+00011970: 2020 2020 2020 2020 2020 2020 2063 6d64               cmd
+00011980: 203d 207b 7d0a 2020 2020 2020 2020 2020   = {}.          
+00011990: 2020 2020 2020 2020 2020 2020 2020 636d                cm
+000119a0: 645b 2263 6d64 225d 203d 2022 5348 4f57  d["cmd"] = "SHOW
+000119b0: 434f 4c55 4d4e 5322 0a20 2020 2020 2020  COLUMNS".       
+000119c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000119d0: 2063 6d64 5b22 7374 6174 696f 6e22 5d20   cmd["station"] 
+000119e0: 3d20 706c 6174 666f 726d 2e6e 6f64 6528  = platform.node(
+000119f0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00011a00: 2020 2020 2020 2020 2020 636d 645b 2243            cmd["C
+00011a10: 4f4c 554d 4e53 225d 203d 2073 656c 662e  OLUMNS"] = self.
+00011a20: 636f 6e74 6573 742e 636f 6c75 6d6e 730a  contest.columns.
+00011a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011a40: 2020 2020 2020 2020 7365 6c66 2e6d 756c          self.mul
+00011a50: 7469 6361 7374 5f69 6e74 6572 6661 6365  ticast_interface
+00011a60: 2e73 656e 645f 6173 5f6a 736f 6e28 636d  .send_as_json(cm
+00011a70: 6429 0a20 2020 2020 2020 2020 2020 2020  d).             
+00011a80: 2020 2069 6620 280a 2020 2020 2020 2020     if (.        
+00011a90: 2020 2020 2020 2020 2020 2020 6a73 6f6e              json
+00011aa0: 5f64 6174 612e 6765 7428 2263 6d64 222c  _data.get("cmd",
+00011ab0: 2022 2229 203d 3d20 2254 554e 4522 0a20   "") == "TUNE". 
+00011ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011ad0: 2020 2061 6e64 206a 736f 6e5f 6461 7461     and json_data
+00011ae0: 2e67 6574 2822 7374 6174 696f 6e22 2c20  .get("station", 
+00011af0: 2222 2920 3d3d 2070 6c61 7466 6f72 6d2e  "") == platform.
+00011b00: 6e6f 6465 2829 0a20 2020 2020 2020 2020  node().         
+00011b10: 2020 2020 2020 2029 3a0a 2020 2020 2020         ):.      
+00011b20: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+00011b30: 6227 7b22 636d 6422 3a20 2254 554e 4522  b'{"cmd": "TUNE"
+00011b40: 2c20 2266 7265 7122 3a20 372e 3032 3335  , "freq": 7.0235
+00011b50: 2c20 2273 706f 7422 3a20 224d 4d30 4447  , "spot": "MM0DG
+00011b60: 4922 7d27 0a20 2020 2020 2020 2020 2020  I"}'.           
+00011b70: 2020 2020 2020 2020 2076 666f 203d 206a           vfo = j
+00011b80: 736f 6e5f 6461 7461 2e67 6574 2822 6672  son_data.get("fr
+00011b90: 6571 2229 0a20 2020 2020 2020 2020 2020  eq").           
+00011ba0: 2020 2020 2020 2020 2076 666f 203d 2066           vfo = f
+00011bb0: 6c6f 6174 2876 666f 2920 2a20 3130 3030  loat(vfo) * 1000
+00011bc0: 3030 300a 2020 2020 2020 2020 2020 2020  000.            
+00011bd0: 2020 2020 2020 2020 7365 6c66 2e72 6164          self.rad
+00011be0: 696f 5f73 7461 7465 5b22 7666 6f61 225d  io_state["vfoa"]
+00011bf0: 203d 2069 6e74 2876 666f 290a 2020 2020   = int(vfo).    
+00011c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011c10: 6966 2073 656c 662e 7269 675f 636f 6e74  if self.rig_cont
+00011c20: 726f 6c3a 0a20 2020 2020 2020 2020 2020  rol:.           
+00011c30: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00011c40: 662e 7269 675f 636f 6e74 726f 6c2e 7365  f.rig_control.se
+00011c50: 745f 7666 6f28 696e 7428 7666 6f29 290a  t_vfo(int(vfo)).
+00011c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011c70: 2020 2020 7370 6f74 203d 206a 736f 6e5f      spot = json_
+00011c80: 6461 7461 2e67 6574 2822 7370 6f74 222c  data.get("spot",
+00011c90: 2022 2229 0a20 2020 2020 2020 2020 2020   "").           
+00011ca0: 2020 2020 2020 2020 2073 656c 662e 6361           self.ca
+00011cb0: 6c6c 7369 676e 2e73 6574 5465 7874 2873  llsign.setText(s
+00011cc0: 706f 7429 0a20 2020 2020 2020 2020 2020  pot).           
+00011cd0: 2020 2020 2020 2020 2073 656c 662e 6361           self.ca
+00011ce0: 6c6c 7369 676e 5f63 6861 6e67 6564 2829  llsign_changed()
+00011cf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011d00: 2020 2020 2073 656c 662e 6361 6c6c 7369       self.callsi
+00011d10: 676e 2e73 6574 466f 6375 7328 290a 2020  gn.setFocus().  
+00011d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011d30: 2020 7365 6c66 2e63 616c 6c73 6967 6e2e    self.callsign.
+00011d40: 6163 7469 7661 7465 5769 6e64 6f77 2829  activateWindow()
+00011d50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011d60: 2020 2020 2077 696e 646f 772e 7261 6973       window.rais
+00011d70: 655f 2829 0a20 2020 2020 2020 2020 2020  e_().           
+00011d80: 2020 2020 2020 2020 2023 2066 6720 3d20           # fg = 
+00011d90: 7769 6e64 6f77 2e66 7261 6d65 4765 6f6d  window.frameGeom
+00011da0: 6574 7279 2829 2e74 6f70 4c65 6674 0a20  etry().topLeft. 
+00011db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011dc0: 2020 2023 2023 205f 7769 6474 6820 3d20     # # _width = 
+00011dd0: 7365 6c66 2e73 697a 6528 292e 7769 6474  self.size().widt
+00011de0: 6828 290a 2020 2020 2020 2020 2020 2020  h().            
+00011df0: 2020 2020 2020 2020 2320 2320 5f68 6569          # # _hei
+00011e00: 6768 7420 3d20 7365 6c66 2e73 697a 6528  ght = self.size(
+00011e10: 292e 6865 6967 6874 2829 0a20 2020 2020  ).height().     
+00011e20: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+00011e30: 2023 205f 7820 3d20 7365 6c66 2e70 6f73   # _x = self.pos
+00011e40: 2829 2e78 2829 0a20 2020 2020 2020 2020  ().x().         
+00011e50: 2020 2020 2020 2020 2020 2023 2023 205f             # # _
+00011e60: 7920 3d20 7365 6c66 2e70 6f73 2829 2e79  y = self.pos().y
+00011e70: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
+00011e80: 2020 2020 2020 2023 2023 2070 7269 6e74         # # print
+00011e90: 2866 222a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  (f"*************
+00011ea0: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a20  *************** 
+00011eb0: 7820 7b5f 787d 2079 207b 5f79 7d22 290a  x {_x} y {_y}").
+00011ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011ed0: 2020 2020 2320 2320 7769 6e64 6f77 2e68      # # window.h
+00011ee0: 6964 6528 290a 2020 2020 2020 2020 2020  ide().          
+00011ef0: 2020 2020 2020 2020 2020 2320 2320 7769            # # wi
+00011f00: 6e64 6f77 2e73 686f 7728 290a 2020 2020  ndow.show().    
+00011f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011f20: 2320 2320 7769 6e64 6f77 2e73 6574 4765  # # window.setGe
+00011f30: 6f6d 6574 7279 2830 2c20 302c 205f 7769  ometry(0, 0, _wi
+00011f40: 6474 682c 205f 6865 6967 6874 290a 2020  dth, _height).  
+00011f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011f60: 2020 2320 7769 6e64 6f77 2e73 686f 7728    # window.show(
+00011f70: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00011f80: 2020 2020 2020 2320 7769 6e64 6f77 2e67        # window.g
+00011f90: 656f 6d65 7472 7928 292e 7365 7458 2831  eometry().setX(1
+00011fa0: 3030 290a 2020 2020 2020 2020 2020 2020  00).            
+00011fb0: 2020 2020 2020 2020 2320 7769 6e64 6f77          # window
+00011fc0: 2e67 656f 6d65 7472 7928 292e 7365 7459  .geometry().setY
+00011fd0: 2831 3030 290a 0a20 2020 2064 6566 2063  (100)..    def c
+00011fe0: 775f 6d61 6372 6f73 5f73 7461 7465 5f63  w_macros_state_c
+00011ff0: 6861 6e67 6564 2873 656c 6629 3a0a 2020  hanged(self):.  
+00012000: 2020 2020 2020 2222 224d 656e 7520 6974        """Menu it
+00012010: 656d 2074 6f20 7368 6f77 2f68 6964 6520  em to show/hide 
+00012020: 6d61 6372 6f20 6275 7474 6f6e 7322 2222  macro buttons"""
+00012030: 0a20 2020 2020 2020 2073 656c 662e 7072  .        self.pr
+00012040: 6566 5b22 6377 5f6d 6163 726f 7322 5d20  ef["cw_macros"] 
+00012050: 3d20 7365 6c66 2e61 6374 696f 6e43 575f  = self.actionCW_
+00012060: 4d61 6372 6f73 2e69 7343 6865 636b 6564  Macros.isChecked
+00012070: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
+00012080: 7772 6974 655f 7072 6566 6572 656e 6365  write_preference
+00012090: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
+000120a0: 7368 6f77 5f43 575f 6d61 6372 6f73 2829  show_CW_macros()
+000120b0: 0a0a 2020 2020 6465 6620 7368 6f77 5f43  ..    def show_C
+000120c0: 575f 6d61 6372 6f73 2873 656c 6629 3a0a  W_macros(self):.
+000120d0: 2020 2020 2020 2020 2222 226d 6163 726f          """macro
+000120e0: 2062 7574 746f 6e20 7374 6174 6520 6368   button state ch
+000120f0: 616e 6765 2222 220a 2020 2020 2020 2020  ange""".        
+00012100: 6966 2073 656c 662e 7072 6566 2e67 6574  if self.pref.get
+00012110: 2822 6377 5f6d 6163 726f 7322 293a 0a20  ("cw_macros"):. 
+00012120: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00012130: 4275 7474 6f6e 5f52 6f77 312e 7368 6f77  Button_Row1.show
+00012140: 2829 0a20 2020 2020 2020 2020 2020 2073  ().            s
+00012150: 656c 662e 4275 7474 6f6e 5f52 6f77 322e  elf.Button_Row2.
+00012160: 7368 6f77 2829 0a20 2020 2020 2020 2065  show().        e
+00012170: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00012180: 2073 656c 662e 4275 7474 6f6e 5f52 6f77   self.Button_Row
+00012190: 312e 6869 6465 2829 0a20 2020 2020 2020  1.hide().       
+000121a0: 2020 2020 2073 656c 662e 4275 7474 6f6e       self.Button
+000121b0: 5f52 6f77 322e 6869 6465 2829 0a0a 2020  _Row2.hide()..  
+000121c0: 2020 6465 6620 636f 6d6d 616e 645f 6275    def command_bu
+000121d0: 7474 6f6e 735f 7374 6174 655f 6368 616e  ttons_state_chan
+000121e0: 6765 2873 656c 6629 3a0a 2020 2020 2020  ge(self):.      
+000121f0: 2020 2222 224d 656e 7520 6974 656d 2074    """Menu item t
+00012200: 6f20 7368 6f77 2f68 6964 6520 636f 6d6d  o show/hide comm
+00012210: 616e 6420 6275 7474 6f6e 7322 2222 0a20  and buttons""". 
+00012220: 2020 2020 2020 2073 656c 662e 7072 6566         self.pref
+00012230: 5b22 636f 6d6d 616e 645f 6275 7474 6f6e  ["command_button
+00012240: 7322 5d20 3d20 7365 6c66 2e61 6374 696f  s"] = self.actio
+00012250: 6e43 6f6d 6d61 6e64 5f42 7574 746f 6e73  nCommand_Buttons
+00012260: 2e69 7343 6865 636b 6564 2829 0a20 2020  .isChecked().   
+00012270: 2020 2020 2073 656c 662e 7772 6974 655f       self.write_
+00012280: 7072 6566 6572 656e 6365 2829 0a20 2020  preference().   
+00012290: 2020 2020 2073 656c 662e 7368 6f77 5f63       self.show_c
+000122a0: 6f6d 6d61 6e64 5f62 7574 746f 6e73 2829  ommand_buttons()
+000122b0: 0a0a 2020 2020 6465 6620 7368 6f77 5f63  ..    def show_c
+000122c0: 6f6d 6d61 6e64 5f62 7574 746f 6e73 2873  ommand_buttons(s
+000122d0: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
+000122e0: 2263 6f6d 6d61 6e64 2062 7574 746f 6e20  "command button 
+000122f0: 7374 6174 6520 6368 616e 6765 2222 220a  state change""".
+00012300: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00012310: 7072 6566 2e67 6574 2822 636f 6d6d 616e  pref.get("comman
+00012320: 645f 6275 7474 6f6e 7322 293a 0a20 2020  d_buttons"):.   
+00012330: 2020 2020 2020 2020 2073 656c 662e 436f           self.Co
+00012340: 6d6d 616e 645f 4275 7474 6f6e 732e 7368  mmand_Buttons.sh
+00012350: 6f77 2829 0a20 2020 2020 2020 2065 6c73  ow().        els
+00012360: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+00012370: 656c 662e 436f 6d6d 616e 645f 4275 7474  elf.Command_Butt
+00012380: 6f6e 732e 6869 6465 2829 0a0a 2020 2020  ons.hide()..    
+00012390: 6465 6620 6973 5f66 6c6f 6174 6162 6c65  def is_floatable
+000123a0: 2873 656c 662c 2069 7465 6d3a 2073 7472  (self, item: str
+000123b0: 2920 2d3e 2062 6f6f 6c3a 0a20 2020 2020  ) -> bool:.     
+000123c0: 2020 2022 2222 6368 6563 6b20 746f 2073     """check to s
+000123d0: 6565 2069 6620 7374 7269 6e67 2063 616e  ee if string can
+000123e0: 2062 6520 6120 666c 6f61 7422 2222 0a20   be a float""". 
+000123f0: 2020 2020 2020 2069 6620 6974 656d 2e69         if item.i
+00012400: 736e 756d 6572 6963 2829 3a0a 2020 2020  snumeric():.    
+00012410: 2020 2020 2020 2020 7265 7475 726e 2054          return T
+00012420: 7275 650a 2020 2020 2020 2020 7472 793a  rue.        try:
+00012430: 0a20 2020 2020 2020 2020 2020 205f 7465  .            _te
+00012440: 7374 203d 2066 6c6f 6174 2869 7465 6d29  st = float(item)
+00012450: 0a20 2020 2020 2020 2065 7863 6570 7420  .        except 
+00012460: 5661 6c75 6545 7272 6f72 3a0a 2020 2020  ValueError:.    
+00012470: 2020 2020 2020 2020 7265 7475 726e 2046          return F
+00012480: 616c 7365 0a20 2020 2020 2020 2072 6574  alse.        ret
+00012490: 7572 6e20 5472 7565 0a0a 2020 2020 6465  urn True..    de
+000124a0: 6620 6f74 6865 725f 325f 6368 616e 6765  f other_2_change
+000124b0: 6428 7365 6c66 293a 0a20 2020 2020 2020  d(self):.       
+000124c0: 2022 2222 4361 6c6c 6564 2077 6865 6e20   """Called when 
+000124d0: 7765 206e 6565 6420 746f 2070 6172 7365  we need to parse
+000124e0: 2053 5320 6578 6368 616e 6765 2e22 2222   SS exchange."""
+000124f0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00012500: 2e63 6f6e 7465 7374 3a0a 2020 2020 2020  .contest:.      
+00012510: 2020 2020 2020 6966 2022 4152 524c 2053        if "ARRL S
+00012520: 7765 6570 7374 616b 6573 2220 696e 2073  weepstakes" in s
+00012530: 656c 662e 636f 6e74 6573 742e 6e61 6d65  elf.contest.name
+00012540: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00012550: 2020 7365 6c66 2e63 6f6e 7465 7374 2e70    self.contest.p
+00012560: 6172 7365 5f65 7863 6861 6e67 6528 7365  arse_exchange(se
+00012570: 6c66 290a 0a20 2020 2064 6566 2063 616c  lf)..    def cal
+00012580: 6c73 6967 6e5f 6368 616e 6765 6428 7365  lsign_changed(se
+00012590: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
+000125a0: 4361 6c6c 6564 2077 6865 6e20 7465 7874  Called when text
+000125b0: 2069 6e20 7468 6520 6361 6c6c 7369 676e   in the callsign
+000125c0: 2066 6965 6c64 2068 6173 2063 6861 6e67   field has chang
+000125d0: 6564 2222 220a 2020 2020 2020 2020 7465  ed""".        te
+000125e0: 7874 203d 2073 656c 662e 6361 6c6c 7369  xt = self.callsi
+000125f0: 676e 2e74 6578 7428 290a 2020 2020 2020  gn.text().      
+00012600: 2020 7465 7874 203d 2074 6578 742e 7570    text = text.up
+00012610: 7065 7228 290a 2020 2020 2020 2020 706f  per().        po
+00012620: 7369 7469 6f6e 203d 2073 656c 662e 6361  sition = self.ca
+00012630: 6c6c 7369 676e 2e63 7572 736f 7250 6f73  llsign.cursorPos
+00012640: 6974 696f 6e28 290a 2020 2020 2020 2020  ition().        
+00012650: 7374 7269 7070 6564 5f74 6578 7420 3d20  stripped_text = 
+00012660: 7465 7874 2e73 7472 6970 2829 2e72 6570  text.strip().rep
+00012670: 6c61 6365 2822 2022 2c20 2222 290a 2020  lace(" ", "").  
+00012680: 2020 2020 2020 7365 6c66 2e63 616c 6c73        self.calls
+00012690: 6967 6e2e 7365 7454 6578 7428 7374 7269  ign.setText(stri
+000126a0: 7070 6564 5f74 6578 7429 0a20 2020 2020  pped_text).     
+000126b0: 2020 2073 656c 662e 6361 6c6c 7369 676e     self.callsign
+000126c0: 2e73 6574 4375 7273 6f72 506f 7369 7469  .setCursorPositi
+000126d0: 6f6e 2870 6f73 6974 696f 6e29 0a0a 2020  on(position)..  
+000126e0: 2020 2020 2020 6966 2022 2022 2069 6e20        if " " in 
+000126f0: 7465 7874 3a0a 2020 2020 2020 2020 2020  text:.          
+00012700: 2020 6966 2073 7472 6970 7065 645f 7465    if stripped_te
+00012710: 7874 203d 3d20 2243 5722 3a0a 2020 2020  xt == "CW":.    
+00012720: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00012730: 2e73 6574 6d6f 6465 2822 4357 2229 0a20  .setmode("CW"). 
+00012740: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00012750: 656c 662e 7261 6469 6f5f 7374 6174 655b  elf.radio_state[
+00012760: 226d 6f64 6522 5d20 3d20 2243 5722 0a20  "mode"] = "CW". 
+00012770: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00012780: 6620 7365 6c66 2e72 6967 5f63 6f6e 7472  f self.rig_contr
+00012790: 6f6c 3a0a 2020 2020 2020 2020 2020 2020  ol:.            
+000127a0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+000127b0: 7269 675f 636f 6e74 726f 6c2e 6f6e 6c69  rig_control.onli
+000127c0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000127d0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000127e0: 2e72 6967 5f63 6f6e 7472 6f6c 2e73 6574  .rig_control.set
+000127f0: 5f6d 6f64 6528 2243 5722 290a 2020 2020  _mode("CW").    
+00012800: 2020 2020 2020 2020 2020 2020 6261 6e64              band
+00012810: 203d 2067 6574 6261 6e64 2873 7472 2873   = getband(str(s
+00012820: 656c 662e 7261 6469 6f5f 7374 6174 652e  elf.radio_state.
+00012830: 6765 7428 2276 666f 6122 2c20 2230 2e30  get("vfoa", "0.0
+00012840: 2229 2929 0a20 2020 2020 2020 2020 2020  "))).           
+00012850: 2020 2020 2073 656c 662e 7365 745f 6261       self.set_ba
+00012860: 6e64 5f69 6e64 6963 6174 6f72 2862 616e  nd_indicator(ban
+00012870: 6429 0a20 2020 2020 2020 2020 2020 2020  d).             
+00012880: 2020 2073 656c 662e 7365 745f 7769 6e64     self.set_wind
+00012890: 6f77 5f74 6974 6c65 2829 0a20 2020 2020  ow_title().     
+000128a0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000128b0: 636c 6561 7269 6e70 7574 7328 290a 2020  clearinputs().  
+000128c0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000128d0: 6c66 2e72 6561 645f 6377 5f6d 6163 726f  lf.read_cw_macro
+000128e0: 7328 290a 2020 2020 2020 2020 2020 2020  s().            
+000128f0: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
+00012900: 2020 2020 2020 2069 6620 7374 7269 7070         if stripp
+00012910: 6564 5f74 6578 7420 3d3d 2022 5254 5459  ed_text == "RTTY
+00012920: 223a 0a20 2020 2020 2020 2020 2020 2020  ":.             
+00012930: 2020 2073 656c 662e 7365 746d 6f64 6528     self.setmode(
+00012940: 2252 5454 5922 290a 2020 2020 2020 2020  "RTTY").        
+00012950: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00012960: 7269 675f 636f 6e74 726f 6c3a 0a20 2020  rig_control:.   
+00012970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012980: 2069 6620 7365 6c66 2e72 6967 5f63 6f6e   if self.rig_con
+00012990: 7472 6f6c 2e6f 6e6c 696e 653a 0a20 2020  trol.online:.   
+000129a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000129b0: 2020 2020 2073 656c 662e 7269 675f 636f       self.rig_co
+000129c0: 6e74 726f 6c2e 7365 745f 6d6f 6465 2822  ntrol.set_mode("
+000129d0: 5254 5459 2229 0a20 2020 2020 2020 2020  RTTY").         
+000129e0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+000129f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012a00: 2020 2020 2020 2020 2073 656c 662e 7261           self.ra
+00012a10: 6469 6f5f 7374 6174 655b 226d 6f64 6522  dio_state["mode"
+00012a20: 5d20 3d20 2252 5454 5922 0a20 2020 2020  ] = "RTTY".     
+00012a30: 2020 2020 2020 2020 2020 2062 616e 6420             band 
+00012a40: 3d20 6765 7462 616e 6428 7374 7228 7365  = getband(str(se
+00012a50: 6c66 2e72 6164 696f 5f73 7461 7465 2e67  lf.radio_state.g
+00012a60: 6574 2822 7666 6f61 222c 2022 302e 3022  et("vfoa", "0.0"
+00012a70: 2929 290a 2020 2020 2020 2020 2020 2020  ))).            
+00012a80: 2020 2020 7365 6c66 2e73 6574 5f62 616e      self.set_ban
+00012a90: 645f 696e 6469 6361 746f 7228 6261 6e64  d_indicator(band
+00012aa0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00012ab0: 2020 7365 6c66 2e73 6574 5f77 696e 646f    self.set_windo
+00012ac0: 775f 7469 746c 6528 290a 2020 2020 2020  w_title().      
+00012ad0: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+00012ae0: 6c65 6172 696e 7075 7473 2829 0a20 2020  learinputs().   
+00012af0: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+00012b00: 7572 6e0a 2020 2020 2020 2020 2020 2020  urn.            
+00012b10: 6966 2073 7472 6970 7065 645f 7465 7874  if stripped_text
+00012b20: 203d 3d20 2253 5342 223a 0a20 2020 2020   == "SSB":.     
+00012b30: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00012b40: 7365 746d 6f64 6528 2253 5342 2229 0a20  setmode("SSB"). 
+00012b50: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00012b60: 6620 696e 7428 7365 6c66 2e72 6164 696f  f int(self.radio
+00012b70: 5f73 7461 7465 2e67 6574 2822 7666 6f61  _state.get("vfoa
+00012b80: 222c 2030 2929 203e 2031 3030 3030 3030  ", 0)) > 1000000
+00012b90: 303a 0a20 2020 2020 2020 2020 2020 2020  0:.             
+00012ba0: 2020 2020 2020 2073 656c 662e 7261 6469         self.radi
+00012bb0: 6f5f 7374 6174 655b 226d 6f64 6522 5d20  o_state["mode"] 
+00012bc0: 3d20 2255 5342 220a 2020 2020 2020 2020  = "USB".        
+00012bd0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00012be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012bf0: 2020 7365 6c66 2e72 6164 696f 5f73 7461    self.radio_sta
+00012c00: 7465 5b22 6d6f 6465 225d 203d 2022 4c53  te["mode"] = "LS
+00012c10: 4222 0a20 2020 2020 2020 2020 2020 2020  B".             
+00012c20: 2020 2062 616e 6420 3d20 6765 7462 616e     band = getban
+00012c30: 6428 7374 7228 7365 6c66 2e72 6164 696f  d(str(self.radio
+00012c40: 5f73 7461 7465 2e67 6574 2822 7666 6f61  _state.get("vfoa
+00012c50: 222c 2022 302e 3022 2929 290a 2020 2020  ", "0.0"))).    
+00012c60: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00012c70: 2e73 6574 5f62 616e 645f 696e 6469 6361  .set_band_indica
+00012c80: 746f 7228 6261 6e64 290a 2020 2020 2020  tor(band).      
+00012c90: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+00012ca0: 6574 5f77 696e 646f 775f 7469 746c 6528  et_window_title(
+00012cb0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00012cc0: 2020 6966 2073 656c 662e 7269 675f 636f    if self.rig_co
+00012cd0: 6e74 726f 6c3a 0a20 2020 2020 2020 2020  ntrol:.         
+00012ce0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00012cf0: 7269 675f 636f 6e74 726f 6c2e 7365 745f  rig_control.set_
+00012d00: 6d6f 6465 2873 656c 662e 7261 6469 6f5f  mode(self.radio_
+00012d10: 7374 6174 652e 6765 7428 226d 6f64 6522  state.get("mode"
+00012d20: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
+00012d30: 2020 2073 656c 662e 636c 6561 7269 6e70     self.clearinp
+00012d40: 7574 7328 290a 2020 2020 2020 2020 2020  uts().          
+00012d50: 2020 2020 2020 7365 6c66 2e72 6561 645f        self.read_
+00012d60: 6377 5f6d 6163 726f 7328 290a 2020 2020  cw_macros().    
+00012d70: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00012d80: 726e 0a20 2020 2020 2020 2020 2020 2069  rn.            i
+00012d90: 6620 7374 7269 7070 6564 5f74 6578 7420  f stripped_text 
+00012da0: 3d3d 2022 4f50 4f4e 223a 0a20 2020 2020  == "OPON":.     
+00012db0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00012dc0: 6765 745f 6f70 6f6e 2829 0a20 2020 2020  get_opon().     
+00012dd0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00012de0: 636c 6561 7269 6e70 7574 7328 290a 2020  clearinputs().  
+00012df0: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00012e00: 7475 726e 0a20 2020 2020 2020 2020 2020  turn.           
+00012e10: 2069 6620 7374 7269 7070 6564 5f74 6578   if stripped_tex
+00012e20: 7420 3d3d 2022 4845 4c50 223a 0a20 2020  t == "HELP":.   
+00012e30: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00012e40: 662e 7368 6f77 5f68 656c 705f 6469 616c  f.show_help_dial
+00012e50: 6f67 2829 0a20 2020 2020 2020 2020 2020  og().           
+00012e60: 2020 2020 2073 656c 662e 636c 6561 7269       self.cleari
+00012e70: 6e70 7574 7328 290a 2020 2020 2020 2020  nputs().        
+00012e80: 2020 2020 2020 2020 7265 7475 726e 0a20          return. 
+00012e90: 2020 2020 2020 2020 2020 2069 6620 7374             if st
+00012ea0: 7269 7070 6564 5f74 6578 7420 3d3d 2022  ripped_text == "
+00012eb0: 5445 5354 223a 0a20 2020 2020 2020 2020  TEST":.         
+00012ec0: 2020 2020 2020 2073 656c 662e 7368 6f77         self.show
+00012ed0: 5f6d 6573 7361 6765 5f62 6f78 280a 2020  _message_box(.  
+00012ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012ef0: 2020 225b 4573 635d 5c74 436c 6561 7273    "[Esc]\tClears
+00012f00: 2074 6865 2069 6e70 7574 2066 6965 6c64   the input field
+00012f10: 7320 6f66 2061 6e79 2074 6578 742e 5c6e  s of any text.\n
+00012f20: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+00012f30: 2020 2020 2020 225b 4354 524c 2d45 7363        "[CTRL-Esc
+00012f40: 5d5c 7453 746f 7073 2063 7764 6165 6d6f  ]\tStops cwdaemo
+00012f50: 6e20 6672 6f6d 2073 656e 6469 6e67 204d  n from sending M
+00012f60: 6f72 7365 2e5c 6e22 0a20 2020 2020 2020  orse.\n".       
+00012f70: 2020 2020 2020 2020 2020 2020 2022 5b50               "[P
+00012f80: 6755 705d 5c74 496e 6372 6561 7365 7320  gUp]\tIncreases 
+00012f90: 7468 6520 6377 2073 656e 6469 6e67 2073  the cw sending s
+00012fa0: 7065 6564 2e5c 6e22 0a20 2020 2020 2020  peed.\n".       
+00012fb0: 2020 2020 2020 2020 2020 2020 2022 5b50               "[P
+00012fc0: 6744 6f77 6e5d 5c74 4465 6372 6561 7365  gDown]\tDecrease
+00012fd0: 7320 7468 6520 6377 2073 656e 6469 6e67  s the cw sending
+00012fe0: 2073 7065 6564 2e5c 6e22 0a20 2020 2020   speed.\n".     
+00012ff0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00013000: 5b41 7272 6f77 2d55 705d 204a 756d 7020  [Arrow-Up] Jump 
+00013010: 746f 2074 6865 206e 6578 7420 7370 6f74  to the next spot
+00013020: 2061 626f 7665 2074 6865 2063 7572 7265   above the curre
+00013030: 6e74 2056 464f 2063 7572 736f 725c 6e22  nt VFO cursor\n"
+00013040: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013050: 2020 2020 2022 5c74 696e 2074 6865 2062       "\tin the b
+00013060: 616e 646d 6170 2077 696e 646f 7720 2843  andmap window (C
+00013070: 4154 2052 6571 7569 7265 6429 2e5c 6e22  AT Required).\n"
+00013080: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013090: 2020 2020 2022 5b41 7272 6f77 2d44 6f77       "[Arrow-Dow
+000130a0: 6e5d 204a 756d 7020 746f 2074 6865 206e  n] Jump to the n
+000130b0: 6578 7420 7370 6f74 2062 656c 6f77 2074  ext spot below t
+000130c0: 6865 2063 7572 7265 6e74 5c6e 220a 2020  he current\n".  
 000130d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000130e0: 2020 2020 225b 5441 425d 5c74 4d6f 7665      "[TAB]\tMove
-000130f0: 2063 7572 736f 7220 746f 2074 6865 2072   cursor to the r
-00013100: 6967 6874 206f 6e65 2066 6965 6c64 2e5c  ight one field.\
-00013110: 6e22 0a20 2020 2020 2020 2020 2020 2020  n".             
-00013120: 2020 2020 2020 2022 5b53 6869 6674 2d54         "[Shift-T
-00013130: 6162 5d5c 744d 6f76 6520 6375 7273 6f72  ab]\tMove cursor
-00013140: 206c 6566 7420 4f6e 6520 6669 656c 642e   left One field.
-00013150: 5c6e 220a 2020 2020 2020 2020 2020 2020  \n".            
-00013160: 2020 2020 2020 2020 225b 5350 4143 455d          "[SPACE]
-00013170: 5c74 5768 656e 2069 6e20 7468 6520 6361  \tWhen in the ca
-00013180: 6c6c 7369 676e 2066 6965 6c64 2c20 7769  llsign field, wi
-00013190: 6c6c 206d 6f76 6520 7468 6520 696e 7075  ll move the inpu
-000131a0: 7420 746f 2074 6865 5c6e 220a 2020 2020  t to the\n".    
-000131b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000131c0: 225c 7466 6972 7374 2066 6965 6c64 206e  "\tfirst field n
-000131d0: 6565 6465 6420 666f 7220 7468 6520 6578  eeded for the ex
-000131e0: 6368 616e 6765 2e5c 6e22 0a20 2020 2020  change.\n".     
-000131f0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00013200: 5b45 6e74 6572 5d5c 7453 7562 6d69 7473  [Enter]\tSubmits
-00013210: 2074 6865 2066 6965 6c64 7320 746f 2074   the fields to t
-00013220: 6865 206c 6f67 2e5c 6e22 0a20 2020 2020  he log.\n".     
-00013230: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00013240: 5b46 312d 4631 325d 5c74 5365 6e64 2028  [F1-F12]\tSend (
-00013250: 4357 206f 7220 566f 6963 6529 206d 6163  CW or Voice) mac
-00013260: 726f 732e 5c6e 220a 2020 2020 2020 2020  ros.\n".        
-00013270: 2020 2020 2020 2020 2020 2020 225b 4354              "[CT
-00013280: 524c 2d53 5d5c 7453 706f 7420 4361 6c6c  RL-S]\tSpot Call
-00013290: 7369 676e 2074 6f20 7468 6520 636c 7573  sign to the clus
-000132a0: 7465 722e 5c6e 220a 2020 2020 2020 2020  ter.\n".        
-000132b0: 2020 2020 2020 2020 2020 2020 225b 4354              "[CT
-000132c0: 524c 2d47 5d5c 7454 756e 6520 746f 2061  RL-G]\tTune to a
-000132d0: 2073 706f 7420 6d61 7463 6869 6e67 2070   spot matching p
-000132e0: 6172 7469 616c 2074 6578 7420 696e 2074  artial text in t
-000132f0: 6865 2063 616c 6c73 6967 6e5c 6e22 0a20  he callsign\n". 
-00013300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013310: 2020 2022 5c74 656e 7472 7920 6669 656c     "\tentry fiel
-00013320: 6420 2843 4154 2052 6571 7569 7265 6429  d (CAT Required)
-00013330: 2e5c 6e22 0a20 2020 2020 2020 2020 2020  .\n".           
-00013340: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-00013350: 2020 2020 2020 2073 656c 662e 636c 6561         self.clea
-00013360: 7269 6e70 7574 7328 290a 2020 2020 2020  rinputs().      
-00013370: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00013380: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00013390: 7365 6c66 2e69 735f 666c 6f61 7461 626c  self.is_floatabl
-000133a0: 6528 7374 7269 7070 6564 5f74 6578 7429  e(stripped_text)
-000133b0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000133c0: 2020 7666 6f20 3d20 666c 6f61 7428 7374    vfo = float(st
-000133d0: 7269 7070 6564 5f74 6578 7429 0a20 2020  ripped_text).   
-000133e0: 2020 2020 2020 2020 2020 2020 2076 666f               vfo
-000133f0: 203d 2069 6e74 2876 666f 202a 2031 3030   = int(vfo * 100
-00013400: 3029 0a20 2020 2020 2020 2020 2020 2020  0).             
-00013410: 2020 2062 616e 6420 3d20 6765 7462 616e     band = getban
-00013420: 6428 7374 7228 7666 6f29 290a 2020 2020  d(str(vfo)).    
-00013430: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00013440: 2e73 6574 5f62 616e 645f 696e 6469 6361  .set_band_indica
-00013450: 746f 7228 6261 6e64 290a 2020 2020 2020  tor(band).      
-00013460: 2020 2020 2020 2020 2020 2320 7365 6c66            # self
-00013470: 2e63 6f6e 7461 6374 5b22 4261 6e64 225d  .contact["Band"]
-00013480: 203d 2067 6574 5f6c 6f67 6765 645f 6261   = get_logged_ba
-00013490: 6e64 2873 7472 2873 656c 662e 7261 6469  nd(str(self.radi
-000134a0: 6f5f 7374 6174 652e 6765 7428 2276 666f  o_state.get("vfo
-000134b0: 6122 2c20 302e 3029 2929 0a20 2020 2020  a", 0.0))).     
-000134c0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000134d0: 7261 6469 6f5f 7374 6174 655b 2276 666f  radio_state["vfo
-000134e0: 6122 5d20 3d20 7666 6f0a 2020 2020 2020  a"] = vfo.      
-000134f0: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
-00013500: 6574 5f77 696e 646f 775f 7469 746c 6528  et_window_title(
-00013510: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00013520: 2020 7365 6c66 2e63 6c65 6172 696e 7075    self.clearinpu
-00013530: 7473 2829 0a20 2020 2020 2020 2020 2020  ts().           
-00013540: 2020 2020 2069 6620 7365 6c66 2e72 6967       if self.rig
-00013550: 5f63 6f6e 7472 6f6c 3a0a 2020 2020 2020  _control:.      
-00013560: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00013570: 6c66 2e72 6967 5f63 6f6e 7472 6f6c 2e73  lf.rig_control.s
-00013580: 6574 5f76 666f 2876 666f 290a 2020 2020  et_vfo(vfo).    
-00013590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000135a0: 7265 7475 726e 0a20 2020 2020 2020 2020  return.         
-000135b0: 2020 2020 2020 2063 6d64 203d 207b 7d0a         cmd = {}.
-000135c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000135d0: 636d 645b 2263 6d64 225d 203d 2022 5241  cmd["cmd"] = "RA
-000135e0: 4449 4f5f 5354 4154 4522 0a20 2020 2020  DIO_STATE".     
-000135f0: 2020 2020 2020 2020 2020 2063 6d64 5b22             cmd["
-00013600: 7374 6174 696f 6e22 5d20 3d20 706c 6174  station"] = plat
-00013610: 666f 726d 2e6e 6f64 6528 290a 2020 2020  form.node().    
-00013620: 2020 2020 2020 2020 2020 2020 636d 645b              cmd[
-00013630: 2262 616e 6422 5d20 3d20 6261 6e64 0a20  "band"] = band. 
-00013640: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00013650: 6d64 5b22 7666 6f61 225d 203d 2076 666f  md["vfoa"] = vfo
-00013660: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013670: 2073 656c 662e 6d75 6c74 6963 6173 745f   self.multicast_
-00013680: 696e 7465 7266 6163 652e 7365 6e64 5f61  interface.send_a
-00013690: 735f 6a73 6f6e 2863 6d64 290a 2020 2020  s_json(cmd).    
-000136a0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-000136b0: 726e 0a0a 2020 2020 2020 2020 2020 2020  rn..            
-000136c0: 7365 6c66 2e63 6865 636b 5f63 616c 6c73  self.check_calls
-000136d0: 6967 6e28 7374 7269 7070 6564 5f74 6578  ign(stripped_tex
-000136e0: 7429 0a20 2020 2020 2020 2020 2020 2069  t).            i
-000136f0: 6620 7365 6c66 2e63 6865 636b 5f64 7570  f self.check_dup
-00013700: 6528 7374 7269 7070 6564 5f74 6578 7429  e(stripped_text)
-00013710: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00013720: 2020 7365 6c66 2e64 7570 655f 696e 6469    self.dupe_indi
-00013730: 6361 746f 722e 7368 6f77 2829 0a20 2020  cator.show().   
-00013740: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-00013750: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00013760: 656c 662e 6475 7065 5f69 6e64 6963 6174  elf.dupe_indicat
-00013770: 6f72 2e68 6964 6528 290a 2020 2020 2020  or.hide().      
-00013780: 2020 2020 2020 5f74 6865 7468 7265 6164        _thethread
-00013790: 203d 2074 6872 6561 6469 6e67 2e54 6872   = threading.Thr
-000137a0: 6561 6428 0a20 2020 2020 2020 2020 2020  ead(.           
-000137b0: 2020 2020 2074 6172 6765 743d 7365 6c66       target=self
-000137c0: 2e63 6865 636b 5f63 616c 6c73 6967 6e32  .check_callsign2
-000137d0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000137e0: 2020 6172 6773 3d28 7465 7874 2c29 2c0a    args=(text,),.
-000137f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013800: 6461 656d 6f6e 3d54 7275 652c 0a20 2020  daemon=True,.   
-00013810: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-00013820: 2020 2020 2020 205f 7468 6574 6872 6561         _thethrea
-00013830: 642e 7374 6172 7428 290a 2020 2020 2020  d.start().      
-00013840: 2020 2020 2020 7365 6c66 2e6e 6578 745f        self.next_
-00013850: 6669 656c 642e 7365 7446 6f63 7573 2829  field.setFocus()
-00013860: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00013870: 7572 6e0a 2020 2020 2020 2020 636d 6420  urn.        cmd 
-00013880: 3d20 7b7d 0a20 2020 2020 2020 2063 6d64  = {}.        cmd
-00013890: 5b22 636d 6422 5d20 3d20 2243 414c 4c43  ["cmd"] = "CALLC
-000138a0: 4841 4e47 4544 220a 2020 2020 2020 2020  HANGED".        
-000138b0: 636d 645b 2273 7461 7469 6f6e 225d 203d  cmd["station"] =
-000138c0: 2070 6c61 7466 6f72 6d2e 6e6f 6465 2829   platform.node()
-000138d0: 0a20 2020 2020 2020 2063 6d64 5b22 6361  .        cmd["ca
-000138e0: 6c6c 225d 203d 2073 7472 6970 7065 645f  ll"] = stripped_
-000138f0: 7465 7874 0a20 2020 2020 2020 2073 656c  text.        sel
-00013900: 662e 6d75 6c74 6963 6173 745f 696e 7465  f.multicast_inte
-00013910: 7266 6163 652e 7365 6e64 5f61 735f 6a73  rface.send_as_js
-00013920: 6f6e 2863 6d64 290a 2020 2020 2020 2020  on(cmd).        
-00013930: 7365 6c66 2e63 6865 636b 5f63 616c 6c73  self.check_calls
-00013940: 6967 6e28 7374 7269 7070 6564 5f74 6578  ign(stripped_tex
-00013950: 7429 0a0a 2020 2020 6465 6620 6368 6563  t)..    def chec
-00013960: 6b5f 6361 6c6c 7369 676e 2873 656c 662c  k_callsign(self,
-00013970: 2063 616c 6c73 6967 6e29 3a0a 2020 2020   callsign):.    
-00013980: 2020 2020 2222 2243 6865 636b 2063 616c      """Check cal
-00013990: 6c20 6173 2065 6e74 6572 6564 2222 220a  l as entered""".
-000139a0: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
-000139b0: 2073 656c 662e 6374 795f 6c6f 6f6b 7570   self.cty_lookup
-000139c0: 2863 616c 6c73 6967 6e29 0a20 2020 2020  (callsign).     
-000139d0: 2020 2064 6562 7567 5f72 6573 756c 7420     debug_result 
-000139e0: 3d20 6622 7b72 6573 756c 747d 220a 2020  = f"{result}".  
-000139f0: 2020 2020 2020 6c6f 6767 6572 2e64 6562        logger.deb
-00013a00: 7567 2822 2573 222c 2064 6562 7567 5f72  ug("%s", debug_r
-00013a10: 6573 756c 7429 0a20 2020 2020 2020 2069  esult).        i
-00013a20: 6620 7265 7375 6c74 3a0a 2020 2020 2020  f result:.      
-00013a30: 2020 2020 2020 666f 7220 6120 696e 2072        for a in r
-00013a40: 6573 756c 742e 6974 656d 7328 293a 0a20  esult.items():. 
-00013a50: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00013a60: 6e74 6974 7920 3d20 615b 315d 2e67 6574  ntity = a[1].get
-00013a70: 2822 656e 7469 7479 222c 2022 2229 0a20  ("entity", ""). 
-00013a80: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00013a90: 7120 3d20 615b 315d 2e67 6574 2822 6371  q = a[1].get("cq
-00013aa0: 222c 2022 2229 0a20 2020 2020 2020 2020  ", "").         
-00013ab0: 2020 2020 2020 2069 7475 203d 2061 5b31         itu = a[1
-00013ac0: 5d2e 6765 7428 2269 7475 222c 2022 2229  ].get("itu", "")
-00013ad0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013ae0: 2063 6f6e 7469 6e65 6e74 203d 2061 5b31   continent = a[1
-00013af0: 5d2e 6765 7428 2263 6f6e 7469 6e65 6e74  ].get("continent
-00013b00: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
-00013b10: 2020 206c 6174 203d 2066 6c6f 6174 2861     lat = float(a
-00013b20: 5b31 5d2e 6765 7428 226c 6174 222c 2022  [1].get("lat", "
-00013b30: 302e 3022 2929 0a20 2020 2020 2020 2020  0.0")).         
-00013b40: 2020 2020 2020 206c 6f6e 203d 2066 6c6f         lon = flo
-00013b50: 6174 2861 5b31 5d2e 6765 7428 226c 6f6e  at(a[1].get("lon
-00013b60: 6722 2c20 2230 2e30 2229 290a 2020 2020  g", "0.0")).    
-00013b70: 2020 2020 2020 2020 2020 2020 6c6f 6e20              lon 
-00013b80: 3d20 6c6f 6e20 2a20 2d31 2020 2320 6374  = lon * -1  # ct
-00013b90: 792e 6461 7420 6669 6c65 2069 6e76 6572  y.dat file inver
-00013ba0: 7473 206c 6f6e 6769 7475 6465 730a 2020  ts longitudes.  
-00013bb0: 2020 2020 2020 2020 2020 2020 2020 7072                pr
-00013bc0: 696d 6172 795f 7066 7820 3d20 615b 315d  imary_pfx = a[1]
-00013bd0: 2e67 6574 2822 7072 696d 6172 795f 7066  .get("primary_pf
-00013be0: 7822 2c20 2222 290a 2020 2020 2020 2020  x", "").        
-00013bf0: 2020 2020 2020 2020 6865 6164 696e 6720          heading 
-00013c00: 3d20 6265 6172 696e 675f 7769 7468 5f6c  = bearing_with_l
-00013c10: 6174 6c6f 6e28 7365 6c66 2e73 7461 7469  atlon(self.stati
-00013c20: 6f6e 2e67 6574 2822 4772 6964 5371 7561  on.get("GridSqua
-00013c30: 7265 2229 2c20 6c61 742c 206c 6f6e 290a  re"), lat, lon).
-00013c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013c50: 6b69 6c6f 6d65 7465 7273 203d 2064 6973  kilometers = dis
-00013c60: 7461 6e63 655f 7769 7468 5f6c 6174 6c6f  tance_with_latlo
-00013c70: 6e28 0a20 2020 2020 2020 2020 2020 2020  n(.             
-00013c80: 2020 2020 2020 2073 656c 662e 7374 6174         self.stat
-00013c90: 696f 6e2e 6765 7428 2247 7269 6453 7175  ion.get("GridSqu
-00013ca0: 6172 6522 292c 206c 6174 2c20 6c6f 6e0a  are"), lat, lon.
-00013cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013cc0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00013cd0: 2020 7365 6c66 2e68 6561 6469 6e67 5f64    self.heading_d
-00013ce0: 6973 7461 6e63 652e 7365 7454 6578 7428  istance.setText(
-00013cf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013d00: 2020 2020 2066 2252 6567 696f 6e61 6c20       f"Regional 
-00013d10: 4864 6720 7b68 6561 6469 6e67 7dc2 b020  Hdg {heading}.. 
-00013d20: 4c50 207b 7265 6369 7072 6f63 6f6c 2868  LP {reciprocol(h
-00013d30: 6561 6469 6e67 297d c2b0 202f 2022 0a20  eading)}.. / ". 
-00013d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013d50: 2020 2066 2264 6973 7461 6e63 6520 7b69     f"distance {i
-00013d60: 6e74 286b 696c 6f6d 6574 6572 732a 302e  nt(kilometers*0.
-00013d70: 3632 3133 3731 297d 6d69 207b 6b69 6c6f  621371)}mi {kilo
-00013d80: 6d65 7465 7273 7d6b 6d22 0a20 2020 2020  meters}km".     
-00013d90: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-00013da0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00013db0: 662e 636f 6e74 6163 745b 2243 6f75 6e74  f.contact["Count
-00013dc0: 7279 5072 6566 6978 225d 203d 2070 7269  ryPrefix"] = pri
-00013dd0: 6d61 7279 5f70 6678 0a20 2020 2020 2020  mary_pfx.       
-00013de0: 2020 2020 2020 2020 2073 656c 662e 636f           self.co
-00013df0: 6e74 6163 745b 225a 4e22 5d20 3d20 696e  ntact["ZN"] = in
-00013e00: 7428 6371 290a 2020 2020 2020 2020 2020  t(cq).          
-00013e10: 2020 2020 2020 7365 6c66 2e63 6f6e 7461        self.conta
-00013e20: 6374 5b22 436f 6e74 696e 656e 7422 5d20  ct["Continent"] 
-00013e30: 3d20 636f 6e74 696e 656e 740a 2020 2020  = continent.    
-00013e40: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00013e50: 2e64 785f 656e 7469 7479 2e73 6574 5465  .dx_entity.setTe
-00013e60: 7874 280a 2020 2020 2020 2020 2020 2020  xt(.            
-00013e70: 2020 2020 2020 2020 6622 7b70 7269 6d61          f"{prima
-00013e80: 7279 5f70 6678 7d3a 207b 636f 6e74 696e  ry_pfx}: {contin
-00013e90: 656e 747d 2f7b 656e 7469 7479 7d20 6371  ent}/{entity} cq
-00013ea0: 3a7b 6371 7d20 6974 753a 7b69 7475 7d22  :{cq} itu:{itu}"
-00013eb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013ec0: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
-00013ed0: 2020 2069 6620 6c65 6e28 6361 6c6c 7369     if len(callsi
-00013ee0: 676e 2920 3e20 323a 0a20 2020 2020 2020  gn) > 2:.       
-00013ef0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00013f00: 7365 6c66 2e63 6f6e 7465 7374 3a0a 2020  self.contest:.  
-00013f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013f20: 2020 2020 2020 7365 6c66 2e63 6f6e 7465        self.conte
-00013f30: 7374 2e70 7265 6669 6c6c 2873 656c 6629  st.prefill(self)
-00013f40: 0a0a 2020 2020 6465 6620 6368 6563 6b5f  ..    def check_
-00013f50: 6361 6c6c 7369 676e 3228 7365 6c66 2c20  callsign2(self, 
-00013f60: 6361 6c6c 7369 676e 293a 0a20 2020 2020  callsign):.     
-00013f70: 2020 2022 2222 4368 6563 6b20 6361 6c6c     """Check call
-00013f80: 206f 6e63 6520 656e 7465 7265 6422 2222   once entered"""
-00013f90: 0a20 2020 2020 2020 2063 616c 6c73 6967  .        callsig
-00013fa0: 6e20 3d20 6361 6c6c 7369 676e 2e73 7472  n = callsign.str
-00013fb0: 6970 2829 0a20 2020 2020 2020 2064 6562  ip().        deb
-00013fc0: 7567 5f6c 6f6f 6b75 7020 3d20 6622 7b73  ug_lookup = f"{s
-00013fd0: 656c 662e 6c6f 6f6b 5f75 707d 220a 2020  elf.look_up}".  
-00013fe0: 2020 2020 2020 6c6f 6767 6572 2e64 6562        logger.deb
-00013ff0: 7567 2822 2573 2c20 2573 222c 2063 616c  ug("%s, %s", cal
-00014000: 6c73 6967 6e2c 2064 6562 7567 5f6c 6f6f  lsign, debug_loo
-00014010: 6b75 7029 0a20 2020 2020 2020 2069 6620  kup).        if 
-00014020: 6861 7361 7474 7228 7365 6c66 2e6c 6f6f  hasattr(self.loo
-00014030: 6b5f 7570 2c20 2273 6573 7369 6f6e 2229  k_up, "session")
-00014040: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
-00014050: 2073 656c 662e 6c6f 6f6b 5f75 702e 7365   self.look_up.se
-00014060: 7373 696f 6e3a 0a20 2020 2020 2020 2020  ssion:.         
-00014070: 2020 2020 2020 2072 6573 706f 6e73 6520         response 
-00014080: 3d20 7365 6c66 2e6c 6f6f 6b5f 7570 2e6c  = self.look_up.l
-00014090: 6f6f 6b75 7028 6361 6c6c 7369 676e 290a  ookup(callsign).
-000140a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000140b0: 6465 6275 675f 7265 7370 6f6e 7365 203d  debug_response =
-000140c0: 2066 227b 7265 7370 6f6e 7365 7d22 0a20   f"{response}". 
-000140d0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-000140e0: 6f67 6765 722e 6465 6275 6728 2254 6865  ogger.debug("The
-000140f0: 2052 6573 706f 6e73 653a 2025 735c 6e22   Response: %s\n"
-00014100: 2c20 6465 6275 675f 7265 7370 6f6e 7365  , debug_response
-00014110: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00014120: 2020 6966 2072 6573 706f 6e73 653a 0a20    if response:. 
-00014130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014140: 2020 2074 6865 6972 6772 6964 203d 2072     theirgrid = r
-00014150: 6573 706f 6e73 652e 6765 7428 2267 7269  esponse.get("gri
-00014160: 6422 290a 2020 2020 2020 2020 2020 2020  d").            
-00014170: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
-00014180: 7461 6374 5b22 4772 6964 5371 7561 7265  tact["GridSquare
-00014190: 225d 203d 2074 6865 6972 6772 6964 0a20  "] = theirgrid. 
-000141a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000141b0: 2020 205f 7468 6569 7263 6f75 6e74 7279     _theircountry
-000141c0: 203d 2072 6573 706f 6e73 652e 6765 7428   = response.get(
-000141d0: 2263 6f75 6e74 7279 2229 0a20 2020 2020  "country").     
-000141e0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-000141f0: 6620 7365 6c66 2e73 7461 7469 6f6e 2e67  f self.station.g
-00014200: 6574 2822 4772 6964 5371 7561 7265 222c  et("GridSquare",
-00014210: 2022 2229 3a0a 2020 2020 2020 2020 2020   ""):.          
-00014220: 2020 2020 2020 2020 2020 2020 2020 6865                he
-00014230: 6164 696e 6720 3d20 6265 6172 696e 6728  ading = bearing(
-00014240: 7365 6c66 2e73 7461 7469 6f6e 2e67 6574  self.station.get
-00014250: 2822 4772 6964 5371 7561 7265 222c 2022  ("GridSquare", "
-00014260: 2229 2c20 7468 6569 7267 7269 6429 0a20  "), theirgrid). 
-00014270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014280: 2020 2020 2020 206b 696c 6f6d 6574 6572         kilometer
-00014290: 7320 3d20 6469 7374 616e 6365 2873 656c  s = distance(sel
-000142a0: 662e 7374 6174 696f 6e2e 6765 7428 2247  f.station.get("G
-000142b0: 7269 6453 7175 6172 6522 292c 2074 6865  ridSquare"), the
-000142c0: 6972 6772 6964 290a 2020 2020 2020 2020  irgrid).        
-000142d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000142e0: 7365 6c66 2e68 6561 6469 6e67 5f64 6973  self.heading_dis
-000142f0: 7461 6e63 652e 7365 7454 6578 7428 0a20  tance.setText(. 
-00014300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014310: 2020 2020 2020 2020 2020 2066 227b 7468             f"{th
-00014320: 6569 7267 7269 647d 2048 6467 207b 6865  eirgrid} Hdg {he
-00014330: 6164 696e 677d c2b0 204c 5020 7b72 6563  ading}.. LP {rec
-00014340: 6970 726f 636f 6c28 6865 6164 696e 6729  iprocol(heading)
-00014350: 7dc2 b020 2f20 220a 2020 2020 2020 2020  }.. / ".        
-00014360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014370: 2020 2020 6622 6469 7374 616e 6365 207b      f"distance {
-00014380: 696e 7428 6b69 6c6f 6d65 7465 7273 2a30  int(kilometers*0
-00014390: 2e36 3231 3337 3129 7d6d 6920 7b6b 696c  .621371)}mi {kil
-000143a0: 6f6d 6574 6572 737d 6b6d 220a 2020 2020  ometers}km".    
-000143b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000143c0: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-000143d0: 2020 2020 2020 2020 2020 2320 7365 6c66            # self
-000143e0: 2e64 785f 656e 7469 7479 2e73 6574 5465  .dx_entity.setTe
-000143f0: 7874 2866 227b 7468 6569 7263 6f75 6e74  xt(f"{theircount
-00014400: 7279 7d22 290a 2020 2020 2020 2020 2020  ry}").          
-00014410: 2020 2020 2020 2320 656c 7365 3a0a 2020        # else:.  
-00014420: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00014430: 7365 6c66 2e68 6561 6469 6e67 5f64 6973  self.heading_dis
-00014440: 7461 6e63 652e 7365 7454 6578 7428 224c  tance.setText("L
-00014450: 6f6f 6b75 7020 6661 696c 6564 2e22 290a  ookup failed.").
-00014460: 0a20 2020 2064 6566 2063 6865 636b 5f64  .    def check_d
-00014470: 7570 6528 7365 6c66 2c20 6361 6c6c 3a20  upe(self, call: 
-00014480: 7374 7229 202d 3e20 626f 6f6c 3a0a 2020  str) -> bool:.  
-00014490: 2020 2020 2020 2222 2243 6865 636b 7320        """Checks 
-000144a0: 6966 2061 2063 616c 6c73 6967 6e20 6973  if a callsign is
-000144b0: 2061 2064 7570 6520 6f6e 2063 7572 7265   a dupe on curre
-000144c0: 6e74 2062 616e 642f 6d6f 6465 2e22 2222  nt band/mode."""
-000144d0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-000144e0: 2e63 6f6e 7465 7374 2069 7320 4e6f 6e65  .contest is None
-000144f0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00014500: 6c66 2e73 686f 775f 6d65 7373 6167 655f  lf.show_message_
-00014510: 626f 7828 2259 6f75 2068 6176 6520 6e6f  box("You have no
-00014520: 2063 6f6e 7465 7374 206c 6f61 6465 642e   contest loaded.
-00014530: 2229 0a20 2020 2020 2020 2020 2020 2072  ").            r
-00014540: 6574 7572 6e20 4661 6c73 650a 2020 2020  eturn False.    
-00014550: 2020 2020 7365 6c66 2e63 6f6e 7465 7374      self.contest
-00014560: 2e70 7265 6475 7065 2873 656c 6629 0a20  .predupe(self). 
-00014570: 2020 2020 2020 2062 616e 6420 3d20 666c         band = fl
-00014580: 6f61 7428 6765 745f 6c6f 6767 6564 5f62  oat(get_logged_b
-00014590: 616e 6428 7374 7228 7365 6c66 2e72 6164  and(str(self.rad
-000145a0: 696f 5f73 7461 7465 2e67 6574 2822 7666  io_state.get("vf
-000145b0: 6f61 222c 2030 2e30 2929 2929 0a20 2020  oa", 0.0)))).   
-000145c0: 2020 2020 206d 6f64 6520 3d20 7365 6c66       mode = self
-000145d0: 2e72 6164 696f 5f73 7461 7465 2e67 6574  .radio_state.get
-000145e0: 2822 6d6f 6465 222c 2022 2229 0a20 2020  ("mode", "").   
-000145f0: 2020 2020 2064 6562 7567 6c69 6e65 203d       debugline =
-00014600: 2028 0a20 2020 2020 2020 2020 2020 2066   (.            f
-00014610: 2243 616c 6c3a 207b 6361 6c6c 7d20 4261  "Call: {call} Ba
-00014620: 6e64 3a20 7b62 616e 647d 204d 6f64 653a  nd: {band} Mode:
-00014630: 207b 6d6f 6465 7d20 4475 7065 7479 7065   {mode} Dupetype
-00014640: 3a20 7b73 656c 662e 636f 6e74 6573 742e  : {self.contest.
-00014650: 6475 7065 5f74 7970 657d 220a 2020 2020  dupe_type}".    
-00014660: 2020 2020 290a 2020 2020 2020 2020 6c6f      ).        lo
-00014670: 6767 6572 2e64 6562 7567 2822 2573 222c  gger.debug("%s",
-00014680: 2064 6562 7567 6c69 6e65 290a 2020 2020   debugline).    
-00014690: 2020 2020 6966 2073 656c 662e 636f 6e74      if self.cont
-000146a0: 6573 742e 6475 7065 5f74 7970 6520 3d3d  est.dupe_type ==
-000146b0: 2031 3a0a 2020 2020 2020 2020 2020 2020   1:.            
-000146c0: 7265 7375 6c74 203d 2073 656c 662e 6461  result = self.da
-000146d0: 7461 6261 7365 2e63 6865 636b 5f64 7570  tabase.check_dup
-000146e0: 6528 6361 6c6c 290a 2020 2020 2020 2020  e(call).        
-000146f0: 6966 2073 656c 662e 636f 6e74 6573 742e  if self.contest.
-00014700: 6475 7065 5f74 7970 6520 3d3d 2032 3a0a  dupe_type == 2:.
-00014710: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-00014720: 6c74 203d 2073 656c 662e 6461 7461 6261  lt = self.databa
-00014730: 7365 2e63 6865 636b 5f64 7570 655f 6f6e  se.check_dupe_on
-00014740: 5f62 616e 6428 6361 6c6c 2c20 6261 6e64  _band(call, band
-00014750: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
-00014760: 662e 636f 6e74 6573 742e 6475 7065 5f74  f.contest.dupe_t
-00014770: 7970 6520 3d3d 2033 3a0a 2020 2020 2020  ype == 3:.      
-00014780: 2020 2020 2020 7265 7375 6c74 203d 2073        result = s
-00014790: 656c 662e 6461 7461 6261 7365 2e63 6865  elf.database.che
-000147a0: 636b 5f64 7570 655f 6f6e 5f62 616e 645f  ck_dupe_on_band_
-000147b0: 6d6f 6465 2863 616c 6c2c 2062 616e 642c  mode(call, band,
-000147c0: 206d 6f64 6529 0a20 2020 2020 2020 2069   mode).        i
-000147d0: 6620 7365 6c66 2e63 6f6e 7465 7374 2e64  f self.contest.d
-000147e0: 7570 655f 7479 7065 203d 3d20 343a 0a20  upe_type == 4:. 
-000147f0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-00014800: 7420 3d20 7b22 6973 6475 7065 223a 2046  t = {"isdupe": F
-00014810: 616c 7365 7d0a 2020 2020 2020 2020 6465  alse}.        de
-00014820: 6275 676c 696e 6520 3d20 6622 7b72 6573  bugline = f"{res
-00014830: 756c 747d 220a 2020 2020 2020 2020 6c6f  ult}".        lo
-00014840: 6767 6572 2e64 6562 7567 2822 2573 222c  gger.debug("%s",
-00014850: 2064 6562 7567 6c69 6e65 290a 2020 2020   debugline).    
-00014860: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
-00014870: 742e 6765 7428 2269 7364 7570 6522 2c20  t.get("isdupe", 
-00014880: 4661 6c73 6529 0a0a 2020 2020 6465 6620  False)..    def 
-00014890: 7365 746d 6f64 6528 7365 6c66 2c20 6d6f  setmode(self, mo
-000148a0: 6465 3a20 7374 7229 202d 3e20 4e6f 6e65  de: str) -> None
-000148b0: 3a0a 2020 2020 2020 2020 2222 2273 7475  :.        """stu
-000148c0: 6220 666f 7220 7768 656e 2074 6865 206d  b for when the m
-000148d0: 6f64 6520 6368 616e 6765 732e 2222 220a  ode changes.""".
-000148e0: 2020 2020 2020 2020 6966 206d 6f64 6520          if mode 
-000148f0: 3d3d 2022 4357 223a 0a20 2020 2020 2020  == "CW":.       
-00014900: 2020 2020 2069 6620 7365 6c66 2e63 7572       if self.cur
-00014910: 7265 6e74 5f6d 6f64 6520 213d 2022 4357  rent_mode != "CW
-00014920: 223a 0a20 2020 2020 2020 2020 2020 2020  ":.             
-00014930: 2020 2073 656c 662e 6375 7272 656e 745f     self.current_
-00014940: 6d6f 6465 203d 2022 4357 220a 2020 2020  mode = "CW".    
-00014950: 2020 2020 2020 2020 2020 2020 2320 7365              # se
-00014960: 6c66 2e6d 6f64 652e 7365 7454 6578 7428  lf.mode.setText(
-00014970: 2243 5722 290a 2020 2020 2020 2020 2020  "CW").          
-00014980: 2020 2020 2020 7365 6c66 2e73 656e 742e        self.sent.
-00014990: 7365 7454 6578 7428 2235 3939 2229 0a20  setText("599"). 
-000149a0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000149b0: 656c 662e 7265 6365 6976 652e 7365 7454  elf.receive.setT
-000149c0: 6578 7428 2235 3939 2229 0a20 2020 2020  ext("599").     
-000149d0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000149e0: 7265 6164 5f63 775f 6d61 6372 6f73 2829  read_cw_macros()
-000149f0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00014a00: 7572 6e0a 2020 2020 2020 2020 6966 206d  urn.        if m
-00014a10: 6f64 6520 3d3d 2022 5353 4222 3a0a 2020  ode == "SSB":.  
-00014a20: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-00014a30: 662e 6375 7272 656e 745f 6d6f 6465 2021  f.current_mode !
-00014a40: 3d20 2253 5342 223a 0a20 2020 2020 2020  = "SSB":.       
-00014a50: 2020 2020 2020 2020 2073 656c 662e 6375           self.cu
-00014a60: 7272 656e 745f 6d6f 6465 203d 2022 5353  rrent_mode = "SS
-00014a70: 4222 0a20 2020 2020 2020 2020 2020 2020  B".             
-00014a80: 2020 2023 2073 656c 662e 6d6f 6465 2e73     # self.mode.s
-00014a90: 6574 5465 7874 2822 5353 4222 290a 2020  etText("SSB").  
-00014aa0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00014ab0: 6c66 2e73 656e 742e 7365 7454 6578 7428  lf.sent.setText(
-00014ac0: 2235 3922 290a 2020 2020 2020 2020 2020  "59").          
-00014ad0: 2020 2020 2020 7365 6c66 2e72 6563 6569        self.recei
-00014ae0: 7665 2e73 6574 5465 7874 2822 3539 2229  ve.setText("59")
-00014af0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014b00: 2073 656c 662e 7265 6164 5f63 775f 6d61   self.read_cw_ma
-00014b10: 6372 6f73 2829 0a20 2020 2020 2020 2020  cros().         
-00014b20: 2020 2072 6574 7572 6e0a 2020 2020 2020     return.      
-00014b30: 2020 6966 206d 6f64 6520 3d3d 2022 5254    if mode == "RT
-00014b40: 5459 223a 0a20 2020 2020 2020 2020 2020  TY":.           
-00014b50: 2069 6620 7365 6c66 2e63 7572 7265 6e74   if self.current
-00014b60: 5f6d 6f64 6520 213d 2022 5254 5459 223a  _mode != "RTTY":
-00014b70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014b80: 2073 656c 662e 6375 7272 656e 745f 6d6f   self.current_mo
-00014b90: 6465 203d 2022 5254 5459 220a 2020 2020  de = "RTTY".    
-00014ba0: 2020 2020 2020 2020 2020 2020 2320 7365              # se
-00014bb0: 6c66 2e6d 6f64 652e 7365 7454 6578 7428  lf.mode.setText(
-00014bc0: 2252 5454 5922 290a 2020 2020 2020 2020  "RTTY").        
-00014bd0: 2020 2020 2020 2020 7365 6c66 2e73 656e          self.sen
-00014be0: 742e 7365 7454 6578 7428 2235 3922 290a  t.setText("59").
-00014bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014c00: 7365 6c66 2e72 6563 6569 7665 2e73 6574  self.receive.set
-00014c10: 5465 7874 2822 3539 2229 0a0a 2020 2020  Text("59")..    
-00014c20: 6465 6620 6765 745f 6f70 6f6e 2873 656c  def get_opon(sel
-00014c30: 6629 3a0a 2020 2020 2020 2020 2222 2243  f):.        """C
-00014c40: 7472 6c2b 4f20 6f72 204f 504f 4e20 6469  trl+O or OPON di
-00014c50: 616c 6f67 2222 220a 2020 2020 2020 2020  alog""".        
-00014c60: 7365 6c66 2e6f 706f 6e5f 6469 616c 6f67  self.opon_dialog
-00014c70: 203d 204f 704f 6e28 574f 524b 494e 475f   = OpOn(WORKING_
-00014c80: 5041 5448 290a 2020 2020 2020 2020 7365  PATH).        se
-00014c90: 6c66 2e6f 706f 6e5f 6469 616c 6f67 2e61  lf.opon_dialog.a
-00014ca0: 6363 6570 7465 642e 636f 6e6e 6563 7428  ccepted.connect(
-00014cb0: 7365 6c66 2e6e 6577 5f6f 7029 0a20 2020  self.new_op).   
-00014cc0: 2020 2020 2073 656c 662e 6f70 6f6e 5f64       self.opon_d
-00014cd0: 6961 6c6f 672e 6f70 656e 2829 0a0a 2020  ialog.open()..  
-00014ce0: 2020 6465 6620 6e65 775f 6f70 2873 656c    def new_op(sel
-00014cf0: 6629 3a0a 2020 2020 2020 2020 2222 2253  f):.        """S
-00014d00: 6176 6520 6e65 7720 4f50 2222 220a 2020  ave new OP""".  
-00014d10: 2020 2020 2020 6966 2073 656c 662e 6f70        if self.op
-00014d20: 6f6e 5f64 6961 6c6f 672e 4e65 774f 7065  on_dialog.NewOpe
-00014d30: 7261 746f 722e 7465 7874 2829 3a0a 2020  rator.text():.  
-00014d40: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-00014d50: 7572 7265 6e74 5f6f 7020 3d20 7365 6c66  urrent_op = self
-00014d60: 2e6f 706f 6e5f 6469 616c 6f67 2e4e 6577  .opon_dialog.New
-00014d70: 4f70 6572 6174 6f72 2e74 6578 7428 292e  Operator.text().
-00014d80: 7570 7065 7228 290a 2020 2020 2020 2020  upper().        
-00014d90: 7365 6c66 2e6f 706f 6e5f 6469 616c 6f67  self.opon_dialog
-00014da0: 2e63 6c6f 7365 2829 0a20 2020 2020 2020  .close().       
-00014db0: 206c 6f67 6765 722e 6465 6275 6728 224e   logger.debug("N
-00014dc0: 6577 204f 703a 2025 7322 2c20 7365 6c66  ew Op: %s", self
-00014dd0: 2e63 7572 7265 6e74 5f6f 7029 0a20 2020  .current_op).   
-00014de0: 2020 2020 2073 656c 662e 6d61 6b65 5f6f       self.make_o
-00014df0: 705f 6469 7228 290a 0a20 2020 2064 6566  p_dir()..    def
-00014e00: 206d 616b 655f 6f70 5f64 6972 2873 656c   make_op_dir(sel
-00014e10: 6629 3a0a 2020 2020 2020 2020 2222 2243  f):.        """C
-00014e20: 7265 6174 6520 4f50 2064 6972 6563 746f  reate OP directo
-00014e30: 7279 2069 6620 6974 2064 6f65 7320 6e6f  ry if it does no
-00014e40: 7420 6578 6973 742e 2222 220a 2020 2020  t exist.""".    
-00014e50: 2020 2020 6966 2073 656c 662e 6375 7272      if self.curr
-00014e60: 656e 745f 6f70 3a0a 2020 2020 2020 2020  ent_op:.        
-00014e70: 2020 2020 6f70 5f70 6174 6820 3d20 5061      op_path = Pa
-00014e80: 7468 2844 4154 415f 5041 5448 2920 2f20  th(DATA_PATH) / 
-00014e90: 7365 6c66 2e63 7572 7265 6e74 5f6f 700a  self.current_op.
-00014ea0: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
-00014eb0: 6572 2e64 6562 7567 2822 6f70 5f70 6174  er.debug("op_pat
-00014ec0: 683a 2025 7322 2c20 7374 7228 6f70 5f70  h: %s", str(op_p
-00014ed0: 6174 6829 290a 2020 2020 2020 2020 2020  ath)).          
-00014ee0: 2020 6966 206f 705f 7061 7468 2e69 735f    if op_path.is_
-00014ef0: 6469 7228 2920 6973 2046 616c 7365 3a0a  dir() is False:.
-00014f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014f10: 6c6f 6767 6572 2e64 6562 7567 2822 4372  logger.debug("Cr
-00014f20: 6561 7469 6e67 204f 7020 4469 7265 6374  eating Op Direct
-00014f30: 6f72 793a 2025 7322 2c20 7374 7228 6f70  ory: %s", str(op
-00014f40: 5f70 6174 6829 290a 2020 2020 2020 2020  _path)).        
-00014f50: 2020 2020 2020 2020 6f73 2e6d 6b64 6972          os.mkdir
-00014f60: 2873 7472 286f 705f 7061 7468 2929 0a20  (str(op_path)). 
-00014f70: 2020 2020 2020 2020 2020 2069 6620 6f70             if op
-00014f80: 5f70 6174 682e 6973 5f64 6972 2829 3a0a  _path.is_dir():.
-00014f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014fa0: 736f 7572 6365 5f70 6174 6820 3d20 5061  source_path = Pa
-00014fb0: 7468 2857 4f52 4b49 4e47 5f50 4154 4829  th(WORKING_PATH)
-00014fc0: 202f 2022 6461 7461 2220 2f20 2270 686f   / "data" / "pho
-00014fd0: 6e65 7469 6373 220a 2020 2020 2020 2020  netics".        
-00014fe0: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
-00014ff0: 6562 7567 2822 736f 7572 6365 5f70 6174  ebug("source_pat
-00015000: 683a 2025 7322 2c20 7374 7228 736f 7572  h: %s", str(sour
-00015010: 6365 5f70 6174 6829 290a 2020 2020 2020  ce_path)).      
-00015020: 2020 2020 2020 2020 2020 666f 7220 6368            for ch
-00015030: 696c 6420 696e 2073 6f75 7263 655f 7061  ild in source_pa
-00015040: 7468 2e69 7465 7264 6972 2829 3a0a 2020  th.iterdir():.  
-00015050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015060: 2020 6465 7374 696e 6174 696f 6e5f 6669    destination_fi
-00015070: 6c65 203d 206f 705f 7061 7468 202f 2063  le = op_path / c
-00015080: 6869 6c64 2e6e 616d 650a 2020 2020 2020  hild.name.      
-00015090: 2020 2020 2020 2020 2020 2020 2020 6966                if
-000150a0: 2064 6573 7469 6e61 7469 6f6e 5f66 696c   destination_fil
-000150b0: 652e 6973 5f66 696c 6528 2920 6973 2046  e.is_file() is F
-000150c0: 616c 7365 3a0a 2020 2020 2020 2020 2020  alse:.          
-000150d0: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
-000150e0: 6767 6572 2e64 6562 7567 2822 4465 7374  gger.debug("Dest
-000150f0: 696e 6174 696f 6e3a 2025 7322 2c20 7374  ination: %s", st
-00015100: 7228 6465 7374 696e 6174 696f 6e5f 6669  r(destination_fi
-00015110: 6c65 2929 0a20 2020 2020 2020 2020 2020  le)).           
-00015120: 2020 2020 2020 2020 2020 2020 2064 6573               des
-00015130: 7469 6e61 7469 6f6e 5f66 696c 652e 7772  tination_file.wr
-00015140: 6974 655f 6279 7465 7328 6368 696c 642e  ite_bytes(child.
-00015150: 7265 6164 5f62 7974 6573 2829 290a 0a20  read_bytes()).. 
-00015160: 2020 2064 6566 2070 6f6c 6c5f 7261 6469     def poll_radi
-00015170: 6f28 7365 6c66 293a 0a20 2020 2020 2020  o(self):.       
-00015180: 2022 2222 7374 7562 2222 220a 2020 2020   """stub""".    
-00015190: 2020 2020 6966 2073 656c 662e 7269 675f      if self.rig_
-000151a0: 636f 6e74 726f 6c3a 0a20 2020 2020 2020  control:.       
-000151b0: 2020 2020 2069 6620 7365 6c66 2e72 6967       if self.rig
-000151c0: 5f63 6f6e 7472 6f6c 2e6f 6e6c 696e 6520  _control.online 
-000151d0: 6973 2046 616c 7365 3a0a 2020 2020 2020  is False:.      
-000151e0: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
-000151f0: 6967 5f63 6f6e 7472 6f6c 2e72 6569 6e69  ig_control.reini
-00015200: 7428 290a 2020 2020 2020 2020 2020 2020  t().            
-00015210: 6966 2073 656c 662e 7269 675f 636f 6e74  if self.rig_cont
-00015220: 726f 6c2e 6f6e 6c69 6e65 3a0a 2020 2020  rol.online:.    
-00015230: 2020 2020 2020 2020 2020 2020 696e 666f              info
-00015240: 5f64 6972 7479 203d 2046 616c 7365 0a20  _dirty = False. 
-00015250: 2020 2020 2020 2020 2020 2020 2020 2076                 v
-00015260: 666f 203d 2073 656c 662e 7269 675f 636f  fo = self.rig_co
-00015270: 6e74 726f 6c2e 6765 745f 7666 6f28 290a  ntrol.get_vfo().
-00015280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015290: 6d6f 6465 203d 2073 656c 662e 7269 675f  mode = self.rig_
-000152a0: 636f 6e74 726f 6c2e 6765 745f 6d6f 6465  control.get_mode
-000152b0: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
-000152c0: 2020 2062 7720 3d20 7365 6c66 2e72 6967     bw = self.rig
-000152d0: 5f63 6f6e 7472 6f6c 2e67 6574 5f62 7728  _control.get_bw(
-000152e0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-000152f0: 2020 2320 7365 6c66 2e72 6164 696f 5f73    # self.radio_s
-00015300: 7461 7465 5b22 7074 7422 5d20 3d20 7365  tate["ptt"] = se
-00015310: 6c66 2e72 6967 5f63 6f6e 7472 6f6c 2e67  lf.rig_control.g
-00015320: 6574 5f70 7474 2829 0a0a 2020 2020 2020  et_ptt()..      
-00015330: 2020 2020 2020 2020 2020 6966 206d 6f64            if mod
-00015340: 6520 3d3d 2022 4357 223a 0a20 2020 2020  e == "CW":.     
-00015350: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00015360: 656c 662e 7365 746d 6f64 6528 6d6f 6465  elf.setmode(mode
-00015370: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00015380: 2020 6966 206d 6f64 6520 3d3d 2022 4c53    if mode == "LS
-00015390: 4222 206f 7220 6d6f 6465 203d 3d20 2255  B" or mode == "U
-000153a0: 5342 223a 0a20 2020 2020 2020 2020 2020  SB":.           
-000153b0: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
-000153c0: 746d 6f64 6528 2253 5342 2229 0a20 2020  tmode("SSB").   
-000153d0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-000153e0: 6d6f 6465 203d 3d20 2252 5454 5922 3a0a  mode == "RTTY":.
+000130e0: 2020 225c 7456 464f 2063 7572 736f 7220    "\tVFO cursor 
+000130f0: 696e 2074 6865 2062 616e 646d 6170 2077  in the bandmap w
+00013100: 696e 646f 7720 2843 4154 2052 6571 7569  indow (CAT Requi
+00013110: 7265 6429 2e5c 6e22 0a20 2020 2020 2020  red).\n".       
+00013120: 2020 2020 2020 2020 2020 2020 2022 5b54               "[T
+00013130: 4142 5d5c 744d 6f76 6520 6375 7273 6f72  AB]\tMove cursor
+00013140: 2074 6f20 7468 6520 7269 6768 7420 6f6e   to the right on
+00013150: 6520 6669 656c 642e 5c6e 220a 2020 2020  e field.\n".    
+00013160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013170: 225b 5368 6966 742d 5461 625d 5c74 4d6f  "[Shift-Tab]\tMo
+00013180: 7665 2063 7572 736f 7220 6c65 6674 204f  ve cursor left O
+00013190: 6e65 2066 6965 6c64 2e5c 6e22 0a20 2020  ne field.\n".   
+000131a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000131b0: 2022 5b53 5041 4345 5d5c 7457 6865 6e20   "[SPACE]\tWhen 
+000131c0: 696e 2074 6865 2063 616c 6c73 6967 6e20  in the callsign 
+000131d0: 6669 656c 642c 2077 696c 6c20 6d6f 7665  field, will move
+000131e0: 2074 6865 2069 6e70 7574 2074 6f20 7468   the input to th
+000131f0: 655c 6e22 0a20 2020 2020 2020 2020 2020  e\n".           
+00013200: 2020 2020 2020 2020 2022 5c74 6669 7273           "\tfirs
+00013210: 7420 6669 656c 6420 6e65 6564 6564 2066  t field needed f
+00013220: 6f72 2074 6865 2065 7863 6861 6e67 652e  or the exchange.
+00013230: 5c6e 220a 2020 2020 2020 2020 2020 2020  \n".            
+00013240: 2020 2020 2020 2020 225b 456e 7465 725d          "[Enter]
+00013250: 5c74 5375 626d 6974 7320 7468 6520 6669  \tSubmits the fi
+00013260: 656c 6473 2074 6f20 7468 6520 6c6f 672e  elds to the log.
+00013270: 5c6e 220a 2020 2020 2020 2020 2020 2020  \n".            
+00013280: 2020 2020 2020 2020 225b 4631 2d46 3132          "[F1-F12
+00013290: 5d5c 7453 656e 6420 2843 5720 6f72 2056  ]\tSend (CW or V
+000132a0: 6f69 6365 2920 6d61 6372 6f73 2e5c 6e22  oice) macros.\n"
+000132b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000132c0: 2020 2020 2022 5b43 5452 4c2d 535d 5c74       "[CTRL-S]\t
+000132d0: 5370 6f74 2043 616c 6c73 6967 6e20 746f  Spot Callsign to
+000132e0: 2074 6865 2063 6c75 7374 6572 2e5c 6e22   the cluster.\n"
+000132f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013300: 2020 2020 2022 5b43 5452 4c2d 475d 5c74       "[CTRL-G]\t
+00013310: 5475 6e65 2074 6f20 6120 7370 6f74 206d  Tune to a spot m
+00013320: 6174 6368 696e 6720 7061 7274 6961 6c20  atching partial 
+00013330: 7465 7874 2069 6e20 7468 6520 6361 6c6c  text in the call
+00013340: 7369 676e 5c6e 220a 2020 2020 2020 2020  sign\n".        
+00013350: 2020 2020 2020 2020 2020 2020 225c 7465              "\te
+00013360: 6e74 7279 2066 6965 6c64 2028 4341 5420  ntry field (CAT 
+00013370: 5265 7175 6972 6564 292e 5c6e 220a 2020  Required).\n".  
+00013380: 2020 2020 2020 2020 2020 2020 2020 290a                ).
+00013390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000133a0: 7365 6c66 2e63 6c65 6172 696e 7075 7473  self.clearinputs
+000133b0: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
+000133c0: 2020 2072 6574 7572 6e0a 2020 2020 2020     return.      
+000133d0: 2020 2020 2020 6966 2073 656c 662e 6973        if self.is
+000133e0: 5f66 6c6f 6174 6162 6c65 2873 7472 6970  _floatable(strip
+000133f0: 7065 645f 7465 7874 293a 0a20 2020 2020  ped_text):.     
+00013400: 2020 2020 2020 2020 2020 2076 666f 203d             vfo =
+00013410: 2066 6c6f 6174 2873 7472 6970 7065 645f   float(stripped_
+00013420: 7465 7874 290a 2020 2020 2020 2020 2020  text).          
+00013430: 2020 2020 2020 7666 6f20 3d20 696e 7428        vfo = int(
+00013440: 7666 6f20 2a20 3130 3030 290a 2020 2020  vfo * 1000).    
+00013450: 2020 2020 2020 2020 2020 2020 6261 6e64              band
+00013460: 203d 2067 6574 6261 6e64 2873 7472 2876   = getband(str(v
+00013470: 666f 2929 0a20 2020 2020 2020 2020 2020  fo)).           
+00013480: 2020 2020 2073 656c 662e 7365 745f 6261       self.set_ba
+00013490: 6e64 5f69 6e64 6963 6174 6f72 2862 616e  nd_indicator(ban
+000134a0: 6429 0a20 2020 2020 2020 2020 2020 2020  d).             
+000134b0: 2020 2023 2073 656c 662e 636f 6e74 6163     # self.contac
+000134c0: 745b 2242 616e 6422 5d20 3d20 6765 745f  t["Band"] = get_
+000134d0: 6c6f 6767 6564 5f62 616e 6428 7374 7228  logged_band(str(
+000134e0: 7365 6c66 2e72 6164 696f 5f73 7461 7465  self.radio_state
+000134f0: 2e67 6574 2822 7666 6f61 222c 2030 2e30  .get("vfoa", 0.0
+00013500: 2929 290a 2020 2020 2020 2020 2020 2020  ))).            
+00013510: 2020 2020 7365 6c66 2e72 6164 696f 5f73      self.radio_s
+00013520: 7461 7465 5b22 7666 6f61 225d 203d 2076  tate["vfoa"] = v
+00013530: 666f 0a20 2020 2020 2020 2020 2020 2020  fo.             
+00013540: 2020 2073 656c 662e 7365 745f 7769 6e64     self.set_wind
+00013550: 6f77 5f74 6974 6c65 2829 0a20 2020 2020  ow_title().     
+00013560: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00013570: 636c 6561 7269 6e70 7574 7328 290a 2020  clearinputs().  
+00013580: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00013590: 2073 656c 662e 7269 675f 636f 6e74 726f   self.rig_contro
+000135a0: 6c3a 0a20 2020 2020 2020 2020 2020 2020  l:.             
+000135b0: 2020 2020 2020 2073 656c 662e 7269 675f         self.rig_
+000135c0: 636f 6e74 726f 6c2e 7365 745f 7666 6f28  control.set_vfo(
+000135d0: 7666 6f29 0a20 2020 2020 2020 2020 2020  vfo).           
+000135e0: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
+000135f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013600: 636d 6420 3d20 7b7d 0a20 2020 2020 2020  cmd = {}.       
+00013610: 2020 2020 2020 2020 2063 6d64 5b22 636d           cmd["cm
+00013620: 6422 5d20 3d20 2252 4144 494f 5f53 5441  d"] = "RADIO_STA
+00013630: 5445 220a 2020 2020 2020 2020 2020 2020  TE".            
+00013640: 2020 2020 636d 645b 2273 7461 7469 6f6e      cmd["station
+00013650: 225d 203d 2070 6c61 7466 6f72 6d2e 6e6f  "] = platform.no
+00013660: 6465 2829 0a20 2020 2020 2020 2020 2020  de().           
+00013670: 2020 2020 2063 6d64 5b22 6261 6e64 225d       cmd["band"]
+00013680: 203d 2062 616e 640a 2020 2020 2020 2020   = band.        
+00013690: 2020 2020 2020 2020 636d 645b 2276 666f          cmd["vfo
+000136a0: 6122 5d20 3d20 7666 6f0a 2020 2020 2020  a"] = vfo.      
+000136b0: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
+000136c0: 756c 7469 6361 7374 5f69 6e74 6572 6661  ulticast_interfa
+000136d0: 6365 2e73 656e 645f 6173 5f6a 736f 6e28  ce.send_as_json(
+000136e0: 636d 6429 0a20 2020 2020 2020 2020 2020  cmd).           
+000136f0: 2020 2020 2072 6574 7572 6e0a 0a20 2020       return..   
+00013700: 2020 2020 2020 2020 2073 656c 662e 6368           self.ch
+00013710: 6563 6b5f 6361 6c6c 7369 676e 2873 7472  eck_callsign(str
+00013720: 6970 7065 645f 7465 7874 290a 2020 2020  ipped_text).    
+00013730: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00013740: 6368 6563 6b5f 6475 7065 2873 7472 6970  check_dupe(strip
+00013750: 7065 645f 7465 7874 293a 0a20 2020 2020  ped_text):.     
+00013760: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00013770: 6475 7065 5f69 6e64 6963 6174 6f72 2e73  dupe_indicator.s
+00013780: 686f 7728 290a 2020 2020 2020 2020 2020  how().          
+00013790: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+000137a0: 2020 2020 2020 2020 7365 6c66 2e64 7570          self.dup
+000137b0: 655f 696e 6469 6361 746f 722e 6869 6465  e_indicator.hide
+000137c0: 2829 0a20 2020 2020 2020 2020 2020 205f  ().            _
+000137d0: 7468 6574 6872 6561 6420 3d20 7468 7265  thethread = thre
+000137e0: 6164 696e 672e 5468 7265 6164 280a 2020  ading.Thread(.  
+000137f0: 2020 2020 2020 2020 2020 2020 2020 7461                ta
+00013800: 7267 6574 3d73 656c 662e 6368 6563 6b5f  rget=self.check_
+00013810: 6361 6c6c 7369 676e 322c 0a20 2020 2020  callsign2,.     
+00013820: 2020 2020 2020 2020 2020 2061 7267 733d             args=
+00013830: 2874 6578 742c 292c 0a20 2020 2020 2020  (text,),.       
+00013840: 2020 2020 2020 2020 2064 6165 6d6f 6e3d           daemon=
+00013850: 5472 7565 2c0a 2020 2020 2020 2020 2020  True,.          
+00013860: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+00013870: 5f74 6865 7468 7265 6164 2e73 7461 7274  _thethread.start
+00013880: 2829 0a20 2020 2020 2020 2020 2020 2073  ().            s
+00013890: 656c 662e 6e65 7874 5f66 6965 6c64 2e73  elf.next_field.s
+000138a0: 6574 466f 6375 7328 290a 2020 2020 2020  etFocus().      
+000138b0: 2020 2020 2020 7265 7475 726e 0a20 2020        return.   
+000138c0: 2020 2020 2063 6d64 203d 207b 7d0a 2020       cmd = {}.  
+000138d0: 2020 2020 2020 636d 645b 2263 6d64 225d        cmd["cmd"]
+000138e0: 203d 2022 4341 4c4c 4348 414e 4745 4422   = "CALLCHANGED"
+000138f0: 0a20 2020 2020 2020 2063 6d64 5b22 7374  .        cmd["st
+00013900: 6174 696f 6e22 5d20 3d20 706c 6174 666f  ation"] = platfo
+00013910: 726d 2e6e 6f64 6528 290a 2020 2020 2020  rm.node().      
+00013920: 2020 636d 645b 2263 616c 6c22 5d20 3d20    cmd["call"] = 
+00013930: 7374 7269 7070 6564 5f74 6578 740a 2020  stripped_text.  
+00013940: 2020 2020 2020 7365 6c66 2e6d 756c 7469        self.multi
+00013950: 6361 7374 5f69 6e74 6572 6661 6365 2e73  cast_interface.s
+00013960: 656e 645f 6173 5f6a 736f 6e28 636d 6429  end_as_json(cmd)
+00013970: 0a20 2020 2020 2020 2073 656c 662e 6368  .        self.ch
+00013980: 6563 6b5f 6361 6c6c 7369 676e 2873 7472  eck_callsign(str
+00013990: 6970 7065 645f 7465 7874 290a 0a20 2020  ipped_text)..   
+000139a0: 2064 6566 2063 6865 636b 5f63 616c 6c73   def check_calls
+000139b0: 6967 6e28 7365 6c66 2c20 6361 6c6c 7369  ign(self, callsi
+000139c0: 676e 293a 0a20 2020 2020 2020 2022 2222  gn):.        """
+000139d0: 4368 6563 6b20 6361 6c6c 2061 7320 656e  Check call as en
+000139e0: 7465 7265 6422 2222 0a20 2020 2020 2020  tered""".       
+000139f0: 2072 6573 756c 7420 3d20 7365 6c66 2e63   result = self.c
+00013a00: 7479 5f6c 6f6f 6b75 7028 6361 6c6c 7369  ty_lookup(callsi
+00013a10: 676e 290a 2020 2020 2020 2020 6465 6275  gn).        debu
+00013a20: 675f 7265 7375 6c74 203d 2066 227b 7265  g_result = f"{re
+00013a30: 7375 6c74 7d22 0a20 2020 2020 2020 206c  sult}".        l
+00013a40: 6f67 6765 722e 6465 6275 6728 2225 7322  ogger.debug("%s"
+00013a50: 2c20 6465 6275 675f 7265 7375 6c74 290a  , debug_result).
+00013a60: 2020 2020 2020 2020 6966 2072 6573 756c          if resul
+00013a70: 743a 0a20 2020 2020 2020 2020 2020 2066  t:.            f
+00013a80: 6f72 2061 2069 6e20 7265 7375 6c74 2e69  or a in result.i
+00013a90: 7465 6d73 2829 3a0a 2020 2020 2020 2020  tems():.        
+00013aa0: 2020 2020 2020 2020 656e 7469 7479 203d          entity =
+00013ab0: 2061 5b31 5d2e 6765 7428 2265 6e74 6974   a[1].get("entit
+00013ac0: 7922 2c20 2222 290a 2020 2020 2020 2020  y", "").        
+00013ad0: 2020 2020 2020 2020 6371 203d 2061 5b31          cq = a[1
+00013ae0: 5d2e 6765 7428 2263 7122 2c20 2222 290a  ].get("cq", "").
+00013af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013b00: 6974 7520 3d20 615b 315d 2e67 6574 2822  itu = a[1].get("
+00013b10: 6974 7522 2c20 2222 290a 2020 2020 2020  itu", "").      
+00013b20: 2020 2020 2020 2020 2020 636f 6e74 696e            contin
+00013b30: 656e 7420 3d20 615b 315d 2e67 6574 2822  ent = a[1].get("
+00013b40: 636f 6e74 696e 656e 7422 290a 2020 2020  continent").    
+00013b50: 2020 2020 2020 2020 2020 2020 6c61 7420              lat 
+00013b60: 3d20 666c 6f61 7428 615b 315d 2e67 6574  = float(a[1].get
+00013b70: 2822 6c61 7422 2c20 2230 2e30 2229 290a  ("lat", "0.0")).
+00013b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013b90: 6c6f 6e20 3d20 666c 6f61 7428 615b 315d  lon = float(a[1]
+00013ba0: 2e67 6574 2822 6c6f 6e67 222c 2022 302e  .get("long", "0.
+00013bb0: 3022 2929 0a20 2020 2020 2020 2020 2020  0")).           
+00013bc0: 2020 2020 206c 6f6e 203d 206c 6f6e 202a       lon = lon *
+00013bd0: 202d 3120 2023 2063 7479 2e64 6174 2066   -1  # cty.dat f
+00013be0: 696c 6520 696e 7665 7274 7320 6c6f 6e67  ile inverts long
+00013bf0: 6974 7564 6573 0a20 2020 2020 2020 2020  itudes.         
+00013c00: 2020 2020 2020 2070 7269 6d61 7279 5f70         primary_p
+00013c10: 6678 203d 2061 5b31 5d2e 6765 7428 2270  fx = a[1].get("p
+00013c20: 7269 6d61 7279 5f70 6678 222c 2022 2229  rimary_pfx", "")
+00013c30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013c40: 2068 6561 6469 6e67 203d 2062 6561 7269   heading = beari
+00013c50: 6e67 5f77 6974 685f 6c61 746c 6f6e 2873  ng_with_latlon(s
+00013c60: 656c 662e 7374 6174 696f 6e2e 6765 7428  elf.station.get(
+00013c70: 2247 7269 6453 7175 6172 6522 292c 206c  "GridSquare"), l
+00013c80: 6174 2c20 6c6f 6e29 0a20 2020 2020 2020  at, lon).       
+00013c90: 2020 2020 2020 2020 206b 696c 6f6d 6574           kilomet
+00013ca0: 6572 7320 3d20 6469 7374 616e 6365 5f77  ers = distance_w
+00013cb0: 6974 685f 6c61 746c 6f6e 280a 2020 2020  ith_latlon(.    
+00013cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013cd0: 7365 6c66 2e73 7461 7469 6f6e 2e67 6574  self.station.get
+00013ce0: 2822 4772 6964 5371 7561 7265 2229 2c20  ("GridSquare"), 
+00013cf0: 6c61 742c 206c 6f6e 0a20 2020 2020 2020  lat, lon.       
+00013d00: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+00013d10: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00013d20: 6865 6164 696e 675f 6469 7374 616e 6365  heading_distance
+00013d30: 2e73 6574 5465 7874 280a 2020 2020 2020  .setText(.      
+00013d40: 2020 2020 2020 2020 2020 2020 2020 6622                f"
+00013d50: 5265 6769 6f6e 616c 2048 6467 207b 6865  Regional Hdg {he
+00013d60: 6164 696e 677d c2b0 204c 5020 7b72 6563  ading}.. LP {rec
+00013d70: 6970 726f 636f 6c28 6865 6164 696e 6729  iprocol(heading)
+00013d80: 7dc2 b020 2f20 220a 2020 2020 2020 2020  }.. / ".        
+00013d90: 2020 2020 2020 2020 2020 2020 6622 6469              f"di
+00013da0: 7374 616e 6365 207b 696e 7428 6b69 6c6f  stance {int(kilo
+00013db0: 6d65 7465 7273 2a30 2e36 3231 3337 3129  meters*0.621371)
+00013dc0: 7d6d 6920 7b6b 696c 6f6d 6574 6572 737d  }mi {kilometers}
+00013dd0: 6b6d 220a 2020 2020 2020 2020 2020 2020  km".            
+00013de0: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+00013df0: 2020 2020 2020 7365 6c66 2e63 6f6e 7461        self.conta
+00013e00: 6374 5b22 436f 756e 7472 7950 7265 6669  ct["CountryPrefi
+00013e10: 7822 5d20 3d20 7072 696d 6172 795f 7066  x"] = primary_pf
+00013e20: 780a 2020 2020 2020 2020 2020 2020 2020  x.              
+00013e30: 2020 7365 6c66 2e63 6f6e 7461 6374 5b22    self.contact["
+00013e40: 5a4e 225d 203d 2069 6e74 2863 7129 0a20  ZN"] = int(cq). 
+00013e50: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00013e60: 656c 662e 636f 6e74 6163 745b 2243 6f6e  elf.contact["Con
+00013e70: 7469 6e65 6e74 225d 203d 2063 6f6e 7469  tinent"] = conti
+00013e80: 6e65 6e74 0a20 2020 2020 2020 2020 2020  nent.           
+00013e90: 2020 2020 2073 656c 662e 6478 5f65 6e74       self.dx_ent
+00013ea0: 6974 792e 7365 7454 6578 7428 0a20 2020  ity.setText(.   
+00013eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013ec0: 2066 227b 7072 696d 6172 795f 7066 787d   f"{primary_pfx}
+00013ed0: 3a20 7b63 6f6e 7469 6e65 6e74 7d2f 7b65  : {continent}/{e
+00013ee0: 6e74 6974 797d 2063 713a 7b63 717d 2069  ntity} cq:{cq} i
+00013ef0: 7475 3a7b 6974 757d 220a 2020 2020 2020  tu:{itu}".      
+00013f00: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+00013f10: 2020 2020 2020 2020 2020 2020 6966 206c              if l
+00013f20: 656e 2863 616c 6c73 6967 6e29 203e 2032  en(callsign) > 2
+00013f30: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00013f40: 2020 2020 2020 6966 2073 656c 662e 636f        if self.co
+00013f50: 6e74 6573 743a 0a20 2020 2020 2020 2020  ntest:.         
+00013f60: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00013f70: 656c 662e 636f 6e74 6573 742e 7072 6566  elf.contest.pref
+00013f80: 696c 6c28 7365 6c66 290a 0a20 2020 2064  ill(self)..    d
+00013f90: 6566 2063 6865 636b 5f63 616c 6c73 6967  ef check_callsig
+00013fa0: 6e32 2873 656c 662c 2063 616c 6c73 6967  n2(self, callsig
+00013fb0: 6e29 3a0a 2020 2020 2020 2020 2222 2243  n):.        """C
+00013fc0: 6865 636b 2063 616c 6c20 6f6e 6365 2065  heck call once e
+00013fd0: 6e74 6572 6564 2222 220a 2020 2020 2020  ntered""".      
+00013fe0: 2020 6361 6c6c 7369 676e 203d 2063 616c    callsign = cal
+00013ff0: 6c73 6967 6e2e 7374 7269 7028 290a 2020  lsign.strip().  
+00014000: 2020 2020 2020 6465 6275 675f 6c6f 6f6b        debug_look
+00014010: 7570 203d 2066 227b 7365 6c66 2e6c 6f6f  up = f"{self.loo
+00014020: 6b5f 7570 7d22 0a20 2020 2020 2020 206c  k_up}".        l
+00014030: 6f67 6765 722e 6465 6275 6728 2225 732c  ogger.debug("%s,
+00014040: 2025 7322 2c20 6361 6c6c 7369 676e 2c20   %s", callsign, 
+00014050: 6465 6275 675f 6c6f 6f6b 7570 290a 2020  debug_lookup).  
+00014060: 2020 2020 2020 6966 2068 6173 6174 7472        if hasattr
+00014070: 2873 656c 662e 6c6f 6f6b 5f75 702c 2022  (self.look_up, "
+00014080: 7365 7373 696f 6e22 293a 0a20 2020 2020  session"):.     
+00014090: 2020 2020 2020 2069 6620 7365 6c66 2e6c         if self.l
+000140a0: 6f6f 6b5f 7570 2e73 6573 7369 6f6e 3a0a  ook_up.session:.
+000140b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000140c0: 7265 7370 6f6e 7365 203d 2073 656c 662e  response = self.
+000140d0: 6c6f 6f6b 5f75 702e 6c6f 6f6b 7570 2863  look_up.lookup(c
+000140e0: 616c 6c73 6967 6e29 0a20 2020 2020 2020  allsign).       
+000140f0: 2020 2020 2020 2020 2064 6562 7567 5f72           debug_r
+00014100: 6573 706f 6e73 6520 3d20 6622 7b72 6573  esponse = f"{res
+00014110: 706f 6e73 657d 220a 2020 2020 2020 2020  ponse}".        
+00014120: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
+00014130: 6562 7567 2822 5468 6520 5265 7370 6f6e  ebug("The Respon
+00014140: 7365 3a20 2573 5c6e 222c 2064 6562 7567  se: %s\n", debug
+00014150: 5f72 6573 706f 6e73 6529 0a20 2020 2020  _response).     
+00014160: 2020 2020 2020 2020 2020 2069 6620 7265             if re
+00014170: 7370 6f6e 7365 3a0a 2020 2020 2020 2020  sponse:.        
+00014180: 2020 2020 2020 2020 2020 2020 7468 6569              thei
+00014190: 7267 7269 6420 3d20 7265 7370 6f6e 7365  rgrid = response
+000141a0: 2e67 6574 2822 6772 6964 2229 0a20 2020  .get("grid").   
+000141b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000141c0: 2073 656c 662e 636f 6e74 6163 745b 2247   self.contact["G
+000141d0: 7269 6453 7175 6172 6522 5d20 3d20 7468  ridSquare"] = th
+000141e0: 6569 7267 7269 640a 2020 2020 2020 2020  eirgrid.        
+000141f0: 2020 2020 2020 2020 2020 2020 5f74 6865              _the
+00014200: 6972 636f 756e 7472 7920 3d20 7265 7370  ircountry = resp
+00014210: 6f6e 7365 2e67 6574 2822 636f 756e 7472  onse.get("countr
+00014220: 7922 290a 2020 2020 2020 2020 2020 2020  y").            
+00014230: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00014240: 7374 6174 696f 6e2e 6765 7428 2247 7269  station.get("Gri
+00014250: 6453 7175 6172 6522 2c20 2222 293a 0a20  dSquare", ""):. 
+00014260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014270: 2020 2020 2020 2068 6561 6469 6e67 203d         heading =
+00014280: 2062 6561 7269 6e67 2873 656c 662e 7374   bearing(self.st
+00014290: 6174 696f 6e2e 6765 7428 2247 7269 6453  ation.get("GridS
+000142a0: 7175 6172 6522 2c20 2222 292c 2074 6865  quare", ""), the
+000142b0: 6972 6772 6964 290a 2020 2020 2020 2020  irgrid).        
+000142c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000142d0: 6b69 6c6f 6d65 7465 7273 203d 2064 6973  kilometers = dis
+000142e0: 7461 6e63 6528 7365 6c66 2e73 7461 7469  tance(self.stati
+000142f0: 6f6e 2e67 6574 2822 4772 6964 5371 7561  on.get("GridSqua
+00014300: 7265 2229 2c20 7468 6569 7267 7269 6429  re"), theirgrid)
+00014310: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014320: 2020 2020 2020 2020 2073 656c 662e 6865           self.he
+00014330: 6164 696e 675f 6469 7374 616e 6365 2e73  ading_distance.s
+00014340: 6574 5465 7874 280a 2020 2020 2020 2020  etText(.        
+00014350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014360: 2020 2020 6622 7b74 6865 6972 6772 6964      f"{theirgrid
+00014370: 7d20 4864 6720 7b68 6561 6469 6e67 7dc2  } Hdg {heading}.
+00014380: b020 4c50 207b 7265 6369 7072 6f63 6f6c  . LP {reciprocol
+00014390: 2868 6561 6469 6e67 297d c2b0 202f 2022  (heading)}.. / "
+000143a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000143b0: 2020 2020 2020 2020 2020 2020 2066 2264               f"d
+000143c0: 6973 7461 6e63 6520 7b69 6e74 286b 696c  istance {int(kil
+000143d0: 6f6d 6574 6572 732a 302e 3632 3133 3731  ometers*0.621371
+000143e0: 297d 6d69 207b 6b69 6c6f 6d65 7465 7273  )}mi {kilometers
+000143f0: 7d6b 6d22 0a20 2020 2020 2020 2020 2020  }km".           
+00014400: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
+00014410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014420: 2020 2023 2073 656c 662e 6478 5f65 6e74     # self.dx_ent
+00014430: 6974 792e 7365 7454 6578 7428 6622 7b74  ity.setText(f"{t
+00014440: 6865 6972 636f 756e 7472 797d 2229 0a20  heircountry}"). 
+00014450: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+00014460: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00014470: 2020 2020 2020 2023 2073 656c 662e 6865         # self.he
+00014480: 6164 696e 675f 6469 7374 616e 6365 2e73  ading_distance.s
+00014490: 6574 5465 7874 2822 4c6f 6f6b 7570 2066  etText("Lookup f
+000144a0: 6169 6c65 642e 2229 0a0a 2020 2020 6465  ailed.")..    de
+000144b0: 6620 6368 6563 6b5f 6475 7065 2873 656c  f check_dupe(sel
+000144c0: 662c 2063 616c 6c3a 2073 7472 2920 2d3e  f, call: str) ->
+000144d0: 2062 6f6f 6c3a 0a20 2020 2020 2020 2022   bool:.        "
+000144e0: 2222 4368 6563 6b73 2069 6620 6120 6361  ""Checks if a ca
+000144f0: 6c6c 7369 676e 2069 7320 6120 6475 7065  llsign is a dupe
+00014500: 206f 6e20 6375 7272 656e 7420 6261 6e64   on current band
+00014510: 2f6d 6f64 652e 2222 220a 2020 2020 2020  /mode.""".      
+00014520: 2020 6966 2073 656c 662e 636f 6e74 6573    if self.contes
+00014530: 7420 6973 204e 6f6e 653a 0a20 2020 2020  t is None:.     
+00014540: 2020 2020 2020 2073 656c 662e 7368 6f77         self.show
+00014550: 5f6d 6573 7361 6765 5f62 6f78 2822 596f  _message_box("Yo
+00014560: 7520 6861 7665 206e 6f20 636f 6e74 6573  u have no contes
+00014570: 7420 6c6f 6164 6564 2e22 290a 2020 2020  t loaded.").    
+00014580: 2020 2020 2020 2020 7265 7475 726e 2046          return F
+00014590: 616c 7365 0a20 2020 2020 2020 2073 656c  alse.        sel
+000145a0: 662e 636f 6e74 6573 742e 7072 6564 7570  f.contest.predup
+000145b0: 6528 7365 6c66 290a 2020 2020 2020 2020  e(self).        
+000145c0: 6261 6e64 203d 2066 6c6f 6174 2867 6574  band = float(get
+000145d0: 5f6c 6f67 6765 645f 6261 6e64 2873 7472  _logged_band(str
+000145e0: 2873 656c 662e 7261 6469 6f5f 7374 6174  (self.radio_stat
+000145f0: 652e 6765 7428 2276 666f 6122 2c20 302e  e.get("vfoa", 0.
+00014600: 3029 2929 290a 2020 2020 2020 2020 6d6f  0)))).        mo
+00014610: 6465 203d 2073 656c 662e 7261 6469 6f5f  de = self.radio_
+00014620: 7374 6174 652e 6765 7428 226d 6f64 6522  state.get("mode"
+00014630: 2c20 2222 290a 2020 2020 2020 2020 6465  , "").        de
+00014640: 6275 676c 696e 6520 3d20 280a 2020 2020  bugline = (.    
+00014650: 2020 2020 2020 2020 6622 4361 6c6c 3a20          f"Call: 
+00014660: 7b63 616c 6c7d 2042 616e 643a 207b 6261  {call} Band: {ba
+00014670: 6e64 7d20 4d6f 6465 3a20 7b6d 6f64 657d  nd} Mode: {mode}
+00014680: 2044 7570 6574 7970 653a 207b 7365 6c66   Dupetype: {self
+00014690: 2e63 6f6e 7465 7374 2e64 7570 655f 7479  .contest.dupe_ty
+000146a0: 7065 7d22 0a20 2020 2020 2020 2029 0a20  pe}".        ). 
+000146b0: 2020 2020 2020 206c 6f67 6765 722e 6465         logger.de
+000146c0: 6275 6728 2225 7322 2c20 6465 6275 676c  bug("%s", debugl
+000146d0: 696e 6529 0a20 2020 2020 2020 2069 6620  ine).        if 
+000146e0: 7365 6c66 2e63 6f6e 7465 7374 2e64 7570  self.contest.dup
+000146f0: 655f 7479 7065 203d 3d20 313a 0a20 2020  e_type == 1:.   
+00014700: 2020 2020 2020 2020 2072 6573 756c 7420           result 
+00014710: 3d20 7365 6c66 2e64 6174 6162 6173 652e  = self.database.
+00014720: 6368 6563 6b5f 6475 7065 2863 616c 6c29  check_dupe(call)
+00014730: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00014740: 2e63 6f6e 7465 7374 2e64 7570 655f 7479  .contest.dupe_ty
+00014750: 7065 203d 3d20 323a 0a20 2020 2020 2020  pe == 2:.       
+00014760: 2020 2020 2072 6573 756c 7420 3d20 7365       result = se
+00014770: 6c66 2e64 6174 6162 6173 652e 6368 6563  lf.database.chec
+00014780: 6b5f 6475 7065 5f6f 6e5f 6261 6e64 2863  k_dupe_on_band(c
+00014790: 616c 6c2c 2062 616e 6429 0a20 2020 2020  all, band).     
+000147a0: 2020 2069 6620 7365 6c66 2e63 6f6e 7465     if self.conte
+000147b0: 7374 2e64 7570 655f 7479 7065 203d 3d20  st.dupe_type == 
+000147c0: 333a 0a20 2020 2020 2020 2020 2020 2072  3:.            r
+000147d0: 6573 756c 7420 3d20 7365 6c66 2e64 6174  esult = self.dat
+000147e0: 6162 6173 652e 6368 6563 6b5f 6475 7065  abase.check_dupe
+000147f0: 5f6f 6e5f 6261 6e64 5f6d 6f64 6528 6361  _on_band_mode(ca
+00014800: 6c6c 2c20 6261 6e64 2c20 6d6f 6465 290a  ll, band, mode).
+00014810: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00014820: 636f 6e74 6573 742e 6475 7065 5f74 7970  contest.dupe_typ
+00014830: 6520 3d3d 2034 3a0a 2020 2020 2020 2020  e == 4:.        
+00014840: 2020 2020 7265 7375 6c74 203d 207b 2269      result = {"i
+00014850: 7364 7570 6522 3a20 4661 6c73 657d 0a20  sdupe": False}. 
+00014860: 2020 2020 2020 2064 6562 7567 6c69 6e65         debugline
+00014870: 203d 2066 227b 7265 7375 6c74 7d22 0a20   = f"{result}". 
+00014880: 2020 2020 2020 206c 6f67 6765 722e 6465         logger.de
+00014890: 6275 6728 2225 7322 2c20 6465 6275 676c  bug("%s", debugl
+000148a0: 696e 6529 0a20 2020 2020 2020 2072 6574  ine).        ret
+000148b0: 7572 6e20 7265 7375 6c74 2e67 6574 2822  urn result.get("
+000148c0: 6973 6475 7065 222c 2046 616c 7365 290a  isdupe", False).
+000148d0: 0a20 2020 2064 6566 2073 6574 6d6f 6465  .    def setmode
+000148e0: 2873 656c 662c 206d 6f64 653a 2073 7472  (self, mode: str
+000148f0: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+00014900: 2020 2022 2222 7374 7562 2066 6f72 2077     """stub for w
+00014910: 6865 6e20 7468 6520 6d6f 6465 2063 6861  hen the mode cha
+00014920: 6e67 6573 2e22 2222 0a20 2020 2020 2020  nges.""".       
+00014930: 2069 6620 6d6f 6465 203d 3d20 2243 5722   if mode == "CW"
+00014940: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+00014950: 2073 656c 662e 6375 7272 656e 745f 6d6f   self.current_mo
+00014960: 6465 2021 3d20 2243 5722 3a0a 2020 2020  de != "CW":.    
+00014970: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00014980: 2e63 7572 7265 6e74 5f6d 6f64 6520 3d20  .current_mode = 
+00014990: 2243 5722 0a20 2020 2020 2020 2020 2020  "CW".           
+000149a0: 2020 2020 2023 2073 656c 662e 6d6f 6465       # self.mode
+000149b0: 2e73 6574 5465 7874 2822 4357 2229 0a20  .setText("CW"). 
+000149c0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000149d0: 656c 662e 7365 6e74 2e73 6574 5465 7874  elf.sent.setText
+000149e0: 2822 3539 3922 290a 2020 2020 2020 2020  ("599").        
+000149f0: 2020 2020 2020 2020 7365 6c66 2e72 6563          self.rec
+00014a00: 6569 7665 2e73 6574 5465 7874 2822 3539  eive.setText("59
+00014a10: 3922 290a 2020 2020 2020 2020 2020 2020  9").            
+00014a20: 2020 2020 7365 6c66 2e72 6561 645f 6377      self.read_cw
+00014a30: 5f6d 6163 726f 7328 290a 2020 2020 2020  _macros().      
+00014a40: 2020 2020 2020 7265 7475 726e 0a20 2020        return.   
+00014a50: 2020 2020 2069 6620 6d6f 6465 203d 3d20       if mode == 
+00014a60: 2253 5342 223a 0a20 2020 2020 2020 2020  "SSB":.         
+00014a70: 2020 2069 6620 7365 6c66 2e63 7572 7265     if self.curre
+00014a80: 6e74 5f6d 6f64 6520 213d 2022 5353 4222  nt_mode != "SSB"
+00014a90: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00014aa0: 2020 7365 6c66 2e63 7572 7265 6e74 5f6d    self.current_m
+00014ab0: 6f64 6520 3d20 2253 5342 220a 2020 2020  ode = "SSB".    
+00014ac0: 2020 2020 2020 2020 2020 2020 2320 7365              # se
+00014ad0: 6c66 2e6d 6f64 652e 7365 7454 6578 7428  lf.mode.setText(
+00014ae0: 2253 5342 2229 0a20 2020 2020 2020 2020  "SSB").         
+00014af0: 2020 2020 2020 2073 656c 662e 7365 6e74         self.sent
+00014b00: 2e73 6574 5465 7874 2822 3539 2229 0a20  .setText("59"). 
+00014b10: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00014b20: 656c 662e 7265 6365 6976 652e 7365 7454  elf.receive.setT
+00014b30: 6578 7428 2235 3922 290a 2020 2020 2020  ext("59").      
+00014b40: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
+00014b50: 6561 645f 6377 5f6d 6163 726f 7328 290a  ead_cw_macros().
+00014b60: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00014b70: 726e 0a20 2020 2020 2020 2069 6620 6d6f  rn.        if mo
+00014b80: 6465 203d 3d20 2252 5454 5922 3a0a 2020  de == "RTTY":.  
+00014b90: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+00014ba0: 662e 6375 7272 656e 745f 6d6f 6465 2021  f.current_mode !
+00014bb0: 3d20 2252 5454 5922 3a0a 2020 2020 2020  = "RTTY":.      
+00014bc0: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+00014bd0: 7572 7265 6e74 5f6d 6f64 6520 3d20 2252  urrent_mode = "R
+00014be0: 5454 5922 0a20 2020 2020 2020 2020 2020  TTY".           
+00014bf0: 2020 2020 2023 2073 656c 662e 6d6f 6465       # self.mode
+00014c00: 2e73 6574 5465 7874 2822 5254 5459 2229  .setText("RTTY")
+00014c10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014c20: 2073 656c 662e 7365 6e74 2e73 6574 5465   self.sent.setTe
+00014c30: 7874 2822 3539 2229 0a20 2020 2020 2020  xt("59").       
+00014c40: 2020 2020 2020 2020 2073 656c 662e 7265           self.re
+00014c50: 6365 6976 652e 7365 7454 6578 7428 2235  ceive.setText("5
+00014c60: 3922 290a 0a20 2020 2064 6566 2067 6574  9")..    def get
+00014c70: 5f6f 706f 6e28 7365 6c66 293a 0a20 2020  _opon(self):.   
+00014c80: 2020 2020 2022 2222 4374 726c 2b4f 206f       """Ctrl+O o
+00014c90: 7220 4f50 4f4e 2064 6961 6c6f 6722 2222  r OPON dialog"""
+00014ca0: 0a20 2020 2020 2020 2073 656c 662e 6f70  .        self.op
+00014cb0: 6f6e 5f64 6961 6c6f 6720 3d20 4f70 4f6e  on_dialog = OpOn
+00014cc0: 2857 4f52 4b49 4e47 5f50 4154 4829 0a20  (WORKING_PATH). 
+00014cd0: 2020 2020 2020 2073 656c 662e 6f70 6f6e         self.opon
+00014ce0: 5f64 6961 6c6f 672e 6163 6365 7074 6564  _dialog.accepted
+00014cf0: 2e63 6f6e 6e65 6374 2873 656c 662e 6e65  .connect(self.ne
+00014d00: 775f 6f70 290a 2020 2020 2020 2020 7365  w_op).        se
+00014d10: 6c66 2e6f 706f 6e5f 6469 616c 6f67 2e6f  lf.opon_dialog.o
+00014d20: 7065 6e28 290a 0a20 2020 2064 6566 206e  pen()..    def n
+00014d30: 6577 5f6f 7028 7365 6c66 293a 0a20 2020  ew_op(self):.   
+00014d40: 2020 2020 2022 2222 5361 7665 206e 6577       """Save new
+00014d50: 204f 5022 2222 0a20 2020 2020 2020 2069   OP""".        i
+00014d60: 6620 7365 6c66 2e6f 706f 6e5f 6469 616c  f self.opon_dial
+00014d70: 6f67 2e4e 6577 4f70 6572 6174 6f72 2e74  og.NewOperator.t
+00014d80: 6578 7428 293a 0a20 2020 2020 2020 2020  ext():.         
+00014d90: 2020 2073 656c 662e 6375 7272 656e 745f     self.current_
+00014da0: 6f70 203d 2073 656c 662e 6f70 6f6e 5f64  op = self.opon_d
+00014db0: 6961 6c6f 672e 4e65 774f 7065 7261 746f  ialog.NewOperato
+00014dc0: 722e 7465 7874 2829 2e75 7070 6572 2829  r.text().upper()
+00014dd0: 0a20 2020 2020 2020 2073 656c 662e 6f70  .        self.op
+00014de0: 6f6e 5f64 6961 6c6f 672e 636c 6f73 6528  on_dialog.close(
+00014df0: 290a 2020 2020 2020 2020 6c6f 6767 6572  ).        logger
+00014e00: 2e64 6562 7567 2822 4e65 7720 4f70 3a20  .debug("New Op: 
+00014e10: 2573 222c 2073 656c 662e 6375 7272 656e  %s", self.curren
+00014e20: 745f 6f70 290a 2020 2020 2020 2020 7365  t_op).        se
+00014e30: 6c66 2e6d 616b 655f 6f70 5f64 6972 2829  lf.make_op_dir()
+00014e40: 0a0a 2020 2020 6465 6620 6d61 6b65 5f6f  ..    def make_o
+00014e50: 705f 6469 7228 7365 6c66 293a 0a20 2020  p_dir(self):.   
+00014e60: 2020 2020 2022 2222 4372 6561 7465 204f       """Create O
+00014e70: 5020 6469 7265 6374 6f72 7920 6966 2069  P directory if i
+00014e80: 7420 646f 6573 206e 6f74 2065 7869 7374  t does not exist
+00014e90: 2e22 2222 0a20 2020 2020 2020 2069 6620  .""".        if 
+00014ea0: 7365 6c66 2e63 7572 7265 6e74 5f6f 703a  self.current_op:
+00014eb0: 0a20 2020 2020 2020 2020 2020 206f 705f  .            op_
+00014ec0: 7061 7468 203d 2050 6174 6828 4441 5441  path = Path(DATA
+00014ed0: 5f50 4154 4829 202f 2073 656c 662e 6375  _PATH) / self.cu
+00014ee0: 7272 656e 745f 6f70 0a20 2020 2020 2020  rrent_op.       
+00014ef0: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
+00014f00: 6728 226f 705f 7061 7468 3a20 2573 222c  g("op_path: %s",
+00014f10: 2073 7472 286f 705f 7061 7468 2929 0a20   str(op_path)). 
+00014f20: 2020 2020 2020 2020 2020 2069 6620 6f70             if op
+00014f30: 5f70 6174 682e 6973 5f64 6972 2829 2069  _path.is_dir() i
+00014f40: 7320 4661 6c73 653a 0a20 2020 2020 2020  s False:.       
+00014f50: 2020 2020 2020 2020 206c 6f67 6765 722e           logger.
+00014f60: 6465 6275 6728 2243 7265 6174 696e 6720  debug("Creating 
+00014f70: 4f70 2044 6972 6563 746f 7279 3a20 2573  Op Directory: %s
+00014f80: 222c 2073 7472 286f 705f 7061 7468 2929  ", str(op_path))
+00014f90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014fa0: 206f 732e 6d6b 6469 7228 7374 7228 6f70   os.mkdir(str(op
+00014fb0: 5f70 6174 6829 290a 2020 2020 2020 2020  _path)).        
+00014fc0: 2020 2020 6966 206f 705f 7061 7468 2e69      if op_path.i
+00014fd0: 735f 6469 7228 293a 0a20 2020 2020 2020  s_dir():.       
+00014fe0: 2020 2020 2020 2020 2073 6f75 7263 655f           source_
+00014ff0: 7061 7468 203d 2050 6174 6828 574f 524b  path = Path(WORK
+00015000: 494e 475f 5041 5448 2920 2f20 2264 6174  ING_PATH) / "dat
+00015010: 6122 202f 2022 7068 6f6e 6574 6963 7322  a" / "phonetics"
+00015020: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015030: 206c 6f67 6765 722e 6465 6275 6728 2273   logger.debug("s
+00015040: 6f75 7263 655f 7061 7468 3a20 2573 222c  ource_path: %s",
+00015050: 2073 7472 2873 6f75 7263 655f 7061 7468   str(source_path
+00015060: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
+00015070: 2020 2066 6f72 2063 6869 6c64 2069 6e20     for child in 
+00015080: 736f 7572 6365 5f70 6174 682e 6974 6572  source_path.iter
+00015090: 6469 7228 293a 0a20 2020 2020 2020 2020  dir():.         
+000150a0: 2020 2020 2020 2020 2020 2064 6573 7469             desti
+000150b0: 6e61 7469 6f6e 5f66 696c 6520 3d20 6f70  nation_file = op
+000150c0: 5f70 6174 6820 2f20 6368 696c 642e 6e61  _path / child.na
+000150d0: 6d65 0a20 2020 2020 2020 2020 2020 2020  me.             
+000150e0: 2020 2020 2020 2069 6620 6465 7374 696e         if destin
+000150f0: 6174 696f 6e5f 6669 6c65 2e69 735f 6669  ation_file.is_fi
+00015100: 6c65 2829 2069 7320 4661 6c73 653a 0a20  le() is False:. 
+00015110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015120: 2020 2020 2020 206c 6f67 6765 722e 6465         logger.de
+00015130: 6275 6728 2244 6573 7469 6e61 7469 6f6e  bug("Destination
+00015140: 3a20 2573 222c 2073 7472 2864 6573 7469  : %s", str(desti
+00015150: 6e61 7469 6f6e 5f66 696c 6529 290a 2020  nation_file)).  
+00015160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015170: 2020 2020 2020 6465 7374 696e 6174 696f        destinatio
+00015180: 6e5f 6669 6c65 2e77 7269 7465 5f62 7974  n_file.write_byt
+00015190: 6573 2863 6869 6c64 2e72 6561 645f 6279  es(child.read_by
+000151a0: 7465 7328 2929 0a0a 2020 2020 6465 6620  tes())..    def 
+000151b0: 706f 6c6c 5f72 6164 696f 2873 656c 6629  poll_radio(self)
+000151c0: 3a0a 2020 2020 2020 2020 2222 2273 7475  :.        """stu
+000151d0: 6222 2222 0a20 2020 2020 2020 2069 6620  b""".        if 
+000151e0: 7365 6c66 2e72 6967 5f63 6f6e 7472 6f6c  self.rig_control
+000151f0: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+00015200: 2073 656c 662e 7269 675f 636f 6e74 726f   self.rig_contro
+00015210: 6c2e 6f6e 6c69 6e65 2069 7320 4661 6c73  l.online is Fals
+00015220: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00015230: 2020 2073 656c 662e 7269 675f 636f 6e74     self.rig_cont
+00015240: 726f 6c2e 7265 696e 6974 2829 0a20 2020  rol.reinit().   
+00015250: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+00015260: 2e72 6967 5f63 6f6e 7472 6f6c 2e6f 6e6c  .rig_control.onl
+00015270: 696e 653a 0a20 2020 2020 2020 2020 2020  ine:.           
+00015280: 2020 2020 2069 6e66 6f5f 6469 7274 7920       info_dirty 
+00015290: 3d20 4661 6c73 650a 2020 2020 2020 2020  = False.        
+000152a0: 2020 2020 2020 2020 7666 6f20 3d20 7365          vfo = se
+000152b0: 6c66 2e72 6967 5f63 6f6e 7472 6f6c 2e67  lf.rig_control.g
+000152c0: 6574 5f76 666f 2829 0a20 2020 2020 2020  et_vfo().       
+000152d0: 2020 2020 2020 2020 206d 6f64 6520 3d20           mode = 
+000152e0: 7365 6c66 2e72 6967 5f63 6f6e 7472 6f6c  self.rig_control
+000152f0: 2e67 6574 5f6d 6f64 6528 290a 2020 2020  .get_mode().    
+00015300: 2020 2020 2020 2020 2020 2020 6277 203d              bw =
+00015310: 2073 656c 662e 7269 675f 636f 6e74 726f   self.rig_contro
+00015320: 6c2e 6765 745f 6277 2829 0a20 2020 2020  l.get_bw().     
+00015330: 2020 2020 2020 2020 2020 2023 2073 656c             # sel
+00015340: 662e 7261 6469 6f5f 7374 6174 655b 2270  f.radio_state["p
+00015350: 7474 225d 203d 2073 656c 662e 7269 675f  tt"] = self.rig_
+00015360: 636f 6e74 726f 6c2e 6765 745f 7074 7428  control.get_ptt(
+00015370: 290a 0a20 2020 2020 2020 2020 2020 2020  )..             
+00015380: 2020 2069 6620 6d6f 6465 203d 3d20 2243     if mode == "C
+00015390: 5722 3a0a 2020 2020 2020 2020 2020 2020  W":.            
+000153a0: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
+000153b0: 6d6f 6465 286d 6f64 6529 0a20 2020 2020  mode(mode).     
+000153c0: 2020 2020 2020 2020 2020 2069 6620 6d6f             if mo
+000153d0: 6465 203d 3d20 224c 5342 2220 6f72 206d  de == "LSB" or m
+000153e0: 6f64 6520 3d3d 2022 5553 4222 3a0a 2020  ode == "USB":.  
 000153f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015400: 2020 2020 7365 6c66 2e73 6574 6d6f 6465      self.setmode
-00015410: 2822 5254 5459 2229 0a0a 2020 2020 2020  ("RTTY")..      
-00015420: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-00015430: 662e 7261 6469 6f5f 7374 6174 652e 6765  f.radio_state.ge
-00015440: 7428 2276 666f 6122 2920 213d 2076 666f  t("vfoa") != vfo
-00015450: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00015460: 2020 2020 2020 696e 666f 5f64 6972 7479        info_dirty
-00015470: 203d 2054 7275 650a 2020 2020 2020 2020   = True.        
-00015480: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00015490: 2e72 6164 696f 5f73 7461 7465 5b22 7666  .radio_state["vf
-000154a0: 6f61 225d 203d 2076 666f 0a20 2020 2020  oa"] = vfo.     
-000154b0: 2020 2020 2020 2020 2020 2062 616e 6420             band 
-000154c0: 3d20 6765 7462 616e 6428 7374 7228 7666  = getband(str(vf
-000154d0: 6f29 290a 2020 2020 2020 2020 2020 2020  o)).            
-000154e0: 2020 2020 7365 6c66 2e72 6164 696f 5f73      self.radio_s
-000154f0: 7461 7465 5b22 6261 6e64 225d 203d 2062  tate["band"] = b
-00015500: 616e 640a 2020 2020 2020 2020 2020 2020  and.            
-00015510: 2020 2020 7365 6c66 2e63 6f6e 7461 6374      self.contact
-00015520: 5b22 4261 6e64 225d 203d 2067 6574 5f6c  ["Band"] = get_l
-00015530: 6f67 6765 645f 6261 6e64 2873 7472 2876  ogged_band(str(v
-00015540: 666f 2929 0a20 2020 2020 2020 2020 2020  fo)).           
-00015550: 2020 2020 2073 656c 662e 7365 745f 6261       self.set_ba
-00015560: 6e64 5f69 6e64 6963 6174 6f72 2862 616e  nd_indicator(ban
-00015570: 6429 0a0a 2020 2020 2020 2020 2020 2020  d)..            
-00015580: 2020 2020 6966 2073 656c 662e 7261 6469      if self.radi
-00015590: 6f5f 7374 6174 652e 6765 7428 226d 6f64  o_state.get("mod
-000155a0: 6522 2920 213d 206d 6f64 653a 0a20 2020  e") != mode:.   
-000155b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000155c0: 2069 6e66 6f5f 6469 7274 7920 3d20 5472   info_dirty = Tr
-000155d0: 7565 0a20 2020 2020 2020 2020 2020 2020  ue.             
-000155e0: 2020 2020 2020 2073 656c 662e 7261 6469         self.radi
-000155f0: 6f5f 7374 6174 655b 226d 6f64 6522 5d20  o_state["mode"] 
-00015600: 3d20 6d6f 6465 0a0a 2020 2020 2020 2020  = mode..        
-00015610: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00015620: 7261 6469 6f5f 7374 6174 652e 6765 7428  radio_state.get(
-00015630: 2262 7722 2920 213d 2062 773a 0a20 2020  "bw") != bw:.   
-00015640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015650: 2069 6e66 6f5f 6469 7274 7920 3d20 5472   info_dirty = Tr
-00015660: 7565 0a20 2020 2020 2020 2020 2020 2020  ue.             
-00015670: 2020 2020 2020 2073 656c 662e 7261 6469         self.radi
-00015680: 6f5f 7374 6174 655b 2262 7722 5d20 3d20  o_state["bw"] = 
-00015690: 6277 0a0a 2020 2020 2020 2020 2020 2020  bw..            
-000156a0: 2020 2020 6966 2064 6174 6574 696d 652e      if datetime.
-000156b0: 6e6f 7728 2920 3e20 676c 6f62 616c 7328  now() > globals(
-000156c0: 295b 2270 6f6c 6c5f 7469 6d65 225d 206f  )["poll_time"] o
-000156d0: 7220 696e 666f 5f64 6972 7479 3a0a 2020  r info_dirty:.  
-000156e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000156f0: 2020 6c6f 6767 6572 2e64 6562 7567 2822    logger.debug("
-00015700: 5646 4f3a 2025 7320 204d 4f44 453a 2025  VFO: %s  MODE: %
-00015710: 7320 4257 3a20 2573 222c 2076 666f 2c20  s BW: %s", vfo, 
-00015720: 6d6f 6465 2c20 6277 290a 2020 2020 2020  mode, bw).      
-00015730: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00015740: 6c66 2e73 6574 5f77 696e 646f 775f 7469  lf.set_window_ti
-00015750: 746c 6528 290a 2020 2020 2020 2020 2020  tle().          
-00015760: 2020 2020 2020 2020 2020 636d 6420 3d20            cmd = 
-00015770: 7b7d 0a20 2020 2020 2020 2020 2020 2020  {}.             
-00015780: 2020 2020 2020 2063 6d64 5b22 636d 6422         cmd["cmd"
-00015790: 5d20 3d20 2252 4144 494f 5f53 5441 5445  ] = "RADIO_STATE
-000157a0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-000157b0: 2020 2020 2020 636d 645b 2273 7461 7469        cmd["stati
-000157c0: 6f6e 225d 203d 2070 6c61 7466 6f72 6d2e  on"] = platform.
-000157d0: 6e6f 6465 2829 0a20 2020 2020 2020 2020  node().         
-000157e0: 2020 2020 2020 2020 2020 2063 6d64 5b22             cmd["
-000157f0: 6261 6e64 225d 203d 2062 616e 640a 2020  band"] = band.  
-00015800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015810: 2020 636d 645b 2276 666f 6122 5d20 3d20    cmd["vfoa"] = 
-00015820: 7666 6f0a 2020 2020 2020 2020 2020 2020  vfo.            
-00015830: 2020 2020 2020 2020 636d 645b 226d 6f64          cmd["mod
-00015840: 6522 5d20 3d20 6d6f 6465 0a20 2020 2020  e"] = mode.     
-00015850: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00015860: 6d64 5b22 6277 225d 203d 2062 770a 2020  md["bw"] = bw.  
+00015400: 2020 7365 6c66 2e73 6574 6d6f 6465 2822    self.setmode("
+00015410: 5353 4222 290a 2020 2020 2020 2020 2020  SSB").          
+00015420: 2020 2020 2020 6966 206d 6f64 6520 3d3d        if mode ==
+00015430: 2022 5254 5459 223a 0a20 2020 2020 2020   "RTTY":.       
+00015440: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00015450: 662e 7365 746d 6f64 6528 2252 5454 5922  f.setmode("RTTY"
+00015460: 290a 0a20 2020 2020 2020 2020 2020 2020  )..             
+00015470: 2020 2069 6620 7365 6c66 2e72 6164 696f     if self.radio
+00015480: 5f73 7461 7465 2e67 6574 2822 7666 6f61  _state.get("vfoa
+00015490: 2229 2021 3d20 7666 6f3a 0a20 2020 2020  ") != vfo:.     
+000154a0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+000154b0: 6e66 6f5f 6469 7274 7920 3d20 5472 7565  nfo_dirty = True
+000154c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000154d0: 2020 2020 2073 656c 662e 7261 6469 6f5f       self.radio_
+000154e0: 7374 6174 655b 2276 666f 6122 5d20 3d20  state["vfoa"] = 
+000154f0: 7666 6f0a 2020 2020 2020 2020 2020 2020  vfo.            
+00015500: 2020 2020 6261 6e64 203d 2067 6574 6261      band = getba
+00015510: 6e64 2873 7472 2876 666f 2929 0a20 2020  nd(str(vfo)).   
+00015520: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00015530: 662e 7261 6469 6f5f 7374 6174 655b 2262  f.radio_state["b
+00015540: 616e 6422 5d20 3d20 6261 6e64 0a20 2020  and"] = band.   
+00015550: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00015560: 662e 636f 6e74 6163 745b 2242 616e 6422  f.contact["Band"
+00015570: 5d20 3d20 6765 745f 6c6f 6767 6564 5f62  ] = get_logged_b
+00015580: 616e 6428 7374 7228 7666 6f29 290a 2020  and(str(vfo)).  
+00015590: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000155a0: 6c66 2e73 6574 5f62 616e 645f 696e 6469  lf.set_band_indi
+000155b0: 6361 746f 7228 6261 6e64 290a 0a20 2020  cator(band)..   
+000155c0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+000155d0: 7365 6c66 2e72 6164 696f 5f73 7461 7465  self.radio_state
+000155e0: 2e67 6574 2822 6d6f 6465 2229 2021 3d20  .get("mode") != 
+000155f0: 6d6f 6465 3a0a 2020 2020 2020 2020 2020  mode:.          
+00015600: 2020 2020 2020 2020 2020 696e 666f 5f64            info_d
+00015610: 6972 7479 203d 2054 7275 650a 2020 2020  irty = True.    
+00015620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015630: 7365 6c66 2e72 6164 696f 5f73 7461 7465  self.radio_state
+00015640: 5b22 6d6f 6465 225d 203d 206d 6f64 650a  ["mode"] = mode.
+00015650: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015660: 2069 6620 7365 6c66 2e72 6164 696f 5f73   if self.radio_s
+00015670: 7461 7465 2e67 6574 2822 6277 2229 2021  tate.get("bw") !
+00015680: 3d20 6277 3a0a 2020 2020 2020 2020 2020  = bw:.          
+00015690: 2020 2020 2020 2020 2020 696e 666f 5f64            info_d
+000156a0: 6972 7479 203d 2054 7275 650a 2020 2020  irty = True.    
+000156b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000156c0: 7365 6c66 2e72 6164 696f 5f73 7461 7465  self.radio_state
+000156d0: 5b22 6277 225d 203d 2062 770a 0a20 2020  ["bw"] = bw..   
+000156e0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+000156f0: 6461 7465 7469 6d65 2e6e 6f77 2829 203e  datetime.now() >
+00015700: 2067 6c6f 6261 6c73 2829 5b22 706f 6c6c   globals()["poll
+00015710: 5f74 696d 6522 5d20 6f72 2069 6e66 6f5f  _time"] or info_
+00015720: 6469 7274 793a 0a20 2020 2020 2020 2020  dirty:.         
+00015730: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
+00015740: 722e 6465 6275 6728 2256 464f 3a20 2573  r.debug("VFO: %s
+00015750: 2020 4d4f 4445 3a20 2573 2042 573a 2025    MODE: %s BW: %
+00015760: 7322 2c20 7666 6f2c 206d 6f64 652c 2062  s", vfo, mode, b
+00015770: 7729 0a20 2020 2020 2020 2020 2020 2020  w).             
+00015780: 2020 2020 2020 2073 656c 662e 7365 745f         self.set_
+00015790: 7769 6e64 6f77 5f74 6974 6c65 2829 0a20  window_title(). 
+000157a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000157b0: 2020 2063 6d64 203d 207b 7d0a 2020 2020     cmd = {}.    
+000157c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000157d0: 636d 645b 2263 6d64 225d 203d 2022 5241  cmd["cmd"] = "RA
+000157e0: 4449 4f5f 5354 4154 4522 0a20 2020 2020  DIO_STATE".     
+000157f0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00015800: 6d64 5b22 7374 6174 696f 6e22 5d20 3d20  md["station"] = 
+00015810: 706c 6174 666f 726d 2e6e 6f64 6528 290a  platform.node().
+00015820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015830: 2020 2020 636d 645b 2262 616e 6422 5d20      cmd["band"] 
+00015840: 3d20 6261 6e64 0a20 2020 2020 2020 2020  = band.         
+00015850: 2020 2020 2020 2020 2020 2063 6d64 5b22             cmd["
+00015860: 7666 6f61 225d 203d 2076 666f 0a20 2020  vfoa"] = vfo.   
 00015870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015880: 2020 7365 6c66 2e6d 756c 7469 6361 7374    self.multicast
-00015890: 5f69 6e74 6572 6661 6365 2e73 656e 645f  _interface.send_
-000158a0: 6173 5f6a 736f 6e28 636d 6429 0a20 2020  as_json(cmd).   
-000158b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000158c0: 2069 6620 7365 6c66 2e6e 316d 6d3a 0a20   if self.n1mm:. 
-000158d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000158e0: 2020 2020 2020 2069 6620 7365 6c66 2e6e         if self.n
-000158f0: 316d 6d2e 7365 6e64 5f72 6164 696f 5f70  1mm.send_radio_p
-00015900: 6163 6b65 7473 3a0a 2020 2020 2020 2020  ackets:.        
-00015910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015920: 2020 2020 7365 6c66 2e6e 316d 6d2e 7261      self.n1mm.ra
-00015930: 6469 6f5f 696e 666f 5b22 4672 6571 225d  dio_info["Freq"]
-00015940: 203d 2076 666f 5b3a 2d31 5d0a 2020 2020   = vfo[:-1].    
-00015950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015960: 2020 2020 2020 2020 7365 6c66 2e6e 316d          self.n1m
-00015970: 6d2e 7261 6469 6f5f 696e 666f 5b22 5458  m.radio_info["TX
-00015980: 4672 6571 225d 203d 2076 666f 5b3a 2d31  Freq"] = vfo[:-1
-00015990: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
-000159a0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-000159b0: 6c66 2e6e 316d 6d2e 7261 6469 6f5f 696e  lf.n1mm.radio_in
-000159c0: 666f 5b22 4d6f 6465 225d 203d 206d 6f64  fo["Mode"] = mod
-000159d0: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
-000159e0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-000159f0: 6c66 2e6e 316d 6d2e 7261 6469 6f5f 696e  lf.n1mm.radio_in
-00015a00: 666f 5b22 4f70 4361 6c6c 225d 203d 2073  fo["OpCall"] = s
-00015a10: 656c 662e 6375 7272 656e 745f 6f70 0a20  elf.current_op. 
+00015880: 2063 6d64 5b22 6d6f 6465 225d 203d 206d   cmd["mode"] = m
+00015890: 6f64 650a 2020 2020 2020 2020 2020 2020  ode.            
+000158a0: 2020 2020 2020 2020 636d 645b 2262 7722          cmd["bw"
+000158b0: 5d20 3d20 6277 0a20 2020 2020 2020 2020  ] = bw.         
+000158c0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000158d0: 6d75 6c74 6963 6173 745f 696e 7465 7266  multicast_interf
+000158e0: 6163 652e 7365 6e64 5f61 735f 6a73 6f6e  ace.send_as_json
+000158f0: 2863 6d64 290a 2020 2020 2020 2020 2020  (cmd).          
+00015900: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+00015910: 662e 6e31 6d6d 3a0a 2020 2020 2020 2020  f.n1mm:.        
+00015920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015930: 6966 2073 656c 662e 6e31 6d6d 2e73 656e  if self.n1mm.sen
+00015940: 645f 7261 6469 6f5f 7061 636b 6574 733a  d_radio_packets:
+00015950: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015960: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00015970: 662e 6e31 6d6d 2e72 6164 696f 5f69 6e66  f.n1mm.radio_inf
+00015980: 6f5b 2246 7265 7122 5d20 3d20 7666 6f5b  o["Freq"] = vfo[
+00015990: 3a2d 315d 0a20 2020 2020 2020 2020 2020  :-1].           
+000159a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000159b0: 2073 656c 662e 6e31 6d6d 2e72 6164 696f   self.n1mm.radio
+000159c0: 5f69 6e66 6f5b 2254 5846 7265 7122 5d20  _info["TXFreq"] 
+000159d0: 3d20 7666 6f5b 3a2d 315d 0a20 2020 2020  = vfo[:-1].     
+000159e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000159f0: 2020 2020 2020 2073 656c 662e 6e31 6d6d         self.n1mm
+00015a00: 2e72 6164 696f 5f69 6e66 6f5b 224d 6f64  .radio_info["Mod
+00015a10: 6522 5d20 3d20 6d6f 6465 0a20 2020 2020  e"] = mode.     
 00015a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015a30: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00015a40: 6e31 6d6d 2e72 6164 696f 5f69 6e66 6f5b  n1mm.radio_info[
-00015a50: 2249 7352 756e 6e69 6e67 225d 203d 2073  "IsRunning"] = s
-00015a60: 7472 280a 2020 2020 2020 2020 2020 2020  tr(.            
+00015a30: 2020 2020 2020 2073 656c 662e 6e31 6d6d         self.n1mm
+00015a40: 2e72 6164 696f 5f69 6e66 6f5b 224f 7043  .radio_info["OpC
+00015a50: 616c 6c22 5d20 3d20 7365 6c66 2e63 7572  all"] = self.cur
+00015a60: 7265 6e74 5f6f 700a 2020 2020 2020 2020  rent_op.        
 00015a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015a80: 2020 2020 7365 6c66 2e70 7265 662e 6765      self.pref.ge
-00015a90: 7428 2272 756e 5f73 7461 7465 222c 2046  t("run_state", F
-00015aa0: 616c 7365 290a 2020 2020 2020 2020 2020  alse).          
+00015a80: 2020 2020 7365 6c66 2e6e 316d 6d2e 7261      self.n1mm.ra
+00015a90: 6469 6f5f 696e 666f 5b22 4973 5275 6e6e  dio_info["IsRunn
+00015aa0: 696e 6722 5d20 3d20 7374 7228 0a20 2020  ing"] = str(.   
 00015ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015ac0: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
-00015ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015ae0: 7365 6c66 2e6e 316d 6d2e 7365 6e64 5f72  self.n1mm.send_r
-00015af0: 6164 696f 2829 0a20 2020 2020 2020 2020  adio().         
-00015b00: 2020 2020 2020 2020 2020 2067 6c6f 6261             globa
-00015b10: 6c73 2829 5b22 706f 6c6c 5f74 696d 6522  ls()["poll_time"
-00015b20: 5d20 3d20 6461 7465 7469 6d65 2e6e 6f77  ] = datetime.now
-00015b30: 2829 202b 2064 742e 7469 6d65 6465 6c74  () + dt.timedelt
-00015b40: 6128 7365 636f 6e64 733d 3130 290a 0a20  a(seconds=10).. 
-00015b50: 2020 2064 6566 2065 6469 745f 6377 5f6d     def edit_cw_m
-00015b60: 6163 726f 7328 7365 6c66 2920 2d3e 204e  acros(self) -> N
-00015b70: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
-00015b80: 0a20 2020 2020 2020 2043 616c 6c73 2074  .        Calls t
-00015b90: 6865 2064 6566 6175 6c74 2074 6578 7420  he default text 
-00015ba0: 6564 6974 6f72 2074 6f20 6564 6974 2074  editor to edit t
-00015bb0: 6865 2043 5720 6d61 6372 6f20 6669 6c65  he CW macro file
-00015bc0: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
-00015bd0: 2020 2020 2020 6966 2073 656c 662e 7261        if self.ra
-00015be0: 6469 6f5f 7374 6174 652e 6765 7428 226d  dio_state.get("m
-00015bf0: 6f64 6522 2920 3d3d 2022 4357 223a 0a20  ode") == "CW":. 
-00015c00: 2020 2020 2020 2020 2020 206d 6163 726f             macro
-00015c10: 5f66 696c 6520 3d20 222f 6377 6d61 6372  _file = "/cwmacr
-00015c20: 6f73 2e74 7874 220a 2020 2020 2020 2020  os.txt".        
-00015c30: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00015c40: 2020 6d61 6372 6f5f 6669 6c65 203d 2022    macro_file = "
-00015c50: 2f73 7362 6d61 6372 6f73 2e74 7874 220a  /ssbmacros.txt".
-00015c60: 2020 2020 2020 2020 6966 206e 6f74 2050          if not P
-00015c70: 6174 6828 4441 5441 5f50 4154 4820 2b20  ath(DATA_PATH + 
-00015c80: 6d61 6372 6f5f 6669 6c65 292e 6578 6973  macro_file).exis
-00015c90: 7473 2829 3a0a 2020 2020 2020 2020 2020  ts():.          
-00015ca0: 2020 6c6f 6767 6572 2e64 6562 7567 2822    logger.debug("
-00015cb0: 7265 6164 5f63 775f 6d61 6372 6f73 3a20  read_cw_macros: 
-00015cc0: 636f 7079 696e 6720 6465 6661 756c 7420  copying default 
-00015cd0: 6d61 6372 6f20 6669 6c65 2e22 290a 2020  macro file.").  
-00015ce0: 2020 2020 2020 2020 2020 636f 7079 6669            copyfi
-00015cf0: 6c65 2857 4f52 4b49 4e47 5f50 4154 4820  le(WORKING_PATH 
-00015d00: 2b20 222f 6461 7461 2220 2b20 6d61 6372  + "/data" + macr
-00015d10: 6f5f 6669 6c65 2c20 4441 5441 5f50 4154  o_file, DATA_PAT
-00015d20: 4820 2b20 6d61 6372 6f5f 6669 6c65 290a  H + macro_file).
-00015d30: 2020 2020 2020 2020 6f73 2e73 7973 7465          os.syste
-00015d40: 6d28 6622 7864 672d 6f70 656e 207b 4441  m(f"xdg-open {DA
-00015d50: 5441 5f50 4154 487d 7b6d 6163 726f 5f66  TA_PATH}{macro_f
-00015d60: 696c 657d 2229 0a0a 2020 2020 6465 6620  ile}")..    def 
-00015d70: 7265 6164 5f63 775f 6d61 6372 6f73 2873  read_cw_macros(s
-00015d80: 656c 6629 202d 3e20 4e6f 6e65 3a0a 2020  elf) -> None:.  
-00015d90: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00015da0: 2020 5265 6164 7320 696e 2074 6865 2043    Reads in the C
-00015db0: 5720 6d61 6372 6f73 2c20 6669 7273 7473  W macros, firsts
-00015dc0: 2069 7420 6368 6563 6b73 2074 6f20 7365   it checks to se
-00015dd0: 6520 6966 2074 6865 2066 696c 6520 6578  e if the file ex
-00015de0: 6973 7473 2e20 4966 2069 7420 646f 6573  ists. If it does
-00015df0: 206e 6f74 2c0a 2020 2020 2020 2020 616e   not,.        an
-00015e00: 6420 7468 6973 2068 6173 2062 6565 6e20  d this has been 
-00015e10: 7061 636b 6167 6564 2077 6974 6820 7079  packaged with py
-00015e20: 696e 7374 616c 6c65 7220 6974 2077 696c  installer it wil
-00015e30: 6c20 636f 7079 2074 6865 2064 6566 6175  l copy the defau
-00015e40: 6c74 2066 696c 6520 6672 6f6d 2074 6865  lt file from the
-00015e50: 0a20 2020 2020 2020 2074 656d 7020 6469  .        temp di
-00015e60: 7265 6374 6f72 7920 7468 6973 2069 7320  rectory this is 
-00015e70: 7275 6e6e 696e 6720 6672 6f6d 2e2e 2e20  running from... 
-00015e80: 496e 2074 6865 6f72 792e 0a20 2020 2020  In theory..     
-00015e90: 2020 2022 2222 0a0a 2020 2020 2020 2020     """..        
-00015ea0: 6966 2073 656c 662e 7261 6469 6f5f 7374  if self.radio_st
-00015eb0: 6174 652e 6765 7428 226d 6f64 6522 2920  ate.get("mode") 
-00015ec0: 3d3d 2022 4357 223a 0a20 2020 2020 2020  == "CW":.       
-00015ed0: 2020 2020 206d 6163 726f 5f66 696c 6520       macro_file 
-00015ee0: 3d20 222f 6377 6d61 6372 6f73 2e74 7874  = "/cwmacros.txt
-00015ef0: 220a 2020 2020 2020 2020 656c 7365 3a0a  ".        else:.
-00015f00: 2020 2020 2020 2020 2020 2020 6d61 6372              macr
-00015f10: 6f5f 6669 6c65 203d 2022 2f73 7362 6d61  o_file = "/ssbma
-00015f20: 6372 6f73 2e74 7874 220a 0a20 2020 2020  cros.txt"..     
-00015f30: 2020 2069 6620 6e6f 7420 5061 7468 2844     if not Path(D
-00015f40: 4154 415f 5041 5448 202b 206d 6163 726f  ATA_PATH + macro
-00015f50: 5f66 696c 6529 2e65 7869 7374 7328 293a  _file).exists():
-00015f60: 0a20 2020 2020 2020 2020 2020 206c 6f67  .            log
-00015f70: 6765 722e 6465 6275 6728 2272 6561 645f  ger.debug("read_
-00015f80: 6377 5f6d 6163 726f 733a 2063 6f70 7969  cw_macros: copyi
-00015f90: 6e67 2064 6566 6175 6c74 206d 6163 726f  ng default macro
-00015fa0: 2066 696c 652e 2229 0a20 2020 2020 2020   file.").       
-00015fb0: 2020 2020 2063 6f70 7966 696c 6528 574f       copyfile(WO
-00015fc0: 524b 494e 475f 5041 5448 202b 2022 2f64  RKING_PATH + "/d
-00015fd0: 6174 6122 202b 206d 6163 726f 5f66 696c  ata" + macro_fil
-00015fe0: 652c 2044 4154 415f 5041 5448 202b 206d  e, DATA_PATH + m
-00015ff0: 6163 726f 5f66 696c 6529 0a20 2020 2020  acro_file).     
-00016000: 2020 2077 6974 6820 6f70 656e 2844 4154     with open(DAT
-00016010: 415f 5041 5448 202b 206d 6163 726f 5f66  A_PATH + macro_f
-00016020: 696c 652c 2022 7222 2c20 656e 636f 6469  ile, "r", encodi
-00016030: 6e67 3d22 7574 662d 3822 2920 6173 2066  ng="utf-8") as f
-00016040: 696c 655f 6465 7363 7269 7074 6f72 3a0a  ile_descriptor:.
-00016050: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00016060: 6c69 6e65 2069 6e20 6669 6c65 5f64 6573  line in file_des
-00016070: 6372 6970 746f 723a 0a20 2020 2020 2020  criptor:.       
-00016080: 2020 2020 2020 2020 2074 7279 3a0a 2020           try:.  
-00016090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000160a0: 2020 6d6f 6465 2c20 666b 6579 2c20 6275    mode, fkey, bu
-000160b0: 7474 6f6e 6e61 6d65 2c20 6377 7465 7874  ttonname, cwtext
-000160c0: 203d 206c 696e 652e 7370 6c69 7428 227c   = line.split("|
-000160d0: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
-000160e0: 2020 2020 2020 2069 6620 6d6f 6465 2e73         if mode.s
-000160f0: 7472 6970 2829 2e75 7070 6572 2829 203d  trip().upper() =
-00016100: 3d20 2252 2220 616e 6420 7365 6c66 2e70  = "R" and self.p
-00016110: 7265 662e 6765 7428 2272 756e 5f73 7461  ref.get("run_sta
-00016120: 7465 2229 3a0a 2020 2020 2020 2020 2020  te"):.          
-00016130: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00016140: 6c66 2e66 6b65 7973 5b66 6b65 792e 7374  lf.fkeys[fkey.st
-00016150: 7269 7028 295d 203d 2028 6275 7474 6f6e  rip()] = (button
-00016160: 6e61 6d65 2e73 7472 6970 2829 2c20 6377  name.strip(), cw
-00016170: 7465 7874 2e73 7472 6970 2829 290a 2020  text.strip()).  
-00016180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016190: 2020 6966 206d 6f64 652e 7374 7269 7028    if mode.strip(
-000161a0: 292e 7570 7065 7228 2920 213d 2022 5222  ).upper() != "R"
-000161b0: 2061 6e64 206e 6f74 2073 656c 662e 7072   and not self.pr
-000161c0: 6566 2e67 6574 2822 7275 6e5f 7374 6174  ef.get("run_stat
-000161d0: 6522 293a 0a20 2020 2020 2020 2020 2020  e"):.           
-000161e0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-000161f0: 662e 666b 6579 735b 666b 6579 2e73 7472  f.fkeys[fkey.str
-00016200: 6970 2829 5d20 3d20 2862 7574 746f 6e6e  ip()] = (buttonn
-00016210: 616d 652e 7374 7269 7028 292c 2063 7774  ame.strip(), cwt
-00016220: 6578 742e 7374 7269 7028 2929 0a20 2020  ext.strip()).   
-00016230: 2020 2020 2020 2020 2020 2020 2065 7863               exc
-00016240: 6570 7420 5661 6c75 6545 7272 6f72 2061  ept ValueError a
-00016250: 7320 6572 723a 0a20 2020 2020 2020 2020  s err:.         
-00016260: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
-00016270: 722e 696e 666f 2822 7265 6164 5f63 775f  r.info("read_cw_
-00016280: 6d61 6372 6f73 3a20 2573 222c 2065 7272  macros: %s", err
-00016290: 290a 2020 2020 2020 2020 6b65 7973 203d  ).        keys =
-000162a0: 2073 656c 662e 666b 6579 732e 6b65 7973   self.fkeys.keys
-000162b0: 2829 0a20 2020 2020 2020 2069 6620 2246  ().        if "F
-000162c0: 3122 2069 6e20 6b65 7973 3a0a 2020 2020  1" in keys:.    
-000162d0: 2020 2020 2020 2020 7365 6c66 2e46 312e          self.F1.
-000162e0: 7365 7454 6578 7428 6622 4631 3a20 7b73  setText(f"F1: {s
-000162f0: 656c 662e 666b 6579 735b 2746 3127 5d5b  elf.fkeys['F1'][
-00016300: 305d 7d22 290a 2020 2020 2020 2020 2020  0]}").          
-00016310: 2020 7365 6c66 2e46 312e 7365 7454 6f6f    self.F1.setToo
-00016320: 6c54 6970 2873 656c 662e 666b 6579 735b  lTip(self.fkeys[
-00016330: 2246 3122 5d5b 315d 290a 2020 2020 2020  "F1"][1]).      
-00016340: 2020 6966 2022 4632 2220 696e 206b 6579    if "F2" in key
-00016350: 733a 0a20 2020 2020 2020 2020 2020 2073  s:.            s
-00016360: 656c 662e 4632 2e73 6574 5465 7874 2866  elf.F2.setText(f
-00016370: 2246 323a 207b 7365 6c66 2e66 6b65 7973  "F2: {self.fkeys
-00016380: 5b27 4632 275d 5b30 5d7d 2229 0a20 2020  ['F2'][0]}").   
-00016390: 2020 2020 2020 2020 2073 656c 662e 4632           self.F2
-000163a0: 2e73 6574 546f 6f6c 5469 7028 7365 6c66  .setToolTip(self
-000163b0: 2e66 6b65 7973 5b22 4632 225d 5b31 5d29  .fkeys["F2"][1])
-000163c0: 0a20 2020 2020 2020 2069 6620 2246 3322  .        if "F3"
-000163d0: 2069 6e20 6b65 7973 3a0a 2020 2020 2020   in keys:.      
-000163e0: 2020 2020 2020 7365 6c66 2e46 332e 7365        self.F3.se
-000163f0: 7454 6578 7428 6622 4633 3a20 7b73 656c  tText(f"F3: {sel
-00016400: 662e 666b 6579 735b 2746 3327 5d5b 305d  f.fkeys['F3'][0]
-00016410: 7d22 290a 2020 2020 2020 2020 2020 2020  }").            
-00016420: 7365 6c66 2e46 332e 7365 7454 6f6f 6c54  self.F3.setToolT
-00016430: 6970 2873 656c 662e 666b 6579 735b 2246  ip(self.fkeys["F
-00016440: 3322 5d5b 315d 290a 2020 2020 2020 2020  3"][1]).        
-00016450: 6966 2022 4634 2220 696e 206b 6579 733a  if "F4" in keys:
-00016460: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00016470: 662e 4634 2e73 6574 5465 7874 2866 2246  f.F4.setText(f"F
-00016480: 343a 207b 7365 6c66 2e66 6b65 7973 5b27  4: {self.fkeys['
-00016490: 4634 275d 5b30 5d7d 2229 0a20 2020 2020  F4'][0]}").     
-000164a0: 2020 2020 2020 2073 656c 662e 4634 2e73         self.F4.s
-000164b0: 6574 546f 6f6c 5469 7028 7365 6c66 2e66  etToolTip(self.f
-000164c0: 6b65 7973 5b22 4634 225d 5b31 5d29 0a20  keys["F4"][1]). 
-000164d0: 2020 2020 2020 2069 6620 2246 3522 2069         if "F5" i
-000164e0: 6e20 6b65 7973 3a0a 2020 2020 2020 2020  n keys:.        
-000164f0: 2020 2020 7365 6c66 2e46 352e 7365 7454      self.F5.setT
-00016500: 6578 7428 6622 4635 3a20 7b73 656c 662e  ext(f"F5: {self.
-00016510: 666b 6579 735b 2746 3527 5d5b 305d 7d22  fkeys['F5'][0]}"
-00016520: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-00016530: 6c66 2e46 352e 7365 7454 6f6f 6c54 6970  lf.F5.setToolTip
-00016540: 2873 656c 662e 666b 6579 735b 2246 3522  (self.fkeys["F5"
-00016550: 5d5b 315d 290a 2020 2020 2020 2020 6966  ][1]).        if
-00016560: 2022 4636 2220 696e 206b 6579 733a 0a20   "F6" in keys:. 
-00016570: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00016580: 4636 2e73 6574 5465 7874 2866 2246 363a  F6.setText(f"F6:
-00016590: 207b 7365 6c66 2e66 6b65 7973 5b27 4636   {self.fkeys['F6
-000165a0: 275d 5b30 5d7d 2229 0a20 2020 2020 2020  '][0]}").       
-000165b0: 2020 2020 2073 656c 662e 4636 2e73 6574       self.F6.set
-000165c0: 546f 6f6c 5469 7028 7365 6c66 2e66 6b65  ToolTip(self.fke
-000165d0: 7973 5b22 4636 225d 5b31 5d29 0a20 2020  ys["F6"][1]).   
-000165e0: 2020 2020 2069 6620 2246 3722 2069 6e20       if "F7" in 
-000165f0: 6b65 7973 3a0a 2020 2020 2020 2020 2020  keys:.          
-00016600: 2020 7365 6c66 2e46 372e 7365 7454 6578    self.F7.setTex
-00016610: 7428 6622 4637 3a20 7b73 656c 662e 666b  t(f"F7: {self.fk
-00016620: 6579 735b 2746 3727 5d5b 305d 7d22 290a  eys['F7'][0]}").
-00016630: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00016640: 2e46 372e 7365 7454 6f6f 6c54 6970 2873  .F7.setToolTip(s
-00016650: 656c 662e 666b 6579 735b 2246 3722 5d5b  elf.fkeys["F7"][
-00016660: 315d 290a 2020 2020 2020 2020 6966 2022  1]).        if "
-00016670: 4638 2220 696e 206b 6579 733a 0a20 2020  F8" in keys:.   
-00016680: 2020 2020 2020 2020 2073 656c 662e 4638           self.F8
-00016690: 2e73 6574 5465 7874 2866 2246 383a 207b  .setText(f"F8: {
-000166a0: 7365 6c66 2e66 6b65 7973 5b27 4638 275d  self.fkeys['F8']
-000166b0: 5b30 5d7d 2229 0a20 2020 2020 2020 2020  [0]}").         
-000166c0: 2020 2073 656c 662e 4638 2e73 6574 546f     self.F8.setTo
-000166d0: 6f6c 5469 7028 7365 6c66 2e66 6b65 7973  olTip(self.fkeys
-000166e0: 5b22 4638 225d 5b31 5d29 0a20 2020 2020  ["F8"][1]).     
-000166f0: 2020 2069 6620 2246 3922 2069 6e20 6b65     if "F9" in ke
-00016700: 7973 3a0a 2020 2020 2020 2020 2020 2020  ys:.            
-00016710: 7365 6c66 2e46 392e 7365 7454 6578 7428  self.F9.setText(
-00016720: 6622 4639 3a20 7b73 656c 662e 666b 6579  f"F9: {self.fkey
-00016730: 735b 2746 3927 5d5b 305d 7d22 290a 2020  s['F9'][0]}").  
-00016740: 2020 2020 2020 2020 2020 7365 6c66 2e46            self.F
-00016750: 392e 7365 7454 6f6f 6c54 6970 2873 656c  9.setToolTip(sel
-00016760: 662e 666b 6579 735b 2246 3922 5d5b 315d  f.fkeys["F9"][1]
-00016770: 290a 2020 2020 2020 2020 6966 2022 4631  ).        if "F1
-00016780: 3022 2069 6e20 6b65 7973 3a0a 2020 2020  0" in keys:.    
-00016790: 2020 2020 2020 2020 7365 6c66 2e46 3130          self.F10
-000167a0: 2e73 6574 5465 7874 2866 2246 3130 3a20  .setText(f"F10: 
-000167b0: 7b73 656c 662e 666b 6579 735b 2746 3130  {self.fkeys['F10
-000167c0: 275d 5b30 5d7d 2229 0a20 2020 2020 2020  '][0]}").       
-000167d0: 2020 2020 2073 656c 662e 4631 302e 7365       self.F10.se
-000167e0: 7454 6f6f 6c54 6970 2873 656c 662e 666b  tToolTip(self.fk
-000167f0: 6579 735b 2246 3130 225d 5b31 5d29 0a20  eys["F10"][1]). 
-00016800: 2020 2020 2020 2069 6620 2246 3131 2220         if "F11" 
-00016810: 696e 206b 6579 733a 0a20 2020 2020 2020  in keys:.       
-00016820: 2020 2020 2073 656c 662e 4631 312e 7365       self.F11.se
-00016830: 7454 6578 7428 6622 4631 313a 207b 7365  tText(f"F11: {se
-00016840: 6c66 2e66 6b65 7973 5b27 4631 3127 5d5b  lf.fkeys['F11'][
-00016850: 305d 7d22 290a 2020 2020 2020 2020 2020  0]}").          
-00016860: 2020 7365 6c66 2e46 3131 2e73 6574 546f    self.F11.setTo
-00016870: 6f6c 5469 7028 7365 6c66 2e66 6b65 7973  olTip(self.fkeys
-00016880: 5b22 4631 3122 5d5b 315d 290a 2020 2020  ["F11"][1]).    
-00016890: 2020 2020 6966 2022 4631 3222 2069 6e20      if "F12" in 
-000168a0: 6b65 7973 3a0a 2020 2020 2020 2020 2020  keys:.          
-000168b0: 2020 7365 6c66 2e46 3132 2e73 6574 5465    self.F12.setTe
-000168c0: 7874 2866 2246 3132 3a20 7b73 656c 662e  xt(f"F12: {self.
-000168d0: 666b 6579 735b 2746 3132 275d 5b30 5d7d  fkeys['F12'][0]}
-000168e0: 2229 0a20 2020 2020 2020 2020 2020 2073  ").            s
-000168f0: 656c 662e 4631 322e 7365 7454 6f6f 6c54  elf.F12.setToolT
-00016900: 6970 2873 656c 662e 666b 6579 735b 2246  ip(self.fkeys["F
-00016910: 3132 225d 5b31 5d29 0a0a 2020 2020 6465  12"][1])..    de
-00016920: 6620 6765 6e65 7261 7465 5f61 6469 6628  f generate_adif(
-00016930: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
-00016940: 2222 4765 6e65 7261 7465 2041 4449 4622  ""Generate ADIF"
-00016950: 2222 0a20 2020 2020 2020 206c 6f67 6765  "".        logge
-00016960: 722e 6465 6275 6728 222a 2a2a 2a2a 2a41  r.debug("******A
-00016970: 4449 462a 2a2a 2a2a 2229 0a20 2020 2020  DIF*****").     
-00016980: 2020 2073 656c 662e 636f 6e74 6573 742e     self.contest.
-00016990: 6164 6966 2873 656c 6629 0a0a 2020 2020  adif(self)..    
-000169a0: 6465 6620 6765 6e65 7261 7465 5f63 6162  def generate_cab
-000169b0: 7269 6c6c 6f28 7365 6c66 293a 0a20 2020  rillo(self):.   
-000169c0: 2020 2020 2022 2222 4765 6e65 7261 7465       """Generate
-000169d0: 7320 4361 6272 696c 6c6f 2066 696c 652e  s Cabrillo file.
-000169e0: 204d 6179 6265 2e22 2222 0a20 2020 2020   Maybe.""".     
-000169f0: 2020 2023 2068 7474 7073 3a2f 2f77 7777     # https://www
-00016a00: 2e63 7177 7078 2e63 6f6d 2f63 6162 7269  .cqwpx.com/cabri
-00016a10: 6c6c 6f2e 6874 6d0a 2020 2020 2020 2020  llo.htm.        
-00016a20: 6c6f 6767 6572 2e64 6562 7567 2822 2a2a  logger.debug("**
-00016a30: 2a2a 2a2a 4361 6272 696c 6c6f 2a2a 2a2a  ****Cabrillo****
-00016a40: 2a22 290a 2020 2020 2020 2020 7365 6c66  *").        self
-00016a50: 2e63 6f6e 7465 7374 2e63 6162 7269 6c6c  .contest.cabrill
-00016a60: 6f28 7365 6c66 290a 0a0a 6465 6620 6c6f  o(self)...def lo
-00016a70: 6164 5f66 6f6e 7473 5f66 726f 6d5f 6469  ad_fonts_from_di
-00016a80: 7228 6469 7265 6374 6f72 793a 2073 7472  r(directory: str
-00016a90: 2920 2d3e 2073 6574 3a0a 2020 2020 2222  ) -> set:.    ""
-00016aa0: 220a 2020 2020 5765 6c6c 2069 7420 6c6f  ".    Well it lo
-00016ab0: 6164 7320 666f 6e74 7320 6672 6f6d 2061  ads fonts from a
-00016ac0: 2064 6972 6563 746f 7279 2e2e 2e0a 2020   directory....  
-00016ad0: 2020 2222 220a 2020 2020 666f 6e74 5f66    """.    font_f
-00016ae0: 616d 696c 6965 7320 3d20 7365 7428 290a  amilies = set().
-00016af0: 2020 2020 666f 7220 5f66 6920 696e 2051      for _fi in Q
-00016b00: 4469 7228 6469 7265 6374 6f72 7929 2e65  Dir(directory).e
-00016b10: 6e74 7279 496e 666f 4c69 7374 285b 222a  ntryInfoList(["*
-00016b20: 2e74 7466 222c 2022 2a2e 776f 6666 222c  .ttf", "*.woff",
-00016b30: 2022 2a2e 776f 6666 3222 5d29 3a0a 2020   "*.woff2"]):.  
-00016b40: 2020 2020 2020 5f69 6420 3d20 5146 6f6e        _id = QFon
-00016b50: 7444 6174 6162 6173 652e 6164 6441 7070  tDatabase.addApp
-00016b60: 6c69 6361 7469 6f6e 466f 6e74 285f 6669  licationFont(_fi
-00016b70: 2e61 6273 6f6c 7574 6546 696c 6550 6174  .absoluteFilePat
-00016b80: 6828 2929 0a20 2020 2020 2020 2066 6f6e  h()).        fon
-00016b90: 745f 6661 6d69 6c69 6573 207c 3d20 7365  t_families |= se
-00016ba0: 7428 5146 6f6e 7444 6174 6162 6173 652e  t(QFontDatabase.
-00016bb0: 6170 706c 6963 6174 696f 6e46 6f6e 7446  applicationFontF
-00016bc0: 616d 696c 6965 7328 5f69 6429 290a 2020  amilies(_id)).  
-00016bd0: 2020 7265 7475 726e 2066 6f6e 745f 6661    return font_fa
-00016be0: 6d69 6c69 6573 0a0a 0a64 6566 2069 6e73  milies...def ins
-00016bf0: 7461 6c6c 5f69 636f 6e73 2829 3a0a 2020  tall_icons():.  
-00016c00: 2020 2222 2249 6e73 7461 6c6c 2069 636f    """Install ico
-00016c10: 6e73 2222 220a 2020 2020 6f73 2e73 7973  ns""".    os.sys
-00016c20: 7465 6d28 0a20 2020 2020 2020 2022 7864  tem(.        "xd
-00016c30: 672d 6963 6f6e 2d72 6573 6f75 7263 6520  g-icon-resource 
-00016c40: 696e 7374 616c 6c20 2d2d 7369 7a65 2033  install --size 3
-00016c50: 3220 2d2d 636f 6e74 6578 7420 6170 7073  2 --context apps
-00016c60: 202d 2d6d 6f64 6520 7573 6572 2022 0a20   --mode user ". 
-00016c70: 2020 2020 2020 2066 227b 574f 524b 494e         f"{WORKIN
-00016c80: 475f 5041 5448 7d2f 6461 7461 2f6b 3667  G_PATH}/data/k6g
-00016c90: 7465 2e6e 6f74 316d 6d2d 3332 2e70 6e67  te.not1mm-32.png
-00016ca0: 206b 3667 7465 2d6e 6f74 316d 6d22 0a20   k6gte-not1mm". 
-00016cb0: 2020 2029 0a20 2020 206f 732e 7379 7374     ).    os.syst
-00016cc0: 656d 280a 2020 2020 2020 2020 2278 6467  em(.        "xdg
-00016cd0: 2d69 636f 6e2d 7265 736f 7572 6365 2069  -icon-resource i
-00016ce0: 6e73 7461 6c6c 202d 2d73 697a 6520 3634  nstall --size 64
-00016cf0: 202d 2d63 6f6e 7465 7874 2061 7070 7320   --context apps 
-00016d00: 2d2d 6d6f 6465 2075 7365 7220 220a 2020  --mode user ".  
-00016d10: 2020 2020 2020 6622 7b57 4f52 4b49 4e47        f"{WORKING
-00016d20: 5f50 4154 487d 2f64 6174 612f 6b36 6774  _PATH}/data/k6gt
-00016d30: 652e 6e6f 7431 6d6d 2d36 342e 706e 6720  e.not1mm-64.png 
-00016d40: 6b36 6774 652d 6e6f 7431 6d6d 220a 2020  k6gte-not1mm".  
-00016d50: 2020 290a 2020 2020 6f73 2e73 7973 7465    ).    os.syste
-00016d60: 6d28 0a20 2020 2020 2020 2022 7864 672d  m(.        "xdg-
-00016d70: 6963 6f6e 2d72 6573 6f75 7263 6520 696e  icon-resource in
-00016d80: 7374 616c 6c20 2d2d 7369 7a65 2031 3238  stall --size 128
-00016d90: 202d 2d63 6f6e 7465 7874 2061 7070 7320   --context apps 
-00016da0: 2d2d 6d6f 6465 2075 7365 7220 220a 2020  --mode user ".  
-00016db0: 2020 2020 2020 6622 7b57 4f52 4b49 4e47        f"{WORKING
-00016dc0: 5f50 4154 487d 2f64 6174 612f 6b36 6774  _PATH}/data/k6gt
-00016dd0: 652e 6e6f 7431 6d6d 2d31 3238 2e70 6e67  e.not1mm-128.png
-00016de0: 206b 3667 7465 2d6e 6f74 316d 6d22 0a20   k6gte-not1mm". 
-00016df0: 2020 2029 0a20 2020 206f 732e 7379 7374     ).    os.syst
-00016e00: 656d 2866 2278 6467 2d64 6573 6b74 6f70  em(f"xdg-desktop
-00016e10: 2d6d 656e 7520 696e 7374 616c 6c20 7b57  -menu install {W
-00016e20: 4f52 4b49 4e47 5f50 4154 487d 2f64 6174  ORKING_PATH}/dat
-00016e30: 612f 6b36 6774 652d 6e6f 7431 6d6d 2e64  a/k6gte-not1mm.d
-00016e40: 6573 6b74 6f70 2229 0a0a 0a64 6566 2064  esktop")...def d
-00016e50: 6f69 6d70 286d 6f64 6e61 6d65 293a 0a20  oimp(modname):. 
-00016e60: 2020 2022 2222 7265 7475 726e 206d 6f64     """return mod
-00016e70: 756c 6520 7061 7468 2222 220a 2020 2020  ule path""".    
-00016e80: 7265 7475 726e 2069 6d70 6f72 746c 6962  return importlib
-00016e90: 2e69 6d70 6f72 745f 6d6f 6475 6c65 2866  .import_module(f
-00016ea0: 226e 6f74 316d 6d2e 706c 7567 696e 732e  "not1mm.plugins.
-00016eb0: 7b6d 6f64 6e61 6d65 7d22 290a 0a0a 6465  {modname}")...de
-00016ec0: 6620 7275 6e28 293a 0a20 2020 2022 2222  f run():.    """
-00016ed0: 0a20 2020 204d 6169 6e20 456e 7472 790a  .    Main Entry.
-00016ee0: 2020 2020 2222 220a 2020 2020 696e 7374      """.    inst
-00016ef0: 616c 6c5f 6963 6f6e 7328 290a 2020 2020  all_icons().    
-00016f00: 7469 6d65 722e 7374 6172 7428 3235 3029  timer.start(250)
-00016f10: 0a20 2020 2073 7973 2e65 7869 7428 6170  .    sys.exit(ap
-00016f20: 702e 6578 6563 2829 290a 0a0a 6c6f 6767  p.exec())...logg
-00016f30: 6572 203d 206c 6f67 6769 6e67 2e67 6574  er = logging.get
-00016f40: 4c6f 6767 6572 2822 5f5f 6d61 696e 5f5f  Logger("__main__
-00016f50: 2229 0a68 616e 646c 6572 203d 206c 6f67  ").handler = log
-00016f60: 6769 6e67 2e53 7472 6561 6d48 616e 646c  ging.StreamHandl
-00016f70: 6572 2829 0a66 6f72 6d61 7474 6572 203d  er().formatter =
-00016f80: 206c 6f67 6769 6e67 2e46 6f72 6d61 7474   logging.Formatt
-00016f90: 6572 280a 2020 2020 6461 7465 666d 743d  er(.    datefmt=
-00016fa0: 2225 483a 254d 3a25 5322 2c0a 2020 2020  "%H:%M:%S",.    
-00016fb0: 666d 743d 225b 2528 6173 6374 696d 6529  fmt="[%(asctime)
-00016fc0: 735d 2025 286c 6576 656c 6e61 6d65 2973  s] %(levelname)s
-00016fd0: 2025 286d 6f64 756c 6529 7320 2d20 2528   %(module)s - %(
-00016fe0: 6675 6e63 4e61 6d65 2973 204c 696e 6520  funcName)s Line 
-00016ff0: 2528 6c69 6e65 6e6f 2964 3a20 2528 6d65  %(lineno)d: %(me
-00017000: 7373 6167 6529 7322 2c0a 290a 6861 6e64  ssage)s",.).hand
-00017010: 6c65 722e 7365 7446 6f72 6d61 7474 6572  ler.setFormatter
-00017020: 2866 6f72 6d61 7474 6572 290a 6c6f 6767  (formatter).logg
-00017030: 6572 2e61 6464 4861 6e64 6c65 7228 6861  er.addHandler(ha
-00017040: 6e64 6c65 7229 0a0a 4245 5441 5f54 4553  ndler)..BETA_TES
-00017050: 5420 3d20 4661 6c73 650a 6966 2050 6174  T = False.if Pat
-00017060: 6828 222e 2f62 6574 6174 6573 7422 292e  h("./betatest").
-00017070: 6578 6973 7473 2829 3a0a 2020 2020 4245  exists():.    BE
-00017080: 5441 5f54 4553 5420 3d20 5472 7565 0a0a  TA_TEST = True..
-00017090: 6966 2050 6174 6828 222e 2f64 6562 7567  if Path("./debug
-000170a0: 2229 2e65 7869 7374 7328 293a 0a20 2020  ").exists():.   
-000170b0: 206c 6f67 6765 722e 7365 744c 6576 656c   logger.setLevel
-000170c0: 286c 6f67 6769 6e67 2e44 4542 5547 290a  (logging.DEBUG).
-000170d0: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
-000170e0: 2822 6465 6275 6767 696e 6720 6f6e 2229  ("debugging on")
-000170f0: 0a65 6c73 653a 0a20 2020 206c 6f67 6765  .else:.    logge
-00017100: 722e 7365 744c 6576 656c 286c 6f67 6769  r.setLevel(loggi
-00017110: 6e67 2e57 4152 4e49 4e47 290a 2020 2020  ng.WARNING).    
-00017120: 6c6f 6767 6572 2e77 6172 6e69 6e67 2822  logger.warning("
-00017130: 6465 6275 6767 696e 6720 6f66 6622 290a  debugging off").
-00017140: 0a61 7070 203d 2051 7457 6964 6765 7473  .app = QtWidgets
-00017150: 2e51 4170 706c 6963 6174 696f 6e28 7379  .QApplication(sy
-00017160: 732e 6172 6776 290a 6170 702e 7365 7453  s.argv).app.setS
-00017170: 7479 6c65 2822 4164 7761 6974 612d 4461  tyle("Adwaita-Da
-00017180: 726b 2229 0a66 6f6e 745f 7061 7468 203d  rk").font_path =
-00017190: 2057 4f52 4b49 4e47 5f50 4154 4820 2b20   WORKING_PATH + 
-000171a0: 222f 6461 7461 220a 6661 6d69 6c69 6573  "/data".families
-000171b0: 203d 206c 6f61 645f 666f 6e74 735f 6672   = load_fonts_fr
-000171c0: 6f6d 5f64 6972 286f 732e 6673 7061 7468  om_dir(os.fspath
-000171d0: 2866 6f6e 745f 7061 7468 2929 0a6c 6f67  (font_path)).log
-000171e0: 6765 722e 696e 666f 2866 616d 696c 6965  ger.info(familie
-000171f0: 7329 0a77 696e 646f 7720 3d20 4d61 696e  s).window = Main
-00017200: 5769 6e64 6f77 2829 0a68 6569 6768 7420  Window().height 
-00017210: 3d20 7769 6e64 6f77 2e70 7265 662e 6765  = window.pref.ge
-00017220: 7428 2277 696e 646f 775f 6865 6967 6874  t("window_height
-00017230: 222c 2033 3030 290a 7769 6474 6820 3d20  ", 300).width = 
-00017240: 7769 6e64 6f77 2e70 7265 662e 6765 7428  window.pref.get(
-00017250: 2277 696e 646f 775f 7769 6474 6822 2c20  "window_width", 
-00017260: 3730 3029 0a78 203d 2077 696e 646f 772e  700).x = window.
-00017270: 7072 6566 2e67 6574 2822 7769 6e64 6f77  pref.get("window
-00017280: 5f78 222c 202d 3129 0a79 203d 2077 696e  _x", -1).y = win
-00017290: 646f 772e 7072 6566 2e67 6574 2822 7769  dow.pref.get("wi
-000172a0: 6e64 6f77 5f79 222c 202d 3129 0a77 696e  ndow_y", -1).win
-000172b0: 646f 772e 7365 7447 656f 6d65 7472 7928  dow.setGeometry(
-000172c0: 782c 2079 2c20 7769 6474 682c 2068 6569  x, y, width, hei
-000172d0: 6768 7429 0a77 696e 646f 772e 6361 6c6c  ght).window.call
-000172e0: 7369 676e 2e73 6574 466f 6375 7328 290a  sign.setFocus().
-000172f0: 7769 6e64 6f77 2e73 686f 7728 290a 7469  window.show().ti
-00017300: 6d65 7220 3d20 5174 436f 7265 2e51 5469  mer = QtCore.QTi
-00017310: 6d65 7228 290a 7469 6d65 722e 7469 6d65  mer().timer.time
-00017320: 6f75 742e 636f 6e6e 6563 7428 7769 6e64  out.connect(wind
-00017330: 6f77 2e70 6f6c 6c5f 7261 6469 6f29 0a0a  ow.poll_radio)..
-00017340: 6966 205f 5f6e 616d 655f 5f20 3d3d 2022  if __name__ == "
-00017350: 5f5f 6d61 696e 5f5f 223a 0a20 2020 2072  __main__":.    r
-00017360: 756e 2829 0a                             un().
+00015ac0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00015ad0: 662e 7072 6566 2e67 6574 2822 7275 6e5f  f.pref.get("run_
+00015ae0: 7374 6174 6522 2c20 4661 6c73 6529 0a20  state", False). 
+00015af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015b00: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00015b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015b20: 2020 2020 2020 2020 2073 656c 662e 6e31           self.n1
+00015b30: 6d6d 2e73 656e 645f 7261 6469 6f28 290a  mm.send_radio().
+00015b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015b50: 2020 2020 676c 6f62 616c 7328 295b 2270      globals()["p
+00015b60: 6f6c 6c5f 7469 6d65 225d 203d 2064 6174  oll_time"] = dat
+00015b70: 6574 696d 652e 6e6f 7728 2920 2b20 6474  etime.now() + dt
+00015b80: 2e74 696d 6564 656c 7461 2873 6563 6f6e  .timedelta(secon
+00015b90: 6473 3d31 3029 0a0a 2020 2020 6465 6620  ds=10)..    def 
+00015ba0: 6564 6974 5f63 775f 6d61 6372 6f73 2873  edit_cw_macros(s
+00015bb0: 656c 6629 202d 3e20 4e6f 6e65 3a0a 2020  elf) -> None:.  
+00015bc0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00015bd0: 2020 4361 6c6c 7320 7468 6520 6465 6661    Calls the defa
+00015be0: 756c 7420 7465 7874 2065 6469 746f 7220  ult text editor 
+00015bf0: 746f 2065 6469 7420 7468 6520 4357 206d  to edit the CW m
+00015c00: 6163 726f 2066 696c 652e 0a20 2020 2020  acro file..     
+00015c10: 2020 2022 2222 0a20 2020 2020 2020 2069     """.        i
+00015c20: 6620 7365 6c66 2e72 6164 696f 5f73 7461  f self.radio_sta
+00015c30: 7465 2e67 6574 2822 6d6f 6465 2229 203d  te.get("mode") =
+00015c40: 3d20 2243 5722 3a0a 2020 2020 2020 2020  = "CW":.        
+00015c50: 2020 2020 6d61 6372 6f5f 6669 6c65 203d      macro_file =
+00015c60: 2022 2f63 776d 6163 726f 732e 7478 7422   "/cwmacros.txt"
+00015c70: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+00015c80: 2020 2020 2020 2020 2020 206d 6163 726f             macro
+00015c90: 5f66 696c 6520 3d20 222f 7373 626d 6163  _file = "/ssbmac
+00015ca0: 726f 732e 7478 7422 0a20 2020 2020 2020  ros.txt".       
+00015cb0: 2069 6620 6e6f 7420 5061 7468 2844 4154   if not Path(DAT
+00015cc0: 415f 5041 5448 202b 206d 6163 726f 5f66  A_PATH + macro_f
+00015cd0: 696c 6529 2e65 7869 7374 7328 293a 0a20  ile).exists():. 
+00015ce0: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
+00015cf0: 722e 6465 6275 6728 2272 6561 645f 6377  r.debug("read_cw
+00015d00: 5f6d 6163 726f 733a 2063 6f70 7969 6e67  _macros: copying
+00015d10: 2064 6566 6175 6c74 206d 6163 726f 2066   default macro f
+00015d20: 696c 652e 2229 0a20 2020 2020 2020 2020  ile.").         
+00015d30: 2020 2063 6f70 7966 696c 6528 574f 524b     copyfile(WORK
+00015d40: 494e 475f 5041 5448 202b 2022 2f64 6174  ING_PATH + "/dat
+00015d50: 6122 202b 206d 6163 726f 5f66 696c 652c  a" + macro_file,
+00015d60: 2044 4154 415f 5041 5448 202b 206d 6163   DATA_PATH + mac
+00015d70: 726f 5f66 696c 6529 0a20 2020 2020 2020  ro_file).       
+00015d80: 206f 732e 7379 7374 656d 2866 2278 6467   os.system(f"xdg
+00015d90: 2d6f 7065 6e20 7b44 4154 415f 5041 5448  -open {DATA_PATH
+00015da0: 7d7b 6d61 6372 6f5f 6669 6c65 7d22 290a  }{macro_file}").
+00015db0: 0a20 2020 2064 6566 2072 6561 645f 6377  .    def read_cw
+00015dc0: 5f6d 6163 726f 7328 7365 6c66 2920 2d3e  _macros(self) ->
+00015dd0: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
+00015de0: 2222 0a20 2020 2020 2020 2052 6561 6473  "".        Reads
+00015df0: 2069 6e20 7468 6520 4357 206d 6163 726f   in the CW macro
+00015e00: 732c 2066 6972 7374 7320 6974 2063 6865  s, firsts it che
+00015e10: 636b 7320 746f 2073 6565 2069 6620 7468  cks to see if th
+00015e20: 6520 6669 6c65 2065 7869 7374 732e 2049  e file exists. I
+00015e30: 6620 6974 2064 6f65 7320 6e6f 742c 0a20  f it does not,. 
+00015e40: 2020 2020 2020 2061 6e64 2074 6869 7320         and this 
+00015e50: 6861 7320 6265 656e 2070 6163 6b61 6765  has been package
+00015e60: 6420 7769 7468 2070 7969 6e73 7461 6c6c  d with pyinstall
+00015e70: 6572 2069 7420 7769 6c6c 2063 6f70 7920  er it will copy 
+00015e80: 7468 6520 6465 6661 756c 7420 6669 6c65  the default file
+00015e90: 2066 726f 6d20 7468 650a 2020 2020 2020   from the.      
+00015ea0: 2020 7465 6d70 2064 6972 6563 746f 7279    temp directory
+00015eb0: 2074 6869 7320 6973 2072 756e 6e69 6e67   this is running
+00015ec0: 2066 726f 6d2e 2e2e 2049 6e20 7468 656f   from... In theo
+00015ed0: 7279 2e0a 2020 2020 2020 2020 2222 220a  ry..        """.
+00015ee0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00015ef0: 2e72 6164 696f 5f73 7461 7465 2e67 6574  .radio_state.get
+00015f00: 2822 6d6f 6465 2229 203d 3d20 2243 5722  ("mode") == "CW"
+00015f10: 3a0a 2020 2020 2020 2020 2020 2020 6d61  :.            ma
+00015f20: 6372 6f5f 6669 6c65 203d 2022 2f63 776d  cro_file = "/cwm
+00015f30: 6163 726f 732e 7478 7422 0a20 2020 2020  acros.txt".     
+00015f40: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00015f50: 2020 2020 206d 6163 726f 5f66 696c 6520       macro_file 
+00015f60: 3d20 222f 7373 626d 6163 726f 732e 7478  = "/ssbmacros.tx
+00015f70: 7422 0a0a 2020 2020 2020 2020 6966 206e  t"..        if n
+00015f80: 6f74 2050 6174 6828 4441 5441 5f50 4154  ot Path(DATA_PAT
+00015f90: 4820 2b20 6d61 6372 6f5f 6669 6c65 292e  H + macro_file).
+00015fa0: 6578 6973 7473 2829 3a0a 2020 2020 2020  exists():.      
+00015fb0: 2020 2020 2020 6c6f 6767 6572 2e64 6562        logger.deb
+00015fc0: 7567 2822 7265 6164 5f63 775f 6d61 6372  ug("read_cw_macr
+00015fd0: 6f73 3a20 636f 7079 696e 6720 6465 6661  os: copying defa
+00015fe0: 756c 7420 6d61 6372 6f20 6669 6c65 2e22  ult macro file."
+00015ff0: 290a 2020 2020 2020 2020 2020 2020 636f  ).            co
+00016000: 7079 6669 6c65 2857 4f52 4b49 4e47 5f50  pyfile(WORKING_P
+00016010: 4154 4820 2b20 222f 6461 7461 2220 2b20  ATH + "/data" + 
+00016020: 6d61 6372 6f5f 6669 6c65 2c20 4441 5441  macro_file, DATA
+00016030: 5f50 4154 4820 2b20 6d61 6372 6f5f 6669  _PATH + macro_fi
+00016040: 6c65 290a 2020 2020 2020 2020 7769 7468  le).        with
+00016050: 206f 7065 6e28 4441 5441 5f50 4154 4820   open(DATA_PATH 
+00016060: 2b20 6d61 6372 6f5f 6669 6c65 2c20 2272  + macro_file, "r
+00016070: 222c 2065 6e63 6f64 696e 673d 2275 7466  ", encoding="utf
+00016080: 2d38 2229 2061 7320 6669 6c65 5f64 6573  -8") as file_des
+00016090: 6372 6970 746f 723a 0a20 2020 2020 2020  criptor:.       
+000160a0: 2020 2020 2066 6f72 206c 696e 6520 696e       for line in
+000160b0: 2066 696c 655f 6465 7363 7269 7074 6f72   file_descriptor
+000160c0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000160d0: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
+000160e0: 2020 2020 2020 2020 2020 206d 6f64 652c             mode,
+000160f0: 2066 6b65 792c 2062 7574 746f 6e6e 616d   fkey, buttonnam
+00016100: 652c 2063 7774 6578 7420 3d20 6c69 6e65  e, cwtext = line
+00016110: 2e73 706c 6974 2822 7c22 290a 2020 2020  .split("|").    
+00016120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016130: 6966 206d 6f64 652e 7374 7269 7028 292e  if mode.strip().
+00016140: 7570 7065 7228 2920 3d3d 2022 5222 2061  upper() == "R" a
+00016150: 6e64 2073 656c 662e 7072 6566 2e67 6574  nd self.pref.get
+00016160: 2822 7275 6e5f 7374 6174 6522 293a 0a20  ("run_state"):. 
+00016170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016180: 2020 2020 2020 2073 656c 662e 666b 6579         self.fkey
+00016190: 735b 666b 6579 2e73 7472 6970 2829 5d20  s[fkey.strip()] 
+000161a0: 3d20 2862 7574 746f 6e6e 616d 652e 7374  = (buttonname.st
+000161b0: 7269 7028 292c 2063 7774 6578 742e 7374  rip(), cwtext.st
+000161c0: 7269 7028 2929 0a20 2020 2020 2020 2020  rip()).         
+000161d0: 2020 2020 2020 2020 2020 2069 6620 6d6f             if mo
+000161e0: 6465 2e73 7472 6970 2829 2e75 7070 6572  de.strip().upper
+000161f0: 2829 2021 3d20 2252 2220 616e 6420 6e6f  () != "R" and no
+00016200: 7420 7365 6c66 2e70 7265 662e 6765 7428  t self.pref.get(
+00016210: 2272 756e 5f73 7461 7465 2229 3a0a 2020  "run_state"):.  
+00016220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016230: 2020 2020 2020 7365 6c66 2e66 6b65 7973        self.fkeys
+00016240: 5b66 6b65 792e 7374 7269 7028 295d 203d  [fkey.strip()] =
+00016250: 2028 6275 7474 6f6e 6e61 6d65 2e73 7472   (buttonname.str
+00016260: 6970 2829 2c20 6377 7465 7874 2e73 7472  ip(), cwtext.str
+00016270: 6970 2829 290a 2020 2020 2020 2020 2020  ip()).          
+00016280: 2020 2020 2020 6578 6365 7074 2056 616c        except Val
+00016290: 7565 4572 726f 7220 6173 2065 7272 3a0a  ueError as err:.
+000162a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000162b0: 2020 2020 6c6f 6767 6572 2e69 6e66 6f28      logger.info(
+000162c0: 2272 6561 645f 6377 5f6d 6163 726f 733a  "read_cw_macros:
+000162d0: 2025 7322 2c20 6572 7229 0a20 2020 2020   %s", err).     
+000162e0: 2020 206b 6579 7320 3d20 7365 6c66 2e66     keys = self.f
+000162f0: 6b65 7973 2e6b 6579 7328 290a 2020 2020  keys.keys().    
+00016300: 2020 2020 6966 2022 4631 2220 696e 206b      if "F1" in k
+00016310: 6579 733a 0a20 2020 2020 2020 2020 2020  eys:.           
+00016320: 2073 656c 662e 4631 2e73 6574 5465 7874   self.F1.setText
+00016330: 2866 2246 313a 207b 7365 6c66 2e66 6b65  (f"F1: {self.fke
+00016340: 7973 5b27 4631 275d 5b30 5d7d 2229 0a20  ys['F1'][0]}"). 
+00016350: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00016360: 4631 2e73 6574 546f 6f6c 5469 7028 7365  F1.setToolTip(se
+00016370: 6c66 2e66 6b65 7973 5b22 4631 225d 5b31  lf.fkeys["F1"][1
+00016380: 5d29 0a20 2020 2020 2020 2069 6620 2246  ]).        if "F
+00016390: 3222 2069 6e20 6b65 7973 3a0a 2020 2020  2" in keys:.    
+000163a0: 2020 2020 2020 2020 7365 6c66 2e46 322e          self.F2.
+000163b0: 7365 7454 6578 7428 6622 4632 3a20 7b73  setText(f"F2: {s
+000163c0: 656c 662e 666b 6579 735b 2746 3227 5d5b  elf.fkeys['F2'][
+000163d0: 305d 7d22 290a 2020 2020 2020 2020 2020  0]}").          
+000163e0: 2020 7365 6c66 2e46 322e 7365 7454 6f6f    self.F2.setToo
+000163f0: 6c54 6970 2873 656c 662e 666b 6579 735b  lTip(self.fkeys[
+00016400: 2246 3222 5d5b 315d 290a 2020 2020 2020  "F2"][1]).      
+00016410: 2020 6966 2022 4633 2220 696e 206b 6579    if "F3" in key
+00016420: 733a 0a20 2020 2020 2020 2020 2020 2073  s:.            s
+00016430: 656c 662e 4633 2e73 6574 5465 7874 2866  elf.F3.setText(f
+00016440: 2246 333a 207b 7365 6c66 2e66 6b65 7973  "F3: {self.fkeys
+00016450: 5b27 4633 275d 5b30 5d7d 2229 0a20 2020  ['F3'][0]}").   
+00016460: 2020 2020 2020 2020 2073 656c 662e 4633           self.F3
+00016470: 2e73 6574 546f 6f6c 5469 7028 7365 6c66  .setToolTip(self
+00016480: 2e66 6b65 7973 5b22 4633 225d 5b31 5d29  .fkeys["F3"][1])
+00016490: 0a20 2020 2020 2020 2069 6620 2246 3422  .        if "F4"
+000164a0: 2069 6e20 6b65 7973 3a0a 2020 2020 2020   in keys:.      
+000164b0: 2020 2020 2020 7365 6c66 2e46 342e 7365        self.F4.se
+000164c0: 7454 6578 7428 6622 4634 3a20 7b73 656c  tText(f"F4: {sel
+000164d0: 662e 666b 6579 735b 2746 3427 5d5b 305d  f.fkeys['F4'][0]
+000164e0: 7d22 290a 2020 2020 2020 2020 2020 2020  }").            
+000164f0: 7365 6c66 2e46 342e 7365 7454 6f6f 6c54  self.F4.setToolT
+00016500: 6970 2873 656c 662e 666b 6579 735b 2246  ip(self.fkeys["F
+00016510: 3422 5d5b 315d 290a 2020 2020 2020 2020  4"][1]).        
+00016520: 6966 2022 4635 2220 696e 206b 6579 733a  if "F5" in keys:
+00016530: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00016540: 662e 4635 2e73 6574 5465 7874 2866 2246  f.F5.setText(f"F
+00016550: 353a 207b 7365 6c66 2e66 6b65 7973 5b27  5: {self.fkeys['
+00016560: 4635 275d 5b30 5d7d 2229 0a20 2020 2020  F5'][0]}").     
+00016570: 2020 2020 2020 2073 656c 662e 4635 2e73         self.F5.s
+00016580: 6574 546f 6f6c 5469 7028 7365 6c66 2e66  etToolTip(self.f
+00016590: 6b65 7973 5b22 4635 225d 5b31 5d29 0a20  keys["F5"][1]). 
+000165a0: 2020 2020 2020 2069 6620 2246 3622 2069         if "F6" i
+000165b0: 6e20 6b65 7973 3a0a 2020 2020 2020 2020  n keys:.        
+000165c0: 2020 2020 7365 6c66 2e46 362e 7365 7454      self.F6.setT
+000165d0: 6578 7428 6622 4636 3a20 7b73 656c 662e  ext(f"F6: {self.
+000165e0: 666b 6579 735b 2746 3627 5d5b 305d 7d22  fkeys['F6'][0]}"
+000165f0: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
+00016600: 6c66 2e46 362e 7365 7454 6f6f 6c54 6970  lf.F6.setToolTip
+00016610: 2873 656c 662e 666b 6579 735b 2246 3622  (self.fkeys["F6"
+00016620: 5d5b 315d 290a 2020 2020 2020 2020 6966  ][1]).        if
+00016630: 2022 4637 2220 696e 206b 6579 733a 0a20   "F7" in keys:. 
+00016640: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00016650: 4637 2e73 6574 5465 7874 2866 2246 373a  F7.setText(f"F7:
+00016660: 207b 7365 6c66 2e66 6b65 7973 5b27 4637   {self.fkeys['F7
+00016670: 275d 5b30 5d7d 2229 0a20 2020 2020 2020  '][0]}").       
+00016680: 2020 2020 2073 656c 662e 4637 2e73 6574       self.F7.set
+00016690: 546f 6f6c 5469 7028 7365 6c66 2e66 6b65  ToolTip(self.fke
+000166a0: 7973 5b22 4637 225d 5b31 5d29 0a20 2020  ys["F7"][1]).   
+000166b0: 2020 2020 2069 6620 2246 3822 2069 6e20       if "F8" in 
+000166c0: 6b65 7973 3a0a 2020 2020 2020 2020 2020  keys:.          
+000166d0: 2020 7365 6c66 2e46 382e 7365 7454 6578    self.F8.setTex
+000166e0: 7428 6622 4638 3a20 7b73 656c 662e 666b  t(f"F8: {self.fk
+000166f0: 6579 735b 2746 3827 5d5b 305d 7d22 290a  eys['F8'][0]}").
+00016700: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00016710: 2e46 382e 7365 7454 6f6f 6c54 6970 2873  .F8.setToolTip(s
+00016720: 656c 662e 666b 6579 735b 2246 3822 5d5b  elf.fkeys["F8"][
+00016730: 315d 290a 2020 2020 2020 2020 6966 2022  1]).        if "
+00016740: 4639 2220 696e 206b 6579 733a 0a20 2020  F9" in keys:.   
+00016750: 2020 2020 2020 2020 2073 656c 662e 4639           self.F9
+00016760: 2e73 6574 5465 7874 2866 2246 393a 207b  .setText(f"F9: {
+00016770: 7365 6c66 2e66 6b65 7973 5b27 4639 275d  self.fkeys['F9']
+00016780: 5b30 5d7d 2229 0a20 2020 2020 2020 2020  [0]}").         
+00016790: 2020 2073 656c 662e 4639 2e73 6574 546f     self.F9.setTo
+000167a0: 6f6c 5469 7028 7365 6c66 2e66 6b65 7973  olTip(self.fkeys
+000167b0: 5b22 4639 225d 5b31 5d29 0a20 2020 2020  ["F9"][1]).     
+000167c0: 2020 2069 6620 2246 3130 2220 696e 206b     if "F10" in k
+000167d0: 6579 733a 0a20 2020 2020 2020 2020 2020  eys:.           
+000167e0: 2073 656c 662e 4631 302e 7365 7454 6578   self.F10.setTex
+000167f0: 7428 6622 4631 303a 207b 7365 6c66 2e66  t(f"F10: {self.f
+00016800: 6b65 7973 5b27 4631 3027 5d5b 305d 7d22  keys['F10'][0]}"
+00016810: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
+00016820: 6c66 2e46 3130 2e73 6574 546f 6f6c 5469  lf.F10.setToolTi
+00016830: 7028 7365 6c66 2e66 6b65 7973 5b22 4631  p(self.fkeys["F1
+00016840: 3022 5d5b 315d 290a 2020 2020 2020 2020  0"][1]).        
+00016850: 6966 2022 4631 3122 2069 6e20 6b65 7973  if "F11" in keys
+00016860: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00016870: 6c66 2e46 3131 2e73 6574 5465 7874 2866  lf.F11.setText(f
+00016880: 2246 3131 3a20 7b73 656c 662e 666b 6579  "F11: {self.fkey
+00016890: 735b 2746 3131 275d 5b30 5d7d 2229 0a20  s['F11'][0]}"). 
+000168a0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000168b0: 4631 312e 7365 7454 6f6f 6c54 6970 2873  F11.setToolTip(s
+000168c0: 656c 662e 666b 6579 735b 2246 3131 225d  elf.fkeys["F11"]
+000168d0: 5b31 5d29 0a20 2020 2020 2020 2069 6620  [1]).        if 
+000168e0: 2246 3132 2220 696e 206b 6579 733a 0a20  "F12" in keys:. 
+000168f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00016900: 4631 322e 7365 7454 6578 7428 6622 4631  F12.setText(f"F1
+00016910: 323a 207b 7365 6c66 2e66 6b65 7973 5b27  2: {self.fkeys['
+00016920: 4631 3227 5d5b 305d 7d22 290a 2020 2020  F12'][0]}").    
+00016930: 2020 2020 2020 2020 7365 6c66 2e46 3132          self.F12
+00016940: 2e73 6574 546f 6f6c 5469 7028 7365 6c66  .setToolTip(self
+00016950: 2e66 6b65 7973 5b22 4631 3222 5d5b 315d  .fkeys["F12"][1]
+00016960: 290a 0a20 2020 2064 6566 2067 656e 6572  )..    def gener
+00016970: 6174 655f 6164 6966 2873 656c 6629 3a0a  ate_adif(self):.
+00016980: 2020 2020 2020 2020 2222 2247 656e 6572          """Gener
+00016990: 6174 6520 4144 4946 2222 220a 2020 2020  ate ADIF""".    
+000169a0: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
+000169b0: 2822 2a2a 2a2a 2a2a 4144 4946 2a2a 2a2a  ("******ADIF****
+000169c0: 2a22 290a 2020 2020 2020 2020 7365 6c66  *").        self
+000169d0: 2e63 6f6e 7465 7374 2e61 6469 6628 7365  .contest.adif(se
+000169e0: 6c66 290a 0a20 2020 2064 6566 2067 656e  lf)..    def gen
+000169f0: 6572 6174 655f 6361 6272 696c 6c6f 2873  erate_cabrillo(s
+00016a00: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
+00016a10: 2247 656e 6572 6174 6573 2043 6162 7269  "Generates Cabri
+00016a20: 6c6c 6f20 6669 6c65 2e20 4d61 7962 652e  llo file. Maybe.
+00016a30: 2222 220a 2020 2020 2020 2020 2320 6874  """.        # ht
+00016a40: 7470 733a 2f2f 7777 772e 6371 7770 782e  tps://www.cqwpx.
+00016a50: 636f 6d2f 6361 6272 696c 6c6f 2e68 746d  com/cabrillo.htm
+00016a60: 0a20 2020 2020 2020 206c 6f67 6765 722e  .        logger.
+00016a70: 6465 6275 6728 222a 2a2a 2a2a 2a43 6162  debug("******Cab
+00016a80: 7269 6c6c 6f2a 2a2a 2a2a 2229 0a20 2020  rillo*****").   
+00016a90: 2020 2020 2073 656c 662e 636f 6e74 6573       self.contes
+00016aa0: 742e 6361 6272 696c 6c6f 2873 656c 6629  t.cabrillo(self)
+00016ab0: 0a0a 0a64 6566 206c 6f61 645f 666f 6e74  ...def load_font
+00016ac0: 735f 6672 6f6d 5f64 6972 2864 6972 6563  s_from_dir(direc
+00016ad0: 746f 7279 3a20 7374 7229 202d 3e20 7365  tory: str) -> se
+00016ae0: 743a 0a20 2020 2022 2222 0a20 2020 2057  t:.    """.    W
+00016af0: 656c 6c20 6974 206c 6f61 6473 2066 6f6e  ell it loads fon
+00016b00: 7473 2066 726f 6d20 6120 6469 7265 6374  ts from a direct
+00016b10: 6f72 792e 2e2e 0a20 2020 2022 2222 0a20  ory....    """. 
+00016b20: 2020 2066 6f6e 745f 6661 6d69 6c69 6573     font_families
+00016b30: 203d 2073 6574 2829 0a20 2020 2066 6f72   = set().    for
+00016b40: 205f 6669 2069 6e20 5144 6972 2864 6972   _fi in QDir(dir
+00016b50: 6563 746f 7279 292e 656e 7472 7949 6e66  ectory).entryInf
+00016b60: 6f4c 6973 7428 5b22 2a2e 7474 6622 2c20  oList(["*.ttf", 
+00016b70: 222a 2e77 6f66 6622 2c20 222a 2e77 6f66  "*.woff", "*.wof
+00016b80: 6632 225d 293a 0a20 2020 2020 2020 205f  f2"]):.        _
+00016b90: 6964 203d 2051 466f 6e74 4461 7461 6261  id = QFontDataba
+00016ba0: 7365 2e61 6464 4170 706c 6963 6174 696f  se.addApplicatio
+00016bb0: 6e46 6f6e 7428 5f66 692e 6162 736f 6c75  nFont(_fi.absolu
+00016bc0: 7465 4669 6c65 5061 7468 2829 290a 2020  teFilePath()).  
+00016bd0: 2020 2020 2020 666f 6e74 5f66 616d 696c        font_famil
+00016be0: 6965 7320 7c3d 2073 6574 2851 466f 6e74  ies |= set(QFont
+00016bf0: 4461 7461 6261 7365 2e61 7070 6c69 6361  Database.applica
+00016c00: 7469 6f6e 466f 6e74 4661 6d69 6c69 6573  tionFontFamilies
+00016c10: 285f 6964 2929 0a20 2020 2072 6574 7572  (_id)).    retur
+00016c20: 6e20 666f 6e74 5f66 616d 696c 6965 730a  n font_families.
+00016c30: 0a0a 6465 6620 696e 7374 616c 6c5f 6963  ..def install_ic
+00016c40: 6f6e 7328 293a 0a20 2020 2022 2222 496e  ons():.    """In
+00016c50: 7374 616c 6c20 6963 6f6e 7322 2222 0a20  stall icons""". 
+00016c60: 2020 206f 732e 7379 7374 656d 280a 2020     os.system(.  
+00016c70: 2020 2020 2020 2278 6467 2d69 636f 6e2d        "xdg-icon-
+00016c80: 7265 736f 7572 6365 2069 6e73 7461 6c6c  resource install
+00016c90: 202d 2d73 697a 6520 3332 202d 2d63 6f6e   --size 32 --con
+00016ca0: 7465 7874 2061 7070 7320 2d2d 6d6f 6465  text apps --mode
+00016cb0: 2075 7365 7220 220a 2020 2020 2020 2020   user ".        
+00016cc0: 6622 7b57 4f52 4b49 4e47 5f50 4154 487d  f"{WORKING_PATH}
+00016cd0: 2f64 6174 612f 6b36 6774 652e 6e6f 7431  /data/k6gte.not1
+00016ce0: 6d6d 2d33 322e 706e 6720 6b36 6774 652d  mm-32.png k6gte-
+00016cf0: 6e6f 7431 6d6d 220a 2020 2020 290a 2020  not1mm".    ).  
+00016d00: 2020 6f73 2e73 7973 7465 6d28 0a20 2020    os.system(.   
+00016d10: 2020 2020 2022 7864 672d 6963 6f6e 2d72       "xdg-icon-r
+00016d20: 6573 6f75 7263 6520 696e 7374 616c 6c20  esource install 
+00016d30: 2d2d 7369 7a65 2036 3420 2d2d 636f 6e74  --size 64 --cont
+00016d40: 6578 7420 6170 7073 202d 2d6d 6f64 6520  ext apps --mode 
+00016d50: 7573 6572 2022 0a20 2020 2020 2020 2066  user ".        f
+00016d60: 227b 574f 524b 494e 475f 5041 5448 7d2f  "{WORKING_PATH}/
+00016d70: 6461 7461 2f6b 3667 7465 2e6e 6f74 316d  data/k6gte.not1m
+00016d80: 6d2d 3634 2e70 6e67 206b 3667 7465 2d6e  m-64.png k6gte-n
+00016d90: 6f74 316d 6d22 0a20 2020 2029 0a20 2020  ot1mm".    ).   
+00016da0: 206f 732e 7379 7374 656d 280a 2020 2020   os.system(.    
+00016db0: 2020 2020 2278 6467 2d69 636f 6e2d 7265      "xdg-icon-re
+00016dc0: 736f 7572 6365 2069 6e73 7461 6c6c 202d  source install -
+00016dd0: 2d73 697a 6520 3132 3820 2d2d 636f 6e74  -size 128 --cont
+00016de0: 6578 7420 6170 7073 202d 2d6d 6f64 6520  ext apps --mode 
+00016df0: 7573 6572 2022 0a20 2020 2020 2020 2066  user ".        f
+00016e00: 227b 574f 524b 494e 475f 5041 5448 7d2f  "{WORKING_PATH}/
+00016e10: 6461 7461 2f6b 3667 7465 2e6e 6f74 316d  data/k6gte.not1m
+00016e20: 6d2d 3132 382e 706e 6720 6b36 6774 652d  m-128.png k6gte-
+00016e30: 6e6f 7431 6d6d 220a 2020 2020 290a 2020  not1mm".    ).  
+00016e40: 2020 6f73 2e73 7973 7465 6d28 6622 7864    os.system(f"xd
+00016e50: 672d 6465 736b 746f 702d 6d65 6e75 2069  g-desktop-menu i
+00016e60: 6e73 7461 6c6c 207b 574f 524b 494e 475f  nstall {WORKING_
+00016e70: 5041 5448 7d2f 6461 7461 2f6b 3667 7465  PATH}/data/k6gte
+00016e80: 2d6e 6f74 316d 6d2e 6465 736b 746f 7022  -not1mm.desktop"
+00016e90: 290a 0a0a 6465 6620 646f 696d 7028 6d6f  )...def doimp(mo
+00016ea0: 646e 616d 6529 3a0a 2020 2020 2222 2272  dname):.    """r
+00016eb0: 6574 7572 6e20 6d6f 6475 6c65 2070 6174  eturn module pat
+00016ec0: 6822 2222 0a20 2020 2072 6574 7572 6e20  h""".    return 
+00016ed0: 696d 706f 7274 6c69 622e 696d 706f 7274  importlib.import
+00016ee0: 5f6d 6f64 756c 6528 6622 6e6f 7431 6d6d  _module(f"not1mm
+00016ef0: 2e70 6c75 6769 6e73 2e7b 6d6f 646e 616d  .plugins.{modnam
+00016f00: 657d 2229 0a0a 0a64 6566 2072 756e 2829  e}")...def run()
+00016f10: 3a0a 2020 2020 2222 220a 2020 2020 4d61  :.    """.    Ma
+00016f20: 696e 2045 6e74 7279 0a20 2020 2022 2222  in Entry.    """
+00016f30: 0a20 2020 2069 6e73 7461 6c6c 5f69 636f  .    install_ico
+00016f40: 6e73 2829 0a20 2020 2074 696d 6572 2e73  ns().    timer.s
+00016f50: 7461 7274 2832 3530 290a 2020 2020 7379  tart(250).    sy
+00016f60: 732e 6578 6974 2861 7070 2e65 7865 6328  s.exit(app.exec(
+00016f70: 2929 0a0a 0a6c 6f67 6765 7220 3d20 6c6f  ))...logger = lo
+00016f80: 6767 696e 672e 6765 744c 6f67 6765 7228  gging.getLogger(
+00016f90: 225f 5f6d 6169 6e5f 5f22 290a 6861 6e64  "__main__").hand
+00016fa0: 6c65 7220 3d20 6c6f 6767 696e 672e 5374  ler = logging.St
+00016fb0: 7265 616d 4861 6e64 6c65 7228 290a 666f  reamHandler().fo
+00016fc0: 726d 6174 7465 7220 3d20 6c6f 6767 696e  rmatter = loggin
+00016fd0: 672e 466f 726d 6174 7465 7228 0a20 2020  g.Formatter(.   
+00016fe0: 2064 6174 6566 6d74 3d22 2548 3a25 4d3a   datefmt="%H:%M:
+00016ff0: 2553 222c 0a20 2020 2066 6d74 3d22 5b25  %S",.    fmt="[%
+00017000: 2861 7363 7469 6d65 2973 5d20 2528 6c65  (asctime)s] %(le
+00017010: 7665 6c6e 616d 6529 7320 2528 6d6f 6475  velname)s %(modu
+00017020: 6c65 2973 202d 2025 2866 756e 634e 616d  le)s - %(funcNam
+00017030: 6529 7320 4c69 6e65 2025 286c 696e 656e  e)s Line %(linen
+00017040: 6f29 643a 2025 286d 6573 7361 6765 2973  o)d: %(message)s
+00017050: 222c 0a29 0a68 616e 646c 6572 2e73 6574  ",.).handler.set
+00017060: 466f 726d 6174 7465 7228 666f 726d 6174  Formatter(format
+00017070: 7465 7229 0a6c 6f67 6765 722e 6164 6448  ter).logger.addH
+00017080: 616e 646c 6572 2868 616e 646c 6572 290a  andler(handler).
+00017090: 0a42 4554 415f 5445 5354 203d 2046 616c  .BETA_TEST = Fal
+000170a0: 7365 0a69 6620 5061 7468 2822 2e2f 6265  se.if Path("./be
+000170b0: 7461 7465 7374 2229 2e65 7869 7374 7328  tatest").exists(
+000170c0: 293a 0a20 2020 2042 4554 415f 5445 5354  ):.    BETA_TEST
+000170d0: 203d 2054 7275 650a 0a69 6620 5061 7468   = True..if Path
+000170e0: 2822 2e2f 6465 6275 6722 292e 6578 6973  ("./debug").exis
+000170f0: 7473 2829 3a0a 2020 2020 6c6f 6767 6572  ts():.    logger
+00017100: 2e73 6574 4c65 7665 6c28 6c6f 6767 696e  .setLevel(loggin
+00017110: 672e 4445 4255 4729 0a20 2020 206c 6f67  g.DEBUG).    log
+00017120: 6765 722e 6465 6275 6728 2264 6562 7567  ger.debug("debug
+00017130: 6769 6e67 206f 6e22 290a 656c 7365 3a0a  ging on").else:.
+00017140: 2020 2020 6c6f 6767 6572 2e73 6574 4c65      logger.setLe
+00017150: 7665 6c28 6c6f 6767 696e 672e 5741 524e  vel(logging.WARN
+00017160: 494e 4729 0a20 2020 206c 6f67 6765 722e  ING).    logger.
+00017170: 7761 726e 696e 6728 2264 6562 7567 6769  warning("debuggi
+00017180: 6e67 206f 6666 2229 0a0a 6170 7020 3d20  ng off")..app = 
+00017190: 5174 5769 6467 6574 732e 5141 7070 6c69  QtWidgets.QAppli
+000171a0: 6361 7469 6f6e 2873 7973 2e61 7267 7629  cation(sys.argv)
+000171b0: 0a61 7070 2e73 6574 5374 796c 6528 2241  .app.setStyle("A
+000171c0: 6477 6169 7461 2d44 6172 6b22 290a 666f  dwaita-Dark").fo
+000171d0: 6e74 5f70 6174 6820 3d20 574f 524b 494e  nt_path = WORKIN
+000171e0: 475f 5041 5448 202b 2022 2f64 6174 6122  G_PATH + "/data"
+000171f0: 0a66 616d 696c 6965 7320 3d20 6c6f 6164  .families = load
+00017200: 5f66 6f6e 7473 5f66 726f 6d5f 6469 7228  _fonts_from_dir(
+00017210: 6f73 2e66 7370 6174 6828 666f 6e74 5f70  os.fspath(font_p
+00017220: 6174 6829 290a 6c6f 6767 6572 2e69 6e66  ath)).logger.inf
+00017230: 6f28 6661 6d69 6c69 6573 290a 7769 6e64  o(families).wind
+00017240: 6f77 203d 204d 6169 6e57 696e 646f 7728  ow = MainWindow(
+00017250: 290a 6865 6967 6874 203d 2077 696e 646f  ).height = windo
+00017260: 772e 7072 6566 2e67 6574 2822 7769 6e64  w.pref.get("wind
+00017270: 6f77 5f68 6569 6768 7422 2c20 3330 3029  ow_height", 300)
+00017280: 0a77 6964 7468 203d 2077 696e 646f 772e  .width = window.
+00017290: 7072 6566 2e67 6574 2822 7769 6e64 6f77  pref.get("window
+000172a0: 5f77 6964 7468 222c 2037 3030 290a 7820  _width", 700).x 
+000172b0: 3d20 7769 6e64 6f77 2e70 7265 662e 6765  = window.pref.ge
+000172c0: 7428 2277 696e 646f 775f 7822 2c20 2d31  t("window_x", -1
+000172d0: 290a 7920 3d20 7769 6e64 6f77 2e70 7265  ).y = window.pre
+000172e0: 662e 6765 7428 2277 696e 646f 775f 7922  f.get("window_y"
+000172f0: 2c20 2d31 290a 7769 6e64 6f77 2e73 6574  , -1).window.set
+00017300: 4765 6f6d 6574 7279 2878 2c20 792c 2077  Geometry(x, y, w
+00017310: 6964 7468 2c20 6865 6967 6874 290a 7769  idth, height).wi
+00017320: 6e64 6f77 2e63 616c 6c73 6967 6e2e 7365  ndow.callsign.se
+00017330: 7446 6f63 7573 2829 0a77 696e 646f 772e  tFocus().window.
+00017340: 7368 6f77 2829 0a74 696d 6572 203d 2051  show().timer = Q
+00017350: 7443 6f72 652e 5154 696d 6572 2829 0a74  tCore.QTimer().t
+00017360: 696d 6572 2e74 696d 656f 7574 2e63 6f6e  imer.timeout.con
+00017370: 6e65 6374 2877 696e 646f 772e 706f 6c6c  nect(window.poll
+00017380: 5f72 6164 696f 290a 0a69 6620 5f5f 6e61  _radio)..if __na
+00017390: 6d65 5f5f 203d 3d20 225f 5f6d 6169 6e5f  me__ == "__main_
+000173a0: 5f22 3a0a 2020 2020 7275 6e28 290a       _":.    run().
```

### Comparing `not1mm-23.6.21.1/not1mm/bandmap.py` & `not1mm-23.6.22/not1mm/bandmap.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/data/JetBrainsMono-Regular.ttf` & `not1mm-23.6.22/not1mm/data/JetBrainsMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/data/MASTER.SCP` & `not1mm-23.6.22/not1mm/data/MASTER.SCP`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/data/about.ui` & `not1mm-23.6.22/not1mm/data/about.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/data/bandmap.ui` & `not1mm-23.6.22/not1mm/data/bandmap.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/data/configuration.ui` & `not1mm-23.6.22/not1mm/data/configuration.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/data/contests.sql` & `not1mm-23.6.22/not1mm/data/contests.sql`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/data/cty.json` & `not1mm-23.6.22/not1mm/data/cty.json`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/data/editcontact.ui` & `not1mm-23.6.22/not1mm/data/editcontact.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/data/editmacro.ui` & `not1mm-23.6.22/not1mm/data/editmacro.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/data/k6gte.not1mm-128.png` & `not1mm-23.6.22/not1mm/data/k6gte.not1mm-128.png`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/data/k6gte.not1mm-32.png` & `not1mm-23.6.22/not1mm/data/k6gte.not1mm-32.png`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/data/k6gte.not1mm-64.png` & `not1mm-23.6.22/not1mm/data/k6gte.not1mm-64.png`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/data/logwindow.ui` & `not1mm-23.6.22/not1mm/data/logwindow.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/data/main.ui` & `not1mm-23.6.22/not1mm/data/main.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/data/new_contest.ui` & `not1mm-23.6.22/not1mm/data/new_contest.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/data/not1mm.html` & `not1mm-23.6.22/not1mm/data/not1mm.html`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/data/opon.ui` & `not1mm-23.6.22/not1mm/data/opon.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/data/phonetics/0.wav` & `not1mm-23.6.22/not1mm/data/phonetics/0.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/data/phonetics/1.wav` & `not1mm-23.6.22/not1mm/data/phonetics/1.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/data/phonetics/2.wav` & `not1mm-23.6.22/not1mm/data/phonetics/2.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/data/phonetics/3.wav` & `not1mm-23.6.22/not1mm/data/phonetics/3.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/data/phonetics/4.wav` & `not1mm-23.6.22/not1mm/data/phonetics/4.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/data/phonetics/5.wav` & `not1mm-23.6.22/not1mm/data/phonetics/5.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/data/phonetics/6.wav` & `not1mm-23.6.22/not1mm/data/phonetics/6.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/data/phonetics/7.wav` & `not1mm-23.6.22/not1mm/data/phonetics/7.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/data/phonetics/73.wav` & `not1mm-23.6.22/not1mm/data/phonetics/73.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/data/phonetics/8.wav` & `not1mm-23.6.22/not1mm/data/phonetics/8.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/data/phonetics/9.wav` & `not1mm-23.6.22/not1mm/data/phonetics/9.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/data/phonetics/a.wav` & `not1mm-23.6.22/not1mm/data/phonetics/a.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/data/phonetics/again.wav` & `not1mm-23.6.22/not1mm/data/phonetics/again.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/data/phonetics/b.wav` & `not1mm-23.6.22/not1mm/data/phonetics/b.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/data/phonetics/c.wav` & `not1mm-23.6.22/not1mm/data/phonetics/c.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/data/phonetics/contest.wav` & `not1mm-23.6.22/not1mm/data/phonetics/contest.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/data/phonetics/cq.wav` & `not1mm-23.6.22/not1mm/data/phonetics/cq.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/data/phonetics/d.wav` & `not1mm-23.6.22/not1mm/data/phonetics/d.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/data/phonetics/e.wav` & `not1mm-23.6.22/not1mm/data/phonetics/e.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/data/phonetics/f.wav` & `not1mm-23.6.22/not1mm/data/phonetics/f.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/data/phonetics/g.wav` & `not1mm-23.6.22/not1mm/data/phonetics/g.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/data/phonetics/h.wav` & `not1mm-23.6.22/not1mm/data/phonetics/h.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/data/phonetics/i.wav` & `not1mm-23.6.22/not1mm/data/phonetics/i.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/data/phonetics/j.wav` & `not1mm-23.6.22/not1mm/data/phonetics/j.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/data/phonetics/k.wav` & `not1mm-23.6.22/not1mm/data/phonetics/k.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/data/phonetics/k6gte.wav` & `not1mm-23.6.22/not1mm/data/phonetics/k6gte.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/data/phonetics/l.wav` & `not1mm-23.6.22/not1mm/data/phonetics/l.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/data/phonetics/m.wav` & `not1mm-23.6.22/not1mm/data/phonetics/m.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/data/phonetics/mynumber.wav` & `not1mm-23.6.22/not1mm/data/phonetics/mynumber.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/data/phonetics/n.wav` & `not1mm-23.6.22/not1mm/data/phonetics/n.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/data/phonetics/nil.wav` & `not1mm-23.6.22/not1mm/data/phonetics/nil.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/data/phonetics/o.wav` & `not1mm-23.6.22/not1mm/data/phonetics/o.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/data/phonetics/p.wav` & `not1mm-23.6.22/not1mm/data/phonetics/p.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/data/phonetics/q.wav` & `not1mm-23.6.22/not1mm/data/phonetics/q.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/data/phonetics/r.wav` & `not1mm-23.6.22/not1mm/data/phonetics/r.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/data/phonetics/roger.wav` & `not1mm-23.6.22/not1mm/data/phonetics/roger.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/data/phonetics/s.wav` & `not1mm-23.6.22/not1mm/data/phonetics/s.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/data/phonetics/space.wav` & `not1mm-23.6.22/not1mm/data/phonetics/space.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/data/phonetics/t.wav` & `not1mm-23.6.22/not1mm/data/phonetics/t.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/data/phonetics/thankyou.wav` & `not1mm-23.6.22/not1mm/data/phonetics/thankyou.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/data/phonetics/thankyouqrz.wav` & `not1mm-23.6.22/not1mm/data/phonetics/thankyouqrz.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/data/phonetics/u.wav` & `not1mm-23.6.22/not1mm/data/phonetics/u.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/data/phonetics/v.wav` & `not1mm-23.6.22/not1mm/data/phonetics/v.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/data/phonetics/w.wav` & `not1mm-23.6.22/not1mm/data/phonetics/w.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/data/phonetics/x.wav` & `not1mm-23.6.22/not1mm/data/phonetics/x.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/data/phonetics/y.wav` & `not1mm-23.6.22/not1mm/data/phonetics/y.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/data/phonetics/yourcall.wav` & `not1mm-23.6.22/not1mm/data/phonetics/yourcall.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/data/phonetics/z.wav` & `not1mm-23.6.22/not1mm/data/phonetics/z.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/data/pickcontest.ui` & `not1mm-23.6.22/not1mm/data/pickcontest.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/data/reddot.png` & `not1mm-23.6.22/not1mm/data/reddot.png`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/data/settings.ui` & `not1mm-23.6.22/not1mm/data/settings.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/lib/cat_interface.py` & `not1mm-23.6.22/not1mm/lib/cat_interface.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/lib/cwinterface.py` & `not1mm-23.6.22/not1mm/lib/cwinterface.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/lib/database.py` & `not1mm-23.6.22/not1mm/lib/database.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/lib/edit_macro.py` & `not1mm-23.6.22/not1mm/lib/edit_macro.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/lib/edit_station.py` & `not1mm-23.6.22/not1mm/lib/edit_station.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/lib/ham_utility.py` & `not1mm-23.6.22/not1mm/lib/ham_utility.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/lib/lookup.py` & `not1mm-23.6.22/not1mm/lib/lookup.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/lib/multicast.py` & `not1mm-23.6.22/not1mm/lib/multicast.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/lib/n1mm.py` & `not1mm-23.6.22/not1mm/lib/n1mm.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/lib/settings.py` & `not1mm-23.6.22/not1mm/lib/settings.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/lib/versiontest.py` & `not1mm-23.6.22/not1mm/lib/versiontest.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/logwindow.py` & `not1mm-23.6.22/not1mm/logwindow.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/plugins/10_10_fall_cw.py` & `not1mm-23.6.22/not1mm/plugins/10_10_fall_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/plugins/10_10_spring_cw.py` & `not1mm-23.6.22/not1mm/plugins/10_10_spring_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/plugins/10_10_summer_phone.py` & `not1mm-23.6.22/not1mm/plugins/10_10_summer_phone.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/plugins/10_10_winter_phone.py` & `not1mm-23.6.22/not1mm/plugins/10_10_winter_phone.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/plugins/arrl_dx_cw.py` & `not1mm-23.6.22/not1mm/plugins/arrl_dx_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/plugins/arrl_dx_ssb.py` & `not1mm-23.6.22/not1mm/plugins/arrl_dx_ssb.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/plugins/arrl_field_day.py` & `not1mm-23.6.22/not1mm/plugins/arrl_field_day.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/plugins/arrl_rtty_ru.py` & `not1mm-23.6.22/not1mm/plugins/arrl_rtty_ru.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/plugins/arrl_ss_cw.py` & `not1mm-23.6.22/not1mm/plugins/arrl_ss_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/plugins/arrl_ss_phone.py` & `not1mm-23.6.22/not1mm/plugins/arrl_ss_phone.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/plugins/cq_wpx_cw.py` & `not1mm-23.6.22/not1mm/plugins/cq_wpx_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/plugins/cq_wpx_ssb.py` & `not1mm-23.6.22/not1mm/plugins/cq_wpx_ssb.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/plugins/cq_ww_cw.py` & `not1mm-23.6.22/not1mm/plugins/cq_ww_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/plugins/cq_ww_ssb.py` & `not1mm-23.6.22/not1mm/plugins/cq_ww_ssb.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/plugins/cwt.py` & `not1mm-23.6.22/not1mm/plugins/cwt.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/plugins/general_logging.py` & `not1mm-23.6.22/not1mm/plugins/general_logging.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/plugins/jidx_cw.py` & `not1mm-23.6.22/not1mm/plugins/jidx_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/plugins/jidx_ph.py` & `not1mm-23.6.22/not1mm/plugins/jidx_ph.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/plugins/winter_field_day.py` & `not1mm-23.6.22/not1mm/plugins/winter_field_day.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/testing/fakeflrig.py` & `not1mm-23.6.22/not1mm/testing/fakeflrig.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/testing/flrigclient.py` & `not1mm-23.6.22/not1mm/testing/flrigclient.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/testing/n1mm_listener.py` & `not1mm-23.6.22/not1mm/testing/n1mm_listener.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm/testing/test.py` & `not1mm-23.6.22/not1mm/testing/test.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/not1mm.egg-info/PKG-INFO` & `not1mm-23.6.22/not1mm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: not1mm
-Version: 23.6.21.1
+Version: 23.6.22
 Summary: NOT1MM Logger
 Author-email: Michael Bridak <michael.bridak@gmail.com>
 Project-URL: Homepage, https://github.com/mbridak/not1mm
 Project-URL: Bug Tracker, https://github.com/mbridak/not1mm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `not1mm-23.6.21.1/not1mm.egg-info/SOURCES.txt` & `not1mm-23.6.22/not1mm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `not1mm-23.6.21.1/pyproject.toml` & `not1mm-23.6.22/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "not1mm" 
-version = "23.6.21.1"
+version = "23.6.22"
 description = "NOT1MM Logger"
 readme = "README.md"
 requires-python = ">=3.9"
 authors = [
   { name="Michael Bridak", email="michael.bridak@gmail.com" },
 ]
 dependencies = [
```

