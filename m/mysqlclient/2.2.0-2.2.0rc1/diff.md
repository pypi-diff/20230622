# Comparing `tmp/mysqlclient-2.2.0.tar.gz` & `tmp/mysqlclient-2.2.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mysqlclient-2.2.0.tar", last modified: Thu Jun 22 05:58:44 2023, max compression
+gzip compressed data, was "mysqlclient-2.2.0rc1.tar", last modified: Fri May 19 04:58:30 2023, max compression
```

## Comparing `mysqlclient-2.2.0.tar` & `mysqlclient-2.2.0rc1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 05:58:44.912430 mysqlclient-2.2.0/
--rw-rw-rw-   0        0        0    16550 2023-06-22 05:52:35.000000 mysqlclient-2.2.0/HISTORY.rst
--rw-rw-rw-   0        0        0    18431 2023-06-22 05:52:35.000000 mysqlclient-2.2.0/LICENSE
--rw-rw-rw-   0        0        0      155 2023-06-22 05:52:35.000000 mysqlclient-2.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0     4520 2023-06-22 05:58:44.912430 mysqlclient-2.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     3192 2023-06-22 05:52:35.000000 mysqlclient-2.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-22 05:58:44.896800 mysqlclient-2.2.0/doc/
--rw-rw-rw-   0        0        0     5073 2023-06-22 05:52:35.000000 mysqlclient-2.2.0/doc/FAQ.rst
--rw-rw-rw-   0        0        0      921 2023-06-22 05:52:35.000000 mysqlclient-2.2.0/doc/MySQLdb.constants.rst
--rw-rw-rw-   0        0        0     1113 2023-06-22 05:52:35.000000 mysqlclient-2.2.0/doc/MySQLdb.rst
--rw-rw-rw-   0        0        0     8265 2023-06-22 05:52:35.000000 mysqlclient-2.2.0/doc/conf.py
--rw-rw-rw-   0        0        0      262 2023-06-22 05:52:35.000000 mysqlclient-2.2.0/doc/index.rst
--rw-rw-rw-   0        0        0    30369 2023-06-22 05:52:35.000000 mysqlclient-2.2.0/doc/user_guide.rst
--rw-rw-rw-   0        0        0     1602 2023-06-22 05:52:35.000000 mysqlclient-2.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-22 05:58:44.912430 mysqlclient-2.2.0/setup.cfg
--rw-rw-rw-   0        0        0     4525 2023-06-22 05:52:35.000000 mysqlclient-2.2.0/setup.py
--rw-rw-rw-   0        0        0       57 2023-06-22 05:52:35.000000 mysqlclient-2.2.0/site.cfg
-drwxrwxrwx   0        0        0        0 2023-06-22 05:58:44.896800 mysqlclient-2.2.0/src/
-drwxrwxrwx   0        0        0        0 2023-06-22 05:58:44.912430 mysqlclient-2.2.0/src/MySQLdb/
--rw-rw-rw-   0        0        0     3561 2023-06-22 05:52:35.000000 mysqlclient-2.2.0/src/MySQLdb/__init__.py
--rw-rw-rw-   0        0        0     2563 2023-06-22 05:52:35.000000 mysqlclient-2.2.0/src/MySQLdb/_exceptions.py
--rw-rw-rw-   0        0        0    85616 2023-06-22 05:52:35.000000 mysqlclient-2.2.0/src/MySQLdb/_mysql.c
--rw-rw-rw-   0        0        0    11988 2023-06-22 05:52:35.000000 mysqlclient-2.2.0/src/MySQLdb/connections.py
-drwxrwxrwx   0        0        0        0 2023-06-22 05:58:44.912430 mysqlclient-2.2.0/src/MySQLdb/constants/
--rw-rw-rw-   0        0        0      693 2023-06-22 05:52:35.000000 mysqlclient-2.2.0/src/MySQLdb/constants/CLIENT.py
--rw-rw-rw-   0        0        0     2923 2023-06-22 05:52:35.000000 mysqlclient-2.2.0/src/MySQLdb/constants/CR.py
--rw-rw-rw-   0        0        0    25705 2023-06-22 05:52:35.000000 mysqlclient-2.2.0/src/MySQLdb/constants/ER.py
--rw-rw-rw-   0        0        0      606 2023-06-22 05:52:35.000000 mysqlclient-2.2.0/src/MySQLdb/constants/FIELD_TYPE.py
--rw-rw-rw-   0        0        0      386 2023-06-22 05:52:35.000000 mysqlclient-2.2.0/src/MySQLdb/constants/FLAG.py
--rw-rw-rw-   0        0        0       56 2023-06-22 05:52:35.000000 mysqlclient-2.2.0/src/MySQLdb/constants/__init__.py
--rw-rw-rw-   0        0        0     3591 2023-06-22 05:52:35.000000 mysqlclient-2.2.0/src/MySQLdb/converters.py
--rw-rw-rw-   0        0        0    16338 2023-06-22 05:52:35.000000 mysqlclient-2.2.0/src/MySQLdb/cursors.py
--rw-rw-rw-   0        0        0      114 2023-06-22 05:52:35.000000 mysqlclient-2.2.0/src/MySQLdb/release.py
--rw-rw-rw-   0        0        0     3754 2023-06-22 05:52:35.000000 mysqlclient-2.2.0/src/MySQLdb/times.py
-drwxrwxrwx   0        0        0        0 2023-06-22 05:58:44.912430 mysqlclient-2.2.0/src/mysqlclient.egg-info/
--rw-rw-rw-   0        0        0     4520 2023-06-22 05:58:44.000000 mysqlclient-2.2.0/src/mysqlclient.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1002 2023-06-22 05:58:44.000000 mysqlclient-2.2.0/src/mysqlclient.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 05:58:44.000000 mysqlclient-2.2.0/src/mysqlclient.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-06-22 05:58:44.000000 mysqlclient-2.2.0/src/mysqlclient.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-22 05:58:44.912430 mysqlclient-2.2.0/tests/
--rw-rw-rw-   0        0        0    10361 2023-06-22 05:52:35.000000 mysqlclient-2.2.0/tests/capabilities.py
--rw-rw-rw-   0        0        0      602 2023-06-22 05:52:35.000000 mysqlclient-2.2.0/tests/configdb.py
--rw-rw-rw-   0        0        0    32361 2023-06-22 05:52:35.000000 mysqlclient-2.2.0/tests/dbapi20.py
--rw-rw-rw-   0        0        0     6482 2023-06-22 05:52:35.000000 mysqlclient-2.2.0/tests/test_MySQLdb_capabilities.py
--rw-rw-rw-   0        0        0     8327 2023-06-22 05:52:35.000000 mysqlclient-2.2.0/tests/test_MySQLdb_dbapi20.py
--rw-rw-rw-   0        0        0     4418 2023-06-22 05:52:35.000000 mysqlclient-2.2.0/tests/test_MySQLdb_nonstandard.py
--rw-rw-rw-   0        0        0     6106 2023-06-22 05:52:35.000000 mysqlclient-2.2.0/tests/test_MySQLdb_times.py
--rw-rw-rw-   0        0        0      139 2023-06-22 05:52:35.000000 mysqlclient-2.2.0/tests/test__mysql.py
--rw-rw-rw-   0        0        0      631 2023-06-22 05:52:35.000000 mysqlclient-2.2.0/tests/test_connection.py
--rw-rw-rw-   0        0        0     7352 2023-06-22 05:52:35.000000 mysqlclient-2.2.0/tests/test_cursor.py
--rw-rw-rw-   0        0        0     1438 2023-06-22 05:52:35.000000 mysqlclient-2.2.0/tests/test_errors.py
+drwxr-xr-x   0 inada-n    (502) staff       (20)        0 2023-05-19 04:58:30.366335 mysqlclient-2.2.0rc1/
+-rw-r--r--   0 inada-n    (502) staff       (20)    15952 2023-05-19 04:35:28.000000 mysqlclient-2.2.0rc1/HISTORY.rst
+-rw-r--r--   0 inada-n    (502) staff       (20)    18092 2010-03-23 23:34:05.000000 mysqlclient-2.2.0rc1/LICENSE
+-rw-r--r--   0 inada-n    (502) staff       (20)      148 2023-05-15 06:20:49.000000 mysqlclient-2.2.0rc1/MANIFEST.in
+-rw-r--r--   0 inada-n    (502) staff       (20)     4393 2023-05-19 04:58:30.366198 mysqlclient-2.2.0rc1/PKG-INFO
+-rw-r--r--   0 inada-n    (502) staff       (20)     3093 2023-05-18 12:51:09.000000 mysqlclient-2.2.0rc1/README.md
+drwxr-xr-x   0 inada-n    (502) staff       (20)        0 2023-05-19 04:58:30.360628 mysqlclient-2.2.0rc1/doc/
+-rw-r--r--   0 inada-n    (502) staff       (20)     4937 2018-12-10 09:24:35.000000 mysqlclient-2.2.0rc1/doc/FAQ.rst
+-rw-r--r--   0 inada-n    (502) staff       (20)      871 2020-07-02 03:56:48.000000 mysqlclient-2.2.0rc1/doc/MySQLdb.constants.rst
+-rw-r--r--   0 inada-n    (502) staff       (20)     1051 2023-05-17 01:59:25.000000 mysqlclient-2.2.0rc1/doc/MySQLdb.rst
+-rw-r--r--   0 inada-n    (502) staff       (20)     8014 2023-05-17 01:59:25.000000 mysqlclient-2.2.0rc1/doc/conf.py
+-rw-r--r--   0 inada-n    (502) staff       (20)      243 2015-12-13 14:19:20.000000 mysqlclient-2.2.0rc1/doc/index.rst
+-rw-r--r--   0 inada-n    (502) staff       (20)    29657 2023-05-15 06:20:49.000000 mysqlclient-2.2.0rc1/doc/user_guide.rst
+-rw-r--r--   0 inada-n    (502) staff       (20)     1551 2023-05-16 04:11:10.000000 mysqlclient-2.2.0rc1/pyproject.toml
+-rw-r--r--   0 inada-n    (502) staff       (20)       38 2023-05-19 04:58:30.366380 mysqlclient-2.2.0rc1/setup.cfg
+-rw-r--r--   0 inada-n    (502) staff       (20)     4456 2023-05-16 04:11:10.000000 mysqlclient-2.2.0rc1/setup.py
+-rw-r--r--   0 inada-n    (502) staff       (20)      275 2023-05-15 06:20:49.000000 mysqlclient-2.2.0rc1/site.cfg
+drwxr-xr-x   0 inada-n    (502) staff       (20)        0 2023-05-19 04:58:30.357443 mysqlclient-2.2.0rc1/src/
+drwxr-xr-x   0 inada-n    (502) staff       (20)        0 2023-05-19 04:58:30.362454 mysqlclient-2.2.0rc1/src/MySQLdb/
+-rw-r--r--   0 inada-n    (502) staff       (20)     3393 2023-05-16 04:11:10.000000 mysqlclient-2.2.0rc1/src/MySQLdb/__init__.py
+-rw-r--r--   0 inada-n    (502) staff       (20)     2472 2023-05-16 04:11:10.000000 mysqlclient-2.2.0rc1/src/MySQLdb/_exceptions.py
+-rw-r--r--   0 inada-n    (502) staff       (20)    82709 2023-05-19 03:57:37.000000 mysqlclient-2.2.0rc1/src/MySQLdb/_mysql.c
+-rw-r--r--   0 inada-n    (502) staff       (20)    11651 2023-05-16 04:11:10.000000 mysqlclient-2.2.0rc1/src/MySQLdb/connections.py
+drwxr-xr-x   0 inada-n    (502) staff       (20)        0 2023-05-19 04:58:30.363295 mysqlclient-2.2.0rc1/src/MySQLdb/constants/
+-rw-r--r--   0 inada-n    (502) staff       (20)      666 2023-05-16 04:11:10.000000 mysqlclient-2.2.0rc1/src/MySQLdb/constants/CLIENT.py
+-rw-r--r--   0 inada-n    (502) staff       (20)     2818 2023-05-16 04:11:10.000000 mysqlclient-2.2.0rc1/src/MySQLdb/constants/CR.py
+-rw-r--r--   0 inada-n    (502) staff       (20)    24878 2023-05-16 04:11:10.000000 mysqlclient-2.2.0rc1/src/MySQLdb/constants/ER.py
+-rw-r--r--   0 inada-n    (502) staff       (20)      566 2023-05-16 04:11:10.000000 mysqlclient-2.2.0rc1/src/MySQLdb/constants/FIELD_TYPE.py
+-rw-r--r--   0 inada-n    (502) staff       (20)      363 2023-05-16 04:11:10.000000 mysqlclient-2.2.0rc1/src/MySQLdb/constants/FLAG.py
+-rw-r--r--   0 inada-n    (502) staff       (20)       55 2023-05-16 04:11:10.000000 mysqlclient-2.2.0rc1/src/MySQLdb/constants/__init__.py
+-rw-r--r--   0 inada-n    (502) staff       (20)     3452 2023-05-16 04:11:10.000000 mysqlclient-2.2.0rc1/src/MySQLdb/converters.py
+-rw-r--r--   0 inada-n    (502) staff       (20)    15838 2023-05-18 17:06:53.000000 mysqlclient-2.2.0rc1/src/MySQLdb/cursors.py
+-rw-r--r--   0 inada-n    (502) staff       (20)      112 2023-05-19 04:35:28.000000 mysqlclient-2.2.0rc1/src/MySQLdb/release.py
+-rw-r--r--   0 inada-n    (502) staff       (20)     3604 2023-05-16 04:11:10.000000 mysqlclient-2.2.0rc1/src/MySQLdb/times.py
+drwxr-xr-x   0 inada-n    (502) staff       (20)        0 2023-05-19 04:58:30.363750 mysqlclient-2.2.0rc1/src/mysqlclient.egg-info/
+-rw-r--r--   0 inada-n    (502) staff       (20)     4393 2023-05-19 04:58:30.000000 mysqlclient-2.2.0rc1/src/mysqlclient.egg-info/PKG-INFO
+-rw-r--r--   0 inada-n    (502) staff       (20)      981 2023-05-19 04:58:30.000000 mysqlclient-2.2.0rc1/src/mysqlclient.egg-info/SOURCES.txt
+-rw-r--r--   0 inada-n    (502) staff       (20)        1 2023-05-19 04:58:30.000000 mysqlclient-2.2.0rc1/src/mysqlclient.egg-info/dependency_links.txt
+-rw-r--r--   0 inada-n    (502) staff       (20)        8 2023-05-19 04:58:30.000000 mysqlclient-2.2.0rc1/src/mysqlclient.egg-info/top_level.txt
+drwxr-xr-x   0 inada-n    (502) staff       (20)        0 2023-05-19 04:58:30.365881 mysqlclient-2.2.0rc1/tests/
+-rw-r--r--   0 inada-n    (502) staff       (20)    10047 2023-05-15 06:20:49.000000 mysqlclient-2.2.0rc1/tests/capabilities.py
+-rw-r--r--   0 inada-n    (502) staff       (20)      577 2020-12-04 03:22:51.000000 mysqlclient-2.2.0rc1/tests/configdb.py
+-rw-r--r--   0 inada-n    (502) staff       (20)    31502 2023-05-15 06:20:49.000000 mysqlclient-2.2.0rc1/tests/dbapi20.py
+-rw-r--r--   0 inada-n    (502) staff       (20)     6277 2023-05-15 06:20:49.000000 mysqlclient-2.2.0rc1/tests/test_MySQLdb_capabilities.py
+-rw-r--r--   0 inada-n    (502) staff       (20)     8096 2020-12-04 03:22:51.000000 mysqlclient-2.2.0rc1/tests/test_MySQLdb_dbapi20.py
+-rw-r--r--   0 inada-n    (502) staff       (20)     4272 2023-05-15 06:20:49.000000 mysqlclient-2.2.0rc1/tests/test_MySQLdb_nonstandard.py
+-rw-r--r--   0 inada-n    (502) staff       (20)     5960 2021-01-08 07:30:30.000000 mysqlclient-2.2.0rc1/tests/test_MySQLdb_times.py
+-rw-r--r--   0 inada-n    (502) staff       (20)      132 2018-12-10 09:24:35.000000 mysqlclient-2.2.0rc1/tests/test__mysql.py
+-rw-r--r--   0 inada-n    (502) staff       (20)      605 2023-05-15 06:20:49.000000 mysqlclient-2.2.0rc1/tests/test_connection.py
+-rw-r--r--   0 inada-n    (502) staff       (20)     7107 2023-05-18 08:59:02.000000 mysqlclient-2.2.0rc1/tests/test_cursor.py
+-rw-r--r--   0 inada-n    (502) staff       (20)     1382 2023-05-15 06:20:49.000000 mysqlclient-2.2.0rc1/tests/test_errors.py
```

### Comparing `mysqlclient-2.2.0/LICENSE` & `mysqlclient-2.2.0rc1/LICENSE`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -1,339 +1,339 @@
-                    GNU GENERAL PUBLIC LICENSE
-                       Version 2, June 1991
-
- Copyright (C) 1989, 1991 Free Software Foundation, Inc.,
- 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
- Everyone is permitted to copy and distribute verbatim copies
- of this license document, but changing it is not allowed.
-
-                            Preamble
-
-  The licenses for most software are designed to take away your
-freedom to share and change it.  By contrast, the GNU General Public
-License is intended to guarantee your freedom to share and change free
-software--to make sure the software is free for all its users.  This
-General Public License applies to most of the Free Software
-Foundation's software and to any other program whose authors commit to
-using it.  (Some other Free Software Foundation software is covered by
-the GNU Lesser General Public License instead.)  You can apply it to
-your programs, too.
-
-  When we speak of free software, we are referring to freedom, not
-price.  Our General Public Licenses are designed to make sure that you
-have the freedom to distribute copies of free software (and charge for
-this service if you wish), that you receive source code or can get it
-if you want it, that you can change the software or use pieces of it
-in new free programs; and that you know you can do these things.
-
-  To protect your rights, we need to make restrictions that forbid
-anyone to deny you these rights or to ask you to surrender the rights.
-These restrictions translate to certain responsibilities for you if you
-distribute copies of the software, or if you modify it.
-
-  For example, if you distribute copies of such a program, whether
-gratis or for a fee, you must give the recipients all the rights that
-you have.  You must make sure that they, too, receive or can get the
-source code.  And you must show them these terms so they know their
-rights.
-
-  We protect your rights with two steps: (1) copyright the software, and
-(2) offer you this license which gives you legal permission to copy,
-distribute and/or modify the software.
-
-  Also, for each author's protection and ours, we want to make certain
-that everyone understands that there is no warranty for this free
-software.  If the software is modified by someone else and passed on, we
-want its recipients to know that what they have is not the original, so
-that any problems introduced by others will not reflect on the original
-authors' reputations.
-
-  Finally, any free program is threatened constantly by software
-patents.  We wish to avoid the danger that redistributors of a free
-program will individually obtain patent licenses, in effect making the
-program proprietary.  To prevent this, we have made it clear that any
-patent must be licensed for everyone's free use or not licensed at all.
-
-  The precise terms and conditions for copying, distribution and
-modification follow.
-
-                    GNU GENERAL PUBLIC LICENSE
-   TERMS AND CONDITIONS FOR COPYING, DISTRIBUTION AND MODIFICATION
-
-  0. This License applies to any program or other work which contains
-a notice placed by the copyright holder saying it may be distributed
-under the terms of this General Public License.  The "Program", below,
-refers to any such program or work, and a "work based on the Program"
-means either the Program or any derivative work under copyright law:
-that is to say, a work containing the Program or a portion of it,
-either verbatim or with modifications and/or translated into another
-language.  (Hereinafter, translation is included without limitation in
-the term "modification".)  Each licensee is addressed as "you".
-
-Activities other than copying, distribution and modification are not
-covered by this License; they are outside its scope.  The act of
-running the Program is not restricted, and the output from the Program
-is covered only if its contents constitute a work based on the
-Program (independent of having been made by running the Program).
-Whether that is true depends on what the Program does.
-
-  1. You may copy and distribute verbatim copies of the Program's
-source code as you receive it, in any medium, provided that you
-conspicuously and appropriately publish on each copy an appropriate
-copyright notice and disclaimer of warranty; keep intact all the
-notices that refer to this License and to the absence of any warranty;
-and give any other recipients of the Program a copy of this License
-along with the Program.
-
-You may charge a fee for the physical act of transferring a copy, and
-you may at your option offer warranty protection in exchange for a fee.
-
-  2. You may modify your copy or copies of the Program or any portion
-of it, thus forming a work based on the Program, and copy and
-distribute such modifications or work under the terms of Section 1
-above, provided that you also meet all of these conditions:
-
-    a) You must cause the modified files to carry prominent notices
-    stating that you changed the files and the date of any change.
-
-    b) You must cause any work that you distribute or publish, that in
-    whole or in part contains or is derived from the Program or any
-    part thereof, to be licensed as a whole at no charge to all third
-    parties under the terms of this License.
-
-    c) If the modified program normally reads commands interactively
-    when run, you must cause it, when started running for such
-    interactive use in the most ordinary way, to print or display an
-    announcement including an appropriate copyright notice and a
-    notice that there is no warranty (or else, saying that you provide
-    a warranty) and that users may redistribute the program under
-    these conditions, and telling the user how to view a copy of this
-    License.  (Exception: if the Program itself is interactive but
-    does not normally print such an announcement, your work based on
-    the Program is not required to print an announcement.)
-
-These requirements apply to the modified work as a whole.  If
-identifiable sections of that work are not derived from the Program,
-and can be reasonably considered independent and separate works in
-themselves, then this License, and its terms, do not apply to those
-sections when you distribute them as separate works.  But when you
-distribute the same sections as part of a whole which is a work based
-on the Program, the distribution of the whole must be on the terms of
-this License, whose permissions for other licensees extend to the
-entire whole, and thus to each and every part regardless of who wrote it.
-
-Thus, it is not the intent of this section to claim rights or contest
-your rights to work written entirely by you; rather, the intent is to
-exercise the right to control the distribution of derivative or
-collective works based on the Program.
-
-In addition, mere aggregation of another work not based on the Program
-with the Program (or with a work based on the Program) on a volume of
-a storage or distribution medium does not bring the other work under
-the scope of this License.
-
-  3. You may copy and distribute the Program (or a work based on it,
-under Section 2) in object code or executable form under the terms of
-Sections 1 and 2 above provided that you also do one of the following:
-
-    a) Accompany it with the complete corresponding machine-readable
-    source code, which must be distributed under the terms of Sections
-    1 and 2 above on a medium customarily used for software interchange; or,
-
-    b) Accompany it with a written offer, valid for at least three
-    years, to give any third party, for a charge no more than your
-    cost of physically performing source distribution, a complete
-    machine-readable copy of the corresponding source code, to be
-    distributed under the terms of Sections 1 and 2 above on a medium
-    customarily used for software interchange; or,
-
-    c) Accompany it with the information you received as to the offer
-    to distribute corresponding source code.  (This alternative is
-    allowed only for noncommercial distribution and only if you
-    received the program in object code or executable form with such
-    an offer, in accord with Subsection b above.)
-
-The source code for a work means the preferred form of the work for
-making modifications to it.  For an executable work, complete source
-code means all the source code for all modules it contains, plus any
-associated interface definition files, plus the scripts used to
-control compilation and installation of the executable.  However, as a
-special exception, the source code distributed need not include
-anything that is normally distributed (in either source or binary
-form) with the major components (compiler, kernel, and so on) of the
-operating system on which the executable runs, unless that component
-itself accompanies the executable.
-
-If distribution of executable or object code is made by offering
-access to copy from a designated place, then offering equivalent
-access to copy the source code from the same place counts as
-distribution of the source code, even though third parties are not
-compelled to copy the source along with the object code.
-
-  4. You may not copy, modify, sublicense, or distribute the Program
-except as expressly provided under this License.  Any attempt
-otherwise to copy, modify, sublicense or distribute the Program is
-void, and will automatically terminate your rights under this License.
-However, parties who have received copies, or rights, from you under
-this License will not have their licenses terminated so long as such
-parties remain in full compliance.
-
-  5. You are not required to accept this License, since you have not
-signed it.  However, nothing else grants you permission to modify or
-distribute the Program or its derivative works.  These actions are
-prohibited by law if you do not accept this License.  Therefore, by
-modifying or distributing the Program (or any work based on the
-Program), you indicate your acceptance of this License to do so, and
-all its terms and conditions for copying, distributing or modifying
-the Program or works based on it.
-
-  6. Each time you redistribute the Program (or any work based on the
-Program), the recipient automatically receives a license from the
-original licensor to copy, distribute or modify the Program subject to
-these terms and conditions.  You may not impose any further
-restrictions on the recipients' exercise of the rights granted herein.
-You are not responsible for enforcing compliance by third parties to
-this License.
-
-  7. If, as a consequence of a court judgment or allegation of patent
-infringement or for any other reason (not limited to patent issues),
-conditions are imposed on you (whether by court order, agreement or
-otherwise) that contradict the conditions of this License, they do not
-excuse you from the conditions of this License.  If you cannot
-distribute so as to satisfy simultaneously your obligations under this
-License and any other pertinent obligations, then as a consequence you
-may not distribute the Program at all.  For example, if a patent
-license would not permit royalty-free redistribution of the Program by
-all those who receive copies directly or indirectly through you, then
-the only way you could satisfy both it and this License would be to
-refrain entirely from distribution of the Program.
-
-If any portion of this section is held invalid or unenforceable under
-any particular circumstance, the balance of the section is intended to
-apply and the section as a whole is intended to apply in other
-circumstances.
-
-It is not the purpose of this section to induce you to infringe any
-patents or other property right claims or to contest validity of any
-such claims; this section has the sole purpose of protecting the
-integrity of the free software distribution system, which is
-implemented by public license practices.  Many people have made
-generous contributions to the wide range of software distributed
-through that system in reliance on consistent application of that
-system; it is up to the author/donor to decide if he or she is willing
-to distribute software through any other system and a licensee cannot
-impose that choice.
-
-This section is intended to make thoroughly clear what is believed to
-be a consequence of the rest of this License.
-
-  8. If the distribution and/or use of the Program is restricted in
-certain countries either by patents or by copyrighted interfaces, the
-original copyright holder who places the Program under this License
-may add an explicit geographical distribution limitation excluding
-those countries, so that distribution is permitted only in or among
-countries not thus excluded.  In such case, this License incorporates
-the limitation as if written in the body of this License.
-
-  9. The Free Software Foundation may publish revised and/or new versions
-of the General Public License from time to time.  Such new versions will
-be similar in spirit to the present version, but may differ in detail to
-address new problems or concerns.
-
-Each version is given a distinguishing version number.  If the Program
-specifies a version number of this License which applies to it and "any
-later version", you have the option of following the terms and conditions
-either of that version or of any later version published by the Free
-Software Foundation.  If the Program does not specify a version number of
-this License, you may choose any version ever published by the Free Software
-Foundation.
-
-  10. If you wish to incorporate parts of the Program into other free
-programs whose distribution conditions are different, write to the author
-to ask for permission.  For software which is copyrighted by the Free
-Software Foundation, write to the Free Software Foundation; we sometimes
-make exceptions for this.  Our decision will be guided by the two goals
-of preserving the free status of all derivatives of our free software and
-of promoting the sharing and reuse of software generally.
-
-                            NO WARRANTY
-
-  11. BECAUSE THE PROGRAM IS LICENSED FREE OF CHARGE, THERE IS NO WARRANTY
-FOR THE PROGRAM, TO THE EXTENT PERMITTED BY APPLICABLE LAW.  EXCEPT WHEN
-OTHERWISE STATED IN WRITING THE COPYRIGHT HOLDERS AND/OR OTHER PARTIES
-PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY OF ANY KIND, EITHER EXPRESSED
-OR IMPLIED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF
-MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.  THE ENTIRE RISK AS
-TO THE QUALITY AND PERFORMANCE OF THE PROGRAM IS WITH YOU.  SHOULD THE
-PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF ALL NECESSARY SERVICING,
-REPAIR OR CORRECTION.
-
-  12. IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
-WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MAY MODIFY AND/OR
-REDISTRIBUTE THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES,
-INCLUDING ANY GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING
-OUT OF THE USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED
-TO LOSS OF DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY
-YOU OR THIRD PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER
-PROGRAMS), EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE
-POSSIBILITY OF SUCH DAMAGES.
-
-                     END OF TERMS AND CONDITIONS
-
-            How to Apply These Terms to Your New Programs
-
-  If you develop a new program, and you want it to be of the greatest
-possible use to the public, the best way to achieve this is to make it
-free software which everyone can redistribute and change under these terms.
-
-  To do so, attach the following notices to the program.  It is safest
-to attach them to the start of each source file to most effectively
-convey the exclusion of warranty; and each file should have at least
-the "copyright" line and a pointer to where the full notice is found.
-
-    <one line to give the program's name and a brief idea of what it does.>
-    Copyright (C) <year>  <name of author>
-
-    This program is free software; you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation; either version 2 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License along
-    with this program; if not, write to the Free Software Foundation, Inc.,
-    51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
-
-Also add information on how to contact you by electronic and paper mail.
-
-If the program is interactive, make it output a short notice like this
-when it starts in an interactive mode:
-
-    Gnomovision version 69, Copyright (C) year name of author
-    Gnomovision comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
-    This is free software, and you are welcome to redistribute it
-    under certain conditions; type `show c' for details.
-
-The hypothetical commands `show w' and `show c' should show the appropriate
-parts of the General Public License.  Of course, the commands you use may
-be called something other than `show w' and `show c'; they could even be
-mouse-clicks or menu items--whatever suits your program.
-
-You should also get your employer (if you work as a programmer) or your
-school, if any, to sign a "copyright disclaimer" for the program, if
-necessary.  Here is a sample; alter the names:
-
-  Yoyodyne, Inc., hereby disclaims all copyright interest in the program
-  `Gnomovision' (which makes passes at compilers) written by James Hacker.
-
-  <signature of Ty Coon>, 1 April 1989
-  Ty Coon, President of Vice
-
-This General Public License does not permit incorporating your program into
-proprietary programs.  If your program is a subroutine library, you may
-consider it more useful to permit linking proprietary applications with the
-library.  If this is what you want to do, use the GNU Lesser General
-Public License instead of this License.
+                    GNU GENERAL PUBLIC LICENSE
+                       Version 2, June 1991
+
+ Copyright (C) 1989, 1991 Free Software Foundation, Inc.,
+ 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
+ Everyone is permitted to copy and distribute verbatim copies
+ of this license document, but changing it is not allowed.
+
+                            Preamble
+
+  The licenses for most software are designed to take away your
+freedom to share and change it.  By contrast, the GNU General Public
+License is intended to guarantee your freedom to share and change free
+software--to make sure the software is free for all its users.  This
+General Public License applies to most of the Free Software
+Foundation's software and to any other program whose authors commit to
+using it.  (Some other Free Software Foundation software is covered by
+the GNU Lesser General Public License instead.)  You can apply it to
+your programs, too.
+
+  When we speak of free software, we are referring to freedom, not
+price.  Our General Public Licenses are designed to make sure that you
+have the freedom to distribute copies of free software (and charge for
+this service if you wish), that you receive source code or can get it
+if you want it, that you can change the software or use pieces of it
+in new free programs; and that you know you can do these things.
+
+  To protect your rights, we need to make restrictions that forbid
+anyone to deny you these rights or to ask you to surrender the rights.
+These restrictions translate to certain responsibilities for you if you
+distribute copies of the software, or if you modify it.
+
+  For example, if you distribute copies of such a program, whether
+gratis or for a fee, you must give the recipients all the rights that
+you have.  You must make sure that they, too, receive or can get the
+source code.  And you must show them these terms so they know their
+rights.
+
+  We protect your rights with two steps: (1) copyright the software, and
+(2) offer you this license which gives you legal permission to copy,
+distribute and/or modify the software.
+
+  Also, for each author's protection and ours, we want to make certain
+that everyone understands that there is no warranty for this free
+software.  If the software is modified by someone else and passed on, we
+want its recipients to know that what they have is not the original, so
+that any problems introduced by others will not reflect on the original
+authors' reputations.
+
+  Finally, any free program is threatened constantly by software
+patents.  We wish to avoid the danger that redistributors of a free
+program will individually obtain patent licenses, in effect making the
+program proprietary.  To prevent this, we have made it clear that any
+patent must be licensed for everyone's free use or not licensed at all.
+
+  The precise terms and conditions for copying, distribution and
+modification follow.
+
+                    GNU GENERAL PUBLIC LICENSE
+   TERMS AND CONDITIONS FOR COPYING, DISTRIBUTION AND MODIFICATION
+
+  0. This License applies to any program or other work which contains
+a notice placed by the copyright holder saying it may be distributed
+under the terms of this General Public License.  The "Program", below,
+refers to any such program or work, and a "work based on the Program"
+means either the Program or any derivative work under copyright law:
+that is to say, a work containing the Program or a portion of it,
+either verbatim or with modifications and/or translated into another
+language.  (Hereinafter, translation is included without limitation in
+the term "modification".)  Each licensee is addressed as "you".
+
+Activities other than copying, distribution and modification are not
+covered by this License; they are outside its scope.  The act of
+running the Program is not restricted, and the output from the Program
+is covered only if its contents constitute a work based on the
+Program (independent of having been made by running the Program).
+Whether that is true depends on what the Program does.
+
+  1. You may copy and distribute verbatim copies of the Program's
+source code as you receive it, in any medium, provided that you
+conspicuously and appropriately publish on each copy an appropriate
+copyright notice and disclaimer of warranty; keep intact all the
+notices that refer to this License and to the absence of any warranty;
+and give any other recipients of the Program a copy of this License
+along with the Program.
+
+You may charge a fee for the physical act of transferring a copy, and
+you may at your option offer warranty protection in exchange for a fee.
+
+  2. You may modify your copy or copies of the Program or any portion
+of it, thus forming a work based on the Program, and copy and
+distribute such modifications or work under the terms of Section 1
+above, provided that you also meet all of these conditions:
+
+    a) You must cause the modified files to carry prominent notices
+    stating that you changed the files and the date of any change.
+
+    b) You must cause any work that you distribute or publish, that in
+    whole or in part contains or is derived from the Program or any
+    part thereof, to be licensed as a whole at no charge to all third
+    parties under the terms of this License.
+
+    c) If the modified program normally reads commands interactively
+    when run, you must cause it, when started running for such
+    interactive use in the most ordinary way, to print or display an
+    announcement including an appropriate copyright notice and a
+    notice that there is no warranty (or else, saying that you provide
+    a warranty) and that users may redistribute the program under
+    these conditions, and telling the user how to view a copy of this
+    License.  (Exception: if the Program itself is interactive but
+    does not normally print such an announcement, your work based on
+    the Program is not required to print an announcement.)
+
+These requirements apply to the modified work as a whole.  If
+identifiable sections of that work are not derived from the Program,
+and can be reasonably considered independent and separate works in
+themselves, then this License, and its terms, do not apply to those
+sections when you distribute them as separate works.  But when you
+distribute the same sections as part of a whole which is a work based
+on the Program, the distribution of the whole must be on the terms of
+this License, whose permissions for other licensees extend to the
+entire whole, and thus to each and every part regardless of who wrote it.
+
+Thus, it is not the intent of this section to claim rights or contest
+your rights to work written entirely by you; rather, the intent is to
+exercise the right to control the distribution of derivative or
+collective works based on the Program.
+
+In addition, mere aggregation of another work not based on the Program
+with the Program (or with a work based on the Program) on a volume of
+a storage or distribution medium does not bring the other work under
+the scope of this License.
+
+  3. You may copy and distribute the Program (or a work based on it,
+under Section 2) in object code or executable form under the terms of
+Sections 1 and 2 above provided that you also do one of the following:
+
+    a) Accompany it with the complete corresponding machine-readable
+    source code, which must be distributed under the terms of Sections
+    1 and 2 above on a medium customarily used for software interchange; or,
+
+    b) Accompany it with a written offer, valid for at least three
+    years, to give any third party, for a charge no more than your
+    cost of physically performing source distribution, a complete
+    machine-readable copy of the corresponding source code, to be
+    distributed under the terms of Sections 1 and 2 above on a medium
+    customarily used for software interchange; or,
+
+    c) Accompany it with the information you received as to the offer
+    to distribute corresponding source code.  (This alternative is
+    allowed only for noncommercial distribution and only if you
+    received the program in object code or executable form with such
+    an offer, in accord with Subsection b above.)
+
+The source code for a work means the preferred form of the work for
+making modifications to it.  For an executable work, complete source
+code means all the source code for all modules it contains, plus any
+associated interface definition files, plus the scripts used to
+control compilation and installation of the executable.  However, as a
+special exception, the source code distributed need not include
+anything that is normally distributed (in either source or binary
+form) with the major components (compiler, kernel, and so on) of the
+operating system on which the executable runs, unless that component
+itself accompanies the executable.
+
+If distribution of executable or object code is made by offering
+access to copy from a designated place, then offering equivalent
+access to copy the source code from the same place counts as
+distribution of the source code, even though third parties are not
+compelled to copy the source along with the object code.
+
+  4. You may not copy, modify, sublicense, or distribute the Program
+except as expressly provided under this License.  Any attempt
+otherwise to copy, modify, sublicense or distribute the Program is
+void, and will automatically terminate your rights under this License.
+However, parties who have received copies, or rights, from you under
+this License will not have their licenses terminated so long as such
+parties remain in full compliance.
+
+  5. You are not required to accept this License, since you have not
+signed it.  However, nothing else grants you permission to modify or
+distribute the Program or its derivative works.  These actions are
+prohibited by law if you do not accept this License.  Therefore, by
+modifying or distributing the Program (or any work based on the
+Program), you indicate your acceptance of this License to do so, and
+all its terms and conditions for copying, distributing or modifying
+the Program or works based on it.
+
+  6. Each time you redistribute the Program (or any work based on the
+Program), the recipient automatically receives a license from the
+original licensor to copy, distribute or modify the Program subject to
+these terms and conditions.  You may not impose any further
+restrictions on the recipients' exercise of the rights granted herein.
+You are not responsible for enforcing compliance by third parties to
+this License.
+
+  7. If, as a consequence of a court judgment or allegation of patent
+infringement or for any other reason (not limited to patent issues),
+conditions are imposed on you (whether by court order, agreement or
+otherwise) that contradict the conditions of this License, they do not
+excuse you from the conditions of this License.  If you cannot
+distribute so as to satisfy simultaneously your obligations under this
+License and any other pertinent obligations, then as a consequence you
+may not distribute the Program at all.  For example, if a patent
+license would not permit royalty-free redistribution of the Program by
+all those who receive copies directly or indirectly through you, then
+the only way you could satisfy both it and this License would be to
+refrain entirely from distribution of the Program.
+
+If any portion of this section is held invalid or unenforceable under
+any particular circumstance, the balance of the section is intended to
+apply and the section as a whole is intended to apply in other
+circumstances.
+
+It is not the purpose of this section to induce you to infringe any
+patents or other property right claims or to contest validity of any
+such claims; this section has the sole purpose of protecting the
+integrity of the free software distribution system, which is
+implemented by public license practices.  Many people have made
+generous contributions to the wide range of software distributed
+through that system in reliance on consistent application of that
+system; it is up to the author/donor to decide if he or she is willing
+to distribute software through any other system and a licensee cannot
+impose that choice.
+
+This section is intended to make thoroughly clear what is believed to
+be a consequence of the rest of this License.
+
+  8. If the distribution and/or use of the Program is restricted in
+certain countries either by patents or by copyrighted interfaces, the
+original copyright holder who places the Program under this License
+may add an explicit geographical distribution limitation excluding
+those countries, so that distribution is permitted only in or among
+countries not thus excluded.  In such case, this License incorporates
+the limitation as if written in the body of this License.
+
+  9. The Free Software Foundation may publish revised and/or new versions
+of the General Public License from time to time.  Such new versions will
+be similar in spirit to the present version, but may differ in detail to
+address new problems or concerns.
+
+Each version is given a distinguishing version number.  If the Program
+specifies a version number of this License which applies to it and "any
+later version", you have the option of following the terms and conditions
+either of that version or of any later version published by the Free
+Software Foundation.  If the Program does not specify a version number of
+this License, you may choose any version ever published by the Free Software
+Foundation.
+
+  10. If you wish to incorporate parts of the Program into other free
+programs whose distribution conditions are different, write to the author
+to ask for permission.  For software which is copyrighted by the Free
+Software Foundation, write to the Free Software Foundation; we sometimes
+make exceptions for this.  Our decision will be guided by the two goals
+of preserving the free status of all derivatives of our free software and
+of promoting the sharing and reuse of software generally.
+
+                            NO WARRANTY
+
+  11. BECAUSE THE PROGRAM IS LICENSED FREE OF CHARGE, THERE IS NO WARRANTY
+FOR THE PROGRAM, TO THE EXTENT PERMITTED BY APPLICABLE LAW.  EXCEPT WHEN
+OTHERWISE STATED IN WRITING THE COPYRIGHT HOLDERS AND/OR OTHER PARTIES
+PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY OF ANY KIND, EITHER EXPRESSED
+OR IMPLIED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF
+MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.  THE ENTIRE RISK AS
+TO THE QUALITY AND PERFORMANCE OF THE PROGRAM IS WITH YOU.  SHOULD THE
+PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF ALL NECESSARY SERVICING,
+REPAIR OR CORRECTION.
+
+  12. IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
+WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MAY MODIFY AND/OR
+REDISTRIBUTE THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES,
+INCLUDING ANY GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING
+OUT OF THE USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED
+TO LOSS OF DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY
+YOU OR THIRD PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER
+PROGRAMS), EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE
+POSSIBILITY OF SUCH DAMAGES.
+
+                     END OF TERMS AND CONDITIONS
+
+            How to Apply These Terms to Your New Programs
+
+  If you develop a new program, and you want it to be of the greatest
+possible use to the public, the best way to achieve this is to make it
+free software which everyone can redistribute and change under these terms.
+
+  To do so, attach the following notices to the program.  It is safest
+to attach them to the start of each source file to most effectively
+convey the exclusion of warranty; and each file should have at least
+the "copyright" line and a pointer to where the full notice is found.
+
+    <one line to give the program's name and a brief idea of what it does.>
+    Copyright (C) <year>  <name of author>
+
+    This program is free software; you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation; either version 2 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License along
+    with this program; if not, write to the Free Software Foundation, Inc.,
+    51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
+
+Also add information on how to contact you by electronic and paper mail.
+
+If the program is interactive, make it output a short notice like this
+when it starts in an interactive mode:
+
+    Gnomovision version 69, Copyright (C) year name of author
+    Gnomovision comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
+    This is free software, and you are welcome to redistribute it
+    under certain conditions; type `show c' for details.
+
+The hypothetical commands `show w' and `show c' should show the appropriate
+parts of the General Public License.  Of course, the commands you use may
+be called something other than `show w' and `show c'; they could even be
+mouse-clicks or menu items--whatever suits your program.
+
+You should also get your employer (if you work as a programmer) or your
+school, if any, to sign a "copyright disclaimer" for the program, if
+necessary.  Here is a sample; alter the names:
+
+  Yoyodyne, Inc., hereby disclaims all copyright interest in the program
+  `Gnomovision' (which makes passes at compilers) written by James Hacker.
+
+  <signature of Ty Coon>, 1 April 1989
+  Ty Coon, President of Vice
+
+This General Public License does not permit incorporating your program into
+proprietary programs.  If your program is a subroutine library, you may
+consider it more useful to permit linking proprietary applications with the
+library.  If this is what you want to do, use the GNU Lesser General
+Public License instead of this License.
```

### Comparing `mysqlclient-2.2.0/PKG-INFO` & `mysqlclient-2.2.0rc1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,130 +1,130 @@
-Metadata-Version: 2.1
-Name: mysqlclient
-Version: 2.2.0
-Summary: Python interface to MySQL
-Author-email: Inada Naoki <songofacandy@gmail.com>
-License: GNU General Public License v2 (GPLv2)
-Project-URL: Project, https://github.com/PyMySQL/mysqlclient
-Project-URL: Documentation, https://mysqlclient.readthedocs.io/
-Keywords: MySQL
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Other Environment
-Classifier: License :: OSI Approved :: GNU General Public License (GPL)
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows :: Windows NT/2000
-Classifier: Operating System :: OS Independent
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: Unix
-Classifier: Programming Language :: C
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Database
-Classifier: Topic :: Database :: Database Engines/Servers
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# mysqlclient
-
-This project is a fork of [MySQLdb1](https://github.com/farcepest/MySQLdb1).
-This project adds Python 3 support and fixed many bugs.
-
-* PyPI: https://pypi.org/project/mysqlclient/
-* GitHub: https://github.com/PyMySQL/mysqlclient
-
-
-## Support
-
-**Do Not use Github Issue Tracker to ask help.  OSS Maintainer is not free tech support**
-
-When your question looks relating to Python rather than MySQL:
-
-* Python mailing list [python-list](https://mail.python.org/mailman/listinfo/python-list)
-* Slack [pythondev.slack.com](https://pyslackers.com/web/slack)
-
-Or when you have question about MySQL:
-
-* [MySQL Community on Slack](https://lefred.be/mysql-community-on-slack/)
-
-
-## Install
-
-### Windows
-
-Building mysqlclient on Windows is very hard.
-But there are some binary wheels you can install easily.
-
-If binary wheels do not exist for your version of Python, it may be possible to
-build from source, but if this does not work, **do not come asking for support.**
-To build from source, download the
-[MariaDB C Connector](https://mariadb.com/downloads/#connectors) and install
-it. It must be installed in the default location
-(usually "C:\Program Files\MariaDB\MariaDB Connector C" or
-"C:\Program Files (x86)\MariaDB\MariaDB Connector C" for 32-bit). If you
-build the connector yourself or install it in a different location, set the
-environment variable `MYSQLCLIENT_CONNECTOR` before installing. Once you have
-the connector installed and an appropriate version of Visual Studio for your
-version of Python:
-
-```
-$ pip install mysqlclient
-```
-
-### macOS (Homebrew)
-
-Install MySQL and mysqlclient:
-
-```
-# Assume you are activating Python 3 venv
-$ brew install mysql pkg-config
-$ pip install mysqlclient
-```
-
-If you don't want to install MySQL server, you can use mysql-client instead:
-
-```
-# Assume you are activating Python 3 venv
-$ brew install mysql-client pkg-config
-$ export PKG_CONFIG_PATH="/opt/homebrew/opt/mysql-client/lib/pkgconfig"
-$ pip install mysqlclient
-```
-
-### Linux
-
-**Note that this is a basic step.  I can not support complete step for build for all
-environment.  If you can see some error, you should fix it by yourself, or ask for
-support in some user forum.  Don't file a issue on the issue tracker.**
-
-You may need to install the Python 3 and MySQL development headers and libraries like so:
-
-* `$ sudo apt-get install python3-dev default-libmysqlclient-dev build-essential`  # Debian / Ubuntu
-* `% sudo yum install python3-devel mysql-devel`  # Red Hat / CentOS
-
-Then you can install mysqlclient via pip now:
-
-```
-$ pip install mysqlclient
-```
-
-### Customize build (POSIX)
-
-mysqlclient uses `pkg-config --clfags --ldflags mysqlclient` by default for finding
-compiler/linker flags.
-
-You can use `MYSQLCLIENT_CFLAGS` and `MYSQLCLIENT_LDFLAGS` environment
-variables to customize compiler/linker options.
-
-```
-$ export MYSQLCLIENT_CFLAGS=`pkg-config mysqlclient --cflags`
-$ export MYSQLCLIENT_LDFLAGS=`pkg-config mysqlclient --libs`
-$ pip install mysqlclient
-```
-
-### Documentation
-
-Documentation is hosted on [Read The Docs](https://mysqlclient.readthedocs.io/)
+Metadata-Version: 2.1
+Name: mysqlclient
+Version: 2.2.0rc1
+Summary: Python interface to MySQL
+Author-email: Inada Naoki <songofacandy@gmail.com>
+License: GNU General Public License v2 (GPLv2)
+Project-URL: Project, https://github.com/PyMySQL/mysqlclient
+Project-URL: Documentation, https://mysqlclient.readthedocs.io/
+Keywords: MySQL
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Other Environment
+Classifier: License :: OSI Approved :: GNU General Public License (GPL)
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows :: Windows NT/2000
+Classifier: Operating System :: OS Independent
+Classifier: Operating System :: POSIX
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: Unix
+Classifier: Programming Language :: C
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Database
+Classifier: Topic :: Database :: Database Engines/Servers
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# mysqlclient
+
+This project is a fork of [MySQLdb1](https://github.com/farcepest/MySQLdb1).
+This project adds Python 3 support and fixed many bugs.
+
+* PyPI: https://pypi.org/project/mysqlclient/
+* GitHub: https://github.com/PyMySQL/mysqlclient
+
+
+## Support
+
+**Do Not use Github Issue Tracker to ask help.  OSS Maintainer is not free tech support**
+
+When your question looks relating to Python rather than MySQL:
+
+* Python mailing list [python-list](https://mail.python.org/mailman/listinfo/python-list)
+* Slack [pythondev.slack.com](https://pyslackers.com/web/slack)
+
+Or when you have question about MySQL:
+
+* [MySQL Community on Slack](https://lefred.be/mysql-community-on-slack/)
+
+
+## Install
+
+### Windows
+
+Building mysqlclient on Windows is very hard.
+But there are some binary wheels you can install easily.
+
+If binary wheels do not exist for your version of Python, it may be possible to
+build from source, but if this does not work, **do not come asking for support.**
+To build from source, download the
+[MariaDB C Connector](https://mariadb.com/downloads/#connectors) and install
+it. It must be installed in the default location
+(usually "C:\Program Files\MariaDB\MariaDB Connector C" or
+"C:\Program Files (x86)\MariaDB\MariaDB Connector C" for 32-bit). If you
+build the connector yourself or install it in a different location, set the
+environment variable `MYSQLCLIENT_CONNECTOR` before installing. Once you have
+the connector installed and an appropriate version of Visual Studio for your
+version of Python:
+
+```
+$ pip install mysqlclient
+```
+
+### macOS (Homebrew)
+
+Install MySQL and mysqlclient:
+
+```
+# Assume you are activating Python 3 venv
+$ brew install mysql pkg-config
+$ pip install mysqlclient
+```
+
+If you don't want to install MySQL server, you can use mysql-client instead:
+
+```
+# Assume you are activating Python 3 venv
+$ brew install mysql-client pkg-config
+$ export PKG_CONFIG_PATH="/opt/homebrew/opt/mysql-client/lib/pkgconfig"
+$ pip install mysqlclient
+```
+
+### Linux
+
+**Note that this is a basic step.  I can not support complete step for build for all
+environment.  If you can see some error, you should fix it by yourself, or ask for
+support in some user forum.  Don't file a issue on the issue tracker.**
+
+You may need to install the Python 3 and MySQL development headers and libraries like so:
+
+* `$ sudo apt-get install python3-dev default-libmysqlclient-dev build-essential`  # Debian / Ubuntu
+* `% sudo yum install python3-devel mysql-devel`  # Red Hat / CentOS
+
+Then you can install mysqlclient via pip now:
+
+```
+$ pip install mysqlclient
+```
+
+### Customize build (POSIX)
+
+mysqlclient uses `pkg-config --clfags --ldflags mysqlclient` by default for finding
+compiler/linker flags.
+
+You can use `MYSQLCLIENT_CFLAGS` and `MYSQLCLIENT_LDFLAGS` environment
+variables to customize compiler/linker options.
+
+```
+$ export MYSQLCLIENT_CFLAGS=`pkg-config mysqlclient --cflags`
+$ export MYSQLCLIENT_LDFLAGS=`pkg-config mysqlclient --libs`
+$ pip install mysqlclient
+```
+
+### Documentation
+
+Documentation is hosted on [Read The Docs](https://mysqlclient.readthedocs.io/)
```

### Comparing `mysqlclient-2.2.0/README.md` & `mysqlclient-2.2.0rc1/README.md`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,99 +1,99 @@
-# mysqlclient
-
-This project is a fork of [MySQLdb1](https://github.com/farcepest/MySQLdb1).
-This project adds Python 3 support and fixed many bugs.
-
-* PyPI: https://pypi.org/project/mysqlclient/
-* GitHub: https://github.com/PyMySQL/mysqlclient
-
-
-## Support
-
-**Do Not use Github Issue Tracker to ask help.  OSS Maintainer is not free tech support**
-
-When your question looks relating to Python rather than MySQL:
-
-* Python mailing list [python-list](https://mail.python.org/mailman/listinfo/python-list)
-* Slack [pythondev.slack.com](https://pyslackers.com/web/slack)
-
-Or when you have question about MySQL:
-
-* [MySQL Community on Slack](https://lefred.be/mysql-community-on-slack/)
-
-
-## Install
-
-### Windows
-
-Building mysqlclient on Windows is very hard.
-But there are some binary wheels you can install easily.
-
-If binary wheels do not exist for your version of Python, it may be possible to
-build from source, but if this does not work, **do not come asking for support.**
-To build from source, download the
-[MariaDB C Connector](https://mariadb.com/downloads/#connectors) and install
-it. It must be installed in the default location
-(usually "C:\Program Files\MariaDB\MariaDB Connector C" or
-"C:\Program Files (x86)\MariaDB\MariaDB Connector C" for 32-bit). If you
-build the connector yourself or install it in a different location, set the
-environment variable `MYSQLCLIENT_CONNECTOR` before installing. Once you have
-the connector installed and an appropriate version of Visual Studio for your
-version of Python:
-
-```
-$ pip install mysqlclient
-```
-
-### macOS (Homebrew)
-
-Install MySQL and mysqlclient:
-
-```
-# Assume you are activating Python 3 venv
-$ brew install mysql pkg-config
-$ pip install mysqlclient
-```
-
-If you don't want to install MySQL server, you can use mysql-client instead:
-
-```
-# Assume you are activating Python 3 venv
-$ brew install mysql-client pkg-config
-$ export PKG_CONFIG_PATH="/opt/homebrew/opt/mysql-client/lib/pkgconfig"
-$ pip install mysqlclient
-```
-
-### Linux
-
-**Note that this is a basic step.  I can not support complete step for build for all
-environment.  If you can see some error, you should fix it by yourself, or ask for
-support in some user forum.  Don't file a issue on the issue tracker.**
-
-You may need to install the Python 3 and MySQL development headers and libraries like so:
-
-* `$ sudo apt-get install python3-dev default-libmysqlclient-dev build-essential`  # Debian / Ubuntu
-* `% sudo yum install python3-devel mysql-devel`  # Red Hat / CentOS
-
-Then you can install mysqlclient via pip now:
-
-```
-$ pip install mysqlclient
-```
-
-### Customize build (POSIX)
-
-mysqlclient uses `pkg-config --clfags --ldflags mysqlclient` by default for finding
-compiler/linker flags.
-
-You can use `MYSQLCLIENT_CFLAGS` and `MYSQLCLIENT_LDFLAGS` environment
-variables to customize compiler/linker options.
-
-```
-$ export MYSQLCLIENT_CFLAGS=`pkg-config mysqlclient --cflags`
-$ export MYSQLCLIENT_LDFLAGS=`pkg-config mysqlclient --libs`
-$ pip install mysqlclient
-```
-
-### Documentation
-
-Documentation is hosted on [Read The Docs](https://mysqlclient.readthedocs.io/)
+# mysqlclient
+
+This project is a fork of [MySQLdb1](https://github.com/farcepest/MySQLdb1).
+This project adds Python 3 support and fixed many bugs.
+
+* PyPI: https://pypi.org/project/mysqlclient/
+* GitHub: https://github.com/PyMySQL/mysqlclient
+
+
+## Support
+
+**Do Not use Github Issue Tracker to ask help.  OSS Maintainer is not free tech support**
+
+When your question looks relating to Python rather than MySQL:
+
+* Python mailing list [python-list](https://mail.python.org/mailman/listinfo/python-list)
+* Slack [pythondev.slack.com](https://pyslackers.com/web/slack)
+
+Or when you have question about MySQL:
+
+* [MySQL Community on Slack](https://lefred.be/mysql-community-on-slack/)
+
+
+## Install
+
+### Windows
+
+Building mysqlclient on Windows is very hard.
+But there are some binary wheels you can install easily.
+
+If binary wheels do not exist for your version of Python, it may be possible to
+build from source, but if this does not work, **do not come asking for support.**
+To build from source, download the
+[MariaDB C Connector](https://mariadb.com/downloads/#connectors) and install
+it. It must be installed in the default location
+(usually "C:\Program Files\MariaDB\MariaDB Connector C" or
+"C:\Program Files (x86)\MariaDB\MariaDB Connector C" for 32-bit). If you
+build the connector yourself or install it in a different location, set the
+environment variable `MYSQLCLIENT_CONNECTOR` before installing. Once you have
+the connector installed and an appropriate version of Visual Studio for your
+version of Python:
+
+```
+$ pip install mysqlclient
+```
+
+### macOS (Homebrew)
+
+Install MySQL and mysqlclient:
+
+```
+# Assume you are activating Python 3 venv
+$ brew install mysql pkg-config
+$ pip install mysqlclient
+```
+
+If you don't want to install MySQL server, you can use mysql-client instead:
+
+```
+# Assume you are activating Python 3 venv
+$ brew install mysql-client pkg-config
+$ export PKG_CONFIG_PATH="/opt/homebrew/opt/mysql-client/lib/pkgconfig"
+$ pip install mysqlclient
+```
+
+### Linux
+
+**Note that this is a basic step.  I can not support complete step for build for all
+environment.  If you can see some error, you should fix it by yourself, or ask for
+support in some user forum.  Don't file a issue on the issue tracker.**
+
+You may need to install the Python 3 and MySQL development headers and libraries like so:
+
+* `$ sudo apt-get install python3-dev default-libmysqlclient-dev build-essential`  # Debian / Ubuntu
+* `% sudo yum install python3-devel mysql-devel`  # Red Hat / CentOS
+
+Then you can install mysqlclient via pip now:
+
+```
+$ pip install mysqlclient
+```
+
+### Customize build (POSIX)
+
+mysqlclient uses `pkg-config --clfags --ldflags mysqlclient` by default for finding
+compiler/linker flags.
+
+You can use `MYSQLCLIENT_CFLAGS` and `MYSQLCLIENT_LDFLAGS` environment
+variables to customize compiler/linker options.
+
+```
+$ export MYSQLCLIENT_CFLAGS=`pkg-config mysqlclient --cflags`
+$ export MYSQLCLIENT_LDFLAGS=`pkg-config mysqlclient --libs`
+$ pip install mysqlclient
+```
+
+### Documentation
+
+Documentation is hosted on [Read The Docs](https://mysqlclient.readthedocs.io/)
```

### Comparing `mysqlclient-2.2.0/doc/FAQ.rst` & `mysqlclient-2.2.0rc1/doc/FAQ.rst`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,136 +1,136 @@
-====================================
- MySQLdb Frequently Asked Questions
-====================================
-
-.. contents::
-..
-
-
-Build Errors
-------------
-
-  mysql.h: No such file or directory
-
-This almost always mean you don't have development packages
-installed. On some systems, C headers for various things (like MySQL)
-are distributed as a separate package. You'll need to figure out
-what that is and install it, but often the name ends with -devel.
-
-Another possibility: Some older versions of mysql_config behave oddly
-and may throw quotes around some of the path names, which confused
-MySQLdb-1.2.0. 1.2.1 works around these problems. If you see things
-like -I'/usr/local/include/mysql' in your compile command, that's
-probably the issue, but it shouldn't happen any more.
-
-
-ImportError
------------
-
-  ImportError: No module named _mysql
-
-If you see this, it's likely you did some wrong when installing
-MySQLdb; re-read (or read) README. _mysql is the low-level C module
-that interfaces with the MySQL client library.
-
-Various versions of MySQLdb in the past have had build issues on
-"weird" platforms; "weird" in this case means "not Linux", though
-generally there aren't problems on Unix/POSIX platforms, including
-BSDs and Mac OS X. Windows has been more problematic, in part because
-there is no `mysql_config` available in the Windows installation of
-MySQL. 1.2.1 solves most, if not all, of these problems, but you will
-still have to edit a configuration file so that the setup knows where
-to find MySQL and what libraries to include.
-
-
-  ImportError: libmysqlclient_r.so.14: cannot open shared object file: No such file or directory
-
-The number after .so may vary, but this means you have a version of
-MySQLdb compiled against one version of MySQL, and are now trying to
-run it against a different version. The shared library version tends
-to change between major releases.
-
-Solution: Rebuilt MySQLdb, or get the matching version of MySQL.
-
-Another thing that can cause this: The MySQL libraries may not be on
-your system path.
-
-Solutions:
-
-* set the LD_LIBRARY_PATH environment variable so that it includes
-  the path to the MySQL libraries.
-
-* set static=True in site.cfg for static linking
-
-* reconfigure your system so that the MySQL libraries are on the
-  default loader path. In Linux, you edit /etc/ld.so.conf and run
-  ldconfig. For Solaris, see `Linker and Libraries Guide
-  <http://docs.oracle.com/cd/E19253-01/817-1984/chapter6-63352/>`_.
-
-
-  ImportError: ld.so.1: python: fatal: libmtmalloc.so.1: DF_1_NOOPEN tagged object may not be dlopen()'ed
-
-This is a weird one from Solaris. What does it mean? I have no idea.
-However, things like this can happen if there is some sort of a compiler
-or environment mismatch between Python and MySQL. For example, on some
-commercial systems, you might have some code compiled with their own
-compiler, and other things compiled with GCC. They don't always mesh
-together. One way to encounter this is by getting binary packages from
-different vendors.
-
-Solution: Rebuild Python or MySQL (or maybe both) from source.
-
-  ImportError: dlopen(./_mysql.so, 2): Symbol not found: _sprintf$LDBLStub
-  Referenced from: ./_mysql.so
-  Expected in: dynamic lookup
-
-This is one from Mac OS X. It seems to have been a compiler mismatch,
-but this time between two different versions of GCC. It seems nearly
-every major release of GCC changes the ABI in some why, so linking
-code compiled with GCC-3.3 and GCC-4.0, for example, can be
-problematic.
-
-
-My data disappeared! (or won't go away!)
-----------------------------------------
-
-Starting with 1.2.0, MySQLdb disables autocommit by default, as
-required by the DB-API standard (`PEP-249`_). If you are using InnoDB
-tables or some other type of transactional table type, you'll need
-to do connection.commit() before closing the connection, or else
-none of your changes will be written to the database.
-
-Conversely, you can also use connection.rollback() to throw away
-any changes you've made since the last commit.
-
-Important note: Some SQL statements -- specifically DDL statements
-like CREATE TABLE -- are non-transactional, so they can't be
-rolled back, and they cause pending transactions to commit.
-
-
-Other Errors
-------------
-
-  OperationalError: (1251, 'Client does not support authentication protocol requested by server; consider upgrading MySQL client')
-
-This means your server and client libraries are not the same version.
-More specifically, it probably means you have a 4.1 or newer server
-and 4.0 or older client. You can either upgrade the client side, or
-try some of the workarounds in `Password Hashing as of MySQL 4.1
-<http://dev.mysql.com/doc/refman/5.0/en/password-hashing.html>`_.
-
-
-Other Resources
----------------
-
-* Help forum. Please search before posting.
-
-* `Google <http://www.google.com/>`_
-
-* READ README!
-
-* Read the User's Guide
-
-* Read `PEP-249`_
-
-.. _`PEP-249`: https://www.python.org/dev/peps/pep-0249/
-
+====================================
+ MySQLdb Frequently Asked Questions
+====================================
+
+.. contents::
+..
+
+
+Build Errors
+------------
+
+  mysql.h: No such file or directory
+
+This almost always mean you don't have development packages
+installed. On some systems, C headers for various things (like MySQL)
+are distributed as a separate package. You'll need to figure out
+what that is and install it, but often the name ends with -devel.
+
+Another possibility: Some older versions of mysql_config behave oddly
+and may throw quotes around some of the path names, which confused
+MySQLdb-1.2.0. 1.2.1 works around these problems. If you see things
+like -I'/usr/local/include/mysql' in your compile command, that's
+probably the issue, but it shouldn't happen any more.
+
+
+ImportError
+-----------
+
+  ImportError: No module named _mysql
+
+If you see this, it's likely you did some wrong when installing
+MySQLdb; re-read (or read) README. _mysql is the low-level C module
+that interfaces with the MySQL client library.
+
+Various versions of MySQLdb in the past have had build issues on
+"weird" platforms; "weird" in this case means "not Linux", though
+generally there aren't problems on Unix/POSIX platforms, including
+BSDs and Mac OS X. Windows has been more problematic, in part because
+there is no `mysql_config` available in the Windows installation of
+MySQL. 1.2.1 solves most, if not all, of these problems, but you will
+still have to edit a configuration file so that the setup knows where
+to find MySQL and what libraries to include.
+
+
+  ImportError: libmysqlclient_r.so.14: cannot open shared object file: No such file or directory
+
+The number after .so may vary, but this means you have a version of
+MySQLdb compiled against one version of MySQL, and are now trying to
+run it against a different version. The shared library version tends
+to change between major releases.
+
+Solution: Rebuilt MySQLdb, or get the matching version of MySQL.
+
+Another thing that can cause this: The MySQL libraries may not be on
+your system path.
+
+Solutions:
+
+* set the LD_LIBRARY_PATH environment variable so that it includes
+  the path to the MySQL libraries.
+
+* set static=True in site.cfg for static linking
+
+* reconfigure your system so that the MySQL libraries are on the
+  default loader path. In Linux, you edit /etc/ld.so.conf and run
+  ldconfig. For Solaris, see `Linker and Libraries Guide
+  <http://docs.oracle.com/cd/E19253-01/817-1984/chapter6-63352/>`_.
+
+
+  ImportError: ld.so.1: python: fatal: libmtmalloc.so.1: DF_1_NOOPEN tagged object may not be dlopen()'ed
+
+This is a weird one from Solaris. What does it mean? I have no idea.
+However, things like this can happen if there is some sort of a compiler
+or environment mismatch between Python and MySQL. For example, on some
+commercial systems, you might have some code compiled with their own
+compiler, and other things compiled with GCC. They don't always mesh
+together. One way to encounter this is by getting binary packages from
+different vendors.
+
+Solution: Rebuild Python or MySQL (or maybe both) from source.
+
+  ImportError: dlopen(./_mysql.so, 2): Symbol not found: _sprintf$LDBLStub
+  Referenced from: ./_mysql.so
+  Expected in: dynamic lookup
+
+This is one from Mac OS X. It seems to have been a compiler mismatch,
+but this time between two different versions of GCC. It seems nearly
+every major release of GCC changes the ABI in some why, so linking
+code compiled with GCC-3.3 and GCC-4.0, for example, can be
+problematic.
+
+
+My data disappeared! (or won't go away!)
+----------------------------------------
+
+Starting with 1.2.0, MySQLdb disables autocommit by default, as
+required by the DB-API standard (`PEP-249`_). If you are using InnoDB
+tables or some other type of transactional table type, you'll need
+to do connection.commit() before closing the connection, or else
+none of your changes will be written to the database.
+
+Conversely, you can also use connection.rollback() to throw away
+any changes you've made since the last commit.
+
+Important note: Some SQL statements -- specifically DDL statements
+like CREATE TABLE -- are non-transactional, so they can't be
+rolled back, and they cause pending transactions to commit.
+
+
+Other Errors
+------------
+
+  OperationalError: (1251, 'Client does not support authentication protocol requested by server; consider upgrading MySQL client')
+
+This means your server and client libraries are not the same version.
+More specifically, it probably means you have a 4.1 or newer server
+and 4.0 or older client. You can either upgrade the client side, or
+try some of the workarounds in `Password Hashing as of MySQL 4.1
+<http://dev.mysql.com/doc/refman/5.0/en/password-hashing.html>`_.
+
+
+Other Resources
+---------------
+
+* Help forum. Please search before posting.
+
+* `Google <http://www.google.com/>`_
+
+* READ README!
+
+* Read the User's Guide
+
+* Read `PEP-249`_
+
+.. _`PEP-249`: https://www.python.org/dev/peps/pep-0249/
+
```

### Comparing `mysqlclient-2.2.0/doc/MySQLdb.rst` & `mysqlclient-2.2.0rc1/doc/MySQLdb.rst`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,62 +1,62 @@
-MySQLdb Package
-===============
-
-:mod:`MySQLdb` Package
-----------------------
-
-.. automodule:: MySQLdb
-    :members:
-    :undoc-members:
-    :show-inheritance:
-
-:mod:`MySQLdb.connections` Module
----------------------------------
-
-.. automodule:: MySQLdb.connections
-    :members: Connection
-    :undoc-members:
-
-:mod:`MySQLdb.converters` Module
---------------------------------
-
-.. automodule:: MySQLdb.converters
-    :members:
-    :undoc-members:
-
-:mod:`MySQLdb.cursors` Module
------------------------------
-
-.. automodule:: MySQLdb.cursors
-    :members:
-    :undoc-members:
-    :show-inheritance:
-
-:mod:`MySQLdb.times` Module
----------------------------
-
-.. automodule:: MySQLdb.times
-    :members:
-    :undoc-members:
-
-:mod:`MySQLdb._mysql` Module
-----------------------------
-
-.. automodule:: MySQLdb._mysql
-    :members:
-    :undoc-members:
-
-:mod:`MySQLdb._exceptions` Module
----------------------------------
-
-.. automodule:: MySQLdb._exceptions
-    :members:
-    :undoc-members:
-
-
-Subpackages
------------
-
-.. toctree::
-
-    MySQLdb.constants
-
+MySQLdb Package
+===============
+
+:mod:`MySQLdb` Package
+----------------------
+
+.. automodule:: MySQLdb
+    :members:
+    :undoc-members:
+    :show-inheritance:
+
+:mod:`MySQLdb.connections` Module
+---------------------------------
+
+.. automodule:: MySQLdb.connections
+    :members: Connection
+    :undoc-members:
+
+:mod:`MySQLdb.converters` Module
+--------------------------------
+
+.. automodule:: MySQLdb.converters
+    :members:
+    :undoc-members:
+
+:mod:`MySQLdb.cursors` Module
+-----------------------------
+
+.. automodule:: MySQLdb.cursors
+    :members:
+    :undoc-members:
+    :show-inheritance:
+
+:mod:`MySQLdb.times` Module
+---------------------------
+
+.. automodule:: MySQLdb.times
+    :members:
+    :undoc-members:
+
+:mod:`MySQLdb._mysql` Module
+----------------------------
+
+.. automodule:: MySQLdb._mysql
+    :members:
+    :undoc-members:
+
+:mod:`MySQLdb._exceptions` Module
+---------------------------------
+
+.. automodule:: MySQLdb._exceptions
+    :members:
+    :undoc-members:
+
+
+Subpackages
+-----------
+
+.. toctree::
+
+    MySQLdb.constants
+
```

### Comparing `mysqlclient-2.2.0/doc/conf.py` & `mysqlclient-2.2.0rc1/doc/conf.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,251 +1,251 @@
-#
-# MySQLdb documentation build configuration file, created by
-# sphinx-quickstart on Sun Oct 07 19:36:17 2012.
-#
-# This file is execfile()d with the current directory set to its containing dir.
-#
-# Note that not all possible configuration values are present in this
-# autogenerated file.
-#
-# All configuration values have a default; values that are commented out
-# serve to show the default.
-
-# skip flake8 and black for this file
-# flake8: noqa
-import sys
-import os
-
-# If extensions (or modules to document with autodoc) are in another directory,
-# add these directories to sys.path here. If the directory is relative to the
-# documentation root, use os.path.abspath to make it absolute, like shown here.
-# sys.path.insert(0, os.path.abspath(".."))
-
-# -- General configuration -----------------------------------------------------
-
-nitpick_ignore = [
-    ("py:class", "datetime.date"),
-    ("py:class", "datetime.time"),
-    ("py:class", "datetime.datetime"),
-]
-
-
-# If your documentation needs a minimal Sphinx version, state it here.
-# needs_sphinx = "1.0"
-
-# Add any Sphinx extension module names here, as strings. They can be extensions
-# coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
-extensions = ["sphinx.ext.autodoc"]
-
-# Add any paths that contain templates here, relative to this directory.
-templates_path = ["_templates"]
-
-# The suffix of source filenames.
-source_suffix = ".rst"
-
-# The encoding of source files.
-# source_encoding = "utf-8-sig"
-
-# The master toctree document.
-master_doc = "index"
-
-# General information about the project.
-project = "MySQLdb"
-copyright = "2012, Andy Dustman"
-
-# The version info for the project you're documenting, acts as replacement for
-# |version| and |release|, also used in various other places throughout the
-# built documents.
-#
-# The short X.Y version.
-version = "1.2"
-# The full version, including alpha/beta/rc tags.
-release = "1.2.4b4"
-
-# The language for content autogenerated by Sphinx. Refer to documentation
-# for a list of supported languages.
-# language = None
-
-# There are two options for replacing |today|: either, you set today to some
-# non-false value, then it is used:
-# today = ""
-# Else, today_fmt is used as the format for a strftime call.
-# today_fmt = "%B %d, %Y"
-
-# List of patterns, relative to source directory, that match files and
-# directories to ignore when looking for source files.
-exclude_patterns = ["_build"]
-
-# The reST default role (used for this markup: `text`) to use for all documents.
-# default_role = None
-
-# If true, '()' will be appended to :func: etc. cross-reference text.
-# add_function_parentheses = True
-
-# If true, the current module name will be prepended to all description
-# unit titles (such as .. function::).
-# add_module_names = True
-
-# If true, sectionauthor and moduleauthor directives will be shown in the
-# output. They are ignored by default.
-# show_authors = False
-
-# The name of the Pygments (syntax highlighting) style to use.
-pygments_style = "sphinx"
-
-# A list of ignored prefixes for module index sorting.
-# modindex_common_prefix = []
-
-
-# -- Options for HTML output ---------------------------------------------------
-
-# The theme to use for HTML and HTML Help pages.  See the documentation for
-# a list of builtin themes.
-html_theme = "default"
-
-# Theme options are theme-specific and customize the look and feel of a theme
-# further.  For a list of options available for each theme, see the
-# documentation.
-# html_theme_options = {}
-
-# Add any paths that contain custom themes here, relative to this directory.
-# html_theme_path = []
-
-# The name for this set of Sphinx documents.  If None, it defaults to
-# "<project> v<release> documentation".
-# html_title = None
-
-# A shorter title for the navigation bar.  Default is the same as html_title.
-# html_short_title = None
-
-# The name of an image file (relative to this directory) to place at the top
-# of the sidebar.
-# html_logo = None
-
-# The name of an image file (within the static path) to use as favicon of the
-# docs.  This file should be a Windows icon file (.ico) being 16x16 or 32x32
-# pixels large.
-# html_favicon = None
-
-# Add any paths that contain custom static files (such as style sheets) here,
-# relative to this directory. They are copied after the builtin static files,
-# so a file named "default.css" will overwrite the builtin "default.css".
-html_static_path = ["_static"]
-
-# If not '', a 'Last updated on:' timestamp is inserted at every page bottom,
-# using the given strftime format.
-# html_last_updated_fmt = "%b %d, %Y"
-
-# If true, SmartyPants will be used to convert quotes and dashes to
-# typographically correct entities.
-# html_use_smartypants = True
-
-# Custom sidebar templates, maps document names to template names.
-# html_sidebars = {}
-
-# Additional templates that should be rendered to pages, maps page names to
-# template names.
-# html_additional_pages = {}
-
-# If false, no module index is generated.
-# html_domain_indices = True
-
-# If false, no index is generated.
-# html_use_index = True
-
-# If true, the index is split into individual pages for each letter.
-# html_split_index = False
-
-# If true, links to the reST sources are added to the pages.
-# html_show_sourcelink = True
-
-# If true, "Created using Sphinx" is shown in the HTML footer. Default is True.
-# html_show_sphinx = True
-
-# If true, "(C) Copyright ..." is shown in the HTML footer. Default is True.
-# html_show_copyright = True
-
-# If true, an OpenSearch description file will be output, and all pages will
-# contain a <link> tag referring to it.  The value of this option must be the
-# base URL from which the finished HTML is served.
-# html_use_opensearch = ""
-
-# This is the file name suffix for HTML files (e.g. ".xhtml").
-# html_file_suffix = None
-
-# Output file base name for HTML help builder.
-htmlhelp_basename = "MySQLdbdoc"
-
-
-# -- Options for LaTeX output --------------------------------------------------
-
-latex_elements = {
-    # The paper size ('letterpaper' or 'a4paper').
-    #'papersize': 'letterpaper',
-    # The font size ('10pt', '11pt' or '12pt').
-    #'pointsize': '10pt',
-    # Additional stuff for the LaTeX preamble.
-    #'preamble': '',
-}
-
-# Grouping the document tree into LaTeX files. List of tuples
-# (source start file, target name, title, author, documentclass [howto/manual]).
-latex_documents = [
-    ("index", "MySQLdb.tex", "MySQLdb Documentation", "Andy Dustman", "manual"),
-]
-
-# The name of an image file (relative to this directory) to place at the top of
-# the title page.
-# latex_logo = None
-
-# For "manual" documents, if this is true, then toplevel headings are parts,
-# not chapters.
-# latex_use_parts = False
-
-# If true, show page references after internal links.
-# latex_show_pagerefs = False
-
-# If true, show URL addresses after external links.
-# latex_show_urls = False
-
-# Documents to append as an appendix to all manuals.
-# latex_appendices = []
-
-# If false, no module index is generated.
-# latex_domain_indices = True
-
-
-# -- Options for manual page output --------------------------------------------
-
-# One entry per manual page. List of tuples
-# (source start file, name, description, authors, manual section).
-man_pages = [("index", "mysqldb", "MySQLdb Documentation", ["Andy Dustman"], 1)]
-
-# If true, show URL addresses after external links.
-# man_show_urls = False
-
-
-# -- Options for Texinfo output ------------------------------------------------
-
-# Grouping the document tree into Texinfo files. List of tuples
-# (source start file, target name, title, author,
-#  dir menu entry, description, category)
-texinfo_documents = [
-    (
-        "index",
-        "MySQLdb",
-        "MySQLdb Documentation",
-        "Andy Dustman",
-        "MySQLdb",
-        "One line description of project.",
-        "Miscellaneous",
-    ),
-]
-
-# Documents to append as an appendix to all manuals.
-# texinfo_appendices = []
-
-# If false, no module index is generated.
-# texinfo_domain_indices = True
-
-# How to display URL addresses: 'footnote', 'no', or 'inline'.
-# texinfo_show_urls = 'footnote'
+#
+# MySQLdb documentation build configuration file, created by
+# sphinx-quickstart on Sun Oct 07 19:36:17 2012.
+#
+# This file is execfile()d with the current directory set to its containing dir.
+#
+# Note that not all possible configuration values are present in this
+# autogenerated file.
+#
+# All configuration values have a default; values that are commented out
+# serve to show the default.
+
+# skip flake8 and black for this file
+# flake8: noqa
+import sys
+import os
+
+# If extensions (or modules to document with autodoc) are in another directory,
+# add these directories to sys.path here. If the directory is relative to the
+# documentation root, use os.path.abspath to make it absolute, like shown here.
+# sys.path.insert(0, os.path.abspath(".."))
+
+# -- General configuration -----------------------------------------------------
+
+nitpick_ignore = [
+    ("py:class", "datetime.date"),
+    ("py:class", "datetime.time"),
+    ("py:class", "datetime.datetime"),
+]
+
+
+# If your documentation needs a minimal Sphinx version, state it here.
+# needs_sphinx = "1.0"
+
+# Add any Sphinx extension module names here, as strings. They can be extensions
+# coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
+extensions = ["sphinx.ext.autodoc"]
+
+# Add any paths that contain templates here, relative to this directory.
+templates_path = ["_templates"]
+
+# The suffix of source filenames.
+source_suffix = ".rst"
+
+# The encoding of source files.
+# source_encoding = "utf-8-sig"
+
+# The master toctree document.
+master_doc = "index"
+
+# General information about the project.
+project = "MySQLdb"
+copyright = "2012, Andy Dustman"
+
+# The version info for the project you're documenting, acts as replacement for
+# |version| and |release|, also used in various other places throughout the
+# built documents.
+#
+# The short X.Y version.
+version = "1.2"
+# The full version, including alpha/beta/rc tags.
+release = "1.2.4b4"
+
+# The language for content autogenerated by Sphinx. Refer to documentation
+# for a list of supported languages.
+# language = None
+
+# There are two options for replacing |today|: either, you set today to some
+# non-false value, then it is used:
+# today = ""
+# Else, today_fmt is used as the format for a strftime call.
+# today_fmt = "%B %d, %Y"
+
+# List of patterns, relative to source directory, that match files and
+# directories to ignore when looking for source files.
+exclude_patterns = ["_build"]
+
+# The reST default role (used for this markup: `text`) to use for all documents.
+# default_role = None
+
+# If true, '()' will be appended to :func: etc. cross-reference text.
+# add_function_parentheses = True
+
+# If true, the current module name will be prepended to all description
+# unit titles (such as .. function::).
+# add_module_names = True
+
+# If true, sectionauthor and moduleauthor directives will be shown in the
+# output. They are ignored by default.
+# show_authors = False
+
+# The name of the Pygments (syntax highlighting) style to use.
+pygments_style = "sphinx"
+
+# A list of ignored prefixes for module index sorting.
+# modindex_common_prefix = []
+
+
+# -- Options for HTML output ---------------------------------------------------
+
+# The theme to use for HTML and HTML Help pages.  See the documentation for
+# a list of builtin themes.
+html_theme = "default"
+
+# Theme options are theme-specific and customize the look and feel of a theme
+# further.  For a list of options available for each theme, see the
+# documentation.
+# html_theme_options = {}
+
+# Add any paths that contain custom themes here, relative to this directory.
+# html_theme_path = []
+
+# The name for this set of Sphinx documents.  If None, it defaults to
+# "<project> v<release> documentation".
+# html_title = None
+
+# A shorter title for the navigation bar.  Default is the same as html_title.
+# html_short_title = None
+
+# The name of an image file (relative to this directory) to place at the top
+# of the sidebar.
+# html_logo = None
+
+# The name of an image file (within the static path) to use as favicon of the
+# docs.  This file should be a Windows icon file (.ico) being 16x16 or 32x32
+# pixels large.
+# html_favicon = None
+
+# Add any paths that contain custom static files (such as style sheets) here,
+# relative to this directory. They are copied after the builtin static files,
+# so a file named "default.css" will overwrite the builtin "default.css".
+html_static_path = ["_static"]
+
+# If not '', a 'Last updated on:' timestamp is inserted at every page bottom,
+# using the given strftime format.
+# html_last_updated_fmt = "%b %d, %Y"
+
+# If true, SmartyPants will be used to convert quotes and dashes to
+# typographically correct entities.
+# html_use_smartypants = True
+
+# Custom sidebar templates, maps document names to template names.
+# html_sidebars = {}
+
+# Additional templates that should be rendered to pages, maps page names to
+# template names.
+# html_additional_pages = {}
+
+# If false, no module index is generated.
+# html_domain_indices = True
+
+# If false, no index is generated.
+# html_use_index = True
+
+# If true, the index is split into individual pages for each letter.
+# html_split_index = False
+
+# If true, links to the reST sources are added to the pages.
+# html_show_sourcelink = True
+
+# If true, "Created using Sphinx" is shown in the HTML footer. Default is True.
+# html_show_sphinx = True
+
+# If true, "(C) Copyright ..." is shown in the HTML footer. Default is True.
+# html_show_copyright = True
+
+# If true, an OpenSearch description file will be output, and all pages will
+# contain a <link> tag referring to it.  The value of this option must be the
+# base URL from which the finished HTML is served.
+# html_use_opensearch = ""
+
+# This is the file name suffix for HTML files (e.g. ".xhtml").
+# html_file_suffix = None
+
+# Output file base name for HTML help builder.
+htmlhelp_basename = "MySQLdbdoc"
+
+
+# -- Options for LaTeX output --------------------------------------------------
+
+latex_elements = {
+    # The paper size ('letterpaper' or 'a4paper').
+    #'papersize': 'letterpaper',
+    # The font size ('10pt', '11pt' or '12pt').
+    #'pointsize': '10pt',
+    # Additional stuff for the LaTeX preamble.
+    #'preamble': '',
+}
+
+# Grouping the document tree into LaTeX files. List of tuples
+# (source start file, target name, title, author, documentclass [howto/manual]).
+latex_documents = [
+    ("index", "MySQLdb.tex", "MySQLdb Documentation", "Andy Dustman", "manual"),
+]
+
+# The name of an image file (relative to this directory) to place at the top of
+# the title page.
+# latex_logo = None
+
+# For "manual" documents, if this is true, then toplevel headings are parts,
+# not chapters.
+# latex_use_parts = False
+
+# If true, show page references after internal links.
+# latex_show_pagerefs = False
+
+# If true, show URL addresses after external links.
+# latex_show_urls = False
+
+# Documents to append as an appendix to all manuals.
+# latex_appendices = []
+
+# If false, no module index is generated.
+# latex_domain_indices = True
+
+
+# -- Options for manual page output --------------------------------------------
+
+# One entry per manual page. List of tuples
+# (source start file, name, description, authors, manual section).
+man_pages = [("index", "mysqldb", "MySQLdb Documentation", ["Andy Dustman"], 1)]
+
+# If true, show URL addresses after external links.
+# man_show_urls = False
+
+
+# -- Options for Texinfo output ------------------------------------------------
+
+# Grouping the document tree into Texinfo files. List of tuples
+# (source start file, target name, title, author,
+#  dir menu entry, description, category)
+texinfo_documents = [
+    (
+        "index",
+        "MySQLdb",
+        "MySQLdb Documentation",
+        "Andy Dustman",
+        "MySQLdb",
+        "One line description of project.",
+        "Miscellaneous",
+    ),
+]
+
+# Documents to append as an appendix to all manuals.
+# texinfo_appendices = []
+
+# If false, no module index is generated.
+# texinfo_domain_indices = True
+
+# How to display URL addresses: 'footnote', 'no', or 'inline'.
+# texinfo_show_urls = 'footnote'
```

### Comparing `mysqlclient-2.2.0/doc/user_guide.rst` & `mysqlclient-2.2.0rc1/doc/user_guide.rst`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,712 +1,712 @@
-====================
-MySQLdb User's Guide
-====================
-
-.. contents::
-..
-
-Introduction
-------------
-
-MySQLdb is an interface to the popular MySQL
-database server that provides the Python database API.
-
-Installation
-------------
-
-The ``README`` file has complete installation instructions.
-
-
-MySQLdb._mysql
---------------
-
-If you want to write applications which are portable across databases,
-use MySQLdb_, and avoid using this module directly. ``MySQLdb._mysql``
-provides an interface which mostly implements the MySQL C API. For
-more information, see the `MySQL documentation`_. The documentation
-for this module is intentionally weak because you probably should use
-the higher-level MySQLdb module. If you really need it, use the
-standard MySQL docs and transliterate as necessary.
-
-.. _`MySQL documentation`: https://dev.mysql.com/doc/
-
-
-MySQL C API translation
-.......................
-
-The MySQL C API has been wrapped in an object-oriented way. The only
-MySQL data structures which are implemented are the ``MYSQL``
-(database connection handle) and ``MYSQL_RES`` (result handle)
-types. In general, any function which takes ``MYSQL *mysql`` as an
-argument is now a method of the connection object, and any function
-which takes ``MYSQL_RES *result`` as an argument is a method of the
-result object. Functions requiring none of the MySQL data structures
-are implemented as functions in the module. Functions requiring one of
-the other MySQL data structures are generally not implemented.
-Deprecated functions are not implemented. In all cases, the ``mysql_``
-prefix is dropped from the name. Most of the ``conn`` methods listed
-are also available as MySQLdb Connection object methods. Their use is
-non-portable.
-
-MySQL C API function mapping
-............................
-
-=================================== ==================================
-      C API                         ``_mysql``
-=================================== ==================================
- ``mysql_affected_rows()``          ``conn.affected_rows()``
- ``mysql_autocommit()``             ``conn.autocommit()``
- ``mysql_character_set_name()``     ``conn.character_set_name()``
- ``mysql_close()``                  ``conn.close()``
- ``mysql_commit()``                 ``conn.commit()``
- ``mysql_connect()``                ``_mysql.connect()``
- ``mysql_data_seek()``              ``result.data_seek()``
- ``mysql_debug()``                  ``_mysql.debug()``
- ``mysql_dump_debug_info``          ``conn.dump_debug_info()``
- ``mysql_escape_string()``          ``_mysql.escape_string()``
- ``mysql_fetch_row()``              ``result.fetch_row()``
- ``mysql_get_character_set_info()`` ``conn.get_character_set_info()``
- ``mysql_get_client_info()``        ``_mysql.get_client_info()``
- ``mysql_get_host_info()``          ``conn.get_host_info()``
- ``mysql_get_proto_info()``         ``conn.get_proto_info()``
- ``mysql_get_server_info()``        ``conn.get_server_info()``
- ``mysql_info()``                   ``conn.info()``
- ``mysql_insert_id()``              ``conn.insert_id()``
- ``mysql_num_fields()``             ``result.num_fields()``
- ``mysql_num_rows()``               ``result.num_rows()``
- ``mysql_options()``                various options to ``_mysql.connect()``
- ``mysql_ping()``                   ``conn.ping()``
- ``mysql_query()``                  ``conn.query()``
- ``mysql_real_connect()``           ``_mysql.connect()``
- ``mysql_real_query()``             ``conn.query()``
- ``mysql_real_escape_string()``     ``conn.escape_string()``
- ``mysql_rollback()``               ``conn.rollback()``
- ``mysql_row_seek()``               ``result.row_seek()``
- ``mysql_row_tell()``               ``result.row_tell()``
- ``mysql_select_db()``              ``conn.select_db()``
- ``mysql_set_character_set()``      ``conn.set_character_set()``
- ``mysql_ssl_set()``                ``ssl`` option to ``_mysql.connect()``
- ``mysql_stat()``                   ``conn.stat()``
- ``mysql_store_result()``           ``conn.store_result()``
- ``mysql_thread_id()``              ``conn.thread_id()``
- ``mysql_use_result()``             ``conn.use_result()``
- ``mysql_warning_count()``          ``conn.warning_count()``
- ``CLIENT_*``                       ``MySQLdb.constants.CLIENT.*``
- ``CR_*``                           ``MySQLdb.constants.CR.*``
- ``ER_*``                           ``MySQLdb.constants.ER.*``
- ``FIELD_TYPE_*``                   ``MySQLdb.constants.FIELD_TYPE.*``
- ``FLAG_*``                         ``MySQLdb.constants.FLAG.*``
-=================================== ==================================
-
-
-Some _mysql examples
-....................
-
-Okay, so you want to use ``_mysql`` anyway. Here are some examples.
-
-The simplest possible database connection is::
-
-    from MySQLdb import _mysql
-    db=_mysql.connect()
-
-This creates a connection to the MySQL server running on the local
-machine using the standard UNIX socket (or named pipe on Windows),
-your login name (from the USER environment variable), no password, and
-does not ``USE`` a database.  Chances are you need to supply more
-information.::
-
-    db=_mysql.connect("localhost","joebob","moonpie","thangs")
-
-This creates a connection to the MySQL server running on the local
-machine via a UNIX socket (or named pipe), the user name "joebob", the
-password "moonpie", and selects the initial database "thangs".
-
-We haven't even begun to touch upon all the parameters ``connect()``
-can take.  For this reason, I prefer to use keyword parameters::
-
-    db=_mysql.connect(host="localhost",user="joebob",
-                      password="moonpie",database="thangs")
-
-This does exactly what the last example did, but is arguably easier to
-read. But since the default host is "localhost", and if your login
-name really was "joebob", you could shorten it to this::
-
-    db=_mysql.connect(password="moonpie",database="thangs")
-
-UNIX sockets and named pipes don't work over a network, so if you
-specify a host other than localhost, TCP will be used, and you can
-specify an odd port if you need to (the default port is 3306)::
-
-    db=_mysql.connect(host="outhouse",port=3307,password="moonpie",database="thangs")
-
-If you really had to, you could connect to the local host with TCP by
-specifying the full host name, or 127.0.0.1.
-
-Generally speaking, putting passwords in your code is not such a good
-idea::
-
-    db=_mysql.connect(host="outhouse",database="thangs",read_default_file="~/.my.cnf")
-
-This does what the previous example does, but gets the username and
-password and other parameters from ~/.my.cnf (UNIX-like systems). Read
-about `option files`_ for more details.
-
-.. _`option files`: http://dev.mysql.com/doc/refman/en/option-files.html
-
-So now you have an open connection as ``db`` and want to do a
-query. Well, there are no cursors in MySQL, and no parameter
-substitution, so you have to pass a complete query string to
-``db.query()``::
-
-    db.query("""SELECT spam, eggs, sausage FROM breakfast
-             WHERE price < 5""")
-
-There's no return value from this, but exceptions can be raised. The
-exceptions are defined in a separate module, ``MySQLdb._exceptions``,
-but ``MySQLdb._mysql`` exports them. Read DB API specification PEP-249_ to
-find out what they are, or you can use the catch-all ``MySQLError``.
-
-.. _PEP-249: https://www.python.org/dev/peps/pep-0249/
-
-At this point your query has been executed and you need to get the
-results. You have two options::
-
-    r=db.store_result()
-    # ...or...
-    r=db.use_result()
-
-Both methods return a result object. What's the difference?
-``store_result()`` returns the entire result set to the client
-immediately. If your result set is really large, this could be a
-problem. One way around this is to add a ``LIMIT`` clause to your
-query, to limit the number of rows returned. The other is to use
-``use_result()``, which keeps the result set in the server and sends
-it row-by-row when you fetch. This does, however, tie up server
-resources, and it ties up the connection: You cannot do any more
-queries until you have fetched **all** the rows. Generally I
-recommend using ``store_result()`` unless your result set is really
-huge and you can't use ``LIMIT`` for some reason.
-
-Now, for actually getting real results::
-
-    >>> r.fetch_row()
-    (('3','2','0'),)
-
-This might look a little odd. The first thing you should know is,
-``fetch_row()`` takes some additional parameters. The first one is,
-how many rows (``maxrows``) should be returned. By default, it returns
-one row. It may return fewer rows than you asked for, but never
-more. If you set ``maxrows=0``, it returns all rows of the result
-set. If you ever get an empty tuple back, you ran out of rows.
-
-The second parameter (``how``) tells it how the row should be
-represented. By default, it is zero which means, return as a tuple.
-``how=1`` means, return it as a dictionary, where the keys are the
-column names, or ``table.column`` if there are two columns with the
-same name (say, from a join). ``how=2`` means the same as ``how=1``
-except that the keys are *always* ``table.column``; this is for
-compatibility with the old ``Mysqldb`` module.
-
-OK, so why did we get a 1-tuple with a tuple inside? Because we
-implicitly asked for one row, since we didn't specify ``maxrows``.
-
-The other oddity is: Assuming these are numeric columns, why are they
-returned as strings? Because MySQL returns all data as strings and
-expects you to convert it yourself. This would be a real pain in the
-ass, but in fact, ``MySQLdb._mysql`` can do this for you. (And ``MySQLdb``
-does do this for you.) To have automatic type conversion done, you
-need to create a type converter dictionary, and pass this to
-``connect()`` as the ``conv`` keyword parameter.
-
-The keys of ``conv`` should be MySQL column types, which in the
-C API are ``FIELD_TYPE_*``. You can get these values like this::
-
-    from MySQLdb.constants import FIELD_TYPE
-
-By default, any column type that can't be found in ``conv`` is
-returned as a string, which works for a lot of stuff. For our
-purposes, we probably want this::
-
-    my_conv = { FIELD_TYPE.LONG: int }
-
-This means, if it's a ``FIELD_TYPE_LONG``, call the builtin ``int()``
-function on it.  Note that ``FIELD_TYPE_LONG`` is an ``INTEGER``
-column, which corresponds to a C ``long``, which is also the type used
-for a normal Python integer. But beware: If it's really an ``UNSIGNED
-INTEGER`` column, this could cause overflows. For this reason,
-``MySQLdb`` actually uses ``long()`` to do the conversion. But we'll
-ignore this potential problem for now.
-
-Then if you use ``db=_mysql.connect(conv=my_conv...)``, the
-results will come back ``((3, 2, 0),)``, which is what you would
-expect.
-
-MySQLdb
--------
-
-MySQLdb is a thin Python wrapper around ``_mysql`` which makes it
-compatible with the Python DB API interface (version 2).  In reality,
-a fair amount of the code which implements the API is in ``_mysql``
-for the sake of efficiency.
-
-The DB API specification PEP-249_ should be your primary guide for
-using this module. Only deviations from the spec and other
-database-dependent things will be documented here.
-
-Functions and attributes
-........................
-
-Only a few top-level functions and attributes are defined within
-MySQLdb.
-
-connect(parameters...)
-         Constructor for creating a connection to the
-         database. Returns a Connection Object. Parameters are the
-         same as for the MySQL C API.  In addition, there are a few
-         additional keywords that correspond to what you would pass
-         ``mysql_options()`` before connecting. Note that some
-         parameters must be specified as keyword arguments! The
-         default value for each parameter is NULL or zero, as
-         appropriate. Consult the MySQL documentation for more
-         details. The important parameters are:
-
-         host
-            name of host to connect to. Default: use the local host
-            via a UNIX socket (where applicable)
-
-         user
-            user to authenticate as. Default: current effective user.
-
-         password
-            password to authenticate with. Default: no password.
-
-         database
-            database to use. Default: no default database.
-
-         port
-            TCP port of MySQL server. Default: standard port (3306).
-
-         unix_socket
-            location of UNIX socket. Default: use default location or
-            TCP for remote hosts.
-
-         conv
-            type conversion dictionary.  Default: a copy of
-            ``MySQLdb.converters.conversions``
-
-         compress
-            Enable protocol compression. Default: no compression.
-
-         connect_timeout
-            Abort if connect is not completed within
-            given number of seconds. Default: no timeout (?)
-
-         named_pipe
-            Use a named pipe (Windows). Default: don't.
-
-         init_command
-            Initial command to issue to server upon
-            connection. Default: Nothing.
-
-         read_default_file
-            MySQL configuration file to read; see
-            the MySQL documentation for ``mysql_options()``.
-
-         read_default_group
-            Default group to read; see the MySQL
-            documentation for ``mysql_options()``.
-
-         cursorclass
-            cursor class that ``cursor()`` uses, unless
-            overridden. Default: ``MySQLdb.cursors.Cursor``.  *This
-            must be a keyword parameter.*
-
-         use_unicode
-            If True, CHAR and VARCHAR and TEXT columns are returned as
-            Unicode strings, using the configured character set. It is
-            best to set the default encoding in the server
-            configuration, or client configuration (read with
-            read_default_file).  If you change the character set after
-            connecting (MySQL-4.1 and later), you'll need to put the
-            correct character set name in connection.charset.
-
-            If False, text-like columns are returned as normal strings,
-            but you can always write Unicode strings.
-
-            *This must be a keyword parameter.*
-
-         charset
-            If present, the connection character set will be changed
-            to this character set, if they are not equal. Support for
-            changing the character set requires MySQL-4.1 and later
-            server; if the server is too old, UnsupportedError will be
-            raised. This option implies use_unicode=True, but you can
-            override this with use_unicode=False, though you probably
-            shouldn't.
-
-            If not present, the default character set is used.
-
-            *This must be a keyword parameter.*
-
-         collation
-            If ``charset`` and ``collation`` are both supplied, the
-            character set and collation for the current connection
-            will be set.
-
-            If omitted, empty string, or None, the default collation
-            for the ``charset`` is implied by the database server.
-
-            To learn more about the quiddities of character sets and
-            collations, consult the `MySQL docs
-            <https://dev.mysql.com/doc/refman/8.0/en/charset.html>`_
-            and `MariaDB docs
-            <https://mariadb.com/kb/en/character-sets/>`_
-
-            *This must be a keyword parameter.*
-
-         sql_mode
-            If present, the session SQL mode will be set to the given
-            string. For more information on sql_mode, see the MySQL
-            documentation. Only available for 4.1 and newer servers.
-
-            If not present, the session SQL mode will be unchanged.
-
-            *This must be a keyword parameter.*
-
-         ssl_mode
-            If present, specify the security settings for the
-            connection to the server. For more information on ssl_mode,
-            see the MySQL documentation. Only one of 'DISABLED',
-            'PREFERRED', 'REQUIRED', 'VERIFY_CA', 'VERIFY_IDENTITY'
-            can be specified.
-
-            If not present, the session ssl_mode will be unchanged,
-            but in version 5.7 and later, the default is PREFERRED.
-
-            *This must be a keyword parameter.*
-
-         ssl
-            This parameter takes a dictionary or mapping, where the
-            keys are parameter names used by the mysql_ssl_set_ MySQL
-            C API call. If this is set, it initiates an SSL connection
-            to the server; if there is no SSL support in the client,
-            an exception is raised. *This must be a keyword
-            parameter.*
-
-.. _mysql_ssl_set: http://dev.mysql.com/doc/refman/en/mysql-ssl-set.html
-
-
-apilevel
-      String constant stating the supported DB API level. '2.0'
-
-threadsafety
-      Integer constant stating the level of thread safety the
-      interface supports. This is set to 1, which means: Threads may
-      share the module.
-
-      The MySQL protocol can not handle multiple threads using the
-      same connection at once. Some earlier versions of MySQLdb
-      utilized locking to achieve a threadsafety of 2. While this is
-      not terribly hard to accomplish using the standard Cursor class
-      (which uses ``mysql_store_result()``), it is complicated by
-      SSCursor (which uses ``mysql_use_result()``; with the latter you
-      must ensure all the rows have been read before another query can
-      be executed.  It is further complicated by the addition of
-      transactions, since transactions start when a cursor executes a
-      query, but end when ``COMMIT`` or ``ROLLBACK`` is executed by
-      the Connection object.  Two threads simply cannot share a
-      connection while a transaction is in progress, in addition to
-      not being able to share it during query execution. This
-      excessively complicated the code to the point where it just
-      isn't worth it.
-
-      The general upshot of this is: Don't share connections between
-      threads. It's really not worth your effort or mine, and in the
-      end, will probably hurt performance, since the MySQL server runs
-      a separate thread for each connection.  You can certainly do
-      things like cache connections in a pool, and give those
-      connections to one thread at a time. If you let two threads use
-      a connection simultaneously, the MySQL client library will
-      probably upchuck and die.  You have been warned.
-
-
-charset
-      The character set used by the connection. In MySQL-4.1 and newer,
-      it is possible (but not recommended) to change the connection's
-      character set with an SQL statement. If you do this, you'll also
-      need to change this attribute. Otherwise, you'll get encoding
-      errors.
-
-paramstyle
-      String constant stating the type of parameter marker formatting
-      expected by the interface. Set to 'format' = ANSI C printf
-      format codes, e.g. '...WHERE name=%s'. If a mapping object is
-      used for conn.execute(), then the interface actually uses
-      'pyformat' = Python extended format codes, e.g. '...WHERE
-      name=%(name)s'. However, the API does not presently allow the
-      specification of more than one style in paramstyle.
-
-      Note that any literal percent signs in the query string passed
-      to execute() must be escaped, i.e. %%.
-
-      Parameter placeholders can **only** be used to insert column
-      values. They can **not** be used for other parts of SQL, such as
-      table names, statements, etc.
-
-conv
-      A dictionary or mapping which controls how types are converted
-      from MySQL to Python and vice versa.
-
-      If the key is a MySQL type (from ``FIELD_TYPE.*``), then the value
-      can be either:
-
-      * a callable object which takes a string argument (the MySQL
-        value), returning a Python value
-
-      * a sequence of 2-tuples, where the first value is a combination
-        of flags from ``MySQLdb.constants.FLAG``, and the second value
-        is a function as above. The sequence is tested until the flags
-        on the field match those of the first value. If both values
-        are None, then the default conversion is done. Presently this
-        is only used to distinguish TEXT and BLOB columns.
-
-      If the key is a Python type or class, then the value is a
-      callable Python object (usually a function) taking two arguments
-      (value to convert, and the conversion dictionary) which converts
-      values of this type to a SQL literal string value.
-
-      This is initialized with reasonable defaults for most
-      types. When creating a Connection object, you can pass your own
-      type converter dictionary as a keyword parameter. Otherwise, it
-      uses a copy of ``MySQLdb.converters.conversions``.  Several
-      non-standard types are returned as strings, which is how MySQL
-      returns all columns. For more details, see the built-in module
-      documentation.
-
-
-Connection Objects
-..................
-
-Connection objects are returned by the ``connect()`` function.
-
-commit()
-      If the database and the tables support transactions, this
-      commits the current transaction; otherwise this method
-      successfully does nothing.
-
-rollback()
-      If the database and tables support transactions, this rolls back
-      (cancels) the current transaction; otherwise a
-      ``NotSupportedError`` is raised.
-
-cursor([cursorclass])
-      MySQL does not support cursors; however, cursors are easily
-      emulated.  You can supply an alternative cursor class as an
-      optional parameter.  If this is not present, it defaults to the
-      value given when creating the connection object, or the standard
-      ``Cursor`` class. Also see the additional supplied cursor
-      classes in the usage section.
-
-There are many more methods defined on the connection object which
-are MySQL-specific. For more information on them, consult the internal
-documentation using ``pydoc``.
-
-
-Cursor Objects
-..............
-
-callproc(procname, args)
-      Calls stored procedure procname with the sequence of arguments
-      in args. Returns the original arguments. Stored procedure
-      support only works with MySQL-5.0 and newer.
-
-      **Compatibility note:** PEP-249_ specifies that if there are
-      OUT or INOUT parameters, the modified values are to be
-      returned. This is not consistently possible with MySQL. Stored
-      procedure arguments must be passed as server variables, and
-      can only be returned with a SELECT statement. Since a stored
-      procedure may return zero or more result sets, it is impossible
-      for MySQLdb to determine if there are result sets to fetch
-      before the modified parameters are accessible.
-
-      The parameters are stored in the server as @_*procname*_*n*,
-      where *n* is the position of the parameter. I.e., if you
-      cursor.callproc('foo', (a, b, c)), the parameters will be
-      accessible by a SELECT statement as @_foo_0, @_foo_1, and
-      @_foo_2.
-
-      **Compatibility note:** It appears that the mere act of
-      executing the CALL statement produces an empty result set, which
-      appears after any result sets which might be generated by the
-      stored procedure. Thus, you will always need to use nextset() to
-      advance result sets.
-
-close()
-      Closes the cursor. Future operations raise ``ProgrammingError``.
-      If you are using server-side cursors, it is very important to
-      close the cursor when you are done with it and before creating a
-      new one.
-
-info()
-      Returns some information about the last query. Normally
-      you don't need to check this. If there are any MySQL
-      warnings, it will cause a Warning to be issued through
-      the Python warning module. By default, Warning causes a
-      message to appear on the console. However, it is possible
-      to filter these out or cause Warning to be raised as exception.
-      See the MySQL docs for ``mysql_info()``, and the Python warning
-      module. (Non-standard)
-
-setinputsizes()
-      Does nothing, successfully.
-
-setoutputsizes()
-      Does nothing, successfully.
-
-nextset()
-      Advances the cursor to the next result set, discarding the remaining
-      rows in the current result set. If there are no additional result
-      sets, it returns None; otherwise it returns a true value.
-
-      Note that MySQL doesn't support multiple result sets until 4.1.
-
-
-Some examples
-.............
-
-The ``connect()`` method works nearly the same as with `MySQLDB._mysql`_::
-
-    import MySQLdb
-    db=MySQLdb.connect(password="moonpie",database="thangs")
-
-To perform a query, you first need a cursor, and then you can execute
-queries on it::
-
-    c=db.cursor()
-    max_price=5
-    c.execute("""SELECT spam, eggs, sausage FROM breakfast
-              WHERE price < %s""", (max_price,))
-
-In this example, ``max_price=5`` Why, then, use ``%s`` in the
-string? Because MySQLdb will convert it to a SQL literal value, which
-is the string '5'. When it's finished, the query will actually say,
-"...WHERE price < 5".
-
-Why the tuple? Because the DB API requires you to pass in any
-parameters as a sequence. Due to the design of the parser, (max_price)
-is interpreted as using algebraic grouping and simply as max_price and
-not a tuple. Adding a comma, i.e. (max_price,) forces it to make a
-tuple.
-
-And now, the results::
-
-    >>> c.fetchone()
-    (3L, 2L, 0L)
-
-Quite unlike the ``_mysql`` example, this returns a single tuple,
-which is the row, and the values are properly converted by default...
-except... What's with the L's?
-
-As mentioned earlier, while MySQL's INTEGER column translates
-perfectly into a Python integer, UNSIGNED INTEGER could overflow, so
-these values are converted to Python long integers instead.
-
-If you wanted more rows, you could use ``c.fetchmany(n)`` or
-``c.fetchall()``. These do exactly what you think they do. On
-``c.fetchmany(n)``, the ``n`` is optional and defaults to
-``c.arraysize``, which is normally 1. Both of these methods return a
-sequence of rows, or an empty sequence if there are no more rows.  If
-you use a weird cursor class, the rows themselves might not be tuples.
-
-Note that in contrast to the above, ``c.fetchone()`` returns ``None``
-when there are no more rows to fetch.
-
-The only other method you are very likely to use is when you have to
-do a multi-row insert::
-
-   c.executemany(
-         """INSERT INTO breakfast (name, spam, eggs, sausage, price)
-         VALUES (%s, %s, %s, %s, %s)""",
-         [
-         ("Spam and Sausage Lover's Plate", 5, 1, 8, 7.95 ),
-         ("Not So Much Spam Plate", 3, 2, 0, 3.95 ),
-         ("Don't Wany ANY SPAM! Plate", 0, 4, 3, 5.95 )
-         ] )
-
-Here we are inserting three rows of five values. Notice that there is
-a mix of types (strings, ints, floats) though we still only use
-``%s``. And also note that we only included format strings for one
-row. MySQLdb picks those out and duplicates them for each row.
-
-Using and extending
--------------------
-
-In general, it is probably wise to not directly interact with the DB
-API except for small applications. Databases, even SQL databases, vary
-widely in capabilities and may have non-standard features. The DB API
-does a good job of providing a reasonably portable interface but some
-methods are non-portable. Specifically, the parameters accepted by
-``connect()`` are completely implementation-dependent.
-
-If you believe your application may need to run on several different
-databases, the author recommends the following approach, based on
-personal experience: Write a simplified API for your application which
-implements the specific queries and operations your application needs
-to perform. Implement this API as a base class which should be have
-few database dependencies, and then derive a subclass from this which
-implements the necessary dependencies. In this way, porting your
-application to a new database should be a relatively simple matter of
-creating a new subclass, assuming the new database is reasonably
-standard.
-
-Because MySQLdb's Connection and Cursor objects are written in Python,
-you can easily derive your own subclasses. There are several Cursor
-classes in MySQLdb.cursors:
-
-BaseCursor
-    The base class for Cursor objects.  This does not raise Warnings.
-
-CursorStoreResultMixIn
-    Causes the Cursor to use the ``mysql_store_result()`` function to
-    get the query result. The entire result set is stored on the
-    client side.
-
-CursorUseResultMixIn
-    Causes the cursor to use the ``mysql_use_result()`` function to
-    get the query result. The result set is stored on the server side
-    and is transferred row by row using fetch operations.
-
-CursorTupleRowsMixIn
-    Causes the cursor to return rows as a tuple of the column values.
-
-CursorDictRowsMixIn
-    Causes the cursor to return rows as a dictionary, where the keys
-    are column names and the values are column values. Note that if
-    the column names are not unique, i.e., you are selecting from two
-    tables that share column names, some of them will be rewritten as
-    ``table.column``.  This can be avoided by using the SQL ``AS``
-    keyword. (This is yet-another reason not to use ``*`` in SQL
-    queries, particularly where ``JOIN`` is involved.)
-
-Cursor
-    The default cursor class. This class is composed of
-    ``CursorStoreResultMixIn``, ``CursorTupleRowsMixIn``, and
-    ``BaseCursor``, i.e. uses ``mysql_store_result()`` and returns
-    rows as tuples.
-
-DictCursor
-    Like ``Cursor`` except it returns rows as dictionaries.
-
-SSCursor
-    A "server-side" cursor. Like ``Cursor`` but uses
-    ``CursorUseResultMixIn``.  Use only if you are dealing with
-    potentially large result sets.
-
-SSDictCursor
-    Like ``SSCursor`` except it returns rows as dictionaries.
-
-
-
-:Title: MySQLdb: a Python interface for MySQL
-:Author: Andy Dustman
-:Version: $Revision$
+====================
+MySQLdb User's Guide
+====================
+
+.. contents::
+..
+
+Introduction
+------------
+
+MySQLdb is an interface to the popular MySQL
+database server that provides the Python database API.
+
+Installation
+------------
+
+The ``README`` file has complete installation instructions.
+
+
+MySQLdb._mysql
+--------------
+
+If you want to write applications which are portable across databases,
+use MySQLdb_, and avoid using this module directly. ``MySQLdb._mysql``
+provides an interface which mostly implements the MySQL C API. For
+more information, see the `MySQL documentation`_. The documentation
+for this module is intentionally weak because you probably should use
+the higher-level MySQLdb module. If you really need it, use the
+standard MySQL docs and transliterate as necessary.
+
+.. _`MySQL documentation`: https://dev.mysql.com/doc/
+
+
+MySQL C API translation
+.......................
+
+The MySQL C API has been wrapped in an object-oriented way. The only
+MySQL data structures which are implemented are the ``MYSQL``
+(database connection handle) and ``MYSQL_RES`` (result handle)
+types. In general, any function which takes ``MYSQL *mysql`` as an
+argument is now a method of the connection object, and any function
+which takes ``MYSQL_RES *result`` as an argument is a method of the
+result object. Functions requiring none of the MySQL data structures
+are implemented as functions in the module. Functions requiring one of
+the other MySQL data structures are generally not implemented.
+Deprecated functions are not implemented. In all cases, the ``mysql_``
+prefix is dropped from the name. Most of the ``conn`` methods listed
+are also available as MySQLdb Connection object methods. Their use is
+non-portable.
+
+MySQL C API function mapping
+............................
+
+=================================== ==================================
+      C API                         ``_mysql``
+=================================== ==================================
+ ``mysql_affected_rows()``          ``conn.affected_rows()``
+ ``mysql_autocommit()``             ``conn.autocommit()``
+ ``mysql_character_set_name()``     ``conn.character_set_name()``
+ ``mysql_close()``                  ``conn.close()``
+ ``mysql_commit()``                 ``conn.commit()``
+ ``mysql_connect()``                ``_mysql.connect()``
+ ``mysql_data_seek()``              ``result.data_seek()``
+ ``mysql_debug()``                  ``_mysql.debug()``
+ ``mysql_dump_debug_info``          ``conn.dump_debug_info()``
+ ``mysql_escape_string()``          ``_mysql.escape_string()``
+ ``mysql_fetch_row()``              ``result.fetch_row()``
+ ``mysql_get_character_set_info()`` ``conn.get_character_set_info()``
+ ``mysql_get_client_info()``        ``_mysql.get_client_info()``
+ ``mysql_get_host_info()``          ``conn.get_host_info()``
+ ``mysql_get_proto_info()``         ``conn.get_proto_info()``
+ ``mysql_get_server_info()``        ``conn.get_server_info()``
+ ``mysql_info()``                   ``conn.info()``
+ ``mysql_insert_id()``              ``conn.insert_id()``
+ ``mysql_num_fields()``             ``result.num_fields()``
+ ``mysql_num_rows()``               ``result.num_rows()``
+ ``mysql_options()``                various options to ``_mysql.connect()``
+ ``mysql_ping()``                   ``conn.ping()``
+ ``mysql_query()``                  ``conn.query()``
+ ``mysql_real_connect()``           ``_mysql.connect()``
+ ``mysql_real_query()``             ``conn.query()``
+ ``mysql_real_escape_string()``     ``conn.escape_string()``
+ ``mysql_rollback()``               ``conn.rollback()``
+ ``mysql_row_seek()``               ``result.row_seek()``
+ ``mysql_row_tell()``               ``result.row_tell()``
+ ``mysql_select_db()``              ``conn.select_db()``
+ ``mysql_set_character_set()``      ``conn.set_character_set()``
+ ``mysql_ssl_set()``                ``ssl`` option to ``_mysql.connect()``
+ ``mysql_stat()``                   ``conn.stat()``
+ ``mysql_store_result()``           ``conn.store_result()``
+ ``mysql_thread_id()``              ``conn.thread_id()``
+ ``mysql_use_result()``             ``conn.use_result()``
+ ``mysql_warning_count()``          ``conn.warning_count()``
+ ``CLIENT_*``                       ``MySQLdb.constants.CLIENT.*``
+ ``CR_*``                           ``MySQLdb.constants.CR.*``
+ ``ER_*``                           ``MySQLdb.constants.ER.*``
+ ``FIELD_TYPE_*``                   ``MySQLdb.constants.FIELD_TYPE.*``
+ ``FLAG_*``                         ``MySQLdb.constants.FLAG.*``
+=================================== ==================================
+
+
+Some _mysql examples
+....................
+
+Okay, so you want to use ``_mysql`` anyway. Here are some examples.
+
+The simplest possible database connection is::
+
+    from MySQLdb import _mysql
+    db=_mysql.connect()
+
+This creates a connection to the MySQL server running on the local
+machine using the standard UNIX socket (or named pipe on Windows),
+your login name (from the USER environment variable), no password, and
+does not ``USE`` a database.  Chances are you need to supply more
+information.::
+
+    db=_mysql.connect("localhost","joebob","moonpie","thangs")
+
+This creates a connection to the MySQL server running on the local
+machine via a UNIX socket (or named pipe), the user name "joebob", the
+password "moonpie", and selects the initial database "thangs".
+
+We haven't even begun to touch upon all the parameters ``connect()``
+can take.  For this reason, I prefer to use keyword parameters::
+
+    db=_mysql.connect(host="localhost",user="joebob",
+                      password="moonpie",database="thangs")
+
+This does exactly what the last example did, but is arguably easier to
+read. But since the default host is "localhost", and if your login
+name really was "joebob", you could shorten it to this::
+
+    db=_mysql.connect(password="moonpie",database="thangs")
+
+UNIX sockets and named pipes don't work over a network, so if you
+specify a host other than localhost, TCP will be used, and you can
+specify an odd port if you need to (the default port is 3306)::
+
+    db=_mysql.connect(host="outhouse",port=3307,password="moonpie",database="thangs")
+
+If you really had to, you could connect to the local host with TCP by
+specifying the full host name, or 127.0.0.1.
+
+Generally speaking, putting passwords in your code is not such a good
+idea::
+
+    db=_mysql.connect(host="outhouse",database="thangs",read_default_file="~/.my.cnf")
+
+This does what the previous example does, but gets the username and
+password and other parameters from ~/.my.cnf (UNIX-like systems). Read
+about `option files`_ for more details.
+
+.. _`option files`: http://dev.mysql.com/doc/refman/en/option-files.html
+
+So now you have an open connection as ``db`` and want to do a
+query. Well, there are no cursors in MySQL, and no parameter
+substitution, so you have to pass a complete query string to
+``db.query()``::
+
+    db.query("""SELECT spam, eggs, sausage FROM breakfast
+             WHERE price < 5""")
+
+There's no return value from this, but exceptions can be raised. The
+exceptions are defined in a separate module, ``MySQLdb._exceptions``,
+but ``MySQLdb._mysql`` exports them. Read DB API specification PEP-249_ to
+find out what they are, or you can use the catch-all ``MySQLError``.
+
+.. _PEP-249: https://www.python.org/dev/peps/pep-0249/
+
+At this point your query has been executed and you need to get the
+results. You have two options::
+
+    r=db.store_result()
+    # ...or...
+    r=db.use_result()
+
+Both methods return a result object. What's the difference?
+``store_result()`` returns the entire result set to the client
+immediately. If your result set is really large, this could be a
+problem. One way around this is to add a ``LIMIT`` clause to your
+query, to limit the number of rows returned. The other is to use
+``use_result()``, which keeps the result set in the server and sends
+it row-by-row when you fetch. This does, however, tie up server
+resources, and it ties up the connection: You cannot do any more
+queries until you have fetched **all** the rows. Generally I
+recommend using ``store_result()`` unless your result set is really
+huge and you can't use ``LIMIT`` for some reason.
+
+Now, for actually getting real results::
+
+    >>> r.fetch_row()
+    (('3','2','0'),)
+
+This might look a little odd. The first thing you should know is,
+``fetch_row()`` takes some additional parameters. The first one is,
+how many rows (``maxrows``) should be returned. By default, it returns
+one row. It may return fewer rows than you asked for, but never
+more. If you set ``maxrows=0``, it returns all rows of the result
+set. If you ever get an empty tuple back, you ran out of rows.
+
+The second parameter (``how``) tells it how the row should be
+represented. By default, it is zero which means, return as a tuple.
+``how=1`` means, return it as a dictionary, where the keys are the
+column names, or ``table.column`` if there are two columns with the
+same name (say, from a join). ``how=2`` means the same as ``how=1``
+except that the keys are *always* ``table.column``; this is for
+compatibility with the old ``Mysqldb`` module.
+
+OK, so why did we get a 1-tuple with a tuple inside? Because we
+implicitly asked for one row, since we didn't specify ``maxrows``.
+
+The other oddity is: Assuming these are numeric columns, why are they
+returned as strings? Because MySQL returns all data as strings and
+expects you to convert it yourself. This would be a real pain in the
+ass, but in fact, ``MySQLdb._mysql`` can do this for you. (And ``MySQLdb``
+does do this for you.) To have automatic type conversion done, you
+need to create a type converter dictionary, and pass this to
+``connect()`` as the ``conv`` keyword parameter.
+
+The keys of ``conv`` should be MySQL column types, which in the
+C API are ``FIELD_TYPE_*``. You can get these values like this::
+
+    from MySQLdb.constants import FIELD_TYPE
+
+By default, any column type that can't be found in ``conv`` is
+returned as a string, which works for a lot of stuff. For our
+purposes, we probably want this::
+
+    my_conv = { FIELD_TYPE.LONG: int }
+
+This means, if it's a ``FIELD_TYPE_LONG``, call the builtin ``int()``
+function on it.  Note that ``FIELD_TYPE_LONG`` is an ``INTEGER``
+column, which corresponds to a C ``long``, which is also the type used
+for a normal Python integer. But beware: If it's really an ``UNSIGNED
+INTEGER`` column, this could cause overflows. For this reason,
+``MySQLdb`` actually uses ``long()`` to do the conversion. But we'll
+ignore this potential problem for now.
+
+Then if you use ``db=_mysql.connect(conv=my_conv...)``, the
+results will come back ``((3, 2, 0),)``, which is what you would
+expect.
+
+MySQLdb
+-------
+
+MySQLdb is a thin Python wrapper around ``_mysql`` which makes it
+compatible with the Python DB API interface (version 2).  In reality,
+a fair amount of the code which implements the API is in ``_mysql``
+for the sake of efficiency.
+
+The DB API specification PEP-249_ should be your primary guide for
+using this module. Only deviations from the spec and other
+database-dependent things will be documented here.
+
+Functions and attributes
+........................
+
+Only a few top-level functions and attributes are defined within
+MySQLdb.
+
+connect(parameters...)
+         Constructor for creating a connection to the
+         database. Returns a Connection Object. Parameters are the
+         same as for the MySQL C API.  In addition, there are a few
+         additional keywords that correspond to what you would pass
+         ``mysql_options()`` before connecting. Note that some
+         parameters must be specified as keyword arguments! The
+         default value for each parameter is NULL or zero, as
+         appropriate. Consult the MySQL documentation for more
+         details. The important parameters are:
+
+         host
+            name of host to connect to. Default: use the local host
+            via a UNIX socket (where applicable)
+
+         user
+            user to authenticate as. Default: current effective user.
+
+         password
+            password to authenticate with. Default: no password.
+
+         database
+            database to use. Default: no default database.
+
+         port
+            TCP port of MySQL server. Default: standard port (3306).
+
+         unix_socket
+            location of UNIX socket. Default: use default location or
+            TCP for remote hosts.
+
+         conv
+            type conversion dictionary.  Default: a copy of
+            ``MySQLdb.converters.conversions``
+
+         compress
+            Enable protocol compression. Default: no compression.
+
+         connect_timeout
+            Abort if connect is not completed within
+            given number of seconds. Default: no timeout (?)
+
+         named_pipe
+            Use a named pipe (Windows). Default: don't.
+
+         init_command
+            Initial command to issue to server upon
+            connection. Default: Nothing.
+
+         read_default_file
+            MySQL configuration file to read; see
+            the MySQL documentation for ``mysql_options()``.
+
+         read_default_group
+            Default group to read; see the MySQL
+            documentation for ``mysql_options()``.
+
+         cursorclass
+            cursor class that ``cursor()`` uses, unless
+            overridden. Default: ``MySQLdb.cursors.Cursor``.  *This
+            must be a keyword parameter.*
+
+         use_unicode
+            If True, CHAR and VARCHAR and TEXT columns are returned as
+            Unicode strings, using the configured character set. It is
+            best to set the default encoding in the server
+            configuration, or client configuration (read with
+            read_default_file).  If you change the character set after
+            connecting (MySQL-4.1 and later), you'll need to put the
+            correct character set name in connection.charset.
+
+            If False, text-like columns are returned as normal strings,
+            but you can always write Unicode strings.
+
+            *This must be a keyword parameter.*
+
+         charset
+            If present, the connection character set will be changed
+            to this character set, if they are not equal. Support for
+            changing the character set requires MySQL-4.1 and later
+            server; if the server is too old, UnsupportedError will be
+            raised. This option implies use_unicode=True, but you can
+            override this with use_unicode=False, though you probably
+            shouldn't.
+
+            If not present, the default character set is used.
+
+            *This must be a keyword parameter.*
+
+         collation
+            If ``charset`` and ``collation`` are both supplied, the
+            character set and collation for the current connection
+            will be set.
+
+            If omitted, empty string, or None, the default collation
+            for the ``charset`` is implied by the database server.
+
+            To learn more about the quiddities of character sets and
+            collations, consult the `MySQL docs
+            <https://dev.mysql.com/doc/refman/8.0/en/charset.html>`_
+            and `MariaDB docs
+            <https://mariadb.com/kb/en/character-sets/>`_
+
+            *This must be a keyword parameter.*
+
+         sql_mode
+            If present, the session SQL mode will be set to the given
+            string. For more information on sql_mode, see the MySQL
+            documentation. Only available for 4.1 and newer servers.
+
+            If not present, the session SQL mode will be unchanged.
+
+            *This must be a keyword parameter.*
+
+         ssl_mode
+            If present, specify the security settings for the
+            connection to the server. For more information on ssl_mode,
+            see the MySQL documentation. Only one of 'DISABLED',
+            'PREFERRED', 'REQUIRED', 'VERIFY_CA', 'VERIFY_IDENTITY'
+            can be specified.
+
+            If not present, the session ssl_mode will be unchanged,
+            but in version 5.7 and later, the default is PREFERRED.
+
+            *This must be a keyword parameter.*
+
+         ssl
+            This parameter takes a dictionary or mapping, where the
+            keys are parameter names used by the mysql_ssl_set_ MySQL
+            C API call. If this is set, it initiates an SSL connection
+            to the server; if there is no SSL support in the client,
+            an exception is raised. *This must be a keyword
+            parameter.*
+
+.. _mysql_ssl_set: http://dev.mysql.com/doc/refman/en/mysql-ssl-set.html
+
+
+apilevel
+      String constant stating the supported DB API level. '2.0'
+
+threadsafety
+      Integer constant stating the level of thread safety the
+      interface supports. This is set to 1, which means: Threads may
+      share the module.
+
+      The MySQL protocol can not handle multiple threads using the
+      same connection at once. Some earlier versions of MySQLdb
+      utilized locking to achieve a threadsafety of 2. While this is
+      not terribly hard to accomplish using the standard Cursor class
+      (which uses ``mysql_store_result()``), it is complicated by
+      SSCursor (which uses ``mysql_use_result()``; with the latter you
+      must ensure all the rows have been read before another query can
+      be executed.  It is further complicated by the addition of
+      transactions, since transactions start when a cursor executes a
+      query, but end when ``COMMIT`` or ``ROLLBACK`` is executed by
+      the Connection object.  Two threads simply cannot share a
+      connection while a transaction is in progress, in addition to
+      not being able to share it during query execution. This
+      excessively complicated the code to the point where it just
+      isn't worth it.
+
+      The general upshot of this is: Don't share connections between
+      threads. It's really not worth your effort or mine, and in the
+      end, will probably hurt performance, since the MySQL server runs
+      a separate thread for each connection.  You can certainly do
+      things like cache connections in a pool, and give those
+      connections to one thread at a time. If you let two threads use
+      a connection simultaneously, the MySQL client library will
+      probably upchuck and die.  You have been warned.
+
+
+charset
+      The character set used by the connection. In MySQL-4.1 and newer,
+      it is possible (but not recommended) to change the connection's
+      character set with an SQL statement. If you do this, you'll also
+      need to change this attribute. Otherwise, you'll get encoding
+      errors.
+
+paramstyle
+      String constant stating the type of parameter marker formatting
+      expected by the interface. Set to 'format' = ANSI C printf
+      format codes, e.g. '...WHERE name=%s'. If a mapping object is
+      used for conn.execute(), then the interface actually uses
+      'pyformat' = Python extended format codes, e.g. '...WHERE
+      name=%(name)s'. However, the API does not presently allow the
+      specification of more than one style in paramstyle.
+
+      Note that any literal percent signs in the query string passed
+      to execute() must be escaped, i.e. %%.
+
+      Parameter placeholders can **only** be used to insert column
+      values. They can **not** be used for other parts of SQL, such as
+      table names, statements, etc.
+
+conv
+      A dictionary or mapping which controls how types are converted
+      from MySQL to Python and vice versa.
+
+      If the key is a MySQL type (from ``FIELD_TYPE.*``), then the value
+      can be either:
+
+      * a callable object which takes a string argument (the MySQL
+        value), returning a Python value
+
+      * a sequence of 2-tuples, where the first value is a combination
+        of flags from ``MySQLdb.constants.FLAG``, and the second value
+        is a function as above. The sequence is tested until the flags
+        on the field match those of the first value. If both values
+        are None, then the default conversion is done. Presently this
+        is only used to distinguish TEXT and BLOB columns.
+
+      If the key is a Python type or class, then the value is a
+      callable Python object (usually a function) taking two arguments
+      (value to convert, and the conversion dictionary) which converts
+      values of this type to a SQL literal string value.
+
+      This is initialized with reasonable defaults for most
+      types. When creating a Connection object, you can pass your own
+      type converter dictionary as a keyword parameter. Otherwise, it
+      uses a copy of ``MySQLdb.converters.conversions``.  Several
+      non-standard types are returned as strings, which is how MySQL
+      returns all columns. For more details, see the built-in module
+      documentation.
+
+
+Connection Objects
+..................
+
+Connection objects are returned by the ``connect()`` function.
+
+commit()
+      If the database and the tables support transactions, this
+      commits the current transaction; otherwise this method
+      successfully does nothing.
+
+rollback()
+      If the database and tables support transactions, this rolls back
+      (cancels) the current transaction; otherwise a
+      ``NotSupportedError`` is raised.
+
+cursor([cursorclass])
+      MySQL does not support cursors; however, cursors are easily
+      emulated.  You can supply an alternative cursor class as an
+      optional parameter.  If this is not present, it defaults to the
+      value given when creating the connection object, or the standard
+      ``Cursor`` class. Also see the additional supplied cursor
+      classes in the usage section.
+
+There are many more methods defined on the connection object which
+are MySQL-specific. For more information on them, consult the internal
+documentation using ``pydoc``.
+
+
+Cursor Objects
+..............
+
+callproc(procname, args)
+      Calls stored procedure procname with the sequence of arguments
+      in args. Returns the original arguments. Stored procedure
+      support only works with MySQL-5.0 and newer.
+
+      **Compatibility note:** PEP-249_ specifies that if there are
+      OUT or INOUT parameters, the modified values are to be
+      returned. This is not consistently possible with MySQL. Stored
+      procedure arguments must be passed as server variables, and
+      can only be returned with a SELECT statement. Since a stored
+      procedure may return zero or more result sets, it is impossible
+      for MySQLdb to determine if there are result sets to fetch
+      before the modified parameters are accessible.
+
+      The parameters are stored in the server as @_*procname*_*n*,
+      where *n* is the position of the parameter. I.e., if you
+      cursor.callproc('foo', (a, b, c)), the parameters will be
+      accessible by a SELECT statement as @_foo_0, @_foo_1, and
+      @_foo_2.
+
+      **Compatibility note:** It appears that the mere act of
+      executing the CALL statement produces an empty result set, which
+      appears after any result sets which might be generated by the
+      stored procedure. Thus, you will always need to use nextset() to
+      advance result sets.
+
+close()
+      Closes the cursor. Future operations raise ``ProgrammingError``.
+      If you are using server-side cursors, it is very important to
+      close the cursor when you are done with it and before creating a
+      new one.
+
+info()
+      Returns some information about the last query. Normally
+      you don't need to check this. If there are any MySQL
+      warnings, it will cause a Warning to be issued through
+      the Python warning module. By default, Warning causes a
+      message to appear on the console. However, it is possible
+      to filter these out or cause Warning to be raised as exception.
+      See the MySQL docs for ``mysql_info()``, and the Python warning
+      module. (Non-standard)
+
+setinputsizes()
+      Does nothing, successfully.
+
+setoutputsizes()
+      Does nothing, successfully.
+
+nextset()
+      Advances the cursor to the next result set, discarding the remaining
+      rows in the current result set. If there are no additional result
+      sets, it returns None; otherwise it returns a true value.
+
+      Note that MySQL doesn't support multiple result sets until 4.1.
+
+
+Some examples
+.............
+
+The ``connect()`` method works nearly the same as with `MySQLDB._mysql`_::
+
+    import MySQLdb
+    db=MySQLdb.connect(password="moonpie",database="thangs")
+
+To perform a query, you first need a cursor, and then you can execute
+queries on it::
+
+    c=db.cursor()
+    max_price=5
+    c.execute("""SELECT spam, eggs, sausage FROM breakfast
+              WHERE price < %s""", (max_price,))
+
+In this example, ``max_price=5`` Why, then, use ``%s`` in the
+string? Because MySQLdb will convert it to a SQL literal value, which
+is the string '5'. When it's finished, the query will actually say,
+"...WHERE price < 5".
+
+Why the tuple? Because the DB API requires you to pass in any
+parameters as a sequence. Due to the design of the parser, (max_price)
+is interpreted as using algebraic grouping and simply as max_price and
+not a tuple. Adding a comma, i.e. (max_price,) forces it to make a
+tuple.
+
+And now, the results::
+
+    >>> c.fetchone()
+    (3L, 2L, 0L)
+
+Quite unlike the ``_mysql`` example, this returns a single tuple,
+which is the row, and the values are properly converted by default...
+except... What's with the L's?
+
+As mentioned earlier, while MySQL's INTEGER column translates
+perfectly into a Python integer, UNSIGNED INTEGER could overflow, so
+these values are converted to Python long integers instead.
+
+If you wanted more rows, you could use ``c.fetchmany(n)`` or
+``c.fetchall()``. These do exactly what you think they do. On
+``c.fetchmany(n)``, the ``n`` is optional and defaults to
+``c.arraysize``, which is normally 1. Both of these methods return a
+sequence of rows, or an empty sequence if there are no more rows.  If
+you use a weird cursor class, the rows themselves might not be tuples.
+
+Note that in contrast to the above, ``c.fetchone()`` returns ``None``
+when there are no more rows to fetch.
+
+The only other method you are very likely to use is when you have to
+do a multi-row insert::
+
+   c.executemany(
+         """INSERT INTO breakfast (name, spam, eggs, sausage, price)
+         VALUES (%s, %s, %s, %s, %s)""",
+         [
+         ("Spam and Sausage Lover's Plate", 5, 1, 8, 7.95 ),
+         ("Not So Much Spam Plate", 3, 2, 0, 3.95 ),
+         ("Don't Wany ANY SPAM! Plate", 0, 4, 3, 5.95 )
+         ] )
+
+Here we are inserting three rows of five values. Notice that there is
+a mix of types (strings, ints, floats) though we still only use
+``%s``. And also note that we only included format strings for one
+row. MySQLdb picks those out and duplicates them for each row.
+
+Using and extending
+-------------------
+
+In general, it is probably wise to not directly interact with the DB
+API except for small applications. Databases, even SQL databases, vary
+widely in capabilities and may have non-standard features. The DB API
+does a good job of providing a reasonably portable interface but some
+methods are non-portable. Specifically, the parameters accepted by
+``connect()`` are completely implementation-dependent.
+
+If you believe your application may need to run on several different
+databases, the author recommends the following approach, based on
+personal experience: Write a simplified API for your application which
+implements the specific queries and operations your application needs
+to perform. Implement this API as a base class which should be have
+few database dependencies, and then derive a subclass from this which
+implements the necessary dependencies. In this way, porting your
+application to a new database should be a relatively simple matter of
+creating a new subclass, assuming the new database is reasonably
+standard.
+
+Because MySQLdb's Connection and Cursor objects are written in Python,
+you can easily derive your own subclasses. There are several Cursor
+classes in MySQLdb.cursors:
+
+BaseCursor
+    The base class for Cursor objects.  This does not raise Warnings.
+
+CursorStoreResultMixIn
+    Causes the Cursor to use the ``mysql_store_result()`` function to
+    get the query result. The entire result set is stored on the
+    client side.
+
+CursorUseResultMixIn
+    Causes the cursor to use the ``mysql_use_result()`` function to
+    get the query result. The result set is stored on the server side
+    and is transferred row by row using fetch operations.
+
+CursorTupleRowsMixIn
+    Causes the cursor to return rows as a tuple of the column values.
+
+CursorDictRowsMixIn
+    Causes the cursor to return rows as a dictionary, where the keys
+    are column names and the values are column values. Note that if
+    the column names are not unique, i.e., you are selecting from two
+    tables that share column names, some of them will be rewritten as
+    ``table.column``.  This can be avoided by using the SQL ``AS``
+    keyword. (This is yet-another reason not to use ``*`` in SQL
+    queries, particularly where ``JOIN`` is involved.)
+
+Cursor
+    The default cursor class. This class is composed of
+    ``CursorStoreResultMixIn``, ``CursorTupleRowsMixIn``, and
+    ``BaseCursor``, i.e. uses ``mysql_store_result()`` and returns
+    rows as tuples.
+
+DictCursor
+    Like ``Cursor`` except it returns rows as dictionaries.
+
+SSCursor
+    A "server-side" cursor. Like ``Cursor`` but uses
+    ``CursorUseResultMixIn``.  Use only if you are dealing with
+    potentially large result sets.
+
+SSDictCursor
+    Like ``SSCursor`` except it returns rows as dictionaries.
+
+
+
+:Title: MySQLdb: a Python interface for MySQL
+:Author: Andy Dustman
+:Version: $Revision$
```

### Comparing `mysqlclient-2.2.0/pyproject.toml` & `mysqlclient-2.2.0rc1/pyproject.toml`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-[project]
-name = "mysqlclient"
-# version = "2.2.0dev0"
-description = "Python interface to MySQL"
-readme = "README.md"
-requires-python = ">=3.8"
-authors = [
-    {name = "Inada Naoki", email = "songofacandy@gmail.com"}
-]
-license = {text = "GNU General Public License v2 (GPLv2)"}
-keywords = ["MySQL"]
-classifiers = [
-    "Development Status :: 5 - Production/Stable",
-    "Environment :: Other Environment",
-    "License :: OSI Approved :: GNU General Public License (GPL)",
-    "Operating System :: MacOS :: MacOS X",
-    "Operating System :: Microsoft :: Windows :: Windows NT/2000",
-    "Operating System :: OS Independent",
-    "Operating System :: POSIX",
-    "Operating System :: POSIX :: Linux",
-    "Operating System :: Unix",
-    "Programming Language :: C",
-    "Programming Language :: Python",
-    "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
-    "Topic :: Database",
-    "Topic :: Database :: Database Engines/Servers",
-]
-dynamic = ["version"]
-
-[project.urls]
-Project = "https://github.com/PyMySQL/mysqlclient"
-Documentation = "https://mysqlclient.readthedocs.io/"
-
-[build-system]
-requires = ["setuptools>=61"]
-build-backend = "setuptools.build_meta"
-
-[tool.setuptools]
-package-dir = {"" = "src"}
-
-[tool.setuptools.packages.find]
-namespaces = false
-where = ["src"]
-include = ["MySQLdb*"]
-
-[tool.setuptools.dynamic]
-version = {attr = "MySQLdb.release.__version__"}
+[project]
+name = "mysqlclient"
+# version = "2.2.0dev0"
+description = "Python interface to MySQL"
+readme = "README.md"
+requires-python = ">=3.8"
+authors = [
+    {name = "Inada Naoki", email = "songofacandy@gmail.com"}
+]
+license = {text = "GNU General Public License v2 (GPLv2)"}
+keywords = ["MySQL"]
+classifiers = [
+    "Development Status :: 5 - Production/Stable",
+    "Environment :: Other Environment",
+    "License :: OSI Approved :: GNU General Public License (GPL)",
+    "Operating System :: MacOS :: MacOS X",
+    "Operating System :: Microsoft :: Windows :: Windows NT/2000",
+    "Operating System :: OS Independent",
+    "Operating System :: POSIX",
+    "Operating System :: POSIX :: Linux",
+    "Operating System :: Unix",
+    "Programming Language :: C",
+    "Programming Language :: Python",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Topic :: Database",
+    "Topic :: Database :: Database Engines/Servers",
+]
+dynamic = ["version"]
+
+[project.urls]
+Project = "https://github.com/PyMySQL/mysqlclient"
+Documentation = "https://mysqlclient.readthedocs.io/"
+
+[build-system]
+requires = ["setuptools>=61"]
+build-backend = "setuptools.build_meta"
+
+[tool.setuptools]
+package-dir = {"" = "src"}
+
+[tool.setuptools.packages.find]
+namespaces = false
+where = ["src"]
+include = ["MySQLdb*"]
+
+[tool.setuptools.dynamic]
+version = {attr = "MySQLdb.release.__version__"}
```

### Comparing `mysqlclient-2.2.0/setup.py` & `mysqlclient-2.2.0rc1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,167 +1,171 @@
-#!/usr/bin/env python
-import os
-import subprocess
-import sys
-
-import setuptools
-from configparser import ConfigParser
-
-
-release_info = {}
-with open("src/MySQLdb/release.py", encoding="utf-8") as f:
-    exec(f.read(), None, release_info)
-
-
-def find_package_name():
-    """Get available pkg-config package name"""
-    packages = ["mysqlclient", "mariadb"]
-    for pkg in packages:
-        try:
-            cmd = f"pkg-config --exists {pkg}"
-            print(f"Trying {cmd}")
-            subprocess.check_call(cmd, shell=True)
-        except subprocess.CalledProcessError as err:
-            print(err)
-        else:
-            return pkg
-    raise Exception(
-        "Can not find valid pkg-config name.\n"
-        "Specify MYSQLCLIENT_CFLAGS and MYSQLCLIENT_LDFLAGS env vars manually"
-    )
-
-
-def get_config_posix(options=None):
-    # allow a command-line option to override the base config file to permit
-    # a static build to be created via requirements.txt
-    # TODO: find a better way for
-    static = False
-    if "--static" in sys.argv:
-        static = True
-        sys.argv.remove("--static")
-
-    ldflags = os.environ.get("MYSQLCLIENT_LDFLAGS")
-    cflags = os.environ.get("MYSQLCLIENT_CFLAGS")
-
-    pkg_name = None
-    static_opt = " --static" if static else ""
-    if not (cflags and ldflags):
-        pkg_name = find_package_name()
-    if not cflags:
-        cflags = subprocess.check_output(
-            f"pkg-config{static_opt} --cflags {pkg_name}", encoding="utf-8", shell=True
-        )
-    if not ldflags:
-        ldflags = subprocess.check_output(
-            f"pkg-config{static_opt} --libs {pkg_name}", encoding="utf-8", shell=True
-        )
-
-    cflags = cflags.split()
-    for f in cflags:
-        if f.startswith("-std="):
-            break
-    else:
-        cflags += ["-std=c99"]
-
-    ldflags = ldflags.split()
-
-    define_macros = [
-        ("version_info", release_info["version_info"]),
-        ("__version__", release_info["__version__"]),
-    ]
-
-    ext_options = dict(
-        extra_compile_args=cflags,
-        extra_link_args=ldflags,
-        define_macros=define_macros,
-    )
-    # newer versions of gcc require libstdc++ if doing a static build
-    if static:
-        ext_options["language"] = "c++"
-
-    return ext_options
-
-
-def get_config_win32(options):
-    client = "mariadbclient"
-    connector = os.environ.get("MYSQLCLIENT_CONNECTOR", options.get("connector"))
-    if not connector:
-        connector = os.path.join(
-            os.environ["ProgramFiles"], "MariaDB", "MariaDB Connector C"
-        )
-
-    extra_objects = []
-
-    library_dirs = [
-        os.path.join(connector, "lib", "mariadb"),
-        os.path.join(connector, "lib"),
-    ]
-    libraries = [
-        "kernel32",
-        "advapi32",
-        "wsock32",
-        "shlwapi",
-        "Ws2_32",
-        "crypt32",
-        "secur32",
-        "bcrypt",
-        client,
-    ]
-    include_dirs = [
-        os.path.join(connector, "include", "mariadb"),
-        os.path.join(connector, "include"),
-    ]
-
-    extra_link_args = ["/MANIFEST"]
-
-    define_macros = [
-        ("version_info", release_info["version_info"]),
-        ("__version__", release_info["__version__"]),
-    ]
-
-    ext_options = dict(
-        library_dirs=library_dirs,
-        libraries=libraries,
-        extra_link_args=extra_link_args,
-        include_dirs=include_dirs,
-        extra_objects=extra_objects,
-        define_macros=define_macros,
-    )
-    return ext_options
-
-
-def enabled(options, option):
-    value = options[option]
-    s = value.lower()
-    if s in ("yes", "true", "1", "y"):
-        return True
-    elif s in ("no", "false", "0", "n"):
-        return False
-    else:
-        raise ValueError(f"Unknown value {value} for option {option}")
-
-
-def get_options():
-    config = ConfigParser()
-    config.read(["site.cfg"])
-    options = dict(config.items("options"))
-    options["static"] = enabled(options, "static")
-    return options
-
-
-if sys.platform == "win32":
-    ext_options = get_config_win32(get_options())
-else:
-    ext_options = get_config_posix(get_options())
-
-print("# Options for building extention module:")
-for k, v in ext_options.items():
-    print(f"  {k}: {v}")
-
-ext_modules = [
-    setuptools.Extension(
-        "MySQLdb._mysql",
-        sources=["src/MySQLdb/_mysql.c"],
-        **ext_options,
-    )
-]
-setuptools.setup(ext_modules=ext_modules)
+#!/usr/bin/env python
+import os
+import subprocess
+import sys
+
+import setuptools
+from configparser import ConfigParser
+
+
+release_info = {}
+with open("src/MySQLdb/release.py", encoding="utf-8") as f:
+    exec(f.read(), None, release_info)
+
+
+def find_package_name():
+    """Get available pkg-config package name"""
+    packages = ["mysqlclient", "mariadb"]
+    for pkg in packages:
+        try:
+            cmd = f"pkg-config --exists {pkg}"
+            print(f"Trying {cmd}")
+            subprocess.check_call(cmd, shell=True)
+        except subprocess.CalledProcessError as err:
+            print(err)
+        else:
+            return pkg
+    raise Exception(
+        "Can not find valid pkg-config name.\n"
+        "Specify MYSQLCLIENT_CFLAGS and MYSQLCLIENT_LDFLAGS env vars manually"
+    )
+
+
+def get_config_posix(options=None):
+    # allow a command-line option to override the base config file to permit
+    # a static build to be created via requirements.txt
+    # TODO: find a better way for
+    static = False
+    if "--static" in sys.argv:
+        static = True
+        sys.argv.remove("--static")
+
+    ldflags = os.environ.get("MYSQLCLIENT_LDFLAGS")
+    cflags = os.environ.get("MYSQLCLIENT_CFLAGS")
+
+    pkg_name = None
+    static_opt = " --static" if static else ""
+    if not (cflags and ldflags):
+        pkg_name = find_package_name()
+    if not cflags:
+        cflags = subprocess.check_output(
+            f"pkg-config{static_opt} --cflags {pkg_name}", encoding="utf-8", shell=True
+        )
+    if not ldflags:
+        ldflags = subprocess.check_output(
+            f"pkg-config{static_opt} --libs {pkg_name}", encoding="utf-8", shell=True
+        )
+
+    cflags = cflags.split()
+    for f in cflags:
+        if f.startswith("-std="):
+            break
+    else:
+        cflags += ["-std=c99"]
+
+    ldflags = ldflags.split()
+
+    define_macros = [
+        ("version_info", release_info["version_info"]),
+        ("__version__", release_info["__version__"]),
+    ]
+
+    ext_options = dict(
+        extra_compile_args=cflags,
+        extra_link_args=ldflags,
+        define_macros=define_macros,
+    )
+    # newer versions of gcc require libstdc++ if doing a static build
+    if static:
+        ext_options["language"] = "c++"
+
+    print("Options for building extention module:")
+    for k, v in ext_options.items():
+        print(f"  {k}: {v}")
+
+    return ext_options
+
+
+def get_config_win32(options):
+    client = "mariadbclient"
+    connector = os.environ.get("MYSQLCLIENT_CONNECTOR", options.get("connector"))
+    if not connector:
+        connector = os.path.join(
+            os.environ["ProgramFiles"], "MariaDB", "MariaDB Connector C"
+        )
+
+    extra_objects = []
+
+    library_dirs = [
+        os.path.join(connector, "lib", "mariadb"),
+        os.path.join(connector, "lib"),
+    ]
+    libraries = [
+        "kernel32",
+        "advapi32",
+        "wsock32",
+        "shlwapi",
+        "Ws2_32",
+        "crypt32",
+        "secur32",
+        "bcrypt",
+        client,
+    ]
+    include_dirs = [
+        os.path.join(connector, "include", "mariadb"),
+        os.path.join(connector, "include"),
+    ]
+
+    extra_link_args = ["/MANIFEST"]
+
+    define_macros = [
+        ("version_info", release_info["version_info"]),
+        ("__version__", release_info["__version__"]),
+    ]
+
+    ext_options = dict(
+        library_dirs=library_dirs,
+        libraries=libraries,
+        extra_link_args=extra_link_args,
+        include_dirs=include_dirs,
+        extra_objects=extra_objects,
+        define_macros=define_macros,
+    )
+    return ext_options
+
+
+def enabled(options, option):
+    value = options[option]
+    s = value.lower()
+    if s in ("yes", "true", "1", "y"):
+        return True
+    elif s in ("no", "false", "0", "n"):
+        return False
+    else:
+        raise ValueError(f"Unknown value {value} for option {option}")
+
+
+def get_options():
+    config = ConfigParser()
+    config.read(["site.cfg"])
+    options = dict(config.items("options"))
+    options["static"] = enabled(options, "static")
+    return options
+
+
+if sys.platform == "win32":
+    ext_options = get_config_win32(get_options())
+else:
+    ext_options = get_config_posix(get_options())
+
+print("# Extention options")
+for k, v in ext_options.items():
+    print(f"  {k}: {v}")
+
+ext_modules = [
+    setuptools.Extension(
+        "MySQLdb._mysql",
+        sources=["src/MySQLdb/_mysql.c"],
+        **ext_options,
+    )
+]
+setuptools.setup(ext_modules=ext_modules)
```

### Comparing `mysqlclient-2.2.0/src/MySQLdb/__init__.py` & `mysqlclient-2.2.0rc1/src/MySQLdb/__init__.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,168 +1,168 @@
-"""
-MySQLdb - A DB API v2.0 compatible interface to MySQL.
-
-This package is a wrapper around _mysql, which mostly implements the
-MySQL C API.
-
-connect() -- connects to server
-
-See the C API specification and the MySQL documentation for more info
-on other items.
-
-For information on how MySQLdb handles type conversion, see the
-MySQLdb.converters module.
-"""
-
-from .release import version_info
-from . import _mysql
-
-if version_info != _mysql.version_info:
-    raise ImportError(
-        f"this is MySQLdb version {version_info}, "
-        f"but _mysql is version {_mysql.version_info!r}\n"
-        f"_mysql: {_mysql.__file__!r}"
-    )
-
-
-from ._mysql import (
-    NotSupportedError,
-    OperationalError,
-    get_client_info,
-    ProgrammingError,
-    Error,
-    InterfaceError,
-    debug,
-    IntegrityError,
-    string_literal,
-    MySQLError,
-    DataError,
-    DatabaseError,
-    InternalError,
-    Warning,
-)
-from MySQLdb.constants import FIELD_TYPE
-from MySQLdb.times import (
-    Date,
-    Time,
-    Timestamp,
-    DateFromTicks,
-    TimeFromTicks,
-    TimestampFromTicks,
-)
-
-threadsafety = 1
-apilevel = "2.0"
-paramstyle = "format"
-
-
-class DBAPISet(frozenset):
-    """A special type of set for which A == x is true if A is a
-    DBAPISet and x is a member of that set."""
-
-    def __eq__(self, other):
-        if isinstance(other, DBAPISet):
-            return not self.difference(other)
-        return other in self
-
-
-STRING = DBAPISet([FIELD_TYPE.ENUM, FIELD_TYPE.STRING, FIELD_TYPE.VAR_STRING])
-BINARY = DBAPISet(
-    [
-        FIELD_TYPE.BLOB,
-        FIELD_TYPE.LONG_BLOB,
-        FIELD_TYPE.MEDIUM_BLOB,
-        FIELD_TYPE.TINY_BLOB,
-    ]
-)
-NUMBER = DBAPISet(
-    [
-        FIELD_TYPE.DECIMAL,
-        FIELD_TYPE.DOUBLE,
-        FIELD_TYPE.FLOAT,
-        FIELD_TYPE.INT24,
-        FIELD_TYPE.LONG,
-        FIELD_TYPE.LONGLONG,
-        FIELD_TYPE.TINY,
-        FIELD_TYPE.YEAR,
-        FIELD_TYPE.NEWDECIMAL,
-    ]
-)
-DATE = DBAPISet([FIELD_TYPE.DATE])
-TIME = DBAPISet([FIELD_TYPE.TIME])
-TIMESTAMP = DBAPISet([FIELD_TYPE.TIMESTAMP, FIELD_TYPE.DATETIME])
-DATETIME = TIMESTAMP
-ROWID = DBAPISet()
-
-
-def test_DBAPISet_set_equality():
-    assert STRING == STRING
-
-
-def test_DBAPISet_set_inequality():
-    assert STRING != NUMBER
-
-
-def test_DBAPISet_set_equality_membership():
-    assert FIELD_TYPE.VAR_STRING == STRING
-
-
-def test_DBAPISet_set_inequality_membership():
-    assert FIELD_TYPE.DATE != STRING
-
-
-def Binary(x):
-    return bytes(x)
-
-
-def Connect(*args, **kwargs):
-    """Factory function for connections.Connection."""
-    from MySQLdb.connections import Connection
-
-    return Connection(*args, **kwargs)
-
-
-connect = Connection = Connect
-
-__all__ = [
-    "BINARY",
-    "Binary",
-    "Connect",
-    "Connection",
-    "DATE",
-    "Date",
-    "Time",
-    "Timestamp",
-    "DateFromTicks",
-    "TimeFromTicks",
-    "TimestampFromTicks",
-    "DataError",
-    "DatabaseError",
-    "Error",
-    "FIELD_TYPE",
-    "IntegrityError",
-    "InterfaceError",
-    "InternalError",
-    "MySQLError",
-    "NUMBER",
-    "NotSupportedError",
-    "DBAPISet",
-    "OperationalError",
-    "ProgrammingError",
-    "ROWID",
-    "STRING",
-    "TIME",
-    "TIMESTAMP",
-    "Warning",
-    "apilevel",
-    "connect",
-    "connections",
-    "constants",
-    "converters",
-    "cursors",
-    "debug",
-    "get_client_info",
-    "paramstyle",
-    "string_literal",
-    "threadsafety",
-    "version_info",
-]
+"""
+MySQLdb - A DB API v2.0 compatible interface to MySQL.
+
+This package is a wrapper around _mysql, which mostly implements the
+MySQL C API.
+
+connect() -- connects to server
+
+See the C API specification and the MySQL documentation for more info
+on other items.
+
+For information on how MySQLdb handles type conversion, see the
+MySQLdb.converters module.
+"""
+
+from .release import version_info
+from . import _mysql
+
+if version_info != _mysql.version_info:
+    raise ImportError(
+        f"this is MySQLdb version {version_info}, "
+        f"but _mysql is version {_mysql.version_info!r}\n"
+        f"_mysql: {_mysql.__file__!r}"
+    )
+
+
+from ._mysql import (
+    NotSupportedError,
+    OperationalError,
+    get_client_info,
+    ProgrammingError,
+    Error,
+    InterfaceError,
+    debug,
+    IntegrityError,
+    string_literal,
+    MySQLError,
+    DataError,
+    DatabaseError,
+    InternalError,
+    Warning,
+)
+from MySQLdb.constants import FIELD_TYPE
+from MySQLdb.times import (
+    Date,
+    Time,
+    Timestamp,
+    DateFromTicks,
+    TimeFromTicks,
+    TimestampFromTicks,
+)
+
+threadsafety = 1
+apilevel = "2.0"
+paramstyle = "format"
+
+
+class DBAPISet(frozenset):
+    """A special type of set for which A == x is true if A is a
+    DBAPISet and x is a member of that set."""
+
+    def __eq__(self, other):
+        if isinstance(other, DBAPISet):
+            return not self.difference(other)
+        return other in self
+
+
+STRING = DBAPISet([FIELD_TYPE.ENUM, FIELD_TYPE.STRING, FIELD_TYPE.VAR_STRING])
+BINARY = DBAPISet(
+    [
+        FIELD_TYPE.BLOB,
+        FIELD_TYPE.LONG_BLOB,
+        FIELD_TYPE.MEDIUM_BLOB,
+        FIELD_TYPE.TINY_BLOB,
+    ]
+)
+NUMBER = DBAPISet(
+    [
+        FIELD_TYPE.DECIMAL,
+        FIELD_TYPE.DOUBLE,
+        FIELD_TYPE.FLOAT,
+        FIELD_TYPE.INT24,
+        FIELD_TYPE.LONG,
+        FIELD_TYPE.LONGLONG,
+        FIELD_TYPE.TINY,
+        FIELD_TYPE.YEAR,
+        FIELD_TYPE.NEWDECIMAL,
+    ]
+)
+DATE = DBAPISet([FIELD_TYPE.DATE])
+TIME = DBAPISet([FIELD_TYPE.TIME])
+TIMESTAMP = DBAPISet([FIELD_TYPE.TIMESTAMP, FIELD_TYPE.DATETIME])
+DATETIME = TIMESTAMP
+ROWID = DBAPISet()
+
+
+def test_DBAPISet_set_equality():
+    assert STRING == STRING
+
+
+def test_DBAPISet_set_inequality():
+    assert STRING != NUMBER
+
+
+def test_DBAPISet_set_equality_membership():
+    assert FIELD_TYPE.VAR_STRING == STRING
+
+
+def test_DBAPISet_set_inequality_membership():
+    assert FIELD_TYPE.DATE != STRING
+
+
+def Binary(x):
+    return bytes(x)
+
+
+def Connect(*args, **kwargs):
+    """Factory function for connections.Connection."""
+    from MySQLdb.connections import Connection
+
+    return Connection(*args, **kwargs)
+
+
+connect = Connection = Connect
+
+__all__ = [
+    "BINARY",
+    "Binary",
+    "Connect",
+    "Connection",
+    "DATE",
+    "Date",
+    "Time",
+    "Timestamp",
+    "DateFromTicks",
+    "TimeFromTicks",
+    "TimestampFromTicks",
+    "DataError",
+    "DatabaseError",
+    "Error",
+    "FIELD_TYPE",
+    "IntegrityError",
+    "InterfaceError",
+    "InternalError",
+    "MySQLError",
+    "NUMBER",
+    "NotSupportedError",
+    "DBAPISet",
+    "OperationalError",
+    "ProgrammingError",
+    "ROWID",
+    "STRING",
+    "TIME",
+    "TIMESTAMP",
+    "Warning",
+    "apilevel",
+    "connect",
+    "connections",
+    "constants",
+    "converters",
+    "cursors",
+    "debug",
+    "get_client_info",
+    "paramstyle",
+    "string_literal",
+    "threadsafety",
+    "version_info",
+]
```

### Comparing `mysqlclient-2.2.0/src/MySQLdb/_exceptions.py` & `mysqlclient-2.2.0rc1/src/MySQLdb/_exceptions.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,91 +1,91 @@
-"""Exception classes for _mysql and MySQLdb.
-
-These classes are dictated by the DB API v2.0:
-
-    https://www.python.org/dev/peps/pep-0249/
-"""
-
-
-class MySQLError(Exception):
-    """Exception related to operation with MySQL."""
-
-    __module__ = "MySQLdb"
-
-
-class Warning(Warning, MySQLError):
-    """Exception raised for important warnings like data truncations
-    while inserting, etc."""
-
-    __module__ = "MySQLdb"
-
-
-class Error(MySQLError):
-    """Exception that is the base class of all other error exceptions
-    (not Warning)."""
-
-    __module__ = "MySQLdb"
-
-
-class InterfaceError(Error):
-    """Exception raised for errors that are related to the database
-    interface rather than the database itself."""
-
-    __module__ = "MySQLdb"
-
-
-class DatabaseError(Error):
-    """Exception raised for errors that are related to the
-    database."""
-
-    __module__ = "MySQLdb"
-
-
-class DataError(DatabaseError):
-    """Exception raised for errors that are due to problems with the
-    processed data like division by zero, numeric value out of range,
-    etc."""
-
-    __module__ = "MySQLdb"
-
-
-class OperationalError(DatabaseError):
-    """Exception raised for errors that are related to the database's
-    operation and not necessarily under the control of the programmer,
-    e.g. an unexpected disconnect occurs, the data source name is not
-    found, a transaction could not be processed, a memory allocation
-    error occurred during processing, etc."""
-
-    __module__ = "MySQLdb"
-
-
-class IntegrityError(DatabaseError):
-    """Exception raised when the relational integrity of the database
-    is affected, e.g. a foreign key check fails, duplicate key,
-    etc."""
-
-    __module__ = "MySQLdb"
-
-
-class InternalError(DatabaseError):
-    """Exception raised when the database encounters an internal
-    error, e.g. the cursor is not valid anymore, the transaction is
-    out of sync, etc."""
-
-    __module__ = "MySQLdb"
-
-
-class ProgrammingError(DatabaseError):
-    """Exception raised for programming errors, e.g. table not found
-    or already exists, syntax error in the SQL statement, wrong number
-    of parameters specified, etc."""
-
-    __module__ = "MySQLdb"
-
-
-class NotSupportedError(DatabaseError):
-    """Exception raised in case a method or database API was used
-    which is not supported by the database, e.g. requesting a
-    .rollback() on a connection that does not support transaction or
-    has transactions turned off."""
-
-    __module__ = "MySQLdb"
+"""Exception classes for _mysql and MySQLdb.
+
+These classes are dictated by the DB API v2.0:
+
+    https://www.python.org/dev/peps/pep-0249/
+"""
+
+
+class MySQLError(Exception):
+    """Exception related to operation with MySQL."""
+
+    __module__ = "MySQLdb"
+
+
+class Warning(Warning, MySQLError):
+    """Exception raised for important warnings like data truncations
+    while inserting, etc."""
+
+    __module__ = "MySQLdb"
+
+
+class Error(MySQLError):
+    """Exception that is the base class of all other error exceptions
+    (not Warning)."""
+
+    __module__ = "MySQLdb"
+
+
+class InterfaceError(Error):
+    """Exception raised for errors that are related to the database
+    interface rather than the database itself."""
+
+    __module__ = "MySQLdb"
+
+
+class DatabaseError(Error):
+    """Exception raised for errors that are related to the
+    database."""
+
+    __module__ = "MySQLdb"
+
+
+class DataError(DatabaseError):
+    """Exception raised for errors that are due to problems with the
+    processed data like division by zero, numeric value out of range,
+    etc."""
+
+    __module__ = "MySQLdb"
+
+
+class OperationalError(DatabaseError):
+    """Exception raised for errors that are related to the database's
+    operation and not necessarily under the control of the programmer,
+    e.g. an unexpected disconnect occurs, the data source name is not
+    found, a transaction could not be processed, a memory allocation
+    error occurred during processing, etc."""
+
+    __module__ = "MySQLdb"
+
+
+class IntegrityError(DatabaseError):
+    """Exception raised when the relational integrity of the database
+    is affected, e.g. a foreign key check fails, duplicate key,
+    etc."""
+
+    __module__ = "MySQLdb"
+
+
+class InternalError(DatabaseError):
+    """Exception raised when the database encounters an internal
+    error, e.g. the cursor is not valid anymore, the transaction is
+    out of sync, etc."""
+
+    __module__ = "MySQLdb"
+
+
+class ProgrammingError(DatabaseError):
+    """Exception raised for programming errors, e.g. table not found
+    or already exists, syntax error in the SQL statement, wrong number
+    of parameters specified, etc."""
+
+    __module__ = "MySQLdb"
+
+
+class NotSupportedError(DatabaseError):
+    """Exception raised in case a method or database API was used
+    which is not supported by the database, e.g. requesting a
+    .rollback() on a connection that does not support transaction or
+    has transactions turned off."""
+
+    __module__ = "MySQLdb"
```

### Comparing `mysqlclient-2.2.0/src/MySQLdb/_mysql.c` & `mysqlclient-2.2.0rc1/src/MySQLdb/_mysql.c`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,2907 +1,2907 @@
-/*
-This program is free software; you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation; either version 2, or (at your option)
-any later version. Alternatively, you may use the original license
-reproduced below.
-
-Copyright 1999 by Comstar.net, Inc., Atlanta, GA, US.
-
-                        All Rights Reserved
-
-Permission to use, copy, modify, and distribute this software and its
-documentation for any purpose and without fee is hereby granted,
-provided that the above copyright notice appear in all copies and that
-both that copyright notice and this permission notice appear in
-supporting documentation, and that the name of Comstar.net, Inc.
-or COMSTAR not be used in advertising or publicity pertaining to
-distribution of the software without specific, written prior permission.
-
-COMSTAR DISCLAIMS ALL WARRANTIES WITH REGARD TO THIS SOFTWARE,
-INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS, IN NO
-EVENT SHALL COMSTAR BE LIABLE FOR ANY SPECIAL, INDIRECT OR
-CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF
-USE, DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR
-OTHER TORTIOUS ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR
-PERFORMANCE OF THIS SOFTWARE.
-*/
-
-#include "mysql.h"
-#include "mysqld_error.h"
-
-#if MYSQL_VERSION_ID >= 80000
-// https://github.com/mysql/mysql-server/commit/eb821c023cedc029ca0b06456dfae365106bee84
-#define my_bool _Bool
-#endif
-
-#if ((MYSQL_VERSION_ID >= 50555 && MYSQL_VERSION_ID <= 50599) || \
-(MYSQL_VERSION_ID >= 50636 && MYSQL_VERSION_ID <= 50699) || \
-(MYSQL_VERSION_ID >= 50711 && MYSQL_VERSION_ID <= 50799) || \
-(MYSQL_VERSION_ID >= 80000)) && \
-!defined(MARIADB_BASE_VERSION) && !defined(MARIADB_VERSION_ID)
-#define HAVE_ENUM_MYSQL_OPT_SSL_MODE
-#endif
-
-#define PY_SSIZE_T_CLEAN 1
-#include "Python.h"
-
-#if PY_MAJOR_VERSION == 2
-#error "Python 2 is not supported"
-#endif
-
-#include "bytesobject.h"
-#include "structmember.h"
-#include "errmsg.h"
-
-#define MyAlloc(s,t) (s *) t.tp_alloc(&t,0)
-#define MyFree(o) Py_TYPE(o)->tp_free((PyObject*)o)
-
-static PyObject *_mysql_MySQLError;
-static PyObject *_mysql_Warning;
-static PyObject *_mysql_Error;
-static PyObject *_mysql_DatabaseError;
-static PyObject *_mysql_InterfaceError;
-static PyObject *_mysql_DataError;
-static PyObject *_mysql_OperationalError;
-static PyObject *_mysql_IntegrityError;
-static PyObject *_mysql_InternalError;
-static PyObject *_mysql_ProgrammingError;
-static PyObject *_mysql_NotSupportedError;
-
-typedef struct {
-    PyObject_HEAD
-    MYSQL connection;
-    int open;
-    PyObject *converter;
-} _mysql_ConnectionObject;
-
-#define check_connection(c) \
-    if (!(c->open)) { \
-        return _mysql_Exception(c); \
-    };
-
-#define result_connection(r) ((_mysql_ConnectionObject *)r->conn)
-#define check_result_connection(r) check_connection(result_connection(r))
-
-extern PyTypeObject _mysql_ConnectionObject_Type;
-
-typedef struct {
-    PyObject_HEAD
-    PyObject *conn;
-    MYSQL_RES *result;
-    int nfields;
-    int use;
-    char has_next;
-    PyObject *converter;
-    const char *encoding;
-} _mysql_ResultObject;
-
-extern PyTypeObject _mysql_ResultObject_Type;
-
-
-PyObject *
-_mysql_Exception(_mysql_ConnectionObject *c)
-{
-    PyObject *t, *e;
-    int merr;
-
-    if (!(t = PyTuple_New(2))) return NULL;
-    if (!(c->open)) {
-        /* GH-270: When connection is closed, accessing the c->connection
-         * object may cause SEGV.
-         */
-        merr = CR_SERVER_GONE_ERROR;
-    }
-    else {
-        merr = mysql_errno(&(c->connection));
-    }
-    switch (merr) {
-    case 0:
-        e = _mysql_InterfaceError;
-        break;
-    case CR_COMMANDS_OUT_OF_SYNC:
-    case ER_DB_CREATE_EXISTS:
-    case ER_SYNTAX_ERROR:
-    case ER_PARSE_ERROR:
-    case ER_NO_SUCH_TABLE:
-    case ER_WRONG_DB_NAME:
-    case ER_WRONG_TABLE_NAME:
-    case ER_FIELD_SPECIFIED_TWICE:
-    case ER_INVALID_GROUP_FUNC_USE:
-    case ER_UNSUPPORTED_EXTENSION:
-    case ER_TABLE_MUST_HAVE_COLUMNS:
-#ifdef ER_CANT_DO_THIS_DURING_AN_TRANSACTION
-    case ER_CANT_DO_THIS_DURING_AN_TRANSACTION:
-#endif
-        e = _mysql_ProgrammingError;
-        break;
-#ifdef WARN_DATA_TRUNCATED
-    case WARN_DATA_TRUNCATED:
-#ifdef WARN_NULL_TO_NOTNULL
-    case WARN_NULL_TO_NOTNULL:
-#endif
-#ifdef ER_WARN_DATA_OUT_OF_RANGE
-    case ER_WARN_DATA_OUT_OF_RANGE:
-#endif
-#ifdef ER_NO_DEFAULT
-    case ER_NO_DEFAULT:
-#endif
-#ifdef ER_PRIMARY_CANT_HAVE_NULL
-    case ER_PRIMARY_CANT_HAVE_NULL:
-#endif
-#ifdef ER_DATA_TOO_LONG
-    case ER_DATA_TOO_LONG:
-#endif
-#ifdef ER_DATETIME_FUNCTION_OVERFLOW
-    case ER_DATETIME_FUNCTION_OVERFLOW:
-#endif
-        e = _mysql_DataError;
-        break;
-#endif
-    case ER_DUP_ENTRY:
-#ifdef ER_DUP_UNIQUE
-    case ER_DUP_UNIQUE:
-#endif
-#ifdef ER_NO_REFERENCED_ROW
-    case ER_NO_REFERENCED_ROW:
-#endif
-#ifdef ER_NO_REFERENCED_ROW_2
-    case ER_NO_REFERENCED_ROW_2:
-#endif
-#ifdef ER_ROW_IS_REFERENCED
-    case ER_ROW_IS_REFERENCED:
-#endif
-#ifdef ER_ROW_IS_REFERENCED_2
-    case ER_ROW_IS_REFERENCED_2:
-#endif
-#ifdef ER_CANNOT_ADD_FOREIGN
-    case ER_CANNOT_ADD_FOREIGN:
-#endif
-#ifdef ER_NO_DEFAULT_FOR_FIELD
-    case ER_NO_DEFAULT_FOR_FIELD:
-#endif
-    case ER_BAD_NULL_ERROR:
-        e = _mysql_IntegrityError;
-        break;
-#ifdef ER_WARNING_NOT_COMPLETE_ROLLBACK
-    case ER_WARNING_NOT_COMPLETE_ROLLBACK:
-#endif
-#ifdef ER_NOT_SUPPORTED_YET
-    case ER_NOT_SUPPORTED_YET:
-#endif
-#ifdef ER_FEATURE_DISABLED
-    case ER_FEATURE_DISABLED:
-#endif
-#ifdef ER_UNKNOWN_STORAGE_ENGINE
-    case ER_UNKNOWN_STORAGE_ENGINE:
-#endif
-        e = _mysql_NotSupportedError;
-        break;
-    default:
-        if (merr < 1000)
-            e = _mysql_InternalError;
-        else
-            e = _mysql_OperationalError;
-        break;
-    }
-    PyTuple_SET_ITEM(t, 0, PyLong_FromLong((long)merr));
-    PyTuple_SET_ITEM(t, 1, PyUnicode_FromString(mysql_error(&(c->connection))));
-    PyErr_SetObject(e, t);
-    Py_DECREF(t);
-    return NULL;
-}
-
-static const char *utf8 = "utf8";
-
-static const char*
-_get_encoding(MYSQL *mysql)
-{
-    MY_CHARSET_INFO cs;
-    mysql_get_character_set_info(mysql, &cs);
-    if (strncmp(utf8, cs.csname, 4) == 0) { // utf8, utf8mb3, utf8mb4
-        return utf8;
-    }
-    else if (strncmp("latin1", cs.csname, 6) == 0) {
-        return "cp1252";
-    }
-    else if (strncmp("koi8r", cs.csname, 5) == 0) {
-        return "koi8_r";
-    }
-    else if (strncmp("koi8u", cs.csname, 5) == 0) {
-        return "koi8_u";
-    }
-    return cs.csname;
-}
-
-static char _mysql_ResultObject__doc__[] =
-"result(connection, use=0, converter={}) -- Result set from a query.\n\
-\n\
-Creating instances of this class directly is an excellent way to\n\
-shoot yourself in the foot. If using _mysql.connection directly,\n\
-use connection.store_result() or connection.use_result() instead.\n\
-If using MySQLdb.Connection, this is done by the cursor class.\n\
-Just forget you ever saw this. Forget... FOR-GET...";
-
-static int
-_mysql_ResultObject_Initialize(
-    _mysql_ResultObject *self,
-    PyObject *args,
-    PyObject *kwargs)
-{
-    static char *kwlist[] = {"connection", "use", "converter", NULL};
-    MYSQL_RES *result;
-    _mysql_ConnectionObject *conn=NULL;
-    int use=0;
-    PyObject *conv=NULL;
-    int n, i;
-    MYSQL_FIELD *fields;
-
-    if (!PyArg_ParseTupleAndKeywords(args, kwargs, "O!|iO", kwlist,
-                     &_mysql_ConnectionObject_Type, &conn, &use, &conv))
-        return -1;
-
-    self->conn = (PyObject *) conn;
-    Py_INCREF(conn);
-    self->use = use;
-    Py_BEGIN_ALLOW_THREADS ;
-    if (use)
-        result = mysql_use_result(&(conn->connection));
-    else
-        result = mysql_store_result(&(conn->connection));
-    self->result = result;
-    self->has_next = (char)mysql_more_results(&(conn->connection));
-    Py_END_ALLOW_THREADS ;
-
-    self->encoding = _get_encoding(&(conn->connection));
-    //fprintf(stderr, "encoding=%s\n", self->encoding);
-    if (!result) {
-        if (mysql_errno(&(conn->connection))) {
-            _mysql_Exception(conn);
-            return -1;
-        }
-        self->converter = PyTuple_New(0);
-        return 0;
-    }
-    n = mysql_num_fields(result);
-    self->nfields = n;
-    if (!(self->converter = PyTuple_New(n))) {
-        return -1;
-    }
-    fields = mysql_fetch_fields(result);
-    for (i=0; i<n; i++) {
-        PyObject *tmp, *fun;
-        tmp = PyLong_FromLong((long) fields[i].type);
-        if (!tmp) {
-            return -1;
-        }
-        fun = conv ? PyObject_GetItem(conv, tmp) : NULL;
-        Py_DECREF(tmp);
-        if (!fun) {
-            if (PyErr_Occurred()) {
-                if (!PyErr_ExceptionMatches(PyExc_KeyError)) {
-                    return -1;
-                }
-                PyErr_Clear();
-            }
-            fun = Py_None;
-            Py_INCREF(Py_None);
-        }
-        else if (PySequence_Check(fun)) {
-            long flags = fields[i].flags;
-            PyObject *fun2=NULL;
-            int j, n2=PySequence_Size(fun);
-            // BINARY_FLAG means ***_bin collation is used.
-            // To distinguish text and binary, we should use charsetnr==63 (binary).
-            // But we abuse BINARY_FLAG for historical reason.
-            if (fields[i].charsetnr == 63) {
-                flags |= BINARY_FLAG;
-            } else {
-                flags &= ~BINARY_FLAG;
-            }
-            for (j=0; j<n2; j++) {
-                PyObject *t = PySequence_GetItem(fun, j);
-                if (!t) {
-                    Py_DECREF(fun);
-                    return -1;
-                }
-                if (PyTuple_Check(t) && PyTuple_GET_SIZE(t) == 2) {
-                    long mask;
-                    PyObject *pmask=NULL;
-                    pmask = PyTuple_GET_ITEM(t, 0);
-                    fun2 = PyTuple_GET_ITEM(t, 1);
-                    Py_XINCREF(fun2);
-                    if (PyLong_Check(pmask)) {
-                        mask = PyLong_AS_LONG(pmask);
-                        if (mask & flags) {
-                            Py_DECREF(t);
-                            break;
-                        }
-                        else {
-                            fun2 = NULL;
-                        }
-                    } else {
-                        Py_DECREF(t);
-                        break;
-                    }
-                }
-                Py_DECREF(t);
-            }
-            if (!fun2) {
-                fun2 = Py_None;
-                Py_INCREF(fun2);
-            }
-            Py_DECREF(fun);
-            fun = fun2;
-        }
-        PyTuple_SET_ITEM(self->converter, i, fun);
-    }
-
-    return 0;
-}
-
-static int _mysql_ResultObject_traverse(
-    _mysql_ResultObject *self,
-    visitproc visit,
-    void *arg)
-{
-    int r;
-    if (self->converter) {
-        if (!(r = visit(self->converter, arg))) return r;
-    }
-    if (self->conn)
-        return visit(self->conn, arg);
-    return 0;
-}
-
-static int _mysql_ResultObject_clear(_mysql_ResultObject *self)
-{
-    Py_CLEAR(self->converter);
-    Py_CLEAR(self->conn);
-    return 0;
-}
-
-enum {
-    SSLMODE_DISABLED = 1,
-    SSLMODE_PREFERRED = 2,
-    SSLMODE_REQUIRED = 3,
-    SSLMODE_VERIFY_CA = 4,
-    SSLMODE_VERIFY_IDENTITY = 5
-};
-
-static int
-_get_ssl_mode_num(char *ssl_mode)
-{
-    static char *ssl_mode_list[] = { "DISABLED", "PREFERRED",
-                  "REQUIRED", "VERIFY_CA", "VERIFY_IDENTITY" };
-    unsigned int i;
-    for (i=0; i < sizeof(ssl_mode_list)/sizeof(ssl_mode_list[0]); i++) {
-        if (strcmp(ssl_mode, ssl_mode_list[i]) == 0) {
-            // SSL_MODE one-based
-            return i + 1;
-        }
-    }
-    return -1;
-}
-
-static int
-_mysql_ConnectionObject_Initialize(
-    _mysql_ConnectionObject *self,
-    PyObject *args,
-    PyObject *kwargs)
-{
-    MYSQL *conn = NULL;
-    PyObject *conv = NULL;
-    PyObject *ssl = NULL;
-    char *ssl_mode = NULL;
-    const char *key = NULL, *cert = NULL, *ca = NULL,
-         *capath = NULL, *cipher = NULL;
-    PyObject *ssl_keepref[5] = {NULL};
-    int n_ssl_keepref = 0;
-    char *host = NULL, *user = NULL, *passwd = NULL,
-         *db = NULL, *unix_socket = NULL;
-    unsigned int port = 0;
-    unsigned int client_flag = 0;
-    static char *kwlist[] = { "host", "user", "password", "database", "port",
-                  "unix_socket", "conv",
-                  "connect_timeout", "compress",
-                  "named_pipe", "init_command",
-                  "read_default_file", "read_default_group",
-                  "client_flag", "ssl", "ssl_mode",
-                  "local_infile",
-                  "read_timeout", "write_timeout", "charset",
-                  "auth_plugin",
-                  NULL } ;
-    int connect_timeout = 0;
-    int read_timeout = 0;
-    int write_timeout = 0;
-    int compress = -1, named_pipe = -1, local_infile = -1;
-    int ssl_mode_num = SSLMODE_DISABLED;
-    char *init_command=NULL,
-         *read_default_file=NULL,
-         *read_default_group=NULL,
-         *charset=NULL,
-         *auth_plugin=NULL;
-
-    self->converter = NULL;
-    self->open = 0;
-
-    if (!PyArg_ParseTupleAndKeywords(args, kwargs,
-                "|ssssisOiiisssiOsiiiss:connect",
-                kwlist,
-                &host, &user, &passwd, &db,
-                &port, &unix_socket, &conv,
-                &connect_timeout,
-                &compress, &named_pipe,
-                &init_command, &read_default_file,
-                &read_default_group,
-                &client_flag, &ssl, &ssl_mode,
-                &local_infile,
-                &read_timeout,
-                &write_timeout,
-                &charset,
-                &auth_plugin
-    ))
-        return -1;
-
-#define _stringsuck(d,t,s) {t=PyMapping_GetItemString(s,#d);\
-        if(t){d=PyUnicode_AsUTF8(t);ssl_keepref[n_ssl_keepref++]=t;}\
-        PyErr_Clear();}
-
-    if (ssl) {
-        PyObject *value = NULL;
-        _stringsuck(ca, value, ssl);
-        _stringsuck(capath, value, ssl);
-        _stringsuck(cert, value, ssl);
-        _stringsuck(key, value, ssl);
-        _stringsuck(cipher, value, ssl);
-    }
-    if (ssl_mode) {
-        if ((ssl_mode_num = _get_ssl_mode_num(ssl_mode)) <= 0) {
-            PyErr_SetString(_mysql_NotSupportedError, "Unknown ssl_mode specification");
-            return -1;
-        }
-    }
-
-    conn = mysql_init(&(self->connection));
-    if (!conn) {
-        PyErr_SetNone(PyExc_MemoryError);
-        return -1;
-    }
-    self->open = 1;
-
-    if (connect_timeout) {
-        unsigned int timeout = connect_timeout;
-        mysql_options(&(self->connection), MYSQL_OPT_CONNECT_TIMEOUT,
-                (char *)&timeout);
-    }
-    if (read_timeout) {
-        unsigned int timeout = read_timeout;
-        mysql_options(&(self->connection), MYSQL_OPT_READ_TIMEOUT,
-                (char *)&timeout);
-    }
-    if (write_timeout) {
-        unsigned int timeout = write_timeout;
-        mysql_options(&(self->connection), MYSQL_OPT_WRITE_TIMEOUT,
-                (char *)&timeout);
-    }
-    if (compress != -1) {
-        mysql_options(&(self->connection), MYSQL_OPT_COMPRESS, 0);
-        client_flag |= CLIENT_COMPRESS;
-    }
-    if (named_pipe != -1)
-        mysql_options(&(self->connection), MYSQL_OPT_NAMED_PIPE, 0);
-    if (init_command != NULL)
-        mysql_options(&(self->connection), MYSQL_INIT_COMMAND, init_command);
-    if (read_default_file != NULL)
-        mysql_options(&(self->connection), MYSQL_READ_DEFAULT_FILE, read_default_file);
-    if (read_default_group != NULL)
-        mysql_options(&(self->connection), MYSQL_READ_DEFAULT_GROUP, read_default_group);
-
-    if (local_infile != -1)
-        mysql_options(&(self->connection), MYSQL_OPT_LOCAL_INFILE, (char *) &local_infile);
-
-    if (ssl) {
-        mysql_ssl_set(&(self->connection), key, cert, ca, capath, cipher);
-    }
-    if (ssl_mode) {
-#ifdef HAVE_ENUM_MYSQL_OPT_SSL_MODE
-        mysql_options(&(self->connection), MYSQL_OPT_SSL_MODE, &ssl_mode_num);
-#else
-        // MariaDB doesn't support MYSQL_OPT_SSL_MODE.
-        // See https://github.com/PyMySQL/mysqlclient/issues/474
-        // TODO: Does MariaDB supports PREFERRED and VERIFY_CA?
-        // We support only two levels for now.
-        my_bool enforce_tls = 1;
-        if (ssl_mode_num >= SSLMODE_REQUIRED) {
-            mysql_optionsv(&(self->connection), MYSQL_OPT_SSL_ENFORCE, (void *)&enforce_tls);
-        }
-        if (ssl_mode_num >= SSLMODE_VERIFY_CA) {
-            mysql_optionsv(&(self->connection), MYSQL_OPT_SSL_VERIFY_SERVER_CERT, (void *)&enforce_tls);
-        }
-#endif
-    }
-
-    if (charset) {
-        mysql_options(&(self->connection), MYSQL_SET_CHARSET_NAME, charset);
-    }
-    if (auth_plugin) {
-        mysql_options(&(self->connection), MYSQL_DEFAULT_AUTH, auth_plugin);
-    }
-
-    Py_BEGIN_ALLOW_THREADS
-    conn = mysql_real_connect(&(self->connection), host, user, passwd, db,
-                  port, unix_socket, client_flag);
-    Py_END_ALLOW_THREADS
-
-    if (ssl) {
-        int i;
-        for (i=0; i<n_ssl_keepref; i++) {
-            Py_DECREF(ssl_keepref[i]);
-            ssl_keepref[i] = NULL;
-        }
-    }
-
-    if (!conn) {
-        _mysql_Exception(self);
-        return -1;
-    }
-
-    /* Internal references to python-land objects */
-    if (!conv)
-        conv = PyDict_New();
-    else
-        Py_INCREF(conv);
-
-    if (!conv)
-        return -1;
-    self->converter = conv;
-
-    /*
-      PyType_GenericAlloc() automatically sets up GC allocation and
-      tracking for GC objects, at least in 2.2.1, so it does not need to
-      be done here. tp_dealloc still needs to call PyObject_GC_UnTrack(),
-      however.
-    */
-    return 0;
-}
-
-static char _mysql_connect__doc__[] =
-"Returns a MYSQL connection object. Exclusive use of\n\
-keyword parameters strongly recommended. Consult the\n\
-MySQL C API documentation for more details.\n\
-\n\
-host\n\
-  string, host to connect\n\
-\n\
-user\n\
-  string, user to connect as\n\
-\n\
-password\n\
-  string, password to use\n\
-\n\
-database\n\
-  string, database to use\n\
-\n\
-port\n\
-  integer, TCP/IP port to connect to\n\
-\n\
-unix_socket\n\
-  string, location of unix_socket (UNIX-ish only)\n\
-\n\
-conv\n\
-  mapping, maps MySQL FIELD_TYPE.* to Python functions which\n\
-  convert a string to the appropriate Python type\n\
-\n\
-connect_timeout\n\
-  number of seconds to wait before the connection\n\
-  attempt fails.\n\
-\n\
-compress\n\
-  if set, gzip compression is enabled\n\
-\n\
-named_pipe\n\
-  if set, connect to server via named pipe (Windows only)\n\
-\n\
-init_command\n\
-  command which is run once the connection is created\n\
-\n\
-read_default_file\n\
-  see the MySQL documentation for mysql_options()\n\
-\n\
-read_default_group\n\
-  see the MySQL documentation for mysql_options()\n\
-\n\
-client_flag\n\
-  client flags from MySQLdb.constants.CLIENT\n\
-\n\
-load_infile\n\
-  int, non-zero enables LOAD LOCAL INFILE, zero disables\n\
-\n\
-";
-
-static PyObject *
-_mysql_connect(
-    PyObject *self,
-    PyObject *args,
-    PyObject *kwargs)
-{
-    _mysql_ConnectionObject *c=NULL;
-
-    c = MyAlloc(_mysql_ConnectionObject, _mysql_ConnectionObject_Type);
-    if (c == NULL) return NULL;
-    if (_mysql_ConnectionObject_Initialize(c, args, kwargs)) {
-        Py_DECREF(c);
-        c = NULL;
-    }
-    return (PyObject *) c;
-}
-
-static int _mysql_ConnectionObject_traverse(
-    _mysql_ConnectionObject *self,
-    visitproc visit,
-    void *arg)
-{
-    if (self->converter)
-        return visit(self->converter, arg);
-    return 0;
-}
-
-static int _mysql_ConnectionObject_clear(
-    _mysql_ConnectionObject *self)
-{
-    Py_XDECREF(self->converter);
-    self->converter = NULL;
-    return 0;
-}
-
-static char _mysql_ConnectionObject_close__doc__[] =
-"Close the connection. No further activity possible.";
-
-static PyObject *
-_mysql_ConnectionObject_close(
-    _mysql_ConnectionObject *self,
-    PyObject *noargs)
-{
-    check_connection(self);
-    Py_BEGIN_ALLOW_THREADS
-    mysql_close(&(self->connection));
-    Py_END_ALLOW_THREADS
-    self->open = 0;
-    _mysql_ConnectionObject_clear(self);
-    Py_RETURN_NONE;
-}
-
-static char _mysql_ConnectionObject_affected_rows__doc__ [] =
-"Return number of rows affected by the last query.\n\
-Non-standard. Use Cursor.rowcount.\n\
-";
-
-static PyObject *
-_mysql_ConnectionObject_affected_rows(
-    _mysql_ConnectionObject *self,
-    PyObject *noargs)
-{
-    my_ulonglong ret;
-    check_connection(self);
-    ret = mysql_affected_rows(&(self->connection));
-    if (ret == (my_ulonglong)-1)
-        return PyLong_FromLong(-1);
-    return PyLong_FromUnsignedLongLong(ret);
-}
-
-static char _mysql_debug__doc__[] =
-"Does a DBUG_PUSH with the given string.\n\
-mysql_debug() uses the Fred Fish debug library.\n\
-To use this function, you must compile the client library to\n\
-support debugging.\n\
-";
-static PyObject *
-_mysql_debug(
-    PyObject *self,
-    PyObject *args)
-{
-    char *debug;
-    if (!PyArg_ParseTuple(args, "s", &debug)) return NULL;
-    mysql_debug(debug);
-    Py_RETURN_NONE;
-}
-
-static char _mysql_ConnectionObject_dump_debug_info__doc__[] =
-"Instructs the server to write some debug information to the\n\
-log. The connected user must have the process privilege for\n\
-this to work. Non-standard.\n\
-";
-
-static PyObject *
-_mysql_ConnectionObject_dump_debug_info(
-    _mysql_ConnectionObject *self,
-    PyObject *noargs)
-{
-    int err;
-    check_connection(self);
-    Py_BEGIN_ALLOW_THREADS
-    err = mysql_dump_debug_info(&(self->connection));
-    Py_END_ALLOW_THREADS
-    if (err) return _mysql_Exception(self);
-    Py_RETURN_NONE;
-}
-
-static char _mysql_ConnectionObject_autocommit__doc__[] =
-"Set the autocommit mode. True values enable; False value disable.\n\
-";
-static PyObject *
-_mysql_ConnectionObject_autocommit(
-    _mysql_ConnectionObject *self,
-    PyObject *args)
-{
-    int flag, err;
-    if (!PyArg_ParseTuple(args, "i", &flag)) return NULL;
-    check_connection(self);
-    Py_BEGIN_ALLOW_THREADS
-    err = mysql_autocommit(&(self->connection), flag);
-    Py_END_ALLOW_THREADS
-    if (err) return _mysql_Exception(self);
-    Py_RETURN_NONE;
-}
-
-static char _mysql_ConnectionObject_get_autocommit__doc__[] =
-"Get the autocommit mode. True when enable; False when disable.\n";
-
-static PyObject *
-_mysql_ConnectionObject_get_autocommit(
-    _mysql_ConnectionObject *self,
-    PyObject *args)
-{
-    check_connection(self);
-    if (self->connection.server_status & SERVER_STATUS_AUTOCOMMIT) {
-        Py_RETURN_TRUE;
-    }
-    Py_RETURN_FALSE;
-}
-
-static char _mysql_ConnectionObject_commit__doc__[] =
-"Commits the current transaction\n\
-";
-static PyObject *
-_mysql_ConnectionObject_commit(
-    _mysql_ConnectionObject *self,
-    PyObject *noargs)
-{
-    int err;
-    check_connection(self);
-    Py_BEGIN_ALLOW_THREADS
-    err = mysql_commit(&(self->connection));
-    Py_END_ALLOW_THREADS
-    if (err) return _mysql_Exception(self);
-    Py_RETURN_NONE;
-}
-
-static char _mysql_ConnectionObject_rollback__doc__[] =
-"Rolls back the current transaction\n\
-";
-static PyObject *
-_mysql_ConnectionObject_rollback(
-    _mysql_ConnectionObject *self,
-    PyObject *noargs)
-{
-    int err;
-    check_connection(self);
-    Py_BEGIN_ALLOW_THREADS
-    err = mysql_rollback(&(self->connection));
-    Py_END_ALLOW_THREADS
-    if (err) return _mysql_Exception(self);
-    Py_RETURN_NONE;
-}
-
-static char _mysql_ConnectionObject_next_result__doc__[] =
-"If more query results exist, next_result() reads the next query\n\
-results and returns the status back to application.\n\
-\n\
-After calling next_result() the state of the connection is as if\n\
-you had called query() for the next query. This means that you can\n\
-now call store_result(), warning_count(), affected_rows()\n\
-, and so forth. \n\
-\n\
-Returns 0 if there are more results; -1 if there are no more results\n\
-\n\
-Non-standard.\n\
-";
-static PyObject *
-_mysql_ConnectionObject_next_result(
-    _mysql_ConnectionObject *self,
-    PyObject *noargs)
-{
-    int err;
-    check_connection(self);
-    Py_BEGIN_ALLOW_THREADS
-    err = mysql_next_result(&(self->connection));
-    Py_END_ALLOW_THREADS
-    if (err > 0) return _mysql_Exception(self);
-    return PyLong_FromLong(err);
-}
-
-
-static char _mysql_ConnectionObject_set_server_option__doc__[] =
-"set_server_option(option) -- Enables or disables an option\n\
-for the connection.\n\
-\n\
-Non-standard.\n\
-";
-static PyObject *
-_mysql_ConnectionObject_set_server_option(
-    _mysql_ConnectionObject *self,
-    PyObject *args)
-{
-    int err, flags=0;
-    if (!PyArg_ParseTuple(args, "i", &flags))
-        return NULL;
-    check_connection(self);
-    Py_BEGIN_ALLOW_THREADS
-    err = mysql_set_server_option(&(self->connection), flags);
-    Py_END_ALLOW_THREADS
-    if (err) return _mysql_Exception(self);
-    return PyLong_FromLong(err);
-}
-
-static char _mysql_ConnectionObject_sqlstate__doc__[] =
-"Returns a string containing the SQLSTATE error code\n\
-for the last error. The error code consists of five characters.\n\
-'00000' means \"no error.\" The values are specified by ANSI SQL\n\
-and ODBC. For a list of possible values, see section 23\n\
-Error Handling in MySQL in the MySQL Manual.\n\
-\n\
-Note that not all MySQL errors are yet mapped to SQLSTATE's.\n\
-The value 'HY000' (general error) is used for unmapped errors.\n\
-\n\
-Non-standard.\n\
-";
-static PyObject *
-_mysql_ConnectionObject_sqlstate(
-    _mysql_ConnectionObject *self,
-    PyObject *noargs)
-{
-    check_connection(self);
-    return PyUnicode_FromString(mysql_sqlstate(&(self->connection)));
-}
-
-static char _mysql_ConnectionObject_warning_count__doc__[] =
-"Returns the number of warnings generated during execution\n\
-of the previous SQL statement.\n\
-\n\
-Non-standard.\n\
-";
-static PyObject *
-_mysql_ConnectionObject_warning_count(
-    _mysql_ConnectionObject *self,
-    PyObject *noargs)
-{
-    check_connection(self);
-    return PyLong_FromLong(mysql_warning_count(&(self->connection)));
-}
-
-static char _mysql_ConnectionObject_errno__doc__[] =
-"Returns the error code for the most recently invoked API function\n\
-that can succeed or fail. A return value of zero means that no error\n\
-occurred.\n\
-";
-
-static PyObject *
-_mysql_ConnectionObject_errno(
-    _mysql_ConnectionObject *self,
-    PyObject *noargs)
-{
-    check_connection(self);
-    return PyLong_FromLong((long)mysql_errno(&(self->connection)));
-}
-
-static char _mysql_ConnectionObject_error__doc__[] =
-"Returns the error message for the most recently invoked API function\n\
-that can succeed or fail. An empty string ("") is returned if no error\n\
-occurred.\n\
-";
-
-static PyObject *
-_mysql_ConnectionObject_error(
-    _mysql_ConnectionObject *self,
-    PyObject *noargs)
-{
-    check_connection(self);
-    return PyUnicode_FromString(mysql_error(&(self->connection)));
-}
-
-static char _mysql_escape_string__doc__[] =
-"escape_string(s) -- quote any SQL-interpreted characters in string s.\n\
-\n\
-Use connection.escape_string(s), if you use it at all.\n\
-_mysql.escape_string(s) cannot handle character sets. You are\n\
-probably better off using connection.escape(o) instead, since\n\
-it will escape entire sequences as well as strings.";
-
-static PyObject *
-_mysql_escape_string(
-    _mysql_ConnectionObject *self,
-    PyObject *args)
-{
-    PyObject *str;
-    char *in, *out;
-    unsigned long len;
-    Py_ssize_t size;
-    if (!PyArg_ParseTuple(args, "s#:escape_string", &in, &size)) return NULL;
-    str = PyBytes_FromStringAndSize((char *) NULL, size*2+1);
-    if (!str) return PyErr_NoMemory();
-    out = PyBytes_AS_STRING(str);
-
-    if (self && PyModule_Check((PyObject*)self))
-        self = NULL;
-    if (self && self->open) {
-#if MYSQL_VERSION_ID >= 50707 && !defined(MARIADB_BASE_VERSION) && !defined(MARIADB_VERSION_ID)
-        len = mysql_real_escape_string_quote(&(self->connection), out, in, size, '\'');
-#else
-        len = mysql_real_escape_string(&(self->connection), out, in, size);
-#endif
-    } else {
-        len = mysql_escape_string(out, in, size);
-    }
-    if (_PyBytes_Resize(&str, len) < 0) return NULL;
-    return (str);
-}
-
-static char _mysql_string_literal__doc__[] =
-"string_literal(obj) -- converts object obj into a SQL string literal.\n\
-This means, any special SQL characters are escaped, and it is enclosed\n\
-within single quotes. In other words, it performs:\n\
-\n\
-\"'%s'\" % escape_string(str(obj))\n\
-\n\
-Use connection.string_literal(obj), if you use it at all.\n\
-_mysql.string_literal(obj) cannot handle character sets.";
-
-static PyObject *
-_mysql_string_literal(
-    _mysql_ConnectionObject *self,
-    PyObject *o)
-{
-    PyObject *s; // input string or bytes. need to decref.
-
-    if (self && PyModule_Check((PyObject*)self))
-        self = NULL;
-
-    if (PyBytes_Check(o)) {
-        s = o;
-        Py_INCREF(s);
-    }
-    else {
-        PyObject *t = PyObject_Str(o);
-        if (!t) return NULL;
-
-        const char *encoding = (self && self->open) ?
-            _get_encoding(&self->connection) : utf8;
-        if (encoding == utf8) {
-            s = t;
-        }
-        else {
-            s = PyUnicode_AsEncodedString(t, encoding, "strict");
-            Py_DECREF(t);
-            if (!s) return NULL;
-        }
-    }
-
-    // Prepare input string (in, size)
-    const char *in;
-    Py_ssize_t size;
-    if (PyUnicode_Check(s)) {
-        in = PyUnicode_AsUTF8AndSize(s, &size);
-    } else {
-        assert(PyBytes_Check(s));
-        in = PyBytes_AsString(s);
-        size = PyBytes_GET_SIZE(s);
-    }
-
-    // Prepare output buffer (str, out)
-    PyObject *str = PyBytes_FromStringAndSize((char *) NULL, size*2+3);
-    if (!str) {
-        Py_DECREF(s);
-        return PyErr_NoMemory();
-    }
-    char *out = PyBytes_AS_STRING(str);
-
-    // escape
-    unsigned long len;
-    if (self && self->open) {
-#if MYSQL_VERSION_ID >= 50707 && !defined(MARIADB_BASE_VERSION) && !defined(MARIADB_VERSION_ID)
-        len = mysql_real_escape_string_quote(&(self->connection), out+1, in, size, '\'');
-#else
-        len = mysql_real_escape_string(&(self->connection), out+1, in, size);
-#endif
-    } else {
-        len = mysql_escape_string(out+1, in, size);
-    }
-
-    Py_DECREF(s);
-    *out = *(out+len+1) = '\'';
-    if (_PyBytes_Resize(&str, len+2) < 0) {
-        Py_DECREF(str);
-        return NULL;
-    }
-    return str;
-}
-
-static PyObject *
-_escape_item(
-    PyObject *self,
-    PyObject *item,
-    PyObject *d)
-{
-    PyObject *quoted=NULL, *itemtype, *itemconv;
-    if (!(itemtype = PyObject_Type(item))) {
-        return NULL;
-    }
-    itemconv = PyObject_GetItem(d, itemtype);
-    Py_DECREF(itemtype);
-    if (!itemconv) {
-        PyErr_Clear();
-        return _mysql_string_literal((_mysql_ConnectionObject*)self, item);
-    }
-    Py_INCREF(d);
-    quoted = PyObject_CallFunction(itemconv, "OO", item, d);
-    Py_DECREF(d);
-    Py_DECREF(itemconv);
-
-    return quoted;
-}
-
-static char _mysql_escape__doc__[] =
-"escape(obj, dict) -- escape any special characters in object obj\n\
-using mapping dict to provide quoting functions for each type.\n\
-Returns a SQL literal string.";
-static PyObject *
-_mysql_escape(
-    PyObject *self,
-    PyObject *args)
-{
-    PyObject *o=NULL, *d=NULL;
-    if (!PyArg_ParseTuple(args, "O|O:escape", &o, &d))
-        return NULL;
-    if (d) {
-        if (!PyMapping_Check(d)) {
-            PyErr_SetString(PyExc_TypeError,
-                    "argument 2 must be a mapping");
-            return NULL;
-        }
-        return _escape_item(self, o, d);
-    } else {
-        if (!self) {
-            PyErr_SetString(PyExc_TypeError,
-                    "argument 2 must be a mapping");
-            return NULL;
-        }
-        return _escape_item(self, o,
-               ((_mysql_ConnectionObject *) self)->converter);
-    }
-}
-
-static char _mysql_ResultObject_describe__doc__[] =
-"Returns the sequence of 7-tuples required by the DB-API for\n\
-the Cursor.description attribute.\n\
-";
-
-static PyObject *
-_mysql_ResultObject_describe(
-    _mysql_ResultObject *self,
-    PyObject *noargs)
-{
-    PyObject *d;
-    MYSQL_FIELD *fields;
-    unsigned int i, n;
-
-    check_result_connection(self);
-
-    n = mysql_num_fields(self->result);
-    fields = mysql_fetch_fields(self->result);
-    if (!(d = PyTuple_New(n))) return NULL;
-    for (i=0; i<n; i++) {
-        PyObject *t;
-        PyObject *name;
-        if (self->encoding == utf8) {
-            name = PyUnicode_DecodeUTF8(fields[i].name, fields[i].name_length, "replace");
-        } else {
-            name = PyUnicode_Decode(fields[i].name, fields[i].name_length, self->encoding, "replace");
-        }
-        if (name == NULL) {
-            goto error;
-        }
-
-        t = Py_BuildValue("(Niiiiii)",
-                  name,
-                  (long) fields[i].type,
-                  (long) fields[i].max_length,
-                  (long) fields[i].length,
-                  (long) fields[i].length,
-                  (long) fields[i].decimals,
-                  (long) !(IS_NOT_NULL(fields[i].flags)));
-        if (!t) goto error;
-        PyTuple_SET_ITEM(d, i, t);
-    }
-    return d;
-  error:
-    Py_XDECREF(d);
-    return NULL;
-}
-
-static char _mysql_ResultObject_field_flags__doc__[] =
-"Returns a tuple of field flags, one for each column in the result.\n\
-" ;
-
-static PyObject *
-_mysql_ResultObject_field_flags(
-    _mysql_ResultObject *self,
-    PyObject *noargs)
-{
-    PyObject *d;
-    MYSQL_FIELD *fields;
-    unsigned int i, n;
-    check_result_connection(self);
-    n = mysql_num_fields(self->result);
-    fields = mysql_fetch_fields(self->result);
-    if (!(d = PyTuple_New(n))) return NULL;
-    for (i=0; i<n; i++) {
-        PyObject *f;
-        if (!(f = PyLong_FromLong((long)fields[i].flags))) goto error;
-        PyTuple_SET_ITEM(d, i, f);
-    }
-    return d;
-  error:
-    Py_XDECREF(d);
-    return NULL;
-}
-
-static PyObject *
-_mysql_field_to_python(
-    PyObject *converter,
-    const char *rowitem,
-    Py_ssize_t length,
-    MYSQL_FIELD *field,
-    const char *encoding)
-{
-    if (rowitem == NULL) {
-        Py_RETURN_NONE;
-    }
-
-    // Fast paths for int, string and binary.
-    if (converter == (PyObject*)&PyUnicode_Type) {
-        if (encoding == utf8) {
-            //fprintf(stderr, "decoding with utf8!\n");
-            return PyUnicode_DecodeUTF8(rowitem, length, NULL);
-        } else {
-            //fprintf(stderr, "decoding with %s\n", encoding);
-            return PyUnicode_Decode(rowitem, length, encoding, NULL);
-        }
-    }
-    if (converter == (PyObject*)&PyBytes_Type || converter == Py_None) {
-        //fprintf(stderr, "decoding with bytes\n", encoding);
-        return PyBytes_FromStringAndSize(rowitem, length);
-    }
-    if (converter == (PyObject*)&PyLong_Type) {
-        //fprintf(stderr, "decoding with int\n", encoding);
-        return PyLong_FromString(rowitem, NULL, 10);
-    }
-
-    //fprintf(stderr, "decoding with callback\n");
-    //PyObject_Print(converter, stderr, 0);
-    //fprintf(stderr, "\n");
-    int binary;
-    switch (field->type) {
-    case FIELD_TYPE_DECIMAL:
-    case FIELD_TYPE_NEWDECIMAL:
-    case FIELD_TYPE_TIMESTAMP:
-    case FIELD_TYPE_DATETIME:
-    case FIELD_TYPE_TIME:
-    case FIELD_TYPE_DATE:
-        binary = 0;  // pass str, because these converters expect it
-        break;
-    default: // Default to just passing bytes
-        binary = 1;
-    }
-    return PyObject_CallFunction(converter,
-            binary ? "y#" : "s#",
-            rowitem, (Py_ssize_t)length);
-}
-
-static PyObject *
-_mysql_row_to_tuple(
-    _mysql_ResultObject *self,
-    MYSQL_ROW row,
-    PyObject *unused)
-{
-    unsigned int n, i;
-    unsigned long *length;
-    PyObject *r, *c;
-    MYSQL_FIELD *fields;
-
-    n = mysql_num_fields(self->result);
-    if (!(r = PyTuple_New(n))) return NULL;
-    length = mysql_fetch_lengths(self->result);
-    fields = mysql_fetch_fields(self->result);
-    for (i=0; i<n; i++) {
-        PyObject *v;
-        c = PyTuple_GET_ITEM(self->converter, i);
-        v = _mysql_field_to_python(c, row[i], length[i], &fields[i], self->encoding);
-        if (!v) goto error;
-        PyTuple_SET_ITEM(r, i, v);
-    }
-    return r;
-  error:
-    Py_XDECREF(r);
-    return NULL;
-}
-
-static PyObject *
-_mysql_row_to_dict(
-    _mysql_ResultObject *self,
-    MYSQL_ROW row,
-    PyObject *cache)
-{
-    unsigned int n, i;
-    unsigned long *length;
-    PyObject *r, *c;
-    MYSQL_FIELD *fields;
-
-    n = mysql_num_fields(self->result);
-    if (!(r = PyDict_New())) return NULL;
-    length = mysql_fetch_lengths(self->result);
-    fields = mysql_fetch_fields(self->result);
-    for (i=0; i<n; i++) {
-        PyObject *v;
-        c = PyTuple_GET_ITEM(self->converter, i);
-        v = _mysql_field_to_python(c, row[i], length[i], &fields[i], self->encoding);
-        if (!v) goto error;
-
-        PyObject *pyname = PyUnicode_FromString(fields[i].name);
-        if (pyname == NULL) {
-            Py_DECREF(v);
-            goto error;
-        }
-        int err = PyDict_Contains(r, pyname);
-        if (err < 0) { // error
-            Py_DECREF(v);
-            goto error;
-        }
-        if (err) { // duplicate
-            Py_DECREF(pyname);
-            pyname = PyUnicode_FromFormat("%s.%s", fields[i].table, fields[i].name);
-            if (pyname == NULL) {
-                Py_DECREF(v);
-                goto error;
-            }
-        }
-
-        err = PyDict_SetItem(r, pyname, v);
-        if (cache) {
-            PyTuple_SET_ITEM(cache, i, pyname);
-        } else {
-            Py_DECREF(pyname);
-        }
-        Py_DECREF(v);
-        if (err) {
-            goto error;
-        }
-    }
-    return r;
-error:
-    Py_DECREF(r);
-    return NULL;
-}
-
-static PyObject *
-_mysql_row_to_dict_old(
-    _mysql_ResultObject *self,
-    MYSQL_ROW row,
-    PyObject *cache)
-{
-    unsigned int n, i;
-    unsigned long *length;
-    PyObject *r, *c;
-    MYSQL_FIELD *fields;
-
-    n = mysql_num_fields(self->result);
-    if (!(r = PyDict_New())) return NULL;
-    length = mysql_fetch_lengths(self->result);
-    fields = mysql_fetch_fields(self->result);
-    for (i=0; i<n; i++) {
-        PyObject *v;
-        c = PyTuple_GET_ITEM(self->converter, i);
-        v = _mysql_field_to_python(c, row[i], length[i], &fields[i], self->encoding);
-        if (!v) {
-            goto error;
-        }
-
-        PyObject *pyname;
-        if (strlen(fields[i].table)) {
-            pyname = PyUnicode_FromFormat("%s.%s", fields[i].table, fields[i].name);
-        } else {
-            pyname = PyUnicode_FromString(fields[i].name);
-        }
-        int err = PyDict_SetItem(r, pyname, v);
-        Py_DECREF(v);
-        if (cache) {
-            PyTuple_SET_ITEM(cache, i, pyname);
-        } else {
-            Py_DECREF(pyname);
-        }
-        if (err) {
-            goto error;
-        }
-    }
-    return r;
-  error:
-    Py_XDECREF(r);
-    return NULL;
-}
-
-static PyObject *
-_mysql_row_to_dict_cached(
-    _mysql_ResultObject *self,
-    MYSQL_ROW row,
-    PyObject *cache)
-{
-    PyObject *r = PyDict_New();
-    if (!r) {
-        return NULL;
-    }
-
-    unsigned int n = mysql_num_fields(self->result);
-    unsigned long *length = mysql_fetch_lengths(self->result);
-    MYSQL_FIELD *fields = mysql_fetch_fields(self->result);
-
-    for (unsigned int i=0; i<n; i++) {
-        PyObject *c = PyTuple_GET_ITEM(self->converter, i);
-        PyObject *v = _mysql_field_to_python(c, row[i], length[i], &fields[i], self->encoding);
-        if (!v) {
-            goto error;
-        }
-
-        PyObject *pyname = PyTuple_GET_ITEM(cache, i); // borrowed
-        int err = PyDict_SetItem(r, pyname, v);
-        Py_DECREF(v);
-        if (err) {
-            goto error;
-        }
-    }
-    return r;
-  error:
-    Py_XDECREF(r);
-    return NULL;
-}
-
-
-typedef PyObject *_convertfunc(_mysql_ResultObject *, MYSQL_ROW, PyObject *);
-static _convertfunc * const row_converters[] = {
-    _mysql_row_to_tuple,
-    _mysql_row_to_dict,
-    _mysql_row_to_dict_old
-};
-
-Py_ssize_t
-_mysql__fetch_row(
-    _mysql_ResultObject *self,
-    PyObject *r, /* list object */
-    Py_ssize_t maxrows,
-    int how)
-{
-    _convertfunc *convert_row = row_converters[how];
-
-    PyObject *cache = NULL;
-    if (maxrows > 0 && how > 0) {
-        cache = PyTuple_New(mysql_num_fields(self->result));
-        if (!cache) {
-            return -1;
-        }
-    }
-
-    Py_ssize_t i;
-    for (i = 0; i < maxrows; i++) {
-        MYSQL_ROW row;
-        if (!self->use)
-            row = mysql_fetch_row(self->result);
-        else {
-            Py_BEGIN_ALLOW_THREADS
-            row = mysql_fetch_row(self->result);
-            Py_END_ALLOW_THREADS
-        }
-        if (!row && mysql_errno(&(((_mysql_ConnectionObject *)(self->conn))->connection))) {
-            _mysql_Exception((_mysql_ConnectionObject *)self->conn);
-            goto error;
-        }
-        if (!row) {
-            break;
-        }
-        PyObject *v = convert_row(self, row, cache);
-        if (!v) {
-            goto error;
-        }
-        if (cache) {
-            convert_row = _mysql_row_to_dict_cached;
-        }
-        if (PyList_Append(r, v)) {
-            Py_DECREF(v);
-            goto error;
-        }
-        Py_DECREF(v);
-    }
-    Py_XDECREF(cache);
-    return i;
-error:
-    Py_XDECREF(cache);
-    return -1;
-}
-
-static char _mysql_ResultObject_fetch_row__doc__[] =
-"fetch_row([maxrows, how]) -- Fetches up to maxrows as a tuple.\n\
-The rows are formatted according to how:\n\
-\n\
-    0 -- tuples (default)\n\
-    1 -- dictionaries, key=column or table.column if duplicated\n\
-    2 -- dictionaries, key=table.column\n\
-";
-
-static PyObject *
-_mysql_ResultObject_fetch_row(
-    _mysql_ResultObject *self,
-    PyObject *args,
-    PyObject *kwargs)
-{
-    static char *kwlist[] = {"maxrows", "how", NULL };
-    int maxrows=1, how=0;
-    PyObject *r=NULL;
-
-    if (!PyArg_ParseTupleAndKeywords(args, kwargs, "|ii:fetch_row", kwlist,
-                     &maxrows, &how))
-        return NULL;
-    check_result_connection(self);
-    if (how >= (int)(sizeof(row_converters) / sizeof(row_converters[0]))) {
-        PyErr_SetString(PyExc_ValueError, "how out of range");
-        return NULL;
-    }
-    if (!maxrows) {
-        if (self->use) {
-            maxrows = INT_MAX;
-        } else {
-            // todo: preallocate.
-            maxrows = (Py_ssize_t) mysql_num_rows(self->result);
-        }
-    }
-    if (!(r = PyList_New(0))) goto error;
-    Py_ssize_t rowsadded = _mysql__fetch_row(self, r, maxrows, how);
-    if (rowsadded == -1) goto error;
-
-    /* DB-API allows return rows as list.
-     * But we need to return list because Django expecting tuple.
-     */
-    PyObject *t = PyList_AsTuple(r);
-    Py_DECREF(r);
-    return t;
-  error:
-    Py_XDECREF(r);
-    return NULL;
-}
-
-static const char _mysql_ResultObject_discard__doc__[] =
-"discard() -- Discard remaining rows in the resultset.";
-
-static PyObject *
-_mysql_ResultObject_discard(
-    _mysql_ResultObject *self,
-    PyObject *noargs)
-{
-    check_result_connection(self);
-
-    MYSQL_ROW row;
-    Py_BEGIN_ALLOW_THREADS
-    while (NULL != (row = mysql_fetch_row(self->result))) {
-        // do nothing
-    }
-    Py_END_ALLOW_THREADS
-    _mysql_ConnectionObject *conn = (_mysql_ConnectionObject *)self->conn;
-    if (mysql_errno(&conn->connection)) {
-        return _mysql_Exception(conn);
-    }
-    Py_RETURN_NONE;
-}
-
-static char _mysql_ConnectionObject_change_user__doc__[] =
-"Changes the user and causes the database specified by db to\n\
-become the default (current) database on the connection\n\
-specified by mysql. In subsequent queries, this database is\n\
-the default for table references that do not include an\n\
-explicit database specifier.\n\
-\n\
-This function was introduced in MySQL Version 3.23.3.\n\
-\n\
-Fails unless the connected user can be authenticated or if he\n\
-doesn't have permission to use the database. In this case the\n\
-user and database are not changed.\n\
-\n\
-The db parameter may be set to None if you don't want to have\n\
-a default database.\n\
-";
-
-static PyObject *
-_mysql_ConnectionObject_change_user(
-    _mysql_ConnectionObject *self,
-    PyObject *args,
-    PyObject *kwargs)
-{
-    char *user, *pwd=NULL, *db=NULL;
-    int r;
-    static char *kwlist[] = { "user", "passwd", "db", NULL } ;
-
-    if (!PyArg_ParseTupleAndKeywords(args, kwargs, "s|ss:change_user",
-                     kwlist, &user, &pwd, &db))
-        return NULL;
-    check_connection(self);
-    Py_BEGIN_ALLOW_THREADS
-        r = mysql_change_user(&(self->connection), user, pwd, db);
-    Py_END_ALLOW_THREADS
-    if (r)     return _mysql_Exception(self);
-    Py_RETURN_NONE;
-}
-
-static char _mysql_ConnectionObject_character_set_name__doc__[] =
-"Returns the default character set for the current connection.\n\
-Non-standard.\n\
-";
-
-static PyObject *
-_mysql_ConnectionObject_character_set_name(
-    _mysql_ConnectionObject *self,
-    PyObject *noargs)
-{
-    const char *s;
-    check_connection(self);
-    s = mysql_character_set_name(&(self->connection));
-    return PyUnicode_FromString(s);
-}
-
-static char _mysql_ConnectionObject_set_character_set__doc__[] =
-"Sets the default character set for the current connection.\n\
-Non-standard.\n\
-";
-
-static PyObject *
-_mysql_ConnectionObject_set_character_set(
-    _mysql_ConnectionObject *self,
-    PyObject *args)
-{
-    const char *s;
-    int err;
-    if (!PyArg_ParseTuple(args, "s", &s)) return NULL;
-    check_connection(self);
-    Py_BEGIN_ALLOW_THREADS
-    err = mysql_set_character_set(&(self->connection), s);
-    Py_END_ALLOW_THREADS
-    if (err) return _mysql_Exception(self);
-    Py_RETURN_NONE;
-}
-
-#if MYSQL_VERSION_ID >= 50010
-static char _mysql_ConnectionObject_get_character_set_info__doc__[] =
-"Returns a dict with information about the current character set:\n\
-\n\
-collation\n\
-    collation name\n\
-name\n\
-    character set name\n\
-comment\n\
-    comment or descriptive name\n\
-dir\n\
-    character set directory\n\
-mbminlen\n\
-    min. length for multibyte string\n\
-mbmaxlen\n\
-    max. length for multibyte string\n\
-\n\
-Not all keys may be present, particularly dir.\n\
-\n\
-Non-standard.\n\
-";
-
-static PyObject *
-_mysql_ConnectionObject_get_character_set_info(
-    _mysql_ConnectionObject *self,
-    PyObject *noargs)
-{
-    PyObject *result;
-    MY_CHARSET_INFO cs;
-
-    check_connection(self);
-    mysql_get_character_set_info(&(self->connection), &cs);
-    if (!(result = PyDict_New())) return NULL;
-    if (cs.csname)
-        PyDict_SetItemString(result, "name", PyUnicode_FromString(cs.csname));
-    if (cs.name)
-        PyDict_SetItemString(result, "collation", PyUnicode_FromString(cs.name));
-    if (cs.comment)
-        PyDict_SetItemString(result, "comment", PyUnicode_FromString(cs.comment));
-    if (cs.dir)
-        PyDict_SetItemString(result, "dir", PyUnicode_FromString(cs.dir));
-    PyDict_SetItemString(result, "mbminlen", PyLong_FromLong(cs.mbminlen));
-    PyDict_SetItemString(result, "mbmaxlen", PyLong_FromLong(cs.mbmaxlen));
-    return result;
-}
-#endif
-
-static char _mysql_ConnectionObject_get_native_connection__doc__[] =
-"Return the internal MYSQL* wrapped in a PyCapsule object.\n\
-NOTE: this is a private API introduced ONLY for XTA integration,\n\
-      don't use it for different use cases.\n\
-      This method is supported only for XTA integration and support must\n\
-      be asked to LIXA project: http://www.tiian.org/lixa/\n\
-      Please DO NOT ask support to PyMySQL/mysqlclient-python project.\n\
-";
-
-static PyObject *
-_mysql_ConnectionObject_get_native_connection(
-    _mysql_ConnectionObject *self,
-    PyObject *noargs)
-{
-    PyObject *result;
-    check_connection(self);
-    result = PyCapsule_New(&(self->connection),
-        "_mysql.connection.native_connection", NULL);
-    return result;
-}
-
-
-static char _mysql_get_client_info__doc__[] =
-"get_client_info() -- Returns a string that represents\n\
-the client library version.";
-static PyObject *
-_mysql_get_client_info(
-    PyObject *self,
-    PyObject *noargs)
-{
-    return PyUnicode_FromString(mysql_get_client_info());
-}
-
-static char _mysql_ConnectionObject_get_host_info__doc__[] =
-"Returns a string that represents the MySQL client library\n\
-version. Non-standard.\n\
-";
-
-static PyObject *
-_mysql_ConnectionObject_get_host_info(
-    _mysql_ConnectionObject *self,
-    PyObject *noargs)
-{
-    check_connection(self);
-    return PyUnicode_FromString(mysql_get_host_info(&(self->connection)));
-}
-
-static char _mysql_ConnectionObject_get_proto_info__doc__[] =
-"Returns an unsigned integer representing the protocol version\n\
-used by the current connection. Non-standard.\n\
-";
-
-static PyObject *
-_mysql_ConnectionObject_get_proto_info(
-    _mysql_ConnectionObject *self,
-    PyObject *noargs)
-{
-    check_connection(self);
-    return PyLong_FromLong((long)mysql_get_proto_info(&(self->connection)));
-}
-
-static char _mysql_ConnectionObject_get_server_info__doc__[] =
-"Returns a string that represents the server version number.\n\
-Non-standard.\n\
-";
-
-static PyObject *
-_mysql_ConnectionObject_get_server_info(
-    _mysql_ConnectionObject *self,
-    PyObject *noargs)
-{
-    check_connection(self);
-    return PyUnicode_FromString(mysql_get_server_info(&(self->connection)));
-}
-
-static char _mysql_ConnectionObject_info__doc__[] =
-"Retrieves a string providing information about the most\n\
-recently executed query. Non-standard. Use messages or\n\
-Cursor.messages.\n\
-";
-
-static PyObject *
-_mysql_ConnectionObject_info(
-    _mysql_ConnectionObject *self,
-    PyObject *noargs)
-{
-    const char *s;
-    check_connection(self);
-    s = mysql_info(&(self->connection));
-    if (s) return PyUnicode_FromString(s);
-    Py_RETURN_NONE;
-}
-
-static char _mysql_ConnectionObject_insert_id__doc__[] =
-"Returns the ID generated for an AUTO_INCREMENT column by the previous\n\
-query. Use this function after you have performed an INSERT query into a\n\
-table that contains an AUTO_INCREMENT field.\n\
-\n\
-Note that this returns 0 if the previous query does not\n\
-generate an AUTO_INCREMENT value. If you need to save the value for\n\
-later, be sure to call this immediately after the query\n\
-that generates the value.\n\
-\n\
-The ID is updated after INSERT and UPDATE statements that generate\n\
-an AUTO_INCREMENT value or that set a column value to\n\
-LAST_INSERT_ID(expr). See section 6.3.5.2 Miscellaneous Functions\n\
-in the MySQL documentation.\n\
-\n\
-Also note that the value of the SQL LAST_INSERT_ID() function always\n\
-contains the most recently generated AUTO_INCREMENT value, and is not\n\
-reset between queries because the value of that function is maintained\n\
-in the server.\n\
-" ;
-
-static PyObject *
-_mysql_ConnectionObject_insert_id(
-    _mysql_ConnectionObject *self,
-    PyObject *noargs)
-{
-    my_ulonglong r;
-    check_connection(self);
-    r = mysql_insert_id(&(self->connection));
-    return PyLong_FromUnsignedLongLong(r);
-}
-
-static char _mysql_ConnectionObject_kill__doc__[] =
-"Asks the server to kill the thread specified by pid.\n\
-Non-standard.";
-
-static PyObject *
-_mysql_ConnectionObject_kill(
-    _mysql_ConnectionObject *self,
-    PyObject *args)
-{
-    unsigned long pid;
-    int r;
-    if (!PyArg_ParseTuple(args, "k:kill", &pid)) return NULL;
-    check_connection(self);
-    Py_BEGIN_ALLOW_THREADS
-    r = mysql_kill(&(self->connection), pid);
-    Py_END_ALLOW_THREADS
-    if (r) return _mysql_Exception(self);
-    Py_RETURN_NONE;
-}
-
-static char _mysql_ConnectionObject_field_count__doc__[] =
-"Returns the number of columns for the most recent query on the\n\
-connection. Non-standard. Will probably give you bogus results\n\
-on most cursor classes. Use Cursor.rowcount.\n\
-";
-
-static PyObject *
-_mysql_ConnectionObject_field_count(
-    _mysql_ConnectionObject *self,
-    PyObject *noargs)
-{
-    check_connection(self);
-    return PyLong_FromLong((long)mysql_field_count(&(self->connection)));
-}
-
-static char _mysql_ConnectionObject_fileno__doc__[] =
-"Return file descriptor of the underlying libmysqlclient connection.\n\
-This provides raw access to the underlying network connection.\n\
-";
-
-static PyObject *
-_mysql_ConnectionObject_fileno(
-    _mysql_ConnectionObject *self,
-    PyObject *noargs)
-{
-    check_connection(self);
-    return PyLong_FromLong(self->connection.net.fd);
-}
-
-static char _mysql_ResultObject_num_fields__doc__[] =
-"Returns the number of fields (column) in the result." ;
-
-static PyObject *
-_mysql_ResultObject_num_fields(
-    _mysql_ResultObject *self,
-    PyObject *noargs)
-{
-    check_result_connection(self);
-    return PyLong_FromLong((long)mysql_num_fields(self->result));
-}
-
-static char _mysql_ResultObject_num_rows__doc__[] =
-"Returns the number of rows in the result set. Note that if\n\
-use=1, this will not return a valid value until the entire result\n\
-set has been read.\n\
-";
-
-static PyObject *
-_mysql_ResultObject_num_rows(
-    _mysql_ResultObject *self,
-    PyObject *noargs)
-{
-    check_result_connection(self);
-    return PyLong_FromUnsignedLongLong(mysql_num_rows(self->result));
-}
-
-static char _mysql_ConnectionObject_ping__doc__[] =
-"Checks whether or not the connection to the server is\n\
-working. If it has gone down, an automatic reconnection is\n\
-attempted.\n\
-\n\
-This function can be used by clients that remain idle for a\n\
-long while, to check whether or not the server has closed the\n\
-connection and reconnect if necessary.\n\
-\n\
-New in 1.2.2: Accepts an optional reconnect parameter. If True,\n\
-then the client will attempt reconnection. Note that this setting\n\
-is persistent. By default, this is on in MySQL<5.0.3, and off\n\
-thereafter.\n\
-\n\
-Non-standard. You should assume that ping() performs an\n\
-implicit rollback; use only when starting a new transaction.\n\
-You have been warned.\n\
-";
-
-static PyObject *
-_mysql_ConnectionObject_ping(
-    _mysql_ConnectionObject *self,
-    PyObject *args)
-{
-    int r, reconnect = -1;
-    if (!PyArg_ParseTuple(args, "|I", &reconnect)) return NULL;
-    check_connection(self);
-    if (reconnect != -1) {
-        my_bool recon = (my_bool)reconnect;
-        mysql_options(&self->connection, MYSQL_OPT_RECONNECT, &recon);
-    }
-    Py_BEGIN_ALLOW_THREADS
-    r = mysql_ping(&(self->connection));
-    Py_END_ALLOW_THREADS
-    if (r)     return _mysql_Exception(self);
-    Py_RETURN_NONE;
-}
-
-static char _mysql_ConnectionObject_query__doc__[] =
-"Execute a query. store_result() or use_result() will get the\n\
-result set, if any. Non-standard. Use cursor() to create a cursor,\n\
-then cursor.execute().\n\
-" ;
-
-static PyObject *
-_mysql_ConnectionObject_query(
-    _mysql_ConnectionObject *self,
-    PyObject *args)
-{
-    char *query;
-    Py_ssize_t len;
-    int r;
-    if (!PyArg_ParseTuple(args, "s#:query", &query, &len)) return NULL;
-    check_connection(self);
-
-    Py_BEGIN_ALLOW_THREADS
-    r = mysql_real_query(&(self->connection), query, len);
-    Py_END_ALLOW_THREADS
-    if (r) return _mysql_Exception(self);
-    Py_RETURN_NONE;
-}
-
-
-static char _mysql_ConnectionObject_send_query__doc__[] =
-"Send a query. Same to query() except not wait response.\n\n\
-Use read_query_result() before calling store_result() or use_result()\n";
-
-static PyObject *
-_mysql_ConnectionObject_send_query(
-    _mysql_ConnectionObject *self,
-    PyObject *args)
-{
-    char *query;
-    Py_ssize_t len;
-    int r;
-    MYSQL *mysql = &(self->connection);
-    if (!PyArg_ParseTuple(args, "s#:query", &query, &len)) return NULL;
-    check_connection(self);
-
-    Py_BEGIN_ALLOW_THREADS
-    r = mysql_send_query(mysql, query, len);
-    Py_END_ALLOW_THREADS
-    if (r) return _mysql_Exception(self);
-    Py_RETURN_NONE;
-}
-
-
-static char _mysql_ConnectionObject_read_query_result__doc__[] =
-"Read result of query sent by send_query().\n";
-
-static PyObject *
-_mysql_ConnectionObject_read_query_result(
-    _mysql_ConnectionObject *self,
-    PyObject *noargs)
-{
-    int r;
-    MYSQL *mysql = &(self->connection);
-    check_connection(self);
-
-    Py_BEGIN_ALLOW_THREADS
-    r = (int)mysql_read_query_result(mysql);
-    Py_END_ALLOW_THREADS
-    if (r) return _mysql_Exception(self);
-    Py_RETURN_NONE;
-}
-
-static char _mysql_ConnectionObject_select_db__doc__[] =
-"Causes the database specified by db to become the default\n\
-(current) database on the connection specified by mysql. In subsequent\n\
-queries, this database is the default for table references that do not\n\
-include an explicit database specifier.\n\
-\n\
-Fails unless the connected user can be authenticated as having\n\
-permission to use the database.\n\
-\n\
-Non-standard.\n\
-";
-
-static PyObject *
-_mysql_ConnectionObject_select_db(
-    _mysql_ConnectionObject *self,
-    PyObject *args)
-{
-    char *db;
-    int r;
-    if (!PyArg_ParseTuple(args, "s:select_db", &db)) return NULL;
-    check_connection(self);
-    Py_BEGIN_ALLOW_THREADS
-    r = mysql_select_db(&(self->connection), db);
-    Py_END_ALLOW_THREADS
-    if (r)     return _mysql_Exception(self);
-    Py_RETURN_NONE;
-}
-
-static char _mysql_ConnectionObject_shutdown__doc__[] =
-"Asks the database server to shut down. The connected user must\n\
-have shutdown privileges. Non-standard.\n\
-";
-
-static PyObject *
-_mysql_ConnectionObject_shutdown(
-    _mysql_ConnectionObject *self,
-    PyObject *noargs)
-{
-    int r;
-    check_connection(self);
-    Py_BEGIN_ALLOW_THREADS
-    r = mysql_shutdown(&(self->connection), SHUTDOWN_DEFAULT);
-    Py_END_ALLOW_THREADS
-    if (r) return _mysql_Exception(self);
-    Py_RETURN_NONE;
-}
-
-static char _mysql_ConnectionObject_stat__doc__[] =
-"Returns a character string containing information similar to\n\
-that provided by the mysqladmin status command. This includes\n\
-uptime in seconds and the number of running threads,\n\
-questions, reloads, and open tables. Non-standard.\n\
-";
-
-static PyObject *
-_mysql_ConnectionObject_stat(
-    _mysql_ConnectionObject *self,
-    PyObject *noargs)
-{
-    const char *s;
-    check_connection(self);
-    Py_BEGIN_ALLOW_THREADS
-    s = mysql_stat(&(self->connection));
-    Py_END_ALLOW_THREADS
-    if (!s) return _mysql_Exception(self);
-    return PyUnicode_FromString(s);
-}
-
-static char _mysql_ConnectionObject_store_result__doc__[] =
-"Returns a result object acquired by mysql_store_result\n\
-(results stored in the client). If no results are available,\n\
-None is returned. Non-standard.\n\
-";
-
-static PyObject *
-_mysql_ConnectionObject_store_result(
-    _mysql_ConnectionObject *self,
-    PyObject *noargs)
-{
-    PyObject *arglist=NULL, *kwarglist=NULL, *result=NULL;
-    _mysql_ResultObject *r=NULL;
-
-    check_connection(self);
-    arglist = Py_BuildValue("(OiO)", self, 0, self->converter);
-    if (!arglist) goto error;
-    kwarglist = PyDict_New();
-    if (!kwarglist) goto error;
-    r = MyAlloc(_mysql_ResultObject, _mysql_ResultObject_Type);
-    if (!r) goto error;
-    if (_mysql_ResultObject_Initialize(r, arglist, kwarglist)) {
-        Py_DECREF(r);
-        goto error;
-    }
-    result = (PyObject *) r;
-    if (!(r->result)) {
-        Py_DECREF(result);
-        Py_INCREF(Py_None);
-        result = Py_None;
-    }
-  error:
-    Py_XDECREF(arglist);
-    Py_XDECREF(kwarglist);
-    return result;
-}
-
-static char _mysql_ConnectionObject_thread_id__doc__[] =
-"Returns the thread ID of the current connection. This value\n\
-can be used as an argument to kill() to kill the thread.\n\
-\n\
-If the connection is lost and you reconnect with ping(), the\n\
-thread ID will change. This means you should not get the\n\
-thread ID and store it for later. You should get it when you\n\
-need it.\n\
-\n\
-Non-standard.";
-
-static PyObject *
-_mysql_ConnectionObject_thread_id(
-    _mysql_ConnectionObject *self,
-    PyObject *noargs)
-{
-    unsigned long pid;
-    check_connection(self);
-    pid = mysql_thread_id(&(self->connection));
-    return PyLong_FromLong((long)pid);
-}
-
-static char _mysql_ConnectionObject_use_result__doc__[] =
-"Returns a result object acquired by mysql_use_result\n\
-(results stored in the server). If no results are available,\n\
-None is returned. Non-standard.\n\
-";
-
-static PyObject *
-_mysql_ConnectionObject_use_result(
-    _mysql_ConnectionObject *self,
-    PyObject *noargs)
-{
-    PyObject *arglist=NULL, *kwarglist=NULL, *result=NULL;
-    _mysql_ResultObject *r=NULL;
-
-    check_connection(self);
-    arglist = Py_BuildValue("(OiO)", self, 1, self->converter);
-    if (!arglist) return NULL;
-    kwarglist = PyDict_New();
-    if (!kwarglist) goto error;
-    r = MyAlloc(_mysql_ResultObject, _mysql_ResultObject_Type);
-    if (!r) goto error;
-    if (_mysql_ResultObject_Initialize(r, arglist, kwarglist)) {
-        Py_DECREF(r);
-        goto error;
-    }
-    result = (PyObject *) r;
-    if (!(r->result)) {
-        Py_DECREF(result);
-        Py_INCREF(Py_None);
-        result = Py_None;
-    }
-  error:
-    Py_DECREF(arglist);
-    Py_XDECREF(kwarglist);
-    return result;
-}
-
-static const char _mysql_ConnectionObject_discard_result__doc__[] =
-"Discard current result set.\n\n"
-"This function can be called instead of use_result() or store_result(). Non-standard.";
-
-static PyObject *
-_mysql_ConnectionObject_discard_result(
-    _mysql_ConnectionObject *self,
-    PyObject *noargs)
-{
-    check_connection(self);
-    MYSQL *conn = &(self->connection);
-
-    Py_BEGIN_ALLOW_THREADS;
-
-    MYSQL_RES *res = mysql_use_result(conn);
-    if (res == NULL) {
-        Py_BLOCK_THREADS;
-        if (mysql_errno(conn) != 0) {
-            // fprintf(stderr, "mysql_use_result failed: %s\n", mysql_error(conn));
-            return _mysql_Exception(self);
-        }
-        Py_RETURN_NONE;
-    }
-
-    MYSQL_ROW row;
-    while (NULL != (row = mysql_fetch_row(res))) {
-        // do nothing.
-    }
-    mysql_free_result(res);
-    Py_END_ALLOW_THREADS;
-    if (mysql_errno(conn)) {
-        // fprintf(stderr, "mysql_free_result failed: %s\n", mysql_error(conn));
-        return _mysql_Exception(self);
-    }
-    Py_RETURN_NONE;
-}
-
-static void
-_mysql_ConnectionObject_dealloc(
-    _mysql_ConnectionObject *self)
-{
-    PyObject_GC_UnTrack(self);
-    if (self->open) {
-        mysql_close(&(self->connection));
-        self->open = 0;
-    }
-    Py_CLEAR(self->converter);
-    MyFree(self);
-}
-
-static PyObject *
-_mysql_ConnectionObject_repr(
-    _mysql_ConnectionObject *self)
-{
-    char buf[300];
-    if (self->open)
-        snprintf(buf, 300, "<_mysql.connection open to '%.256s' at %p>",
-            self->connection.host, self);
-    else
-        snprintf(buf, 300, "<_mysql.connection closed at %p>", self);
-    return PyUnicode_FromString(buf);
-}
-
-static char _mysql_ResultObject_data_seek__doc__[] =
-"data_seek(n) -- seek to row n of result set";
-static PyObject *
-_mysql_ResultObject_data_seek(
-     _mysql_ResultObject *self,
-     PyObject *args)
-{
-    unsigned int row;
-    if (!PyArg_ParseTuple(args, "i:data_seek", &row)) return NULL;
-    check_result_connection(self);
-    mysql_data_seek(self->result, row);
-    Py_RETURN_NONE;
-}
-
-static void
-_mysql_ResultObject_dealloc(
-    _mysql_ResultObject *self)
-{
-    PyObject_GC_UnTrack((PyObject *)self);
-    mysql_free_result(self->result);
-    _mysql_ResultObject_clear(self);
-    MyFree(self);
-}
-
-static PyObject *
-_mysql_ResultObject_repr(
-    _mysql_ResultObject *self)
-{
-    char buf[300];
-    snprintf(buf, 300, "<_mysql.result object at %p>", self);
-    return PyUnicode_FromString(buf);
-}
-
-static PyMethodDef _mysql_ConnectionObject_methods[] = {
-    {
-        "affected_rows",
-        (PyCFunction)_mysql_ConnectionObject_affected_rows,
-        METH_NOARGS,
-        _mysql_ConnectionObject_affected_rows__doc__
-    },
-    {
-        "autocommit",
-        (PyCFunction)_mysql_ConnectionObject_autocommit,
-        METH_VARARGS,
-        _mysql_ConnectionObject_autocommit__doc__
-    },
-    {
-        "get_autocommit",
-        (PyCFunction)_mysql_ConnectionObject_get_autocommit,
-        METH_NOARGS,
-        _mysql_ConnectionObject_get_autocommit__doc__
-    },
-    {
-        "commit",
-        (PyCFunction)_mysql_ConnectionObject_commit,
-        METH_NOARGS,
-        _mysql_ConnectionObject_commit__doc__
-    },
-    {
-        "rollback",
-        (PyCFunction)_mysql_ConnectionObject_rollback,
-        METH_NOARGS,
-        _mysql_ConnectionObject_rollback__doc__
-    },
-    {
-        "next_result",
-        (PyCFunction)_mysql_ConnectionObject_next_result,
-        METH_NOARGS,
-        _mysql_ConnectionObject_next_result__doc__
-    },
-    {
-        "set_server_option",
-        (PyCFunction)_mysql_ConnectionObject_set_server_option,
-        METH_VARARGS,
-        _mysql_ConnectionObject_set_server_option__doc__
-    },
-    {
-        "sqlstate",
-        (PyCFunction)_mysql_ConnectionObject_sqlstate,
-        METH_NOARGS,
-        _mysql_ConnectionObject_sqlstate__doc__
-    },
-    {
-        "warning_count",
-        (PyCFunction)_mysql_ConnectionObject_warning_count,
-        METH_NOARGS,
-        _mysql_ConnectionObject_warning_count__doc__
-    },
-    {
-        "change_user",
-        (PyCFunction)_mysql_ConnectionObject_change_user,
-        METH_VARARGS | METH_KEYWORDS,
-        _mysql_ConnectionObject_change_user__doc__
-    },
-    {
-        "character_set_name",
-        (PyCFunction)_mysql_ConnectionObject_character_set_name,
-        METH_NOARGS,
-        _mysql_ConnectionObject_character_set_name__doc__
-    },
-    {
-        "set_character_set",
-        (PyCFunction)_mysql_ConnectionObject_set_character_set,
-        METH_VARARGS,
-        _mysql_ConnectionObject_set_character_set__doc__
-    },
-#if MYSQL_VERSION_ID >= 50010
-    {
-        "get_character_set_info",
-        (PyCFunction)_mysql_ConnectionObject_get_character_set_info,
-        METH_NOARGS,
-        _mysql_ConnectionObject_get_character_set_info__doc__
-    },
-#endif
-    {
-        "_get_native_connection",
-        (PyCFunction)_mysql_ConnectionObject_get_native_connection,
-        METH_NOARGS,
-        _mysql_ConnectionObject_get_native_connection__doc__
-    },
-    {
-        "close",
-        (PyCFunction)_mysql_ConnectionObject_close,
-        METH_NOARGS,
-        _mysql_ConnectionObject_close__doc__
-    },
-    {
-        "dump_debug_info",
-        (PyCFunction)_mysql_ConnectionObject_dump_debug_info,
-        METH_NOARGS,
-        _mysql_ConnectionObject_dump_debug_info__doc__
-    },
-    {
-        "escape",
-        (PyCFunction)_mysql_escape,
-        METH_VARARGS,
-        _mysql_escape__doc__
-    },
-    {
-        "escape_string",
-        (PyCFunction)_mysql_escape_string,
-        METH_VARARGS,
-        _mysql_escape_string__doc__
-    },
-    {
-        "error",
-        (PyCFunction)_mysql_ConnectionObject_error,
-        METH_NOARGS,
-        _mysql_ConnectionObject_error__doc__
-    },
-    {
-        "errno",
-        (PyCFunction)_mysql_ConnectionObject_errno,
-        METH_NOARGS,
-        _mysql_ConnectionObject_errno__doc__
-    },
-    {
-        "field_count",
-        (PyCFunction)_mysql_ConnectionObject_field_count,
-        METH_NOARGS,
-        _mysql_ConnectionObject_field_count__doc__
-    },
-    {
-        "fileno",
-        (PyCFunction)_mysql_ConnectionObject_fileno,
-        METH_NOARGS,
-        _mysql_ConnectionObject_fileno__doc__
-    },
-    {
-        "get_host_info",
-        (PyCFunction)_mysql_ConnectionObject_get_host_info,
-        METH_NOARGS,
-        _mysql_ConnectionObject_get_host_info__doc__
-    },
-    {
-        "get_proto_info",
-        (PyCFunction)_mysql_ConnectionObject_get_proto_info,
-        METH_NOARGS,
-        _mysql_ConnectionObject_get_proto_info__doc__
-    },
-    {
-        "get_server_info",
-        (PyCFunction)_mysql_ConnectionObject_get_server_info,
-        METH_NOARGS,
-        _mysql_ConnectionObject_get_server_info__doc__
-    },
-    {
-        "info",
-        (PyCFunction)_mysql_ConnectionObject_info,
-        METH_NOARGS,
-        _mysql_ConnectionObject_info__doc__
-    },
-    {
-        "insert_id",
-        (PyCFunction)_mysql_ConnectionObject_insert_id,
-        METH_NOARGS,
-        _mysql_ConnectionObject_insert_id__doc__
-    },
-    {
-        "kill",
-        (PyCFunction)_mysql_ConnectionObject_kill,
-        METH_VARARGS,
-        _mysql_ConnectionObject_kill__doc__
-    },
-    {
-        "ping",
-        (PyCFunction)_mysql_ConnectionObject_ping,
-        METH_VARARGS,
-        _mysql_ConnectionObject_ping__doc__
-    },
-    {
-        "query",
-        (PyCFunction)_mysql_ConnectionObject_query,
-        METH_VARARGS,
-        _mysql_ConnectionObject_query__doc__
-    },
-    {
-        "send_query",
-        (PyCFunction)_mysql_ConnectionObject_send_query,
-        METH_VARARGS,
-        _mysql_ConnectionObject_send_query__doc__,
-    },
-    {
-        "read_query_result",
-        (PyCFunction)_mysql_ConnectionObject_read_query_result,
-        METH_NOARGS,
-        _mysql_ConnectionObject_read_query_result__doc__,
-    },
-    {
-        "select_db",
-        (PyCFunction)_mysql_ConnectionObject_select_db,
-        METH_VARARGS,
-        _mysql_ConnectionObject_select_db__doc__
-    },
-    {
-        "shutdown",
-        (PyCFunction)_mysql_ConnectionObject_shutdown,
-        METH_NOARGS,
-        _mysql_ConnectionObject_shutdown__doc__
-    },
-    {
-        "stat",
-        (PyCFunction)_mysql_ConnectionObject_stat,
-        METH_NOARGS,
-        _mysql_ConnectionObject_stat__doc__
-    },
-    {
-        "store_result",
-        (PyCFunction)_mysql_ConnectionObject_store_result,
-        METH_NOARGS,
-        _mysql_ConnectionObject_store_result__doc__
-    },
-    {
-        "string_literal",
-        (PyCFunction)_mysql_string_literal,
-        METH_O,
-        _mysql_string_literal__doc__},
-    {
-        "thread_id",
-        (PyCFunction)_mysql_ConnectionObject_thread_id,
-        METH_NOARGS,
-        _mysql_ConnectionObject_thread_id__doc__
-    },
-    {
-        "use_result",
-        (PyCFunction)_mysql_ConnectionObject_use_result,
-        METH_NOARGS,
-        _mysql_ConnectionObject_use_result__doc__
-    },
-    {
-        "discard_result",
-        (PyCFunction)_mysql_ConnectionObject_discard_result,
-        METH_NOARGS,
-        _mysql_ConnectionObject_discard_result__doc__
-    },
-    {NULL,              NULL} /* sentinel */
-};
-
-static struct PyMemberDef _mysql_ConnectionObject_memberlist[] = {
-    {
-        "open",
-        T_INT,
-        offsetof(_mysql_ConnectionObject,open),
-        READONLY,
-        "True if connection is open"
-    },
-    {
-        "converter",
-        T_OBJECT,
-        offsetof(_mysql_ConnectionObject,converter),
-        0,
-        "Type conversion mapping"
-    },
-    {
-        "server_capabilities",
-        T_ULONG,
-        offsetof(_mysql_ConnectionObject,connection.server_capabilities),
-        READONLY,
-        "Capabilities of server; consult MySQLdb.constants.CLIENT"
-    },
-    {
-        "port",
-        T_UINT,
-        offsetof(_mysql_ConnectionObject,connection.port),
-        READONLY,
-        "TCP/IP port of the server connection"
-    },
-    {
-        "client_flag",
-        T_ULONG,
-        offsetof(_mysql_ConnectionObject,connection.client_flag),
-        READONLY,
-        "Client flags; refer to MySQLdb.constants.CLIENT"
-    },
-    {NULL} /* Sentinel */
-};
-
-static PyMethodDef _mysql_ResultObject_methods[] = {
-    {
-        "data_seek",
-        (PyCFunction)_mysql_ResultObject_data_seek,
-        METH_VARARGS,
-        _mysql_ResultObject_data_seek__doc__
-    },
-    {
-        "describe",
-        (PyCFunction)_mysql_ResultObject_describe,
-        METH_NOARGS,
-        _mysql_ResultObject_describe__doc__
-    },
-    {
-        "fetch_row",
-        (PyCFunction)_mysql_ResultObject_fetch_row,
-        METH_VARARGS | METH_KEYWORDS,
-        _mysql_ResultObject_fetch_row__doc__
-    },
-    {
-        "discard",
-        (PyCFunction)_mysql_ResultObject_discard,
-        METH_NOARGS,
-        _mysql_ResultObject_discard__doc__
-    },
-    {
-        "field_flags",
-        (PyCFunction)_mysql_ResultObject_field_flags,
-        METH_NOARGS,
-        _mysql_ResultObject_field_flags__doc__
-    },
-    {
-        "num_fields",
-        (PyCFunction)_mysql_ResultObject_num_fields,
-        METH_NOARGS,
-        _mysql_ResultObject_num_fields__doc__
-    },
-    {
-        "num_rows",
-        (PyCFunction)_mysql_ResultObject_num_rows,
-        METH_NOARGS,
-        _mysql_ResultObject_num_rows__doc__
-    },
-    {NULL,              NULL} /* sentinel */
-};
-
-static struct PyMemberDef _mysql_ResultObject_memberlist[] = {
-    {
-        "converter",
-        T_OBJECT,
-        offsetof(_mysql_ResultObject,converter),
-        READONLY,
-        "Type conversion mapping"
-    },
-    {
-        "has_next",
-        T_BOOL,
-        offsetof(_mysql_ResultObject, has_next),
-        READONLY,
-        "Has next result"
-    },
-    {NULL} /* Sentinel */
-};
-
-static PyObject *
-_mysql_ConnectionObject_getattro(
-    _mysql_ConnectionObject *self,
-    PyObject *name)
-{
-    const char *cname;
-    cname = PyUnicode_AsUTF8(name);
-    if (strcmp(cname, "closed") == 0)
-        return PyLong_FromLong((long)!(self->open));
-
-    return PyObject_GenericGetAttr((PyObject *)self, name);
-}
-
-static int
-_mysql_ConnectionObject_setattro(
-    _mysql_ConnectionObject *self,
-    PyObject *name,
-    PyObject *v)
-{
-    if (v == NULL) {
-        PyErr_SetString(PyExc_AttributeError,
-                "can't delete connection attributes");
-        return -1;
-    }
-    return PyObject_GenericSetAttr((PyObject *)self, name, v);
-}
-
-static int
-_mysql_ResultObject_setattro(
-    _mysql_ResultObject *self,
-    PyObject *name,
-    PyObject *v)
-{
-    if (v == NULL) {
-        PyErr_SetString(PyExc_AttributeError,
-                "can't delete connection attributes");
-        return -1;
-    }
-    return PyObject_GenericSetAttr((PyObject *)self, name, v);
-}
-
-PyTypeObject _mysql_ConnectionObject_Type = {
-    PyVarObject_HEAD_INIT(NULL, 0)
-    "_mysql.connection", /* (char *)tp_name For printing */
-    sizeof(_mysql_ConnectionObject),
-    0,
-    (destructor)_mysql_ConnectionObject_dealloc, /* tp_dealloc */
-    0, /*tp_print*/
-    0, /* tp_getattr */
-    0, /* tp_setattr */
-    0, /*tp_compare*/
-    (reprfunc)_mysql_ConnectionObject_repr, /* tp_repr */
-
-    /* Method suites for standard classes */
-
-    0, /* (PyNumberMethods *) tp_as_number */
-    0, /* (PySequenceMethods *) tp_as_sequence */
-    0, /* (PyMappingMethods *) tp_as_mapping */
-
-    /* More standard operations (here for binary compatibility) */
-
-    0, /* (hashfunc) tp_hash */
-    0, /* (ternaryfunc) tp_call */
-    0, /* (reprfunc) tp_str */
-    (getattrofunc)_mysql_ConnectionObject_getattro, /* tp_getattro */
-    (setattrofunc)_mysql_ConnectionObject_setattro, /* tp_setattro */
-
-    /* Functions to access object as input/output buffer */
-    0, /* (PyBufferProcs *) tp_as_buffer */
-
-    /* (tp_flags) Flags to define presence of optional/expanded features */
-    Py_TPFLAGS_DEFAULT | Py_TPFLAGS_HAVE_GC | Py_TPFLAGS_BASETYPE,
-    _mysql_connect__doc__, /* (char *) tp_doc Documentation string */
-
-    /* call function for all accessible objects */
-    (traverseproc) _mysql_ConnectionObject_traverse, /* tp_traverse */
-
-    /* delete references to contained objects */
-    (inquiry) _mysql_ConnectionObject_clear, /* tp_clear */
-
-    /* rich comparisons */
-    0, /* (richcmpfunc) tp_richcompare */
-
-    /* weak reference enabler */
-    0, /* (long) tp_weaklistoffset */
-
-    /* Iterators */
-    0, /* (getiterfunc) tp_iter */
-    0, /* (iternextfunc) tp_iternext */
-
-    /* Attribute descriptor and subclassing stuff */
-    (struct PyMethodDef *)_mysql_ConnectionObject_methods, /* tp_methods */
-    (struct PyMemberDef *)_mysql_ConnectionObject_memberlist, /* tp_members */
-    0, /* (struct getsetlist *) tp_getset; */
-    0, /* (struct _typeobject *) tp_base; */
-    0, /* (PyObject *) tp_dict */
-    0, /* (descrgetfunc) tp_descr_get */
-    0, /* (descrsetfunc) tp_descr_set */
-    0, /* (long) tp_dictoffset */
-    (initproc)_mysql_ConnectionObject_Initialize, /* tp_init */
-    NULL, /* tp_alloc */
-    PyType_GenericNew, /* tp_new */
-    NULL, /* tp_free Low-level free-memory routine */
-    0, /* (PyObject *) tp_bases */
-    0, /* (PyObject *) tp_mro method resolution order */
-    0, /* (PyObject *) tp_defined */
-} ;
-
-PyTypeObject _mysql_ResultObject_Type = {
-    PyVarObject_HEAD_INIT(NULL, 0)
-    "_mysql.result",
-    sizeof(_mysql_ResultObject),
-    0,
-    (destructor)_mysql_ResultObject_dealloc, /* tp_dealloc */
-    0, /*tp_print*/
-    0, /* tp_getattr */
-    0, /* tp_setattr */
-    0, /*tp_compare*/
-    (reprfunc)_mysql_ResultObject_repr, /* tp_repr */
-
-    /* Method suites for standard classes */
-
-    0, /* (PyNumberMethods *) tp_as_number */
-    0, /* (PySequenceMethods *) tp_as_sequence */
-    0, /* (PyMappingMethods *) tp_as_mapping */
-
-    /* More standard operations (here for binary compatibility) */
-
-    0, /* (hashfunc) tp_hash */
-    0, /* (ternaryfunc) tp_call */
-    0, /* (reprfunc) tp_str */
-    (getattrofunc)PyObject_GenericGetAttr, /* tp_getattro */
-    (setattrofunc)_mysql_ResultObject_setattro, /* tp_setattr */
-
-    /* Functions to access object as input/output buffer */
-    0, /* (PyBufferProcs *) tp_as_buffer */
-
-    /* Flags to define presence of optional/expanded features */
-    Py_TPFLAGS_DEFAULT | Py_TPFLAGS_HAVE_GC | Py_TPFLAGS_BASETYPE,
-
-    _mysql_ResultObject__doc__, /* (char *) tp_doc Documentation string */
-
-    /* call function for all accessible objects */
-    (traverseproc) _mysql_ResultObject_traverse, /* tp_traverse */
-
-    /* delete references to contained objects */
-    (inquiry) _mysql_ResultObject_clear, /* tp_clear */
-
-    /* rich comparisons */
-    0, /* (richcmpfunc) tp_richcompare */
-
-    /* weak reference enabler */
-    0, /* (long) tp_weaklistoffset */
-
-    /* Iterators */
-    0, /* (getiterfunc) tp_iter */
-    0, /* (iternextfunc) tp_iternext */
-
-    /* Attribute descriptor and subclassing stuff */
-    (struct PyMethodDef *) _mysql_ResultObject_methods, /* tp_methods */
-    (struct PyMemberDef *) _mysql_ResultObject_memberlist, /*tp_members */
-    0, /* (struct getsetlist *) tp_getset; */
-    0, /* (struct _typeobject *) tp_base; */
-    0, /* (PyObject *) tp_dict */
-    0, /* (descrgetfunc) tp_descr_get */
-    0, /* (descrsetfunc) tp_descr_set */
-    0, /* (long) tp_dictoffset */
-    (initproc)_mysql_ResultObject_Initialize, /* tp_init */
-    NULL, /* tp_alloc */
-    PyType_GenericNew, /* tp_new */
-    NULL, /* tp_free Low-level free-memory routine */
-    0, /* (PyObject *) tp_bases */
-    0, /* (PyObject *) tp_mro method resolution order */
-    0, /* (PyObject *) tp_defined */
-};
-
-static PyMethodDef
-_mysql_methods[] = {
-    {
-        "connect",
-        (PyCFunction)_mysql_connect,
-        METH_VARARGS | METH_KEYWORDS,
-        _mysql_connect__doc__
-    },
-    {
-        "debug",
-        (PyCFunction)_mysql_debug,
-        METH_VARARGS,
-        _mysql_debug__doc__
-    },
-    {
-        "escape",
-        (PyCFunction)_mysql_escape,
-        METH_VARARGS,
-        _mysql_escape__doc__
-    },
-    {
-        "escape_string",
-        (PyCFunction)_mysql_escape_string,
-        METH_VARARGS,
-        _mysql_escape_string__doc__
-    },
-    {
-        "string_literal",
-        (PyCFunction)_mysql_string_literal,
-        METH_O,
-        _mysql_string_literal__doc__
-    },
-    {
-        "get_client_info",
-        (PyCFunction)_mysql_get_client_info,
-        METH_NOARGS,
-        _mysql_get_client_info__doc__
-    },
-    {NULL, NULL} /* sentinel */
-};
-
-static PyObject *
-_mysql_NewException(
-    PyObject *dict,
-    PyObject *edict,
-    char *name)
-{
-    PyObject *e;
-    if (!(e = PyDict_GetItemString(edict, name)))
-        return NULL;
-    if (PyDict_SetItemString(dict, name, e))
-        return NULL;
-    Py_INCREF(e);
-    return e;
-}
-
-#define QUOTE(X) _QUOTE(X)
-#define _QUOTE(X) #X
-
-static char _mysql___doc__[] =
-"an adaptation of the MySQL C API (mostly)\n\
-\n\
-You probably are better off using MySQLdb instead of using this\n\
-module directly.\n\
-\n\
-In general, renaming goes from mysql_* to _mysql.*. _mysql.connect()\n\
-returns a connection object (MYSQL). Functions which expect MYSQL * as\n\
-an argument are now methods of the connection object. A number of things\n\
-return result objects (MYSQL_RES). Functions which expect MYSQL_RES * as\n\
-an argument are now methods of the result object. Deprecated functions\n\
-(as of 3.23) are NOT implemented.\n\
-";
-
-static struct PyModuleDef _mysqlmodule = {
-   PyModuleDef_HEAD_INIT,
-   "_mysql",   /* name of module */
-   _mysql___doc__, /* module documentation, may be NULL */
-   -1,       /* size of per-interpreter state of the module,
-                or -1 if the module keeps state in global variables. */
-   _mysql_methods
-};
-
-PyMODINIT_FUNC
-PyInit__mysql(void)
-{
-    PyObject *dict, *module, *emod, *edict;
-
-    if (mysql_library_init(0, NULL, NULL)) {
-        PyErr_SetString(PyExc_ImportError, "_mysql: mysql_library_init failed");
-        return NULL;
-    }
-
-    if (PyType_Ready(&_mysql_ConnectionObject_Type) < 0)
-        return NULL;
-    if (PyType_Ready(&_mysql_ResultObject_Type) < 0)
-        return NULL;
-
-    module = PyModule_Create(&_mysqlmodule);
-    if (!module) return module; /* this really should never happen */
-
-    if (!(dict = PyModule_GetDict(module))) goto error;
-    if (PyDict_SetItemString(dict, "version_info",
-                   PyRun_String(QUOTE(version_info), Py_eval_input,
-                       dict, dict)))
-        goto error;
-    if (PyDict_SetItemString(dict, "__version__",
-                   PyUnicode_FromString(QUOTE(__version__))))
-        goto error;
-    if (PyDict_SetItemString(dict, "connection",
-                   (PyObject *)&_mysql_ConnectionObject_Type))
-        goto error;
-    Py_INCREF(&_mysql_ConnectionObject_Type);
-    if (PyDict_SetItemString(dict, "result",
-                   (PyObject *)&_mysql_ResultObject_Type))
-        goto error;
-    Py_INCREF(&_mysql_ResultObject_Type);
-    if (!(emod = PyImport_ImportModule("MySQLdb._exceptions"))) {
-        PyErr_Print();
-        goto error;
-    }
-    if (!(edict = PyModule_GetDict(emod))) goto error;
-    if (!(_mysql_MySQLError =
-          _mysql_NewException(dict, edict, "MySQLError")))
-        goto error;
-    if (!(_mysql_Warning =
-          _mysql_NewException(dict, edict, "Warning")))
-        goto error;
-    if (!(_mysql_Error =
-          _mysql_NewException(dict, edict, "Error")))
-        goto error;
-    if (!(_mysql_InterfaceError =
-          _mysql_NewException(dict, edict, "InterfaceError")))
-        goto error;
-    if (!(_mysql_DatabaseError =
-          _mysql_NewException(dict, edict, "DatabaseError")))
-        goto error;
-    if (!(_mysql_DataError =
-          _mysql_NewException(dict, edict, "DataError")))
-        goto error;
-    if (!(_mysql_OperationalError =
-          _mysql_NewException(dict, edict, "OperationalError")))
-        goto error;
-    if (!(_mysql_IntegrityError =
-          _mysql_NewException(dict, edict, "IntegrityError")))
-        goto error;
-    if (!(_mysql_InternalError =
-          _mysql_NewException(dict, edict, "InternalError")))
-        goto error;
-    if (!(_mysql_ProgrammingError =
-          _mysql_NewException(dict, edict, "ProgrammingError")))
-        goto error;
-    if (!(_mysql_NotSupportedError =
-          _mysql_NewException(dict, edict, "NotSupportedError")))
-        goto error;
-    Py_DECREF(emod);
-  error:
-    if (PyErr_Occurred()) {
-        PyErr_SetString(PyExc_ImportError, "_mysql: init failed");
-        module = NULL;
-    }
-    return module;
-}
-
-/* vim: set ts=4 sts=4 sw=4 expandtab : */
+/*
+This program is free software; you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation; either version 2, or (at your option)
+any later version. Alternatively, you may use the original license
+reproduced below.
+
+Copyright 1999 by Comstar.net, Inc., Atlanta, GA, US.
+
+                        All Rights Reserved
+
+Permission to use, copy, modify, and distribute this software and its
+documentation for any purpose and without fee is hereby granted,
+provided that the above copyright notice appear in all copies and that
+both that copyright notice and this permission notice appear in
+supporting documentation, and that the name of Comstar.net, Inc.
+or COMSTAR not be used in advertising or publicity pertaining to
+distribution of the software without specific, written prior permission.
+
+COMSTAR DISCLAIMS ALL WARRANTIES WITH REGARD TO THIS SOFTWARE,
+INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS, IN NO
+EVENT SHALL COMSTAR BE LIABLE FOR ANY SPECIAL, INDIRECT OR
+CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF
+USE, DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR
+OTHER TORTIOUS ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR
+PERFORMANCE OF THIS SOFTWARE.
+*/
+
+#include "mysql.h"
+#include "mysqld_error.h"
+
+#if MYSQL_VERSION_ID >= 80000
+// https://github.com/mysql/mysql-server/commit/eb821c023cedc029ca0b06456dfae365106bee84
+#define my_bool _Bool
+#endif
+
+#if ((MYSQL_VERSION_ID >= 50555 && MYSQL_VERSION_ID <= 50599) || \
+(MYSQL_VERSION_ID >= 50636 && MYSQL_VERSION_ID <= 50699) || \
+(MYSQL_VERSION_ID >= 50711 && MYSQL_VERSION_ID <= 50799) || \
+(MYSQL_VERSION_ID >= 80000)) && \
+!defined(MARIADB_BASE_VERSION) && !defined(MARIADB_VERSION_ID)
+#define HAVE_ENUM_MYSQL_OPT_SSL_MODE
+#endif
+
+#define PY_SSIZE_T_CLEAN 1
+#include "Python.h"
+
+#if PY_MAJOR_VERSION == 2
+#error "Python 2 is not supported"
+#endif
+
+#include "bytesobject.h"
+#include "structmember.h"
+#include "errmsg.h"
+
+#define MyAlloc(s,t) (s *) t.tp_alloc(&t,0)
+#define MyFree(o) Py_TYPE(o)->tp_free((PyObject*)o)
+
+static PyObject *_mysql_MySQLError;
+static PyObject *_mysql_Warning;
+static PyObject *_mysql_Error;
+static PyObject *_mysql_DatabaseError;
+static PyObject *_mysql_InterfaceError;
+static PyObject *_mysql_DataError;
+static PyObject *_mysql_OperationalError;
+static PyObject *_mysql_IntegrityError;
+static PyObject *_mysql_InternalError;
+static PyObject *_mysql_ProgrammingError;
+static PyObject *_mysql_NotSupportedError;
+
+typedef struct {
+    PyObject_HEAD
+    MYSQL connection;
+    int open;
+    PyObject *converter;
+} _mysql_ConnectionObject;
+
+#define check_connection(c) \
+    if (!(c->open)) { \
+        return _mysql_Exception(c); \
+    };
+
+#define result_connection(r) ((_mysql_ConnectionObject *)r->conn)
+#define check_result_connection(r) check_connection(result_connection(r))
+
+extern PyTypeObject _mysql_ConnectionObject_Type;
+
+typedef struct {
+    PyObject_HEAD
+    PyObject *conn;
+    MYSQL_RES *result;
+    int nfields;
+    int use;
+    char has_next;
+    PyObject *converter;
+    const char *encoding;
+} _mysql_ResultObject;
+
+extern PyTypeObject _mysql_ResultObject_Type;
+
+
+PyObject *
+_mysql_Exception(_mysql_ConnectionObject *c)
+{
+    PyObject *t, *e;
+    int merr;
+
+    if (!(t = PyTuple_New(2))) return NULL;
+    if (!(c->open)) {
+        /* GH-270: When connection is closed, accessing the c->connection
+         * object may cause SEGV.
+         */
+        merr = CR_SERVER_GONE_ERROR;
+    }
+    else {
+        merr = mysql_errno(&(c->connection));
+    }
+    switch (merr) {
+    case 0:
+        e = _mysql_InterfaceError;
+        break;
+    case CR_COMMANDS_OUT_OF_SYNC:
+    case ER_DB_CREATE_EXISTS:
+    case ER_SYNTAX_ERROR:
+    case ER_PARSE_ERROR:
+    case ER_NO_SUCH_TABLE:
+    case ER_WRONG_DB_NAME:
+    case ER_WRONG_TABLE_NAME:
+    case ER_FIELD_SPECIFIED_TWICE:
+    case ER_INVALID_GROUP_FUNC_USE:
+    case ER_UNSUPPORTED_EXTENSION:
+    case ER_TABLE_MUST_HAVE_COLUMNS:
+#ifdef ER_CANT_DO_THIS_DURING_AN_TRANSACTION
+    case ER_CANT_DO_THIS_DURING_AN_TRANSACTION:
+#endif
+        e = _mysql_ProgrammingError;
+        break;
+#ifdef WARN_DATA_TRUNCATED
+    case WARN_DATA_TRUNCATED:
+#ifdef WARN_NULL_TO_NOTNULL
+    case WARN_NULL_TO_NOTNULL:
+#endif
+#ifdef ER_WARN_DATA_OUT_OF_RANGE
+    case ER_WARN_DATA_OUT_OF_RANGE:
+#endif
+#ifdef ER_NO_DEFAULT
+    case ER_NO_DEFAULT:
+#endif
+#ifdef ER_PRIMARY_CANT_HAVE_NULL
+    case ER_PRIMARY_CANT_HAVE_NULL:
+#endif
+#ifdef ER_DATA_TOO_LONG
+    case ER_DATA_TOO_LONG:
+#endif
+#ifdef ER_DATETIME_FUNCTION_OVERFLOW
+    case ER_DATETIME_FUNCTION_OVERFLOW:
+#endif
+        e = _mysql_DataError;
+        break;
+#endif
+    case ER_DUP_ENTRY:
+#ifdef ER_DUP_UNIQUE
+    case ER_DUP_UNIQUE:
+#endif
+#ifdef ER_NO_REFERENCED_ROW
+    case ER_NO_REFERENCED_ROW:
+#endif
+#ifdef ER_NO_REFERENCED_ROW_2
+    case ER_NO_REFERENCED_ROW_2:
+#endif
+#ifdef ER_ROW_IS_REFERENCED
+    case ER_ROW_IS_REFERENCED:
+#endif
+#ifdef ER_ROW_IS_REFERENCED_2
+    case ER_ROW_IS_REFERENCED_2:
+#endif
+#ifdef ER_CANNOT_ADD_FOREIGN
+    case ER_CANNOT_ADD_FOREIGN:
+#endif
+#ifdef ER_NO_DEFAULT_FOR_FIELD
+    case ER_NO_DEFAULT_FOR_FIELD:
+#endif
+    case ER_BAD_NULL_ERROR:
+        e = _mysql_IntegrityError;
+        break;
+#ifdef ER_WARNING_NOT_COMPLETE_ROLLBACK
+    case ER_WARNING_NOT_COMPLETE_ROLLBACK:
+#endif
+#ifdef ER_NOT_SUPPORTED_YET
+    case ER_NOT_SUPPORTED_YET:
+#endif
+#ifdef ER_FEATURE_DISABLED
+    case ER_FEATURE_DISABLED:
+#endif
+#ifdef ER_UNKNOWN_STORAGE_ENGINE
+    case ER_UNKNOWN_STORAGE_ENGINE:
+#endif
+        e = _mysql_NotSupportedError;
+        break;
+    default:
+        if (merr < 1000)
+            e = _mysql_InternalError;
+        else
+            e = _mysql_OperationalError;
+        break;
+    }
+    PyTuple_SET_ITEM(t, 0, PyLong_FromLong((long)merr));
+    PyTuple_SET_ITEM(t, 1, PyUnicode_FromString(mysql_error(&(c->connection))));
+    PyErr_SetObject(e, t);
+    Py_DECREF(t);
+    return NULL;
+}
+
+static const char *utf8 = "utf8";
+
+static const char*
+_get_encoding(MYSQL *mysql)
+{
+    MY_CHARSET_INFO cs;
+    mysql_get_character_set_info(mysql, &cs);
+    if (strncmp(utf8, cs.csname, 4) == 0) { // utf8, utf8mb3, utf8mb4
+        return utf8;
+    }
+    else if (strncmp("latin1", cs.csname, 6) == 0) {
+        return "cp1252";
+    }
+    else if (strncmp("koi8r", cs.csname, 5) == 0) {
+        return "koi8_r";
+    }
+    else if (strncmp("koi8u", cs.csname, 5) == 0) {
+        return "koi8_u";
+    }
+    return cs.csname;
+}
+
+static char _mysql_ResultObject__doc__[] =
+"result(connection, use=0, converter={}) -- Result set from a query.\n\
+\n\
+Creating instances of this class directly is an excellent way to\n\
+shoot yourself in the foot. If using _mysql.connection directly,\n\
+use connection.store_result() or connection.use_result() instead.\n\
+If using MySQLdb.Connection, this is done by the cursor class.\n\
+Just forget you ever saw this. Forget... FOR-GET...";
+
+static int
+_mysql_ResultObject_Initialize(
+    _mysql_ResultObject *self,
+    PyObject *args,
+    PyObject *kwargs)
+{
+    static char *kwlist[] = {"connection", "use", "converter", NULL};
+    MYSQL_RES *result;
+    _mysql_ConnectionObject *conn=NULL;
+    int use=0;
+    PyObject *conv=NULL;
+    int n, i;
+    MYSQL_FIELD *fields;
+
+    if (!PyArg_ParseTupleAndKeywords(args, kwargs, "O!|iO", kwlist,
+                     &_mysql_ConnectionObject_Type, &conn, &use, &conv))
+        return -1;
+
+    self->conn = (PyObject *) conn;
+    Py_INCREF(conn);
+    self->use = use;
+    Py_BEGIN_ALLOW_THREADS ;
+    if (use)
+        result = mysql_use_result(&(conn->connection));
+    else
+        result = mysql_store_result(&(conn->connection));
+    self->result = result;
+    self->has_next = (char)mysql_more_results(&(conn->connection));
+    Py_END_ALLOW_THREADS ;
+
+    self->encoding = _get_encoding(&(conn->connection));
+    //fprintf(stderr, "encoding=%s\n", self->encoding);
+    if (!result) {
+        if (mysql_errno(&(conn->connection))) {
+            _mysql_Exception(conn);
+            return -1;
+        }
+        self->converter = PyTuple_New(0);
+        return 0;
+    }
+    n = mysql_num_fields(result);
+    self->nfields = n;
+    if (!(self->converter = PyTuple_New(n))) {
+        return -1;
+    }
+    fields = mysql_fetch_fields(result);
+    for (i=0; i<n; i++) {
+        PyObject *tmp, *fun;
+        tmp = PyLong_FromLong((long) fields[i].type);
+        if (!tmp) {
+            return -1;
+        }
+        fun = conv ? PyObject_GetItem(conv, tmp) : NULL;
+        Py_DECREF(tmp);
+        if (!fun) {
+            if (PyErr_Occurred()) {
+                if (!PyErr_ExceptionMatches(PyExc_KeyError)) {
+                    return -1;
+                }
+                PyErr_Clear();
+            }
+            fun = Py_None;
+            Py_INCREF(Py_None);
+        }
+        else if (PySequence_Check(fun)) {
+            long flags = fields[i].flags;
+            PyObject *fun2=NULL;
+            int j, n2=PySequence_Size(fun);
+            // BINARY_FLAG means ***_bin collation is used.
+            // To distinguish text and binary, we should use charsetnr==63 (binary).
+            // But we abuse BINARY_FLAG for historical reason.
+            if (fields[i].charsetnr == 63) {
+                flags |= BINARY_FLAG;
+            } else {
+                flags &= ~BINARY_FLAG;
+            }
+            for (j=0; j<n2; j++) {
+                PyObject *t = PySequence_GetItem(fun, j);
+                if (!t) {
+                    Py_DECREF(fun);
+                    return -1;
+                }
+                if (PyTuple_Check(t) && PyTuple_GET_SIZE(t) == 2) {
+                    long mask;
+                    PyObject *pmask=NULL;
+                    pmask = PyTuple_GET_ITEM(t, 0);
+                    fun2 = PyTuple_GET_ITEM(t, 1);
+                    Py_XINCREF(fun2);
+                    if (PyLong_Check(pmask)) {
+                        mask = PyLong_AS_LONG(pmask);
+                        if (mask & flags) {
+                            Py_DECREF(t);
+                            break;
+                        }
+                        else {
+                            fun2 = NULL;
+                        }
+                    } else {
+                        Py_DECREF(t);
+                        break;
+                    }
+                }
+                Py_DECREF(t);
+            }
+            if (!fun2) {
+                fun2 = Py_None;
+                Py_INCREF(fun2);
+            }
+            Py_DECREF(fun);
+            fun = fun2;
+        }
+        PyTuple_SET_ITEM(self->converter, i, fun);
+    }
+
+    return 0;
+}
+
+static int _mysql_ResultObject_traverse(
+    _mysql_ResultObject *self,
+    visitproc visit,
+    void *arg)
+{
+    int r;
+    if (self->converter) {
+        if (!(r = visit(self->converter, arg))) return r;
+    }
+    if (self->conn)
+        return visit(self->conn, arg);
+    return 0;
+}
+
+static int _mysql_ResultObject_clear(_mysql_ResultObject *self)
+{
+    Py_CLEAR(self->converter);
+    Py_CLEAR(self->conn);
+    return 0;
+}
+
+enum {
+    SSLMODE_DISABLED = 1,
+    SSLMODE_PREFERRED = 2,
+    SSLMODE_REQUIRED = 3,
+    SSLMODE_VERIFY_CA = 4,
+    SSLMODE_VERIFY_IDENTITY = 5
+};
+
+static int
+_get_ssl_mode_num(char *ssl_mode)
+{
+    static char *ssl_mode_list[] = { "DISABLED", "PREFERRED",
+                  "REQUIRED", "VERIFY_CA", "VERIFY_IDENTITY" };
+    unsigned int i;
+    for (i=0; i < sizeof(ssl_mode_list)/sizeof(ssl_mode_list[0]); i++) {
+        if (strcmp(ssl_mode, ssl_mode_list[i]) == 0) {
+            // SSL_MODE one-based
+            return i + 1;
+        }
+    }
+    return -1;
+}
+
+static int
+_mysql_ConnectionObject_Initialize(
+    _mysql_ConnectionObject *self,
+    PyObject *args,
+    PyObject *kwargs)
+{
+    MYSQL *conn = NULL;
+    PyObject *conv = NULL;
+    PyObject *ssl = NULL;
+    char *ssl_mode = NULL;
+    const char *key = NULL, *cert = NULL, *ca = NULL,
+         *capath = NULL, *cipher = NULL;
+    PyObject *ssl_keepref[5] = {NULL};
+    int n_ssl_keepref = 0;
+    char *host = NULL, *user = NULL, *passwd = NULL,
+         *db = NULL, *unix_socket = NULL;
+    unsigned int port = 0;
+    unsigned int client_flag = 0;
+    static char *kwlist[] = { "host", "user", "password", "database", "port",
+                  "unix_socket", "conv",
+                  "connect_timeout", "compress",
+                  "named_pipe", "init_command",
+                  "read_default_file", "read_default_group",
+                  "client_flag", "ssl", "ssl_mode",
+                  "local_infile",
+                  "read_timeout", "write_timeout", "charset",
+                  "auth_plugin",
+                  NULL } ;
+    int connect_timeout = 0;
+    int read_timeout = 0;
+    int write_timeout = 0;
+    int compress = -1, named_pipe = -1, local_infile = -1;
+    int ssl_mode_num = SSLMODE_DISABLED;
+    char *init_command=NULL,
+         *read_default_file=NULL,
+         *read_default_group=NULL,
+         *charset=NULL,
+         *auth_plugin=NULL;
+
+    self->converter = NULL;
+    self->open = 0;
+
+    if (!PyArg_ParseTupleAndKeywords(args, kwargs,
+                "|ssssisOiiisssiOsiiiss:connect",
+                kwlist,
+                &host, &user, &passwd, &db,
+                &port, &unix_socket, &conv,
+                &connect_timeout,
+                &compress, &named_pipe,
+                &init_command, &read_default_file,
+                &read_default_group,
+                &client_flag, &ssl, &ssl_mode,
+                &local_infile,
+                &read_timeout,
+                &write_timeout,
+                &charset,
+                &auth_plugin
+    ))
+        return -1;
+
+#define _stringsuck(d,t,s) {t=PyMapping_GetItemString(s,#d);\
+        if(t){d=PyUnicode_AsUTF8(t);ssl_keepref[n_ssl_keepref++]=t;}\
+        PyErr_Clear();}
+
+    if (ssl) {
+        PyObject *value = NULL;
+        _stringsuck(ca, value, ssl);
+        _stringsuck(capath, value, ssl);
+        _stringsuck(cert, value, ssl);
+        _stringsuck(key, value, ssl);
+        _stringsuck(cipher, value, ssl);
+    }
+    if (ssl_mode) {
+        if ((ssl_mode_num = _get_ssl_mode_num(ssl_mode)) <= 0) {
+            PyErr_SetString(_mysql_NotSupportedError, "Unknown ssl_mode specification");
+            return -1;
+        }
+    }
+
+    conn = mysql_init(&(self->connection));
+    if (!conn) {
+        PyErr_SetNone(PyExc_MemoryError);
+        return -1;
+    }
+    self->open = 1;
+
+    if (connect_timeout) {
+        unsigned int timeout = connect_timeout;
+        mysql_options(&(self->connection), MYSQL_OPT_CONNECT_TIMEOUT,
+                (char *)&timeout);
+    }
+    if (read_timeout) {
+        unsigned int timeout = read_timeout;
+        mysql_options(&(self->connection), MYSQL_OPT_READ_TIMEOUT,
+                (char *)&timeout);
+    }
+    if (write_timeout) {
+        unsigned int timeout = write_timeout;
+        mysql_options(&(self->connection), MYSQL_OPT_WRITE_TIMEOUT,
+                (char *)&timeout);
+    }
+    if (compress != -1) {
+        mysql_options(&(self->connection), MYSQL_OPT_COMPRESS, 0);
+        client_flag |= CLIENT_COMPRESS;
+    }
+    if (named_pipe != -1)
+        mysql_options(&(self->connection), MYSQL_OPT_NAMED_PIPE, 0);
+    if (init_command != NULL)
+        mysql_options(&(self->connection), MYSQL_INIT_COMMAND, init_command);
+    if (read_default_file != NULL)
+        mysql_options(&(self->connection), MYSQL_READ_DEFAULT_FILE, read_default_file);
+    if (read_default_group != NULL)
+        mysql_options(&(self->connection), MYSQL_READ_DEFAULT_GROUP, read_default_group);
+
+    if (local_infile != -1)
+        mysql_options(&(self->connection), MYSQL_OPT_LOCAL_INFILE, (char *) &local_infile);
+
+    if (ssl) {
+        mysql_ssl_set(&(self->connection), key, cert, ca, capath, cipher);
+    }
+    if (ssl_mode) {
+#ifdef HAVE_ENUM_MYSQL_OPT_SSL_MODE
+        mysql_options(&(self->connection), MYSQL_OPT_SSL_MODE, &ssl_mode_num);
+#else
+        // MariaDB doesn't support MYSQL_OPT_SSL_MODE.
+        // See https://github.com/PyMySQL/mysqlclient/issues/474
+        // TODO: Does MariaDB supports PREFERRED and VERIFY_CA?
+        // We support only two levels for now.
+        my_bool enforce_tls = 1;
+        if (ssl_mode_num >= SSLMODE_REQUIRED) {
+            mysql_optionsv(&(self->connection), MYSQL_OPT_SSL_ENFORCE, (void *)&enforce_tls);
+        }
+        if (ssl_mode_num >= SSLMODE_VERIFY_CA) {
+            mysql_optionsv(&(self->connection), MYSQL_OPT_SSL_VERIFY_SERVER_CERT, (void *)&enforce_tls);
+        }
+#endif
+    }
+
+    if (charset) {
+        mysql_options(&(self->connection), MYSQL_SET_CHARSET_NAME, charset);
+    }
+    if (auth_plugin) {
+        mysql_options(&(self->connection), MYSQL_DEFAULT_AUTH, auth_plugin);
+    }
+
+    Py_BEGIN_ALLOW_THREADS
+    conn = mysql_real_connect(&(self->connection), host, user, passwd, db,
+                  port, unix_socket, client_flag);
+    Py_END_ALLOW_THREADS
+
+    if (ssl) {
+        int i;
+        for (i=0; i<n_ssl_keepref; i++) {
+            Py_DECREF(ssl_keepref[i]);
+            ssl_keepref[i] = NULL;
+        }
+    }
+
+    if (!conn) {
+        _mysql_Exception(self);
+        return -1;
+    }
+
+    /* Internal references to python-land objects */
+    if (!conv)
+        conv = PyDict_New();
+    else
+        Py_INCREF(conv);
+
+    if (!conv)
+        return -1;
+    self->converter = conv;
+
+    /*
+      PyType_GenericAlloc() automatically sets up GC allocation and
+      tracking for GC objects, at least in 2.2.1, so it does not need to
+      be done here. tp_dealloc still needs to call PyObject_GC_UnTrack(),
+      however.
+    */
+    return 0;
+}
+
+static char _mysql_connect__doc__[] =
+"Returns a MYSQL connection object. Exclusive use of\n\
+keyword parameters strongly recommended. Consult the\n\
+MySQL C API documentation for more details.\n\
+\n\
+host\n\
+  string, host to connect\n\
+\n\
+user\n\
+  string, user to connect as\n\
+\n\
+password\n\
+  string, password to use\n\
+\n\
+database\n\
+  string, database to use\n\
+\n\
+port\n\
+  integer, TCP/IP port to connect to\n\
+\n\
+unix_socket\n\
+  string, location of unix_socket (UNIX-ish only)\n\
+\n\
+conv\n\
+  mapping, maps MySQL FIELD_TYPE.* to Python functions which\n\
+  convert a string to the appropriate Python type\n\
+\n\
+connect_timeout\n\
+  number of seconds to wait before the connection\n\
+  attempt fails.\n\
+\n\
+compress\n\
+  if set, gzip compression is enabled\n\
+\n\
+named_pipe\n\
+  if set, connect to server via named pipe (Windows only)\n\
+\n\
+init_command\n\
+  command which is run once the connection is created\n\
+\n\
+read_default_file\n\
+  see the MySQL documentation for mysql_options()\n\
+\n\
+read_default_group\n\
+  see the MySQL documentation for mysql_options()\n\
+\n\
+client_flag\n\
+  client flags from MySQLdb.constants.CLIENT\n\
+\n\
+load_infile\n\
+  int, non-zero enables LOAD LOCAL INFILE, zero disables\n\
+\n\
+";
+
+static PyObject *
+_mysql_connect(
+    PyObject *self,
+    PyObject *args,
+    PyObject *kwargs)
+{
+    _mysql_ConnectionObject *c=NULL;
+
+    c = MyAlloc(_mysql_ConnectionObject, _mysql_ConnectionObject_Type);
+    if (c == NULL) return NULL;
+    if (_mysql_ConnectionObject_Initialize(c, args, kwargs)) {
+        Py_DECREF(c);
+        c = NULL;
+    }
+    return (PyObject *) c;
+}
+
+static int _mysql_ConnectionObject_traverse(
+    _mysql_ConnectionObject *self,
+    visitproc visit,
+    void *arg)
+{
+    if (self->converter)
+        return visit(self->converter, arg);
+    return 0;
+}
+
+static int _mysql_ConnectionObject_clear(
+    _mysql_ConnectionObject *self)
+{
+    Py_XDECREF(self->converter);
+    self->converter = NULL;
+    return 0;
+}
+
+static char _mysql_ConnectionObject_close__doc__[] =
+"Close the connection. No further activity possible.";
+
+static PyObject *
+_mysql_ConnectionObject_close(
+    _mysql_ConnectionObject *self,
+    PyObject *noargs)
+{
+    check_connection(self);
+    Py_BEGIN_ALLOW_THREADS
+    mysql_close(&(self->connection));
+    Py_END_ALLOW_THREADS
+    self->open = 0;
+    _mysql_ConnectionObject_clear(self);
+    Py_RETURN_NONE;
+}
+
+static char _mysql_ConnectionObject_affected_rows__doc__ [] =
+"Return number of rows affected by the last query.\n\
+Non-standard. Use Cursor.rowcount.\n\
+";
+
+static PyObject *
+_mysql_ConnectionObject_affected_rows(
+    _mysql_ConnectionObject *self,
+    PyObject *noargs)
+{
+    my_ulonglong ret;
+    check_connection(self);
+    ret = mysql_affected_rows(&(self->connection));
+    if (ret == (my_ulonglong)-1)
+        return PyLong_FromLong(-1);
+    return PyLong_FromUnsignedLongLong(ret);
+}
+
+static char _mysql_debug__doc__[] =
+"Does a DBUG_PUSH with the given string.\n\
+mysql_debug() uses the Fred Fish debug library.\n\
+To use this function, you must compile the client library to\n\
+support debugging.\n\
+";
+static PyObject *
+_mysql_debug(
+    PyObject *self,
+    PyObject *args)
+{
+    char *debug;
+    if (!PyArg_ParseTuple(args, "s", &debug)) return NULL;
+    mysql_debug(debug);
+    Py_RETURN_NONE;
+}
+
+static char _mysql_ConnectionObject_dump_debug_info__doc__[] =
+"Instructs the server to write some debug information to the\n\
+log. The connected user must have the process privilege for\n\
+this to work. Non-standard.\n\
+";
+
+static PyObject *
+_mysql_ConnectionObject_dump_debug_info(
+    _mysql_ConnectionObject *self,
+    PyObject *noargs)
+{
+    int err;
+    check_connection(self);
+    Py_BEGIN_ALLOW_THREADS
+    err = mysql_dump_debug_info(&(self->connection));
+    Py_END_ALLOW_THREADS
+    if (err) return _mysql_Exception(self);
+    Py_RETURN_NONE;
+}
+
+static char _mysql_ConnectionObject_autocommit__doc__[] =
+"Set the autocommit mode. True values enable; False value disable.\n\
+";
+static PyObject *
+_mysql_ConnectionObject_autocommit(
+    _mysql_ConnectionObject *self,
+    PyObject *args)
+{
+    int flag, err;
+    if (!PyArg_ParseTuple(args, "i", &flag)) return NULL;
+    check_connection(self);
+    Py_BEGIN_ALLOW_THREADS
+    err = mysql_autocommit(&(self->connection), flag);
+    Py_END_ALLOW_THREADS
+    if (err) return _mysql_Exception(self);
+    Py_RETURN_NONE;
+}
+
+static char _mysql_ConnectionObject_get_autocommit__doc__[] =
+"Get the autocommit mode. True when enable; False when disable.\n";
+
+static PyObject *
+_mysql_ConnectionObject_get_autocommit(
+    _mysql_ConnectionObject *self,
+    PyObject *args)
+{
+    check_connection(self);
+    if (self->connection.server_status & SERVER_STATUS_AUTOCOMMIT) {
+        Py_RETURN_TRUE;
+    }
+    Py_RETURN_FALSE;
+}
+
+static char _mysql_ConnectionObject_commit__doc__[] =
+"Commits the current transaction\n\
+";
+static PyObject *
+_mysql_ConnectionObject_commit(
+    _mysql_ConnectionObject *self,
+    PyObject *noargs)
+{
+    int err;
+    check_connection(self);
+    Py_BEGIN_ALLOW_THREADS
+    err = mysql_commit(&(self->connection));
+    Py_END_ALLOW_THREADS
+    if (err) return _mysql_Exception(self);
+    Py_RETURN_NONE;
+}
+
+static char _mysql_ConnectionObject_rollback__doc__[] =
+"Rolls back the current transaction\n\
+";
+static PyObject *
+_mysql_ConnectionObject_rollback(
+    _mysql_ConnectionObject *self,
+    PyObject *noargs)
+{
+    int err;
+    check_connection(self);
+    Py_BEGIN_ALLOW_THREADS
+    err = mysql_rollback(&(self->connection));
+    Py_END_ALLOW_THREADS
+    if (err) return _mysql_Exception(self);
+    Py_RETURN_NONE;
+}
+
+static char _mysql_ConnectionObject_next_result__doc__[] =
+"If more query results exist, next_result() reads the next query\n\
+results and returns the status back to application.\n\
+\n\
+After calling next_result() the state of the connection is as if\n\
+you had called query() for the next query. This means that you can\n\
+now call store_result(), warning_count(), affected_rows()\n\
+, and so forth. \n\
+\n\
+Returns 0 if there are more results; -1 if there are no more results\n\
+\n\
+Non-standard.\n\
+";
+static PyObject *
+_mysql_ConnectionObject_next_result(
+    _mysql_ConnectionObject *self,
+    PyObject *noargs)
+{
+    int err;
+    check_connection(self);
+    Py_BEGIN_ALLOW_THREADS
+    err = mysql_next_result(&(self->connection));
+    Py_END_ALLOW_THREADS
+    if (err > 0) return _mysql_Exception(self);
+    return PyLong_FromLong(err);
+}
+
+
+static char _mysql_ConnectionObject_set_server_option__doc__[] =
+"set_server_option(option) -- Enables or disables an option\n\
+for the connection.\n\
+\n\
+Non-standard.\n\
+";
+static PyObject *
+_mysql_ConnectionObject_set_server_option(
+    _mysql_ConnectionObject *self,
+    PyObject *args)
+{
+    int err, flags=0;
+    if (!PyArg_ParseTuple(args, "i", &flags))
+        return NULL;
+    check_connection(self);
+    Py_BEGIN_ALLOW_THREADS
+    err = mysql_set_server_option(&(self->connection), flags);
+    Py_END_ALLOW_THREADS
+    if (err) return _mysql_Exception(self);
+    return PyLong_FromLong(err);
+}
+
+static char _mysql_ConnectionObject_sqlstate__doc__[] =
+"Returns a string containing the SQLSTATE error code\n\
+for the last error. The error code consists of five characters.\n\
+'00000' means \"no error.\" The values are specified by ANSI SQL\n\
+and ODBC. For a list of possible values, see section 23\n\
+Error Handling in MySQL in the MySQL Manual.\n\
+\n\
+Note that not all MySQL errors are yet mapped to SQLSTATE's.\n\
+The value 'HY000' (general error) is used for unmapped errors.\n\
+\n\
+Non-standard.\n\
+";
+static PyObject *
+_mysql_ConnectionObject_sqlstate(
+    _mysql_ConnectionObject *self,
+    PyObject *noargs)
+{
+    check_connection(self);
+    return PyUnicode_FromString(mysql_sqlstate(&(self->connection)));
+}
+
+static char _mysql_ConnectionObject_warning_count__doc__[] =
+"Returns the number of warnings generated during execution\n\
+of the previous SQL statement.\n\
+\n\
+Non-standard.\n\
+";
+static PyObject *
+_mysql_ConnectionObject_warning_count(
+    _mysql_ConnectionObject *self,
+    PyObject *noargs)
+{
+    check_connection(self);
+    return PyLong_FromLong(mysql_warning_count(&(self->connection)));
+}
+
+static char _mysql_ConnectionObject_errno__doc__[] =
+"Returns the error code for the most recently invoked API function\n\
+that can succeed or fail. A return value of zero means that no error\n\
+occurred.\n\
+";
+
+static PyObject *
+_mysql_ConnectionObject_errno(
+    _mysql_ConnectionObject *self,
+    PyObject *noargs)
+{
+    check_connection(self);
+    return PyLong_FromLong((long)mysql_errno(&(self->connection)));
+}
+
+static char _mysql_ConnectionObject_error__doc__[] =
+"Returns the error message for the most recently invoked API function\n\
+that can succeed or fail. An empty string ("") is returned if no error\n\
+occurred.\n\
+";
+
+static PyObject *
+_mysql_ConnectionObject_error(
+    _mysql_ConnectionObject *self,
+    PyObject *noargs)
+{
+    check_connection(self);
+    return PyUnicode_FromString(mysql_error(&(self->connection)));
+}
+
+static char _mysql_escape_string__doc__[] =
+"escape_string(s) -- quote any SQL-interpreted characters in string s.\n\
+\n\
+Use connection.escape_string(s), if you use it at all.\n\
+_mysql.escape_string(s) cannot handle character sets. You are\n\
+probably better off using connection.escape(o) instead, since\n\
+it will escape entire sequences as well as strings.";
+
+static PyObject *
+_mysql_escape_string(
+    _mysql_ConnectionObject *self,
+    PyObject *args)
+{
+    PyObject *str;
+    char *in, *out;
+    unsigned long len;
+    Py_ssize_t size;
+    if (!PyArg_ParseTuple(args, "s#:escape_string", &in, &size)) return NULL;
+    str = PyBytes_FromStringAndSize((char *) NULL, size*2+1);
+    if (!str) return PyErr_NoMemory();
+    out = PyBytes_AS_STRING(str);
+
+    if (self && PyModule_Check((PyObject*)self))
+        self = NULL;
+    if (self && self->open) {
+#if MYSQL_VERSION_ID >= 50707 && !defined(MARIADB_BASE_VERSION) && !defined(MARIADB_VERSION_ID)
+        len = mysql_real_escape_string_quote(&(self->connection), out, in, size, '\'');
+#else
+        len = mysql_real_escape_string(&(self->connection), out, in, size);
+#endif
+    } else {
+        len = mysql_escape_string(out, in, size);
+    }
+    if (_PyBytes_Resize(&str, len) < 0) return NULL;
+    return (str);
+}
+
+static char _mysql_string_literal__doc__[] =
+"string_literal(obj) -- converts object obj into a SQL string literal.\n\
+This means, any special SQL characters are escaped, and it is enclosed\n\
+within single quotes. In other words, it performs:\n\
+\n\
+\"'%s'\" % escape_string(str(obj))\n\
+\n\
+Use connection.string_literal(obj), if you use it at all.\n\
+_mysql.string_literal(obj) cannot handle character sets.";
+
+static PyObject *
+_mysql_string_literal(
+    _mysql_ConnectionObject *self,
+    PyObject *o)
+{
+    PyObject *s; // input string or bytes. need to decref.
+
+    if (self && PyModule_Check((PyObject*)self))
+        self = NULL;
+
+    if (PyBytes_Check(o)) {
+        s = o;
+        Py_INCREF(s);
+    }
+    else {
+        PyObject *t = PyObject_Str(o);
+        if (!t) return NULL;
+
+        const char *encoding = (self && self->open) ?
+            _get_encoding(&self->connection) : utf8;
+        if (encoding == utf8) {
+            s = t;
+        }
+        else {
+            s = PyUnicode_AsEncodedString(t, encoding, "strict");
+            Py_DECREF(t);
+            if (!s) return NULL;
+        }
+    }
+
+    // Prepare input string (in, size)
+    const char *in;
+    Py_ssize_t size;
+    if (PyUnicode_Check(s)) {
+        in = PyUnicode_AsUTF8AndSize(s, &size);
+    } else {
+        assert(PyBytes_Check(s));
+        in = PyBytes_AsString(s);
+        size = PyBytes_GET_SIZE(s);
+    }
+
+    // Prepare output buffer (str, out)
+    PyObject *str = PyBytes_FromStringAndSize((char *) NULL, size*2+3);
+    if (!str) {
+        Py_DECREF(s);
+        return PyErr_NoMemory();
+    }
+    char *out = PyBytes_AS_STRING(str);
+
+    // escape
+    unsigned long len;
+    if (self && self->open) {
+#if MYSQL_VERSION_ID >= 50707 && !defined(MARIADB_BASE_VERSION) && !defined(MARIADB_VERSION_ID)
+        len = mysql_real_escape_string_quote(&(self->connection), out+1, in, size, '\'');
+#else
+        len = mysql_real_escape_string(&(self->connection), out+1, in, size);
+#endif
+    } else {
+        len = mysql_escape_string(out+1, in, size);
+    }
+
+    Py_DECREF(s);
+    *out = *(out+len+1) = '\'';
+    if (_PyBytes_Resize(&str, len+2) < 0) {
+        Py_DECREF(str);
+        return NULL;
+    }
+    return str;
+}
+
+static PyObject *
+_escape_item(
+    PyObject *self,
+    PyObject *item,
+    PyObject *d)
+{
+    PyObject *quoted=NULL, *itemtype, *itemconv;
+    if (!(itemtype = PyObject_Type(item))) {
+        return NULL;
+    }
+    itemconv = PyObject_GetItem(d, itemtype);
+    Py_DECREF(itemtype);
+    if (!itemconv) {
+        PyErr_Clear();
+        return _mysql_string_literal((_mysql_ConnectionObject*)self, item);
+    }
+    Py_INCREF(d);
+    quoted = PyObject_CallFunction(itemconv, "OO", item, d);
+    Py_DECREF(d);
+    Py_DECREF(itemconv);
+
+    return quoted;
+}
+
+static char _mysql_escape__doc__[] =
+"escape(obj, dict) -- escape any special characters in object obj\n\
+using mapping dict to provide quoting functions for each type.\n\
+Returns a SQL literal string.";
+static PyObject *
+_mysql_escape(
+    PyObject *self,
+    PyObject *args)
+{
+    PyObject *o=NULL, *d=NULL;
+    if (!PyArg_ParseTuple(args, "O|O:escape", &o, &d))
+        return NULL;
+    if (d) {
+        if (!PyMapping_Check(d)) {
+            PyErr_SetString(PyExc_TypeError,
+                    "argument 2 must be a mapping");
+            return NULL;
+        }
+        return _escape_item(self, o, d);
+    } else {
+        if (!self) {
+            PyErr_SetString(PyExc_TypeError,
+                    "argument 2 must be a mapping");
+            return NULL;
+        }
+        return _escape_item(self, o,
+               ((_mysql_ConnectionObject *) self)->converter);
+    }
+}
+
+static char _mysql_ResultObject_describe__doc__[] =
+"Returns the sequence of 7-tuples required by the DB-API for\n\
+the Cursor.description attribute.\n\
+";
+
+static PyObject *
+_mysql_ResultObject_describe(
+    _mysql_ResultObject *self,
+    PyObject *noargs)
+{
+    PyObject *d;
+    MYSQL_FIELD *fields;
+    unsigned int i, n;
+
+    check_result_connection(self);
+
+    n = mysql_num_fields(self->result);
+    fields = mysql_fetch_fields(self->result);
+    if (!(d = PyTuple_New(n))) return NULL;
+    for (i=0; i<n; i++) {
+        PyObject *t;
+        PyObject *name;
+        if (self->encoding == utf8) {
+            name = PyUnicode_DecodeUTF8(fields[i].name, fields[i].name_length, "replace");
+        } else {
+            name = PyUnicode_Decode(fields[i].name, fields[i].name_length, self->encoding, "replace");
+        }
+        if (name == NULL) {
+            goto error;
+        }
+
+        t = Py_BuildValue("(Niiiiii)",
+                  name,
+                  (long) fields[i].type,
+                  (long) fields[i].max_length,
+                  (long) fields[i].length,
+                  (long) fields[i].length,
+                  (long) fields[i].decimals,
+                  (long) !(IS_NOT_NULL(fields[i].flags)));
+        if (!t) goto error;
+        PyTuple_SET_ITEM(d, i, t);
+    }
+    return d;
+  error:
+    Py_XDECREF(d);
+    return NULL;
+}
+
+static char _mysql_ResultObject_field_flags__doc__[] =
+"Returns a tuple of field flags, one for each column in the result.\n\
+" ;
+
+static PyObject *
+_mysql_ResultObject_field_flags(
+    _mysql_ResultObject *self,
+    PyObject *noargs)
+{
+    PyObject *d;
+    MYSQL_FIELD *fields;
+    unsigned int i, n;
+    check_result_connection(self);
+    n = mysql_num_fields(self->result);
+    fields = mysql_fetch_fields(self->result);
+    if (!(d = PyTuple_New(n))) return NULL;
+    for (i=0; i<n; i++) {
+        PyObject *f;
+        if (!(f = PyLong_FromLong((long)fields[i].flags))) goto error;
+        PyTuple_SET_ITEM(d, i, f);
+    }
+    return d;
+  error:
+    Py_XDECREF(d);
+    return NULL;
+}
+
+static PyObject *
+_mysql_field_to_python(
+    PyObject *converter,
+    const char *rowitem,
+    Py_ssize_t length,
+    MYSQL_FIELD *field,
+    const char *encoding)
+{
+    if (rowitem == NULL) {
+        Py_RETURN_NONE;
+    }
+
+    // Fast paths for int, string and binary.
+    if (converter == (PyObject*)&PyUnicode_Type) {
+        if (encoding == utf8) {
+            //fprintf(stderr, "decoding with utf8!\n");
+            return PyUnicode_DecodeUTF8(rowitem, length, NULL);
+        } else {
+            //fprintf(stderr, "decoding with %s\n", encoding);
+            return PyUnicode_Decode(rowitem, length, encoding, NULL);
+        }
+    }
+    if (converter == (PyObject*)&PyBytes_Type || converter == Py_None) {
+        //fprintf(stderr, "decoding with bytes\n", encoding);
+        return PyBytes_FromStringAndSize(rowitem, length);
+    }
+    if (converter == (PyObject*)&PyLong_Type) {
+        //fprintf(stderr, "decoding with int\n", encoding);
+        return PyLong_FromString(rowitem, NULL, 10);
+    }
+
+    //fprintf(stderr, "decoding with callback\n");
+    //PyObject_Print(converter, stderr, 0);
+    //fprintf(stderr, "\n");
+    int binary;
+    switch (field->type) {
+    case FIELD_TYPE_DECIMAL:
+    case FIELD_TYPE_NEWDECIMAL:
+    case FIELD_TYPE_TIMESTAMP:
+    case FIELD_TYPE_DATETIME:
+    case FIELD_TYPE_TIME:
+    case FIELD_TYPE_DATE:
+        binary = 0;  // pass str, because these converters expect it
+        break;
+    default: // Default to just passing bytes
+        binary = 1;
+    }
+    return PyObject_CallFunction(converter,
+            binary ? "y#" : "s#",
+            rowitem, (Py_ssize_t)length);
+}
+
+static PyObject *
+_mysql_row_to_tuple(
+    _mysql_ResultObject *self,
+    MYSQL_ROW row,
+    PyObject *unused)
+{
+    unsigned int n, i;
+    unsigned long *length;
+    PyObject *r, *c;
+    MYSQL_FIELD *fields;
+
+    n = mysql_num_fields(self->result);
+    if (!(r = PyTuple_New(n))) return NULL;
+    length = mysql_fetch_lengths(self->result);
+    fields = mysql_fetch_fields(self->result);
+    for (i=0; i<n; i++) {
+        PyObject *v;
+        c = PyTuple_GET_ITEM(self->converter, i);
+        v = _mysql_field_to_python(c, row[i], length[i], &fields[i], self->encoding);
+        if (!v) goto error;
+        PyTuple_SET_ITEM(r, i, v);
+    }
+    return r;
+  error:
+    Py_XDECREF(r);
+    return NULL;
+}
+
+static PyObject *
+_mysql_row_to_dict(
+    _mysql_ResultObject *self,
+    MYSQL_ROW row,
+    PyObject *cache)
+{
+    unsigned int n, i;
+    unsigned long *length;
+    PyObject *r, *c;
+    MYSQL_FIELD *fields;
+
+    n = mysql_num_fields(self->result);
+    if (!(r = PyDict_New())) return NULL;
+    length = mysql_fetch_lengths(self->result);
+    fields = mysql_fetch_fields(self->result);
+    for (i=0; i<n; i++) {
+        PyObject *v;
+        c = PyTuple_GET_ITEM(self->converter, i);
+        v = _mysql_field_to_python(c, row[i], length[i], &fields[i], self->encoding);
+        if (!v) goto error;
+
+        PyObject *pyname = PyUnicode_FromString(fields[i].name);
+        if (pyname == NULL) {
+            Py_DECREF(v);
+            goto error;
+        }
+        int err = PyDict_Contains(r, pyname);
+        if (err < 0) { // error
+            Py_DECREF(v);
+            goto error;
+        }
+        if (err) { // duplicate
+            Py_DECREF(pyname);
+            pyname = PyUnicode_FromFormat("%s.%s", fields[i].table, fields[i].name);
+            if (pyname == NULL) {
+                Py_DECREF(v);
+                goto error;
+            }
+        }
+
+        err = PyDict_SetItem(r, pyname, v);
+        if (cache) {
+            PyTuple_SET_ITEM(cache, i, pyname);
+        } else {
+            Py_DECREF(pyname);
+        }
+        Py_DECREF(v);
+        if (err) {
+            goto error;
+        }
+    }
+    return r;
+error:
+    Py_DECREF(r);
+    return NULL;
+}
+
+static PyObject *
+_mysql_row_to_dict_old(
+    _mysql_ResultObject *self,
+    MYSQL_ROW row,
+    PyObject *cache)
+{
+    unsigned int n, i;
+    unsigned long *length;
+    PyObject *r, *c;
+    MYSQL_FIELD *fields;
+
+    n = mysql_num_fields(self->result);
+    if (!(r = PyDict_New())) return NULL;
+    length = mysql_fetch_lengths(self->result);
+    fields = mysql_fetch_fields(self->result);
+    for (i=0; i<n; i++) {
+        PyObject *v;
+        c = PyTuple_GET_ITEM(self->converter, i);
+        v = _mysql_field_to_python(c, row[i], length[i], &fields[i], self->encoding);
+        if (!v) {
+            goto error;
+        }
+
+        PyObject *pyname;
+        if (strlen(fields[i].table)) {
+            pyname = PyUnicode_FromFormat("%s.%s", fields[i].table, fields[i].name);
+        } else {
+            pyname = PyUnicode_FromString(fields[i].name);
+        }
+        int err = PyDict_SetItem(r, pyname, v);
+        Py_DECREF(v);
+        if (cache) {
+            PyTuple_SET_ITEM(cache, i, pyname);
+        } else {
+            Py_DECREF(pyname);
+        }
+        if (err) {
+            goto error;
+        }
+    }
+    return r;
+  error:
+    Py_XDECREF(r);
+    return NULL;
+}
+
+static PyObject *
+_mysql_row_to_dict_cached(
+    _mysql_ResultObject *self,
+    MYSQL_ROW row,
+    PyObject *cache)
+{
+    PyObject *r = PyDict_New();
+    if (!r) {
+        return NULL;
+    }
+
+    unsigned int n = mysql_num_fields(self->result);
+    unsigned long *length = mysql_fetch_lengths(self->result);
+    MYSQL_FIELD *fields = mysql_fetch_fields(self->result);
+
+    for (unsigned int i=0; i<n; i++) {
+        PyObject *c = PyTuple_GET_ITEM(self->converter, i);
+        PyObject *v = _mysql_field_to_python(c, row[i], length[i], &fields[i], self->encoding);
+        if (!v) {
+            goto error;
+        }
+
+        PyObject *pyname = PyTuple_GET_ITEM(cache, i); // borrowed
+        int err = PyDict_SetItem(r, pyname, v);
+        Py_DECREF(v);
+        if (err) {
+            goto error;
+        }
+    }
+    return r;
+  error:
+    Py_XDECREF(r);
+    return NULL;
+}
+
+
+typedef PyObject *_convertfunc(_mysql_ResultObject *, MYSQL_ROW, PyObject *);
+static _convertfunc * const row_converters[] = {
+    _mysql_row_to_tuple,
+    _mysql_row_to_dict,
+    _mysql_row_to_dict_old
+};
+
+Py_ssize_t
+_mysql__fetch_row(
+    _mysql_ResultObject *self,
+    PyObject *r, /* list object */
+    Py_ssize_t maxrows,
+    int how)
+{
+    _convertfunc *convert_row = row_converters[how];
+
+    PyObject *cache = NULL;
+    if (maxrows > 0 && how > 0) {
+        cache = PyTuple_New(mysql_num_fields(self->result));
+        if (!cache) {
+            return -1;
+        }
+    }
+
+    Py_ssize_t i;
+    for (i = 0; i < maxrows; i++) {
+        MYSQL_ROW row;
+        if (!self->use)
+            row = mysql_fetch_row(self->result);
+        else {
+            Py_BEGIN_ALLOW_THREADS
+            row = mysql_fetch_row(self->result);
+            Py_END_ALLOW_THREADS
+        }
+        if (!row && mysql_errno(&(((_mysql_ConnectionObject *)(self->conn))->connection))) {
+            _mysql_Exception((_mysql_ConnectionObject *)self->conn);
+            goto error;
+        }
+        if (!row) {
+            break;
+        }
+        PyObject *v = convert_row(self, row, cache);
+        if (!v) {
+            goto error;
+        }
+        if (cache) {
+            convert_row = _mysql_row_to_dict_cached;
+        }
+        if (PyList_Append(r, v)) {
+            Py_DECREF(v);
+            goto error;
+        }
+        Py_DECREF(v);
+    }
+    Py_XDECREF(cache);
+    return i;
+error:
+    Py_XDECREF(cache);
+    return -1;
+}
+
+static char _mysql_ResultObject_fetch_row__doc__[] =
+"fetch_row([maxrows, how]) -- Fetches up to maxrows as a tuple.\n\
+The rows are formatted according to how:\n\
+\n\
+    0 -- tuples (default)\n\
+    1 -- dictionaries, key=column or table.column if duplicated\n\
+    2 -- dictionaries, key=table.column\n\
+";
+
+static PyObject *
+_mysql_ResultObject_fetch_row(
+    _mysql_ResultObject *self,
+    PyObject *args,
+    PyObject *kwargs)
+{
+    static char *kwlist[] = {"maxrows", "how", NULL };
+    int maxrows=1, how=0;
+    PyObject *r=NULL;
+
+    if (!PyArg_ParseTupleAndKeywords(args, kwargs, "|ii:fetch_row", kwlist,
+                     &maxrows, &how))
+        return NULL;
+    check_result_connection(self);
+    if (how >= (int)(sizeof(row_converters) / sizeof(row_converters[0]))) {
+        PyErr_SetString(PyExc_ValueError, "how out of range");
+        return NULL;
+    }
+    if (!maxrows) {
+        if (self->use) {
+            maxrows = INT_MAX;
+        } else {
+            // todo: preallocate.
+            maxrows = (Py_ssize_t) mysql_num_rows(self->result);
+        }
+    }
+    if (!(r = PyList_New(0))) goto error;
+    Py_ssize_t rowsadded = _mysql__fetch_row(self, r, maxrows, how);
+    if (rowsadded == -1) goto error;
+
+    /* DB-API allows return rows as list.
+     * But we need to return list because Django expecting tuple.
+     */
+    PyObject *t = PyList_AsTuple(r);
+    Py_DECREF(r);
+    return t;
+  error:
+    Py_XDECREF(r);
+    return NULL;
+}
+
+static const char _mysql_ResultObject_discard__doc__[] =
+"discard() -- Discard remaining rows in the resultset.";
+
+static PyObject *
+_mysql_ResultObject_discard(
+    _mysql_ResultObject *self,
+    PyObject *noargs)
+{
+    check_result_connection(self);
+
+    MYSQL_ROW row;
+    Py_BEGIN_ALLOW_THREADS
+    while (NULL != (row = mysql_fetch_row(self->result))) {
+        // do nothing
+    }
+    Py_END_ALLOW_THREADS
+    _mysql_ConnectionObject *conn = (_mysql_ConnectionObject *)self->conn;
+    if (mysql_errno(&conn->connection)) {
+        return _mysql_Exception(conn);
+    }
+    Py_RETURN_NONE;
+}
+
+static char _mysql_ConnectionObject_change_user__doc__[] =
+"Changes the user and causes the database specified by db to\n\
+become the default (current) database on the connection\n\
+specified by mysql. In subsequent queries, this database is\n\
+the default for table references that do not include an\n\
+explicit database specifier.\n\
+\n\
+This function was introduced in MySQL Version 3.23.3.\n\
+\n\
+Fails unless the connected user can be authenticated or if he\n\
+doesn't have permission to use the database. In this case the\n\
+user and database are not changed.\n\
+\n\
+The db parameter may be set to None if you don't want to have\n\
+a default database.\n\
+";
+
+static PyObject *
+_mysql_ConnectionObject_change_user(
+    _mysql_ConnectionObject *self,
+    PyObject *args,
+    PyObject *kwargs)
+{
+    char *user, *pwd=NULL, *db=NULL;
+    int r;
+    static char *kwlist[] = { "user", "passwd", "db", NULL } ;
+
+    if (!PyArg_ParseTupleAndKeywords(args, kwargs, "s|ss:change_user",
+                     kwlist, &user, &pwd, &db))
+        return NULL;
+    check_connection(self);
+    Py_BEGIN_ALLOW_THREADS
+        r = mysql_change_user(&(self->connection), user, pwd, db);
+    Py_END_ALLOW_THREADS
+    if (r)     return _mysql_Exception(self);
+    Py_RETURN_NONE;
+}
+
+static char _mysql_ConnectionObject_character_set_name__doc__[] =
+"Returns the default character set for the current connection.\n\
+Non-standard.\n\
+";
+
+static PyObject *
+_mysql_ConnectionObject_character_set_name(
+    _mysql_ConnectionObject *self,
+    PyObject *noargs)
+{
+    const char *s;
+    check_connection(self);
+    s = mysql_character_set_name(&(self->connection));
+    return PyUnicode_FromString(s);
+}
+
+static char _mysql_ConnectionObject_set_character_set__doc__[] =
+"Sets the default character set for the current connection.\n\
+Non-standard.\n\
+";
+
+static PyObject *
+_mysql_ConnectionObject_set_character_set(
+    _mysql_ConnectionObject *self,
+    PyObject *args)
+{
+    const char *s;
+    int err;
+    if (!PyArg_ParseTuple(args, "s", &s)) return NULL;
+    check_connection(self);
+    Py_BEGIN_ALLOW_THREADS
+    err = mysql_set_character_set(&(self->connection), s);
+    Py_END_ALLOW_THREADS
+    if (err) return _mysql_Exception(self);
+    Py_RETURN_NONE;
+}
+
+#if MYSQL_VERSION_ID >= 50010
+static char _mysql_ConnectionObject_get_character_set_info__doc__[] =
+"Returns a dict with information about the current character set:\n\
+\n\
+collation\n\
+    collation name\n\
+name\n\
+    character set name\n\
+comment\n\
+    comment or descriptive name\n\
+dir\n\
+    character set directory\n\
+mbminlen\n\
+    min. length for multibyte string\n\
+mbmaxlen\n\
+    max. length for multibyte string\n\
+\n\
+Not all keys may be present, particularly dir.\n\
+\n\
+Non-standard.\n\
+";
+
+static PyObject *
+_mysql_ConnectionObject_get_character_set_info(
+    _mysql_ConnectionObject *self,
+    PyObject *noargs)
+{
+    PyObject *result;
+    MY_CHARSET_INFO cs;
+
+    check_connection(self);
+    mysql_get_character_set_info(&(self->connection), &cs);
+    if (!(result = PyDict_New())) return NULL;
+    if (cs.csname)
+        PyDict_SetItemString(result, "name", PyUnicode_FromString(cs.csname));
+    if (cs.name)
+        PyDict_SetItemString(result, "collation", PyUnicode_FromString(cs.name));
+    if (cs.comment)
+        PyDict_SetItemString(result, "comment", PyUnicode_FromString(cs.comment));
+    if (cs.dir)
+        PyDict_SetItemString(result, "dir", PyUnicode_FromString(cs.dir));
+    PyDict_SetItemString(result, "mbminlen", PyLong_FromLong(cs.mbminlen));
+    PyDict_SetItemString(result, "mbmaxlen", PyLong_FromLong(cs.mbmaxlen));
+    return result;
+}
+#endif
+
+static char _mysql_ConnectionObject_get_native_connection__doc__[] =
+"Return the internal MYSQL* wrapped in a PyCapsule object.\n\
+NOTE: this is a private API introduced ONLY for XTA integration,\n\
+      don't use it for different use cases.\n\
+      This method is supported only for XTA integration and support must\n\
+      be asked to LIXA project: http://www.tiian.org/lixa/\n\
+      Please DO NOT ask support to PyMySQL/mysqlclient-python project.\n\
+";
+
+static PyObject *
+_mysql_ConnectionObject_get_native_connection(
+    _mysql_ConnectionObject *self,
+    PyObject *noargs)
+{
+    PyObject *result;
+    check_connection(self);
+    result = PyCapsule_New(&(self->connection),
+        "_mysql.connection.native_connection", NULL);
+    return result;
+}
+
+
+static char _mysql_get_client_info__doc__[] =
+"get_client_info() -- Returns a string that represents\n\
+the client library version.";
+static PyObject *
+_mysql_get_client_info(
+    PyObject *self,
+    PyObject *noargs)
+{
+    return PyUnicode_FromString(mysql_get_client_info());
+}
+
+static char _mysql_ConnectionObject_get_host_info__doc__[] =
+"Returns a string that represents the MySQL client library\n\
+version. Non-standard.\n\
+";
+
+static PyObject *
+_mysql_ConnectionObject_get_host_info(
+    _mysql_ConnectionObject *self,
+    PyObject *noargs)
+{
+    check_connection(self);
+    return PyUnicode_FromString(mysql_get_host_info(&(self->connection)));
+}
+
+static char _mysql_ConnectionObject_get_proto_info__doc__[] =
+"Returns an unsigned integer representing the protocol version\n\
+used by the current connection. Non-standard.\n\
+";
+
+static PyObject *
+_mysql_ConnectionObject_get_proto_info(
+    _mysql_ConnectionObject *self,
+    PyObject *noargs)
+{
+    check_connection(self);
+    return PyLong_FromLong((long)mysql_get_proto_info(&(self->connection)));
+}
+
+static char _mysql_ConnectionObject_get_server_info__doc__[] =
+"Returns a string that represents the server version number.\n\
+Non-standard.\n\
+";
+
+static PyObject *
+_mysql_ConnectionObject_get_server_info(
+    _mysql_ConnectionObject *self,
+    PyObject *noargs)
+{
+    check_connection(self);
+    return PyUnicode_FromString(mysql_get_server_info(&(self->connection)));
+}
+
+static char _mysql_ConnectionObject_info__doc__[] =
+"Retrieves a string providing information about the most\n\
+recently executed query. Non-standard. Use messages or\n\
+Cursor.messages.\n\
+";
+
+static PyObject *
+_mysql_ConnectionObject_info(
+    _mysql_ConnectionObject *self,
+    PyObject *noargs)
+{
+    const char *s;
+    check_connection(self);
+    s = mysql_info(&(self->connection));
+    if (s) return PyUnicode_FromString(s);
+    Py_RETURN_NONE;
+}
+
+static char _mysql_ConnectionObject_insert_id__doc__[] =
+"Returns the ID generated for an AUTO_INCREMENT column by the previous\n\
+query. Use this function after you have performed an INSERT query into a\n\
+table that contains an AUTO_INCREMENT field.\n\
+\n\
+Note that this returns 0 if the previous query does not\n\
+generate an AUTO_INCREMENT value. If you need to save the value for\n\
+later, be sure to call this immediately after the query\n\
+that generates the value.\n\
+\n\
+The ID is updated after INSERT and UPDATE statements that generate\n\
+an AUTO_INCREMENT value or that set a column value to\n\
+LAST_INSERT_ID(expr). See section 6.3.5.2 Miscellaneous Functions\n\
+in the MySQL documentation.\n\
+\n\
+Also note that the value of the SQL LAST_INSERT_ID() function always\n\
+contains the most recently generated AUTO_INCREMENT value, and is not\n\
+reset between queries because the value of that function is maintained\n\
+in the server.\n\
+" ;
+
+static PyObject *
+_mysql_ConnectionObject_insert_id(
+    _mysql_ConnectionObject *self,
+    PyObject *noargs)
+{
+    my_ulonglong r;
+    check_connection(self);
+    r = mysql_insert_id(&(self->connection));
+    return PyLong_FromUnsignedLongLong(r);
+}
+
+static char _mysql_ConnectionObject_kill__doc__[] =
+"Asks the server to kill the thread specified by pid.\n\
+Non-standard.";
+
+static PyObject *
+_mysql_ConnectionObject_kill(
+    _mysql_ConnectionObject *self,
+    PyObject *args)
+{
+    unsigned long pid;
+    int r;
+    if (!PyArg_ParseTuple(args, "k:kill", &pid)) return NULL;
+    check_connection(self);
+    Py_BEGIN_ALLOW_THREADS
+    r = mysql_kill(&(self->connection), pid);
+    Py_END_ALLOW_THREADS
+    if (r) return _mysql_Exception(self);
+    Py_RETURN_NONE;
+}
+
+static char _mysql_ConnectionObject_field_count__doc__[] =
+"Returns the number of columns for the most recent query on the\n\
+connection. Non-standard. Will probably give you bogus results\n\
+on most cursor classes. Use Cursor.rowcount.\n\
+";
+
+static PyObject *
+_mysql_ConnectionObject_field_count(
+    _mysql_ConnectionObject *self,
+    PyObject *noargs)
+{
+    check_connection(self);
+    return PyLong_FromLong((long)mysql_field_count(&(self->connection)));
+}
+
+static char _mysql_ConnectionObject_fileno__doc__[] =
+"Return file descriptor of the underlying libmysqlclient connection.\n\
+This provides raw access to the underlying network connection.\n\
+";
+
+static PyObject *
+_mysql_ConnectionObject_fileno(
+    _mysql_ConnectionObject *self,
+    PyObject *noargs)
+{
+    check_connection(self);
+    return PyLong_FromLong(self->connection.net.fd);
+}
+
+static char _mysql_ResultObject_num_fields__doc__[] =
+"Returns the number of fields (column) in the result." ;
+
+static PyObject *
+_mysql_ResultObject_num_fields(
+    _mysql_ResultObject *self,
+    PyObject *noargs)
+{
+    check_result_connection(self);
+    return PyLong_FromLong((long)mysql_num_fields(self->result));
+}
+
+static char _mysql_ResultObject_num_rows__doc__[] =
+"Returns the number of rows in the result set. Note that if\n\
+use=1, this will not return a valid value until the entire result\n\
+set has been read.\n\
+";
+
+static PyObject *
+_mysql_ResultObject_num_rows(
+    _mysql_ResultObject *self,
+    PyObject *noargs)
+{
+    check_result_connection(self);
+    return PyLong_FromUnsignedLongLong(mysql_num_rows(self->result));
+}
+
+static char _mysql_ConnectionObject_ping__doc__[] =
+"Checks whether or not the connection to the server is\n\
+working. If it has gone down, an automatic reconnection is\n\
+attempted.\n\
+\n\
+This function can be used by clients that remain idle for a\n\
+long while, to check whether or not the server has closed the\n\
+connection and reconnect if necessary.\n\
+\n\
+New in 1.2.2: Accepts an optional reconnect parameter. If True,\n\
+then the client will attempt reconnection. Note that this setting\n\
+is persistent. By default, this is on in MySQL<5.0.3, and off\n\
+thereafter.\n\
+\n\
+Non-standard. You should assume that ping() performs an\n\
+implicit rollback; use only when starting a new transaction.\n\
+You have been warned.\n\
+";
+
+static PyObject *
+_mysql_ConnectionObject_ping(
+    _mysql_ConnectionObject *self,
+    PyObject *args)
+{
+    int r, reconnect = -1;
+    if (!PyArg_ParseTuple(args, "|I", &reconnect)) return NULL;
+    check_connection(self);
+    if (reconnect != -1) {
+        my_bool recon = (my_bool)reconnect;
+        mysql_options(&self->connection, MYSQL_OPT_RECONNECT, &recon);
+    }
+    Py_BEGIN_ALLOW_THREADS
+    r = mysql_ping(&(self->connection));
+    Py_END_ALLOW_THREADS
+    if (r)     return _mysql_Exception(self);
+    Py_RETURN_NONE;
+}
+
+static char _mysql_ConnectionObject_query__doc__[] =
+"Execute a query. store_result() or use_result() will get the\n\
+result set, if any. Non-standard. Use cursor() to create a cursor,\n\
+then cursor.execute().\n\
+" ;
+
+static PyObject *
+_mysql_ConnectionObject_query(
+    _mysql_ConnectionObject *self,
+    PyObject *args)
+{
+    char *query;
+    Py_ssize_t len;
+    int r;
+    if (!PyArg_ParseTuple(args, "s#:query", &query, &len)) return NULL;
+    check_connection(self);
+
+    Py_BEGIN_ALLOW_THREADS
+    r = mysql_real_query(&(self->connection), query, len);
+    Py_END_ALLOW_THREADS
+    if (r) return _mysql_Exception(self);
+    Py_RETURN_NONE;
+}
+
+
+static char _mysql_ConnectionObject_send_query__doc__[] =
+"Send a query. Same to query() except not wait response.\n\n\
+Use read_query_result() before calling store_result() or use_result()\n";
+
+static PyObject *
+_mysql_ConnectionObject_send_query(
+    _mysql_ConnectionObject *self,
+    PyObject *args)
+{
+    char *query;
+    Py_ssize_t len;
+    int r;
+    MYSQL *mysql = &(self->connection);
+    if (!PyArg_ParseTuple(args, "s#:query", &query, &len)) return NULL;
+    check_connection(self);
+
+    Py_BEGIN_ALLOW_THREADS
+    r = mysql_send_query(mysql, query, len);
+    Py_END_ALLOW_THREADS
+    if (r) return _mysql_Exception(self);
+    Py_RETURN_NONE;
+}
+
+
+static char _mysql_ConnectionObject_read_query_result__doc__[] =
+"Read result of query sent by send_query().\n";
+
+static PyObject *
+_mysql_ConnectionObject_read_query_result(
+    _mysql_ConnectionObject *self,
+    PyObject *noargs)
+{
+    int r;
+    MYSQL *mysql = &(self->connection);
+    check_connection(self);
+
+    Py_BEGIN_ALLOW_THREADS
+    r = (int)mysql_read_query_result(mysql);
+    Py_END_ALLOW_THREADS
+    if (r) return _mysql_Exception(self);
+    Py_RETURN_NONE;
+}
+
+static char _mysql_ConnectionObject_select_db__doc__[] =
+"Causes the database specified by db to become the default\n\
+(current) database on the connection specified by mysql. In subsequent\n\
+queries, this database is the default for table references that do not\n\
+include an explicit database specifier.\n\
+\n\
+Fails unless the connected user can be authenticated as having\n\
+permission to use the database.\n\
+\n\
+Non-standard.\n\
+";
+
+static PyObject *
+_mysql_ConnectionObject_select_db(
+    _mysql_ConnectionObject *self,
+    PyObject *args)
+{
+    char *db;
+    int r;
+    if (!PyArg_ParseTuple(args, "s:select_db", &db)) return NULL;
+    check_connection(self);
+    Py_BEGIN_ALLOW_THREADS
+    r = mysql_select_db(&(self->connection), db);
+    Py_END_ALLOW_THREADS
+    if (r)     return _mysql_Exception(self);
+    Py_RETURN_NONE;
+}
+
+static char _mysql_ConnectionObject_shutdown__doc__[] =
+"Asks the database server to shut down. The connected user must\n\
+have shutdown privileges. Non-standard.\n\
+";
+
+static PyObject *
+_mysql_ConnectionObject_shutdown(
+    _mysql_ConnectionObject *self,
+    PyObject *noargs)
+{
+    int r;
+    check_connection(self);
+    Py_BEGIN_ALLOW_THREADS
+    r = mysql_shutdown(&(self->connection), SHUTDOWN_DEFAULT);
+    Py_END_ALLOW_THREADS
+    if (r) return _mysql_Exception(self);
+    Py_RETURN_NONE;
+}
+
+static char _mysql_ConnectionObject_stat__doc__[] =
+"Returns a character string containing information similar to\n\
+that provided by the mysqladmin status command. This includes\n\
+uptime in seconds and the number of running threads,\n\
+questions, reloads, and open tables. Non-standard.\n\
+";
+
+static PyObject *
+_mysql_ConnectionObject_stat(
+    _mysql_ConnectionObject *self,
+    PyObject *noargs)
+{
+    const char *s;
+    check_connection(self);
+    Py_BEGIN_ALLOW_THREADS
+    s = mysql_stat(&(self->connection));
+    Py_END_ALLOW_THREADS
+    if (!s) return _mysql_Exception(self);
+    return PyUnicode_FromString(s);
+}
+
+static char _mysql_ConnectionObject_store_result__doc__[] =
+"Returns a result object acquired by mysql_store_result\n\
+(results stored in the client). If no results are available,\n\
+None is returned. Non-standard.\n\
+";
+
+static PyObject *
+_mysql_ConnectionObject_store_result(
+    _mysql_ConnectionObject *self,
+    PyObject *noargs)
+{
+    PyObject *arglist=NULL, *kwarglist=NULL, *result=NULL;
+    _mysql_ResultObject *r=NULL;
+
+    check_connection(self);
+    arglist = Py_BuildValue("(OiO)", self, 0, self->converter);
+    if (!arglist) goto error;
+    kwarglist = PyDict_New();
+    if (!kwarglist) goto error;
+    r = MyAlloc(_mysql_ResultObject, _mysql_ResultObject_Type);
+    if (!r) goto error;
+    if (_mysql_ResultObject_Initialize(r, arglist, kwarglist)) {
+        Py_DECREF(r);
+        goto error;
+    }
+    result = (PyObject *) r;
+    if (!(r->result)) {
+        Py_DECREF(result);
+        Py_INCREF(Py_None);
+        result = Py_None;
+    }
+  error:
+    Py_XDECREF(arglist);
+    Py_XDECREF(kwarglist);
+    return result;
+}
+
+static char _mysql_ConnectionObject_thread_id__doc__[] =
+"Returns the thread ID of the current connection. This value\n\
+can be used as an argument to kill() to kill the thread.\n\
+\n\
+If the connection is lost and you reconnect with ping(), the\n\
+thread ID will change. This means you should not get the\n\
+thread ID and store it for later. You should get it when you\n\
+need it.\n\
+\n\
+Non-standard.";
+
+static PyObject *
+_mysql_ConnectionObject_thread_id(
+    _mysql_ConnectionObject *self,
+    PyObject *noargs)
+{
+    unsigned long pid;
+    check_connection(self);
+    pid = mysql_thread_id(&(self->connection));
+    return PyLong_FromLong((long)pid);
+}
+
+static char _mysql_ConnectionObject_use_result__doc__[] =
+"Returns a result object acquired by mysql_use_result\n\
+(results stored in the server). If no results are available,\n\
+None is returned. Non-standard.\n\
+";
+
+static PyObject *
+_mysql_ConnectionObject_use_result(
+    _mysql_ConnectionObject *self,
+    PyObject *noargs)
+{
+    PyObject *arglist=NULL, *kwarglist=NULL, *result=NULL;
+    _mysql_ResultObject *r=NULL;
+
+    check_connection(self);
+    arglist = Py_BuildValue("(OiO)", self, 1, self->converter);
+    if (!arglist) return NULL;
+    kwarglist = PyDict_New();
+    if (!kwarglist) goto error;
+    r = MyAlloc(_mysql_ResultObject, _mysql_ResultObject_Type);
+    if (!r) goto error;
+    if (_mysql_ResultObject_Initialize(r, arglist, kwarglist)) {
+        Py_DECREF(r);
+        goto error;
+    }
+    result = (PyObject *) r;
+    if (!(r->result)) {
+        Py_DECREF(result);
+        Py_INCREF(Py_None);
+        result = Py_None;
+    }
+  error:
+    Py_DECREF(arglist);
+    Py_XDECREF(kwarglist);
+    return result;
+}
+
+static const char _mysql_ConnectionObject_discard_result__doc__[] =
+"Discard current result set.\n\n"
+"This function can be called instead of use_result() or store_result(). Non-standard.";
+
+static PyObject *
+_mysql_ConnectionObject_discard_result(
+    _mysql_ConnectionObject *self,
+    PyObject *noargs)
+{
+    check_connection(self);
+    MYSQL *conn = &(self->connection);
+
+    Py_BEGIN_ALLOW_THREADS;
+
+    MYSQL_RES *res = mysql_use_result(conn);
+    if (res == NULL) {
+        Py_BLOCK_THREADS;
+        if (mysql_errno(conn) != 0) {
+            // fprintf(stderr, "mysql_use_result failed: %s\n", mysql_error(conn));
+            return _mysql_Exception(self);
+        }
+        Py_RETURN_NONE;
+    }
+
+    MYSQL_ROW row;
+    while (NULL != (row = mysql_fetch_row(res))) {
+        // do nothing.
+    }
+    mysql_free_result(res);
+    Py_END_ALLOW_THREADS;
+    if (mysql_errno(conn)) {
+        // fprintf(stderr, "mysql_free_result failed: %s\n", mysql_error(conn));
+        return _mysql_Exception(self);
+    }
+    Py_RETURN_NONE;
+}
+
+static void
+_mysql_ConnectionObject_dealloc(
+    _mysql_ConnectionObject *self)
+{
+    PyObject_GC_UnTrack(self);
+    if (self->open) {
+        mysql_close(&(self->connection));
+        self->open = 0;
+    }
+    Py_CLEAR(self->converter);
+    MyFree(self);
+}
+
+static PyObject *
+_mysql_ConnectionObject_repr(
+    _mysql_ConnectionObject *self)
+{
+    char buf[300];
+    if (self->open)
+        snprintf(buf, 300, "<_mysql.connection open to '%.256s' at %p>",
+            self->connection.host, self);
+    else
+        snprintf(buf, 300, "<_mysql.connection closed at %p>", self);
+    return PyUnicode_FromString(buf);
+}
+
+static char _mysql_ResultObject_data_seek__doc__[] =
+"data_seek(n) -- seek to row n of result set";
+static PyObject *
+_mysql_ResultObject_data_seek(
+     _mysql_ResultObject *self,
+     PyObject *args)
+{
+    unsigned int row;
+    if (!PyArg_ParseTuple(args, "i:data_seek", &row)) return NULL;
+    check_result_connection(self);
+    mysql_data_seek(self->result, row);
+    Py_RETURN_NONE;
+}
+
+static void
+_mysql_ResultObject_dealloc(
+    _mysql_ResultObject *self)
+{
+    PyObject_GC_UnTrack((PyObject *)self);
+    mysql_free_result(self->result);
+    _mysql_ResultObject_clear(self);
+    MyFree(self);
+}
+
+static PyObject *
+_mysql_ResultObject_repr(
+    _mysql_ResultObject *self)
+{
+    char buf[300];
+    snprintf(buf, 300, "<_mysql.result object at %p>", self);
+    return PyUnicode_FromString(buf);
+}
+
+static PyMethodDef _mysql_ConnectionObject_methods[] = {
+    {
+        "affected_rows",
+        (PyCFunction)_mysql_ConnectionObject_affected_rows,
+        METH_NOARGS,
+        _mysql_ConnectionObject_affected_rows__doc__
+    },
+    {
+        "autocommit",
+        (PyCFunction)_mysql_ConnectionObject_autocommit,
+        METH_VARARGS,
+        _mysql_ConnectionObject_autocommit__doc__
+    },
+    {
+        "get_autocommit",
+        (PyCFunction)_mysql_ConnectionObject_get_autocommit,
+        METH_NOARGS,
+        _mysql_ConnectionObject_get_autocommit__doc__
+    },
+    {
+        "commit",
+        (PyCFunction)_mysql_ConnectionObject_commit,
+        METH_NOARGS,
+        _mysql_ConnectionObject_commit__doc__
+    },
+    {
+        "rollback",
+        (PyCFunction)_mysql_ConnectionObject_rollback,
+        METH_NOARGS,
+        _mysql_ConnectionObject_rollback__doc__
+    },
+    {
+        "next_result",
+        (PyCFunction)_mysql_ConnectionObject_next_result,
+        METH_NOARGS,
+        _mysql_ConnectionObject_next_result__doc__
+    },
+    {
+        "set_server_option",
+        (PyCFunction)_mysql_ConnectionObject_set_server_option,
+        METH_VARARGS,
+        _mysql_ConnectionObject_set_server_option__doc__
+    },
+    {
+        "sqlstate",
+        (PyCFunction)_mysql_ConnectionObject_sqlstate,
+        METH_NOARGS,
+        _mysql_ConnectionObject_sqlstate__doc__
+    },
+    {
+        "warning_count",
+        (PyCFunction)_mysql_ConnectionObject_warning_count,
+        METH_NOARGS,
+        _mysql_ConnectionObject_warning_count__doc__
+    },
+    {
+        "change_user",
+        (PyCFunction)_mysql_ConnectionObject_change_user,
+        METH_VARARGS | METH_KEYWORDS,
+        _mysql_ConnectionObject_change_user__doc__
+    },
+    {
+        "character_set_name",
+        (PyCFunction)_mysql_ConnectionObject_character_set_name,
+        METH_NOARGS,
+        _mysql_ConnectionObject_character_set_name__doc__
+    },
+    {
+        "set_character_set",
+        (PyCFunction)_mysql_ConnectionObject_set_character_set,
+        METH_VARARGS,
+        _mysql_ConnectionObject_set_character_set__doc__
+    },
+#if MYSQL_VERSION_ID >= 50010
+    {
+        "get_character_set_info",
+        (PyCFunction)_mysql_ConnectionObject_get_character_set_info,
+        METH_NOARGS,
+        _mysql_ConnectionObject_get_character_set_info__doc__
+    },
+#endif
+    {
+        "_get_native_connection",
+        (PyCFunction)_mysql_ConnectionObject_get_native_connection,
+        METH_NOARGS,
+        _mysql_ConnectionObject_get_native_connection__doc__
+    },
+    {
+        "close",
+        (PyCFunction)_mysql_ConnectionObject_close,
+        METH_NOARGS,
+        _mysql_ConnectionObject_close__doc__
+    },
+    {
+        "dump_debug_info",
+        (PyCFunction)_mysql_ConnectionObject_dump_debug_info,
+        METH_NOARGS,
+        _mysql_ConnectionObject_dump_debug_info__doc__
+    },
+    {
+        "escape",
+        (PyCFunction)_mysql_escape,
+        METH_VARARGS,
+        _mysql_escape__doc__
+    },
+    {
+        "escape_string",
+        (PyCFunction)_mysql_escape_string,
+        METH_VARARGS,
+        _mysql_escape_string__doc__
+    },
+    {
+        "error",
+        (PyCFunction)_mysql_ConnectionObject_error,
+        METH_NOARGS,
+        _mysql_ConnectionObject_error__doc__
+    },
+    {
+        "errno",
+        (PyCFunction)_mysql_ConnectionObject_errno,
+        METH_NOARGS,
+        _mysql_ConnectionObject_errno__doc__
+    },
+    {
+        "field_count",
+        (PyCFunction)_mysql_ConnectionObject_field_count,
+        METH_NOARGS,
+        _mysql_ConnectionObject_field_count__doc__
+    },
+    {
+        "fileno",
+        (PyCFunction)_mysql_ConnectionObject_fileno,
+        METH_NOARGS,
+        _mysql_ConnectionObject_fileno__doc__
+    },
+    {
+        "get_host_info",
+        (PyCFunction)_mysql_ConnectionObject_get_host_info,
+        METH_NOARGS,
+        _mysql_ConnectionObject_get_host_info__doc__
+    },
+    {
+        "get_proto_info",
+        (PyCFunction)_mysql_ConnectionObject_get_proto_info,
+        METH_NOARGS,
+        _mysql_ConnectionObject_get_proto_info__doc__
+    },
+    {
+        "get_server_info",
+        (PyCFunction)_mysql_ConnectionObject_get_server_info,
+        METH_NOARGS,
+        _mysql_ConnectionObject_get_server_info__doc__
+    },
+    {
+        "info",
+        (PyCFunction)_mysql_ConnectionObject_info,
+        METH_NOARGS,
+        _mysql_ConnectionObject_info__doc__
+    },
+    {
+        "insert_id",
+        (PyCFunction)_mysql_ConnectionObject_insert_id,
+        METH_NOARGS,
+        _mysql_ConnectionObject_insert_id__doc__
+    },
+    {
+        "kill",
+        (PyCFunction)_mysql_ConnectionObject_kill,
+        METH_VARARGS,
+        _mysql_ConnectionObject_kill__doc__
+    },
+    {
+        "ping",
+        (PyCFunction)_mysql_ConnectionObject_ping,
+        METH_VARARGS,
+        _mysql_ConnectionObject_ping__doc__
+    },
+    {
+        "query",
+        (PyCFunction)_mysql_ConnectionObject_query,
+        METH_VARARGS,
+        _mysql_ConnectionObject_query__doc__
+    },
+    {
+        "send_query",
+        (PyCFunction)_mysql_ConnectionObject_send_query,
+        METH_VARARGS,
+        _mysql_ConnectionObject_send_query__doc__,
+    },
+    {
+        "read_query_result",
+        (PyCFunction)_mysql_ConnectionObject_read_query_result,
+        METH_NOARGS,
+        _mysql_ConnectionObject_read_query_result__doc__,
+    },
+    {
+        "select_db",
+        (PyCFunction)_mysql_ConnectionObject_select_db,
+        METH_VARARGS,
+        _mysql_ConnectionObject_select_db__doc__
+    },
+    {
+        "shutdown",
+        (PyCFunction)_mysql_ConnectionObject_shutdown,
+        METH_NOARGS,
+        _mysql_ConnectionObject_shutdown__doc__
+    },
+    {
+        "stat",
+        (PyCFunction)_mysql_ConnectionObject_stat,
+        METH_NOARGS,
+        _mysql_ConnectionObject_stat__doc__
+    },
+    {
+        "store_result",
+        (PyCFunction)_mysql_ConnectionObject_store_result,
+        METH_NOARGS,
+        _mysql_ConnectionObject_store_result__doc__
+    },
+    {
+        "string_literal",
+        (PyCFunction)_mysql_string_literal,
+        METH_O,
+        _mysql_string_literal__doc__},
+    {
+        "thread_id",
+        (PyCFunction)_mysql_ConnectionObject_thread_id,
+        METH_NOARGS,
+        _mysql_ConnectionObject_thread_id__doc__
+    },
+    {
+        "use_result",
+        (PyCFunction)_mysql_ConnectionObject_use_result,
+        METH_NOARGS,
+        _mysql_ConnectionObject_use_result__doc__
+    },
+    {
+        "discard_result",
+        (PyCFunction)_mysql_ConnectionObject_discard_result,
+        METH_NOARGS,
+        _mysql_ConnectionObject_discard_result__doc__
+    },
+    {NULL,              NULL} /* sentinel */
+};
+
+static struct PyMemberDef _mysql_ConnectionObject_memberlist[] = {
+    {
+        "open",
+        T_INT,
+        offsetof(_mysql_ConnectionObject,open),
+        READONLY,
+        "True if connection is open"
+    },
+    {
+        "converter",
+        T_OBJECT,
+        offsetof(_mysql_ConnectionObject,converter),
+        0,
+        "Type conversion mapping"
+    },
+    {
+        "server_capabilities",
+        T_ULONG,
+        offsetof(_mysql_ConnectionObject,connection.server_capabilities),
+        READONLY,
+        "Capabilities of server; consult MySQLdb.constants.CLIENT"
+    },
+    {
+        "port",
+        T_UINT,
+        offsetof(_mysql_ConnectionObject,connection.port),
+        READONLY,
+        "TCP/IP port of the server connection"
+    },
+    {
+        "client_flag",
+        T_ULONG,
+        offsetof(_mysql_ConnectionObject,connection.client_flag),
+        READONLY,
+        "Client flags; refer to MySQLdb.constants.CLIENT"
+    },
+    {NULL} /* Sentinel */
+};
+
+static PyMethodDef _mysql_ResultObject_methods[] = {
+    {
+        "data_seek",
+        (PyCFunction)_mysql_ResultObject_data_seek,
+        METH_VARARGS,
+        _mysql_ResultObject_data_seek__doc__
+    },
+    {
+        "describe",
+        (PyCFunction)_mysql_ResultObject_describe,
+        METH_NOARGS,
+        _mysql_ResultObject_describe__doc__
+    },
+    {
+        "fetch_row",
+        (PyCFunction)_mysql_ResultObject_fetch_row,
+        METH_VARARGS | METH_KEYWORDS,
+        _mysql_ResultObject_fetch_row__doc__
+    },
+    {
+        "discard",
+        (PyCFunction)_mysql_ResultObject_discard,
+        METH_NOARGS,
+        _mysql_ResultObject_discard__doc__
+    },
+    {
+        "field_flags",
+        (PyCFunction)_mysql_ResultObject_field_flags,
+        METH_NOARGS,
+        _mysql_ResultObject_field_flags__doc__
+    },
+    {
+        "num_fields",
+        (PyCFunction)_mysql_ResultObject_num_fields,
+        METH_NOARGS,
+        _mysql_ResultObject_num_fields__doc__
+    },
+    {
+        "num_rows",
+        (PyCFunction)_mysql_ResultObject_num_rows,
+        METH_NOARGS,
+        _mysql_ResultObject_num_rows__doc__
+    },
+    {NULL,              NULL} /* sentinel */
+};
+
+static struct PyMemberDef _mysql_ResultObject_memberlist[] = {
+    {
+        "converter",
+        T_OBJECT,
+        offsetof(_mysql_ResultObject,converter),
+        READONLY,
+        "Type conversion mapping"
+    },
+    {
+        "has_next",
+        T_BOOL,
+        offsetof(_mysql_ResultObject, has_next),
+        READONLY,
+        "Has next result"
+    },
+    {NULL} /* Sentinel */
+};
+
+static PyObject *
+_mysql_ConnectionObject_getattro(
+    _mysql_ConnectionObject *self,
+    PyObject *name)
+{
+    const char *cname;
+    cname = PyUnicode_AsUTF8(name);
+    if (strcmp(cname, "closed") == 0)
+        return PyLong_FromLong((long)!(self->open));
+
+    return PyObject_GenericGetAttr((PyObject *)self, name);
+}
+
+static int
+_mysql_ConnectionObject_setattro(
+    _mysql_ConnectionObject *self,
+    PyObject *name,
+    PyObject *v)
+{
+    if (v == NULL) {
+        PyErr_SetString(PyExc_AttributeError,
+                "can't delete connection attributes");
+        return -1;
+    }
+    return PyObject_GenericSetAttr((PyObject *)self, name, v);
+}
+
+static int
+_mysql_ResultObject_setattro(
+    _mysql_ResultObject *self,
+    PyObject *name,
+    PyObject *v)
+{
+    if (v == NULL) {
+        PyErr_SetString(PyExc_AttributeError,
+                "can't delete connection attributes");
+        return -1;
+    }
+    return PyObject_GenericSetAttr((PyObject *)self, name, v);
+}
+
+PyTypeObject _mysql_ConnectionObject_Type = {
+    PyVarObject_HEAD_INIT(NULL, 0)
+    "_mysql.connection", /* (char *)tp_name For printing */
+    sizeof(_mysql_ConnectionObject),
+    0,
+    (destructor)_mysql_ConnectionObject_dealloc, /* tp_dealloc */
+    0, /*tp_print*/
+    0, /* tp_getattr */
+    0, /* tp_setattr */
+    0, /*tp_compare*/
+    (reprfunc)_mysql_ConnectionObject_repr, /* tp_repr */
+
+    /* Method suites for standard classes */
+
+    0, /* (PyNumberMethods *) tp_as_number */
+    0, /* (PySequenceMethods *) tp_as_sequence */
+    0, /* (PyMappingMethods *) tp_as_mapping */
+
+    /* More standard operations (here for binary compatibility) */
+
+    0, /* (hashfunc) tp_hash */
+    0, /* (ternaryfunc) tp_call */
+    0, /* (reprfunc) tp_str */
+    (getattrofunc)_mysql_ConnectionObject_getattro, /* tp_getattro */
+    (setattrofunc)_mysql_ConnectionObject_setattro, /* tp_setattro */
+
+    /* Functions to access object as input/output buffer */
+    0, /* (PyBufferProcs *) tp_as_buffer */
+
+    /* (tp_flags) Flags to define presence of optional/expanded features */
+    Py_TPFLAGS_DEFAULT | Py_TPFLAGS_HAVE_GC | Py_TPFLAGS_BASETYPE,
+    _mysql_connect__doc__, /* (char *) tp_doc Documentation string */
+
+    /* call function for all accessible objects */
+    (traverseproc) _mysql_ConnectionObject_traverse, /* tp_traverse */
+
+    /* delete references to contained objects */
+    (inquiry) _mysql_ConnectionObject_clear, /* tp_clear */
+
+    /* rich comparisons */
+    0, /* (richcmpfunc) tp_richcompare */
+
+    /* weak reference enabler */
+    0, /* (long) tp_weaklistoffset */
+
+    /* Iterators */
+    0, /* (getiterfunc) tp_iter */
+    0, /* (iternextfunc) tp_iternext */
+
+    /* Attribute descriptor and subclassing stuff */
+    (struct PyMethodDef *)_mysql_ConnectionObject_methods, /* tp_methods */
+    (struct PyMemberDef *)_mysql_ConnectionObject_memberlist, /* tp_members */
+    0, /* (struct getsetlist *) tp_getset; */
+    0, /* (struct _typeobject *) tp_base; */
+    0, /* (PyObject *) tp_dict */
+    0, /* (descrgetfunc) tp_descr_get */
+    0, /* (descrsetfunc) tp_descr_set */
+    0, /* (long) tp_dictoffset */
+    (initproc)_mysql_ConnectionObject_Initialize, /* tp_init */
+    NULL, /* tp_alloc */
+    PyType_GenericNew, /* tp_new */
+    NULL, /* tp_free Low-level free-memory routine */
+    0, /* (PyObject *) tp_bases */
+    0, /* (PyObject *) tp_mro method resolution order */
+    0, /* (PyObject *) tp_defined */
+} ;
+
+PyTypeObject _mysql_ResultObject_Type = {
+    PyVarObject_HEAD_INIT(NULL, 0)
+    "_mysql.result",
+    sizeof(_mysql_ResultObject),
+    0,
+    (destructor)_mysql_ResultObject_dealloc, /* tp_dealloc */
+    0, /*tp_print*/
+    0, /* tp_getattr */
+    0, /* tp_setattr */
+    0, /*tp_compare*/
+    (reprfunc)_mysql_ResultObject_repr, /* tp_repr */
+
+    /* Method suites for standard classes */
+
+    0, /* (PyNumberMethods *) tp_as_number */
+    0, /* (PySequenceMethods *) tp_as_sequence */
+    0, /* (PyMappingMethods *) tp_as_mapping */
+
+    /* More standard operations (here for binary compatibility) */
+
+    0, /* (hashfunc) tp_hash */
+    0, /* (ternaryfunc) tp_call */
+    0, /* (reprfunc) tp_str */
+    (getattrofunc)PyObject_GenericGetAttr, /* tp_getattro */
+    (setattrofunc)_mysql_ResultObject_setattro, /* tp_setattr */
+
+    /* Functions to access object as input/output buffer */
+    0, /* (PyBufferProcs *) tp_as_buffer */
+
+    /* Flags to define presence of optional/expanded features */
+    Py_TPFLAGS_DEFAULT | Py_TPFLAGS_HAVE_GC | Py_TPFLAGS_BASETYPE,
+
+    _mysql_ResultObject__doc__, /* (char *) tp_doc Documentation string */
+
+    /* call function for all accessible objects */
+    (traverseproc) _mysql_ResultObject_traverse, /* tp_traverse */
+
+    /* delete references to contained objects */
+    (inquiry) _mysql_ResultObject_clear, /* tp_clear */
+
+    /* rich comparisons */
+    0, /* (richcmpfunc) tp_richcompare */
+
+    /* weak reference enabler */
+    0, /* (long) tp_weaklistoffset */
+
+    /* Iterators */
+    0, /* (getiterfunc) tp_iter */
+    0, /* (iternextfunc) tp_iternext */
+
+    /* Attribute descriptor and subclassing stuff */
+    (struct PyMethodDef *) _mysql_ResultObject_methods, /* tp_methods */
+    (struct PyMemberDef *) _mysql_ResultObject_memberlist, /*tp_members */
+    0, /* (struct getsetlist *) tp_getset; */
+    0, /* (struct _typeobject *) tp_base; */
+    0, /* (PyObject *) tp_dict */
+    0, /* (descrgetfunc) tp_descr_get */
+    0, /* (descrsetfunc) tp_descr_set */
+    0, /* (long) tp_dictoffset */
+    (initproc)_mysql_ResultObject_Initialize, /* tp_init */
+    NULL, /* tp_alloc */
+    PyType_GenericNew, /* tp_new */
+    NULL, /* tp_free Low-level free-memory routine */
+    0, /* (PyObject *) tp_bases */
+    0, /* (PyObject *) tp_mro method resolution order */
+    0, /* (PyObject *) tp_defined */
+};
+
+static PyMethodDef
+_mysql_methods[] = {
+    {
+        "connect",
+        (PyCFunction)_mysql_connect,
+        METH_VARARGS | METH_KEYWORDS,
+        _mysql_connect__doc__
+    },
+    {
+        "debug",
+        (PyCFunction)_mysql_debug,
+        METH_VARARGS,
+        _mysql_debug__doc__
+    },
+    {
+        "escape",
+        (PyCFunction)_mysql_escape,
+        METH_VARARGS,
+        _mysql_escape__doc__
+    },
+    {
+        "escape_string",
+        (PyCFunction)_mysql_escape_string,
+        METH_VARARGS,
+        _mysql_escape_string__doc__
+    },
+    {
+        "string_literal",
+        (PyCFunction)_mysql_string_literal,
+        METH_O,
+        _mysql_string_literal__doc__
+    },
+    {
+        "get_client_info",
+        (PyCFunction)_mysql_get_client_info,
+        METH_NOARGS,
+        _mysql_get_client_info__doc__
+    },
+    {NULL, NULL} /* sentinel */
+};
+
+static PyObject *
+_mysql_NewException(
+    PyObject *dict,
+    PyObject *edict,
+    char *name)
+{
+    PyObject *e;
+    if (!(e = PyDict_GetItemString(edict, name)))
+        return NULL;
+    if (PyDict_SetItemString(dict, name, e))
+        return NULL;
+    Py_INCREF(e);
+    return e;
+}
+
+#define QUOTE(X) _QUOTE(X)
+#define _QUOTE(X) #X
+
+static char _mysql___doc__[] =
+"an adaptation of the MySQL C API (mostly)\n\
+\n\
+You probably are better off using MySQLdb instead of using this\n\
+module directly.\n\
+\n\
+In general, renaming goes from mysql_* to _mysql.*. _mysql.connect()\n\
+returns a connection object (MYSQL). Functions which expect MYSQL * as\n\
+an argument are now methods of the connection object. A number of things\n\
+return result objects (MYSQL_RES). Functions which expect MYSQL_RES * as\n\
+an argument are now methods of the result object. Deprecated functions\n\
+(as of 3.23) are NOT implemented.\n\
+";
+
+static struct PyModuleDef _mysqlmodule = {
+   PyModuleDef_HEAD_INIT,
+   "_mysql",   /* name of module */
+   _mysql___doc__, /* module documentation, may be NULL */
+   -1,       /* size of per-interpreter state of the module,
+                or -1 if the module keeps state in global variables. */
+   _mysql_methods
+};
+
+PyMODINIT_FUNC
+PyInit__mysql(void)
+{
+    PyObject *dict, *module, *emod, *edict;
+
+    if (mysql_library_init(0, NULL, NULL)) {
+        PyErr_SetString(PyExc_ImportError, "_mysql: mysql_library_init failed");
+        return NULL;
+    }
+
+    if (PyType_Ready(&_mysql_ConnectionObject_Type) < 0)
+        return NULL;
+    if (PyType_Ready(&_mysql_ResultObject_Type) < 0)
+        return NULL;
+
+    module = PyModule_Create(&_mysqlmodule);
+    if (!module) return module; /* this really should never happen */
+
+    if (!(dict = PyModule_GetDict(module))) goto error;
+    if (PyDict_SetItemString(dict, "version_info",
+                   PyRun_String(QUOTE(version_info), Py_eval_input,
+                       dict, dict)))
+        goto error;
+    if (PyDict_SetItemString(dict, "__version__",
+                   PyUnicode_FromString(QUOTE(__version__))))
+        goto error;
+    if (PyDict_SetItemString(dict, "connection",
+                   (PyObject *)&_mysql_ConnectionObject_Type))
+        goto error;
+    Py_INCREF(&_mysql_ConnectionObject_Type);
+    if (PyDict_SetItemString(dict, "result",
+                   (PyObject *)&_mysql_ResultObject_Type))
+        goto error;
+    Py_INCREF(&_mysql_ResultObject_Type);
+    if (!(emod = PyImport_ImportModule("MySQLdb._exceptions"))) {
+        PyErr_Print();
+        goto error;
+    }
+    if (!(edict = PyModule_GetDict(emod))) goto error;
+    if (!(_mysql_MySQLError =
+          _mysql_NewException(dict, edict, "MySQLError")))
+        goto error;
+    if (!(_mysql_Warning =
+          _mysql_NewException(dict, edict, "Warning")))
+        goto error;
+    if (!(_mysql_Error =
+          _mysql_NewException(dict, edict, "Error")))
+        goto error;
+    if (!(_mysql_InterfaceError =
+          _mysql_NewException(dict, edict, "InterfaceError")))
+        goto error;
+    if (!(_mysql_DatabaseError =
+          _mysql_NewException(dict, edict, "DatabaseError")))
+        goto error;
+    if (!(_mysql_DataError =
+          _mysql_NewException(dict, edict, "DataError")))
+        goto error;
+    if (!(_mysql_OperationalError =
+          _mysql_NewException(dict, edict, "OperationalError")))
+        goto error;
+    if (!(_mysql_IntegrityError =
+          _mysql_NewException(dict, edict, "IntegrityError")))
+        goto error;
+    if (!(_mysql_InternalError =
+          _mysql_NewException(dict, edict, "InternalError")))
+        goto error;
+    if (!(_mysql_ProgrammingError =
+          _mysql_NewException(dict, edict, "ProgrammingError")))
+        goto error;
+    if (!(_mysql_NotSupportedError =
+          _mysql_NewException(dict, edict, "NotSupportedError")))
+        goto error;
+    Py_DECREF(emod);
+  error:
+    if (PyErr_Occurred()) {
+        PyErr_SetString(PyExc_ImportError, "_mysql: init failed");
+        module = NULL;
+    }
+    return module;
+}
+
+/* vim: set ts=4 sts=4 sw=4 expandtab : */
```

### Comparing `mysqlclient-2.2.0/src/MySQLdb/connections.py` & `mysqlclient-2.2.0rc1/src/MySQLdb/connections.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,337 +1,337 @@
-"""
-This module implements connections for MySQLdb. Presently there is
-only one class: Connection. Others are unlikely. However, you might
-want to make your own subclasses. In most cases, you will probably
-override Connection.default_cursor with a non-standard Cursor class.
-"""
-import re
-
-from . import cursors, _mysql
-from ._exceptions import (
-    Warning,
-    Error,
-    InterfaceError,
-    DataError,
-    DatabaseError,
-    OperationalError,
-    IntegrityError,
-    InternalError,
-    NotSupportedError,
-    ProgrammingError,
-)
-
-# Mapping from MySQL charset name to Python codec name
-_charset_to_encoding = {
-    "utf8mb4": "utf8",
-    "utf8mb3": "utf8",
-    "latin1": "cp1252",
-    "koi8r": "koi8_r",
-    "koi8u": "koi8_u",
-}
-
-re_numeric_part = re.compile(r"^(\d+)")
-
-
-def numeric_part(s):
-    """Returns the leading numeric part of a string.
-
-    >>> numeric_part("20-alpha")
-    20
-    >>> numeric_part("foo")
-    >>> numeric_part("16b")
-    16
-    """
-
-    m = re_numeric_part.match(s)
-    if m:
-        return int(m.group(1))
-    return None
-
-
-class Connection(_mysql.connection):
-    """MySQL Database Connection Object"""
-
-    default_cursor = cursors.Cursor
-
-    def __init__(self, *args, **kwargs):
-        """
-        Create a connection to the database. It is strongly recommended
-        that you only use keyword parameters. Consult the MySQL C API
-        documentation for more information.
-
-        :param str host:        host to connect
-        :param str user:        user to connect as
-        :param str password:    password to use
-        :param str passwd:      alias of password (deprecated)
-        :param str database:    database to use
-        :param str db:          alias of database (deprecated)
-        :param int port:        TCP/IP port to connect to
-        :param str unix_socket: location of unix_socket to use
-        :param dict conv:       conversion dictionary, see MySQLdb.converters
-        :param int connect_timeout:
-            number of seconds to wait before the connection attempt fails.
-
-        :param bool compress:   if set, compression is enabled
-        :param str named_pipe:  if set, a named pipe is used to connect (Windows only)
-        :param str init_command:
-            command which is run once the connection is created
-
-        :param str read_default_file:
-            file from which default client values are read
-
-        :param str read_default_group:
-            configuration group to use from the default file
-
-        :param type cursorclass:
-            class object, used to create cursors (keyword only)
-
-        :param bool use_unicode:
-            If True, text-like columns are returned as unicode objects
-            using the connection's character set. Otherwise, text-like
-            columns are returned as bytes. Unicode objects will always
-            be encoded to the connection's character set regardless of
-            this setting.
-            Default to True.
-
-        :param str charset:
-            If supplied, the connection character set will be changed
-            to this character set.
-
-        :param str collation:
-            If ``charset`` and ``collation`` are both supplied, the
-            character set and collation for the current connection
-            will be set.
-
-            If omitted, empty string, or None, the default collation
-            for the ``charset`` is implied.
-
-        :param str auth_plugin:
-            If supplied, the connection default authentication plugin will be
-            changed to this value. Example values:
-            `mysql_native_password` or `caching_sha2_password`
-
-        :param str sql_mode:
-            If supplied, the session SQL mode will be changed to this
-            setting.
-            For more details and legal values, see the MySQL documentation.
-
-        :param int client_flag:
-            flags to use or 0 (see MySQL docs or constants/CLIENTS.py)
-
-        :param bool multi_statements:
-            If True, enable multi statements for clients >= 4.1.
-            Defaults to True.
-
-        :param str ssl_mode:
-            specify the security settings for connection to the server;
-            see the MySQL documentation for more details
-            (mysql_option(), MYSQL_OPT_SSL_MODE).
-            Only one of 'DISABLED', 'PREFERRED', 'REQUIRED',
-            'VERIFY_CA', 'VERIFY_IDENTITY' can be specified.
-
-        :param dict ssl:
-            dictionary or mapping contains SSL connection parameters;
-            see the MySQL documentation for more details
-            (mysql_ssl_set()).  If this is set, and the client does not
-            support SSL, NotSupportedError will be raised.
-
-        :param bool local_infile:
-            enables LOAD LOCAL INFILE; zero disables
-
-        :param bool autocommit:
-            If False (default), autocommit is disabled.
-            If True, autocommit is enabled.
-            If None, autocommit isn't set and server default is used.
-
-        :param bool binary_prefix:
-            If set, the '_binary' prefix will be used for raw byte query
-            arguments (e.g. Binary). This is disabled by default.
-
-        There are a number of undocumented, non-standard methods. See the
-        documentation for the MySQL C API for some hints on what they do.
-        """
-        from MySQLdb.constants import CLIENT, FIELD_TYPE
-        from MySQLdb.converters import conversions, _bytes_or_str
-
-        kwargs2 = kwargs.copy()
-
-        if "db" in kwargs2:
-            kwargs2["database"] = kwargs2.pop("db")
-        if "passwd" in kwargs2:
-            kwargs2["password"] = kwargs2.pop("passwd")
-
-        if "conv" in kwargs:
-            conv = kwargs["conv"]
-        else:
-            conv = conversions
-
-        conv2 = {}
-        for k, v in conv.items():
-            if isinstance(k, int) and isinstance(v, list):
-                conv2[k] = v[:]
-            else:
-                conv2[k] = v
-        kwargs2["conv"] = conv2
-
-        cursorclass = kwargs2.pop("cursorclass", self.default_cursor)
-        charset = kwargs2.get("charset", "")
-        collation = kwargs2.pop("collation", "")
-        use_unicode = kwargs2.pop("use_unicode", True)
-        sql_mode = kwargs2.pop("sql_mode", "")
-        self._binary_prefix = kwargs2.pop("binary_prefix", False)
-
-        client_flag = kwargs.get("client_flag", 0)
-        client_flag |= CLIENT.MULTI_RESULTS
-        multi_statements = kwargs2.pop("multi_statements", True)
-        if multi_statements:
-            client_flag |= CLIENT.MULTI_STATEMENTS
-        kwargs2["client_flag"] = client_flag
-
-        # PEP-249 requires autocommit to be initially off
-        autocommit = kwargs2.pop("autocommit", False)
-
-        super().__init__(*args, **kwargs2)
-        self.cursorclass = cursorclass
-        self.encoders = {k: v for k, v in conv.items() if type(k) is not int}
-
-        self._server_version = tuple(
-            [numeric_part(n) for n in self.get_server_info().split(".")[:2]]
-        )
-
-        self.encoding = "ascii"  # overridden in set_character_set()
-
-        if not charset:
-            charset = self.character_set_name()
-        self.set_character_set(charset, collation)
-
-        if sql_mode:
-            self.set_sql_mode(sql_mode)
-
-        if use_unicode:
-            for t in (
-                FIELD_TYPE.STRING,
-                FIELD_TYPE.VAR_STRING,
-                FIELD_TYPE.VARCHAR,
-                FIELD_TYPE.TINY_BLOB,
-                FIELD_TYPE.MEDIUM_BLOB,
-                FIELD_TYPE.LONG_BLOB,
-                FIELD_TYPE.BLOB,
-            ):
-                self.converter[t] = _bytes_or_str
-            # Unlike other string/blob types, JSON is always text.
-            # MySQL may return JSON with charset==binary.
-            self.converter[FIELD_TYPE.JSON] = str
-
-        self._transactional = self.server_capabilities & CLIENT.TRANSACTIONS
-        if self._transactional:
-            if autocommit is not None:
-                self.autocommit(autocommit)
-        self.messages = []
-
-    def __enter__(self):
-        return self
-
-    def __exit__(self, exc_type, exc_value, traceback):
-        self.close()
-
-    def autocommit(self, on):
-        on = bool(on)
-        if self.get_autocommit() != on:
-            _mysql.connection.autocommit(self, on)
-
-    def cursor(self, cursorclass=None):
-        """
-        Create a cursor on which queries may be performed. The
-        optional cursorclass parameter is used to create the
-        Cursor. By default, self.cursorclass=cursors.Cursor is
-        used.
-        """
-        return (cursorclass or self.cursorclass)(self)
-
-    def query(self, query):
-        # Since _mysql releases GIL while querying, we need immutable buffer.
-        if isinstance(query, bytearray):
-            query = bytes(query)
-        _mysql.connection.query(self, query)
-
-    def _bytes_literal(self, bs):
-        assert isinstance(bs, (bytes, bytearray))
-        x = self.string_literal(bs)  # x is escaped and quoted bytes
-        if self._binary_prefix:
-            return b"_binary" + x
-        return x
-
-    def _tuple_literal(self, t):
-        return b"(%s)" % (b",".join(map(self.literal, t)))
-
-    def literal(self, o):
-        """If o is a single object, returns an SQL literal as a string.
-        If o is a non-string sequence, the items of the sequence are
-        converted and returned as a sequence.
-
-        Non-standard. For internal use; do not use this in your
-        applications.
-        """
-        if isinstance(o, str):
-            s = self.string_literal(o.encode(self.encoding))
-        elif isinstance(o, bytearray):
-            s = self._bytes_literal(o)
-        elif isinstance(o, bytes):
-            s = self._bytes_literal(o)
-        elif isinstance(o, (tuple, list)):
-            s = self._tuple_literal(o)
-        else:
-            s = self.escape(o, self.encoders)
-            if isinstance(s, str):
-                s = s.encode(self.encoding)
-        assert isinstance(s, bytes)
-        return s
-
-    def begin(self):
-        """Explicitly begin a connection.
-
-        This method is not used when autocommit=False (default).
-        """
-        self.query(b"BEGIN")
-
-    def set_character_set(self, charset, collation=None):
-        """Set the connection character set to charset."""
-        super().set_character_set(charset)
-        self.encoding = _charset_to_encoding.get(charset, charset)
-        if collation:
-            self.query(f"SET NAMES {charset} COLLATE {collation}")
-            self.store_result()
-
-    def set_sql_mode(self, sql_mode):
-        """Set the connection sql_mode. See MySQL documentation for
-        legal values."""
-        if self._server_version < (4, 1):
-            raise NotSupportedError("server is too old to set sql_mode")
-        self.query("SET SESSION sql_mode='%s'" % sql_mode)
-        self.store_result()
-
-    def show_warnings(self):
-        """Return detailed information about warnings as a
-        sequence of tuples of (Level, Code, Message). This
-        is only supported in MySQL-4.1 and up. If your server
-        is an earlier version, an empty sequence is returned."""
-        if self._server_version < (4, 1):
-            return ()
-        self.query("SHOW WARNINGS")
-        r = self.store_result()
-        warnings = r.fetch_row(0)
-        return warnings
-
-    Warning = Warning
-    Error = Error
-    InterfaceError = InterfaceError
-    DatabaseError = DatabaseError
-    DataError = DataError
-    OperationalError = OperationalError
-    IntegrityError = IntegrityError
-    InternalError = InternalError
-    ProgrammingError = ProgrammingError
-    NotSupportedError = NotSupportedError
-
-
-# vim: colorcolumn=100
+"""
+This module implements connections for MySQLdb. Presently there is
+only one class: Connection. Others are unlikely. However, you might
+want to make your own subclasses. In most cases, you will probably
+override Connection.default_cursor with a non-standard Cursor class.
+"""
+import re
+
+from . import cursors, _mysql
+from ._exceptions import (
+    Warning,
+    Error,
+    InterfaceError,
+    DataError,
+    DatabaseError,
+    OperationalError,
+    IntegrityError,
+    InternalError,
+    NotSupportedError,
+    ProgrammingError,
+)
+
+# Mapping from MySQL charset name to Python codec name
+_charset_to_encoding = {
+    "utf8mb4": "utf8",
+    "utf8mb3": "utf8",
+    "latin1": "cp1252",
+    "koi8r": "koi8_r",
+    "koi8u": "koi8_u",
+}
+
+re_numeric_part = re.compile(r"^(\d+)")
+
+
+def numeric_part(s):
+    """Returns the leading numeric part of a string.
+
+    >>> numeric_part("20-alpha")
+    20
+    >>> numeric_part("foo")
+    >>> numeric_part("16b")
+    16
+    """
+
+    m = re_numeric_part.match(s)
+    if m:
+        return int(m.group(1))
+    return None
+
+
+class Connection(_mysql.connection):
+    """MySQL Database Connection Object"""
+
+    default_cursor = cursors.Cursor
+
+    def __init__(self, *args, **kwargs):
+        """
+        Create a connection to the database. It is strongly recommended
+        that you only use keyword parameters. Consult the MySQL C API
+        documentation for more information.
+
+        :param str host:        host to connect
+        :param str user:        user to connect as
+        :param str password:    password to use
+        :param str passwd:      alias of password (deprecated)
+        :param str database:    database to use
+        :param str db:          alias of database (deprecated)
+        :param int port:        TCP/IP port to connect to
+        :param str unix_socket: location of unix_socket to use
+        :param dict conv:       conversion dictionary, see MySQLdb.converters
+        :param int connect_timeout:
+            number of seconds to wait before the connection attempt fails.
+
+        :param bool compress:   if set, compression is enabled
+        :param str named_pipe:  if set, a named pipe is used to connect (Windows only)
+        :param str init_command:
+            command which is run once the connection is created
+
+        :param str read_default_file:
+            file from which default client values are read
+
+        :param str read_default_group:
+            configuration group to use from the default file
+
+        :param type cursorclass:
+            class object, used to create cursors (keyword only)
+
+        :param bool use_unicode:
+            If True, text-like columns are returned as unicode objects
+            using the connection's character set. Otherwise, text-like
+            columns are returned as bytes. Unicode objects will always
+            be encoded to the connection's character set regardless of
+            this setting.
+            Default to True.
+
+        :param str charset:
+            If supplied, the connection character set will be changed
+            to this character set.
+
+        :param str collation:
+            If ``charset`` and ``collation`` are both supplied, the
+            character set and collation for the current connection
+            will be set.
+
+            If omitted, empty string, or None, the default collation
+            for the ``charset`` is implied.
+
+        :param str auth_plugin:
+            If supplied, the connection default authentication plugin will be
+            changed to this value. Example values:
+            `mysql_native_password` or `caching_sha2_password`
+
+        :param str sql_mode:
+            If supplied, the session SQL mode will be changed to this
+            setting.
+            For more details and legal values, see the MySQL documentation.
+
+        :param int client_flag:
+            flags to use or 0 (see MySQL docs or constants/CLIENTS.py)
+
+        :param bool multi_statements:
+            If True, enable multi statements for clients >= 4.1.
+            Defaults to True.
+
+        :param str ssl_mode:
+            specify the security settings for connection to the server;
+            see the MySQL documentation for more details
+            (mysql_option(), MYSQL_OPT_SSL_MODE).
+            Only one of 'DISABLED', 'PREFERRED', 'REQUIRED',
+            'VERIFY_CA', 'VERIFY_IDENTITY' can be specified.
+
+        :param dict ssl:
+            dictionary or mapping contains SSL connection parameters;
+            see the MySQL documentation for more details
+            (mysql_ssl_set()).  If this is set, and the client does not
+            support SSL, NotSupportedError will be raised.
+
+        :param bool local_infile:
+            enables LOAD LOCAL INFILE; zero disables
+
+        :param bool autocommit:
+            If False (default), autocommit is disabled.
+            If True, autocommit is enabled.
+            If None, autocommit isn't set and server default is used.
+
+        :param bool binary_prefix:
+            If set, the '_binary' prefix will be used for raw byte query
+            arguments (e.g. Binary). This is disabled by default.
+
+        There are a number of undocumented, non-standard methods. See the
+        documentation for the MySQL C API for some hints on what they do.
+        """
+        from MySQLdb.constants import CLIENT, FIELD_TYPE
+        from MySQLdb.converters import conversions, _bytes_or_str
+
+        kwargs2 = kwargs.copy()
+
+        if "db" in kwargs2:
+            kwargs2["database"] = kwargs2.pop("db")
+        if "passwd" in kwargs2:
+            kwargs2["password"] = kwargs2.pop("passwd")
+
+        if "conv" in kwargs:
+            conv = kwargs["conv"]
+        else:
+            conv = conversions
+
+        conv2 = {}
+        for k, v in conv.items():
+            if isinstance(k, int) and isinstance(v, list):
+                conv2[k] = v[:]
+            else:
+                conv2[k] = v
+        kwargs2["conv"] = conv2
+
+        cursorclass = kwargs2.pop("cursorclass", self.default_cursor)
+        charset = kwargs2.get("charset", "")
+        collation = kwargs2.pop("collation", "")
+        use_unicode = kwargs2.pop("use_unicode", True)
+        sql_mode = kwargs2.pop("sql_mode", "")
+        self._binary_prefix = kwargs2.pop("binary_prefix", False)
+
+        client_flag = kwargs.get("client_flag", 0)
+        client_flag |= CLIENT.MULTI_RESULTS
+        multi_statements = kwargs2.pop("multi_statements", True)
+        if multi_statements:
+            client_flag |= CLIENT.MULTI_STATEMENTS
+        kwargs2["client_flag"] = client_flag
+
+        # PEP-249 requires autocommit to be initially off
+        autocommit = kwargs2.pop("autocommit", False)
+
+        super().__init__(*args, **kwargs2)
+        self.cursorclass = cursorclass
+        self.encoders = {k: v for k, v in conv.items() if type(k) is not int}
+
+        self._server_version = tuple(
+            [numeric_part(n) for n in self.get_server_info().split(".")[:2]]
+        )
+
+        self.encoding = "ascii"  # overridden in set_character_set()
+
+        if not charset:
+            charset = self.character_set_name()
+        self.set_character_set(charset, collation)
+
+        if sql_mode:
+            self.set_sql_mode(sql_mode)
+
+        if use_unicode:
+            for t in (
+                FIELD_TYPE.STRING,
+                FIELD_TYPE.VAR_STRING,
+                FIELD_TYPE.VARCHAR,
+                FIELD_TYPE.TINY_BLOB,
+                FIELD_TYPE.MEDIUM_BLOB,
+                FIELD_TYPE.LONG_BLOB,
+                FIELD_TYPE.BLOB,
+            ):
+                self.converter[t] = _bytes_or_str
+            # Unlike other string/blob types, JSON is always text.
+            # MySQL may return JSON with charset==binary.
+            self.converter[FIELD_TYPE.JSON] = str
+
+        self._transactional = self.server_capabilities & CLIENT.TRANSACTIONS
+        if self._transactional:
+            if autocommit is not None:
+                self.autocommit(autocommit)
+        self.messages = []
+
+    def __enter__(self):
+        return self
+
+    def __exit__(self, exc_type, exc_value, traceback):
+        self.close()
+
+    def autocommit(self, on):
+        on = bool(on)
+        if self.get_autocommit() != on:
+            _mysql.connection.autocommit(self, on)
+
+    def cursor(self, cursorclass=None):
+        """
+        Create a cursor on which queries may be performed. The
+        optional cursorclass parameter is used to create the
+        Cursor. By default, self.cursorclass=cursors.Cursor is
+        used.
+        """
+        return (cursorclass or self.cursorclass)(self)
+
+    def query(self, query):
+        # Since _mysql releases GIL while querying, we need immutable buffer.
+        if isinstance(query, bytearray):
+            query = bytes(query)
+        _mysql.connection.query(self, query)
+
+    def _bytes_literal(self, bs):
+        assert isinstance(bs, (bytes, bytearray))
+        x = self.string_literal(bs)  # x is escaped and quoted bytes
+        if self._binary_prefix:
+            return b"_binary" + x
+        return x
+
+    def _tuple_literal(self, t):
+        return b"(%s)" % (b",".join(map(self.literal, t)))
+
+    def literal(self, o):
+        """If o is a single object, returns an SQL literal as a string.
+        If o is a non-string sequence, the items of the sequence are
+        converted and returned as a sequence.
+
+        Non-standard. For internal use; do not use this in your
+        applications.
+        """
+        if isinstance(o, str):
+            s = self.string_literal(o.encode(self.encoding))
+        elif isinstance(o, bytearray):
+            s = self._bytes_literal(o)
+        elif isinstance(o, bytes):
+            s = self._bytes_literal(o)
+        elif isinstance(o, (tuple, list)):
+            s = self._tuple_literal(o)
+        else:
+            s = self.escape(o, self.encoders)
+            if isinstance(s, str):
+                s = s.encode(self.encoding)
+        assert isinstance(s, bytes)
+        return s
+
+    def begin(self):
+        """Explicitly begin a connection.
+
+        This method is not used when autocommit=False (default).
+        """
+        self.query(b"BEGIN")
+
+    def set_character_set(self, charset, collation=None):
+        """Set the connection character set to charset."""
+        super().set_character_set(charset)
+        self.encoding = _charset_to_encoding.get(charset, charset)
+        if collation:
+            self.query(f"SET NAMES {charset} COLLATE {collation}")
+            self.store_result()
+
+    def set_sql_mode(self, sql_mode):
+        """Set the connection sql_mode. See MySQL documentation for
+        legal values."""
+        if self._server_version < (4, 1):
+            raise NotSupportedError("server is too old to set sql_mode")
+        self.query("SET SESSION sql_mode='%s'" % sql_mode)
+        self.store_result()
+
+    def show_warnings(self):
+        """Return detailed information about warnings as a
+        sequence of tuples of (Level, Code, Message). This
+        is only supported in MySQL-4.1 and up. If your server
+        is an earlier version, an empty sequence is returned."""
+        if self._server_version < (4, 1):
+            return ()
+        self.query("SHOW WARNINGS")
+        r = self.store_result()
+        warnings = r.fetch_row(0)
+        return warnings
+
+    Warning = Warning
+    Error = Error
+    InterfaceError = InterfaceError
+    DatabaseError = DatabaseError
+    DataError = DataError
+    OperationalError = OperationalError
+    IntegrityError = IntegrityError
+    InternalError = InternalError
+    ProgrammingError = ProgrammingError
+    NotSupportedError = NotSupportedError
+
+
+# vim: colorcolumn=100
```

### Comparing `mysqlclient-2.2.0/src/MySQLdb/constants/CR.py` & `mysqlclient-2.2.0rc1/src/MySQLdb/constants/CR.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,105 +1,105 @@
-"""MySQL Connection Errors
-
-Nearly all of these raise OperationalError. COMMANDS_OUT_OF_SYNC
-raises ProgrammingError.
-
-"""
-
-if __name__ == "__main__":
-    """
-    Usage: python CR.py [/path/to/mysql/errmsg.h ...] >> CR.py
-    """
-    import fileinput
-    import re
-
-    data = {}
-    error_last = None
-    for line in fileinput.input():
-        line = re.sub(r"/\*.*?\*/", "", line)
-        m = re.match(r"^\s*#define\s+CR_([A-Z0-9_]+)\s+(\d+)(\s.*|$)", line)
-        if m:
-            name = m.group(1)
-            value = int(m.group(2))
-            if name == "ERROR_LAST":
-                if error_last is None or error_last < value:
-                    error_last = value
-                continue
-            if value not in data:
-                data[value] = set()
-            data[value].add(name)
-    for value, names in sorted(data.items()):
-        for name in sorted(names):
-            print(f"{name} = {value}")
-    if error_last is not None:
-        print("ERROR_LAST = %s" % error_last)
-
-
-ERROR_FIRST = 2000
-MIN_ERROR = 2000
-UNKNOWN_ERROR = 2000
-SOCKET_CREATE_ERROR = 2001
-CONNECTION_ERROR = 2002
-CONN_HOST_ERROR = 2003
-IPSOCK_ERROR = 2004
-UNKNOWN_HOST = 2005
-SERVER_GONE_ERROR = 2006
-VERSION_ERROR = 2007
-OUT_OF_MEMORY = 2008
-WRONG_HOST_INFO = 2009
-LOCALHOST_CONNECTION = 2010
-TCP_CONNECTION = 2011
-SERVER_HANDSHAKE_ERR = 2012
-SERVER_LOST = 2013
-COMMANDS_OUT_OF_SYNC = 2014
-NAMEDPIPE_CONNECTION = 2015
-NAMEDPIPEWAIT_ERROR = 2016
-NAMEDPIPEOPEN_ERROR = 2017
-NAMEDPIPESETSTATE_ERROR = 2018
-CANT_READ_CHARSET = 2019
-NET_PACKET_TOO_LARGE = 2020
-EMBEDDED_CONNECTION = 2021
-PROBE_SLAVE_STATUS = 2022
-PROBE_SLAVE_HOSTS = 2023
-PROBE_SLAVE_CONNECT = 2024
-PROBE_MASTER_CONNECT = 2025
-SSL_CONNECTION_ERROR = 2026
-MALFORMED_PACKET = 2027
-WRONG_LICENSE = 2028
-NULL_POINTER = 2029
-NO_PREPARE_STMT = 2030
-PARAMS_NOT_BOUND = 2031
-DATA_TRUNCATED = 2032
-NO_PARAMETERS_EXISTS = 2033
-INVALID_PARAMETER_NO = 2034
-INVALID_BUFFER_USE = 2035
-UNSUPPORTED_PARAM_TYPE = 2036
-SHARED_MEMORY_CONNECTION = 2037
-SHARED_MEMORY_CONNECT_REQUEST_ERROR = 2038
-SHARED_MEMORY_CONNECT_ANSWER_ERROR = 2039
-SHARED_MEMORY_CONNECT_FILE_MAP_ERROR = 2040
-SHARED_MEMORY_CONNECT_MAP_ERROR = 2041
-SHARED_MEMORY_FILE_MAP_ERROR = 2042
-SHARED_MEMORY_MAP_ERROR = 2043
-SHARED_MEMORY_EVENT_ERROR = 2044
-SHARED_MEMORY_CONNECT_ABANDONED_ERROR = 2045
-SHARED_MEMORY_CONNECT_SET_ERROR = 2046
-CONN_UNKNOW_PROTOCOL = 2047
-INVALID_CONN_HANDLE = 2048
-UNUSED_1 = 2049
-FETCH_CANCELED = 2050
-NO_DATA = 2051
-NO_STMT_METADATA = 2052
-NO_RESULT_SET = 2053
-NOT_IMPLEMENTED = 2054
-SERVER_LOST_EXTENDED = 2055
-STMT_CLOSED = 2056
-NEW_STMT_METADATA = 2057
-ALREADY_CONNECTED = 2058
-AUTH_PLUGIN_CANNOT_LOAD = 2059
-DUPLICATE_CONNECTION_ATTR = 2060
-AUTH_PLUGIN_ERR = 2061
-INSECURE_API_ERR = 2062
-FILE_NAME_TOO_LONG = 2063
-SSL_FIPS_MODE_ERR = 2064
-MAX_ERROR = 2999
-ERROR_LAST = 2064
+"""MySQL Connection Errors
+
+Nearly all of these raise OperationalError. COMMANDS_OUT_OF_SYNC
+raises ProgrammingError.
+
+"""
+
+if __name__ == "__main__":
+    """
+    Usage: python CR.py [/path/to/mysql/errmsg.h ...] >> CR.py
+    """
+    import fileinput
+    import re
+
+    data = {}
+    error_last = None
+    for line in fileinput.input():
+        line = re.sub(r"/\*.*?\*/", "", line)
+        m = re.match(r"^\s*#define\s+CR_([A-Z0-9_]+)\s+(\d+)(\s.*|$)", line)
+        if m:
+            name = m.group(1)
+            value = int(m.group(2))
+            if name == "ERROR_LAST":
+                if error_last is None or error_last < value:
+                    error_last = value
+                continue
+            if value not in data:
+                data[value] = set()
+            data[value].add(name)
+    for value, names in sorted(data.items()):
+        for name in sorted(names):
+            print(f"{name} = {value}")
+    if error_last is not None:
+        print("ERROR_LAST = %s" % error_last)
+
+
+ERROR_FIRST = 2000
+MIN_ERROR = 2000
+UNKNOWN_ERROR = 2000
+SOCKET_CREATE_ERROR = 2001
+CONNECTION_ERROR = 2002
+CONN_HOST_ERROR = 2003
+IPSOCK_ERROR = 2004
+UNKNOWN_HOST = 2005
+SERVER_GONE_ERROR = 2006
+VERSION_ERROR = 2007
+OUT_OF_MEMORY = 2008
+WRONG_HOST_INFO = 2009
+LOCALHOST_CONNECTION = 2010
+TCP_CONNECTION = 2011
+SERVER_HANDSHAKE_ERR = 2012
+SERVER_LOST = 2013
+COMMANDS_OUT_OF_SYNC = 2014
+NAMEDPIPE_CONNECTION = 2015
+NAMEDPIPEWAIT_ERROR = 2016
+NAMEDPIPEOPEN_ERROR = 2017
+NAMEDPIPESETSTATE_ERROR = 2018
+CANT_READ_CHARSET = 2019
+NET_PACKET_TOO_LARGE = 2020
+EMBEDDED_CONNECTION = 2021
+PROBE_SLAVE_STATUS = 2022
+PROBE_SLAVE_HOSTS = 2023
+PROBE_SLAVE_CONNECT = 2024
+PROBE_MASTER_CONNECT = 2025
+SSL_CONNECTION_ERROR = 2026
+MALFORMED_PACKET = 2027
+WRONG_LICENSE = 2028
+NULL_POINTER = 2029
+NO_PREPARE_STMT = 2030
+PARAMS_NOT_BOUND = 2031
+DATA_TRUNCATED = 2032
+NO_PARAMETERS_EXISTS = 2033
+INVALID_PARAMETER_NO = 2034
+INVALID_BUFFER_USE = 2035
+UNSUPPORTED_PARAM_TYPE = 2036
+SHARED_MEMORY_CONNECTION = 2037
+SHARED_MEMORY_CONNECT_REQUEST_ERROR = 2038
+SHARED_MEMORY_CONNECT_ANSWER_ERROR = 2039
+SHARED_MEMORY_CONNECT_FILE_MAP_ERROR = 2040
+SHARED_MEMORY_CONNECT_MAP_ERROR = 2041
+SHARED_MEMORY_FILE_MAP_ERROR = 2042
+SHARED_MEMORY_MAP_ERROR = 2043
+SHARED_MEMORY_EVENT_ERROR = 2044
+SHARED_MEMORY_CONNECT_ABANDONED_ERROR = 2045
+SHARED_MEMORY_CONNECT_SET_ERROR = 2046
+CONN_UNKNOW_PROTOCOL = 2047
+INVALID_CONN_HANDLE = 2048
+UNUSED_1 = 2049
+FETCH_CANCELED = 2050
+NO_DATA = 2051
+NO_STMT_METADATA = 2052
+NO_RESULT_SET = 2053
+NOT_IMPLEMENTED = 2054
+SERVER_LOST_EXTENDED = 2055
+STMT_CLOSED = 2056
+NEW_STMT_METADATA = 2057
+ALREADY_CONNECTED = 2058
+AUTH_PLUGIN_CANNOT_LOAD = 2059
+DUPLICATE_CONNECTION_ATTR = 2060
+AUTH_PLUGIN_ERR = 2061
+INSECURE_API_ERR = 2062
+FILE_NAME_TOO_LONG = 2063
+SSL_FIPS_MODE_ERR = 2064
+MAX_ERROR = 2999
+ERROR_LAST = 2064
```

### Comparing `mysqlclient-2.2.0/src/MySQLdb/constants/ER.py` & `mysqlclient-2.2.0rc1/src/MySQLdb/constants/ER.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,827 +1,827 @@
-"""MySQL ER Constants
-
-These constants are error codes for the bulk of the error conditions
-that may occur.
-"""
-
-if __name__ == "__main__":
-    """
-    Usage: python ER.py [/path/to/mysql/mysqld_error.h ...] >> ER.py
-    """
-    import fileinput
-    import re
-
-    data = {}
-    error_last = None
-    for line in fileinput.input():
-        line = re.sub(r"/\*.*?\*/", "", line)
-        m = re.match(r"^\s*#define\s+((ER|WARN)_[A-Z0-9_]+)\s+(\d+)\s*", line)
-        if m:
-            name = m.group(1)
-            if name.startswith("ER_"):
-                name = name[3:]
-            value = int(m.group(3))
-            if name == "ERROR_LAST":
-                if error_last is None or error_last < value:
-                    error_last = value
-                continue
-            if value not in data:
-                data[value] = set()
-            data[value].add(name)
-    for value, names in sorted(data.items()):
-        for name in sorted(names):
-            print(f"{name} = {value}")
-    if error_last is not None:
-        print("ERROR_LAST = %s" % error_last)
-
-
-ERROR_FIRST = 1000
-NO = 1002
-YES = 1003
-CANT_CREATE_FILE = 1004
-CANT_CREATE_TABLE = 1005
-CANT_CREATE_DB = 1006
-DB_CREATE_EXISTS = 1007
-DB_DROP_EXISTS = 1008
-DB_DROP_RMDIR = 1010
-CANT_FIND_SYSTEM_REC = 1012
-CANT_GET_STAT = 1013
-CANT_LOCK = 1015
-CANT_OPEN_FILE = 1016
-FILE_NOT_FOUND = 1017
-CANT_READ_DIR = 1018
-CHECKREAD = 1020
-DUP_KEY = 1022
-ERROR_ON_READ = 1024
-ERROR_ON_RENAME = 1025
-ERROR_ON_WRITE = 1026
-FILE_USED = 1027
-FILSORT_ABORT = 1028
-GET_ERRNO = 1030
-ILLEGAL_HA = 1031
-KEY_NOT_FOUND = 1032
-NOT_FORM_FILE = 1033
-NOT_KEYFILE = 1034
-OLD_KEYFILE = 1035
-OPEN_AS_READONLY = 1036
-OUTOFMEMORY = 1037
-OUT_OF_SORTMEMORY = 1038
-CON_COUNT_ERROR = 1040
-OUT_OF_RESOURCES = 1041
-BAD_HOST_ERROR = 1042
-HANDSHAKE_ERROR = 1043
-DBACCESS_DENIED_ERROR = 1044
-ACCESS_DENIED_ERROR = 1045
-NO_DB_ERROR = 1046
-UNKNOWN_COM_ERROR = 1047
-BAD_NULL_ERROR = 1048
-BAD_DB_ERROR = 1049
-TABLE_EXISTS_ERROR = 1050
-BAD_TABLE_ERROR = 1051
-NON_UNIQ_ERROR = 1052
-SERVER_SHUTDOWN = 1053
-BAD_FIELD_ERROR = 1054
-WRONG_FIELD_WITH_GROUP = 1055
-WRONG_GROUP_FIELD = 1056
-WRONG_SUM_SELECT = 1057
-WRONG_VALUE_COUNT = 1058
-TOO_LONG_IDENT = 1059
-DUP_FIELDNAME = 1060
-DUP_KEYNAME = 1061
-DUP_ENTRY = 1062
-WRONG_FIELD_SPEC = 1063
-PARSE_ERROR = 1064
-EMPTY_QUERY = 1065
-NONUNIQ_TABLE = 1066
-INVALID_DEFAULT = 1067
-MULTIPLE_PRI_KEY = 1068
-TOO_MANY_KEYS = 1069
-TOO_MANY_KEY_PARTS = 1070
-TOO_LONG_KEY = 1071
-KEY_COLUMN_DOES_NOT_EXITS = 1072
-BLOB_USED_AS_KEY = 1073
-TOO_BIG_FIELDLENGTH = 1074
-WRONG_AUTO_KEY = 1075
-READY = 1076
-SHUTDOWN_COMPLETE = 1079
-FORCING_CLOSE = 1080
-IPSOCK_ERROR = 1081
-NO_SUCH_INDEX = 1082
-WRONG_FIELD_TERMINATORS = 1083
-BLOBS_AND_NO_TERMINATED = 1084
-TEXTFILE_NOT_READABLE = 1085
-FILE_EXISTS_ERROR = 1086
-LOAD_INFO = 1087
-ALTER_INFO = 1088
-WRONG_SUB_KEY = 1089
-CANT_REMOVE_ALL_FIELDS = 1090
-CANT_DROP_FIELD_OR_KEY = 1091
-INSERT_INFO = 1092
-UPDATE_TABLE_USED = 1093
-NO_SUCH_THREAD = 1094
-KILL_DENIED_ERROR = 1095
-NO_TABLES_USED = 1096
-TOO_BIG_SET = 1097
-NO_UNIQUE_LOGFILE = 1098
-TABLE_NOT_LOCKED_FOR_WRITE = 1099
-TABLE_NOT_LOCKED = 1100
-BLOB_CANT_HAVE_DEFAULT = 1101
-WRONG_DB_NAME = 1102
-WRONG_TABLE_NAME = 1103
-TOO_BIG_SELECT = 1104
-UNKNOWN_ERROR = 1105
-UNKNOWN_PROCEDURE = 1106
-WRONG_PARAMCOUNT_TO_PROCEDURE = 1107
-WRONG_PARAMETERS_TO_PROCEDURE = 1108
-UNKNOWN_TABLE = 1109
-FIELD_SPECIFIED_TWICE = 1110
-INVALID_GROUP_FUNC_USE = 1111
-UNSUPPORTED_EXTENSION = 1112
-TABLE_MUST_HAVE_COLUMNS = 1113
-RECORD_FILE_FULL = 1114
-UNKNOWN_CHARACTER_SET = 1115
-TOO_MANY_TABLES = 1116
-TOO_MANY_FIELDS = 1117
-TOO_BIG_ROWSIZE = 1118
-STACK_OVERRUN = 1119
-WRONG_OUTER_JOIN_UNUSED = 1120
-NULL_COLUMN_IN_INDEX = 1121
-CANT_FIND_UDF = 1122
-CANT_INITIALIZE_UDF = 1123
-UDF_NO_PATHS = 1124
-UDF_EXISTS = 1125
-CANT_OPEN_LIBRARY = 1126
-CANT_FIND_DL_ENTRY = 1127
-FUNCTION_NOT_DEFINED = 1128
-HOST_IS_BLOCKED = 1129
-HOST_NOT_PRIVILEGED = 1130
-PASSWORD_ANONYMOUS_USER = 1131
-PASSWORD_NOT_ALLOWED = 1132
-PASSWORD_NO_MATCH = 1133
-UPDATE_INFO = 1134
-CANT_CREATE_THREAD = 1135
-WRONG_VALUE_COUNT_ON_ROW = 1136
-CANT_REOPEN_TABLE = 1137
-INVALID_USE_OF_NULL = 1138
-REGEXP_ERROR = 1139
-MIX_OF_GROUP_FUNC_AND_FIELDS = 1140
-NONEXISTING_GRANT = 1141
-TABLEACCESS_DENIED_ERROR = 1142
-COLUMNACCESS_DENIED_ERROR = 1143
-ILLEGAL_GRANT_FOR_TABLE = 1144
-GRANT_WRONG_HOST_OR_USER = 1145
-NO_SUCH_TABLE = 1146
-NONEXISTING_TABLE_GRANT = 1147
-NOT_ALLOWED_COMMAND = 1148
-SYNTAX_ERROR = 1149
-ABORTING_CONNECTION = 1152
-NET_PACKET_TOO_LARGE = 1153
-NET_READ_ERROR_FROM_PIPE = 1154
-NET_FCNTL_ERROR = 1155
-NET_PACKETS_OUT_OF_ORDER = 1156
-NET_UNCOMPRESS_ERROR = 1157
-NET_READ_ERROR = 1158
-NET_READ_INTERRUPTED = 1159
-NET_ERROR_ON_WRITE = 1160
-NET_WRITE_INTERRUPTED = 1161
-TOO_LONG_STRING = 1162
-TABLE_CANT_HANDLE_BLOB = 1163
-TABLE_CANT_HANDLE_AUTO_INCREMENT = 1164
-WRONG_COLUMN_NAME = 1166
-WRONG_KEY_COLUMN = 1167
-WRONG_MRG_TABLE = 1168
-DUP_UNIQUE = 1169
-BLOB_KEY_WITHOUT_LENGTH = 1170
-PRIMARY_CANT_HAVE_NULL = 1171
-TOO_MANY_ROWS = 1172
-REQUIRES_PRIMARY_KEY = 1173
-UPDATE_WITHOUT_KEY_IN_SAFE_MODE = 1175
-KEY_DOES_NOT_EXITS = 1176
-CHECK_NO_SUCH_TABLE = 1177
-CHECK_NOT_IMPLEMENTED = 1178
-CANT_DO_THIS_DURING_AN_TRANSACTION = 1179
-ERROR_DURING_COMMIT = 1180
-ERROR_DURING_ROLLBACK = 1181
-ERROR_DURING_FLUSH_LOGS = 1182
-NEW_ABORTING_CONNECTION = 1184
-MASTER = 1188
-MASTER_NET_READ = 1189
-MASTER_NET_WRITE = 1190
-FT_MATCHING_KEY_NOT_FOUND = 1191
-LOCK_OR_ACTIVE_TRANSACTION = 1192
-UNKNOWN_SYSTEM_VARIABLE = 1193
-CRASHED_ON_USAGE = 1194
-CRASHED_ON_REPAIR = 1195
-WARNING_NOT_COMPLETE_ROLLBACK = 1196
-TRANS_CACHE_FULL = 1197
-SLAVE_NOT_RUNNING = 1199
-BAD_SLAVE = 1200
-MASTER_INFO = 1201
-SLAVE_THREAD = 1202
-TOO_MANY_USER_CONNECTIONS = 1203
-SET_CONSTANTS_ONLY = 1204
-LOCK_WAIT_TIMEOUT = 1205
-LOCK_TABLE_FULL = 1206
-READ_ONLY_TRANSACTION = 1207
-WRONG_ARGUMENTS = 1210
-NO_PERMISSION_TO_CREATE_USER = 1211
-LOCK_DEADLOCK = 1213
-TABLE_CANT_HANDLE_FT = 1214
-CANNOT_ADD_FOREIGN = 1215
-NO_REFERENCED_ROW = 1216
-ROW_IS_REFERENCED = 1217
-CONNECT_TO_MASTER = 1218
-ERROR_WHEN_EXECUTING_COMMAND = 1220
-WRONG_USAGE = 1221
-WRONG_NUMBER_OF_COLUMNS_IN_SELECT = 1222
-CANT_UPDATE_WITH_READLOCK = 1223
-MIXING_NOT_ALLOWED = 1224
-DUP_ARGUMENT = 1225
-USER_LIMIT_REACHED = 1226
-SPECIFIC_ACCESS_DENIED_ERROR = 1227
-LOCAL_VARIABLE = 1228
-GLOBAL_VARIABLE = 1229
-NO_DEFAULT = 1230
-WRONG_VALUE_FOR_VAR = 1231
-WRONG_TYPE_FOR_VAR = 1232
-VAR_CANT_BE_READ = 1233
-CANT_USE_OPTION_HERE = 1234
-NOT_SUPPORTED_YET = 1235
-MASTER_FATAL_ERROR_READING_BINLOG = 1236
-SLAVE_IGNORED_TABLE = 1237
-INCORRECT_GLOBAL_LOCAL_VAR = 1238
-WRONG_FK_DEF = 1239
-KEY_REF_DO_NOT_MATCH_TABLE_REF = 1240
-OPERAND_COLUMNS = 1241
-SUBQUERY_NO_1_ROW = 1242
-UNKNOWN_STMT_HANDLER = 1243
-CORRUPT_HELP_DB = 1244
-AUTO_CONVERT = 1246
-ILLEGAL_REFERENCE = 1247
-DERIVED_MUST_HAVE_ALIAS = 1248
-SELECT_REDUCED = 1249
-TABLENAME_NOT_ALLOWED_HERE = 1250
-NOT_SUPPORTED_AUTH_MODE = 1251
-SPATIAL_CANT_HAVE_NULL = 1252
-COLLATION_CHARSET_MISMATCH = 1253
-TOO_BIG_FOR_UNCOMPRESS = 1256
-ZLIB_Z_MEM_ERROR = 1257
-ZLIB_Z_BUF_ERROR = 1258
-ZLIB_Z_DATA_ERROR = 1259
-CUT_VALUE_GROUP_CONCAT = 1260
-WARN_TOO_FEW_RECORDS = 1261
-WARN_TOO_MANY_RECORDS = 1262
-WARN_NULL_TO_NOTNULL = 1263
-WARN_DATA_OUT_OF_RANGE = 1264
-WARN_DATA_TRUNCATED = 1265
-WARN_USING_OTHER_HANDLER = 1266
-CANT_AGGREGATE_2COLLATIONS = 1267
-REVOKE_GRANTS = 1269
-CANT_AGGREGATE_3COLLATIONS = 1270
-CANT_AGGREGATE_NCOLLATIONS = 1271
-VARIABLE_IS_NOT_STRUCT = 1272
-UNKNOWN_COLLATION = 1273
-SLAVE_IGNORED_SSL_PARAMS = 1274
-SERVER_IS_IN_SECURE_AUTH_MODE = 1275
-WARN_FIELD_RESOLVED = 1276
-BAD_SLAVE_UNTIL_COND = 1277
-MISSING_SKIP_SLAVE = 1278
-UNTIL_COND_IGNORED = 1279
-WRONG_NAME_FOR_INDEX = 1280
-WRONG_NAME_FOR_CATALOG = 1281
-BAD_FT_COLUMN = 1283
-UNKNOWN_KEY_CACHE = 1284
-WARN_HOSTNAME_WONT_WORK = 1285
-UNKNOWN_STORAGE_ENGINE = 1286
-WARN_DEPRECATED_SYNTAX = 1287
-NON_UPDATABLE_TABLE = 1288
-FEATURE_DISABLED = 1289
-OPTION_PREVENTS_STATEMENT = 1290
-DUPLICATED_VALUE_IN_TYPE = 1291
-TRUNCATED_WRONG_VALUE = 1292
-INVALID_ON_UPDATE = 1294
-UNSUPPORTED_PS = 1295
-GET_ERRMSG = 1296
-GET_TEMPORARY_ERRMSG = 1297
-UNKNOWN_TIME_ZONE = 1298
-WARN_INVALID_TIMESTAMP = 1299
-INVALID_CHARACTER_STRING = 1300
-WARN_ALLOWED_PACKET_OVERFLOWED = 1301
-CONFLICTING_DECLARATIONS = 1302
-SP_NO_RECURSIVE_CREATE = 1303
-SP_ALREADY_EXISTS = 1304
-SP_DOES_NOT_EXIST = 1305
-SP_DROP_FAILED = 1306
-SP_STORE_FAILED = 1307
-SP_LILABEL_MISMATCH = 1308
-SP_LABEL_REDEFINE = 1309
-SP_LABEL_MISMATCH = 1310
-SP_UNINIT_VAR = 1311
-SP_BADSELECT = 1312
-SP_BADRETURN = 1313
-SP_BADSTATEMENT = 1314
-UPDATE_LOG_DEPRECATED_IGNORED = 1315
-UPDATE_LOG_DEPRECATED_TRANSLATED = 1316
-QUERY_INTERRUPTED = 1317
-SP_WRONG_NO_OF_ARGS = 1318
-SP_COND_MISMATCH = 1319
-SP_NORETURN = 1320
-SP_NORETURNEND = 1321
-SP_BAD_CURSOR_QUERY = 1322
-SP_BAD_CURSOR_SELECT = 1323
-SP_CURSOR_MISMATCH = 1324
-SP_CURSOR_ALREADY_OPEN = 1325
-SP_CURSOR_NOT_OPEN = 1326
-SP_UNDECLARED_VAR = 1327
-SP_WRONG_NO_OF_FETCH_ARGS = 1328
-SP_FETCH_NO_DATA = 1329
-SP_DUP_PARAM = 1330
-SP_DUP_VAR = 1331
-SP_DUP_COND = 1332
-SP_DUP_CURS = 1333
-SP_CANT_ALTER = 1334
-SP_SUBSELECT_NYI = 1335
-STMT_NOT_ALLOWED_IN_SF_OR_TRG = 1336
-SP_VARCOND_AFTER_CURSHNDLR = 1337
-SP_CURSOR_AFTER_HANDLER = 1338
-SP_CASE_NOT_FOUND = 1339
-FPARSER_TOO_BIG_FILE = 1340
-FPARSER_BAD_HEADER = 1341
-FPARSER_EOF_IN_COMMENT = 1342
-FPARSER_ERROR_IN_PARAMETER = 1343
-FPARSER_EOF_IN_UNKNOWN_PARAMETER = 1344
-VIEW_NO_EXPLAIN = 1345
-WRONG_OBJECT = 1347
-NONUPDATEABLE_COLUMN = 1348
-VIEW_SELECT_CLAUSE = 1350
-VIEW_SELECT_VARIABLE = 1351
-VIEW_SELECT_TMPTABLE = 1352
-VIEW_WRONG_LIST = 1353
-WARN_VIEW_MERGE = 1354
-WARN_VIEW_WITHOUT_KEY = 1355
-VIEW_INVALID = 1356
-SP_NO_DROP_SP = 1357
-TRG_ALREADY_EXISTS = 1359
-TRG_DOES_NOT_EXIST = 1360
-TRG_ON_VIEW_OR_TEMP_TABLE = 1361
-TRG_CANT_CHANGE_ROW = 1362
-TRG_NO_SUCH_ROW_IN_TRG = 1363
-NO_DEFAULT_FOR_FIELD = 1364
-DIVISION_BY_ZERO = 1365
-TRUNCATED_WRONG_VALUE_FOR_FIELD = 1366
-ILLEGAL_VALUE_FOR_TYPE = 1367
-VIEW_NONUPD_CHECK = 1368
-VIEW_CHECK_FAILED = 1369
-PROCACCESS_DENIED_ERROR = 1370
-RELAY_LOG_FAIL = 1371
-UNKNOWN_TARGET_BINLOG = 1373
-IO_ERR_LOG_INDEX_READ = 1374
-BINLOG_PURGE_PROHIBITED = 1375
-FSEEK_FAIL = 1376
-BINLOG_PURGE_FATAL_ERR = 1377
-LOG_IN_USE = 1378
-LOG_PURGE_UNKNOWN_ERR = 1379
-RELAY_LOG_INIT = 1380
-NO_BINARY_LOGGING = 1381
-RESERVED_SYNTAX = 1382
-PS_MANY_PARAM = 1390
-KEY_PART_0 = 1391
-VIEW_CHECKSUM = 1392
-VIEW_MULTIUPDATE = 1393
-VIEW_NO_INSERT_FIELD_LIST = 1394
-VIEW_DELETE_MERGE_VIEW = 1395
-CANNOT_USER = 1396
-XAER_NOTA = 1397
-XAER_INVAL = 1398
-XAER_RMFAIL = 1399
-XAER_OUTSIDE = 1400
-XAER_RMERR = 1401
-XA_RBROLLBACK = 1402
-NONEXISTING_PROC_GRANT = 1403
-PROC_AUTO_GRANT_FAIL = 1404
-PROC_AUTO_REVOKE_FAIL = 1405
-DATA_TOO_LONG = 1406
-SP_BAD_SQLSTATE = 1407
-STARTUP = 1408
-LOAD_FROM_FIXED_SIZE_ROWS_TO_VAR = 1409
-CANT_CREATE_USER_WITH_GRANT = 1410
-WRONG_VALUE_FOR_TYPE = 1411
-TABLE_DEF_CHANGED = 1412
-SP_DUP_HANDLER = 1413
-SP_NOT_VAR_ARG = 1414
-SP_NO_RETSET = 1415
-CANT_CREATE_GEOMETRY_OBJECT = 1416
-BINLOG_UNSAFE_ROUTINE = 1418
-BINLOG_CREATE_ROUTINE_NEED_SUPER = 1419
-STMT_HAS_NO_OPEN_CURSOR = 1421
-COMMIT_NOT_ALLOWED_IN_SF_OR_TRG = 1422
-NO_DEFAULT_FOR_VIEW_FIELD = 1423
-SP_NO_RECURSION = 1424
-TOO_BIG_SCALE = 1425
-TOO_BIG_PRECISION = 1426
-M_BIGGER_THAN_D = 1427
-WRONG_LOCK_OF_SYSTEM_TABLE = 1428
-CONNECT_TO_FOREIGN_DATA_SOURCE = 1429
-QUERY_ON_FOREIGN_DATA_SOURCE = 1430
-FOREIGN_DATA_SOURCE_DOESNT_EXIST = 1431
-FOREIGN_DATA_STRING_INVALID_CANT_CREATE = 1432
-FOREIGN_DATA_STRING_INVALID = 1433
-TRG_IN_WRONG_SCHEMA = 1435
-STACK_OVERRUN_NEED_MORE = 1436
-TOO_LONG_BODY = 1437
-WARN_CANT_DROP_DEFAULT_KEYCACHE = 1438
-TOO_BIG_DISPLAYWIDTH = 1439
-XAER_DUPID = 1440
-DATETIME_FUNCTION_OVERFLOW = 1441
-CANT_UPDATE_USED_TABLE_IN_SF_OR_TRG = 1442
-VIEW_PREVENT_UPDATE = 1443
-PS_NO_RECURSION = 1444
-SP_CANT_SET_AUTOCOMMIT = 1445
-VIEW_FRM_NO_USER = 1447
-VIEW_OTHER_USER = 1448
-NO_SUCH_USER = 1449
-FORBID_SCHEMA_CHANGE = 1450
-ROW_IS_REFERENCED_2 = 1451
-NO_REFERENCED_ROW_2 = 1452
-SP_BAD_VAR_SHADOW = 1453
-TRG_NO_DEFINER = 1454
-OLD_FILE_FORMAT = 1455
-SP_RECURSION_LIMIT = 1456
-SP_WRONG_NAME = 1458
-TABLE_NEEDS_UPGRADE = 1459
-SP_NO_AGGREGATE = 1460
-MAX_PREPARED_STMT_COUNT_REACHED = 1461
-VIEW_RECURSIVE = 1462
-NON_GROUPING_FIELD_USED = 1463
-TABLE_CANT_HANDLE_SPKEYS = 1464
-NO_TRIGGERS_ON_SYSTEM_SCHEMA = 1465
-REMOVED_SPACES = 1466
-AUTOINC_READ_FAILED = 1467
-USERNAME = 1468
-HOSTNAME = 1469
-WRONG_STRING_LENGTH = 1470
-NON_INSERTABLE_TABLE = 1471
-ADMIN_WRONG_MRG_TABLE = 1472
-TOO_HIGH_LEVEL_OF_NESTING_FOR_SELECT = 1473
-NAME_BECOMES_EMPTY = 1474
-AMBIGUOUS_FIELD_TERM = 1475
-FOREIGN_SERVER_EXISTS = 1476
-FOREIGN_SERVER_DOESNT_EXIST = 1477
-ILLEGAL_HA_CREATE_OPTION = 1478
-PARTITION_REQUIRES_VALUES_ERROR = 1479
-PARTITION_WRONG_VALUES_ERROR = 1480
-PARTITION_MAXVALUE_ERROR = 1481
-PARTITION_WRONG_NO_PART_ERROR = 1484
-PARTITION_WRONG_NO_SUBPART_ERROR = 1485
-WRONG_EXPR_IN_PARTITION_FUNC_ERROR = 1486
-FIELD_NOT_FOUND_PART_ERROR = 1488
-INCONSISTENT_PARTITION_INFO_ERROR = 1490
-PARTITION_FUNC_NOT_ALLOWED_ERROR = 1491
-PARTITIONS_MUST_BE_DEFINED_ERROR = 1492
-RANGE_NOT_INCREASING_ERROR = 1493
-INCONSISTENT_TYPE_OF_FUNCTIONS_ERROR = 1494
-MULTIPLE_DEF_CONST_IN_LIST_PART_ERROR = 1495
-PARTITION_ENTRY_ERROR = 1496
-MIX_HANDLER_ERROR = 1497
-PARTITION_NOT_DEFINED_ERROR = 1498
-TOO_MANY_PARTITIONS_ERROR = 1499
-SUBPARTITION_ERROR = 1500
-CANT_CREATE_HANDLER_FILE = 1501
-BLOB_FIELD_IN_PART_FUNC_ERROR = 1502
-UNIQUE_KEY_NEED_ALL_FIELDS_IN_PF = 1503
-NO_PARTS_ERROR = 1504
-PARTITION_MGMT_ON_NONPARTITIONED = 1505
-FOREIGN_KEY_ON_PARTITIONED = 1506
-DROP_PARTITION_NON_EXISTENT = 1507
-DROP_LAST_PARTITION = 1508
-COALESCE_ONLY_ON_HASH_PARTITION = 1509
-REORG_HASH_ONLY_ON_SAME_NO = 1510
-REORG_NO_PARAM_ERROR = 1511
-ONLY_ON_RANGE_LIST_PARTITION = 1512
-ADD_PARTITION_SUBPART_ERROR = 1513
-ADD_PARTITION_NO_NEW_PARTITION = 1514
-COALESCE_PARTITION_NO_PARTITION = 1515
-REORG_PARTITION_NOT_EXIST = 1516
-SAME_NAME_PARTITION = 1517
-NO_BINLOG_ERROR = 1518
-CONSECUTIVE_REORG_PARTITIONS = 1519
-REORG_OUTSIDE_RANGE = 1520
-PARTITION_FUNCTION_FAILURE = 1521
-LIMITED_PART_RANGE = 1523
-PLUGIN_IS_NOT_LOADED = 1524
-WRONG_VALUE = 1525
-NO_PARTITION_FOR_GIVEN_VALUE = 1526
-FILEGROUP_OPTION_ONLY_ONCE = 1527
-CREATE_FILEGROUP_FAILED = 1528
-DROP_FILEGROUP_FAILED = 1529
-TABLESPACE_AUTO_EXTEND_ERROR = 1530
-WRONG_SIZE_NUMBER = 1531
-SIZE_OVERFLOW_ERROR = 1532
-ALTER_FILEGROUP_FAILED = 1533
-BINLOG_ROW_LOGGING_FAILED = 1534
-EVENT_ALREADY_EXISTS = 1537
-EVENT_DOES_NOT_EXIST = 1539
-EVENT_INTERVAL_NOT_POSITIVE_OR_TOO_BIG = 1542
-EVENT_ENDS_BEFORE_STARTS = 1543
-EVENT_EXEC_TIME_IN_THE_PAST = 1544
-EVENT_SAME_NAME = 1551
-DROP_INDEX_FK = 1553
-WARN_DEPRECATED_SYNTAX_WITH_VER = 1554
-CANT_LOCK_LOG_TABLE = 1556
-FOREIGN_DUPLICATE_KEY_OLD_UNUSED = 1557
-COL_COUNT_DOESNT_MATCH_PLEASE_UPDATE = 1558
-TEMP_TABLE_PREVENTS_SWITCH_OUT_OF_RBR = 1559
-STORED_FUNCTION_PREVENTS_SWITCH_BINLOG_FORMAT = 1560
-PARTITION_NO_TEMPORARY = 1562
-PARTITION_CONST_DOMAIN_ERROR = 1563
-PARTITION_FUNCTION_IS_NOT_ALLOWED = 1564
-NULL_IN_VALUES_LESS_THAN = 1566
-WRONG_PARTITION_NAME = 1567
-CANT_CHANGE_TX_CHARACTERISTICS = 1568
-DUP_ENTRY_AUTOINCREMENT_CASE = 1569
-EVENT_SET_VAR_ERROR = 1571
-PARTITION_MERGE_ERROR = 1572
-BASE64_DECODE_ERROR = 1575
-EVENT_RECURSION_FORBIDDEN = 1576
-ONLY_INTEGERS_ALLOWED = 1578
-UNSUPORTED_LOG_ENGINE = 1579
-BAD_LOG_STATEMENT = 1580
-CANT_RENAME_LOG_TABLE = 1581
-WRONG_PARAMCOUNT_TO_NATIVE_FCT = 1582
-WRONG_PARAMETERS_TO_NATIVE_FCT = 1583
-WRONG_PARAMETERS_TO_STORED_FCT = 1584
-NATIVE_FCT_NAME_COLLISION = 1585
-DUP_ENTRY_WITH_KEY_NAME = 1586
-BINLOG_PURGE_EMFILE = 1587
-EVENT_CANNOT_CREATE_IN_THE_PAST = 1588
-EVENT_CANNOT_ALTER_IN_THE_PAST = 1589
-NO_PARTITION_FOR_GIVEN_VALUE_SILENT = 1591
-BINLOG_UNSAFE_STATEMENT = 1592
-BINLOG_FATAL_ERROR = 1593
-BINLOG_LOGGING_IMPOSSIBLE = 1598
-VIEW_NO_CREATION_CTX = 1599
-VIEW_INVALID_CREATION_CTX = 1600
-TRG_CORRUPTED_FILE = 1602
-TRG_NO_CREATION_CTX = 1603
-TRG_INVALID_CREATION_CTX = 1604
-EVENT_INVALID_CREATION_CTX = 1605
-TRG_CANT_OPEN_TABLE = 1606
-NO_FORMAT_DESCRIPTION_EVENT_BEFORE_BINLOG_STATEMENT = 1609
-SLAVE_CORRUPT_EVENT = 1610
-LOG_PURGE_NO_FILE = 1612
-XA_RBTIMEOUT = 1613
-XA_RBDEADLOCK = 1614
-NEED_REPREPARE = 1615
-WARN_NO_MASTER_INFO = 1617
-WARN_OPTION_IGNORED = 1618
-PLUGIN_DELETE_BUILTIN = 1619
-WARN_PLUGIN_BUSY = 1620
-VARIABLE_IS_READONLY = 1621
-WARN_ENGINE_TRANSACTION_ROLLBACK = 1622
-SLAVE_HEARTBEAT_VALUE_OUT_OF_RANGE = 1624
-NDB_REPLICATION_SCHEMA_ERROR = 1625
-CONFLICT_FN_PARSE_ERROR = 1626
-EXCEPTIONS_WRITE_ERROR = 1627
-TOO_LONG_TABLE_COMMENT = 1628
-TOO_LONG_FIELD_COMMENT = 1629
-FUNC_INEXISTENT_NAME_COLLISION = 1630
-DATABASE_NAME = 1631
-TABLE_NAME = 1632
-PARTITION_NAME = 1633
-SUBPARTITION_NAME = 1634
-TEMPORARY_NAME = 1635
-RENAMED_NAME = 1636
-TOO_MANY_CONCURRENT_TRXS = 1637
-WARN_NON_ASCII_SEPARATOR_NOT_IMPLEMENTED = 1638
-DEBUG_SYNC_TIMEOUT = 1639
-DEBUG_SYNC_HIT_LIMIT = 1640
-DUP_SIGNAL_SET = 1641
-SIGNAL_WARN = 1642
-SIGNAL_NOT_FOUND = 1643
-SIGNAL_EXCEPTION = 1644
-RESIGNAL_WITHOUT_ACTIVE_HANDLER = 1645
-SIGNAL_BAD_CONDITION_TYPE = 1646
-WARN_COND_ITEM_TRUNCATED = 1647
-COND_ITEM_TOO_LONG = 1648
-UNKNOWN_LOCALE = 1649
-SLAVE_IGNORE_SERVER_IDS = 1650
-SAME_NAME_PARTITION_FIELD = 1652
-PARTITION_COLUMN_LIST_ERROR = 1653
-WRONG_TYPE_COLUMN_VALUE_ERROR = 1654
-TOO_MANY_PARTITION_FUNC_FIELDS_ERROR = 1655
-MAXVALUE_IN_VALUES_IN = 1656
-TOO_MANY_VALUES_ERROR = 1657
-ROW_SINGLE_PARTITION_FIELD_ERROR = 1658
-FIELD_TYPE_NOT_ALLOWED_AS_PARTITION_FIELD = 1659
-PARTITION_FIELDS_TOO_LONG = 1660
-BINLOG_ROW_ENGINE_AND_STMT_ENGINE = 1661
-BINLOG_ROW_MODE_AND_STMT_ENGINE = 1662
-BINLOG_UNSAFE_AND_STMT_ENGINE = 1663
-BINLOG_ROW_INJECTION_AND_STMT_ENGINE = 1664
-BINLOG_STMT_MODE_AND_ROW_ENGINE = 1665
-BINLOG_ROW_INJECTION_AND_STMT_MODE = 1666
-BINLOG_MULTIPLE_ENGINES_AND_SELF_LOGGING_ENGINE = 1667
-BINLOG_UNSAFE_LIMIT = 1668
-BINLOG_UNSAFE_SYSTEM_TABLE = 1670
-BINLOG_UNSAFE_AUTOINC_COLUMNS = 1671
-BINLOG_UNSAFE_UDF = 1672
-BINLOG_UNSAFE_SYSTEM_VARIABLE = 1673
-BINLOG_UNSAFE_SYSTEM_FUNCTION = 1674
-BINLOG_UNSAFE_NONTRANS_AFTER_TRANS = 1675
-MESSAGE_AND_STATEMENT = 1676
-SLAVE_CANT_CREATE_CONVERSION = 1678
-INSIDE_TRANSACTION_PREVENTS_SWITCH_BINLOG_FORMAT = 1679
-PATH_LENGTH = 1680
-WARN_DEPRECATED_SYNTAX_NO_REPLACEMENT = 1681
-WRONG_NATIVE_TABLE_STRUCTURE = 1682
-WRONG_PERFSCHEMA_USAGE = 1683
-WARN_I_S_SKIPPED_TABLE = 1684
-INSIDE_TRANSACTION_PREVENTS_SWITCH_BINLOG_DIRECT = 1685
-STORED_FUNCTION_PREVENTS_SWITCH_BINLOG_DIRECT = 1686
-SPATIAL_MUST_HAVE_GEOM_COL = 1687
-TOO_LONG_INDEX_COMMENT = 1688
-LOCK_ABORTED = 1689
-DATA_OUT_OF_RANGE = 1690
-WRONG_SPVAR_TYPE_IN_LIMIT = 1691
-BINLOG_UNSAFE_MULTIPLE_ENGINES_AND_SELF_LOGGING_ENGINE = 1692
-BINLOG_UNSAFE_MIXED_STATEMENT = 1693
-INSIDE_TRANSACTION_PREVENTS_SWITCH_SQL_LOG_BIN = 1694
-STORED_FUNCTION_PREVENTS_SWITCH_SQL_LOG_BIN = 1695
-FAILED_READ_FROM_PAR_FILE = 1696
-VALUES_IS_NOT_INT_TYPE_ERROR = 1697
-ACCESS_DENIED_NO_PASSWORD_ERROR = 1698
-SET_PASSWORD_AUTH_PLUGIN = 1699
-TRUNCATE_ILLEGAL_FK = 1701
-PLUGIN_IS_PERMANENT = 1702
-SLAVE_HEARTBEAT_VALUE_OUT_OF_RANGE_MIN = 1703
-SLAVE_HEARTBEAT_VALUE_OUT_OF_RANGE_MAX = 1704
-STMT_CACHE_FULL = 1705
-MULTI_UPDATE_KEY_CONFLICT = 1706
-TABLE_NEEDS_REBUILD = 1707
-WARN_OPTION_BELOW_LIMIT = 1708
-INDEX_COLUMN_TOO_LONG = 1709
-ERROR_IN_TRIGGER_BODY = 1710
-ERROR_IN_UNKNOWN_TRIGGER_BODY = 1711
-INDEX_CORRUPT = 1712
-UNDO_RECORD_TOO_BIG = 1713
-BINLOG_UNSAFE_INSERT_IGNORE_SELECT = 1714
-BINLOG_UNSAFE_INSERT_SELECT_UPDATE = 1715
-BINLOG_UNSAFE_REPLACE_SELECT = 1716
-BINLOG_UNSAFE_CREATE_IGNORE_SELECT = 1717
-BINLOG_UNSAFE_CREATE_REPLACE_SELECT = 1718
-BINLOG_UNSAFE_UPDATE_IGNORE = 1719
-PLUGIN_NO_UNINSTALL = 1720
-PLUGIN_NO_INSTALL = 1721
-BINLOG_UNSAFE_WRITE_AUTOINC_SELECT = 1722
-BINLOG_UNSAFE_CREATE_SELECT_AUTOINC = 1723
-BINLOG_UNSAFE_INSERT_TWO_KEYS = 1724
-TABLE_IN_FK_CHECK = 1725
-UNSUPPORTED_ENGINE = 1726
-BINLOG_UNSAFE_AUTOINC_NOT_FIRST = 1727
-CANNOT_LOAD_FROM_TABLE_V2 = 1728
-MASTER_DELAY_VALUE_OUT_OF_RANGE = 1729
-ONLY_FD_AND_RBR_EVENTS_ALLOWED_IN_BINLOG_STATEMENT = 1730
-PARTITION_EXCHANGE_DIFFERENT_OPTION = 1731
-PARTITION_EXCHANGE_PART_TABLE = 1732
-PARTITION_EXCHANGE_TEMP_TABLE = 1733
-PARTITION_INSTEAD_OF_SUBPARTITION = 1734
-UNKNOWN_PARTITION = 1735
-TABLES_DIFFERENT_METADATA = 1736
-ROW_DOES_NOT_MATCH_PARTITION = 1737
-BINLOG_CACHE_SIZE_GREATER_THAN_MAX = 1738
-WARN_INDEX_NOT_APPLICABLE = 1739
-PARTITION_EXCHANGE_FOREIGN_KEY = 1740
-RPL_INFO_DATA_TOO_LONG = 1742
-BINLOG_STMT_CACHE_SIZE_GREATER_THAN_MAX = 1745
-CANT_UPDATE_TABLE_IN_CREATE_TABLE_SELECT = 1746
-PARTITION_CLAUSE_ON_NONPARTITIONED = 1747
-ROW_DOES_NOT_MATCH_GIVEN_PARTITION_SET = 1748
-CHANGE_RPL_INFO_REPOSITORY_FAILURE = 1750
-WARNING_NOT_COMPLETE_ROLLBACK_WITH_CREATED_TEMP_TABLE = 1751
-WARNING_NOT_COMPLETE_ROLLBACK_WITH_DROPPED_TEMP_TABLE = 1752
-MTS_FEATURE_IS_NOT_SUPPORTED = 1753
-MTS_UPDATED_DBS_GREATER_MAX = 1754
-MTS_CANT_PARALLEL = 1755
-MTS_INCONSISTENT_DATA = 1756
-FULLTEXT_NOT_SUPPORTED_WITH_PARTITIONING = 1757
-DA_INVALID_CONDITION_NUMBER = 1758
-INSECURE_PLAIN_TEXT = 1759
-INSECURE_CHANGE_MASTER = 1760
-FOREIGN_DUPLICATE_KEY_WITH_CHILD_INFO = 1761
-FOREIGN_DUPLICATE_KEY_WITHOUT_CHILD_INFO = 1762
-SQLTHREAD_WITH_SECURE_SLAVE = 1763
-TABLE_HAS_NO_FT = 1764
-VARIABLE_NOT_SETTABLE_IN_SF_OR_TRIGGER = 1765
-VARIABLE_NOT_SETTABLE_IN_TRANSACTION = 1766
-SET_STATEMENT_CANNOT_INVOKE_FUNCTION = 1769
-GTID_NEXT_CANT_BE_AUTOMATIC_IF_GTID_NEXT_LIST_IS_NON_NULL = 1770
-MALFORMED_GTID_SET_SPECIFICATION = 1772
-MALFORMED_GTID_SET_ENCODING = 1773
-MALFORMED_GTID_SPECIFICATION = 1774
-GNO_EXHAUSTED = 1775
-BAD_SLAVE_AUTO_POSITION = 1776
-AUTO_POSITION_REQUIRES_GTID_MODE_NOT_OFF = 1777
-CANT_DO_IMPLICIT_COMMIT_IN_TRX_WHEN_GTID_NEXT_IS_SET = 1778
-GTID_MODE_ON_REQUIRES_ENFORCE_GTID_CONSISTENCY_ON = 1779
-CANT_SET_GTID_NEXT_TO_GTID_WHEN_GTID_MODE_IS_OFF = 1781
-CANT_SET_GTID_NEXT_TO_ANONYMOUS_WHEN_GTID_MODE_IS_ON = 1782
-CANT_SET_GTID_NEXT_LIST_TO_NON_NULL_WHEN_GTID_MODE_IS_OFF = 1783
-GTID_UNSAFE_NON_TRANSACTIONAL_TABLE = 1785
-GTID_UNSAFE_CREATE_SELECT = 1786
-GTID_UNSAFE_CREATE_DROP_TEMPORARY_TABLE_IN_TRANSACTION = 1787
-GTID_MODE_CAN_ONLY_CHANGE_ONE_STEP_AT_A_TIME = 1788
-MASTER_HAS_PURGED_REQUIRED_GTIDS = 1789
-CANT_SET_GTID_NEXT_WHEN_OWNING_GTID = 1790
-UNKNOWN_EXPLAIN_FORMAT = 1791
-CANT_EXECUTE_IN_READ_ONLY_TRANSACTION = 1792
-TOO_LONG_TABLE_PARTITION_COMMENT = 1793
-SLAVE_CONFIGURATION = 1794
-INNODB_FT_LIMIT = 1795
-INNODB_NO_FT_TEMP_TABLE = 1796
-INNODB_FT_WRONG_DOCID_COLUMN = 1797
-INNODB_FT_WRONG_DOCID_INDEX = 1798
-INNODB_ONLINE_LOG_TOO_BIG = 1799
-UNKNOWN_ALTER_ALGORITHM = 1800
-UNKNOWN_ALTER_LOCK = 1801
-MTS_CHANGE_MASTER_CANT_RUN_WITH_GAPS = 1802
-MTS_RECOVERY_FAILURE = 1803
-MTS_RESET_WORKERS = 1804
-COL_COUNT_DOESNT_MATCH_CORRUPTED_V2 = 1805
-SLAVE_SILENT_RETRY_TRANSACTION = 1806
-DISCARD_FK_CHECKS_RUNNING = 1807
-TABLE_SCHEMA_MISMATCH = 1808
-TABLE_IN_SYSTEM_TABLESPACE = 1809
-IO_READ_ERROR = 1810
-IO_WRITE_ERROR = 1811
-TABLESPACE_MISSING = 1812
-TABLESPACE_EXISTS = 1813
-TABLESPACE_DISCARDED = 1814
-INTERNAL_ERROR = 1815
-INNODB_IMPORT_ERROR = 1816
-INNODB_INDEX_CORRUPT = 1817
-INVALID_YEAR_COLUMN_LENGTH = 1818
-NOT_VALID_PASSWORD = 1819
-MUST_CHANGE_PASSWORD = 1820
-FK_NO_INDEX_CHILD = 1821
-FK_NO_INDEX_PARENT = 1822
-FK_FAIL_ADD_SYSTEM = 1823
-FK_CANNOT_OPEN_PARENT = 1824
-FK_INCORRECT_OPTION = 1825
-FK_DUP_NAME = 1826
-PASSWORD_FORMAT = 1827
-FK_COLUMN_CANNOT_DROP = 1828
-FK_COLUMN_CANNOT_DROP_CHILD = 1829
-FK_COLUMN_NOT_NULL = 1830
-DUP_INDEX = 1831
-FK_COLUMN_CANNOT_CHANGE = 1832
-FK_COLUMN_CANNOT_CHANGE_CHILD = 1833
-MALFORMED_PACKET = 1835
-READ_ONLY_MODE = 1836
-GTID_NEXT_TYPE_UNDEFINED_GTID = 1837
-VARIABLE_NOT_SETTABLE_IN_SP = 1838
-CANT_SET_GTID_PURGED_WHEN_GTID_EXECUTED_IS_NOT_EMPTY = 1840
-CANT_SET_GTID_PURGED_WHEN_OWNED_GTIDS_IS_NOT_EMPTY = 1841
-GTID_PURGED_WAS_CHANGED = 1842
-GTID_EXECUTED_WAS_CHANGED = 1843
-BINLOG_STMT_MODE_AND_NO_REPL_TABLES = 1844
-ALTER_OPERATION_NOT_SUPPORTED = 1845
-ALTER_OPERATION_NOT_SUPPORTED_REASON = 1846
-ALTER_OPERATION_NOT_SUPPORTED_REASON_COPY = 1847
-ALTER_OPERATION_NOT_SUPPORTED_REASON_PARTITION = 1848
-ALTER_OPERATION_NOT_SUPPORTED_REASON_FK_RENAME = 1849
-ALTER_OPERATION_NOT_SUPPORTED_REASON_COLUMN_TYPE = 1850
-ALTER_OPERATION_NOT_SUPPORTED_REASON_FK_CHECK = 1851
-ALTER_OPERATION_NOT_SUPPORTED_REASON_NOPK = 1853
-ALTER_OPERATION_NOT_SUPPORTED_REASON_AUTOINC = 1854
-ALTER_OPERATION_NOT_SUPPORTED_REASON_HIDDEN_FTS = 1855
-ALTER_OPERATION_NOT_SUPPORTED_REASON_CHANGE_FTS = 1856
-ALTER_OPERATION_NOT_SUPPORTED_REASON_FTS = 1857
-SQL_SLAVE_SKIP_COUNTER_NOT_SETTABLE_IN_GTID_MODE = 1858
-DUP_UNKNOWN_IN_INDEX = 1859
-IDENT_CAUSES_TOO_LONG_PATH = 1860
-ALTER_OPERATION_NOT_SUPPORTED_REASON_NOT_NULL = 1861
-MUST_CHANGE_PASSWORD_LOGIN = 1862
-ROW_IN_WRONG_PARTITION = 1863
-MTS_EVENT_BIGGER_PENDING_JOBS_SIZE_MAX = 1864
-BINLOG_LOGICAL_CORRUPTION = 1866
-WARN_PURGE_LOG_IN_USE = 1867
-WARN_PURGE_LOG_IS_ACTIVE = 1868
-AUTO_INCREMENT_CONFLICT = 1869
-WARN_ON_BLOCKHOLE_IN_RBR = 1870
-SLAVE_MI_INIT_REPOSITORY = 1871
-SLAVE_RLI_INIT_REPOSITORY = 1872
-ACCESS_DENIED_CHANGE_USER_ERROR = 1873
-INNODB_READ_ONLY = 1874
-STOP_SLAVE_SQL_THREAD_TIMEOUT = 1875
-STOP_SLAVE_IO_THREAD_TIMEOUT = 1876
-TABLE_CORRUPT = 1877
-TEMP_FILE_WRITE_FAILURE = 1878
-INNODB_FT_AUX_NOT_HEX_ID = 1879
-OLD_TEMPORALS_UPGRADED = 1880
-INNODB_FORCED_RECOVERY = 1881
-AES_INVALID_IV = 1882
-PLUGIN_CANNOT_BE_UNINSTALLED = 1883
-GTID_UNSAFE_BINLOG_SPLITTABLE_STATEMENT_AND_ASSIGNED_GTID = 1884
-SLAVE_HAS_MORE_GTIDS_THAN_MASTER = 1885
-MISSING_KEY = 1886
-ERROR_LAST = 1973
+"""MySQL ER Constants
+
+These constants are error codes for the bulk of the error conditions
+that may occur.
+"""
+
+if __name__ == "__main__":
+    """
+    Usage: python ER.py [/path/to/mysql/mysqld_error.h ...] >> ER.py
+    """
+    import fileinput
+    import re
+
+    data = {}
+    error_last = None
+    for line in fileinput.input():
+        line = re.sub(r"/\*.*?\*/", "", line)
+        m = re.match(r"^\s*#define\s+((ER|WARN)_[A-Z0-9_]+)\s+(\d+)\s*", line)
+        if m:
+            name = m.group(1)
+            if name.startswith("ER_"):
+                name = name[3:]
+            value = int(m.group(3))
+            if name == "ERROR_LAST":
+                if error_last is None or error_last < value:
+                    error_last = value
+                continue
+            if value not in data:
+                data[value] = set()
+            data[value].add(name)
+    for value, names in sorted(data.items()):
+        for name in sorted(names):
+            print(f"{name} = {value}")
+    if error_last is not None:
+        print("ERROR_LAST = %s" % error_last)
+
+
+ERROR_FIRST = 1000
+NO = 1002
+YES = 1003
+CANT_CREATE_FILE = 1004
+CANT_CREATE_TABLE = 1005
+CANT_CREATE_DB = 1006
+DB_CREATE_EXISTS = 1007
+DB_DROP_EXISTS = 1008
+DB_DROP_RMDIR = 1010
+CANT_FIND_SYSTEM_REC = 1012
+CANT_GET_STAT = 1013
+CANT_LOCK = 1015
+CANT_OPEN_FILE = 1016
+FILE_NOT_FOUND = 1017
+CANT_READ_DIR = 1018
+CHECKREAD = 1020
+DUP_KEY = 1022
+ERROR_ON_READ = 1024
+ERROR_ON_RENAME = 1025
+ERROR_ON_WRITE = 1026
+FILE_USED = 1027
+FILSORT_ABORT = 1028
+GET_ERRNO = 1030
+ILLEGAL_HA = 1031
+KEY_NOT_FOUND = 1032
+NOT_FORM_FILE = 1033
+NOT_KEYFILE = 1034
+OLD_KEYFILE = 1035
+OPEN_AS_READONLY = 1036
+OUTOFMEMORY = 1037
+OUT_OF_SORTMEMORY = 1038
+CON_COUNT_ERROR = 1040
+OUT_OF_RESOURCES = 1041
+BAD_HOST_ERROR = 1042
+HANDSHAKE_ERROR = 1043
+DBACCESS_DENIED_ERROR = 1044
+ACCESS_DENIED_ERROR = 1045
+NO_DB_ERROR = 1046
+UNKNOWN_COM_ERROR = 1047
+BAD_NULL_ERROR = 1048
+BAD_DB_ERROR = 1049
+TABLE_EXISTS_ERROR = 1050
+BAD_TABLE_ERROR = 1051
+NON_UNIQ_ERROR = 1052
+SERVER_SHUTDOWN = 1053
+BAD_FIELD_ERROR = 1054
+WRONG_FIELD_WITH_GROUP = 1055
+WRONG_GROUP_FIELD = 1056
+WRONG_SUM_SELECT = 1057
+WRONG_VALUE_COUNT = 1058
+TOO_LONG_IDENT = 1059
+DUP_FIELDNAME = 1060
+DUP_KEYNAME = 1061
+DUP_ENTRY = 1062
+WRONG_FIELD_SPEC = 1063
+PARSE_ERROR = 1064
+EMPTY_QUERY = 1065
+NONUNIQ_TABLE = 1066
+INVALID_DEFAULT = 1067
+MULTIPLE_PRI_KEY = 1068
+TOO_MANY_KEYS = 1069
+TOO_MANY_KEY_PARTS = 1070
+TOO_LONG_KEY = 1071
+KEY_COLUMN_DOES_NOT_EXITS = 1072
+BLOB_USED_AS_KEY = 1073
+TOO_BIG_FIELDLENGTH = 1074
+WRONG_AUTO_KEY = 1075
+READY = 1076
+SHUTDOWN_COMPLETE = 1079
+FORCING_CLOSE = 1080
+IPSOCK_ERROR = 1081
+NO_SUCH_INDEX = 1082
+WRONG_FIELD_TERMINATORS = 1083
+BLOBS_AND_NO_TERMINATED = 1084
+TEXTFILE_NOT_READABLE = 1085
+FILE_EXISTS_ERROR = 1086
+LOAD_INFO = 1087
+ALTER_INFO = 1088
+WRONG_SUB_KEY = 1089
+CANT_REMOVE_ALL_FIELDS = 1090
+CANT_DROP_FIELD_OR_KEY = 1091
+INSERT_INFO = 1092
+UPDATE_TABLE_USED = 1093
+NO_SUCH_THREAD = 1094
+KILL_DENIED_ERROR = 1095
+NO_TABLES_USED = 1096
+TOO_BIG_SET = 1097
+NO_UNIQUE_LOGFILE = 1098
+TABLE_NOT_LOCKED_FOR_WRITE = 1099
+TABLE_NOT_LOCKED = 1100
+BLOB_CANT_HAVE_DEFAULT = 1101
+WRONG_DB_NAME = 1102
+WRONG_TABLE_NAME = 1103
+TOO_BIG_SELECT = 1104
+UNKNOWN_ERROR = 1105
+UNKNOWN_PROCEDURE = 1106
+WRONG_PARAMCOUNT_TO_PROCEDURE = 1107
+WRONG_PARAMETERS_TO_PROCEDURE = 1108
+UNKNOWN_TABLE = 1109
+FIELD_SPECIFIED_TWICE = 1110
+INVALID_GROUP_FUNC_USE = 1111
+UNSUPPORTED_EXTENSION = 1112
+TABLE_MUST_HAVE_COLUMNS = 1113
+RECORD_FILE_FULL = 1114
+UNKNOWN_CHARACTER_SET = 1115
+TOO_MANY_TABLES = 1116
+TOO_MANY_FIELDS = 1117
+TOO_BIG_ROWSIZE = 1118
+STACK_OVERRUN = 1119
+WRONG_OUTER_JOIN_UNUSED = 1120
+NULL_COLUMN_IN_INDEX = 1121
+CANT_FIND_UDF = 1122
+CANT_INITIALIZE_UDF = 1123
+UDF_NO_PATHS = 1124
+UDF_EXISTS = 1125
+CANT_OPEN_LIBRARY = 1126
+CANT_FIND_DL_ENTRY = 1127
+FUNCTION_NOT_DEFINED = 1128
+HOST_IS_BLOCKED = 1129
+HOST_NOT_PRIVILEGED = 1130
+PASSWORD_ANONYMOUS_USER = 1131
+PASSWORD_NOT_ALLOWED = 1132
+PASSWORD_NO_MATCH = 1133
+UPDATE_INFO = 1134
+CANT_CREATE_THREAD = 1135
+WRONG_VALUE_COUNT_ON_ROW = 1136
+CANT_REOPEN_TABLE = 1137
+INVALID_USE_OF_NULL = 1138
+REGEXP_ERROR = 1139
+MIX_OF_GROUP_FUNC_AND_FIELDS = 1140
+NONEXISTING_GRANT = 1141
+TABLEACCESS_DENIED_ERROR = 1142
+COLUMNACCESS_DENIED_ERROR = 1143
+ILLEGAL_GRANT_FOR_TABLE = 1144
+GRANT_WRONG_HOST_OR_USER = 1145
+NO_SUCH_TABLE = 1146
+NONEXISTING_TABLE_GRANT = 1147
+NOT_ALLOWED_COMMAND = 1148
+SYNTAX_ERROR = 1149
+ABORTING_CONNECTION = 1152
+NET_PACKET_TOO_LARGE = 1153
+NET_READ_ERROR_FROM_PIPE = 1154
+NET_FCNTL_ERROR = 1155
+NET_PACKETS_OUT_OF_ORDER = 1156
+NET_UNCOMPRESS_ERROR = 1157
+NET_READ_ERROR = 1158
+NET_READ_INTERRUPTED = 1159
+NET_ERROR_ON_WRITE = 1160
+NET_WRITE_INTERRUPTED = 1161
+TOO_LONG_STRING = 1162
+TABLE_CANT_HANDLE_BLOB = 1163
+TABLE_CANT_HANDLE_AUTO_INCREMENT = 1164
+WRONG_COLUMN_NAME = 1166
+WRONG_KEY_COLUMN = 1167
+WRONG_MRG_TABLE = 1168
+DUP_UNIQUE = 1169
+BLOB_KEY_WITHOUT_LENGTH = 1170
+PRIMARY_CANT_HAVE_NULL = 1171
+TOO_MANY_ROWS = 1172
+REQUIRES_PRIMARY_KEY = 1173
+UPDATE_WITHOUT_KEY_IN_SAFE_MODE = 1175
+KEY_DOES_NOT_EXITS = 1176
+CHECK_NO_SUCH_TABLE = 1177
+CHECK_NOT_IMPLEMENTED = 1178
+CANT_DO_THIS_DURING_AN_TRANSACTION = 1179
+ERROR_DURING_COMMIT = 1180
+ERROR_DURING_ROLLBACK = 1181
+ERROR_DURING_FLUSH_LOGS = 1182
+NEW_ABORTING_CONNECTION = 1184
+MASTER = 1188
+MASTER_NET_READ = 1189
+MASTER_NET_WRITE = 1190
+FT_MATCHING_KEY_NOT_FOUND = 1191
+LOCK_OR_ACTIVE_TRANSACTION = 1192
+UNKNOWN_SYSTEM_VARIABLE = 1193
+CRASHED_ON_USAGE = 1194
+CRASHED_ON_REPAIR = 1195
+WARNING_NOT_COMPLETE_ROLLBACK = 1196
+TRANS_CACHE_FULL = 1197
+SLAVE_NOT_RUNNING = 1199
+BAD_SLAVE = 1200
+MASTER_INFO = 1201
+SLAVE_THREAD = 1202
+TOO_MANY_USER_CONNECTIONS = 1203
+SET_CONSTANTS_ONLY = 1204
+LOCK_WAIT_TIMEOUT = 1205
+LOCK_TABLE_FULL = 1206
+READ_ONLY_TRANSACTION = 1207
+WRONG_ARGUMENTS = 1210
+NO_PERMISSION_TO_CREATE_USER = 1211
+LOCK_DEADLOCK = 1213
+TABLE_CANT_HANDLE_FT = 1214
+CANNOT_ADD_FOREIGN = 1215
+NO_REFERENCED_ROW = 1216
+ROW_IS_REFERENCED = 1217
+CONNECT_TO_MASTER = 1218
+ERROR_WHEN_EXECUTING_COMMAND = 1220
+WRONG_USAGE = 1221
+WRONG_NUMBER_OF_COLUMNS_IN_SELECT = 1222
+CANT_UPDATE_WITH_READLOCK = 1223
+MIXING_NOT_ALLOWED = 1224
+DUP_ARGUMENT = 1225
+USER_LIMIT_REACHED = 1226
+SPECIFIC_ACCESS_DENIED_ERROR = 1227
+LOCAL_VARIABLE = 1228
+GLOBAL_VARIABLE = 1229
+NO_DEFAULT = 1230
+WRONG_VALUE_FOR_VAR = 1231
+WRONG_TYPE_FOR_VAR = 1232
+VAR_CANT_BE_READ = 1233
+CANT_USE_OPTION_HERE = 1234
+NOT_SUPPORTED_YET = 1235
+MASTER_FATAL_ERROR_READING_BINLOG = 1236
+SLAVE_IGNORED_TABLE = 1237
+INCORRECT_GLOBAL_LOCAL_VAR = 1238
+WRONG_FK_DEF = 1239
+KEY_REF_DO_NOT_MATCH_TABLE_REF = 1240
+OPERAND_COLUMNS = 1241
+SUBQUERY_NO_1_ROW = 1242
+UNKNOWN_STMT_HANDLER = 1243
+CORRUPT_HELP_DB = 1244
+AUTO_CONVERT = 1246
+ILLEGAL_REFERENCE = 1247
+DERIVED_MUST_HAVE_ALIAS = 1248
+SELECT_REDUCED = 1249
+TABLENAME_NOT_ALLOWED_HERE = 1250
+NOT_SUPPORTED_AUTH_MODE = 1251
+SPATIAL_CANT_HAVE_NULL = 1252
+COLLATION_CHARSET_MISMATCH = 1253
+TOO_BIG_FOR_UNCOMPRESS = 1256
+ZLIB_Z_MEM_ERROR = 1257
+ZLIB_Z_BUF_ERROR = 1258
+ZLIB_Z_DATA_ERROR = 1259
+CUT_VALUE_GROUP_CONCAT = 1260
+WARN_TOO_FEW_RECORDS = 1261
+WARN_TOO_MANY_RECORDS = 1262
+WARN_NULL_TO_NOTNULL = 1263
+WARN_DATA_OUT_OF_RANGE = 1264
+WARN_DATA_TRUNCATED = 1265
+WARN_USING_OTHER_HANDLER = 1266
+CANT_AGGREGATE_2COLLATIONS = 1267
+REVOKE_GRANTS = 1269
+CANT_AGGREGATE_3COLLATIONS = 1270
+CANT_AGGREGATE_NCOLLATIONS = 1271
+VARIABLE_IS_NOT_STRUCT = 1272
+UNKNOWN_COLLATION = 1273
+SLAVE_IGNORED_SSL_PARAMS = 1274
+SERVER_IS_IN_SECURE_AUTH_MODE = 1275
+WARN_FIELD_RESOLVED = 1276
+BAD_SLAVE_UNTIL_COND = 1277
+MISSING_SKIP_SLAVE = 1278
+UNTIL_COND_IGNORED = 1279
+WRONG_NAME_FOR_INDEX = 1280
+WRONG_NAME_FOR_CATALOG = 1281
+BAD_FT_COLUMN = 1283
+UNKNOWN_KEY_CACHE = 1284
+WARN_HOSTNAME_WONT_WORK = 1285
+UNKNOWN_STORAGE_ENGINE = 1286
+WARN_DEPRECATED_SYNTAX = 1287
+NON_UPDATABLE_TABLE = 1288
+FEATURE_DISABLED = 1289
+OPTION_PREVENTS_STATEMENT = 1290
+DUPLICATED_VALUE_IN_TYPE = 1291
+TRUNCATED_WRONG_VALUE = 1292
+INVALID_ON_UPDATE = 1294
+UNSUPPORTED_PS = 1295
+GET_ERRMSG = 1296
+GET_TEMPORARY_ERRMSG = 1297
+UNKNOWN_TIME_ZONE = 1298
+WARN_INVALID_TIMESTAMP = 1299
+INVALID_CHARACTER_STRING = 1300
+WARN_ALLOWED_PACKET_OVERFLOWED = 1301
+CONFLICTING_DECLARATIONS = 1302
+SP_NO_RECURSIVE_CREATE = 1303
+SP_ALREADY_EXISTS = 1304
+SP_DOES_NOT_EXIST = 1305
+SP_DROP_FAILED = 1306
+SP_STORE_FAILED = 1307
+SP_LILABEL_MISMATCH = 1308
+SP_LABEL_REDEFINE = 1309
+SP_LABEL_MISMATCH = 1310
+SP_UNINIT_VAR = 1311
+SP_BADSELECT = 1312
+SP_BADRETURN = 1313
+SP_BADSTATEMENT = 1314
+UPDATE_LOG_DEPRECATED_IGNORED = 1315
+UPDATE_LOG_DEPRECATED_TRANSLATED = 1316
+QUERY_INTERRUPTED = 1317
+SP_WRONG_NO_OF_ARGS = 1318
+SP_COND_MISMATCH = 1319
+SP_NORETURN = 1320
+SP_NORETURNEND = 1321
+SP_BAD_CURSOR_QUERY = 1322
+SP_BAD_CURSOR_SELECT = 1323
+SP_CURSOR_MISMATCH = 1324
+SP_CURSOR_ALREADY_OPEN = 1325
+SP_CURSOR_NOT_OPEN = 1326
+SP_UNDECLARED_VAR = 1327
+SP_WRONG_NO_OF_FETCH_ARGS = 1328
+SP_FETCH_NO_DATA = 1329
+SP_DUP_PARAM = 1330
+SP_DUP_VAR = 1331
+SP_DUP_COND = 1332
+SP_DUP_CURS = 1333
+SP_CANT_ALTER = 1334
+SP_SUBSELECT_NYI = 1335
+STMT_NOT_ALLOWED_IN_SF_OR_TRG = 1336
+SP_VARCOND_AFTER_CURSHNDLR = 1337
+SP_CURSOR_AFTER_HANDLER = 1338
+SP_CASE_NOT_FOUND = 1339
+FPARSER_TOO_BIG_FILE = 1340
+FPARSER_BAD_HEADER = 1341
+FPARSER_EOF_IN_COMMENT = 1342
+FPARSER_ERROR_IN_PARAMETER = 1343
+FPARSER_EOF_IN_UNKNOWN_PARAMETER = 1344
+VIEW_NO_EXPLAIN = 1345
+WRONG_OBJECT = 1347
+NONUPDATEABLE_COLUMN = 1348
+VIEW_SELECT_CLAUSE = 1350
+VIEW_SELECT_VARIABLE = 1351
+VIEW_SELECT_TMPTABLE = 1352
+VIEW_WRONG_LIST = 1353
+WARN_VIEW_MERGE = 1354
+WARN_VIEW_WITHOUT_KEY = 1355
+VIEW_INVALID = 1356
+SP_NO_DROP_SP = 1357
+TRG_ALREADY_EXISTS = 1359
+TRG_DOES_NOT_EXIST = 1360
+TRG_ON_VIEW_OR_TEMP_TABLE = 1361
+TRG_CANT_CHANGE_ROW = 1362
+TRG_NO_SUCH_ROW_IN_TRG = 1363
+NO_DEFAULT_FOR_FIELD = 1364
+DIVISION_BY_ZERO = 1365
+TRUNCATED_WRONG_VALUE_FOR_FIELD = 1366
+ILLEGAL_VALUE_FOR_TYPE = 1367
+VIEW_NONUPD_CHECK = 1368
+VIEW_CHECK_FAILED = 1369
+PROCACCESS_DENIED_ERROR = 1370
+RELAY_LOG_FAIL = 1371
+UNKNOWN_TARGET_BINLOG = 1373
+IO_ERR_LOG_INDEX_READ = 1374
+BINLOG_PURGE_PROHIBITED = 1375
+FSEEK_FAIL = 1376
+BINLOG_PURGE_FATAL_ERR = 1377
+LOG_IN_USE = 1378
+LOG_PURGE_UNKNOWN_ERR = 1379
+RELAY_LOG_INIT = 1380
+NO_BINARY_LOGGING = 1381
+RESERVED_SYNTAX = 1382
+PS_MANY_PARAM = 1390
+KEY_PART_0 = 1391
+VIEW_CHECKSUM = 1392
+VIEW_MULTIUPDATE = 1393
+VIEW_NO_INSERT_FIELD_LIST = 1394
+VIEW_DELETE_MERGE_VIEW = 1395
+CANNOT_USER = 1396
+XAER_NOTA = 1397
+XAER_INVAL = 1398
+XAER_RMFAIL = 1399
+XAER_OUTSIDE = 1400
+XAER_RMERR = 1401
+XA_RBROLLBACK = 1402
+NONEXISTING_PROC_GRANT = 1403
+PROC_AUTO_GRANT_FAIL = 1404
+PROC_AUTO_REVOKE_FAIL = 1405
+DATA_TOO_LONG = 1406
+SP_BAD_SQLSTATE = 1407
+STARTUP = 1408
+LOAD_FROM_FIXED_SIZE_ROWS_TO_VAR = 1409
+CANT_CREATE_USER_WITH_GRANT = 1410
+WRONG_VALUE_FOR_TYPE = 1411
+TABLE_DEF_CHANGED = 1412
+SP_DUP_HANDLER = 1413
+SP_NOT_VAR_ARG = 1414
+SP_NO_RETSET = 1415
+CANT_CREATE_GEOMETRY_OBJECT = 1416
+BINLOG_UNSAFE_ROUTINE = 1418
+BINLOG_CREATE_ROUTINE_NEED_SUPER = 1419
+STMT_HAS_NO_OPEN_CURSOR = 1421
+COMMIT_NOT_ALLOWED_IN_SF_OR_TRG = 1422
+NO_DEFAULT_FOR_VIEW_FIELD = 1423
+SP_NO_RECURSION = 1424
+TOO_BIG_SCALE = 1425
+TOO_BIG_PRECISION = 1426
+M_BIGGER_THAN_D = 1427
+WRONG_LOCK_OF_SYSTEM_TABLE = 1428
+CONNECT_TO_FOREIGN_DATA_SOURCE = 1429
+QUERY_ON_FOREIGN_DATA_SOURCE = 1430
+FOREIGN_DATA_SOURCE_DOESNT_EXIST = 1431
+FOREIGN_DATA_STRING_INVALID_CANT_CREATE = 1432
+FOREIGN_DATA_STRING_INVALID = 1433
+TRG_IN_WRONG_SCHEMA = 1435
+STACK_OVERRUN_NEED_MORE = 1436
+TOO_LONG_BODY = 1437
+WARN_CANT_DROP_DEFAULT_KEYCACHE = 1438
+TOO_BIG_DISPLAYWIDTH = 1439
+XAER_DUPID = 1440
+DATETIME_FUNCTION_OVERFLOW = 1441
+CANT_UPDATE_USED_TABLE_IN_SF_OR_TRG = 1442
+VIEW_PREVENT_UPDATE = 1443
+PS_NO_RECURSION = 1444
+SP_CANT_SET_AUTOCOMMIT = 1445
+VIEW_FRM_NO_USER = 1447
+VIEW_OTHER_USER = 1448
+NO_SUCH_USER = 1449
+FORBID_SCHEMA_CHANGE = 1450
+ROW_IS_REFERENCED_2 = 1451
+NO_REFERENCED_ROW_2 = 1452
+SP_BAD_VAR_SHADOW = 1453
+TRG_NO_DEFINER = 1454
+OLD_FILE_FORMAT = 1455
+SP_RECURSION_LIMIT = 1456
+SP_WRONG_NAME = 1458
+TABLE_NEEDS_UPGRADE = 1459
+SP_NO_AGGREGATE = 1460
+MAX_PREPARED_STMT_COUNT_REACHED = 1461
+VIEW_RECURSIVE = 1462
+NON_GROUPING_FIELD_USED = 1463
+TABLE_CANT_HANDLE_SPKEYS = 1464
+NO_TRIGGERS_ON_SYSTEM_SCHEMA = 1465
+REMOVED_SPACES = 1466
+AUTOINC_READ_FAILED = 1467
+USERNAME = 1468
+HOSTNAME = 1469
+WRONG_STRING_LENGTH = 1470
+NON_INSERTABLE_TABLE = 1471
+ADMIN_WRONG_MRG_TABLE = 1472
+TOO_HIGH_LEVEL_OF_NESTING_FOR_SELECT = 1473
+NAME_BECOMES_EMPTY = 1474
+AMBIGUOUS_FIELD_TERM = 1475
+FOREIGN_SERVER_EXISTS = 1476
+FOREIGN_SERVER_DOESNT_EXIST = 1477
+ILLEGAL_HA_CREATE_OPTION = 1478
+PARTITION_REQUIRES_VALUES_ERROR = 1479
+PARTITION_WRONG_VALUES_ERROR = 1480
+PARTITION_MAXVALUE_ERROR = 1481
+PARTITION_WRONG_NO_PART_ERROR = 1484
+PARTITION_WRONG_NO_SUBPART_ERROR = 1485
+WRONG_EXPR_IN_PARTITION_FUNC_ERROR = 1486
+FIELD_NOT_FOUND_PART_ERROR = 1488
+INCONSISTENT_PARTITION_INFO_ERROR = 1490
+PARTITION_FUNC_NOT_ALLOWED_ERROR = 1491
+PARTITIONS_MUST_BE_DEFINED_ERROR = 1492
+RANGE_NOT_INCREASING_ERROR = 1493
+INCONSISTENT_TYPE_OF_FUNCTIONS_ERROR = 1494
+MULTIPLE_DEF_CONST_IN_LIST_PART_ERROR = 1495
+PARTITION_ENTRY_ERROR = 1496
+MIX_HANDLER_ERROR = 1497
+PARTITION_NOT_DEFINED_ERROR = 1498
+TOO_MANY_PARTITIONS_ERROR = 1499
+SUBPARTITION_ERROR = 1500
+CANT_CREATE_HANDLER_FILE = 1501
+BLOB_FIELD_IN_PART_FUNC_ERROR = 1502
+UNIQUE_KEY_NEED_ALL_FIELDS_IN_PF = 1503
+NO_PARTS_ERROR = 1504
+PARTITION_MGMT_ON_NONPARTITIONED = 1505
+FOREIGN_KEY_ON_PARTITIONED = 1506
+DROP_PARTITION_NON_EXISTENT = 1507
+DROP_LAST_PARTITION = 1508
+COALESCE_ONLY_ON_HASH_PARTITION = 1509
+REORG_HASH_ONLY_ON_SAME_NO = 1510
+REORG_NO_PARAM_ERROR = 1511
+ONLY_ON_RANGE_LIST_PARTITION = 1512
+ADD_PARTITION_SUBPART_ERROR = 1513
+ADD_PARTITION_NO_NEW_PARTITION = 1514
+COALESCE_PARTITION_NO_PARTITION = 1515
+REORG_PARTITION_NOT_EXIST = 1516
+SAME_NAME_PARTITION = 1517
+NO_BINLOG_ERROR = 1518
+CONSECUTIVE_REORG_PARTITIONS = 1519
+REORG_OUTSIDE_RANGE = 1520
+PARTITION_FUNCTION_FAILURE = 1521
+LIMITED_PART_RANGE = 1523
+PLUGIN_IS_NOT_LOADED = 1524
+WRONG_VALUE = 1525
+NO_PARTITION_FOR_GIVEN_VALUE = 1526
+FILEGROUP_OPTION_ONLY_ONCE = 1527
+CREATE_FILEGROUP_FAILED = 1528
+DROP_FILEGROUP_FAILED = 1529
+TABLESPACE_AUTO_EXTEND_ERROR = 1530
+WRONG_SIZE_NUMBER = 1531
+SIZE_OVERFLOW_ERROR = 1532
+ALTER_FILEGROUP_FAILED = 1533
+BINLOG_ROW_LOGGING_FAILED = 1534
+EVENT_ALREADY_EXISTS = 1537
+EVENT_DOES_NOT_EXIST = 1539
+EVENT_INTERVAL_NOT_POSITIVE_OR_TOO_BIG = 1542
+EVENT_ENDS_BEFORE_STARTS = 1543
+EVENT_EXEC_TIME_IN_THE_PAST = 1544
+EVENT_SAME_NAME = 1551
+DROP_INDEX_FK = 1553
+WARN_DEPRECATED_SYNTAX_WITH_VER = 1554
+CANT_LOCK_LOG_TABLE = 1556
+FOREIGN_DUPLICATE_KEY_OLD_UNUSED = 1557
+COL_COUNT_DOESNT_MATCH_PLEASE_UPDATE = 1558
+TEMP_TABLE_PREVENTS_SWITCH_OUT_OF_RBR = 1559
+STORED_FUNCTION_PREVENTS_SWITCH_BINLOG_FORMAT = 1560
+PARTITION_NO_TEMPORARY = 1562
+PARTITION_CONST_DOMAIN_ERROR = 1563
+PARTITION_FUNCTION_IS_NOT_ALLOWED = 1564
+NULL_IN_VALUES_LESS_THAN = 1566
+WRONG_PARTITION_NAME = 1567
+CANT_CHANGE_TX_CHARACTERISTICS = 1568
+DUP_ENTRY_AUTOINCREMENT_CASE = 1569
+EVENT_SET_VAR_ERROR = 1571
+PARTITION_MERGE_ERROR = 1572
+BASE64_DECODE_ERROR = 1575
+EVENT_RECURSION_FORBIDDEN = 1576
+ONLY_INTEGERS_ALLOWED = 1578
+UNSUPORTED_LOG_ENGINE = 1579
+BAD_LOG_STATEMENT = 1580
+CANT_RENAME_LOG_TABLE = 1581
+WRONG_PARAMCOUNT_TO_NATIVE_FCT = 1582
+WRONG_PARAMETERS_TO_NATIVE_FCT = 1583
+WRONG_PARAMETERS_TO_STORED_FCT = 1584
+NATIVE_FCT_NAME_COLLISION = 1585
+DUP_ENTRY_WITH_KEY_NAME = 1586
+BINLOG_PURGE_EMFILE = 1587
+EVENT_CANNOT_CREATE_IN_THE_PAST = 1588
+EVENT_CANNOT_ALTER_IN_THE_PAST = 1589
+NO_PARTITION_FOR_GIVEN_VALUE_SILENT = 1591
+BINLOG_UNSAFE_STATEMENT = 1592
+BINLOG_FATAL_ERROR = 1593
+BINLOG_LOGGING_IMPOSSIBLE = 1598
+VIEW_NO_CREATION_CTX = 1599
+VIEW_INVALID_CREATION_CTX = 1600
+TRG_CORRUPTED_FILE = 1602
+TRG_NO_CREATION_CTX = 1603
+TRG_INVALID_CREATION_CTX = 1604
+EVENT_INVALID_CREATION_CTX = 1605
+TRG_CANT_OPEN_TABLE = 1606
+NO_FORMAT_DESCRIPTION_EVENT_BEFORE_BINLOG_STATEMENT = 1609
+SLAVE_CORRUPT_EVENT = 1610
+LOG_PURGE_NO_FILE = 1612
+XA_RBTIMEOUT = 1613
+XA_RBDEADLOCK = 1614
+NEED_REPREPARE = 1615
+WARN_NO_MASTER_INFO = 1617
+WARN_OPTION_IGNORED = 1618
+PLUGIN_DELETE_BUILTIN = 1619
+WARN_PLUGIN_BUSY = 1620
+VARIABLE_IS_READONLY = 1621
+WARN_ENGINE_TRANSACTION_ROLLBACK = 1622
+SLAVE_HEARTBEAT_VALUE_OUT_OF_RANGE = 1624
+NDB_REPLICATION_SCHEMA_ERROR = 1625
+CONFLICT_FN_PARSE_ERROR = 1626
+EXCEPTIONS_WRITE_ERROR = 1627
+TOO_LONG_TABLE_COMMENT = 1628
+TOO_LONG_FIELD_COMMENT = 1629
+FUNC_INEXISTENT_NAME_COLLISION = 1630
+DATABASE_NAME = 1631
+TABLE_NAME = 1632
+PARTITION_NAME = 1633
+SUBPARTITION_NAME = 1634
+TEMPORARY_NAME = 1635
+RENAMED_NAME = 1636
+TOO_MANY_CONCURRENT_TRXS = 1637
+WARN_NON_ASCII_SEPARATOR_NOT_IMPLEMENTED = 1638
+DEBUG_SYNC_TIMEOUT = 1639
+DEBUG_SYNC_HIT_LIMIT = 1640
+DUP_SIGNAL_SET = 1641
+SIGNAL_WARN = 1642
+SIGNAL_NOT_FOUND = 1643
+SIGNAL_EXCEPTION = 1644
+RESIGNAL_WITHOUT_ACTIVE_HANDLER = 1645
+SIGNAL_BAD_CONDITION_TYPE = 1646
+WARN_COND_ITEM_TRUNCATED = 1647
+COND_ITEM_TOO_LONG = 1648
+UNKNOWN_LOCALE = 1649
+SLAVE_IGNORE_SERVER_IDS = 1650
+SAME_NAME_PARTITION_FIELD = 1652
+PARTITION_COLUMN_LIST_ERROR = 1653
+WRONG_TYPE_COLUMN_VALUE_ERROR = 1654
+TOO_MANY_PARTITION_FUNC_FIELDS_ERROR = 1655
+MAXVALUE_IN_VALUES_IN = 1656
+TOO_MANY_VALUES_ERROR = 1657
+ROW_SINGLE_PARTITION_FIELD_ERROR = 1658
+FIELD_TYPE_NOT_ALLOWED_AS_PARTITION_FIELD = 1659
+PARTITION_FIELDS_TOO_LONG = 1660
+BINLOG_ROW_ENGINE_AND_STMT_ENGINE = 1661
+BINLOG_ROW_MODE_AND_STMT_ENGINE = 1662
+BINLOG_UNSAFE_AND_STMT_ENGINE = 1663
+BINLOG_ROW_INJECTION_AND_STMT_ENGINE = 1664
+BINLOG_STMT_MODE_AND_ROW_ENGINE = 1665
+BINLOG_ROW_INJECTION_AND_STMT_MODE = 1666
+BINLOG_MULTIPLE_ENGINES_AND_SELF_LOGGING_ENGINE = 1667
+BINLOG_UNSAFE_LIMIT = 1668
+BINLOG_UNSAFE_SYSTEM_TABLE = 1670
+BINLOG_UNSAFE_AUTOINC_COLUMNS = 1671
+BINLOG_UNSAFE_UDF = 1672
+BINLOG_UNSAFE_SYSTEM_VARIABLE = 1673
+BINLOG_UNSAFE_SYSTEM_FUNCTION = 1674
+BINLOG_UNSAFE_NONTRANS_AFTER_TRANS = 1675
+MESSAGE_AND_STATEMENT = 1676
+SLAVE_CANT_CREATE_CONVERSION = 1678
+INSIDE_TRANSACTION_PREVENTS_SWITCH_BINLOG_FORMAT = 1679
+PATH_LENGTH = 1680
+WARN_DEPRECATED_SYNTAX_NO_REPLACEMENT = 1681
+WRONG_NATIVE_TABLE_STRUCTURE = 1682
+WRONG_PERFSCHEMA_USAGE = 1683
+WARN_I_S_SKIPPED_TABLE = 1684
+INSIDE_TRANSACTION_PREVENTS_SWITCH_BINLOG_DIRECT = 1685
+STORED_FUNCTION_PREVENTS_SWITCH_BINLOG_DIRECT = 1686
+SPATIAL_MUST_HAVE_GEOM_COL = 1687
+TOO_LONG_INDEX_COMMENT = 1688
+LOCK_ABORTED = 1689
+DATA_OUT_OF_RANGE = 1690
+WRONG_SPVAR_TYPE_IN_LIMIT = 1691
+BINLOG_UNSAFE_MULTIPLE_ENGINES_AND_SELF_LOGGING_ENGINE = 1692
+BINLOG_UNSAFE_MIXED_STATEMENT = 1693
+INSIDE_TRANSACTION_PREVENTS_SWITCH_SQL_LOG_BIN = 1694
+STORED_FUNCTION_PREVENTS_SWITCH_SQL_LOG_BIN = 1695
+FAILED_READ_FROM_PAR_FILE = 1696
+VALUES_IS_NOT_INT_TYPE_ERROR = 1697
+ACCESS_DENIED_NO_PASSWORD_ERROR = 1698
+SET_PASSWORD_AUTH_PLUGIN = 1699
+TRUNCATE_ILLEGAL_FK = 1701
+PLUGIN_IS_PERMANENT = 1702
+SLAVE_HEARTBEAT_VALUE_OUT_OF_RANGE_MIN = 1703
+SLAVE_HEARTBEAT_VALUE_OUT_OF_RANGE_MAX = 1704
+STMT_CACHE_FULL = 1705
+MULTI_UPDATE_KEY_CONFLICT = 1706
+TABLE_NEEDS_REBUILD = 1707
+WARN_OPTION_BELOW_LIMIT = 1708
+INDEX_COLUMN_TOO_LONG = 1709
+ERROR_IN_TRIGGER_BODY = 1710
+ERROR_IN_UNKNOWN_TRIGGER_BODY = 1711
+INDEX_CORRUPT = 1712
+UNDO_RECORD_TOO_BIG = 1713
+BINLOG_UNSAFE_INSERT_IGNORE_SELECT = 1714
+BINLOG_UNSAFE_INSERT_SELECT_UPDATE = 1715
+BINLOG_UNSAFE_REPLACE_SELECT = 1716
+BINLOG_UNSAFE_CREATE_IGNORE_SELECT = 1717
+BINLOG_UNSAFE_CREATE_REPLACE_SELECT = 1718
+BINLOG_UNSAFE_UPDATE_IGNORE = 1719
+PLUGIN_NO_UNINSTALL = 1720
+PLUGIN_NO_INSTALL = 1721
+BINLOG_UNSAFE_WRITE_AUTOINC_SELECT = 1722
+BINLOG_UNSAFE_CREATE_SELECT_AUTOINC = 1723
+BINLOG_UNSAFE_INSERT_TWO_KEYS = 1724
+TABLE_IN_FK_CHECK = 1725
+UNSUPPORTED_ENGINE = 1726
+BINLOG_UNSAFE_AUTOINC_NOT_FIRST = 1727
+CANNOT_LOAD_FROM_TABLE_V2 = 1728
+MASTER_DELAY_VALUE_OUT_OF_RANGE = 1729
+ONLY_FD_AND_RBR_EVENTS_ALLOWED_IN_BINLOG_STATEMENT = 1730
+PARTITION_EXCHANGE_DIFFERENT_OPTION = 1731
+PARTITION_EXCHANGE_PART_TABLE = 1732
+PARTITION_EXCHANGE_TEMP_TABLE = 1733
+PARTITION_INSTEAD_OF_SUBPARTITION = 1734
+UNKNOWN_PARTITION = 1735
+TABLES_DIFFERENT_METADATA = 1736
+ROW_DOES_NOT_MATCH_PARTITION = 1737
+BINLOG_CACHE_SIZE_GREATER_THAN_MAX = 1738
+WARN_INDEX_NOT_APPLICABLE = 1739
+PARTITION_EXCHANGE_FOREIGN_KEY = 1740
+RPL_INFO_DATA_TOO_LONG = 1742
+BINLOG_STMT_CACHE_SIZE_GREATER_THAN_MAX = 1745
+CANT_UPDATE_TABLE_IN_CREATE_TABLE_SELECT = 1746
+PARTITION_CLAUSE_ON_NONPARTITIONED = 1747
+ROW_DOES_NOT_MATCH_GIVEN_PARTITION_SET = 1748
+CHANGE_RPL_INFO_REPOSITORY_FAILURE = 1750
+WARNING_NOT_COMPLETE_ROLLBACK_WITH_CREATED_TEMP_TABLE = 1751
+WARNING_NOT_COMPLETE_ROLLBACK_WITH_DROPPED_TEMP_TABLE = 1752
+MTS_FEATURE_IS_NOT_SUPPORTED = 1753
+MTS_UPDATED_DBS_GREATER_MAX = 1754
+MTS_CANT_PARALLEL = 1755
+MTS_INCONSISTENT_DATA = 1756
+FULLTEXT_NOT_SUPPORTED_WITH_PARTITIONING = 1757
+DA_INVALID_CONDITION_NUMBER = 1758
+INSECURE_PLAIN_TEXT = 1759
+INSECURE_CHANGE_MASTER = 1760
+FOREIGN_DUPLICATE_KEY_WITH_CHILD_INFO = 1761
+FOREIGN_DUPLICATE_KEY_WITHOUT_CHILD_INFO = 1762
+SQLTHREAD_WITH_SECURE_SLAVE = 1763
+TABLE_HAS_NO_FT = 1764
+VARIABLE_NOT_SETTABLE_IN_SF_OR_TRIGGER = 1765
+VARIABLE_NOT_SETTABLE_IN_TRANSACTION = 1766
+SET_STATEMENT_CANNOT_INVOKE_FUNCTION = 1769
+GTID_NEXT_CANT_BE_AUTOMATIC_IF_GTID_NEXT_LIST_IS_NON_NULL = 1770
+MALFORMED_GTID_SET_SPECIFICATION = 1772
+MALFORMED_GTID_SET_ENCODING = 1773
+MALFORMED_GTID_SPECIFICATION = 1774
+GNO_EXHAUSTED = 1775
+BAD_SLAVE_AUTO_POSITION = 1776
+AUTO_POSITION_REQUIRES_GTID_MODE_NOT_OFF = 1777
+CANT_DO_IMPLICIT_COMMIT_IN_TRX_WHEN_GTID_NEXT_IS_SET = 1778
+GTID_MODE_ON_REQUIRES_ENFORCE_GTID_CONSISTENCY_ON = 1779
+CANT_SET_GTID_NEXT_TO_GTID_WHEN_GTID_MODE_IS_OFF = 1781
+CANT_SET_GTID_NEXT_TO_ANONYMOUS_WHEN_GTID_MODE_IS_ON = 1782
+CANT_SET_GTID_NEXT_LIST_TO_NON_NULL_WHEN_GTID_MODE_IS_OFF = 1783
+GTID_UNSAFE_NON_TRANSACTIONAL_TABLE = 1785
+GTID_UNSAFE_CREATE_SELECT = 1786
+GTID_UNSAFE_CREATE_DROP_TEMPORARY_TABLE_IN_TRANSACTION = 1787
+GTID_MODE_CAN_ONLY_CHANGE_ONE_STEP_AT_A_TIME = 1788
+MASTER_HAS_PURGED_REQUIRED_GTIDS = 1789
+CANT_SET_GTID_NEXT_WHEN_OWNING_GTID = 1790
+UNKNOWN_EXPLAIN_FORMAT = 1791
+CANT_EXECUTE_IN_READ_ONLY_TRANSACTION = 1792
+TOO_LONG_TABLE_PARTITION_COMMENT = 1793
+SLAVE_CONFIGURATION = 1794
+INNODB_FT_LIMIT = 1795
+INNODB_NO_FT_TEMP_TABLE = 1796
+INNODB_FT_WRONG_DOCID_COLUMN = 1797
+INNODB_FT_WRONG_DOCID_INDEX = 1798
+INNODB_ONLINE_LOG_TOO_BIG = 1799
+UNKNOWN_ALTER_ALGORITHM = 1800
+UNKNOWN_ALTER_LOCK = 1801
+MTS_CHANGE_MASTER_CANT_RUN_WITH_GAPS = 1802
+MTS_RECOVERY_FAILURE = 1803
+MTS_RESET_WORKERS = 1804
+COL_COUNT_DOESNT_MATCH_CORRUPTED_V2 = 1805
+SLAVE_SILENT_RETRY_TRANSACTION = 1806
+DISCARD_FK_CHECKS_RUNNING = 1807
+TABLE_SCHEMA_MISMATCH = 1808
+TABLE_IN_SYSTEM_TABLESPACE = 1809
+IO_READ_ERROR = 1810
+IO_WRITE_ERROR = 1811
+TABLESPACE_MISSING = 1812
+TABLESPACE_EXISTS = 1813
+TABLESPACE_DISCARDED = 1814
+INTERNAL_ERROR = 1815
+INNODB_IMPORT_ERROR = 1816
+INNODB_INDEX_CORRUPT = 1817
+INVALID_YEAR_COLUMN_LENGTH = 1818
+NOT_VALID_PASSWORD = 1819
+MUST_CHANGE_PASSWORD = 1820
+FK_NO_INDEX_CHILD = 1821
+FK_NO_INDEX_PARENT = 1822
+FK_FAIL_ADD_SYSTEM = 1823
+FK_CANNOT_OPEN_PARENT = 1824
+FK_INCORRECT_OPTION = 1825
+FK_DUP_NAME = 1826
+PASSWORD_FORMAT = 1827
+FK_COLUMN_CANNOT_DROP = 1828
+FK_COLUMN_CANNOT_DROP_CHILD = 1829
+FK_COLUMN_NOT_NULL = 1830
+DUP_INDEX = 1831
+FK_COLUMN_CANNOT_CHANGE = 1832
+FK_COLUMN_CANNOT_CHANGE_CHILD = 1833
+MALFORMED_PACKET = 1835
+READ_ONLY_MODE = 1836
+GTID_NEXT_TYPE_UNDEFINED_GTID = 1837
+VARIABLE_NOT_SETTABLE_IN_SP = 1838
+CANT_SET_GTID_PURGED_WHEN_GTID_EXECUTED_IS_NOT_EMPTY = 1840
+CANT_SET_GTID_PURGED_WHEN_OWNED_GTIDS_IS_NOT_EMPTY = 1841
+GTID_PURGED_WAS_CHANGED = 1842
+GTID_EXECUTED_WAS_CHANGED = 1843
+BINLOG_STMT_MODE_AND_NO_REPL_TABLES = 1844
+ALTER_OPERATION_NOT_SUPPORTED = 1845
+ALTER_OPERATION_NOT_SUPPORTED_REASON = 1846
+ALTER_OPERATION_NOT_SUPPORTED_REASON_COPY = 1847
+ALTER_OPERATION_NOT_SUPPORTED_REASON_PARTITION = 1848
+ALTER_OPERATION_NOT_SUPPORTED_REASON_FK_RENAME = 1849
+ALTER_OPERATION_NOT_SUPPORTED_REASON_COLUMN_TYPE = 1850
+ALTER_OPERATION_NOT_SUPPORTED_REASON_FK_CHECK = 1851
+ALTER_OPERATION_NOT_SUPPORTED_REASON_NOPK = 1853
+ALTER_OPERATION_NOT_SUPPORTED_REASON_AUTOINC = 1854
+ALTER_OPERATION_NOT_SUPPORTED_REASON_HIDDEN_FTS = 1855
+ALTER_OPERATION_NOT_SUPPORTED_REASON_CHANGE_FTS = 1856
+ALTER_OPERATION_NOT_SUPPORTED_REASON_FTS = 1857
+SQL_SLAVE_SKIP_COUNTER_NOT_SETTABLE_IN_GTID_MODE = 1858
+DUP_UNKNOWN_IN_INDEX = 1859
+IDENT_CAUSES_TOO_LONG_PATH = 1860
+ALTER_OPERATION_NOT_SUPPORTED_REASON_NOT_NULL = 1861
+MUST_CHANGE_PASSWORD_LOGIN = 1862
+ROW_IN_WRONG_PARTITION = 1863
+MTS_EVENT_BIGGER_PENDING_JOBS_SIZE_MAX = 1864
+BINLOG_LOGICAL_CORRUPTION = 1866
+WARN_PURGE_LOG_IN_USE = 1867
+WARN_PURGE_LOG_IS_ACTIVE = 1868
+AUTO_INCREMENT_CONFLICT = 1869
+WARN_ON_BLOCKHOLE_IN_RBR = 1870
+SLAVE_MI_INIT_REPOSITORY = 1871
+SLAVE_RLI_INIT_REPOSITORY = 1872
+ACCESS_DENIED_CHANGE_USER_ERROR = 1873
+INNODB_READ_ONLY = 1874
+STOP_SLAVE_SQL_THREAD_TIMEOUT = 1875
+STOP_SLAVE_IO_THREAD_TIMEOUT = 1876
+TABLE_CORRUPT = 1877
+TEMP_FILE_WRITE_FAILURE = 1878
+INNODB_FT_AUX_NOT_HEX_ID = 1879
+OLD_TEMPORALS_UPGRADED = 1880
+INNODB_FORCED_RECOVERY = 1881
+AES_INVALID_IV = 1882
+PLUGIN_CANNOT_BE_UNINSTALLED = 1883
+GTID_UNSAFE_BINLOG_SPLITTABLE_STATEMENT_AND_ASSIGNED_GTID = 1884
+SLAVE_HAS_MORE_GTIDS_THAN_MASTER = 1885
+MISSING_KEY = 1886
+ERROR_LAST = 1973
```

### Comparing `mysqlclient-2.2.0/src/MySQLdb/converters.py` & `mysqlclient-2.2.0rc1/src/MySQLdb/converters.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,139 +1,139 @@
-"""MySQLdb type conversion module
-
-This module handles all the type conversions for MySQL. If the default
-type conversions aren't what you need, you can make your own. The
-dictionary conversions maps some kind of type to a conversion function
-which returns the corresponding value:
-
-Key: FIELD_TYPE.* (from MySQLdb.constants)
-
-Conversion function:
-
-    Arguments: string
-
-    Returns: Python object
-
-Key: Python type object (from types) or class
-
-Conversion function:
-
-    Arguments: Python object of indicated type or class AND
-               conversion dictionary
-
-    Returns: SQL literal value
-
-    Notes: Most conversion functions can ignore the dictionary, but
-           it is a required parameter. It is necessary for converting
-           things like sequences and instances.
-
-Don't modify conversions if you can avoid it. Instead, make copies
-(with the copy() method), modify the copies, and then pass them to
-MySQL.connect().
-"""
-from decimal import Decimal
-
-from MySQLdb._mysql import string_literal
-from MySQLdb.constants import FIELD_TYPE, FLAG
-from MySQLdb.times import (
-    Date,
-    DateTimeType,
-    DateTime2literal,
-    DateTimeDeltaType,
-    DateTimeDelta2literal,
-    DateTime_or_None,
-    TimeDelta_or_None,
-    Date_or_None,
-)
-from MySQLdb._exceptions import ProgrammingError
-
-import array
-
-NoneType = type(None)
-
-try:
-    ArrayType = array.ArrayType
-except AttributeError:
-    ArrayType = array.array
-
-
-def Bool2Str(s, d):
-    return b"1" if s else b"0"
-
-
-def Set2Str(s, d):
-    # Only support ascii string.  Not tested.
-    return string_literal(",".join(s))
-
-
-def Thing2Str(s, d):
-    """Convert something into a string via str()."""
-    return str(s)
-
-
-def Float2Str(o, d):
-    s = repr(o)
-    if s in ("inf", "-inf", "nan"):
-        raise ProgrammingError("%s can not be used with MySQL" % s)
-    if "e" not in s:
-        s += "e0"
-    return s
-
-
-def None2NULL(o, d):
-    """Convert None to NULL."""
-    return b"NULL"
-
-
-def Thing2Literal(o, d):
-    """Convert something into a SQL string literal.  If using
-    MySQL-3.23 or newer, string_literal() is a method of the
-    _mysql.MYSQL object, and this function will be overridden with
-    that method when the connection is created."""
-    return string_literal(o)
-
-
-def Decimal2Literal(o, d):
-    return format(o, "f")
-
-
-def array2Str(o, d):
-    return Thing2Literal(o.tostring(), d)
-
-
-# bytes or str regarding to BINARY_FLAG.
-_bytes_or_str = ((FLAG.BINARY, bytes), (None, str))
-
-conversions = {
-    int: Thing2Str,
-    float: Float2Str,
-    NoneType: None2NULL,
-    ArrayType: array2Str,
-    bool: Bool2Str,
-    Date: Thing2Literal,
-    DateTimeType: DateTime2literal,
-    DateTimeDeltaType: DateTimeDelta2literal,
-    set: Set2Str,
-    Decimal: Decimal2Literal,
-    FIELD_TYPE.TINY: int,
-    FIELD_TYPE.SHORT: int,
-    FIELD_TYPE.LONG: int,
-    FIELD_TYPE.FLOAT: float,
-    FIELD_TYPE.DOUBLE: float,
-    FIELD_TYPE.DECIMAL: Decimal,
-    FIELD_TYPE.NEWDECIMAL: Decimal,
-    FIELD_TYPE.LONGLONG: int,
-    FIELD_TYPE.INT24: int,
-    FIELD_TYPE.YEAR: int,
-    FIELD_TYPE.TIMESTAMP: DateTime_or_None,
-    FIELD_TYPE.DATETIME: DateTime_or_None,
-    FIELD_TYPE.TIME: TimeDelta_or_None,
-    FIELD_TYPE.DATE: Date_or_None,
-    FIELD_TYPE.TINY_BLOB: bytes,
-    FIELD_TYPE.MEDIUM_BLOB: bytes,
-    FIELD_TYPE.LONG_BLOB: bytes,
-    FIELD_TYPE.BLOB: bytes,
-    FIELD_TYPE.STRING: bytes,
-    FIELD_TYPE.VAR_STRING: bytes,
-    FIELD_TYPE.VARCHAR: bytes,
-    FIELD_TYPE.JSON: bytes,
-}
+"""MySQLdb type conversion module
+
+This module handles all the type conversions for MySQL. If the default
+type conversions aren't what you need, you can make your own. The
+dictionary conversions maps some kind of type to a conversion function
+which returns the corresponding value:
+
+Key: FIELD_TYPE.* (from MySQLdb.constants)
+
+Conversion function:
+
+    Arguments: string
+
+    Returns: Python object
+
+Key: Python type object (from types) or class
+
+Conversion function:
+
+    Arguments: Python object of indicated type or class AND
+               conversion dictionary
+
+    Returns: SQL literal value
+
+    Notes: Most conversion functions can ignore the dictionary, but
+           it is a required parameter. It is necessary for converting
+           things like sequences and instances.
+
+Don't modify conversions if you can avoid it. Instead, make copies
+(with the copy() method), modify the copies, and then pass them to
+MySQL.connect().
+"""
+from decimal import Decimal
+
+from MySQLdb._mysql import string_literal
+from MySQLdb.constants import FIELD_TYPE, FLAG
+from MySQLdb.times import (
+    Date,
+    DateTimeType,
+    DateTime2literal,
+    DateTimeDeltaType,
+    DateTimeDelta2literal,
+    DateTime_or_None,
+    TimeDelta_or_None,
+    Date_or_None,
+)
+from MySQLdb._exceptions import ProgrammingError
+
+import array
+
+NoneType = type(None)
+
+try:
+    ArrayType = array.ArrayType
+except AttributeError:
+    ArrayType = array.array
+
+
+def Bool2Str(s, d):
+    return b"1" if s else b"0"
+
+
+def Set2Str(s, d):
+    # Only support ascii string.  Not tested.
+    return string_literal(",".join(s))
+
+
+def Thing2Str(s, d):
+    """Convert something into a string via str()."""
+    return str(s)
+
+
+def Float2Str(o, d):
+    s = repr(o)
+    if s in ("inf", "-inf", "nan"):
+        raise ProgrammingError("%s can not be used with MySQL" % s)
+    if "e" not in s:
+        s += "e0"
+    return s
+
+
+def None2NULL(o, d):
+    """Convert None to NULL."""
+    return b"NULL"
+
+
+def Thing2Literal(o, d):
+    """Convert something into a SQL string literal.  If using
+    MySQL-3.23 or newer, string_literal() is a method of the
+    _mysql.MYSQL object, and this function will be overridden with
+    that method when the connection is created."""
+    return string_literal(o)
+
+
+def Decimal2Literal(o, d):
+    return format(o, "f")
+
+
+def array2Str(o, d):
+    return Thing2Literal(o.tostring(), d)
+
+
+# bytes or str regarding to BINARY_FLAG.
+_bytes_or_str = ((FLAG.BINARY, bytes), (None, str))
+
+conversions = {
+    int: Thing2Str,
+    float: Float2Str,
+    NoneType: None2NULL,
+    ArrayType: array2Str,
+    bool: Bool2Str,
+    Date: Thing2Literal,
+    DateTimeType: DateTime2literal,
+    DateTimeDeltaType: DateTimeDelta2literal,
+    set: Set2Str,
+    Decimal: Decimal2Literal,
+    FIELD_TYPE.TINY: int,
+    FIELD_TYPE.SHORT: int,
+    FIELD_TYPE.LONG: int,
+    FIELD_TYPE.FLOAT: float,
+    FIELD_TYPE.DOUBLE: float,
+    FIELD_TYPE.DECIMAL: Decimal,
+    FIELD_TYPE.NEWDECIMAL: Decimal,
+    FIELD_TYPE.LONGLONG: int,
+    FIELD_TYPE.INT24: int,
+    FIELD_TYPE.YEAR: int,
+    FIELD_TYPE.TIMESTAMP: DateTime_or_None,
+    FIELD_TYPE.DATETIME: DateTime_or_None,
+    FIELD_TYPE.TIME: TimeDelta_or_None,
+    FIELD_TYPE.DATE: Date_or_None,
+    FIELD_TYPE.TINY_BLOB: bytes,
+    FIELD_TYPE.MEDIUM_BLOB: bytes,
+    FIELD_TYPE.LONG_BLOB: bytes,
+    FIELD_TYPE.BLOB: bytes,
+    FIELD_TYPE.STRING: bytes,
+    FIELD_TYPE.VAR_STRING: bytes,
+    FIELD_TYPE.VARCHAR: bytes,
+    FIELD_TYPE.JSON: bytes,
+}
```

### Comparing `mysqlclient-2.2.0/src/MySQLdb/cursors.py` & `mysqlclient-2.2.0rc1/src/MySQLdb/cursors.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,500 +1,500 @@
-"""MySQLdb Cursors
-
-This module implements Cursors of various types for MySQLdb. By
-default, MySQLdb uses the Cursor class.
-"""
-import re
-
-from ._exceptions import ProgrammingError
-
-
-#: Regular expression for ``Cursor.executemany```.
-#: executemany only supports simple bulk insert.
-#: You can use it to load large dataset.
-RE_INSERT_VALUES = re.compile(
-    "".join(
-        [
-            r"\s*((?:INSERT|REPLACE)\b.+\bVALUES?\s*)",
-            r"(\(\s*(?:%s|%\(.+\)s)\s*(?:,\s*(?:%s|%\(.+\)s)\s*)*\))",
-            r"(\s*(?:ON DUPLICATE.*)?);?\s*\Z",
-        ]
-    ),
-    re.IGNORECASE | re.DOTALL,
-)
-
-
-class BaseCursor:
-    """A base for Cursor classes. Useful attributes:
-
-    description
-        A tuple of DB API 7-tuples describing the columns in
-        the last executed query; see PEP-249 for details.
-
-    description_flags
-        Tuple of column flags for last query, one entry per column
-        in the result set. Values correspond to those in
-        MySQLdb.constants.FLAG. See MySQL documentation (C API)
-        for more information. Non-standard extension.
-
-    arraysize
-        default number of rows fetchmany() will fetch
-    """
-
-    #: Max statement size which :meth:`executemany` generates.
-    #:
-    #: Max size of allowed statement is max_allowed_packet - packet_header_size.
-    #: Default value of max_allowed_packet is 1048576.
-    max_stmt_length = 64 * 1024
-
-    from ._exceptions import (
-        MySQLError,
-        Warning,
-        Error,
-        InterfaceError,
-        DatabaseError,
-        DataError,
-        OperationalError,
-        IntegrityError,
-        InternalError,
-        ProgrammingError,
-        NotSupportedError,
-    )
-
-    connection = None
-
-    def __init__(self, connection):
-        self.connection = connection
-        self.description = None
-        self.description_flags = None
-        self.rowcount = 0
-        self.arraysize = 1
-        self._executed = None
-
-        self.lastrowid = None
-        self._result = None
-        self.rownumber = None
-        self._rows = None
-
-    def _discard(self):
-        self.description = None
-        self.description_flags = None
-        # Django uses some member after __exit__.
-        # So we keep rowcount and lastrowid here. They are cleared in Cursor._query().
-        # self.rowcount = 0
-        # self.lastrowid = None
-        self._rows = None
-        self.rownumber = None
-
-        if self._result:
-            self._result.discard()
-            self._result = None
-
-        con = self.connection
-        if con is None:
-            return
-        while con.next_result() == 0:  # -1 means no more data.
-            con.discard_result()
-
-    def close(self):
-        """Close the cursor. No further queries will be possible."""
-        try:
-            if self.connection is None:
-                return
-            self._discard()
-        finally:
-            self.connection = None
-            self._result = None
-
-    def __enter__(self):
-        return self
-
-    def __exit__(self, *exc_info):
-        del exc_info
-        self.close()
-
-    def _check_executed(self):
-        if not self._executed:
-            raise ProgrammingError("execute() first")
-
-    def nextset(self):
-        """Advance to the next result set.
-
-        Returns None if there are no more result sets.
-        """
-        if self._executed:
-            self.fetchall()
-
-        db = self._get_db()
-        nr = db.next_result()
-        if nr == -1:
-            return None
-        self._do_get_result(db)
-        self._post_get_result()
-        return 1
-
-    def _do_get_result(self, db):
-        self._result = result = self._get_result()
-        if result is None:
-            self.description = self.description_flags = None
-        else:
-            self.description = result.describe()
-            self.description_flags = result.field_flags()
-
-        self.rowcount = db.affected_rows()
-        self.rownumber = 0
-        self.lastrowid = db.insert_id()
-
-    def _post_get_result(self):
-        pass
-
-    def setinputsizes(self, *args):
-        """Does nothing, required by DB API."""
-
-    def setoutputsizes(self, *args):
-        """Does nothing, required by DB API."""
-
-    def _get_db(self):
-        con = self.connection
-        if con is None:
-            raise ProgrammingError("cursor closed")
-        return con
-
-    def execute(self, query, args=None):
-        """Execute a query.
-
-        query -- string, query to execute on server
-        args -- optional sequence or mapping, parameters to use with query.
-
-        Note: If args is a sequence, then %s must be used as the
-        parameter placeholder in the query. If a mapping is used,
-        %(key)s must be used as the placeholder.
-
-        Returns integer represents rows affected, if any
-        """
-        self._discard()
-
-        mogrified_query = self._mogrify(query, args)
-
-        assert isinstance(mogrified_query, (bytes, bytearray))
-        res = self._query(mogrified_query)
-        return res
-
-    def _mogrify(self, query, args=None):
-        """Return query after binding args."""
-        db = self._get_db()
-
-        if isinstance(query, str):
-            query = query.encode(db.encoding)
-
-        if args is not None:
-            if isinstance(args, dict):
-                nargs = {}
-                for key, item in args.items():
-                    if isinstance(key, str):
-                        key = key.encode(db.encoding)
-                    nargs[key] = db.literal(item)
-                args = nargs
-            else:
-                args = tuple(map(db.literal, args))
-            try:
-                query = query % args
-            except TypeError as m:
-                raise ProgrammingError(str(m))
-
-        return query
-
-    def mogrify(self, query, args=None):
-        """Return query after binding args.
-
-        query -- string, query to mogrify
-        args -- optional sequence or mapping, parameters to use with query.
-
-        Note: If args is a sequence, then %s must be used as the
-        parameter placeholder in the query. If a mapping is used,
-        %(key)s must be used as the placeholder.
-
-        Returns string representing query that would be executed by the server
-        """
-        return self._mogrify(query, args).decode(self._get_db().encoding)
-
-    def executemany(self, query, args):
-        # type: (str, list) -> int
-        """Execute a multi-row query.
-
-        :param query: query to execute on server
-        :param args:  Sequence of sequences or mappings.  It is used as parameter.
-        :return: Number of rows affected, if any.
-
-        This method improves performance on multiple-row INSERT and
-        REPLACE. Otherwise it is equivalent to looping over args with
-        execute().
-        """
-        if not args:
-            return
-
-        m = RE_INSERT_VALUES.match(query)
-        if m:
-            q_prefix = m.group(1) % ()
-            q_values = m.group(2).rstrip()
-            q_postfix = m.group(3) or ""
-            assert q_values[0] == "(" and q_values[-1] == ")"
-            return self._do_execute_many(
-                q_prefix,
-                q_values,
-                q_postfix,
-                args,
-                self.max_stmt_length,
-                self._get_db().encoding,
-            )
-
-        self.rowcount = sum(self.execute(query, arg) for arg in args)
-        return self.rowcount
-
-    def _do_execute_many(
-        self, prefix, values, postfix, args, max_stmt_length, encoding
-    ):
-        if isinstance(prefix, str):
-            prefix = prefix.encode(encoding)
-        if isinstance(values, str):
-            values = values.encode(encoding)
-        if isinstance(postfix, str):
-            postfix = postfix.encode(encoding)
-        sql = bytearray(prefix)
-        args = iter(args)
-        v = self._mogrify(values, next(args))
-        sql += v
-        rows = 0
-        for arg in args:
-            v = self._mogrify(values, arg)
-            if len(sql) + len(v) + len(postfix) + 1 > max_stmt_length:
-                rows += self.execute(sql + postfix)
-                sql = bytearray(prefix)
-            else:
-                sql += b","
-            sql += v
-        rows += self.execute(sql + postfix)
-        self.rowcount = rows
-        return rows
-
-    def callproc(self, procname, args=()):
-        """Execute stored procedure procname with args
-
-        procname -- string, name of procedure to execute on server
-
-        args -- Sequence of parameters to use with procedure
-
-        Returns the original args.
-
-        Compatibility warning: PEP-249 specifies that any modified
-        parameters must be returned. This is currently impossible
-        as they are only available by storing them in a server
-        variable and then retrieved by a query. Since stored
-        procedures return zero or more result sets, there is no
-        reliable way to get at OUT or INOUT parameters via callproc.
-        The server variables are named @_procname_n, where procname
-        is the parameter above and n is the position of the parameter
-        (from zero). Once all result sets generated by the procedure
-        have been fetched, you can issue a SELECT @_procname_0, ...
-        query using .execute() to get any OUT or INOUT values.
-
-        Compatibility warning: The act of calling a stored procedure
-        itself creates an empty result set. This appears after any
-        result sets generated by the procedure. This is non-standard
-        behavior with respect to the DB-API. Be sure to use nextset()
-        to advance through all result sets; otherwise you may get
-        disconnected.
-        """
-        db = self._get_db()
-        if isinstance(procname, str):
-            procname = procname.encode(db.encoding)
-        if args:
-            fmt = b"@_" + procname + b"_%d=%s"
-            q = b"SET %s" % b",".join(
-                fmt % (index, db.literal(arg)) for index, arg in enumerate(args)
-            )
-            self._query(q)
-            self.nextset()
-
-        q = b"CALL %s(%s)" % (
-            procname,
-            b",".join([b"@_%s_%d" % (procname, i) for i in range(len(args))]),
-        )
-        self._query(q)
-        return args
-
-    def _query(self, q):
-        db = self._get_db()
-        self._result = None
-        self.rowcount = None
-        self.lastrowid = None
-        db.query(q)
-        self._do_get_result(db)
-        self._post_get_result()
-        self._executed = q
-        return self.rowcount
-
-    def _fetch_row(self, size=1):
-        if not self._result:
-            return ()
-        return self._result.fetch_row(size, self._fetch_type)
-
-    def __iter__(self):
-        return iter(self.fetchone, None)
-
-    Warning = Warning
-    Error = Error
-    InterfaceError = InterfaceError
-    DatabaseError = DatabaseError
-    DataError = DataError
-    OperationalError = OperationalError
-    IntegrityError = IntegrityError
-    InternalError = InternalError
-    ProgrammingError = ProgrammingError
-    NotSupportedError = NotSupportedError
-
-
-class CursorStoreResultMixIn:
-    """This is a MixIn class which causes the entire result set to be
-    stored on the client side, i.e. it uses mysql_store_result(). If the
-    result set can be very large, consider adding a LIMIT clause to your
-    query, or using CursorUseResultMixIn instead."""
-
-    def _get_result(self):
-        return self._get_db().store_result()
-
-    def _post_get_result(self):
-        self._rows = self._fetch_row(0)
-        self._result = None
-
-    def fetchone(self):
-        """Fetches a single row from the cursor. None indicates that
-        no more rows are available."""
-        self._check_executed()
-        if self.rownumber >= len(self._rows):
-            return None
-        result = self._rows[self.rownumber]
-        self.rownumber = self.rownumber + 1
-        return result
-
-    def fetchmany(self, size=None):
-        """Fetch up to size rows from the cursor. Result set may be smaller
-        than size. If size is not defined, cursor.arraysize is used."""
-        self._check_executed()
-        end = self.rownumber + (size or self.arraysize)
-        result = self._rows[self.rownumber : end]
-        self.rownumber = min(end, len(self._rows))
-        return result
-
-    def fetchall(self):
-        """Fetches all available rows from the cursor."""
-        self._check_executed()
-        if self.rownumber:
-            result = self._rows[self.rownumber :]
-        else:
-            result = self._rows
-        self.rownumber = len(self._rows)
-        return result
-
-    def scroll(self, value, mode="relative"):
-        """Scroll the cursor in the result set to a new position according
-        to mode.
-
-        If mode is 'relative' (default), value is taken as offset to
-        the current position in the result set, if set to 'absolute',
-        value states an absolute target position."""
-        self._check_executed()
-        if mode == "relative":
-            r = self.rownumber + value
-        elif mode == "absolute":
-            r = value
-        else:
-            raise ProgrammingError("unknown scroll mode %s" % repr(mode))
-        if r < 0 or r >= len(self._rows):
-            raise IndexError("out of range")
-        self.rownumber = r
-
-    def __iter__(self):
-        self._check_executed()
-        result = self.rownumber and self._rows[self.rownumber :] or self._rows
-        return iter(result)
-
-
-class CursorUseResultMixIn:
-
-    """This is a MixIn class which causes the result set to be stored
-    in the server and sent row-by-row to client side, i.e. it uses
-    mysql_use_result(). You MUST retrieve the entire result set and
-    close() the cursor before additional queries can be performed on
-    the connection."""
-
-    def _get_result(self):
-        return self._get_db().use_result()
-
-    def fetchone(self):
-        """Fetches a single row from the cursor."""
-        self._check_executed()
-        r = self._fetch_row(1)
-        if not r:
-            return None
-        self.rownumber = self.rownumber + 1
-        return r[0]
-
-    def fetchmany(self, size=None):
-        """Fetch up to size rows from the cursor. Result set may be smaller
-        than size. If size is not defined, cursor.arraysize is used."""
-        self._check_executed()
-        r = self._fetch_row(size or self.arraysize)
-        self.rownumber = self.rownumber + len(r)
-        return r
-
-    def fetchall(self):
-        """Fetches all available rows from the cursor."""
-        self._check_executed()
-        r = self._fetch_row(0)
-        self.rownumber = self.rownumber + len(r)
-        return r
-
-    def __iter__(self):
-        return self
-
-    def next(self):
-        row = self.fetchone()
-        if row is None:
-            raise StopIteration
-        return row
-
-    __next__ = next
-
-
-class CursorTupleRowsMixIn:
-    """This is a MixIn class that causes all rows to be returned as tuples,
-    which is the standard form required by DB API."""
-
-    _fetch_type = 0
-
-
-class CursorDictRowsMixIn:
-    """This is a MixIn class that causes all rows to be returned as
-    dictionaries. This is a non-standard feature."""
-
-    _fetch_type = 1
-
-
-class Cursor(CursorStoreResultMixIn, CursorTupleRowsMixIn, BaseCursor):
-    """This is the standard Cursor class that returns rows as tuples
-    and stores the result set in the client."""
-
-
-class DictCursor(CursorStoreResultMixIn, CursorDictRowsMixIn, BaseCursor):
-    """This is a Cursor class that returns rows as dictionaries and
-    stores the result set in the client."""
-
-
-class SSCursor(CursorUseResultMixIn, CursorTupleRowsMixIn, BaseCursor):
-    """This is a Cursor class that returns rows as tuples and stores
-    the result set in the server."""
-
-
-class SSDictCursor(CursorUseResultMixIn, CursorDictRowsMixIn, BaseCursor):
-    """This is a Cursor class that returns rows as dictionaries and
-    stores the result set in the server."""
+"""MySQLdb Cursors
+
+This module implements Cursors of various types for MySQLdb. By
+default, MySQLdb uses the Cursor class.
+"""
+import re
+
+from ._exceptions import ProgrammingError
+
+
+#: Regular expression for ``Cursor.executemany```.
+#: executemany only supports simple bulk insert.
+#: You can use it to load large dataset.
+RE_INSERT_VALUES = re.compile(
+    "".join(
+        [
+            r"\s*((?:INSERT|REPLACE)\b.+\bVALUES?\s*)",
+            r"(\(\s*(?:%s|%\(.+\)s)\s*(?:,\s*(?:%s|%\(.+\)s)\s*)*\))",
+            r"(\s*(?:ON DUPLICATE.*)?);?\s*\Z",
+        ]
+    ),
+    re.IGNORECASE | re.DOTALL,
+)
+
+
+class BaseCursor:
+    """A base for Cursor classes. Useful attributes:
+
+    description
+        A tuple of DB API 7-tuples describing the columns in
+        the last executed query; see PEP-249 for details.
+
+    description_flags
+        Tuple of column flags for last query, one entry per column
+        in the result set. Values correspond to those in
+        MySQLdb.constants.FLAG. See MySQL documentation (C API)
+        for more information. Non-standard extension.
+
+    arraysize
+        default number of rows fetchmany() will fetch
+    """
+
+    #: Max statement size which :meth:`executemany` generates.
+    #:
+    #: Max size of allowed statement is max_allowed_packet - packet_header_size.
+    #: Default value of max_allowed_packet is 1048576.
+    max_stmt_length = 64 * 1024
+
+    from ._exceptions import (
+        MySQLError,
+        Warning,
+        Error,
+        InterfaceError,
+        DatabaseError,
+        DataError,
+        OperationalError,
+        IntegrityError,
+        InternalError,
+        ProgrammingError,
+        NotSupportedError,
+    )
+
+    connection = None
+
+    def __init__(self, connection):
+        self.connection = connection
+        self.description = None
+        self.description_flags = None
+        self.rowcount = 0
+        self.arraysize = 1
+        self._executed = None
+
+        self.lastrowid = None
+        self._result = None
+        self.rownumber = None
+        self._rows = None
+
+    def _discard(self):
+        self.description = None
+        self.description_flags = None
+        # Django uses some member after __exit__.
+        # So we keep rowcount and lastrowid here. They are cleared in Cursor._query().
+        # self.rowcount = 0
+        # self.lastrowid = None
+        self._rows = None
+        self.rownumber = None
+
+        if self._result:
+            self._result.discard()
+            self._result = None
+
+        con = self.connection
+        if con is None:
+            return
+        while con.next_result() == 0:  # -1 means no more data.
+            con.discard_result()
+
+    def close(self):
+        """Close the cursor. No further queries will be possible."""
+        try:
+            if self.connection is None:
+                return
+            self._discard()
+        finally:
+            self.connection = None
+            self._result = None
+
+    def __enter__(self):
+        return self
+
+    def __exit__(self, *exc_info):
+        del exc_info
+        self.close()
+
+    def _check_executed(self):
+        if not self._executed:
+            raise ProgrammingError("execute() first")
+
+    def nextset(self):
+        """Advance to the next result set.
+
+        Returns None if there are no more result sets.
+        """
+        if self._executed:
+            self.fetchall()
+
+        db = self._get_db()
+        nr = db.next_result()
+        if nr == -1:
+            return None
+        self._do_get_result(db)
+        self._post_get_result()
+        return 1
+
+    def _do_get_result(self, db):
+        self._result = result = self._get_result()
+        if result is None:
+            self.description = self.description_flags = None
+        else:
+            self.description = result.describe()
+            self.description_flags = result.field_flags()
+
+        self.rowcount = db.affected_rows()
+        self.rownumber = 0
+        self.lastrowid = db.insert_id()
+
+    def _post_get_result(self):
+        pass
+
+    def setinputsizes(self, *args):
+        """Does nothing, required by DB API."""
+
+    def setoutputsizes(self, *args):
+        """Does nothing, required by DB API."""
+
+    def _get_db(self):
+        con = self.connection
+        if con is None:
+            raise ProgrammingError("cursor closed")
+        return con
+
+    def execute(self, query, args=None):
+        """Execute a query.
+
+        query -- string, query to execute on server
+        args -- optional sequence or mapping, parameters to use with query.
+
+        Note: If args is a sequence, then %s must be used as the
+        parameter placeholder in the query. If a mapping is used,
+        %(key)s must be used as the placeholder.
+
+        Returns integer represents rows affected, if any
+        """
+        self._discard()
+
+        mogrified_query = self._mogrify(query, args)
+
+        assert isinstance(mogrified_query, (bytes, bytearray))
+        res = self._query(mogrified_query)
+        return res
+
+    def _mogrify(self, query, args=None):
+        """Return query after binding args."""
+        db = self._get_db()
+
+        if isinstance(query, str):
+            query = query.encode(db.encoding)
+
+        if args is not None:
+            if isinstance(args, dict):
+                nargs = {}
+                for key, item in args.items():
+                    if isinstance(key, str):
+                        key = key.encode(db.encoding)
+                    nargs[key] = db.literal(item)
+                args = nargs
+            else:
+                args = tuple(map(db.literal, args))
+            try:
+                query = query % args
+            except TypeError as m:
+                raise ProgrammingError(str(m))
+
+        return query
+
+    def mogrify(self, query, args=None):
+        """Return query after binding args.
+
+        query -- string, query to mogrify
+        args -- optional sequence or mapping, parameters to use with query.
+
+        Note: If args is a sequence, then %s must be used as the
+        parameter placeholder in the query. If a mapping is used,
+        %(key)s must be used as the placeholder.
+
+        Returns string representing query that would be executed by the server
+        """
+        return self._mogrify(query, args).decode(self._get_db().encoding)
+
+    def executemany(self, query, args):
+        # type: (str, list) -> int
+        """Execute a multi-row query.
+
+        :param query: query to execute on server
+        :param args:  Sequence of sequences or mappings.  It is used as parameter.
+        :return: Number of rows affected, if any.
+
+        This method improves performance on multiple-row INSERT and
+        REPLACE. Otherwise it is equivalent to looping over args with
+        execute().
+        """
+        if not args:
+            return
+
+        m = RE_INSERT_VALUES.match(query)
+        if m:
+            q_prefix = m.group(1) % ()
+            q_values = m.group(2).rstrip()
+            q_postfix = m.group(3) or ""
+            assert q_values[0] == "(" and q_values[-1] == ")"
+            return self._do_execute_many(
+                q_prefix,
+                q_values,
+                q_postfix,
+                args,
+                self.max_stmt_length,
+                self._get_db().encoding,
+            )
+
+        self.rowcount = sum(self.execute(query, arg) for arg in args)
+        return self.rowcount
+
+    def _do_execute_many(
+        self, prefix, values, postfix, args, max_stmt_length, encoding
+    ):
+        if isinstance(prefix, str):
+            prefix = prefix.encode(encoding)
+        if isinstance(values, str):
+            values = values.encode(encoding)
+        if isinstance(postfix, str):
+            postfix = postfix.encode(encoding)
+        sql = bytearray(prefix)
+        args = iter(args)
+        v = self._mogrify(values, next(args))
+        sql += v
+        rows = 0
+        for arg in args:
+            v = self._mogrify(values, arg)
+            if len(sql) + len(v) + len(postfix) + 1 > max_stmt_length:
+                rows += self.execute(sql + postfix)
+                sql = bytearray(prefix)
+            else:
+                sql += b","
+            sql += v
+        rows += self.execute(sql + postfix)
+        self.rowcount = rows
+        return rows
+
+    def callproc(self, procname, args=()):
+        """Execute stored procedure procname with args
+
+        procname -- string, name of procedure to execute on server
+
+        args -- Sequence of parameters to use with procedure
+
+        Returns the original args.
+
+        Compatibility warning: PEP-249 specifies that any modified
+        parameters must be returned. This is currently impossible
+        as they are only available by storing them in a server
+        variable and then retrieved by a query. Since stored
+        procedures return zero or more result sets, there is no
+        reliable way to get at OUT or INOUT parameters via callproc.
+        The server variables are named @_procname_n, where procname
+        is the parameter above and n is the position of the parameter
+        (from zero). Once all result sets generated by the procedure
+        have been fetched, you can issue a SELECT @_procname_0, ...
+        query using .execute() to get any OUT or INOUT values.
+
+        Compatibility warning: The act of calling a stored procedure
+        itself creates an empty result set. This appears after any
+        result sets generated by the procedure. This is non-standard
+        behavior with respect to the DB-API. Be sure to use nextset()
+        to advance through all result sets; otherwise you may get
+        disconnected.
+        """
+        db = self._get_db()
+        if isinstance(procname, str):
+            procname = procname.encode(db.encoding)
+        if args:
+            fmt = b"@_" + procname + b"_%d=%s"
+            q = b"SET %s" % b",".join(
+                fmt % (index, db.literal(arg)) for index, arg in enumerate(args)
+            )
+            self._query(q)
+            self.nextset()
+
+        q = b"CALL %s(%s)" % (
+            procname,
+            b",".join([b"@_%s_%d" % (procname, i) for i in range(len(args))]),
+        )
+        self._query(q)
+        return args
+
+    def _query(self, q):
+        db = self._get_db()
+        self._result = None
+        self.rowcount = None
+        self.lastrowid = None
+        db.query(q)
+        self._do_get_result(db)
+        self._post_get_result()
+        self._executed = q
+        return self.rowcount
+
+    def _fetch_row(self, size=1):
+        if not self._result:
+            return ()
+        return self._result.fetch_row(size, self._fetch_type)
+
+    def __iter__(self):
+        return iter(self.fetchone, None)
+
+    Warning = Warning
+    Error = Error
+    InterfaceError = InterfaceError
+    DatabaseError = DatabaseError
+    DataError = DataError
+    OperationalError = OperationalError
+    IntegrityError = IntegrityError
+    InternalError = InternalError
+    ProgrammingError = ProgrammingError
+    NotSupportedError = NotSupportedError
+
+
+class CursorStoreResultMixIn:
+    """This is a MixIn class which causes the entire result set to be
+    stored on the client side, i.e. it uses mysql_store_result(). If the
+    result set can be very large, consider adding a LIMIT clause to your
+    query, or using CursorUseResultMixIn instead."""
+
+    def _get_result(self):
+        return self._get_db().store_result()
+
+    def _post_get_result(self):
+        self._rows = self._fetch_row(0)
+        self._result = None
+
+    def fetchone(self):
+        """Fetches a single row from the cursor. None indicates that
+        no more rows are available."""
+        self._check_executed()
+        if self.rownumber >= len(self._rows):
+            return None
+        result = self._rows[self.rownumber]
+        self.rownumber = self.rownumber + 1
+        return result
+
+    def fetchmany(self, size=None):
+        """Fetch up to size rows from the cursor. Result set may be smaller
+        than size. If size is not defined, cursor.arraysize is used."""
+        self._check_executed()
+        end = self.rownumber + (size or self.arraysize)
+        result = self._rows[self.rownumber : end]
+        self.rownumber = min(end, len(self._rows))
+        return result
+
+    def fetchall(self):
+        """Fetches all available rows from the cursor."""
+        self._check_executed()
+        if self.rownumber:
+            result = self._rows[self.rownumber :]
+        else:
+            result = self._rows
+        self.rownumber = len(self._rows)
+        return result
+
+    def scroll(self, value, mode="relative"):
+        """Scroll the cursor in the result set to a new position according
+        to mode.
+
+        If mode is 'relative' (default), value is taken as offset to
+        the current position in the result set, if set to 'absolute',
+        value states an absolute target position."""
+        self._check_executed()
+        if mode == "relative":
+            r = self.rownumber + value
+        elif mode == "absolute":
+            r = value
+        else:
+            raise ProgrammingError("unknown scroll mode %s" % repr(mode))
+        if r < 0 or r >= len(self._rows):
+            raise IndexError("out of range")
+        self.rownumber = r
+
+    def __iter__(self):
+        self._check_executed()
+        result = self.rownumber and self._rows[self.rownumber :] or self._rows
+        return iter(result)
+
+
+class CursorUseResultMixIn:
+
+    """This is a MixIn class which causes the result set to be stored
+    in the server and sent row-by-row to client side, i.e. it uses
+    mysql_use_result(). You MUST retrieve the entire result set and
+    close() the cursor before additional queries can be performed on
+    the connection."""
+
+    def _get_result(self):
+        return self._get_db().use_result()
+
+    def fetchone(self):
+        """Fetches a single row from the cursor."""
+        self._check_executed()
+        r = self._fetch_row(1)
+        if not r:
+            return None
+        self.rownumber = self.rownumber + 1
+        return r[0]
+
+    def fetchmany(self, size=None):
+        """Fetch up to size rows from the cursor. Result set may be smaller
+        than size. If size is not defined, cursor.arraysize is used."""
+        self._check_executed()
+        r = self._fetch_row(size or self.arraysize)
+        self.rownumber = self.rownumber + len(r)
+        return r
+
+    def fetchall(self):
+        """Fetches all available rows from the cursor."""
+        self._check_executed()
+        r = self._fetch_row(0)
+        self.rownumber = self.rownumber + len(r)
+        return r
+
+    def __iter__(self):
+        return self
+
+    def next(self):
+        row = self.fetchone()
+        if row is None:
+            raise StopIteration
+        return row
+
+    __next__ = next
+
+
+class CursorTupleRowsMixIn:
+    """This is a MixIn class that causes all rows to be returned as tuples,
+    which is the standard form required by DB API."""
+
+    _fetch_type = 0
+
+
+class CursorDictRowsMixIn:
+    """This is a MixIn class that causes all rows to be returned as
+    dictionaries. This is a non-standard feature."""
+
+    _fetch_type = 1
+
+
+class Cursor(CursorStoreResultMixIn, CursorTupleRowsMixIn, BaseCursor):
+    """This is the standard Cursor class that returns rows as tuples
+    and stores the result set in the client."""
+
+
+class DictCursor(CursorStoreResultMixIn, CursorDictRowsMixIn, BaseCursor):
+    """This is a Cursor class that returns rows as dictionaries and
+    stores the result set in the client."""
+
+
+class SSCursor(CursorUseResultMixIn, CursorTupleRowsMixIn, BaseCursor):
+    """This is a Cursor class that returns rows as tuples and stores
+    the result set in the server."""
+
+
+class SSDictCursor(CursorUseResultMixIn, CursorDictRowsMixIn, BaseCursor):
+    """This is a Cursor class that returns rows as dictionaries and
+    stores the result set in the server."""
```

### Comparing `mysqlclient-2.2.0/src/MySQLdb/times.py` & `mysqlclient-2.2.0rc1/src/MySQLdb/times.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,150 +1,150 @@
-"""times module
-
-This module provides some Date and Time classes for dealing with MySQL data.
-
-Use Python datetime module to handle date and time columns.
-"""
-from time import localtime
-from datetime import date, datetime, time, timedelta
-from MySQLdb._mysql import string_literal
-
-Date = date
-Time = time
-TimeDelta = timedelta
-Timestamp = datetime
-
-DateTimeDeltaType = timedelta
-DateTimeType = datetime
-
-
-def DateFromTicks(ticks):
-    """Convert UNIX ticks into a date instance."""
-    return date(*localtime(ticks)[:3])
-
-
-def TimeFromTicks(ticks):
-    """Convert UNIX ticks into a time instance."""
-    return time(*localtime(ticks)[3:6])
-
-
-def TimestampFromTicks(ticks):
-    """Convert UNIX ticks into a datetime instance."""
-    return datetime(*localtime(ticks)[:6])
-
-
-format_TIME = format_DATE = str
-
-
-def format_TIMEDELTA(v):
-    seconds = int(v.seconds) % 60
-    minutes = int(v.seconds // 60) % 60
-    hours = int(v.seconds // 3600) % 24
-    return "%d %d:%d:%d" % (v.days, hours, minutes, seconds)
-
-
-def format_TIMESTAMP(d):
-    """
-    :type d: datetime.datetime
-    """
-    if d.microsecond:
-        fmt = " ".join(
-            [
-                "{0.year:04}-{0.month:02}-{0.day:02}",
-                "{0.hour:02}:{0.minute:02}:{0.second:02}.{0.microsecond:06}",
-            ]
-        )
-    else:
-        fmt = " ".join(
-            [
-                "{0.year:04}-{0.month:02}-{0.day:02}",
-                "{0.hour:02}:{0.minute:02}:{0.second:02}",
-            ]
-        )
-    return fmt.format(d)
-
-
-def DateTime_or_None(s):
-    try:
-        if len(s) < 11:
-            return Date_or_None(s)
-
-        micros = s[20:]
-
-        if len(micros) == 0:
-            # 12:00:00
-            micros = 0
-        elif len(micros) < 7:
-            # 12:00:00.123456
-            micros = int(micros) * 10 ** (6 - len(micros))
-        else:
-            return None
-
-        return datetime(
-            int(s[:4]),  # year
-            int(s[5:7]),  # month
-            int(s[8:10]),  # day
-            int(s[11:13] or 0),  # hour
-            int(s[14:16] or 0),  # minute
-            int(s[17:19] or 0),  # second
-            micros,  # microsecond
-        )
-    except ValueError:
-        return None
-
-
-def TimeDelta_or_None(s):
-    try:
-        h, m, s = s.split(":")
-        if "." in s:
-            s, ms = s.split(".")
-            ms = ms.ljust(6, "0")
-        else:
-            ms = 0
-        if h[0] == "-":
-            negative = True
-        else:
-            negative = False
-        h, m, s, ms = abs(int(h)), int(m), int(s), int(ms)
-        td = timedelta(hours=h, minutes=m, seconds=s, microseconds=ms)
-        if negative:
-            return -td
-        else:
-            return td
-    except ValueError:
-        # unpacking or int/float conversion failed
-        return None
-
-
-def Time_or_None(s):
-    try:
-        h, m, s = s.split(":")
-        if "." in s:
-            s, ms = s.split(".")
-            ms = ms.ljust(6, "0")
-        else:
-            ms = 0
-        h, m, s, ms = int(h), int(m), int(s), int(ms)
-        return time(hour=h, minute=m, second=s, microsecond=ms)
-    except ValueError:
-        return None
-
-
-def Date_or_None(s):
-    try:
-        return date(
-            int(s[:4]),
-            int(s[5:7]),
-            int(s[8:10]),
-        )  # year  # month  # day
-    except ValueError:
-        return None
-
-
-def DateTime2literal(d, c):
-    """Format a DateTime object as an ISO timestamp."""
-    return string_literal(format_TIMESTAMP(d))
-
-
-def DateTimeDelta2literal(d, c):
-    """Format a DateTimeDelta object as a time."""
-    return string_literal(format_TIMEDELTA(d))
+"""times module
+
+This module provides some Date and Time classes for dealing with MySQL data.
+
+Use Python datetime module to handle date and time columns.
+"""
+from time import localtime
+from datetime import date, datetime, time, timedelta
+from MySQLdb._mysql import string_literal
+
+Date = date
+Time = time
+TimeDelta = timedelta
+Timestamp = datetime
+
+DateTimeDeltaType = timedelta
+DateTimeType = datetime
+
+
+def DateFromTicks(ticks):
+    """Convert UNIX ticks into a date instance."""
+    return date(*localtime(ticks)[:3])
+
+
+def TimeFromTicks(ticks):
+    """Convert UNIX ticks into a time instance."""
+    return time(*localtime(ticks)[3:6])
+
+
+def TimestampFromTicks(ticks):
+    """Convert UNIX ticks into a datetime instance."""
+    return datetime(*localtime(ticks)[:6])
+
+
+format_TIME = format_DATE = str
+
+
+def format_TIMEDELTA(v):
+    seconds = int(v.seconds) % 60
+    minutes = int(v.seconds // 60) % 60
+    hours = int(v.seconds // 3600) % 24
+    return "%d %d:%d:%d" % (v.days, hours, minutes, seconds)
+
+
+def format_TIMESTAMP(d):
+    """
+    :type d: datetime.datetime
+    """
+    if d.microsecond:
+        fmt = " ".join(
+            [
+                "{0.year:04}-{0.month:02}-{0.day:02}",
+                "{0.hour:02}:{0.minute:02}:{0.second:02}.{0.microsecond:06}",
+            ]
+        )
+    else:
+        fmt = " ".join(
+            [
+                "{0.year:04}-{0.month:02}-{0.day:02}",
+                "{0.hour:02}:{0.minute:02}:{0.second:02}",
+            ]
+        )
+    return fmt.format(d)
+
+
+def DateTime_or_None(s):
+    try:
+        if len(s) < 11:
+            return Date_or_None(s)
+
+        micros = s[20:]
+
+        if len(micros) == 0:
+            # 12:00:00
+            micros = 0
+        elif len(micros) < 7:
+            # 12:00:00.123456
+            micros = int(micros) * 10 ** (6 - len(micros))
+        else:
+            return None
+
+        return datetime(
+            int(s[:4]),  # year
+            int(s[5:7]),  # month
+            int(s[8:10]),  # day
+            int(s[11:13] or 0),  # hour
+            int(s[14:16] or 0),  # minute
+            int(s[17:19] or 0),  # second
+            micros,  # microsecond
+        )
+    except ValueError:
+        return None
+
+
+def TimeDelta_or_None(s):
+    try:
+        h, m, s = s.split(":")
+        if "." in s:
+            s, ms = s.split(".")
+            ms = ms.ljust(6, "0")
+        else:
+            ms = 0
+        if h[0] == "-":
+            negative = True
+        else:
+            negative = False
+        h, m, s, ms = abs(int(h)), int(m), int(s), int(ms)
+        td = timedelta(hours=h, minutes=m, seconds=s, microseconds=ms)
+        if negative:
+            return -td
+        else:
+            return td
+    except ValueError:
+        # unpacking or int/float conversion failed
+        return None
+
+
+def Time_or_None(s):
+    try:
+        h, m, s = s.split(":")
+        if "." in s:
+            s, ms = s.split(".")
+            ms = ms.ljust(6, "0")
+        else:
+            ms = 0
+        h, m, s, ms = int(h), int(m), int(s), int(ms)
+        return time(hour=h, minute=m, second=s, microsecond=ms)
+    except ValueError:
+        return None
+
+
+def Date_or_None(s):
+    try:
+        return date(
+            int(s[:4]),
+            int(s[5:7]),
+            int(s[8:10]),
+        )  # year  # month  # day
+    except ValueError:
+        return None
+
+
+def DateTime2literal(d, c):
+    """Format a DateTime object as an ISO timestamp."""
+    return string_literal(format_TIMESTAMP(d))
+
+
+def DateTimeDelta2literal(d, c):
+    """Format a DateTimeDelta object as a time."""
+    return string_literal(format_TIMEDELTA(d))
```

### Comparing `mysqlclient-2.2.0/src/mysqlclient.egg-info/PKG-INFO` & `mysqlclient-2.2.0rc1/src/mysqlclient.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,130 +1,130 @@
-Metadata-Version: 2.1
-Name: mysqlclient
-Version: 2.2.0
-Summary: Python interface to MySQL
-Author-email: Inada Naoki <songofacandy@gmail.com>
-License: GNU General Public License v2 (GPLv2)
-Project-URL: Project, https://github.com/PyMySQL/mysqlclient
-Project-URL: Documentation, https://mysqlclient.readthedocs.io/
-Keywords: MySQL
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Other Environment
-Classifier: License :: OSI Approved :: GNU General Public License (GPL)
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows :: Windows NT/2000
-Classifier: Operating System :: OS Independent
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: Unix
-Classifier: Programming Language :: C
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Database
-Classifier: Topic :: Database :: Database Engines/Servers
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# mysqlclient
-
-This project is a fork of [MySQLdb1](https://github.com/farcepest/MySQLdb1).
-This project adds Python 3 support and fixed many bugs.
-
-* PyPI: https://pypi.org/project/mysqlclient/
-* GitHub: https://github.com/PyMySQL/mysqlclient
-
-
-## Support
-
-**Do Not use Github Issue Tracker to ask help.  OSS Maintainer is not free tech support**
-
-When your question looks relating to Python rather than MySQL:
-
-* Python mailing list [python-list](https://mail.python.org/mailman/listinfo/python-list)
-* Slack [pythondev.slack.com](https://pyslackers.com/web/slack)
-
-Or when you have question about MySQL:
-
-* [MySQL Community on Slack](https://lefred.be/mysql-community-on-slack/)
-
-
-## Install
-
-### Windows
-
-Building mysqlclient on Windows is very hard.
-But there are some binary wheels you can install easily.
-
-If binary wheels do not exist for your version of Python, it may be possible to
-build from source, but if this does not work, **do not come asking for support.**
-To build from source, download the
-[MariaDB C Connector](https://mariadb.com/downloads/#connectors) and install
-it. It must be installed in the default location
-(usually "C:\Program Files\MariaDB\MariaDB Connector C" or
-"C:\Program Files (x86)\MariaDB\MariaDB Connector C" for 32-bit). If you
-build the connector yourself or install it in a different location, set the
-environment variable `MYSQLCLIENT_CONNECTOR` before installing. Once you have
-the connector installed and an appropriate version of Visual Studio for your
-version of Python:
-
-```
-$ pip install mysqlclient
-```
-
-### macOS (Homebrew)
-
-Install MySQL and mysqlclient:
-
-```
-# Assume you are activating Python 3 venv
-$ brew install mysql pkg-config
-$ pip install mysqlclient
-```
-
-If you don't want to install MySQL server, you can use mysql-client instead:
-
-```
-# Assume you are activating Python 3 venv
-$ brew install mysql-client pkg-config
-$ export PKG_CONFIG_PATH="/opt/homebrew/opt/mysql-client/lib/pkgconfig"
-$ pip install mysqlclient
-```
-
-### Linux
-
-**Note that this is a basic step.  I can not support complete step for build for all
-environment.  If you can see some error, you should fix it by yourself, or ask for
-support in some user forum.  Don't file a issue on the issue tracker.**
-
-You may need to install the Python 3 and MySQL development headers and libraries like so:
-
-* `$ sudo apt-get install python3-dev default-libmysqlclient-dev build-essential`  # Debian / Ubuntu
-* `% sudo yum install python3-devel mysql-devel`  # Red Hat / CentOS
-
-Then you can install mysqlclient via pip now:
-
-```
-$ pip install mysqlclient
-```
-
-### Customize build (POSIX)
-
-mysqlclient uses `pkg-config --clfags --ldflags mysqlclient` by default for finding
-compiler/linker flags.
-
-You can use `MYSQLCLIENT_CFLAGS` and `MYSQLCLIENT_LDFLAGS` environment
-variables to customize compiler/linker options.
-
-```
-$ export MYSQLCLIENT_CFLAGS=`pkg-config mysqlclient --cflags`
-$ export MYSQLCLIENT_LDFLAGS=`pkg-config mysqlclient --libs`
-$ pip install mysqlclient
-```
-
-### Documentation
-
-Documentation is hosted on [Read The Docs](https://mysqlclient.readthedocs.io/)
+Metadata-Version: 2.1
+Name: mysqlclient
+Version: 2.2.0rc1
+Summary: Python interface to MySQL
+Author-email: Inada Naoki <songofacandy@gmail.com>
+License: GNU General Public License v2 (GPLv2)
+Project-URL: Project, https://github.com/PyMySQL/mysqlclient
+Project-URL: Documentation, https://mysqlclient.readthedocs.io/
+Keywords: MySQL
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Other Environment
+Classifier: License :: OSI Approved :: GNU General Public License (GPL)
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows :: Windows NT/2000
+Classifier: Operating System :: OS Independent
+Classifier: Operating System :: POSIX
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: Unix
+Classifier: Programming Language :: C
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Database
+Classifier: Topic :: Database :: Database Engines/Servers
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# mysqlclient
+
+This project is a fork of [MySQLdb1](https://github.com/farcepest/MySQLdb1).
+This project adds Python 3 support and fixed many bugs.
+
+* PyPI: https://pypi.org/project/mysqlclient/
+* GitHub: https://github.com/PyMySQL/mysqlclient
+
+
+## Support
+
+**Do Not use Github Issue Tracker to ask help.  OSS Maintainer is not free tech support**
+
+When your question looks relating to Python rather than MySQL:
+
+* Python mailing list [python-list](https://mail.python.org/mailman/listinfo/python-list)
+* Slack [pythondev.slack.com](https://pyslackers.com/web/slack)
+
+Or when you have question about MySQL:
+
+* [MySQL Community on Slack](https://lefred.be/mysql-community-on-slack/)
+
+
+## Install
+
+### Windows
+
+Building mysqlclient on Windows is very hard.
+But there are some binary wheels you can install easily.
+
+If binary wheels do not exist for your version of Python, it may be possible to
+build from source, but if this does not work, **do not come asking for support.**
+To build from source, download the
+[MariaDB C Connector](https://mariadb.com/downloads/#connectors) and install
+it. It must be installed in the default location
+(usually "C:\Program Files\MariaDB\MariaDB Connector C" or
+"C:\Program Files (x86)\MariaDB\MariaDB Connector C" for 32-bit). If you
+build the connector yourself or install it in a different location, set the
+environment variable `MYSQLCLIENT_CONNECTOR` before installing. Once you have
+the connector installed and an appropriate version of Visual Studio for your
+version of Python:
+
+```
+$ pip install mysqlclient
+```
+
+### macOS (Homebrew)
+
+Install MySQL and mysqlclient:
+
+```
+# Assume you are activating Python 3 venv
+$ brew install mysql pkg-config
+$ pip install mysqlclient
+```
+
+If you don't want to install MySQL server, you can use mysql-client instead:
+
+```
+# Assume you are activating Python 3 venv
+$ brew install mysql-client pkg-config
+$ export PKG_CONFIG_PATH="/opt/homebrew/opt/mysql-client/lib/pkgconfig"
+$ pip install mysqlclient
+```
+
+### Linux
+
+**Note that this is a basic step.  I can not support complete step for build for all
+environment.  If you can see some error, you should fix it by yourself, or ask for
+support in some user forum.  Don't file a issue on the issue tracker.**
+
+You may need to install the Python 3 and MySQL development headers and libraries like so:
+
+* `$ sudo apt-get install python3-dev default-libmysqlclient-dev build-essential`  # Debian / Ubuntu
+* `% sudo yum install python3-devel mysql-devel`  # Red Hat / CentOS
+
+Then you can install mysqlclient via pip now:
+
+```
+$ pip install mysqlclient
+```
+
+### Customize build (POSIX)
+
+mysqlclient uses `pkg-config --clfags --ldflags mysqlclient` by default for finding
+compiler/linker flags.
+
+You can use `MYSQLCLIENT_CFLAGS` and `MYSQLCLIENT_LDFLAGS` environment
+variables to customize compiler/linker options.
+
+```
+$ export MYSQLCLIENT_CFLAGS=`pkg-config mysqlclient --cflags`
+$ export MYSQLCLIENT_LDFLAGS=`pkg-config mysqlclient --libs`
+$ pip install mysqlclient
+```
+
+### Documentation
+
+Documentation is hosted on [Read The Docs](https://mysqlclient.readthedocs.io/)
```

### Comparing `mysqlclient-2.2.0/src/mysqlclient.egg-info/SOURCES.txt` & `mysqlclient-2.2.0rc1/src/mysqlclient.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 site.cfg
 doc/FAQ.rst
 doc/MySQLdb.constants.rst
 doc/MySQLdb.rst
 doc/conf.py
 doc/index.rst
 doc/user_guide.rst
-src/MySQLdb/_mysql.c
 src/MySQLdb/__init__.py
 src/MySQLdb/_exceptions.py
 src/MySQLdb/_mysql.c
 src/MySQLdb/connections.py
 src/MySQLdb/converters.py
 src/MySQLdb/cursors.py
 src/MySQLdb/release.py
```

### Comparing `mysqlclient-2.2.0/tests/capabilities.py` & `mysqlclient-2.2.0rc1/tests/capabilities.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,314 +1,314 @@
-#!/usr/bin/env python -O
-""" Script to test database capabilities and the DB-API interface
-    for functionality and memory leaks.
-
-    Adapted from a script by M-A Lemburg.
-
-"""
-from time import time
-import unittest
-from configdb import connection_factory
-
-
-class DatabaseTest(unittest.TestCase):
-    db_module = None
-    connect_args = ()
-    connect_kwargs = dict()
-    create_table_extra = ""
-    rows = 10
-    debug = False
-
-    def setUp(self):
-        db = connection_factory(**self.connect_kwargs)
-        self.connection = db
-        self.cursor = db.cursor()
-        self.BLOBUText = "".join([chr(i) for i in range(16384)])
-        self.BLOBBinary = self.db_module.Binary(
-            ("".join([chr(i) for i in range(256)] * 16)).encode("latin1")
-        )
-
-    leak_test = True
-
-    def tearDown(self):
-        if self.leak_test:
-            import gc
-
-            del self.cursor
-            orphans = gc.collect()
-            self.assertFalse(
-                orphans, "%d orphaned objects found after deleting cursor" % orphans
-            )
-
-            del self.connection
-            orphans = gc.collect()
-            self.assertFalse(
-                orphans, "%d orphaned objects found after deleting connection" % orphans
-            )
-
-    def table_exists(self, name):
-        try:
-            self.cursor.execute("select * from %s where 1=0" % name)
-        except Exception:
-            return False
-        else:
-            return True
-
-    def quote_identifier(self, ident):
-        return '"%s"' % ident
-
-    def new_table_name(self):
-        i = id(self.cursor)
-        while True:
-            name = self.quote_identifier("tb%08x" % i)
-            if not self.table_exists(name):
-                return name
-            i = i + 1
-
-    def create_table(self, columndefs):
-        """Create a table using a list of column definitions given in
-        columndefs.
-
-        generator must be a function taking arguments (row_number,
-        col_number) returning a suitable data object for insertion
-        into the table.
-
-        """
-        self.table = self.new_table_name()
-        self.cursor.execute(
-            "CREATE TABLE %s (%s) %s"
-            % (self.table, ",\n".join(columndefs), self.create_table_extra)
-        )
-
-    def check_data_integrity(self, columndefs, generator):
-        # insert
-        self.create_table(columndefs)
-        insert_statement = "INSERT INTO {} VALUES ({})".format(
-            self.table,
-            ",".join(["%s"] * len(columndefs)),
-        )
-        data = [
-            [generator(i, j) for j in range(len(columndefs))] for i in range(self.rows)
-        ]
-        self.cursor.executemany(insert_statement, data)
-        self.connection.commit()
-        # verify
-        self.cursor.execute("select * from %s" % self.table)
-        res = self.cursor.fetchall()
-        self.assertEqual(len(res), self.rows)
-        try:
-            for i in range(self.rows):
-                for j in range(len(columndefs)):
-                    self.assertEqual(res[i][j], generator(i, j))
-        finally:
-            if not self.debug:
-                self.cursor.execute("drop table %s" % (self.table))
-
-    def test_transactions(self):
-        columndefs = ("col1 INT", "col2 VARCHAR(255)")
-
-        def generator(row, col):
-            if col == 0:
-                return row
-            else:
-                return ("%i" % (row % 10)) * 255
-
-        self.create_table(columndefs)
-        insert_statement = "INSERT INTO {} VALUES ({})".format(
-            self.table,
-            ",".join(["%s"] * len(columndefs)),
-        )
-        data = [
-            [generator(i, j) for j in range(len(columndefs))] for i in range(self.rows)
-        ]
-        self.cursor.executemany(insert_statement, data)
-        # verify
-        self.connection.commit()
-        self.cursor.execute("select * from %s" % self.table)
-        res = self.cursor.fetchall()
-        self.assertEqual(len(res), self.rows)
-        for i in range(self.rows):
-            for j in range(len(columndefs)):
-                self.assertEqual(res[i][j], generator(i, j))
-        delete_statement = "delete from %s where col1=%%s" % self.table
-        self.cursor.execute(delete_statement, (0,))
-        self.cursor.execute(f"select col1 from {self.table} where col1=%s", (0,))
-        res = self.cursor.fetchall()
-        self.assertFalse(res, "DELETE didn't work")
-        self.connection.rollback()
-        self.cursor.execute(f"select col1 from {self.table} where col1=%s", (0,))
-        res = self.cursor.fetchall()
-        self.assertTrue(len(res) == 1, "ROLLBACK didn't work")
-        self.cursor.execute("drop table %s" % (self.table))
-
-    def test_truncation(self):
-        columndefs = ("col1 INT", "col2 VARCHAR(255)")
-
-        def generator(row, col):
-            if col == 0:
-                return row
-            else:
-                return ("%i" % (row % 10)) * ((255 - self.rows // 2) + row)
-
-        self.create_table(columndefs)
-        insert_statement = "INSERT INTO {} VALUES ({})".format(
-            self.table,
-            ",".join(["%s"] * len(columndefs)),
-        )
-
-        try:
-            self.cursor.execute(insert_statement, (0, "0" * 256))
-        except self.connection.DataError:
-            pass
-        else:
-            self.fail(
-                "Over-long column did not generate warnings/exception with single insert"  # noqa: E501
-            )
-
-        self.connection.rollback()
-
-        try:
-            for i in range(self.rows):
-                data = []
-                for j in range(len(columndefs)):
-                    data.append(generator(i, j))
-                self.cursor.execute(insert_statement, tuple(data))
-        except self.connection.DataError:
-            pass
-        else:
-            self.fail(
-                "Over-long columns did not generate warnings/exception with execute()"  # noqa: E501
-            )
-
-        self.connection.rollback()
-
-        try:
-            data = [
-                [generator(i, j) for j in range(len(columndefs))]
-                for i in range(self.rows)
-            ]
-            self.cursor.executemany(insert_statement, data)
-        except self.connection.DataError:
-            pass
-        else:
-            self.fail(
-                "Over-long columns did not generate warnings/exception with executemany()"  # noqa: E501
-            )
-
-        self.connection.rollback()
-        self.cursor.execute("drop table %s" % (self.table))
-
-    def test_CHAR(self):
-        # Character data
-        def generator(row, col):
-            return ("%i" % ((row + col) % 10)) * 255
-
-        self.check_data_integrity(("col1 char(255)", "col2 char(255)"), generator)
-
-    def test_INT(self):
-        # Number data
-        def generator(row, col):
-            return row * row
-
-        self.check_data_integrity(("col1 INT",), generator)
-
-    def test_DECIMAL(self):
-        # DECIMAL
-        from decimal import Decimal
-
-        def generator(row, col):
-            return Decimal("%d.%02d" % (row, col))
-
-        self.check_data_integrity(("col1 DECIMAL(5,2)",), generator)
-
-        val = Decimal("1.11111111111111119E-7")
-        self.cursor.execute("SELECT %s", (val,))
-        result = self.cursor.fetchone()[0]
-        self.assertEqual(result, val)
-        self.assertIsInstance(result, Decimal)
-
-        self.cursor.execute("SELECT %s + %s", (Decimal("0.1"), Decimal("0.2")))
-        result = self.cursor.fetchone()[0]
-        self.assertEqual(result, Decimal("0.3"))
-        self.assertIsInstance(result, Decimal)
-
-    def test_DATE(self):
-        ticks = time()
-
-        def generator(row, col):
-            return self.db_module.DateFromTicks(ticks + row * 86400 - col * 1313)
-
-        self.check_data_integrity(("col1 DATE",), generator)
-
-    def test_TIME(self):
-        ticks = time()
-
-        def generator(row, col):
-            return self.db_module.TimeFromTicks(ticks + row * 86400 - col * 1313)
-
-        self.check_data_integrity(("col1 TIME",), generator)
-
-    def test_DATETIME(self):
-        ticks = time()
-
-        def generator(row, col):
-            return self.db_module.TimestampFromTicks(ticks + row * 86400 - col * 1313)
-
-        self.check_data_integrity(("col1 DATETIME",), generator)
-
-    def test_TIMESTAMP(self):
-        ticks = time()
-
-        def generator(row, col):
-            return self.db_module.TimestampFromTicks(ticks + row * 86400 - col * 1313)
-
-        self.check_data_integrity(("col1 TIMESTAMP",), generator)
-
-    def test_fractional_TIMESTAMP(self):
-        ticks = time()
-
-        def generator(row, col):
-            return self.db_module.TimestampFromTicks(
-                ticks + row * 86400 - col * 1313 + row * 0.7 * col / 3.0
-            )
-
-        self.check_data_integrity(("col1 TIMESTAMP",), generator)
-
-    def test_LONG(self):
-        def generator(row, col):
-            if col == 0:
-                return row
-            else:
-                return self.BLOBUText  # 'BLOB Text ' * 1024
-
-        self.check_data_integrity(("col1 INT", "col2 LONG"), generator)
-
-    def test_TEXT(self):
-        def generator(row, col):
-            return self.BLOBUText  # 'BLOB Text ' * 1024
-
-        self.check_data_integrity(("col2 TEXT",), generator)
-
-    def test_LONG_BYTE(self):
-        def generator(row, col):
-            if col == 0:
-                return row
-            else:
-                return self.BLOBBinary  # 'BLOB\000Binary ' * 1024
-
-        self.check_data_integrity(("col1 INT", "col2 LONG BYTE"), generator)
-
-    def test_BLOB(self):
-        def generator(row, col):
-            if col == 0:
-                return row
-            else:
-                return self.BLOBBinary  # 'BLOB\000Binary ' * 1024
-
-        self.check_data_integrity(("col1 INT", "col2 BLOB"), generator)
-
-    def test_DOUBLE(self):
-        for val in (18014398509481982.0, 0.1):
-            self.cursor.execute("SELECT %s", (val,))
-            result = self.cursor.fetchone()[0]
-            self.assertEqual(result, val)
-            self.assertIsInstance(result, float)
+#!/usr/bin/env python -O
+""" Script to test database capabilities and the DB-API interface
+    for functionality and memory leaks.
+
+    Adapted from a script by M-A Lemburg.
+
+"""
+from time import time
+import unittest
+from configdb import connection_factory
+
+
+class DatabaseTest(unittest.TestCase):
+    db_module = None
+    connect_args = ()
+    connect_kwargs = dict()
+    create_table_extra = ""
+    rows = 10
+    debug = False
+
+    def setUp(self):
+        db = connection_factory(**self.connect_kwargs)
+        self.connection = db
+        self.cursor = db.cursor()
+        self.BLOBUText = "".join([chr(i) for i in range(16384)])
+        self.BLOBBinary = self.db_module.Binary(
+            ("".join([chr(i) for i in range(256)] * 16)).encode("latin1")
+        )
+
+    leak_test = True
+
+    def tearDown(self):
+        if self.leak_test:
+            import gc
+
+            del self.cursor
+            orphans = gc.collect()
+            self.assertFalse(
+                orphans, "%d orphaned objects found after deleting cursor" % orphans
+            )
+
+            del self.connection
+            orphans = gc.collect()
+            self.assertFalse(
+                orphans, "%d orphaned objects found after deleting connection" % orphans
+            )
+
+    def table_exists(self, name):
+        try:
+            self.cursor.execute("select * from %s where 1=0" % name)
+        except Exception:
+            return False
+        else:
+            return True
+
+    def quote_identifier(self, ident):
+        return '"%s"' % ident
+
+    def new_table_name(self):
+        i = id(self.cursor)
+        while True:
+            name = self.quote_identifier("tb%08x" % i)
+            if not self.table_exists(name):
+                return name
+            i = i + 1
+
+    def create_table(self, columndefs):
+        """Create a table using a list of column definitions given in
+        columndefs.
+
+        generator must be a function taking arguments (row_number,
+        col_number) returning a suitable data object for insertion
+        into the table.
+
+        """
+        self.table = self.new_table_name()
+        self.cursor.execute(
+            "CREATE TABLE %s (%s) %s"
+            % (self.table, ",\n".join(columndefs), self.create_table_extra)
+        )
+
+    def check_data_integrity(self, columndefs, generator):
+        # insert
+        self.create_table(columndefs)
+        insert_statement = "INSERT INTO {} VALUES ({})".format(
+            self.table,
+            ",".join(["%s"] * len(columndefs)),
+        )
+        data = [
+            [generator(i, j) for j in range(len(columndefs))] for i in range(self.rows)
+        ]
+        self.cursor.executemany(insert_statement, data)
+        self.connection.commit()
+        # verify
+        self.cursor.execute("select * from %s" % self.table)
+        res = self.cursor.fetchall()
+        self.assertEqual(len(res), self.rows)
+        try:
+            for i in range(self.rows):
+                for j in range(len(columndefs)):
+                    self.assertEqual(res[i][j], generator(i, j))
+        finally:
+            if not self.debug:
+                self.cursor.execute("drop table %s" % (self.table))
+
+    def test_transactions(self):
+        columndefs = ("col1 INT", "col2 VARCHAR(255)")
+
+        def generator(row, col):
+            if col == 0:
+                return row
+            else:
+                return ("%i" % (row % 10)) * 255
+
+        self.create_table(columndefs)
+        insert_statement = "INSERT INTO {} VALUES ({})".format(
+            self.table,
+            ",".join(["%s"] * len(columndefs)),
+        )
+        data = [
+            [generator(i, j) for j in range(len(columndefs))] for i in range(self.rows)
+        ]
+        self.cursor.executemany(insert_statement, data)
+        # verify
+        self.connection.commit()
+        self.cursor.execute("select * from %s" % self.table)
+        res = self.cursor.fetchall()
+        self.assertEqual(len(res), self.rows)
+        for i in range(self.rows):
+            for j in range(len(columndefs)):
+                self.assertEqual(res[i][j], generator(i, j))
+        delete_statement = "delete from %s where col1=%%s" % self.table
+        self.cursor.execute(delete_statement, (0,))
+        self.cursor.execute(f"select col1 from {self.table} where col1=%s", (0,))
+        res = self.cursor.fetchall()
+        self.assertFalse(res, "DELETE didn't work")
+        self.connection.rollback()
+        self.cursor.execute(f"select col1 from {self.table} where col1=%s", (0,))
+        res = self.cursor.fetchall()
+        self.assertTrue(len(res) == 1, "ROLLBACK didn't work")
+        self.cursor.execute("drop table %s" % (self.table))
+
+    def test_truncation(self):
+        columndefs = ("col1 INT", "col2 VARCHAR(255)")
+
+        def generator(row, col):
+            if col == 0:
+                return row
+            else:
+                return ("%i" % (row % 10)) * ((255 - self.rows // 2) + row)
+
+        self.create_table(columndefs)
+        insert_statement = "INSERT INTO {} VALUES ({})".format(
+            self.table,
+            ",".join(["%s"] * len(columndefs)),
+        )
+
+        try:
+            self.cursor.execute(insert_statement, (0, "0" * 256))
+        except self.connection.DataError:
+            pass
+        else:
+            self.fail(
+                "Over-long column did not generate warnings/exception with single insert"  # noqa: E501
+            )
+
+        self.connection.rollback()
+
+        try:
+            for i in range(self.rows):
+                data = []
+                for j in range(len(columndefs)):
+                    data.append(generator(i, j))
+                self.cursor.execute(insert_statement, tuple(data))
+        except self.connection.DataError:
+            pass
+        else:
+            self.fail(
+                "Over-long columns did not generate warnings/exception with execute()"  # noqa: E501
+            )
+
+        self.connection.rollback()
+
+        try:
+            data = [
+                [generator(i, j) for j in range(len(columndefs))]
+                for i in range(self.rows)
+            ]
+            self.cursor.executemany(insert_statement, data)
+        except self.connection.DataError:
+            pass
+        else:
+            self.fail(
+                "Over-long columns did not generate warnings/exception with executemany()"  # noqa: E501
+            )
+
+        self.connection.rollback()
+        self.cursor.execute("drop table %s" % (self.table))
+
+    def test_CHAR(self):
+        # Character data
+        def generator(row, col):
+            return ("%i" % ((row + col) % 10)) * 255
+
+        self.check_data_integrity(("col1 char(255)", "col2 char(255)"), generator)
+
+    def test_INT(self):
+        # Number data
+        def generator(row, col):
+            return row * row
+
+        self.check_data_integrity(("col1 INT",), generator)
+
+    def test_DECIMAL(self):
+        # DECIMAL
+        from decimal import Decimal
+
+        def generator(row, col):
+            return Decimal("%d.%02d" % (row, col))
+
+        self.check_data_integrity(("col1 DECIMAL(5,2)",), generator)
+
+        val = Decimal("1.11111111111111119E-7")
+        self.cursor.execute("SELECT %s", (val,))
+        result = self.cursor.fetchone()[0]
+        self.assertEqual(result, val)
+        self.assertIsInstance(result, Decimal)
+
+        self.cursor.execute("SELECT %s + %s", (Decimal("0.1"), Decimal("0.2")))
+        result = self.cursor.fetchone()[0]
+        self.assertEqual(result, Decimal("0.3"))
+        self.assertIsInstance(result, Decimal)
+
+    def test_DATE(self):
+        ticks = time()
+
+        def generator(row, col):
+            return self.db_module.DateFromTicks(ticks + row * 86400 - col * 1313)
+
+        self.check_data_integrity(("col1 DATE",), generator)
+
+    def test_TIME(self):
+        ticks = time()
+
+        def generator(row, col):
+            return self.db_module.TimeFromTicks(ticks + row * 86400 - col * 1313)
+
+        self.check_data_integrity(("col1 TIME",), generator)
+
+    def test_DATETIME(self):
+        ticks = time()
+
+        def generator(row, col):
+            return self.db_module.TimestampFromTicks(ticks + row * 86400 - col * 1313)
+
+        self.check_data_integrity(("col1 DATETIME",), generator)
+
+    def test_TIMESTAMP(self):
+        ticks = time()
+
+        def generator(row, col):
+            return self.db_module.TimestampFromTicks(ticks + row * 86400 - col * 1313)
+
+        self.check_data_integrity(("col1 TIMESTAMP",), generator)
+
+    def test_fractional_TIMESTAMP(self):
+        ticks = time()
+
+        def generator(row, col):
+            return self.db_module.TimestampFromTicks(
+                ticks + row * 86400 - col * 1313 + row * 0.7 * col / 3.0
+            )
+
+        self.check_data_integrity(("col1 TIMESTAMP",), generator)
+
+    def test_LONG(self):
+        def generator(row, col):
+            if col == 0:
+                return row
+            else:
+                return self.BLOBUText  # 'BLOB Text ' * 1024
+
+        self.check_data_integrity(("col1 INT", "col2 LONG"), generator)
+
+    def test_TEXT(self):
+        def generator(row, col):
+            return self.BLOBUText  # 'BLOB Text ' * 1024
+
+        self.check_data_integrity(("col2 TEXT",), generator)
+
+    def test_LONG_BYTE(self):
+        def generator(row, col):
+            if col == 0:
+                return row
+            else:
+                return self.BLOBBinary  # 'BLOB\000Binary ' * 1024
+
+        self.check_data_integrity(("col1 INT", "col2 LONG BYTE"), generator)
+
+    def test_BLOB(self):
+        def generator(row, col):
+            if col == 0:
+                return row
+            else:
+                return self.BLOBBinary  # 'BLOB\000Binary ' * 1024
+
+        self.check_data_integrity(("col1 INT", "col2 BLOB"), generator)
+
+    def test_DOUBLE(self):
+        for val in (18014398509481982.0, 0.1):
+            self.cursor.execute("SELECT %s", (val,))
+            result = self.cursor.fetchone()[0]
+            self.assertEqual(result, val)
+            self.assertIsInstance(result, float)
```

### Comparing `mysqlclient-2.2.0/tests/configdb.py` & `mysqlclient-2.2.0rc1/tests/configdb.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-"""Configure database connection for tests."""
-
-from os import environ, path
-
-tests_path = path.dirname(__file__)
-conf_file = environ.get("TESTDB", "default.cnf")
-conf_path = path.join(tests_path, conf_file)
-connect_kwargs = dict(
-    read_default_file=conf_path,
-    read_default_group="MySQLdb-tests",
-)
-
-
-def connection_kwargs(kwargs):
-    db_kwargs = connect_kwargs.copy()
-    db_kwargs.update(kwargs)
-    return db_kwargs
-
-
-def connection_factory(**kwargs):
-    import MySQLdb
-
-    db_kwargs = connection_kwargs(kwargs)
-    db = MySQLdb.connect(**db_kwargs)
-    return db
+"""Configure database connection for tests."""
+
+from os import environ, path
+
+tests_path = path.dirname(__file__)
+conf_file = environ.get("TESTDB", "default.cnf")
+conf_path = path.join(tests_path, conf_file)
+connect_kwargs = dict(
+    read_default_file=conf_path,
+    read_default_group="MySQLdb-tests",
+)
+
+
+def connection_kwargs(kwargs):
+    db_kwargs = connect_kwargs.copy()
+    db_kwargs.update(kwargs)
+    return db_kwargs
+
+
+def connection_factory(**kwargs):
+    import MySQLdb
+
+    db_kwargs = connection_kwargs(kwargs)
+    db = MySQLdb.connect(**db_kwargs)
+    return db
```

### Comparing `mysqlclient-2.2.0/tests/dbapi20.py` & `mysqlclient-2.2.0rc1/tests/dbapi20.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,859 +1,859 @@
-#!/usr/bin/env python
-""" Python DB API 2.0 driver compliance unit test suite.
-
-    This software is Public Domain and may be used without restrictions.
-
- "Now we have booze and barflies entering the discussion, plus rumours of
-  DBAs on drugs... and I won't tell you what flashes through my mind each
-  time I read the subject line with 'Anal Compliance' in it.  All around
-  this is turning out to be a thoroughly unwholesome unit test."
-
-    -- Ian Bicking
-"""
-
-__rcs_id__ = "$Id$"
-__version__ = "$Revision$"[11:-2]
-__author__ = "Stuart Bishop <zen@shangri-la.dropbear.id.au>"
-
-import unittest
-import time
-
-# $Log$
-# Revision 1.1.2.1  2006/02/25 03:44:32  adustman
-# Generic DB-API unit test module
-#
-# Revision 1.10  2003/10/09 03:14:14  zenzen
-# Add test for DB API 2.0 optional extension, where database exceptions
-# are exposed as attributes on the Connection object.
-#
-# Revision 1.9  2003/08/13 01:16:36  zenzen
-# Minor tweak from Stefan Fleiter
-#
-# Revision 1.8  2003/04/10 00:13:25  zenzen
-# Changes, as per suggestions by M.-A. Lemburg
-# - Add a table prefix, to ensure namespace collisions can always be avoided
-#
-# Revision 1.7  2003/02/26 23:33:37  zenzen
-# Break out DDL into helper functions, as per request by David Rushby
-#
-# Revision 1.6  2003/02/21 03:04:33  zenzen
-# Stuff from Henrik Ekelund:
-#     added test_None
-#     added test_nextset & hooks
-#
-# Revision 1.5  2003/02/17 22:08:43  zenzen
-# Implement suggestions and code from Henrik Eklund - test that cursor.arraysize
-# defaults to 1 & generic cursor.callproc test added
-#
-# Revision 1.4  2003/02/15 00:16:33  zenzen
-# Changes, as per suggestions and bug reports by M.-A. Lemburg,
-# Matthew T. Kromer, Federico Di Gregorio and Daniel Dittmar
-# - Class renamed
-# - Now a subclass of TestCase, to avoid requiring the driver stub
-#   to use multiple inheritance
-# - Reversed the polarity of buggy test in test_description
-# - Test exception hierarchy correctly
-# - self.populate is now self._populate(), so if a driver stub
-#   overrides self.ddl1 this change propagates
-# - VARCHAR columns now have a width, which will hopefully make the
-#   DDL even more portable (this will be reversed if it causes more problems)
-# - cursor.rowcount being checked after various execute and fetchXXX methods
-# - Check for fetchall and fetchmany returning empty lists after results
-#   are exhausted (already checking for empty lists if select retrieved
-#   nothing
-# - Fix bugs in test_setoutputsize_basic and test_setinputsizes
-#
-
-
-class DatabaseAPI20Test(unittest.TestCase):
-    """Test a database self.driver for DB API 2.0 compatibility.
-    This implementation tests Gadfly, but the TestCase
-    is structured so that other self.drivers can subclass this
-    test case to ensure compiliance with the DB-API. It is
-    expected that this TestCase may be expanded in the future
-    if ambiguities or edge conditions are discovered.
-
-    The 'Optional Extensions' are not yet being tested.
-
-    self.drivers should subclass this test, overriding setUp, tearDown,
-    self.driver, connect_args and connect_kw_args. Class specification
-    should be as follows:
-
-    import dbapi20
-    class mytest(dbapi20.DatabaseAPI20Test):
-       [...]
-
-    Don't 'import DatabaseAPI20Test from dbapi20', or you will
-    confuse the unit tester - just 'import dbapi20'.
-    """
-
-    # The self.driver module. This should be the module where the 'connect'
-    # method is to be found
-    driver = None
-    connect_args = ()  # List of arguments to pass to connect
-    connect_kw_args = {}  # Keyword arguments for connect
-    table_prefix = "dbapi20test_"  # If you need to specify a prefix for tables
-
-    ddl1 = "create table %sbooze (name varchar(20))" % table_prefix
-    ddl2 = "create table %sbarflys (name varchar(20))" % table_prefix
-    xddl1 = "drop table %sbooze" % table_prefix
-    xddl2 = "drop table %sbarflys" % table_prefix
-
-    lowerfunc = "lower"  # Name of stored procedure to convert string->lowercase
-
-    # Some drivers may need to override these helpers, for example adding
-    # a 'commit' after the execute.
-    def executeDDL1(self, cursor):
-        cursor.execute(self.ddl1)
-
-    def executeDDL2(self, cursor):
-        cursor.execute(self.ddl2)
-
-    def setUp(self):
-        """self.drivers should override this method to perform required setup
-        if any is necessary, such as creating the database.
-        """
-        pass
-
-    def tearDown(self):
-        """self.drivers should override this method to perform required cleanup
-        if any is necessary, such as deleting the test database.
-        The default drops the tables that may be created.
-        """
-        con = self._connect()
-        try:
-            cur = con.cursor()
-            for ddl in (self.xddl1, self.xddl2):
-                try:
-                    cur.execute(ddl)
-                    con.commit()
-                except self.driver.Error:
-                    # Assume table didn't exist. Other tests will check if
-                    # execute is busted.
-                    pass
-        finally:
-            con.close()
-
-    def _connect(self):
-        try:
-            return self.driver.connect(*self.connect_args, **self.connect_kw_args)
-        except AttributeError:
-            self.fail("No connect method found in self.driver module")
-
-    def test_connect(self):
-        con = self._connect()
-        con.close()
-
-    def test_apilevel(self):
-        try:
-            # Must exist
-            apilevel = self.driver.apilevel
-            # Must equal 2.0
-            self.assertEqual(apilevel, "2.0")
-        except AttributeError:
-            self.fail("Driver doesn't define apilevel")
-
-    def test_threadsafety(self):
-        try:
-            # Must exist
-            threadsafety = self.driver.threadsafety
-            # Must be a valid value
-            self.assertTrue(threadsafety in (0, 1, 2, 3))
-        except AttributeError:
-            self.fail("Driver doesn't define threadsafety")
-
-    def test_paramstyle(self):
-        try:
-            # Must exist
-            paramstyle = self.driver.paramstyle
-            # Must be a valid value
-            self.assertTrue(
-                paramstyle in ("qmark", "numeric", "named", "format", "pyformat")
-            )
-        except AttributeError:
-            self.fail("Driver doesn't define paramstyle")
-
-    def test_Exceptions(self):
-        # Make sure required exceptions exist, and are in the
-        # defined hierarchy.
-        self.assertTrue(issubclass(self.driver.Warning, Exception))
-        self.assertTrue(issubclass(self.driver.Error, Exception))
-        self.assertTrue(issubclass(self.driver.InterfaceError, self.driver.Error))
-        self.assertTrue(issubclass(self.driver.DatabaseError, self.driver.Error))
-        self.assertTrue(issubclass(self.driver.OperationalError, self.driver.Error))
-        self.assertTrue(issubclass(self.driver.IntegrityError, self.driver.Error))
-        self.assertTrue(issubclass(self.driver.InternalError, self.driver.Error))
-        self.assertTrue(issubclass(self.driver.ProgrammingError, self.driver.Error))
-        self.assertTrue(issubclass(self.driver.NotSupportedError, self.driver.Error))
-
-    def test_ExceptionsAsConnectionAttributes(self):
-        # OPTIONAL EXTENSION
-        # Test for the optional DB API 2.0 extension, where the exceptions
-        # are exposed as attributes on the Connection object
-        # I figure this optional extension will be implemented by any
-        # driver author who is using this test suite, so it is enabled
-        # by default.
-        con = self._connect()
-        drv = self.driver
-        self.assertTrue(con.Warning is drv.Warning)
-        self.assertTrue(con.Error is drv.Error)
-        self.assertTrue(con.InterfaceError is drv.InterfaceError)
-        self.assertTrue(con.DatabaseError is drv.DatabaseError)
-        self.assertTrue(con.OperationalError is drv.OperationalError)
-        self.assertTrue(con.IntegrityError is drv.IntegrityError)
-        self.assertTrue(con.InternalError is drv.InternalError)
-        self.assertTrue(con.ProgrammingError is drv.ProgrammingError)
-        self.assertTrue(con.NotSupportedError is drv.NotSupportedError)
-
-    def test_commit(self):
-        con = self._connect()
-        try:
-            # Commit must work, even if it doesn't do anything
-            con.commit()
-        finally:
-            con.close()
-
-    def test_rollback(self):
-        con = self._connect()
-        # If rollback is defined, it should either work or throw
-        # the documented exception
-        if hasattr(con, "rollback"):
-            try:
-                con.rollback()
-            except self.driver.NotSupportedError:
-                pass
-
-    def test_cursor(self):
-        con = self._connect()
-        try:
-            _ = con.cursor()
-        finally:
-            con.close()
-
-    def test_cursor_isolation(self):
-        con = self._connect()
-        try:
-            # Make sure cursors created from the same connection have
-            # the documented transaction isolation level
-            cur1 = con.cursor()
-            cur2 = con.cursor()
-            self.executeDDL1(cur1)
-            cur1.execute(
-                "insert into %sbooze values ('Victoria Bitter')" % (self.table_prefix)
-            )
-            cur2.execute("select name from %sbooze" % self.table_prefix)
-            booze = cur2.fetchall()
-            self.assertEqual(len(booze), 1)
-            self.assertEqual(len(booze[0]), 1)
-            self.assertEqual(booze[0][0], "Victoria Bitter")
-        finally:
-            con.close()
-
-    def test_description(self):
-        con = self._connect()
-        try:
-            cur = con.cursor()
-            self.executeDDL1(cur)
-            self.assertEqual(
-                cur.description,
-                None,
-                "cursor.description should be none after executing a "
-                "statement that can return no rows (such as DDL)",
-            )
-            cur.execute("select name from %sbooze" % self.table_prefix)
-            self.assertEqual(
-                len(cur.description), 1, "cursor.description describes too many columns"
-            )
-            self.assertEqual(
-                len(cur.description[0]),
-                7,
-                "cursor.description[x] tuples must have 7 elements",
-            )
-            self.assertEqual(
-                cur.description[0][0].lower(),
-                "name",
-                "cursor.description[x][0] must return column name",
-            )
-            self.assertEqual(
-                cur.description[0][1],
-                self.driver.STRING,
-                "cursor.description[x][1] must return column type. Got %r"
-                % cur.description[0][1],
-            )
-
-            # Make sure self.description gets reset
-            self.executeDDL2(cur)
-            self.assertEqual(
-                cur.description,
-                None,
-                "cursor.description not being set to None when executing "
-                "no-result statements (eg. DDL)",
-            )
-        finally:
-            con.close()
-
-    def test_rowcount(self):
-        con = self._connect()
-        try:
-            cur = con.cursor()
-            self.executeDDL1(cur)
-            self.assertEqual(
-                cur.rowcount,
-                -1,
-                "cursor.rowcount should be -1 after executing no-result " "statements",
-            )
-            cur.execute(
-                "insert into %sbooze values ('Victoria Bitter')" % (self.table_prefix)
-            )
-            self.assertTrue(
-                cur.rowcount in (-1, 1),
-                "cursor.rowcount should == number or rows inserted, or "
-                "set to -1 after executing an insert statement",
-            )
-            cur.execute("select name from %sbooze" % self.table_prefix)
-            self.assertTrue(
-                cur.rowcount in (-1, 1),
-                "cursor.rowcount should == number of rows returned, or "
-                "set to -1 after executing a select statement",
-            )
-            self.executeDDL2(cur)
-            self.assertEqual(
-                cur.rowcount,
-                -1,
-                "cursor.rowcount not being reset to -1 after executing "
-                "no-result statements",
-            )
-        finally:
-            con.close()
-
-    lower_func = "lower"
-
-    def test_callproc(self):
-        con = self._connect()
-        try:
-            cur = con.cursor()
-            if self.lower_func and hasattr(cur, "callproc"):
-                r = cur.callproc(self.lower_func, ("FOO",))
-                self.assertEqual(len(r), 1)
-                self.assertEqual(r[0], "FOO")
-                r = cur.fetchall()
-                self.assertEqual(len(r), 1, "callproc produced no result set")
-                self.assertEqual(len(r[0]), 1, "callproc produced invalid result set")
-                self.assertEqual(r[0][0], "foo", "callproc produced invalid results")
-        finally:
-            con.close()
-
-    def test_close(self):
-        con = self._connect()
-        try:
-            cur = con.cursor()
-        finally:
-            con.close()
-
-        # cursor.execute should raise an Error if called after connection
-        # closed
-        self.assertRaises(self.driver.Error, self.executeDDL1, cur)
-
-        # connection.commit should raise an Error if called after connection'
-        # closed.'
-        self.assertRaises(self.driver.Error, con.commit)
-
-        # connection.close should raise an Error if called more than once
-        self.assertRaises(self.driver.Error, con.close)
-
-    def test_execute(self):
-        con = self._connect()
-        try:
-            cur = con.cursor()
-            self._paraminsert(cur)
-        finally:
-            con.close()
-
-    def _paraminsert(self, cur):
-        self.executeDDL1(cur)
-        cur.execute(
-            "insert into %sbooze values ('Victoria Bitter')" % (self.table_prefix)
-        )
-        self.assertTrue(cur.rowcount in (-1, 1))
-
-        if self.driver.paramstyle == "qmark":
-            cur.execute(
-                "insert into %sbooze values (?)" % self.table_prefix, ("Cooper's",)
-            )
-        elif self.driver.paramstyle == "numeric":
-            cur.execute(
-                "insert into %sbooze values (:1)" % self.table_prefix, ("Cooper's",)
-            )
-        elif self.driver.paramstyle == "named":
-            cur.execute(
-                "insert into %sbooze values (:beer)" % self.table_prefix,
-                {"beer": "Cooper's"},
-            )
-        elif self.driver.paramstyle == "format":
-            cur.execute(
-                "insert into %sbooze values (%%s)" % self.table_prefix, ("Cooper's",)
-            )
-        elif self.driver.paramstyle == "pyformat":
-            cur.execute(
-                "insert into %sbooze values (%%(beer)s)" % self.table_prefix,
-                {"beer": "Cooper's"},
-            )
-        else:
-            self.fail("Invalid paramstyle")
-        self.assertTrue(cur.rowcount in (-1, 1))
-
-        cur.execute("select name from %sbooze" % self.table_prefix)
-        res = cur.fetchall()
-        self.assertEqual(len(res), 2, "cursor.fetchall returned too few rows")
-        beers = [res[0][0], res[1][0]]
-        beers.sort()
-        self.assertEqual(
-            beers[0],
-            "Cooper's",
-            "cursor.fetchall retrieved incorrect data, or data inserted " "incorrectly",
-        )
-        self.assertEqual(
-            beers[1],
-            "Victoria Bitter",
-            "cursor.fetchall retrieved incorrect data, or data inserted " "incorrectly",
-        )
-
-    def test_executemany(self):
-        con = self._connect()
-        try:
-            cur = con.cursor()
-            self.executeDDL1(cur)
-            largs = [("Cooper's",), ("Boag's",)]
-            margs = [{"beer": "Cooper's"}, {"beer": "Boag's"}]
-            if self.driver.paramstyle == "qmark":
-                cur.executemany(
-                    "insert into %sbooze values (?)" % self.table_prefix, largs
-                )
-            elif self.driver.paramstyle == "numeric":
-                cur.executemany(
-                    "insert into %sbooze values (:1)" % self.table_prefix, largs
-                )
-            elif self.driver.paramstyle == "named":
-                cur.executemany(
-                    "insert into %sbooze values (:beer)" % self.table_prefix, margs
-                )
-            elif self.driver.paramstyle == "format":
-                cur.executemany(
-                    "insert into %sbooze values (%%s)" % self.table_prefix, largs
-                )
-            elif self.driver.paramstyle == "pyformat":
-                cur.executemany(
-                    "insert into %sbooze values (%%(beer)s)" % (self.table_prefix),
-                    margs,
-                )
-            else:
-                self.fail("Unknown paramstyle")
-            self.assertTrue(
-                cur.rowcount in (-1, 2),
-                "insert using cursor.executemany set cursor.rowcount to "
-                "incorrect value %r" % cur.rowcount,
-            )
-            cur.execute("select name from %sbooze" % self.table_prefix)
-            res = cur.fetchall()
-            self.assertEqual(
-                len(res), 2, "cursor.fetchall retrieved incorrect number of rows"
-            )
-            beers = [res[0][0], res[1][0]]
-            beers.sort()
-            self.assertEqual(beers[0], "Boag's", "incorrect data retrieved")
-            self.assertEqual(beers[1], "Cooper's", "incorrect data retrieved")
-        finally:
-            con.close()
-
-    def test_fetchone(self):
-        con = self._connect()
-        try:
-            cur = con.cursor()
-
-            # cursor.fetchone should raise an Error if called before
-            # executing a select-type query
-            self.assertRaises(self.driver.Error, cur.fetchone)
-
-            # cursor.fetchone should raise an Error if called after
-            # executing a query that cannot return rows
-            self.executeDDL1(cur)
-            self.assertRaises(self.driver.Error, cur.fetchone)
-
-            cur.execute("select name from %sbooze" % self.table_prefix)
-            self.assertEqual(
-                cur.fetchone(),
-                None,
-                "cursor.fetchone should return None if a query retrieves " "no rows",
-            )
-            self.assertTrue(cur.rowcount in (-1, 0))
-
-            # cursor.fetchone should raise an Error if called after
-            # executing a query that cannot return rows
-            cur.execute(
-                "insert into %sbooze values ('Victoria Bitter')" % (self.table_prefix)
-            )
-            self.assertRaises(self.driver.Error, cur.fetchone)
-
-            cur.execute("select name from %sbooze" % self.table_prefix)
-            r = cur.fetchone()
-            self.assertEqual(
-                len(r), 1, "cursor.fetchone should have retrieved a single row"
-            )
-            self.assertEqual(
-                r[0], "Victoria Bitter", "cursor.fetchone retrieved incorrect data"
-            )
-            self.assertEqual(
-                cur.fetchone(),
-                None,
-                "cursor.fetchone should return None if no more rows available",
-            )
-            self.assertTrue(cur.rowcount in (-1, 1))
-        finally:
-            con.close()
-
-    samples = [
-        "Carlton Cold",
-        "Carlton Draft",
-        "Mountain Goat",
-        "Redback",
-        "Victoria Bitter",
-        "XXXX",
-    ]
-
-    def _populate(self):
-        """Return a list of sql commands to setup the DB for the fetch
-        tests.
-        """
-        populate = [
-            f"insert into {self.table_prefix}booze values ('{s}')" for s in self.samples
-        ]
-        return populate
-
-    def test_fetchmany(self):
-        con = self._connect()
-        try:
-            cur = con.cursor()
-
-            # cursor.fetchmany should raise an Error if called without
-            # issuing a query
-            self.assertRaises(self.driver.Error, cur.fetchmany, 4)
-
-            self.executeDDL1(cur)
-            for sql in self._populate():
-                cur.execute(sql)
-
-            cur.execute("select name from %sbooze" % self.table_prefix)
-            r = cur.fetchmany()
-            self.assertEqual(
-                len(r),
-                1,
-                "cursor.fetchmany retrieved incorrect number of rows, "
-                "default of arraysize is one.",
-            )
-            cur.arraysize = 10
-            r = cur.fetchmany(3)  # Should get 3 rows
-            self.assertEqual(
-                len(r), 3, "cursor.fetchmany retrieved incorrect number of rows"
-            )
-            r = cur.fetchmany(4)  # Should get 2 more
-            self.assertEqual(
-                len(r), 2, "cursor.fetchmany retrieved incorrect number of rows"
-            )
-            r = cur.fetchmany(4)  # Should be an empty sequence
-            self.assertEqual(
-                len(r),
-                0,
-                "cursor.fetchmany should return an empty sequence after "
-                "results are exhausted",
-            )
-            self.assertTrue(cur.rowcount in (-1, 6))
-
-            # Same as above, using cursor.arraysize
-            cur.arraysize = 4
-            cur.execute("select name from %sbooze" % self.table_prefix)
-            r = cur.fetchmany()  # Should get 4 rows
-            self.assertEqual(
-                len(r), 4, "cursor.arraysize not being honoured by fetchmany"
-            )
-            r = cur.fetchmany()  # Should get 2 more
-            self.assertEqual(len(r), 2)
-            r = cur.fetchmany()  # Should be an empty sequence
-            self.assertEqual(len(r), 0)
-            self.assertTrue(cur.rowcount in (-1, 6))
-
-            cur.arraysize = 6
-            cur.execute("select name from %sbooze" % self.table_prefix)
-            rows = cur.fetchmany()  # Should get all rows
-            self.assertTrue(cur.rowcount in (-1, 6))
-            self.assertEqual(len(rows), 6)
-            self.assertEqual(len(rows), 6)
-            rows = [r[0] for r in rows]
-            rows.sort()
-
-            # Make sure we get the right data back out
-            for i in range(0, 6):
-                self.assertEqual(
-                    rows[i],
-                    self.samples[i],
-                    "incorrect data retrieved by cursor.fetchmany",
-                )
-
-            rows = cur.fetchmany()  # Should return an empty list
-            self.assertEqual(
-                len(rows),
-                0,
-                "cursor.fetchmany should return an empty sequence if "
-                "called after the whole result set has been fetched",
-            )
-            self.assertTrue(cur.rowcount in (-1, 6))
-
-            self.executeDDL2(cur)
-            cur.execute("select name from %sbarflys" % self.table_prefix)
-            r = cur.fetchmany()  # Should get empty sequence
-            self.assertEqual(
-                len(r),
-                0,
-                "cursor.fetchmany should return an empty sequence if "
-                "query retrieved no rows",
-            )
-            self.assertTrue(cur.rowcount in (-1, 0))
-
-        finally:
-            con.close()
-
-    def test_fetchall(self):
-        con = self._connect()
-        try:
-            cur = con.cursor()
-            # cursor.fetchall should raise an Error if called
-            # without executing a query that may return rows (such
-            # as a select)
-            self.assertRaises(self.driver.Error, cur.fetchall)
-
-            self.executeDDL1(cur)
-            for sql in self._populate():
-                cur.execute(sql)
-
-            # cursor.fetchall should raise an Error if called
-            # after executing a statement that cannot return rows
-            self.assertRaises(self.driver.Error, cur.fetchall)
-
-            cur.execute("select name from %sbooze" % self.table_prefix)
-            rows = cur.fetchall()
-            self.assertTrue(cur.rowcount in (-1, len(self.samples)))
-            self.assertEqual(
-                len(rows),
-                len(self.samples),
-                "cursor.fetchall did not retrieve all rows",
-            )
-            rows = [r[0] for r in rows]
-            rows.sort()
-            for i in range(0, len(self.samples)):
-                self.assertEqual(
-                    rows[i], self.samples[i], "cursor.fetchall retrieved incorrect rows"
-                )
-            rows = cur.fetchall()
-            self.assertEqual(
-                len(rows),
-                0,
-                "cursor.fetchall should return an empty list if called "
-                "after the whole result set has been fetched",
-            )
-            self.assertTrue(cur.rowcount in (-1, len(self.samples)))
-
-            self.executeDDL2(cur)
-            cur.execute("select name from %sbarflys" % self.table_prefix)
-            rows = cur.fetchall()
-            self.assertTrue(cur.rowcount in (-1, 0))
-            self.assertEqual(
-                len(rows),
-                0,
-                "cursor.fetchall should return an empty list if "
-                "a select query returns no rows",
-            )
-
-        finally:
-            con.close()
-
-    def test_mixedfetch(self):
-        con = self._connect()
-        try:
-            cur = con.cursor()
-            self.executeDDL1(cur)
-            for sql in self._populate():
-                cur.execute(sql)
-
-            cur.execute("select name from %sbooze" % self.table_prefix)
-            rows1 = cur.fetchone()
-            rows23 = cur.fetchmany(2)
-            rows4 = cur.fetchone()
-            rows56 = cur.fetchall()
-            self.assertTrue(cur.rowcount in (-1, 6))
-            self.assertEqual(
-                len(rows23), 2, "fetchmany returned incorrect number of rows"
-            )
-            self.assertEqual(
-                len(rows56), 2, "fetchall returned incorrect number of rows"
-            )
-
-            rows = [rows1[0]]
-            rows.extend([rows23[0][0], rows23[1][0]])
-            rows.append(rows4[0])
-            rows.extend([rows56[0][0], rows56[1][0]])
-            rows.sort()
-            for i in range(0, len(self.samples)):
-                self.assertEqual(
-                    rows[i], self.samples[i], "incorrect data retrieved or inserted"
-                )
-        finally:
-            con.close()
-
-    def help_nextset_setUp(self, cur):
-        """Should create a procedure called deleteme
-        that returns two result sets, first the
-        number of rows in booze then "name from booze"
-        """
-        raise NotImplementedError("Helper not implemented")
-        # sql="""
-        #    create procedure deleteme as
-        #    begin
-        #        select count(*) from booze
-        #        select name from booze
-        #    end
-        # """
-        # cur.execute(sql)
-
-    def help_nextset_tearDown(self, cur):
-        "If cleaning up is needed after nextSetTest"
-        raise NotImplementedError("Helper not implemented")
-        # cur.execute("drop procedure deleteme")
-
-    def test_nextset(self):
-        con = self._connect()
-        try:
-            cur = con.cursor()
-            if not hasattr(cur, "nextset"):
-                return
-
-            try:
-                self.executeDDL1(cur)
-                sql = self._populate()
-                for sql in self._populate():
-                    cur.execute(sql)
-
-                self.help_nextset_setUp(cur)
-
-                cur.callproc("deleteme")
-                numberofrows = cur.fetchone()
-                assert numberofrows[0] == len(self.samples)
-                assert cur.nextset()
-                names = cur.fetchall()
-                assert len(names) == len(self.samples)
-                s = cur.nextset()
-                assert s is None, "No more return sets, should return None"
-            finally:
-                self.help_nextset_tearDown(cur)
-
-        finally:
-            con.close()
-
-    def test_nextset(self):  # noqa: F811
-        raise NotImplementedError("Drivers need to override this test")
-
-    def test_arraysize(self):
-        # Not much here - rest of the tests for this are in test_fetchmany
-        con = self._connect()
-        try:
-            cur = con.cursor()
-            self.assertTrue(
-                hasattr(cur, "arraysize"), "cursor.arraysize must be defined"
-            )
-        finally:
-            con.close()
-
-    def test_setinputsizes(self):
-        con = self._connect()
-        try:
-            cur = con.cursor()
-            cur.setinputsizes((25,))
-            self._paraminsert(cur)  # Make sure cursor still works
-        finally:
-            con.close()
-
-    def test_setoutputsize_basic(self):
-        # Basic test is to make sure setoutputsize doesn't blow up
-        con = self._connect()
-        try:
-            cur = con.cursor()
-            cur.setoutputsize(1000)
-            cur.setoutputsize(2000, 0)
-            self._paraminsert(cur)  # Make sure the cursor still works
-        finally:
-            con.close()
-
-    def test_setoutputsize(self):
-        # Real test for setoutputsize is driver dependent
-        raise NotImplementedError("Driver need to override this test")
-
-    def test_None(self):
-        con = self._connect()
-        try:
-            cur = con.cursor()
-            self.executeDDL1(cur)
-            cur.execute("insert into %sbooze values (NULL)" % self.table_prefix)
-            cur.execute("select name from %sbooze" % self.table_prefix)
-            r = cur.fetchall()
-            self.assertEqual(len(r), 1)
-            self.assertEqual(len(r[0]), 1)
-            self.assertEqual(r[0][0], None, "NULL value not returned as None")
-        finally:
-            con.close()
-
-    def test_Date(self):
-        d1 = self.driver.Date(2002, 12, 25)  # noqa F841
-        d2 = self.driver.DateFromTicks(  # noqa F841
-            time.mktime((2002, 12, 25, 0, 0, 0, 0, 0, 0))
-        )
-        # Can we assume this? API doesn't specify, but it seems implied
-        # self.assertEqual(str(d1),str(d2))
-
-    def test_Time(self):
-        t1 = self.driver.Time(13, 45, 30)  # noqa F841
-        t2 = self.driver.TimeFromTicks(  # noqa F841
-            time.mktime((2001, 1, 1, 13, 45, 30, 0, 0, 0))
-        )
-        # Can we assume this? API doesn't specify, but it seems implied
-        # self.assertEqual(str(t1),str(t2))
-
-    def test_Timestamp(self):
-        t1 = self.driver.Timestamp(2002, 12, 25, 13, 45, 30)  # noqa F841
-        t2 = self.driver.TimestampFromTicks(  # noqa F841
-            time.mktime((2002, 12, 25, 13, 45, 30, 0, 0, 0))
-        )
-        # Can we assume this? API doesn't specify, but it seems implied
-        # self.assertEqual(str(t1),str(t2))
-
-    def test_Binary(self):
-        b = self.driver.Binary(b"Something")
-        b = self.driver.Binary(b"")  # noqa F841
-
-    def test_STRING(self):
-        self.assertTrue(hasattr(self.driver, "STRING"), "module.STRING must be defined")
-
-    def test_BINARY(self):
-        self.assertTrue(
-            hasattr(self.driver, "BINARY"), "module.BINARY must be defined."
-        )
-
-    def test_NUMBER(self):
-        self.assertTrue(
-            hasattr(self.driver, "NUMBER"), "module.NUMBER must be defined."
-        )
-
-    def test_DATETIME(self):
-        self.assertTrue(
-            hasattr(self.driver, "DATETIME"), "module.DATETIME must be defined."
-        )
-
-    def test_ROWID(self):
-        self.assertTrue(hasattr(self.driver, "ROWID"), "module.ROWID must be defined.")
+#!/usr/bin/env python
+""" Python DB API 2.0 driver compliance unit test suite.
+
+    This software is Public Domain and may be used without restrictions.
+
+ "Now we have booze and barflies entering the discussion, plus rumours of
+  DBAs on drugs... and I won't tell you what flashes through my mind each
+  time I read the subject line with 'Anal Compliance' in it.  All around
+  this is turning out to be a thoroughly unwholesome unit test."
+
+    -- Ian Bicking
+"""
+
+__rcs_id__ = "$Id$"
+__version__ = "$Revision$"[11:-2]
+__author__ = "Stuart Bishop <zen@shangri-la.dropbear.id.au>"
+
+import unittest
+import time
+
+# $Log$
+# Revision 1.1.2.1  2006/02/25 03:44:32  adustman
+# Generic DB-API unit test module
+#
+# Revision 1.10  2003/10/09 03:14:14  zenzen
+# Add test for DB API 2.0 optional extension, where database exceptions
+# are exposed as attributes on the Connection object.
+#
+# Revision 1.9  2003/08/13 01:16:36  zenzen
+# Minor tweak from Stefan Fleiter
+#
+# Revision 1.8  2003/04/10 00:13:25  zenzen
+# Changes, as per suggestions by M.-A. Lemburg
+# - Add a table prefix, to ensure namespace collisions can always be avoided
+#
+# Revision 1.7  2003/02/26 23:33:37  zenzen
+# Break out DDL into helper functions, as per request by David Rushby
+#
+# Revision 1.6  2003/02/21 03:04:33  zenzen
+# Stuff from Henrik Ekelund:
+#     added test_None
+#     added test_nextset & hooks
+#
+# Revision 1.5  2003/02/17 22:08:43  zenzen
+# Implement suggestions and code from Henrik Eklund - test that cursor.arraysize
+# defaults to 1 & generic cursor.callproc test added
+#
+# Revision 1.4  2003/02/15 00:16:33  zenzen
+# Changes, as per suggestions and bug reports by M.-A. Lemburg,
+# Matthew T. Kromer, Federico Di Gregorio and Daniel Dittmar
+# - Class renamed
+# - Now a subclass of TestCase, to avoid requiring the driver stub
+#   to use multiple inheritance
+# - Reversed the polarity of buggy test in test_description
+# - Test exception hierarchy correctly
+# - self.populate is now self._populate(), so if a driver stub
+#   overrides self.ddl1 this change propagates
+# - VARCHAR columns now have a width, which will hopefully make the
+#   DDL even more portable (this will be reversed if it causes more problems)
+# - cursor.rowcount being checked after various execute and fetchXXX methods
+# - Check for fetchall and fetchmany returning empty lists after results
+#   are exhausted (already checking for empty lists if select retrieved
+#   nothing
+# - Fix bugs in test_setoutputsize_basic and test_setinputsizes
+#
+
+
+class DatabaseAPI20Test(unittest.TestCase):
+    """Test a database self.driver for DB API 2.0 compatibility.
+    This implementation tests Gadfly, but the TestCase
+    is structured so that other self.drivers can subclass this
+    test case to ensure compiliance with the DB-API. It is
+    expected that this TestCase may be expanded in the future
+    if ambiguities or edge conditions are discovered.
+
+    The 'Optional Extensions' are not yet being tested.
+
+    self.drivers should subclass this test, overriding setUp, tearDown,
+    self.driver, connect_args and connect_kw_args. Class specification
+    should be as follows:
+
+    import dbapi20
+    class mytest(dbapi20.DatabaseAPI20Test):
+       [...]
+
+    Don't 'import DatabaseAPI20Test from dbapi20', or you will
+    confuse the unit tester - just 'import dbapi20'.
+    """
+
+    # The self.driver module. This should be the module where the 'connect'
+    # method is to be found
+    driver = None
+    connect_args = ()  # List of arguments to pass to connect
+    connect_kw_args = {}  # Keyword arguments for connect
+    table_prefix = "dbapi20test_"  # If you need to specify a prefix for tables
+
+    ddl1 = "create table %sbooze (name varchar(20))" % table_prefix
+    ddl2 = "create table %sbarflys (name varchar(20))" % table_prefix
+    xddl1 = "drop table %sbooze" % table_prefix
+    xddl2 = "drop table %sbarflys" % table_prefix
+
+    lowerfunc = "lower"  # Name of stored procedure to convert string->lowercase
+
+    # Some drivers may need to override these helpers, for example adding
+    # a 'commit' after the execute.
+    def executeDDL1(self, cursor):
+        cursor.execute(self.ddl1)
+
+    def executeDDL2(self, cursor):
+        cursor.execute(self.ddl2)
+
+    def setUp(self):
+        """self.drivers should override this method to perform required setup
+        if any is necessary, such as creating the database.
+        """
+        pass
+
+    def tearDown(self):
+        """self.drivers should override this method to perform required cleanup
+        if any is necessary, such as deleting the test database.
+        The default drops the tables that may be created.
+        """
+        con = self._connect()
+        try:
+            cur = con.cursor()
+            for ddl in (self.xddl1, self.xddl2):
+                try:
+                    cur.execute(ddl)
+                    con.commit()
+                except self.driver.Error:
+                    # Assume table didn't exist. Other tests will check if
+                    # execute is busted.
+                    pass
+        finally:
+            con.close()
+
+    def _connect(self):
+        try:
+            return self.driver.connect(*self.connect_args, **self.connect_kw_args)
+        except AttributeError:
+            self.fail("No connect method found in self.driver module")
+
+    def test_connect(self):
+        con = self._connect()
+        con.close()
+
+    def test_apilevel(self):
+        try:
+            # Must exist
+            apilevel = self.driver.apilevel
+            # Must equal 2.0
+            self.assertEqual(apilevel, "2.0")
+        except AttributeError:
+            self.fail("Driver doesn't define apilevel")
+
+    def test_threadsafety(self):
+        try:
+            # Must exist
+            threadsafety = self.driver.threadsafety
+            # Must be a valid value
+            self.assertTrue(threadsafety in (0, 1, 2, 3))
+        except AttributeError:
+            self.fail("Driver doesn't define threadsafety")
+
+    def test_paramstyle(self):
+        try:
+            # Must exist
+            paramstyle = self.driver.paramstyle
+            # Must be a valid value
+            self.assertTrue(
+                paramstyle in ("qmark", "numeric", "named", "format", "pyformat")
+            )
+        except AttributeError:
+            self.fail("Driver doesn't define paramstyle")
+
+    def test_Exceptions(self):
+        # Make sure required exceptions exist, and are in the
+        # defined hierarchy.
+        self.assertTrue(issubclass(self.driver.Warning, Exception))
+        self.assertTrue(issubclass(self.driver.Error, Exception))
+        self.assertTrue(issubclass(self.driver.InterfaceError, self.driver.Error))
+        self.assertTrue(issubclass(self.driver.DatabaseError, self.driver.Error))
+        self.assertTrue(issubclass(self.driver.OperationalError, self.driver.Error))
+        self.assertTrue(issubclass(self.driver.IntegrityError, self.driver.Error))
+        self.assertTrue(issubclass(self.driver.InternalError, self.driver.Error))
+        self.assertTrue(issubclass(self.driver.ProgrammingError, self.driver.Error))
+        self.assertTrue(issubclass(self.driver.NotSupportedError, self.driver.Error))
+
+    def test_ExceptionsAsConnectionAttributes(self):
+        # OPTIONAL EXTENSION
+        # Test for the optional DB API 2.0 extension, where the exceptions
+        # are exposed as attributes on the Connection object
+        # I figure this optional extension will be implemented by any
+        # driver author who is using this test suite, so it is enabled
+        # by default.
+        con = self._connect()
+        drv = self.driver
+        self.assertTrue(con.Warning is drv.Warning)
+        self.assertTrue(con.Error is drv.Error)
+        self.assertTrue(con.InterfaceError is drv.InterfaceError)
+        self.assertTrue(con.DatabaseError is drv.DatabaseError)
+        self.assertTrue(con.OperationalError is drv.OperationalError)
+        self.assertTrue(con.IntegrityError is drv.IntegrityError)
+        self.assertTrue(con.InternalError is drv.InternalError)
+        self.assertTrue(con.ProgrammingError is drv.ProgrammingError)
+        self.assertTrue(con.NotSupportedError is drv.NotSupportedError)
+
+    def test_commit(self):
+        con = self._connect()
+        try:
+            # Commit must work, even if it doesn't do anything
+            con.commit()
+        finally:
+            con.close()
+
+    def test_rollback(self):
+        con = self._connect()
+        # If rollback is defined, it should either work or throw
+        # the documented exception
+        if hasattr(con, "rollback"):
+            try:
+                con.rollback()
+            except self.driver.NotSupportedError:
+                pass
+
+    def test_cursor(self):
+        con = self._connect()
+        try:
+            _ = con.cursor()
+        finally:
+            con.close()
+
+    def test_cursor_isolation(self):
+        con = self._connect()
+        try:
+            # Make sure cursors created from the same connection have
+            # the documented transaction isolation level
+            cur1 = con.cursor()
+            cur2 = con.cursor()
+            self.executeDDL1(cur1)
+            cur1.execute(
+                "insert into %sbooze values ('Victoria Bitter')" % (self.table_prefix)
+            )
+            cur2.execute("select name from %sbooze" % self.table_prefix)
+            booze = cur2.fetchall()
+            self.assertEqual(len(booze), 1)
+            self.assertEqual(len(booze[0]), 1)
+            self.assertEqual(booze[0][0], "Victoria Bitter")
+        finally:
+            con.close()
+
+    def test_description(self):
+        con = self._connect()
+        try:
+            cur = con.cursor()
+            self.executeDDL1(cur)
+            self.assertEqual(
+                cur.description,
+                None,
+                "cursor.description should be none after executing a "
+                "statement that can return no rows (such as DDL)",
+            )
+            cur.execute("select name from %sbooze" % self.table_prefix)
+            self.assertEqual(
+                len(cur.description), 1, "cursor.description describes too many columns"
+            )
+            self.assertEqual(
+                len(cur.description[0]),
+                7,
+                "cursor.description[x] tuples must have 7 elements",
+            )
+            self.assertEqual(
+                cur.description[0][0].lower(),
+                "name",
+                "cursor.description[x][0] must return column name",
+            )
+            self.assertEqual(
+                cur.description[0][1],
+                self.driver.STRING,
+                "cursor.description[x][1] must return column type. Got %r"
+                % cur.description[0][1],
+            )
+
+            # Make sure self.description gets reset
+            self.executeDDL2(cur)
+            self.assertEqual(
+                cur.description,
+                None,
+                "cursor.description not being set to None when executing "
+                "no-result statements (eg. DDL)",
+            )
+        finally:
+            con.close()
+
+    def test_rowcount(self):
+        con = self._connect()
+        try:
+            cur = con.cursor()
+            self.executeDDL1(cur)
+            self.assertEqual(
+                cur.rowcount,
+                -1,
+                "cursor.rowcount should be -1 after executing no-result " "statements",
+            )
+            cur.execute(
+                "insert into %sbooze values ('Victoria Bitter')" % (self.table_prefix)
+            )
+            self.assertTrue(
+                cur.rowcount in (-1, 1),
+                "cursor.rowcount should == number or rows inserted, or "
+                "set to -1 after executing an insert statement",
+            )
+            cur.execute("select name from %sbooze" % self.table_prefix)
+            self.assertTrue(
+                cur.rowcount in (-1, 1),
+                "cursor.rowcount should == number of rows returned, or "
+                "set to -1 after executing a select statement",
+            )
+            self.executeDDL2(cur)
+            self.assertEqual(
+                cur.rowcount,
+                -1,
+                "cursor.rowcount not being reset to -1 after executing "
+                "no-result statements",
+            )
+        finally:
+            con.close()
+
+    lower_func = "lower"
+
+    def test_callproc(self):
+        con = self._connect()
+        try:
+            cur = con.cursor()
+            if self.lower_func and hasattr(cur, "callproc"):
+                r = cur.callproc(self.lower_func, ("FOO",))
+                self.assertEqual(len(r), 1)
+                self.assertEqual(r[0], "FOO")
+                r = cur.fetchall()
+                self.assertEqual(len(r), 1, "callproc produced no result set")
+                self.assertEqual(len(r[0]), 1, "callproc produced invalid result set")
+                self.assertEqual(r[0][0], "foo", "callproc produced invalid results")
+        finally:
+            con.close()
+
+    def test_close(self):
+        con = self._connect()
+        try:
+            cur = con.cursor()
+        finally:
+            con.close()
+
+        # cursor.execute should raise an Error if called after connection
+        # closed
+        self.assertRaises(self.driver.Error, self.executeDDL1, cur)
+
+        # connection.commit should raise an Error if called after connection'
+        # closed.'
+        self.assertRaises(self.driver.Error, con.commit)
+
+        # connection.close should raise an Error if called more than once
+        self.assertRaises(self.driver.Error, con.close)
+
+    def test_execute(self):
+        con = self._connect()
+        try:
+            cur = con.cursor()
+            self._paraminsert(cur)
+        finally:
+            con.close()
+
+    def _paraminsert(self, cur):
+        self.executeDDL1(cur)
+        cur.execute(
+            "insert into %sbooze values ('Victoria Bitter')" % (self.table_prefix)
+        )
+        self.assertTrue(cur.rowcount in (-1, 1))
+
+        if self.driver.paramstyle == "qmark":
+            cur.execute(
+                "insert into %sbooze values (?)" % self.table_prefix, ("Cooper's",)
+            )
+        elif self.driver.paramstyle == "numeric":
+            cur.execute(
+                "insert into %sbooze values (:1)" % self.table_prefix, ("Cooper's",)
+            )
+        elif self.driver.paramstyle == "named":
+            cur.execute(
+                "insert into %sbooze values (:beer)" % self.table_prefix,
+                {"beer": "Cooper's"},
+            )
+        elif self.driver.paramstyle == "format":
+            cur.execute(
+                "insert into %sbooze values (%%s)" % self.table_prefix, ("Cooper's",)
+            )
+        elif self.driver.paramstyle == "pyformat":
+            cur.execute(
+                "insert into %sbooze values (%%(beer)s)" % self.table_prefix,
+                {"beer": "Cooper's"},
+            )
+        else:
+            self.fail("Invalid paramstyle")
+        self.assertTrue(cur.rowcount in (-1, 1))
+
+        cur.execute("select name from %sbooze" % self.table_prefix)
+        res = cur.fetchall()
+        self.assertEqual(len(res), 2, "cursor.fetchall returned too few rows")
+        beers = [res[0][0], res[1][0]]
+        beers.sort()
+        self.assertEqual(
+            beers[0],
+            "Cooper's",
+            "cursor.fetchall retrieved incorrect data, or data inserted " "incorrectly",
+        )
+        self.assertEqual(
+            beers[1],
+            "Victoria Bitter",
+            "cursor.fetchall retrieved incorrect data, or data inserted " "incorrectly",
+        )
+
+    def test_executemany(self):
+        con = self._connect()
+        try:
+            cur = con.cursor()
+            self.executeDDL1(cur)
+            largs = [("Cooper's",), ("Boag's",)]
+            margs = [{"beer": "Cooper's"}, {"beer": "Boag's"}]
+            if self.driver.paramstyle == "qmark":
+                cur.executemany(
+                    "insert into %sbooze values (?)" % self.table_prefix, largs
+                )
+            elif self.driver.paramstyle == "numeric":
+                cur.executemany(
+                    "insert into %sbooze values (:1)" % self.table_prefix, largs
+                )
+            elif self.driver.paramstyle == "named":
+                cur.executemany(
+                    "insert into %sbooze values (:beer)" % self.table_prefix, margs
+                )
+            elif self.driver.paramstyle == "format":
+                cur.executemany(
+                    "insert into %sbooze values (%%s)" % self.table_prefix, largs
+                )
+            elif self.driver.paramstyle == "pyformat":
+                cur.executemany(
+                    "insert into %sbooze values (%%(beer)s)" % (self.table_prefix),
+                    margs,
+                )
+            else:
+                self.fail("Unknown paramstyle")
+            self.assertTrue(
+                cur.rowcount in (-1, 2),
+                "insert using cursor.executemany set cursor.rowcount to "
+                "incorrect value %r" % cur.rowcount,
+            )
+            cur.execute("select name from %sbooze" % self.table_prefix)
+            res = cur.fetchall()
+            self.assertEqual(
+                len(res), 2, "cursor.fetchall retrieved incorrect number of rows"
+            )
+            beers = [res[0][0], res[1][0]]
+            beers.sort()
+            self.assertEqual(beers[0], "Boag's", "incorrect data retrieved")
+            self.assertEqual(beers[1], "Cooper's", "incorrect data retrieved")
+        finally:
+            con.close()
+
+    def test_fetchone(self):
+        con = self._connect()
+        try:
+            cur = con.cursor()
+
+            # cursor.fetchone should raise an Error if called before
+            # executing a select-type query
+            self.assertRaises(self.driver.Error, cur.fetchone)
+
+            # cursor.fetchone should raise an Error if called after
+            # executing a query that cannot return rows
+            self.executeDDL1(cur)
+            self.assertRaises(self.driver.Error, cur.fetchone)
+
+            cur.execute("select name from %sbooze" % self.table_prefix)
+            self.assertEqual(
+                cur.fetchone(),
+                None,
+                "cursor.fetchone should return None if a query retrieves " "no rows",
+            )
+            self.assertTrue(cur.rowcount in (-1, 0))
+
+            # cursor.fetchone should raise an Error if called after
+            # executing a query that cannot return rows
+            cur.execute(
+                "insert into %sbooze values ('Victoria Bitter')" % (self.table_prefix)
+            )
+            self.assertRaises(self.driver.Error, cur.fetchone)
+
+            cur.execute("select name from %sbooze" % self.table_prefix)
+            r = cur.fetchone()
+            self.assertEqual(
+                len(r), 1, "cursor.fetchone should have retrieved a single row"
+            )
+            self.assertEqual(
+                r[0], "Victoria Bitter", "cursor.fetchone retrieved incorrect data"
+            )
+            self.assertEqual(
+                cur.fetchone(),
+                None,
+                "cursor.fetchone should return None if no more rows available",
+            )
+            self.assertTrue(cur.rowcount in (-1, 1))
+        finally:
+            con.close()
+
+    samples = [
+        "Carlton Cold",
+        "Carlton Draft",
+        "Mountain Goat",
+        "Redback",
+        "Victoria Bitter",
+        "XXXX",
+    ]
+
+    def _populate(self):
+        """Return a list of sql commands to setup the DB for the fetch
+        tests.
+        """
+        populate = [
+            f"insert into {self.table_prefix}booze values ('{s}')" for s in self.samples
+        ]
+        return populate
+
+    def test_fetchmany(self):
+        con = self._connect()
+        try:
+            cur = con.cursor()
+
+            # cursor.fetchmany should raise an Error if called without
+            # issuing a query
+            self.assertRaises(self.driver.Error, cur.fetchmany, 4)
+
+            self.executeDDL1(cur)
+            for sql in self._populate():
+                cur.execute(sql)
+
+            cur.execute("select name from %sbooze" % self.table_prefix)
+            r = cur.fetchmany()
+            self.assertEqual(
+                len(r),
+                1,
+                "cursor.fetchmany retrieved incorrect number of rows, "
+                "default of arraysize is one.",
+            )
+            cur.arraysize = 10
+            r = cur.fetchmany(3)  # Should get 3 rows
+            self.assertEqual(
+                len(r), 3, "cursor.fetchmany retrieved incorrect number of rows"
+            )
+            r = cur.fetchmany(4)  # Should get 2 more
+            self.assertEqual(
+                len(r), 2, "cursor.fetchmany retrieved incorrect number of rows"
+            )
+            r = cur.fetchmany(4)  # Should be an empty sequence
+            self.assertEqual(
+                len(r),
+                0,
+                "cursor.fetchmany should return an empty sequence after "
+                "results are exhausted",
+            )
+            self.assertTrue(cur.rowcount in (-1, 6))
+
+            # Same as above, using cursor.arraysize
+            cur.arraysize = 4
+            cur.execute("select name from %sbooze" % self.table_prefix)
+            r = cur.fetchmany()  # Should get 4 rows
+            self.assertEqual(
+                len(r), 4, "cursor.arraysize not being honoured by fetchmany"
+            )
+            r = cur.fetchmany()  # Should get 2 more
+            self.assertEqual(len(r), 2)
+            r = cur.fetchmany()  # Should be an empty sequence
+            self.assertEqual(len(r), 0)
+            self.assertTrue(cur.rowcount in (-1, 6))
+
+            cur.arraysize = 6
+            cur.execute("select name from %sbooze" % self.table_prefix)
+            rows = cur.fetchmany()  # Should get all rows
+            self.assertTrue(cur.rowcount in (-1, 6))
+            self.assertEqual(len(rows), 6)
+            self.assertEqual(len(rows), 6)
+            rows = [r[0] for r in rows]
+            rows.sort()
+
+            # Make sure we get the right data back out
+            for i in range(0, 6):
+                self.assertEqual(
+                    rows[i],
+                    self.samples[i],
+                    "incorrect data retrieved by cursor.fetchmany",
+                )
+
+            rows = cur.fetchmany()  # Should return an empty list
+            self.assertEqual(
+                len(rows),
+                0,
+                "cursor.fetchmany should return an empty sequence if "
+                "called after the whole result set has been fetched",
+            )
+            self.assertTrue(cur.rowcount in (-1, 6))
+
+            self.executeDDL2(cur)
+            cur.execute("select name from %sbarflys" % self.table_prefix)
+            r = cur.fetchmany()  # Should get empty sequence
+            self.assertEqual(
+                len(r),
+                0,
+                "cursor.fetchmany should return an empty sequence if "
+                "query retrieved no rows",
+            )
+            self.assertTrue(cur.rowcount in (-1, 0))
+
+        finally:
+            con.close()
+
+    def test_fetchall(self):
+        con = self._connect()
+        try:
+            cur = con.cursor()
+            # cursor.fetchall should raise an Error if called
+            # without executing a query that may return rows (such
+            # as a select)
+            self.assertRaises(self.driver.Error, cur.fetchall)
+
+            self.executeDDL1(cur)
+            for sql in self._populate():
+                cur.execute(sql)
+
+            # cursor.fetchall should raise an Error if called
+            # after executing a statement that cannot return rows
+            self.assertRaises(self.driver.Error, cur.fetchall)
+
+            cur.execute("select name from %sbooze" % self.table_prefix)
+            rows = cur.fetchall()
+            self.assertTrue(cur.rowcount in (-1, len(self.samples)))
+            self.assertEqual(
+                len(rows),
+                len(self.samples),
+                "cursor.fetchall did not retrieve all rows",
+            )
+            rows = [r[0] for r in rows]
+            rows.sort()
+            for i in range(0, len(self.samples)):
+                self.assertEqual(
+                    rows[i], self.samples[i], "cursor.fetchall retrieved incorrect rows"
+                )
+            rows = cur.fetchall()
+            self.assertEqual(
+                len(rows),
+                0,
+                "cursor.fetchall should return an empty list if called "
+                "after the whole result set has been fetched",
+            )
+            self.assertTrue(cur.rowcount in (-1, len(self.samples)))
+
+            self.executeDDL2(cur)
+            cur.execute("select name from %sbarflys" % self.table_prefix)
+            rows = cur.fetchall()
+            self.assertTrue(cur.rowcount in (-1, 0))
+            self.assertEqual(
+                len(rows),
+                0,
+                "cursor.fetchall should return an empty list if "
+                "a select query returns no rows",
+            )
+
+        finally:
+            con.close()
+
+    def test_mixedfetch(self):
+        con = self._connect()
+        try:
+            cur = con.cursor()
+            self.executeDDL1(cur)
+            for sql in self._populate():
+                cur.execute(sql)
+
+            cur.execute("select name from %sbooze" % self.table_prefix)
+            rows1 = cur.fetchone()
+            rows23 = cur.fetchmany(2)
+            rows4 = cur.fetchone()
+            rows56 = cur.fetchall()
+            self.assertTrue(cur.rowcount in (-1, 6))
+            self.assertEqual(
+                len(rows23), 2, "fetchmany returned incorrect number of rows"
+            )
+            self.assertEqual(
+                len(rows56), 2, "fetchall returned incorrect number of rows"
+            )
+
+            rows = [rows1[0]]
+            rows.extend([rows23[0][0], rows23[1][0]])
+            rows.append(rows4[0])
+            rows.extend([rows56[0][0], rows56[1][0]])
+            rows.sort()
+            for i in range(0, len(self.samples)):
+                self.assertEqual(
+                    rows[i], self.samples[i], "incorrect data retrieved or inserted"
+                )
+        finally:
+            con.close()
+
+    def help_nextset_setUp(self, cur):
+        """Should create a procedure called deleteme
+        that returns two result sets, first the
+        number of rows in booze then "name from booze"
+        """
+        raise NotImplementedError("Helper not implemented")
+        # sql="""
+        #    create procedure deleteme as
+        #    begin
+        #        select count(*) from booze
+        #        select name from booze
+        #    end
+        # """
+        # cur.execute(sql)
+
+    def help_nextset_tearDown(self, cur):
+        "If cleaning up is needed after nextSetTest"
+        raise NotImplementedError("Helper not implemented")
+        # cur.execute("drop procedure deleteme")
+
+    def test_nextset(self):
+        con = self._connect()
+        try:
+            cur = con.cursor()
+            if not hasattr(cur, "nextset"):
+                return
+
+            try:
+                self.executeDDL1(cur)
+                sql = self._populate()
+                for sql in self._populate():
+                    cur.execute(sql)
+
+                self.help_nextset_setUp(cur)
+
+                cur.callproc("deleteme")
+                numberofrows = cur.fetchone()
+                assert numberofrows[0] == len(self.samples)
+                assert cur.nextset()
+                names = cur.fetchall()
+                assert len(names) == len(self.samples)
+                s = cur.nextset()
+                assert s is None, "No more return sets, should return None"
+            finally:
+                self.help_nextset_tearDown(cur)
+
+        finally:
+            con.close()
+
+    def test_nextset(self):  # noqa: F811
+        raise NotImplementedError("Drivers need to override this test")
+
+    def test_arraysize(self):
+        # Not much here - rest of the tests for this are in test_fetchmany
+        con = self._connect()
+        try:
+            cur = con.cursor()
+            self.assertTrue(
+                hasattr(cur, "arraysize"), "cursor.arraysize must be defined"
+            )
+        finally:
+            con.close()
+
+    def test_setinputsizes(self):
+        con = self._connect()
+        try:
+            cur = con.cursor()
+            cur.setinputsizes((25,))
+            self._paraminsert(cur)  # Make sure cursor still works
+        finally:
+            con.close()
+
+    def test_setoutputsize_basic(self):
+        # Basic test is to make sure setoutputsize doesn't blow up
+        con = self._connect()
+        try:
+            cur = con.cursor()
+            cur.setoutputsize(1000)
+            cur.setoutputsize(2000, 0)
+            self._paraminsert(cur)  # Make sure the cursor still works
+        finally:
+            con.close()
+
+    def test_setoutputsize(self):
+        # Real test for setoutputsize is driver dependent
+        raise NotImplementedError("Driver need to override this test")
+
+    def test_None(self):
+        con = self._connect()
+        try:
+            cur = con.cursor()
+            self.executeDDL1(cur)
+            cur.execute("insert into %sbooze values (NULL)" % self.table_prefix)
+            cur.execute("select name from %sbooze" % self.table_prefix)
+            r = cur.fetchall()
+            self.assertEqual(len(r), 1)
+            self.assertEqual(len(r[0]), 1)
+            self.assertEqual(r[0][0], None, "NULL value not returned as None")
+        finally:
+            con.close()
+
+    def test_Date(self):
+        d1 = self.driver.Date(2002, 12, 25)  # noqa F841
+        d2 = self.driver.DateFromTicks(  # noqa F841
+            time.mktime((2002, 12, 25, 0, 0, 0, 0, 0, 0))
+        )
+        # Can we assume this? API doesn't specify, but it seems implied
+        # self.assertEqual(str(d1),str(d2))
+
+    def test_Time(self):
+        t1 = self.driver.Time(13, 45, 30)  # noqa F841
+        t2 = self.driver.TimeFromTicks(  # noqa F841
+            time.mktime((2001, 1, 1, 13, 45, 30, 0, 0, 0))
+        )
+        # Can we assume this? API doesn't specify, but it seems implied
+        # self.assertEqual(str(t1),str(t2))
+
+    def test_Timestamp(self):
+        t1 = self.driver.Timestamp(2002, 12, 25, 13, 45, 30)  # noqa F841
+        t2 = self.driver.TimestampFromTicks(  # noqa F841
+            time.mktime((2002, 12, 25, 13, 45, 30, 0, 0, 0))
+        )
+        # Can we assume this? API doesn't specify, but it seems implied
+        # self.assertEqual(str(t1),str(t2))
+
+    def test_Binary(self):
+        b = self.driver.Binary(b"Something")
+        b = self.driver.Binary(b"")  # noqa F841
+
+    def test_STRING(self):
+        self.assertTrue(hasattr(self.driver, "STRING"), "module.STRING must be defined")
+
+    def test_BINARY(self):
+        self.assertTrue(
+            hasattr(self.driver, "BINARY"), "module.BINARY must be defined."
+        )
+
+    def test_NUMBER(self):
+        self.assertTrue(
+            hasattr(self.driver, "NUMBER"), "module.NUMBER must be defined."
+        )
+
+    def test_DATETIME(self):
+        self.assertTrue(
+            hasattr(self.driver, "DATETIME"), "module.DATETIME must be defined."
+        )
+
+    def test_ROWID(self):
+        self.assertTrue(hasattr(self.driver, "ROWID"), "module.ROWID must be defined.")
```

### Comparing `mysqlclient-2.2.0/tests/test_MySQLdb_capabilities.py` & `mysqlclient-2.2.0rc1/tests/test_MySQLdb_capabilities.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,205 +1,205 @@
-#!/usr/bin/env python
-import capabilities
-from datetime import timedelta
-from contextlib import closing
-import unittest
-import MySQLdb
-from configdb import connection_factory
-import warnings
-
-
-warnings.filterwarnings("ignore")
-
-
-class test_MySQLdb(capabilities.DatabaseTest):
-    db_module = MySQLdb
-    connect_args = ()
-    connect_kwargs = dict(
-        use_unicode=True, sql_mode="ANSI,STRICT_TRANS_TABLES,TRADITIONAL"
-    )
-    create_table_extra = "ENGINE=INNODB CHARACTER SET UTF8"
-    leak_test = False
-
-    def quote_identifier(self, ident):
-        return "`%s`" % ident
-
-    def test_TIME(self):
-        def generator(row, col):
-            return timedelta(0, row * 8000)
-
-        self.check_data_integrity(("col1 TIME",), generator)
-
-    def test_TINYINT(self):
-        # Number data
-        def generator(row, col):
-            v = (row * row) % 256
-            if v > 127:
-                v = v - 256
-            return v
-
-        self.check_data_integrity(("col1 TINYINT",), generator)
-
-    def test_stored_procedures(self):
-        db = self.connection
-        c = self.cursor
-        self.create_table(("pos INT", "tree CHAR(20)"))
-        c.executemany(
-            "INSERT INTO %s (pos,tree) VALUES (%%s,%%s)" % self.table,
-            list(enumerate("ash birch cedar Lärche pine".split())),
-        )
-        db.commit()
-
-        c.execute(
-            """
-        CREATE PROCEDURE test_sp(IN t VARCHAR(255))
-        BEGIN
-            SELECT pos FROM %s WHERE tree = t;
-        END
-        """
-            % self.table
-        )
-        db.commit()
-
-        c.callproc("test_sp", ("Lärche",))
-        rows = c.fetchall()
-        self.assertEqual(len(rows), 1)
-        self.assertEqual(rows[0][0], 3)
-        c.nextset()
-
-        c.execute("DROP PROCEDURE test_sp")
-        c.execute("drop table %s" % (self.table))
-
-    def test_small_CHAR(self):
-        # Character data
-        def generator(row, col):
-            i = (row * col + 62) % 256
-            if i == 62:
-                return ""
-            if i == 63:
-                return None
-            return chr(i)
-
-        self.check_data_integrity(("col1 char(1)", "col2 char(1)"), generator)
-
-    def test_BIT(self):
-        c = self.cursor
-        try:
-            c.execute(
-                """create table test_BIT (
-                b3 BIT(3),
-                b7 BIT(10),
-                b64 BIT(64))"""
-            )
-
-            one64 = "1" * 64
-            c.execute(
-                "insert into test_BIT (b3, b7, b64)"
-                " VALUES (b'011', b'1111111111', b'%s')" % one64
-            )
-
-            c.execute("SELECT b3, b7, b64 FROM test_BIT")
-            row = c.fetchone()
-            self.assertEqual(row[0], b"\x03")
-            self.assertEqual(row[1], b"\x03\xff")
-            self.assertEqual(row[2], b"\xff" * 8)
-        finally:
-            c.execute("drop table if exists test_BIT")
-
-    def test_MULTIPOLYGON(self):
-        c = self.cursor
-        try:
-            c.execute(
-                """create table test_MULTIPOLYGON (
-                id INTEGER PRIMARY KEY,
-                border MULTIPOLYGON)"""
-            )
-
-            c.execute(
-                """
-INSERT INTO test_MULTIPOLYGON
-            (id, border)
-VALUES      (1,
-             ST_Geomfromtext(
-'MULTIPOLYGON(((1 1, 1 -1, -1 -1, -1 1, 1 1)),((1 1, 3 1, 3 3, 1 3, 1 1)))'))
-"""
-            )
-
-            c.execute("SELECT id, ST_AsText(border) FROM test_MULTIPOLYGON")
-            row = c.fetchone()
-            self.assertEqual(row[0], 1)
-            self.assertEqual(
-                row[1],
-                "MULTIPOLYGON(((1 1,1 -1,-1 -1,-1 1,1 1)),((1 1,3 1,3 3,1 3,1 1)))",
-            )
-
-            c.execute("SELECT id, ST_AsWKB(border) FROM test_MULTIPOLYGON")
-            row = c.fetchone()
-            self.assertEqual(row[0], 1)
-            self.assertNotEqual(len(row[1]), 0)
-
-            c.execute("SELECT id, border FROM test_MULTIPOLYGON")
-            row = c.fetchone()
-            self.assertEqual(row[0], 1)
-            self.assertNotEqual(len(row[1]), 0)
-        finally:
-            c.execute("drop table if exists test_MULTIPOLYGON")
-
-    def test_bug_2671682(self):
-        from MySQLdb.constants import ER
-
-        try:
-            self.cursor.execute("describe some_non_existent_table")
-        except self.connection.ProgrammingError as msg:
-            self.assertTrue(str(ER.NO_SUCH_TABLE) in str(msg))
-
-    def test_bug_3514287(self):
-        c = self.cursor
-        try:
-            c.execute(
-                """create table bug_3541287 (
-                c1 CHAR(10),
-                t1 TIMESTAMP)"""
-            )
-            c.execute("insert into bug_3541287 (c1,t1) values (%s, NOW())", ("blah",))
-        finally:
-            c.execute("drop table if exists bug_3541287")
-
-    def test_ping(self):
-        self.connection.ping()
-
-    def test_reraise_exception(self):
-        c = self.cursor
-        try:
-            c.execute("SELECT x FROM not_existing_table")
-        except MySQLdb.ProgrammingError as e:
-            self.assertEqual(e.args[0], 1146)
-            return
-        self.fail("Should raise ProgrammingError")
-
-    def test_binary_prefix(self):
-        # verify prefix behaviour when enabled, disabled and for default (disabled)
-        for binary_prefix in (True, False, None):
-            kwargs = self.connect_kwargs.copy()
-            # needs to be set to can guarantee CHARSET response for normal strings
-            kwargs["charset"] = "utf8mb4"
-            if binary_prefix is not None:
-                kwargs["binary_prefix"] = binary_prefix
-
-            with closing(connection_factory(**kwargs)) as conn:
-                with closing(conn.cursor()) as c:
-                    c.execute("SELECT CHARSET(%s)", (MySQLdb.Binary(b"raw bytes"),))
-                    self.assertEqual(
-                        c.fetchall()[0][0], "binary" if binary_prefix else "utf8mb4"
-                    )
-                    # normal strings should not get prefix
-                    c.execute("SELECT CHARSET(%s)", ("str",))
-                    self.assertEqual(c.fetchall()[0][0], "utf8mb4")
-
-
-if __name__ == "__main__":
-    if test_MySQLdb.leak_test:
-        import gc
-
-        gc.enable()
-        gc.set_debug(gc.DEBUG_LEAK)
-    unittest.main()
+#!/usr/bin/env python
+import capabilities
+from datetime import timedelta
+from contextlib import closing
+import unittest
+import MySQLdb
+from configdb import connection_factory
+import warnings
+
+
+warnings.filterwarnings("ignore")
+
+
+class test_MySQLdb(capabilities.DatabaseTest):
+    db_module = MySQLdb
+    connect_args = ()
+    connect_kwargs = dict(
+        use_unicode=True, sql_mode="ANSI,STRICT_TRANS_TABLES,TRADITIONAL"
+    )
+    create_table_extra = "ENGINE=INNODB CHARACTER SET UTF8"
+    leak_test = False
+
+    def quote_identifier(self, ident):
+        return "`%s`" % ident
+
+    def test_TIME(self):
+        def generator(row, col):
+            return timedelta(0, row * 8000)
+
+        self.check_data_integrity(("col1 TIME",), generator)
+
+    def test_TINYINT(self):
+        # Number data
+        def generator(row, col):
+            v = (row * row) % 256
+            if v > 127:
+                v = v - 256
+            return v
+
+        self.check_data_integrity(("col1 TINYINT",), generator)
+
+    def test_stored_procedures(self):
+        db = self.connection
+        c = self.cursor
+        self.create_table(("pos INT", "tree CHAR(20)"))
+        c.executemany(
+            "INSERT INTO %s (pos,tree) VALUES (%%s,%%s)" % self.table,
+            list(enumerate("ash birch cedar Lärche pine".split())),
+        )
+        db.commit()
+
+        c.execute(
+            """
+        CREATE PROCEDURE test_sp(IN t VARCHAR(255))
+        BEGIN
+            SELECT pos FROM %s WHERE tree = t;
+        END
+        """
+            % self.table
+        )
+        db.commit()
+
+        c.callproc("test_sp", ("Lärche",))
+        rows = c.fetchall()
+        self.assertEqual(len(rows), 1)
+        self.assertEqual(rows[0][0], 3)
+        c.nextset()
+
+        c.execute("DROP PROCEDURE test_sp")
+        c.execute("drop table %s" % (self.table))
+
+    def test_small_CHAR(self):
+        # Character data
+        def generator(row, col):
+            i = (row * col + 62) % 256
+            if i == 62:
+                return ""
+            if i == 63:
+                return None
+            return chr(i)
+
+        self.check_data_integrity(("col1 char(1)", "col2 char(1)"), generator)
+
+    def test_BIT(self):
+        c = self.cursor
+        try:
+            c.execute(
+                """create table test_BIT (
+                b3 BIT(3),
+                b7 BIT(10),
+                b64 BIT(64))"""
+            )
+
+            one64 = "1" * 64
+            c.execute(
+                "insert into test_BIT (b3, b7, b64)"
+                " VALUES (b'011', b'1111111111', b'%s')" % one64
+            )
+
+            c.execute("SELECT b3, b7, b64 FROM test_BIT")
+            row = c.fetchone()
+            self.assertEqual(row[0], b"\x03")
+            self.assertEqual(row[1], b"\x03\xff")
+            self.assertEqual(row[2], b"\xff" * 8)
+        finally:
+            c.execute("drop table if exists test_BIT")
+
+    def test_MULTIPOLYGON(self):
+        c = self.cursor
+        try:
+            c.execute(
+                """create table test_MULTIPOLYGON (
+                id INTEGER PRIMARY KEY,
+                border MULTIPOLYGON)"""
+            )
+
+            c.execute(
+                """
+INSERT INTO test_MULTIPOLYGON
+            (id, border)
+VALUES      (1,
+             ST_Geomfromtext(
+'MULTIPOLYGON(((1 1, 1 -1, -1 -1, -1 1, 1 1)),((1 1, 3 1, 3 3, 1 3, 1 1)))'))
+"""
+            )
+
+            c.execute("SELECT id, ST_AsText(border) FROM test_MULTIPOLYGON")
+            row = c.fetchone()
+            self.assertEqual(row[0], 1)
+            self.assertEqual(
+                row[1],
+                "MULTIPOLYGON(((1 1,1 -1,-1 -1,-1 1,1 1)),((1 1,3 1,3 3,1 3,1 1)))",
+            )
+
+            c.execute("SELECT id, ST_AsWKB(border) FROM test_MULTIPOLYGON")
+            row = c.fetchone()
+            self.assertEqual(row[0], 1)
+            self.assertNotEqual(len(row[1]), 0)
+
+            c.execute("SELECT id, border FROM test_MULTIPOLYGON")
+            row = c.fetchone()
+            self.assertEqual(row[0], 1)
+            self.assertNotEqual(len(row[1]), 0)
+        finally:
+            c.execute("drop table if exists test_MULTIPOLYGON")
+
+    def test_bug_2671682(self):
+        from MySQLdb.constants import ER
+
+        try:
+            self.cursor.execute("describe some_non_existent_table")
+        except self.connection.ProgrammingError as msg:
+            self.assertTrue(str(ER.NO_SUCH_TABLE) in str(msg))
+
+    def test_bug_3514287(self):
+        c = self.cursor
+        try:
+            c.execute(
+                """create table bug_3541287 (
+                c1 CHAR(10),
+                t1 TIMESTAMP)"""
+            )
+            c.execute("insert into bug_3541287 (c1,t1) values (%s, NOW())", ("blah",))
+        finally:
+            c.execute("drop table if exists bug_3541287")
+
+    def test_ping(self):
+        self.connection.ping()
+
+    def test_reraise_exception(self):
+        c = self.cursor
+        try:
+            c.execute("SELECT x FROM not_existing_table")
+        except MySQLdb.ProgrammingError as e:
+            self.assertEqual(e.args[0], 1146)
+            return
+        self.fail("Should raise ProgrammingError")
+
+    def test_binary_prefix(self):
+        # verify prefix behaviour when enabled, disabled and for default (disabled)
+        for binary_prefix in (True, False, None):
+            kwargs = self.connect_kwargs.copy()
+            # needs to be set to can guarantee CHARSET response for normal strings
+            kwargs["charset"] = "utf8mb4"
+            if binary_prefix is not None:
+                kwargs["binary_prefix"] = binary_prefix
+
+            with closing(connection_factory(**kwargs)) as conn:
+                with closing(conn.cursor()) as c:
+                    c.execute("SELECT CHARSET(%s)", (MySQLdb.Binary(b"raw bytes"),))
+                    self.assertEqual(
+                        c.fetchall()[0][0], "binary" if binary_prefix else "utf8mb4"
+                    )
+                    # normal strings should not get prefix
+                    c.execute("SELECT CHARSET(%s)", ("str",))
+                    self.assertEqual(c.fetchall()[0][0], "utf8mb4")
+
+
+if __name__ == "__main__":
+    if test_MySQLdb.leak_test:
+        import gc
+
+        gc.enable()
+        gc.set_debug(gc.DEBUG_LEAK)
+    unittest.main()
```

### Comparing `mysqlclient-2.2.0/tests/test_MySQLdb_dbapi20.py` & `mysqlclient-2.2.0rc1/tests/test_MySQLdb_dbapi20.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,231 +1,231 @@
-#!/usr/bin/env python
-import dbapi20
-import unittest
-import MySQLdb
-from configdb import connection_kwargs
-import warnings
-
-warnings.simplefilter("ignore")
-
-
-class test_MySQLdb(dbapi20.DatabaseAPI20Test):
-    driver = MySQLdb
-    connect_args = ()
-    connect_kw_args = connection_kwargs(
-        dict(sql_mode="ANSI,STRICT_TRANS_TABLES,TRADITIONAL")
-    )
-
-    def test_setoutputsize(self):
-        pass
-
-    def test_setoutputsize_basic(self):
-        pass
-
-    """The tests on fetchone and fetchall and rowcount bogusly
-    test for an exception if the statement cannot return a
-    result set. MySQL always returns a result set; it's just that
-    some things return empty result sets."""
-
-    def test_fetchall(self):
-        con = self._connect()
-        try:
-            cur = con.cursor()
-            # cursor.fetchall should raise an Error if called
-            # without executing a query that may return rows (such
-            # as a select)
-            self.assertRaises(self.driver.Error, cur.fetchall)
-
-            self.executeDDL1(cur)
-            for sql in self._populate():
-                cur.execute(sql)
-
-            # cursor.fetchall should raise an Error if called
-            # after executing a statement that cannot return rows
-            # self.assertRaises(self.driver.Error,cur.fetchall)
-
-            cur.execute("select name from %sbooze" % self.table_prefix)
-            rows = cur.fetchall()
-            self.assertTrue(cur.rowcount in (-1, len(self.samples)))
-            self.assertEqual(
-                len(rows),
-                len(self.samples),
-                "cursor.fetchall did not retrieve all rows",
-            )
-            rows = [r[0] for r in rows]
-            rows.sort()
-            for i in range(0, len(self.samples)):
-                self.assertEqual(
-                    rows[i], self.samples[i], "cursor.fetchall retrieved incorrect rows"
-                )
-            rows = cur.fetchall()
-            self.assertEqual(
-                len(rows),
-                0,
-                "cursor.fetchall should return an empty list if called "
-                "after the whole result set has been fetched",
-            )
-            self.assertTrue(cur.rowcount in (-1, len(self.samples)))
-
-            self.executeDDL2(cur)
-            cur.execute("select name from %sbarflys" % self.table_prefix)
-            rows = cur.fetchall()
-            self.assertTrue(cur.rowcount in (-1, 0))
-            self.assertEqual(
-                len(rows),
-                0,
-                "cursor.fetchall should return an empty list if "
-                "a select query returns no rows",
-            )
-
-        finally:
-            con.close()
-
-    def test_fetchone(self):
-        con = self._connect()
-        try:
-            cur = con.cursor()
-
-            # cursor.fetchone should raise an Error if called before
-            # executing a select-type query
-            self.assertRaises(self.driver.Error, cur.fetchone)
-
-            # cursor.fetchone should raise an Error if called after
-            # executing a query that cannot return rows
-            self.executeDDL1(cur)
-            # self.assertRaises(self.driver.Error,cur.fetchone)
-
-            cur.execute("select name from %sbooze" % self.table_prefix)
-            self.assertEqual(
-                cur.fetchone(),
-                None,
-                "cursor.fetchone should return None if a query retrieves " "no rows",
-            )
-            self.assertTrue(cur.rowcount in (-1, 0))
-
-            # cursor.fetchone should raise an Error if called after
-            # executing a query that cannot return rows
-            cur.execute(
-                "insert into %sbooze values ('Victoria Bitter')" % (self.table_prefix)
-            )
-            # self.assertRaises(self.driver.Error,cur.fetchone)
-
-            cur.execute("select name from %sbooze" % self.table_prefix)
-            r = cur.fetchone()
-            self.assertEqual(
-                len(r), 1, "cursor.fetchone should have retrieved a single row"
-            )
-            self.assertEqual(
-                r[0], "Victoria Bitter", "cursor.fetchone retrieved incorrect data"
-            )
-            # self.assertEqual(
-            #    cur.fetchone(),
-            #    None,
-            #    "cursor.fetchone should return None if no more rows available",
-            # )
-            self.assertTrue(cur.rowcount in (-1, 1))
-        finally:
-            con.close()
-
-    # Same complaint as for fetchall and fetchone
-    def test_rowcount(self):
-        con = self._connect()
-        try:
-            cur = con.cursor()
-            self.executeDDL1(cur)
-            #             self.assertEqual(cur.rowcount,-1,
-            #                 'cursor.rowcount should be -1 after executing no-result '
-            #                 'statements'
-            #                 )
-            cur.execute(
-                "insert into %sbooze values ('Victoria Bitter')" % (self.table_prefix)
-            )
-            #             self.assertTrue(cur.rowcount in (-1,1),
-            #                 'cursor.rowcount should == number or rows inserted, or '
-            #                 'set to -1 after executing an insert statement'
-            #                 )
-            cur.execute("select name from %sbooze" % self.table_prefix)
-            self.assertTrue(
-                cur.rowcount in (-1, 1),
-                "cursor.rowcount should == number of rows returned, or "
-                "set to -1 after executing a select statement",
-            )
-            self.executeDDL2(cur)
-        #             self.assertEqual(cur.rowcount,-1,
-        #                 'cursor.rowcount not being reset to -1 after executing '
-        #                 'no-result statements'
-        #                 )
-        finally:
-            con.close()
-
-    def test_callproc(self):
-        pass  # performed in test_MySQL_capabilities
-
-    def help_nextset_setUp(self, cur):
-        """
-        Should create a procedure called deleteme
-        that returns two result sets, first the
-        number of rows in booze then "name from booze"
-        """
-        sql = """
-           create procedure deleteme()
-           begin
-               select count(*) from %(tp)sbooze;
-               select name from %(tp)sbooze;
-           end
-        """ % dict(
-            tp=self.table_prefix
-        )
-        cur.execute(sql)
-
-    def help_nextset_tearDown(self, cur):
-        "If cleaning up is needed after nextSetTest"
-        cur.execute("drop procedure deleteme")
-
-    def test_nextset(self):
-        # from warnings import warn
-
-        con = self._connect()
-        try:
-            cur = con.cursor()
-            if not hasattr(cur, "nextset"):
-                return
-
-            try:
-                self.executeDDL1(cur)
-                sql = self._populate()
-                for sql in self._populate():
-                    cur.execute(sql)
-
-                self.help_nextset_setUp(cur)
-
-                cur.callproc("deleteme")
-                numberofrows = cur.fetchone()
-                assert numberofrows[0] == len(self.samples)
-                assert cur.nextset()
-                names = cur.fetchall()
-                assert len(names) == len(self.samples)
-                s = cur.nextset()
-                if s:
-                    empty = cur.fetchall()
-                    self.assertEqual(
-                        len(empty), 0, "non-empty result set after other result sets"
-                    )
-                    # warn(
-                    #    ": ".join(
-                    #        [
-                    #            "Incompatibility",
-                    #            "MySQL returns an empty result set for the CALL itself"
-                    #        ]
-                    #    ),
-                    #    Warning,
-                    # )
-                # assert s == None, "No more return sets, should return None"
-            finally:
-                self.help_nextset_tearDown(cur)
-
-        finally:
-            con.close()
-
-
-if __name__ == "__main__":
-    unittest.main()
+#!/usr/bin/env python
+import dbapi20
+import unittest
+import MySQLdb
+from configdb import connection_kwargs
+import warnings
+
+warnings.simplefilter("ignore")
+
+
+class test_MySQLdb(dbapi20.DatabaseAPI20Test):
+    driver = MySQLdb
+    connect_args = ()
+    connect_kw_args = connection_kwargs(
+        dict(sql_mode="ANSI,STRICT_TRANS_TABLES,TRADITIONAL")
+    )
+
+    def test_setoutputsize(self):
+        pass
+
+    def test_setoutputsize_basic(self):
+        pass
+
+    """The tests on fetchone and fetchall and rowcount bogusly
+    test for an exception if the statement cannot return a
+    result set. MySQL always returns a result set; it's just that
+    some things return empty result sets."""
+
+    def test_fetchall(self):
+        con = self._connect()
+        try:
+            cur = con.cursor()
+            # cursor.fetchall should raise an Error if called
+            # without executing a query that may return rows (such
+            # as a select)
+            self.assertRaises(self.driver.Error, cur.fetchall)
+
+            self.executeDDL1(cur)
+            for sql in self._populate():
+                cur.execute(sql)
+
+            # cursor.fetchall should raise an Error if called
+            # after executing a statement that cannot return rows
+            # self.assertRaises(self.driver.Error,cur.fetchall)
+
+            cur.execute("select name from %sbooze" % self.table_prefix)
+            rows = cur.fetchall()
+            self.assertTrue(cur.rowcount in (-1, len(self.samples)))
+            self.assertEqual(
+                len(rows),
+                len(self.samples),
+                "cursor.fetchall did not retrieve all rows",
+            )
+            rows = [r[0] for r in rows]
+            rows.sort()
+            for i in range(0, len(self.samples)):
+                self.assertEqual(
+                    rows[i], self.samples[i], "cursor.fetchall retrieved incorrect rows"
+                )
+            rows = cur.fetchall()
+            self.assertEqual(
+                len(rows),
+                0,
+                "cursor.fetchall should return an empty list if called "
+                "after the whole result set has been fetched",
+            )
+            self.assertTrue(cur.rowcount in (-1, len(self.samples)))
+
+            self.executeDDL2(cur)
+            cur.execute("select name from %sbarflys" % self.table_prefix)
+            rows = cur.fetchall()
+            self.assertTrue(cur.rowcount in (-1, 0))
+            self.assertEqual(
+                len(rows),
+                0,
+                "cursor.fetchall should return an empty list if "
+                "a select query returns no rows",
+            )
+
+        finally:
+            con.close()
+
+    def test_fetchone(self):
+        con = self._connect()
+        try:
+            cur = con.cursor()
+
+            # cursor.fetchone should raise an Error if called before
+            # executing a select-type query
+            self.assertRaises(self.driver.Error, cur.fetchone)
+
+            # cursor.fetchone should raise an Error if called after
+            # executing a query that cannot return rows
+            self.executeDDL1(cur)
+            # self.assertRaises(self.driver.Error,cur.fetchone)
+
+            cur.execute("select name from %sbooze" % self.table_prefix)
+            self.assertEqual(
+                cur.fetchone(),
+                None,
+                "cursor.fetchone should return None if a query retrieves " "no rows",
+            )
+            self.assertTrue(cur.rowcount in (-1, 0))
+
+            # cursor.fetchone should raise an Error if called after
+            # executing a query that cannot return rows
+            cur.execute(
+                "insert into %sbooze values ('Victoria Bitter')" % (self.table_prefix)
+            )
+            # self.assertRaises(self.driver.Error,cur.fetchone)
+
+            cur.execute("select name from %sbooze" % self.table_prefix)
+            r = cur.fetchone()
+            self.assertEqual(
+                len(r), 1, "cursor.fetchone should have retrieved a single row"
+            )
+            self.assertEqual(
+                r[0], "Victoria Bitter", "cursor.fetchone retrieved incorrect data"
+            )
+            # self.assertEqual(
+            #    cur.fetchone(),
+            #    None,
+            #    "cursor.fetchone should return None if no more rows available",
+            # )
+            self.assertTrue(cur.rowcount in (-1, 1))
+        finally:
+            con.close()
+
+    # Same complaint as for fetchall and fetchone
+    def test_rowcount(self):
+        con = self._connect()
+        try:
+            cur = con.cursor()
+            self.executeDDL1(cur)
+            #             self.assertEqual(cur.rowcount,-1,
+            #                 'cursor.rowcount should be -1 after executing no-result '
+            #                 'statements'
+            #                 )
+            cur.execute(
+                "insert into %sbooze values ('Victoria Bitter')" % (self.table_prefix)
+            )
+            #             self.assertTrue(cur.rowcount in (-1,1),
+            #                 'cursor.rowcount should == number or rows inserted, or '
+            #                 'set to -1 after executing an insert statement'
+            #                 )
+            cur.execute("select name from %sbooze" % self.table_prefix)
+            self.assertTrue(
+                cur.rowcount in (-1, 1),
+                "cursor.rowcount should == number of rows returned, or "
+                "set to -1 after executing a select statement",
+            )
+            self.executeDDL2(cur)
+        #             self.assertEqual(cur.rowcount,-1,
+        #                 'cursor.rowcount not being reset to -1 after executing '
+        #                 'no-result statements'
+        #                 )
+        finally:
+            con.close()
+
+    def test_callproc(self):
+        pass  # performed in test_MySQL_capabilities
+
+    def help_nextset_setUp(self, cur):
+        """
+        Should create a procedure called deleteme
+        that returns two result sets, first the
+        number of rows in booze then "name from booze"
+        """
+        sql = """
+           create procedure deleteme()
+           begin
+               select count(*) from %(tp)sbooze;
+               select name from %(tp)sbooze;
+           end
+        """ % dict(
+            tp=self.table_prefix
+        )
+        cur.execute(sql)
+
+    def help_nextset_tearDown(self, cur):
+        "If cleaning up is needed after nextSetTest"
+        cur.execute("drop procedure deleteme")
+
+    def test_nextset(self):
+        # from warnings import warn
+
+        con = self._connect()
+        try:
+            cur = con.cursor()
+            if not hasattr(cur, "nextset"):
+                return
+
+            try:
+                self.executeDDL1(cur)
+                sql = self._populate()
+                for sql in self._populate():
+                    cur.execute(sql)
+
+                self.help_nextset_setUp(cur)
+
+                cur.callproc("deleteme")
+                numberofrows = cur.fetchone()
+                assert numberofrows[0] == len(self.samples)
+                assert cur.nextset()
+                names = cur.fetchall()
+                assert len(names) == len(self.samples)
+                s = cur.nextset()
+                if s:
+                    empty = cur.fetchall()
+                    self.assertEqual(
+                        len(empty), 0, "non-empty result set after other result sets"
+                    )
+                    # warn(
+                    #    ": ".join(
+                    #        [
+                    #            "Incompatibility",
+                    #            "MySQL returns an empty result set for the CALL itself"
+                    #        ]
+                    #    ),
+                    #    Warning,
+                    # )
+                # assert s == None, "No more return sets, should return None"
+            finally:
+                self.help_nextset_tearDown(cur)
+
+        finally:
+            con.close()
+
+
+if __name__ == "__main__":
+    unittest.main()
```

### Comparing `mysqlclient-2.2.0/tests/test_MySQLdb_times.py` & `mysqlclient-2.2.0rc1/tests/test_MySQLdb_times.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,146 +1,146 @@
-from datetime import time, date, datetime, timedelta
-from time import gmtime
-import unittest
-from unittest import mock
-import warnings
-
-from MySQLdb import times
-
-
-warnings.simplefilter("ignore")
-
-
-class TestX_or_None(unittest.TestCase):
-    def test_date_or_none(self):
-        assert times.Date_or_None("1969-01-01") == date(1969, 1, 1)
-        assert times.Date_or_None("2015-01-01") == date(2015, 1, 1)
-        assert times.Date_or_None("2015-12-13") == date(2015, 12, 13)
-
-        assert times.Date_or_None("") is None
-        assert times.Date_or_None("fail") is None
-        assert times.Date_or_None("2015-12") is None
-        assert times.Date_or_None("2015-12-40") is None
-        assert times.Date_or_None("0000-00-00") is None
-
-    def test_time_or_none(self):
-        assert times.Time_or_None("00:00:00") == time(0, 0)
-        assert times.Time_or_None("01:02:03") == time(1, 2, 3)
-        assert times.Time_or_None("01:02:03.123456") == time(1, 2, 3, 123456)
-
-        assert times.Time_or_None("") is None
-        assert times.Time_or_None("fail") is None
-        assert times.Time_or_None("24:00:00") is None
-        assert times.Time_or_None("01:02:03.123456789") is None
-
-    def test_datetime_or_none(self):
-        assert times.DateTime_or_None("1000-01-01") == date(1000, 1, 1)
-        assert times.DateTime_or_None("2015-12-13") == date(2015, 12, 13)
-        assert times.DateTime_or_None("2015-12-13 01:02") == datetime(
-            2015, 12, 13, 1, 2
-        )
-        assert times.DateTime_or_None("2015-12-13T01:02") == datetime(
-            2015, 12, 13, 1, 2
-        )
-        assert times.DateTime_or_None("2015-12-13 01:02:03") == datetime(
-            2015, 12, 13, 1, 2, 3
-        )
-        assert times.DateTime_or_None("2015-12-13T01:02:03") == datetime(
-            2015, 12, 13, 1, 2, 3
-        )
-        assert times.DateTime_or_None("2015-12-13 01:02:03.123") == datetime(
-            2015, 12, 13, 1, 2, 3, 123000
-        )
-        assert times.DateTime_or_None("2015-12-13 01:02:03.000123") == datetime(
-            2015, 12, 13, 1, 2, 3, 123
-        )
-        assert times.DateTime_or_None("2015-12-13 01:02:03.123456") == datetime(
-            2015, 12, 13, 1, 2, 3, 123456
-        )
-        assert times.DateTime_or_None("2015-12-13T01:02:03.123456") == datetime(
-            2015, 12, 13, 1, 2, 3, 123456
-        )
-
-        assert times.DateTime_or_None("") is None
-        assert times.DateTime_or_None("fail") is None
-        assert times.DateTime_or_None("0000-00-00 00:00:00") is None
-        assert times.DateTime_or_None("0000-00-00 00:00:00.000000") is None
-        assert times.DateTime_or_None("2015-12-13T01:02:03.123456789") is None
-
-    def test_timedelta_or_none(self):
-        assert times.TimeDelta_or_None("-1:0:0") == timedelta(0, -3600)
-        assert times.TimeDelta_or_None("1:0:0") == timedelta(0, 3600)
-        assert times.TimeDelta_or_None("12:55:30") == timedelta(0, 46530)
-        assert times.TimeDelta_or_None("12:55:30.123456") == timedelta(0, 46530, 123456)
-        assert times.TimeDelta_or_None("12:55:30.123456789") == timedelta(
-            0, 46653, 456789
-        )
-        assert times.TimeDelta_or_None("12:55:30.123456789123456") == timedelta(
-            1429, 37719, 123456
-        )
-
-        assert times.TimeDelta_or_None("") is None
-        assert times.TimeDelta_or_None("0") is None
-        assert times.TimeDelta_or_None("fail") is None
-
-
-class TestTicks(unittest.TestCase):
-    @mock.patch("MySQLdb.times.localtime", side_effect=gmtime)
-    def test_date_from_ticks(self, mock):
-        assert times.DateFromTicks(0) == date(1970, 1, 1)
-        assert times.DateFromTicks(1430000000) == date(2015, 4, 25)
-
-    @mock.patch("MySQLdb.times.localtime", side_effect=gmtime)
-    def test_time_from_ticks(self, mock):
-        assert times.TimeFromTicks(0) == time(0, 0, 0)
-        assert times.TimeFromTicks(1431100000) == time(15, 46, 40)
-        assert times.TimeFromTicks(1431100000.123) == time(15, 46, 40)
-
-    @mock.patch("MySQLdb.times.localtime", side_effect=gmtime)
-    def test_timestamp_from_ticks(self, mock):
-        assert times.TimestampFromTicks(0) == datetime(1970, 1, 1, 0, 0, 0)
-        assert times.TimestampFromTicks(1430000000) == datetime(2015, 4, 25, 22, 13, 20)
-        assert times.TimestampFromTicks(1430000000.123) == datetime(
-            2015, 4, 25, 22, 13, 20
-        )
-
-
-class TestToLiteral(unittest.TestCase):
-    def test_datetime_to_literal(self):
-        self.assertEqual(
-            times.DateTime2literal(datetime(2015, 12, 13), ""), b"'2015-12-13 00:00:00'"
-        )
-        self.assertEqual(
-            times.DateTime2literal(datetime(2015, 12, 13, 11, 12, 13), ""),
-            b"'2015-12-13 11:12:13'",
-        )
-        self.assertEqual(
-            times.DateTime2literal(datetime(2015, 12, 13, 11, 12, 13, 123456), ""),
-            b"'2015-12-13 11:12:13.123456'",
-        )
-
-    def test_datetimedelta_to_literal(self):
-        d = datetime(2015, 12, 13, 1, 2, 3) - datetime(2015, 12, 13, 1, 2, 2)
-        assert times.DateTimeDelta2literal(d, "") == b"'0 0:0:1'"
-
-
-class TestFormat(unittest.TestCase):
-    def test_format_timedelta(self):
-        d = datetime(2015, 1, 1) - datetime(2015, 1, 1)
-        assert times.format_TIMEDELTA(d) == "0 0:0:0"
-
-        d = datetime(2015, 1, 1, 10, 11, 12) - datetime(2015, 1, 1, 8, 9, 10)
-        assert times.format_TIMEDELTA(d) == "0 2:2:2"
-
-        d = datetime(2015, 1, 1, 10, 11, 12) - datetime(2015, 1, 1, 11, 12, 13)
-        assert times.format_TIMEDELTA(d) == "-1 22:58:59"
-
-    def test_format_timestamp(self):
-        assert times.format_TIMESTAMP(datetime(2015, 2, 3)) == "2015-02-03 00:00:00"
-        self.assertEqual(
-            times.format_TIMESTAMP(datetime(2015, 2, 3, 17, 18, 19)),
-            "2015-02-03 17:18:19",
-        )
-        self.assertEqual(
-            times.format_TIMESTAMP(datetime(15, 2, 3, 17, 18, 19)),
-            "0015-02-03 17:18:19",
-        )
+from datetime import time, date, datetime, timedelta
+from time import gmtime
+import unittest
+from unittest import mock
+import warnings
+
+from MySQLdb import times
+
+
+warnings.simplefilter("ignore")
+
+
+class TestX_or_None(unittest.TestCase):
+    def test_date_or_none(self):
+        assert times.Date_or_None("1969-01-01") == date(1969, 1, 1)
+        assert times.Date_or_None("2015-01-01") == date(2015, 1, 1)
+        assert times.Date_or_None("2015-12-13") == date(2015, 12, 13)
+
+        assert times.Date_or_None("") is None
+        assert times.Date_or_None("fail") is None
+        assert times.Date_or_None("2015-12") is None
+        assert times.Date_or_None("2015-12-40") is None
+        assert times.Date_or_None("0000-00-00") is None
+
+    def test_time_or_none(self):
+        assert times.Time_or_None("00:00:00") == time(0, 0)
+        assert times.Time_or_None("01:02:03") == time(1, 2, 3)
+        assert times.Time_or_None("01:02:03.123456") == time(1, 2, 3, 123456)
+
+        assert times.Time_or_None("") is None
+        assert times.Time_or_None("fail") is None
+        assert times.Time_or_None("24:00:00") is None
+        assert times.Time_or_None("01:02:03.123456789") is None
+
+    def test_datetime_or_none(self):
+        assert times.DateTime_or_None("1000-01-01") == date(1000, 1, 1)
+        assert times.DateTime_or_None("2015-12-13") == date(2015, 12, 13)
+        assert times.DateTime_or_None("2015-12-13 01:02") == datetime(
+            2015, 12, 13, 1, 2
+        )
+        assert times.DateTime_or_None("2015-12-13T01:02") == datetime(
+            2015, 12, 13, 1, 2
+        )
+        assert times.DateTime_or_None("2015-12-13 01:02:03") == datetime(
+            2015, 12, 13, 1, 2, 3
+        )
+        assert times.DateTime_or_None("2015-12-13T01:02:03") == datetime(
+            2015, 12, 13, 1, 2, 3
+        )
+        assert times.DateTime_or_None("2015-12-13 01:02:03.123") == datetime(
+            2015, 12, 13, 1, 2, 3, 123000
+        )
+        assert times.DateTime_or_None("2015-12-13 01:02:03.000123") == datetime(
+            2015, 12, 13, 1, 2, 3, 123
+        )
+        assert times.DateTime_or_None("2015-12-13 01:02:03.123456") == datetime(
+            2015, 12, 13, 1, 2, 3, 123456
+        )
+        assert times.DateTime_or_None("2015-12-13T01:02:03.123456") == datetime(
+            2015, 12, 13, 1, 2, 3, 123456
+        )
+
+        assert times.DateTime_or_None("") is None
+        assert times.DateTime_or_None("fail") is None
+        assert times.DateTime_or_None("0000-00-00 00:00:00") is None
+        assert times.DateTime_or_None("0000-00-00 00:00:00.000000") is None
+        assert times.DateTime_or_None("2015-12-13T01:02:03.123456789") is None
+
+    def test_timedelta_or_none(self):
+        assert times.TimeDelta_or_None("-1:0:0") == timedelta(0, -3600)
+        assert times.TimeDelta_or_None("1:0:0") == timedelta(0, 3600)
+        assert times.TimeDelta_or_None("12:55:30") == timedelta(0, 46530)
+        assert times.TimeDelta_or_None("12:55:30.123456") == timedelta(0, 46530, 123456)
+        assert times.TimeDelta_or_None("12:55:30.123456789") == timedelta(
+            0, 46653, 456789
+        )
+        assert times.TimeDelta_or_None("12:55:30.123456789123456") == timedelta(
+            1429, 37719, 123456
+        )
+
+        assert times.TimeDelta_or_None("") is None
+        assert times.TimeDelta_or_None("0") is None
+        assert times.TimeDelta_or_None("fail") is None
+
+
+class TestTicks(unittest.TestCase):
+    @mock.patch("MySQLdb.times.localtime", side_effect=gmtime)
+    def test_date_from_ticks(self, mock):
+        assert times.DateFromTicks(0) == date(1970, 1, 1)
+        assert times.DateFromTicks(1430000000) == date(2015, 4, 25)
+
+    @mock.patch("MySQLdb.times.localtime", side_effect=gmtime)
+    def test_time_from_ticks(self, mock):
+        assert times.TimeFromTicks(0) == time(0, 0, 0)
+        assert times.TimeFromTicks(1431100000) == time(15, 46, 40)
+        assert times.TimeFromTicks(1431100000.123) == time(15, 46, 40)
+
+    @mock.patch("MySQLdb.times.localtime", side_effect=gmtime)
+    def test_timestamp_from_ticks(self, mock):
+        assert times.TimestampFromTicks(0) == datetime(1970, 1, 1, 0, 0, 0)
+        assert times.TimestampFromTicks(1430000000) == datetime(2015, 4, 25, 22, 13, 20)
+        assert times.TimestampFromTicks(1430000000.123) == datetime(
+            2015, 4, 25, 22, 13, 20
+        )
+
+
+class TestToLiteral(unittest.TestCase):
+    def test_datetime_to_literal(self):
+        self.assertEqual(
+            times.DateTime2literal(datetime(2015, 12, 13), ""), b"'2015-12-13 00:00:00'"
+        )
+        self.assertEqual(
+            times.DateTime2literal(datetime(2015, 12, 13, 11, 12, 13), ""),
+            b"'2015-12-13 11:12:13'",
+        )
+        self.assertEqual(
+            times.DateTime2literal(datetime(2015, 12, 13, 11, 12, 13, 123456), ""),
+            b"'2015-12-13 11:12:13.123456'",
+        )
+
+    def test_datetimedelta_to_literal(self):
+        d = datetime(2015, 12, 13, 1, 2, 3) - datetime(2015, 12, 13, 1, 2, 2)
+        assert times.DateTimeDelta2literal(d, "") == b"'0 0:0:1'"
+
+
+class TestFormat(unittest.TestCase):
+    def test_format_timedelta(self):
+        d = datetime(2015, 1, 1) - datetime(2015, 1, 1)
+        assert times.format_TIMEDELTA(d) == "0 0:0:0"
+
+        d = datetime(2015, 1, 1, 10, 11, 12) - datetime(2015, 1, 1, 8, 9, 10)
+        assert times.format_TIMEDELTA(d) == "0 2:2:2"
+
+        d = datetime(2015, 1, 1, 10, 11, 12) - datetime(2015, 1, 1, 11, 12, 13)
+        assert times.format_TIMEDELTA(d) == "-1 22:58:59"
+
+    def test_format_timestamp(self):
+        assert times.format_TIMESTAMP(datetime(2015, 2, 3)) == "2015-02-03 00:00:00"
+        self.assertEqual(
+            times.format_TIMESTAMP(datetime(2015, 2, 3, 17, 18, 19)),
+            "2015-02-03 17:18:19",
+        )
+        self.assertEqual(
+            times.format_TIMESTAMP(datetime(15, 2, 3, 17, 18, 19)),
+            "0015-02-03 17:18:19",
+        )
```

### Comparing `mysqlclient-2.2.0/tests/test_connection.py` & `mysqlclient-2.2.0rc1/tests/test_connection.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-import pytest
-
-from MySQLdb._exceptions import ProgrammingError
-
-from configdb import connection_factory
-
-
-def test_multi_statements_default_true():
-    conn = connection_factory()
-    cursor = conn.cursor()
-
-    cursor.execute("select 17; select 2")
-    rows = cursor.fetchall()
-    assert rows == ((17,),)
-
-
-def test_multi_statements_false():
-    conn = connection_factory(multi_statements=False)
-    cursor = conn.cursor()
-
-    with pytest.raises(ProgrammingError):
-        cursor.execute("select 17; select 2")
-
-    cursor.execute("select 17")
-    rows = cursor.fetchall()
-    assert rows == ((17,),)
+import pytest
+
+from MySQLdb._exceptions import ProgrammingError
+
+from configdb import connection_factory
+
+
+def test_multi_statements_default_true():
+    conn = connection_factory()
+    cursor = conn.cursor()
+
+    cursor.execute("select 17; select 2")
+    rows = cursor.fetchall()
+    assert rows == ((17,),)
+
+
+def test_multi_statements_false():
+    conn = connection_factory(multi_statements=False)
+    cursor = conn.cursor()
+
+    with pytest.raises(ProgrammingError):
+        cursor.execute("select 17; select 2")
+
+    cursor.execute("select 17")
+    rows = cursor.fetchall()
+    assert rows == ((17,),)
```

### Comparing `mysqlclient-2.2.0/tests/test_cursor.py` & `mysqlclient-2.2.0rc1/tests/test_cursor.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,245 +1,245 @@
-import pytest
-import MySQLdb.cursors
-from configdb import connection_factory
-
-
-_conns = []
-_tables = []
-
-
-def connect(**kwargs):
-    conn = connection_factory(**kwargs)
-    _conns.append(conn)
-    return conn
-
-
-def teardown_function(function):
-    if _tables:
-        c = _conns[0]
-        cur = c.cursor()
-        for t in _tables:
-            cur.execute(f"DROP TABLE {t}")
-        cur.close()
-        del _tables[:]
-
-    for c in _conns:
-        c.close()
-    del _conns[:]
-
-
-def test_executemany():
-    conn = connect()
-    cursor = conn.cursor()
-
-    cursor.execute("create table test (data varchar(10))")
-    _tables.append("test")
-
-    m = MySQLdb.cursors.RE_INSERT_VALUES.match(
-        "INSERT INTO TEST (ID, NAME) VALUES (%s, %s)"
-    )
-    assert m is not None, "error parse %s"
-    assert m.group(3) == "", "group 3 not blank, bug in RE_INSERT_VALUES?"
-
-    m = MySQLdb.cursors.RE_INSERT_VALUES.match(
-        "INSERT INTO TEST (ID, NAME) VALUES (%(id)s, %(name)s)"
-    )
-    assert m is not None, "error parse %(name)s"
-    assert m.group(3) == "", "group 3 not blank, bug in RE_INSERT_VALUES?"
-
-    m = MySQLdb.cursors.RE_INSERT_VALUES.match(
-        "INSERT INTO TEST (ID, NAME) VALUES (%(id_name)s, %(name)s)"
-    )
-    assert m is not None, "error parse %(id_name)s"
-    assert m.group(3) == "", "group 3 not blank, bug in RE_INSERT_VALUES?"
-
-    m = MySQLdb.cursors.RE_INSERT_VALUES.match(
-        "INSERT INTO TEST (ID, NAME) VALUES (%(id_name)s, %(name)s) ON duplicate update"
-    )
-    assert m is not None, "error parse %(id_name)s"
-    assert (
-        m.group(3) == " ON duplicate update"
-    ), "group 3 not ON duplicate update, bug in RE_INSERT_VALUES?"
-
-    # https://github.com/PyMySQL/mysqlclient-python/issues/178
-    m = MySQLdb.cursors.RE_INSERT_VALUES.match(
-        "INSERT INTO bloup(foo, bar)VALUES(%s, %s)"
-    )
-    assert m is not None
-
-    # cursor._executed myst bee
-    # """
-    # insert into test (data)
-    # values (0),(1),(2),(3),(4),(5),(6),(7),(8),(9)
-    # """
-    # list args
-    data = [(i,) for i in range(10)]
-    cursor.executemany("insert into test (data) values (%s)", data)
-    assert cursor._executed.endswith(
-        b",(7),(8),(9)"
-    ), "execute many with %s not in one query"
-
-    # dict args
-    data_dict = [{"data": i} for i in range(10)]
-    cursor.executemany("insert into test (data) values (%(data)s)", data_dict)
-    assert cursor._executed.endswith(
-        b",(7),(8),(9)"
-    ), "execute many with %(data)s not in one query"
-
-    # %% in column set
-    cursor.execute(
-        """\
-        CREATE TABLE percent_test (
-            `A%` INTEGER,
-            `B%` INTEGER)"""
-    )
-    try:
-        q = "INSERT INTO percent_test (`A%%`, `B%%`) VALUES (%s, %s)"
-        assert MySQLdb.cursors.RE_INSERT_VALUES.match(q) is not None
-        cursor.executemany(q, [(3, 4), (5, 6)])
-        assert cursor._executed.endswith(
-            b"(3, 4),(5, 6)"
-        ), "executemany with %% not in one query"
-    finally:
-        cursor.execute("DROP TABLE IF EXISTS percent_test")
-
-
-def test_pyparam():
-    conn = connect()
-    cursor = conn.cursor()
-
-    cursor.execute("SELECT %(a)s, %(b)s", {"a": 1, "b": 2})
-    assert cursor._executed == b"SELECT 1, 2"
-    cursor.execute(b"SELECT %(a)s, %(b)s", {b"a": 3, b"b": 4})
-    assert cursor._executed == b"SELECT 3, 4"
-
-
-def test_dictcursor():
-    conn = connect()
-    cursor = conn.cursor(MySQLdb.cursors.DictCursor)
-
-    cursor.execute("CREATE TABLE t1 (a int, b int, c int)")
-    _tables.append("t1")
-    cursor.execute("INSERT INTO t1 (a,b,c) VALUES (1,1,47), (2,2,47)")
-
-    cursor.execute("CREATE TABLE t2 (b int, c int)")
-    _tables.append("t2")
-    cursor.execute("INSERT INTO t2 (b,c) VALUES (1,1), (2,2)")
-
-    cursor.execute("SELECT * FROM t1 JOIN t2 ON t1.b=t2.b")
-    rows = cursor.fetchall()
-
-    assert len(rows) == 2
-    assert rows[0] == {"a": 1, "b": 1, "c": 47, "t2.b": 1, "t2.c": 1}
-    assert rows[1] == {"a": 2, "b": 2, "c": 47, "t2.b": 2, "t2.c": 2}
-
-    names1 = sorted(rows[0])
-    names2 = sorted(rows[1])
-    for a, b in zip(names1, names2):
-        assert a is b
-
-    # Old fetchtype
-    cursor._fetch_type = 2
-    cursor.execute("SELECT * FROM t1 JOIN t2 ON t1.b=t2.b")
-    rows = cursor.fetchall()
-
-    assert len(rows) == 2
-    assert rows[0] == {"t1.a": 1, "t1.b": 1, "t1.c": 47, "t2.b": 1, "t2.c": 1}
-    assert rows[1] == {"t1.a": 2, "t1.b": 2, "t1.c": 47, "t2.b": 2, "t2.c": 2}
-
-    names1 = sorted(rows[0])
-    names2 = sorted(rows[1])
-    for a, b in zip(names1, names2):
-        assert a is b
-
-
-def test_mogrify_without_args():
-    conn = connect()
-    cursor = conn.cursor()
-
-    query = "SELECT VERSION()"
-    mogrified_query = cursor.mogrify(query)
-    cursor.execute(query)
-
-    assert mogrified_query == query
-    assert mogrified_query == cursor._executed.decode()
-
-
-def test_mogrify_with_tuple_args():
-    conn = connect()
-    cursor = conn.cursor()
-
-    query_with_args = "SELECT %s, %s", (1, 2)
-    mogrified_query = cursor.mogrify(*query_with_args)
-    cursor.execute(*query_with_args)
-
-    assert mogrified_query == "SELECT 1, 2"
-    assert mogrified_query == cursor._executed.decode()
-
-
-def test_mogrify_with_dict_args():
-    conn = connect()
-    cursor = conn.cursor()
-
-    query_with_args = "SELECT %(a)s, %(b)s", {"a": 1, "b": 2}
-    mogrified_query = cursor.mogrify(*query_with_args)
-    cursor.execute(*query_with_args)
-
-    assert mogrified_query == "SELECT 1, 2"
-    assert mogrified_query == cursor._executed.decode()
-
-
-# Test that cursor can be used without reading whole resultset.
-@pytest.mark.parametrize("Cursor", [MySQLdb.cursors.Cursor, MySQLdb.cursors.SSCursor])
-def test_cursor_discard_result(Cursor):
-    conn = connect()
-    cursor = conn.cursor(Cursor)
-
-    cursor.execute(
-        """\
-CREATE TABLE test_cursor_discard_result (
-    id INTEGER PRIMARY KEY AUTO_INCREMENT,
-    data VARCHAR(100)
-)"""
-    )
-    _tables.append("test_cursor_discard_result")
-
-    cursor.executemany(
-        "INSERT INTO test_cursor_discard_result (id, data) VALUES (%s, %s)",
-        [(i, f"row {i}") for i in range(1, 101)],
-    )
-
-    cursor.execute(
-        """\
-SELECT * FROM test_cursor_discard_result WHERE id <= 10;
-SELECT * FROM test_cursor_discard_result WHERE id BETWEEN 11 AND 20;
-SELECT * FROM test_cursor_discard_result WHERE id BETWEEN 21 AND 30;
-"""
-    )
-    cursor.nextset()
-    assert cursor.fetchone() == (11, "row 11")
-
-    cursor.execute(
-        "SELECT * FROM test_cursor_discard_result WHERE id BETWEEN 31 AND 40"
-    )
-    assert cursor.fetchone() == (31, "row 31")
-
-
-def test_binary_prefix():
-    # https://github.com/PyMySQL/mysqlclient/issues/494
-    conn = connect(binary_prefix=True)
-    cursor = conn.cursor()
-
-    cursor.execute("DROP TABLE IF EXISTS test_binary_prefix")
-    cursor.execute(
-        """\
-CREATE TABLE test_binary_prefix (
-	id INTEGER NOT NULL AUTO_INCREMENT,
-	json JSON NOT NULL,
-	PRIMARY KEY (id)
-) CHARSET=utf8mb4"""
-    )
-
-    cursor.executemany(
-        "INSERT INTO test_binary_prefix (id, json) VALUES (%(id)s, %(json)s)",
-        ({"id": 1, "json": "{}"}, {"id": 2, "json": "{}"}),
-    )
+import pytest
+import MySQLdb.cursors
+from configdb import connection_factory
+
+
+_conns = []
+_tables = []
+
+
+def connect(**kwargs):
+    conn = connection_factory(**kwargs)
+    _conns.append(conn)
+    return conn
+
+
+def teardown_function(function):
+    if _tables:
+        c = _conns[0]
+        cur = c.cursor()
+        for t in _tables:
+            cur.execute(f"DROP TABLE {t}")
+        cur.close()
+        del _tables[:]
+
+    for c in _conns:
+        c.close()
+    del _conns[:]
+
+
+def test_executemany():
+    conn = connect()
+    cursor = conn.cursor()
+
+    cursor.execute("create table test (data varchar(10))")
+    _tables.append("test")
+
+    m = MySQLdb.cursors.RE_INSERT_VALUES.match(
+        "INSERT INTO TEST (ID, NAME) VALUES (%s, %s)"
+    )
+    assert m is not None, "error parse %s"
+    assert m.group(3) == "", "group 3 not blank, bug in RE_INSERT_VALUES?"
+
+    m = MySQLdb.cursors.RE_INSERT_VALUES.match(
+        "INSERT INTO TEST (ID, NAME) VALUES (%(id)s, %(name)s)"
+    )
+    assert m is not None, "error parse %(name)s"
+    assert m.group(3) == "", "group 3 not blank, bug in RE_INSERT_VALUES?"
+
+    m = MySQLdb.cursors.RE_INSERT_VALUES.match(
+        "INSERT INTO TEST (ID, NAME) VALUES (%(id_name)s, %(name)s)"
+    )
+    assert m is not None, "error parse %(id_name)s"
+    assert m.group(3) == "", "group 3 not blank, bug in RE_INSERT_VALUES?"
+
+    m = MySQLdb.cursors.RE_INSERT_VALUES.match(
+        "INSERT INTO TEST (ID, NAME) VALUES (%(id_name)s, %(name)s) ON duplicate update"
+    )
+    assert m is not None, "error parse %(id_name)s"
+    assert (
+        m.group(3) == " ON duplicate update"
+    ), "group 3 not ON duplicate update, bug in RE_INSERT_VALUES?"
+
+    # https://github.com/PyMySQL/mysqlclient-python/issues/178
+    m = MySQLdb.cursors.RE_INSERT_VALUES.match(
+        "INSERT INTO bloup(foo, bar)VALUES(%s, %s)"
+    )
+    assert m is not None
+
+    # cursor._executed myst bee
+    # """
+    # insert into test (data)
+    # values (0),(1),(2),(3),(4),(5),(6),(7),(8),(9)
+    # """
+    # list args
+    data = [(i,) for i in range(10)]
+    cursor.executemany("insert into test (data) values (%s)", data)
+    assert cursor._executed.endswith(
+        b",(7),(8),(9)"
+    ), "execute many with %s not in one query"
+
+    # dict args
+    data_dict = [{"data": i} for i in range(10)]
+    cursor.executemany("insert into test (data) values (%(data)s)", data_dict)
+    assert cursor._executed.endswith(
+        b",(7),(8),(9)"
+    ), "execute many with %(data)s not in one query"
+
+    # %% in column set
+    cursor.execute(
+        """\
+        CREATE TABLE percent_test (
+            `A%` INTEGER,
+            `B%` INTEGER)"""
+    )
+    try:
+        q = "INSERT INTO percent_test (`A%%`, `B%%`) VALUES (%s, %s)"
+        assert MySQLdb.cursors.RE_INSERT_VALUES.match(q) is not None
+        cursor.executemany(q, [(3, 4), (5, 6)])
+        assert cursor._executed.endswith(
+            b"(3, 4),(5, 6)"
+        ), "executemany with %% not in one query"
+    finally:
+        cursor.execute("DROP TABLE IF EXISTS percent_test")
+
+
+def test_pyparam():
+    conn = connect()
+    cursor = conn.cursor()
+
+    cursor.execute("SELECT %(a)s, %(b)s", {"a": 1, "b": 2})
+    assert cursor._executed == b"SELECT 1, 2"
+    cursor.execute(b"SELECT %(a)s, %(b)s", {b"a": 3, b"b": 4})
+    assert cursor._executed == b"SELECT 3, 4"
+
+
+def test_dictcursor():
+    conn = connect()
+    cursor = conn.cursor(MySQLdb.cursors.DictCursor)
+
+    cursor.execute("CREATE TABLE t1 (a int, b int, c int)")
+    _tables.append("t1")
+    cursor.execute("INSERT INTO t1 (a,b,c) VALUES (1,1,47), (2,2,47)")
+
+    cursor.execute("CREATE TABLE t2 (b int, c int)")
+    _tables.append("t2")
+    cursor.execute("INSERT INTO t2 (b,c) VALUES (1,1), (2,2)")
+
+    cursor.execute("SELECT * FROM t1 JOIN t2 ON t1.b=t2.b")
+    rows = cursor.fetchall()
+
+    assert len(rows) == 2
+    assert rows[0] == {"a": 1, "b": 1, "c": 47, "t2.b": 1, "t2.c": 1}
+    assert rows[1] == {"a": 2, "b": 2, "c": 47, "t2.b": 2, "t2.c": 2}
+
+    names1 = sorted(rows[0])
+    names2 = sorted(rows[1])
+    for a, b in zip(names1, names2):
+        assert a is b
+
+    # Old fetchtype
+    cursor._fetch_type = 2
+    cursor.execute("SELECT * FROM t1 JOIN t2 ON t1.b=t2.b")
+    rows = cursor.fetchall()
+
+    assert len(rows) == 2
+    assert rows[0] == {"t1.a": 1, "t1.b": 1, "t1.c": 47, "t2.b": 1, "t2.c": 1}
+    assert rows[1] == {"t1.a": 2, "t1.b": 2, "t1.c": 47, "t2.b": 2, "t2.c": 2}
+
+    names1 = sorted(rows[0])
+    names2 = sorted(rows[1])
+    for a, b in zip(names1, names2):
+        assert a is b
+
+
+def test_mogrify_without_args():
+    conn = connect()
+    cursor = conn.cursor()
+
+    query = "SELECT VERSION()"
+    mogrified_query = cursor.mogrify(query)
+    cursor.execute(query)
+
+    assert mogrified_query == query
+    assert mogrified_query == cursor._executed.decode()
+
+
+def test_mogrify_with_tuple_args():
+    conn = connect()
+    cursor = conn.cursor()
+
+    query_with_args = "SELECT %s, %s", (1, 2)
+    mogrified_query = cursor.mogrify(*query_with_args)
+    cursor.execute(*query_with_args)
+
+    assert mogrified_query == "SELECT 1, 2"
+    assert mogrified_query == cursor._executed.decode()
+
+
+def test_mogrify_with_dict_args():
+    conn = connect()
+    cursor = conn.cursor()
+
+    query_with_args = "SELECT %(a)s, %(b)s", {"a": 1, "b": 2}
+    mogrified_query = cursor.mogrify(*query_with_args)
+    cursor.execute(*query_with_args)
+
+    assert mogrified_query == "SELECT 1, 2"
+    assert mogrified_query == cursor._executed.decode()
+
+
+# Test that cursor can be used without reading whole resultset.
+@pytest.mark.parametrize("Cursor", [MySQLdb.cursors.Cursor, MySQLdb.cursors.SSCursor])
+def test_cursor_discard_result(Cursor):
+    conn = connect()
+    cursor = conn.cursor(Cursor)
+
+    cursor.execute(
+        """\
+CREATE TABLE test_cursor_discard_result (
+    id INTEGER PRIMARY KEY AUTO_INCREMENT,
+    data VARCHAR(100)
+)"""
+    )
+    _tables.append("test_cursor_discard_result")
+
+    cursor.executemany(
+        "INSERT INTO test_cursor_discard_result (id, data) VALUES (%s, %s)",
+        [(i, f"row {i}") for i in range(1, 101)],
+    )
+
+    cursor.execute(
+        """\
+SELECT * FROM test_cursor_discard_result WHERE id <= 10;
+SELECT * FROM test_cursor_discard_result WHERE id BETWEEN 11 AND 20;
+SELECT * FROM test_cursor_discard_result WHERE id BETWEEN 21 AND 30;
+"""
+    )
+    cursor.nextset()
+    assert cursor.fetchone() == (11, "row 11")
+
+    cursor.execute(
+        "SELECT * FROM test_cursor_discard_result WHERE id BETWEEN 31 AND 40"
+    )
+    assert cursor.fetchone() == (31, "row 31")
+
+
+def test_binary_prefix():
+    # https://github.com/PyMySQL/mysqlclient/issues/494
+    conn = connect(binary_prefix=True)
+    cursor = conn.cursor()
+
+    cursor.execute("DROP TABLE IF EXISTS test_binary_prefix")
+    cursor.execute(
+        """\
+CREATE TABLE test_binary_prefix (
+	id INTEGER NOT NULL AUTO_INCREMENT,
+	json JSON NOT NULL,
+	PRIMARY KEY (id)
+) CHARSET=utf8mb4"""
+    )
+
+    cursor.executemany(
+        "INSERT INTO test_binary_prefix (id, json) VALUES (%(id)s, %(json)s)",
+        ({"id": 1, "json": "{}"}, {"id": 2, "json": "{}"}),
+    )
```

