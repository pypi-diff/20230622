# Comparing `tmp/html5svg2-0.1.2.tar.gz` & `tmp/html5svg2-0.1.4.tar.gz`

## Comparing `html5svg2-0.1.2.tar` & `html5svg2-0.1.4.tar`

### file list

```diff
@@ -1,40 +1,51 @@
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 html5svg2-0.1.2/.readthedocs.yaml
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 html5svg2-0.1.2/MANIFEST.in
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 html5svg2-0.1.2/mkdocs.yml
--rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 html5svg2-0.1.2/docs/1_intro.md
--rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 html5svg2-0.1.2/docs/2_html.md
--rw-r--r--   0        0        0     9647 2020-02-02 00:00:00.000000 html5svg2-0.1.2/docs/3_svg.md
--rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 html5svg2-0.1.2/docs/index.md
--rw-r--r--   0        0        0     8045 2020-02-02 00:00:00.000000 html5svg2-0.1.2/docs/imgs/circulo.svg
--rw-r--r--   0        0        0   127792 2020-02-02 00:00:00.000000 html5svg2-0.1.2/docs/imgs/demo00.png
--rw-r--r--   0        0        0     5193 2020-02-02 00:00:00.000000 html5svg2-0.1.2/docs/imgs/elipse.svg
--rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 html5svg2-0.1.2/docs/imgs/estructura_html.svg
--rw-r--r--   0        0        0     2442 2020-02-02 00:00:00.000000 html5svg2-0.1.2/docs/imgs/jirish-nazca.svg
--rw-r--r--   0        0        0     5222 2020-02-02 00:00:00.000000 html5svg2-0.1.2/docs/imgs/linea.svg
--rw-r--r--   0        0        0     4818 2020-02-02 00:00:00.000000 html5svg2-0.1.2/docs/imgs/poligono.svg
--rw-r--r--   0        0        0     4820 2020-02-02 00:00:00.000000 html5svg2-0.1.2/docs/imgs/polilinea.svg
--rw-r--r--   0        0        0     5531 2020-02-02 00:00:00.000000 html5svg2-0.1.2/docs/imgs/rectangulo.svg
--rw-r--r--   0        0        0    15790 2020-02-02 00:00:00.000000 html5svg2-0.1.2/docs/imgs/reporte.html.png
--rw-r--r--   0        0        0     2167 2020-02-02 00:00:00.000000 html5svg2-0.1.2/docs/imgs/sistema_coordenadas.svg
--rw-r--r--   0        0        0     6715 2020-02-02 00:00:00.000000 html5svg2-0.1.2/docs/imgs/texto.svg
--rw-r--r--   0        0        0     5163 2020-02-02 00:00:00.000000 html5svg2-0.1.2/docs/imgs/trayectoria.svg
--rw-r--r--   0        0        0    17477 2020-02-02 00:00:00.000000 html5svg2-0.1.2/docs/imgs/tw.html.png
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 html5svg2-0.1.2/ejemplos/circulo.py
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 html5svg2-0.1.2/ejemplos/elipse.py
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 html5svg2-0.1.2/ejemplos/estructura_html.py
--rw-r--r--   0        0        0    20459 2020-02-02 00:00:00.000000 html5svg2-0.1.2/ejemplos/jirish-nazca.json
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 html5svg2-0.1.2/ejemplos/jirish-nazca.py
--rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 html5svg2-0.1.2/ejemplos/linea.py
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 html5svg2-0.1.2/ejemplos/poligono.py
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 html5svg2-0.1.2/ejemplos/polilinea.py
--rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 html5svg2-0.1.2/ejemplos/rectangulo.py
--rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 html5svg2-0.1.2/ejemplos/sistema_coordenadas.py
--rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 html5svg2-0.1.2/ejemplos/texto.py
--rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 html5svg2-0.1.2/ejemplos/trayectoria.py
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 html5svg2-0.1.2/html5svg2/__init__.py
--rw-r--r--   0        0        0    10372 2020-02-02 00:00:00.000000 html5svg2-0.1.2/html5svg2/prg.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 html5svg2-0.1.2/.gitignore
--rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 html5svg2-0.1.2/LICENSE
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 html5svg2-0.1.2/README.md
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 html5svg2-0.1.2/pyproject.toml
--rw-r--r--   0        0        0    41315 2020-02-02 00:00:00.000000 html5svg2-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 html5svg2-0.1.4/.readthedocs.yaml
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 html5svg2-0.1.4/MANIFEST.in
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 html5svg2-0.1.4/mkdocs.yml
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 html5svg2-0.1.4/setup.py
+-rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 html5svg2-0.1.4/docs/1_intro.md
+-rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 html5svg2-0.1.4/docs/2_html.md
+-rw-r--r--   0        0        0    11719 2020-02-02 00:00:00.000000 html5svg2-0.1.4/docs/3_svg.md
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 html5svg2-0.1.4/docs/4_grf.md
+-rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 html5svg2-0.1.4/docs/index.md
+-rw-r--r--   0        0        0     5147 2020-02-02 00:00:00.000000 html5svg2-0.1.4/docs/imgs/arco.svg
+-rw-r--r--   0        0        0     8045 2020-02-02 00:00:00.000000 html5svg2-0.1.4/docs/imgs/circulo.svg
+-rw-r--r--   0        0        0   127792 2020-02-02 00:00:00.000000 html5svg2-0.1.4/docs/imgs/demo00.png
+-rw-r--r--   0        0        0     5193 2020-02-02 00:00:00.000000 html5svg2-0.1.4/docs/imgs/elipse.svg
+-rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 html5svg2-0.1.4/docs/imgs/estructura_html.svg
+-rw-r--r--   0        0        0     3774 2020-02-02 00:00:00.000000 html5svg2-0.1.4/docs/imgs/grf_xy_01.svg
+-rw-r--r--   0        0        0     2442 2020-02-02 00:00:00.000000 html5svg2-0.1.4/docs/imgs/jirish-nazca.svg
+-rw-r--r--   0        0        0     5222 2020-02-02 00:00:00.000000 html5svg2-0.1.4/docs/imgs/linea.svg
+-rw-r--r--   0        0        0     6030 2020-02-02 00:00:00.000000 html5svg2-0.1.4/docs/imgs/poligono-regular.svg
+-rw-r--r--   0        0        0     4818 2020-02-02 00:00:00.000000 html5svg2-0.1.4/docs/imgs/poligono.svg
+-rw-r--r--   0        0        0     4820 2020-02-02 00:00:00.000000 html5svg2-0.1.4/docs/imgs/polilinea.svg
+-rw-r--r--   0        0        0     5531 2020-02-02 00:00:00.000000 html5svg2-0.1.4/docs/imgs/rectangulo.svg
+-rw-r--r--   0        0        0    15790 2020-02-02 00:00:00.000000 html5svg2-0.1.4/docs/imgs/reporte.html.png
+-rw-r--r--   0        0        0     5502 2020-02-02 00:00:00.000000 html5svg2-0.1.4/docs/imgs/rotar.svg
+-rw-r--r--   0        0        0     2167 2020-02-02 00:00:00.000000 html5svg2-0.1.4/docs/imgs/sistema_coordenadas.svg
+-rw-r--r--   0        0        0     6715 2020-02-02 00:00:00.000000 html5svg2-0.1.4/docs/imgs/texto.svg
+-rw-r--r--   0        0        0     5163 2020-02-02 00:00:00.000000 html5svg2-0.1.4/docs/imgs/trayectoria.svg
+-rw-r--r--   0        0        0    17477 2020-02-02 00:00:00.000000 html5svg2-0.1.4/docs/imgs/tw.html.png
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 html5svg2-0.1.4/ejemplos/arco.py
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 html5svg2-0.1.4/ejemplos/circulo.py
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 html5svg2-0.1.4/ejemplos/elipse.py
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 html5svg2-0.1.4/ejemplos/estructura_html.py
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 html5svg2-0.1.4/ejemplos/grf_xy_01.py
+-rw-r--r--   0        0        0    20459 2020-02-02 00:00:00.000000 html5svg2-0.1.4/ejemplos/jirish-nazca.json
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 html5svg2-0.1.4/ejemplos/jirish-nazca.py
+-rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 html5svg2-0.1.4/ejemplos/linea.py
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 html5svg2-0.1.4/ejemplos/poligono-regular.py
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 html5svg2-0.1.4/ejemplos/poligono.py
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 html5svg2-0.1.4/ejemplos/polilinea.py
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 html5svg2-0.1.4/ejemplos/rectangulo.py
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 html5svg2-0.1.4/ejemplos/rotar.py
+-rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 html5svg2-0.1.4/ejemplos/sistema_coordenadas.py
+-rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 html5svg2-0.1.4/ejemplos/texto.py
+-rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 html5svg2-0.1.4/ejemplos/trayectoria.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 html5svg2-0.1.4/html5svg2/__init__.py
+-rw-r--r--   0        0        0    34395 2020-02-02 00:00:00.000000 html5svg2-0.1.4/html5svg2/prg.py
+-rw-r--r--   0        0        0     5752 2020-02-02 00:00:00.000000 html5svg2-0.1.4/html5svg2/utl.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 html5svg2-0.1.4/.gitignore
+-rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 html5svg2-0.1.4/LICENSE
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 html5svg2-0.1.4/README.md
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 html5svg2-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0    41315 2020-02-02 00:00:00.000000 html5svg2-0.1.4/PKG-INFO
```

