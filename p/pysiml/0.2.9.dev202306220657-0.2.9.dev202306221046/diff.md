# Comparing `tmp/pysiml-0.2.9.dev202306220657-py3-none-any.whl.zip` & `tmp/pysiml-0.2.9.dev202306221046-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 170251 bytes, number of entries: 138
+Zip file size: 170250 bytes, number of entries: 138
 -rw-r--r--  2.0 unx     1520 b- defN 80-Jan-01 00:00 pyproject.toml
 -rw-r--r--  2.0 unx      638 b- defN 80-Jan-01 00:00 siml/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 siml/__main__/__init__.py
 -rw-r--r--  2.0 unx      900 b- defN 80-Jan-01 00:00 siml/__main__/convert_interim_data.py
 -rw-r--r--  2.0 unx     1400 b- defN 80-Jan-01 00:00 siml/__main__/convert_raw_data.py
 -rw-r--r--  2.0 unx     1742 b- defN 80-Jan-01 00:00 siml/__main__/optimize.py
 -rw-r--r--  2.0 unx     8663 b- defN 80-Jan-01 00:00 siml/__main__/plot_losses.py
@@ -128,13 +128,13 @@
 -rw-r--r--  2.0 unx     1774 b- defN 80-Jan-01 00:00 siml/update_functions/element_batch_update.py
 -rw-r--r--  2.0 unx     3623 b- defN 80-Jan-01 00:00 siml/update_functions/pseudo_batch_update.py
 -rw-r--r--  2.0 unx     2702 b- defN 80-Jan-01 00:00 siml/update_functions/standard_update.py
 -rw-r--r--  2.0 unx      429 b- defN 80-Jan-01 00:00 siml/update_functions/update_interface.py
 -rw-r--r--  2.0 unx    23027 b- defN 80-Jan-01 00:00 siml/util.py
 -rw-r--r--  2.0 unx       37 b- defN 80-Jan-01 00:00 siml/utils/__init__.py
 -rw-r--r--  2.0 unx     7682 b- defN 80-Jan-01 00:00 siml/utils/fem_data_utils.py
--rw-r--r--  2.0 unx    11431 b- defN 80-Jan-01 00:00 pysiml-0.2.9.dev202306220657.dist-info/LICENSE
--rw-r--r--  2.0 unx     1638 b- defN 80-Jan-01 00:00 pysiml-0.2.9.dev202306220657.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 pysiml-0.2.9.dev202306220657.dist-info/WHEEL
--rw-r--r--  2.0 unx      388 b- defN 80-Jan-01 00:00 pysiml-0.2.9.dev202306220657.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx    12580 b- defN 16-Jan-01 00:00 pysiml-0.2.9.dev202306220657.dist-info/RECORD
-138 files, 600479 bytes uncompressed, 150145 bytes compressed:  75.0%
+-rw-r--r--  2.0 unx    11431 b- defN 80-Jan-01 00:00 pysiml-0.2.9.dev202306221046.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1638 b- defN 80-Jan-01 00:00 pysiml-0.2.9.dev202306221046.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 pysiml-0.2.9.dev202306221046.dist-info/WHEEL
+-rw-r--r--  2.0 unx      388 b- defN 80-Jan-01 00:00 pysiml-0.2.9.dev202306221046.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx    12580 b- defN 16-Jan-01 00:00 pysiml-0.2.9.dev202306221046.dist-info/RECORD
+138 files, 600479 bytes uncompressed, 150144 bytes compressed:  75.0%
```

## zipnote {}

```diff
@@ -393,23 +393,23 @@
 
 Filename: siml/utils/__init__.py
 Comment: 
 
 Filename: siml/utils/fem_data_utils.py
 Comment: 
 
-Filename: pysiml-0.2.9.dev202306220657.dist-info/LICENSE
+Filename: pysiml-0.2.9.dev202306221046.dist-info/LICENSE
 Comment: 
 
-Filename: pysiml-0.2.9.dev202306220657.dist-info/METADATA
+Filename: pysiml-0.2.9.dev202306221046.dist-info/METADATA
 Comment: 
 
-Filename: pysiml-0.2.9.dev202306220657.dist-info/WHEEL
+Filename: pysiml-0.2.9.dev202306221046.dist-info/WHEEL
 Comment: 
 
-Filename: pysiml-0.2.9.dev202306220657.dist-info/entry_points.txt
+Filename: pysiml-0.2.9.dev202306221046.dist-info/entry_points.txt
 Comment: 
 
