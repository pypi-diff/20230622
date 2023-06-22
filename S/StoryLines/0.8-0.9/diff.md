# Comparing `tmp/StoryLines-0.8.tar.gz` & `tmp/StoryLines-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "StoryLines-0.8.tar", last modified: Sat Jul 30 16:30:16 2022, max compression
+gzip compressed data, was "StoryLines-0.9.tar", last modified: Sat Nov 19 18:18:11 2022, max compression
```

## Comparing `StoryLines-0.8.tar` & `StoryLines-0.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 jan       (1000) jan       (1000)        0 2022-07-30 16:30:16.047201 StoryLines-0.8/
--rw-rw-r--   0 jan       (1000) jan       (1000)      643 2022-01-06 18:38:11.000000 StoryLines-0.8/LICENSE
--rw-r--r--   0 jan       (1000) jan       (1000)     1562 2022-07-30 16:30:16.047201 StoryLines-0.8/PKG-INFO
--rw-r--r--   0 jan       (1000) jan       (1000)     1166 2022-06-15 07:55:15.000000 StoryLines-0.8/README.md
-drwxr-xr-x   0 jan       (1000) jan       (1000)        0 2022-07-30 16:30:16.047201 StoryLines-0.8/StoryLines.egg-info/
--rw-r--r--   0 jan       (1000) jan       (1000)     1562 2022-07-30 16:30:16.000000 StoryLines-0.8/StoryLines.egg-info/PKG-INFO
--rw-r--r--   0 jan       (1000) jan       (1000)      407 2022-07-30 16:30:16.000000 StoryLines-0.8/StoryLines.egg-info/SOURCES.txt
--rw-r--r--   0 jan       (1000) jan       (1000)        1 2022-07-30 16:30:16.000000 StoryLines-0.8/StoryLines.egg-info/dependency_links.txt
--rw-r--r--   0 jan       (1000) jan       (1000)       11 2022-07-30 16:30:16.000000 StoryLines-0.8/StoryLines.egg-info/top_level.txt
--rw-rw-r--   0 jan       (1000) jan       (1000)       98 2021-05-20 16:11:53.000000 StoryLines-0.8/pyproject.toml
--rw-r--r--   0 jan       (1000) jan       (1000)      502 2022-07-30 16:30:16.047201 StoryLines-0.8/setup.cfg
--rwxrwxr-x   0 jan       (1000) jan       (1000)       62 2022-05-21 20:15:34.000000 StoryLines-0.8/setup.py
-drwxr-xr-x   0 jan       (1000) jan       (1000)        0 2022-07-30 16:30:16.047201 StoryLines-0.8/storylines/
--rw-r--r--   0 jan       (1000) jan       (1000)      668 2022-07-30 16:27:39.000000 StoryLines-0.8/storylines/__init__.py
--rw-r--r--   0 jan       (1000) jan       (1000)     3855 2022-06-17 06:49:44.000000 StoryLines-0.8/storylines/calc.py
--rw-r--r--   0 jan       (1000) jan       (1000)     7931 2022-07-30 10:35:42.000000 StoryLines-0.8/storylines/color.py
--rw-r--r--   0 jan       (1000) jan       (1000)      967 2022-06-17 06:49:44.000000 StoryLines-0.8/storylines/convert.py
--rw-r--r--   0 jan       (1000) jan       (1000)     6610 2022-06-17 06:49:44.000000 StoryLines-0.8/storylines/cut.py
--rw-r--r--   0 jan       (1000) jan       (1000)     4385 2022-06-17 06:49:44.000000 StoryLines-0.8/storylines/fatband.py
--rw-r--r--   0 jan       (1000) jan       (1000)     4440 2022-06-17 06:49:44.000000 StoryLines-0.8/storylines/files.py
--rw-r--r--   0 jan       (1000) jan       (1000)     1230 2022-06-17 06:49:44.000000 StoryLines-0.8/storylines/group.py
--rw-r--r--   0 jan       (1000) jan       (1000)    49123 2022-07-30 07:09:47.000000 StoryLines-0.8/storylines/plot.py
--rw-r--r--   0 jan       (1000) jan       (1000)     2772 2022-06-17 06:49:44.000000 StoryLines-0.8/storylines/png.py
--rw-r--r--   0 jan       (1000) jan       (1000)     3159 2022-06-17 06:49:25.000000 StoryLines-0.8/storylines/proj.py
+drwxr-xr-x   0 jan       (1000) jan       (1000)        0 2022-11-19 18:18:11.291002 StoryLines-0.9/
+-rw-rw-r--   0 jan       (1000) jan       (1000)      643 2022-01-06 18:38:11.000000 StoryLines-0.9/LICENSE
+-rw-r--r--   0 jan       (1000) jan       (1000)     1562 2022-11-19 18:18:11.291002 StoryLines-0.9/PKG-INFO
+-rw-r--r--   0 jan       (1000) jan       (1000)     1166 2022-06-15 07:55:15.000000 StoryLines-0.9/README.md
+drwxr-xr-x   0 jan       (1000) jan       (1000)        0 2022-11-19 18:18:11.291002 StoryLines-0.9/StoryLines.egg-info/
+-rw-r--r--   0 jan       (1000) jan       (1000)     1562 2022-11-19 18:18:11.000000 StoryLines-0.9/StoryLines.egg-info/PKG-INFO
+-rw-r--r--   0 jan       (1000) jan       (1000)      407 2022-11-19 18:18:11.000000 StoryLines-0.9/StoryLines.egg-info/SOURCES.txt
+-rw-r--r--   0 jan       (1000) jan       (1000)        1 2022-11-19 18:18:11.000000 StoryLines-0.9/StoryLines.egg-info/dependency_links.txt
+-rw-r--r--   0 jan       (1000) jan       (1000)       11 2022-11-19 18:18:11.000000 StoryLines-0.9/StoryLines.egg-info/top_level.txt
+-rw-rw-r--   0 jan       (1000) jan       (1000)       98 2021-05-20 16:11:53.000000 StoryLines-0.9/pyproject.toml
+-rw-r--r--   0 jan       (1000) jan       (1000)      502 2022-11-19 18:18:11.291002 StoryLines-0.9/setup.cfg
+-rwxrwxr-x   0 jan       (1000) jan       (1000)       62 2022-05-21 20:15:34.000000 StoryLines-0.9/setup.py
+drwxr-xr-x   0 jan       (1000) jan       (1000)        0 2022-11-19 18:18:11.291002 StoryLines-0.9/storylines/
+-rw-r--r--   0 jan       (1000) jan       (1000)      668 2022-11-19 18:15:46.000000 StoryLines-0.9/storylines/__init__.py
+-rw-r--r--   0 jan       (1000) jan       (1000)     3855 2022-06-17 06:49:44.000000 StoryLines-0.9/storylines/calc.py
+-rw-r--r--   0 jan       (1000) jan       (1000)     7931 2022-07-30 10:35:42.000000 StoryLines-0.9/storylines/color.py
+-rw-r--r--   0 jan       (1000) jan       (1000)      967 2022-06-17 06:49:44.000000 StoryLines-0.9/storylines/convert.py
+-rw-r--r--   0 jan       (1000) jan       (1000)     6610 2022-06-17 06:49:44.000000 StoryLines-0.9/storylines/cut.py
+-rw-r--r--   0 jan       (1000) jan       (1000)     4385 2022-06-17 06:49:44.000000 StoryLines-0.9/storylines/fatband.py
+-rw-r--r--   0 jan       (1000) jan       (1000)     4437 2022-10-06 14:37:35.000000 StoryLines-0.9/storylines/files.py
+-rw-r--r--   0 jan       (1000) jan       (1000)     1230 2022-06-17 06:49:44.000000 StoryLines-0.9/storylines/group.py
+-rw-r--r--   0 jan       (1000) jan       (1000)    51482 2022-11-04 12:43:57.000000 StoryLines-0.9/storylines/plot.py
+-rw-r--r--   0 jan       (1000) jan       (1000)     2772 2022-06-17 06:49:44.000000 StoryLines-0.9/storylines/png.py
+-rw-r--r--   0 jan       (1000) jan       (1000)     3493 2022-11-19 17:57:13.000000 StoryLines-0.9/storylines/proj.py
```

### Comparing `StoryLines-0.8/LICENSE` & `StoryLines-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `StoryLines-0.8/PKG-INFO` & `StoryLines-0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: StoryLines
-Version: 0.8
+Version: 0.9
 Summary: Line plots with Python & TikZ
 Home-page: https://github.com/janberges/StoryLines
 Author: Jan Berges
 Author-email: 
 Classifier: Programming Language :: Python
 Classifier: License :: Freely Distributable
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `StoryLines-0.8/README.md` & `StoryLines-0.9/README.md`

 * *Files identical despite different names*

### Comparing `StoryLines-0.8/StoryLines.egg-info/PKG-INFO` & `StoryLines-0.9/StoryLines.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: StoryLines
-Version: 0.8
+Version: 0.9
 Summary: Line plots with Python & TikZ
 Home-page: https://github.com/janberges/StoryLines
 Author: Jan Berges
 Author-email: 
 Classifier: Programming Language :: Python
 Classifier: License :: Freely Distributable
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `StoryLines-0.8/storylines/__init__.py` & `StoryLines-0.9/storylines/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright (C) 2016-2022 Jan Berges
 # This program is free software under the terms of the BSD Zero Clause License.
 
 """Line plots with Python & TikZ."""
 
-__version__ = '0.8'
+__version__ = '0.9'
 
 from .plot import Plot
 from .calc import (order_of_magnitude, power_of_ten, xround, xround_mantissa,
     multiples, dot, cross, bonds)
 from .color import Color, colormap, colorize, HSV2RGB, RGB2HSV, PSV2RGB
 from .convert import inch, pt, csv
 from .cut import relevant, shortcut, cut, cut2d, jump
```