### Comparing `html5svg2-0.1.2/docs/1_intro.md` & `html5svg2-0.1.4/docs/1_intro.md`

 * *Files identical despite different names*

### Comparing `html5svg2-0.1.2/docs/2_html.md` & `html5svg2-0.1.4/docs/2_html.md`

 * *Files identical despite different names*

### Comparing `html5svg2-0.1.2/docs/3_svg.md` & `html5svg2-0.1.4/docs/3_svg.md`

 * *Files 12% similar despite different names*

```diff
@@ -84,14 +84,46 @@
 svg.dibujar(poligono(pts_1, style="fill:none;stroke:blue;"))
 svg.dibujar(poligono(pts_2, style="fill:gold;stroke:blue;"))
 svg.gravar("poligono.svg")
 ```
 
 ![svg](imgs/poligono.svg)
 
+### Polígono regular
+```python
+poligono_regular(po, n, r, ang, **cv)
+# po = (x, y): punto central
+# n: número de lados
+# r: radio al vértice
+# ang: ángulo del vértice inicial
+```
+Ejemplo:
+```python
+from html5svg2 import SVG2, poligono_regular
+
+svg = SVG2('ajustable', W=330, H=130, letra="Consolas", color_fondo="rgb(250,250,230)")
+svg.cuadricula(10, style="stroke:SlateBlue;stroke-width:0.1px;")
+
+l_db = [
+	poligono_regular((80, 65), 5, 60, 18, style="fill:gold;stroke:crimson;"),
+	poligono_regular((80, 65), 4, 40, 45, style="fill:yellow;stroke:blue;"),
+	poligono_regular((80, 65), 3, 20, -30, style="fill:lime;stroke:green;"),
+	poligono_regular((250, 65), 10, 60, 18, style="fill:gold;stroke:crimson;"),
+	poligono_regular((250, 65), 8, 40, 45, style="fill:yellow;stroke:blue;"),
+	poligono_regular((250, 65), 6, 20, -30, style="fill:lime;stroke:green;"),
+]
+
+for db in l_db:
+	svg.dibujar(db)
+	
+svg.gravar("poligono-regular.svg")
+```
+
+![svg](imgs/poligono-regular.svg)
+
 ### Rectángulo
 ```python
 rectangulo(px, w, h, **jx)
 # px = (x,y) vértice inferior izquierdo del rectángulo
 # **js: argumentos clave:valor
 #	rx: radio de curvatura en vértices
 #	ry: radio de curvatura en vértices
@@ -249,14 +281,53 @@
 	
 svg.dibujar(trayectoria(ldx, style="fill:none;stroke:white;stroke-width:2px;"))
 
 svg.gravar("jirish-nazca.svg")
 ```
 ![svg](imgs/jirish-nazca.svg)
 
