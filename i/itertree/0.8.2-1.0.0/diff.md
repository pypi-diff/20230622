# Comparing `tmp/itertree-0.8.2.tar.gz` & `tmp/itertree-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "itertree-0.8.2.tar", last modified: Thu Jun  9 18:44:32 2022, max compression
+gzip compressed data, was "itertree-1.0.0.tar", last modified: Thu Jun 22 19:18:29 2023, max compression
```

## Comparing `itertree-0.8.2.tar` & `itertree-1.0.0.tar`

### file list

```diff
@@ -1,34 +1,50 @@
-drwxrwxrwx   0        0        0        0 2022-06-09 18:44:32.864080 itertree-0.8.2/
--rw-rw-rw-   0        0        0     1091 2021-03-31 14:10:05.000000 itertree-0.8.2/LICENSE
--rw-rw-rw-   0        0        0    12031 2022-06-09 18:44:32.864080 itertree-0.8.2/PKG-INFO
--rw-rw-rw-   0        0        0      108 2021-03-31 14:04:49.000000 itertree-0.8.2/pyproject.toml
--rw-rw-rw-   0        0        0      733 2022-06-09 18:44:32.865078 itertree-0.8.2/setup.cfg
--rw-rw-rw-   0        0        0      404 2022-06-09 18:44:11.000000 itertree-0.8.2/setup.py
-drwxrwxrwx   0        0        0        0 2022-06-09 18:44:32.826693 itertree-0.8.2/src/
-drwxrwxrwx   0        0        0        0 2022-06-09 18:44:32.841141 itertree-0.8.2/src/itertree/
--rw-rw-rw-   0        0        0     2201 2022-06-06 20:50:29.000000 itertree-0.8.2/src/itertree/__init__.py
-drwxrwxrwx   0        0        0        0 2022-06-09 18:44:32.856101 itertree-0.8.2/src/itertree/examples/
--rw-rw-rw-   0        0        0        0 2021-03-15 06:47:19.000000 itertree-0.8.2/src/itertree/examples/__init__.py
--rw-rw-rw-   0        0        0    24612 2022-06-06 20:50:29.000000 itertree-0.8.2/src/itertree/examples/itree_data_models.py
-drwxrwxrwx   0        0        0        0 2022-06-09 18:44:32.863083 itertree-0.8.2/src/itertree/examples/itree_editor/
--rw-rw-rw-   0        0        0        0 2022-05-16 07:51:42.000000 itertree-0.8.2/src/itertree/examples/itree_editor/__init__.py
--rw-rw-rw-   0        0        0    46989 2022-06-06 20:50:29.000000 itertree-0.8.2/src/itertree/examples/itree_editor/controller.py
--rw-rw-rw-   0        0        0     9276 2022-06-06 20:52:11.000000 itertree-0.8.2/src/itertree/examples/itree_editor/data_models.py
--rw-rw-rw-   0        0        0    35734 2022-06-06 20:50:29.000000 itertree-0.8.2/src/itertree/examples/itree_editor/gui.py
--rw-rw-rw-   0        0        0     1955 2022-06-06 20:52:11.000000 itertree-0.8.2/src/itertree/examples/itree_editor/main.py
--rw-rw-rw-   0        0        0     3933 2022-06-06 20:50:29.000000 itertree-0.8.2/src/itertree/examples/itree_link_example1.py
--rw-rw-rw-   0        0        0    22446 2022-06-06 20:50:29.000000 itertree-0.8.2/src/itertree/examples/itree_performance.py
--rw-rw-rw-   0        0        0    16444 2022-06-06 20:50:29.000000 itertree-0.8.2/src/itertree/examples/itree_performance2.py
--rw-rw-rw-   0        0        0     2647 2022-06-06 20:50:29.000000 itertree-0.8.2/src/itertree/examples/itree_profile.py
--rw-rw-rw-   0        0        0     3975 2022-06-06 20:50:29.000000 itertree-0.8.2/src/itertree/examples/itree_profile2.py
--rw-rw-rw-   0        0        0     8242 2022-06-06 21:14:33.000000 itertree-0.8.2/src/itertree/examples/itree_usage_example1.py
--rw-rw-rw-   0        0        0    23502 2022-06-07 18:56:34.000000 itertree-0.8.2/src/itertree/itree_data.py
--rw-rw-rw-   0        0        0    19224 2022-06-06 20:50:29.000000 itertree-0.8.2/src/itertree/itree_filter.py
--rw-rw-rw-   0        0        0    30959 2022-06-06 20:50:29.000000 itertree-0.8.2/src/itertree/itree_helpers.py
--rw-rw-rw-   0        0        0   121731 2022-06-06 20:50:29.000000 itertree-0.8.2/src/itertree/itree_main.py
--rw-rw-rw-   0        0        0    23304 2022-06-07 17:04:57.000000 itertree-0.8.2/src/itertree/itree_serialize.py
-drwxrwxrwx   0        0        0        0 2022-06-09 18:44:32.845131 itertree-0.8.2/src/itertree.egg-info/
--rw-rw-rw-   0        0        0    12031 2022-06-09 18:44:32.000000 itertree-0.8.2/src/itertree.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      920 2022-06-09 18:44:32.000000 itertree-0.8.2/src/itertree.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-06-09 18:44:32.000000 itertree-0.8.2/src/itertree.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2022-06-09 18:44:32.000000 itertree-0.8.2/src/itertree.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-22 19:18:29.249858 itertree-1.0.0/
+-rw-rw-rw-   0        0        0     1091 2021-03-31 14:10:05.000000 itertree-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0    17135 2023-06-22 19:18:29.249858 itertree-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0    16523 2023-06-15 20:25:43.000000 itertree-1.0.0/README.md
+-rw-rw-rw-   0        0        0      108 2021-03-31 14:04:49.000000 itertree-1.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0      733 2023-06-22 19:18:29.265485 itertree-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      371 2023-06-12 09:57:53.000000 itertree-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-22 19:18:29.187362 itertree-1.0.0/src/
+drwxrwxrwx   0        0        0        0 2023-06-22 19:18:29.202988 itertree-1.0.0/src/itertree/
+-rw-rw-rw-   0        0        0     2452 2023-05-27 19:27:59.000000 itertree-1.0.0/src/itertree/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-22 19:18:29.218611 itertree-1.0.0/src/itertree/examples/
+-rw-rw-rw-   0        0        0        0 2021-03-15 06:47:19.000000 itertree-1.0.0/src/itertree/examples/__init__.py
+-rw-rw-rw-   0        0        0    19734 2023-05-30 05:28:38.000000 itertree-1.0.0/src/itertree/examples/calendar_example.py
+-rw-rw-rw-   0        0        0     9669 2023-04-23 18:45:52.000000 itertree-1.0.0/src/itertree/examples/itree_data_models.py
+-rw-rw-rw-   0        0        0    37511 2023-06-22 06:07:16.000000 itertree-1.0.0/src/itertree/examples/itree_docu_examples.py
+drwxrwxrwx   0        0        0        0 2023-06-22 19:18:29.234235 itertree-1.0.0/src/itertree/examples/itree_editor/
+-rw-rw-rw-   0        0        0        0 2022-05-16 07:51:42.000000 itertree-1.0.0/src/itertree/examples/itree_editor/__init__.py
+-rw-rw-rw-   0        0        0    47292 2023-05-11 19:41:36.000000 itertree-1.0.0/src/itertree/examples/itree_editor/controller.py
+-rw-rw-rw-   0        0        0     1824 2023-02-04 15:18:42.000000 itertree-1.0.0/src/itertree/examples/itree_editor/data_models.py
+-rw-rw-rw-   0        0        0    36134 2023-05-11 18:57:11.000000 itertree-1.0.0/src/itertree/examples/itree_editor/gui.py
+-rw-rw-rw-   0        0        0     2193 2023-02-04 15:18:42.000000 itertree-1.0.0/src/itertree/examples/itree_editor/main.py
+-rw-rw-rw-   0        0        0     4376 2023-03-20 13:18:45.000000 itertree-1.0.0/src/itertree/examples/itree_link_example1.py
+-rw-rw-rw-   0        0        0     4643 2023-06-15 20:29:07.000000 itertree-1.0.0/src/itertree/examples/itree_usage_example1.py
+-rw-rw-rw-   0        0        0     5654 2023-06-15 20:27:56.000000 itertree-1.0.0/src/itertree/examples/itree_usage_example2.py
+-rw-rw-rw-   0        0        0    60955 2023-05-11 21:12:50.000000 itertree-1.0.0/src/itertree/examples/lldict4.py
+-rw-rw-rw-   0        0        0    58456 2023-06-21 11:29:14.000000 itertree-1.0.0/src/itertree/itree_data.py
+-rw-rw-rw-   0        0        0    23415 2023-04-15 10:59:11.000000 itertree-1.0.0/src/itertree/itree_filters.py
+-rw-rw-rw-   0        0        0    48086 2023-06-21 12:47:55.000000 itertree-1.0.0/src/itertree/itree_getitem.py
+-rw-rw-rw-   0        0        0    12135 2023-06-21 12:25:15.000000 itertree-1.0.0/src/itertree/itree_helpers.py
+-rw-rw-rw-   0        0        0    47842 2023-06-22 19:17:46.000000 itertree-1.0.0/src/itertree/itree_indepth.py
+-rw-rw-rw-   0        0        0   144996 2023-06-22 16:13:44.000000 itertree-1.0.0/src/itertree/itree_main.py
+-rw-rw-rw-   0        0        0    86824 2023-06-21 13:31:07.000000 itertree-1.0.0/src/itertree/itree_mathsets.py
+-rw-rw-rw-   0        0        0    37511 2023-06-19 20:09:54.000000 itertree-1.0.0/src/itertree/itree_private.py
+drwxrwxrwx   0        0        0        0 2023-06-22 19:18:29.218611 itertree-1.0.0/src/itertree.egg-info/
+-rw-rw-rw-   0        0        0    17135 2023-06-22 19:18:29.000000 itertree-1.0.0/src/itertree.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1375 2023-06-22 19:18:29.000000 itertree-1.0.0/src/itertree.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 19:18:29.000000 itertree-1.0.0/src/itertree.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-22 19:18:29.000000 itertree-1.0.0/src/itertree.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-22 19:18:29.249858 itertree-1.0.0/tests/
+-rw-rw-rw-   0        0        0    78641 2023-06-22 06:07:16.000000 itertree-1.0.0/tests/test_itertree_base1.py
+-rw-rw-rw-   0        0        0    30758 2023-05-30 05:28:36.000000 itertree-1.0.0/tests/test_itertree_base_old.py
+-rw-rw-rw-   0        0        0     4280 2023-06-12 06:06:03.000000 itertree-1.0.0/tests/test_itertree_examples.py
+-rw-rw-rw-   0        0        0    10082 2023-05-11 19:41:36.000000 itertree-1.0.0/tests/test_itertree_flags.py
+-rw-rw-rw-   0        0        0    16286 2023-05-30 05:28:36.000000 itertree-1.0.0/tests/test_itertree_full_feature_trees.py
+-rw-rw-rw-   0        0        0    19598 2023-02-20 15:28:39.000000 itertree-1.0.0/tests/test_itertree_intervals.py
+-rw-rw-rw-   0        0        0    59029 2023-06-22 17:29:00.000000 itertree-1.0.0/tests/test_itertree_iter.py
+-rw-rw-rw-   0        0        0    19488 2023-05-30 05:28:36.000000 itertree-1.0.0/tests/test_itertree_links.py
+-rw-rw-rw-   0        0        0    59933 2023-02-19 17:40:31.000000 itertree-1.0.0/tests/test_itertree_mathsets.py
+-rw-rw-rw-   0        0        0    10216 2023-06-12 06:13:24.000000 itertree-1.0.0/tests/test_itertree_serialize.py
+-rw-rw-rw-   0        0        0    19651 2023-03-01 21:50:32.000000 itertree-1.0.0/tests/test_itertree_value_models.py
```

### Comparing `itertree-0.8.2/LICENSE` & `itertree-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `itertree-0.8.2/setup.cfg` & `itertree-1.0.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2069 7465 7274 7265 652d 425f 520d   = itertree-B_R.
-00000020: 0a76 6572 7369 6f6e 203d 2030 2e38 2e31  .version = 0.8.1
+00000020: 0a76 6572 7369 6f6e 203d 2031 2e30 2e30  .version = 1.0.0
 00000030: 0d0a 6175 7468 6f72 203d 2042 2e52 2e0d  ..author = B.R..
 00000040: 0a61 7574 686f 725f 656d 6169 6c20 3d20  .author_email = 
 00000050: 6272 5f64 6576 656c 6f70 6d65 6e74 4070  br_development@p
 00000060: 6f73 7465 6f2e 6f72 670d 0a64 6573 6372  osteo.org..descr
 00000070: 6970 7469 6f6e 203d 2041 2070 6163 6b61  iption = A packa
 00000080: 6765 2066 6f72 2063 7265 6174 696e 6720  ge for creating 
 00000090: 7472 6565 2073 7472 7563 7475 7265 7320  tree structures 
@@ -34,13 +34,13 @@
 00000210: 7365 0d0a 094f 7065 7261 7469 6e67 2053  se...Operating S
 00000220: 7973 7465 6d20 3a3a 204f 5320 496e 6465  ystem :: OS Inde
 00000230: 7065 6e64 656e 740d 0a0d 0a5b 6f70 7469  pendent....[opti
 00000240: 6f6e 735d 0d0a 7061 636b 6167 655f 6469  ons]..package_di
 00000250: 7220 3d20 0d0a 093d 2073 7263 0d0a 7061  r = ...= src..pa
 00000260: 636b 6167 6573 203d 2066 696e 643a 0d0a  ckages = find:..
 00000270: 7079 7468 6f6e 5f72 6571 7569 7265 7320  python_requires 
-00000280: 3d20 3e3d 332e 300d 0a0d 0a5b 6f70 7469  = >=3.0....[opti
+00000280: 3d20 3e3d 332e 340d 0a0d 0a5b 6f70 7469  = >=3.4....[opti
 00000290: 6f6e 732e 7061 636b 6167 6573 2e66 696e  ons.packages.fin
 000002a0: 645d 0d0a 7768 6572 6520 3d20 7372 630d  d]..where = src.
 000002b0: 0a0d 0a5b 6567 675f 696e 666f 5d0d 0a74  ...[egg_info]..t
 000002c0: 6167 5f62 7569 6c64 203d 200d 0a74 6167  ag_build = ..tag
 000002d0: 5f64 6174 6520 3d20 300d 0a0d 0a         _date = 0....
```

### Comparing `itertree-0.8.2/src/itertree/__init__.py` & `itertree-1.0.0/src/itertree/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,24 +3,28 @@
 This code is taken from the itertree package:
 https://pypi.org/project/itertree/
 GIT Home:
 https://github.com/BR1py/itertree
 The documentation can be found here:
 https://itertree.readthedocs.io/en/latest/index.html
 
-The code is published under MIT license:
+The code is published under MIT license incl. human protect patch:
 
-The MIT License (MIT)
+The MIT License (MIT) incl. human protect patch
 Copyright © 2022 <copyright holders>
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 documentation files (the “Software”), to deal in the Software without restriction, including without limitation
 the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and
 to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
+Human protect patch:
+The program and its derivative work will neither be modified or executed to harm any human being nor through
+inaction permit any human being to be harmed.
+
 The above copyright notice and this permission notice shall be included in all copies or substantial
 portions of the Software.
 
 THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO
 THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS
 OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT
 OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
@@ -30,19 +34,20 @@
 
 This part of code contains the initialization and publishing of the iTree related classes of the itertree package.
 """
 
 from __future__ import absolute_import
 
 __package__ = 'itertree'
-__version__ = '0.8.0'
-__licence__ = 'MIT'
+__version__ = '1.0.0'
+__licence__ = 'MIT incl. human protect patch'
 __author__ = 'B.R.'
 __url__ = 'https://github.com/BR1py/itertree'
 __description__ = 'Python tree structure for data storage and iterations'
 
-from .itree_helpers import iTLink,iTMatch,TagIdx,TagIdxStr,TagMultiIdx,TagIdxBytes,iTInterval,TEMPORARY,READ_ONLY,LINKED,COPY_DEEP,COPY_OFF,COPY_NORMAL
-from .itree_main import iTree,iTreeLink,iTreeTemporary,iTreeReadOnly
+from .itree_helpers import iTLink, NoTag, NoKey, NoValue, Tag, iTFLAG, getter_to_list,INF,INF_PLUS,INF_MINUS,Any,TagIdx
+from .itree_main import iTree
 
 from . import itree_data as Data
-from . import itree_serialize as Serializer
-from . import itree_filter as Filter
+from . import itree_filters as Filters
+from .itree_serializer.itree_render_dot import _iTreeRenderDot
+iTreeRenderDot=_iTreeRenderDot().renders
```

### Comparing `itertree-0.8.2/src/itertree/examples/itree_editor/controller.py` & `itertree-1.0.0/src/itertree/examples/itree_editor/controller.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,34 +3,39 @@
 This code is taken from the itertree package:
 https://pypi.org/project/itertree/
 GIT Home:
 https://github.com/BR1py/itertree
 The documentation can be found here:
 https://itertree.readthedocs.io/en/latest/index.html
 
-The code is published under MIT license:
+The code is published under MIT license incl. human protect patch:
 
-The MIT License (MIT)
+The MIT License (MIT) incl. human protect patch
 Copyright © 2022 <copyright holders>
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 documentation files (the “Software”), to deal in the Software without restriction, including without limitation
 the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and
 to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
+Human protect patch:
+The program and its derivative work will neither be modified or executed to harm any human being nor through
+inaction permit any human being to be harmed.
+
 The above copyright notice and this permission notice shall be included in all copies or substantial
 portions of the Software.
 
 THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO
 THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS
 OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT
 OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 For more information see: https://en.wikipedia.org/wiki/MIT_License
 
+
 """
 from __future__ import absolute_import
 
 from threading import Lock
 from collections import deque,OrderedDict
 from ast import literal_eval
 import tempfile
@@ -98,71 +103,71 @@
             if detail.get('key'):
                 return self.DATA_KEY
             return self.DATA
         if detail.get('is_link'):
             if detail.get('key'):
                 return self.LINK_KEY
             return self.LINK
-        if isinstance(item,iTreeLink):
+        if item.is_link_root:
             return self.ITREELINK
-        if isinstance(item, iTreeReadOnly):
+        if item.is_tree_read_only:
             return self.ITREEREADONLY
         return self.ITREE
 
     def _create_data_popup(self,context_menu,item,detail,clp_data):
         if item.is_linked:
             if not item.link_root:
                 return context_menu
         if item.is_read_only:
             return context_menu
         # data dialog
-        data_item = iTree('item', data={'name': 'data manipulations:'})
+        data_item = iTree('item', value={'name': 'data manipulations:'})
         context_menu.append(data_item)
         context_menu.append(iTree('separator'))
