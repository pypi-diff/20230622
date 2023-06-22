# Comparing `tmp/pysvgedit-0.0.1.tar.gz` & `tmp/pysvgedit-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysvgedit-0.0.1.tar", last modified: Tue Jun 20 07:35:11 2023, max compression
+gzip compressed data, was "pysvgedit-0.0.2.tar", last modified: Thu Jun 22 18:11:04 2023, max compression
```

## Comparing `pysvgedit-0.0.1.tar` & `pysvgedit-0.0.2.tar`

### file list

```diff
@@ -1,29 +1,35 @@
-drwx------   0 joe       (1000) joe       (1000)        0 2023-06-20 07:35:11.054881 pysvgedit-0.0.1/
--rw-------   0 joe       (1000) joe       (1000)    35142 2023-06-18 18:53:00.000000 pysvgedit-0.0.1/LICENSE
--rw-------   0 joe       (1000) joe       (1000)     1178 2023-06-20 07:35:11.054881 pysvgedit-0.0.1/PKG-INFO
--rw-------   0 joe       (1000) joe       (1000)      207 2023-06-20 07:23:51.000000 pysvgedit-0.0.1/README.md
-drwx------   0 joe       (1000) joe       (1000)        0 2023-06-20 07:35:11.054881 pysvgedit-0.0.1/pysvgedit/
--rw-------   0 joe       (1000) joe       (1000)     1378 2023-06-18 08:01:01.000000 pysvgedit-0.0.1/pysvgedit/SVGCircle.py
--rw-------   0 joe       (1000) joe       (1000)     1005 2023-06-18 08:01:04.000000 pysvgedit-0.0.1/pysvgedit/SVGDefs.py
--rw-------   0 joe       (1000) joe       (1000)     3084 2023-06-18 18:50:45.000000 pysvgedit-0.0.1/pysvgedit/SVGDocument.py
--rw-------   0 joe       (1000) joe       (1000)     1422 2023-06-18 17:58:55.000000 pysvgedit-0.0.1/pysvgedit/SVGGroup.py
--rw-------   0 joe       (1000) joe       (1000)     4249 2023-06-18 08:01:18.000000 pysvgedit-0.0.1/pysvgedit/SVGObject.py
--rw-------   0 joe       (1000) joe       (1000)     2310 2023-06-18 08:01:22.000000 pysvgedit-0.0.1/pysvgedit/SVGPath.py
--rw-------   0 joe       (1000) joe       (1000)     1236 2023-06-18 08:01:26.000000 pysvgedit-0.0.1/pysvgedit/SVGRect.py
--rw-------   0 joe       (1000) joe       (1000)     4006 2023-06-18 18:48:17.000000 pysvgedit-0.0.1/pysvgedit/SVGStyle.py
--rw-------   0 joe       (1000) joe       (1000)     2532 2023-06-18 17:57:58.000000 pysvgedit-0.0.1/pysvgedit/SVGText.py
--rw-------   0 joe       (1000) joe       (1000)     1157 2023-06-18 08:01:57.000000 pysvgedit-0.0.1/pysvgedit/Vector2D.py
--rw-------   0 joe       (1000) joe       (1000)     1967 2023-06-18 18:50:02.000000 pysvgedit-0.0.1/pysvgedit/XMLTools.py
--rw-------   0 joe       (1000) joe       (1000)     1140 2023-06-20 07:34:13.000000 pysvgedit-0.0.1/pysvgedit/__init__.py
-drwx------   0 joe       (1000) joe       (1000)        0 2023-06-20 07:35:11.054881 pysvgedit-0.0.1/pysvgedit/apps/
--rw-------   0 joe       (1000) joe       (1000)     3101 2023-06-18 08:03:19.000000 pysvgedit-0.0.1/pysvgedit/apps/FriendlyArgumentParser.py
--rw-------   0 joe       (1000) joe       (1000)     4243 2023-06-20 07:32:23.000000 pysvgedit-0.0.1/pysvgedit/apps/MakoRendererApp.py
--rw-------   0 joe       (1000) joe       (1000)      841 2023-06-18 08:03:02.000000 pysvgedit-0.0.1/pysvgedit/apps/__init__.py
-drwx------   0 joe       (1000) joe       (1000)        0 2023-06-20 07:35:11.054881 pysvgedit-0.0.1/pysvgedit.egg-info/
--rw-------   0 joe       (1000) joe       (1000)     1178 2023-06-20 07:35:11.000000 pysvgedit-0.0.1/pysvgedit.egg-info/PKG-INFO
--rw-------   0 joe       (1000) joe       (1000)      561 2023-06-20 07:35:11.000000 pysvgedit-0.0.1/pysvgedit.egg-info/SOURCES.txt
--rw-------   0 joe       (1000) joe       (1000)        1 2023-06-20 07:35:11.000000 pysvgedit-0.0.1/pysvgedit.egg-info/dependency_links.txt
--rw-------   0 joe       (1000) joe       (1000)       86 2023-06-20 07:35:11.000000 pysvgedit-0.0.1/pysvgedit.egg-info/entry_points.txt
--rw-------   0 joe       (1000) joe       (1000)       10 2023-06-20 07:35:11.000000 pysvgedit-0.0.1/pysvgedit.egg-info/top_level.txt
--rw-------   0 joe       (1000) joe       (1000)       38 2023-06-20 07:35:11.054881 pysvgedit-0.0.1/setup.cfg
--rw-------   0 joe       (1000) joe       (1000)     1282 2023-06-20 07:35:10.000000 pysvgedit-0.0.1/setup.py
+drwx------   0 joe       (1000) joe       (1000)        0 2023-06-22 18:11:04.478366 pysvgedit-0.0.2/
+-rw-------   0 joe       (1000) joe       (1000)    35142 2023-06-18 18:53:00.000000 pysvgedit-0.0.2/LICENSE
+-rw-------   0 joe       (1000) joe       (1000)     1178 2023-06-22 18:11:04.478366 pysvgedit-0.0.2/PKG-INFO
+-rw-------   0 joe       (1000) joe       (1000)      207 2023-06-20 07:23:51.000000 pysvgedit-0.0.2/README.md
+drwx------   0 joe       (1000) joe       (1000)        0 2023-06-22 18:11:04.478366 pysvgedit-0.0.2/pysvgedit/
+-rw-------   0 joe       (1000) joe       (1000)      975 2023-06-22 13:27:51.000000 pysvgedit-0.0.2/pysvgedit/Exceptions.py
+-rw-------   0 joe       (1000) joe       (1000)     4993 2023-06-22 16:21:37.000000 pysvgedit-0.0.2/pysvgedit/SVGAnimation.py
+-rw-------   0 joe       (1000) joe       (1000)     1377 2023-06-22 17:42:00.000000 pysvgedit-0.0.2/pysvgedit/SVGCircle.py
+-rw-------   0 joe       (1000) joe       (1000)     1005 2023-06-18 08:01:04.000000 pysvgedit-0.0.2/pysvgedit/SVGDefs.py
+-rw-------   0 joe       (1000) joe       (1000)     3084 2023-06-18 18:50:45.000000 pysvgedit-0.0.2/pysvgedit/SVGDocument.py
+-rw-------   0 joe       (1000) joe       (1000)     1422 2023-06-18 17:58:55.000000 pysvgedit-0.0.2/pysvgedit/SVGGroup.py
+-rw-------   0 joe       (1000) joe       (1000)     4372 2023-06-22 17:41:48.000000 pysvgedit-0.0.2/pysvgedit/SVGObject.py
+-rw-------   0 joe       (1000) joe       (1000)     2294 2023-06-22 15:54:39.000000 pysvgedit-0.0.2/pysvgedit/SVGPath.py
+-rw-------   0 joe       (1000) joe       (1000)     1513 2023-06-22 17:50:27.000000 pysvgedit-0.0.2/pysvgedit/SVGRect.py
+-rw-------   0 joe       (1000) joe       (1000)     4340 2023-06-22 17:34:07.000000 pysvgedit-0.0.2/pysvgedit/SVGStyle.py
+-rw-------   0 joe       (1000) joe       (1000)     2574 2023-06-22 17:30:05.000000 pysvgedit-0.0.2/pysvgedit/SVGText.py
+-rw-------   0 joe       (1000) joe       (1000)     1700 2023-06-22 15:55:00.000000 pysvgedit-0.0.2/pysvgedit/SVGTransformation.py
+-rw-------   0 joe       (1000) joe       (1000)     2466 2023-06-22 15:53:47.000000 pysvgedit-0.0.2/pysvgedit/SVGValidator.py
+-rw-------   0 joe       (1000) joe       (1000)     1693 2023-06-22 18:01:49.000000 pysvgedit-0.0.2/pysvgedit/Vector2D.py
+-rw-------   0 joe       (1000) joe       (1000)     1967 2023-06-18 18:50:02.000000 pysvgedit-0.0.2/pysvgedit/XMLTools.py
+-rw-------   0 joe       (1000) joe       (1000)     1273 2023-06-22 18:10:57.000000 pysvgedit-0.0.2/pysvgedit/__init__.py
+drwx------   0 joe       (1000) joe       (1000)        0 2023-06-22 18:11:04.478366 pysvgedit-0.0.2/pysvgedit/apps/
+-rw-------   0 joe       (1000) joe       (1000)     3109 2023-06-22 16:15:36.000000 pysvgedit-0.0.2/pysvgedit/apps/AnimationRendererApp.py
+-rw-------   0 joe       (1000) joe       (1000)     3101 2023-06-18 08:03:19.000000 pysvgedit-0.0.2/pysvgedit/apps/FriendlyArgumentParser.py
+-rw-------   0 joe       (1000) joe       (1000)     4243 2023-06-22 15:58:07.000000 pysvgedit-0.0.2/pysvgedit/apps/MakoRendererApp.py
+-rw-------   0 joe       (1000) joe       (1000)     1536 2023-06-22 15:58:00.000000 pysvgedit-0.0.2/pysvgedit/apps/ValidatorApp.py
+-rw-------   0 joe       (1000) joe       (1000)      841 2023-06-18 08:03:02.000000 pysvgedit-0.0.2/pysvgedit/apps/__init__.py
+drwx------   0 joe       (1000) joe       (1000)        0 2023-06-22 18:11:04.478366 pysvgedit-0.0.2/pysvgedit.egg-info/
+-rw-------   0 joe       (1000) joe       (1000)     1178 2023-06-22 18:11:04.000000 pysvgedit-0.0.2/pysvgedit.egg-info/PKG-INFO
+-rw-------   0 joe       (1000) joe       (1000)      738 2023-06-22 18:11:04.000000 pysvgedit-0.0.2/pysvgedit.egg-info/SOURCES.txt
+-rw-------   0 joe       (1000) joe       (1000)        1 2023-06-22 18:11:04.000000 pysvgedit-0.0.2/pysvgedit.egg-info/dependency_links.txt
+-rw-------   0 joe       (1000) joe       (1000)      229 2023-06-22 18:11:04.000000 pysvgedit-0.0.2/pysvgedit.egg-info/entry_points.txt
+-rw-------   0 joe       (1000) joe       (1000)       10 2023-06-22 18:11:04.000000 pysvgedit-0.0.2/pysvgedit.egg-info/top_level.txt
+-rw-------   0 joe       (1000) joe       (1000)       38 2023-06-22 18:11:04.478366 pysvgedit-0.0.2/setup.cfg
+-rw-------   0 joe       (1000) joe       (1000)     1438 2023-06-22 18:11:04.000000 pysvgedit-0.0.2/setup.py
```

### Comparing `pysvgedit-0.0.1/LICENSE` & `pysvgedit-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pysvgedit-0.0.1/PKG-INFO` & `pysvgedit-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pysvgedit
-Version: 0.0.1
+Version: 0.0.2
 Summary: Native Python library to create and edit SVG documents
 Home-page: https://github.com/johndoe31415/pysvgedit