+
+### Arco
+
+```python
+arco_circular(po, r, angi, angf, **cv)
+arco_eliptico(po, rx, ry, angi, angf, **cv)
+# po = (x,y): punto central del círculo o elipse
+# r: radio del círculo
+# rx: radio de la elipse en el eje X
+# ry: radio de la elipse en el eje Y
+# angi: ángulo inicial (en grados)
+# angf: ángulo final (en grados)
+# **js: argumentos clave:valor
+```
+
+Ejemplo:
+```python
+from html5svg2 import SVG2, arco_circular, arco_eliptico
+
+svg = SVG2('ajustable', W=330, H=130, letra="Consolas", color_fondo="rgb(250,250,230)")
+svg.cuadricula(10, style="stroke:SlateBlue;stroke-width:0.1px;")
+st1 = "fill:none;stroke:blue;stroke-width:2px;"
+st2 = "fill:none;stroke:red;stroke-width:2px;"
+
+l_db = [
+	arco_circular((80, 65), 50, 00, 120, style=st1),
+	arco_circular((80, 65), 50, 120, 360, style=st2),
+	arco_eliptico((245, 65), 50, 30, 0, 290, style=st1),
+	arco_eliptico((245, 65), 50, 30, 290, 360, style=st2)
+]
+
+for db in l_db:
+	svg.dibujar(db)
+	
+svg.gravar("arco.svg")
+```
+
+![svg](imgs/arco.svg)
+
 ## Texto
 ```python
 texto(px, tx, **jx)
 # px = (x,y): punto de ubicación del texto
 # tx: texto a mostrar
 # **js: argumentos clave:valor
 #  ang: ángulo de rotación sobre el punto po y la horizontal (en grados)
@@ -297,8 +368,10 @@
 for db in l_db:
 	svg.dibujar(db)
 	
 svg.gravar("texto.svg")
 ```
 ![svg](imgs/texto.svg)
 