### Comparing `StoryLines-0.8/storylines/calc.py` & `StoryLines-0.9/storylines/calc.py`

 * *Files identical despite different names*

### Comparing `StoryLines-0.8/storylines/color.py` & `StoryLines-0.9/storylines/color.py`

 * *Files identical despite different names*

### Comparing `StoryLines-0.8/storylines/convert.py` & `StoryLines-0.9/storylines/convert.py`

 * *Files identical despite different names*

### Comparing `StoryLines-0.8/storylines/cut.py` & `StoryLines-0.9/storylines/cut.py`

 * *Files identical despite different names*

### Comparing `StoryLines-0.8/storylines/fatband.py` & `StoryLines-0.9/storylines/fatband.py`

 * *Files identical despite different names*

### Comparing `StoryLines-0.8/storylines/files.py` & `StoryLines-0.9/storylines/files.py`

 * *Files 0% similar despite different names*

```diff
@@ -124,15 +124,15 @@
     """
     stem, typ, home = goto(filename)
 
     png = png or typ == 'png'
     pdf = pdf or typ == 'pdf' or png
 
     with open('%s.tex' % stem, 'w') as tex:
-        tex.write('\\documentclass[varwidth=\maxdimen]{standalone}\n'
+        tex.write('\\documentclass[varwidth=1189mm]{standalone}\n'
             '\\usepackage{graphicx}\n'
             '\\begin{document}\n'
             '\\noindent%\n')
 
         if halign == 'center':
             tex.write('\\centering%\n')
         elif halign == 'right':
```