-        data_item = iTree('item', data={'name': 'set data value',
+        data_item = iTree('item', value={'name': 'set data value',
                                         'tooltip': 'enter a data value directly (no model)',
                                         'action': 'set_data_value'})
         context_menu.append(data_item)
-        data_item = iTree('item', data={'name': 'add new data key',
+        data_item = iTree('item', value={'name': 'add new data key',
                                         'tooltip': 'add a data key where a value can be added afterwards',
                                         'action': 'add_empty_data_key'})
         context_menu.append(data_item)
-        data_item = iTree('item', data={'name': 'edit data model',
+        data_item = iTree('item', value={'name': 'edit data model',
                                         'tooltip': 'edit the specific data-model',
                                         'action': 'edit_data_model'})
         context_menu.append(data_item)
-        context_menu.d_set('data_key', NOKEY)
+        context_menu.set_key_value('data_key', NOKEY)
         return context_menu
 
 
     def _create_data_key_popup(self, context_menu, item, detail,clp_data):
         if item.is_linked:
             if not item.link_root:
                 return context_menu
         if item.is_read_only:
             return context_menu
         key = detail['text']
         try:
             key = literal_eval(key)
         except:
             pass
-        context_menu.d_set('data_key', key)
-        m_item = iTree('item', data={'name': 'data-key related data manipulations:'})
+        context_menu.set_key_value('data_key', key)
+        m_item = iTree('item', value={'name': 'data-key related data manipulations:'})
         context_menu.append(m_item)
         context_menu.append(iTree('separator'))
-        m_item = iTree('item', data={'name': 'set data value',
+        m_item = iTree('item', value={'name': 'set data value',
                                         'tooltip': 'enter a data value directly (no model)',
                                         'action': 'set_data_value'})
         context_menu.append(m_item)
-        m_item = iTree('item', data={'name': 'delete data key',
+        m_item = iTree('item', value={'name': 'delete data key',
                                      'tooltip': 'remove the key from the data structure',
                                      'action': 'remove_data_key'})
         context_menu.append(m_item)
 
-        m_item = iTree('item', data={'name': 'edit data model',
+        m_item = iTree('item', value={'name': 'edit data model',
                                         'tooltip': 'edit/define the specific data-model',
                                         'action': 'edit_data_model'})
         context_menu.append(m_item)
         return context_menu
 
     def _create_link_popup(self,context_menu,item,detail,clp_data):
         return context_menu
@@ -170,528 +175,528 @@
     def _create_link_key_popup(self, context_menu, item, detail, clp_data):
         if isinstance(item,iTreeLink) and item.is_link_root:
             key = detail['text']
             try:
                 key = literal_eval(key)
             except:
                 pass
-            context_menu.d_set('data_key', key)
-            m_item = iTree('item', data={'name': 'set link value',
+            context_menu.set_key_value('data_key', key)
+            m_item = iTree('item', value={'name': 'set link value',
                                          'action': 'set_link_value'})
             context_menu.append(m_item)
         return context_menu
 
 
     def _create_itree_popup(self, context_menu, item, detail,clp_data):
         if item.is_root:
-            title = iTree('item', data={'name': 'Tag: ' + item.tag})
+            title = iTree('item', value={'name': 'Tag: ' + item.tag})
         else:
-            name = ['TagIdx(%s,%i)' % (t[0], t[1]) for t in item.tag_idx_path]
-            title = iTree('item', data={'name': 'Tag-Idx-Path: ' + str(name)})
+            name = ['(%s,%i)' % (t[0], t[1]) for t in item.tag_idx_path]
+            title = iTree('item', value={'name': 'Key-Path: ' + str(name)})
         context_menu.append(title)
 
-        title.append(iTree('item', data={'name': 'Show item representations:'}))
+        title.append(iTree('item', value={'name': 'Show item representations:'}))
         title+=iTree('separator')
-        title.append(iTree('item', data={'name': 'Short repr() (no subtree)',
+        title.append(iTree('item', value={'name': 'Short repr() (no subtree)',
                                          'tooltip': 'print item repr in the log',
                                          'action': 'log_item_repr_short'}))
-        title.append(iTree('item', data={'name': 'Full repr() (with subtree)',
+        title.append(iTree('item', value={'name': 'Full repr() (with subtree)',
                                          'tooltip': 'print item repr in the log',
                                          'action': 'log_item_repr'}))
-        title.append(iTree('item', data={'name': 'Render Tree',
+        title.append(iTree('item', value={'name': 'Render Tree',
                                          'tooltip': 'Give the rendered item tree in the log',
                                          'action': 'log_item_render'}))
 
         context_menu.append(iTree('separator'))
-        item_edit=iTree('item', data={'name': 'edit item'})
+        item_edit=iTree('item', value={'name': 'edit item'})
         context_menu.append(item_edit)
-        item_edit.append(iTree('item', data={'name': 'edit item tag',
+        item_edit.append(iTree('item', value={'name': 'edit item tag',
                                                 'tooltip': 'change the tag of the item',
                                                 'key': 'Ctrl-t',
                                                 'action': 'edit_tag'}))
-        if item.data.is_empty:
-            item_edit.append(iTree('item', data={'name': 'set data value (no model)',
+        if item.value is NoValue:
+            item_edit.append(iTree('item', value={'name': 'set data value (no model)',
                                                 'tooltip': 'enter a data value directly (no model)',
                                                 'action': 'set_data_value'}))
-            item_edit.append(iTree('item', data={'name': 'add new data key',
+            item_edit.append(iTree('item', {'name': 'add new data key',
                                                 'tooltip': 'add a data key where a value can be added afterwards',
                                                 'action': 'add_empty_data_key'}))
-            item_edit.append(iTree('item', data={'name': 'edit data model',
+            item_edit.append(iTree('item', {'name': 'edit data model',
                                                 'tooltip': 'edit/define the specific data-model',
                                                 'action': 'edit_data_model'}))
-        new_menu=iTree('item', data={'name': 'Create new iTree'})
+        new_menu=iTree('item', {'name': 'Create new iTree'})
         if not item.is_root:
             new_menu.append(
-                iTree('item', data={'name': 'insert sibling before','action': 'insert_new_sibling_before'}))
+                iTree('item', {'name': 'insert sibling before','action': 'insert_new_sibling_before'}))
             new_menu.append(
-                iTree('item', data={'name': 'insert sibling after','action': 'insert_new_sibling_after'}))
+                iTree('item', {'name': 'insert sibling after','action': 'insert_new_sibling_after'}))
             new_menu.append(
-                iTree('item', data={'name': 'append sibling', 'action': 'append_new_sibling_after'}))
+                iTree('item', {'name': 'append sibling', 'action': 'append_new_sibling_after'}))
         new_menu.append(
-                iTree('item', data={'name': 'append child',
+                iTree('item', {'name': 'append child',
                                 'tooltip': 'append new child to selected item',
                                 'action': 'append_new_child'}))
         context_menu.append(new_menu)
 
-        new2_menu=iTree('item', data={'name': 'Create new iTreeLink'})
+        new2_menu=iTree('item', {'name': 'Create new iTreeLink'})
         if not item.is_root:
             new2_menu.append(
-                iTree('item', data={'name': 'insert sibling before','action': 'insert_new_link_sibling_before'}))
+                iTree('item', {'name': 'insert sibling before','action': 'insert_new_link_sibling_before'}))
             new2_menu.append(
-                iTree('item', data={'name': 'insert sibling after','action': 'insert_new_link_sibling_after'}))
+                iTree('item', {'name': 'insert sibling after','action': 'insert_new_link_sibling_after'}))
             new2_menu.append(
-                iTree('item', data={'name': 'append sibling', 'action': 'append_new_link_sibling_after'}))
+                iTree('item', {'name': 'append sibling', 'action': 'append_new_link_sibling_after'}))
         new2_menu.append(
-                iTree('item', data={'name': 'append child link',
+                iTree('item', {'name': 'append child link',
                                 'action': 'append_new_child_link'}))
         context_menu.append(new2_menu)
 
         if not item.is_root:
             context_menu.append(
-                iTree('item', data={'name': 'make item read-only',
+                iTree('item', {'name': 'make item read-only',
                                     'action': 'make_read_only_item'}))
 
             context_menu.append(
-                iTree('item', data={'name': 'delete selected item',
+                iTree('item', {'name': 'delete selected item',
                                     'tooltip': 'delete the selected item',
                                     'action': 'delete_item'}))
         context_menu.append(iTree('separator'))
         if not item.is_root:
             move_item = iTree('item',
-                              data={'name': 'Move selected item:'})
+                              {'name': 'Move selected item:'})
             set=False
             if item.idx != 0:
                 set=True
                 move_item.append(
                     iTree('item',
-                          data={'name': 'move up', 'action': 'move_up'}))
+                          {'name': 'move up', 'action': 'move_up'}))
             if item.idx < len(item.parent) - 1:
                 set = True
 
                 move_item.append(
                     iTree('item',
-                          data={'name': 'move down', 'action': 'move_down'}))
+                          {'name': 'move down', 'action': 'move_down'}))
             if item.idx != 0:
                 set = True
                 move_item.append(
                     iTree('item',
-                          data={'name': 'move inside first (make child)',
+                          {'name': 'move inside first (make child)',
                                 'action': 'move_inside_first'}))
             move_item.append(
                 iTree('item',
-                      data={'name': 'move inside last (make child)',
+                      value={'name': 'move inside last (make child)',
                             'action': 'move_inside_last'}))
             if not item.parent.is_root:
                 set=True
                 move_item.append(
                     iTree('item',
-                          data={'name': 'move outside (make parents sibling)',
+                          value={'name': 'move outside (make parents sibling)',
                                 'tooltip': 'move selected item inside previous item (append as child)'}))
             if set:
                 context_menu.append(move_item)
 
             context_menu.append(iTree('separator'))
         context_menu.append(
             iTree('item',
-                  data={'name': 'Cut item',
+                  value={'name': 'Cut item',
                         'action': 'cut_to_clp'}))
         context_menu.append(
             iTree('item',
-                  data={'name': 'Copy',
+                  value={'name': 'Copy',
                         'action': 'copy_to_clp'}))
         context_menu.append(
             iTree('item',
-                  data={'name': 'Copy item key-path',
+                  value={'name': 'Copy item key-path',
                         'action': 'copy_key_path_to_clp'}))
 
         if self._valid_clipboard_object(clp_data):
             context_menu.append(
                 iTree('item',
-                      data={'name': 'Paste',
+                      value={'name': 'Paste',
                             'action': 'paste_from_clp_after_item'}))
             context_menu.append(
                 iTree('item',
-                      data={'name': 'Paste inside',
+                      value={'name': 'Paste inside',
                             'action': 'paste_from_clp_inside_item'}))
 
         context_menu.append(iTree('separator'))
         v_menu=iTree('item',
-              data={'name': 'Tree visibility'})
+              value={'name': 'Tree visibility'})
         context_menu.append(v_menu)
         v_menu.append(
             iTree('item',
-                  data={'name': 'collapse item',
+                  value={'name': 'collapse item',
                         'action': 'collapse_item'}))
         v_menu.append(
             iTree('item',
-                  data={'name': 'expand item',
+                  value={'name': 'expand item',
                         'action': 'expand_item'}))
         v_menu.append(
             iTree('item',
-                  data={'name': 'collapse item and children',
+                  value={'name': 'collapse item and children',
                         'action': 'collapse_all_sub_items'}))
         v_menu.append(
             iTree('item',
-                  data={'name': 'expand item and children',
+                  value={'name': 'expand item and children',
                         'action': 'expand_all_sub_items'}))
         #context_menu.render()
-        context_menu.d_set('data_key', NOKEY)
+        context_menu.set_key_value('data_key', NOKEY)
         return context_menu
 
     def _create_itreereadonly_popup(self, context_menu, item, detail,clp_data):
         parent_read_only=item.parent.is_read_only
 
         name = ['TagIdx(%s,%i)' % (t[0], t[1]) for t in item.tag_idx_path]
-        title = iTree('item', data={'name': 'Tag-Idx-Path: ' + str(name)})
+        title = iTree('item', value={'name': 'Tag-Idx-Path: ' + str(name)})
         context_menu.append(title)
 
-        title.append(iTree('item', data={'name': 'Show item representations:'}))
+        title.append(iTree('item', value={'name': 'Show item representations:'}))
         title.append(iTree('separator'))
-        title.append(iTree('item', data={'name': 'Short repr() (no subtree)',
+        title.append(iTree('item', value={'name': 'Short repr() (no subtree)',
                                          'tooltip': 'print item repr in the log',
                                          'action': 'log_item_repr_short'}))
-        title.append(iTree('item', data={'name': 'Full repr() (with subtree)',
+        title.append(iTree('item', value={'name': 'Full repr() (with subtree)',
                                          'tooltip': 'print item repr in the log',
                                          'action': 'log_item_repr'}))
-        title.append(iTree('item', data={'name': 'Render Tree',
+        title.append(iTree('item', value={'name': 'Render Tree',
                                          'tooltip': 'Give the rendered item tree in the log',
                                          'action': 'log_item_render'}))
 
         context_menu.append(iTree('separator'))
         if not parent_read_only:
-            new_menu=iTree('item', data={'name': 'Create new iTree'})
+            new_menu=iTree('item', value={'name': 'Create new iTree'})
             if not item.is_root:
                 new_menu.append(
-                    iTree('item', data={'name': 'insert sibling before','action': 'insert_new_sibling_before'}))
+                    iTree('item', value={'name': 'insert sibling before','action': 'insert_new_sibling_before'}))
                 new_menu.append(
-                    iTree('item', data={'name': 'insert sibling after','action': 'insert_new_sibling_after'}))
+                    iTree('item', value={'name': 'insert sibling after','action': 'insert_new_sibling_after'}))
                 new_menu.append(
-                    iTree('item', data={'name': 'append sibling', 'action': 'append_new_sibling_after'}))
+                    iTree('item', value={'name': 'append sibling', 'action': 'append_new_sibling_after'}))
             context_menu.append(new_menu)
 
-            new2_menu=iTree('item', data={'name': 'Create new iTreeLink'})
+            new2_menu=iTree('item', value={'name': 'Create new iTreeLink'})
             if not item.is_root:
                 new2_menu.append(
-                    iTree('item', data={'name': 'insert sibling before','action': 'insert_new_link_sibling_before'}))
+                    iTree('item', value={'name': 'insert sibling before','action': 'insert_new_link_sibling_before'}))
                 new2_menu.append(
-                    iTree('item', data={'name': 'insert sibling after','action': 'insert_new_link_sibling_after'}))
+                    iTree('item', value={'name': 'insert sibling after','action': 'insert_new_link_sibling_after'}))
                 new2_menu.append(
-                    iTree('item', data={'name': 'append sibling', 'action': 'append_new_link_sibling_after'}))
+                    iTree('item', value={'name': 'append sibling', 'action': 'append_new_link_sibling_after'}))
             context_menu.append(new2_menu)
 
             context_menu.append(
-                iTree('item', data={'name': 'make item writeable',
+                iTree('item', value={'name': 'make item writeable',
                                     'action': 'make_writeable_item'}))
 
             context_menu.append(
-                iTree('item', data={'name': 'make item and all sub children writeable',
+                iTree('item', value={'name': 'make item and all sub children writeable',
                                     'action': 'make_writeable_item_all'}))
 
             context_menu.append(
-                iTree('item', data={'name': 'delete selected item',
+                iTree('item', value={'name': 'delete selected item',
                                     'tooltip': 'delete the selected item',
                                     'action': 'delete_item'}))
             context_menu+=iTree('separator')
             move_item = iTree('item',
-                              data={'name': 'Move selected item:'})
+                              value={'name': 'Move selected item:'})
             set=False
             if item.idx != 0:
                 set=True
                 move_item.append(
                     iTree('item',
-                          data={'name': 'move up', 'action': 'move_up'}))
+                          value={'name': 'move up', 'action': 'move_up'}))
             if item.idx < len(item.parent) - 1:
                 set = True
 
                 move_item.append(
                     iTree('item',
-                          data={'name': 'move down', 'action': 'move_down'}))
+                          value={'name': 'move down', 'action': 'move_down'}))
             if not item.parent.is_root:
                 set=True
                 move_item.append(
                     iTree('item',
-                          data={'name': 'move outside (make parents sibling)',
+                          value={'name': 'move outside (make parents sibling)',
                                 'tooltip': 'move selected item inside previous item (append as child)'}))
             if set:
                 context_menu.append(move_item)
 
             context_menu.append(iTree('separator'))
             context_menu.append(
                 iTree('item',
-                      data={'name': 'Cut item',
+                      value={'name': 'Cut item',
                             'action': 'cut_to_clp'}))
         context_menu.append(
             iTree('item',
-                  data={'name': 'Copy',
+                  value={'name': 'Copy',
                         'action': 'copy_to_clp'}))
         context_menu.append(
             iTree('item',
-                  data={'name': 'Copy item key-path',
+                  value={'name': 'Copy item key-path',
                         'action': 'copy_key_path_to_clp'}))
 
         if not parent_read_only:
             if self._valid_clipboard_object(clp_data):
                 context_menu.append(
                     iTree('item',
-                          data={'name': 'Paste',
+                          value={'name': 'Paste',
                                 'action': 'paste_from_clp_after_item'}))
 
         context_menu.append(iTree('separator'))
         v_menu=iTree('item',
-              data={'name': 'Tree visibility'})
+              value={'name': 'Tree visibility'})
         context_menu.append(v_menu)
         v_menu.append(
             iTree('item',
-                  data={'name': 'collapse item',
+                  value={'name': 'collapse item',
                         'action': 'collapse_item'}))
         v_menu.append(
             iTree('item',
-                  data={'name': 'expand item',
+                  value={'name': 'expand item',
                         'action': 'expand_item'}))
         v_menu.append(
             iTree('item',
-                  data={'name': 'collapse item and children',
+                  value={'name': 'collapse item and children',
                         'action': 'collapse_all_sub_items'}))
         v_menu.append(
             iTree('item',
-                  data={'name': 'expand item and children',
+                  value={'name': 'expand item and children',
                         'action': 'expand_all_sub_items'}))
         #context_menu.render()
-        context_menu.d_set('data_key', NOKEY)
+        context_menu.set_key_value('data_key', NOKEY)
         return context_menu
 
 
     def _create_itreelink_popup(self, context_menu, item, detail,clp_data):
         is_link_root=item.link_root==item
         if item.is_root:
-            title = iTree('item', data={'name': 'Tag: ' + item.tag})
+            title = iTree('item', value={'name': 'Tag: ' + item.tag})
         else:
             name = ['TagIdx(%s,%i)' % (t[0], t[1]) for t in item.tag_idx_path]
-            title = iTree('item', data={'name': 'Tag-Idx-Path: ' + str(name)})
+            title = iTree('item', value={'name': 'Tag-Idx-Path: ' + str(name)})
         context_menu.append(title)
 
-        title.append(iTree('item', data={'name': 'Show item representations:'}))
+        title.append(iTree('item', value={'name': 'Show item representations:'}))
         title.append(iTree('separator'))
-        title.append(iTree('item', data={'name': 'Short repr() (no subtree)',
+        title.append(iTree('item', value={'name': 'Short repr() (no subtree)',
                                          'tooltip': 'print item repr in the log',
                                          'action': 'log_item_repr_short'}))
-        title.append(iTree('item', data={'name': 'Full repr() (with subtree)',
+        title.append(iTree('item', value={'name': 'Full repr() (with subtree)',
                                          'tooltip': 'print item repr in the log',
                                          'action': 'log_item_repr'}))
-        title.append(iTree('item', data={'name': 'Render Tree',
+        title.append(iTree('item', value={'name': 'Render Tree',
                                          'tooltip': 'Give the rendered item tree in the log',
                                          'action': 'log_item_render'}))
 
         context_menu.append(iTree('separator'))
         if is_link_root:
-            item_edit=iTree('item', data={'name': 'edit item'})
+            item_edit=iTree('item', value={'name': 'edit item'})
             context_menu.append(item_edit)
-            item_edit.append(iTree('item', data={'name': 'edit item tag',
+            item_edit.append(iTree('item', value={'name': 'edit item tag',
                                                     'tooltip': 'change the tag of the item',
                                                     'key': 'Ctrl-t',
                                                     'action': 'edit_tag'}))
-            item_edit.append(iTree('item', data={'name': 'edit file link',
+            item_edit.append(iTree('item', value={'name': 'edit file link',
                                                  'action': 'edit_file_link'}))
 
-            item_edit.append(iTree('item', data={'name': 'edit key link',
+            item_edit.append(iTree('item', value={'name': 'edit key link',
                                                  'action': 'edit_key_link'}))
 
             if item.data.is_empty:
-                item_edit.append(iTree('item', data={'name': 'set data value (no model)',
+                item_edit.append(iTree('item', value={'name': 'set data value (no model)',
                                                     'tooltip': 'enter a data value directly (no model)',
                                                     'action': 'set_data_value'}))
-                item_edit.append(iTree('item', data={'name': 'add new data key',
+                item_edit.append(iTree('item', value={'name': 'add new data key',
                                                     'tooltip': 'add a data key where a value can be added afterwards',
                                                     'action': 'add_empty_data_key'}))
-                item_edit.append(iTree('item', data={'name': 'edit data model',
+                item_edit.append(iTree('item', value={'name': 'edit data model',
                                                     'tooltip': 'edit/define the specific data-model',
                                                     'action': 'edit_data_model'}))
-        new_menu=iTree('item', data={'name': 'Create new iTree'})
+        new_menu=iTree('item', value={'name': 'Create new iTree'})
         if not item.is_root:
             new_menu.append(
-                iTree('item', data={'name': 'insert sibling before','action': 'insert_new_sibling_before'}))
+                iTree('item', value={'name': 'insert sibling before','action': 'insert_new_sibling_before'}))
             new_menu.append(
-                iTree('item', data={'name': 'insert sibling after','action': 'insert_new_sibling_after'}))
+                iTree('item', value={'name': 'insert sibling after','action': 'insert_new_sibling_after'}))
             new_menu.append(
-                iTree('item', data={'name': 'append sibling', 'action': 'append_new_sibling_after'}))
+                iTree('item', value={'name': 'append sibling', 'action': 'append_new_sibling_after'}))
         context_menu.append(new_menu)
 
-        new2_menu=iTree('item', data={'name': 'Create new iTreeLink'})
+        new2_menu=iTree('item', value={'name': 'Create new iTreeLink'})
         if not item.is_root:
             new2_menu.append(
-                iTree('item', data={'name': 'insert sibling before','action': 'insert_new_link_sibling_before'}))
+                iTree('item', value={'name': 'insert sibling before','action': 'insert_new_link_sibling_before'}))
             new2_menu.append(
-                iTree('item', data={'name': 'insert sibling after','action': 'insert_new_link_sibling_after'}))
+                iTree('item', value={'name': 'insert sibling after','action': 'insert_new_link_sibling_after'}))
             new2_menu.append(
-                iTree('item', data={'name': 'append sibling', 'action': 'append_new_link_sibling_after'}))
+                iTree('item', value={'name': 'append sibling', 'action': 'append_new_link_sibling_after'}))
         context_menu.append(new2_menu)
         context_menu.append(
-            iTree('item', data={'name': 'load/relaod reference', 'action': 'load_links'}))
+            iTree('item', value={'name': 'load/relaod reference', 'action': 'load_links'}))
         if not is_link_root:
             context_menu.append(
-                    iTree('item', data={'name': 'make local', 'action': 'make_item_local'}))
+                    iTree('item', value={'name': 'make local', 'action': 'make_item_local'}))
             if is_link_root:
                 context_menu.append(
-                    iTree('item', data={'name': 'delete selected item',
+                    iTree('item', value={'name': 'delete selected item',
                                         'tooltip': 'delete the selected item',
                                         'action': 'delete_item'}))
 
         if is_link_root:
 
-            new2_menu = iTree('item', data={'name': 'Load/Reload Links',
+            new2_menu = iTree('item', value={'name': 'Load/Reload Links',
                                             'action': 'load_links'})
             context_menu.append(new2_menu)
 
 
             context_menu.append(iTree('separator'))
             if not item.is_root:
                 move_item = iTree('item',
-                                  data={'name': 'Move selected item:'})
+                                  value={'name': 'Move selected item:'})
                 set=False
                 if item.idx != 0:
                     set=True
                     move_item.append(
                         iTree('item',
-                              data={'name': 'move up', 'action': 'move_up'}))
+                              value={'name': 'move up', 'action': 'move_up'}))
                 if item.idx < len(item.parent) - 1:
                     set = True
 
                     move_item.append(
                         iTree('item',
-                              data={'name': 'move down', 'action': 'move_down'}))
+                              value={'name': 'move down', 'action': 'move_down'}))
                 if set:
                     context_menu.append(move_item)
 
                 context_menu.append(iTree('separator'))
             context_menu.append(
                 iTree('item',
-                      data={'name': 'Cut item',
+                      value={'name': 'Cut item',
                             'action': 'cut_to_clp'}))
             context_menu.append(
                 iTree('item',
-                      data={'name': 'Copy',
+                      value={'name': 'Copy',
                             'action': 'copy_to_clp'}))
         context_menu.append(
         iTree('item',
-              data={'name': 'Copy item key-path',
+              value={'name': 'Copy item key-path',
                     'action': 'copy_key_path_to_clp'}))
 
         if self._valid_clipboard_object(clp_data):
             context_menu.append(
                 iTree('item',
-                      data={'name': 'Paste',
+                      value={'name': 'Paste',
                             'action': 'paste_from_clp_after_item'}))
 
         context_menu.append(iTree('separator'))
         v_menu=iTree('item',
-              data={'name': 'Tree visibility'})
+              value={'name': 'Tree visibility'})
         context_menu.append(v_menu)
         v_menu.append(
             iTree('item',
-                  data={'name': 'collapse item',
+                  value={'name': 'collapse item',
                         'action': 'collapse_item'}))
         v_menu.append(
             iTree('item',
-                  data={'name': 'expand item',
+                  value={'name': 'expand item',
                         'action': 'expand_item'}))
         v_menu.append(
             iTree('item',
-                  data={'name': 'collapse item and children',
+                  value={'name': 'collapse item and children',
                         'action': 'collapse_all_sub_items'}))
         v_menu.append(
             iTree('item',
-                  data={'name': 'expand item and children',
+                  value={'name': 'expand item and children',
                         'action': 'expand_all_sub_items'}))
         #context_menu.render()
-        context_menu.d_set('data_key', NOKEY)
+        context_menu.set_value_key('data_key', NOKEY)
         return context_menu
 
     def build_data_item_popup(self,data_item_root,data_item):
         data_item_root.append(
-                            iTree('item', data={'name': 'edit value',
+                            iTree('item', value={'name': 'edit value',
                                                 'tooltip': 'change the data content'
                                 ,'action':'edit_data_item'}))
         data_item_root.append(iTree('separator'))
         if isinstance(data_item,Data.iTDataModel):
             if data_item.__class__ in DATA_MODELS:
                 data_item_root.append(
-                    iTree('item', data={'name': data_item.__class__.__name__,
+                    iTree('item', value={'name': data_item.__class__.__name__,
                                         'tooltip': 'edit data-model properties',
                                         'action':'edit_data_item_model'}))
             else:
                 data_item_root.append(
-                    iTree('item', data={'name': data_item.__class__.__name__, 'tooltip': 'unknown data model (no model properties editable)'}))
+                    iTree('item', value={'name': data_item.__class__.__name__, 'tooltip': 'unknown data model (no model properties editable)'}))
         else:
             data_item_root.append(
-                iTree('item', data={'name': 'No data-model',
+                iTree('item', value={'name': 'No data-model',
                                     'tooltip': 'No data-model value only type (no model properties editable)'}))
         data_item_root.append(iTree('separator'))
-        data_models=iTree('item', data={'name': 'change data-model to:',
+        data_models=iTree('item', value={'name': 'change data-model to:',
                                 'tooltip': 'change data-model'})
         data_item_root.append(data_models)
         data_models.append(
-            iTree('item', data={'name': 'NO data model/ value only',
+            iTree('item', value={'name': 'NO data model/ value only',
                                 'tooltip': 'change remove data model and switch to value only mode'}))
         for m in DATA_MODELS:
             data_models.append(
-                iTree('item', data={'name': m.__class__.__name__,
+                iTree('item', value={'name': m.__class__.__name__,
                                     'tooltip': m.Description}))
 
 
     def _create_list_popup(self, context_menu, items,clp_data):
 
-        title = iTree('item', data={'Multi-Selection'})
+        title = iTree('item', value={'Multi-Selection'})
         context_menu.append(title)
         context_menu.append(iTree('separator'))
         context_menu.append(
-        iTree('item', data={'name': 'Delete',
+        iTree('item', value={'name': 'Delete',
                                 'tooltip': 'delete the selected item',
                                 'action': 'delete_item'}))
         context_menu.append(
             iTree('item',
-                  data={'name': 'Cut items',
+                  value={'name': 'Cut items',
                         'action': 'cut_to_clp'}))
         context_menu.append(
             iTree('item',
-                  data={'name': 'Copy items',
+                  value={'name': 'Copy items',
                         'action': 'copy_to_clp'}))
         context_menu.append(iTree('separator'))
         v_menu=iTree('item',
-              data={'name': 'Tree visibility'})
+              value={'name': 'Tree visibility'})
         context_menu.append(v_menu)
         v_menu.append(
             iTree('item',
-                  data={'name': 'collapse item',
+                  value={'name': 'collapse item',
                         'action': 'collapse_item'}))
         v_menu.append(
             iTree('item',
-                  data={'name': 'expand item',
+                  value={'name': 'expand item',
                         'action': 'expand_item'}))
         v_menu.append(
             iTree('item',
-                  data={'name': 'collapse item and children',
+                  value={'name': 'collapse item and children',
                         'action': 'collapse_all_sub_items'}))
         v_menu.append(
             iTree('item',
-                  data={'name': 'expand item and children',
+                  value={'name': 'expand item and children',
                         'action': 'expand_all_sub_items'}))
 
-        context_menu.d_set('data_key', NOKEY)
+        context_menu.set_key_value('data_key', NOKEY)
         return context_menu
 
     def create_popup_menu_tree_items(self,sel_items,sel_details,x,y,clp_data):
         '''
         create an itree containing the related popup menu entries
         the context menu depends on the type of selection made
 
         :param item: selects items
         :return:
         '''
 
-        context_menu = iTree('root', data={'x': x, 'y': y, 'sel_items': sel_items, 'sel_details': sel_details})
+        context_menu = iTree('root', value={'x': x, 'y': y, 'sel_items': sel_items, 'sel_details': sel_details})
         l=len(sel_items)
         if l==0:
             return context_menu
         elif l==1:
             item=sel_items[0]
             if item is None:
                 return context_menu
@@ -759,15 +764,15 @@
 
     def item_set_data_value(self,item,key,raw_value):
         try:
             value = eval(raw_value)
         except:
             value=raw_value
         try:
-            item.d_set(key,value)
+            item.set_key_value(key,value)
             action = ActionItem('update_tree',item )
             self.distribute(action)
             action = ActionItem('make_visible_itree_item', item,True,key)
             self.distribute(action)
         except Exception as e:
             action = ActionItem('log', '%s'%str(e))
             self.distribute(action)
@@ -777,15 +782,15 @@
             value = eval(raw_value)
         except:
             value=raw_value
         try:
             if key=='linked_file_path':
                 new_item=iTreeLink(item.tag,
                                    link_file_path=value,
-                                   link_key_path=item._link.key_path,
+                                   link_key_path=item._link.tag_idx_path,
                                    subtree=item.iter_locals(add_placeholders=True),
                                    load_links=False)
             elif key=='linked_key_path':
                 new_item=iTreeLink(item.tag,
                                    link_file_path=item._link.file_path,
                                    link_key_path=value,
                                    subtree=item.iter_locals(add_placeholders=True),
@@ -803,15 +808,15 @@
 
     def item_add_data_key(self,item,raw_key):
         try:
             key = literal_eval(raw_key)
         except:
             key=raw_key
         #We set no value first
-        item.d_set(key=key)
+        item.set_value(key)
         action = ActionItem('update_tree',item )
         self.distribute(action)
         action = ActionItem('make_visible_itree_item', item,True,key)
         self.distribute(action)
 
 
     def item_append_child(self,item,new_tag,itreelink=False):
@@ -929,15 +934,15 @@
         action = ActionItem('log', 'References loaded')
         self.distribute(action)
 
     def items_make_local(self, items):
         for item in items:
             if isinstance(item, iTreeLink) and not item.is_link_root:
                 coupled_object=item.coupled_object
-                old_items=item.iter_all()
+                old_items=list(item.deep)
                 item=item.make_self_local()
         action = ActionItem('update_tree')
         self.distribute(action)
         action = ActionItem('make_visible_itree_item', item,True)
         self.distribute(action)
 
     def items_make_read_only(self, items):
@@ -1079,8 +1084,8 @@
         tmp.destroy()
 
     def paste_from_os_clp(self):
         tmp = Tk()
         return tmp.clipboard_get()
 
     def __del__(self):
-        self._temp_dir.cleanup()
+        self._temp_dir.cleanup()
```

### Comparing `itertree-0.8.2/src/itertree/examples/itree_editor/gui.py` & `itertree-1.0.0/src/itertree/examples/itree_editor/gui.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,34 +3,39 @@
 This code is taken from the itertree package:
 https://pypi.org/project/itertree/
 GIT Home:
 https://github.com/BR1py/itertree
 The documentation can be found here:
 https://itertree.readthedocs.io/en/latest/index.html
 
-The code is published under MIT license:
+The code is published under MIT license incl. human protect patch:
 
-The MIT License (MIT)
+The MIT License (MIT) incl. human protect patch
 Copyright © 2022 <copyright holders>
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 documentation files (the “Software”), to deal in the Software without restriction, including without limitation
 the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and
 to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
+Human protect patch:
+The program and its derivative work will neither be modified or executed to harm any human being nor through
+inaction permit any human being to be harmed.
+
 The above copyright notice and this permission notice shall be included in all copies or substantial
 portions of the Software.
 
 THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO
 THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS
 OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT
 OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 For more information see: https://en.wikipedia.org/wiki/MIT_License
 
+
 """
 from __future__ import absolute_import
 import datetime
 import pickle
 import tkinter as tk
 from tkinter import ttk
 from tkinter import simpledialog, filedialog, commondialog
@@ -187,275 +192,275 @@
 
         self._active_popup = None
 
     def set_active_popup(self, active_popup):
         self._active_popup = active_popup
 
     def log_item_repr_short(self):
-        items = self._active_popup.data.get('sel_items')
+        items = self._active_popup.value.get('sel_items')
         if len(items) != 1:
             return
         out = repr(items[0])
         tmp = out.split(', subtree')
         if len(tmp) > 1:
             out = tmp[0] + ')'
         self.log(out)
 
     def log_item_repr(self):
-        items = self._active_popup.data.get('sel_items')
+        items = self._active_popup.value.get('sel_items')
         if len(items) != 1:
             return
         self.log(repr(items[0]))
 
     def log_item_render(self):
-        items = self._active_popup.data.get('sel_items')
+        items = self._active_popup.value.get('sel_items')
         if len(items) != 1:
             return
         self.log('\n' + items[0].renders())
 
     def edit_tag(self):
-        items = self._active_popup.data.get('sel_items')
+        items = self._active_popup.value.get('sel_items')
         if len(items) != 1:
             return
         tag = items[0].tag
         if type(tag) is not str:
             tag = repr(tag)
         answer = simpledialog.askstring("Change Item Tag", "TAG: ", initialvalue=tag,
                                         parent=self._tk_main)
         if answer is not None or answer != tag:
             self._controller.item_rename(items[0], answer)
 
     def edit_data_model(self):
-        items = self._active_popup.data.get('sel_items')
+        items = self._active_popup.value.get('sel_items')
         if len(items) != 1:
             return
         item = items[0]
-        key = self._active_popup.data.get('data_key')
+        key = self._active_popup.value.get('data_key')
         try:
-            data_item = item.d_get(key, return_type=Data.FULL)
-            data = item.d_get(key)
+            data_item = item.get_key_value(key)
+            data = item.value
         except KeyError:
             data_item = None
             data = Data.__NOVALUE__
-        if isinstance(data_item, Data.iTDataModel):
+        if hasattr(data_item, 'is_iTValueModel'):
             current_model = data_item
         else:
             current_model = None
         ModelDialog(self, current_model, (item, key,data))
 
     def set_data_model(self, item, key,data, model):
         if model is None:
             # no model selected
-            item.d_set(key, data)
+            item.set_key_value(key, data)
         else:
             try:
-                model.set(data)
+                model.set_value(data)
             except:
                 self.log('Old value does not match to new model, old data value is not filled in')
 
             else:
                 self.log('Old value put in new model')
-            item.data.update([(key,model)],replace_models=True)
+            item.value.update([(key,model)],replace_models=True)
             self._parent.update_tree(item)
 
     def set_data_value(self):
-        items = self._active_popup.data.get('sel_items')
+        items = self._active_popup.value.get('sel_items')
         if len(items) != 1:
             return
         answer = simpledialog.askstring("Data Value Input", "VALUE: ", parent=self._tk_main)
         if answer is not None:
-            self._controller.item_set_data_value(items[0], key=self._active_popup.data.get('data_key'),
+            self._controller.item_set_data_value(items[0], key=self._active_popup.value.get('data_key'),
                                                  raw_value=answer)
 
     def set_link_value(self):
-        items = self._active_popup.data.get('sel_items')
-        key=self._active_popup.data.get('data_key')
+        items = self._active_popup.value.get('sel_items')
+        key=self._active_popup.value.get('data_key')
         if len(items) != 1:
             return
         answer = simpledialog.askstring("Link Value Input", "%s: "%key, parent=self._tk_main)
         if answer is not None:
             self._controller.item_set_link_value(items[0], key=key,
                                                  raw_value=answer)
 
     def add_empty_data_key(self):
-        items = self._active_popup.data.get('sel_items')
+        items = self._active_popup.value.get('sel_items')
         if len(items) != 1:
             return
         answer = simpledialog.askstring("Data Key Input", "KEY: ", parent=self._tk_main)
         if answer is not None:
             self._controller.item_add_data_key(items[0], answer)
 
     def append_new_child(self):
-        items = self._active_popup.data.get('sel_items')
+        items = self._active_popup.value.get('sel_items')
         if len(items) != 1:
             return
         answer = simpledialog.askstring("Give tag of new child to be appended", "TAG: ",
                                         parent=self._tk_main)
         if answer is not None:
             self._controller.item_append_child(items[0], answer)
 
     def insert_new_sibling_before(self):
-        items = self._active_popup.data.get('sel_items')
+        items = self._active_popup.value.get('sel_items')
         if len(items) != 1:
             return
         answer = simpledialog.askstring("Give tag of new item", "TAG: ",
                                         parent=self._tk_main)
         if answer is not None:
             self._controller.item_insert_new(items[0], answer, before=True)
 
     def insert_new_sibling_after(self):
-        items = self._active_popup.data.get('sel_items')
+        items = self._active_popup.value.get('sel_items')
         if len(items) != 1:
             return
         answer = simpledialog.askstring("Give tag of new item", "TAG: ",
                                         parent=self._tk_main)
         if answer is not None:
             self._controller.item_insert_new(items[0], answer, before=False)
 
     def append_new_sibling_after(self):
-        items = self._active_popup.data.get('sel_items')
+        items = self._active_popup.value.get('sel_items')
         if len(items) != 1:
             return
         answer = simpledialog.askstring("Give tag of new item", "TAG: ",
                                         parent=self._tk_main)
         if answer is not None:
             self._controller.item_append_child(items[0].parent, answer)
 
     def append_new_child_link(self):
-        items = self._active_popup.data.get('sel_items')
+        items = self._active_popup.value.get('sel_items')
         if len(items) != 1:
             return
         answer = simpledialog.askstring("Give tag of new child to be appended", "TAG: ",
                                         parent=self._tk_main)
         if answer is not None:
             self._controller.item_append_child(items[0], answer,itreelink=True)
 
     def insert_new_link_sibling_before(self):
-        items = self._active_popup.data.get('sel_items')
+        items = self._active_popup.value.get('sel_items')
         if len(items) != 1:
             return
         answer = simpledialog.askstring("Give tag of new link-item", "TAG: ",
                                         parent=self._tk_main)
         if answer is not None:
             self._controller.item_insert_new(items[0], answer, before=True,itreelink=True)
 
     def insert_new_link_sibling_after(self):
-        items = self._active_popup.data.get('sel_items')
+        items = self._active_popup.value.get('sel_items')
         if len(items) != 1:
             return
         answer = simpledialog.askstring("Give tag of new link-item", "TAG: ",
                                         parent=self._tk_main)
         if answer is not None:
             self._controller.item_insert_new(items[0], answer, before=False,itreelink=True)
 
     def append_new_link_sibling_after(self):
-        items = self._active_popup.data.get('sel_items')
+        items = self._active_popup.value.get('sel_items')
         if len(items) != 1:
             return
         answer = simpledialog.askstring("Give tag of new link-item", "TAG: ",
                                         parent=self._tk_main)
         if answer is not None:
             self._controller.item_append_child(items[0].parent, answer,itreelink=True)
 
     def load_links(self):
-        items = self._active_popup.data.get('sel_items')
+        items = self._active_popup.value.get('sel_items')
         self._controller.items_load_links(items)
 
     def make_item_local(self):
-        items = self._active_popup.data.get('sel_items')
+        items = self._active_popup.value.get('sel_items')
         self._controller.items_make_local(items)
 
     def make_writeable_item(self):
-        items = self._active_popup.data.get('sel_items')
+        items = self._active_popup.value.get('sel_items')
         self._controller.items_make_writeable(items)
 
     def make_writeable_item_all(self):
-        items = self._active_popup.data.get('sel_items')
+        items = self._active_popup.value.get('sel_items')
         self._controller.items_make_writeable(items,all=True)
 
     def make_read_only_item(self):
-        items = self._active_popup.data.get('sel_items')
+        items = self._active_popup.value.get('sel_items')
         self._controller.items_make_read_only(items)
 
     def delete_item(self):
-        items = self._active_popup.data.get('sel_items')
+        items = self._active_popup.value.get('sel_items')
         self._controller.items_delete(items)
 
     def move_up(self):
-        items = self._active_popup.data.get('sel_items')
+        items = self._active_popup.value.get('sel_items')
         self._controller.move(items[0], up=True)
 
     def move_down(self):
-        items = self._active_popup.data.get('sel_items')
+        items = self._active_popup.value.get('sel_items')
         self._controller.move(items[0], up=False)
 
     def move_inside_first(self):
-        items = self._active_popup.data.get('sel_items')
+        items = self._active_popup.value.get('sel_items')
         self._controller.move_inside(items, first=True)
 
     def move_inside_last(self):
-        items = self._active_popup.data.get('sel_items')
+        items = self._active_popup.value.get('sel_items')
         self._controller.move_inside(items, first=False)
 
     def cut_to_clp(self):
-        items = self._active_popup.data.get('sel_items')
+        items = self._active_popup.value.get('sel_items')
         self._controller.cut_items(items)
 
     def copy_to_clp(self):
-        items = self._active_popup.data.get('sel_items')
+        items = self._active_popup.value.get('sel_items')
         self._controller.copy_items(items)
 
     def copy_key_path_to_clp(self):
-        items = self._active_popup.data.get('sel_items')
+        items = self._active_popup.value.get('sel_items')
         if len(items)!=1:
             return
         path=items[0].tag_idx_path
         self._controller.copy_to_os_clp(repr(path))
 
     def paste_from_clp_after_item(self):
-        items = self._active_popup.data.get('sel_items')
+        items = self._active_popup.value.get('sel_items')
         clp_raw = self._tk_main.clipboard_get()
         for item in items:
             self._controller.item_insert_clp(item, clp_raw, inside=False)
 
     def paste_from_clp_inside_item(self):
-        items = self._active_popup.data.get('sel_items')
+        items = self._active_popup.value.get('sel_items')
         clp_raw = self._tk_main.clipboard_get()
         for item in items:
             self._controller.item_insert_clp(item, clp_raw, inside=True)
 
     def expand_item(self, item=None):
         tree = self._parent._tree
-        items = self._active_popup.data.get('sel_items')
+        items = self._active_popup.value.get('sel_items')
         for itree_item in items:
             item = itree_item.coupled_object
             tree.item(item, open=True)
             for child in self._parent._tree.get_children(item):
                 if tree.item(child).get('text') == 'data':
                     tree.item(child, open=True)
                     for key in self._parent._tree.get_children(child):
                         tree.item(key, open=True)
             tree.see(item)
 
     def collapse_item(self):
         tree = self._parent._tree
-        items = self._active_popup.data.get('sel_items')
+        items = self._active_popup.value.get('sel_items')
         for itree_item in items:
             item = itree_item.coupled_object
             tree.item(item, open=False)
             for child in self._parent._tree.get_children(item):
                 if tree.item(child).get('text') == 'data':
                     tree.item(child, open=False)
                     for key in self._parent._tree.get_children(child):
                         tree.item(key, open=False)
 
     def expand_all_sub_items(self, item=None):
         tree = self._parent._tree
         if item is None:
-            items = self._active_popup.data.get('sel_items')
+            items = self._active_popup.value.get('sel_items')
         else:
             items = [item]
         for itree_item in items:
             if type(itree_item) is str:
                 item = itree_item
             else:
                 item = itree_item.coupled_object
@@ -463,15 +468,15 @@
             for child in tree.get_children(item):
                 self.expand_all_sub_items(child)
         tree.see(item)
 
     def collapse_all_sub_items(self, item=None):
         tree = self._parent._tree
         if item is None:
-            items = self._active_popup.data.get('sel_items')
+            items = self._active_popup.value.get('sel_items')
         else:
             items = [item]
         for itree_item in items:
             if type(itree_item) is str:
                 item = itree_item
             else:
                 item = itree_item.coupled_object
@@ -588,30 +593,30 @@
         for c in popup_itree:
             if c.tag == 'separator':
                 menu.add_separator()
                 continue
             if len(c) != 0:
                 sub_menu = tk.Menu(self._tk_main, tearoff=0)
                 self.create_popup(c, sub_menu)
-                menu.add_cascade(label=c.data.get('name'), menu=sub_menu)
+                menu.add_cascade(label=c.get_key_value('name'), menu=sub_menu)
             else:
                 caller = None
-                action = c.data.get('action')
+                action = c.value.get('action')
                 if action is not None:
                     try:
                         caller = self.popup_commands.__getattribute__(action)
                     except:
                         pass
                 if caller is None:
-                    menu.add_command(label=c.data.get('name'))
+                    menu.add_command(label=c.get_key_value('name'))
                 else:
-                    menu.add_command(label=c.data.get('name'), command=caller)
+                    menu.add_command(label=c.get_key_value('name'), command=caller)
         if parent is None:
             try:
-                menu.tk_popup(popup_itree.data.get('x'), popup_itree.data.get('y'), 0)
+                menu.tk_popup(popup_itree.get_key_value('x'), popup_itree.get_key_value('y'), 0)
             except:
                 pass
 
     def __update_from_controller(self):
         # Timer function that takes the actions from the controller to be done
         while 1:
             if len(self._action_buffer) == 0:
@@ -649,60 +654,62 @@
         self._log_box.insert('end', '%s %s%s' % (t, str(log_str), n))
         self._log_box.update()
         self._log_box.see(tk.END)
         self._log_box.config(state='disable')
 
     def _add_link(self,it_item,item):
         root = self._tree
-        link_obj = it_item._link
-        if link_obj  is None:
+        if it_item.is_link_root:
+            link_obj = it_item._link
+        else:
             return
         link_item = root.insert('', 'end', text='link',  tag='ItalicItem')
         root.move(link_item, item, 'end')
         if link_obj.source_path is not None:
             sub_item = root.insert('', 'end', text='source_path',value=[str(link_obj.source_path)])
             root.move(sub_item, link_item, 'end')
         link_added=False
         if link_obj.file_path is not None:
             sub_item = root.insert('', 'end', text='linked_file_path', value=[str(link_obj.file_path)], tag='ItalicItem')
             root.move(sub_item, link_item, 'end')
             link_added = True
 
-        if link_obj.key_path is not None:
+        if link_obj.tag_idx_path is not None:
             if not link_added:
                 sub_item = root.insert('', 'end', text='linked_file_path', value=[str(None)],
                                        tag='ItalicItem')
                 root.move(sub_item, link_item, 'end')
-            sub_item = root.insert('', 'end', text='linked_key_path', value=[str(link_obj.key_path)], tag='ItalicItem')
+            sub_item = root.insert('', 'end', text='linked_key_path', value=[str(link_obj.tag_idx_path)], tag='ItalicItem')
             root.move(sub_item, link_item, 'end')
 
     def _add_data(self, it_item, item):
         root = self._tree
         v = ''
-        if not it_item.data.is_empty:
-            if not it_item.data.is_key_empty():
-                v = it_item.d_get()
-                if isinstance(v, Data.iTDataModel):
-                    v = v.value
-                v_str = repr(v)
-                data_item = root.insert('', 'end', text='data', value=[v_str], tag='ItalicItem')
-            else:
-                data_item = root.insert('', 'end', text='data', tag='ItalicItem')
+        if not it_item.value is NoValue:
+            v = it_item.get_value()
+            if hasattr(v, 'is_iTValueModel'):
+                v = v.value
+            v_str = repr(v)
+            data_item = root.insert('', 'end', text='value', value=[v_str], tag='ItalicItem')
+            root.move(data_item, item, 'end')
+            if hasattr(it_item.value,'items'):
+                for k, v in it_item.value.items():
+                    if k == NOKEY:
+                        continue
+                    if hasattr(v, 'is_iTValueModel'):
+                        v = v.value
+                    v_str = repr(v)
+                    if v is NOVALUE:
+                        sub_data_item = root.insert('', 'end', text=repr(k), tag='ItalicItem')
+                    else:
+                        sub_data_item = root.insert('', 'end', text=repr(k), value=[v_str], tag='ItalicItem')
+                    root.move(sub_data_item, data_item, 'end')
+        else:
+            data_item = root.insert('', 'end', text='value', tag='ItalicItem')
             root.move(data_item, item, 'end')
-            for k, v in it_item.data.items():
-                if k == NOKEY:
-                    continue
-                if isinstance(v, Data.iTData):
-                    v = v.value
-                v_str = repr(v)
-                if v is NOVALUE:
-                    sub_data_item = root.insert('', 'end', text=repr(k), tag='ItalicItem')
-                else:
-                    sub_data_item = root.insert('', 'end', text=repr(k), value=[v_str], tag='ItalicItem')
-                root.move(sub_data_item, data_item, 'end')
 
     def update_tree(self, it_item=None, clean=True):
         root = self._tree
         if it_item is None:
             for v in self._tree_to_item_dict.values():
                 it_item=v.root
                 break
@@ -717,15 +724,15 @@
         else:
             if clean:
                 self.clear_tree(it_item.parent)
                 it_item = it_item.parent
         t_parent = it_item.coupled_object
         for child in it_item:
             text = '%s(%s)' % (child.__class__.__name__, child.tag)
-            if isinstance(child,iTree) and (child.is_linked or child.is_read_only or child.is_placeholder):
+            if isinstance(child,iTree) and (child.is_linked or child.is_tree_read_only or child.is_placeholder):
                 t_item = root.insert('', 'end', text=text)
             else:
                 t_item = root.insert('', 'end', text=text, tag='BoldItem')
             root.move(t_item, t_parent, tk.END)
             child.set_coupled_object(t_item)
             self._tree_to_item_dict[t_item] = child
             self._add_link(child,t_item)
```

### Comparing `itertree-0.8.2/src/itertree/examples/itree_editor/main.py` & `itertree-1.0.0/src/itertree/examples/itree_editor/main.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,45 +3,50 @@
 This code is taken from the itertree package:
 https://pypi.org/project/itertree/
 GIT Home:
 https://github.com/BR1py/itertree
 The documentation can be found here:
 https://itertree.readthedocs.io/en/latest/index.html
 
-The code is published under MIT license:
+The code is published under MIT license incl. human protect patch:
 
-The MIT License (MIT)
+The MIT License (MIT) incl. human protect patch
 Copyright © 2022 <copyright holders>
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 documentation files (the “Software”), to deal in the Software without restriction, including without limitation
 the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and
 to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
+Human protect patch:
+The program and its derivative work will neither be modified or executed to harm any human being nor through
+inaction permit any human being to be harmed.
+
 The above copyright notice and this permission notice shall be included in all copies or substantial
 portions of the Software.
 
 THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO
 THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS
 OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT
 OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 For more information see: https://en.wikipedia.org/wiki/MIT_License
 
+
 """
 from __future__ import absolute_import
 
 from controller import iTreeEditorController
 from gui import iTreeEditorGUI
 from data_models import *
 
 class iTreeEditor():
     def __init__(self):
         self._controller=iTreeEditorController()
-        self._controller.get_data_model_data(IntegerModel())
+        self._controller.get_data_model_data(Data.iTIntModel())
         self._editor_gui=iTreeEditorGUI(self._controller)
         self._editor_gui.run()
 
 if __name__ == '__main__':
     editor=iTreeEditor()
 
 #ToDO:
```

### Comparing `itertree-0.8.2/src/itertree/examples/itree_link_example1.py` & `itertree-1.0.0/src/itertree/examples/itree_link_example1.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,35 +3,40 @@
 This code is taken from the itertree package:
 https://pypi.org/project/itertree/
 GIT Home:
 https://github.com/BR1py/itertree
 The documentation can be found here:
 https://itertree.readthedocs.io/en/latest/index.html
 
-The code is published under MIT license:
+The code is published under MIT license incl. human protect patch:
 
-The MIT License (MIT)
+The MIT License (MIT) incl. human protect patch
 Copyright © 2022 <copyright holders>
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 documentation files (the “Software”), to deal in the Software without restriction, including without limitation
 the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and
 to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
+Human protect patch:
+The program and its derivative work will neither be modified or executed to harm any human being nor through
+inaction permit any human being to be harmed.
+
 The above copyright notice and this permission notice shall be included in all copies or substantial
 portions of the Software.
 
 THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO
 THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS
 OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT
 OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 For more information see: https://en.wikipedia.org/wiki/MIT_License
 
 
+
 This part of code contains some examples for the usage of itertree module
 
 """
 
 from __future__ import absolute_import
 import os
 import shutil
@@ -46,55 +51,69 @@
 B += iTree('Ba')
 B += iTree('Bb')
 B += iTree('Bb')  # we create multiple 'Bb' elements to show how the placeholders are used during save and load
 B += iTree('Bc')
 root += B
 
 # Now we create a internal link:
-linked_element = iTreeLink('internal_link', link_key_path=['/', TagIdx('B', 1)], load_links=False)
+linked_element = iTree('internal_link', link=iTLink(target_path=[('B', 1)]))
 root.append(linked_element)
 print('iTree with linked element but no links loaded:')
 print(root.render())
-root.load_links()
-print('iTree with linked element with links loaded:')
-print(root.render())
+updated=root.load_links()
+if updated:
+    print('iTree with linked element with links loaded')
+else:
+    print('iTree links loaded, but no update required')
+
+print('iTree loaded links:\n')
+root.render()
+
 # changes in "B" are only considered after reloading the links
 B += iTree('B_post_append')
-print('iTree with updated linked element but no reload of the links:\n', root.render())
-print(root.render())
+print('iTree with updated linked element but no reload of the links:\n')
+root.render()
+
+updated=root.load_links()
+if updated:
+    print('iTree with linked element with links loaded')
+else:
+    print('iTree links loaded, but no update required')
 
-root.load_links(force=True)
 print('iTree with updated linked element and with links reloaded:')
-print(root.render())
+
+
+root.render()
 # get the linked element
-il = root[TagIdx('internal_link', 0)]
+il = root[('internal_link', 0)]
 # append an item
 il.append(iTree('new'))
 # we make second element local
-local = il.make_child_local(2)
-local += iTree('sublocal')
+local = il[2].make_local()
+local.append(iTree('sublocal'))
+local.set_value('myvalue')
 print('iTree with linked element and additional local items:')
-print(root.render())
+root.render()
 
 # we store the iTree in a file for later usage:
 temp_dir = tempfile.mkdtemp()
 target_path = os.path.join(temp_dir, 'out_linked.itr')
 root.dump(target_path=target_path, overwrite=True, pack=False)
 
 # if we delete the local object the linked object will come back in the tree:
-del il[TagIdx('Bb', 1)]
+del il[('Bb', 1)]
 print('iTree with linked element and the overloading local item deleted:')
-print(root.render())
+root.render()
 
 # we load without loading the links
 reload_tree = iTree('root').load(target_path, load_links=False)
 # we do not need the stored data anymore:
 shutil.rmtree(temp_dir)
 print('iTree load from file with load_links parameter disabled (to make internal structure visible):')
-print('-> See the placeholder element that was added to keep the TagIdx of the local item Bb[1]')
+print('-> See the placeholder element that was added to keep the key of the local item Bb[1] (flags==0b10000)')
 
-print(reload_tree.render())
+reload_tree.render()
 
 # finally we load the links again and we expect the result before we saved the tree in the file
 print('iTree load from file with load_links() executed:')
 reload_tree.load_links()
-print(reload_tree.render())
+reload_tree.render()
```

### Comparing `itertree-0.8.2/src/itertree/itree_main.py` & `itertree-1.0.0/src/itertree/itree_main.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,2992 +1,3265 @@
 # -*- coding: utf-8 -*-
+
 """
+
 This code is taken from the itertree package:
 https://pypi.org/project/itertree/
 GIT Home:
 https://github.com/BR1py/itertree
 The documentation can be found here:
 https://itertree.readthedocs.io/en/latest/index.html
 
-The code is published under MIT license:
+The code is published under MIT license incl. human protect patch:
 
-The MIT License (MIT)
+The MIT License (MIT) incl. human protect patch
 Copyright © 2022 <copyright holders>
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 documentation files (the “Software”), to deal in the Software without restriction, including without limitation
 the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and
 to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
+Human protect patch:
+The program and its derivative work will neither be modified or executed to harm any human being nor through
+inaction permit any human being to be harmed.
+
 The above copyright notice and this permission notice shall be included in all copies or substantial
 portions of the Software.
 
 THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO
 THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS
 OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT
 OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 For more information see: https://en.wikipedia.org/wiki/MIT_License
 
 
 This part of code contains the main iTree object
+
 """
 
 from __future__ import absolute_import
-import os
 import copy
-import itertools
-from collections import deque
-from .itree_data import iTData, iTDataReadOnly, iTDataModel,__NOKEY__,FULL,VALUE
-from .itree_filter import *
+import pickle
+import traceback
+from itertools import chain, dropwhile, zip_longest, takewhile, repeat, tee, product
+from contextlib import suppress
+from collections import OrderedDict, deque
+from itertools import dropwhile
+# import fnmatch
+# import functools
+# import operator
+import sys
 
 try:
-    # This really recommended for faster operations!
-    from blist import blist
+    from typing import Hashable, Iterable, Callable, Union, Optional
+except ImportError:
+    # <Python 3.5
+    # Only required for doc strings!
+    Hashable = None
+    Iterable = None
+    Callable = None
+    Union = None
+    Optional = None
+
+from .itree_helpers import itree_list, TagIdx, NoTarget, iTFLAG, iTLink, _iTFLAG, NoTag, \
+    NoValue, INF,BLIST_SWITCH
+from .itree_serializer.itree_renderer import iTreeRender
+from .itree_serializer.itree_json_serialize import iTStdJSONSerializer2
+from .itree_indepth import _iTreeIndepthTree
+from .itree_getitem import _iTreeGetitem
+from .itree_private import _iTreePrivate
+
+
+class iTree(_iTreePrivate):
+    __slots__ = (  # Attributes
+        '_tag', '_value', '_link', '_flags', '_coupled',
+        # private helper classes
+        '_itree_prt_idx', '_families', '_items',
+        # serializing objects
+        '__renderer', '__itree_serializer',
+        # quick access methods
+        '__len__', '__iter__', 'getitem_by_idx', '_is_list',
+        # quick access methods
+        '_setitem_list',
+        '_getitem_fam', '_setitem_fam',"_get_fam",
+        # helpers
+        '_hc_tree', 'get'
+    )
 
-    BLIST_ACTIVE = True
-except:
-    # if not available we take normal list
-    blist = list
-    BLIST_ACTIVE = False
+    # we define some static private variables:
+    _filter_linked_roots = lambda i: i.is_link_root
+    _filter_linked_roots_and_linked = lambda i: i.is_link_root or i.is_linked
 
-# This is the second try after self._map[key] was not found!
+    # flags
+    _READ_ONLY_TREE = iTFLAG.READ_ONLY_TREE
+    _READ_ONLY_VALUE = iTFLAG.READ_ONLY_VALUE
+    _LOAD_LINKS = iTFLAG.LOAD_LINKS
 
-__GETITEM_RETURN__ = {
-    TagMultiIdx: lambda self, key, _: self.__get_tag_idxs__(key),
-    TagIdx: lambda self, key, _: self._map[key[0]][key[1]],
-    TagIdxStr: lambda self, key, _: self._map[key[0]][key[1]],
-    TagIdxBytes: lambda self, key, _: self._map[key[0]][key[1]],
-    slice: lambda self, key, _: itertools.islice(super(iTree, self).__iter__(), key.start, key.stop, key.step),
-    iTMatch: lambda self, key, _: filter(lambda item: key.check(item), super(iTree, self).__iter__()),
-    list: lambda self, key, _: accu_iterator(key, lambda c, k: self[k]),
-    # list: lambda self, key, _: iter((self[k] for k in key)),
-    tuple: lambda self, key, _: self._map[key[0]][key[1]],
-    str: lambda self, key, str_index_separator: self.__getitem__(TagIdxStr(key, str_index_separator)),
-    bytes: lambda self, key, str_index_separator: self.__getitem__(TagIdxBytes(key, str_index_separator))
-}
+    # internal flags
+    _LINKED = _iTFLAG.LINKED
+    _LINK_ROOT = _iTFLAG.LINK_ROOT
+    _PLACEHOLDER = _iTFLAG.PLACEHOLDER
+    _FLAG_MASK = _iTFLAG.FLAG_MASK
+    _IS_TREE_PROTECTED = _READ_ONLY_TREE | _PLACEHOLDER | _LINKED | _LINK_ROOT
+    _IS_VALUE_PROTECTED = _READ_ONLY_VALUE | _PLACEHOLDER | _LINKED
+    _DEEP_FLAG_MASK = _LOAD_LINKS | _READ_ONLY_TREE
 
+    _NoneSlice = slice(None)
+    _ONE_ITEM_LIST = itree_list([0])  # used for quickest possible instance of blist
 
-# class iTree(iTMagicList):
-class iTree(blist):
-    """
-    This is the main class related to iTrees.
+    def __init__(self,
+                 tag=NoTag,  # family tag (any hashable object)
+                 value=NoValue,  # data object to be stored in the item
+                 subtree=None,  # subtree definition
+                 link=None,  # link to another iTree
+                 flags=0,  # property flags
+                 ):
+        """
+        This is the main class related to itertree module. It represents the node in the nested tree structure.
 
-    This object is the parent of a sub-tree (children, sub-children, etc.). The iTree object itself can also be a
-    child of a parent iTree object. If this is not the case the iTree object is the root of the tree.
+        In case the object contains a subtree this object is the parent of the children in the subtree and its inner
+        children (children, sub-children, etc.). The ´iTree´-object itself can also be a
+        child of a parent ´iTree´-object. If this is not the case the ´iTree´-object is the root of the tree.
 
-    A iTree object can only be integrated in one tree (one parent only)!
+        *Limitation:* An ´iTree´-object can be integrated as a child in one ´iTree´ only (one parent only principle)!
 
-    Each iTree object contains a tag. In case your tags are stings it's recommended to use tag strings without
-    wildcards "*","?" and without the standard separators "/" and "#". If you use these characters you might get
-    confusing results in find, filter and match operations.
+        Each ´iTree´-object contains a "tag". The objects tag can be any hashable object.
 
-    In general we allow all hashable objects to be used as a tag in the iTree objects (only search operation might be
-    limited in this case).
-    But we have two exceptions: We do not allow integers and TagIdx objects as tags because those objects used for
-    direct item access.
+        Different as dictionaries it is allowed to put multiple items with the same tag inside the ´iTree´.
+        Those items with
+        the same tag are placed and ordered (enumerated) in the related tag-family. The specific items can be targeted
+        via a zag_idx tuple (family-tag,family-index) which is the items unique key.
 
-    Different than in dictionaries it is allowed to put multiple times the same tag inside the iTree. The items with
-    the same tag are placed and ordered (enumerated) in the related tag-family. They can be reached via TagIdx
-    objects by giving the tag, index pair (tag_idx).
+        Linked ´iTree´-objects will behave a bit special. They have a read only structure (children) and they contain
+        the children (tree) of the linked ´iTree´.
+        The "local" attributes like tag, value, ... can be set independent of the linked item (local properties).
 
-    Linked iTree objects will behave different. They have a read only structure (children) and they contain
-    the children (tree) of the linked iTree.
-    The "local" attributes like tag, data, ... can be set independent from the linked item (local properties).
-    To change the tree structure of such an object you must manipulated the source object and reload the link.
+        To change the tree structure of such an object you can change the original link target. But an explicit reload
+        ( ´load_links()´ ) is required to get the change active in the linked items.
 
-    Additionally a iTree object can contain:
+        Beside the linked item the user can add local items and mix them with the linked ones. But the general
+        structure is always determined by the linked in children.
 
-    * data - a iTData object to store any kind of python objects
+        Beside the subtree the ´iTree´-object can also contain a value. The value can be any type of Python objects
+        that is stored in the tree-node (comparable with the value of a dictionary). If it is required by the user to
+        calculate the hash
+        of the íTree´ via ´hash(item)´ some value objects might not be hashable and will raise an exception. But as long
+        as the objects can be pickled a hash replacement will be found in the hash of ´iTree´. E.g. a dict placed
+        as a value makes no troubles even if teh user likes to hash the tree.
 
-    * couple - you can couple the object to another one by giving a pointer
+        As a helper the ´iTree´-object can be coupled with other objects (which might be helpful if you have a displayed
+        tree in a GUI that is connected with the ´íTree´. Be aware that this helper function has only temporary
+        character.
+        It is not stored when dumping (standard dump) or considered in comparisons, etc. The coupled object is
+        ignored by all internal functionalities. Also in linked items the coupled object is not taken over from the link
+        and can be set independent.
 
-    * is_temporary - you can mark it as temporary. Those iTree items behave like normal ones. But they will not be
-      considered during encoding for storage, etc.
+        The behavior of a íTree´ object can be influenced by specific properties or flags:
 
-    There are different ways to access the children and sub-children in the tree of a iTree object.
+            * Read-only tree: An ´iTree´ object where the subtree is protected and cannot be changed
+            * Read-only value: An ´iTree´ object where the value is protected and cannot be changed
 
-    The standard access for single items is via itree_obj[] (__getitem__()) call.
+        The ´iTree´ object contains a large number of properties which should help the user to reach the
+        required information as comfortable as possible. Especially the tree related information might be interesting:
 
-    More complex access is available via find() and findall() methods. Have a look in the documentation
-    related to each method.
+            * mytree.tag -> family-tag of the item
+            * mytree.idx -> absolute index of the object
+            * mytree.tag_idx -> key tuple (family-tag, family-index)
+            * mytree.idx_path -> tuple of absolute indexes from the root to the item
+            * mytree.tag_idx_path -> tuple of key-tuples from the root to the item
+            * mytree.parent -> parent item of the item
+            * mytree.root -> root item of the item (highest level parent)
+            * mytree.pre_item -> pre item (the children in the parent that is before this item)
+            * mytree.post_item -> post item (the children in the parent that is after this item)
+            * mytree.level -> How deep the item is in the tree related to the root
+            * mytree.max_depth -> How deep the sub-items (nested) of the ´iTree´ go in maximum (deep levels)
 
-    The delivery of access related operations in the iTree objects is for unique targets an
-    iTree object and for multi target operations an iterator over the matching items. We don't deliver
-    something like a list.
+        In case the ´iTree´ object is not part of another ´iTree´ (is root) those attributes
+        will deliver in most cases ´None´.
 
-    If really needed an iterator can be easily converted into a list by list() method but this may take a long time
-    for huge iterators. The iterator should only be used in the final step of the operation. It's recommended to have
-    a look into itertools for better usage of the delivered iterators.
+            * mytree.is_root -> True in case the item is a root ´iTree´)no parent)
+            * mytree.is_tree_read_only -> True in case the subtree is protected and read-only
+            * mytree.is_value_read_only -> True in case the item value is protected and read-only
+            * mytree.is_linked -> True in case the item is a linked item (read_only)
+            * mytree.is_link_root-> True in case the item is a root for a link to another ´iTree´
+            * mytree.link_root-> Delivers the related link-root in case the item is linked
 
-    The design of the object is made to have best possible performance even that it is pure python.
-    For more details you may run the performance tests in the test section (But you might have to install
-    additional packages run the comparisons and to get the full picture.)
+            * mytree.value-> Delivers the value object stored in the ´iTree´ item
 
-    The function related to iterations iter; iter_children and find_all can be used with an item_filter. By this
-    mechanism you can create queries regarding any property in an iTree.
+        There are different ways to access the children and sub-children in the tree of a ´iTree´ object.
 
-    To initialize the class the following parameters are available
+        The standard access for single items is via ´itree_obj[target]´ ( ´__getitem__(target)´) call.
+        As targets the user has different options:
 
-    :param tag: tag string or hashable object used for the iTree identification
-    :param data: data dict or item to be stored in the node
-    :param subtree: The subtree is a iterable structure that contains sub-items (iTree objects) that should be \
-                    the children of this iTree.
+           * index - absolute target index integer (fastest operation)
+           * key - key tuple (family_tag, family_index)
+           * tag or tag sets- family_tag object targeting a whole family
+           * target-list - absolute indexes or keys to be replaced (indexes and keys can be mixed)
+           * index slice - slice of absolute indexes
+           * key slice - tuple of (family_tag, family_index_slice)
+           * filter-method - method to filtering specific children
 
-                    .. warning:: subtree: In case the given iTree objects have already a parent an implicit copy will
-                                          be made.
-    """
+        Beside the first level functions the `iTree`-object contains the helper class `.deep` which contains
+        the in-depth functionalities targeting all the nested sub-children of the object.
 
-    # we define some static private variables:
-    _is_read_only = False
-    _is_temporary = False
-    _is_placeholder = False
-    _is_linked = False
-    # make global local
-    _get_return = __GETITEM_RETURN__
-
-    __slots__ = ('_tag', '_parent', '_map', '_coupled', '_data', '_cache', '_def_serializer', '_link')
-
-    def __init__(self, tag, data=None, subtree=None):
-        super().__init__()
-
-        t = type(tag)
-        if (t is int) or (t is TagIdx):
-            raise TypeError('Given tag cannot be used in iTree wrong type (int or TagIdx)')
-        self._tag = tag
-        self._parent = None
-        self._map = None
-        self._link = None
-        self._coupled = None
-        self._cache = (0, 0)
-
-        if subtree is not None:
-            self._load_subtree(subtree)
-
-        if data is None:
-            self._data = iTData()
-        # elif hasattr(data,'is_iTData'):
-        elif isinstance(data, iTData):
-            self._data = data.__copy__()  # here we make an implicit copy!
-        else:
-            self._data = iTData(data)
-
-    def init_serializer(self, force=False, exporter=None, importer=None, serializer=None, renderer=None) -> None:
-        """
-        Method sets the exchange environment that should be used. If you leave the parameters as default,
-        the standard objects will be used.
-
-        .. note:: The method logic is called only one time the first time serializing is needed.
-
-        :param force: False (Default) - do not reload in case we have already loaded the items
-        :param exporter: exporter object for file export of iTree (dump, dumps)
-        :param importer: importer object in ces a file import is done (load, loads)
-        :param serializer: Object serializer (especially needed for data objects!)
-        :param renderer:  A renderer for pretty print output of the iTree object
+        As the name itertree should suggest a wide range of iteration methods are available in the class.
+        They can be combined with different kind of filters.
 
-        :return: None
-        """
-        # A post import must be done here against common python rules
-        # reason is that a pre import will lead into cyclic importing
+        .. _filter_method:
 
-        if (not hasattr(self, '_def_serializer')) or (self._def_serializer is None) or force:
-            if serializer is None:
-                from .itree_serialize import iTStdObjSerializer
-                serializer = iTStdObjSerializer
-            if exporter is None or importer is None:
-                from .itree_serialize import iTStdJSONSerializer
-                if exporter is None:
-                    exporter = iTStdJSONSerializer(obj_serializer=serializer())
-                if importer is None:
-                    importer = iTStdJSONSerializer(obj_serializer=serializer())
-            if renderer is None:
-                from .itree_serialize import iTStdRenderer
-                renderer = iTStdRenderer()
-            self._def_serializer = (exporter, importer, serializer, renderer)
-
-    def __setitem__(self, key, value):
-        """
-        put the item in the iTree for (re)setting a child
-
-        HINT: A iTree child can only be child of one iTree (one parent only)
-        HINT2: Linked items cannot be changed change the linked item and reload the tree!
+        .. note:: As optional `filter_method`-parameter the user can give:
 
-        :param key: single identifier for the item can be integer index or TagIdx
-        :param value: iTree object that should be child of called iTree
+                    * `None`- filter inactive
+                    * `Callable` delivering `True`/`False` related to a characteristic of the
+                      `ìTree`-object (iterated items)
 
-        :return: value
-        """
-        old_item = self.__getitem__(key)
-        try:
-            if value._parent is not None:
-                if value._parent == self:
-                    # check for __iadd__()
-                    if super().__getitem__(value.idx) is value:
-                        return None
-                if value._parent == old_item:
-                    # check for __iadd__()
-                    if old_item.__getitem__(value.idx) is value:
-                        return None
-                raise RecursionError('Given item has already a parent iTree!')
-        except AttributeError:
-            if type(value) is not iTree:
-                raise TypeError('In iTree only children of type iTree can be integrated')
-            raise
-        idx = old_item.idx
-        tag_idx = old_item.tag_idx
-        old_item._parent = None
-        o_tag = tag_idx[0]
-        value._parent = self
-        super().__setitem__(idx, value)
-        v_tag = value._tag
-        if v_tag == o_tag:
-            family = self._map[v_tag]
-            family.__setitem__(tag_idx[1], value)
-        else:
-            m = self._map
-            m[old_item._tag].remove(old_item)
-            try:
-                family = m.__getitem__(v_tag)
-                tag_idx = self.__get_family_insertion_idx(family, idx)
-                value._cache = (idx, tag_idx)
-                family.insert(tag_idx, value)
-            except (KeyError, IndexError):
-                m.__setitem__(v_tag, blist((value,)))
-        return value
+                  Beside this the internal filtering is normally a hierarchical filtering (If the parent does not match
+                  to the filter all children are excluded too, even that they match to the filter). Some methods contain
+                  a switch
+                  for non-hierarchical filtering too. But most often the non-hierarchical filtering can be realized via the
+                  build-in `filter()` method and in this case the switch is not available.
 
-    def __getitem__(self, key, str_index_separator='#'):
-        """
-        Main getter for items
+        Here the power of the iterators is obvious because cascaded filter queries can be constructed and finally in
+        only **one** full iteration over all the items is required to get the results back
+        (sometimes the full iteration is not required).
 
-        If given key targets to only one item we will deliver an iTree. If no matching item is found an IndexError
-        or KeyError exception will be raised.
+        It's recommended to have a look into itertools package  for better usage of the delivered iteration-generators.
 
-        If the given key targets to multiple items (tag family, slice, iterable of single target keys) and iterator
-        will be delivered.
+        The design of the ´iTree´´ object is made for best possible performance even that it is pure Python.
+        Some part of
+        the code might look less good readable or in the iteration-generators you find the if else outside the
+        iteration functionality which is not realized via sub-functions we have here redundant codings.
+        But its is made to avoid conditions or function calls inside the loops which would be bad for the performance.
 
-        .. node:: If a tag is given a iterator of the tag family will be returned even if there is only one item
-                  with the tag in the tree!!!
+        :type tag: Hashable
+        :param tag: family tag of the iTree object (any hashable object)
 
-        :param key: single target: index, TagIdx or tuple (tag, index) (not recommended)
-                    multi target: TagIdx_s; iMatch; slice or an iterable (like list) of these keys
-        :return: iTree item or iterator (multi target)
-        """
-        m = self._map
-        try:
-            if key in m:
-                # give iterator over whole family back
-                return iter(m.__getitem__(key))
-        except TypeError:
-            # we might have a slice!
-            pass
-        t = type(key)
-        if t is int:
-            return super().__getitem__(key)
-        try:
-            return self._get_return[t](self, key, str_index_separator)
-        except ValueError:
-            raise KeyError('Key %s not found in iTree' % repr(key))
+        :type value: object
+        :param value: value to be stored in the iTree object
 
-    def __delitem__(self, key):
-        """
-        delete an item in the tree
+        :type subtree: Optional[Iterable]
+        :param subtree: Iterable or Iterator containing the subtree items or an argument list (internal functionality)
 
-        :param key: key targeting the item to be deleted
-                    single target: iTree object (remove), index, TagIdx or tuple (tag, index) (not recommended)
-                    multi target: TagIdx_s or an iterable (like list) of these keys or a slice
+        :type link: Optional[iTLink]
+        :param link: iTLink object targeting another iTree
 
-        :return: deleted item
-        """
-        t = type(key)
-        m = self._map
-        if t is int:
-            del_item = super(iTree, self).pop(key)
-            family = m[del_item._tag]
-            if len(family) == 1:
-                del m[del_item._tag]
-            else:
-                del family[del_item.tag_idx[1]]
-            del_item._parent = None
-            return del_item
-        elif isinstance(key, TagIdx):
-            family = m[key[0]]
-            del_item = family.pop(key[1])
-            if len(family) == 0:
-                del m[del_item._tag]
-            # here we go for _delitem__ and not remove because we expect the item "knows" the correct index (cache)
-            super(iTree, self).__delitem__(del_item.idx)
-            del_item._parent = None
-            return del_item
-        elif t is TagMultiIdx:
-            idxs = key[1]
-            family = m[key[0]]
-            t2 = type(idxs)
-            if t2 is slice:
-                del_list = list(itertools.islice(family, idxs.start, idxs.stop, idxs.step))
-            elif t2 is list or hasattr(key, '__next__'):
-                del_list = [family[k] for k in key]
-            else:
-                raise TypeError('TagIdx_s object contains invalid indexes')
-            for i in del_list:
-                super().__delitem__(i.idx)
-                tag_idx = i.tag_idx
-                family = m[tag_idx.tag]
-                del_item = family.pop(tag_idx.idx)
-                if len(family) == 0:
-                    m.pop(tag_idx.tag)
-                del_item._parent = None
-            return iter(del_list)
-        elif isinstance(key, iTree):
-            idx = key.idx
-            super().__delitem__(idx)
-            tag_idx = key.tag_idx
-            family = m[tag_idx.tag]
-            del_item = family.pop(tag_idx.idx)
-            if len(family) == 0:
-                m.pop(tag_idx.tag)
-            del_item._parent = None
-            return del_item
-        else:
-            # family tag given?
-            try:
-                family = m.pop(key)
-                for item in family:
-                    super().remove(item)
-                    item._parent = None
-                return iter(family)
-            except KeyError:
-                # iterator or iterable given?
-                if hasattr(key, '__iter__') or hasattr(key, '__next__'):
-                    # return an iterator over the slice
-                    return_list = list(self[key])
-                    for i in return_list:
-                        super().__delitem__(i.idx)
-                        tag, tag_idx = i.tag_idx
-                        family = m[tag]
-                        del family[tag_idx]
-                        if len(family) == 0:
-                            del m[tag]
-                        i._parent = None
-                    return iter(return_list)
-                else:
-                    # no valid key found!
-                    raise KeyError('No related item (key = %s) found for deletion' % key)
+        :type flags: int
+        :param flags: flags taken from iTFLAG class:
 
-    def __mul__(self, factor):
-        """
-        Multiplication function a iTree is multiplied (copies) and put in a new iTree:
+                          * iTFLAG.READ_ONLY_TREE - mark the subtree of this iTree as read-only
+                            the subtree will be protected from changes in this case
 
-        my_single_item=iTree('multi')
-        multi=my_single_item*1000
+                          * iTFLAG.READ_ONLY_VALUE - mark the value of this iTree object as read-only
 
-        HINT: In this operation multiple copies of the original item generated.
+                          * iTFLAG.LOAD_LINKS - load the links during instance automatically
 
-        :param factor: integer to multiply with
-        :return: iTree object containing multiplied children
-        """
-        return iTree(self._tag, data=self._data, subtree=[self.__copy__() for _ in range(factor)])
+                      Multiple flags can be combined via `|`
 
-    def __add__(self, other):
         """
-        If two iTree objects are added the children in the two added iTrees are copied and combined
-        to a new iTree object the other attributes are taken over from the first iTree in the sum
-
-        :param other: iTree object that should be added
-        :return: New iTree object containing copies of all children
-        """
-        self.extend(other)
-        return self
+        # handle family tag:
+        if not tag.__hash__:
+            raise TypeError('Given tag is not hashable')
+        self._tag = tag
 
-    def __iadd__(self, other):
-        try:
-            if other._parent is not None:
-                raise RecursionError('Given item has already a parent iTree!')
-        except AttributeError:
-            if type(other) is not iTree:
-                raise TypeError('In iTree only children of type iTree can be integrated')
-            raise
-        self + [other]
-        return self
+        # set data value
+        self._value = value
 
-    def __iter__(self, item_filter=None):
-        """
-        standard iterator over all items in the iTree
-        :param item_filter: ALL = default
-        :return:
-        """
-        return self.iter_children(item_filter=item_filter)
+        # flags
+        if flags:
+            self._flags = flags = flags & self._FLAG_MASK
+        else:
+            self._flags = 0
+
+        # _itree_prt_idx
+        # 1. hasattr((o,'_itree_prt_idx') -> Used for class/object identification ->
+        # 2. o._iter_parent is None -> iTree-object is not part of a parent iTree
+        # 3. o._itree_prt_idx is list -> iTree-object is part of a iTree
+        # list: [parent_itree_object, absolute_index_cache, family_index]
+        #   a. o._itree_prt_idx[0] -> iTree parent-object
+        #   b. o._itree_prt_idx[1] -> cached absolute index in iTree parent-object (might be outdated!)
+        #   c. o._itree_prt_idx[3] -> cached family index in iTree parent-object (might be outdated!)
+        self._itree_prt_idx = None
+        self.get = getitem = _iTreeGetitem(self)
+
+        # internals like self._families are created only in case elements added to the object
+
+        # load the subtree
+        if subtree:
+            # we only mask out the flags that should be brought into the deeper levels!
+            if flags:
+                sl = list(self._iter_extend(self, subtree, flags & self._DEEP_FLAG_MASK, init=True))
+            else:
+                sl = list(self._iter_extend(self, subtree, init=True))
+            self._items = sl = itree_list(sl)
+        else:
+            self._items = sl = []
+        self.getitem_by_idx = getitem.getitem_by_idx = sl.__getitem__
+        self.__len__, self.__iter__ = sl.__len__, sl.__iter__
+
+        # links
+        if link:
+            t = type(link)
+            if t is iTLink:
+                # we create a new object -> to be sure that we have a virgin iTLink-object
+                link = link.get_args()
+            elif t is tuple and len(link) > 4:
+                raise TypeError('Given link %s not supported!' % repr(link))
+            self._link = iTLink(*link)
+            self._flags = self._flags | self._LINK_ROOT
+            # load links
+            if flags & self._LOAD_LINKS:
+                self.load_links()
 
-    def __contains__(self, item):
-        """
-        checks if an iTree object is part of the iTree
-        :param item: iTree object we searching for
-        :return:
-        """
-        if id(item._parent) == id(self):
-            return True
-        if item._parent is None:
-            return False
-        return item._parent in self
+    # *** parent related properties and methods ************************************************************************
 
-    def __eq__(self, other):
-        """
-        A iTree object is always unique we test therefore just for matching object IDs
-        This is needed for quick index findings!
-        ..node:: To check if properties content is equal use equal() instead
-        :param other: iTree object to compare with
-        :return:
+    @property
+    def parent(self):
         """
-        return id(self) == id(other)
+        Property delivers current items parent-object.
 
-    def __ne__(self, other):
+        :rtype: Union[iTree, None]
+        :return: iTree parent-object or None (in case no parent exists)
         """
-        A iTree object is always unique we test therefore just for object for not matching IDs
-        This is needed for quick index findings!
-        ..node:: To check if attribute content is equal use not equal() instead
-        :param other: other item to be compared with
-        :return: True/False
-        """
-        if id(self) != id(other):
-            return True
-        return False
+        # Implementation state: ready, tested, doc ok
+        return self._itree_prt_idx[0] if self._itree_prt_idx else None
 
-    def __lt__(self, other):
-        """
-        less than is a size comparison (length are compared)
-        :param other: iTree object self should be compared with
-        :return: True/False
+    @property
+    def is_root(self):
         """
-        return len(self) < len(other)
+        Is this item a root-item (has no parent)?
 
-    def __le__(self, other):
-        """
-        less than or equal is a size comparison (length are compared)
-        :param other: iTree object self should be compared with
-        :return: True/False
+        :rtype: bool
+        :return:
+                * *True* - is root
+                * *False* - is not root
         """
-        return len(self) <= len(other)
+        # Implementation state: ready, tested, doc ok
+        return self._itree_prt_idx is None
 
-    def __gt__(self, other):
-        """
-        greater than is a size comparison (length are compared)
-        :param other: iTree object self should be compared with
-        :return: True/False
+    @property
+    def root(self):
         """
-        return len(self) > len(other)
+        property delivers the root-item of the tree
 
-    def __ge__(self, other):
-        """
-        greater than or equal is a size comparison (length are compared)
-        :param other: iTree object self should be compared with
-        :return: True/False
-        """
-        return len(self) >= len(other)
+        In case the item has no parent it will deliver itself
 
-    def __repr__(self):
-        """
-        create representation string from which the object can be reconstructed via eval (might not work in case of
-        data that do not have a working repr method)
-        :return: representation string
+        :rtype: iTree
+        :return: iTree root item
         """
-        repr_str = '%s(%s' % (self.__class__.__name__,repr(self._tag))
-        if not self._data.is_empty:
-            if self._data.is_no_key_only:
-                repr_str = repr_str + ', data=%s' % repr(self.d_get())
-            else:
-                repr_str = repr_str + ', data=%s' % repr(self._data)
-        subtree = super(iTree, self).__repr__()
-        if subtree[0] == 'b':
-            # we shorten blist from definition
-            subtree = subtree[6:-1]
-            return repr_str + ', subtree=%s)' % subtree
-        else:
-            return repr_str + ')'
+        # Implementation state: ready, tested, doc ok
+        p = self
+        while p is not None:
+            root, p = p, p.parent
+        return root
 
-    def __hash__(self):
-        """
-        The hash operation is available but not a quick operation!
-        ..node::: We do here not consider, parent and coupled item
-        :return: integer hash
+    @property
+    def tag(self):
         """
-        return hash((tuple(self.iter_children()), (self._tag, self._data)))
-
-    def __len__(self):
-        return super(iTree, self).__len__()
-
-    # unsupported operands
-    def __sub__(self, other):
-        return self.__unsupport_op(other)
-
-    def __isub__(self, other):
-        return self.__unsupport_op(other)
-
-    def __imul__(self, other):
-        return self.__unsupport_op(other)
+        This is the access to the object-tag. The tag gives the relation to the tag-family in `iTree`-objects.
 
-    def __rmul__(self, other):
-        return self.__unsupport_op(other)
+        The tag is comparable with a key in dictionaries but in iTrees the tag is not unique! For unique iTree
+        identification the `tag_idx` property must be used.
 
-    def __reversed__(self):
-        return self.__unsupport_op()
+        Any hashable object can be used as a tag, but in case "exotic" objects are used and serialization is required
+        the user may have to extend the functionality of the serializer.
 
-    def __reduce__(self):
-        return self.__unsupport_op()
+        :rtype: Hashable
 
-    def __reduce_ex__(self, protocol):
-        return self.__unsupport_op()
+        :return: tag - hashable object giving the family relation
 
-    def sort(self, *arg, **kwargs):
         """
-        sort operation is not supported, method exists just because super class supports it.
-        Here a TypeError will be raised.
-        """
-        return self.__unsupport_op()
-
-    # properties
+        # Implementation state: ready, tested, doc ok
+        return self._tag
 
     @property
-    def data(self):
+    def idx(self):
         """
-        delivers the data-attribute object of the item
+        Index of this object in the iTree (related to the absolute order)
 
-        :return: data object of the item
-        """
-        return self._data
+        *Method is very important for internal functionalities*
 
-    # These are the mandatory methods we expect in the data object
+        .. note::
+            In general the item index is cached but in case of deleted items or reorder operations
+            the cache might be outdated. In this case the index update based on a search might take longer.
+
+        :rtype: Union[int, None]
+        :return: unsigned integer representing the index (related to absolute order of iTree)
+        """
+        # Implementation state: ready, tested, doc ok
+        parent_list = self._itree_prt_idx
+        if parent_list:
+            parent, abs_idx, _ = parent_list
+            siblings = parent._items
+            # create locals for multi use functions
+            size = len(siblings)
+            if abs_idx < size and siblings[abs_idx] is self:
+                # cache matches
+                return abs_idx
+            # cache index must be updated
+            # search in near area
+            delta = 20
+            limit = min(size, abs_idx + delta + 1)
+            start = max(0, abs_idx - delta)
+            for i in range(start, limit):
+                if siblings[i] is self:
+                    parent_list[1] = i
+                    return i
+            if abs_idx < size / 2:
+                # start -> end
+                i = 0
+                for item in siblings:
+                    item._itree_prt_idx.__setitem__(1, i)
+                    if item is self:
+                        return i
+                    i = i + 1
+                raise IndexError('Internal error for this iTree we found no related index in the parent-object!')
+            else:
+                # end -> start
+                for i in range((size - 1), -1, -1):
+                    item = siblings[i]
+                    item._itree_prt_idx.__setitem__(1, i)
+                    if item is self:
+                        return i
+                raise IndexError('Internal error for this iTree we found no related index in the parent-object!')
 
-    def d_set(self, *args, **kwargs):
+    @property
+    def idx_path(self):
         """
-        set function for a data-attribute
+        delivers a list of absolute indexes from the root to this item
 
-        In case the standard iTData object is used we have:
+        For items with no parent (root_item) an empty tuple will be delivered
 
-        :param key: give key under which the data will be stored, in case data is None the first key parameter is taken
-                    as data object and it is stored in the "__NOKEY__" item
+        .. note::
+                We deliver here a tuple because it might be helpful if the object is hashable
+                (usage as a dict key)
 
-        :param value: data value the object that should be stored in the data structure of this iTree
+        :rtype: tuple
+        :return: tuple of index integers (here we do not deliver an iterator!)
 
-        :return:  None
         """
-        return self._data.__setitem__(*args, **kwargs)
+        # Implementation state: ready, tested, doc ok
+        p = self
+        idx_list = deque()
+        while 1:
+            root, p = p, p.parent
+            if p is None:
+                break
+            else:
+                idx_list.appendleft(root.idx)
+        return tuple(idx_list)
 
-    def d_get(self, key=__NOKEY__,return_type=VALUE):
+    @property
+    def tag_idx(self):
         """
-        get function for a data attribute
-
-        In case the standard iTData object is used we have:
+        The tag_idx is a unique identification of the item. It is represented by a tuple containing the family-tag
+        and the family related index of the item.
 
-        :param key: key under which the data is stored, in case no key is given the "__NOKEY__" item will be returned
+        If  the item is not part of a parent-tree (root-item) in this case the result will be `None`.
 
-        :return: data attribute object
+        :rtype: Union[tuple, None]
+        :return: tuple (family-tag, family-index) or None (if item has no parent)
         """
-        return self._data.__getitem__(key,return_type)
+        parent_list = self._itree_prt_idx
+        if parent_list:
+            parent = parent_list[0]
+            getitem_fams = parent._getitem_fam
+            tag = self._tag
+            # we use cached index to be quicker
+            family_idx = parent_list[2]
+            family = getitem_fams(tag)
+            fm_getitem = family.__getitem__
+            size = family.__len__()
+            if family_idx < size and fm_getitem(family_idx) is self:
+                return tag, family_idx
+
+            delta = 20
+
+            limit = min(size, family_idx + delta + 1)
+            start = max(0, family_idx - delta)
+            for i in range(start, limit):
+                if fm_getitem(i) is self:
+                    parent_list[2] = i
+                    return tag, i
+
+            # update the whole list
+            if family_idx < size / 2:
+                # start -> end
+                i = 0
+                for item in family:
+                    item._itree_prt_idx.__setitem__(2, i)
+                    if item is self:
+                        return i
+                    i = i + 1
+                raise IndexError('Internal error for this iTree we found no related index in the parent-object!')
+            else:
+                # end -> start
+                for i in range((size - 1), -1, -1):
+                    item = family[i]
+                    item._itree_prt_idx.__setitem__(2, i)
+                    if item is self:
+                        return i
+                raise IndexError('Internal error for this iTree we found no related index in the parent-object!')
 
-    def d_update(self, *args, **kwargs):
+    @property
+    def tag_idx_path(self):
         """
-        update function data-attribute
+        The path is a tuple of tag_idx tuples from root to this item.
+        Each tag_idx is a tuple containing the pair family-tag and family-index.
 
-        In case the standard iTData object is used we have:
+        For items with no parent (rooot_item) an empty tuple will be delivered
 
-        :param key: give key under which the data will be stored, in case data is None the first key parameter is taken
-                    as data object and it is stored in the "__NOKEY__" item
+        .. note::
+                    We deliver here a tuple because it might be helpful if the object is hashable
+                    (usage as a dict key)
 
-        :param value: data value the object that should be stored in the data structure of this iTree
+        :rtype: tuple
+        :return: tuple of key tuples containing family-tag and family-index
 
-        :return:  None
         """
-        return self._data.update(*args, **kwargs)
+        # Implementation state: ready, tested, doc ok
 
-    def d_check(self, value,key=__NOKEY__):
-        """
-        check if the given data-item can be stored under the given key. The check make only sense in case there is
-        a iTreeDataModel or matching object is already stored under the key
+        p = self
+        key_list = deque()
+        while 1:
+            root, p = p, p.parent
+            if p is None:
+                break
+            else:
+                key_list.appendleft(root.tag_idx)
+        return tuple(key_list)
 
-        :exception:  check will raise an iDataValueError or  iDataTypeError exception in case the value is not matching
-                     in case given key is not found a KeyError will be raised
+    def force_cache_update(self, idx=True, fam_keys=True, all_keys=True):
+        """
+        Forces the update of the index and keys in cache
 
-        :param value: data value the object that should be checked
+        Normally this is not required the methode is mainly used for testing proposes
 
-        :param key: give key under which contains the DataModel, in case key is not given the "__NOKEY__" item will be used
+        :param idx: True - update absolute-indexes
 
-        :return: valid value
-        """
-        try:
-            value=self._data.__getitem__(key=key, _return_type=FULL).validator(value)
-        except AttributeError:
-            pass
-        except KeyError:
-            if key!=__NOKEY__:
-                raise
-        return value
+        :param fam_keys: True - update this items family-indexes
 
-    def d_pop(self, *args, **kwargs):
-        """
-        data related pop (will delete the given key from data-attribute)
+        :param all_keys: True - update all families faimily-indexes
 
-        :return: deleted value
         """
-        return self._data.pop(*args, **kwargs)
+        parent_list = self._itree_prt_idx
+        if parent_list:
+            parent = parent_list[0]
+            if idx:
+                list(item._itree_prt_idx.__setitem__(1, i) for i, item in enumerate(parent))
+            if fam_keys and not all_keys:
+                family = self._getitem_fam(self._tag)
+                list(item._itree_prt_idx.__setitem__(2, i) for i, item in enumerate(family))
+            elif all_keys:
+                for family in parent._families.values():
+                    list(item._itree_prt_idx.__setitem__(2, i) for i, item in enumerate(family))
 
-    def d_del(self, *args, **kwargs):
+    @property
+    def pre_item(self):
         """
-        data related del (will delete the given key)
+        Delivers the pre-item (predecessor) of this object in the parent-tree.
+        If self is first item or there is no parent `None` will be delivered.
 
-        :return: deleted value
+        :rtype: Union[iTree,None]
+        :return: iTree predecessor or None (no match)
         """
-        return self._data.__delitem__(*args, **kwargs)
+        # Implementation state: ready, tested, doc ok
+        if self._itree_prt_idx is None:
+            return None
+        idx = self.idx - 1
+        return None if idx < 0 else self._itree_prt_idx[0]._items.__getitem__(idx)
 
     @property
-    def parent(self):
+    def post_item(self):
         """
-        property contains the parent item
 
-        :return: iTree parent object (or None in case no parent exists)
+        Delivers the post-item (successor) of this object in the parent-tree.
+        If self is first item or there is no parent `None` will be delivered.
+
+        :rtype: Union[iTree,None]
+        :return: `iTree` successor or `None` (no match)
         """
-        return self._parent
+        # Implementation state: ready, tested, doc ok
+        if self._itree_prt_idx is None:
+            return None
+        idx = self.idx + 1
+        sl = self._itree_prt_idx[0]._items
+        return sl.__getitem__(idx) if idx < sl.__len__() else None
 
     @property
-    def is_root(self):
+    def level(self):
         """
-        is this item a root item (has no parent)
+        Delivers the distance (number of levels) to the root-item of the tree. Or in other words how
+        deep in tree the item is positioned.
+        In case item has no parent (is a root-item) this method will deliver 0.
 
-        :return: True/False
+        :rtype: int
+        :return: integer - number of levels (outer direction)
         """
-        return self._parent is None
+        # Implementation state: ready, tested, doc ok
+        i = 0
+        pt = self._itree_prt_idx
+        while (pt):
+            p = pt[0]
+            i = i + 1
+            pt = p._itree_prt_idx
+        return i
 
     @property
-    def root(self):
+    def max_depth(self):
         """
-        property delivers the root item of the tree
+        Relative from this item the method measures the maximum depth of the tree and delivers
+        the maximum number of levels that are found in this object.
 
-        :return: iTree root item
+        If the user wants to now the maximum depth of the whole tree ensure that the property of the root-item is read.
+        The user might use `my_tree.root.max_depth` to ensure this.
+
+        :rtype: int
+
+        :return: integer maximal number of levels that exists in the tree (inner direction)
         """
-        # We use an iterative not recursive solution here because we allow tree depth > recursion limit of the
-        # interpreter!
-        p = self
+        # Implementation state: ready, tested, doc ok
+        if not self:
+            return 0
+        max_depth = 0
+        items = [self]
         while 1:
-            p1 = p._parent
-            if p1 is None:
-                return p
-            p = p1
+            new_items = []
+            deque((new_items.extend(list(i)) for i in items), maxlen=0)
+            if len(items) == 0:
+                break
+            else:
+                max_depth += 1
+            items = new_items
+        return max_depth - 1
 
     @property
-    def is_read_only(self):
+    def tag_number(self):
         """
-        In contrast to iTreeReadOnly class this is False
-
-        :return: False
+        property contains the number of tags (families) the itree contains
+        :return: integer
         """
-        return self._is_read_only
+        if self:
+            return len(self._families)
+        else:
+            return 0
+
+    # *** properties targeting internal sub/helper classes *************************************************************
 
     @property
-    def is_temporary(self):
+    def deep(self):
         """
-        In contrast to iTreeTemporary class this is False
-
-        :return: False
+        Subclass containing the deep access to the nested structures of iTree
+        :return:
         """
-        return self._is_temporary
+        try:
+            return self._hc_tree
+        except AttributeError:
+            # The subclass is only instanced if it is first used
+            tree, tree._itree, tree.get = _iTreeIndepthTree(), self, self.get
+            self._hc_tree = tree
+            return tree
+
+    # flags
 
     @property
-    def is_placeholder(self):
+    def flags(self):
         """
-        In contrast to iTreePlaceholder class this is False
+        Give the flags value of the object. The integer value stored in this property contains the bit flags
+        related to the constants iTFLAG or _iTFLAG.
 
-        :return: False
-        """
-        return self._is_placeholder
+        To see the details the user might use `bin()` or the helper property `flags_repr` which delivers a
+        string containing all set flags.
 
-    @property
-    def is_linked(self):
+        ;rtype: int
+        :return: The flags set for this item
         """
-        In contrast to iTreeLinked class this is False
+        # Implementation state: ready, tested, doc ok
+        return self._flags
 
-        :return: False
+    def flags_repr(self, public_only=True):
         """
-        return self._is_linked
+        String representation of flags for this item
 
-    @property
-    def link_item(self):
-        """
-        in case we have "covered" a linked item this property delivers the original linked item
-        (mainly for internal use)
+        :type public_only: bool
+        :param public_only:
+                        * True - Consider only the public flags (given by the user) -> default
+                        * False - Show all flags (also linked and placeholder flags)
 
-        :return: None - no linked item
-                 iTreeLink object the covered item
+        ;rtype: str
+        :return: String repr of the flags set for this item
         """
-        if self._link is not None:
-            return self._link.link_item
-        return None
+        # Implementation state: ready, partly tested, doc ok
+        out = []
+        if self._flags & self._READ_ONLY_TREE != 0:
+            out.extend(('iTFLAG.READ_ONLY_TREE', '|'))
+        if self._flags & self._READ_ONLY_VALUE != 0:
+            out.extend(('iTFLAG.READ_ONLY_VALUE', '|'))
+
+        if self._flags & self._LOAD_LINKS != 0:
+            out.extend(('iTFLAG.LOAD_LINKS', '|'))
+        if not public_only:
+            if self._flags & self._LINKED != 0:
+                out.extend(('_iTFLAG.LINKED', '|'))
+            if self._flags & self._LINK_ROOT != 0:
+                out.extend(('_iTFLAG.LINK_ROOT', '|'))
+            if self._flags & self._PLACEHOLDER != 0:
+                out.extend(('_iTFLAG.PLACEHOLDER', '|'))
+        return ''.join(out).rstrip('|')
 
     @property
-    def pre_item(self):
+    def is_tree_read_only(self):
         """
-        delivers the pre item (predecessor) of this object
+        Is the tree protection flag set? In this case the tree structure cannot be changed
 
-        :return: iTree predecessor or None (no match)
-        """
-        idx = self.idx - 1
-        if idx < 0:
-            return None
-        return super(iTree, self._parent).__getitem__(idx)
+        This property targets the tree structure not the value!
 
-    @property
-    def post_item(self):
+        :rtype: bool
+        :return:
+                * False - subtree can be changed (writeable)
+                * True -  subtree is protected (read-only)
         """
-        delivers the post item (successor)
+        # Implementation state: ready, tested, doc ok
+        return bool(self._flags & (self._READ_ONLY_TREE | self._LINKED))
 
-        :return: iTree successor or None (no match)
+    def set_tree_read_only(self):
         """
-        idx = self.idx + 1
-        sl = super(iTree, self._parent)
-        if idx < sl.__len__():
-            return sl.__getitem__(idx)
-        return None
+        Set the tree protection flag. If the flag is set the subtree structure can not be changed anymore.
 
-    @property
-    def _a_debug_children_list(self):
+        .. Warning:: Setting the structural protection is always a deep operation. In all children and sub-children
+                     the protection flag will be activated too! But when unset the behavior it is not automatically
+                     made as a deep operation`. Here the differentiation in between the two methods
+                     `unset_tree_read_only()` and `unset_tree_read_only_deep()` exists.
         """
-        This is a property for debugging only do not use for manipulations!
+        # Implementation state: ready, tested, doc ok
+        if self._flags & self._LINKED:
+            _iTreePrivate._raise_read_only_exception(self)
+        set_flags = _iTreePrivate._set_flags
+        read_only_tree_flag = self._READ_ONLY_TREE
+        set_flags(self, read_only_tree_flag)
+        for i in self.deep:
+            set_flags(i, read_only_tree_flag)
 
-        :return: list of children
+    def unset_tree_read_only(self):
         """
-        return list(self.iter_children())
+        Unset the tree protection flag on the item. Only the children structure of this item is made
+        writable by this operation.
 
-    @property
-    def _a_debug_children_map(self):
+        :except: If the parent contains the tree protection flag a PermissionError will be raised
         """
-        This is a property for debugging only do not use for manipulations!
+        # Implementation state: ready, tested, doc ok
+        if self._itree_prt_idx is not None and self._itree_prt_idx[0]._flags & self._READ_ONLY_TREE:
+            raise PermissionError('The structural protection flag can only be unset in '
+                                  'case the parent is not protected. But here the parent holds the protection flag')
 
-        :return: dict of children
-        """
-        return self._map
+        self._unset_flags(self, self._READ_ONLY_TREE)
 
     @property
-    def depth_up(self):
+    def is_value_read_only(self):
         """
-        delivers the distance (number of levels) to the root element of the tree
+        Is iTree value read_only? Is the value protection flag iTFLAG.READ_ONLY_VALUE is set?
 
-        :return: integer
+        :rtype: bool
+        :return:
+                True - read-only protection of value active
+                False - value is writeable
         """
-        # We use an iterative not recursive solution here because we allow tree depth > recursion limit of the
-        # interpreter!
-        p = self
-        i = 0
-        while 1:
-            p = p._parent
-            if p is None:
-                return i
-            i += 1
+        # Implementation state: ready, tested, doc ok
 
-    @property
-    def max_depth_down(self):
-        """
-        delivers the max_depth in the direction of the children
+        return bool(self._flags & (self._READ_ONLY_VALUE | self._LINKED))
 
-        :return: integer maximal children depth
+    def set_value_read_only(self):
         """
-        if self.__len__() == 0:
-            return 0
-        max_depth = 0
-        items = [self]
-        while 1:
-            new_items = []
-            deque((new_items.extend(list(i.iter_children())) for i in items), maxlen=0)
-            if len(items) == 0:
-                break
-            else:
-                max_depth += 1
-            items = new_items
-        return max_depth - 1
-
-    @property
-    def idx_path(self):
+        Set the write protection of the value (set flag: iTFLAG.READ_ONLY_VALUE)
         """
-        delivers the a list of indexes from the root to this item
+        # Implementation state: ready, tested, doc ok
 
-        :return: list of index integers (here we do not deliver an iterator)
-        """
-        # We use an iterative not recursive solution here because we allow tree depth > recursion limit of the
-        # interpreter!
-        p = self
-        idx_list = []
-        while 1:
-            if p is None:
-                return idx_list
-            idx = p.idx
-            if idx is None:
-                break
-            idx_list.insert(0, idx)
-            p = p._parent
-        return idx_list
+        self._set_flags(self, self._READ_ONLY_VALUE)
 
-    @property
-    def tag_idx_path(self):
+    def unset_value_read_only(self):
         """
-        delivers the a list of TagIdx objects from the root to this item
-
-        :return: list of TagIdx (here we do not deliver an iterator)
+        Unset the write protection flag of the value (set flag: iTFLAG.READ_ONLY_VALUE).
+        Value will be writeable afterwards
         """
-        # We use an iterative not recursive solution here because we allow tree depth > recursion limit of the
-        # interpreter!
-        p = self
-        idx_list = []
-        while 1:
-            tag_idx = p.tag_idx
-            if tag_idx is None:
-                return idx_list
-            idx_list.insert(0, tag_idx)
-            p = p._parent
+        # Implementation state: ready, tested, doc ok
 
-    @property
-    def tag_idx(self):
-        """
-        Get the TagIdx object related to this object
-        (contains the tag and the index of the object in the tag-family)
+        if self._flags & self._LINKED:
+            _iTreePrivate._raise_read_only_exception(self)
+        self._unset_flags(self, self._READ_ONLY_VALUE)
 
-        :return: TagIdx
-        """
-        parent = self.parent
-        if parent is None:
-            return None
-        # we use cached index to be quicker
-        cache = self._cache
-        c_idx = cache[1]
-        family = parent._map[self._tag]
-        try:
-            if family[c_idx] is self:
-                return TagIdx(self._tag, c_idx)
-        except IndexError:
-            pass
-        # full search cached index must be updated
-        idx = parent._map[self._tag].index(self)
-        self._cache = (cache[0], idx)
-        return TagIdx(self._tag, idx)
+    # *** value and coupled object related properties/methods **********************************************************
 
     @property
-    def tag(self):
+    def value(self):
         """
-        This objects tag
+        Delivers the full value object stored in the `iTree`-object
 
-        :return: tag object
+        :rtype: object
+        :return: value-object of the item
         """
-        return self._tag
+        # Implementation state: ready, tested, doc ok
+        return self._value
 
-    @property
-    def idx(self):
+    def set_value(self, value):
         """
-        Index of this object in the iTree
+        Set/replace the value content of the `iTree`-object.
 
-        :return: integer index
-        """
-        parent = self._parent
-        if parent is None:
-            return None
-        # we use cached index to be quicker
-        cache = self._cache
-        sl = super(iTree, parent)  # do not delete parameters here!
-        c_idx = cache[0]
-        try:
-            if sl.__getitem__(c_idx) is self:
-                return c_idx
-        except IndexError:
-            pass
-        # cached index must be updated
-        idx = sl.index(self)
-        self._cache = (idx, cache[1])
-        return idx
+        The method returns the previous stored value object that was replaced by the operation.
 
-    @property
-    def coupled_object(self):
-        """
-        The iTree object can be couple with another python object. The pointer to the object is stored and can be
-        reached via this property. (E.g. this can be helpful when connecting the iTree with a visual element
-        (tree-list item) in a GUI)
+        .. note:: If an `iTValueModel` is stored as value in the `iTree` by default the set_value() method will
+                  target the value which is stored inside the model. If the model itself should be exchanged the
+                  user must
+                  give the new model as value parameter of this method. To replace the model with another Python
+                  object the user must first delete the model via `del_value()` command and afterwards set the new value.
 
-        :return: pointer to coupled object
-        """
-        try:
-            return self._coupled
-        except AttributeError:
-            return None
+        :type value: object
+        :param value: data-object that should be placed as value or in case we
+                      have a `iTValueModel` already as value it is placed inside the model.
 
-    # set properties
-    def set_coupled_object(self, coupled_object):
+        :rtype: object
+        :return: old value object that was stored in iTree before
         """
-        User can couple this object with others with the help of this attribute
-        .. note:: E.g. this might be an object in a GUI that are related to this item
+        # Implementation state: ready, tested, doc ok
+        if self._flags & self._IS_VALUE_PROTECTED:
+            raise PermissionError('iTree value is read only')
+        old_value = self._value
+        # do we have a model?
+        if (
+                hasattr(old_value, 'is_iTValueModel')
+                and hasattr(value, 'is_iTValueModel')
+                or not hasattr(old_value, 'is_iTValueModel')
+        ):
+            # new model given!
+            self._value = value
+        else:
+            old_value = old_value.set(value)
+        return old_value
 
-        :param couple_object: object pointer to the object that should be coupled with this iTree item
+    def set_key_value(self, key, value):
         """
-        self._coupled = coupled_object
+        Depending on the already stored object this operation is a sub-replacement of a part only.
 
+        The method returns the previous stored value object that was replaced by the operation.
 
-    def equal(self, other, check_parent=False, check_coupled=False):
-        """
-        compares if the data content of another item matches with this item
+        The user can influence the behavior by giving the `key` parameter. And it depends on the already
+        stored value object (e.g. a `list` or `dict` ). Only the value of the related
+        item will be replaced or in case the item did not exist yet the might object will be extended by the
+        given value ( `dict` only).
 
-        :param other: other iTree
+        Depending on given key parameter and the already stored object we have the following possible behaviours:
 
-        :param check_parent: check if item has same parent object too? (Default False)
+            * dict stored in value -> store the value in the dict with the key given in key_index
+            * dict stored in value and matching item-value is a `iTValueModel` -> replace value inside the model
+            * list stored in value -> key_index must be an index and replace the related item in the list with the
+              value given
+            * list stored in value and matching (index) item-value is a `iTValueModel` -> replace value inside the model
+            * key == `INF` and list stored in value -> append given value in the list
 
-        :param check_coupled: check the couple object too? (Default False)
+        .. note:: If an `iTValueModel` is stored as value in the `iTree` by default the `mytree.set_value()`-method will
+                  target the value which is stored inside the model. If the model itself should be exchanged
+                  the user must give a new model as value parameter of this method. To replace the model with another
+                  Python object the user must first delete the model via `del mytree.value[key]` command and afterwards
+                  set the new value or he sets  the value directly via `mytree.value[key]==new_value` .
 
-        :return: boolean match result (True match/False no match)
+        :type key: Optional[Hashable,int]
+        :param key: key or index of the value object (depends on the object already stored in `iTree` ).
+                    if `key==INF` the value will be appended in case a list-like object is already
+                    stored in the `iTree`-object.
+
+        :type value: object,
+        :param value: value object that should be placed as value or in case a key is given the sub-value in
+                      the `iTree`
+                      or in case we have a `iTValueModel` is used inside the model.
+
+
+        :rtype: object
+        :return: old value object that was stored in iTree before
         """
-        if self == other:
-            return True
-        if type(other) is not iTree:
-            return False
-        if check_parent:
-            if other._parent != self._parent:
-                return False
-        if self._map is None:
-            l1 = 0
-            if other._map is not None:
-                return False
-            l2 = 0
+        # Implementation state: ready, tested, doc ok
+        if self._flags & self._IS_VALUE_PROTECTED:
+            raise PermissionError('iTree value is read only')
+        old_value = self._value
+        try:
+            old_value = old_value[key]
+        except KeyError:
+            old_value[key] = value
+            return NoValue
+        except TypeError:
+            if key == INF:
+                old_value.append(value)
+                return NoValue
+            raise
+        # do we have a model?
+        if (
+                hasattr(old_value, 'is_iTValueModel')
+                and hasattr(value, 'is_iTValueModel')
+                or not hasattr(old_value, 'is_iTValueModel')
+        ):
+            # new model given!
+            self._value[key] = value
         else:
-            l1 = len(self._map)
-            l2 = len(other._map)
-        my_data = (self._tag, super(iTree, self).__len__(), l1)
-        other_data = (other._tag, super(iTree, other).__len__(), l2)
-        if my_data != other_data:
-            return False
-        for si, oi in zip(other.iter_children(), self.iter_children()):
-            if not si.equal(oi):
-                return False
-        if check_coupled:
-            try:
-                if self._coupled != other._coupled:
-                    return False
-            except AttributeError:
-                if hasattr(self, '_coupled'):
-                    return False
-                if hasattr(other, '_coupled'):
-                    return False
-        return True
+            old_value = old_value.set(value)
+        return old_value
 
-    def __copy__(self):
+    def get_value(self):
         """
-        create a copy of this item
+        Delivers the value-object of the item or a sub-value in case key_index parameter is used and a
+        matching object is stored in the `iTree` .
 
-        The difference in between copy and deepcopy for iTree is just that we do in deepcopy a copy
-        of all data items too. In copy we just copy the iTData object not the items itself, they stay as pointers
-        to the original objects.
+        .. note:: If `iTValueModel` is stored in `iTree` the method will not target the model it will
+                  target the value inside. If the model itself is required the `value`-property of `iTree` must be used.
 
-        The function is used internally in extend operations too. And we can see (profiler) that
-        improvements in this method might have big impact.
+        :except: In case a key_index is given but the object is not a `dict` or a `list` like object an `AttributeError`
+                 will be raised ( `__getitem__()`required). If no matching item is found an
+                 `IndexError` or `KeyError` will be raised.
 
-        :return: copied iTree object
+        :rtype: object
+        :return: value object the `iTree` or `iTValueModel` (in case a model is stored in the `iTree` )
         """
-        new = self.__class__(self._tag,
-                    data=self._data.__copy__(),
-                    subtree=[i.__copy__() for i in super(iTree, self).__iter__()]
-                    # here we create a recursion -> subtree is copied!!
-                    )
+        # Implementation state: ready, tested, doc ok
+        value = self._value
+        return value.value if hasattr(value, 'is_iTValueModel') else value
 
-        return new
-
-    def copy(self, *args, **kwargs):
+    def get_key_value(self, key):
         """
-        create a copy of this item
+        Delivers the value-object of the item or a sub-value in case key_index parameter is used and a
+        matching object is stored in the `iTree` .
 
-        The difference in between copy and deepcopy for iTree is just that we do in deepcopy a copy
-        of all data items too. In copy we just copy the iTData object not the items itself, they stay as pointers
-        to the original objects.
 
-        The function is used internally in extend operations too. And we can see (profiler) that
-        improvements in this method might have big impact.
+        In case the stored value is a `dict`-like object the key will be used as the key of the dict.
+        In case the stored value is a `list`-like object the keyx will be used as the index of the list.
 
-        :return: copied iTree object
-        """
-        return self.__copy__()
+        In case the target value is a `iTValueModel` the value inside will be targeted and not the model itself.
 
-    def __deepcopy__(self):
-        """
-        create a deepcopy of this item
+        .. note:: If `iTValueModel` is stored in `iTree` the method will not target the model it will
+                  target the value inside. If the model itself is required the `value`-property of `iTree` must be used.
 
-        The difference in between copy and deepcopy for iTree is just that we do in deepcopy a copy
-        of all data items too. In copy we just copy the iTData object not the items itself, they stay as pointers
-        to the original objects.
+        :except: In case a key_index is given but the object is not a `dict` or `list` like object an `AttributeError`
+                 will be raised ( `__getitem__()`-method required). If no matching item is found an
+                 `IndexError` or `KeyError`
+                 will be raised.
 
-        :return: deep copied new iTree object
-        """
-        new = self.__class__(self._tag,
-                    data=self._data.__deepcopy__(),
-                    subtree=[i.__deepcopy__() for i in super(iTree, self).__iter__()]  # here we create a recursion!
-                    )
-        return new
+        :type key: Optional[Hashable,int]
+        :param key: Optional key or index parameter
 
-    def deepcopy(self, *args, **kwargs):
+        :rtype: object
+        :return: value object the `iTree` or `iTValueModel` (in case a model is stored in the `iTree`)
         """
-        create a deepcopy of this item
-
-        The difference in between copy and deepcopy for iTree is just that we do in deepcopy a copy
-        of all data items too. In copy we just copy the iTData object not the items itself, they stay as pointers
-        to the original objects.
+        # Implementation state: ready, tested, doc ok
+        value = self._value[key]
+        return value.value if hasattr(value, 'is_iTValueModel') else value
 
-        :return: deep copied new iTree object
+    def del_value(self):
         """
-        return self.__deepcopy__()
+        Deletes the full value-object stored in ´iTree´ ( ´NoValue´ is stored in iTree).
 
-    def count(self, item_filter=None):
+        This method will always delete the whole object stored in `iTree` even `iTValueModel`-objects are deleted. To
+        delete the value content of a model `mytree.value.clear()` or 'set_value(NoValue)' might be used.
+
+        :return: deleted value
         """
-        count the number of children that match to the given filter
-        :: note: The operation is not very quick on huge iTrees and complicate filters!
+        # Implementation state: ready, tested, doc ok
+        if self._flags & self._READ_ONLY_VALUE:
+            raise PermissionError('iTree value is read only')
+        old_value, self._value = self._value, NoValue
+        return old_value
+
+    def del_key_value(self, key):
+        """
+        If no parameter is given deletes the full value-object stored in ´iTree´ (store ´NoValue´ ).
+
+        In case a key or index is given and the value contains a matching object we will only pop out the
+        related sub-item.
+
+        This method will always delete the whole targeted object even `iTValueModel`-objects are deleted. To
+        delete the value content of a model `mytree.value.clear()` or 'set_value(NoValue)' might be used.
+
+        :except: In case a key is given but the object is not `dict` or `list` like a TypeError or AttributeError
+                 will be raised
+                 ( `__delitem__()`-method is targeted);
+                 If the given key does not exist or an invalid parameter is given a KeyError or IndexError
+                 will be raised.
 
-        :param item_filter:
+        :type key: Optional[Hashable,int]
+        :param key: Optional key or index to exchange just sub-items in the value
 
-        :return: integer number of children matching to the filter
+        :return: deleted value
         """
-        if item_filter is None:
-            return super(iTree, self).__len__()
-        return len(list(filter(item_filter, super(iTree, self).__iter__())))
+        # Implementation state: ready, tested, doc ok
+        if self._flags & self._READ_ONLY_VALUE:
+            raise PermissionError('iTree value is read only')
+        return self._value.pop(key)
 
-    def count_all(self, item_filter=None):
+    @property
+    def coupled_object(self):
         """
-        count deep the number of children and sub children the element has and that match to the given filter
-        :: note: The operation is not very quick on huge iTrees and complicate filters!
+        The `iTree`-object can be coupled with another Python-object. The pointer to the object is stored and can be
+        reached via this property. (E.g. this can be helpful when connecting the `iTree` with a visual item
+        (hypertree-list item) in a GUI)
 
-        :param item_filter:
-
-        :return: integer number of children matching to the filter
+        :return: pointer to coupled-object or None if no object is stored
         """
-        cnt = 0
-        i = -1
-        for i, item in enumerate(self.iter_children(item_filter=item_filter)):
-            cnt += item.count_all()
-        cnt += (i + 1)
-        return cnt
+        # Implementation state: ready, tested, doc ok
+        try:
+            return self._coupled
+        except AttributeError:
+            return None
 
-    # deep getter
-    def get_deep(self, key_list):
+    # set properties
+    def set_coupled_object(self, coupled_object):
         """
-        deep key access
-        the function is a replacement for `self[key_list[0]][key_list[1]]...[key_list[-1]]`
-        but you can also feed with an iterator
+        Couple another Python-object with this `iTree`-object.
 
-        dives into the tree `key_list=[1,0,2]` -> second element level 1 -> first element level 2 ->
-        third element level 3
-        -> same as `self[1][0][2]`
+        Compared with the `value` the coupled-object is not tracked by any internal functions. We do not consider
+        it in any relation (e.g. `__contains__()` and do not dump it in files, etc. Even in linked items the
+        coupled-object is not protected. And in copies it is ignored and not taken over.
 
-        .. note:: Each key in the key list must target to a single item only!
-                     E.g. do not use tags here they deliver always a family iterator not a single item
-                     (the method will raise an exception). Use index integers or TagIdx objects instead
+        .. note:: E.g. The coupled-object might be an object in a GUI that is related to this item.
 
-        :param key_list:  list or iterator of keys (indexes,TagIdx, tuple(tag,index) -> only in case no tuple tags!
 
-        :return: iTree object the key list targets
+        :param coupled_object: object pointer to the object that should be coupled with this iTree item
         """
-        item = self
-        for key in key_list:
-            item = item.__getitem__(key)
-        return item
+        # Implementation state: ready, tested, doc ok
+        self._coupled = coupled_object
 
-    # structural manipulations
+    # *** structure related functions **********************************************************************************
 
-    def clear(self):
-        """
-        deletes all children
-        and data!
-        All flags stay unchanged!
-        """
-        self._data = None
-        self._coupled = None
-        super().clear()
-        self._map = {}
+    # setters:
 
-    def insert(self, insert_key, item):
+    def append(self, item=NoValue):
         """
-        Insert an item before a specific position
+        Append the given `iTree`-object to the `iTree` (new last child)
+        The `append()` method is the fastest way to add a single item to the end of the tree.
 
-        :param insert_key: position key (integer index or TagIdx)
+        :except: In case `iTree`-object has already a parent a `RecursionError` will be raised
+                 Other exceptions might come up in case the `iTree` is protected (tree read-only mode).
 
-        :param item: item that should be inserted in the tree (new child)
-        """
-        try:
-            if item._parent is not None:
-                raise RecursionError('Given item has already a parent iTree!')
-        except AttributeError:
-            if not isinstance(item, iTree):
-                raise TypeError('In iTree only children of type iTree can be integrated')
-            raise
-        if type(insert_key) is int:
-            idx = insert_key
-            if idx < 0:
-                idx = super().__len__() - idx
-        elif isinstance(insert_key, TagIdx):
-            idx = self.__getitem__(insert_key).idx
-        else:
-            raise TypeError('In iTree only children of type iTree can be integrated')
-        item._parent = self
-        super().insert(idx, item)
-        tag = item._tag
-        try:
-            m = self._map
-            if m.__contains__(tag):
-                family = m.__getitem__(tag)
-                t_idx = self.__get_family_insertion_idx(family, idx)
-                family.insert(t_idx, item)
-            else:
-                m.__setitem__(tag, blist((item,)))
-                t_idx = 0
-        except (AttributeError, IndexError):
-            self._map = {tag: blist((item,))}
-            t_idx = 0
-        item._cache = (idx, t_idx)
 
-    def append(self, item):
-        """
-        Append the given iTree object to the tree (new last child)
+        :type item: Union[iTree,object]
+        :param item: `iTree`-object to be appended
+
+                     .. warning::
+                        In case the given item-object is not a `iTree`-object the item is interpreted
+                        as a value and the `iTree` will be created implicit (with tag-family `NoTag`) in the way:
 
-        :except: raise TypeError in case iTree object has already a parent
+                        `iTree(tag=NoTag, value=item)` ~ ìTree(value=item)
+                        If no item is given an empty iTree is created tag=`NoTag`; value=`NoValue`.
 
-        :param item: iTree object to be appended
+                            >>> root=iTree('root')
+                            >>> root.append('myvalue')
+                            iTree(value='myvalue')
+                            >>> root.append() # append an empty iTree-object
+                            iTree()
 
-        :return: True in case append was successful
+        :rtype: iTree
+        :return: Delivers the appended item itself
+                 (it might be useful for the user to get the updated information of the object).
         """
+        if self._flags & self._IS_TREE_PROTECTED:
+            if self.is_link_root:
+                if hasattr(item, '_itree_prt_idx') and item.flags & (
+                        self._LINKED | self._LINK_ROOT | self._PLACEHOLDER):
+                    raise TypeError('Linked items cannot be appended to linked item as local item')
+            else:
+                self._raise_read_only_exception(self)
         try:
-            if item._parent is not None:
+            if item._itree_prt_idx is not None:
                 raise RecursionError('Given item has already a parent iTree!')
+            tag = item._tag
         except AttributeError:
-            if not isinstance(item, iTree):
-                raise TypeError('In iTree only children of type iTree can be integrated')
-            raise
-        # append item:
-        item._parent = self
-        # append to blist:
-        sl = super()
-        idx = sl.__len__()
-        sl.append(item)
-        # append to map
-        tag = item._tag
-        if idx:
-            m = self._map
-            if m.__contains__(tag):
-                family = m.__getitem__(tag)
-                t_idx = family.__len__()
-                family.append(item)
+            # implicit definition of iTree:
+            item = iTree(value=item)
+            tag = NoTag
+        # return self._append_item(self,item)
+        # Just for performance we keep the code for append here and do not use the helper
+        abs_idx = len(self)  # after tests here the len() is quicker (not understood why)
+        if abs_idx:
+            self._items.append(item)
+            # append item to family
+            family = self._get_fam(tag)
+            if family is None:
+                self._setitem_fam(tag, [item])
+                item._itree_prt_idx = [self, abs_idx, 0]
             else:
-                # first time tag is used!
-                t_idx = 0
-                m.__setitem__(tag, blist((item,)))
-        else:
-            self._map = {tag: blist((item,))}
-            t_idx = 0
-        item._cache = (idx, t_idx)
-        return True
+                fm_idx = family.__len__()  # after tests here the .>__len__ is quicker (not understood why)
+                family.append(item)
+                if fm_idx==BLIST_SWITCH:
+                    self._setitem_fam(tag,itree_list(family))
+                item._itree_prt_idx = [self, abs_idx, fm_idx]
+        else:
+            # here we must init all family and item related attributes
+            getitem = self.get
+            # items
+            self._items = sl = self._ONE_ITEM_LIST.copy()
+            sl[0] = item
+            self.getitem_by_idx = getitem.getitem_by_idx = sl.__getitem__
+            self.__len__, self.__iter__, self._setitem_list = sl.__len__, sl.__iter__, sl.__setitem__
+            # family
+            self._families = families = {tag: sl.copy()}
+            getitem._getitem_fam=self._getitem_fam=families.__getitem__
+            self._get_fam, self._setitem_fam = families.get, families.__setitem__
+            item._itree_prt_idx = [self, 0, 0]
+        return item
 
-    def appendleft(self, item):
+    def __iadd__(self, other):
         """
-        Append the given iTree object to the left of the the tree (new first child)
-
-        :except: raise TypeError in case iTree object has already a parent
+        append the given item to the iTree (short form of `append()`)
 
-        :param item: iTree object to be appended
-        """
-        return self.insert(0, item)
+        :except: In case `iTree`-object has already a parent a `RecursionError` will be raised
+                 Other exceptions might come up in case the `iTree` is protected (tree read-only mode).
 
-    def extend(self, extend_items):
-        """
-        We extend the iTree with given items (multi append)
+        :type other: Union[iTree,object]
+        :param other: `iTree`-object to be appended.
 
-        .. note:: In case the extend items have already a parent an implicit copy will be made. We do this because
-               we might get an iTree-object as extend_items parameter and then the children will have automatically a
-               parent even that the parent object might be a temporary one.
+                     .. warning::
 
-        :param extend_items: iterable object that contains iTree objects as items
+                        As in `append()` in case the given item-object is not a `iTree`-object the item is interpreted
+                        as a value and the `iTree` will be created implicit (with `NoTag` tag).
 
-        :return: True
+        :rtype: `ìTree`
+        :return: self
         """
-        # collect for operation
-        return self._load_subtree(extend_items)
+        # Implementation state: ready, tested, doc ok
+        self.append(other)
+        return self
 
-    def extendleft(self, extend_items):
+    def appendleft(self, item=NoValue):
         """
-        We extend the iTree with given items in the beginning (multi appendleft)
-
-        .. note:: In case the extend items have already a parent an implicit copy will be made. We do this because
-               we might get an iTree-object as extend_items parameter and then the children will have automatically a
-               parent even that the parent object might be a temporary one.
+        Append the given `iTree`-object to the left of the parent-tree (new first child)
+        The `appendleft()` method is the recommended method to add a new first item to iTree
+        (quicker than `insert(0,item)` ).
+        Compared to `append()` the method is slower and the cache index information gets invalid after the operation
+        (will be automatically updated later on if required).
+
+        :except: In case `iTree`-object has already a parent a `RecursionError` will be raised.
+                 Other exceptions might come up in case the `iTree` is protected (tree read-only mode).
+
+        :type item: Union[iTree,object]
+        :param item: `iTree`-object to be appended as first item.
+
+                     .. warning::
+
+                        As in `append()` in case the given item-object is not a `iTree`-object the item is interpreted
+                        as a value and the `iTree` will be created implicit.
+
+        :rtype: iTree
+        :return: Delivers the appended item itself
+                 (it might be useful for the user to get the updated information of the object).
+        """
+        # Implementation state: ready, tested, doc ok
+        flags = self._flags
+        if flags & self._IS_TREE_PROTECTED:
+            if self.is_link_root:
+                # if self is link_root and the tag of the given item is different then the linked
+                # ones operation is allowed!
+                if hasattr(item, '_itree_prt_idx'):
+                    if item.flags & (self._LINKED | self._LINK_ROOT | self._PLACEHOLDER):
+                        raise TypeError('Linked items cannot be appended to linked item as local item')
+                    if self._link.is_loaded and item.tag in self._link.tags:
+                        self._raise_read_only_exception(self)
+                elif self._link.is_loaded and NoTag in self._link._tags:
+                    self._raise_read_only_exception(self)
+            else:
+                self._raise_read_only_exception(self)
+        try:
+            if item._itree_prt_idx is not None:
+                raise RecursionError('Given item has already a parent iTree!')
+        except AttributeError:
+            # implicit definition of iTree:
+            item = iTree(value=item)
+        if self:
+            return self._append_item_left(self, item)
+        else:
+            return self._append_item(self, item)
+
+    def insert(self, target, item=NoValue):
+        """
+        Insert an item **before** a given target-position. The insertion works like in lists.
+
+        The insertion operation is slower as the append operations.
+
+        If `target=None` is given the operation inserts in the last position (== `append()`).
+
+        :except: In case `iTree`-object has already a parent a `RecursionError` will be raised
+                 Other exceptions might come up in case the `iTree` is protected (tree read-only mode).
+
+        :type target: Union[Integer,tuple,iTree,None]
+        :param target: target position definition; **target must target a single/unique item!**
+                       Possible targets:
+
+                       * index - absolute target index integer, negative values supported too (count from the end).
+                       * key - key-tuple (family_tag, family_index) pair
+                       * item - `iTree`-item that is already a children (future successor)
+                       * None - if `None` is given we will append the item in the last position of the ´iTree´-object
+
+        :type item: Union[iTree,object]
+        :param item: `iTree`-object to be inserted in the tree.
+
+                     .. warning::
+
+                        As in `append()` in case the given item-object is not a `iTree`-object the item is interpreted
+                        as a value and the `iTree` will be created implicit.
+
+        :rtype: iTree
+        :return: Delivers the inserted item itself
+                 (it might be useful for the user to get the updated information of the object).
+        """
+        # Implementation state: ready, tested, doc ok
+        if target is None:
+            return self.append(item)
+        flags = self._flags
+        if flags & self._IS_TREE_PROTECTED:
+            if self.is_link_root:
+                # if self is link_root and the tag of the given item is different then the linked
+                # ones operation is allowed!
+                if hasattr(item, '_itree_prt_idx'):
+                    if item.flags & (self._LINKED | self._LINK_ROOT | self._PLACEHOLDER):
+                        raise TypeError('Linked items cannot be appended to linked item as local item')
+                    if self._link.is_loaded and item.tag in self._link._tags:
+                        self._raise_read_only_exception(self)
+                elif self._link.is_loaded and NoTag in self._link._tags:
+                    self._raise_read_only_exception(self)
+            else:
+                self._raise_read_only_exception(self)
+        try:
+            if item._itree_prt_idx is not None:
+                raise RecursionError('Given item has already a parent iTree!')
+        except AttributeError:
+            # implicit definition of iTree:
+            item = iTree(value=item)
+        if self:
+            sl = self._items
+            size = sl.__len__()
+            if size == 0 and target != 0:
+                raise KeyError('iTree is empty no valid target given!')
+            # absolute index of the target
+            if type(target) is int:  # is already the absolute index!
+                abs_idx = size + target if target < 0 else target
+            elif hasattr(target, '_itree_prt_idx'):
+                if target._itree_prt_idx is not self:
+                    raise ValueError('Given target is not part of the iTree')
+                abs_idx = target.idx
+            else:
+                abs_idx = self.__getitem__(target).idx
+            if abs_idx == 0:
+                return self._append_item_left(self, item)
+            # insert in list
+            sl.insert(abs_idx, item)
+            # insert item to family
+            tag = item._tag
+            family = self._get_fam(tag)
+            if family is None:
+                self._setitem_fam(tag, [item])
+                item._itree_prt_idx = [self, abs_idx, 0]
+            else:
+                fm_idx = self._get_family_insertion_idx(family, abs_idx)
+                family.insert(fm_idx, item)
+                if fm_idx==BLIST_SWITCH:
+                    self._setitem_fam(tag,itree_list(family))
+                item._itree_prt_idx = [self, abs_idx, fm_idx]
+            return item
+        else:
+            # first item insert is append
+            return self._append_item(self, item)
 
-        .. note:: The `extendleft()` operation is a lot slower then the normal extend operation
+    # multiple appends
 
-        :param extend_items: iterable object that contains iTree objects as items
+    def extend(self, items):
         """
-        # start_idx=len(extend_items)-1
-        # collect for operation
-        sl = super(iTree, self)
-        m = self._map
-        il = len(extend_items)
-        for i in range(il):
-            item = extend_items[il - i - 1]
-            if item._parent is not None:
-                item = item.copy()
-            item._parent = self
-            item._cache = (0, 0)
-            sl.insert(0, item)
-            tag = item._tag
-            try:
-                family = m.__getitem__(tag)
-                family.insert(0, item)
-            except KeyError:
-                m.__setitem__(tag, blist((item,)))
-            except AttributeError:
-                self._map = m = {tag: blist((item,))}
-        return True
+        We extend the `iTree` with given items (multi append). The function is high performant and if you have to
+        append a large number of items it is recommended to create an iterator of the items and
+        feed them into this method. This is quicker compared to a loop doing multiple normal `append()` operations.
+
+        .. note:: In case the to be extended items have already a parent an implicit copy will be made.
+                  We do this because the internal copy can be created more effective.
+                  We accept also iTree-objects as extend_items parameter and the children which have a parent will be
+                  automatically copied to be integrated in this second tree. We have the same situation with a
+                  filtered iterator which might be used to extend this `iTree` too.
+
+        :type items: Iterable
+        :param items: iterable-object that contains `iTree`-objects as items it can be:
+
+                     * iterator or generator of `iTree`-objects (using next)
+                     * `iTree`-object (children will be copied and extended in this tree)
+                     * iterable of `iTree`-objects (list, tuple, ...)
+                     * argument list for `iTree`-instance ( ´__init__()´ ) (created by ´get_init_args()´
+                       or ´get_init_args_deep()´ ) -> this is most often an internal functionality.
+                     * iterator or generator of value-objects (using next) - implicit `iTree`-objects created
+                     * iterable of value-objects (list, tuple, ...)- implicit `iTree`-objects created
+
+        """
+        if self._flags & self._IS_TREE_PROTECTED:
+            if self.is_link_root:
+                # extend is allowed on link_root items
+                # we must check the items in this case!
+                items, check_items = tee(items, 2)  # we must reuse the iterator in this case
+                if self._link.is_loaded:
+                    flag_mask = self._LINKED | self._LINK_ROOT | self._PLACEHOLDER
+                    error = any(
+                        hasattr(i, '_itree_prt_idx') and i.flags & flag_mask
+                        for i in check_items
+                    )
+                    if error:
+                        raise PermissionError(
+                            'It is not allowed to append linked items in an already linked item iTree')
+            else:
+                self._raise_read_only_exception(self)
+        return self._items.extend(_iTreePrivate._iter_extend(self, items))
 
-    def pop(self, key=-1):
+    def extendleft(self, items):
         """
-        pop the item out of the tree, if no key is given the last item will be popped out
+        Multy item append on left hand-side (at the beginning) of the ´iTree´.
 
-        :param key: specific identification key for an item (integer index, TagIdx)
+        The operation is slower than ´extend()´ because it requires a reordering of all items in the `iTree`.
 
-        :return: popped out item (parent will be set to None)
-        """
-        return self.__delitem__(key)
+        .. note::
+                The order of extended items is kept in the operation. It's comparable with:
+                ´[1,2,3]+[4,5,6]=[1,2,3,4,5,6]´ but the result is not a new instance, self is kept.
+
+        .. note:: In case the to be extended items have already a parent an implicit copy will be made.
+                  We do this because the internal copy can be created more effective.
+                  We accept also iTree-objects as extend_items parameter and the children which have a parent will be
+                  automatically copied to be integrated in this second tree. We have the same situation with a
+                  filtered iterator which might be used to extend this `iTree` too.
+
+        :type items: Iterable
+        :param items: iterable-object that contains `iTree`-objects as items it can be:
+
+                     * iterator or generator of `iTree`-objects (using next)
+                     * `iTree`-object (children will be copied and extended in this tree
+                     * iterable of `iTree`-objects (list, tuple, ...)
+                     * argument list for `iTree`-instance ( ´__init__()´ ) (created by ´get_init_args()´
+                       or ´get_init_args_deep()´ )
+                     * iterator or generator of value-objects (using next) - implicit `iTree`-objects created
+                     * iterable of value-objects (list, tuple, ...)- implicit `iTree`-objects created
+        """
+        if self._flags & self._IS_TREE_PROTECTED:
+            if self.is_link_root:
+                # extend is allowed on link_root items
+                # we must check the items in this case!
+                items, check_items = tee(items, 2)  # we must reuse the iterator in this case
+                if self._link.is_loaded:
+                    error = False
+                    tags = self._link.tags
+                    flag_mask = self._LINKED | self._LINK_ROOT | self._PLACEHOLDER
+                    for i in check_items:
+                        if hasattr(i, '_itree_prt_idx'):
+                            if i.flags & flag_mask or i.tag in tags:
+                                error = True
+                                break
+                        elif NoTag in tags:
+                            error = True
+                            break
+                    if error:
+                        self._raise_read_only_exception(self)
+            else:
+                self._raise_read_only_exception(self)
+        # prepare a list of the items in the tree
+        old_items = list(self._items.__iter__())
+        for i in old_items:
+            # delete parent so that no copy is required for later re-extend
+            i._itree_prt_idx = None
+        # clean the internal structure
+        self._families = {}
+        self._items.clear()
+        # extend new and old itmes
+        return self._items.extend(_iTreePrivate._iter_extend(self, chain(items, old_items)))
 
-    def popleft(self):
-        """
-        pop the first item out of the tree
+    # item manipulations
 
-        :return: popped out item (parent will be set to None)
+    def __setitem__(self, target, value):
         """
-        return self.__delitem__(0)
+        Replace an item with the given new item given in the `value`-parameter. The method handles also
+        multiple replaces (rearrangements) like:
 
-    def remove(self, item):
-        """
-        remove the given item out of the tree (delete the child)
+        ::
 
-        :param item: iTree object that should be removed from the tree
+            >>> mytree[1],mytree[0]=mytree[0],mytree[1]
 
-        :return: removed item will be returned (parent is set to None)
-        """
-        return self.__delitem__(item.idx)
+        .. warning::
 
-    def move(self, insert_key):
-        """
-        move the item in another position
+            Because of the parent only principle in rearrangements operations
+            an implicit copy might be created.
+
+        .. note:: Linked items cannot be changed. If changes are required The user
+                  must change the link source tree items
+                  and afterwards actively rerun `load_links()` to reload the linked tree.
+
+        :except: In case the target is not found or the `iTree` is protected (read-only tree).
+
+        :param target: target object defining the replacement target;
+                       possible types are:
+
+                       * index - absolute target index integer (fastest operation)
+                       * key - key tuple (family_tag, family_index)
+                       * tag - Tag(family_tag) object targeting a whole family
+                       * target-list - absolute indexes or keys to be replaced (indexes and keys can be mixed)
+                       * index slice - slice of absolute indexes
+                       * key slice - tuple:  (family_tag, family_index_slice)
+
+                       For multi targets the given value must have a matching structure (item list with same length).
+
+                       We have two special targets which are used for placing/replacing single items in the iTree:
+
+                       * Ellipsis `...` - new_items tag-family will be deleted and the new-item is placed in families
+                         first item position
+                       * items_tag - new_items tag-family will be delted and the new-item is placed in families
+                         last item position
+
+                       If those two special targets are used and the new-items family does not exist yet, the method will
+                       just append the new item, no exception will be raised.
+
+        :param value: iTree object that should replace the target or in case of multi targets a
+                      tuple of items that should be used for replacements
+
+        :return: value added items (only for internal usage)
+        """
+        flags = self._flags
+        if flags & self._IS_TREE_PROTECTED:
+            if self.is_link_root:
+                # if self is link_root and the tag of the given item is different then the linked
+                # ones operation is allowed!
+                if hasattr(value, '_itree_prt_idx'):
+                    if value.flags & (self._LINKED | self._LINK_ROOT | self._PLACEHOLDER):
+                        raise TypeError('Linked items cannot be appended to linked item as local item')
+                    if self._link.is_loaded and value.tag in self._link._tags:
+                        self._raise_read_only_exception(self)
+                elif self._link.is_loaded and NoTag in self._link._tags:
+                    self._raise_read_only_exception(self)
+            else:
+                self._raise_read_only_exception(self)
+
+        old_item = self.__getitem__(target)
+        if old_item is value:
+            return value
+
+        # rearrangement?
+        t = type(value)
+        if type(value) is tuple or type(value) is list or type(value) is itree_list:
+            old_items = old_item
+            it_setitem = self.__setitem__
+            return [it_setitem(old_items[i].idx, new) for i, new in enumerate(value)]
+
+        # prepare new item
+        if hasattr(value, '_itree_prt_idx'):
+            parent_list = value._itree_prt_idx
+            if parent_list is not None:
+                if parent_list[0] == self:
+                    # reorder operation!
+                    value = self._iter_copy(value, iTree._get_args_skip_subtree)
+                else:
+                    raise RecursionError('Given item has already a parent iTree!')
+        else:
+            # implicit iTree definition
+            value = iTree(value=value)
 
-        :param insert_key: item will be insert before this key
+        if target is ...:  # Ellipsis is used for single append
+            if self:
+                tag = value.tag
+                if tag in self._families:
+                    # delete family
+                    self.__delitem__(tag)
+            return self.append(value)
+        elif target == value.tag:  # family tag replaces family with the single item (same position as fist item in family
+            tag = value.tag
+            family= self._get_fam(tag)
+            if family is None:
+                return self.append(value)
+            else:
+                list(
+                    self._raise_exception(AttributeError('Single operations on linked items are not supported')) for
+                    i
+                    in family if i.is_link_cover)
+                old_item_idx = family[0].idx
+                sl = self._items
+                for i in reversed(family[1:]):
+                    sl.__delitem__(i.idx)
+                sl.__setitem__(old_item_idx, value)
+                self._families[tag] = [value]
+                value._itree_prt_idx = (self, old_item_idx, 0)
+                return value
+        # normal setitem replaces old item
+        # handle old item
+        try:
+            abs_idx = old_item.idx
+        except AttributeError as e:
+            raise LookupError(
+                'Given target is not unique; set operation can only be made on unique items!'
+            ) from e
+        # if old_item.is_linked:
+        #    raise PermissionError('The target item is read_only (linked)!')
+        o_tag, o_fm_idx = old_item.tag_idx
+        # start the manipulation
+        old_item._itree_prt_idx = None
+        # replace old item in super list
+        self._items.__setitem__(abs_idx, value)
+        v_tag = value._tag
+        if v_tag == o_tag:  # same family
+            family = self._getitem_fam(v_tag)
+            # replace old item in family list
+            family.__setitem__(o_fm_idx, value)
+            fm_idx = o_fm_idx
+        else:
+            # different families
+            # del old item from family
+            self._getitem_fam(o_tag).__delitem__(o_fm_idx)
+            try:
+                family = self._getitem_fam(v_tag)
+                fm_idx = self._get_family_insertion_idx(family, abs_idx)
+                family.insert(fm_idx, value)
+            except (KeyError, IndexError):
+                self._setitem_fam(v_tag, [value])
+                fm_idx = 0
+        value._itree_prt_idx = [self, abs_idx, fm_idx]
+        return value
+
+    def move(self, target=None):
         """
-        if self._parent is None:
-            raise LookupError('Given item is not a children of a iTree!')
-        parent = self._parent
+        Move this item in given target position (item will be positioned **before** the given target).
+        The given target must be a unique item! If None is given
+        the item will be moved in the last position of the `iTree`. If an ìTree`-object
+        is given as target it must be a children of the same parent (sibling).
+
+        :type target: Union[Integer,tuple,iTree,None]
+        :except: LookupError in case the target is not found or not unique!
+
+        :param target: target-object defining the replacement target;
+                       possible types are:
+
+                       * index - absolute target index integer, negative values supported too (count from the end).
+                       * key - key-tuple (family_tag, family_index) pair
+                       * item - `iTree`-item that is already a children (future successor)
+                       * None - if `None` is given we will move the item to the last position in the ´iTree´-object
+
+        :return: self (with updated indexes)
+        """
+        if self._itree_prt_idx is None:
+            raise LookupError('This item is not a children of a iTree!')
+        parent = self._itree_prt_idx[0]
+        flags = parent._flags
+        if flags & self._IS_TREE_PROTECTED:
+            if parent.is_link_root:
+                if parent._link.is_loaded and self.tag in parent._link._tags:
+                    self._raise_read_only_exception(self)
+            else:
+                self._raise_read_only_exception(self)
+        if target is None:
+            move_item = parent.__delitem__(self.idx)
+            return parent.append(move_item)
         # check if target exists:
-        if type(insert_key) is not int:
-            target_idx = parent.__getitem__(insert_key).idx
+        if type(target) is not int:
+            try:
+                target_idx = parent.__getitem__(target).idx
+            except AttributeError as e:
+                raise LookupError('Given target is not unique') from e
         else:
-            target_idx = insert_key
+            target_idx = target
         src_idx = self.idx
         move_item = parent.__delitem__(src_idx)
-        parent.insert(target_idx, move_item)
+        return parent.insert(target_idx, move_item)
 
     def rename(self, new_tag):
         """
-        give the item a new tag
+        give the item a new family tag
 
-        :param new_tag: new tag object string or hashable object
-        """
-        t = type(new_tag)
-        if t is int or t is TagIdx:
-            raise TypeError('Given tag cannot be used in iTree wrong type (int or TagIdx)')
-        parent = self.parent
-        if parent is None:
+        The renaming of the item implies a reordering of the items in the tree because the family order
+        depends on the global/absolute order of items.
+
+        :type new_tag: Hashable
+        :param new_tag: new tag (any kind of hashable object)
+
+        :rtype: iTree
+        :return: Delivers the renamed item itself
+                 (it might be useful for the user to get the updated information of the object).
+
+        """
+        parent_list = self._itree_prt_idx
+
+        if parent_list is not None:
+            parent = parent_list[0]
+            flags = parent._flags
+            if flags & self._IS_TREE_PROTECTED:
+                if parent.is_link_root:
+                    if parent._link.is_loaded:
+                        tags = parent._link._tags
+                        if new_tag in tags:
+                            self._raise_read_only_exception(self)
+                        if self._flags & (self._LINKED | self._PLACEHOLDER):
+                            self._raise_read_only_exception(self)
+                else:
+                    self._raise_read_only_exception(self)
+        else:
             self._tag = new_tag
             return
-        pm = parent._map
+        families = parent._families
         tag = self._tag
         # remove old tag in the map-dict
-        family = pm.__getitem__(tag)
+        family = families.__getitem__(tag)
         if len(family) == 1:
-            pm.__delitem__(tag)
+            families.__delitem__(tag)
         else:
             family.remove(self)
         # insert new tag
         self._tag = new_tag
-        if new_tag in pm:
-            new_family = pm.__getitem__(new_tag)
-            idx = self.__get_family_insertion_idx(new_family, self.idx)
-            new_family.insert(idx, self)
-            self._cache = (self._cache[0], idx)
+        if new_tag in families:
+            new_family = families.__getitem__(new_tag)
+            fm_idx = self._get_family_insertion_idx(new_family, self.idx)
+            new_family.insert(fm_idx, self)
+            self._itree_prt_idx[2] = fm_idx
         else:
             # create new family
-            pm.__setitem__(new_tag, blist((self,)))
-            self._cache = (self._cache[0], 0)
+            families.__setitem__(new_tag, [self])
+            self._itree_prt_idx[2] = 0
+        return self
 
     def reverse(self):
         """
-        reverse the order of all children in the iTree object
+        Reverse the order of all children in the `iTree`.
+
+        If you do not want to change the object itself (in place operation) you might use the iterator
+        `reversed()` instead.
 
         """
-        super(iTree, self).reverse()
-        for item in self._map.values():
-            item.reverse()
+        flags = self._flags
+        if flags & self._IS_TREE_PROTECTED:
+            if not self.is_link_root or self._link.is_loaded:
+                self._raise_read_only_exception(self)
+        else:
+            self._items.reverse()
+            for family in self._families.values():
+                family.reverse()
 
-    def rotate(self, n):
+    def rotate(self, n=1):
         """
-        rotate children of the iTree object n times
-        (rotate  1 times means move last element to first position)
+        Rotate children of the `iTree`-object n times (n positions)
+        (rotate 1 times means move last item to first position)
 
-        :param n:
+        If no parameter is given we rotate by one position only.
 
-        """
-        if n > 0:
-            for i in range(n):
-                rot_item = self.pop()
-                self.insert(0, rot_item)
-        elif n < 0:
-            for i in range(n):
-                rot_item = self.popleft()
-                self.__iadd__(rot_item)
+        The rotation can be made in negative direction too (give negative numbers).
 
-    # iterators
+        In case zero is given the operation is neutral and nothing will be changed.
 
-    def iter_all(self, item_filter=None, filter_or=True):
-        """
-        main iterator for whole tree runs in top-> down order
-        e.g.
-        ::
-            iTree('child')
-             └──iTree('sub0')
-                 └──iTree('sub0_0')
-                 └──iTree('sub0_1')
-                 └──iTree('sub0_2')
-                 └──iTree('sub0_3')
-             └──iTree('sub1')
-                 └──iTree('sub1_0')
-        will be iterated like:
-        ::
-             iTree('child')
-             iTree('sub0')
-             iTree('sub0_0')
-             iTree('sub0_1')
-             iTree('sub0_2')
-             iTree('sub0_3')
-             iTree('sub1')
-             iTree('sub1_0')
-
-        :param item_filter: filter for filter the items you can give a filter constant or
-                            a method for filtering (should return True/False)
-
-        :param filter_or:
-
-                          * True  - we combine the filtering with or this means even if we have no match in the higher
-                            levels of the tree we will go deeper to find matches
-
-                          * False - filters are combined with and which means children will only be parsed in
-                            case the parent matches also to the filter condition
-
-        :return: iterator
-        """
-        if filter_or:
-            for item in self.iter_children(item_filter=None):
-                if item_filter is None or item_filter(item):
-                    yield item
-                for subitem in item.iter_all(item_filter=item_filter, filter_or=filter_or):
-                    yield subitem
-        else:
-            for item in self.iter_children(item_filter=item_filter):
-                yield item
-                for subitem in item.iter_all(item_filter=item_filter, filter_or=filter_or):
-                    yield subitem
+        .. note:: There is no in-depth counterpart of this method available.
 
-    def iter_all_bottom_up(self, item_filter=None, filter_or=True):
+        :type n: integer
+        :param n: number of positions the items should be rotated
         """
-        main iterator for whole tree runs in down-> top order (We start at the children and afterwards the parents:
-        e.g.:
-        ::
-            iTree('child')
-             └──iTree('sub0')
-                 └──iTree('sub0_0')
-                 └──iTree('sub0_1')
-                 └──iTree('sub0_2')
-                 └──iTree('sub0_3')
-             └──iTree('sub1')
-                 └──iTree('sub1_0')
-        Will be iterated:
-        ::
-             iTree('sub0_0')
-             iTree('sub0_1')
-             iTree('sub0_2')
-             iTree('sub0_3')
-             iTree('sub0')
-             iTree('sub1_0')
-             iTree('sub1')
-             iTree('child')
-
-        :param item_filter: filter method for filtering (should return True/False when fet with an item) or
-                            iTFilter object
-
-        :param filter_or:
-
-                          * True - we combine the filtering with or this means even if we have no match in the higher
-                            levels of the tree we will go deeper to find matches
-
-                          * False - filters are combined with and which means children will only be parsed in
-                            case the parent matches also to the filter condition
-
-        :return: iterator
-        """
-        if filter_or:
-            for item in self.iter_children(item_filter=None):
-                for subitem in item.iter_all(item_filter=item_filter, filter_or=filter_or):
-                    yield subitem
-                if item_filter is None or item_filter(item):
-                    yield item
-        else:
-            for item in self.iter_children(item_filter=item_filter):
-                for subitem in item.iter_all(item_filter=item_filter, filter_or=filter_or):
-                    yield subitem
-                yield item
+        flags = self._flags
+        if flags & self._IS_TREE_PROTECTED:
+            if not self.is_link_root or self._link.is_loaded:
+                self._raise_read_only_exception(self)
+        elif n > 0:
+            move_items = [self.pop() for _ in range(n)]
+            move_items.reverse()
+            self.extendleft(move_items)
+        elif n < 0:
+            move_items = [self.pop(0) for _ in range(-n)]
+            # move_items.reverse()
+            self.extend(move_items)
 
-    def iter_children(self, item_filter=None):
+    def sort(self, key=None, reverse=False):
         """
-        main iterator in children level
+        Sorting operation -> same behavior as sort of lists (parameter description is taken from list documentation).
 
-        :param item_filter: the items can be filtered by giving a filter constants or giving a filter method or
-                            iTFilter object
+        .. note:: This is an "in place" operation which changes the content of the object the build-in `sorted()`
+                    might be use instead (if the original object should not be changed):
 
-        :return: iterator
-        """
-        if item_filter is None:
-            return super(iTree, self).__iter__()
-        else:
-            return filter(item_filter, super(iTree, self).__iter__())
+                        >>> a=iTree(subtree=[iTree(3),iTree(2),iTree(4),iTree(1)])
+                        >>> a.render()
+                        iTree()
+                        > iTree(3)
+                        > iTree(2)
+                        > iTree(4)
+                        > iTree(1)
+                        >>> b=iTree(subtree=(a[i] for i in sorted(a.keys())))
+                        iTree()
+                        > iTree(1)
+                        > iTree(2)
+                        > iTree(3)
+                        > iTree(4)
 
-    def iter_tag_idxs(self, item_filter=None):
-        """
-        iter over all children and deliver the children TagIdx
 
-        :param item_filter: the items can be filtered by giving a filter constants or giving a filter method or
-                            iTFilter object
 
-        :return: iterator over the TagIdx of the children
-        """
-        tag_cnts = {}
-        for item in self.iter_children(item_filter=item_filter):
-            tag = item._tag
-            try:
-                tag_cnts[tag] = cnt = tag_cnts[tag] + 1
-            except KeyError:
-                tag_cnts[tag] = cnt = 0
-            yield TagIdx(tag, cnt)
+        Internally in this operation a copied sorted list is created, and afterwards the whole structure is cleared
+        and rebuild based on the sorted list.
 
-    def iter_tag_idxs_all(self, item_filter=None):
-        """
-        Delivers an iterator over all items tag_idx_paths
+        The default-operation is to the sort based on the list of keys
+        (tag-family, family_index) pair of the items. The base of the sorting can be modified by changing
+        the `target_type` parameter.
 
-        :param item_filter: the items can be filtered by giving a filter constants or giving a filter method or
-                            iTFilter object
+        :param key:  specifies a function of one argument that is used to extract a comparison key
+                     from each list element (for example, key=str.lower). The key corresponding to each item in
+                     the list is calculated once and then used for the entire sorting process.
+                     The default value of None means that list items are sorted directly without calculating
+                     a separate key value.
 
-        :return: iterator over tuples of tag_idxs_paths of all items
-        """
-        tag_cnts = {}
-        for item in self.iter_children(item_filter):
-            tag = item._tag
-            try:
-                tag_cnts[tag] = cnt = tag_cnts[tag] + 1
-            except KeyError:
-                tag_cnts[tag] = cnt = 0
-            ti_l = (TagIdx(tag, cnt),)
-            yield ti_l
-            for tag_idx_list in item.iter_tag_idxs_all(item_filter):
-                yield ti_l + tag_idx_list
+        :param reverse: is a boolean value. If set to True, then the list elements are sorted
+                        as if each comparison were reversed.
 
-    def iter_idxs_all(self, item_filter=None):
         """
-        Delivers an iterator over all items index path tuples
-        .. note:: This method is mainly usd for internal proposes (max_depth_down)
+        flags = self._flags
+        if flags & self._IS_TREE_PROTECTED:
+            if not self.is_link_root or self._link.is_loaded:
+                self._raise_read_only_exception(self)
+        else:
+            sort_list = list(self._items.__iter__())
+            sort_list.sort(key=key, reverse=reverse)
+            self._items.clear()
+            self._families = {}
+            self.extend(sort_list)
 
-        :param item_filter: item_filter filter method might be used
 
-        :return: iterator over tuples of index paths of all items
+    def __delitem__(self, target):
         """
-        i = 0
-        for item in self.iter_children(item_filter):  # not use enumerate here because this consumes the iterator!
-            i = i + 1  # quicker then i+=1  i =
-            t = (i,)
-            yield t
-            for idx_list in item.iter_idxs_all(item_filter):
-                yield t + idx_list
-
-    def find_all(self, key_path, item_filter=None, str_path_separator='/', str_index_separator='#'):
-        """
-        The find all function works on all levels of the tree. The key_path given (e.g. a list of indexes) addresses
-        the items into the depth first item first level, second item second level,....
-
-        The method returns always an iterator or in case of no match an empty list! If you target to unique objects
-        you will get anyway an iterator containing this unique element.
+        The function deletes the targeted item in the tree.
 
-        .. warning:: It's possible to create invalid recursions when constructing the key_path. In these cases the
-                  recursion depth exceeded exception will be raised by the interpreter
+        :except: In case the target is not found or the `iTree` is protected (read-only tree).
 
-        In case the target in the upper keys is not unique, all matches will be delivered!
-        e.g. The operation `my_tree.find_all(['child','sub_child'])` takes first all items in the "child" family:
+        :type target: Union[int,tuple,Hashable,Iterable,slice]
+        :param target: target object defining the replacement target;
+                       possible types are:
 
-             `TagIdx('child',0),TagIdx('child',1),...TagIdx('child',n)` in an iterator and in the next step the function
-             will go one level deeper and will cumulate all the 'sub_child' families in these items as the result:
+                           * *index* - absolute target index integer (fastest operation)
+                           * *key* - key tuple (family_tag, family_index)
+                           * *tag* - Tag(family_tag) object targeting a whole family
+                           * *target-list* - absolute indexes or keys to be replaced (indexes and keys can be mixed)
+                           * *index-slice* - slice of absolute indexes
+                           * *key-slice* - tuple of (family_tag, family_index_slice)
+                           * *itree_filter* - method (callable) for filtering the children of the object
 
-             This means we have something like this:
+        :return: deleted item
+        """
+        is_link_root = False
+        if self._flags & self._IS_TREE_PROTECTED:
+            if not self.is_link_root:
+                self._raise_read_only_exception(self)
+            elif self.is_link_loaded:
+                is_link_root = True
+        if self:
+            if type(target) is int:  # special very quick access:
+                if is_link_root:
+                    item = self.getitem_by_idx(target)
+                    if item._flags & (self._LINKED | self._PLACEHOLDER):
+                        self._raise_read_only_exception(self)
+                del_item = self._items.pop(target)
+                tag = del_item._tag
+                family = self._getitem_fam(tag)
+                size_fam = len(family)
+                if hasattr(del_item, '_link') and del_item._link._link_item is not None:
+                    f_idx = del_item.tag_idx[1]
+                    link_item = del_item._link._link_item
+                    self._items.insert(target, link_item)
+                    family[f_idx] = link_item
+                    link_item._itree_prt_idx = [self, target, f_idx]
+                    del_item._itree_prt_idx = None
+                    return del_item
+                elif size_fam - 1:
+                    # find family index
+                    i = del_item._itree_prt_idx[2]
+                    if i < size_fam and del_item is family[i]:
+                        family.__delitem__(i)
+                    else:
+                        start = 0
+                        for _ in family:  # for is quicker as while
+                            i = family.index(del_item, start)
+                            if family[i] is del_item:
+                                f_idx = i
+                                break
+                            start = i + 1
+                        family.__delitem__(f_idx)
+                else:
+                    self._families.__delitem__(tag)
+                del_item._itree_prt_idx = None
+                return del_item
+            else:
+                items = self.__getitem__(target)
+                if hasattr(items, '_itree_prt_idx'):
+                    return self.__delitem__(items.idx)
+                else:
+                    return [self.__delitem__(item.idx) for item in items]
+        raise KeyError('Given target %s not found in item %s' % (repr(target), str(self)))
 
-             `my_tree[TagIdx('child',0)][TagIdx('sub_child',0)],my_tree[TagIdx('child',0)][TagIdx('sub_child',1)],...,`
+    def clear(self, keep_value=False, local_only=False):
+        """
+        deletes all children
+        and the value!
 
-             `my_tree[TagIdx('child',1)][TagIdx('sub_child',0)],my_tree[TagIdx('child',0)][TagIdx('sub_child',1)],...,`
+        All flags stay unchanged, except the load_links flag!
 
-             ...
+        :type keep_value: bool
+        :param keep_value:
+                        * True - value is not deleted
+                        * False - value will be replaced with NoValue
 
-             and in case of no match in the keys items are skipped.
+        :type local_only: bool
+        :param local_only:
 
-             .. note::  It's not at all the same as: my_tree['child']['sub_child'] -> this operation will raise an
-                        exception!
+                        * True - clear only the local items
+                        * False - clear whole object (The object is reset to the no links loaded
+                          state and locals are deleted)
+        """
+        flags = self._flags
+        if flags & self._IS_TREE_PROTECTED and not self.is_link_root:
+            self._raise_read_only_exception(self)
+        if self.is_link_root:
+            if local_only:
+                for item in self._iter_locals_add_placeholders(self):
+                    if item.is_placeholder:
+                        continue
+                    self.__delitem__(item.idx)
+            else:
+                self._link._loaded = False
+                self._unset_flags(self, self._LOAD_LINKS)
+                self._items.clear()
+                self._families = {}
+        else:
+            self._unset_flags(self, self._LOAD_LINKS)
+            self._items.clear()
+            self._families = {}
+        if not keep_value:
+            self._value = NoValue
 
-        .. note::  When addressing a single item it's quicker (~10x faster depending on tree depth) to use the
-                   `get_deep()` method instead of the `find_all()` method.
+    def pop(self, target=-1):
+        """
+        pop the item out of the tree, if no key is given the last item will be popped out
 
-        The key_path parameter is very flexible in case of the objects you put in. We have several possibilities:
+        We do not have the method popleft because `pop(0)` does the same.
 
-        0. Special keys: We have the following special keys that might be used in the key_path:
+        :type target: Union[int,tuple,Hashable,Iterable,slice,iTree]
+        :param target: target of popped item(s):
 
-            - "/" default path separator (might be changed by str_path_separator parameter)
-              If this is the first key the `find_all()` search will be started in the root element not in the
-              element the method is called.
+                       * *index* - absolute target index integer (fastest operation)
+                       * *key* - key tuple (family_tag, family_index)
+                       * *tag* - Tag(family_tag) object targeting a whole family
+                       * *target-list* - absolute indexes or keys to be replaced (indexes and keys can be mixed)
+                       * *index-slice* - slice of absolute indexes
+                       * *key-slice* - tuple of (family_tag, family_index_slice)
+                       * *itree_filter* - method (callable) for filtering the children of the object
 
-              .. note::  Be careful with "//" or "/" placed not in the beginning of the path this will rollback the
-                     `find_all()` to the root which means anything in the key_path before this key will be ignored.
+        :return: popped out item(s) (parent will be set to None). In case multiple items are
+                 removed an iterator over the removed items is given.
+        """
+        return self.__delitem__(target)
 
-            - "*"-wildcard will iterate over all children of the item
+    def remove(self, item):
+        """
+        With remove the given target is a `iTree` child that should be removed.
 
-            - "**"-wildcard will iterate over all items of the item. The item itself is the first element
-              of the iterator delivered
+        The method is only in because we like to be compatible with lists interface but the pop method target
+        allows already to use a child as a target too.
 
-              .. note::  `find_all('**')` creates an different iterator then `iter_all()`
-                         `list(my_tree.find_all('**')) = [my_tree] + list(my_tree.iter_all())`
+        :except: If given item is not a child of the parent or the ìTree`-objects tree is protected
 
-            .. warning::  It's always recommended to avoid the usage of string tags containing functional characters
-                          like "**","*","/","#","?". E.g. In case the iTree contains a family with the tag "/" or "*"
-                          or "**" the related family will be delivered. The special functionality is blocked in this
-                          moment (for "/" you might use the str_path_separator parameter to keep the functionality).
-                          Also filtering via iTMatch objects is limited in this case.
+        :type item: Union[iTree,Iterable]
+        :param item: Child or iterable of children to be removed from the tree
 
-        1. Give normal keys like in `__getitem__()` method:
-           normal keys can be:
+        :return: removed item(s) (parent will be set to None) - in case of multiple removes the
+                 method delivers a list no iterator because anyway a list is created
+        """
+        if hasattr(item, '_itree_prt_idx'):
+            if item._itree_prt_idx is not None and item._itree_prt_idx[0] is self:
+                return self.__delitem__(item.idx)
+            else:
+                raise ValueError('Given iTree object is not a child of this iTree-object')
+        try:
+            is_link_root = self.is_link_root and self.is_link_loaded
+            item_list = list(
+                item)  # we consume the iterator here because we need it multiple times we used list to reverse later on
+            for i in item_list:  # check if the items in the iterator are valid for the operation
+                try:
+                    if i._itree_prt_idx[0] is not self:
+                        raise AttributeError()
+                    if is_link_root and (i.is_linked or i.is_placeholder):
+                        self._raise_read_only_exception(self)
+                    continue
+                except AttributeError as e:
+                    raise ValueError(
+                        'The object %r is not a child of this iTree-object'
+                        % repr(i)
+                    ) from e
+            for i in reversed(item_list):  # we see advantage for most cases if we remove in reversed order
+                self.__delitem__(i.idx)
+            return item_list
+        except (PermissionError, ValueError):
+            raise
+        except:
+            raise TypeError('As item parameter we expect an iTree child or a Iterable of children')
 
-             * index integers
-             * tag strings
-             * TagIdx,TagIdxStr,TagIdxBytes
-             * TagMultiIdx,slices
-             * for index lists you must give[[1,2,3,4]] because first level will be interpreted as
-             * a list targeting into the depth of the tree
+    # *** getters: *****************************************************************************************************
 
-             e.g. by index
+    def __getitem__(self, target):
+        """
+        Main common get method for children (first level items).
 
-                 * `my_tree.find_all(1)` is same as `my_tree[1]`
-                 * `my_tree.find_all('child')` is same as `my_tree['child']`
-                 * `my_tree.find_all(TagIdx('child',1))`is same as `my_tree[TagIdx('child',1)]`
-                 ...
+        In case the given targets is a absolute index or a key (tag,family-index) pair the method will
+        deliver a unique item back. This operation is prioritized over the other operations.
+
+        For all other targets the method will deliver a list with the targeted items as result.
+
+        In some cases an empty list might be delivered and no exception might be raised
+        (e.g. filter query delivers no match).
+
+        In case user likes to have other return-types he might check the other available get methods
+        ( `get()`, `get.single()`, `get.iter()`) or he might also use the itertree helper method `getter_to_list()` to
+        convert any of the possible results into a list.
+
+        :except: In case of no match (even if a part is not matching (e.g. one index in an index-list) the
+                 method will raise
+                 a KeyError (no matching target given); IndexError (no matching index given) or
+                 ValueError (no valid type of target given).
+
+        :type target: Union[int,tuple,list,slice]
+        :param target: target object targeting a child or multiple children in the ´iTree´.
+                       Possible types are:
+
+                           * *index* - absolute target index integer (fastest operation)
+                           * *key* - key tuple (family_tag, family_index)
+                           * *index-slice* - slice of absolute indexes
+                           * *key-index-slice* - tuple of (family_tag, family_index_slice)
+                           * *target-list* - absolute indexes or keys to be replaced (indexes and keys can be mixed)
+                           * *key-index-list* - tuple of (family_tag, family_index_list)
+                           * *tag* - family_tag object targeting a whole family
+                           * *tag-set* - a set of family-tags targeting the items of multiple families
+                           * *itree_filter* - method (callable) for filtering the children of the object
+                           * *all-children* - if build-in `iter` or `...`(Ellipsis) is given a list
+                             of all children will be given (same like list(itree.__iter__())`)
+
+        :rtype: Union[iTree,list]
+        :return: Target was *index* or *key* -> one `iTree` item will be given;
+                 for all other targets a list will be delivered.
+        """
+        if self:
+            t = type(target)
+            if t is tuple:
+                try:
+                    # check for key as quick as possible!
+                    fam_tag, fam_idx = target  # unpack to be sure we have a tuple of two items
+                    if fam_idx is ...:
+                        return self._getitem_fam(fam_tag)[:]
+                    # key, family-index or  key, family-index-slice:
+                    return self._getitem_fam(fam_tag)[fam_idx]
+                except TypeError:
+                    try:
+                        family = self._getitem_fam(fam_tag)
+                        return [family[i] for i in fam_idx]
+                    except:
+                        try:
+                            return list(self._getitem_fam(target))
+                        except:
+                            raise ValueError('Given target {} is invalid'.format(repr(target)))  # from e
+                except IndexError:
+                    try:
+                        return list(self._getitem_fam(target))
+                    except:
+                        raise IndexError(
+                            'Given family-idx of target {} not found in iTree'.format(repr(target)))  # from e
+                except:
+                    try:
+                        return list(self._getitem_fam(target))
+                    except:
+                        if 'fam_idx' in locals():
+                            raise KeyError(
+                                'Given target {} invalid or not found in iTree'.format(repr(target)))  # from e
+                        else:
+                            raise ValueError('Given target {} is invalid'.format(repr(target)))  # from e
+            elif t is int or t is slice:
+                # absolute index or absolute index-slice
+                try:
+                    return self.getitem_by_idx(target)
+                except IndexError:
+                    try:
+                        # Maybe we have a tag that matches?
+                        return list(self._getitem_fam(target))
+                    except:
+                        raise IndexError(
+                            'Given abs-idx in target {} is out of range'.format(repr(target)))  # from e
+
+            elif t is TagIdx:  # downward compatibility
+                fam_tag, fam_idx = target  # unpack
+                return self._getitem_fam(fam_tag)[fam_idx]
+            elif t is set:
+                # tags-set
+                result = []
+                for tag in target:
+                    result.extend(self._families[tag])
+                if result:
+                    return result
+                raise KeyError('No matching item found')
+            elif t is list:
+                # multiple targets given they will be combined in one list
+                result = []
+                for sub_target in target:
+                    r = self[sub_target]
+                    if type(r) is list:
+                        result.extend(r)
+                    else:
+                        result.append(r)
+                if result:
+                    return result
+                raise KeyError('No matching item found')
+            elif target is Ellipsis:
+                return self.getitem_by_idx(self._NoneSlice)  # full slice is incredible fast on blists
+            elif callable(target):
+                if target is iter:
+                    # give all items
+                    return self.getitem_by_idx(self._NoneSlice)
+                # filter given?
+                try:
+                    return list(filter(target, self))
+                except Exception:
+                    if "<lambda>" in str(target):
+                        # We try to identify in this case which child made the troubles
+                        for c in self:
+                            try:
+                                target(c)
+                            except Exception:
+                                raise TypeError('lambda: raised an exception in filter-calculation, the %i. child %s'
+                                                ' is incompatible with the calculation' % (c.idx, str(c)))
+            result= self._get_fam(target)
+            if result is not None:
+                return result[:] # slice is quicker then copy
+        raise KeyError('Given target: %s not found in iTree!' % repr(target))
 
-        2. Give a list of normal keys:
+    # *** math operations and operations creating new/copied representations *******************************************
 
-           e.g. by index
+    def __reversed__(self):
+        return self.__class__(self._tag,
+                              value=copy.copy(self._value),
+                              subtree=[i.__copy__() for i in reversed(list(self._items.__iter__()))],
+                              # here we create a recursion -> subtree is copied!!
+                              )
 
-            * `my_tree.find_all([1,2])`is same as my_tree[1][2]
-            * `my_tree.find_all(['child','sub_child'])` delivers an iterator over all "sub_child" families found
-               in all "child" families
-            * `my_tree.find_all([TagIdx('child',1),TagIdx('sub_child',1)])`is  same as
-              `my_tree[TagIdx('child',1)][TagIdx('sub_child',1)]`
-            ...
+    def __mul__(self, factor):
+        """
+        Multiplication function a iTree is multiplied (copies) and put in a new iTree:
 
-        3. Give `iTMatch()` object or list of `iTMatch()` objects:
+        my_single_item=iTree('multi')
+        multi=my_single_item*1000
 
-           An iterator of all matching tags will be created the matches will be combined with the and operation.
-           You can also use an item_filter containing the Filter.iTFilterItemTagMatch to have the same functionality.
-           In case a list is given the find_all() function is again going one level deeper for each element in the list.
+        In case factor is another iTree the cartesian product will be calculated. The resulting iTree
+        will have a length of: len(self)*len(factor)*2 (The factor 2 results
+        from the difference of the cartesian to the normal product)
+        The subtree looks like (item1_x from self item2_x from factor):
+        item1_0, item_2_0, item1_0, item_2_1, item1_0, item2_2, ..., item1_1, item2_0, item1_1, item2_1, ...
 
-        :param key_path: iterable/iterator that addresses items in the tree (see above explanations and examples)
 
-        :param item_filter: item_filter method
 
-        :param str_path_separator: In case of string tags the user can give also strings that are internally casted
-                                   into a list by using the str_path_separator (default="/")
-                                   e.g.: "/child_tag/sub_child_tag" -> ["child_tag","sub_child_tag"]
+        HINT: In this operation multiple copies of the original item generated.
 
-        :param str_index_separator: In case of string tags the user can give TgaIdx also by string definition this is
-                                    the separator used to separate the index number from the tag (default="#")
-                                    e.g. "child_tag#89" -> TagIdx("child_tag",89)
+        :param factor: integer to multiply with
+        :return: iTree object containing multiplied children
+        """
+        if hasattr(factor, '_itree_prt_idx'):
+            if self.is_link_root:
+                raise TypeError('__mul__() on link-root items is not supported')
+            subtree = chain.from_iterable(
+                product((i.copy() for i in self), (i.copy() for i in factor)))
+        else:
+            subtree = repeat(self.copy(), factor)
+        return iTree(self._tag, copy.copy(self._value), subtree, None, self._flags)
 
-        :return: iterator over the matches or in case of no match found an empty list -> []
+    def __rmul__(self, other):
+        if hasattr(other, '_itree_prt_idx'):
+            subtree = chain.from_iterable(
+                product((i.copy() for i in self), (i.copy() for i in other)))
+        else:
+            subtree = repeat(self.copy(), other)
+        return iTree(NoTag, NoValue, subtree)
 
+    def __sub__(self, other):
         """
+        To subtract two iTree objects we copy the self-object and we iterate over the other object items.
+        In case a matching key is found in self the item will be deleted in the copy.
 
-        sl = super()
-        m = self._map
-        if m is None:
-            m = {}
-        try:  # direct match ?
-            if key_path in m:
-                return self.__build_find_all_result(m.__getitem__(key_path), item_filter)
-        except TypeError:
-            pass
-        t = type(key_path)
-        if t is str:
-            lkp = key_path.__len__()
-            if lkp == 0:
-                return []
-            if key_path[0] == '*':
-                if lkp == 1:
-                    # from here on the item must have children!
-                    if sl.__len__() == 0:
-                        return []
-                    return itertools.chain(self.__build_find_all_result(self, item_filter),
-                                           self.iter_children(item_filter=item_filter))
-                if key_path[1] == '*':
-                    if lkp == 2:
-                        return self.iter_all(item_filter=item_filter)
-            try:
-                return self.__build_find_all_result(self.__getitem__(key_path, str_index_separator), item_filter)
-            except KeyError:
-                pass
-            # from here on we create a list from the given keys by splitting
-            key_list = key_path.split(str_path_separator)
-            if len(key_list) == 1:  # single key this means the item was not found!
-                return []
-            if key_list[0] == '':
-                # we must ensure we start from the root
-                return self.root.find_all(key_list[1:], item_filter, str_path_separator, str_index_separator)
-            return self.find_all(key_list, item_filter, str_path_separator, str_index_separator)
-        # for those objects we do a direct search: (list is not in because in fnd we go deeper!!)
-        if t in (int, str, TagIdx, TagIdxStr, TagIdxBytes, TagMultiIdx, iTMatch, slice):
-            return self.__build_find_all_result(self.__getitem__(key_path, str_index_separator), item_filter)
-        # from here on we expect a list or iterator
-        # analyse iterator:
-        key, new_key_iter = self.__extract_first_iter_items(key_path)
-        # create the result of the key (first item)
-        if key is None:
-            # somethings wrong (empty iterator)
-            return []
-        if key == str_path_separator:
-            if key not in m:
-                # we switch up to root!
-                if new_key_iter is not None:
-                    return self.root.find_all(new_key_iter)
-                else:
-                    return self.__build_find_all_result(self.root, item_filter)
-        try:
-            result = self.__build_find_all_result(self.__getitem__(key, str_index_separator), item_filter)
-            if not result:
-                return []
-        except (IndexError, KeyError):
-            if type(key) is not str:
-                # we had no match on the object!
-                return []
-            if key[0] == '*':
-                if len(key) == 1:
-                    result = self.iter_children(item_filter=item_filter)
-                else:
-                    if key[1] == '*':
-                        if len(key) == 2:
-                            result = itertools.chain(self.__build_find_all_result(self, item_filter),
-                                                     self.iter_all(item_filter=item_filter))
-                        else:
-                            return []
-            else:
-                return []
-        if new_key_iter is None:
-            return result
-        else:
-            sub_method = lambda c, item: item.find_all(new_key_iter, item_filter,
-                                                       str_path_separator, str_index_separator)
-            # for debugging:
-            # results = [item.find_all(new_key_iter, item_filter,
-            #                          str_path_separator, str_index_separator) for item in result]
-            # return result
-            return itertools.chain.from_iterable(accu_iterator(result, sub_method))
-
-    def find_all2(self, key_path, item_filter=None, str_path_separator='/', str_index_separator='#',
-                  _initial=True):
-        """
-        Method is outdated use find_all instead!
-
-        The find_all function targets over multiple levels of the datatree, it returns a list or iterator of the
-        matching  items!
-
-        The key_path parameter given is normally a list. This can be a list of keys or TagIdx objects. The function
-        will search for the first item in the first level, fo next item in the next level and so on...
-
-        Absolut and relative key_paths:
-
-        If the first item is the separator (default: '/') the find search is like an absolute path and we start at the
-        root of the datatree.
-        If the first item is different, the key_path is relative and we start from the actual
-        item and search the children and sub-children.
-
-        Single string key_path:
-        If the user searches for string type tags he can use a string with a separator (default: '/') in between the
-        tags (These type of key_paths will be implicit translated in a list in the function). An index separator
-        (default = '#') in between the tag and the index can also be used to identify to identify items in the tag
-        family. If the key_path argument is already a list the single keys will not be parsed regarding the
-        str_path_separator anymore.
-
-        HINT: Quickest find operations can be performed by giving a list containing index integers or TagIdx objects
-
-        The items can be filtered regarding specific content, for this a look into the available filer constructors:
-        create_xxx_item_filter() might be interesting. The filter method or the filter constant can be given
-        in the item_filter parameter
-
-        The parameters in detail:
-
-        :param key_path: single key or list of keys
-                    identification path for the item/items to be searched.
-                    Possible keys:
-                    integer - behaves like normal __getitem__() -> itree_item[key]
-                    TagIdx- behaves like normal __getitem__() -> itree_item[key]
-                    iTreeTagSlice - select a tag sliced group of sub-elements
-                    iTMatch - search pattern can be used too, but keep in mind it must deliver a unique result!
-                    Slice - a slice of indexes (like a special index list)
-                    string - will be parsed by the separators
-                    iterable list/tuple/deque,... -
-                             run over single keys if sub_key is again an iterable it will be taken as an index list
-                             (e.g. [1,2,3] - will go deeper in the tree 1. item; 2. subitem; 3. subsubitem
-                             but [[1,2,3]] - will stay in the first level and deliver 1. item; 2. item; 3. item)
-
-        :param item_filter: filters the item content regarding NORMAL, TEMPORARY and LINKED flag or a given
-                            filtering method
-        :param str_path_separator: separator character in case of strings for the search levels (default: "/")
-        :param str_index_separator: separator character for given tag indexes (default: "#")
-        :param _initial: Internal flag that should protect against cyclic constructs
-        :return: list or iterator of matching iTrees; in case of no match and empty list is returned
-        """
-
-        t = type(key_path)
-        if t is str:
-            # empty key?
-            if len(key_path) == 0 or self.__len__() == 0:
-                # empty string
-                return []
-
-            # is string matching to a tag?
-            try:
-                items = self.__getitem__(key_path, str_index_separator=str_index_separator)
-                return self.__build_find_all_result(items,
-                                                    item_filter=item_filter)
-            except (KeyError, IndexError, ValueError):
-                pass
-            # we check some other quick exceptions:
-            if key_path.strip(' ') == '*':
-                return self.iter_children(item_filter=item_filter)
-            if key_path.strip(' ') == '**':
-                return self.iter_all(item_filter=item_filter)
-            # now we split based on separator
-            key_list = key_path.split(str_path_separator)
-            if key_list[0] == '':
-                # we must ensure we start from the root
-                return self.root.find_all(key_list[1:], item_filter, str_path_separator, str_index_separator)
-            if len(key_list) == 1:  # single key this means the item was not found!
-                return []
-            return self.find_all(key_list, item_filter, str_path_separator, str_index_separator)
-        # first we check we have a valid tag:
-        if (not _initial) or (t in (int, str, TagIdx, TagIdxStr, TagIdxBytes, TagMultiIdx, iTMatch, slice)):
-            # if not _initial we are in deeper level of the iterator and we interpret here as an index list!
-            items = self[key_path]
-            return self.__build_find_all_result(items,
-                                                item_filter=item_filter)
-        # If we reach this point we expect an iterable object as key_path
-        # that iterates deeper into the tree
-        key = None  # will be overwritten anyway
-        new_key_path = None
-        sub_iter = iter(key_path)
-        post_item = None
-        post_post_item = None
-        set_initial = False
-        try:
-            key = next(sub_iter)
-        except StopIteration:
-            # empty iterator!
-            return []
-        try:
-            post_item = next(sub_iter)
-            new_key_path = itertools.chain((post_item,), sub_iter)
-            try:
-                post_post_item = next(sub_iter)
-                # create a new iterator that contains the post items and the original iterator
-                new_key_path = itertools.chain((post_item, post_post_item), sub_iter)
-                set_initial = True
-            except StopIteration:
-                # there is only one item left in iterator we will give the item directly
-                # as key to the next level find()
-                new_key_path = post_item
-        except StopIteration:
-            pass
-        if key == str_path_separator:
-            if new_key_path is None:
-                # this is not possible we catch this already but we keep the code to complete the condition
-                if item_filter(self.root):
-                    return iter([self.root])
-                else:
-                    return []
-            if not _initial:
-                # cyclic construct we have to break!
-                return []
-            return self.root.find_all2(new_key_path,
-                                       item_filter,
-                                       str_path_separator,
-                                       str_index_separator,
-                                       _initial=set_initial
-                                       )
-        elif key == '*':
-            result = itertools.chain((self,), self.iter_children(item_filter=item_filter))
-        elif key == '**':
-            result = itertools.chain((self,), self.iter_all(item_filter=item_filter))
-        else:
-            result = self.find_all2(key, item_filter,
-                                    str_path_separator,
-                                    str_index_separator,
-                                    _initial=False)
-        # result can only be a single item
-        if new_key_path is None or result == []:
-            # we will not go deeper
-            return result
-        # iter into the next level
-        # We keep this for debugging proposes!
-        # results = [item.find_all(new_key_path,
-        #                         item_filter,
-        #                         str_path_separator,
-        #                         str_index_separator,
-        #                         _initial=set_initial) for item in result]
-        if True:
-            results = itertools.islice(
-                itertools.accumulate(
-                    itertools.chain((None,), result), lambda c, item: item.find_all(new_key_path,
-                                                                                    item_filter,
-                                                                                    str_path_separator,
-                                                                                    str_index_separator,
-                                                                                    _initial=set_initial)), 1, None,
-                1),  # python <3.8 no initial parameter
-        return itertools.chain.from_iterable(*results)
-
-    def find(self, key_path, item_filter=None, default_return=None, str_path_separator='/',
-             str_index_separator='#'):
-        """
-        The find function targets over multiple levels of the iTree, it returns single items only! This means in
-        case the key_path targets to multiple items the default_return will be given. If the key_path targets to a
-        family with only one item inside  or the item_filter extracts only one item in a family
-        the item will be given back as result. For multiple result utilize the `find_all()` method (which is slower).
-
-        .. note:: The method will deliver a default_return when ever in the whole key_path a match is not unique.
-                 This means iteration is stopped here and even that a deeper iteration with the defined filtering might
-                 deliver at least a unique result. To ensure to find this deeper results you must utilize the slower
-                 `find_all()` method.
-
-        The key_path parameter given is normally a list. This can be a list of keys or TagIdx objects. The function
-        will search for the first item in the first level, fo next item in the next level and so on...
-
-        Absolut and relative key_paths:
-
-        If the first item is the separator (default: '/') the find search is like an absolute path and we start at the
-        root of the iTree. For compatibility reasons with find_all we accept  a leading "./"
-        (or to be exact: ".%s"#str_path_separator) as absolute path indicator.
-        If the first item is different, the key_path is relative and we start from the actual
-        item and search the children and sub-children.
-
-        Single string key_path:
-        If the user searches for string type tags he can use a string with a separator (default: '/') in between the
-        tags (Those key_paths will be implicit translated in a list). An index separator (default = '#') in between
-        the tag and the index can also be used in this case. If the argument is already a list the single keys will not
-        be parsed regarding the str_path_separator.
-
-        .. note:: If iTree contains tags with characters that used for separators or the all match '*' character
-              the find() result might contain that tagged item instead of the expected separated or wildcard match.
-
-        .. note:: Quickest find operations can be performed by giving a list containing index integers or TagIdx objects
-
-        The parameters in detail:
-
-        :param key_path: single key or list of keys
-                    identification path for the item/items to be searched.
-                    Possible keys:
-                    integer - behaves like normal __getitem__() -> itree_item[key]
-                    TagIdx- behaves like normal __getitem__() -> itree_item[key]
-                    iTreeTagSlice - select a tag sliced group of sub-elements
-                    iTMatch - search pattern can be used too, but keep in mind it must deliver a unique result!
-                    Slice - a slice of indexes (like a special index list)
-                    string - will be parsed by the separators, special string '*" is as interpreted as any match
-                    iterable list/tuple/deque,... -
-                             run over single items
-
-        :param item_filter: filters the item content regarding NORMAL, TEMPORARY and LINKED flag or a given
-                            filtering method
-
-        :param default_return: object will be return in case of no match (default = None)
-
-        :param str_path_separator: separator character in case of strings for the search levels (default: "/")
-
-        :param str_index_separator: separator character for given tag indexes (default: "#")
-
-        :return: iTree single item
-        """
-        # internally we use the find_all() to get a list of items
-        # and than return single match or default_return depending on result items
-
-        result = self.find_all(key_path, item_filter=item_filter,
-                               str_path_separator=str_path_separator,
-                               str_index_separator=str_index_separator)
-        # here we check if the iterator contains a unique item:
-        item_iter = iter(result)
-        try:
-            item = next(item_iter)
+        :param other:
+        :return:
+        """
+        new = self.copy()
+        if self.tag == other.tag:
+            new._tag = NoTag
+        else:
             try:
-                next(item_iter)
-                # no StopIteration Exception! more then one element we return no match
-                return default_return
-            except (TypeError, StopIteration):
-                # match!
-                return item
-        except StopIteration:
-            # empty iterator!
-            return default_return
-
-    def index(self, item, item_filter=None):
-        """
-        The index method allows to search for the index of the item in a parent object
-        This is especially useful if you must use a item_filter. The delivered index is delivered relative
-        to the given item filter!
-
-        For the item index of the item in the unfiltered tree (ALL) it's recommended
-        to use the idx property instead: `(parent.index(item,ALL) == item.idx)`
-
-        :param item: item index should be delivered for
-
-        :param item_filter: filter integer; method can not handle filter methods yet!
-
-        :return: index integer of the item relative to the given filter
-        """
-        if type(item) in {int, TagIdx}:
-            item = self.__getitem__(item)
-        if item.parent is not self:
-            raise LookupError('Given item is not children of this iTree!')
-        if item_filter is None:
-            return super().index(item)
+                new._tag = new._tag - other._tag
+            except Exception:
+                t = type(new._tag)
+                t2 = type(other._tag)
+                if t == t2:
+                    if t is str:
+                        new._tag = new._tag.replace(other._tag, '')
+                    if t is bytes:
+                        new._tag = new._tag.replace(other._tag, b'')
+        if self._value_equal(self.value, other.value):
+            new._value = NoValue
         else:
-            for i, sibling in self.iter_children(item_filter=item_filter):
-                if sibling == item:
-                    return i
-
-    # serialize + file operations
+            try:
+                new._value = new._value - other._value
+            except Exception:
+                t = type(new._value)
+                t2 = type(other._value)
+                if t == t2:
+                    if t is str:
+                        new._value = new._value.replace(other._value, '')
+                    if t is bytes:
+                        new._value = new._value.replace(other._value, b'')
+        # This code might be improved!
+        del_idx = []
+        for item in other:
+            key = item.tag_idx
+            if key in new and new[key] == item:
+                del_idx.append(new[key].idx)
+                continue
+            new[key] = new[key] - item
+        for i in reversed(del_idx):  # we delete from the end if not the index would change after deleting first one
+            del new[i]
+        return new
 
-    def load_links(self, force=False, delete_invalid_items=False):
+    def __add__(self, other):
         """
-        Runs ove all children and sub children in case a ITreeLink object is found the linked items are load in
-
-        :param force: True - linked items will be reloaded even that they are already loaded
+        If two iTree objects are added the children in the two added iTrees are copied and combined
+        to a new iTree object the other attributes are taken over from the first iTree in the given sum.
 
-        :param delete_invalid_items: In case a iTreeLink refers to an invalid item (internal exception) the related
-                                     iTreeLink object will be deleted from teh tree
+        :param other: iTree object that should be added
+        :return: New iTree object containing copies of all children
         """
-        for i in self.iter_all(item_filter=iTFilterItemType(iTreeLink)):
-            i.load_links(force=force, delete_invalid_items=delete_invalid_items)
-        # the following better code is is not working, don't know why?:
-        # (i.load_links() for i in self.iter_all(item_filter=self.create_item_type_filter(iTreeLink)))
+        if hasattr(other, '_itree_prt_idx'):
+            if self.is_link_root:
+                raise TypeError('__add__() on link-root items is not supported')
+            return iTree(copy.copy(self._tag), copy.copy(self._value),
+                         subtree=chain((item.__copy__() for item in self),
+                                       (item.__copy__() for item in other)), flags=self._flags)
+        else:
+            raise TypeError('Added item is not of type iTree')
 
-    def loads(self, data_str, check_hash=True, load_links=True):
+    def __copy__(self):
         """
-        create an iTree object by loading from a string
-
-        If not overloaded or reinitialized the iTree Standard Serializer will be used. In this case we expect a
-        matching JSON representation.
+        create a copy of this item
 
-        :param data_str: source string that contains the iTree information
+        The difference in between copy and deepcopy for iTree is just that we do in deepcopy a copy
+        of all data items too. In copy we just copy the iTData object not the items itself, they stay as pointers
+        to the original objects.
 
-        :param check_hash: True the hash of the file will be checked and the loading will be stopped if it doesn't match
-                           False - do not check the iTree hash
+        The operation is very important for `iTree`-class because of the one parent only principle we are forced to
+        do a copy of all sub-items (in-depth). It's not possible to copy just the top-level element only.
 
-        :param load_links: True - linked iTree objects will be loaded
+        The function is used internally in extend operations too. And we can see (profiler) that
+        improvements in this method have big impact.
 
-        :return: iTree object loaded from file
+        :return: copied iTree object
         """
-        if (not hasattr(self, '_def_serializer')) or (self._def_serializer is None):
-            self.init_serializer()
-        return self._def_serializer[1].loads(data_str, check_hash=check_hash, load_links=load_links)
+        return self._iter_copy(self, iTree._get_copy_args)
 
-    def load(self, file_path, check_hash=True, load_links=True):
+    def copy_keep_value(self):
         """
-        create an iTree object by loading from a file
+        Create a copy of this item.
 
-        If not overloaded or reinitialized the iTree Standard Serializer will be used. In this case we expect a
-        matching JSON representation.
+        The difference in between normal `copy()` and this method is that the value objects are
+        completely untouched in this operation (for immutable objects there is no difference
+        in between the two copy operations).
 
-        :param file_path: file path to the file that contains the iTree information
+        :return: copied iTree object
+        """
+        return self._iter_copy(self, iTree._get_args_skip_subtree)
 
-        :param check_hash: True the hash of the file will be checked and the loading will be stopped if it doesn't match
-                           False - do not check the iTree hash
+    def copy(self, *args, **kwargs):
+        """
+        create a copy of this item
 
-        :param load_links: True - linked iTree objects will be loaded
+        The difference in between `copy()` and `deepcopy()` for `iTree` is just that we do in `deepcopy()` a deepcopy
+        of all value items. In `copy()` we just copy the value object not the items inside, the pointers
+        to the original objects are kept (for immutable objects there is no difference).
 
-        :return: iTree object loaded from file
+        :return: copied iTree object
         """
-        if (not hasattr(self, '_def_serializer')) or (self._def_serializer is None):
-            self.init_serializer()
-        return self._def_serializer[1].load(file_path, check_hash=check_hash, load_links=load_links)
+        return self._iter_copy(self, iTree._get_copy_args)
 
-    def dumps(self, calc_hash=True):
+    def __deepcopy__(self, *args, **kwargs):
         """
-        serializes the iTree object to JSON (default serializer)
+        create a deepcopy of this item
 
-        :param calc_hash: Tell if the hash should be calculated and stored in the header of string
+        The difference in between `copy()` and `deepcopy()` for `iTree` is just that we do in `deepcopy()` a deepcopy
+        of all value items. In `copy()` we just copy the value object not the items inside, the pointers
+        to the original objects are kept (for immutable objects there is no difference).
 
-        :return: serialized string (JSON in case of default serializer)
+        :return: deep copied new iTree object
         """
-        if (not hasattr(self, '_def_serializer')) or (self._def_serializer is None):
-            self.init_serializer()
-        return self._def_serializer[0].dumps(self, calc_hash=calc_hash)
+        return self._iter_copy(self, iTree._get_deepcopy_args)
 
-    def dump(self, target_path, pack=True, calc_hash=True, overwrite=False):
+    def deepcopy(self, *args, **kwargs):
         """
-        serializes the iTree object to JSON (default serializer) and store it in a file
+        create a deepcopy of this item
 
-        :param target_path: target path of the file where the iTree should be stored in
-        :param pack: True - data will be packed via gzip before storage
-        :param calc_hash: True - create the hash information of iTree and store it in the header
-        :param overwrite: True - overwrite an existing file
-        :return: True if file is stored successful
+        The difference in between `copy()` and `deepcopy()` for `iTree` is just that we do in `deepcopy()` a deepcopy
+        of all value items. In `copy()` we just copy the value object not the items inside, the pointers
+        to the original objects are kept (for immutable objects there is no difference).
+
+        :return: deep copied new iTree object
         """
-        if (not hasattr(self, '_def_serializer')) or (self._def_serializer is None):
-            self.init_serializer()
-        return self._def_serializer[0].dump(self, target_path, pack=pack, calc_hash=calc_hash, overwrite=overwrite)
+        return self._iter_copy(self, iTree._get_deepcopy_args)
+
+    # *** size & comparisons *******************************************************************************************
+
+    # __len__() of the super-class blist is not overloaded!
 
-    def renders(self, item_filter=None):
+    def filtered_len(self, filter_method):
         """
-        render the iTree into a string
+        Calculates the number of filtered children.
 
-        :param item_filter: the items can be filtered by giving a filter constants or giving a filter method or
-                            iTFilter object
+        :type filter_method: Callable
+        :param filter_method: filter method that checks for matching items
+                            and delivers `True`/`False`.
+                            The filter_method targets always the `iTree`-child-object and checks a characteristic
+                            of this object for matches (see :ref:`filter_method <filter_method>`)
 
-        :return: Tree representation as string
+        :rtype: int
+        :return: Number of matching items found
         """
-        if (not hasattr(self, '_def_serializer')) or (self._def_serializer is None):
-            self.init_serializer()
-        return self._def_serializer[3].renders(self, item_filter)
+        return sum(1 for _ in filter(filter_method, self))
 
-    def render(self, item_filter=None):
+
+    def __contains__(self, target):
         """
-          print the rendered the iTree string to the terminal
+        Checks if an ´iTree´ object is part of the ´iTree´
+        for comparison == -> ´__eq__()´ is used. For finding a specific object use ´is_parent()´ or 'is_in()` instead.
+        
+        In case no ´iTree´ object is given the function uses ´__getitem__´ to check 
+        if matching item(s) exists.
 
-          :param item_filter: the items can be filtered by giving a filter constants or giving a filter method or
-                              iTFilter object
-          """
+        .. note:: There is no coresponding in-depth function available the user can easy search via:
+                     >>> # Let itree be the iTree object the target should be searched in
+                     >>> any(tag == i.tag for i in itree.deep)
+                     >>> any(searchkey == i[0][-1] for i in itree.deep.tag_idx_paths())
+                     >>> s=len(index_list)
+                     >>> any(len(i[0])>s and index_list == i[0][(-s+1):] for i in itree.deep.idx_paths())
 
-        if (not hasattr(self, '_def_serializer')) or (self._def_serializer is None):
-            self.init_serializer()
-        return self._def_serializer[3].render(self, item_filter)
 
-    # helpers
-    def _load_subtree(self, extend_items):
+        :param target: iTree object searched for or a target used by ´__getitem__()´ method
+        :return:
+                * True - matching child is found
+                * False - no matching item found
         """
-        We extend the iTree with given items (multi append)
-
-        :note: In case the extend items have already a parent an implicit copy will be made. We do this because
-               we might get an iTree-object as extend_items parameter and then the children will have automatically a
-               parent even that the parent object might be a temporary one.
+        if hasattr(target, '_itree_prt_idx'):
+            for child in self:
+                if child == target:
+                    return True
+        else:
+            with suppress(Exception):
+                item = self.__getitem__(target)
+                if not hasattr(item, '_itree_prt_idx'):
+                    next(item)
+                return True
+        return False
 
-        :param extend_items: iterable object that contains iTree objects as items
-        :return: True
+    def is_tag_in(self, tag):
         """
-        # collect for operation
-        sl = super()
-        m = self._map
-        idx = sl.__len__() - 1
-        for item in extend_items:
-            if item is None:
-                continue
-            if item._parent is not None:  # and (parent != self):
-                item = item.__copy__()
-            item._parent = self
-            tag = item._tag
-            idx += 1
-            sl.append(item)
-            try:
-                if m.__contains__(tag):
-                    family = m.__getitem__(tag)
-                    item._cache = (idx, family.__len__())
-                    family.append(item)
-                else:
-                    item._cache = (idx, 0)
-                    m.__setitem__(tag, blist((item,)))
-            except AttributeError:
-                item._cache = (idx, 0)
-                self._map = m = {tag: blist((item,))}
-        return True
-
-    def __get_family_insertion_idx(self, family, item_idx, last_index=0):
-        fl = len(family)
-        if fl == 1:
-            if family[0].idx < item_idx:
-                return 1 + last_index
-            else:
-                return last_index
-        i = round(fl / 2)
-        idx = family[i].idx
-        if idx < item_idx:
-            return self.__get_family_insertion_idx(family[i:], item_idx, last_index + i)
-        else:
-            return self.__get_family_insertion_idx(family[:i], item_idx, last_index)
-
-    def __unsupport_op(self, *args, **kwargs):
-        raise TypeError('unsupported operand or function in iTree')
-
-    @property
-    def __read_only_struct_exception_property(self):
-        raise PermissionError('The iTree element is read_only (linked or read_only flag)!')
-
-    # find helper methods for different types of keys
-
-    def __extract_first_iter_items(self, iterator):
-        """
-        analysis the iterator
-        :param iterator: iterator to be analysed
-        :return: tuple  -> (None,None,None) -> empty iterator
-                        -> (first_item,None,None) -> last element of iterator (no elements left afterwards)
-                        -> (first_item,second_item,None) -> last two elements of iterator (no elements left afterwards)
-                        -> (first_item,None,rest_iteratorNone) -> first item and the rest of the iterator
-                           (without first item)
-        """
-        # iterator/generator
-        if hasattr(iterator, '__len__'):
-            l1 = len(iterator)
-            if l1 == 0:
-                return None, None
-            elif l1 == 1:
-                return iterator[0], None
-            else:
-                return iterator[0], iterator[1:]
-        else:
-            try:
-                i1 = next(iterator)
-            except StopIteration:
-                return None, None
-            try:
-                i2 = next(iterator)
-                return i1, itertools.chain((i2,), iterator)
-            except StopIteration:
-                return i1, None
-
-    def __build_find_all_result(self, result, item_filter=None):
-        """
-        helper function for find method
-        :param result: result found by the key
-        :param item_filter: filter
-        :return: final result
-        """
-        if isinstance(result, iTree):
-            if item_filter is None:
-                return iter((result,))
-            elif item_filter(result):
-                return iter((result,))
-            else:
-                return []
-        if not result:  # != []
-            return result
-        if item_filter is None:
-            return result
-        return filter(lambda item: item_filter(item), result)
-
-    def __find_single_item(self, key_path, item_filter=None):
-        """
-        find normal item via __getitem__ in the children
-        :param key_path: key
-        :param item_filter: filter method
-        :return: list with one item
+        Checks if a iTree contains the given family-tag (first-level only)
+        :param tag: family tag
+        :return: True/False
         """
-        try:
-            item = self.__getitem__(key_path)
-        except (KeyError, IndexError):
-            return []
-        return self.__build_find_all_result(item, item_filter)
-
-    def __find_tag_slice(self, tag_slice, item_filter=None):
-        idx = tag_slice.idx  # slice!?
-        if idx is int:
-            return self.__find_single_item(key_path=tag_slice, item_filter=item_filter)
-        tag = tag_slice.tag
-        try:
-            family = self._map[tag]
-        except KeyError:
-            return []
-        return itertools.islice(self.__build_find_all_result(family, item_filter=item_filter), idx.start, idx.stop,
-                                idx.step)
+        if self:
+            return tag in self._families
+        else:
+            return False
 
-    def __find_slice(self, slice_obj, item_filter=None):
-        return itertools.islice(self.iter_children(item_filter=item_filter), slice_obj.start, slice_obj.stop,
-                                slice_obj.step)
+    def is_in(self, item):
+        """
+        Checks if the given object is child of the iTree.
+        Different to ´__contains__()´ we check here for the instance (specific) object (is)
+        and not based on ´__eq__()´.
 
-    def __find_set(self, set_obj, item_filter=None):
-        return filter(lambda item: item.idx in set_obj, self.iter_children(item_filter=item_filter))
+        :param item: iTree object to be searched for
+        :return:
+                * True - matching child is found
+                * False - no matching item found
+        """
+        if hasattr(item, '_itree_prt_idx'):
+            p = item._itree_prt_idx
+            return p is not None and p[0] is self
+        else:
+            raise TypeError('Given item is not of type iTree')
 
-    def __find_match(self, match, item_filter=None):
-        return filter(lambda item: match.check(item)[0], self.iter_children(item_filter=item_filter))
+    def __eq__(self, other):
 
+        """
+        compares if the tag, value and children content of another item matches with this item
 
-class iTreeReadOnly(iTree):
-    """
-    This iTree object is read only the initial parameters given cannot be changed the object remains
-    static in the tree and can only be changed when deleted and replaced
-    """
-    _is_read_only = True
-    _is_temporary = False
-    _is_placeholder = False
-    _is_linked = False
+        .. note::
 
-    __slots__ = (
-        '_tag', '_parent', '_map', '_coupled', '_data', '_cache', '_def_serializer')
+                If you like to check if it is really the same object you should use ´is´ instead of ´==´ operator
 
-    def __init__(self, tag, data=None, subtree=None, freeze_struct_only=False):
-        if freeze_struct_only:
-            if data is None:
-                data = iTDataReadOnly()
-            else:
-                data = iTDataReadOnly(data)
-        if subtree is None:
-            super(iTreeReadOnly, self).__init__(tag, data)
-        else:
-            super(iTreeReadOnly, self).__init__(tag, data, [iTreeReadOnly(item.tag,item.data,subtree=item) for item in subtree])
+        :param other: other iTree
 
-    # block all setting commands
-    def __setitem__(self, *args, **kwargs):
-        """
-        :except: PermissionError not possible on iTreeReadOnly objects
+        :return: boolean match result (True match/False no match)
         """
-        raise PermissionError('The iTreeReadOnly element is read_only (linked or read_only flag)!')
+        if self is other:
+            return True
+        try:
+            if self._tag != other._tag or \
+                    len(self) != len(other) or \
+                    not self._value_equal(self._value, other._value):
+                return False
+            for i, ii in zip(self.deep, other.deep):
+                try:
+                    a1 = i.get_init_args(None, False)
+                    a2 = ii.get_init_args(None, False)
+                    if a1 == a2:
+                        # quick compare might fail because of the value
+                        continue
+                    if self._value_equal(a1[1], a2[1]):
+                        continue
+                    return False
+                except AttributeError:
+                    return False  # None
+                except Exception:
+                    if not self._value_equal(a1[1], a2[1]):
+                        return False
+                    elif a1[0] != a2[0]:
+                        return False
+                    elif len(a1) > 2 and a1[2:] != a2[2:]:
+                        return False
+            return True
+        except Exception:
+            return False
 
-    def __delitem__(self, *args, **kwargs):
+    def __ne__(self, other):
         """
-        :except: PermissionError not possible on iTreeReadOnly objects
+        This is just the inverse operation of __eq__
+        :param other: other item to be compared with
+        :return: True/False
         """
-        raise PermissionError('The iTreeReadOnly element is read_only (linked or read_only flag)!')
+        return not self.__eq__(other)
 
-    def __iadd__(self, *args, **kwargs):
+    def __lt__(self, other):
         """
-        :except: PermissionError not possible on iTreeReadOnly objects
+        less than is a size comparison (length are compared)
+        :param other: iTree object self should be compared with
+        :return: True/False
         """
-        raise PermissionError('The iTreeReadOnly element is read_only (linked or read_only flag)!')
+        return len(self) < len(other)
 
-    def insert(self, *args, **kwargs):
+    def __le__(self, other):
         """
-        :except: PermissionError not possible on iTreeReadOnly objects
+        less than or equal is a size comparison (length are compared)
+        :param other: iTree object self should be compared with
+        :return: True/False
         """
-        raise PermissionError('The iTreeReadOnly element is read_only (linked or read_only flag)!')
+        return len(self) <= len(other)
 
-    def append(self, *args, **kwargs):
+    def __gt__(self, other):
         """
-        :except: PermissionError not possible on iTreeReadOnly objects
+        greater than is a size comparison (length are compared)
+        :param other: iTree object self should be compared with
+        :return: True/False
         """
-        raise PermissionError('The iTreeReadOnly element is read_only (linked or read_only flag)!')
+        return len(self) > len(other)
 
-    def appendleft(self, *args, **kwargs):
+    def __ge__(self, other):
         """
-        :except: PermissionError not possible on iTreeReadOnly objects
+        greater than or equal is a size comparison (length are compared)
+        :param other: iTree object self should be compared with
+        :return: True/False
         """
-        raise PermissionError('The iTreeReadOnly element is read_only (linked or read_only flag)!')
+        return len(self) >= len(other)
 
-    def extend(self, *args, **kwargs):
-        """
-        :except: PermissionError not possible on iTreeReadOnly objects
+    def equal(self, other, check_coupled=False, check_flags=False):
         """
-        raise PermissionError('The iTreeReadOnly element is read_only (linked or read_only flag)!')
+        compares if the data content of another item matches with this item
 
-    def extendleft(self, *args, **kwargs):
-        """
-        :except: PermissionError not possible on iTreeReadOnly objects
-        """
-        raise PermissionError('The iTreeReadOnly element is read_only (linked or read_only flag)!')
+        :param other: other iTree
 
-    def rotate(self, *args, **kwargs):
-        """
-        :except: PermissionError not possible on iTreeReadOnly objects
-        """
-        raise PermissionError('The iTreeReadOnly element is read_only (linked or read_only flag)!')
+        :param check_coupled: check the couple object too? (Default False)
 
-    def reverse(self, *args, **kwargs):
-        """
-        :except: PermissionError not possible on iTreeReadOnly objects
-        """
-        raise PermissionError('The iTreeReadOnly element is read_only (linked or read_only flag)!')
+        :param check_flags: check the flags of the objects? (Default False)
 
-    def pop(self, *args, **kwargs):
-        """
-        :except: PermissionError not possible on iTreeReadOnly objects
+        :return: boolean match result (True match/False no match)
         """
-        raise PermissionError('The iTreeReadOnly element is read_only (linked or read_only flag)!')
 
-    def popleft(self, *args, **kwargs):
-        """
-        :except: PermissionError not possible on iTreeReadOnly objects
-        """
-        raise PermissionError('The iTreeReadOnly element is read_only (linked or read_only flag)!')
+        if self is other:
+            return True
 
-    def remove(self, *args, **kwargs):
-        """
-        :except: PermissionError not possible on iTreeReadOnly objects
+        if check_flags:
+            check1 = lambda i, ii: i._flags == ii._flags
+        else:
+            check1 = lambda i, ii: True
+
+        if check_coupled:
+            check2 = lambda i, ii: (hasattr(i, '_coupled') and hasattr(ii, '_coupled')) and \
+                                   i._coupled is ii._coupled if (hasattr(i, '_coupled') or hasattr(ii, '_coupled')) \
+                else True
+        else:
+            check2 = lambda i, ii: True
+        check = lambda i, ii: check1(i, ii) and check2(i, ii)
+        if not check(self, other):
+            return False
+        try:
+            if self._tag != other._tag or \
+                    len(self) != len(other) or \
+                    not self._value_equal(self._value, other._value):
+                return False
+            for i, ii in zip(self.deep, other.deep):
+                if not check(i, ii):
+                    return False
+                a1 = i.get_init_args(None, False)
+                a2 = ii.get_init_args(None, False)
+                try:
+                    if a1 == a2:
+                        # quick compare might fail because of the value
+                        continue
+                    if self._value_equal(a1[1], a2[1]):
+                        continue
+                    return False
+                except Exception:
+                    if not self._value_equal(a1[1], a2[1]):
+                        return False
+                    elif a1[0] != a2[0]:
+                        return False
+                    elif len(a1) > 2 and a1[2:] != a2[2:]:
+                        return False
+            return True
+        except Exception:
+            return False
+
+    def count(self, item):
         """
-        raise PermissionError('The iTreeReadOnly element is read_only (linked or read_only flag)!')
+        Counts how many equal (`==`) children are in the `iTree`-object.
+
+        :type item: iTree
+        :param item: The `iTree`-items will be compared with this item
 
-    def clear(self):
+        :rtype: int
+        :return: Number of matching items found
+        """
+        return sum(item == i for i in self)
+
+    def index(self, item, start=None, stop=None):
+        """
+        The index method allows to search for the absolute index of a matching item in the `iTree`.
+        The item must be a iTree object and the index will deliver the first match. The comparison is made via
+        `==` operator.
+
+        If item is not found a IndexError will be raised
+
+        .. note:: To get the index of a specific item instance the `.idx`- property
+                  should be used.
+
+        :type item: iTree
+        :param item: iTree object to be searched for
+
+        :type start: Union[iTree,target_path]
+        :param start: iTree item or start target_path where index search should be started (start item is included in search)
+
+        :type stop: Union[iTree,target_path]
+        :param stop: iTree item or stop target_path  where index search should be stopped (stop item is not included in search)
+
+        ;rtype: int
+        :return: absolute index of the found item
+        """
+        if self:
+            iterator = self.__iter__()
+            if start is not None:
+                if not hasattr(start, '_itree_prt_idx'):
+                    start = self.get.single(start)
+                try:
+                    first_item = next(dropwhile(lambda i: i is not start, iterator))
+                    if first_item == item:
+                        return first_item.idx
+                except StopIteration:
+                    raise IndexError('No matching item found in iTree')
+            if stop is not None:
+                if not hasattr(stop, '_itree_prt_idx'):
+                    stop = self.get.single(stop)
+                try:
+                    item = next(dropwhile(lambda i: i is not stop and i != item, iterator))
+                    if item is not stop:
+                        return item.idx
+                    raise StopIteration
+                except StopIteration:
+                    raise IndexError('No matching item found in iTree')
+            else:
+                try:
+                    item = next(dropwhile(lambda i: i != item, iterator))
+                    return item.idx
+                except StopIteration:
+                    raise IndexError('No matching item found in iTree')
+
+    def __hash__(self):
         """
-        :except: PermissionError not possible on iTreeReadOnly objects
+        The hash operation is available
+
+        .. node::As for the `==` operator we do not consider, parent, coupled items or flags properties of the object
+
+        :return: integer hash
         """
-        raise PermissionError('The iTreeReadOnly element is read_only (linked or read_only flag)!')
+        try:
+            h = hash(self._value)
+        except TypeError:
+            h = hash(pickle.dumps(self._value))
+        return hash((tuple(self), self._tag, h))
 
-    def __repr__(self):
+    # *** ITERATORS ****************************************************************************************************
+
+    # standard iterators list/dict
+
+    # def __iter__(self): #use function of the super class!
+
+    # dict like iterators:
+
+    def keys(self, filter_method=None):
         """
-        create representation string from which the object can be reconstructed via eval (might not work in case of
-        data that do not have a working repr method)
-        :return: representation string
+        Iterates over all children and deliver the children tag-idx tuple (family-tag,family_index)
+
+        .. note::
+            This is a dict like iterator that delivers the unique keys for all children.
+
+        :type filter_method: Union[Callable,None]
+        :param filter_method: filter method that checks the item
+                            and delivers `True`/`False`.
+                            The filter_method targets always the `iTree`-child-object and checks a characteristic
+                            of this object for matches
+
+                            If `None` is given filtering is inactive.
+
+        :rtype: Iterator
+        :return: iterator over the tag-idx of the children
         """
-        repr_str = 'iTreeReadOnly("%s"' % (repr(self._tag))
-        if not self._data.is_empty:
-            if self._data.is_no_key_only:
-                repr_str = repr_str + ', data=%s' % repr(self._data[__NOKEY__])
-            else:
-                repr_str = repr_str + ', data=%s' % repr(self._data)
-            subtree = super(iTree, self).__repr__()
-            if subtree[0] == 'b':
-                # we shorten blist from definition
-                subtree = subtree[6:-1]
-            return repr_str + ', subtree=%s)' % subtree
-        else:
-            return repr_str + ')'
-
-
-class iTreeTemporary(iTree):
-    """
-    This is a temporary item that will not be considered if the iTree is saved into a file.
-    """
-    _is_read_only = False
-    _is_temporary = True
-    _is_placeholder = False
-    _is_linked = False
+        tag_cnts = {tag: -1 for tag in self._families.keys()}
+        if filter_method:
+            for item in self:
+                tag = item._tag
+                # as side effect we update the item cache too:
+                item._itree_prt_idx[2] = tag_cnts[tag] = cnt = tag_cnts[tag] + 1
+                if filter_method(item):
+                    yield tag, cnt
+        else:
+            for item in self:
+                tag = item._tag
+                item._itree_prt_idx[2] = tag_cnts[tag] = cnt = tag_cnts[tag] + 1
+                yield tag, cnt
 
-    def __repr__(self):
+    def values(self, filter_method=None):
         """
-        create representation string from which the object can be reconstructed via eval (might not work in case of
-        data that do not have a working repr method)
-        :return: representation string
+        Iterates over all children and deliver the children values
+
+        :type filter_method: Union[Callable,None]
+        :param filter_method: filter method that checks for matching items
+                            and delivers `True`/`False`.
+                            The filter_method targets always the `iTree`-child-object and checks a characteristic
+                            of this object for matches (see :ref:`filter_method <filter_method>`)
+
+                            If `None` is given filtering is inactive.
+
+        :rtype: Iterator
+        :return: iterator over the values stored in the children
         """
-        repr_str = 'iTreeTemporary("%s"' % (repr(self._tag))
-        if not self._data.is_empty:
-            if self._data.is_no_key_only:
-                repr_str = repr_str + ', data=%s' % repr(self._data[__NOKEY__])
-            else:
-                repr_str = repr_str + ', data=%s' % repr(self._data)
-            subtree = super(iTree, self).__repr__()
-            if subtree[0] == 'b':
-                # we shorten blist from definition
-                subtree = subtree[6:-1]
-            return repr_str + ', subtree=%s)' % subtree
-        else:
-            return repr_str + ')'
-
-
-class iTreeLink(iTree):
-    """
-    This class is used to define linked subtrees in a iTree object.
-    The target source can be a subtree in another iTree related file (external links) or
-    internal links to a subtree of the already loaded subtree.
-
-    Linking has some functional limitations so is it not allowed to link to already linked objects
-    (we must protect iTree from circular definitions).
-
-    The iTreeLink objects supports local items which can be added additional to the linked items.
-    Furthermore there is also a mechanism so that local items can overlay the linked items in the tree. This is done
-    by localizing the linked items with the `make_child_local()` or `make_self_local()` method. Afterwards the item can
-    be manipulated as a normal iTree object. Only exception is that after deleting such a overlaying item the linked
-    item will come back into the iTree.
-
-    """
-
-    _is_read_only = False
-    _is_temporary = False
-    _is_placeholder = False
-    _is_linked = True
-
-    __slots__ = (
-        '_tag', '_parent', '_map', '_data', '_cache', '_def_serializer', '_link')
-
-    def __init__(self, tag, data=None, subtree=None, link_file_path=None, link_key_path=None, load_links=True):
-        t = type(tag)
-        if t is int or t is TagIdx:
-            raise TypeError('Given tag cannot be used in iTree wrong type (int or TagIdx)')
-        else:
-            self._tag = tag
-
-        super(iTreeLink, self).__init__(tag, data, subtree=subtree)
-
-        if link_file_path is not None or link_key_path is not None:
-            self._link = iTLink(link_file_path, link_key_path)
-            if load_links:
-                self.load_links()
+        if filter_method:
+            for item in filter(filter_method, self):
+                yield item._value
         else:
-            self._link = None
+            for item in self:
+                yield item.value
 
-    def __setitem__(self, key, item):
+    def items(self, filter_method=None, values_only=False):
         """
+        Iterates over all children and deliver the children
+        item-tuples (key,item) or (key,value). As key we use the unique tag-idx: (tag-family,family-index).
+
+        The function is comparable with dicts `items()` function.
 
-        :except: PermissionError will be raised if the parent is not the root linked element
-                 PermissionError will be raised if target is a linked element
-                 TypeError if given item is temporary (not supported)
 
-        :param key: single identifier for the item can be integer index or TagIdx
+        :type filter_method: Union[Callable,None]
+        :param filter_method: filter method that checks for matching items
+                            and delivers `True`/`False`.
+                            The filter_method targets always the `iTree`-child-object and checks a characteristic
+                            of this object for matches (see :ref:`filter_method <filter_method>`)
 
-        :param item: item to be placed in iTree
+                            If `None` is given filtering is inactive.
 
+        :type values_only: bool
+        :param values_only:
+                    * `False` (default) - in the key,value tuple the iterator put the iTree object as value in
+                    * `True` - in the key,value tuple the iterator put "only" the value object of the `iTree`-object in
+
+        :rtype: Generator
+        :return: iterator over the target keys and item value of the children
         """
-        if self._parent is not None:
-            if self._parent._is_linked:
-                raise PermissionError('The parent is read_only (linked)!')
-        if item._is_temporary:
-            raise TypeError('Given item is temporary and we cannot add temporary items as locals in a linked tree')
-        try:
-            old_item = super().__getitem__(key)
-        except (KeyError, IndexError):
-            return super().__setitem__(key, item)
-        if old_item._is_linked:
-            raise PermissionError('The target element is read_only (linked)!')
-        else:
-            return super().__setitem__(key, item)
-
-    def __delitem__(self, key):
-        """
-        delete a child item in the tree (only on local items)
-
-        :except: Method will raise a PermissionError if delete is done on a linked item
-
-        :param key: single identifier for the item can be integer index or TagIdx for item to be deleted
-
-        :return: deleted item will be returned
-        """
-        if self._parent is not None:
-            if self._parent._is_linked:
-                raise PermissionError('The parent is read_only (linked)!')
-        item = self.__getitem__(key)
-        if isinstance(item, iTree):
-            if item._is_linked:
-                raise PermissionError('The target element is read_only (linked)!')
-            else:
-                # maybe the deleted local item must be replaced by a linked item:
-                if item._link is not None:
-                    if item._link._link_item is not None:
-                        super().__setitem__(item.tag_idx, item._link._link_item)
-                        return item
-            # else no overloaded item we just delete
-            return super().__delitem__(item.idx)
-        else:
-            if key in self._map:
-                del_items = []
-                for item in self._map[key]:
-                    del_items.append(item)
-                    self.__delitem__(item.idx)
-                return del_items
+        tag_cnts = {tag: -1 for tag in self._families.keys()}
+        if values_only:
+            if filter_method:
+                for item in self:
+                    tag = item._tag
+                    # as side effect we update the item cache too:
+                    item._itree_prt_idx[2] = tag_cnts[tag] = cnt = tag_cnts[tag] + 1
+                    if filter_method(item):
+                        yield (tag, cnt), item.value
             else:
-                raise KeyError('Given key not found in iTree object, delete not possible')
+                for item in self:
+                    tag = item._tag
+                    item._itree_prt_idx[2] = tag_cnts[tag] = cnt = tag_cnts[tag] + 1
+                    yield (tag, cnt), item.value
+        elif filter_method:
+            for item in self:
+                tag = item._tag
+                # as side effect we update the item cache too:
+                item._itree_prt_idx[2] = tag_cnts[tag] = cnt = tag_cnts[tag] + 1
+                if filter_method(item):
+                    yield (tag, cnt), item
+        else:
+            for item in self:
+                tag = item._tag
+                item._itree_prt_idx[2] = tag_cnts[tag] = cnt = tag_cnts[tag] + 1
+                yield (tag, cnt), item
+
+    def iter_families(self, filter_method=None, order_last=False):
+        """
+        This is a special iterator that iterates over the families in `iTree`. It delivers per family the tag and
+        a list of the containing items. The order is defined by the absolute index of the first item in each family
+
+        Method will be reached via `iTree.Families.iter()`
+
+        :type filter_method: Union[Callable,None]
+        :param filter_method: filter method that checks for matching items
+                              and delivers `True`/`False`.
+                              The filter_method targets always the `iTree`-child-object and checks a characteristic
+                              of this object for matches (see :ref:`filter_method <filter_method>`)
+
+                              If filter_method is None no filtering is performed
+
+                              .. note:: An internal filtering is available because this may change the order of
+                                        the delivered items. An external filter with same method might
+                                        deliver a different result!
+
+        :type order_last: bool
+        :param order_last:
+            * False (default) - The tag-order is based on the order of the first items in the family
+            * True - The tag-order is based on the order of the last items in the family
+
+        :rtype: Generator
+        :return: iterator over all families delivers tuples of (family-tag, family-item-list)
+        """
+        if self:
+            if order_last:
+                index = -1
+            else:
+                index = 0
 
-    def __iadd__(self, other):
-        if self._parent is not None:
-            if self._parent._is_linked:
-                raise PermissionError('The parent is read_only (linked)!')
-        if other._is_temporary:
-            raise TypeError('Given item is temporary and we cannot add temporary items as locals in a linked tree')
-        if other._is_linked:
-            raise PermissionError('__iadd__ operation is not possible with a linked element!')
-        return super().__iadd__(other)
+            if filter_method:
 
-    def rotate(self, *args, **kwargs):
-        """
-        :except: PermissionError not possible on iTreeReadOnly objects
-        """
-        raise PermissionError('Rotation operation is not possible on a linked element!')
+                return ((i.tag, [i for i in self._getitem_fam(i._tag) if filter_method(i)])
+                        for i in sorted((v[index] for v in self._families.values()), key=lambda i: i.idx))
+            else:
+                return ((i.tag, list(self._getitem_fam(i._tag)))
+                        for i in sorted((v[index] for v in self._families.values()), key=lambda i: i.idx))
 
-    def reverse(self, *args, **kwargs):
-        """
-        :except: PermissionError not possible on iTreeReadOnly objects
+    def iter_family_items(self, order_last=False):
         """
-        raise PermissionError('Reverse operation is not possible on a linked element!')
+        This is a special iterator that iterates over the families in `iTree`. It iters over the items of each family
+        the ordered by the first or the last items of the families.
 
-    def append(self, item):
-        """
-        append of items is allowed (items are appended as locals
-        :param item: item to be appended
-        :return:
-        """
-        if self._parent is not None:
-            if self._parent._is_linked:
-                raise PermissionError('The parent is read_only (linked)!')
-        if item._is_temporary:
-            raise TypeError('Given item is temporary and we cannot add temporary items as locals in a linked tree')
-        if item._link is not None:
-            if item._link._file_path is None and item._link._key_path is None:
-                raise TypeError('Linked items cannot be appended to linked item as local item')
-        return super().append(item)
+        :type order_last: bool
+        :param order_last:
+            * False (default) - The tag-order is based on the order of the first items in the family
+            * True - The tag-order is based on the order of the last items in the family
 
-    def extend(self, items):
+        :rtype: Generator
+        :return: iterator over all families delivers tuples of (family-tag, family-item-list)
         """
-        extend of items is allowed, items are appended as locals
-        :param items: items to be appended (iterator)
-        :return: None
+        if self:
+            if order_last:
+                index = -1
+            else:
+                index = 0
+
+            for i in sorted((v[index] for v in self._families.values()), key=lambda i: i.idx):
+                for item in self._getitem_fam(i._tag):
+                    yield item
+
+    def tags(self, order_last=False):
         """
+        iters over all family-tags in level 1 (children). The order is based on first or
+        last item in the family.
 
-        for item in items:
-            if item._parent is not None:
-                self.append(item.copy())
+        :type order_last: bool
+        :param order_last:
+            * False (default) - The tag-order is based on the order of the first items in the family
+            * True - The tag-order is based on the order of the last items in the family
+
+        :rtype: Iterator
+        :return: tag iterator
+        """
+        if self:
+            s = len(self._families)
+            s2 = len(self)
+            if s2 == 1:
+                # only a single family tag exists
+                yield self.getitem_by_idx(0).tag
+            elif s == s2:
+                # all items in the tree have another tag
+                for i in self:
+                    yield i.tag
             else:
-                self.append(item)
+                if order_last:
+                    index = -1
+                else:
+                    index = 0
+                for i in sorted((v[index] for v in self._families.values()), key=lambda i: i.idx):
+                    yield i.tag
 
-    def extendleft(self, item):
-        """
-        :except: PermissionError not possible on iTreeReadOnly objects
-        """
-        raise PermissionError('extendleft operation is not possible on a linked element!')
+    # *** outputs/dumps ************************************************************************************************
 
-    def appendleft(self, item):
-        """
-        :except: PermissionError not possible on iTreeReadOnly objects
+    def __repr__(self):
         """
-        raise PermissionError('appendleft operation is not possible on a linked element!')
+        Create representation string from which the object can be theoretically be reconstructed via `eval()`
+        (might not work in case of
+        value-objects that do not have a working `__repr()` method)
 
-    def insert(self, insert_key, item):
-        """
-        :except: PermissionError not possible on iTreeReadOnly objects
+        :rtype: str
+        :return: representation string
         """
-        raise PermissionError('insert operation is not possible on a linked element!')
+        out = ['iTree(']
+        if self._tag is not NoTag:
+            out.append(repr(self._tag))
+            out.append(', ')
+        if self._value is not NoValue:
+            out.append('value=')
+            out.append(repr(self._value))
+            out.append(', ')
+        if self:
+            if self.level > (sys.getrecursionlimit() / 5):
+                out.append('subtree=[ ... ]')
+            else:
+                subtree = self._items.__repr__()
+                if subtree[0] == 'b':
+                    # we shorten blist from definition
+                    subtree = subtree[6:-1]
+                out.append('subtree=')
+                out.append(subtree)
+                out.append(', ')
+        is_links_loaded = False
+        if hasattr(self, '_link'):
+            link = self._link
+            if link._link_item is not None:
+                out.append('link=iTLink(link_item=%s)' % (repr(link._link_item)))
+            else:
+                out.append('link=iTLink(%s,%s)' % (repr(link.file_path), repr(link.target_path)))
+            is_links_loaded = link.is_loaded
+            out.append(', ')
+        if self._flags or is_links_loaded:
+            flags = self._flags
+            if is_links_loaded:
+                flags = flags | iTFLAG.LOAD_LINKS
+            out.append('flags=%s' % (bin(flags)))
+        if out[-1] == ', ':
+            out = out[:-1]
+        if out[-1] == ',':
+            out = out[:-1]
+        out.append(')')
+        return ''.join(out)
+
+    def __str__(self):
+        """
+        String repr of the item stripping the subtree to the first and last element only and giving ".." inbetween
+
+        For full representation-string use `repr()`.
+
+        :return: shorten representation string
+        """
+        out = ['iTree(']
+        if self._tag is not NoTag:
+            out.append(repr(self._tag))
+            out.append(', ')
+        if self._value is not NoValue:
+            out.append('value=')
+            out.append(repr(self._value))
+            out.append(', ')
+        if len(self):
+            if self.level > (sys.getrecursionlimit() / 5):
+                out.append('subtree=[ ... ]')
+            else:
+                out.append('subtree=[')
+                if len(self) <= 2:
+                    for i in self:
+                        out.append(str(i))
+                        out.append(',')
+                    out[-1] = ']'
+                else:
+                    out.append(str(self[0]))
+                    out.append(',...,')
+                    out.append(str(self[-1]))
+                    out.append(']')
+                out.append(', ')
+        is_links_loaded = False
+        if hasattr(self, '_link'):
+            link = self._link
+            if link._link_item is not None:
+                out.append('link=iTLink(link_item=%s)' % (repr(link._link_item)))
+            else:
+                out.append('link=iTLink(%s,%s)' % (repr(link.file_path), repr(link.target_path)))
+            is_links_loaded = link.is_loaded
+            out.append(', ')
+        if self._flags or is_links_loaded:
+            flags = self._flags
+            if is_links_loaded:
+                flags = flags | iTFLAG.LOAD_LINKS
+            out.append('flags=%s' % (bin(flags)))
+        if out[-1] == ', ':
+            out = out[:-1]
+        if out[-1] == ',':
+            out = out[:-1]
+        out.append(')')
+        return ''.join(out)
 
-    def pop(self, key):
+    def renders(self, filter_method=None, enumerate=None, renderer=iTreeRender):
         """
-        pop the object out of the tree (only possible on local objects)
+        render the iTree into a string
+
+        :type filter_method: Union[Callable,None]
+        :param filter_method: filter method that checks for matching items
+                            and delivers `True`/`False`.
+                            The filter_method targets always the `iTree`-child-object and checks a characteristic
+                            of this object for matches (see :ref:`filter_method <filter_method>`)
+
+                            If `None` is given filtering is inactive.
+
+                            The method uses the given filter always as an hierachical filter.
 
-        :except: In case a linked item is selected an PermissionError is raised
+        :type enumerate: bool
+        :param enumerate:
+                            * True - Add an enumeration before the items
+                            * False (default) - Output without enumeration
 
-        :param key: identification key for the child that should be popped out
+        :type renderer: class
+        :param renderer: Give another renderer class for different formatting
 
-        :return: popped out item (parent set to None)
+        :rtype: str
+        :return: Tree representation as string
         """
-        if self._parent is not None:
-            if self._parent._is_linked:
-                raise PermissionError('The parent is read_only (linked)!')
-        item = super().__getitem__(key)
-        if item._is_linked:
-            raise PermissionError('The target element is read_only (linked)!')
-        else:
-            # maybe the deleted local item must be replaced by a linked item:
-            if item._link is not None:
-                if item._link._link_item is not None:
-                    super().__setitem__(item.tag_idx, item._link._link_item)
-                    item._parent = None
-                    return item
-            # else no overloaded item we just delete
-            return super().pop(key)
+        render_obj = getattr(self, '__renderer', None)
+        if render_obj is None or type(render_obj) != renderer:
+            self.__renderer = render_obj = renderer()
+        return render_obj.renders(self, filter_method, enumerate)
 
-    def popleft(self):
+    def render(self, filter_method=None, enumerate=False, renderer=iTreeRender):
         """
-        pop the first child out of the tree (only possible on local object)
+        Print the rendered string of the `iTree`-object to the console (stdout).
+
+        :type filter_method: Union[Callable,None]
+        :param filter_method: filter method that checks for matching items
+                            and delivers `True`/`False`.
+                            The filter_method targets always the `iTree`-child-object and checks a characteristic
+                            of this object for matches.
+                            If `None` is given filtering is inactive.
 
-        :except: In case a linked item is selected an PermissionError is raised
+        :param enumerate:  add an enumeration before the rendered items
+
+        :param renderer: Render to be used (The given render is stored and will be used until another renderer is given).
+
+        :return:
 
-        :return: popped first item (parent set to None)
         """
+        print(
+            self.renders(filter_method, enumerate, renderer=iTreeRender).encode(
+                errors='replace').decode(
+                'utf8')[:-1])
 
-        return self.__delitem__(0)
+    # for pickle
+    def __reduce__(self):
+        return iTree, tuple(self.get_init_args())
 
-    def remove(self, item):
+    def get_init_args(self, filter_method=None, _subtree_not_none=True):
         """
-        remove the given child item out of the tree (only possible on local object)
+        Method creates list of arguments that can be used as a pointer to create an equal instance of an iTree object.
+        This is a method is used in most cases for internal functionalities (especially copy()).
 
-        :except: In case a linked item is selected an PermissionError is raised
+        :type filter_method: Union[Callable,None]
+        :param filter_method: filter method that checks for matching items
+                            and delivers `True`/`False`.
+                            The filter_method targets always the `iTree`-child-object and checks a characteristic
+                            of this object for matches (see :ref:`filter_method <filter_method>`)
 
-        :param item: item to be removed from the iTree
+                            If `None` is given filtering is inactive.
 
-        :return: removed item (parent set to None)
+        :param _subtree_not_none: internal parameter controlling if the subtree is added or not
+        :return:
         """
+        if _subtree_not_none and self:
+            if self.is_link_root:
+                if filter_method:
+                    subtree = list(filter(filter_method, self._iter_locals_add_placeholders(self)))
+                else:
+                    subtree = list(self._iter_locals_add_placeholders(self))
+            elif filter_method:
+                subtree = list(filter(filter_method, self))
+            else:
+                subtree = list(self)
+            if len(subtree) == 0:
+                subtree = None
+        else:
+            subtree = None
+        result = [self._tag, self._value, subtree]
+        if self.is_link_root:
+            result.append(iTLink(self._link.file_path, self._link.target_path))
+        flags = self._flags
+        if flags:
+            if len(result) == 3:
+                result.append(None)
+            result.append(flags)
+        return result
 
-        return self.__delitem__(item.idx)
+    # serialize + file operations
 
-    def rename(self, item_tag):
+    def loads(self, data_str, check_hash=True, load_links=True,
+              itree_serializer=iTStdJSONSerializer2):
         """
-        :except: PermissionError not possible on iTreeReadOnly objects
-        """
-        raise PermissionError('rename operation is not possible on a linked element!')
+        create an iTree object by loading from a string
 
-    @property
-    def is_link_root(self):
-        """
-        Is this item the highest level linked element?
+        If not overloaded or reinitialized the iTree Standard Serializer will be used. In this case we expect a
+        matching JSON representation.
 
-        :return: True/False
-        """
-        return self.link_root == self
+        :param data_str: source string that contains the iTree information
 
-    @property
-    def link_root(self):
-        """
-        delivers the highest level element that is  linked
-        in case item is not linked it delivers it self
+        :param check_hash: True the hash of the file will be checked and the loading will be stopped if it doesn't match
+                           False - do not check the iTree hash
 
-        :return: highest level linked item found in the parents
-        """
-        if self._is_linked:
-            parent = self._parent
-            if (parent is not None) and parent._is_linked:
-                return self._parent.link_root
-            else:
-                return self
-        return None
+        :param load_links: True - linked iTree objects will be loaded
 
-    @property
-    def is_link_loaded(self):
+        :param itree_serializer: optional user defined serializer for iTree objects
+
+        :return: iTree object loaded from file
         """
-        For linked iTree objects we deliver here the state of loading the links
+        serializer_obj = getattr(self, '__itree_serializer', None)
+        if serializer_obj is None or type(serializer_obj) != itree_serializer:
+            self.__itree_serializer = serializer_obj = itree_serializer(iTree)
 
-        :return: True/False
+        return serializer_obj.loads(data_str, check_hash=check_hash, load_links=load_links)
+
+    def load(self, file_path, check_hash=True, load_links=True,
+             itree_serializer=iTStdJSONSerializer2):
         """
-        return self._link.is_loaded
+        create an iTree object by loading from a file
+
+        If not overloaded or reinitialized the iTree Standard Serializer will be used. In this case we expect a
+        matching JSON representation.
+
+        :param file_path: file path to the file that contains the iTree information
+
+        :param check_hash: True the hash of the file will be checked and the loading will be stopped if it doesn't match
+                           False - do not check the iTree hash
+
+        :param load_links: True - linked iTree objects will be loaded
+
+        :param itree_serializer: optional user defined serializer for iTree objects
 
-    def _convert_to_linked_item(self, item):
+        :return: iTree object loaded from file
         """
-        helper function that creates a linked clone of a normal item
-        helper method is need in the load_links method
+        serializer_obj = getattr(self, '__itree_serializer', None)
+        if serializer_obj is None or type(serializer_obj) != itree_serializer:
+            self.__itree_serializer = serializer_obj = itree_serializer(iTree)
+
+        return serializer_obj.load(file_path, check_hash=check_hash, load_links=load_links)
 
-        :param item: item to be "cloned"
+    def dumps(self, calc_hash=False, filter_method=None,
+              itree_serializer=iTStdJSONSerializer2):
 
-        :return: converted item
         """
-        if item._is_linked:
-            return item
-        data = item._data
-        if type(data) is not iTDataReadOnly:
-            data = iTDataReadOnly(data)
-        return iTreeLink(item._tag, data, subtree=[self._convert_to_linked_item(i) for i in item.iter_children()])
+        serializes the iTree object to JSON (default serializer)
+
+        :param calc_hash: Tell if the hash should be calculated and stored in the header of string
+
+        :param itree_serializer: optional user defined serializer for iTree objects
 
-    def _convert_to_local_item(self, item):
+        :return: serialized string (JSON in case of default serializer)
+        """
+        serializer_obj = getattr(self, '__itree_serializer', None)
+        if serializer_obj is None or type(serializer_obj) != itree_serializer:
+            self.__itree_serializer = serializer_obj = itree_serializer(iTree)
+        return serializer_obj.dumps(self, calc_hash=calc_hash, filter_method=filter_method)
+
+    def dump(self, target_path, pack=True, calc_hash=True, overwrite=False,
+             filter_method=None,
+             itree_serializer=iTStdJSONSerializer2):
         """
-        helper method to clone a none linked item from a linked item
-        this helper function is needed for localizing items
+        serializes the iTree object to JSON (default serializer) and store it in a file
+
+        :param target_path: target path of the file where the iTree should be stored in
+        :param pack: True - data will be packed via gzip before storage
+        :param calc_hash: True - create the hash information of iTree and store it in the header
+        :param overwrite: True - overwrite an existing file
 
-        :param item: linked item to be cloned as none linked item
+        :param itree_serializer: optional user defined serializer for iTree obbjects
 
-        :return: result of the conversion
+        :return: True if file is stored successful
         """
-        if not item._is_linked:
-            return item
-        try:
-            data = iTData(item._data)
-        except:
-            data = None
-        sub_items = [self._convert_to_local_item(i) for i in item.iter_children()]
-        new_item = iTree(item._tag, data, subtree=sub_items)
-        new_item._link = iTLink(link_item=item)
-        return new_item
+        serializer_obj = getattr(self, '__itree_serializer', None)
+        if serializer_obj is None or type(serializer_obj) != itree_serializer:
+            self.__itree_serializer = serializer_obj = itree_serializer(iTree)
+        return serializer_obj.dump(self,
+                                   target_path,
+                                   pack=pack,
+                                   calc_hash=calc_hash,
+                                   overwrite=overwrite,
+                                   filter_method=filter_method)
+
+    # *** link root related functions: *********************************************************************************
+    # *** link related properties **************************************************************************************
 
-    def make_self_local(self):
+    @property
+    def is_placeholder(self):
         """
-        make the current linked object a local object
-        This is only possible if the parent parent is a normal iTree object ->
-        only the first level children in a linked iTree can be made local
-        The operation raises an SyntaxError in case it is used on a deeper level of the linked tree
+        Property shows that item is a placeholder class
 
-        :return: None
+        Normally there should be no placeholder class in the iTree but in case a loaded link does no more contain
+        the expected items it might happen that such a class artifact is still in the tree.
+        In placeholders the value contains the family index in the linked class.
+
+        :rtype: bool
+        :return: True/False
         """
-        if self._parent is None or not self._is_linked:
-            raise SyntaxError('Item is not linked or has no parent, invalid operation!')
-        return self._parent.make_child_local(self)
+        return bool(self._flags & self._PLACEHOLDER)
 
-    def make_child_local(self, key):
+    @property
+    def is_link_cover(self):
         """
-        make the item related to the given key a local object
-        This is only possible if the parent of self is a normal iTree object ->
-        only the first level children in a linked iTree can be made local
-        The operation raises an SyntaxError in case it is used on a deeper level of the linked tree
+        If the item is local and covers a linked item the property is True
+
+        :rtype: bool
+        :return: True/False
 
-        :param key: identification key for the child item that should be converted in a local item
-        :return: None
         """
-        if isinstance(key, iTree):
-            item = key
-        else:
-            item = self.__getitem__(key)
-        if not item._is_linked:
-            raise TypeError('The addressed item is already local!')
-        parent = self._parent
-        if parent is None:
-            raise SyntaxError('The item has no valid parent we cannot change to local!')
-        if parent._is_linked:
-            raise TypeError('The item parent is linked we cannot make this item local!')
-        local_item = self._convert_to_local_item(item)
-        # keep the link to the overloaded element
-        local_item._link = iTLink(link_item=item)
-        super().__setitem__(item.idx, local_item)
-        return local_item
+        return hasattr(self, '_link') and self._link and (type(self._link._link_item) is iTree)
 
-    def iter_locals(self, add_placeholders=False):
+    @property
+    def is_linked(self):
         """
-        iterator that iterates only over the local elements
+        In contrast to iTreeLinked class this is False
 
-        :param add_placeholders: If this flag is set the (normally ignored) placeholder items are included
-                                 in the iteration
+        :rtype: bool
+        :return: True/False
 
-        :return: iterator over local items
         """
-        if add_placeholders:
-            tags = {}
-            for i in self.iter_children():
-                tag = i._tag
-                if tag not in tags:
-                    tags[tag] = self.get_last_local_idx(tag)
-                if tags[tag] is None:
-                    continue
-                if not i._is_linked and not i._is_placeholder and not i._is_temporary:
-                    yield i
-                else:
-                    idx = tags.get(tag)
-                    if idx is not None:
-                        if idx >= i.idx:
-                            yield iTreePlaceHolder(tag)
-                        else:
-                            tags[tag] = None
+        return bool(self._flags & self._LINKED)
+
+    @property
+    def is_link_loaded(self):
+        if hasattr(self, '_link'):
+            return self._link.is_loaded
         else:
-            for i in self.iter_children():
-                if not i._is_linked:
-                    yield i
+            # we return False in case we have no link_roots inside the subtree
+            return any(
+                i.is_link_loaded for i in filter(iTree._filter_linked_roots, self.deep))
 
-    def get_last_local_idx(self, tag):
+    @property
+    def link_root(self):
         """
-        helper function which searches for local items in the tag family and
-        delivers the last index of a local item found in the family. If no local item is found it delivers None.
-
-        iTreePlaceHolder items ignored in this operation!
+        delivers the highest level item that is linked
+        in case item is not linked it delivers itself
 
-        :param tag: tag to identify the family to be searched in
+        :rtype: iTree
+        :return: highest level linked item found in the parents
 
-        :return: last local item idx in tag family or None (no local item found)
         """
-        for item in reversed(self._map[tag]):
-            if not item._is_linked and not item._is_placeholder and not item._is_temporary:
-                return item.tag_idx[1]
+        if self.is_linked:
+            parent = self._itree_prt_idx
+            if (parent is not None) and parent[0].is_linked:
+                return parent[0].link_root
+            else:
+                return self
         return None
 
-    def load_links(self, force=False, delete_invalid_items=False, _items=None):
+    @property
+    def is_link_root(self):
         """
-        load all linked items
+        property that marks the iTree item as an item that contains a link
 
-        :param force: False (default) - load only if not already loaded
-                      True - load even if already loaded (update)
+        :return:
+                 * True - is a link root item
+                 * False is no iTree link item
+        """
+        return bool(self._flags & self._LINK_ROOT)
+
+    def load_links(self, force=False, delete_invalid_items=False, _items=None, _depth=0):
+        """
+        Runs ove all children and sub children in case a ITreeLink object is found the linked items are load in
 
-        :param delete_invalid_items: False (default) - in case of invalid items we will raise an exception!
-                                     True - invalid items will be removed from parent no exception raised
+        In case ´iTree´ is link root: load all linked items
+
+        :param force:
+                      * False (default) - load only if not already loaded
+                      * True - load even if already loaded (update)
+
+        :param delete_invalid_items:
+                                     * False (default) - in case of invalid items we will raise an exception!
+                                     * True - invalid items will be removed from parent no exception raised
 
         :param _items: internal list parameter used for recursive calls of the function
 
+        :param _depth: Internal parameter related to current item depth
         :return:
 
                  * True - success
                  * False - load failed
         """
-        if _items is None:
-            _items = []
-        load_ok = True
-        load_item = None
-        if self._link is not None:
-            if force or not self.is_link_loaded:
-                if self._link.file_path is not None:
-                    if not os.path.exists(self._link.file_path):
-                        if delete_invalid_items:
-                            if self._parent is not None:
-                                self._parent.remove(self)
-                            return False
-                        else:
-                            raise FileNotFoundError('Source file of the link not found!')
-                    full_tree = self.load(self._link.file_path, load_links=True)
-                    if self._link.key_path is None:
-                        load_item = full_tree
+        if _depth > 200:
+            raise RecursionError('Circular link definition couldnot integrate linked item '
+                                 '%s' % (repr(self.tag_idx_path)))
+
+        if self.is_link_root:
+            load_ok = True
+            load_item = None
+            link_handler = self._link
+            if link_handler is not None:
+                if force:
+                    load_active = True
                 else:
-                    full_tree = self._parent
-                if self._link is not None and self._link.key_path is not None:
-                    load_item = full_tree.find(self._link.key_path)
-                    if load_item is None:
+                    # We try to detect if the original link was changed
+                    load_active = False
+                    if link_handler.is_loaded:
+                        load_active = link_handler.is_file_updated()
+                        if not load_active and link_handler.file_path is None:
+                            # internal link check the source tree
+                            try:
+                                target_tree = link_handler.get_target_tree(self)
+                                if len(target_tree) != len(link_handler._keys):
+                                    raise Exception()
+                                for key_old, key_new in zip(link_handler._keys,
+                                                            target_tree.keys()):
+                                    if key_old != key_new:
+                                        raise ValueError()
+                            except:
+                                load_active = True
+                    else:
+                        load_active = True
+                if load_active:
+                    try:
+                        load_item = link_handler.get_target_tree(self)
+                    except:
                         if delete_invalid_items:
-                            if self._parent is not None:
-                                self._parent.remove(self)
+                            if self._itree_prt_idx is not None:
+                                self._itree_prt_idx[0].remove(self)
                             return False
                         else:
-                            raise KeyError('Given key_path not found;'
-                                           'loading of linked items is stopped at item %s!' % self.tag_idx_path)
-                    t = type(load_item)
-                    if t is not iTree and t is not iTreeReadOnly:
-                        if delete_invalid_items:
-                            if self._parent is not None:
-                                self._parent.remove(self)
-                            return False
+                            raise
+                    # keep the locals and coupled objects then clean all
+                    sl = self._items
+                    # now we take over the tree
+                    local_items = OrderedDict()
+                    for i in self._iter_locals_add_placeholders(self):
+                        if i.is_placeholder:
+                            local_items[(i._tag, i._value)] = i
                         else:
-
-                            if load_item._is_linked:
-                                raise TypeError('Given key_path is already linked (circular protection); '
-                                                'loading of linked items is stopped at item %s!' % self.tag_idx_path)
-                            else:
-                                raise LookupError('Given key_path is not matching or is not distinct; '
-                                                  'loading of linked items is stopped at item %s!' % self.tag_idx_path)
-                sl = super(iTree, self)
-                # now we take over the tree
-                local_items = {i.tag_idx: i for i in self.iter_children() if not i._is_linked}
-                sl.clear()
-                # here we run a special extend (we don't care about parents and is_linked flag)
-                m = self._map = {}
-                if load_item is not None:
+                            local_items[i.tag_idx] = i
+                    old_coupled_objects = {i.tag_idx: i.coupled_object for i in self if
+                                           i.is_linked and i.coupled_object}
+                    sl.clear()
+                    self._families = families = {}
+                    linked_flag = self._LINKED
+                    tags = set()
+                    keys = []
+                    append_item_to_tree = self._append_item
+                    convert_to_linked_item = self._convert_to_linked_item
+                    # load the linked items
                     for item in load_item:
-                        if item._is_linked:
-                            if not item.load_links(force=force, delete_invalid_items=delete_invalid_items):
-                                load_ok = False
-                                continue
-                            new_item = item
+                        if item.is_link_root:
+                            try:
+                                item.load_links(force=force, delete_invalid_items=delete_invalid_items,
+                                                _depth=(_depth + 1))
+                                new_item = item.copy()
+                            except (TypeError, RecursionError):
+                                raise RecursionError('Circular link definition couldnot integrate linked item '
+                                                     '%s' % (repr(item.tag_idx_path)))
+                            new_item._flags = new_item._flags | linked_flag
                         else:
-                            new_item = self._convert_to_linked_item(item)
-                        tag_idx = item.tag_idx
-                        if tag_idx in local_items:
-                            # overloading with local!
-                            new_item = local_items.pop(tag_idx)
-                            new_item._parent = None
-                            new_item._link = iTLink(link_item=item)
-                            if new_item._is_placeholder:
-                                new_item = self._convert_to_linked_item(item)
-                        new_item._parent = self
-                        idx = sl.__len__()
-                        sl.append(new_item)
-                        tag = new_item.tag
-                        try:
-                            if m.__contains__(tag):
-                                family = m.__getitem__(tag)
-                                new_item._cache = (idx, family.__len__())
-                                family.append(new_item)
-                            else:
-                                new_item._cache = (idx, 0)
-                                m.__setitem__(tag, blist((new_item,)))
-                        except AttributeError:
-                            new_item._cache = (idx, 0)
-                            self._map = m = {tag: blist((new_item,))}
-                    # append the locals that were not integrated
-                    for item in local_items.values():
-                        item._parent = None
-                        sl.append(item)
-                    self._link.set_loaded(load_item.tag, load_item.data)
-        return load_ok
+                            new_item = convert_to_linked_item(item)
+                        key = item.tag_idx
+                        if key in old_coupled_objects:
+                            new_item.set_coupled_object(old_coupled_objects[key])
+                        keys.append(key)
+                        tags.add(key[0])
+                        # here we build the order of locals ("inheritance" of structure)
+                        if key in local_items:
+                            # append all locals before the match
+                            append_list = []
+                            for k, i in local_items.items():
+                                if k == key:
+                                    if i.is_placeholder:
+                                        append_list.append((k, new_item))
+                                    else:
+                                        i._link = iTLink(link_item=new_item)
+                                        append_list.append((k, i))
+                                    break
+                                elif k in load_item:
+                                    append_list = []
+                                elif not i.is_placeholder:
+                                    # in case of placeholders the new linked tree is reordered
+                                    # and we skip the old placeholders
+                                    # the idea is to keep at least the order of the local items
+                                    append_list.append((k, i))
+
+                            # this does not work must investigate why
+                            # sl.extend(
+                            #    self._iter_extend(self, ((local_items.__delitem__(k ) or i) for k,i in append_list)))
+                            for k, i in append_list:
+                                del local_items[k]
+                                append_item_to_tree(self, i)
 
-    def clear(self, local_only=False):
-        """
-        We clear the object
+                        else:
+                            append_item_to_tree(self, new_item)
 
-        :param local_only:
+                    # append all other local_items
+                    # we do not use _iter_extend() here to avoid copies
+                    for i in filter(lambda i: not i.is_placeholder, local_items.values()):
+                        append_item_to_tree(self, i)
+                    link_handler.set_tags_and_keys(tags, keys)
+                    link_handler.set_loaded(load_item.tag, load_item.value)
+                    return True
+                else:
+                    return False
+        else:
+            loaded = False
+            for i in filter(iTree._filter_linked_roots, self.deep):
+                if i.load_links(force=force, delete_invalid_items=delete_invalid_items, _depth=(_depth + 1)):
+                    loaded = True
+            return loaded
 
-                        * True - clear only the local items
-                        * False - clear whole object (The object is reset to the no links loaded state and locals
-                                   are deleted)
-        :return:
+    def make_local(self, copy_subtree=True):
         """
-        if local_only:
-            for item in self.iter_locals(add_placeholders=True):
-                self.__delitem__(item.idx)
-        else:
-            self._data = None
-            self._coupled = None
-            super().clear()
-            self._map = {}
-            self._link._loaded = False
+        make the current linked object a local object
+        This is only possible if the parent is a iTree object is the link root->
+        only the first level children in a linked iTree can be made local
+        The operation raises an SyntaxError in case it is used on a deeper level of the linked tree
 
-    def equal(self, other, check_parent=False, check_coupled=False, check_link=False):
+        :return: None
         """
-        compares if the data content of another item matches with this item
-
-        :param other: other iTree
+        if self._itree_prt_idx is None or not self.is_linked:
+            raise SyntaxError('Item is not linked or has no parent, invalid operation')
+        parent = self._itree_prt_idx[0]
+        if not parent.is_link_root:
+            raise SyntaxError('local items can just be added to the root objects of links')
+        local_item = self._convert_to_local_item(self, copy_subtree)
+        abs_idx = self.idx
+        tag, f_idx = self.tag_idx
+        # replace old item in super list
+        parent._items[abs_idx] = local_item
+        # replace old item in family list
+        parent._getitem_fam(tag)[f_idx] = local_item
+        local_item._itree_prt_idx = [parent, abs_idx, f_idx]
+        return local_item
 
-        :param check_parent: check the parent object too? (Default False)
+    # *** unsupported methode (overload super() methods with exceptions ************************************************
 
-        :param check_coupled: check the couple object too? (Default False)
+    def __isub__(self, other):
+        raise TypeError('iTree: unsupported operand or function')
 
-        :param check_link: check the internal link variable too? (Default False)
+    def __imul__(self, other):
+        raise TypeError('iTree: unsupported operand or function')
 
+    # *** helpers ******************************************************************************************************
 
-        :return: boolean match result (True match/False no match)
-        """
-        if self == other:
-            return True
-        if type(other) is not iTree:
-            return False
-        if check_parent:
-            if other._parent != self._parent:
-                return False
-        if check_link:
-            if self._link != other._link:
-                return False
-        my_data = (self._tag, super(iTree, self).__len__(), len(self._map), self._link)
-        other_data = (other._tag, super(iTree, other).__len__(), len(other._map), other._link)
-        if my_data != other_data:
-            return False
-        for si, oi in zip(other.iter_children(), self.iter_children()):
-            if not si.equal(oi):
-                return False
-        if check_coupled:
-            try:
-                if self._coupled != other._coupled:
-                    return False
-            except AttributeError:
-                if hasattr(self, '_coupled'):
-                    return False
-                if hasattr(other, '_coupled'):
-                    return False
-        return True
-
-    def __repr__(self):
-        """
-        create representation string from which the object can be reconstructed via eval (might not work in case of
-        data that do not have a working repr method)
-        :return: representation string
+    # property for debugging
+    @property
+    def _debug_children_list(self):
         """
-        repr_str = 'iTreeLink("%s"' % (repr(self._tag))
-        if not self._data.is_empty:
-            if self._data.is_no_key_only:
-                repr_str = repr_str + ', data=%s' % repr(self._data.__getitem__())
-            else:
-                repr_str = repr_str + ', data=%s' % repr(self._data)
-            if self._link is not None:
-                if self._link.file_path is not None:
-                    repr_str = repr_str + ', link_file_path=%s' % repr(self._link.file_path)
-                if self._link.key_path is not None:
-                    repr_str = repr_str + ', link_key_path=%s' % repr(self._link.key_path)
-            locals = list(self.iter_locals(add_placeholders=True))
-            if len(locals) > 0:
-                repr_str = repr_str + ', subtree=%s' % repr(locals)
-        return repr_str + ')'
-
-
-class iTreePlaceHolder(iTreeReadOnly):
-    """
-    place holder item that helps to keep items name in the overloading mechanism
-    """
-
-    _is_read_only = False
-    _is_temporary = False
-    _is_placeholder = True
-    _is_linked = False
-
-    __slots__ = (
-        '_tag', '_parent', '_map', '_coupled', '_data', '_cache', '_def_serializer', '_link')
-
-    def __init__(self, tag):
-        t = type(tag)
-        if t is int or t is TagIdx:
-            raise TypeError('Given tag cannot be used in iTree wrong type (int or TagIdx)')
-        else:
-            self._tag = tag
-        super().__init__(tag)
+        This is a property for debugging proposes only
 
-    def __repr__(self):
-        """
-        create representation string from which the object can be reconstructed via eval (might not work in case of
-        data that do not have a working repr method)
-        :return: representation string
+        :return: list of children
         """
-        return 'iTreePlaceHolder("%s")' % (repr(self._tag))
+        return list(self)
```

