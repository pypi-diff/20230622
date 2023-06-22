# Comparing `tmp/plantuml_markdown-3.9.1-py3-none-any.whl.zip` & `tmp/plantuml_markdown-3.9.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 17557 bytes, number of entries: 6
--rw-rw-r--  2.0 unx    31183 b- defN 23-Apr-27 05:38 plantuml_markdown.py
--rw-rw-r--  2.0 unx     1299 b- defN 23-Apr-27 05:46 plantuml_markdown-3.9.1.dist-info/LICENSE
--rw-rw-r--  2.0 unx    17482 b- defN 23-Apr-27 05:46 plantuml_markdown-3.9.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-27 05:46 plantuml_markdown-3.9.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx       18 b- defN 23-Apr-27 05:46 plantuml_markdown-3.9.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      515 b- defN 23-Apr-27 05:46 plantuml_markdown-3.9.1.dist-info/RECORD
-6 files, 50589 bytes uncompressed, 16621 bytes compressed:  67.1%
+Zip file size: 17584 bytes, number of entries: 6
+-rw-rw-r--  2.0 unx    31222 b- defN 23-Jun-22 18:06 plantuml_markdown.py
+-rw-rw-r--  2.0 unx     1299 b- defN 23-Jun-22 18:10 plantuml_markdown-3.9.2.dist-info/LICENSE
+-rw-rw-r--  2.0 unx    17482 b- defN 23-Jun-22 18:10 plantuml_markdown-3.9.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-22 18:10 plantuml_markdown-3.9.2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       18 b- defN 23-Jun-22 18:10 plantuml_markdown-3.9.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      515 b- defN 23-Jun-22 18:10 plantuml_markdown-3.9.2.dist-info/RECORD
+6 files, 50628 bytes uncompressed, 16648 bytes compressed:  67.1%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: plantuml_markdown.py
 Comment: 
 
-Filename: plantuml_markdown-3.9.1.dist-info/LICENSE
+Filename: plantuml_markdown-3.9.2.dist-info/LICENSE
 Comment: 
 
-Filename: plantuml_markdown-3.9.1.dist-info/METADATA
+Filename: plantuml_markdown-3.9.2.dist-info/METADATA
 Comment: 
 
-Filename: plantuml_markdown-3.9.1.dist-info/WHEEL
+Filename: plantuml_markdown-3.9.2.dist-info/WHEEL
 Comment: 
 
-Filename: plantuml_markdown-3.9.1.dist-info/top_level.txt
+Filename: plantuml_markdown-3.9.2.dist-info/top_level.txt
 Comment: 
 
-Filename: plantuml_markdown-3.9.1.dist-info/RECORD
+Filename: plantuml_markdown-3.9.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## plantuml_markdown.py

```diff
@@ -234,32 +234,32 @@
         elif img_format == 'svg':
             return self._svg_image(diagram, options)
         elif img_format == 'svg_object':
             return self._svg_object_image(diagram, options)
         else:  # png format, explicitly set or as a default when format is not recognized
             return self._png_image(diagram, options, code)
 
-    @staticmethod
-    def _txt_code(diagram: bytes) -> str:
+    def _txt_code(self, diagram: bytes) -> str:
         # logger.debug(diagram)
         img = etree.Element('pre')
         code = etree.SubElement(img, 'code')
         code.attrib['class'] = 'text'
         code.text = AtomicString(diagram.decode('UTF-8'))
-        return etree.tostring(img, short_empty_elements=True).decode()
+        return self.md.htmlStash.store(etree.tostring(img, short_empty_elements=True).decode())
 
     def _inline_svg_image(self, diagram: bytes, options: Dict[str, Optional[str]]) -> str:
         data = self.ADAPT_SVG_REGEX.sub('<svg \\1\\2>', diagram.decode('UTF-8'))
         img = etree.fromstring(data.encode('UTF-8'))
         if bool(self.config["remove_inline_svg_size"]):
             # remove width and height in style attribute
             img.attrib['style'] = re.sub(r'\b(?:width|height):\d+px;', '', img.attrib['style'])
         img.attrib['preserveAspectRatio'] = 'xMaxYMax meet'
         self._set_tag_attributes(img, options)
-        return etree.tostring(img, short_empty_elements=True).decode()
+
+        return self.md.htmlStash.store(etree.tostring(img, short_empty_elements=True).decode())
 
     def _svg_image(self, diagram: bytes, options: Dict[str, Optional[str]]) -> str:
         # Firefox handles only base64 encoded SVGs
         data = 'data:image/svg+xml;base64,{0}'.format(base64.b64encode(diagram).decode('ascii'))
         img = etree.Element('img')
         img.attrib['src'] = data
         self._set_tag_attributes(img, options)
```

## Comparing `plantuml_markdown-3.9.1.dist-info/LICENSE` & `plantuml_markdown-3.9.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `plantuml_markdown-3.9.1.dist-info/METADATA` & `plantuml_markdown-3.9.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plantuml-markdown
-Version: 3.9.1
+Version: 3.9.2
 Summary: A PlantUML plugin for Markdown
 Home-page: https://github.com/mikitex70/plantuml-markdown
 Author: Michele Tessaro
 Author-email: michele.tessaro@email.it
 Keywords: Markdown,typesetting,include,plugin,extension
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: BSD License
```

## Comparing `plantuml_markdown-3.9.1.dist-info/RECORD` & `plantuml_markdown-3.9.2.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,6 +1,6 @@
-plantuml_markdown.py,sha256=hZlbDH9RDvX_3dbbD_6vnz7r-bxXFXOOxinRfGA2WGk,31183
-plantuml_markdown-3.9.1.dist-info/LICENSE,sha256=bsJBUgOT3HznIWIHgzMSbwk7xWI0i0bptHJyUgU6Qsg,1299
-plantuml_markdown-3.9.1.dist-info/METADATA,sha256=7sv4OGAqq_kg0CVxnZ27IGkb-X685Bc2npFn8CRWeMM,17482
-plantuml_markdown-3.9.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-plantuml_markdown-3.9.1.dist-info/top_level.txt,sha256=-nFvHZOilZwd9Usv166IF3L2OGkr5IT7uTpQEjw2I5M,18
-plantuml_markdown-3.9.1.dist-info/RECORD,,
+plantuml_markdown.py,sha256=h-W-irEjmElSY9AaPd1CZ7mg3qvTCBRYp0DQjQhcYWI,31222
+plantuml_markdown-3.9.2.dist-info/LICENSE,sha256=bsJBUgOT3HznIWIHgzMSbwk7xWI0i0bptHJyUgU6Qsg,1299
+plantuml_markdown-3.9.2.dist-info/METADATA,sha256=msqJoVVIWVqCrZDSyoOF6rXLF50aN8d717pQNF1YrpE,17482
+plantuml_markdown-3.9.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+plantuml_markdown-3.9.2.dist-info/top_level.txt,sha256=-nFvHZOilZwd9Usv166IF3L2OGkr5IT7uTpQEjw2I5M,18
+plantuml_markdown-3.9.2.dist-info/RECORD,,
```