### Comparing `StoryLines-0.8/storylines/group.py` & `StoryLines-0.9/storylines/group.py`

 * *Files identical despite different names*

### Comparing `StoryLines-0.8/storylines/plot.py` & `StoryLines-0.9/storylines/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,36 +5,37 @@
 
 from __future__ import division
 
 import math
 import re
 
 from .calc import power_of_ten, xround_mantissa, multiples
-from .color import colorize
+from .color import Color, colormap, colorize
 from .convert import inch, pt, csv
 from .cut import relevant, shortcut, cut2d, jump
 from .fatband import fatband, miter_butt
 from .files import goto, typeset, rasterize
 from .group import islands, groups
 from .png import save
 
 class Plot():
     """Plot object.
 
     Parameters
     ----------
-    width : float, default 8.0
+    width : float, default None
          Figure width in cm. A negative value is interpreted as the inner width
          (without left and right margins). If zero, the x-axis scale is set
-         equal to the y-axis scale and the width is inferred from the height.
-    height : float, default 6.0
+         equal to the y-axis scale and the width is inferred from the height. By
+         default, the single-column width for the chosen `style` is used.
+    height : float, default None
          Figure height in cm. A negative value is interpreted as the inner
          height (without bottom and top margins). If zero, the y-axis scale is
          set equal to the x-axis scale and the height is inferred from the
-         width.
+         width. By default, it is inferred from `width` for a 4:3 aspect ratio.
     margin : float, default None
         Default margin in cm. If ``None``, margins are set automatically. This
         is not always the best option.
     xyaxes : bool, default True
         Draw x and y axes?
     style : str, default None
         Predefined style. Possible values are ``'Nature'``, ``'NatCommun'``,
@@ -84,17 +85,19 @@
     xpadding, ypadding, zpadding : float, default 0.0
         Padding between data and axes in data units.
     xclose, yclose, zclose : bool, default False
         Place axis labels in space reserved for tick labels.
     xformat, yformat, zformat : function
         Tick formatter. Takes tick position as argument.
     lower : str, default 'blue'
-        Lower color of colorbar.
+        Lower color of colorbar. Can also be of type ``Color`` as long as
+        `upper` has the same type.
     upper : str, default 'red'
-        Upper color of colorbar.
+        Upper color of colorbar. Can also be of type ``Color`` as long as
+        `lower` has the same type.
     cmap : function, default None
         Colormap for colorbar used instead of `lower` and `upper`.
     title : str, default None
         Plot title.
     label : str, default None
         Subfigure label, e.g., ``'a'``.
     labelsize : int, default None
@@ -162,27 +165,37 @@
         otherwise.
     font : str, default None
         Predefined font selection. Imitates well-known fonts. Possible values
         are ``'Gill Sans'``, ``'Helvetica'``, ``'Iwona'``, ``'Latin Modern'``,
         and ``'Times'``.
     fontsize : int, default 10
         Font size for standalone figures in pt.
+    single : float, default 8.0
+        Single-column width for the chosen `style`.
+    double : float, default 17.0
+        Full textwidth for the chosen `style`.
+    resolution : float, default 1e-3
+        Smallest distance in cm expected to be discernible when looking at the
+        plot. The default is acceptable when the plot is viewed or printed in
+        its original size. For zooming, smaller values may be necessary. This
+        parameter determines the number of vertices used to render a line and
+        thus affects the file size.
     lines : list
         List of all line objects.
     options : dict
         Global TikZ options.
 
     Notes
     -----
     In all textual attributes and parameters, numbers in angle brackets are
     interpreted as values in y data units, e.g., ``line_width='<0.1>'``. For
     the parameters `line_width` and `mark_size` this is also the case if an
     integer or float is passed instead of a string.
     """