-Filename: pysiml-0.2.9.dev202306220657.dist-info/RECORD
+Filename: pysiml-0.2.9.dev202306221046.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyproject.toml

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pysiml"
-version = "0.2.9.dev202306220657"
+version = "0.2.9.dev202306221046"
 description = "SiML - a Simulation ML library"
 license = "Apache-2.0"
 authors = ["RICOS Co. Ltd."]
 readme = "README.md"
 repository = "https://github.com/ricosjp/pysiml"
 documentation = "https://ricosjp.github.io/pysiml/"
 packages = [
```

## Comparing `pysiml-0.2.9.dev202306220657.dist-info/LICENSE` & `pysiml-0.2.9.dev202306221046.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pysiml-0.2.9.dev202306220657.dist-info/METADATA` & `pysiml-0.2.9.dev202306221046.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysiml
-Version: 0.2.9.dev202306220657
+Version: 0.2.9.dev202306221046
 Summary: SiML - a Simulation ML library
 Home-page: https://github.com/ricosjp/pysiml
 License: Apache-2.0
 Author: RICOS Co. Ltd.
 Requires-Python: >=3.9,<3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

## Comparing `pysiml-0.2.9.dev202306220657.dist-info/RECORD` & `pysiml-0.2.9.dev202306221046.dist-info/RECORD`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-pyproject.toml,sha256=lLsllupURffw1NjzfRuh9a2wjUVzbCWoNaWkuu_Oj-M,1520
+pyproject.toml,sha256=aBmyKDRN80DodfitTBgxIwvI1QCZx8ptCROyiJvH9MU,1520
 siml/__init__.py,sha256=mC61oSLHO5F6zXHhOrzH51R-vkH0mL4MShhSBiRRe6s,638
 siml/__main__/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 siml/__main__/convert_interim_data.py,sha256=jA6GD7BlnsEjARcln3UBwXlFj64BeFALAmgD1ohBkqo,900
 siml/__main__/convert_raw_data.py,sha256=VNVOyx9lChopF2Q-9OXtN_-MtfBsyjS_JvFwCjdkv0c,1400
 siml/__main__/optimize.py,sha256=6HALn60Mxh4GUiPbSXjvrdpkoQ4NgYSzCHCBRbli4W0,1742
 siml/__main__/plot_losses.py,sha256=0uMsoPN-xR0JhPg0WzSQL5GbD80ovuFO12eVpc0x6Xc,8663
 siml/__main__/prepare_preprocess_converters.py,sha256=w_rzic--RUyISagQOJw_5-oEkOFEKXUN7G1TkTOxd8g,927
@@ -127,12 +127,12 @@
 siml/update_functions/element_batch_update.py,sha256=93_L9jl4D9lFQXmEX1Lo8l4n3rDf1wdZljPJIQd9rUs,1774
 siml/update_functions/pseudo_batch_update.py,sha256=7PS6SEXOMB57uaJQhZ8VrtEiIkDF59JE1c6yyrKL3YY,3623
 siml/update_functions/standard_update.py,sha256=jIgeQ_c9R1dgcxDQWzx-w5TkJ7naDKmNi_WUFFchxc4,2702
 siml/update_functions/update_interface.py,sha256=O1fGrE21iXckz7NTOTDNlyQ4rll1SQDehdc_Kk5we0Q,429
 siml/util.py,sha256=AzvnYN1svE28ioHGPgMjkpiK35hCA5m5qwFEDb3agHA,23027
 siml/utils/__init__.py,sha256=DVdxWEBXfapWAWNM0jUouKJzru4RyK2ru2QheBmrm_s,37
 siml/utils/fem_data_utils.py,sha256=LDB_MxYPg_WELl6D_az9ikMZxAF5Ml5qKUXR2CnuxvE,7682
-pysiml-0.2.9.dev202306220657.dist-info/LICENSE,sha256=Ok4O8jxCIpLhGZjTNzgBW8V8xITF_SUVEp1juLijZpA,11431
-pysiml-0.2.9.dev202306220657.dist-info/METADATA,sha256=kWhJ6Yj0kslZmNa1slwoGhuR8FmLxGG1oesoFk24ucg,1638
-pysiml-0.2.9.dev202306220657.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
-pysiml-0.2.9.dev202306220657.dist-info/entry_points.txt,sha256=zXU0Gd56XeUfgaeG-CGXcYaTpORSU6kVeQ_vVvjIFPs,388
-pysiml-0.2.9.dev202306220657.dist-info/RECORD,,
+pysiml-0.2.9.dev202306221046.dist-info/LICENSE,sha256=Ok4O8jxCIpLhGZjTNzgBW8V8xITF_SUVEp1juLijZpA,11431
+pysiml-0.2.9.dev202306221046.dist-info/METADATA,sha256=0g7_IM96ckM4t6bB-BqDBNih2nPQftu1893xsf5kX_I,1638
+pysiml-0.2.9.dev202306221046.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
+pysiml-0.2.9.dev202306221046.dist-info/entry_points.txt,sha256=zXU0Gd56XeUfgaeG-CGXcYaTpORSU6kVeQ_vVvjIFPs,388
+pysiml-0.2.9.dev202306221046.dist-info/RECORD,,
```

