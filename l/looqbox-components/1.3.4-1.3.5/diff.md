# Comparing `tmp/looqbox_components-1.3.4-py3-none-any.whl.zip` & `tmp/looqbox_components-1.3.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 9918 bytes, number of entries: 16
+Zip file size: 9929 bytes, number of entries: 16
 -rw-r--r--  2.0 unx      231 b- defN 23-May-03 16:35 looqbox_components/__init__.py
 -rw-r--r--  2.0 unx        1 b- defN 23-Apr-28 18:07 looqbox_components/templates/__init__.py
 -rw-r--r--  2.0 unx     7156 b- defN 23-May-16 13:35 looqbox_components/templates/container.py
 -rw-r--r--  2.0 unx     2688 b- defN 23-May-16 13:35 looqbox_components/templates/simple_card.py
--rw-r--r--  2.0 unx     5683 b- defN 23-Apr-28 18:07 looqbox_components/templates/tag.py
+-rw-r--r--  2.0 unx     5754 b- defN 23-Jun-22 12:16 looqbox_components/templates/tag.py
 -rw-r--r--  2.0 unx     2840 b- defN 23-Apr-28 18:07 looqbox_components/templates/toplist.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-28 18:07 looqbox_components/templates/tests/__init__.py
 -rw-r--r--  2.0 unx      591 b- defN 23-May-16 13:35 looqbox_components/templates/tests/test_simple_card.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-28 18:07 looqbox_components/tests/__init__.py
 -rw-r--r--  2.0 unx      233 b- defN 23-Apr-28 18:07 looqbox_components/tests/test_looqbox_components.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-28 18:07 looqbox_components/utils/__init__.py
 -rw-r--r--  2.0 unx      775 b- defN 23-May-16 13:35 looqbox_components/utils/parent_parameters.py
--rw-r--r--  2.0 unx      989 b- defN 23-Jun-01 18:09 looqbox_components-1.3.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-01 18:09 looqbox_components-1.3.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       19 b- defN 23-Jun-01 18:09 looqbox_components-1.3.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1505 b- defN 23-Jun-01 18:09 looqbox_components-1.3.4.dist-info/RECORD
-16 files, 22803 bytes uncompressed, 7344 bytes compressed:  67.8%
+-rw-r--r--  2.0 unx      989 b- defN 23-Jun-22 12:18 looqbox_components-1.3.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-22 12:18 looqbox_components-1.3.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       19 b- defN 23-Jun-22 12:18 looqbox_components-1.3.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1505 b- defN 23-Jun-22 12:18 looqbox_components-1.3.5.dist-info/RECORD
+16 files, 22874 bytes uncompressed, 7355 bytes compressed:  67.8%
```

## zipnote {}

```diff
@@ -30,20 +30,20 @@
 
 Filename: looqbox_components/utils/__init__.py
 Comment: 
 
 Filename: looqbox_components/utils/parent_parameters.py
 Comment: 
 
-Filename: looqbox_components-1.3.4.dist-info/METADATA
+Filename: looqbox_components-1.3.5.dist-info/METADATA
 Comment: 
 
-Filename: looqbox_components-1.3.4.dist-info/WHEEL
+Filename: looqbox_components-1.3.5.dist-info/WHEEL
 Comment: 
 
-Filename: looqbox_components-1.3.4.dist-info/top_level.txt
+Filename: looqbox_components-1.3.5.dist-info/top_level.txt
 Comment: 
 
-Filename: looqbox_components-1.3.4.dist-info/RECORD
+Filename: looqbox_components-1.3.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## looqbox_components/templates/tag.py

```diff
@@ -77,14 +77,16 @@
 
     def _set_element_style(self, element) -> css:
         for style in self._get_defined_style():
             element.css_options = css.add(element.css_options, style)
         return element
 
     def _get_defined_style(self):
+        if self.css_options is None:
+            self.css_options = []
         return list(set(self.css_options).union(set(self._container_default_style)))
 
     @property
     def invert_default_color(self):
         range_list = [e.get("range") for e in self.tag_rules]
         inverse_range_list = list(reversed(range_list))
         for rule, new_rule in zip(self.tag_rules, inverse_range_list):
```

## Comparing `looqbox_components-1.3.4.dist-info/METADATA` & `looqbox_components-1.3.5.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: looqbox-components
-Version: 1.3.4
+Version: 1.3.5
 Summary: A looqbox package with most used visual components templates
 Home-page: https://github.com/looqbox/python-visual-components
 Author: Looqbox
 Author-email: admin@looqbox.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

## Comparing `looqbox_components-1.3.4.dist-info/RECORD` & `looqbox_components-1.3.5.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 looqbox_components/__init__.py,sha256=t-xfKsHcJ7n8NfeWb6JLRJeBgdPD86Aqm_nQid_fZxw,231
 looqbox_components/templates/__init__.py,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
 looqbox_components/templates/container.py,sha256=QFClUUkX2GtwiT8MmIPJQmSrfZBg3PRnWM01BQodMfw,7156
 looqbox_components/templates/simple_card.py,sha256=yqYXcZMaNt1BwtPOGvulOwgMLH2ox-5nqr0roa6kH7o,2688
-looqbox_components/templates/tag.py,sha256=EciZ3VRCIdloOUTC68hF7FHL-_9xtQ2TVi1K60oAKDw,5683
+looqbox_components/templates/tag.py,sha256=qqUpb2Tn86kjgSn1kZNccM7BlaLbtZqHs40NhW9UDrg,5754
 looqbox_components/templates/toplist.py,sha256=mAlFkUBYXMMqSSIz5MogMascE1OfzVoT5sfGfFiuC5Y,2840
 looqbox_components/templates/tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 looqbox_components/templates/tests/test_simple_card.py,sha256=p7axi8j3Fqs5Ka_GSSDM7JImPZaH-xpDc4ZmBYCdupU,591
 looqbox_components/tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 looqbox_components/tests/test_looqbox_components.py,sha256=8fVRfEvqcxlJDuNp6RlucKwH13JMCrXkeGgSmkdxonU,233
 looqbox_components/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 looqbox_components/utils/parent_parameters.py,sha256=SEgVvejN3PqjcSkKJztrYykjo-m626BY0s1WvpGEmOs,775
-looqbox_components-1.3.4.dist-info/METADATA,sha256=K6_Y_Sr6Y0o8PsXWpdDE_w2VyEjM4OiS80Ru0Els9f0,989
-looqbox_components-1.3.4.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-looqbox_components-1.3.4.dist-info/top_level.txt,sha256=Zb_QlF8DlA-rP1wb-5-vbk_U_exlVnC4IXl1bBro5kQ,19
-looqbox_components-1.3.4.dist-info/RECORD,,
+looqbox_components-1.3.5.dist-info/METADATA,sha256=RZMzTYPc1eFCLQORqvIyEzJ8YwbMQSqzqNrWCDLN0GI,989
+looqbox_components-1.3.5.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+looqbox_components-1.3.5.dist-info/top_level.txt,sha256=Zb_QlF8DlA-rP1wb-5-vbk_U_exlVnC4IXl1bBro5kQ,19
+looqbox_components-1.3.5.dist-info/RECORD,,
```