-Download-URL: https://github.com/johndoe31415/pysvgedit/archive/v0.0.1.tar.gz
+Download-URL: https://github.com/johndoe31415/pysvgedit/archive/v0.0.2.tar.gz
 Author: Johannes Bauer
 Author-email: joe@johannes-bauer.com
 License: gpl-3.0
 Keywords: svg
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `pysvgedit-0.0.1/pysvgedit/SVGCircle.py` & `pysvgedit-0.0.2/pysvgedit/SVGCircle.py`

 * *Files 19% similar despite different names*

```diff
@@ -14,20 +14,21 @@
 #	GNU General Public License for more details.
 #
 #	You should have received a copy of the GNU General Public License
 #	along with pysvgedit; if not, write to the Free Software
 #	Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307  USA
 #
 
-from .SVGObject import SVGObject, SVGXYObject, SVGWidthHeightObject, SVGStyleObject
-from .Vector2D import Vector2D
+from .SVGObject import SVGObject, SVGXYObject, SVGStyleObject
 
 @SVGObject.register
 class SVGCircle(SVGObject, SVGXYObject, SVGStyleObject):
 	_TAG_NAME = "circle"
+	_X_ATTRIBUTE_NAME = "cx"
+	_X_ATTRIBUTE_NAME = "cy"
 
 	@property
 	def radius(self):
 		return self._get_float_attribute("r")
 
 	@radius.setter
 	def radius(self, value):
```