-    def __init__(self, width=8.0, height=6.0, margin=None, xyaxes=True,
+    def __init__(self, width=None, height=None, margin=None, xyaxes=True,
             style=None, rounded=True, **more):
 
         self.width = width
         self.height = height
 
         self.left = margin
         self.right = margin
@@ -252,14 +265,19 @@
 
         self.preamble = ''
         self.inputenc = None
         self.fontenc = None
         self.font = None
         self.fontsize = 10
 
+        self.single = 8.0
+        self.double = 17.0
+
+        self.resolution = 1e-3
+
         self.lines = []
 
         self.options = dict(mark_size='0.05cm')
 
         if rounded:
             self.options.update(line_cap='round', line_join='round')
 
@@ -268,29 +286,35 @@
                 self.font = 'Helvetica'
                 self.fontsize = 7
                 self.labelsize = 8
                 self.labelformat = lambda x: '\\textbf{%s}' % x
                 self.single = 8.9
                 self.double = 18.3
 
-            if style == 'NatCommun':
+            elif style == 'NatCommun':
                 self.font = 'Helvetica'
                 self.fontsize = 8
                 self.labelsize = 9
                 self.labelformat = lambda x: '\\textbf{%s}' % x
                 self.single = 8.8
                 self.double = 18.0
 
             elif style == 'APS':
                 self.font = 'Times'
                 self.fontsize = 9
                 self.labelformat = lambda x: '(%s)' % x
                 self.single = 8.6
                 self.double = 17.8
 
+        if self.width is None:
+            self.width = self.single
+
+        if self.height is None:
+            self.height = 3 * self.width / 4
+
         for name, value in more.items():
             if hasattr(self, name):
                 setattr(self, name, value)
             else:
                 self.options[name] = value
 
     def line(self,
@@ -310,15 +334,15 @@
             nib=None,
             omit=None,
             protrusion=0,
             sgn=+1,
             shifts=None,
             shortcut=0,
             shortcut_rel=0.5,
-            thickness=1,
+            thickness=0.05,
             weights=None,
             xref=None,
             yref=None,
             zindex=None,
 
             **options):
         """Add line/curve.
@@ -330,16 +354,18 @@
         z : float, default None
             z value for entire line, represented by color.
         axes : bool, default False
             Draw axes at current z index? By default, the axes are drawn on top
             of all data.
         code : str, default None
             Literal TikZ code to be inserted at current position.
-        cut : bool, default False
-            Cut off line segments beyond plotting range?
+        cut : bool or tuple, default False
+            Cut off line segments beyond plotting range? It is also possible to
+            pass the clipping window as a tuple ``(xmin, xmax, ymin, ymax)`` in
+            data coordinates, where ``None`` is replaced by the plot bounds.
         frame : bool, default False
             Draw frame at current z index? By default, the frame is drawn just
             below the axes.
         grid : bool, default False
             Add grid lines (at tick positions) at current z index? By default,
             the grid is drawn just below the frame.
         join : bool, default None
@@ -368,16 +394,16 @@
         shifts : list of float
             Displacements in weight direction of fatband.
         shortcut : float, default 0
             Maximum length of loop to be cut off.
         shortcut_rel : float, default 0.5
             Maximum length of loop to be cut off relative to the total length
             of the curve. This is only used if `shortcut` is nonzero.
-        thickness : float, default 1
-            Overall fatband linewidth scaling factor.
+        thickness : float, default 0.05
+           Fatband linewidth in cm.
         weights : list of float
             Fatband weights.
         xref, yref : float, default None
             Reference values for filled curves. This is useful to visualize
             integrands such as a density of states.
         zindex : int, default None
             Index of list of lines where new line is inserted. By default, the
@@ -421,25 +447,28 @@
             )
 
         if zindex is None:
             self.lines.append(new_line)
         else:
             self.lines.insert(zindex, new_line)
 
-    def fatband(self, x, y, weights=1.0, shifts=0.0, **options):
+    def fatband(self, x, y, weights=1.0, shifts=0.0, fill=True, draw='none',
+            **options):
         """Draw fatband.
 
         Parameters
         ----------
         x, y : list
             Vertices of linear spline.
-        weights : list of float or float
+        weights : list of float or float, default 1.0
             Weights of `x` and `y`.
-        shifts : list of float or float
+        shifts : list of float or float, default 0.0
             Displacements in weight direction.
+        fill, draw : str or Color
+            TikZ line options (filled without outline by default).
         **options
             Options passed to `line` function.
         """
         try:
             iter(weights)
         except TypeError:
             weights = [weights] * len(x)
@@ -450,15 +479,15 @@
 
         for island in islands(len(weights),
             lambda n: any(weights[max(n - 1, 0):n + 2])):
 
             if len(island) > 1:
                 n = slice(island[0], island[-1] + 1)
                 self.line(x[n], y[n], weights=weights[n], shifts=shifts[n],
-                    **options)
+                    fill=fill, draw=draw, **options)
 
     def compline(self, x, y, weights=1.0, colors=True, threshold=0.0,
             **options):
         """Represent points of multiple weights as composite fatband.
 
         Parameters
         ----------
@@ -834,14 +863,20 @@
             for line in self.lines:
                 if not len(line[x]) and len(line[y]) == 1:
                     line[x] = [lower[x], upper[x]]
                     line[y] = [line[y][0]] * 2
 
                     line['options'].setdefault('line_cap', 'butt')
 
+        # create simple colormap from special lower and upper colors:
+
+        if self.cmap is None:
+            if isinstance(self.upper, Color) and isinstance(self.lower, Color):
+                self.cmap = colormap((0, self.lower), (1, self.upper))
+
         # build LaTeX file
 
         labels = []
 
         stem, typ, home = goto(filename)
 
         png = png or typ == 'png'
@@ -850,16 +885,15 @@
         if pdf:
             standalone = True
 
         with open('%s.tex' % stem, 'w') as file:
             # print premable and open document
 
             if standalone:
-                file.write('\\documentclass[class=%s, %dpt, '
-                    'varwidth=\\maxdimen]{standalone}\n'
+                file.write('\\documentclass[class=%s, %dpt]{standalone}\n'
                     % ('article' if 10 <= self.fontsize <= 12 else 'scrartcl',
                         self.fontsize))
                 file.write('\\usepackage{tikz}\n')
 
                 if self.inputenc and 'inputenc' not in self.preamble:
                     file.write('\\usepackage[%s]{inputenc}\n' % self.inputenc)
 
@@ -981,15 +1015,15 @@
                 if draw_axes.done:
                     return
 
                 # paint colorbar
 
                 if self.colorbar:
                     if self.cmap is not None:
-                        dots = int(round(extent['z'] / inch * dpi))
+                        dots = max(2, int(round(extent['z'] / inch * dpi)))
 
                         colorbar = colorize([[n / (dots - 1.0)]
                             for n in reversed(range(dots))], self.cmap)
 
                         self.colorbar = '%s.bar.png' % stem
 
                         save(self.colorbar, colorbar)
@@ -1180,37 +1214,53 @@
                     if line['weights'] is not None:
                         segments = [(miter_butt if line['miter'] else fatband)(
                             segment, line['thickness'], line['weights'],
                             line['shifts'], line['nib'])
                             for segment in segments]
 
                     if line['cut']:
+                        try:
+                            xmin, xmax, ymin, ymax = line['cut']
+                        except (TypeError, ValueError):
+                            xmin = xmax = ymin = ymax = None
+
+                        xmin = (scale['x'] * (xmin - lower['x'])
+                            if xmin is not None else 0)
+
+                        xmax = (scale['x'] * (xmax - lower['x'])
+                            if xmax is not None else extent['x'])
+
+                        ymin = (scale['y'] * (ymin - lower['y'])
+                            if ymin is not None else 0)
+
+                        ymax = (scale['y'] * (ymax - lower['y'])
+                            if ymax is not None else extent['y'])
+
                         if line['join'] is None:
                             line['join'] = (line['options'].get('fill')
                                 is not None)
 
                         if line['options'].get('only_marks'):
                             segments = [[(x, y)
                                 for segment in segments
                                 for x, y in segment
-                                if 0 <= x <= extent['x']
-                                and 0 <= y <= extent['y']]]
+                                if xmin <= x <= xmax and ymin <= y <= ymax]]
                         else:
                             segments = [segment
                                 for segment in segments
                                 for segment in cut2d(segment,
-                                    0, extent['x'], 0, extent['y'],
-                                        line['join'])]
+                                    xmin, xmax, ymin, ymax, line['join'])]
 
                     if line['omit'] is None:
                         line['omit'] = 'mark' not in line['options']
 
                     for segment in segments:
                         if line['omit']:
-                            segment = relevant(segment[::line['sgn']])
+                            segment = relevant(segment[::line['sgn']],
+                                self.resolution)
 
                         elif line['cut'] and line['options'].get('mark') \
                                 and not line['options'].get('only_marks'):
 
                             line['options']['mark_indices'] \
                                 = '{%s}' % ','.join(str(n)
                                     for n, point in enumerate(segment, 1)
```

### Comparing `StoryLines-0.8/storylines/png.py` & `StoryLines-0.9/storylines/png.py`

 * *Files identical despite different names*

### Comparing `StoryLines-0.8/storylines/proj.py` & `StoryLines-0.9/storylines/proj.py`

 * *Files 14% similar despite different names*

```diff
@@ -66,35 +66,42 @@
     y = dot(Y, D) / adj
 
     # magnification factor ("zoom", "z-index"):
     z = sec / adj
 
     return [x, y, z]
 
-def project(objects, *args, **kwargs):
+def project(objects, by_distance=True, return_order=False, *args, **kwargs):
     """Project list of 3D objects onto 2D screen.
 
     Line width, mark sizes, and length in angle brackets are scaled according
-    to the distance from the observer. The objects are sorted by distance so
-    that close object overlay remote objects.
+    to the distance from the observer.
+
 
     Parameters
     ----------
     objects : list of tuple
         List of objects. Each object is represented by a tuple, which consists
         of a list of three-tuples ``(x, y, z)`` and a style dictionary.
+    by_distance : bool, default True
+        Sort the objects by distance so that close object overlay remote
+        objects?
+    return_order : bool, default False
+        Also return sorting order as list of indices?
 
     *args, **kwargs
         Arguments passed to `projection`.
 
     Returns
     -------
     list of tuple
         Objects is same format, but sorted with transformed coordinates and
         adjusted styles.
+    list of int, optional
+        Sorting order.
     """
     objects = [([projection(coordinate, *args, **kwargs)
         for coordinate in coordinates], style.copy())
         for coordinates, style in objects]
 
     zoom = [sum(coordinate[2]
         for coordinate in coordinates) / len(coordinates)
@@ -106,10 +113,15 @@
                 style[option] *= zoom[n]
 
         for option in style:
             if isinstance(style[option], str):
                 style[option] = re.sub('(?<=<)([\d.]+)(?=>)', lambda match:
                     '%.3f' % (float(match.group(1)) * zoom[n]), style[option])
 
-    order = sorted(range(len(zoom)), key=lambda n: zoom[n])
+    if by_distance:
+        order = sorted(range(len(zoom)), key=lambda n: zoom[n])
+        objects = [objects[n] for n in order]
+
+        if return_order:
+            return objects, order
 
-    return [objects[n] for n in order]
+    return objects
```