+## Rotar
 
+![svg](imgs/rotar.svg)
```

### Comparing `html5svg2-0.1.2/docs/index.md` & `html5svg2-0.1.4/docs/index.md`

 * *Files identical despite different names*

### Comparing `html5svg2-0.1.2/docs/imgs/circulo.svg` & `html5svg2-0.1.4/docs/imgs/circulo.svg`

 * *Files identical despite different names*

### Comparing `html5svg2-0.1.2/docs/imgs/demo00.png` & `html5svg2-0.1.4/docs/imgs/demo00.png`

 * *Files identical despite different names*

### Comparing `html5svg2-0.1.2/docs/imgs/elipse.svg` & `html5svg2-0.1.4/docs/imgs/elipse.svg`

 * *Files identical despite different names*

### Comparing `html5svg2-0.1.2/docs/imgs/estructura_html.svg` & `html5svg2-0.1.4/docs/imgs/estructura_html.svg`

 * *Files identical despite different names*

### Comparing `html5svg2-0.1.2/docs/imgs/jirish-nazca.svg` & `html5svg2-0.1.4/docs/imgs/jirish-nazca.svg`

 * *Files identical despite different names*

### Comparing `html5svg2-0.1.2/docs/imgs/linea.svg` & `html5svg2-0.1.4/docs/imgs/linea.svg`

 * *Files identical despite different names*

### Comparing `html5svg2-0.1.2/docs/imgs/poligono.svg` & `html5svg2-0.1.4/docs/imgs/poligono.svg`

 * *Files identical despite different names*

### Comparing `html5svg2-0.1.2/docs/imgs/polilinea.svg` & `html5svg2-0.1.4/docs/imgs/polilinea.svg`

 * *Files identical despite different names*

### Comparing `html5svg2-0.1.2/docs/imgs/rectangulo.svg` & `html5svg2-0.1.4/docs/imgs/rectangulo.svg`

 * *Files identical despite different names*

### Comparing `html5svg2-0.1.2/docs/imgs/reporte.html.png` & `html5svg2-0.1.4/docs/imgs/reporte.html.png`

 * *Files identical despite different names*

### Comparing `html5svg2-0.1.2/docs/imgs/sistema_coordenadas.svg` & `html5svg2-0.1.4/docs/imgs/sistema_coordenadas.svg`

 * *Files identical despite different names*

### Comparing `html5svg2-0.1.2/docs/imgs/texto.svg` & `html5svg2-0.1.4/docs/imgs/texto.svg`

 * *Files identical despite different names*

### Comparing `html5svg2-0.1.2/docs/imgs/trayectoria.svg` & `html5svg2-0.1.4/docs/imgs/trayectoria.svg`

 * *Files identical despite different names*

### Comparing `html5svg2-0.1.2/docs/imgs/tw.html.png` & `html5svg2-0.1.4/docs/imgs/tw.html.png`

 * *Files identical despite different names*

### Comparing `html5svg2-0.1.2/ejemplos/circulo.py` & `html5svg2-0.1.4/ejemplos/circulo.py`

 * *Files identical despite different names*

### Comparing `html5svg2-0.1.2/ejemplos/elipse.py` & `html5svg2-0.1.4/ejemplos/elipse.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import math
 from pathlib import Path
 