### Comparing `pysvgedit-0.0.1/pysvgedit/SVGDefs.py` & `pysvgedit-0.0.2/pysvgedit/SVGDefs.py`

 * *Files identical despite different names*

### Comparing `pysvgedit-0.0.1/pysvgedit/SVGDocument.py` & `pysvgedit-0.0.2/pysvgedit/SVGDocument.py`

 * *Files identical despite different names*

### Comparing `pysvgedit-0.0.1/pysvgedit/SVGGroup.py` & `pysvgedit-0.0.2/pysvgedit/SVGGroup.py`

 * *Files identical despite different names*

### Comparing `pysvgedit-0.0.1/pysvgedit/SVGObject.py` & `pysvgedit-0.0.2/pysvgedit/SVGObject.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,32 +19,35 @@
 #
 
 from .XMLTools import XMLTools
 from .SVGStyle import SVGStyle
 from .Vector2D import Vector2D
 
 class SVGXYObject():
+	_X_ATTRIBUTE_NAME = "x"
+	_Y_ATTRIBUTE_NAME = "y"
+
 	@property
 	def pos(self):
-		return Vector2D(x = self._get_float_attribute("x"), y = self._get_float_attribute("y"))
+		return Vector2D(x = self._get_float_attribute(self._X_ATTRIBUTE_NAME), y = self._get_float_attribute(self._Y_ATTRIBUTE_NAME))
 
 	@pos.setter
 	def pos(self, value: Vector2D):