-from html5svg2 import SVG2, circulo, elipse
+from html5svg2 import SVG2, elipse
 
 svg = SVG2('ajustable', W=330, H=130, letra="Consolas", color_fondo="rgb(250,250,230)")
 svg.cuadricula(10, style="stroke:SlateBlue;stroke-width:0.1px;")
 
 stl1 = "stroke:blue;stroke-width:0.5;fill:gold;opacity:0.6;"
 stl2 = "stroke:red;stroke-width:1.5;fill:OrangeRed;opacity:0.3;"
 xo = 165
```

### Comparing `html5svg2-0.1.2/ejemplos/estructura_html.py` & `html5svg2-0.1.4/ejemplos/estructura_html.py`

 * *Files identical despite different names*

### Comparing `html5svg2-0.1.2/ejemplos/jirish-nazca.json` & `html5svg2-0.1.4/ejemplos/jirish-nazca.json`

 * *Files identical despite different names*

### Comparing `html5svg2-0.1.2/ejemplos/linea.py` & `html5svg2-0.1.4/ejemplos/linea.py`

 * *Files identical despite different names*

### Comparing `html5svg2-0.1.2/ejemplos/poligono.py` & `html5svg2-0.1.4/ejemplos/poligono.py`

 * *Files identical despite different names*

### Comparing `html5svg2-0.1.2/ejemplos/polilinea.py` & `html5svg2-0.1.4/ejemplos/polilinea.py`

 * *Files identical despite different names*

### Comparing `html5svg2-0.1.2/ejemplos/rectangulo.py` & `html5svg2-0.1.4/ejemplos/rectangulo.py`

 * *Files identical despite different names*

### Comparing `html5svg2-0.1.2/ejemplos/sistema_coordenadas.py` & `html5svg2-0.1.4/ejemplos/sistema_coordenadas.py`

 * *Files identical despite different names*

### Comparing `html5svg2-0.1.2/ejemplos/texto.py` & `html5svg2-0.1.4/ejemplos/texto.py`

 * *Files identical despite different names*

### Comparing `html5svg2-0.1.2/ejemplos/trayectoria.py` & `html5svg2-0.1.4/ejemplos/trayectoria.py`

 * *Files identical despite different names*

### Comparing `html5svg2-0.1.2/LICENSE` & `html5svg2-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `html5svg2-0.1.2/pyproject.toml` & `html5svg2-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "html5svg2"
-version = "0.1.2"
+version = "0.1.4"
 authors = [
     { name="Borsi Romero", borsifelix="xxx@gmail.com" },
 ]
 description = "Generador de reportes en formato HTML y SVG"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.3"
```

### Comparing `html5svg2-0.1.2/PKG-INFO` & `html5svg2-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: html5svg2
-Version: 0.1.2
+Version: 0.1.4
 Summary: Generador de reportes en formato HTML y SVG
 Project-URL: Homepage, https://github.com/borsifelix/html5svg2
 Project-URL: Bug Tracker, https://github.com/borsifelix/html5svg2/releases
 Author: Borsi Romero
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
```