-		self._node.setAttribute("x", str(value.x))
-		self._node.setAttribute("y", str(value.y))
+		self.node.setAttribute(self._X_ATTRIBUTE_NAME, str(value.x))
+		self.node.setAttribute(self._Y_ATTRIBUTE_NAME, str(value.y))
 
 class SVGWidthHeightObject():
 	@property
 	def extents(self):
 		return Vector2D(x = self._get_float_attribute("width"), y = self._get_float_attribute("height"))
 
 	@extents.setter
 	def extents(self, value: Vector2D):
-		self._node.setAttribute("width", str(value.x))
-		self._node.setAttribute("height", str(value.y))
+		self.node.setAttribute("width", str(value.x))
+		self.node.setAttribute("height", str(value.y))
 
 
 class SVGStyleObject():
 	@property
 	def style(self):
 		return SVGStyle.from_node(self.node, auto_sync = True)
```

### Comparing `pysvgedit-0.0.1/pysvgedit/SVGPath.py` & `pysvgedit-0.0.2/pysvgedit/SVGPath.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from .Vector2D import Vector2D
 
 @SVGObject.register
 class SVGPath(SVGObject, SVGStyleObject):
 	_TAG_NAME = "path"
 
 	def clear(self, pos):
-		path.node.setAttribute("d", f"M {pos.x} {pos.y}")
+		self.node.setAttribute("d", f"M {pos.x} {pos.y}")
 		return self
 
 	def __append_path(self, strvalue):
 		self.node.setAttribute("d", f"{self.node.getAttribute('d')} {strvalue}")
 
 	def horizontal(self, x, relative = False):
 		self.__append_path(f"{'h' if relative else 'H'} {x}")
@@ -41,15 +41,15 @@
 		return self
 
 	def lineto(self, pos, relative = False):
 		self.__append_path(f"{'l' if relative else 'L'} {pos.x} {pos.y}")
 		return self
 
 	def bezierto(self, p1, p2, p3, relative = False):
-		self.__append_path(f"{'c' if relative else 'C'} {pos.x} {pos.y} {p1.x} {p1.y} {p2.x} {p2.y} {p3.x} {p3.y}")
+		self.__append_path(f"{'c' if relative else 'C'} {p1.x} {p1.y} {p2.x} {p2.y} {p3.x} {p3.y}")
 		return self
 
 	def arcto(self, pos, radius, xrotation = 0, large_arc = True, sweep = True, relative = False):
 		if isinstance(radius, float) or isinstance(radius, int):
 			radius = Vector2D(radius, radius)
 		self.__append_path(f"{'a' if relative else 'A'} {radius.x} {radius.y} {xrotation} {1 if large_arc else 0},{1 if sweep else 0} {pos.x} {pos.y}")
 		return self
```

### Comparing `pysvgedit-0.0.1/pysvgedit/SVGRect.py` & `pysvgedit-0.0.2/pysvgedit/SVGRect.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,21 +14,37 @@
 #	GNU General Public License for more details.
 #
 #	You should have received a copy of the GNU General Public License
 #	along with pysvgedit; if not, write to the Free Software
 #	Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307  USA
 #
 
-from .SVGObject import SVGObject, SVGXYObject, SVGWidthHeightObject, SVGStyleObject
 from .Vector2D import Vector2D
+from .SVGObject import SVGObject, SVGXYObject, SVGWidthHeightObject, SVGStyleObject
 
 @SVGObject.register
 class SVGRect(SVGObject, SVGXYObject, SVGWidthHeightObject, SVGStyleObject):
 	_TAG_NAME = "rect"
 
+	@property
+	def p1(self):
+		return self.pos
+
+	@property
+	def p2(self):
+		return Vector2D(self.pos.x, self.pos.y + self.extents.y)
+
+	@property
+	def p3(self):
+		return self.pos + self.extents
+
+	@property
+	def p4(self):
+		return Vector2D(self.pos.x + self.extents.x, self.pos.y)
+
 	@classmethod
 	def new(cls, pos, extents):
 		path = cls(cls._new_element())
 		path.pos = pos
 		path.extents = extents
 		path.style.default_path()
 		return path
```

### Comparing `pysvgedit-0.0.1/pysvgedit/SVGStyle.py` & `pysvgedit-0.0.2/pysvgedit/SVGStyle.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,14 +52,18 @@
 	@property
 	def is_visible(self):
 		if "display" in self._style:
 			hidden = (self["display"].lower() == "none")
 			return not hidden
 		return True
 
+	def clear(self):
+		self._style = { }
+		self._on_style_changed()
+
 	def hide(self):
 		self["display"] = "none"
 
 	def show(self):
 		self["display"] = None
 
 	@classmethod
@@ -132,23 +136,30 @@
 			"stroke":			"none",
 		})
 		return self
 
 	def _setitem(self, key, value):
 		changed = False
 		if (value is None) and (key in self._style):
-			del self._style[value]
+			del self._style[key]
 			changed = True
 		else:
 			changed = self[key] != value
 			self._style[key] = value
 		return changed
 
 	def __setitem__(self, key: str, value: str):
 		if self._setitem(key, value):
 			self._on_style_changed()
 
 	def __getitem__(self, key: str):
 		return self._style.get(key)
 
+	def get(self, key: str, unstringify = False):
+		value = self._style.get(key)
+		if unstringify and (value is not None):
+			if (value.startswith("'") and value.endswith("'")) or (value.startswith("\"") and value.endswith("\"")):
+				value = value[1 : -1]
+		return value
+
 	def __str__(self):
 		return f"SVGStyle<{self._style}>"
```

### Comparing `pysvgedit-0.0.1/pysvgedit/SVGText.py` & `pysvgedit-0.0.2/pysvgedit/SVGText.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,35 +16,35 @@
 #	You should have received a copy of the GNU General Public License
 #	along with pysvgedit; if not, write to the Free Software
 #	Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307  USA
 #
 
 from .SVGObject import SVGObject, SVGXYObject, SVGStyleObject
 from .XMLTools import XMLTools
-from .SVGStyle import SVGStyle
 
 @SVGObject.register
 class SVGTextSpan(SVGObject, SVGXYObject, SVGStyleObject):
 	_TAG_NAME = "tspan"
 
 	def __init__(self, tspan_node):
 		super().__init__(tspan_node)
 		try:
 			self._text_node = next(child for child in tspan_node.childNodes if (child.nodeType == child.TEXT_NODE))
 		except StopIteration:
 			# No text node, create one (with empty text)
 			self._text_node = tspan_node.appendChild(tspan_node.ownerDocument.createTextNode(""))
 
 	@classmethod
-	def new(cls, pos, text = ""):
+	def new(cls, pos = None, text = ""):
 		tspan_node = cls._new_element()
 		tspan_node.appendChild(tspan_node.ownerDocument.createTextNode(text))
 
 		svg_textspan = cls(tspan_node)
-		svg_textspan.pos = pos
+		if pos is not None:
+			svg_textspan.pos = pos
 		return svg_textspan
 
 	@property
 	def text(self):
 		return self._text_node.wholeText
 
 	@text.setter
@@ -58,20 +58,21 @@
 		return f"tspan<{self.text}>"
 
 @SVGObject.register
 class SVGText(SVGObject, SVGStyleObject):
 	_TAG_NAME = "text"
 
 	@classmethod
-	def new(cls, pos, text = ""):
+	def new(cls, pos = None, text = ""):
 		svg_text = cls(cls._new_element())
 		svg_text.node.setAttribute("xml:space", "preserve")
-		svg_text.pos = pos
+		if pos is not None:
+			svg_text.pos = pos
 		svg_text.style.default_text()
-		svg_text.node.appendChild(SVGTextSpan.new(pos, text).node)
+		svg_text.node.appendChild(SVGTextSpan.new(pos = pos, text = text).node)
 		return svg_text
 
 	@property
 	def tspans(self):
 		return (SVGTextSpan(node) for node in XMLTools.find_all_elements(self.node, "tspan"))
 
 	@property
```

### Comparing `pysvgedit-0.0.1/pysvgedit/XMLTools.py` & `pysvgedit-0.0.2/pysvgedit/XMLTools.py`

 * *Files identical despite different names*

### Comparing `pysvgedit-0.0.1/pysvgedit/__init__.py` & `pysvgedit-0.0.2/pysvgedit/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -23,9 +23,12 @@
 from .SVGDefs import SVGDefs
 from .SVGGroup import SVGGroup
 from .SVGStyle import SVGStyle
 from .SVGText import SVGText
 from .SVGPath import SVGPath
 from .SVGRect import SVGRect
 from .SVGCircle import SVGCircle
+from .SVGAnimation import SVGAnimation, SVGAnimationMode
+from .SVGValidator import SVGValidator
+from .Exceptions import SVGException
 
-VERSION = "0.0.1"
+VERSION = "0.0.2"
```

### Comparing `pysvgedit-0.0.1/pysvgedit/apps/FriendlyArgumentParser.py` & `pysvgedit-0.0.2/pysvgedit/apps/FriendlyArgumentParser.py`

 * *Files identical despite different names*

### Comparing `pysvgedit-0.0.1/pysvgedit/apps/MakoRendererApp.py` & `pysvgedit-0.0.2/pysvgedit/apps/MakoRendererApp.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -18,17 +18,17 @@
 #	Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307  USA
 #
 
 import sys
 import json
 import tempfile
 import subprocess
+import datetime
 import mako.template
 import pysvgedit
-import datetime
 from .FriendlyArgumentParser import FriendlyArgumentParser
 
 class HelperClass():
 	pass
 
 class MakoRendererApp():
 	def __init__(self, args):
```

### Comparing `pysvgedit-0.0.1/pysvgedit/apps/__init__.py` & `pysvgedit-0.0.2/pysvgedit/apps/__init__.py`

 * *Files identical despite different names*

### Comparing `pysvgedit-0.0.1/pysvgedit.egg-info/PKG-INFO` & `pysvgedit-0.0.2/pysvgedit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pysvgedit
-Version: 0.0.1
+Version: 0.0.2
 Summary: Native Python library to create and edit SVG documents
 Home-page: https://github.com/johndoe31415/pysvgedit
-Download-URL: https://github.com/johndoe31415/pysvgedit/archive/v0.0.1.tar.gz
+Download-URL: https://github.com/johndoe31415/pysvgedit/archive/v0.0.2.tar.gz
 Author: Johannes Bauer
 Author-email: joe@johannes-bauer.com
 License: gpl-3.0
 Keywords: svg
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `pysvgedit-0.0.1/pysvgedit.egg-info/SOURCES.txt` & `pysvgedit-0.0.2/pysvgedit.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 LICENSE
 README.md
 setup.py
+pysvgedit/Exceptions.py
+pysvgedit/SVGAnimation.py
 pysvgedit/SVGCircle.py
 pysvgedit/SVGDefs.py
 pysvgedit/SVGDocument.py
 pysvgedit/SVGGroup.py
 pysvgedit/SVGObject.py
 pysvgedit/SVGPath.py
 pysvgedit/SVGRect.py
 pysvgedit/SVGStyle.py
 pysvgedit/SVGText.py
+pysvgedit/SVGTransformation.py
+pysvgedit/SVGValidator.py
 pysvgedit/Vector2D.py
 pysvgedit/XMLTools.py
 pysvgedit/__init__.py
 pysvgedit.egg-info/PKG-INFO
 pysvgedit.egg-info/SOURCES.txt
 pysvgedit.egg-info/dependency_links.txt
 pysvgedit.egg-info/entry_points.txt
 pysvgedit.egg-info/top_level.txt
+pysvgedit/apps/AnimationRendererApp.py
 pysvgedit/apps/FriendlyArgumentParser.py
 pysvgedit/apps/MakoRendererApp.py
+pysvgedit/apps/ValidatorApp.py
 pysvgedit/apps/__init__.py
```

### Comparing `pysvgedit-0.0.1/setup.py` & `pysvgedit-0.0.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,29 +2,31 @@
 
 with open("README.md") as f:
 	long_description = f.read()
 
 setuptools.setup(
 	name = "pysvgedit",
 	packages = setuptools.find_packages(),
-	version = "0.0.1",
+	version = "0.0.2",
 	license = "gpl-3.0",
 	description = "Native Python library to create and edit SVG documents",
 	long_description = long_description,
 	long_description_content_type = "text/markdown",
 	author = "Johannes Bauer",
 	author_email = "joe@johannes-bauer.com",
 	url = "https://github.com/johndoe31415/pysvgedit",
-	download_url = "https://github.com/johndoe31415/pysvgedit/archive/v0.0.1.tar.gz",
+	download_url = "https://github.com/johndoe31415/pysvgedit/archive/v0.0.2.tar.gz",
 	keywords = [ "svg" ],
 	install_requires = [
 	],
 	entry_points = {
 		"console_scripts": [
-			"svgmakorender = pysvgedit.apps.MakoRendererApp:MakoRendererApp.main"
+			"svgmakorender = pysvgedit.apps.MakoRendererApp:MakoRendererApp.main",
+			"svganimationrender = pysvgedit.apps.AnimationRendererApp:AnimationRendererApp.main",
+			"svgvalidate = pysvgedit.apps.ValidatorApp:ValidatorApp.main",
 		]
 	},
 	include_package_data = False,
 	classifiers = [
 		"Development Status :: 4 - Beta",
 		"Intended Audience :: Developers",
 		"License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
```

