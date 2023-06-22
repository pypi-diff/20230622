# Comparing `tmp/PteraSoftware-2.2.1.tar.gz` & `tmp/PteraSoftware-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PteraSoftware-2.2.1.tar", last modified: Tue Jun 28 22:06:15 2022, max compression
+gzip compressed data, was "PteraSoftware-3.0.0.tar", last modified: Thu Jun 22 18:57:29 2023, max compression
```

## Comparing `PteraSoftware-2.2.1.tar` & `PteraSoftware-3.0.0.tar`

### file list

```diff
@@ -1,1582 +1,1593 @@
-drwxrwxrwx   0        0        0        0 2022-06-28 22:06:15.729263 PteraSoftware-2.2.1/
--rw-rw-rw-   0        0        0     1093 2022-06-27 17:48:47.000000 PteraSoftware-2.2.1/LICENSE.txt
--rw-rw-rw-   0        0        0      138 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/MANIFEST.in
--rw-rw-rw-   0        0        0    14765 2022-06-28 22:06:15.729263 PteraSoftware-2.2.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2022-06-28 22:06:09.628956 PteraSoftware-2.2.1/PteraSoftware.egg-info/
--rw-rw-rw-   0        0        0    14765 2022-06-28 22:06:09.000000 PteraSoftware-2.2.1/PteraSoftware.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    53557 2022-06-28 22:06:09.000000 PteraSoftware-2.2.1/PteraSoftware.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-06-28 22:06:09.000000 PteraSoftware-2.2.1/PteraSoftware.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      172 2022-06-28 22:06:09.000000 PteraSoftware-2.2.1/PteraSoftware.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2022-06-28 22:06:09.000000 PteraSoftware-2.2.1/PteraSoftware.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    13660 2022-06-28 21:56:29.000000 PteraSoftware-2.2.1/README.md
-drwxrwxrwx   0        0        0        0 2022-06-28 22:06:09.666817 PteraSoftware-2.2.1/pterasoftware/
--rw-rw-rw-   0        0        0     2469 2022-06-27 17:48:47.000000 PteraSoftware-2.2.1/pterasoftware/__init__.py
--rw-rw-rw-   0        0        0    42174 2022-05-16 20:47:35.000000 PteraSoftware-2.2.1/pterasoftware/aerodynamics.py
-drwxrwxrwx   0        0        0        0 2022-06-28 22:06:15.729263 PteraSoftware-2.2.1/pterasoftware/airfoils/
--rw-rw-rw-   0        0        0      685 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/2032c.dat
--rw-rw-rw-   0        0        0      104 2022-06-27 17:48:47.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/__init__.py
--rw-rw-rw-   0        0        0      918 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/a18.dat
--rw-rw-rw-   0        0        0     2228 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/a18sm.dat
--rw-rw-rw-   0        0        0     1285 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/a63a108c.dat
--rw-rw-rw-   0        0        0     4885 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ag03.dat
--rw-rw-rw-   0        0        0     4866 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ag04.dat
--rw-rw-rw-   0        0        0     4866 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ag08.dat
--rw-rw-rw-   0        0        0     4866 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ag09.dat
--rw-rw-rw-   0        0        0     4866 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ag10.dat
--rw-rw-rw-   0        0        0     4947 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ag11.dat
--rw-rw-rw-   0        0        0     4326 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ag12.dat
--rw-rw-rw-   0        0        0     4326 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ag13.dat
--rw-rw-rw-   0        0        0     4326 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ag14.dat
--rw-rw-rw-   0        0        0     4326 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ag16.dat
--rw-rw-rw-   0        0        0     3686 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ag17.dat
--rw-rw-rw-   0        0        0     3686 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ag18.dat
--rw-rw-rw-   0        0        0     4326 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ag19.dat
--rw-rw-rw-   0        0        0     4470 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ag24.dat
--rw-rw-rw-   0        0        0     4470 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ag25.dat
--rw-rw-rw-   0        0        0     4470 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ag26.dat
--rw-rw-rw-   0        0        0     4472 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ag27.dat
--rw-rw-rw-   0        0        0     4866 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ag35.dat
--rw-rw-rw-   0        0        0     4866 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ag36.dat
--rw-rw-rw-   0        0        0     4866 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ag37.dat
--rw-rw-rw-   0        0        0     4866 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ag38.dat
--rw-rw-rw-   0        0        0     4603 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ag44ct02r.dat
--rw-rw-rw-   0        0        0     4609 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ag455ct02r.dat
--rw-rw-rw-   0        0        0     4575 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ag45c03.dat
--rw-rw-rw-   0        0        0     4603 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ag45ct02r.dat
--rw-rw-rw-   0        0        0     4656 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ag46c03.dat
--rw-rw-rw-   0        0        0     4636 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ag46ct02r.dat
--rw-rw-rw-   0        0        0     4575 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ag47c03.dat
--rw-rw-rw-   0        0        0     4636 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ag47ct02r.dat
--rw-rw-rw-   0        0        0     1436 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ah21-7.dat
--rw-rw-rw-   0        0        0     1375 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ah21-9.dat
--rw-rw-rw-   0        0        0     2089 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ah63k127.dat
--rw-rw-rw-   0        0        0      670 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ah6407.dat
--rw-rw-rw-   0        0        0      670 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ah7476.dat
--rw-rw-rw-   0        0        0     2058 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ah79100a.dat
--rw-rw-rw-   0        0        0     2058 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ah79100b.dat
--rw-rw-rw-   0        0        0     2058 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ah79100c.dat
--rw-rw-rw-   0        0        0     2095 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ah79k132.dat
--rw-rw-rw-   0        0        0     2098 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ah79k135.dat
--rw-rw-rw-   0        0        0     2096 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ah79k143.dat
--rw-rw-rw-   0        0        0     2095 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ah80129.dat
--rw-rw-rw-   0        0        0     2096 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ah80136.dat
--rw-rw-rw-   0        0        0     2095 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ah80140.dat
--rw-rw-rw-   0        0        0     2101 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ah81131.dat
--rw-rw-rw-   0        0        0     2097 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ah81k144.dat
--rw-rw-rw-   0        0        0     2108 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ah81k144wfKlappe.dat
--rw-rw-rw-   0        0        0     2087 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ah82150a.dat
--rw-rw-rw-   0        0        0     2091 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ah82150f.dat
--rw-rw-rw-   0        0        0     2088 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ah83150q.dat
--rw-rw-rw-   0        0        0     2085 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ah83159.dat
--rw-rw-rw-   0        0        0     2100 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ah85l120.dat
--rw-rw-rw-   0        0        0     2088 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ah88k130.dat
--rw-rw-rw-   0        0        0     2296 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ah88k136.dat
--rw-rw-rw-   0        0        0     2291 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ah93156.dat
--rw-rw-rw-   0        0        0     2291 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ah93157.dat
--rw-rw-rw-   0        0        0     2296 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ah93k130.dat
--rw-rw-rw-   0        0        0     2296 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ah93k131.dat
--rw-rw-rw-   0        0        0     2296 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ah93k132.dat
--rw-rw-rw-   0        0        0     2098 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ah93w145.dat
--rw-rw-rw-   0        0        0     2087 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ah93w174.dat
--rw-rw-rw-   0        0        0     2100 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ah93w215.dat
--rw-rw-rw-   0        0        0     2098 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ah93w257.dat
--rw-rw-rw-   0        0        0     2098 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ah93w300.dat
--rw-rw-rw-   0        0        0     2161 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ah93w480b.dat
--rw-rw-rw-   0        0        0     2291 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ah94145.dat
--rw-rw-rw-   0        0        0     2291 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ah94156.dat
--rw-rw-rw-   0        0        0     2098 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ah94w301.dat
--rw-rw-rw-   0        0        0     2291 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ah95160.dat
--rw-rw-rw-   0        0        0     1240 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ames01.dat
--rw-rw-rw-   0        0        0     1756 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ames02.dat
--rw-rw-rw-   0        0        0     1758 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ames03.dat
--rw-rw-rw-   0        0        0     1189 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/amsoil1.dat
--rw-rw-rw-   0        0        0     1187 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/amsoil2.dat
--rw-rw-rw-   0        0        0      990 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/apex16.dat
--rw-rw-rw-   0        0        0     1461 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/aquilasm.dat
--rw-rw-rw-   0        0        0      864 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/arad10.dat
--rw-rw-rw-   0        0        0      864 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/arad13.dat
--rw-rw-rw-   0        0        0      864 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/arad20.dat
--rw-rw-rw-   0        0        0      847 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/arad6.dat
--rw-rw-rw-   0        0        0     1321 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/as5045.dat
--rw-rw-rw-   0        0        0     1427 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/as5046.dat
--rw-rw-rw-   0        0        0     1368 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/as5048.dat
--rw-rw-rw-   0        0        0     1676 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/atr72sm.dat
--rw-rw-rw-   0        0        0     2096 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/august160.dat
--rw-rw-rw-   0        0        0     2066 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/avistar.dat
--rw-rw-rw-   0        0        0      838 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/b29root.dat
--rw-rw-rw-   0        0        0      837 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/b29tip.dat
--rw-rw-rw-   0        0        0     1506 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/b540ols.dat
--rw-rw-rw-   0        0        0     2570 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/b707a.dat
--rw-rw-rw-   0        0        0      632 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/b707b.dat
--rw-rw-rw-   0        0        0      539 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/b707c.dat
--rw-rw-rw-   0        0        0      601 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/b707d.dat
--rw-rw-rw-   0        0        0     2570 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/b707e.dat
--rw-rw-rw-   0        0        0      901 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/b737a.dat
--rw-rw-rw-   0        0        0      904 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/b737b.dat
--rw-rw-rw-   0        0        0      905 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/b737c.dat
--rw-rw-rw-   0        0        0      906 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/b737d.dat
--rw-rw-rw-   0        0        0     1960 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/bacj.dat
--rw-rw-rw-   0        0        0      939 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/bacxxx.dat
--rw-rw-rw-   0        0        0      638 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/bambino6.dat
--rw-rw-rw-   0        0        0      963 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/be50.dat
--rw-rw-rw-   0        0        0     2229 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/be50sm.dat
--rw-rw-rw-   0        0        0      734 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/boe103.dat
--rw-rw-rw-   0        0        0      713 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/boe106.dat
--rw-rw-rw-   0        0        0     1903 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/bqm34.dat
--rw-rw-rw-   0        0        0     2000 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/bw3.dat
--rw-rw-rw-   0        0        0     1394 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/c141a.dat
--rw-rw-rw-   0        0        0     1398 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/c141b.dat
--rw-rw-rw-   0        0        0     1399 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/c141c.dat
--rw-rw-rw-   0        0        0     1399 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/c141d.dat
--rw-rw-rw-   0        0        0     1399 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/c141e.dat
--rw-rw-rw-   0        0        0     1399 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/c141f.dat
--rw-rw-rw-   0        0        0     1309 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/c5a.dat
--rw-rw-rw-   0        0        0     1313 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/c5b.dat
--rw-rw-rw-   0        0        0     1311 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/c5c.dat
--rw-rw-rw-   0        0        0     1313 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/c5d.dat
--rw-rw-rw-   0        0        0     1312 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/c5e.dat
--rw-rw-rw-   0        0        0      794 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/cap21c.dat
--rw-rw-rw-   0        0        0     1211 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/cast102.dat
--rw-rw-rw-   0        0        0     2229 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ch10sm.dat
--rw-rw-rw-   0        0        0     2073 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/chen.dat
--rw-rw-rw-   0        0        0      584 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/clarkk.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/clarkv.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/clarkw.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/clarkx.dat
--rw-rw-rw-   0        0        0     2559 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/clarky.dat
--rw-rw-rw-   0        0        0      608 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/clarkyh.dat
--rw-rw-rw-   0        0        0      711 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/clarkys.dat
--rw-rw-rw-   0        0        0     1468 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/clarkysm.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/clarkz.dat
--rw-rw-rw-   0        0        0      714 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/clarym15.dat
--rw-rw-rw-   0        0        0      714 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/clarym18.dat
--rw-rw-rw-   0        0        0      637 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/coanda1.dat
--rw-rw-rw-   0        0        0      637 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/coanda2.dat
--rw-rw-rw-   0        0        0      637 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/coanda3.dat
--rw-rw-rw-   0        0        0      648 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/cootie.dat
--rw-rw-rw-   0        0        0     1909 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/cr001sm.dat
--rw-rw-rw-   0        0        0     2623 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/cr1.dat
--rw-rw-rw-   0        0        0      640 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/curtisc72.dat
--rw-rw-rw-   0        0        0     1717 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/dae11.dat
--rw-rw-rw-   0        0        0     1696 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/dae21.dat
--rw-rw-rw-   0        0        0     1738 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/dae31.dat
--rw-rw-rw-   0        0        0     1696 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/dae51.dat
--rw-rw-rw-   0        0        0      708 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/davis.dat
--rw-rw-rw-   0        0        0     1942 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/davis_corrected.dat
--rw-rw-rw-   0        0        0     1909 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/davissm.dat
--rw-rw-rw-   0        0        0      644 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/daytonwright6.dat
--rw-rw-rw-   0        0        0      646 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/daytonwrightt1.dat
--rw-rw-rw-   0        0        0      703 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/dbln526.dat
--rw-rw-rw-   0        0        0     1688 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/defcnd1.dat
--rw-rw-rw-   0        0        0     1689 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/defcnd2.dat
--rw-rw-rw-   0        0        0     1690 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/defcnd3.dat
--rw-rw-rw-   0        0        0     1318 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/df101.dat
--rw-rw-rw-   0        0        0     1240 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/df102.dat
--rw-rw-rw-   0        0        0     2927 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/dfvlrr4.dat
--rw-rw-rw-   0        0        0      640 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/dga1138.dat
--rw-rw-rw-   0        0        0      655 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/dga1182.dat
--rw-rw-rw-   0        0        0     1910 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/dh4009sm.dat
--rw-rw-rw-   0        0        0     2058 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/doa5.dat
--rw-rw-rw-   0        0        0      635 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/dormoy.dat
--rw-rw-rw-   0        0        0     2958 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/drgnfly.dat
--rw-rw-rw-   0        0        0     2318 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/dsma523a.dat
--rw-rw-rw-   0        0        0     2321 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/dsma523b.dat
--rw-rw-rw-   0        0        0     2042 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/du8608418.dat
--rw-rw-rw-   0        0        0      862 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/du861372.dat
--rw-rw-rw-   0        0        0     1324 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e1098.dat
--rw-rw-rw-   0        0        0     1323 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e1200.dat
--rw-rw-rw-   0        0        0     1302 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e1210.dat
--rw-rw-rw-   0        0        0     1281 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e1211.dat
--rw-rw-rw-   0        0        0      985 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e1212.dat
--rw-rw-rw-   0        0        0     1139 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e1212mod.dat
--rw-rw-rw-   0        0        0     1281 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e1213.dat
--rw-rw-rw-   0        0        0     1302 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e1214.dat
--rw-rw-rw-   0        0        0     1494 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e1230.dat
--rw-rw-rw-   0        0        0     2059 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e1233.dat
--rw-rw-rw-   0        0        0     1313 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e168.dat
--rw-rw-rw-   0        0        0     1313 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e169.dat
--rw-rw-rw-   0        0        0     1313 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e171.dat
--rw-rw-rw-   0        0        0     1318 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e174.dat
--rw-rw-rw-   0        0        0     1313 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e176.dat
--rw-rw-rw-   0        0        0     1297 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e178.dat
--rw-rw-rw-   0        0        0     1312 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e180.dat
--rw-rw-rw-   0        0        0     1296 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e182.dat
--rw-rw-rw-   0        0        0     1312 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e184.dat
--rw-rw-rw-   0        0        0     1312 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e186.dat
--rw-rw-rw-   0        0        0     1312 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e193.dat
--rw-rw-rw-   0        0        0     1312 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e195.dat
--rw-rw-rw-   0        0        0     1312 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e197.dat
--rw-rw-rw-   0        0        0     1312 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e201.dat
--rw-rw-rw-   0        0        0     1312 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e203.dat
--rw-rw-rw-   0        0        0     1312 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e205.dat
--rw-rw-rw-   0        0        0     1312 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e207.dat
--rw-rw-rw-   0        0        0     1312 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e209.dat
--rw-rw-rw-   0        0        0     1312 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e210.dat
--rw-rw-rw-   0        0        0     1312 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e211.dat
--rw-rw-rw-   0        0        0     1312 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e212.dat
--rw-rw-rw-   0        0        0     1312 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e214.dat
--rw-rw-rw-   0        0        0     1312 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e216.dat
--rw-rw-rw-   0        0        0     1312 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e220.dat
--rw-rw-rw-   0        0        0     1312 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e221.dat
--rw-rw-rw-   0        0        0     1312 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e222.dat
--rw-rw-rw-   0        0        0     1312 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e224.dat
--rw-rw-rw-   0        0        0     1312 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e226.dat
--rw-rw-rw-   0        0        0     1313 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e228.dat
--rw-rw-rw-   0        0        0     1312 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e230.dat
--rw-rw-rw-   0        0        0      977 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e231.dat
--rw-rw-rw-   0        0        0     1301 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e266.dat
--rw-rw-rw-   0        0        0     1490 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e297.dat
--rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e325.dat
--rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e326.dat
--rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e327.dat
--rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e328.dat
--rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e329.dat
--rw-rw-rw-   0        0        0     1511 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e330.dat
--rw-rw-rw-   0        0        0     1511 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e331.dat
--rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e332.dat
--rw-rw-rw-   0        0        0     1511 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e333.dat
--rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e334.dat
--rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e335.dat
--rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e336.dat
--rw-rw-rw-   0        0        0     1553 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e337.dat
--rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e338.dat
--rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e339.dat
--rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e340.dat
--rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e341.dat
--rw-rw-rw-   0        0        0     1511 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e342.dat
--rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e343.dat
--rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e344.dat
--rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e360.dat
--rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e361.dat
--rw-rw-rw-   0        0        0     1285 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e374.dat
--rw-rw-rw-   0        0        0     1302 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e376.dat
--rw-rw-rw-   0        0        0     1302 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e377.dat
--rw-rw-rw-   0        0        0     1418 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e377m.dat
--rw-rw-rw-   0        0        0     1302 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e378.dat
--rw-rw-rw-   0        0        0     1302 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e379.dat
--rw-rw-rw-   0        0        0     1312 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e385.dat
--rw-rw-rw-   0        0        0     1287 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e387.dat
--rw-rw-rw-   0        0        0     1312 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e392.dat
--rw-rw-rw-   0        0        0     1322 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e393.dat
--rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e395.dat
--rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e396.dat
--rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e397.dat
--rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e398.dat
--rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e399.dat
--rw-rw-rw-   0        0        0     1301 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e403.dat
--rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e407.dat
--rw-rw-rw-   0        0        0     1301 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e417.dat
--rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e420.dat
--rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e421.dat
--rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e422.dat
--rw-rw-rw-   0        0        0     1447 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e423.dat
--rw-rw-rw-   0        0        0      860 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e426.dat
--rw-rw-rw-   0        0        0      860 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e428.dat
--rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e431.dat
--rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e432.dat
--rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e433.dat
--rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e434.dat
--rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e435.dat
--rw-rw-rw-   0        0        0     1312 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e471.dat
--rw-rw-rw-   0        0        0     1301 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e472.dat
--rw-rw-rw-   0        0        0     1301 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e473.dat
--rw-rw-rw-   0        0        0     1312 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e474.dat
--rw-rw-rw-   0        0        0     1312 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e475.dat
--rw-rw-rw-   0        0        0     1284 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e476.dat
--rw-rw-rw-   0        0        0     1284 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e477.dat
--rw-rw-rw-   0        0        0     1284 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e478.dat
--rw-rw-rw-   0        0        0     1301 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e479.dat
--rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e485.dat
--rw-rw-rw-   0        0        0      523 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e49.dat
--rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e502.dat
--rw-rw-rw-   0        0        0     1490 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e520.dat
--rw-rw-rw-   0        0        0     1490 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e521.dat
--rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e540.dat
--rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e541.dat
--rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e542.dat
--rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e543.dat
--rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e544.dat
--rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e545.dat
--rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e546.dat
--rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e547.dat
--rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e548.dat
--rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e549.dat
--rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e550.dat
--rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e551.dat
--rw-rw-rw-   0        0        0     1511 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e552.dat
--rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e553.dat
--rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e554.dat
--rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e555.dat
--rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e556.dat
--rw-rw-rw-   0        0        0     1511 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e557.dat
--rw-rw-rw-   0        0        0     1301 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e558.dat
--rw-rw-rw-   0        0        0     1301 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e559.dat
--rw-rw-rw-   0        0        0     1301 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e560.dat
--rw-rw-rw-   0        0        0     1301 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e561.dat
--rw-rw-rw-   0        0        0     1301 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e562.dat
--rw-rw-rw-   0        0        0      754 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e58.dat
--rw-rw-rw-   0        0        0     1301 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e580.dat
--rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e582.dat
--rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e583.dat
--rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e584.dat
--rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e585.dat
--rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e587.dat
--rw-rw-rw-   0        0        0      754 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e59.dat
--rw-rw-rw-   0        0        0      936 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e591.dat
--rw-rw-rw-   0        0        0     1511 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e593.dat
--rw-rw-rw-   0        0        0     1511 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e598.dat
--rw-rw-rw-   0        0        0     1301 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e603.dat
--rw-rw-rw-   0        0        0     1490 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e604.dat
--rw-rw-rw-   0        0        0     1312 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e61.dat
--rw-rw-rw-   0        0        0     1312 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e62.dat
--rw-rw-rw-   0        0        0     2099 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e625.dat
--rw-rw-rw-   0        0        0     1312 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e63.dat
--rw-rw-rw-   0        0        0     1301 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e635.dat
--rw-rw-rw-   0        0        0     1301 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e636.dat
--rw-rw-rw-   0        0        0     1301 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e637.dat
--rw-rw-rw-   0        0        0     1301 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e638.dat
--rw-rw-rw-   0        0        0     1301 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e639.dat
--rw-rw-rw-   0        0        0     1312 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e64.dat
--rw-rw-rw-   0        0        0     1301 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e642.dat
--rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e654.dat
--rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e655.dat
--rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e656.dat
--rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e657.dat
--rw-rw-rw-   0        0        0     1300 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e66.dat
--rw-rw-rw-   0        0        0      980 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e662.dat
--rw-rw-rw-   0        0        0     1302 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e664.dat
--rw-rw-rw-   0        0        0     1364 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e664ex.dat
--rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e668.dat
--rw-rw-rw-   0        0        0     1321 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e67.dat
--rw-rw-rw-   0        0        0     1301 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e678.dat
--rw-rw-rw-   0        0        0     1321 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e68.dat
--rw-rw-rw-   0        0        0     1301 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e682.dat
--rw-rw-rw-   0        0        0     1301 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e694.dat
--rw-rw-rw-   0        0        0     1312 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e71.dat
--rw-rw-rw-   0        0        0     1427 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e715.dat
--rw-rw-rw-   0        0        0     1302 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e748.dat
--rw-rw-rw-   0        0        0     1301 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e793.dat
--rw-rw-rw-   0        0        0     1458 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e817.dat
--rw-rw-rw-   0        0        0     1437 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e818.dat
--rw-rw-rw-   0        0        0     1312 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e836.dat
--rw-rw-rw-   0        0        0     1312 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e837.dat
--rw-rw-rw-   0        0        0     1312 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e838.dat
--rw-rw-rw-   0        0        0     1543 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e850.dat
--rw-rw-rw-   0        0        0     1428 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e851.dat
--rw-rw-rw-   0        0        0     1428 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e852.dat
--rw-rw-rw-   0        0        0     1407 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e853.dat
--rw-rw-rw-   0        0        0     1428 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e854.dat
--rw-rw-rw-   0        0        0     1406 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e855.dat
--rw-rw-rw-   0        0        0     1427 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e856.dat
--rw-rw-rw-   0        0        0     1406 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e857.dat
--rw-rw-rw-   0        0        0     1427 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e858.dat
--rw-rw-rw-   0        0        0     1307 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e862.dat
--rw-rw-rw-   0        0        0     1307 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e863.dat
--rw-rw-rw-   0        0        0     1307 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e864.dat
--rw-rw-rw-   0        0        0     2550 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e874.dat
--rw-rw-rw-   0        0        0     2309 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e904.dat
--rw-rw-rw-   0        0        0     2309 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/e908.dat
--rw-rw-rw-   0        0        0      596 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ea61009.dat
--rw-rw-rw-   0        0        0      596 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ea61012.dat
--rw-rw-rw-   0        0        0      596 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ea81006.dat
--rw-rw-rw-   0        0        0      639 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ebambino7.dat
--rw-rw-rw-   0        0        0      681 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ec863914.dat
--rw-rw-rw-   0        0        0     2012 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/eh0009.dat
--rw-rw-rw-   0        0        0     1778 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/eh1070.dat
--rw-rw-rw-   0        0        0     2289 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/eh1090.dat
--rw-rw-rw-   0        0        0     2289 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/eh1590.dat
--rw-rw-rw-   0        0        0     2329 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/eh2010.dat
--rw-rw-rw-   0        0        0     2234 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/eh2012.dat
--rw-rw-rw-   0        0        0     1779 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/eh2070.dat
--rw-rw-rw-   0        0        0     1991 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/eh2510.dat
--rw-rw-rw-   0        0        0     2031 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/eh3012.dat
--rw-rw-rw-   0        0        0      626 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/eiffel10.dat
--rw-rw-rw-   0        0        0      647 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/eiffel371.dat
--rw-rw-rw-   0        0        0      649 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/eiffel385.dat
--rw-rw-rw-   0        0        0      649 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/eiffel428.dat
--rw-rw-rw-   0        0        0      652 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/eiffel430.dat
--rw-rw-rw-   0        0        0     2064 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/esa40.dat
--rw-rw-rw-   0        0        0     1587 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/falcon.dat
--rw-rw-rw-   0        0        0      755 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fauvel.dat
--rw-rw-rw-   0        0        0      645 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fg1.dat
--rw-rw-rw-   0        0        0      645 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fg2.dat
--rw-rw-rw-   0        0        0      645 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fg3.dat
--rw-rw-rw-   0        0        0      645 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fg4.dat
--rw-rw-rw-   0        0        0      515 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx049915.dat
--rw-rw-rw-   0        0        0     1057 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx05188.dat
--rw-rw-rw-   0        0        0     1057 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx05191.dat
--rw-rw-rw-   0        0        0      505 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx057816.dat
--rw-rw-rw-   0        0        0     1059 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx05h126.dat
--rw-rw-rw-   0        0        0      510 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx082512.dat
--rw-rw-rw-   0        0        0     1059 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx08s176.dat
--rw-rw-rw-   0        0        0     1010 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx2.dat
--rw-rw-rw-   0        0        0     1010 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx3.dat
--rw-rw-rw-   0        0        0     2056 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx38153.dat
--rw-rw-rw-   0        0        0     2056 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx60100.dat
--rw-rw-rw-   0        0        0      760 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx601001.dat
--rw-rw-rw-   0        0        0     1469 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx60100sm.dat
--rw-rw-rw-   0        0        0     2065 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx60126.dat
--rw-rw-rw-   0        0        0     2058 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx601261.dat
--rw-rw-rw-   0        0        0     2056 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx60157.dat
--rw-rw-rw-   0        0        0      796 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx60160.dat
--rw-rw-rw-   0        0        0     2056 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx60177.dat
--rw-rw-rw-   0        0        0     2056 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx61140.dat
--rw-rw-rw-   0        0        0     2056 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx61147.dat
--rw-rw-rw-   0        0        0     2056 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx61163.dat
--rw-rw-rw-   0        0        0     2056 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx61168.dat
--rw-rw-rw-   0        0        0     2056 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx61184.dat
--rw-rw-rw-   0        0        0     1710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx62k131.dat
--rw-rw-rw-   0        0        0     2061 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx62k153.dat
--rw-rw-rw-   0        0        0      712 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx63100.dat
--rw-rw-rw-   0        0        0      712 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx63110.dat
--rw-rw-rw-   0        0        0      754 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx63120.dat
--rw-rw-rw-   0        0        0     1894 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx63137.dat
--rw-rw-rw-   0        0        0     1407 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx63137sm.dat
--rw-rw-rw-   0        0        0     2056 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx63143.dat
--rw-rw-rw-   0        0        0     2056 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx63145.dat
--rw-rw-rw-   0        0        0     2056 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx63147.dat
--rw-rw-rw-   0        0        0     2056 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx63158.dat
--rw-rw-rw-   0        0        0     1852 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx6617a2.dat
--rw-rw-rw-   0        0        0     1339 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx6617ai.dat
--rw-rw-rw-   0        0        0     1846 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx66182.dat
--rw-rw-rw-   0        0        0     1851 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx66196v.dat
--rw-rw-rw-   0        0        0     1718 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx66a175.dat
--rw-rw-rw-   0        0        0     2096 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx66h60.dat
--rw-rw-rw-   0        0        0     2099 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx66h80.dat
--rw-rw-rw-   0        0        0     1848 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx66s161.dat
--rw-rw-rw-   0        0        0     1848 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx66s171.dat
--rw-rw-rw-   0        0        0     1848 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx66s196.dat
--rw-rw-rw-   0        0        0     1851 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx67k150.dat
--rw-rw-rw-   0        0        0     1851 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx67k170.dat
--rw-rw-rw-   0        0        0     2097 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx68h120.dat
--rw-rw-rw-   0        0        0     2095 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx69274.dat
--rw-rw-rw-   0        0        0      929 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx69h083.dat
--rw-rw-rw-   0        0        0      815 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx69h098.dat
--rw-rw-rw-   0        0        0     2084 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx69pr281.dat
--rw-rw-rw-   0        0        0     1814 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx71089a.dat
--rw-rw-rw-   0        0        0     1813 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx71120.dat
--rw-rw-rw-   0        0        0     1851 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx711520.dat
--rw-rw-rw-   0        0        0     1851 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx711525.dat
--rw-rw-rw-   0        0        0     1719 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx711530.dat
--rw-rw-rw-   0        0        0     1303 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx71l150.dat
--rw-rw-rw-   0        0        0     1859 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx72150a.dat
--rw-rw-rw-   0        0        0     1859 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx72150b.dat
--rw-rw-rw-   0        0        0     2070 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx72ls160.dat
--rw-rw-rw-   0        0        0     2082 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx73170.dat
--rw-rw-rw-   0        0        0     2090 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx73170a.dat
--rw-rw-rw-   0        0        0     2076 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx73cl1152.dat
--rw-rw-rw-   0        0        0     2072 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx73cl2152.dat
--rw-rw-rw-   0        0        0     2071 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx73cl3152.dat
--rw-rw-rw-   0        0        0     2087 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx73k170.dat
--rw-rw-rw-   0        0        0     2066 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx74080.dat
--rw-rw-rw-   0        0        0     2088 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx74130wp1.dat
--rw-rw-rw-   0        0        0     2086 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx74130wp2.dat
--rw-rw-rw-   0        0        0     2090 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx74130wp2mod.dat
--rw-rw-rw-   0        0        0     1665 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx74cl5140.dat
--rw-rw-rw-   0        0        0     2070 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx74cl6140.dat
--rw-rw-rw-   0        0        0     2243 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx74modsm.dat
--rw-rw-rw-   0        0        0     2080 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx75141.dat
--rw-rw-rw-   0        0        0     2083 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx75193.dat
--rw-rw-rw-   0        0        0     2097 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx75vg166.dat
--rw-rw-rw-   0        0        0     2095 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx76100.dat
--rw-rw-rw-   0        0        0     2095 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx76120.dat
--rw-rw-rw-   0        0        0     2065 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx76mp120.dat
--rw-rw-rw-   0        0        0     2071 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx76mp140.dat
--rw-rw-rw-   0        0        0     2080 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx76mp160.dat
--rw-rw-rw-   0        0        0     2095 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx77080.dat
--rw-rw-rw-   0        0        0     2097 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx77w121.dat
--rw-rw-rw-   0        0        0     2025 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx77w153.dat
--rw-rw-rw-   0        0        0     2025 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx77w258.dat
--rw-rw-rw-   0        0        0     2098 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx77w270.dat
--rw-rw-rw-   0        0        0     2099 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx77w270s.dat
--rw-rw-rw-   0        0        0     2025 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx77w343.dat
--rw-rw-rw-   0        0        0     2100 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx78k140.dat
--rw-rw-rw-   0        0        0     2098 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx78k140a20.dat
--rw-rw-rw-   0        0        0     2100 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx78k150.dat
--rw-rw-rw-   0        0        0     2097 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx78k161.dat
--rw-rw-rw-   0        0        0     2101 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx78pk188.dat
--rw-rw-rw-   0        0        0     1917 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx79k144.dat
--rw-rw-rw-   0        0        0     2097 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx79l100.dat
--rw-rw-rw-   0        0        0     2097 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx79l120.dat
--rw-rw-rw-   0        0        0     2099 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx79w151a.dat
--rw-rw-rw-   0        0        0     2100 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx79w470a.dat
--rw-rw-rw-   0        0        0     2099 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx79w660a.dat
--rw-rw-rw-   0        0        0     2083 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx80080.dat
--rw-rw-rw-   0        0        0     2078 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx83w108.dat
--rw-rw-rw-   0        0        0     2085 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx83w160.dat
--rw-rw-rw-   0        0        0     2097 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx83w227.dat
--rw-rw-rw-   0        0        0     2091 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx84w097.dat
--rw-rw-rw-   0        0        0     2088 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx84w127.dat
--rw-rw-rw-   0        0        0     2088 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx84w140.dat
--rw-rw-rw-   0        0        0     2088 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx84w150.dat
--rw-rw-rw-   0        0        0     2089 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx84w175.dat
--rw-rw-rw-   0        0        0     2093 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fx84w218.dat
--rw-rw-rw-   0        0        0     2063 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fxl142k.dat
--rw-rw-rw-   0        0        0     1919 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fxlv152.dat
--rw-rw-rw-   0        0        0     1877 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fxm2.dat
--rw-rw-rw-   0        0        0     2058 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fxs02196.dat
--rw-rw-rw-   0        0        0     2058 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fxs03182.dat
--rw-rw-rw-   0        0        0     2060 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/fxs21158.dat
--rw-rw-rw-   0        0        0     2231 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/geminism.dat
--rw-rw-rw-   0        0        0     1090 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/giiia.dat
--rw-rw-rw-   0        0        0     1091 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/giiib.dat
--rw-rw-rw-   0        0        0     1091 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/giiic.dat
--rw-rw-rw-   0        0        0     1091 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/giiid.dat
--rw-rw-rw-   0        0        0     1092 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/giiie.dat
--rw-rw-rw-   0        0        0     1092 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/giiif.dat
--rw-rw-rw-   0        0        0     1092 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/giiig.dat
--rw-rw-rw-   0        0        0     1092 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/giiih.dat
--rw-rw-rw-   0        0        0     1092 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/giiii.dat
--rw-rw-rw-   0        0        0     1092 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/giiij.dat
--rw-rw-rw-   0        0        0     1092 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/giiik.dat
--rw-rw-rw-   0        0        0     1092 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/giiil.dat
--rw-rw-rw-   0        0        0     1092 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/giiim.dat
--rw-rw-rw-   0        0        0     1092 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/giiin.dat
--rw-rw-rw-   0        0        0      644 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/glennmartin2.dat
--rw-rw-rw-   0        0        0      643 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/glennmartin3.dat
--rw-rw-rw-   0        0        0      645 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/glennmartin4.dat
--rw-rw-rw-   0        0        0     2229 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/gm15sm.dat
--rw-rw-rw-   0        0        0      667 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe05k.dat
--rw-rw-rw-   0        0        0      667 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe06k.dat
--rw-rw-rw-   0        0        0      667 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe07k.dat
--rw-rw-rw-   0        0        0      667 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe08k.dat
--rw-rw-rw-   0        0        0      625 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe09k.dat
--rw-rw-rw-   0        0        0      720 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe100.dat
--rw-rw-rw-   0        0        0      668 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe101.dat
--rw-rw-rw-   0        0        0      626 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe10k.dat
--rw-rw-rw-   0        0        0      668 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe113.dat
--rw-rw-rw-   0        0        0      721 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe114.dat
--rw-rw-rw-   0        0        0      721 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe115.dat
--rw-rw-rw-   0        0        0      721 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe116.dat
--rw-rw-rw-   0        0        0      721 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe117.dat
--rw-rw-rw-   0        0        0      721 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe118.dat
--rw-rw-rw-   0        0        0      626 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe11k.dat
--rw-rw-rw-   0        0        0      720 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe121.dat
--rw-rw-rw-   0        0        0      720 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe122.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe123.dat
--rw-rw-rw-   0        0        0      720 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe124.dat
--rw-rw-rw-   0        0        0      626 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe12k.dat
--rw-rw-rw-   0        0        0      721 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe133.dat
--rw-rw-rw-   0        0        0      721 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe134.dat
--rw-rw-rw-   0        0        0      721 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe137.dat
--rw-rw-rw-   0        0        0      626 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe13k.dat
--rw-rw-rw-   0        0        0      709 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe14.dat
--rw-rw-rw-   0        0        0      721 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe140.dat
--rw-rw-rw-   0        0        0     2107 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe142.dat
--rw-rw-rw-   0        0        0      721 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe143.dat
--rw-rw-rw-   0        0        0      721 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe144.dat
--rw-rw-rw-   0        0        0      720 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe147.dat
--rw-rw-rw-   0        0        0      626 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe14k.dat
--rw-rw-rw-   0        0        0      709 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe15.dat
--rw-rw-rw-   0        0        0      720 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe155.dat
--rw-rw-rw-   0        0        0      626 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe15k.dat
--rw-rw-rw-   0        0        0      722 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe164.dat
--rw-rw-rw-   0        0        0      722 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe165.dat
--rw-rw-rw-   0        0        0      728 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe167.dat
--rw-rw-rw-   0        0        0      626 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe16k.dat
--rw-rw-rw-   0        0        0      726 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe173.dat
--rw-rw-rw-   0        0        0      726 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe174.dat
--rw-rw-rw-   0        0        0      726 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe176.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe177.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe178.dat
--rw-rw-rw-   0        0        0      721 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe180.dat
--rw-rw-rw-   0        0        0      721 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe182.dat
--rw-rw-rw-   0        0        0      721 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe184.dat
--rw-rw-rw-   0        0        0      730 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe187.dat
--rw-rw-rw-   0        0        0      730 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe188.dat
--rw-rw-rw-   0        0        0      722 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe190.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe195.dat
--rw-rw-rw-   0        0        0      724 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe198.dat
--rw-rw-rw-   0        0        0      724 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe199.dat
--rw-rw-rw-   0        0        0      723 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe207.dat
--rw-rw-rw-   0        0        0      720 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe210.dat
--rw-rw-rw-   0        0        0      722 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe217.dat
--rw-rw-rw-   0        0        0      721 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe222.dat
--rw-rw-rw-   0        0        0      721 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe223.dat
--rw-rw-rw-   0        0        0      721 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe225.dat
--rw-rw-rw-   0        0        0      721 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe226.dat
--rw-rw-rw-   0        0        0      721 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe227.dat
--rw-rw-rw-   0        0        0      721 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe228.dat
--rw-rw-rw-   0        0        0      721 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe229.dat
--rw-rw-rw-   0        0        0      720 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe233.dat
--rw-rw-rw-   0        0        0      720 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe234.dat
--rw-rw-rw-   0        0        0      725 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe235.dat
--rw-rw-rw-   0        0        0      730 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe238.dat
--rw-rw-rw-   0        0        0      721 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe239.dat
--rw-rw-rw-   0        0        0      719 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe240.dat
--rw-rw-rw-   0        0        0      721 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe241.dat
--rw-rw-rw-   0        0        0      721 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe242.dat
--rw-rw-rw-   0        0        0      721 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe243.dat
--rw-rw-rw-   0        0        0      721 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe244.dat
--rw-rw-rw-   0        0        0      721 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe255.dat
--rw-rw-rw-   0        0        0      722 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe256.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe257.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe264.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe265.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe269.dat
--rw-rw-rw-   0        0        0      722 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe274.dat
--rw-rw-rw-   0        0        0      723 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe275.dat
--rw-rw-rw-   0        0        0      724 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe276.dat
--rw-rw-rw-   0        0        0      725 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe277.dat
--rw-rw-rw-   0        0        0      723 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe278.dat
--rw-rw-rw-   0        0        0      722 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe279.dat
--rw-rw-rw-   0        0        0      723 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe280.dat
--rw-rw-rw-   0        0        0      724 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe281.dat
--rw-rw-rw-   0        0        0      725 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe282.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe284.dat
--rw-rw-rw-   0        0        0      752 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe285.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe286.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe287.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe288.dat
--rw-rw-rw-   0        0        0      720 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe289.dat
--rw-rw-rw-   0        0        0      720 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe290.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe298.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe29b.dat
--rw-rw-rw-   0        0        0      606 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe300.dat
--rw-rw-rw-   0        0        0      733 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe301.dat
--rw-rw-rw-   0        0        0      732 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe303.dat
--rw-rw-rw-   0        0        0      732 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe304.dat
--rw-rw-rw-   0        0        0      721 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe308.dat
--rw-rw-rw-   0        0        0      721 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe309.dat
--rw-rw-rw-   0        0        0      721 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe310.dat
--rw-rw-rw-   0        0        0      721 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe311.dat
--rw-rw-rw-   0        0        0      730 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe314.dat
--rw-rw-rw-   0        0        0      736 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe315.dat
--rw-rw-rw-   0        0        0      735 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe316.dat
--rw-rw-rw-   0        0        0      735 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe318.dat
--rw-rw-rw-   0        0        0      733 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe319.dat
--rw-rw-rw-   0        0        0      735 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe320.dat
--rw-rw-rw-   0        0        0      736 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe321.dat
--rw-rw-rw-   0        0        0      735 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe322.dat
--rw-rw-rw-   0        0        0      734 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe323.dat
--rw-rw-rw-   0        0        0      730 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe324.dat
--rw-rw-rw-   0        0        0      721 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe325.dat
--rw-rw-rw-   0        0        0      721 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe326.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe328.dat
--rw-rw-rw-   0        0        0      721 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe329.dat
--rw-rw-rw-   0        0        0      721 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe330.dat
--rw-rw-rw-   0        0        0      721 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe331.dat
--rw-rw-rw-   0        0        0      721 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe332.dat
--rw-rw-rw-   0        0        0      719 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe335.dat
--rw-rw-rw-   0        0        0      721 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe336.dat
--rw-rw-rw-   0        0        0      668 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe342.dat
--rw-rw-rw-   0        0        0      721 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe344.dat
--rw-rw-rw-   0        0        0      736 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe346.dat
--rw-rw-rw-   0        0        0      584 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe358.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe359.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe360.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe361.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe362.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe363.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe364.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe365.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe366.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe367.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe368.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe369.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe370.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe371.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe372.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe373.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe374.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe375.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe376.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe377.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe379.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe380.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe381.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe382.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe383.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe384.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe385.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe386.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe387.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe388.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe389.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe390.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe391.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe392.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe393.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe394.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe395.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe396.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe397.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe398.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe399.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe400.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe401.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe402.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe403.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe404.dat
--rw-rw-rw-   0        0        0      626 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe405.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe406.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe407.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe408.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe409.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe410.dat
--rw-rw-rw-   0        0        0      668 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe411.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe412.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe413.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe414.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe415.dat
--rw-rw-rw-   0        0        0      711 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe416a.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe417.dat
--rw-rw-rw-   0        0        0      683 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe417a.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe418.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe419.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe420.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe421.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe422.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe423.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe424.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe425.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe426.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe427.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe428.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe429.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe430.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe431.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe432.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe433.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe434.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe435.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe436.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe437.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe438.dat
--rw-rw-rw-   0        0        0      626 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe439.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe440.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe441.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe442.dat
--rw-rw-rw-   0        0        0      626 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe443.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe444.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe445.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe446.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe447.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe448.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe449.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe450.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe451.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe456.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe457.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe458.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe459.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe460.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe462.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe464.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe474.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe476.dat
--rw-rw-rw-   0        0        0      542 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe477.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe478.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe479.dat
--rw-rw-rw-   0        0        0      542 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe480.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe481.dat
--rw-rw-rw-   0        0        0      711 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe481a.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe482.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe483.dat
--rw-rw-rw-   0        0        0      668 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe484.dat
--rw-rw-rw-   0        0        0      668 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe488.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe490.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe491.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe492.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe493.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe494.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe495.dat
--rw-rw-rw-   0        0        0      626 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe496.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe497.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe498.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe499.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe500.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe501.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe502.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe503.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe504.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe505.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe506.dat
--rw-rw-rw-   0        0        0      542 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe507.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe508.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe509.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe510.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe511.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe512.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe513.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe514.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe515.dat
--rw-rw-rw-   0        0        0      542 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe517.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe518.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe522.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe523.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe525.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe526.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe527.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe528.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe529.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe530.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe531.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe532.dat
--rw-rw-rw-   0        0        0      668 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe533.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe534.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe535.dat
--rw-rw-rw-   0        0        0      709 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe54.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe546.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe547.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe548.dat
--rw-rw-rw-   0        0        0      878 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe549.dat
--rw-rw-rw-   0        0        0      709 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe55.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe550.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe553.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe559.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe561.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe562.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe563.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe564.dat
--rw-rw-rw-   0        0        0      668 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe565.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe566.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe567.dat
--rw-rw-rw-   0        0        0      709 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe57.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe570.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe571.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe572.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe573.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe574.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe575.dat
--rw-rw-rw-   0        0        0      542 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe584.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe585.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe587.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe590.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe591.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe592.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe593.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe595.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe596.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe598.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe599.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe600.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe601.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe602.dat
--rw-rw-rw-   0        0        0      715 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe602m.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe604.dat
--rw-rw-rw-   0        0        0      670 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe610b.dat
--rw-rw-rw-   0        0        0      633 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe610bm.dat
--rw-rw-rw-   0        0        0      668 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe611.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe612.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe613.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe614.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe615.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe617.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe619.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe620.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe621.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe622.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe623.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe624.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe625.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe626.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe627.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe628.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe629.dat
--rw-rw-rw-   0        0        0      709 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe63.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe630.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe632.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe633.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe645.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe646.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe647.dat
--rw-rw-rw-   0        0        0      731 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe648.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe650.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe652.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe654.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe655.dat
--rw-rw-rw-   0        0        0      626 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe670.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe673.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe675.dat
--rw-rw-rw-   0        0        0      719 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe676.dat
--rw-rw-rw-   0        0        0      718 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe677.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe679.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe681.dat
--rw-rw-rw-   0        0        0      626 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe682.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe683.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe685.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe692.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe693.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe701.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe702.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe703.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe704.dat
--rw-rw-rw-   0        0        0      668 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe711.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe723.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe735.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe738.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe741.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe744.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe746.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe758.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe766.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe767.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe769.dat
--rw-rw-rw-   0        0        0      668 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe770.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe775.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe776.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe777.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe780.dat
--rw-rw-rw-   0        0        0      720 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe79.dat
--rw-rw-rw-   0        0        0     2054 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe795.dat
--rw-rw-rw-   0        0        0     1466 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe795sm.dat
--rw-rw-rw-   0        0        0      878 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe796.dat
--rw-rw-rw-   0        0        0      584 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe797.dat
--rw-rw-rw-   0        0        0      668 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe798.dat
--rw-rw-rw-   0        0        0      720 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe801.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe802.dat
--rw-rw-rw-   0        0        0      880 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe802a.dat
--rw-rw-rw-   0        0        0      985 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe802b.dat
--rw-rw-rw-   0        0        0      849 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe803h.dat
--rw-rw-rw-   0        0        0      675 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe804.dat
--rw-rw-rw-   0        0        0      709 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe81.dat
--rw-rw-rw-   0        0        0      709 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/goe92.dat
--rw-rw-rw-   0        0        0     2074 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/griffith30SymSuction.dat
--rw-rw-rw-   0        0        0      674 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/gs1.dat
--rw-rw-rw-   0        0        0      771 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/gu255118.dat
--rw-rw-rw-   0        0        0     1658 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/hh02.dat
--rw-rw-rw-   0        0        0      602 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/hobie.dat
--rw-rw-rw-   0        0        0     1428 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/hobiesm.dat
--rw-rw-rw-   0        0        0     2054 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/hq010.dat
--rw-rw-rw-   0        0        0     2053 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/hq07.dat
--rw-rw-rw-   0        0        0     2053 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/hq09.dat
--rw-rw-rw-   0        0        0     1636 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/hq1010.dat
--rw-rw-rw-   0        0        0     1636 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/hq1012.dat
--rw-rw-rw-   0        0        0     1635 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/hq108.dat
--rw-rw-rw-   0        0        0     1635 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/hq109.dat
--rw-rw-rw-   0        0        0     1636 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/hq1510.dat
--rw-rw-rw-   0        0        0     2056 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/hq1511.dat
--rw-rw-rw-   0        0        0     1636 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/hq1512.dat
--rw-rw-rw-   0        0        0     1635 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/hq158.dat
--rw-rw-rw-   0        0        0      839 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/hq1585.dat
--rw-rw-rw-   0        0        0     1635 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/hq159.dat
--rw-rw-rw-   0        0        0     1049 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/hq159b.dat
--rw-rw-rw-   0        0        0     1636 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/hq2010.dat
--rw-rw-rw-   0        0        0     1636 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/hq2012.dat
--rw-rw-rw-   0        0        0     1635 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/hq208.dat
--rw-rw-rw-   0        0        0     1635 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/hq209.dat
--rw-rw-rw-   0        0        0      797 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/hq2090sm.dat
--rw-rw-rw-   0        0        0     1133 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/hq2195.dat
--rw-rw-rw-   0        0        0     1636 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/hq2510.dat
--rw-rw-rw-   0        0        0     2056 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/hq2511.dat
--rw-rw-rw-   0        0        0     1636 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/hq2512.dat
--rw-rw-rw-   0        0        0     1635 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/hq258.dat
--rw-rw-rw-   0        0        0     1635 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/hq259.dat
--rw-rw-rw-   0        0        0      933 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/hq2590sm.dat
--rw-rw-rw-   0        0        0     1133 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/hq259b.dat
--rw-rw-rw-   0        0        0     1727 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/hq300gd2.dat
--rw-rw-rw-   0        0        0     1636 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/hq3010.dat
--rw-rw-rw-   0        0        0     1636 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/hq3011.dat
--rw-rw-rw-   0        0        0     1636 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/hq3012.dat
--rw-rw-rw-   0        0        0     1636 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/hq3013.dat
--rw-rw-rw-   0        0        0     1636 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/hq3014.dat
--rw-rw-rw-   0        0        0     1636 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/hq3015.dat
--rw-rw-rw-   0        0        0     1635 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/hq308.dat
--rw-rw-rw-   0        0        0     1635 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/hq309.dat
--rw-rw-rw-   0        0        0     1636 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/hq3510.dat
--rw-rw-rw-   0        0        0     1636 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/hq3512.dat
--rw-rw-rw-   0        0        0     1636 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/hq3513.dat
--rw-rw-rw-   0        0        0      838 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/hq3514.dat
--rw-rw-rw-   0        0        0      838 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/hq3518.dat
--rw-rw-rw-   0        0        0     1635 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/hq358.dat
--rw-rw-rw-   0        0        0     1635 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/hq359.dat
--rw-rw-rw-   0        0        0     2522 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/hsnlf213.dat
--rw-rw-rw-   0        0        0     4839 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ht05.dat
--rw-rw-rw-   0        0        0     4326 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ht08.dat
--rw-rw-rw-   0        0        0     3813 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ht12.dat
--rw-rw-rw-   0        0        0     3867 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ht22.dat
--rw-rw-rw-   0        0        0     3867 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ht23.dat
--rw-rw-rw-   0        0        0      639 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/isa571.dat
--rw-rw-rw-   0        0        0      639 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/isa960.dat
--rw-rw-rw-   0        0        0      639 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/isa961.dat
--rw-rw-rw-   0        0        0      639 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/isa962.dat
--rw-rw-rw-   0        0        0     1359 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/j5012.dat
--rw-rw-rw-   0        0        0     2537 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/jn153.dat
--rw-rw-rw-   0        0        0     1934 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/joukowsk.dat
--rw-rw-rw-   0        0        0     3575 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/k1.dat
--rw-rw-rw-   0        0        0     3759 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/k2.dat
--rw-rw-rw-   0        0        0     3864 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/k3.dat
--rw-rw-rw-   0        0        0     1487 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/k3311.dat
--rw-rw-rw-   0        0        0     2230 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/k3311sm.dat
--rw-rw-rw-   0        0        0     1095 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/kc135a.dat
--rw-rw-rw-   0        0        0     1096 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/kc135b.dat
--rw-rw-rw-   0        0        0     1096 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/kc135c.dat
--rw-rw-rw-   0        0        0     1095 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/kc135d.dat
--rw-rw-rw-   0        0        0     2151 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/kenmar.dat
--rw-rw-rw-   0        0        0     1941 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/l188root.dat
--rw-rw-rw-   0        0        0     1940 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/l188tip.dat
--rw-rw-rw-   0        0        0      717 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/l7769.dat
--rw-rw-rw-   0        0        0     1943 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/la203a.dat
--rw-rw-rw-   0        0        0     2684 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/la2573a.dat
--rw-rw-rw-   0        0        0     1125 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/lds2.dat
--rw-rw-rw-   0        0        0     1590 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/lg10sc.dat
--rw-rw-rw-   0        0        0     2030 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/lnv109a.dat
--rw-rw-rw-   0        0        0     1897 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/lrn1007.dat
--rw-rw-rw-   0        0        0     1003 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ls013.dat
--rw-rw-rw-   0        0        0     1428 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ls413.dat
--rw-rw-rw-   0        0        0     1405 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ls413mod.dat
--rw-rw-rw-   0        0        0     1211 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ls417.dat
--rw-rw-rw-   0        0        0     1463 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ls417mod.dat
--rw-rw-rw-   0        0        0     1200 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ls421.dat
--rw-rw-rw-   0        0        0     1421 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ls421mod.dat
--rw-rw-rw-   0        0        0     2096 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/lwk79100.dat
--rw-rw-rw-   0        0        0     2096 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/lwk80080.dat
--rw-rw-rw-   0        0        0     2096 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/lwk80100.dat
--rw-rw-rw-   0        0        0     2100 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/lwk80120k25.dat
--rw-rw-rw-   0        0        0     2100 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/lwk80150k25.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/m1.dat
--rw-rw-rw-   0        0        0      711 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/m10.dat
--rw-rw-rw-   0        0        0      711 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/m11.dat
--rw-rw-rw-   0        0        0      711 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/m12.dat
--rw-rw-rw-   0        0        0      711 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/m13.dat
--rw-rw-rw-   0        0        0      711 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/m14.dat
--rw-rw-rw-   0        0        0      711 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/m15.dat
--rw-rw-rw-   0        0        0      711 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/m16.dat
--rw-rw-rw-   0        0        0      711 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/m17.dat
--rw-rw-rw-   0        0        0      711 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/m18.dat
--rw-rw-rw-   0        0        0      711 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/m19.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/m2.dat
--rw-rw-rw-   0        0        0      711 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/m20.dat
--rw-rw-rw-   0        0        0      711 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/m21.dat
--rw-rw-rw-   0        0        0      711 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/m22.dat
--rw-rw-rw-   0        0        0      711 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/m23.dat
--rw-rw-rw-   0        0        0      711 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/m24.dat
--rw-rw-rw-   0        0        0      711 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/m25.dat
--rw-rw-rw-   0        0        0      711 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/m26.dat
--rw-rw-rw-   0        0        0      711 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/m27.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/m3.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/m4.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/m5.dat
--rw-rw-rw-   0        0        0      660 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/m6.dat
--rw-rw-rw-   0        0        0      767 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/m665.dat
--rw-rw-rw-   0        0        0      767 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/m685.dat
--rw-rw-rw-   0        0        0      668 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/m7.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/m8.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/m9.dat
--rw-rw-rw-   0        0        0      920 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ma409.dat
--rw-rw-rw-   0        0        0     2230 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ma409sm.dat
--rw-rw-rw-   0        0        0     2177 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/marsden.dat
--rw-rw-rw-   0        0        0      674 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/marske1.dat
--rw-rw-rw-   0        0        0      696 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/marske2.dat
--rw-rw-rw-   0        0        0      703 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/marske3.dat
--rw-rw-rw-   0        0        0      701 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/marske4.dat
--rw-rw-rw-   0        0        0      680 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/marske5.dat
--rw-rw-rw-   0        0        0     1528 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/marske7.dat
--rw-rw-rw-   0        0        0     1427 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/mb253515sm.dat
--rw-rw-rw-   0        0        0     1785 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/mh102.dat
--rw-rw-rw-   0        0        0     1759 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/mh104.dat
--rw-rw-rw-   0        0        0     1785 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/mh106.dat
--rw-rw-rw-   0        0        0     1785 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/mh108.dat
--rw-rw-rw-   0        0        0     1785 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/mh110.dat
--rw-rw-rw-   0        0        0     1603 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/mh112.dat
--rw-rw-rw-   0        0        0     1603 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/mh113.dat
--rw-rw-rw-   0        0        0     1785 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/mh114.dat
--rw-rw-rw-   0        0        0     1785 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/mh115.dat
--rw-rw-rw-   0        0        0     1758 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/mh116.dat
--rw-rw-rw-   0        0        0     1783 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/mh117.dat
--rw-rw-rw-   0        0        0     1603 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/mh120.dat
--rw-rw-rw-   0        0        0     1784 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/mh121.dat
--rw-rw-rw-   0        0        0     1784 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/mh122.dat
--rw-rw-rw-   0        0        0     1603 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/mh150.dat
--rw-rw-rw-   0        0        0     1758 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/mh18.dat
--rw-rw-rw-   0        0        0     1783 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/mh20.dat
--rw-rw-rw-   0        0        0     1785 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/mh200.dat
--rw-rw-rw-   0        0        0     1759 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/mh201.dat
--rw-rw-rw-   0        0        0     1782 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/mh22.dat
--rw-rw-rw-   0        0        0     1780 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/mh23.dat
--rw-rw-rw-   0        0        0     1783 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/mh24.dat
--rw-rw-rw-   0        0        0     1757 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/mh25.dat
--rw-rw-rw-   0        0        0     1758 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/mh26.dat
--rw-rw-rw-   0        0        0     1784 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/mh27.dat
--rw-rw-rw-   0        0        0     1757 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/mh30.dat
--rw-rw-rw-   0        0        0     1782 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/mh32.dat
--rw-rw-rw-   0        0        0     1783 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/mh38.dat
--rw-rw-rw-   0        0        0     1757 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/mh42.dat
--rw-rw-rw-   0        0        0     1782 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/mh43.dat
--rw-rw-rw-   0        0        0     1783 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/mh44.dat
--rw-rw-rw-   0        0        0     1757 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/mh45.dat
--rw-rw-rw-   0        0        0     1782 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/mh46.dat
--rw-rw-rw-   0        0        0     1203 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/mh49.dat
--rw-rw-rw-   0        0        0     1784 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/mh60.dat
--rw-rw-rw-   0        0        0     1784 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/mh61.dat
--rw-rw-rw-   0        0        0     1782 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/mh62.dat
--rw-rw-rw-   0        0        0     1783 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/mh64.dat
--rw-rw-rw-   0        0        0     1784 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/mh70.dat
--rw-rw-rw-   0        0        0     1758 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/mh78.dat
--rw-rw-rw-   0        0        0     1784 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/mh80.dat
--rw-rw-rw-   0        0        0     1755 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/mh81.dat
--rw-rw-rw-   0        0        0     1784 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/mh82.dat
--rw-rw-rw-   0        0        0     1602 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/mh83.dat
--rw-rw-rw-   0        0        0     1758 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/mh84.dat
--rw-rw-rw-   0        0        0     1784 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/mh91.dat
--rw-rw-rw-   0        0        0     1784 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/mh92.dat
--rw-rw-rw-   0        0        0     1784 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/mh93.dat
--rw-rw-rw-   0        0        0     1784 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/mh94.dat
--rw-rw-rw-   0        0        0     1602 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/mh95.dat
--rw-rw-rw-   0        0        0     1174 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/miley.dat
--rw-rw-rw-   0        0        0     2768 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/mrc-16.dat
--rw-rw-rw-   0        0        0     2768 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/mrc-20.dat
--rw-rw-rw-   0        0        0     1507 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ms313.dat
--rw-rw-rw-   0        0        0     1417 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ms317.dat
--rw-rw-rw-   0        0        0     2093 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/mue139.dat
--rw-rw-rw-   0        0        0     1395 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/n0009sm.dat
--rw-rw-rw-   0        0        0     1583 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/n0011sc.dat
--rw-rw-rw-   0        0        0     2772 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/n0012.dat
--rw-rw-rw-   0        0        0      633 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/n10.dat
--rw-rw-rw-   0        0        0      633 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/n11.dat
--rw-rw-rw-   0        0        0      799 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/n11h9.dat
--rw-rw-rw-   0        0        0      648 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/n12.dat
--rw-rw-rw-   0        0        0      648 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/n13.dat
--rw-rw-rw-   0        0        0      648 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/n14.dat
--rw-rw-rw-   0        0        0      756 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/n1h15.dat
--rw-rw-rw-   0        0        0      633 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/n22.dat
--rw-rw-rw-   0        0        0      633 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/n24.dat
--rw-rw-rw-   0        0        0     1170 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/n2414.dat
--rw-rw-rw-   0        0        0     1170 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/n2415.dat
--rw-rw-rw-   0        0        0      756 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/n2h15.dat
--rw-rw-rw-   0        0        0      756 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/n5h10.dat
--rw-rw-rw-   0        0        0      756 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/n5h15.dat
--rw-rw-rw-   0        0        0      756 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/n5h20.dat
--rw-rw-rw-   0        0        0     1015 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/n63010a.dat
--rw-rw-rw-   0        0        0     1016 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/n63012a.dat
--rw-rw-rw-   0        0        0     1016 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/n63015a.dat
--rw-rw-rw-   0        0        0     1013 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/n63210.dat
--rw-rw-rw-   0        0        0     1013 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/n63212.dat
--rw-rw-rw-   0        0        0     1013 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/n63215.dat
--rw-rw-rw-   0        0        0     1803 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/n63215b.dat
--rw-rw-rw-   0        0        0     1011 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/n63412.dat
--rw-rw-rw-   0        0        0     1012 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/n63415.dat
--rw-rw-rw-   0        0        0     1016 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/n64008a.dat
--rw-rw-rw-   0        0        0     1022 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/n64012.dat
--rw-rw-rw-   0        0        0     1016 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/n64012a.dat
--rw-rw-rw-   0        0        0      991 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/n64015.dat
--rw-rw-rw-   0        0        0     1017 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/n64015a.dat
--rw-rw-rw-   0        0        0     1242 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/n6409.dat
--rw-rw-rw-   0        0        0     1014 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/n64108.dat
--rw-rw-rw-   0        0        0     1014 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/n64110.dat
--rw-rw-rw-   0        0        0     1089 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/n64212.dat
--rw-rw-rw-   0        0        0     1221 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/n64212ma.dat
--rw-rw-rw-   0        0        0      906 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/n64212mb.dat
--rw-rw-rw-   0        0        0     1014 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/n64215.dat
--rw-rw-rw-   0        0        0      770 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/n642415.dat
--rw-rw-rw-   0        0        0     1014 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/n66021.dat
--rw-rw-rw-   0        0        0      756 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/n6h10.dat
--rw-rw-rw-   0        0        0      756 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/n6h15.dat
--rw-rw-rw-   0        0        0      756 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/n6h20.dat
--rw-rw-rw-   0        0        0      777 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/n8h12.dat
--rw-rw-rw-   0        0        0      632 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/n9.dat
--rw-rw-rw-   0        0        0      728 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/naca0006.dat
--rw-rw-rw-   0        0        0      728 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/naca0008.dat
--rw-rw-rw-   0        0        0      690 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/naca000834.dat
--rw-rw-rw-   0        0        0      728 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/naca0010.dat
--rw-rw-rw-   0        0        0      690 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/naca001034.dat
--rw-rw-rw-   0        0        0      782 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/naca001034a08cli0.2.dat
--rw-rw-rw-   0        0        0      690 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/naca001035.dat
--rw-rw-rw-   0        0        0      690 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/naca001064.dat
--rw-rw-rw-   0        0        0      690 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/naca001065.dat
--rw-rw-rw-   0        0        0      690 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/naca001066.dat
--rw-rw-rw-   0        0        0      690 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/naca001234.dat
--rw-rw-rw-   0        0        0      690 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/naca001264.dat
--rw-rw-rw-   0        0        0      739 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/naca001264a08cli0.2.dat
--rw-rw-rw-   0        0        0      728 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/naca0015.dat
--rw-rw-rw-   0        0        0      728 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/naca0018.dat
--rw-rw-rw-   0        0        0      728 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/naca0021.dat
--rw-rw-rw-   0        0        0      728 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/naca0024.dat
--rw-rw-rw-   0        0        0     1609 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/naca1.dat
--rw-rw-rw-   0        0        0      763 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/naca1408.dat
--rw-rw-rw-   0        0        0      763 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/naca1410.dat
--rw-rw-rw-   0        0        0      763 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/naca1412.dat
--rw-rw-rw-   0        0        0      689 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/naca16006.dat
--rw-rw-rw-   0        0        0     2097 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/naca16009.dat
--rw-rw-rw-   0        0        0      689 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/naca16012.dat
--rw-rw-rw-   0        0        0      689 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/naca16015.dat
--rw-rw-rw-   0        0        0      689 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/naca16018.dat
--rw-rw-rw-   0        0        0      689 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/naca16021.dat
--rw-rw-rw-   0        0        0     1300 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/naca23012.dat
--rw-rw-rw-   0        0        0      755 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/naca23015.dat
--rw-rw-rw-   0        0        0      755 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/naca23018.dat
--rw-rw-rw-   0        0        0      755 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/naca23021.dat
--rw-rw-rw-   0        0        0      763 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/naca23024.dat
--rw-rw-rw-   0        0        0      763 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/naca2408.dat
--rw-rw-rw-   0        0        0      763 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/naca2410.dat
--rw-rw-rw-   0        0        0     1240 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/naca2411.dat
--rw-rw-rw-   0        0        0      754 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/naca2415.dat
--rw-rw-rw-   0        0        0      754 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/naca2418.dat
--rw-rw-rw-   0        0        0      754 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/naca2421.dat
--rw-rw-rw-   0        0        0      762 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/naca2424.dat
--rw-rw-rw-   0        0        0      734 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/naca4412.dat
--rw-rw-rw-   0        0        0     2095 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/naca4415.dat
--rw-rw-rw-   0        0        0      754 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/naca4418.dat
--rw-rw-rw-   0        0        0      754 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/naca4421.dat
--rw-rw-rw-   0        0        0      762 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/naca4424.dat
--rw-rw-rw-   0        0        0     1106 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/naca63206.dat
--rw-rw-rw-   0        0        0     1107 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/naca63209.dat
--rw-rw-rw-   0        0        0     1107 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/naca632615.dat
--rw-rw-rw-   0        0        0     2101 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/naca632a015.dat
--rw-rw-rw-   0        0        0     2100 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/naca633018.dat
--rw-rw-rw-   0        0        0     1111 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/naca633218.dat
--rw-rw-rw-   0        0        0     2089 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/naca633418.dat
--rw-rw-rw-   0        0        0     1108 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/naca633618.dat
--rw-rw-rw-   0        0        0     1111 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/naca634221.dat
--rw-rw-rw-   0        0        0     1110 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/naca634421.dat
--rw-rw-rw-   0        0        0     1130 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/naca63a210.dat
--rw-rw-rw-   0        0        0     1111 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/naca641112.dat
--rw-rw-rw-   0        0        0     1499 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/naca6412.dat
--rw-rw-rw-   0        0        0     1106 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/naca64206.dat
--rw-rw-rw-   0        0        0     1107 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/naca64208.dat
--rw-rw-rw-   0        0        0     1107 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/naca64209.dat
--rw-rw-rw-   0        0        0     1107 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/naca64210.dat
--rw-rw-rw-   0        0        0     1111 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/naca642215.dat
--rw-rw-rw-   0        0        0     1109 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/naca642415.dat
--rw-rw-rw-   0        0        0     1111 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/naca643218.dat
--rw-rw-rw-   0        0        0     1088 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/naca643418.dat
--rw-rw-rw-   0        0        0     1108 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/naca643618.dat
--rw-rw-rw-   0        0        0     1111 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/naca644221.dat
--rw-rw-rw-   0        0        0     1110 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/naca644421.dat
--rw-rw-rw-   0        0        0     3574 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/naca64a010.dat
--rw-rw-rw-   0        0        0     1109 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/naca64a210.dat
--rw-rw-rw-   0        0        0     1109 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/naca64a410.dat
--rw-rw-rw-   0        0        0     1111 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/naca651212.dat
--rw-rw-rw-   0        0        0     1117 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/naca651212a06.dat
--rw-rw-rw-   0        0        0     1065 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/naca651412.dat
--rw-rw-rw-   0        0        0     1106 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/naca65206.dat
--rw-rw-rw-   0        0        0     1107 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/naca65209.dat
--rw-rw-rw-   0        0        0     1107 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/naca65210.dat
--rw-rw-rw-   0        0        0     1111 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/naca652215.dat
--rw-rw-rw-   0        0        0     1110 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/naca652415.dat
--rw-rw-rw-   0        0        0     1117 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/naca652415a05.dat
--rw-rw-rw-   0        0        0     1111 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/naca653218.dat
--rw-rw-rw-   0        0        0     1106 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/naca65410.dat
--rw-rw-rw-   0        0        0     1111 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/naca654221.dat
--rw-rw-rw-   0        0        0     1110 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/naca654421.dat
--rw-rw-rw-   0        0        0     1117 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/naca654421a05.dat
--rw-rw-rw-   0        0        0     1429 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/naca66-018.dat
--rw-rw-rw-   0        0        0     1111 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/naca661212.dat
--rw-rw-rw-   0        0        0     1107 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/naca66206.dat
--rw-rw-rw-   0        0        0     1108 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/naca66209.dat
--rw-rw-rw-   0        0        0     1108 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/naca66210.dat
--rw-rw-rw-   0        0        0     1111 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/naca662215.dat
--rw-rw-rw-   0        0        0     1110 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/naca662415.dat
--rw-rw-rw-   0        0        0     1111 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/naca663218.dat
--rw-rw-rw-   0        0        0     1111 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/naca663418.dat
--rw-rw-rw-   0        0        0     1111 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/naca664221.dat
--rw-rw-rw-   0        0        0     1110 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/naca671215.dat
--rw-rw-rw-   0        0        0     1109 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/naca747a315.dat
--rw-rw-rw-   0        0        0     1109 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/naca747a415.dat
--rw-rw-rw-   0        0        0      637 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/nacacyh.dat
--rw-rw-rw-   0        0        0      653 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/nacam12.dat
--rw-rw-rw-   0        0        0      637 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/nacam18.dat
--rw-rw-rw-   0        0        0      652 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/nacam2.dat
--rw-rw-rw-   0        0        0      652 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/nacam3.dat
--rw-rw-rw-   0        0        0      690 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/nacam6.dat
--rw-rw-rw-   0        0        0     1686 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/nasasc2-0714.dat
--rw-rw-rw-   0        0        0     1687 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ncambre.dat
--rw-rw-rw-   0        0        0     2326 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/nl722343.dat
--rw-rw-rw-   0        0        0     2258 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/nl722362.dat
--rw-rw-rw-   0        0        0     1174 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/nlf0115.dat
--rw-rw-rw-   0        0        0      974 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/nlf0215f.dat
--rw-rw-rw-   0        0        0     1357 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/nlf1015.dat
--rw-rw-rw-   0        0        0     1754 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/nlf414f.dat
--rw-rw-rw-   0        0        0     2786 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/nlf415.dat
--rw-rw-rw-   0        0        0      990 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/nlf416.dat
--rw-rw-rw-   0        0        0     1146 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/nlr1t.dat
--rw-rw-rw-   0        0        0     1627 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/nlr7301.dat
--rw-rw-rw-   0        0        0     2080 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/nn7mk20.dat
--rw-rw-rw-   0        0        0     2128 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/npl9510.dat
--rw-rw-rw-   0        0        0     2224 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/npl9615.dat
--rw-rw-rw-   0        0        0     1762 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/npl9626.dat
--rw-rw-rw-   0        0        0     1762 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/npl9627.dat
--rw-rw-rw-   0        0        0     2392 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/npl9660.dat
--rw-rw-rw-   0        0        0     1336 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/nplx.dat
--rw-rw-rw-   0        0        0     2395 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/oa206.dat
--rw-rw-rw-   0        0        0     2395 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/oa209.dat
--rw-rw-rw-   0        0        0     2395 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/oa212.dat
--rw-rw-rw-   0        0        0     2395 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/oa213.dat
--rw-rw-rw-   0        0        0     2137 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/oaf095.dat
--rw-rw-rw-   0        0        0     2137 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/oaf102.dat
--rw-rw-rw-   0        0        0     2137 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/oaf117.dat
--rw-rw-rw-   0        0        0     2137 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/oaf128.dat
--rw-rw-rw-   0        0        0     2137 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/oaf139.dat
--rw-rw-rw-   0        0        0      890 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/p51droot.dat
--rw-rw-rw-   0        0        0      888 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/p51dtip.dat
--rw-rw-rw-   0        0        0     1934 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/p51hroot.dat
--rw-rw-rw-   0        0        0     1931 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/p51htip.dat
--rw-rw-rw-   0        0        0     1031 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/pfcm.dat
--rw-rw-rw-   0        0        0     1916 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/pmc19sm.dat
--rw-rw-rw-   0        0        0     1815 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/prandtldroot.dat
--rw-rw-rw-   0        0        0     2694 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/prandtldtip.dat
--rw-rw-rw-   0        0        0     1234 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/psu-90-125wl.dat
--rw-rw-rw-   0        0        0     1183 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/psu94097.dat
--rw-rw-rw-   0        0        0     2063 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/pt40.dat
--rw-rw-rw-   0        0        0     2535 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/r1046.dat
--rw-rw-rw-   0        0        0     2542 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/r1080.dat
--rw-rw-rw-   0        0        0     2547 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/r1082.dat
--rw-rw-rw-   0        0        0     2547 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/r1082t.dat
--rw-rw-rw-   0        0        0     2156 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/r140.dat
--rw-rw-rw-   0        0        0     2071 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/r140sm.dat
--rw-rw-rw-   0        0        0     3350 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/rae100.dat
--rw-rw-rw-   0        0        0     3350 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/rae101.dat
--rw-rw-rw-   0        0        0     3350 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/rae102.dat
--rw-rw-rw-   0        0        0     3350 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/rae103.dat
--rw-rw-rw-   0        0        0     3350 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/rae104.dat
--rw-rw-rw-   0        0        0     2470 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/rae2822.dat
--rw-rw-rw-   0        0        0     1471 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/rae5212.dat
--rw-rw-rw-   0        0        0     1468 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/rae5213.dat
--rw-rw-rw-   0        0        0     1463 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/rae5214.dat
--rw-rw-rw-   0        0        0     1463 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/rae5215.dat
--rw-rw-rw-   0        0        0     2521 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/rae69ck.dat
--rw-rw-rw-   0        0        0      667 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/raf15.dat
--rw-rw-rw-   0        0        0      709 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/raf19.dat
--rw-rw-rw-   0        0        0      709 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/raf25.dat
--rw-rw-rw-   0        0        0      709 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/raf26.dat
--rw-rw-rw-   0        0        0      709 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/raf27.dat
--rw-rw-rw-   0        0        0      709 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/raf28.dat
--rw-rw-rw-   0        0        0      667 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/raf30.dat
--rw-rw-rw-   0        0        0      629 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/raf30md.dat
--rw-rw-rw-   0        0        0      751 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/raf31.dat
--rw-rw-rw-   0        0        0      541 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/raf32.dat
--rw-rw-rw-   0        0        0      629 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/raf32md.dat
--rw-rw-rw-   0        0        0      709 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/raf33.dat
--rw-rw-rw-   0        0        0      709 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/raf34.dat
--rw-rw-rw-   0        0        0      541 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/raf38.dat
--rw-rw-rw-   0        0        0      658 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/raf48.dat
--rw-rw-rw-   0        0        0      540 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/raf6.dat
--rw-rw-rw-   0        0        0      541 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/raf69.dat
--rw-rw-rw-   0        0        0      541 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/raf89.dat
--rw-rw-rw-   0        0        0     1197 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/rc0864c.dat
--rw-rw-rw-   0        0        0     1268 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/rc08b3.dat
--rw-rw-rw-   0        0        0     1776 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/rc08n1.dat
--rw-rw-rw-   0        0        0     1129 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/rc1064c.dat
--rw-rw-rw-   0        0        0     1268 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/rc10b3.dat
--rw-rw-rw-   0        0        0     1776 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/rc10n1.dat
--rw-rw-rw-   0        0        0      925 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/rc1264c.dat
--rw-rw-rw-   0        0        0     1268 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/rc12b3.dat
--rw-rw-rw-   0        0        0     1776 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/rc12n1.dat
--rw-rw-rw-   0        0        0     1755 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/rc410.dat
--rw-rw-rw-   0        0        0     1755 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/rc510.dat
--rw-rw-rw-   0        0        0     1280 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/rcsc2.dat
--rw-rw-rw-   0        0        0     2177 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/rg12.dat
--rw-rw-rw-   0        0        0     1274 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/rg12a.dat
--rw-rw-rw-   0        0        0     1347 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/rg12a189.dat
--rw-rw-rw-   0        0        0     1317 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/rg14.dat
--rw-rw-rw-   0        0        0     1258 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/rg1410.dat
--rw-rw-rw-   0        0        0     1257 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/rg149.dat
--rw-rw-rw-   0        0        0     1259 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/rg1495.dat
--rw-rw-rw-   0        0        0     1347 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/rg14a147.dat
--rw-rw-rw-   0        0        0     1242 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/rg15.dat
--rw-rw-rw-   0        0        0     1348 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/rg15a111.dat
--rw-rw-rw-   0        0        0     1348 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/rg15a213.dat
--rw-rw-rw-   0        0        0     1295 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/rg8.dat
--rw-rw-rw-   0        0        0      648 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/rhodesg30.dat
--rw-rw-rw-   0        0        0      648 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/rhodesg32.dat
--rw-rw-rw-   0        0        0      648 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/rhodesg34.dat
--rw-rw-rw-   0        0        0      648 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/rhodesg36.dat
--rw-rw-rw-   0        0        0     1483 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/s1010.dat
--rw-rw-rw-   0        0        0     1471 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/s1012.dat
--rw-rw-rw-   0        0        0     1471 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/s1014.dat
--rw-rw-rw-   0        0        0     1471 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/s1016.dat
--rw-rw-rw-   0        0        0     1493 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/s1020.dat
--rw-rw-rw-   0        0        0     1741 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/s1046.dat
--rw-rw-rw-   0        0        0     1741 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/s1048.dat
--rw-rw-rw-   0        0        0     2275 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/s1091.dat
--rw-rw-rw-   0        0        0     2287 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/s1210.dat
--rw-rw-rw-   0        0        0     2927 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/s1221.dat
--rw-rw-rw-   0        0        0     6612 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/s1223.dat
--rw-rw-rw-   0        0        0     3411 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/s1223rtl.dat
--rw-rw-rw-   0        0        0     1125 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/s2027.dat
--rw-rw-rw-   0        0        0     1125 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/s2046.dat
--rw-rw-rw-   0        0        0     1291 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/s2048.dat
--rw-rw-rw-   0        0        0     1843 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/s2050.dat
--rw-rw-rw-   0        0        0     1291 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/s2055.dat
--rw-rw-rw-   0        0        0     1479 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/s2060.dat
--rw-rw-rw-   0        0        0     1479 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/s2062.dat
--rw-rw-rw-   0        0        0     1294 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/s2091.dat
--rw-rw-rw-   0        0        0      742 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/s3.dat
--rw-rw-rw-   0        0        0     1057 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/s3002.dat
--rw-rw-rw-   0        0        0     1051 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/s3010.dat
--rw-rw-rw-   0        0        0     1232 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/s3014.dat
--rw-rw-rw-   0        0        0     1053 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/s3016.dat
--rw-rw-rw-   0        0        0     1294 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/s3021.dat
--rw-rw-rw-   0        0        0     1240 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/s3024.dat
--rw-rw-rw-   0        0        0     1176 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/s3025.dat
--rw-rw-rw-   0        0        0     1123 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/s4022.dat
--rw-rw-rw-   0        0        0     1123 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/s4053.dat
--rw-rw-rw-   0        0        0     1294 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/s4061.dat
--rw-rw-rw-   0        0        0     1051 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/s4062.dat
--rw-rw-rw-   0        0        0     2280 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/s4083.dat
--rw-rw-rw-   0        0        0     1123 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/s4110.dat
--rw-rw-rw-   0        0        0     1123 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/s4158.dat
--rw-rw-rw-   0        0        0     1232 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/s4180.dat
--rw-rw-rw-   0        0        0     1294 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/s4233.dat
--rw-rw-rw-   0        0        0     1123 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/s4310.dat
--rw-rw-rw-   0        0        0     1123 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/s4320.dat
--rw-rw-rw-   0        0        0     2142 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/s5010.dat
--rw-rw-rw-   0        0        0     2142 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/s5020.dat
--rw-rw-rw-   0        0        0     1475 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/s6061.dat
--rw-rw-rw-   0        0        0     1476 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/s6062.dat
--rw-rw-rw-   0        0        0     1477 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/s6063.dat
--rw-rw-rw-   0        0        0     2281 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/s7012.dat
--rw-rw-rw-   0        0        0     1973 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/s7055.dat
--rw-rw-rw-   0        0        0     2280 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/s7075.dat
--rw-rw-rw-   0        0        0     3400 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/s8025.dat
--rw-rw-rw-   0        0        0     3425 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/s8035.dat
--rw-rw-rw-   0        0        0     2281 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/s8036.dat
--rw-rw-rw-   0        0        0     2281 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/s8037.dat
--rw-rw-rw-   0        0        0     2281 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/s8038.dat
--rw-rw-rw-   0        0        0     2284 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/s8052.dat
--rw-rw-rw-   0        0        0     2282 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/s8055.dat
--rw-rw-rw-   0        0        0     2916 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/s9000.dat
--rw-rw-rw-   0        0        0     3404 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/s9026.dat
--rw-rw-rw-   0        0        0     3402 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/s9027.dat
--rw-rw-rw-   0        0        0     2916 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/s9032.dat
--rw-rw-rw-   0        0        0     2918 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/s9033.dat
--rw-rw-rw-   0        0        0     2311 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/s9037.dat
--rw-rw-rw-   0        0        0     2276 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/sa7035.dat
--rw-rw-rw-   0        0        0     2276 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/sa7036.dat
--rw-rw-rw-   0        0        0     2276 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/sa7038.dat
--rw-rw-rw-   0        0        0      626 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/saratov.dat
--rw-rw-rw-   0        0        0     3067 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/sc1012r8.dat
--rw-rw-rw-   0        0        0     3075 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/sc1094r8.dat
--rw-rw-rw-   0        0        0     2775 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/sc1095.dat
--rw-rw-rw-   0        0        0     2243 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/sc1095r8.dat
--rw-rw-rw-   0        0        0     4022 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/sc20010.dat
--rw-rw-rw-   0        0        0     4022 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/sc20012.dat
--rw-rw-rw-   0        0        0     4027 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/sc20402.dat
--rw-rw-rw-   0        0        0     4018 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/sc20403.dat
--rw-rw-rw-   0        0        0     4024 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/sc20404.dat
--rw-rw-rw-   0        0        0     4024 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/sc20406.dat
--rw-rw-rw-   0        0        0     4009 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/sc20410.dat
--rw-rw-rw-   0        0        0     4009 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/sc20412.dat
--rw-rw-rw-   0        0        0     4009 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/sc20414.dat
--rw-rw-rw-   0        0        0     4028 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/sc20503.dat
--rw-rw-rw-   0        0        0     4017 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/sc20518.dat
--rw-rw-rw-   0        0        0     4028 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/sc20606.dat
--rw-rw-rw-   0        0        0     4025 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/sc20610.dat
--rw-rw-rw-   0        0        0     4025 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/sc20612.dat
--rw-rw-rw-   0        0        0     4025 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/sc20614.dat
--rw-rw-rw-   0        0        0     4029 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/sc20706.dat
--rw-rw-rw-   0        0        0     4027 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/sc20710.dat
--rw-rw-rw-   0        0        0     4027 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/sc20712.dat
--rw-rw-rw-   0        0        0     4026 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/sc20714.dat
--rw-rw-rw-   0        0        0     4042 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/sc21006.dat
--rw-rw-rw-   0        0        0     4038 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/sc21010.dat
--rw-rw-rw-   0        0        0     1847 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/sc2110.dat
--rw-rw-rw-   0        0        0     1231 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/sd2030.dat
--rw-rw-rw-   0        0        0     1233 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/sd2083.dat
--rw-rw-rw-   0        0        0     1233 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/sd5060.dat
--rw-rw-rw-   0        0        0     1233 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/sd6060.dat
--rw-rw-rw-   0        0        0     1233 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/sd6080.dat
--rw-rw-rw-   0        0        0     1233 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/sd7003.dat
--rw-rw-rw-   0        0        0     1233 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/sd7032.dat
--rw-rw-rw-   0        0        0     1227 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/sd7034.dat
--rw-rw-rw-   0        0        0     1233 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/sd7037.dat
--rw-rw-rw-   0        0        0     1233 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/sd7043.dat
--rw-rw-rw-   0        0        0     1232 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/sd7062.dat
--rw-rw-rw-   0        0        0     1233 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/sd7080.dat
--rw-rw-rw-   0        0        0     1233 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/sd7084.dat
--rw-rw-rw-   0        0        0     1232 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/sd7090.dat
--rw-rw-rw-   0        0        0     1233 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/sd8000.dat
--rw-rw-rw-   0        0        0     1229 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/sd8020.dat
--rw-rw-rw-   0        0        0     1232 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/sd8040.dat
--rw-rw-rw-   0        0        0     2276 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/sg6040.dat
--rw-rw-rw-   0        0        0     1952 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/sg6041.dat
--rw-rw-rw-   0        0        0     2276 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/sg6042.dat
--rw-rw-rw-   0        0        0     1952 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/sg6043.dat
--rw-rw-rw-   0        0        0     2276 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/sg6050.dat
--rw-rw-rw-   0        0        0     2276 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/sg6051.dat
--rw-rw-rw-   0        0        0     1316 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/sm701.dat
--rw-rw-rw-   0        0        0      752 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/sokolov.dat
--rw-rw-rw-   0        0        0      994 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/spicasm.dat
--rw-rw-rw-   0        0        0     2778 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ssca07.dat
--rw-rw-rw-   0        0        0     2779 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ssca09.dat
--rw-rw-rw-   0        0        0      663 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/stcyr171.dat
--rw-rw-rw-   0        0        0      663 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/stcyr172.dat
--rw-rw-rw-   0        0        0      655 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/stcyr234.dat
--rw-rw-rw-   0        0        0      656 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/stcyr24.dat
--rw-rw-rw-   0        0        0     1288 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ste87151.dat
--rw-rw-rw-   0        0        0     1291 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ste87391.dat
--rw-rw-rw-   0        0        0     1288 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/stf86361.dat
--rw-rw-rw-   0        0        0      602 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/strand.dat
--rw-rw-rw-   0        0        0     2559 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/tempest1.dat
--rw-rw-rw-   0        0        0     2557 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/tempest2.dat
--rw-rw-rw-   0        0        0     2560 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/tempest3.dat
--rw-rw-rw-   0        0        0     1207 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/th25816.dat
--rw-rw-rw-   0        0        0     2067 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/trainer60.dat
--rw-rw-rw-   0        0        0      712 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/tsagi12.dat
--rw-rw-rw-   0        0        0      711 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/tsagi8.dat
--rw-rw-rw-   0        0        0     1063 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ua2-180.dat
--rw-rw-rw-   0        0        0     1246 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ua2-180sm.dat
--rw-rw-rw-   0        0        0     1450 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ua79sf18.dat
--rw-rw-rw-   0        0        0      798 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ua79sff.dat
--rw-rw-rw-   0        0        0     1007 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ua79sfm.dat
--rw-rw-rw-   0        0        0     2096 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/uag8814320.dat
--rw-rw-rw-   0        0        0     1612 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ui1720.dat
--rw-rw-rw-   0        0        0     2066 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ultimate.dat
--rw-rw-rw-   0        0        0     2068 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/us1000root.dat
--rw-rw-rw-   0        0        0      709 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/usa22.dat
--rw-rw-rw-   0        0        0      709 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/usa25.dat
--rw-rw-rw-   0        0        0      709 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/usa26.dat
--rw-rw-rw-   0        0        0      709 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/usa27.dat
--rw-rw-rw-   0        0        0      714 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/usa27m2.dat
--rw-rw-rw-   0        0        0      709 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/usa28.dat
--rw-rw-rw-   0        0        0      709 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/usa29.dat
--rw-rw-rw-   0        0        0      709 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/usa31.dat
--rw-rw-rw-   0        0        0      709 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/usa32.dat
--rw-rw-rw-   0        0        0      709 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/usa33.dat
--rw-rw-rw-   0        0        0      709 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/usa34.dat
--rw-rw-rw-   0        0        0      709 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/usa35.dat
--rw-rw-rw-   0        0        0      711 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/usa35a.dat
--rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/usa35b.dat
--rw-rw-rw-   0        0        0      709 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/usa40.dat
--rw-rw-rw-   0        0        0      711 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/usa40b.dat
--rw-rw-rw-   0        0        0      709 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/usa41.dat
--rw-rw-rw-   0        0        0      709 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/usa45.dat
--rw-rw-rw-   0        0        0      711 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/usa45m.dat
--rw-rw-rw-   0        0        0      709 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/usa46.dat
--rw-rw-rw-   0        0        0      709 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/usa48.dat
--rw-rw-rw-   0        0        0      709 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/usa49.dat
--rw-rw-rw-   0        0        0      708 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/usa5.dat
--rw-rw-rw-   0        0        0      709 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/usa50.dat
--rw-rw-rw-   0        0        0      709 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/usa51.dat
--rw-rw-rw-   0        0        0      541 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/usa98.dat
--rw-rw-rw-   0        0        0     1994 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/usnps4.dat
--rw-rw-rw-   0        0        0      890 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/v13006.dat
--rw-rw-rw-   0        0        0      861 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/v13009.dat
--rw-rw-rw-   0        0        0     1083 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/v23010.dat
--rw-rw-rw-   0        0        0     1570 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/v43012.dat
--rw-rw-rw-   0        0        0      898 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/v43015.dat
--rw-rw-rw-   0        0        0      771 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/vr1.dat
--rw-rw-rw-   0        0        0     1041 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/vr11x.dat
--rw-rw-rw-   0        0        0     1607 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/vr12.dat
--rw-rw-rw-   0        0        0     1607 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/vr13.dat
--rw-rw-rw-   0        0        0     1607 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/vr14.dat
--rw-rw-rw-   0        0        0     1607 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/vr15.dat
--rw-rw-rw-   0        0        0      867 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/vr5.dat
--rw-rw-rw-   0        0        0      940 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/vr7.dat
--rw-rw-rw-   0        0        0      917 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/vr7b.dat
--rw-rw-rw-   0        0        0      781 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/vr8.dat
--rw-rw-rw-   0        0        0      777 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/vr8b.dat
--rw-rw-rw-   0        0        0      825 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/vr9.dat
--rw-rw-rw-   0        0        0     2229 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/waspsm.dat
--rw-rw-rw-   0        0        0     1174 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/wb13535sm.dat
--rw-rw-rw-   0        0        0      899 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/wb140.dat
--rw-rw-rw-   0        0        0     1017 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/whitcomb.dat
--rw-rw-rw-   0        0        0     2122 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ys900.dat
--rw-rw-rw-   0        0        0     2244 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ys915.dat
--rw-rw-rw-   0        0        0     2358 2022-03-22 17:49:10.000000 PteraSoftware-2.2.1/pterasoftware/airfoils/ys930.dat
--rw-rw-rw-   0        0        0    68650 2022-06-27 17:48:47.000000 PteraSoftware-2.2.1/pterasoftware/convergence.py
--rw-rw-rw-   0        0        0    27335 2022-06-27 17:48:47.000000 PteraSoftware-2.2.1/pterasoftware/functions.py
--rw-rw-rw-   0        0        0    43804 2022-06-27 17:48:47.000000 PteraSoftware-2.2.1/pterasoftware/geometry.py
--rw-rw-rw-   0        0        0    39210 2022-06-27 17:48:47.000000 PteraSoftware-2.2.1/pterasoftware/meshing.py
--rw-rw-rw-   0        0        0    65154 2022-06-27 17:48:47.000000 PteraSoftware-2.2.1/pterasoftware/movement.py
--rw-rw-rw-   0        0        0     6403 2022-04-19 18:41:43.000000 PteraSoftware-2.2.1/pterasoftware/operating_point.py
--rw-rw-rw-   0        0        0    47945 2022-06-27 17:48:47.000000 PteraSoftware-2.2.1/pterasoftware/output.py
--rw-rw-rw-   0        0        0    10339 2022-06-27 17:48:47.000000 PteraSoftware-2.2.1/pterasoftware/panel.py
--rw-rw-rw-   0        0        0     5114 2022-06-27 17:48:47.000000 PteraSoftware-2.2.1/pterasoftware/problems.py
--rw-rw-rw-   0        0        0    16700 2022-06-27 17:48:47.000000 PteraSoftware-2.2.1/pterasoftware/steady_horseshoe_vortex_lattice_method.py
--rw-rw-rw-   0        0        0    31868 2022-06-27 17:48:47.000000 PteraSoftware-2.2.1/pterasoftware/steady_ring_vortex_lattice_method.py
--rw-rw-rw-   0        0        0    12239 2022-06-27 17:48:47.000000 PteraSoftware-2.2.1/pterasoftware/trim.py
--rw-rw-rw-   0        0        0    87336 2022-06-28 21:56:29.000000 PteraSoftware-2.2.1/pterasoftware/unsteady_ring_vortex_lattice_method.py
--rw-rw-rw-   0        0        0      122 2022-06-28 21:56:29.000000 PteraSoftware-2.2.1/pyproject.toml
--rw-rw-rw-   0        0        0     1484 2022-06-28 22:06:15.738809 PteraSoftware-2.2.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-22 18:57:29.022927 PteraSoftware-3.0.0/
+-rw-rw-rw-   0        0        0     1093 2023-06-22 18:55:41.000000 PteraSoftware-3.0.0/LICENSE.txt
+-rw-rw-rw-   0        0        0      138 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    14950 2023-06-22 18:57:29.022927 PteraSoftware-3.0.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-22 18:57:22.526295 PteraSoftware-3.0.0/PteraSoftware.egg-info/
+-rw-rw-rw-   0        0        0    14950 2023-06-22 18:57:22.000000 PteraSoftware-3.0.0/PteraSoftware.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    54086 2023-06-22 18:57:22.000000 PteraSoftware-3.0.0/PteraSoftware.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 18:57:22.000000 PteraSoftware-3.0.0/PteraSoftware.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      200 2023-06-22 18:57:22.000000 PteraSoftware-3.0.0/PteraSoftware.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-22 18:57:22.000000 PteraSoftware-3.0.0/PteraSoftware.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    13845 2023-06-22 18:55:41.000000 PteraSoftware-3.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-22 18:57:22.543362 PteraSoftware-3.0.0/pterasoftware/
+-rw-rw-rw-   0        0        0     2469 2023-06-22 18:55:41.000000 PteraSoftware-3.0.0/pterasoftware/__init__.py
+-rw-rw-rw-   0        0        0    46408 2023-06-22 18:55:41.000000 PteraSoftware-3.0.0/pterasoftware/aerodynamics.py
+drwxrwxrwx   0        0        0        0 2023-06-22 18:57:29.012959 PteraSoftware-3.0.0/pterasoftware/airfoils/
+-rw-rw-rw-   0        0        0      685 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/2032c.dat
+-rw-rw-rw-   0        0        0      104 2023-06-22 18:55:41.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/__init__.py
+-rw-rw-rw-   0        0        0      918 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/a18.dat
+-rw-rw-rw-   0        0        0     2228 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/a18sm.dat
+-rw-rw-rw-   0        0        0     1285 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/a63a108c.dat
+-rw-rw-rw-   0        0        0     4885 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ag03.dat
+-rw-rw-rw-   0        0        0     4866 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ag04.dat
+-rw-rw-rw-   0        0        0     4866 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ag08.dat
+-rw-rw-rw-   0        0        0     4866 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ag09.dat
+-rw-rw-rw-   0        0        0     4866 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ag10.dat
+-rw-rw-rw-   0        0        0     4947 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ag11.dat
+-rw-rw-rw-   0        0        0     4326 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ag12.dat
+-rw-rw-rw-   0        0        0     4326 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ag13.dat
+-rw-rw-rw-   0        0        0     4326 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ag14.dat
+-rw-rw-rw-   0        0        0     4326 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ag16.dat
+-rw-rw-rw-   0        0        0     3686 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ag17.dat
+-rw-rw-rw-   0        0        0     3686 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ag18.dat
+-rw-rw-rw-   0        0        0     4326 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ag19.dat
+-rw-rw-rw-   0        0        0     4470 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ag24.dat
+-rw-rw-rw-   0        0        0     4470 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ag25.dat
+-rw-rw-rw-   0        0        0     4470 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ag26.dat
+-rw-rw-rw-   0        0        0     4472 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ag27.dat
+-rw-rw-rw-   0        0        0     4866 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ag35.dat
+-rw-rw-rw-   0        0        0     4866 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ag36.dat
+-rw-rw-rw-   0        0        0     4866 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ag37.dat
+-rw-rw-rw-   0        0        0     4866 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ag38.dat
+-rw-rw-rw-   0        0        0     4603 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ag44ct02r.dat
+-rw-rw-rw-   0        0        0     4609 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ag455ct02r.dat
+-rw-rw-rw-   0        0        0     4575 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ag45c03.dat
+-rw-rw-rw-   0        0        0     4603 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ag45ct02r.dat
+-rw-rw-rw-   0        0        0     4656 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ag46c03.dat
+-rw-rw-rw-   0        0        0     4636 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ag46ct02r.dat
+-rw-rw-rw-   0        0        0     4575 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ag47c03.dat
+-rw-rw-rw-   0        0        0     4636 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ag47ct02r.dat
+-rw-rw-rw-   0        0        0     1436 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ah21-7.dat
+-rw-rw-rw-   0        0        0     1375 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ah21-9.dat
+-rw-rw-rw-   0        0        0     2089 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ah63k127.dat
+-rw-rw-rw-   0        0        0      670 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ah6407.dat
+-rw-rw-rw-   0        0        0      670 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ah7476.dat
+-rw-rw-rw-   0        0        0     2058 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ah79100a.dat
+-rw-rw-rw-   0        0        0     2058 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ah79100b.dat
+-rw-rw-rw-   0        0        0     2058 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ah79100c.dat
+-rw-rw-rw-   0        0        0     2095 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ah79k132.dat
+-rw-rw-rw-   0        0        0     2098 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ah79k135.dat
+-rw-rw-rw-   0        0        0     2096 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ah79k143.dat
+-rw-rw-rw-   0        0        0     2095 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ah80129.dat
+-rw-rw-rw-   0        0        0     2096 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ah80136.dat
+-rw-rw-rw-   0        0        0     2095 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ah80140.dat
+-rw-rw-rw-   0        0        0     2101 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ah81131.dat
+-rw-rw-rw-   0        0        0     2097 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ah81k144.dat
+-rw-rw-rw-   0        0        0     2108 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ah81k144wfKlappe.dat
+-rw-rw-rw-   0        0        0     2087 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ah82150a.dat
+-rw-rw-rw-   0        0        0     2091 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ah82150f.dat
+-rw-rw-rw-   0        0        0     2088 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ah83150q.dat
+-rw-rw-rw-   0        0        0     2085 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ah83159.dat
+-rw-rw-rw-   0        0        0     2100 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ah85l120.dat
+-rw-rw-rw-   0        0        0     2088 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ah88k130.dat
+-rw-rw-rw-   0        0        0     2296 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ah88k136.dat
+-rw-rw-rw-   0        0        0     2291 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ah93156.dat
+-rw-rw-rw-   0        0        0     2291 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ah93157.dat
+-rw-rw-rw-   0        0        0     2296 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ah93k130.dat
+-rw-rw-rw-   0        0        0     2296 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ah93k131.dat
+-rw-rw-rw-   0        0        0     2296 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ah93k132.dat
+-rw-rw-rw-   0        0        0     2098 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ah93w145.dat
+-rw-rw-rw-   0        0        0     2087 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ah93w174.dat
+-rw-rw-rw-   0        0        0     2100 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ah93w215.dat
+-rw-rw-rw-   0        0        0     2098 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ah93w257.dat
+-rw-rw-rw-   0        0        0     2098 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ah93w300.dat
+-rw-rw-rw-   0        0        0     2161 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ah93w480b.dat
+-rw-rw-rw-   0        0        0     2291 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ah94145.dat
+-rw-rw-rw-   0        0        0     2291 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ah94156.dat
+-rw-rw-rw-   0        0        0     2098 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ah94w301.dat
+-rw-rw-rw-   0        0        0     2291 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ah95160.dat
+-rw-rw-rw-   0        0        0     1240 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ames01.dat
+-rw-rw-rw-   0        0        0     1756 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ames02.dat
+-rw-rw-rw-   0        0        0     1758 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ames03.dat
+-rw-rw-rw-   0        0        0     1189 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/amsoil1.dat
+-rw-rw-rw-   0        0        0     1187 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/amsoil2.dat
+-rw-rw-rw-   0        0        0      990 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/apex16.dat
+-rw-rw-rw-   0        0        0     1461 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/aquilasm.dat
+-rw-rw-rw-   0        0        0      864 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/arad10.dat
+-rw-rw-rw-   0        0        0      864 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/arad13.dat
+-rw-rw-rw-   0        0        0      864 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/arad20.dat
+-rw-rw-rw-   0        0        0      847 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/arad6.dat
+-rw-rw-rw-   0        0        0     1321 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/as5045.dat
+-rw-rw-rw-   0        0        0     1427 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/as5046.dat
+-rw-rw-rw-   0        0        0     1368 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/as5048.dat
+-rw-rw-rw-   0        0        0     1676 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/atr72sm.dat
+-rw-rw-rw-   0        0        0     2096 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/august160.dat
+-rw-rw-rw-   0        0        0     2066 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/avistar.dat
+-rw-rw-rw-   0        0        0      838 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/b29root.dat
+-rw-rw-rw-   0        0        0      837 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/b29tip.dat
+-rw-rw-rw-   0        0        0     1506 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/b540ols.dat
+-rw-rw-rw-   0        0        0     2570 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/b707a.dat
+-rw-rw-rw-   0        0        0      632 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/b707b.dat
+-rw-rw-rw-   0        0        0      539 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/b707c.dat
+-rw-rw-rw-   0        0        0      601 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/b707d.dat
+-rw-rw-rw-   0        0        0     2570 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/b707e.dat
+-rw-rw-rw-   0        0        0      901 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/b737a.dat
+-rw-rw-rw-   0        0        0      904 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/b737b.dat
+-rw-rw-rw-   0        0        0      905 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/b737c.dat
+-rw-rw-rw-   0        0        0      906 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/b737d.dat
+-rw-rw-rw-   0        0        0     1960 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/bacj.dat
+-rw-rw-rw-   0        0        0      939 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/bacxxx.dat
+-rw-rw-rw-   0        0        0      638 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/bambino6.dat
+-rw-rw-rw-   0        0        0      963 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/be50.dat
+-rw-rw-rw-   0        0        0     2229 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/be50sm.dat
+-rw-rw-rw-   0        0        0      734 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/boe103.dat
+-rw-rw-rw-   0        0        0      713 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/boe106.dat
+-rw-rw-rw-   0        0        0     1903 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/bqm34.dat
+-rw-rw-rw-   0        0        0     2000 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/bw3.dat
+-rw-rw-rw-   0        0        0     1394 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/c141a.dat
+-rw-rw-rw-   0        0        0     1398 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/c141b.dat
+-rw-rw-rw-   0        0        0     1399 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/c141c.dat
+-rw-rw-rw-   0        0        0     1399 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/c141d.dat
+-rw-rw-rw-   0        0        0     1399 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/c141e.dat
+-rw-rw-rw-   0        0        0     1399 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/c141f.dat
+-rw-rw-rw-   0        0        0     1309 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/c5a.dat
+-rw-rw-rw-   0        0        0     1313 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/c5b.dat
+-rw-rw-rw-   0        0        0     1311 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/c5c.dat
+-rw-rw-rw-   0        0        0     1313 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/c5d.dat
+-rw-rw-rw-   0        0        0     1312 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/c5e.dat
+-rw-rw-rw-   0        0        0      794 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/cap21c.dat
+-rw-rw-rw-   0        0        0     1211 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/cast102.dat
+-rw-rw-rw-   0        0        0     2229 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ch10sm.dat
+-rw-rw-rw-   0        0        0     2073 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/chen.dat
+-rw-rw-rw-   0        0        0      584 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/clarkk.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/clarkv.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/clarkw.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/clarkx.dat
+-rw-rw-rw-   0        0        0     2559 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/clarky.dat
+-rw-rw-rw-   0        0        0      608 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/clarkyh.dat
+-rw-rw-rw-   0        0        0      711 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/clarkys.dat
+-rw-rw-rw-   0        0        0     1468 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/clarkysm.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/clarkz.dat
+-rw-rw-rw-   0        0        0      714 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/clarym15.dat
+-rw-rw-rw-   0        0        0      714 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/clarym18.dat
+-rw-rw-rw-   0        0        0      637 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/coanda1.dat
+-rw-rw-rw-   0        0        0      637 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/coanda2.dat
+-rw-rw-rw-   0        0        0      637 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/coanda3.dat
+-rw-rw-rw-   0        0        0      648 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/cootie.dat
+-rw-rw-rw-   0        0        0     1909 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/cr001sm.dat
+-rw-rw-rw-   0        0        0     2623 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/cr1.dat
+-rw-rw-rw-   0        0        0      640 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/curtisc72.dat
+-rw-rw-rw-   0        0        0     1717 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/dae11.dat
+-rw-rw-rw-   0        0        0     1696 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/dae21.dat
+-rw-rw-rw-   0        0        0     1738 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/dae31.dat
+-rw-rw-rw-   0        0        0     1696 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/dae51.dat
+-rw-rw-rw-   0        0        0      708 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/davis.dat
+-rw-rw-rw-   0        0        0     1942 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/davis_corrected.dat
+-rw-rw-rw-   0        0        0     1909 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/davissm.dat
+-rw-rw-rw-   0        0        0      644 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/daytonwright6.dat
+-rw-rw-rw-   0        0        0      646 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/daytonwrightt1.dat
+-rw-rw-rw-   0        0        0      703 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/dbln526.dat
+-rw-rw-rw-   0        0        0     1688 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/defcnd1.dat
+-rw-rw-rw-   0        0        0     1689 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/defcnd2.dat
+-rw-rw-rw-   0        0        0     1690 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/defcnd3.dat
+-rw-rw-rw-   0        0        0     1318 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/df101.dat
+-rw-rw-rw-   0        0        0     1240 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/df102.dat
+-rw-rw-rw-   0        0        0     2927 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/dfvlrr4.dat
+-rw-rw-rw-   0        0        0      640 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/dga1138.dat
+-rw-rw-rw-   0        0        0      655 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/dga1182.dat
+-rw-rw-rw-   0        0        0     1910 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/dh4009sm.dat
+-rw-rw-rw-   0        0        0     2058 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/doa5.dat
+-rw-rw-rw-   0        0        0      635 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/dormoy.dat
+-rw-rw-rw-   0        0        0     2958 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/drgnfly.dat
+-rw-rw-rw-   0        0        0     2318 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/dsma523a.dat
+-rw-rw-rw-   0        0        0     2321 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/dsma523b.dat
+-rw-rw-rw-   0        0        0     2042 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/du8608418.dat
+-rw-rw-rw-   0        0        0      862 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/du861372.dat
+-rw-rw-rw-   0        0        0     1324 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e1098.dat
+-rw-rw-rw-   0        0        0     1323 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e1200.dat
+-rw-rw-rw-   0        0        0     1302 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e1210.dat
+-rw-rw-rw-   0        0        0     1281 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e1211.dat
+-rw-rw-rw-   0        0        0      985 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e1212.dat
+-rw-rw-rw-   0        0        0     1139 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e1212mod.dat
+-rw-rw-rw-   0        0        0     1281 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e1213.dat
+-rw-rw-rw-   0        0        0     1302 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e1214.dat
+-rw-rw-rw-   0        0        0     1494 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e1230.dat
+-rw-rw-rw-   0        0        0     2059 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e1233.dat
+-rw-rw-rw-   0        0        0     1313 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e168.dat
+-rw-rw-rw-   0        0        0     1313 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e169.dat
+-rw-rw-rw-   0        0        0     1313 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e171.dat
+-rw-rw-rw-   0        0        0     1318 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e174.dat
+-rw-rw-rw-   0        0        0     1313 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e176.dat
+-rw-rw-rw-   0        0        0     1297 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e178.dat
+-rw-rw-rw-   0        0        0     1312 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e180.dat
+-rw-rw-rw-   0        0        0     1296 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e182.dat
+-rw-rw-rw-   0        0        0     1312 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e184.dat
+-rw-rw-rw-   0        0        0     1312 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e186.dat
+-rw-rw-rw-   0        0        0     1312 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e193.dat
+-rw-rw-rw-   0        0        0     1312 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e195.dat
+-rw-rw-rw-   0        0        0     1312 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e197.dat
+-rw-rw-rw-   0        0        0     1312 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e201.dat
+-rw-rw-rw-   0        0        0     1312 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e203.dat
+-rw-rw-rw-   0        0        0     1312 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e205.dat
+-rw-rw-rw-   0        0        0     1312 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e207.dat
+-rw-rw-rw-   0        0        0     1312 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e209.dat
+-rw-rw-rw-   0        0        0     1312 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e210.dat
+-rw-rw-rw-   0        0        0     1312 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e211.dat
+-rw-rw-rw-   0        0        0     1312 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e212.dat
+-rw-rw-rw-   0        0        0     1312 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e214.dat
+-rw-rw-rw-   0        0        0     1312 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e216.dat
+-rw-rw-rw-   0        0        0     1312 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e220.dat
+-rw-rw-rw-   0        0        0     1312 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e221.dat
+-rw-rw-rw-   0        0        0     1312 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e222.dat
+-rw-rw-rw-   0        0        0     1312 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e224.dat
+-rw-rw-rw-   0        0        0     1312 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e226.dat
+-rw-rw-rw-   0        0        0     1313 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e228.dat
+-rw-rw-rw-   0        0        0     1312 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e230.dat
+-rw-rw-rw-   0        0        0      977 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e231.dat
+-rw-rw-rw-   0        0        0     1301 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e266.dat
+-rw-rw-rw-   0        0        0     1490 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e297.dat
+-rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e325.dat
+-rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e326.dat
+-rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e327.dat
+-rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e328.dat
+-rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e329.dat
+-rw-rw-rw-   0        0        0     1511 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e330.dat
+-rw-rw-rw-   0        0        0     1511 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e331.dat
+-rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e332.dat
+-rw-rw-rw-   0        0        0     1511 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e333.dat
+-rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e334.dat
+-rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e335.dat
+-rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e336.dat
+-rw-rw-rw-   0        0        0     1553 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e337.dat
+-rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e338.dat
+-rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e339.dat
+-rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e340.dat
+-rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e341.dat
+-rw-rw-rw-   0        0        0     1511 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e342.dat
+-rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e343.dat
+-rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e344.dat
+-rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e360.dat
+-rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e361.dat
+-rw-rw-rw-   0        0        0     1285 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e374.dat
+-rw-rw-rw-   0        0        0     1302 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e376.dat
+-rw-rw-rw-   0        0        0     1302 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e377.dat
+-rw-rw-rw-   0        0        0     1418 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e377m.dat
+-rw-rw-rw-   0        0        0     1302 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e378.dat
+-rw-rw-rw-   0        0        0     1302 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e379.dat
+-rw-rw-rw-   0        0        0     1312 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e385.dat
+-rw-rw-rw-   0        0        0     1287 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e387.dat
+-rw-rw-rw-   0        0        0     1312 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e392.dat
+-rw-rw-rw-   0        0        0     1322 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e393.dat
+-rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e395.dat
+-rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e396.dat
+-rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e397.dat
+-rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e398.dat
+-rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e399.dat
+-rw-rw-rw-   0        0        0     1301 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e403.dat
+-rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e407.dat
+-rw-rw-rw-   0        0        0     1301 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e417.dat
+-rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e420.dat
+-rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e421.dat
+-rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e422.dat
+-rw-rw-rw-   0        0        0     1447 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e423.dat
+-rw-rw-rw-   0        0        0      860 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e426.dat
+-rw-rw-rw-   0        0        0      860 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e428.dat
+-rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e431.dat
+-rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e432.dat
+-rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e433.dat
+-rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e434.dat
+-rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e435.dat
+-rw-rw-rw-   0        0        0     1312 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e471.dat
+-rw-rw-rw-   0        0        0     1301 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e472.dat
+-rw-rw-rw-   0        0        0     1301 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e473.dat
+-rw-rw-rw-   0        0        0     1312 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e474.dat
+-rw-rw-rw-   0        0        0     1312 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e475.dat
+-rw-rw-rw-   0        0        0     1284 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e476.dat
+-rw-rw-rw-   0        0        0     1284 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e477.dat
+-rw-rw-rw-   0        0        0     1284 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e478.dat
+-rw-rw-rw-   0        0        0     1301 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e479.dat
+-rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e485.dat
+-rw-rw-rw-   0        0        0      523 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e49.dat
+-rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e502.dat
+-rw-rw-rw-   0        0        0     1490 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e520.dat
+-rw-rw-rw-   0        0        0     1490 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e521.dat
+-rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e540.dat
+-rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e541.dat
+-rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e542.dat
+-rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e543.dat
+-rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e544.dat
+-rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e545.dat
+-rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e546.dat
+-rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e547.dat
+-rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e548.dat
+-rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e549.dat
+-rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e550.dat
+-rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e551.dat
+-rw-rw-rw-   0        0        0     1511 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e552.dat
+-rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e553.dat
+-rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e554.dat
+-rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e555.dat
+-rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e556.dat
+-rw-rw-rw-   0        0        0     1511 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e557.dat
+-rw-rw-rw-   0        0        0     1301 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e558.dat
+-rw-rw-rw-   0        0        0     1301 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e559.dat
+-rw-rw-rw-   0        0        0     1301 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e560.dat
+-rw-rw-rw-   0        0        0     1301 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e561.dat
+-rw-rw-rw-   0        0        0     1301 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e562.dat
+-rw-rw-rw-   0        0        0      754 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e58.dat
+-rw-rw-rw-   0        0        0     1301 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e580.dat
+-rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e582.dat
+-rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e583.dat
+-rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e584.dat
+-rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e585.dat
+-rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e587.dat
+-rw-rw-rw-   0        0        0      754 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e59.dat
+-rw-rw-rw-   0        0        0      936 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e591.dat
+-rw-rw-rw-   0        0        0     1511 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e593.dat
+-rw-rw-rw-   0        0        0     1511 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e598.dat
+-rw-rw-rw-   0        0        0     1301 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e603.dat
+-rw-rw-rw-   0        0        0     1490 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e604.dat
+-rw-rw-rw-   0        0        0     1312 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e61.dat
+-rw-rw-rw-   0        0        0     1312 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e62.dat
+-rw-rw-rw-   0        0        0     2099 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e625.dat
+-rw-rw-rw-   0        0        0     1312 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e63.dat
+-rw-rw-rw-   0        0        0     1301 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e635.dat
+-rw-rw-rw-   0        0        0     1301 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e636.dat
+-rw-rw-rw-   0        0        0     1301 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e637.dat
+-rw-rw-rw-   0        0        0     1301 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e638.dat
+-rw-rw-rw-   0        0        0     1301 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e639.dat
+-rw-rw-rw-   0        0        0     1312 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e64.dat
+-rw-rw-rw-   0        0        0     1301 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e642.dat
+-rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e654.dat
+-rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e655.dat
+-rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e656.dat
+-rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e657.dat
+-rw-rw-rw-   0        0        0     1300 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e66.dat
+-rw-rw-rw-   0        0        0      980 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e662.dat
+-rw-rw-rw-   0        0        0     1302 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e664.dat
+-rw-rw-rw-   0        0        0     1364 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e664ex.dat
+-rw-rw-rw-   0        0        0     1532 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e668.dat
+-rw-rw-rw-   0        0        0     1321 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e67.dat
+-rw-rw-rw-   0        0        0     1301 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e678.dat
+-rw-rw-rw-   0        0        0     1321 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e68.dat
+-rw-rw-rw-   0        0        0     1301 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e682.dat
+-rw-rw-rw-   0        0        0     1301 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e694.dat
+-rw-rw-rw-   0        0        0     1312 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e71.dat
+-rw-rw-rw-   0        0        0     1427 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e715.dat
+-rw-rw-rw-   0        0        0     1302 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e748.dat
+-rw-rw-rw-   0        0        0     1301 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e793.dat
+-rw-rw-rw-   0        0        0     1458 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e817.dat
+-rw-rw-rw-   0        0        0     1437 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e818.dat
+-rw-rw-rw-   0        0        0     1312 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e836.dat
+-rw-rw-rw-   0        0        0     1312 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e837.dat
+-rw-rw-rw-   0        0        0     1312 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e838.dat
+-rw-rw-rw-   0        0        0     1543 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e850.dat
+-rw-rw-rw-   0        0        0     1428 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e851.dat
+-rw-rw-rw-   0        0        0     1428 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e852.dat
+-rw-rw-rw-   0        0        0     1407 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e853.dat
+-rw-rw-rw-   0        0        0     1428 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e854.dat
+-rw-rw-rw-   0        0        0     1406 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e855.dat
+-rw-rw-rw-   0        0        0     1427 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e856.dat
+-rw-rw-rw-   0        0        0     1406 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e857.dat
+-rw-rw-rw-   0        0        0     1427 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e858.dat
+-rw-rw-rw-   0        0        0     1307 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e862.dat
+-rw-rw-rw-   0        0        0     1307 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e863.dat
+-rw-rw-rw-   0        0        0     1307 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e864.dat
+-rw-rw-rw-   0        0        0     2550 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e874.dat
+-rw-rw-rw-   0        0        0     2309 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e904.dat
+-rw-rw-rw-   0        0        0     2309 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/e908.dat
+-rw-rw-rw-   0        0        0      596 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ea61009.dat
+-rw-rw-rw-   0        0        0      596 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ea61012.dat
+-rw-rw-rw-   0        0        0      596 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ea81006.dat
+-rw-rw-rw-   0        0        0      639 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ebambino7.dat
+-rw-rw-rw-   0        0        0      681 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ec863914.dat
+-rw-rw-rw-   0        0        0     2012 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/eh0009.dat
+-rw-rw-rw-   0        0        0     1778 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/eh1070.dat
+-rw-rw-rw-   0        0        0     2289 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/eh1090.dat
+-rw-rw-rw-   0        0        0     2289 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/eh1590.dat
+-rw-rw-rw-   0        0        0     2329 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/eh2010.dat
+-rw-rw-rw-   0        0        0     2234 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/eh2012.dat
+-rw-rw-rw-   0        0        0     1779 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/eh2070.dat
+-rw-rw-rw-   0        0        0     1991 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/eh2510.dat
+-rw-rw-rw-   0        0        0     2031 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/eh3012.dat
+-rw-rw-rw-   0        0        0      626 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/eiffel10.dat
+-rw-rw-rw-   0        0        0      647 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/eiffel371.dat
+-rw-rw-rw-   0        0        0      649 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/eiffel385.dat
+-rw-rw-rw-   0        0        0      649 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/eiffel428.dat
+-rw-rw-rw-   0        0        0      652 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/eiffel430.dat
+-rw-rw-rw-   0        0        0     2064 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/esa40.dat
+-rw-rw-rw-   0        0        0     1587 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/falcon.dat
+-rw-rw-rw-   0        0        0      755 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fauvel.dat
+-rw-rw-rw-   0        0        0      645 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fg1.dat
+-rw-rw-rw-   0        0        0      645 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fg2.dat
+-rw-rw-rw-   0        0        0      645 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fg3.dat
+-rw-rw-rw-   0        0        0      645 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fg4.dat
+-rw-rw-rw-   0        0        0      515 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx049915.dat
+-rw-rw-rw-   0        0        0     1057 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx05188.dat
+-rw-rw-rw-   0        0        0     1057 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx05191.dat
+-rw-rw-rw-   0        0        0      505 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx057816.dat
+-rw-rw-rw-   0        0        0     1059 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx05h126.dat
+-rw-rw-rw-   0        0        0      510 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx082512.dat
+-rw-rw-rw-   0        0        0     1059 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx08s176.dat
+-rw-rw-rw-   0        0        0     1010 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx2.dat
+-rw-rw-rw-   0        0        0     1010 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx3.dat
+-rw-rw-rw-   0        0        0     2056 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx38153.dat
+-rw-rw-rw-   0        0        0     2056 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx60100.dat
+-rw-rw-rw-   0        0        0      760 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx601001.dat
+-rw-rw-rw-   0        0        0     1469 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx60100sm.dat
+-rw-rw-rw-   0        0        0     2065 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx60126.dat
+-rw-rw-rw-   0        0        0     2058 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx601261.dat
+-rw-rw-rw-   0        0        0     2056 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx60157.dat
+-rw-rw-rw-   0        0        0      796 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx60160.dat
+-rw-rw-rw-   0        0        0     2056 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx60177.dat
+-rw-rw-rw-   0        0        0     2056 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx61140.dat
+-rw-rw-rw-   0        0        0     2056 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx61147.dat
+-rw-rw-rw-   0        0        0     2056 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx61163.dat
+-rw-rw-rw-   0        0        0     2056 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx61168.dat
+-rw-rw-rw-   0        0        0     2056 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx61184.dat
+-rw-rw-rw-   0        0        0     1710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx62k131.dat
+-rw-rw-rw-   0        0        0     2061 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx62k153.dat
+-rw-rw-rw-   0        0        0      712 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx63100.dat
+-rw-rw-rw-   0        0        0      712 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx63110.dat
+-rw-rw-rw-   0        0        0      754 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx63120.dat
+-rw-rw-rw-   0        0        0     1894 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx63137.dat
+-rw-rw-rw-   0        0        0     1407 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx63137sm.dat
+-rw-rw-rw-   0        0        0     2056 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx63143.dat
+-rw-rw-rw-   0        0        0     2056 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx63145.dat
+-rw-rw-rw-   0        0        0     2056 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx63147.dat
+-rw-rw-rw-   0        0        0     2056 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx63158.dat
+-rw-rw-rw-   0        0        0     1852 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx6617a2.dat
+-rw-rw-rw-   0        0        0     1339 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx6617ai.dat
+-rw-rw-rw-   0        0        0     1846 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx66182.dat
+-rw-rw-rw-   0        0        0     1851 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx66196v.dat
+-rw-rw-rw-   0        0        0     1718 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx66a175.dat
+-rw-rw-rw-   0        0        0     2096 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx66h60.dat
+-rw-rw-rw-   0        0        0     2099 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx66h80.dat
+-rw-rw-rw-   0        0        0     1848 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx66s161.dat
+-rw-rw-rw-   0        0        0     1848 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx66s171.dat
+-rw-rw-rw-   0        0        0     1848 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx66s196.dat
+-rw-rw-rw-   0        0        0     1851 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx67k150.dat
+-rw-rw-rw-   0        0        0     1851 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx67k170.dat
+-rw-rw-rw-   0        0        0     2097 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx68h120.dat
+-rw-rw-rw-   0        0        0     2095 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx69274.dat
+-rw-rw-rw-   0        0        0      929 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx69h083.dat
+-rw-rw-rw-   0        0        0      815 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx69h098.dat
+-rw-rw-rw-   0        0        0     2084 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx69pr281.dat
+-rw-rw-rw-   0        0        0     1814 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx71089a.dat
+-rw-rw-rw-   0        0        0     1813 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx71120.dat
+-rw-rw-rw-   0        0        0     1851 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx711520.dat
+-rw-rw-rw-   0        0        0     1851 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx711525.dat
+-rw-rw-rw-   0        0        0     1719 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx711530.dat
+-rw-rw-rw-   0        0        0     1303 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx71l150.dat
+-rw-rw-rw-   0        0        0     1859 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx72150a.dat
+-rw-rw-rw-   0        0        0     1859 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx72150b.dat
+-rw-rw-rw-   0        0        0     2070 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx72ls160.dat
+-rw-rw-rw-   0        0        0     2082 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx73170.dat
+-rw-rw-rw-   0        0        0     2090 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx73170a.dat
+-rw-rw-rw-   0        0        0     2076 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx73cl1152.dat
+-rw-rw-rw-   0        0        0     2072 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx73cl2152.dat
+-rw-rw-rw-   0        0        0     2071 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx73cl3152.dat
+-rw-rw-rw-   0        0        0     2087 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx73k170.dat
+-rw-rw-rw-   0        0        0     2066 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx74080.dat
+-rw-rw-rw-   0        0        0     2088 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx74130wp1.dat
+-rw-rw-rw-   0        0        0     2086 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx74130wp2.dat
+-rw-rw-rw-   0        0        0     2090 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx74130wp2mod.dat
+-rw-rw-rw-   0        0        0     1665 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx74cl5140.dat
+-rw-rw-rw-   0        0        0     2070 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx74cl6140.dat
+-rw-rw-rw-   0        0        0     2243 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx74modsm.dat
+-rw-rw-rw-   0        0        0     2080 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx75141.dat
+-rw-rw-rw-   0        0        0     2083 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx75193.dat
+-rw-rw-rw-   0        0        0     2097 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx75vg166.dat
+-rw-rw-rw-   0        0        0     2095 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx76100.dat
+-rw-rw-rw-   0        0        0     2095 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx76120.dat
+-rw-rw-rw-   0        0        0     2065 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx76mp120.dat
+-rw-rw-rw-   0        0        0     2071 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx76mp140.dat
+-rw-rw-rw-   0        0        0     2080 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx76mp160.dat
+-rw-rw-rw-   0        0        0     2095 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx77080.dat
+-rw-rw-rw-   0        0        0     2097 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx77w121.dat
+-rw-rw-rw-   0        0        0     2025 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx77w153.dat
+-rw-rw-rw-   0        0        0     2025 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx77w258.dat
+-rw-rw-rw-   0        0        0     2098 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx77w270.dat
+-rw-rw-rw-   0        0        0     2099 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx77w270s.dat
+-rw-rw-rw-   0        0        0     2025 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx77w343.dat
+-rw-rw-rw-   0        0        0     2100 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx78k140.dat
+-rw-rw-rw-   0        0        0     2098 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx78k140a20.dat
+-rw-rw-rw-   0        0        0     2100 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx78k150.dat
+-rw-rw-rw-   0        0        0     2097 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx78k161.dat
+-rw-rw-rw-   0        0        0     2101 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx78pk188.dat
+-rw-rw-rw-   0        0        0     1917 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx79k144.dat
+-rw-rw-rw-   0        0        0     2097 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx79l100.dat
+-rw-rw-rw-   0        0        0     2097 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx79l120.dat
+-rw-rw-rw-   0        0        0     2099 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx79w151a.dat
+-rw-rw-rw-   0        0        0     2100 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx79w470a.dat
+-rw-rw-rw-   0        0        0     2099 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx79w660a.dat
+-rw-rw-rw-   0        0        0     2083 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx80080.dat
+-rw-rw-rw-   0        0        0     2078 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx83w108.dat
+-rw-rw-rw-   0        0        0     2085 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx83w160.dat
+-rw-rw-rw-   0        0        0     2097 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx83w227.dat
+-rw-rw-rw-   0        0        0     2091 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx84w097.dat
+-rw-rw-rw-   0        0        0     2088 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx84w127.dat
+-rw-rw-rw-   0        0        0     2088 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx84w140.dat
+-rw-rw-rw-   0        0        0     2088 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx84w150.dat
+-rw-rw-rw-   0        0        0     2089 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx84w175.dat
+-rw-rw-rw-   0        0        0     2093 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fx84w218.dat
+-rw-rw-rw-   0        0        0     2063 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fxl142k.dat
+-rw-rw-rw-   0        0        0     1919 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fxlv152.dat
+-rw-rw-rw-   0        0        0     1877 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fxm2.dat
+-rw-rw-rw-   0        0        0     2058 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fxs02196.dat
+-rw-rw-rw-   0        0        0     2058 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fxs03182.dat
+-rw-rw-rw-   0        0        0     2060 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/fxs21158.dat
+-rw-rw-rw-   0        0        0     2231 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/geminism.dat
+-rw-rw-rw-   0        0        0     1090 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/giiia.dat
+-rw-rw-rw-   0        0        0     1091 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/giiib.dat
+-rw-rw-rw-   0        0        0     1091 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/giiic.dat
+-rw-rw-rw-   0        0        0     1091 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/giiid.dat
+-rw-rw-rw-   0        0        0     1092 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/giiie.dat
+-rw-rw-rw-   0        0        0     1092 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/giiif.dat
+-rw-rw-rw-   0        0        0     1092 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/giiig.dat
+-rw-rw-rw-   0        0        0     1092 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/giiih.dat
+-rw-rw-rw-   0        0        0     1092 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/giiii.dat
+-rw-rw-rw-   0        0        0     1092 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/giiij.dat
+-rw-rw-rw-   0        0        0     1092 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/giiik.dat
+-rw-rw-rw-   0        0        0     1092 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/giiil.dat
+-rw-rw-rw-   0        0        0     1092 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/giiim.dat
+-rw-rw-rw-   0        0        0     1092 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/giiin.dat
+-rw-rw-rw-   0        0        0      644 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/glennmartin2.dat
+-rw-rw-rw-   0        0        0      643 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/glennmartin3.dat
+-rw-rw-rw-   0        0        0      645 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/glennmartin4.dat
+-rw-rw-rw-   0        0        0     2229 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/gm15sm.dat
+-rw-rw-rw-   0        0        0      667 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe05k.dat
+-rw-rw-rw-   0        0        0      667 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe06k.dat
+-rw-rw-rw-   0        0        0      667 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe07k.dat
+-rw-rw-rw-   0        0        0      667 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe08k.dat
+-rw-rw-rw-   0        0        0      625 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe09k.dat
+-rw-rw-rw-   0        0        0      720 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe100.dat
+-rw-rw-rw-   0        0        0      668 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe101.dat
+-rw-rw-rw-   0        0        0      626 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe10k.dat
+-rw-rw-rw-   0        0        0      668 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe113.dat
+-rw-rw-rw-   0        0        0      721 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe114.dat
+-rw-rw-rw-   0        0        0      721 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe115.dat
+-rw-rw-rw-   0        0        0      721 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe116.dat
+-rw-rw-rw-   0        0        0      721 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe117.dat
+-rw-rw-rw-   0        0        0      721 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe118.dat
+-rw-rw-rw-   0        0        0      626 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe11k.dat
+-rw-rw-rw-   0        0        0      720 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe121.dat
+-rw-rw-rw-   0        0        0      720 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe122.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe123.dat
+-rw-rw-rw-   0        0        0      720 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe124.dat
+-rw-rw-rw-   0        0        0      626 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe12k.dat
+-rw-rw-rw-   0        0        0      721 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe133.dat
+-rw-rw-rw-   0        0        0      721 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe134.dat
+-rw-rw-rw-   0        0        0      721 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe137.dat
+-rw-rw-rw-   0        0        0      626 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe13k.dat
+-rw-rw-rw-   0        0        0      709 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe14.dat
+-rw-rw-rw-   0        0        0      721 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe140.dat
+-rw-rw-rw-   0        0        0     2107 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe142.dat
+-rw-rw-rw-   0        0        0      721 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe143.dat
+-rw-rw-rw-   0        0        0      721 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe144.dat
+-rw-rw-rw-   0        0        0      720 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe147.dat
+-rw-rw-rw-   0        0        0      626 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe14k.dat
+-rw-rw-rw-   0        0        0      709 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe15.dat
+-rw-rw-rw-   0        0        0      720 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe155.dat
+-rw-rw-rw-   0        0        0      626 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe15k.dat
+-rw-rw-rw-   0        0        0      722 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe164.dat
+-rw-rw-rw-   0        0        0      722 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe165.dat
+-rw-rw-rw-   0        0        0      728 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe167.dat
+-rw-rw-rw-   0        0        0      626 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe16k.dat
+-rw-rw-rw-   0        0        0      726 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe173.dat
+-rw-rw-rw-   0        0        0      726 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe174.dat
+-rw-rw-rw-   0        0        0      726 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe176.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe177.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe178.dat
+-rw-rw-rw-   0        0        0      721 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe180.dat
+-rw-rw-rw-   0        0        0      721 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe182.dat
+-rw-rw-rw-   0        0        0      721 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe184.dat
+-rw-rw-rw-   0        0        0      730 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe187.dat
+-rw-rw-rw-   0        0        0      730 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe188.dat
+-rw-rw-rw-   0        0        0      722 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe190.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe195.dat
+-rw-rw-rw-   0        0        0      724 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe198.dat
+-rw-rw-rw-   0        0        0      724 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe199.dat
+-rw-rw-rw-   0        0        0      723 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe207.dat
+-rw-rw-rw-   0        0        0      720 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe210.dat
+-rw-rw-rw-   0        0        0      722 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe217.dat
+-rw-rw-rw-   0        0        0      721 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe222.dat
+-rw-rw-rw-   0        0        0      721 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe223.dat
+-rw-rw-rw-   0        0        0      721 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe225.dat
+-rw-rw-rw-   0        0        0      721 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe226.dat
+-rw-rw-rw-   0        0        0      721 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe227.dat
+-rw-rw-rw-   0        0        0      721 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe228.dat
+-rw-rw-rw-   0        0        0      721 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe229.dat
+-rw-rw-rw-   0        0        0      720 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe233.dat
+-rw-rw-rw-   0        0        0      720 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe234.dat
+-rw-rw-rw-   0        0        0      725 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe235.dat
+-rw-rw-rw-   0        0        0      730 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe238.dat
+-rw-rw-rw-   0        0        0      721 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe239.dat
+-rw-rw-rw-   0        0        0      719 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe240.dat
+-rw-rw-rw-   0        0        0      721 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe241.dat
+-rw-rw-rw-   0        0        0      721 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe242.dat
+-rw-rw-rw-   0        0        0      721 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe243.dat
+-rw-rw-rw-   0        0        0      721 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe244.dat
+-rw-rw-rw-   0        0        0      721 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe255.dat
+-rw-rw-rw-   0        0        0      722 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe256.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe257.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe264.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe265.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe269.dat
+-rw-rw-rw-   0        0        0      722 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe274.dat
+-rw-rw-rw-   0        0        0      723 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe275.dat
+-rw-rw-rw-   0        0        0      724 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe276.dat
+-rw-rw-rw-   0        0        0      725 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe277.dat
+-rw-rw-rw-   0        0        0      723 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe278.dat
+-rw-rw-rw-   0        0        0      722 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe279.dat
+-rw-rw-rw-   0        0        0      723 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe280.dat
+-rw-rw-rw-   0        0        0      724 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe281.dat
+-rw-rw-rw-   0        0        0      725 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe282.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe284.dat
+-rw-rw-rw-   0        0        0      752 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe285.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe286.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe287.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe288.dat
+-rw-rw-rw-   0        0        0      720 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe289.dat
+-rw-rw-rw-   0        0        0      720 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe290.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe298.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe29b.dat
+-rw-rw-rw-   0        0        0      606 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe300.dat
+-rw-rw-rw-   0        0        0      733 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe301.dat
+-rw-rw-rw-   0        0        0      732 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe303.dat
+-rw-rw-rw-   0        0        0      732 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe304.dat
+-rw-rw-rw-   0        0        0      721 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe308.dat
+-rw-rw-rw-   0        0        0      721 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe309.dat
+-rw-rw-rw-   0        0        0      721 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe310.dat
+-rw-rw-rw-   0        0        0      721 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe311.dat
+-rw-rw-rw-   0        0        0      730 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe314.dat
+-rw-rw-rw-   0        0        0      736 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe315.dat
+-rw-rw-rw-   0        0        0      735 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe316.dat
+-rw-rw-rw-   0        0        0      735 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe318.dat
+-rw-rw-rw-   0        0        0      733 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe319.dat
+-rw-rw-rw-   0        0        0      735 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe320.dat
+-rw-rw-rw-   0        0        0      736 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe321.dat
+-rw-rw-rw-   0        0        0      735 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe322.dat
+-rw-rw-rw-   0        0        0      734 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe323.dat
+-rw-rw-rw-   0        0        0      730 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe324.dat
+-rw-rw-rw-   0        0        0      721 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe325.dat
+-rw-rw-rw-   0        0        0      721 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe326.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe328.dat
+-rw-rw-rw-   0        0        0      721 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe329.dat
+-rw-rw-rw-   0        0        0      721 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe330.dat
+-rw-rw-rw-   0        0        0      721 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe331.dat
+-rw-rw-rw-   0        0        0      721 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe332.dat
+-rw-rw-rw-   0        0        0      719 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe335.dat
+-rw-rw-rw-   0        0        0      721 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe336.dat
+-rw-rw-rw-   0        0        0      668 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe342.dat
+-rw-rw-rw-   0        0        0      721 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe344.dat
+-rw-rw-rw-   0        0        0      736 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe346.dat
+-rw-rw-rw-   0        0        0      584 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe358.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe359.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe360.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe361.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe362.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe363.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe364.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe365.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe366.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe367.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe368.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe369.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe370.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe371.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe372.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe373.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe374.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe375.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe376.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe377.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe379.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe380.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe381.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe382.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe383.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe384.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe385.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe386.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe387.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe388.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe389.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe390.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe391.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe392.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe393.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe394.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe395.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe396.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe397.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe398.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe399.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe400.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe401.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe402.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe403.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe404.dat
+-rw-rw-rw-   0        0        0      626 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe405.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe406.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe407.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe408.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe409.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe410.dat
+-rw-rw-rw-   0        0        0      668 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe411.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe412.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe413.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe414.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe415.dat
+-rw-rw-rw-   0        0        0      711 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe416a.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe417.dat
+-rw-rw-rw-   0        0        0      683 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe417a.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe418.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe419.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe420.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe421.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe422.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe423.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe424.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe425.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe426.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe427.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe428.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe429.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe430.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe431.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe432.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe433.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe434.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe435.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe436.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe437.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe438.dat
+-rw-rw-rw-   0        0        0      626 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe439.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe440.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe441.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe442.dat
+-rw-rw-rw-   0        0        0      626 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe443.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe444.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe445.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe446.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe447.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe448.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe449.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe450.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe451.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe456.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe457.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe458.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe459.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe460.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe462.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe464.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe474.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe476.dat
+-rw-rw-rw-   0        0        0      542 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe477.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe478.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe479.dat
+-rw-rw-rw-   0        0        0      542 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe480.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe481.dat
+-rw-rw-rw-   0        0        0      711 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe481a.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe482.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe483.dat
+-rw-rw-rw-   0        0        0      668 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe484.dat
+-rw-rw-rw-   0        0        0      668 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe488.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe490.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe491.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe492.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe493.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe494.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe495.dat
+-rw-rw-rw-   0        0        0      626 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe496.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe497.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe498.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe499.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe500.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe501.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe502.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe503.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe504.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe505.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe506.dat
+-rw-rw-rw-   0        0        0      542 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe507.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe508.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe509.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe510.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe511.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe512.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe513.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe514.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe515.dat
+-rw-rw-rw-   0        0        0      542 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe517.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe518.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe522.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe523.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe525.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe526.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe527.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe528.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe529.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe530.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe531.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe532.dat
+-rw-rw-rw-   0        0        0      668 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe533.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe534.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe535.dat
+-rw-rw-rw-   0        0        0      709 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe54.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe546.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe547.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe548.dat
+-rw-rw-rw-   0        0        0      878 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe549.dat
+-rw-rw-rw-   0        0        0      709 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe55.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe550.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe553.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe559.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe561.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe562.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe563.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe564.dat
+-rw-rw-rw-   0        0        0      668 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe565.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe566.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe567.dat
+-rw-rw-rw-   0        0        0      709 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe57.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe570.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe571.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe572.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe573.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe574.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe575.dat
+-rw-rw-rw-   0        0        0      542 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe584.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe585.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe587.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe590.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe591.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe592.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe593.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe595.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe596.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe598.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe599.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe600.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe601.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe602.dat
+-rw-rw-rw-   0        0        0      715 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe602m.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe604.dat
+-rw-rw-rw-   0        0        0      670 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe610b.dat
+-rw-rw-rw-   0        0        0      633 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe610bm.dat
+-rw-rw-rw-   0        0        0      668 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe611.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe612.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe613.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe614.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe615.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe617.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe619.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe620.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe621.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe622.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe623.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe624.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe625.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe626.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe627.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe628.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe629.dat
+-rw-rw-rw-   0        0        0      709 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe63.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe630.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe632.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe633.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe645.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe646.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe647.dat
+-rw-rw-rw-   0        0        0      731 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe648.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe650.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe652.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe654.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe655.dat
+-rw-rw-rw-   0        0        0      626 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe670.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe673.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe675.dat
+-rw-rw-rw-   0        0        0      719 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe676.dat
+-rw-rw-rw-   0        0        0      718 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe677.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe679.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe681.dat
+-rw-rw-rw-   0        0        0      626 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe682.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe683.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe685.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe692.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe693.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe701.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe702.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe703.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe704.dat
+-rw-rw-rw-   0        0        0      668 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe711.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe723.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe735.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe738.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe741.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe744.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe746.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe758.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe766.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe767.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe769.dat
+-rw-rw-rw-   0        0        0      668 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe770.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe775.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe776.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe777.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe780.dat
+-rw-rw-rw-   0        0        0      720 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe79.dat
+-rw-rw-rw-   0        0        0     2054 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe795.dat
+-rw-rw-rw-   0        0        0     1466 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe795sm.dat
+-rw-rw-rw-   0        0        0      878 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe796.dat
+-rw-rw-rw-   0        0        0      584 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe797.dat
+-rw-rw-rw-   0        0        0      668 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe798.dat
+-rw-rw-rw-   0        0        0      720 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe801.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe802.dat
+-rw-rw-rw-   0        0        0      880 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe802a.dat
+-rw-rw-rw-   0        0        0      985 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe802b.dat
+-rw-rw-rw-   0        0        0      849 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe803h.dat
+-rw-rw-rw-   0        0        0      675 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe804.dat
+-rw-rw-rw-   0        0        0      709 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe81.dat
+-rw-rw-rw-   0        0        0      709 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/goe92.dat
+-rw-rw-rw-   0        0        0     2074 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/griffith30SymSuction.dat
+-rw-rw-rw-   0        0        0      674 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/gs1.dat
+-rw-rw-rw-   0        0        0      771 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/gu255118.dat
+-rw-rw-rw-   0        0        0     1658 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/hh02.dat
+-rw-rw-rw-   0        0        0      602 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/hobie.dat
+-rw-rw-rw-   0        0        0     1428 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/hobiesm.dat
+-rw-rw-rw-   0        0        0     2054 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/hq010.dat
+-rw-rw-rw-   0        0        0     2053 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/hq07.dat
+-rw-rw-rw-   0        0        0     2053 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/hq09.dat
+-rw-rw-rw-   0        0        0     1636 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/hq1010.dat
+-rw-rw-rw-   0        0        0     1636 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/hq1012.dat
+-rw-rw-rw-   0        0        0     1635 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/hq108.dat
+-rw-rw-rw-   0        0        0     1635 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/hq109.dat
+-rw-rw-rw-   0        0        0     1636 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/hq1510.dat
+-rw-rw-rw-   0        0        0     2056 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/hq1511.dat
+-rw-rw-rw-   0        0        0     1636 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/hq1512.dat
+-rw-rw-rw-   0        0        0     1635 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/hq158.dat
+-rw-rw-rw-   0        0        0      839 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/hq1585.dat
+-rw-rw-rw-   0        0        0     1635 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/hq159.dat
+-rw-rw-rw-   0        0        0     1049 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/hq159b.dat
+-rw-rw-rw-   0        0        0     1636 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/hq2010.dat
+-rw-rw-rw-   0        0        0     1636 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/hq2012.dat
+-rw-rw-rw-   0        0        0     1635 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/hq208.dat
+-rw-rw-rw-   0        0        0     1635 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/hq209.dat
+-rw-rw-rw-   0        0        0      797 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/hq2090sm.dat
+-rw-rw-rw-   0        0        0     1133 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/hq2195.dat
+-rw-rw-rw-   0        0        0     1636 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/hq2510.dat
+-rw-rw-rw-   0        0        0     2056 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/hq2511.dat
+-rw-rw-rw-   0        0        0     1636 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/hq2512.dat
+-rw-rw-rw-   0        0        0     1635 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/hq258.dat
+-rw-rw-rw-   0        0        0     1635 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/hq259.dat
+-rw-rw-rw-   0        0        0      933 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/hq2590sm.dat
+-rw-rw-rw-   0        0        0     1133 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/hq259b.dat
+-rw-rw-rw-   0        0        0     1727 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/hq300gd2.dat
+-rw-rw-rw-   0        0        0     1636 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/hq3010.dat
+-rw-rw-rw-   0        0        0     1636 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/hq3011.dat
+-rw-rw-rw-   0        0        0     1636 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/hq3012.dat
+-rw-rw-rw-   0        0        0     1636 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/hq3013.dat
+-rw-rw-rw-   0        0        0     1636 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/hq3014.dat
+-rw-rw-rw-   0        0        0     1636 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/hq3015.dat
+-rw-rw-rw-   0        0        0     1635 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/hq308.dat
+-rw-rw-rw-   0        0        0     1635 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/hq309.dat
+-rw-rw-rw-   0        0        0     1636 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/hq3510.dat
+-rw-rw-rw-   0        0        0     1636 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/hq3512.dat
+-rw-rw-rw-   0        0        0     1636 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/hq3513.dat
+-rw-rw-rw-   0        0        0      838 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/hq3514.dat
+-rw-rw-rw-   0        0        0      838 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/hq3518.dat
+-rw-rw-rw-   0        0        0     1635 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/hq358.dat
+-rw-rw-rw-   0        0        0     1635 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/hq359.dat
+-rw-rw-rw-   0        0        0     2522 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/hsnlf213.dat
+-rw-rw-rw-   0        0        0     4839 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ht05.dat
+-rw-rw-rw-   0        0        0     4326 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ht08.dat
+-rw-rw-rw-   0        0        0     3813 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ht12.dat
+-rw-rw-rw-   0        0        0     3867 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ht22.dat
+-rw-rw-rw-   0        0        0     3867 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ht23.dat
+-rw-rw-rw-   0        0        0      639 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/isa571.dat
+-rw-rw-rw-   0        0        0      639 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/isa960.dat
+-rw-rw-rw-   0        0        0      639 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/isa961.dat
+-rw-rw-rw-   0        0        0      639 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/isa962.dat
+-rw-rw-rw-   0        0        0     1359 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/j5012.dat
+-rw-rw-rw-   0        0        0     2537 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/jn153.dat
+-rw-rw-rw-   0        0        0     1934 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/joukowsk.dat
+-rw-rw-rw-   0        0        0     3575 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/k1.dat
+-rw-rw-rw-   0        0        0     3759 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/k2.dat
+-rw-rw-rw-   0        0        0     3864 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/k3.dat
+-rw-rw-rw-   0        0        0     1487 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/k3311.dat
+-rw-rw-rw-   0        0        0     2230 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/k3311sm.dat
+-rw-rw-rw-   0        0        0     1095 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/kc135a.dat
+-rw-rw-rw-   0        0        0     1096 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/kc135b.dat
+-rw-rw-rw-   0        0        0     1096 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/kc135c.dat
+-rw-rw-rw-   0        0        0     1095 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/kc135d.dat
+-rw-rw-rw-   0        0        0     2151 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/kenmar.dat
+-rw-rw-rw-   0        0        0     1941 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/l188root.dat
+-rw-rw-rw-   0        0        0     1940 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/l188tip.dat
+-rw-rw-rw-   0        0        0      717 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/l7769.dat
+-rw-rw-rw-   0        0        0     1943 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/la203a.dat
+-rw-rw-rw-   0        0        0     2684 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/la2573a.dat
+-rw-rw-rw-   0        0        0     1125 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/lds2.dat
+-rw-rw-rw-   0        0        0     1590 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/lg10sc.dat
+-rw-rw-rw-   0        0        0     2030 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/lnv109a.dat
+-rw-rw-rw-   0        0        0     1897 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/lrn1007.dat
+-rw-rw-rw-   0        0        0     1003 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ls013.dat
+-rw-rw-rw-   0        0        0     1428 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ls413.dat
+-rw-rw-rw-   0        0        0     1405 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ls413mod.dat
+-rw-rw-rw-   0        0        0     1211 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ls417.dat
+-rw-rw-rw-   0        0        0     1463 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ls417mod.dat
+-rw-rw-rw-   0        0        0     1200 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ls421.dat
+-rw-rw-rw-   0        0        0     1421 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ls421mod.dat
+-rw-rw-rw-   0        0        0     2096 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/lwk79100.dat
+-rw-rw-rw-   0        0        0     2096 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/lwk80080.dat
+-rw-rw-rw-   0        0        0     2096 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/lwk80100.dat
+-rw-rw-rw-   0        0        0     2100 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/lwk80120k25.dat
+-rw-rw-rw-   0        0        0     2100 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/lwk80150k25.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/m1.dat
+-rw-rw-rw-   0        0        0      711 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/m10.dat
+-rw-rw-rw-   0        0        0      711 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/m11.dat
+-rw-rw-rw-   0        0        0      711 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/m12.dat
+-rw-rw-rw-   0        0        0      711 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/m13.dat
+-rw-rw-rw-   0        0        0      711 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/m14.dat
+-rw-rw-rw-   0        0        0      711 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/m15.dat
+-rw-rw-rw-   0        0        0      711 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/m16.dat
+-rw-rw-rw-   0        0        0      711 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/m17.dat
+-rw-rw-rw-   0        0        0      711 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/m18.dat
+-rw-rw-rw-   0        0        0      711 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/m19.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/m2.dat
+-rw-rw-rw-   0        0        0      711 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/m20.dat
+-rw-rw-rw-   0        0        0      711 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/m21.dat
+-rw-rw-rw-   0        0        0      711 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/m22.dat
+-rw-rw-rw-   0        0        0      711 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/m23.dat
+-rw-rw-rw-   0        0        0      711 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/m24.dat
+-rw-rw-rw-   0        0        0      711 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/m25.dat
+-rw-rw-rw-   0        0        0      711 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/m26.dat
+-rw-rw-rw-   0        0        0      711 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/m27.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/m3.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/m4.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/m5.dat
+-rw-rw-rw-   0        0        0      660 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/m6.dat
+-rw-rw-rw-   0        0        0      767 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/m665.dat
+-rw-rw-rw-   0        0        0      767 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/m685.dat
+-rw-rw-rw-   0        0        0      668 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/m7.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/m8.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/m9.dat
+-rw-rw-rw-   0        0        0      920 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ma409.dat
+-rw-rw-rw-   0        0        0     2230 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ma409sm.dat
+-rw-rw-rw-   0        0        0     2177 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/marsden.dat
+-rw-rw-rw-   0        0        0      674 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/marske1.dat
+-rw-rw-rw-   0        0        0      696 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/marske2.dat
+-rw-rw-rw-   0        0        0      703 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/marske3.dat
+-rw-rw-rw-   0        0        0      701 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/marske4.dat
+-rw-rw-rw-   0        0        0      680 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/marske5.dat
+-rw-rw-rw-   0        0        0     1528 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/marske7.dat
+-rw-rw-rw-   0        0        0     1427 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/mb253515sm.dat
+-rw-rw-rw-   0        0        0     1785 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/mh102.dat
+-rw-rw-rw-   0        0        0     1759 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/mh104.dat
+-rw-rw-rw-   0        0        0     1785 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/mh106.dat
+-rw-rw-rw-   0        0        0     1785 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/mh108.dat
+-rw-rw-rw-   0        0        0     1785 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/mh110.dat
+-rw-rw-rw-   0        0        0     1603 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/mh112.dat
+-rw-rw-rw-   0        0        0     1603 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/mh113.dat
+-rw-rw-rw-   0        0        0     1785 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/mh114.dat
+-rw-rw-rw-   0        0        0     1785 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/mh115.dat
+-rw-rw-rw-   0        0        0     1758 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/mh116.dat
+-rw-rw-rw-   0        0        0     1783 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/mh117.dat
+-rw-rw-rw-   0        0        0     1603 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/mh120.dat
+-rw-rw-rw-   0        0        0     1784 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/mh121.dat
+-rw-rw-rw-   0        0        0     1784 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/mh122.dat
+-rw-rw-rw-   0        0        0     1603 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/mh150.dat
+-rw-rw-rw-   0        0        0     1758 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/mh18.dat
+-rw-rw-rw-   0        0        0     1783 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/mh20.dat
+-rw-rw-rw-   0        0        0     1785 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/mh200.dat
+-rw-rw-rw-   0        0        0     1759 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/mh201.dat
+-rw-rw-rw-   0        0        0     1782 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/mh22.dat
+-rw-rw-rw-   0        0        0     1780 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/mh23.dat
+-rw-rw-rw-   0        0        0     1783 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/mh24.dat
+-rw-rw-rw-   0        0        0     1757 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/mh25.dat
+-rw-rw-rw-   0        0        0     1758 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/mh26.dat
+-rw-rw-rw-   0        0        0     1784 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/mh27.dat
+-rw-rw-rw-   0        0        0     1757 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/mh30.dat
+-rw-rw-rw-   0        0        0     1782 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/mh32.dat
+-rw-rw-rw-   0        0        0     1783 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/mh38.dat
+-rw-rw-rw-   0        0        0     1757 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/mh42.dat
+-rw-rw-rw-   0        0        0     1782 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/mh43.dat
+-rw-rw-rw-   0        0        0     1783 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/mh44.dat
+-rw-rw-rw-   0        0        0     1757 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/mh45.dat
+-rw-rw-rw-   0        0        0     1782 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/mh46.dat
+-rw-rw-rw-   0        0        0     1203 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/mh49.dat
+-rw-rw-rw-   0        0        0     1784 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/mh60.dat
+-rw-rw-rw-   0        0        0     1784 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/mh61.dat
+-rw-rw-rw-   0        0        0     1782 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/mh62.dat
+-rw-rw-rw-   0        0        0     1783 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/mh64.dat
+-rw-rw-rw-   0        0        0     1784 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/mh70.dat
+-rw-rw-rw-   0        0        0     1758 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/mh78.dat
+-rw-rw-rw-   0        0        0     1784 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/mh80.dat
+-rw-rw-rw-   0        0        0     1755 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/mh81.dat
+-rw-rw-rw-   0        0        0     1784 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/mh82.dat
+-rw-rw-rw-   0        0        0     1602 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/mh83.dat
+-rw-rw-rw-   0        0        0     1758 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/mh84.dat
+-rw-rw-rw-   0        0        0     1784 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/mh91.dat
+-rw-rw-rw-   0        0        0     1784 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/mh92.dat
+-rw-rw-rw-   0        0        0     1784 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/mh93.dat
+-rw-rw-rw-   0        0        0     1784 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/mh94.dat
+-rw-rw-rw-   0        0        0     1602 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/mh95.dat
+-rw-rw-rw-   0        0        0     1174 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/miley.dat
+-rw-rw-rw-   0        0        0     2768 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/mrc-16.dat
+-rw-rw-rw-   0        0        0     2768 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/mrc-20.dat
+-rw-rw-rw-   0        0        0     1507 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ms313.dat
+-rw-rw-rw-   0        0        0     1417 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ms317.dat
+-rw-rw-rw-   0        0        0     2093 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/mue139.dat
+-rw-rw-rw-   0        0        0     1395 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/n0009sm.dat
+-rw-rw-rw-   0        0        0     1583 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/n0011sc.dat
+-rw-rw-rw-   0        0        0     2772 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/n0012.dat
+-rw-rw-rw-   0        0        0      633 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/n10.dat
+-rw-rw-rw-   0        0        0      633 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/n11.dat
+-rw-rw-rw-   0        0        0      799 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/n11h9.dat
+-rw-rw-rw-   0        0        0      648 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/n12.dat
+-rw-rw-rw-   0        0        0      648 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/n13.dat
+-rw-rw-rw-   0        0        0      648 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/n14.dat
+-rw-rw-rw-   0        0        0      756 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/n1h15.dat
+-rw-rw-rw-   0        0        0      633 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/n22.dat
+-rw-rw-rw-   0        0        0      633 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/n24.dat
+-rw-rw-rw-   0        0        0     1170 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/n2414.dat
+-rw-rw-rw-   0        0        0     1170 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/n2415.dat
+-rw-rw-rw-   0        0        0      756 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/n2h15.dat
+-rw-rw-rw-   0        0        0      756 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/n5h10.dat
+-rw-rw-rw-   0        0        0      756 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/n5h15.dat
+-rw-rw-rw-   0        0        0      756 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/n5h20.dat
+-rw-rw-rw-   0        0        0     1015 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/n63010a.dat
+-rw-rw-rw-   0        0        0     1016 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/n63012a.dat
+-rw-rw-rw-   0        0        0     1016 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/n63015a.dat
+-rw-rw-rw-   0        0        0     1013 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/n63210.dat
+-rw-rw-rw-   0        0        0     1013 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/n63212.dat
+-rw-rw-rw-   0        0        0     1013 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/n63215.dat
+-rw-rw-rw-   0        0        0     1803 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/n63215b.dat
+-rw-rw-rw-   0        0        0     1011 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/n63412.dat
+-rw-rw-rw-   0        0        0     1012 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/n63415.dat
+-rw-rw-rw-   0        0        0     1016 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/n64008a.dat
+-rw-rw-rw-   0        0        0     1022 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/n64012.dat
+-rw-rw-rw-   0        0        0     1016 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/n64012a.dat
+-rw-rw-rw-   0        0        0      991 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/n64015.dat
+-rw-rw-rw-   0        0        0     1017 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/n64015a.dat
+-rw-rw-rw-   0        0        0     1242 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/n6409.dat
+-rw-rw-rw-   0        0        0     1014 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/n64108.dat
+-rw-rw-rw-   0        0        0     1014 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/n64110.dat
+-rw-rw-rw-   0        0        0     1089 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/n64212.dat
+-rw-rw-rw-   0        0        0     1221 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/n64212ma.dat
+-rw-rw-rw-   0        0        0      906 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/n64212mb.dat
+-rw-rw-rw-   0        0        0     1014 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/n64215.dat
+-rw-rw-rw-   0        0        0      770 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/n642415.dat
+-rw-rw-rw-   0        0        0     1014 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/n66021.dat
+-rw-rw-rw-   0        0        0      756 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/n6h10.dat
+-rw-rw-rw-   0        0        0      756 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/n6h15.dat
+-rw-rw-rw-   0        0        0      756 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/n6h20.dat
+-rw-rw-rw-   0        0        0      777 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/n8h12.dat
+-rw-rw-rw-   0        0        0      632 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/n9.dat
+-rw-rw-rw-   0        0        0      728 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/naca0006.dat
+-rw-rw-rw-   0        0        0      728 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/naca0008.dat
+-rw-rw-rw-   0        0        0      690 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/naca000834.dat
+-rw-rw-rw-   0        0        0      728 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/naca0010.dat
+-rw-rw-rw-   0        0        0      690 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/naca001034.dat
+-rw-rw-rw-   0        0        0      782 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/naca001034a08cli0.2.dat
+-rw-rw-rw-   0        0        0      690 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/naca001035.dat
+-rw-rw-rw-   0        0        0      690 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/naca001064.dat
+-rw-rw-rw-   0        0        0      690 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/naca001065.dat
+-rw-rw-rw-   0        0        0      690 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/naca001066.dat
+-rw-rw-rw-   0        0        0      690 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/naca001234.dat
+-rw-rw-rw-   0        0        0      690 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/naca001264.dat
+-rw-rw-rw-   0        0        0      739 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/naca001264a08cli0.2.dat
+-rw-rw-rw-   0        0        0      728 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/naca0015.dat
+-rw-rw-rw-   0        0        0      728 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/naca0018.dat
+-rw-rw-rw-   0        0        0      728 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/naca0021.dat
+-rw-rw-rw-   0        0        0      728 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/naca0024.dat
+-rw-rw-rw-   0        0        0     1609 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/naca1.dat
+-rw-rw-rw-   0        0        0      763 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/naca1408.dat
+-rw-rw-rw-   0        0        0      763 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/naca1410.dat
+-rw-rw-rw-   0        0        0      763 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/naca1412.dat
+-rw-rw-rw-   0        0        0      689 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/naca16006.dat
+-rw-rw-rw-   0        0        0     2097 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/naca16009.dat
+-rw-rw-rw-   0        0        0      689 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/naca16012.dat
+-rw-rw-rw-   0        0        0      689 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/naca16015.dat
+-rw-rw-rw-   0        0        0      689 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/naca16018.dat
+-rw-rw-rw-   0        0        0      689 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/naca16021.dat
+-rw-rw-rw-   0        0        0     1300 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/naca23012.dat
+-rw-rw-rw-   0        0        0      755 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/naca23015.dat
+-rw-rw-rw-   0        0        0      755 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/naca23018.dat
+-rw-rw-rw-   0        0        0      755 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/naca23021.dat
+-rw-rw-rw-   0        0        0      763 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/naca23024.dat
+-rw-rw-rw-   0        0        0      763 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/naca2408.dat
+-rw-rw-rw-   0        0        0      763 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/naca2410.dat
+-rw-rw-rw-   0        0        0     1240 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/naca2411.dat
+-rw-rw-rw-   0        0        0      754 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/naca2415.dat
+-rw-rw-rw-   0        0        0      754 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/naca2418.dat
+-rw-rw-rw-   0        0        0      754 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/naca2421.dat
+-rw-rw-rw-   0        0        0      762 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/naca2424.dat
+-rw-rw-rw-   0        0        0      734 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/naca4412.dat
+-rw-rw-rw-   0        0        0     2095 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/naca4415.dat
+-rw-rw-rw-   0        0        0      754 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/naca4418.dat
+-rw-rw-rw-   0        0        0      754 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/naca4421.dat
+-rw-rw-rw-   0        0        0      762 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/naca4424.dat
+-rw-rw-rw-   0        0        0     1106 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/naca63206.dat
+-rw-rw-rw-   0        0        0     1107 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/naca63209.dat
+-rw-rw-rw-   0        0        0     1107 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/naca632615.dat
+-rw-rw-rw-   0        0        0     2101 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/naca632a015.dat
+-rw-rw-rw-   0        0        0     2100 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/naca633018.dat
+-rw-rw-rw-   0        0        0     1111 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/naca633218.dat
+-rw-rw-rw-   0        0        0     2089 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/naca633418.dat
+-rw-rw-rw-   0        0        0     1108 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/naca633618.dat
+-rw-rw-rw-   0        0        0     1111 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/naca634221.dat
+-rw-rw-rw-   0        0        0     1110 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/naca634421.dat
+-rw-rw-rw-   0        0        0     1130 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/naca63a210.dat
+-rw-rw-rw-   0        0        0     1111 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/naca641112.dat
+-rw-rw-rw-   0        0        0     1499 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/naca6412.dat
+-rw-rw-rw-   0        0        0     1106 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/naca64206.dat
+-rw-rw-rw-   0        0        0     1107 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/naca64208.dat
+-rw-rw-rw-   0        0        0     1107 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/naca64209.dat
+-rw-rw-rw-   0        0        0     1107 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/naca64210.dat
+-rw-rw-rw-   0        0        0     1111 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/naca642215.dat
+-rw-rw-rw-   0        0        0     1109 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/naca642415.dat
+-rw-rw-rw-   0        0        0     1111 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/naca643218.dat
+-rw-rw-rw-   0        0        0     1088 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/naca643418.dat
+-rw-rw-rw-   0        0        0     1108 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/naca643618.dat
+-rw-rw-rw-   0        0        0     1111 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/naca644221.dat
+-rw-rw-rw-   0        0        0     1110 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/naca644421.dat
+-rw-rw-rw-   0        0        0     3574 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/naca64a010.dat
+-rw-rw-rw-   0        0        0     1109 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/naca64a210.dat
+-rw-rw-rw-   0        0        0     1109 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/naca64a410.dat
+-rw-rw-rw-   0        0        0     1111 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/naca651212.dat
+-rw-rw-rw-   0        0        0     1117 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/naca651212a06.dat
+-rw-rw-rw-   0        0        0     1065 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/naca651412.dat
+-rw-rw-rw-   0        0        0     1106 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/naca65206.dat
+-rw-rw-rw-   0        0        0     1107 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/naca65209.dat
+-rw-rw-rw-   0        0        0     1107 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/naca65210.dat
+-rw-rw-rw-   0        0        0     1111 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/naca652215.dat
+-rw-rw-rw-   0        0        0     1110 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/naca652415.dat
+-rw-rw-rw-   0        0        0     1117 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/naca652415a05.dat
+-rw-rw-rw-   0        0        0     1111 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/naca653218.dat
+-rw-rw-rw-   0        0        0     1106 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/naca65410.dat
+-rw-rw-rw-   0        0        0     1111 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/naca654221.dat
+-rw-rw-rw-   0        0        0     1110 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/naca654421.dat
+-rw-rw-rw-   0        0        0     1117 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/naca654421a05.dat
+-rw-rw-rw-   0        0        0     1429 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/naca66-018.dat
+-rw-rw-rw-   0        0        0     1111 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/naca661212.dat
+-rw-rw-rw-   0        0        0     1107 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/naca66206.dat
+-rw-rw-rw-   0        0        0     1108 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/naca66209.dat
+-rw-rw-rw-   0        0        0     1108 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/naca66210.dat
+-rw-rw-rw-   0        0        0     1111 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/naca662215.dat
+-rw-rw-rw-   0        0        0     1110 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/naca662415.dat
+-rw-rw-rw-   0        0        0     1111 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/naca663218.dat
+-rw-rw-rw-   0        0        0     1111 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/naca663418.dat
+-rw-rw-rw-   0        0        0     1111 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/naca664221.dat
+-rw-rw-rw-   0        0        0     1110 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/naca671215.dat
+-rw-rw-rw-   0        0        0     1109 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/naca747a315.dat
+-rw-rw-rw-   0        0        0     1109 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/naca747a415.dat
+-rw-rw-rw-   0        0        0      637 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/nacacyh.dat
+-rw-rw-rw-   0        0        0      653 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/nacam12.dat
+-rw-rw-rw-   0        0        0      637 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/nacam18.dat
+-rw-rw-rw-   0        0        0      652 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/nacam2.dat
+-rw-rw-rw-   0        0        0      652 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/nacam3.dat
+-rw-rw-rw-   0        0        0      690 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/nacam6.dat
+-rw-rw-rw-   0        0        0     1686 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/nasasc2-0714.dat
+-rw-rw-rw-   0        0        0     1687 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ncambre.dat
+-rw-rw-rw-   0        0        0     2326 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/nl722343.dat
+-rw-rw-rw-   0        0        0     2258 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/nl722362.dat
+-rw-rw-rw-   0        0        0     1174 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/nlf0115.dat
+-rw-rw-rw-   0        0        0      974 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/nlf0215f.dat
+-rw-rw-rw-   0        0        0     1357 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/nlf1015.dat
+-rw-rw-rw-   0        0        0     1754 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/nlf414f.dat
+-rw-rw-rw-   0        0        0     2786 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/nlf415.dat
+-rw-rw-rw-   0        0        0      990 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/nlf416.dat
+-rw-rw-rw-   0        0        0     1146 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/nlr1t.dat
+-rw-rw-rw-   0        0        0     1627 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/nlr7301.dat
+-rw-rw-rw-   0        0        0     2080 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/nn7mk20.dat
+-rw-rw-rw-   0        0        0     2128 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/npl9510.dat
+-rw-rw-rw-   0        0        0     2224 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/npl9615.dat
+-rw-rw-rw-   0        0        0     1762 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/npl9626.dat
+-rw-rw-rw-   0        0        0     1762 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/npl9627.dat
+-rw-rw-rw-   0        0        0     2392 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/npl9660.dat
+-rw-rw-rw-   0        0        0     1336 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/nplx.dat
+-rw-rw-rw-   0        0        0     2395 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/oa206.dat
+-rw-rw-rw-   0        0        0     2395 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/oa209.dat
+-rw-rw-rw-   0        0        0     2395 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/oa212.dat
+-rw-rw-rw-   0        0        0     2395 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/oa213.dat
+-rw-rw-rw-   0        0        0     2137 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/oaf095.dat
+-rw-rw-rw-   0        0        0     2137 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/oaf102.dat
+-rw-rw-rw-   0        0        0     2137 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/oaf117.dat
+-rw-rw-rw-   0        0        0     2137 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/oaf128.dat
+-rw-rw-rw-   0        0        0     2137 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/oaf139.dat
+-rw-rw-rw-   0        0        0      890 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/p51droot.dat
+-rw-rw-rw-   0        0        0      888 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/p51dtip.dat
+-rw-rw-rw-   0        0        0     1934 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/p51hroot.dat
+-rw-rw-rw-   0        0        0     1931 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/p51htip.dat
+-rw-rw-rw-   0        0        0     1031 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/pfcm.dat
+-rw-rw-rw-   0        0        0     1916 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/pmc19sm.dat
+-rw-rw-rw-   0        0        0     1815 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/prandtldroot.dat
+-rw-rw-rw-   0        0        0     2694 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/prandtldtip.dat
+-rw-rw-rw-   0        0        0     1234 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/psu-90-125wl.dat
+-rw-rw-rw-   0        0        0     1183 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/psu94097.dat
+-rw-rw-rw-   0        0        0     2063 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/pt40.dat
+-rw-rw-rw-   0        0        0     2535 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/r1046.dat
+-rw-rw-rw-   0        0        0     2542 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/r1080.dat
+-rw-rw-rw-   0        0        0     2547 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/r1082.dat
+-rw-rw-rw-   0        0        0     2547 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/r1082t.dat
+-rw-rw-rw-   0        0        0     2156 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/r140.dat
+-rw-rw-rw-   0        0        0     2071 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/r140sm.dat
+-rw-rw-rw-   0        0        0     3350 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/rae100.dat
+-rw-rw-rw-   0        0        0     3350 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/rae101.dat
+-rw-rw-rw-   0        0        0     3350 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/rae102.dat
+-rw-rw-rw-   0        0        0     3350 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/rae103.dat
+-rw-rw-rw-   0        0        0     3350 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/rae104.dat
+-rw-rw-rw-   0        0        0     2470 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/rae2822.dat
+-rw-rw-rw-   0        0        0     1471 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/rae5212.dat
+-rw-rw-rw-   0        0        0     1468 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/rae5213.dat
+-rw-rw-rw-   0        0        0     1463 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/rae5214.dat
+-rw-rw-rw-   0        0        0     1463 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/rae5215.dat
+-rw-rw-rw-   0        0        0     2521 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/rae69ck.dat
+-rw-rw-rw-   0        0        0      667 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/raf15.dat
+-rw-rw-rw-   0        0        0      709 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/raf19.dat
+-rw-rw-rw-   0        0        0      709 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/raf25.dat
+-rw-rw-rw-   0        0        0      709 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/raf26.dat
+-rw-rw-rw-   0        0        0      709 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/raf27.dat
+-rw-rw-rw-   0        0        0      709 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/raf28.dat
+-rw-rw-rw-   0        0        0      667 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/raf30.dat
+-rw-rw-rw-   0        0        0      629 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/raf30md.dat
+-rw-rw-rw-   0        0        0      751 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/raf31.dat
+-rw-rw-rw-   0        0        0      541 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/raf32.dat
+-rw-rw-rw-   0        0        0      629 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/raf32md.dat
+-rw-rw-rw-   0        0        0      709 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/raf33.dat
+-rw-rw-rw-   0        0        0      709 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/raf34.dat
+-rw-rw-rw-   0        0        0      541 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/raf38.dat
+-rw-rw-rw-   0        0        0      658 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/raf48.dat
+-rw-rw-rw-   0        0        0      540 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/raf6.dat
+-rw-rw-rw-   0        0        0      541 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/raf69.dat
+-rw-rw-rw-   0        0        0      541 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/raf89.dat
+-rw-rw-rw-   0        0        0     1197 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/rc0864c.dat
+-rw-rw-rw-   0        0        0     1268 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/rc08b3.dat
+-rw-rw-rw-   0        0        0     1776 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/rc08n1.dat
+-rw-rw-rw-   0        0        0     1129 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/rc1064c.dat
+-rw-rw-rw-   0        0        0     1268 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/rc10b3.dat
+-rw-rw-rw-   0        0        0     1776 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/rc10n1.dat
+-rw-rw-rw-   0        0        0      925 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/rc1264c.dat
+-rw-rw-rw-   0        0        0     1268 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/rc12b3.dat
+-rw-rw-rw-   0        0        0     1776 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/rc12n1.dat
+-rw-rw-rw-   0        0        0     1755 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/rc410.dat
+-rw-rw-rw-   0        0        0     1755 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/rc510.dat
+-rw-rw-rw-   0        0        0     1280 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/rcsc2.dat
+-rw-rw-rw-   0        0        0     2177 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/rg12.dat
+-rw-rw-rw-   0        0        0     1274 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/rg12a.dat
+-rw-rw-rw-   0        0        0     1347 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/rg12a189.dat
+-rw-rw-rw-   0        0        0     1317 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/rg14.dat
+-rw-rw-rw-   0        0        0     1258 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/rg1410.dat
+-rw-rw-rw-   0        0        0     1257 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/rg149.dat
+-rw-rw-rw-   0        0        0     1259 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/rg1495.dat
+-rw-rw-rw-   0        0        0     1347 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/rg14a147.dat
+-rw-rw-rw-   0        0        0     1242 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/rg15.dat
+-rw-rw-rw-   0        0        0     1348 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/rg15a111.dat
+-rw-rw-rw-   0        0        0     1348 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/rg15a213.dat
+-rw-rw-rw-   0        0        0     1295 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/rg8.dat
+-rw-rw-rw-   0        0        0      648 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/rhodesg30.dat
+-rw-rw-rw-   0        0        0      648 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/rhodesg32.dat
+-rw-rw-rw-   0        0        0      648 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/rhodesg34.dat
+-rw-rw-rw-   0        0        0      648 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/rhodesg36.dat
+-rw-rw-rw-   0        0        0     1483 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/s1010.dat
+-rw-rw-rw-   0        0        0     1471 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/s1012.dat
+-rw-rw-rw-   0        0        0     1471 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/s1014.dat
+-rw-rw-rw-   0        0        0     1471 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/s1016.dat
+-rw-rw-rw-   0        0        0     1493 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/s1020.dat
+-rw-rw-rw-   0        0        0     1741 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/s1046.dat
+-rw-rw-rw-   0        0        0     1741 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/s1048.dat
+-rw-rw-rw-   0        0        0     2275 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/s1091.dat
+-rw-rw-rw-   0        0        0     2287 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/s1210.dat
+-rw-rw-rw-   0        0        0     2927 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/s1221.dat
+-rw-rw-rw-   0        0        0     6612 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/s1223.dat
+-rw-rw-rw-   0        0        0     3411 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/s1223rtl.dat
+-rw-rw-rw-   0        0        0     1125 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/s2027.dat
+-rw-rw-rw-   0        0        0     1125 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/s2046.dat
+-rw-rw-rw-   0        0        0     1291 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/s2048.dat
+-rw-rw-rw-   0        0        0     1843 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/s2050.dat
+-rw-rw-rw-   0        0        0     1291 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/s2055.dat
+-rw-rw-rw-   0        0        0     1479 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/s2060.dat
+-rw-rw-rw-   0        0        0     1479 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/s2062.dat
+-rw-rw-rw-   0        0        0     1294 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/s2091.dat
+-rw-rw-rw-   0        0        0      742 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/s3.dat
+-rw-rw-rw-   0        0        0     1057 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/s3002.dat
+-rw-rw-rw-   0        0        0     1051 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/s3010.dat
+-rw-rw-rw-   0        0        0     1232 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/s3014.dat
+-rw-rw-rw-   0        0        0     1053 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/s3016.dat
+-rw-rw-rw-   0        0        0     1294 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/s3021.dat
+-rw-rw-rw-   0        0        0     1240 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/s3024.dat
+-rw-rw-rw-   0        0        0     1176 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/s3025.dat
+-rw-rw-rw-   0        0        0     1123 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/s4022.dat
+-rw-rw-rw-   0        0        0     1123 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/s4053.dat
+-rw-rw-rw-   0        0        0     1294 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/s4061.dat
+-rw-rw-rw-   0        0        0     1051 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/s4062.dat
+-rw-rw-rw-   0        0        0     2280 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/s4083.dat
+-rw-rw-rw-   0        0        0     1123 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/s4110.dat
+-rw-rw-rw-   0        0        0     1123 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/s4158.dat
+-rw-rw-rw-   0        0        0     1232 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/s4180.dat
+-rw-rw-rw-   0        0        0     1294 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/s4233.dat
+-rw-rw-rw-   0        0        0     1123 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/s4310.dat
+-rw-rw-rw-   0        0        0     1123 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/s4320.dat
+-rw-rw-rw-   0        0        0     2142 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/s5010.dat
+-rw-rw-rw-   0        0        0     2142 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/s5020.dat
+-rw-rw-rw-   0        0        0     1475 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/s6061.dat
+-rw-rw-rw-   0        0        0     1476 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/s6062.dat
+-rw-rw-rw-   0        0        0     1477 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/s6063.dat
+-rw-rw-rw-   0        0        0     2281 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/s7012.dat
+-rw-rw-rw-   0        0        0     1973 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/s7055.dat
+-rw-rw-rw-   0        0        0     2280 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/s7075.dat
+-rw-rw-rw-   0        0        0     3400 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/s8025.dat
+-rw-rw-rw-   0        0        0     3425 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/s8035.dat
+-rw-rw-rw-   0        0        0     2281 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/s8036.dat
+-rw-rw-rw-   0        0        0     2281 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/s8037.dat
+-rw-rw-rw-   0        0        0     2281 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/s8038.dat
+-rw-rw-rw-   0        0        0     2284 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/s8052.dat
+-rw-rw-rw-   0        0        0     2282 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/s8055.dat
+-rw-rw-rw-   0        0        0     2916 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/s9000.dat
+-rw-rw-rw-   0        0        0     3404 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/s9026.dat
+-rw-rw-rw-   0        0        0     3402 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/s9027.dat
+-rw-rw-rw-   0        0        0     2916 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/s9032.dat
+-rw-rw-rw-   0        0        0     2918 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/s9033.dat
+-rw-rw-rw-   0        0        0     2311 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/s9037.dat
+-rw-rw-rw-   0        0        0     2276 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/sa7035.dat
+-rw-rw-rw-   0        0        0     2276 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/sa7036.dat
+-rw-rw-rw-   0        0        0     2276 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/sa7038.dat
+-rw-rw-rw-   0        0        0      626 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/saratov.dat
+-rw-rw-rw-   0        0        0     3067 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/sc1012r8.dat
+-rw-rw-rw-   0        0        0     3075 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/sc1094r8.dat
+-rw-rw-rw-   0        0        0     2775 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/sc1095.dat
+-rw-rw-rw-   0        0        0     2243 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/sc1095r8.dat
+-rw-rw-rw-   0        0        0     4022 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/sc20010.dat
+-rw-rw-rw-   0        0        0     4022 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/sc20012.dat
+-rw-rw-rw-   0        0        0     4027 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/sc20402.dat
+-rw-rw-rw-   0        0        0     4018 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/sc20403.dat
+-rw-rw-rw-   0        0        0     4024 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/sc20404.dat
+-rw-rw-rw-   0        0        0     4024 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/sc20406.dat
+-rw-rw-rw-   0        0        0     4009 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/sc20410.dat
+-rw-rw-rw-   0        0        0     4009 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/sc20412.dat
+-rw-rw-rw-   0        0        0     4009 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/sc20414.dat
+-rw-rw-rw-   0        0        0     4028 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/sc20503.dat
+-rw-rw-rw-   0        0        0     4017 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/sc20518.dat
+-rw-rw-rw-   0        0        0     4028 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/sc20606.dat
+-rw-rw-rw-   0        0        0     4025 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/sc20610.dat
+-rw-rw-rw-   0        0        0     4025 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/sc20612.dat
+-rw-rw-rw-   0        0        0     4025 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/sc20614.dat
+-rw-rw-rw-   0        0        0     4029 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/sc20706.dat
+-rw-rw-rw-   0        0        0     4027 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/sc20710.dat
+-rw-rw-rw-   0        0        0     4027 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/sc20712.dat
+-rw-rw-rw-   0        0        0     4026 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/sc20714.dat
+-rw-rw-rw-   0        0        0     4042 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/sc21006.dat
+-rw-rw-rw-   0        0        0     4038 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/sc21010.dat
+-rw-rw-rw-   0        0        0     1847 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/sc2110.dat
+-rw-rw-rw-   0        0        0     1231 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/sd2030.dat
+-rw-rw-rw-   0        0        0     1233 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/sd2083.dat
+-rw-rw-rw-   0        0        0     1233 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/sd5060.dat
+-rw-rw-rw-   0        0        0     1233 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/sd6060.dat
+-rw-rw-rw-   0        0        0     1233 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/sd6080.dat
+-rw-rw-rw-   0        0        0     1233 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/sd7003.dat
+-rw-rw-rw-   0        0        0     1233 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/sd7032.dat
+-rw-rw-rw-   0        0        0     1227 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/sd7034.dat
+-rw-rw-rw-   0        0        0     1233 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/sd7037.dat
+-rw-rw-rw-   0        0        0     1233 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/sd7043.dat
+-rw-rw-rw-   0        0        0     1232 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/sd7062.dat
+-rw-rw-rw-   0        0        0     1233 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/sd7080.dat
+-rw-rw-rw-   0        0        0     1233 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/sd7084.dat
+-rw-rw-rw-   0        0        0     1232 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/sd7090.dat
+-rw-rw-rw-   0        0        0     1233 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/sd8000.dat
+-rw-rw-rw-   0        0        0     1229 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/sd8020.dat
+-rw-rw-rw-   0        0        0     1232 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/sd8040.dat
+-rw-rw-rw-   0        0        0     2276 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/sg6040.dat
+-rw-rw-rw-   0        0        0     1952 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/sg6041.dat
+-rw-rw-rw-   0        0        0     2276 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/sg6042.dat
+-rw-rw-rw-   0        0        0     1952 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/sg6043.dat
+-rw-rw-rw-   0        0        0     2276 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/sg6050.dat
+-rw-rw-rw-   0        0        0     2276 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/sg6051.dat
+-rw-rw-rw-   0        0        0     1316 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/sm701.dat
+-rw-rw-rw-   0        0        0      752 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/sokolov.dat
+-rw-rw-rw-   0        0        0      994 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/spicasm.dat
+-rw-rw-rw-   0        0        0     2778 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ssca07.dat
+-rw-rw-rw-   0        0        0     2779 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ssca09.dat
+-rw-rw-rw-   0        0        0      663 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/stcyr171.dat
+-rw-rw-rw-   0        0        0      663 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/stcyr172.dat
+-rw-rw-rw-   0        0        0      655 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/stcyr234.dat
+-rw-rw-rw-   0        0        0      656 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/stcyr24.dat
+-rw-rw-rw-   0        0        0     1288 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ste87151.dat
+-rw-rw-rw-   0        0        0     1291 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ste87391.dat
+-rw-rw-rw-   0        0        0     1288 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/stf86361.dat
+-rw-rw-rw-   0        0        0      602 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/strand.dat
+-rw-rw-rw-   0        0        0     2559 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/tempest1.dat
+-rw-rw-rw-   0        0        0     2557 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/tempest2.dat
+-rw-rw-rw-   0        0        0     2560 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/tempest3.dat
+-rw-rw-rw-   0        0        0     1207 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/th25816.dat
+-rw-rw-rw-   0        0        0     2067 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/trainer60.dat
+-rw-rw-rw-   0        0        0      712 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/tsagi12.dat
+-rw-rw-rw-   0        0        0      711 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/tsagi8.dat
+-rw-rw-rw-   0        0        0     1063 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ua2-180.dat
+-rw-rw-rw-   0        0        0     1246 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ua2-180sm.dat
+-rw-rw-rw-   0        0        0     1450 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ua79sf18.dat
+-rw-rw-rw-   0        0        0      798 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ua79sff.dat
+-rw-rw-rw-   0        0        0     1007 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ua79sfm.dat
+-rw-rw-rw-   0        0        0     2096 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/uag8814320.dat
+-rw-rw-rw-   0        0        0     1612 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ui1720.dat
+-rw-rw-rw-   0        0        0     2066 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ultimate.dat
+-rw-rw-rw-   0        0        0     2068 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/us1000root.dat
+-rw-rw-rw-   0        0        0      709 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/usa22.dat
+-rw-rw-rw-   0        0        0      709 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/usa25.dat
+-rw-rw-rw-   0        0        0      709 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/usa26.dat
+-rw-rw-rw-   0        0        0      709 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/usa27.dat
+-rw-rw-rw-   0        0        0      714 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/usa27m2.dat
+-rw-rw-rw-   0        0        0      709 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/usa28.dat
+-rw-rw-rw-   0        0        0      709 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/usa29.dat
+-rw-rw-rw-   0        0        0      709 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/usa31.dat
+-rw-rw-rw-   0        0        0      709 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/usa32.dat
+-rw-rw-rw-   0        0        0      709 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/usa33.dat
+-rw-rw-rw-   0        0        0      709 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/usa34.dat
+-rw-rw-rw-   0        0        0      709 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/usa35.dat
+-rw-rw-rw-   0        0        0      711 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/usa35a.dat
+-rw-rw-rw-   0        0        0      710 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/usa35b.dat
+-rw-rw-rw-   0        0        0      709 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/usa40.dat
+-rw-rw-rw-   0        0        0      711 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/usa40b.dat
+-rw-rw-rw-   0        0        0      709 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/usa41.dat
+-rw-rw-rw-   0        0        0      709 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/usa45.dat
+-rw-rw-rw-   0        0        0      711 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/usa45m.dat
+-rw-rw-rw-   0        0        0      709 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/usa46.dat
+-rw-rw-rw-   0        0        0      709 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/usa48.dat
+-rw-rw-rw-   0        0        0      709 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/usa49.dat
+-rw-rw-rw-   0        0        0      708 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/usa5.dat
+-rw-rw-rw-   0        0        0      709 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/usa50.dat
+-rw-rw-rw-   0        0        0      709 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/usa51.dat
+-rw-rw-rw-   0        0        0      541 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/usa98.dat
+-rw-rw-rw-   0        0        0     1994 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/usnps4.dat
+-rw-rw-rw-   0        0        0      890 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/v13006.dat
+-rw-rw-rw-   0        0        0      861 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/v13009.dat
+-rw-rw-rw-   0        0        0     1083 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/v23010.dat
+-rw-rw-rw-   0        0        0     1570 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/v43012.dat
+-rw-rw-rw-   0        0        0      898 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/v43015.dat
+-rw-rw-rw-   0        0        0      771 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/vr1.dat
+-rw-rw-rw-   0        0        0     1041 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/vr11x.dat
+-rw-rw-rw-   0        0        0     1607 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/vr12.dat
+-rw-rw-rw-   0        0        0     1607 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/vr13.dat
+-rw-rw-rw-   0        0        0     1607 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/vr14.dat
+-rw-rw-rw-   0        0        0     1607 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/vr15.dat
+-rw-rw-rw-   0        0        0      867 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/vr5.dat
+-rw-rw-rw-   0        0        0      940 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/vr7.dat
+-rw-rw-rw-   0        0        0      917 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/vr7b.dat
+-rw-rw-rw-   0        0        0      781 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/vr8.dat
+-rw-rw-rw-   0        0        0      777 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/vr8b.dat
+-rw-rw-rw-   0        0        0      825 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/vr9.dat
+-rw-rw-rw-   0        0        0     2229 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/waspsm.dat
+-rw-rw-rw-   0        0        0     1174 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/wb13535sm.dat
+-rw-rw-rw-   0        0        0      899 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/wb140.dat
+-rw-rw-rw-   0        0        0     1017 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/whitcomb.dat
+-rw-rw-rw-   0        0        0     2122 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ys900.dat
+-rw-rw-rw-   0        0        0     2244 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ys915.dat
+-rw-rw-rw-   0        0        0     2358 2022-03-22 17:49:10.000000 PteraSoftware-3.0.0/pterasoftware/airfoils/ys930.dat
+-rw-rw-rw-   0        0        0    66001 2023-06-22 18:55:41.000000 PteraSoftware-3.0.0/pterasoftware/convergence.py
+-rw-rw-rw-   0        0        0    27266 2023-06-22 18:55:41.000000 PteraSoftware-3.0.0/pterasoftware/functions.py
+-rw-rw-rw-   0        0        0    43804 2023-06-22 18:55:41.000000 PteraSoftware-3.0.0/pterasoftware/geometry.py
+-rw-rw-rw-   0        0        0    39210 2023-06-22 18:55:41.000000 PteraSoftware-3.0.0/pterasoftware/meshing.py
+drwxrwxrwx   0        0        0        0 2023-06-22 18:57:29.018929 PteraSoftware-3.0.0/pterasoftware/models/
+-rw-rw-rw-   0        0        0        0 2023-06-22 18:55:41.000000 PteraSoftware-3.0.0/pterasoftware/models/__init__.py
+-rw-rw-rw-   0        0        0     4080 2023-06-22 18:55:41.000000 PteraSoftware-3.0.0/pterasoftware/models/steady_horseshoe_vortex_lattice_method_solver.py
+-rw-rw-rw-   0        0        0    14073 2023-06-22 18:55:41.000000 PteraSoftware-3.0.0/pterasoftware/models/steady_ring_vortex_lattice_method_solver.py
+-rw-rw-rw-   0        0        0    25511 2023-06-22 18:55:41.000000 PteraSoftware-3.0.0/pterasoftware/models/unsteady_ring_vortex_lattice_method_solver_static.py
+-rw-rw-rw-   0        0        0    24062 2023-06-22 18:55:41.000000 PteraSoftware-3.0.0/pterasoftware/models/unsteady_ring_vortex_lattice_method_solver_variable.py
+-rw-rw-rw-   0        0        0    15046 2023-06-22 18:55:41.000000 PteraSoftware-3.0.0/pterasoftware/models/unsteady_ring_vortex_lattice_method_solver_variable_formation.py
+-rw-rw-rw-   0        0        0    65154 2023-06-22 18:55:41.000000 PteraSoftware-3.0.0/pterasoftware/movement.py
+-rw-rw-rw-   0        0        0     6403 2022-04-19 18:41:43.000000 PteraSoftware-3.0.0/pterasoftware/operating_point.py
+-rw-rw-rw-   0        0        0    47945 2023-06-22 18:55:41.000000 PteraSoftware-3.0.0/pterasoftware/output.py
+-rw-rw-rw-   0        0        0    10319 2023-06-22 18:55:41.000000 PteraSoftware-3.0.0/pterasoftware/panel.py
+-rw-rw-rw-   0        0        0     6073 2023-06-22 18:55:41.000000 PteraSoftware-3.0.0/pterasoftware/problems.py
+-rw-rw-rw-   0        0        0    16695 2023-06-22 18:55:41.000000 PteraSoftware-3.0.0/pterasoftware/steady_horseshoe_vortex_lattice_method.py
+-rw-rw-rw-   0        0        0    31807 2023-06-22 18:55:41.000000 PteraSoftware-3.0.0/pterasoftware/steady_ring_vortex_lattice_method.py
+-rw-rw-rw-   0        0        0    12239 2023-06-22 18:55:41.000000 PteraSoftware-3.0.0/pterasoftware/trim.py
+drwxrwxrwx   0        0        0        0 2023-06-22 18:57:29.021928 PteraSoftware-3.0.0/pterasoftware/ui_resources/
+-rw-rw-rw-   0        0        0    52858 2023-06-22 18:55:41.000000 PteraSoftware-3.0.0/pterasoftware/ui_resources/main_window.py
+-rw-rw-rw-   0        0        0    49472 2023-06-22 18:55:41.000000 PteraSoftware-3.0.0/pterasoftware/ui_resources/main_window.ui
+-rw-rw-rw-   0        0        0     1927 2023-06-22 18:55:41.000000 PteraSoftware-3.0.0/pterasoftware/ui_resources/textdialog.py
+-rw-rw-rw-   0        0        0    87906 2023-06-22 18:55:41.000000 PteraSoftware-3.0.0/pterasoftware/unsteady_ring_vortex_lattice_method.py
+-rw-rw-rw-   0        0        0      122 2023-06-22 18:55:41.000000 PteraSoftware-3.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0     1518 2023-06-22 18:57:29.027936 PteraSoftware-3.0.0/setup.cfg
```

### Comparing `PteraSoftware-2.2.1/LICENSE.txt` & `PteraSoftware-3.0.0/LICENSE.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Cameron Urban
+Copyright (c) 2023 Cameron Urban
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this
 software and associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy, modify,
 merge, publish, distribute, sublicense, and/or sell copies of the Software, and to
 permit persons to whom the Software is furnished to do so, subject to the following
 conditions:
```

### Comparing `PteraSoftware-2.2.1/PKG-INFO` & `PteraSoftware-3.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PteraSoftware
-Version: 2.2.1
+Version: 3.0.0
 Summary: This is an open-source, unsteady aerodynamics solver for analyzing flapping-wing flight.
 Home-page: https://github.com/camurban/pterasoftware
 Author: Cameron Urban
 Author-email: camerongurban@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/camurban/pterasoftware/issues
 Keywords: python,uav,simulation,aerospace,computational-biology,cfd,solvers,computational-fluid-dynamics,aerodynamics,aeronautics,potential-flow,vlm,aerospace-engineering,unsteady-flows,aircraft-design,unmanned-aerial-vehicle,ornithopter,ornithology,vortex-lattice-method,pyvista
@@ -19,15 +19,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 ![Logo](https://raw.githubusercontent.com/camUrban/PteraSoftware/master/docs/Logo.png)
 
 ***
 
-![build](https://img.shields.io/travis/camUrban/PteraSoftware/master)
+![build](https://app.travis-ci.com/camUrban/PteraSoftware.svg?branch=master)
 ![coverage](https://img.shields.io/codecov/c/gh/camUrban/PteraSoftware/master)
 ![code quality](https://img.shields.io/codefactor/grade/github/camUrban/PteraSoftware/master)
 ![source rank](https://img.shields.io/librariesio/sourcerank/pypi/PteraSoftware?color=blue&label=source%20rank)
 ![license](https://img.shields.io/github/license/camUrban/PteraSoftware?color=blue)
 ![code style](https://img.shields.io/badge/code%20style-black-black)
 
 ***
@@ -55,14 +55,18 @@
 to develop a solver package capable of unsteady simulations.
 
 Through the combined efforts of Peter Sharpe, Suhas Kodali, and me, Ptera Software was 
 born. It is an easy-to-use, open-source, and actively-maintained UVLM package capable 
 of analyzing flapping-wing flight. Moreover, it's written in Python, is well 
 documented, tested, and validated.
 
+Beginning with version 3.0.0, Ptera Software also includes a GUI developed by Zach Tait.
+Although it is still rudimentary, we hope that it will help make this tool accessible to
+even more users.
+
 With your help, I hope we will increase the open-source community's interest and 
 understanding of biological flight.
 
 ## Features
 
 1. Various Aerodynamic Simulation Methods
    * Steady simulations can be run with a standard horseshoe vortex-lattice method 
@@ -94,15 +98,18 @@
    airplane.
    * This feature can be used to analyze the aerodynamics of flapping-wing formation 
    flight!
 7. Features for Flapping-Wing Vehicle Design
    * Ptera Software is focused on developing features to facilitate designing 
    flapping-wing vehicles.
    * For example, use the functions in the trim module to automatically search for a 
-   trim operating point for steady and unsteady simulations of aircraft. 
+   trim operating point for steady and unsteady simulations of aircraft.
+8. A Basic GUI
+   * This is still in its beta stage, but we will be adding more functionality over the 
+   next several releases.
 
 ## Installation and Use
 
 First things first, you will need a copy of Python 3.8. Python 3.9 is not yet supported 
 due to a dependency issue in VTK. Download Python 3.8 from the official Python website. 
 At this time, I do not recommend using a version from the Anaconda distribution as it 
 could introduce compatibility issues with PyPI.
@@ -160,57 +167,59 @@
 the docstrings there.
 
 I am hoping to implement a web-based documentation guide soon! If you'd like to 
 contribute to this, feel free to open a feature request issue and start a conversation!
 
 ### What If I'm Having Trouble Getting Set Up?
 
-Not to worry! I am working on a video that walks through getting Ptera Software up and 
-running. It will include every step, from downloading Python for the first time to 
-setting up your IDE to running the software. In the meantime, feel free to open an 
-issue for guidance.
+Not to worry! I've made [a video](https://www.youtube.com/watch?v=oX8u2ZflJM4) that walks through getting Ptera Software up and 
+running. It includes every step, from downloading Python for the first time to setting 
+up your IDE to running the software. If you still run into problems, feel free to open 
+an issue for guidance.
 
 ## Example Code
 
 The following code snippet is all that is needed (after running pip install 
-pterasoftware) to run the steady horseshoe solver on a custom airplane object.
+pterasoftware) to run the steady horseshoe solver on an airplane with custom geometry.
 
 ```
 import pterasoftware as ps
 
-example_airplane = ps.geometry.Airplane(
+airplane = ps.geometry.Airplane(
     wings=[
         ps.geometry.Wing(
             symmetric=True,
             wing_cross_sections=[
                 ps.geometry.WingCrossSection(
-                    airfoil=ps.geometry.Airfoil(name="naca2412",),
+                    airfoil=ps.geometry.Airfoil(name="naca2412"),
                 ),
                 ps.geometry.WingCrossSection(
-                    y_le=5.0, airfoil=ps.geometry.Airfoil(name="naca2412",),
+                    y_le=5.0,
+                    airfoil=ps.geometry.Airfoil(name="naca2412"),
                 ),
             ],
         ),
     ],
 )
 
-example_operating_point = ps.operating_point.OperatingPoint()
+operating_point = ps.operating_point.OperatingPoint()
 
-example_problem = ps.problems.SteadyProblem(
-   airplane=example_airplane,
-   operating_point=example_operating_point
+problem = ps.problems.SteadyProblem(
+    airplanes=[airplane], operating_point=operating_point
 )
 
-example_solver = ps.steady_horseshoe_vortex_lattice_method.SteadyHorseshoeVortexLatticeMethodSolver(
-    steady_problem=example_problem
+solver = (
+    ps.steady_horseshoe_vortex_lattice_method.SteadyHorseshoeVortexLatticeMethodSolver(
+        steady_problem=problem
+    )
 )
 
-example_solver.run()
+solver.run()
 
-ps.output.draw(solver=example_solver, show_delta_pressures=True, show_streamlines=True)
+ps.output.draw(solver=solver, scalar_type="lift", show_streamlines=True)
 ```
 
 ## Example Output
 
 This package currently supports three different solvers, a steady horseshoe vortex 
 lattice method (VLM), a steady ring VLM, and an unsteady ring VLM (UVLM). Here are 
 examples of the output you can expect to receive from each of them.
@@ -231,32 +240,34 @@
 
 ![Example Unsteady Ring VLM Moment Coefficient Output](https://raw.githubusercontent.com/camUrban/PteraSoftware/master/docs/examples%20expected%20output/unsteady%20ring%20vortex%20lattice%20method%20solver%20static/Example%20Airplane%20Moment%20Coefficients.png)
 
 ## Requirements
 
 Here are the requirements necessary to run Ptera Software:
 
-* matplotlib >= 3.5.2, < 4.0.0
-* numpy >= 1.22.4, < 1.24.0
-* pyvista >= 0.34.1, < 1.0.0
-* scipy >= 1.8.1, < 2.0.0
-* numba >= 0.55.2, < 1.0.0
-* cmocean >= 2.0.0, < 3.0.0
-* tqdm >= 4.64.0, < 5.0.0
-* webp >= 0.1.4, < 1.0.0
+* matplotlib >= 3.7.1, < 4.0.0
+* numpy >= 1.24.3, < 1.25.0
+* pyvista >= 0.39.1, < 1.0.0
+* scipy >= 1.10.1, < 2.0.0
+* numba >= 0.57.1, < 1.0.0
+* cmocean >= 3.0.3, < 4.0.0
+* tqdm >= 4.65.0, < 5.0.0
+* webp >= 0.1.6, < 1.0.0
+* PySide2 >= 5.15.2.1, < 6.0.0.0
 
 Additionally, these packages are useful for continued development of the software:
 
-* codecov >= 2.1.12, < 3.0.0
-* black >= 22.6.0, < 23.0.0
-* pre-commit >= 2.19.0, < 3.0.0
-* build >= 0.8.0, < 1.0.0
-* twine >= 4.0.1, < 5.0.0
-* setuptools >= 62.6.0, < 63.0.0
-* wheel >= 0.37.1, < 0.38.0
+* codecov >= 2.1.13, < 3.0.0
+* black >= 23.3.0, < 24.0.0
+* pre-commit >= 3.3.3, < 4.0.0
+* build >= 0.10.0, < 1.0.0
+* twine >= 4.0.2, < 5.0.0
+* PyInstaller >= 5.12.0, < 6.0.0
+* setuptools >= 68.0.0, < 69.0.0
+* wheel >= 0.40.0, < 1.0.0
 
 ## Validation
 
 Since the release of version 1.0.0, Ptera Software is now validated against 
 experimental flapping-wing data! See the "validation" directory to run the test case 
 and read a report on the software's accuracy.
 
@@ -282,34 +293,31 @@
 * Maintain the repository's A CodeFactor Rating.
 * We should fill in any of the "Properly document this..." TODO statements.
 * We should ensure that all files be at least 30% comment lines.
 * We should continue to ensure that all source code is formatted using Black.
 
 ### Features
 
-* We should create a setup tutorial video and add it to the documentation. This should 
-be geared toward a user who doesn't have Python, an IDE, or Ptera Software installed on 
-their computer yet.
 * We should implement a leading-edge model to account for flow separation. See 
 "Modified Unsteady Vortex-Lattice Method to Study Flapping Wings in Hover Flight." by 
 Bruno Roccia, Sergio Preidikman, Julio Massa, and Dean Mook for details.
-* We should create a command-line interface or GUI.
 * We should try to implement aeroelastic effects in Ptera Software's solvers.
 * Flapping wing controls is both fascinating and complicated. We should try to create a 
 workflow in Ptera Software for controls systems identification for flapping-wing 
 vehicles.
 
 ## Credits
 
 Here is a list of all the people and packages that helped me created Ptera Software in
 no particular order. Specific citations can be found in the source code's docstrings
 where applicable.
 
 * Suhas Kodali
 * Peter Sharpe
+* Zach Tait
 * Ramesh Agarwal
 * Joseph Katz
 * Allen Plotkin
 * Austin Stover
 * AeroSandbox
 * Black
 * Codecov
```

### Comparing `PteraSoftware-2.2.1/PteraSoftware.egg-info/PKG-INFO` & `PteraSoftware-3.0.0/PteraSoftware.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PteraSoftware
-Version: 2.2.1
+Version: 3.0.0
 Summary: This is an open-source, unsteady aerodynamics solver for analyzing flapping-wing flight.
 Home-page: https://github.com/camurban/pterasoftware
 Author: Cameron Urban
 Author-email: camerongurban@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/camurban/pterasoftware/issues
 Keywords: python,uav,simulation,aerospace,computational-biology,cfd,solvers,computational-fluid-dynamics,aerodynamics,aeronautics,potential-flow,vlm,aerospace-engineering,unsteady-flows,aircraft-design,unmanned-aerial-vehicle,ornithopter,ornithology,vortex-lattice-method,pyvista
@@ -19,15 +19,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 ![Logo](https://raw.githubusercontent.com/camUrban/PteraSoftware/master/docs/Logo.png)
 
 ***
 
-![build](https://img.shields.io/travis/camUrban/PteraSoftware/master)
+![build](https://app.travis-ci.com/camUrban/PteraSoftware.svg?branch=master)
 ![coverage](https://img.shields.io/codecov/c/gh/camUrban/PteraSoftware/master)
 ![code quality](https://img.shields.io/codefactor/grade/github/camUrban/PteraSoftware/master)
 ![source rank](https://img.shields.io/librariesio/sourcerank/pypi/PteraSoftware?color=blue&label=source%20rank)
 ![license](https://img.shields.io/github/license/camUrban/PteraSoftware?color=blue)
 ![code style](https://img.shields.io/badge/code%20style-black-black)
 
 ***
@@ -55,14 +55,18 @@
 to develop a solver package capable of unsteady simulations.
 
 Through the combined efforts of Peter Sharpe, Suhas Kodali, and me, Ptera Software was 
 born. It is an easy-to-use, open-source, and actively-maintained UVLM package capable 
 of analyzing flapping-wing flight. Moreover, it's written in Python, is well 
 documented, tested, and validated.
 
+Beginning with version 3.0.0, Ptera Software also includes a GUI developed by Zach Tait.
+Although it is still rudimentary, we hope that it will help make this tool accessible to
+even more users.
+
 With your help, I hope we will increase the open-source community's interest and 
 understanding of biological flight.
 
 ## Features
 
 1. Various Aerodynamic Simulation Methods
    * Steady simulations can be run with a standard horseshoe vortex-lattice method 
@@ -94,15 +98,18 @@
    airplane.
    * This feature can be used to analyze the aerodynamics of flapping-wing formation 
    flight!
 7. Features for Flapping-Wing Vehicle Design
    * Ptera Software is focused on developing features to facilitate designing 
    flapping-wing vehicles.
    * For example, use the functions in the trim module to automatically search for a 
-   trim operating point for steady and unsteady simulations of aircraft. 
+   trim operating point for steady and unsteady simulations of aircraft.
+8. A Basic GUI
+   * This is still in its beta stage, but we will be adding more functionality over the 
+   next several releases.
 
 ## Installation and Use
 
 First things first, you will need a copy of Python 3.8. Python 3.9 is not yet supported 
 due to a dependency issue in VTK. Download Python 3.8 from the official Python website. 
 At this time, I do not recommend using a version from the Anaconda distribution as it 
 could introduce compatibility issues with PyPI.
@@ -160,57 +167,59 @@
 the docstrings there.
 
 I am hoping to implement a web-based documentation guide soon! If you'd like to 
 contribute to this, feel free to open a feature request issue and start a conversation!
 
 ### What If I'm Having Trouble Getting Set Up?
 
-Not to worry! I am working on a video that walks through getting Ptera Software up and 
-running. It will include every step, from downloading Python for the first time to 
-setting up your IDE to running the software. In the meantime, feel free to open an 
-issue for guidance.
+Not to worry! I've made [a video](https://www.youtube.com/watch?v=oX8u2ZflJM4) that walks through getting Ptera Software up and 
+running. It includes every step, from downloading Python for the first time to setting 
+up your IDE to running the software. If you still run into problems, feel free to open 
+an issue for guidance.
 
 ## Example Code
 
 The following code snippet is all that is needed (after running pip install 
-pterasoftware) to run the steady horseshoe solver on a custom airplane object.
+pterasoftware) to run the steady horseshoe solver on an airplane with custom geometry.
 
 ```
 import pterasoftware as ps
 
-example_airplane = ps.geometry.Airplane(
+airplane = ps.geometry.Airplane(
     wings=[
         ps.geometry.Wing(
             symmetric=True,
             wing_cross_sections=[
                 ps.geometry.WingCrossSection(
-                    airfoil=ps.geometry.Airfoil(name="naca2412",),
+                    airfoil=ps.geometry.Airfoil(name="naca2412"),
                 ),
                 ps.geometry.WingCrossSection(
-                    y_le=5.0, airfoil=ps.geometry.Airfoil(name="naca2412",),
+                    y_le=5.0,
+                    airfoil=ps.geometry.Airfoil(name="naca2412"),
                 ),
             ],
         ),
     ],
 )
 
-example_operating_point = ps.operating_point.OperatingPoint()
+operating_point = ps.operating_point.OperatingPoint()
 
-example_problem = ps.problems.SteadyProblem(
-   airplane=example_airplane,
-   operating_point=example_operating_point
+problem = ps.problems.SteadyProblem(
+    airplanes=[airplane], operating_point=operating_point
 )
 
-example_solver = ps.steady_horseshoe_vortex_lattice_method.SteadyHorseshoeVortexLatticeMethodSolver(
-    steady_problem=example_problem
+solver = (
+    ps.steady_horseshoe_vortex_lattice_method.SteadyHorseshoeVortexLatticeMethodSolver(
+        steady_problem=problem
+    )
 )
 
-example_solver.run()
+solver.run()
 
-ps.output.draw(solver=example_solver, show_delta_pressures=True, show_streamlines=True)
+ps.output.draw(solver=solver, scalar_type="lift", show_streamlines=True)
 ```
 
 ## Example Output
 
 This package currently supports three different solvers, a steady horseshoe vortex 
 lattice method (VLM), a steady ring VLM, and an unsteady ring VLM (UVLM). Here are 
 examples of the output you can expect to receive from each of them.
@@ -231,32 +240,34 @@
 
 ![Example Unsteady Ring VLM Moment Coefficient Output](https://raw.githubusercontent.com/camUrban/PteraSoftware/master/docs/examples%20expected%20output/unsteady%20ring%20vortex%20lattice%20method%20solver%20static/Example%20Airplane%20Moment%20Coefficients.png)
 
 ## Requirements
 
 Here are the requirements necessary to run Ptera Software:
 
-* matplotlib >= 3.5.2, < 4.0.0
-* numpy >= 1.22.4, < 1.24.0
-* pyvista >= 0.34.1, < 1.0.0
-* scipy >= 1.8.1, < 2.0.0
-* numba >= 0.55.2, < 1.0.0
-* cmocean >= 2.0.0, < 3.0.0
-* tqdm >= 4.64.0, < 5.0.0
-* webp >= 0.1.4, < 1.0.0
+* matplotlib >= 3.7.1, < 4.0.0
+* numpy >= 1.24.3, < 1.25.0
+* pyvista >= 0.39.1, < 1.0.0
+* scipy >= 1.10.1, < 2.0.0
+* numba >= 0.57.1, < 1.0.0
+* cmocean >= 3.0.3, < 4.0.0
+* tqdm >= 4.65.0, < 5.0.0
+* webp >= 0.1.6, < 1.0.0
+* PySide2 >= 5.15.2.1, < 6.0.0.0
 
 Additionally, these packages are useful for continued development of the software:
 
-* codecov >= 2.1.12, < 3.0.0
-* black >= 22.6.0, < 23.0.0
-* pre-commit >= 2.19.0, < 3.0.0
-* build >= 0.8.0, < 1.0.0
-* twine >= 4.0.1, < 5.0.0
-* setuptools >= 62.6.0, < 63.0.0
-* wheel >= 0.37.1, < 0.38.0
+* codecov >= 2.1.13, < 3.0.0
+* black >= 23.3.0, < 24.0.0
+* pre-commit >= 3.3.3, < 4.0.0
+* build >= 0.10.0, < 1.0.0
+* twine >= 4.0.2, < 5.0.0
+* PyInstaller >= 5.12.0, < 6.0.0
+* setuptools >= 68.0.0, < 69.0.0
+* wheel >= 0.40.0, < 1.0.0
 
 ## Validation
 
 Since the release of version 1.0.0, Ptera Software is now validated against 
 experimental flapping-wing data! See the "validation" directory to run the test case 
 and read a report on the software's accuracy.
 
@@ -282,34 +293,31 @@
 * Maintain the repository's A CodeFactor Rating.
 * We should fill in any of the "Properly document this..." TODO statements.
 * We should ensure that all files be at least 30% comment lines.
 * We should continue to ensure that all source code is formatted using Black.
 
 ### Features
 
-* We should create a setup tutorial video and add it to the documentation. This should 
-be geared toward a user who doesn't have Python, an IDE, or Ptera Software installed on 
-their computer yet.
 * We should implement a leading-edge model to account for flow separation. See 
 "Modified Unsteady Vortex-Lattice Method to Study Flapping Wings in Hover Flight." by 
 Bruno Roccia, Sergio Preidikman, Julio Massa, and Dean Mook for details.
-* We should create a command-line interface or GUI.
 * We should try to implement aeroelastic effects in Ptera Software's solvers.
 * Flapping wing controls is both fascinating and complicated. We should try to create a 
 workflow in Ptera Software for controls systems identification for flapping-wing 
 vehicles.
 
 ## Credits
 
 Here is a list of all the people and packages that helped me created Ptera Software in
 no particular order. Specific citations can be found in the source code's docstrings
 where applicable.
 
 * Suhas Kodali
 * Peter Sharpe
+* Zach Tait
 * Ramesh Agarwal
 * Joseph Katz
 * Allen Plotkin
 * Austin Stover
 * AeroSandbox
 * Black
 * Codecov
```

### Comparing `PteraSoftware-2.2.1/PteraSoftware.egg-info/SOURCES.txt` & `PteraSoftware-3.0.0/PteraSoftware.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1570,8 +1570,17 @@
 pterasoftware/airfoils/vr9.dat
 pterasoftware/airfoils/waspsm.dat
 pterasoftware/airfoils/wb13535sm.dat
 pterasoftware/airfoils/wb140.dat
 pterasoftware/airfoils/whitcomb.dat
 pterasoftware/airfoils/ys900.dat
 pterasoftware/airfoils/ys915.dat
-pterasoftware/airfoils/ys930.dat
+pterasoftware/airfoils/ys930.dat
+pterasoftware/models/__init__.py
+pterasoftware/models/steady_horseshoe_vortex_lattice_method_solver.py
+pterasoftware/models/steady_ring_vortex_lattice_method_solver.py
+pterasoftware/models/unsteady_ring_vortex_lattice_method_solver_static.py
+pterasoftware/models/unsteady_ring_vortex_lattice_method_solver_variable.py
+pterasoftware/models/unsteady_ring_vortex_lattice_method_solver_variable_formation.py
+pterasoftware/ui_resources/main_window.py
+pterasoftware/ui_resources/main_window.ui
+pterasoftware/ui_resources/textdialog.py
```

### Comparing `PteraSoftware-2.2.1/README.md` & `PteraSoftware-3.0.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ![Logo](https://raw.githubusercontent.com/camUrban/PteraSoftware/master/docs/Logo.png)
 
 ***
 
-![build](https://img.shields.io/travis/camUrban/PteraSoftware/master)
+![build](https://app.travis-ci.com/camUrban/PteraSoftware.svg?branch=master)
 ![coverage](https://img.shields.io/codecov/c/gh/camUrban/PteraSoftware/master)
 ![code quality](https://img.shields.io/codefactor/grade/github/camUrban/PteraSoftware/master)
 ![source rank](https://img.shields.io/librariesio/sourcerank/pypi/PteraSoftware?color=blue&label=source%20rank)
 ![license](https://img.shields.io/github/license/camUrban/PteraSoftware?color=blue)
 ![code style](https://img.shields.io/badge/code%20style-black-black)
 
 ***
@@ -34,14 +34,18 @@
 to develop a solver package capable of unsteady simulations.
 
 Through the combined efforts of Peter Sharpe, Suhas Kodali, and me, Ptera Software was 
 born. It is an easy-to-use, open-source, and actively-maintained UVLM package capable 
 of analyzing flapping-wing flight. Moreover, it's written in Python, is well 
 documented, tested, and validated.
 
+Beginning with version 3.0.0, Ptera Software also includes a GUI developed by Zach Tait.
+Although it is still rudimentary, we hope that it will help make this tool accessible to
+even more users.
+
 With your help, I hope we will increase the open-source community's interest and 
 understanding of biological flight.
 
 ## Features
 
 1. Various Aerodynamic Simulation Methods
    * Steady simulations can be run with a standard horseshoe vortex-lattice method 
@@ -73,15 +77,18 @@
    airplane.
    * This feature can be used to analyze the aerodynamics of flapping-wing formation 
    flight!
 7. Features for Flapping-Wing Vehicle Design
    * Ptera Software is focused on developing features to facilitate designing 
    flapping-wing vehicles.
    * For example, use the functions in the trim module to automatically search for a 
-   trim operating point for steady and unsteady simulations of aircraft. 
+   trim operating point for steady and unsteady simulations of aircraft.
+8. A Basic GUI
+   * This is still in its beta stage, but we will be adding more functionality over the 
+   next several releases.
 
 ## Installation and Use
 
 First things first, you will need a copy of Python 3.8. Python 3.9 is not yet supported 
 due to a dependency issue in VTK. Download Python 3.8 from the official Python website. 
 At this time, I do not recommend using a version from the Anaconda distribution as it 
 could introduce compatibility issues with PyPI.
@@ -139,57 +146,59 @@
 the docstrings there.
 
 I am hoping to implement a web-based documentation guide soon! If you'd like to 
 contribute to this, feel free to open a feature request issue and start a conversation!
 
 ### What If I'm Having Trouble Getting Set Up?
 
-Not to worry! I am working on a video that walks through getting Ptera Software up and 
-running. It will include every step, from downloading Python for the first time to 
-setting up your IDE to running the software. In the meantime, feel free to open an 
-issue for guidance.
+Not to worry! I've made [a video](https://www.youtube.com/watch?v=oX8u2ZflJM4) that walks through getting Ptera Software up and 
+running. It includes every step, from downloading Python for the first time to setting 
+up your IDE to running the software. If you still run into problems, feel free to open 
+an issue for guidance.
 
 ## Example Code
 
 The following code snippet is all that is needed (after running pip install 
-pterasoftware) to run the steady horseshoe solver on a custom airplane object.
+pterasoftware) to run the steady horseshoe solver on an airplane with custom geometry.
 
 ```
 import pterasoftware as ps
 
-example_airplane = ps.geometry.Airplane(
+airplane = ps.geometry.Airplane(
     wings=[
         ps.geometry.Wing(
             symmetric=True,
             wing_cross_sections=[
                 ps.geometry.WingCrossSection(
-                    airfoil=ps.geometry.Airfoil(name="naca2412",),
+                    airfoil=ps.geometry.Airfoil(name="naca2412"),
                 ),
                 ps.geometry.WingCrossSection(
-                    y_le=5.0, airfoil=ps.geometry.Airfoil(name="naca2412",),
+                    y_le=5.0,
+                    airfoil=ps.geometry.Airfoil(name="naca2412"),
                 ),
             ],
         ),
     ],
 )
 
-example_operating_point = ps.operating_point.OperatingPoint()
+operating_point = ps.operating_point.OperatingPoint()
 
-example_problem = ps.problems.SteadyProblem(
-   airplane=example_airplane,
-   operating_point=example_operating_point
+problem = ps.problems.SteadyProblem(
+    airplanes=[airplane], operating_point=operating_point
 )
 
-example_solver = ps.steady_horseshoe_vortex_lattice_method.SteadyHorseshoeVortexLatticeMethodSolver(
-    steady_problem=example_problem
+solver = (
+    ps.steady_horseshoe_vortex_lattice_method.SteadyHorseshoeVortexLatticeMethodSolver(
+        steady_problem=problem
+    )
 )
 
-example_solver.run()
+solver.run()
 
-ps.output.draw(solver=example_solver, show_delta_pressures=True, show_streamlines=True)
+ps.output.draw(solver=solver, scalar_type="lift", show_streamlines=True)
 ```
 
 ## Example Output
 
 This package currently supports three different solvers, a steady horseshoe vortex 
 lattice method (VLM), a steady ring VLM, and an unsteady ring VLM (UVLM). Here are 
 examples of the output you can expect to receive from each of them.
@@ -210,32 +219,34 @@
 
 ![Example Unsteady Ring VLM Moment Coefficient Output](https://raw.githubusercontent.com/camUrban/PteraSoftware/master/docs/examples%20expected%20output/unsteady%20ring%20vortex%20lattice%20method%20solver%20static/Example%20Airplane%20Moment%20Coefficients.png)
 
 ## Requirements
 
 Here are the requirements necessary to run Ptera Software:
 
-* matplotlib >= 3.5.2, < 4.0.0
-* numpy >= 1.22.4, < 1.24.0
-* pyvista >= 0.34.1, < 1.0.0
-* scipy >= 1.8.1, < 2.0.0
-* numba >= 0.55.2, < 1.0.0
-* cmocean >= 2.0.0, < 3.0.0
-* tqdm >= 4.64.0, < 5.0.0
-* webp >= 0.1.4, < 1.0.0
+* matplotlib >= 3.7.1, < 4.0.0
+* numpy >= 1.24.3, < 1.25.0
+* pyvista >= 0.39.1, < 1.0.0
+* scipy >= 1.10.1, < 2.0.0
+* numba >= 0.57.1, < 1.0.0
+* cmocean >= 3.0.3, < 4.0.0
+* tqdm >= 4.65.0, < 5.0.0
+* webp >= 0.1.6, < 1.0.0
+* PySide2 >= 5.15.2.1, < 6.0.0.0
 
 Additionally, these packages are useful for continued development of the software:
 
-* codecov >= 2.1.12, < 3.0.0
-* black >= 22.6.0, < 23.0.0
-* pre-commit >= 2.19.0, < 3.0.0
-* build >= 0.8.0, < 1.0.0
-* twine >= 4.0.1, < 5.0.0
-* setuptools >= 62.6.0, < 63.0.0
-* wheel >= 0.37.1, < 0.38.0
+* codecov >= 2.1.13, < 3.0.0
+* black >= 23.3.0, < 24.0.0
+* pre-commit >= 3.3.3, < 4.0.0
+* build >= 0.10.0, < 1.0.0
+* twine >= 4.0.2, < 5.0.0
+* PyInstaller >= 5.12.0, < 6.0.0
+* setuptools >= 68.0.0, < 69.0.0
+* wheel >= 0.40.0, < 1.0.0
 
 ## Validation
 
 Since the release of version 1.0.0, Ptera Software is now validated against 
 experimental flapping-wing data! See the "validation" directory to run the test case 
 and read a report on the software's accuracy.
 
@@ -261,34 +272,31 @@
 * Maintain the repository's A CodeFactor Rating.
 * We should fill in any of the "Properly document this..." TODO statements.
 * We should ensure that all files be at least 30% comment lines.
 * We should continue to ensure that all source code is formatted using Black.
 
 ### Features
 
-* We should create a setup tutorial video and add it to the documentation. This should 
-be geared toward a user who doesn't have Python, an IDE, or Ptera Software installed on 
-their computer yet.
 * We should implement a leading-edge model to account for flow separation. See 
 "Modified Unsteady Vortex-Lattice Method to Study Flapping Wings in Hover Flight." by 
 Bruno Roccia, Sergio Preidikman, Julio Massa, and Dean Mook for details.
-* We should create a command-line interface or GUI.
 * We should try to implement aeroelastic effects in Ptera Software's solvers.
 * Flapping wing controls is both fascinating and complicated. We should try to create a 
 workflow in Ptera Software for controls systems identification for flapping-wing 
 vehicles.
 
 ## Credits
 
 Here is a list of all the people and packages that helped me created Ptera Software in
 no particular order. Specific citations can be found in the source code's docstrings
 where applicable.
 
 * Suhas Kodali
 * Peter Sharpe
+* Zach Tait
 * Ramesh Agarwal
 * Joseph Katz
 * Allen Plotkin
 * Austin Stover
 * AeroSandbox
 * Black
 * Codecov
```

### Comparing `PteraSoftware-2.2.1/pterasoftware/__init__.py` & `PteraSoftware-3.0.0/pterasoftware/__init__.py`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/aerodynamics.py` & `PteraSoftware-3.0.0/pterasoftware/aerodynamics.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,14 +19,19 @@
     points, and the attributes of a group of horseshoe vortices. At every point,
     it finds the induced velocity due to each horseshoe vortex.
 
     collapsed_velocities_from_ring_vortices: This function takes in a group of
     points, and the attributes of a group of ring vortices. At every point, it finds
     the cumulative induced velocity due to all the ring vortices.
 
+    collapsed_velocities_from_ring_vortices_chordwise_segments: This function takes
+    in a group of points, and the attributes of a group of ring vortices. At every
+    point, it finds the cumulative induced velocity due to all the ring vortices'
+    chordwise segments.
+
     expanded_velocities_from_ring_vortices: This function takes in a group of points,
     and the attributes of a group of ring vortices. At every point, it finds the
     induced velocity due to each ring vortex.
 
     collapsed_velocities_from_line_vortices: This function takes in a group of
     points, and the attributes of a group of line vortices. At every point, it finds
     the cumulative induced velocity due to all the line vortices.
@@ -581,14 +586,96 @@
         induced_velocities += collapsed_velocities_from_line_vortices(
             points=points,
             origins=origins_list[i],
             terminations=terminations_list[i],
             strengths=strengths,
             ages=ages,
             nu=nu,
+        )
+    return induced_velocities
+
+
+@njit(cache=True, fastmath=False)
+def collapsed_velocities_from_ring_vortices_chordwise_segments(
+    points,
+    back_right_vortex_vertices,
+    front_right_vortex_vertices,
+    front_left_vortex_vertices,
+    back_left_vortex_vertices,
+    strengths,
+    ages=None,
+    nu=0.0,
+):
+    """This function takes in a group of points, and the attributes of a group of
+    ring vortices. At every point, it finds the cumulative induced velocity due to
+    all the ring vortices' chordwise segments.
+
+    Note: This function's performance has been highly optimized for unsteady
+    simulations via Numba. While using Numba dramatically increases unsteady
+    simulation performance, it does cause a performance drop for the less intense
+    steady simulations.
+
+    :param points: 2D array of floats
+        This variable is an array of shape (N x 3), where N is the number of points.
+        Each row contains the x, y, and z float coordinates of that point's position
+        in meters.
+    :param back_right_vortex_vertices: 2D array of floats
+        This variable is an array of shape (M x 3), where M is the number of ring
+        vortices. Each row contains the x, y, and z float coordinates of that ring
+        vortex's back right vertex's position in meters.
+    :param front_right_vortex_vertices: 2D array of floats
+        This variable is an array of shape (M x 3), where M is the number of ring
+        vortices. Each row contains the x, y, and z float coordinates of that ring
+        vortex's front right vertex's position in meters.
+    :param front_left_vortex_vertices: 2D array of floats
+        This variable is an array of shape (M x 3), where M is the number of ring
+        vortices. Each row contains the x, y, and z float coordinates of that ring
+        vortex's front left vertex's position in meters.
+    :param back_left_vortex_vertices: 2D array of floats
+        This variable is an array of shape (M x 3), where M is the number of ring
+        vortices. Each row contains the x, y, and z float coordinates of that ring
+        vortex's front left vertex's position in meters.
+    :param strengths: 1D array of floats
+        This variable is an array of shape (, M), where M is the number of ring
+        vortices. Each holds the strength of that ring vortex in meters squared per
+        second.
+    :param ages: 1D array of floats, optional
+        This variable is an array of shape (, M), where M is the number of line
+        vortices. Each position contains the age of that ring vortex in seconds. This
+        is only relevant for vortices that have been shed into the wake. The default
+        value is None. If the age of a specific vortex is 0.0 seconds, then the
+        vortex core radius is set to 0.0 meters.
+    :param nu: float, optional
+        This variable is a float that represents the kinematic viscosity of the fluid
+        in meters squared per second. The default value is 0.0 meters squared per
+        second.
+    :return velocities: 2D array of floats
+        This is an array of shape (N x 3), and it holds the cumulative induced
+        velocity at each of the N points due to all the ring vortices' spanwise
+        segments. The units are meters per second.
+    """
+    origins_list = [
+        back_right_vortex_vertices,
+        front_left_vortex_vertices,
+    ]
+    terminations_list = [
+        front_right_vortex_vertices,
+        back_left_vortex_vertices,
+    ]
+    induced_velocities = np.zeros((points.shape[0], 3))
+
+    # Get the velocity induced by each leg of the ring vortex.
+    for i in range(2):
+        induced_velocities += collapsed_velocities_from_line_vortices(
+            points=points,
+            origins=origins_list[i],
+            terminations=terminations_list[i],
+            strengths=strengths,
+            ages=ages,
+            nu=nu,
         )
     return induced_velocities
 
 
 @njit(cache=True, fastmath=False)
 def expanded_velocities_from_ring_vortices(
     points,
```

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/2032c.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/2032c.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/a18.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/a18.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/a18sm.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/a18sm.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/a63a108c.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/a63a108c.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ag03.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ag03.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ag04.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ag04.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ag08.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ag08.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ag09.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ag09.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ag10.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ag10.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ag11.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ag11.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ag12.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ag12.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ag13.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ag13.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ag14.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ag14.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ag16.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ag16.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ag17.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ag17.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ag18.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ag18.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ag19.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ag19.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ag24.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ag24.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ag25.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ag25.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ag26.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ag26.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ag27.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ag27.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ag35.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ag35.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ag36.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ag36.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ag37.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ag37.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ag38.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ag38.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ag44ct02r.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ag44ct02r.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ag455ct02r.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ag455ct02r.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ag45c03.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ag45c03.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ag45ct02r.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ag45ct02r.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ag46c03.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ag46c03.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ag46ct02r.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ag46ct02r.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ag47c03.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ag47c03.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ag47ct02r.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ag47ct02r.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ah21-7.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ah21-7.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ah21-9.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ah21-9.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ah63k127.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ah63k127.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ah6407.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ah6407.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ah7476.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ah7476.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ah79100a.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ah79100a.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ah79100b.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ah79100b.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ah79100c.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ah79100c.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ah79k132.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ah79k132.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ah79k135.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ah79k135.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ah79k143.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ah79k143.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ah80129.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ah80129.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ah80136.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ah80136.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ah80140.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ah80140.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ah81131.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ah81131.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ah81k144.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ah81k144.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ah81k144wfKlappe.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ah81k144wfKlappe.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ah82150a.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ah82150a.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ah82150f.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ah82150f.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ah83150q.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ah83150q.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ah83159.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ah83159.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ah85l120.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ah85l120.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ah88k130.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ah88k130.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ah88k136.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ah88k136.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ah93156.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ah93156.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ah93157.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ah93157.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ah93k130.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ah93k130.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ah93k131.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ah93k131.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ah93k132.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ah93k132.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ah93w145.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ah93w145.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ah93w174.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ah93w174.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ah93w215.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ah93w215.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ah93w257.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ah93w257.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ah93w300.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ah93w300.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ah93w480b.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ah93w480b.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ah94145.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ah94145.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ah94156.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ah94156.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ah94w301.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ah94w301.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ah95160.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ah95160.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ames01.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ames01.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ames02.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ames02.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ames03.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ames03.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/amsoil1.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/amsoil1.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/amsoil2.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/amsoil2.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/apex16.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/apex16.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/aquilasm.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/aquilasm.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/arad10.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/arad10.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/arad13.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/arad13.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/arad20.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/arad20.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/arad6.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/arad6.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/as5045.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/as5045.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/as5046.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/as5046.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/as5048.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/as5048.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/atr72sm.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/atr72sm.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/august160.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/august160.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/avistar.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/avistar.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/b29root.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/b29root.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/b29tip.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/b29tip.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/b540ols.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/b540ols.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/b707a.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/b707a.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/b707b.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/b707b.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/b707c.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/b707c.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/b707d.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/b707d.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/b707e.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/b707e.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/b737a.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/b737a.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/b737b.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/b737b.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/b737c.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/b737c.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/b737d.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/b737d.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/bacj.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/bacj.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/bacxxx.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/bacxxx.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/bambino6.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/bambino6.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/be50.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/be50.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/be50sm.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/be50sm.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/boe103.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/boe103.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/boe106.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/boe106.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/bqm34.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/bqm34.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/bw3.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/bw3.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/c141a.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/c141a.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/c141b.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/c141b.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/c141c.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/c141c.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/c141d.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/c141d.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/c141e.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/c141e.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/c141f.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/c141f.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/c5a.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/c5a.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/c5b.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/c5b.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/c5c.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/c5c.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/c5d.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/c5d.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/c5e.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/c5e.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/cap21c.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/cap21c.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/cast102.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/cast102.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ch10sm.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ch10sm.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/chen.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/chen.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/clarkk.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/clarkk.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/clarkv.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/clarkv.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/clarkw.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/clarkw.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/clarkx.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/clarkx.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/clarky.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/clarky.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/clarkyh.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/clarkyh.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/clarkys.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/clarkys.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/clarkysm.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/clarkysm.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/clarkz.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/clarkz.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/clarym15.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/clarym15.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/clarym18.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/clarym18.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/coanda1.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/coanda1.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/coanda2.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/coanda2.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/coanda3.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/coanda3.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/cootie.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/cootie.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/cr001sm.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/cr001sm.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/cr1.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/cr1.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/curtisc72.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/curtisc72.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/dae11.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/dae11.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/dae21.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/dae21.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/dae31.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/dae31.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/dae51.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/dae51.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/davis.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/davis.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/davis_corrected.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/davis_corrected.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/davissm.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/davissm.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/daytonwright6.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/daytonwright6.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/daytonwrightt1.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/daytonwrightt1.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/dbln526.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/dbln526.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/defcnd1.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/defcnd1.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/defcnd2.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/defcnd2.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/defcnd3.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/defcnd3.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/df101.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/df101.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/df102.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/df102.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/dfvlrr4.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/dfvlrr4.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/dga1138.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/dga1138.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/dga1182.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/dga1182.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/dh4009sm.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/dh4009sm.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/doa5.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/doa5.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/dormoy.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/dormoy.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/drgnfly.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/drgnfly.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/dsma523a.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/dsma523a.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/dsma523b.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/dsma523b.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/du8608418.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/du8608418.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/du861372.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/du861372.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e1098.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e1098.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e1200.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e1200.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e1210.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e1210.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e1211.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e1211.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e1212.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e1212.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e1212mod.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e1212mod.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e1213.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e1213.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e1214.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e1214.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e1230.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e1230.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e1233.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e1233.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e168.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e168.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e169.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e169.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e171.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e171.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e174.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e174.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e176.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e176.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e178.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e178.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e180.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e180.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e182.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e182.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e184.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e184.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e186.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e186.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e193.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e193.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e195.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e195.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e197.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e197.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e201.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e201.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e203.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e203.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e205.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e205.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e207.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e207.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e209.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e209.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e210.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e210.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e211.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e211.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e212.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e212.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e214.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e214.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e216.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e216.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e220.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e220.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e221.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e221.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e222.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e222.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e224.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e224.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e226.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e226.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e228.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e228.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e230.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e230.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e231.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e231.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e266.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e266.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e297.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e297.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e325.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e325.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e326.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e326.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e327.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e327.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e328.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e328.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e329.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e329.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e330.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e330.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e331.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e331.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e332.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e332.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e333.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e333.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e334.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e334.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e335.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e335.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e336.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e336.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e337.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e337.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e338.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e338.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e339.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e339.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e340.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e340.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e341.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e341.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e342.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e342.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e343.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e343.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e344.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e344.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e360.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e360.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e361.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e361.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e374.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e374.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e376.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e376.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e377.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e377.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e377m.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e377m.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e378.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e378.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e379.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e379.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e385.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e385.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e387.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e387.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e392.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e392.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e393.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e393.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e395.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e395.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e396.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e396.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e397.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e397.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e398.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e398.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e399.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e399.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e403.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e403.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e407.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e407.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e417.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e417.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e420.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e420.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e421.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e421.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e422.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e422.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e423.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e423.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e426.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e426.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e428.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e428.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e431.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e431.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e432.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e432.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e433.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e433.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e434.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e434.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e435.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e435.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e471.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e471.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e472.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e472.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e473.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e473.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e474.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e474.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e475.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e475.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e476.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e476.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e477.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e477.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e478.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e478.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e479.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e479.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e485.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e485.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e49.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e49.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e502.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e502.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e520.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e520.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e521.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e521.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e540.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e540.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e541.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e541.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e542.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e542.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e543.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e543.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e544.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e544.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e545.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e545.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e546.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e546.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e547.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e547.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e548.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e548.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e549.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e549.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e550.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e550.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e551.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e551.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e552.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e552.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e553.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e553.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e554.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e554.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e555.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e555.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e556.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e556.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e557.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e557.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e558.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e558.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e559.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e559.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e560.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e560.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e561.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e561.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e562.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e562.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e58.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e58.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e580.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e580.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e582.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e582.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e583.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e583.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e584.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e584.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e585.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e585.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e587.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e587.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e59.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e59.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e591.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e591.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e593.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e593.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e598.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e598.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e603.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e603.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e604.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e604.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e61.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e61.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e62.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e62.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e625.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e625.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e63.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e63.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e635.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e635.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e636.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e636.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e637.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e637.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e638.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e638.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e639.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e639.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e64.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e64.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e642.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e642.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e654.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e654.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e655.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e655.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e656.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e656.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e657.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e657.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e66.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e66.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e662.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e662.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e664.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e664.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e664ex.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e664ex.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e668.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e668.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e67.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e67.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e678.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e678.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e68.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e68.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e682.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e682.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e694.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e694.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e71.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e71.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e715.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e715.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e748.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e748.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e793.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e793.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e817.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e817.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e818.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e818.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e836.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e836.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e837.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e837.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e838.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e838.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e850.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e850.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e851.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e851.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e852.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e852.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e853.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e853.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e854.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e854.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e855.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e855.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e856.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e856.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e857.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e857.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e858.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e858.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e862.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e862.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e863.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e863.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e864.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e864.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e874.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e874.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e904.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e904.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/e908.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/e908.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ea61009.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ea61009.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ea61012.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ea61012.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ea81006.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ea81006.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ebambino7.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ebambino7.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ec863914.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ec863914.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/eh0009.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/eh0009.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/eh1070.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/eh1070.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/eh1090.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/eh1090.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/eh1590.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/eh1590.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/eh2010.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/eh2010.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/eh2012.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/eh2012.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/eh2070.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/eh2070.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/eh2510.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/eh2510.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/eh3012.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/eh3012.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/eiffel10.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/eiffel10.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/eiffel371.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/eiffel371.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/eiffel385.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/eiffel385.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/eiffel428.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/eiffel428.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/eiffel430.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/eiffel430.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/esa40.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/esa40.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/falcon.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/falcon.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fauvel.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fauvel.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fg1.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fg1.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fg2.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fg2.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fg3.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fg3.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fg4.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fg4.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx049915.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx049915.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx05188.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx05188.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx05191.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx05191.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx05h126.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx05h126.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx08s176.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx08s176.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx2.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx2.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx3.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx3.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx38153.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx38153.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx60100.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx60100.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx601001.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx601001.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx60100sm.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx60100sm.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx60126.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx60126.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx601261.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx601261.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx60157.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx60157.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx60160.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx60160.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx60177.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx60177.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx61140.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx61140.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx61147.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx61147.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx61163.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx61163.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx61168.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx61168.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx61184.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx61184.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx62k131.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx62k131.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx62k153.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx62k153.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx63100.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx63100.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx63110.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx63110.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx63120.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx63120.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx63137.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx63137.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx63137sm.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx63137sm.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx63143.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx63143.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx63145.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx63145.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx63147.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx63147.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx63158.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx63158.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx6617a2.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx6617a2.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx6617ai.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx6617ai.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx66182.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx66182.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx66196v.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx66196v.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx66a175.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx66a175.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx66h60.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx66h60.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx66h80.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx66h80.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx66s161.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx66s161.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx66s171.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx66s171.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx66s196.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx66s196.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx67k150.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx67k150.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx67k170.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx67k170.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx68h120.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx68h120.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx69274.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx69274.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx69h083.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx69h083.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx69h098.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx69h098.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx69pr281.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx69pr281.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx71089a.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx71089a.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx71120.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx71120.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx711520.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx711520.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx711525.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx711525.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx711530.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx711530.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx71l150.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx71l150.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx72150a.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx72150a.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx72150b.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx72150b.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx72ls160.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx72ls160.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx73170.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx73170.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx73170a.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx73170a.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx73cl1152.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx73cl1152.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx73cl2152.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx73cl2152.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx73cl3152.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx73cl3152.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx73k170.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx73k170.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx74080.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx74080.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx74130wp1.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx74130wp1.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx74130wp2.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx74130wp2.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx74130wp2mod.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx74130wp2mod.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx74cl5140.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx74cl5140.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx74cl6140.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx74cl6140.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx74modsm.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx74modsm.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx75141.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx75141.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx75193.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx75193.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx75vg166.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx75vg166.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx76100.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx76100.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx76120.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx76120.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx76mp120.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx76mp120.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx76mp140.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx76mp140.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx76mp160.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx76mp160.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx77080.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx77080.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx77w121.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx77w121.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx77w153.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx77w153.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx77w258.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx77w258.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx77w270.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx77w270.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx77w270s.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx77w270s.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx77w343.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx77w343.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx78k140.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx78k140.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx78k140a20.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx78k140a20.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx78k150.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx78k150.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx78k161.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx78k161.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx78pk188.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx78pk188.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx79k144.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx79k144.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx79l100.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx79l100.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx79l120.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx79l120.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx79w151a.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx79w151a.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx79w470a.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx79w470a.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx79w660a.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx79w660a.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx80080.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx80080.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx83w108.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx83w108.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx83w160.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx83w160.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx83w227.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx83w227.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx84w097.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx84w097.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx84w127.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx84w127.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx84w140.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx84w140.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx84w150.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx84w150.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx84w175.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx84w175.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fx84w218.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fx84w218.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fxl142k.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fxl142k.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fxlv152.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fxlv152.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fxm2.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fxm2.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fxs02196.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fxs02196.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fxs03182.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fxs03182.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/fxs21158.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/fxs21158.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/geminism.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/geminism.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/giiia.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/giiia.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/giiib.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/giiib.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/giiic.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/giiic.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/giiid.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/giiid.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/giiie.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/giiie.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/giiif.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/giiif.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/giiig.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/giiig.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/giiih.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/giiih.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/giiii.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/giiii.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/giiij.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/giiij.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/giiik.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/giiik.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/giiil.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/giiil.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/giiim.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/giiim.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/giiin.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/giiin.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/glennmartin2.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/glennmartin2.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/glennmartin3.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/glennmartin3.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/glennmartin4.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/glennmartin4.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/gm15sm.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/gm15sm.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe05k.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe05k.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe06k.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe06k.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe07k.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe07k.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe08k.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe08k.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe09k.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe09k.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe100.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe100.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe101.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe101.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe10k.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe10k.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe113.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe113.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe114.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe114.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe115.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe115.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe116.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe116.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe117.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe117.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe118.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe118.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe11k.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe11k.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe121.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe121.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe122.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe122.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe123.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe123.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe124.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe124.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe12k.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe12k.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe133.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe133.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe134.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe134.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe137.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe137.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe13k.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe13k.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe14.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe14.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe140.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe140.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe142.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe142.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe143.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe143.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe144.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe144.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe147.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe147.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe14k.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe14k.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe15.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe15.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe155.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe155.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe15k.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe15k.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe164.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe164.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe165.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe165.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe167.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe167.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe16k.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe16k.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe173.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe173.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe174.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe174.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe176.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe176.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe177.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe177.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe178.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe178.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe180.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe180.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe182.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe182.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe184.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe184.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe187.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe187.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe188.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe188.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe190.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe190.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe195.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe195.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe198.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe198.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe199.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe199.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe207.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe207.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe210.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe210.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe217.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe217.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe222.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe222.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe223.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe223.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe225.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe225.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe226.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe226.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe227.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe227.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe228.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe228.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe229.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe229.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe233.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe233.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe234.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe234.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe235.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe235.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe238.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe238.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe239.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe239.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe240.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe240.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe241.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe241.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe242.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe242.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe243.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe243.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe244.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe244.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe255.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe255.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe256.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe256.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe257.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe257.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe264.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe264.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe265.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe265.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe269.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe269.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe274.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe274.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe275.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe275.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe276.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe276.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe277.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe277.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe278.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe278.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe279.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe279.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe280.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe280.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe281.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe281.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe282.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe282.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe284.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe284.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe285.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe285.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe286.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe286.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe287.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe287.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe288.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe288.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe289.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe289.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe290.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe290.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe298.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe298.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe29b.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe29b.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe300.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe300.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe301.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe301.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe303.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe303.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe304.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe304.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe308.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe308.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe309.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe309.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe310.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe310.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe311.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe311.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe314.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe314.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe315.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe315.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe316.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe316.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe318.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe318.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe319.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe319.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe320.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe320.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe321.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe321.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe322.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe322.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe323.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe323.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe324.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe324.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe325.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe325.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe326.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe326.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe328.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe328.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe329.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe329.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe330.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe330.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe331.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe331.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe332.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe332.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe335.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe335.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe336.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe336.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe342.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe342.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe344.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe344.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe346.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe346.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe358.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe358.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe359.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe359.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe360.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe360.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe361.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe361.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe362.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe362.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe363.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe363.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe364.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe364.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe365.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe365.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe366.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe366.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe367.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe367.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe368.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe368.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe369.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe369.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe370.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe370.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe371.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe371.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe372.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe372.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe373.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe373.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe374.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe374.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe375.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe375.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe376.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe376.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe377.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe377.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe379.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe379.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe380.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe380.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe381.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe381.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe382.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe382.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe383.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe383.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe384.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe384.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe385.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe385.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe386.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe386.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe387.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe387.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe388.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe388.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe389.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe389.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe390.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe390.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe391.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe391.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe392.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe392.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe393.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe393.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe394.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe394.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe395.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe395.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe396.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe396.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe397.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe397.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe398.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe398.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe399.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe399.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe400.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe400.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe401.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe401.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe402.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe402.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe403.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe403.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe404.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe404.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe405.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe405.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe406.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe406.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe407.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe407.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe408.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe408.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe409.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe409.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe410.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe410.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe411.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe411.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe412.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe412.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe413.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe413.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe414.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe414.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe415.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe415.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe416a.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe416a.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe417.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe417.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe417a.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe417a.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe418.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe418.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe419.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe419.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe420.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe420.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe421.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe421.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe422.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe422.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe423.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe423.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe424.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe424.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe425.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe425.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe426.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe426.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe427.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe427.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe428.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe428.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe429.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe429.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe430.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe430.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe431.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe431.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe432.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe432.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe433.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe433.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe434.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe434.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe435.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe435.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe436.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe436.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe437.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe437.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe438.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe438.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe439.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe439.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe440.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe440.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe441.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe441.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe442.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe442.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe443.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe443.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe444.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe444.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe445.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe445.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe446.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe446.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe447.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe447.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe448.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe448.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe449.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe449.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe450.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe450.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe451.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe451.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe456.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe456.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe457.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe457.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe458.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe458.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe459.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe459.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe460.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe460.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe462.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe462.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe464.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe464.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe474.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe474.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe476.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe476.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe477.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe477.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe478.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe478.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe479.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe479.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe480.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe480.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe481.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe481.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe481a.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe481a.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe482.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe482.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe483.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe483.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe484.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe484.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe488.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe488.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe490.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe490.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe491.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe491.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe492.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe492.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe493.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe493.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe494.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe494.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe495.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe495.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe496.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe496.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe497.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe497.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe498.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe498.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe499.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe499.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe500.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe500.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe501.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe501.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe502.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe502.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe503.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe503.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe504.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe504.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe505.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe505.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe506.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe506.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe507.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe507.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe508.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe508.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe509.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe509.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe510.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe510.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe511.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe511.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe512.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe512.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe513.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe513.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe514.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe514.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe515.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe515.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe517.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe517.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe518.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe518.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe522.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe522.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe523.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe523.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe525.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe525.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe526.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe526.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe527.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe527.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe528.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe528.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe529.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe529.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe530.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe530.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe531.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe531.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe532.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe532.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe533.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe533.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe534.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe534.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe535.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe535.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe54.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe54.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe546.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe546.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe547.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe547.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe548.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe548.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe549.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe549.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe55.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe55.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe550.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe550.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe553.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe553.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe559.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe559.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe561.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe561.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe562.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe562.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe563.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe563.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe564.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe564.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe565.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe565.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe566.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe566.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe567.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe567.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe57.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe57.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe570.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe570.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe571.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe571.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe572.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe572.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe573.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe573.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe574.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe574.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe575.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe575.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe584.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe584.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe585.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe585.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe587.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe587.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe590.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe590.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe591.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe591.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe592.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe592.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe593.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe593.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe595.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe595.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe596.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe596.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe598.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe598.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe599.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe599.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe600.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe600.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe601.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe601.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe602.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe602.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe602m.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe602m.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe604.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe604.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe610b.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe610b.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe610bm.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe610bm.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe611.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe611.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe612.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe612.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe613.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe613.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe614.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe614.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe615.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe615.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe617.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe617.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe619.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe619.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe620.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe620.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe621.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe621.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe622.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe622.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe623.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe623.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe624.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe624.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe625.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe625.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe626.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe626.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe627.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe627.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe628.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe628.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe629.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe629.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe63.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe63.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe630.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe630.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe632.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe632.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe633.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe633.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe645.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe645.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe646.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe646.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe647.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe647.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe648.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe648.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe650.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe650.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe652.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe652.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe654.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe654.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe655.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe655.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe670.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe670.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe673.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe673.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe675.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe675.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe676.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe676.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe677.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe677.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe679.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe679.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe681.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe681.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe682.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe682.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe683.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe683.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe685.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe685.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe692.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe692.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe693.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe693.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe701.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe701.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe702.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe702.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe703.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe703.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe704.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe704.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe711.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe711.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe723.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe723.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe735.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe735.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe738.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe738.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe741.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe741.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe744.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe744.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe746.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe746.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe758.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe758.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe766.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe766.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe767.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe767.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe769.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe769.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe770.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe770.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe775.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe775.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe776.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe776.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe777.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe777.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe780.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe780.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe79.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe79.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe795.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe795.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe795sm.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe795sm.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe796.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe796.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe797.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe797.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe798.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe798.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe801.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe801.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe802.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe802.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe802a.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe802a.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe802b.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe802b.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe803h.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe803h.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe804.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe804.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe81.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe81.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/goe92.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/goe92.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/griffith30SymSuction.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/griffith30SymSuction.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/gs1.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/gs1.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/gu255118.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/gu255118.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/hh02.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/hh02.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/hobie.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/hobie.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/hobiesm.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/hobiesm.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/hq010.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/hq010.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/hq07.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/hq07.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/hq09.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/hq09.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/hq1010.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/hq1010.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/hq1012.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/hq1012.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/hq108.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/hq108.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/hq109.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/hq109.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/hq1510.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/hq1510.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/hq1511.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/hq1511.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/hq1512.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/hq1512.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/hq158.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/hq158.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/hq1585.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/hq1585.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/hq159.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/hq159.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/hq159b.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/hq159b.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/hq2010.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/hq2010.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/hq2012.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/hq2012.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/hq208.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/hq208.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/hq209.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/hq209.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/hq2090sm.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/hq2090sm.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/hq2195.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/hq2195.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/hq2510.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/hq2510.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/hq2511.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/hq2511.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/hq2512.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/hq2512.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/hq258.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/hq258.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/hq259.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/hq259.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/hq2590sm.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/hq2590sm.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/hq259b.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/hq259b.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/hq300gd2.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/hq300gd2.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/hq3010.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/hq3010.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/hq3011.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/hq3011.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/hq3012.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/hq3012.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/hq3013.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/hq3013.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/hq3014.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/hq3014.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/hq3015.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/hq3015.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/hq308.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/hq308.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/hq309.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/hq309.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/hq3510.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/hq3510.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/hq3512.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/hq3512.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/hq3513.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/hq3513.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/hq3514.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/hq3514.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/hq3518.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/hq3518.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/hq358.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/hq358.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/hq359.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/hq359.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/hsnlf213.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/hsnlf213.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ht05.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ht05.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ht08.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ht08.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ht12.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ht12.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ht22.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ht22.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ht23.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ht23.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/isa571.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/isa571.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/isa960.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/isa960.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/isa961.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/isa961.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/isa962.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/isa962.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/j5012.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/j5012.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/jn153.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/jn153.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/joukowsk.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/joukowsk.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/k1.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/k1.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/k2.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/k2.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/k3.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/k3.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/k3311.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/k3311.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/k3311sm.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/k3311sm.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/kc135a.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/kc135a.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/kc135b.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/kc135b.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/kc135c.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/kc135c.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/kc135d.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/kc135d.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/kenmar.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/kenmar.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/l188root.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/l188root.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/l188tip.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/l188tip.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/l7769.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/l7769.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/la203a.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/la203a.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/la2573a.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/la2573a.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/lds2.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/lds2.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/lg10sc.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/lg10sc.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/lnv109a.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/lnv109a.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/lrn1007.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/lrn1007.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ls013.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ls013.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ls413.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ls413.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ls413mod.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ls413mod.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ls417.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ls417.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ls417mod.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ls417mod.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ls421.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ls421.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ls421mod.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ls421mod.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/lwk79100.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/lwk79100.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/lwk80080.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/lwk80080.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/lwk80100.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/lwk80100.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/lwk80120k25.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/lwk80120k25.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/lwk80150k25.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/lwk80150k25.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/m1.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/m1.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/m10.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/m10.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/m11.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/m11.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/m12.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/m12.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/m13.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/m13.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/m14.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/m14.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/m15.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/m15.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/m16.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/m16.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/m17.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/m17.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/m18.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/m18.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/m19.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/m19.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/m2.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/m2.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/m20.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/m20.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/m21.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/m21.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/m22.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/m22.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/m23.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/m23.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/m24.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/m24.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/m25.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/m25.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/m26.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/m26.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/m27.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/m27.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/m3.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/m3.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/m4.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/m4.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/m5.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/m5.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/m6.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/m6.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/m665.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/m665.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/m685.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/m685.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/m7.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/m7.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/m8.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/m8.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/m9.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/m9.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ma409.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ma409.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ma409sm.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ma409sm.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/marsden.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/marsden.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/marske1.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/marske1.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/marske2.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/marske2.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/marske3.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/marske3.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/marske4.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/marske4.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/marske5.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/marske5.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/marske7.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/marske7.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/mb253515sm.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/mb253515sm.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/mh102.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/mh102.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/mh104.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/mh104.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/mh106.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/mh106.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/mh108.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/mh108.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/mh110.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/mh110.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/mh112.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/mh112.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/mh113.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/mh113.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/mh114.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/mh114.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/mh115.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/mh115.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/mh116.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/mh116.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/mh117.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/mh117.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/mh120.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/mh120.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/mh121.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/mh121.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/mh122.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/mh122.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/mh150.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/mh150.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/mh18.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/mh18.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/mh20.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/mh20.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/mh200.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/mh200.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/mh201.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/mh201.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/mh22.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/mh22.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/mh23.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/mh23.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/mh24.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/mh24.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/mh25.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/mh25.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/mh26.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/mh26.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/mh27.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/mh27.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/mh30.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/mh30.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/mh32.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/mh32.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/mh38.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/mh38.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/mh42.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/mh42.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/mh43.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/mh43.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/mh44.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/mh44.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/mh45.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/mh45.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/mh46.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/mh46.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/mh49.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/mh49.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/mh60.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/mh60.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/mh61.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/mh61.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/mh62.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/mh62.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/mh64.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/mh64.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/mh70.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/mh70.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/mh78.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/mh78.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/mh80.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/mh80.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/mh81.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/mh81.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/mh82.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/mh82.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/mh83.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/mh83.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/mh84.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/mh84.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/mh91.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/mh91.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/mh92.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/mh92.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/mh93.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/mh93.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/mh94.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/mh94.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/mh95.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/mh95.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/miley.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/miley.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/mrc-16.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/mrc-16.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/mrc-20.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/mrc-20.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ms313.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ms313.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ms317.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ms317.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/mue139.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/mue139.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/n0009sm.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/n0009sm.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/n0011sc.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/n0011sc.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/n0012.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/n0012.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/n10.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/n10.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/n11.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/n11.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/n11h9.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/n11h9.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/n12.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/n12.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/n13.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/n13.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/n14.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/n14.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/n1h15.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/n1h15.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/n22.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/n22.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/n24.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/n24.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/n2414.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/n2414.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/n2415.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/n2415.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/n2h15.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/n2h15.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/n5h10.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/n5h10.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/n5h15.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/n5h15.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/n5h20.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/n5h20.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/n63010a.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/n63010a.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/n63012a.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/n63012a.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/n63015a.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/n63015a.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/n63210.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/n63210.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/n63212.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/n63212.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/n63215.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/n63215.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/n63215b.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/n63215b.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/n63412.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/n63412.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/n63415.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/n63415.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/n64008a.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/n64008a.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/n64012.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/n64012.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/n64012a.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/n64012a.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/n64015.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/n64015.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/n64015a.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/n64015a.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/n6409.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/n6409.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/n64108.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/n64108.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/n64110.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/n64110.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/n64212.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/n64212.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/n64212ma.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/n64212ma.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/n64212mb.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/n64212mb.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/n64215.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/n64215.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/n642415.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/n642415.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/n66021.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/n66021.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/n6h10.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/n6h10.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/n6h15.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/n6h15.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/n6h20.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/n6h20.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/n8h12.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/n8h12.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/n9.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/n9.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/naca0006.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/naca0006.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/naca0008.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/naca0008.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/naca000834.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/naca000834.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/naca0010.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/naca0010.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/naca001034.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/naca001034.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/naca001034a08cli0.2.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/naca001034a08cli0.2.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/naca001035.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/naca001035.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/naca001064.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/naca001064.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/naca001065.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/naca001065.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/naca001066.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/naca001066.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/naca001234.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/naca001234.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/naca001264.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/naca001264.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/naca001264a08cli0.2.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/naca001264a08cli0.2.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/naca0015.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/naca0015.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/naca0018.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/naca0018.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/naca0021.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/naca0021.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/naca0024.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/naca0024.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/naca1.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/naca1.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/naca1408.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/naca1408.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/naca1410.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/naca1410.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/naca1412.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/naca1412.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/naca16006.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/naca16006.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/naca16009.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/naca16009.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/naca16012.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/naca16012.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/naca16015.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/naca16015.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/naca16018.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/naca16018.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/naca16021.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/naca16021.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/naca23012.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/naca23012.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/naca23015.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/naca23015.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/naca23018.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/naca23018.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/naca23021.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/naca23021.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/naca23024.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/naca23024.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/naca2408.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/naca2408.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/naca2410.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/naca2410.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/naca2411.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/naca2411.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/naca2415.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/naca2415.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/naca2418.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/naca2418.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/naca2421.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/naca2421.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/naca2424.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/naca2424.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/naca4412.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/naca4412.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/naca4415.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/naca4415.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/naca4418.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/naca4418.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/naca4421.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/naca4421.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/naca4424.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/naca4424.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/naca63206.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/naca63206.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/naca63209.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/naca63209.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/naca632615.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/naca632615.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/naca632a015.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/naca632a015.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/naca633018.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/naca633018.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/naca633218.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/naca633218.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/naca633418.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/naca633418.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/naca633618.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/naca633618.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/naca634221.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/naca634221.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/naca634421.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/naca634421.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/naca63a210.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/naca63a210.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/naca641112.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/naca641112.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/naca6412.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/naca6412.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/naca64206.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/naca64206.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/naca64208.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/naca64208.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/naca64209.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/naca64209.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/naca64210.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/naca64210.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/naca642215.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/naca642215.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/naca642415.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/naca642415.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/naca643218.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/naca643218.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/naca643418.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/naca643418.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/naca643618.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/naca643618.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/naca644221.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/naca644221.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/naca644421.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/naca644421.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/naca64a010.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/naca64a010.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/naca64a210.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/naca64a210.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/naca64a410.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/naca64a410.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/naca651212.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/naca651212.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/naca651212a06.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/naca651212a06.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/naca651412.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/naca651412.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/naca65206.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/naca65206.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/naca65209.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/naca65209.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/naca65210.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/naca65210.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/naca652215.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/naca652215.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/naca652415.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/naca652415.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/naca652415a05.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/naca652415a05.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/naca653218.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/naca653218.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/naca65410.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/naca65410.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/naca654221.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/naca654221.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/naca654421.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/naca654421.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/naca654421a05.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/naca654421a05.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/naca66-018.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/naca66-018.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/naca661212.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/naca661212.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/naca66206.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/naca66206.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/naca66209.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/naca66209.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/naca66210.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/naca66210.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/naca662215.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/naca662215.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/naca662415.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/naca662415.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/naca663218.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/naca663218.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/naca663418.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/naca663418.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/naca664221.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/naca664221.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/naca671215.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/naca671215.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/naca747a315.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/naca747a315.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/naca747a415.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/naca747a415.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/nacacyh.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/nacacyh.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/nacam12.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/nacam12.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/nacam18.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/nacam18.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/nacam2.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/nacam2.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/nacam3.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/nacam3.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/nacam6.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/nacam6.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/nasasc2-0714.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/nasasc2-0714.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ncambre.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ncambre.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/nl722343.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/nl722343.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/nl722362.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/nl722362.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/nlf0115.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/nlf0115.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/nlf0215f.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/nlf0215f.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/nlf1015.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/nlf1015.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/nlf414f.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/nlf414f.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/nlf415.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/nlf415.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/nlf416.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/nlf416.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/nlr1t.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/nlr1t.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/nlr7301.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/nlr7301.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/nn7mk20.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/nn7mk20.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/npl9510.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/npl9510.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/npl9615.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/npl9615.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/npl9626.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/npl9626.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/npl9627.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/npl9627.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/npl9660.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/npl9660.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/nplx.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/nplx.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/oa206.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/oa206.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/oa209.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/oa209.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/oa212.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/oa212.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/oa213.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/oa213.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/oaf095.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/oaf095.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/oaf102.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/oaf102.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/oaf117.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/oaf117.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/oaf128.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/oaf128.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/oaf139.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/oaf139.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/p51droot.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/p51droot.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/p51dtip.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/p51dtip.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/p51hroot.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/p51hroot.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/p51htip.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/p51htip.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/pfcm.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/pfcm.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/pmc19sm.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/pmc19sm.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/prandtldroot.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/prandtldroot.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/prandtldtip.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/prandtldtip.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/psu-90-125wl.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/psu-90-125wl.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/psu94097.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/psu94097.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/pt40.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/pt40.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/r1046.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/r1046.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/r1080.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/r1080.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/r1082.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/r1082.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/r1082t.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/r1082t.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/r140.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/r140.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/r140sm.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/r140sm.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/rae100.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/rae100.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/rae101.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/rae101.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/rae102.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/rae102.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/rae103.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/rae103.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/rae104.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/rae104.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/rae2822.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/rae2822.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/rae5212.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/rae5212.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/rae5213.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/rae5213.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/rae5214.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/rae5214.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/rae5215.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/rae5215.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/rae69ck.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/rae69ck.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/raf15.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/raf15.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/raf19.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/raf19.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/raf25.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/raf25.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/raf26.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/raf26.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/raf27.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/raf27.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/raf28.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/raf28.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/raf30.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/raf30.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/raf30md.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/raf30md.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/raf31.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/raf31.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/raf32.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/raf32.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/raf32md.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/raf32md.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/raf33.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/raf33.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/raf34.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/raf34.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/raf38.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/raf38.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/raf48.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/raf48.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/raf6.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/raf6.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/raf69.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/raf69.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/raf89.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/raf89.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/rc0864c.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/rc0864c.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/rc08b3.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/rc08b3.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/rc08n1.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/rc08n1.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/rc1064c.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/rc1064c.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/rc10b3.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/rc10b3.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/rc10n1.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/rc10n1.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/rc1264c.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/rc1264c.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/rc12b3.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/rc12b3.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/rc12n1.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/rc12n1.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/rc410.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/rc410.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/rc510.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/rc510.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/rcsc2.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/rcsc2.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/rg12.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/rg12.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/rg12a.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/rg12a.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/rg12a189.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/rg12a189.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/rg14.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/rg14.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/rg1410.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/rg1410.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/rg149.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/rg149.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/rg1495.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/rg1495.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/rg14a147.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/rg14a147.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/rg15.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/rg15.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/rg15a111.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/rg15a111.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/rg15a213.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/rg15a213.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/rg8.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/rg8.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/rhodesg30.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/rhodesg30.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/rhodesg32.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/rhodesg32.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/rhodesg34.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/rhodesg34.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/rhodesg36.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/rhodesg36.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/s1010.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/s1010.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/s1012.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/s1012.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/s1014.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/s1014.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/s1016.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/s1016.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/s1020.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/s1020.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/s1046.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/s1046.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/s1048.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/s1048.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/s1091.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/s1091.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/s1210.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/s1210.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/s1221.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/s1221.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/s1223.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/s1223.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/s1223rtl.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/s1223rtl.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/s2027.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/s2027.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/s2046.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/s2046.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/s2048.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/s2048.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/s2050.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/s2050.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/s2055.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/s2055.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/s2060.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/s2060.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/s2062.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/s2062.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/s2091.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/s2091.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/s3.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/s3.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/s3002.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/s3002.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/s3010.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/s3010.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/s3014.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/s3014.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/s3016.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/s3016.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/s3021.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/s3021.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/s3024.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/s3024.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/s3025.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/s3025.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/s4022.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/s4022.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/s4053.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/s4053.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/s4061.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/s4061.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/s4062.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/s4062.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/s4083.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/s4083.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/s4110.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/s4110.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/s4158.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/s4158.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/s4180.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/s4180.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/s4233.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/s4233.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/s4310.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/s4310.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/s4320.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/s4320.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/s5010.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/s5010.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/s5020.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/s5020.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/s6061.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/s6061.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/s6062.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/s6062.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/s6063.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/s6063.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/s7012.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/s7012.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/s7055.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/s7055.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/s7075.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/s7075.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/s8025.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/s8025.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/s8035.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/s8035.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/s8036.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/s8036.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/s8037.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/s8037.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/s8038.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/s8038.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/s8052.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/s8052.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/s8055.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/s8055.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/s9000.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/s9000.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/s9026.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/s9026.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/s9027.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/s9027.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/s9032.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/s9032.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/s9033.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/s9033.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/s9037.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/s9037.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/sa7035.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/sa7035.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/sa7036.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/sa7036.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/sa7038.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/sa7038.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/saratov.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/saratov.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/sc1012r8.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/sc1012r8.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/sc1094r8.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/sc1094r8.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/sc1095.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/sc1095.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/sc1095r8.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/sc1095r8.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/sc20010.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/sc20010.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/sc20012.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/sc20012.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/sc20402.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/sc20402.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/sc20403.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/sc20403.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/sc20404.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/sc20404.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/sc20406.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/sc20406.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/sc20410.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/sc20410.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/sc20412.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/sc20412.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/sc20414.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/sc20414.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/sc20503.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/sc20503.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/sc20518.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/sc20518.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/sc20606.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/sc20606.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/sc20610.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/sc20610.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/sc20612.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/sc20612.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/sc20614.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/sc20614.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/sc20706.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/sc20706.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/sc20710.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/sc20710.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/sc20712.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/sc20712.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/sc20714.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/sc20714.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/sc21006.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/sc21006.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/sc21010.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/sc21010.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/sc2110.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/sc2110.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/sd2030.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/sd2030.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/sd2083.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/sd2083.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/sd5060.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/sd5060.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/sd6060.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/sd6060.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/sd6080.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/sd6080.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/sd7003.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/sd7003.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/sd7032.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/sd7032.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/sd7034.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/sd7034.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/sd7037.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/sd7037.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/sd7043.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/sd7043.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/sd7062.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/sd7062.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/sd7080.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/sd7080.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/sd7084.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/sd7084.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/sd7090.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/sd7090.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/sd8000.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/sd8000.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/sd8020.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/sd8020.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/sd8040.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/sd8040.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/sg6040.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/sg6040.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/sg6041.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/sg6041.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/sg6042.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/sg6042.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/sg6043.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/sg6043.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/sg6050.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/sg6050.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/sg6051.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/sg6051.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/sm701.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/sm701.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/sokolov.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/sokolov.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/spicasm.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/spicasm.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ssca07.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ssca07.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ssca09.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ssca09.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/stcyr171.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/stcyr171.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/stcyr172.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/stcyr172.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/stcyr234.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/stcyr234.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/stcyr24.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/stcyr24.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ste87151.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ste87151.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ste87391.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ste87391.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/stf86361.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/stf86361.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/strand.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/strand.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/tempest1.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/tempest1.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/tempest2.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/tempest2.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/tempest3.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/tempest3.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/th25816.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/th25816.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/trainer60.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/trainer60.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/tsagi12.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/tsagi12.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/tsagi8.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/tsagi8.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ua2-180.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ua2-180.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ua2-180sm.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ua2-180sm.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ua79sf18.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ua79sf18.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ua79sff.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ua79sff.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ua79sfm.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ua79sfm.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/uag8814320.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/uag8814320.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ui1720.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ui1720.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ultimate.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ultimate.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/us1000root.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/us1000root.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/usa22.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/usa22.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/usa25.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/usa25.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/usa26.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/usa26.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/usa27.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/usa27.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/usa27m2.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/usa27m2.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/usa28.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/usa28.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/usa29.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/usa29.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/usa31.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/usa31.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/usa32.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/usa32.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/usa33.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/usa33.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/usa34.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/usa34.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/usa35.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/usa35.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/usa35a.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/usa35a.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/usa35b.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/usa35b.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/usa40.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/usa40.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/usa40b.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/usa40b.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/usa41.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/usa41.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/usa45.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/usa45.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/usa45m.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/usa45m.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/usa46.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/usa46.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/usa48.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/usa48.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/usa49.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/usa49.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/usa5.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/usa5.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/usa50.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/usa50.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/usa51.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/usa51.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/usa98.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/usa98.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/usnps4.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/usnps4.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/v13006.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/v13006.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/v13009.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/v13009.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/v23010.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/v23010.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/v43012.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/v43012.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/v43015.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/v43015.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/vr1.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/vr1.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/vr11x.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/vr11x.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/vr12.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/vr12.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/vr13.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/vr13.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/vr14.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/vr14.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/vr15.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/vr15.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/vr5.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/vr5.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/vr7.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/vr7.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/vr7b.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/vr7b.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/vr8.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/vr8.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/vr8b.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/vr8b.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/vr9.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/vr9.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/waspsm.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/waspsm.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/wb13535sm.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/wb13535sm.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/wb140.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/wb140.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/whitcomb.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/whitcomb.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ys900.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ys900.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ys915.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ys915.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/airfoils/ys930.dat` & `PteraSoftware-3.0.0/pterasoftware/airfoils/ys930.dat`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/convergence.py` & `PteraSoftware-3.0.0/pterasoftware/convergence.py`

 * *Files 9% similar despite different names*

```diff
@@ -341,16 +341,16 @@
                 )
             else:
                 convergence_logger.info(
                     "\t\tMaximum coefficient change from panel aspect ratio: "
                     + str(max_ar_pc)
                 )
 
-            # If this isn't the first number of chordwise panels, the number of
-            # chordwise panels APE.
+            # If this isn't the first number of chordwise panels, calculate the
+            # number of chordwise panels APE.
             if chord_id > 0:
                 last_chord_force_coefficients = force_coefficients[
                     ar_id, chord_id - 1, :
                 ]
                 last_chord_moment_coefficients = moment_coefficients[
                     ar_id, chord_id - 1, :
                 ]
@@ -463,22 +463,24 @@
     # If all iterations have been checked and none of them resulted in both
     # convergence parameters passing, then indicate that no converged solution was
     # found and return values of None for the converged parameters.
     convergence_logger.info("The analysis did not find a converged mesh.")
     return [None, None]
 
 
+# ToDo: Add the new parameters to the documentation.
 def analyze_unsteady_convergence(
     ref_problem,
     prescribed_wake=True,
     free_wake=True,
-    num_cycles_bounds=(1, 4),
+    num_cycles_bounds=(2, 4),
     num_chords_bounds=(3, 7),
     panel_aspect_ratio_bounds=(4, 1),
     num_chordwise_panels_bounds=(3, 12),
+    coefficient_mask=None,
     convergence_criteria=5.0,
 ):
     """This function finds the converged parameters of an unsteady problem.
 
     Convergence is found by varying if the solver's wake state (prescribed or free),
     the final length of the problem's wake (in number of chord lengths for static
     geometry and number of flap cycles for variable geometry), the airplanes' panel
@@ -573,14 +575,19 @@
 
     ref_movement = ref_problem.movement
     is_static = ref_movement.get_max_period() == 0
 
     ref_airplane_movements = ref_movement.airplane_movements
     ref_operating_point_movement = ref_movement.operating_point_movement
 
+    if coefficient_mask is None:
+        coefficient_mask = [True, True, True, True, True, True]
+
+    num_coefficients = coefficient_mask.count(True)
+
     wake_list = []
     if prescribed_wake:
         wake_list.append(True)
     if free_wake:
         wake_list.append(False)
 
     # If this problem has static geometry, base the wake length on the number of
@@ -605,30 +612,22 @@
         (
             len(wake_list),
             len(wake_lengths_list),
             len(panel_aspect_ratios_list),
             len(num_chordwise_panels_list),
         )
     )
-    force_coefficients = np.zeros(
-        (
-            len(wake_list),
-            len(wake_lengths_list),
-            len(panel_aspect_ratios_list),
-            len(num_chordwise_panels_list),
-            len(ref_airplane_movements),
-        )
-    )
-    moment_coefficients = np.zeros(
+    coefficients = np.zeros(
         (
             len(wake_list),
             len(wake_lengths_list),
             len(panel_aspect_ratios_list),
             len(num_chordwise_panels_list),
             len(ref_airplane_movements),
+            num_coefficients,
         )
     )
 
     iteration = 0
     num_iterations = (
         len(wake_list)
         * len(wake_lengths_list)
@@ -962,36 +961,50 @@
                         calculate_streamlines=False,
                     )
                     iter_stop = time.time()
                     this_iter_time = iter_stop - iter_start
 
                     # Create and fill arrays with each of this iteration's airplane's
                     # resultant force and moment coefficients.
-                    these_force_coefficients = np.zeros(len(these_airplane_movements))
-                    these_moment_coefficients = np.zeros(len(these_airplane_movements))
+                    these_coefficients = np.zeros(
+                        (len(these_airplane_movements), num_coefficients)
+                    )
                     for airplane_id, airplane in enumerate(these_airplane_movements):
-                        these_force_coefficients[airplane_id] = np.linalg.norm(
-                            this_problem.final_total_near_field_force_coefficients_wind_axes[
+
+                        # If this problem is static, then get it's final load
+                        # coefficients. If it's variable, get the final RMS load
+                        # coefficients.
+                        if is_static:
+                            all_force_coefficients = this_problem.final_near_field_force_coefficients_wind_axes[
                                 airplane_id
                             ]
-                        )
-                        these_moment_coefficients[airplane_id] = np.linalg.norm(
-                            this_problem.final_total_near_field_moment_coefficients_wind_axes[
+                            all_moment_coefficients = this_problem.final_near_field_moment_coefficients_wind_axes[
+                                airplane_id
+                            ]
+                        else:
+                            all_force_coefficients = this_problem.final_rms_near_field_force_coefficients_wind_axes[
                                 airplane_id
                             ]
+                            all_moment_coefficients = this_problem.final_rms_near_field_moment_coefficients_wind_axes[
+                                airplane_id
+                            ]
+
+                        all_coefficients = np.concatenate(
+                            [all_force_coefficients, all_moment_coefficients]
                         )
 
+                        these_coefficients[airplane_id] = all_coefficients[
+                            coefficient_mask
+                        ]
+
                     # Populate the arrays that store information of all the
                     # iterations with the data from this iteration.
-                    force_coefficients[
-                        wake_id, length_id, ar_id, chord_id, :
-                    ] = these_force_coefficients
-                    moment_coefficients[
-                        wake_id, length_id, ar_id, chord_id, :
-                    ] = these_moment_coefficients
+                    coefficients[
+                        wake_id, length_id, ar_id, chord_id, :, :
+                    ] = these_coefficients
                     iter_times[wake_id, length_id, ar_id, chord_id] = this_iter_time
 
                     convergence_logger.info(
                         "\t\t\t\tIteration Time: "
                         + str(round(this_iter_time, 3))
                         + " s"
                     )
@@ -999,82 +1012,48 @@
                     max_wake_pc = np.inf
                     max_length_pc = np.inf
                     max_ar_pc = np.inf
                     max_chord_pc = np.inf
 
                     # If this isn't the first wake state, calculate the wake state APE.
                     if wake_id > 0:
-                        last_wake_force_coefficients = force_coefficients[
-                            wake_id - 1, length_id, ar_id, chord_id, :
-                        ]
-                        last_wake_moment_coefficients = moment_coefficients[
-                            wake_id - 1, length_id, ar_id, chord_id, :
+                        last_wake_coefficients = coefficients[
+                            wake_id - 1, length_id, ar_id, chord_id, :, :
                         ]
-                        max_wake_force_pc = max(
+                        max_wake_pc = np.max(
                             100
                             * np.abs(
-                                (
-                                    these_force_coefficients
-                                    - last_wake_force_coefficients
-                                )
-                                / last_wake_force_coefficients
+                                (these_coefficients - last_wake_coefficients)
+                                / last_wake_coefficients
                             )
                         )
-                        max_wake_moment_pc = max(
-                            100
-                            * np.abs(
-                                (
-                                    these_moment_coefficients
-                                    - last_wake_moment_coefficients
-                                )
-                                / last_wake_moment_coefficients
-                            )
-                        )
-                        max_wake_pc = max(max_wake_force_pc, max_wake_moment_pc)
 
                         convergence_logger.info(
                             "\t\t\t\tMaximum coefficient change from wake type: "
                             + str(round(max_wake_pc, 2))
                             + "%"
                         )
                     else:
                         convergence_logger.info(
                             "\t\t\t\tMaximum coefficient change from wake type: "
                             + str(max_wake_pc)
                         )
 
                     # If this isn't the first wake length, calculate the wake state APE.
                     if length_id > 0:
-                        last_length_force_coefficients = force_coefficients[
-                            wake_id, length_id - 1, ar_id, chord_id, :
+                        last_length_coefficients = coefficients[
+                            wake_id, length_id - 1, ar_id, chord_id, :, :
                         ]
-                        last_length_moment_coefficients = moment_coefficients[
-                            wake_id, length_id - 1, ar_id, chord_id, :
-                        ]
-                        max_length_force_pc = max(
-                            100
-                            * np.abs(
-                                (
-                                    these_force_coefficients
-                                    - last_length_force_coefficients
-                                )
-                                / last_length_force_coefficients
-                            )
-                        )
-                        max_length_moment_pc = max(
+                        max_length_pc = np.max(
                             100
                             * np.abs(
-                                (
-                                    these_moment_coefficients
-                                    - last_length_moment_coefficients
-                                )
-                                / last_length_moment_coefficients
+                                (these_coefficients - last_length_coefficients)
+                                / last_length_coefficients
                             )
                         )
-                        max_length_pc = max(max_length_force_pc, max_length_moment_pc)
 
                         convergence_logger.info(
                             "\t\t\t\tMaximum coefficient change from wake length: "
                             + str(round(max_length_pc, 2))
                             + "%"
                         )
                     else:
@@ -1082,79 +1061,48 @@
                             "\t\t\t\tMaximum coefficient change from wake length: "
                             + str(max_length_pc)
                         )
 
                     # If this isn't the first panel aspect ratio, calculate the panel
                     # aspect ratio APE.
                     if ar_id > 0:
-                        last_ar_force_coefficients = force_coefficients[
-                            wake_id, length_id, ar_id - 1, chord_id, :
-                        ]
-                        last_ar_moment_coefficients = moment_coefficients[
-                            wake_id, length_id, ar_id - 1, chord_id, :
+                        last_ar_coefficients = coefficients[
+                            wake_id, length_id, ar_id - 1, chord_id, :, :
                         ]
-                        max_ar_force_pc = max(
+                        max_ar_pc = np.max(
                             100
                             * np.abs(
-                                (these_force_coefficients - last_ar_force_coefficients)
-                                / last_ar_force_coefficients
+                                (these_coefficients - last_ar_coefficients)
+                                / last_ar_coefficients
                             )
                         )
-                        max_ar_moment_pc = max(
-                            100
-                            * np.abs(
-                                (
-                                    these_moment_coefficients
-                                    - last_ar_moment_coefficients
-                                )
-                                / last_ar_moment_coefficients
-                            )
-                        )
-                        max_ar_pc = max(max_ar_force_pc, max_ar_moment_pc)
 
                         convergence_logger.info(
                             "\t\t\t\tMaximum coefficient change from panel aspect "
                             "ratio: " + str(round(max_ar_pc, 2)) + "%"
                         )
                     else:
                         convergence_logger.info(
                             "\t\t\t\tMaximum coefficient change from panel aspect "
                             "ratio: " + str(max_ar_pc)
                         )
 
-                    # If this isn't the first number of chordwise panels, the number
-                    # of chordwise panels APE.
+                    # If this isn't the first number of chordwise panels, calculate
+                    # the number of chordwise panels APE.
                     if chord_id > 0:
-                        last_chord_force_coefficients = force_coefficients[
-                            wake_id, length_id, ar_id, chord_id - 1, :
-                        ]
-                        last_chord_moment_coefficients = moment_coefficients[
-                            wake_id, length_id, ar_id, chord_id - 1, :
+                        last_chord_coefficients = coefficients[
+                            wake_id, length_id, ar_id, chord_id - 1, :, :
                         ]
-                        max_chord_force_pc = max(
+                        max_chord_pc = np.max(
                             100
                             * np.abs(
-                                (
-                                    these_force_coefficients
-                                    - last_chord_force_coefficients
-                                )
-                                / last_chord_force_coefficients
-                            )
-                        )
-                        max_chord_moment_pc = max(
-                            100
-                            * np.abs(
-                                (
-                                    these_moment_coefficients
-                                    - last_chord_moment_coefficients
-                                )
-                                / last_chord_moment_coefficients
+                                (these_coefficients - last_chord_coefficients)
+                                / last_chord_coefficients
                             )
                         )
-                        max_chord_pc = max(max_chord_force_pc, max_chord_moment_pc)
 
                         convergence_logger.info(
                             "\t\t\t\tMaximum coefficient change from chordwise panels: "
                             + str(round(max_chord_pc, 2))
                             + "%"
                         )
                     else:
```

### Comparing `PteraSoftware-2.2.1/pterasoftware/functions.py` & `PteraSoftware-3.0.0/pterasoftware/functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -543,17 +543,16 @@
     :param airplane: Airplane
         This is the Airplane object to which the Panel object belongs.
     :return:
     """
 
     # Update the solver's list of attributes with this panel's attributes.
     solver.panels[global_panel_position] = panel
-    solver.panel_normal_directions[global_panel_position, :] = panel.normal_direction
+    solver.panel_normal_directions[global_panel_position, :] = panel.unit_normal
     solver.panel_areas[global_panel_position] = panel.area
-    solver.panel_centers[global_panel_position] = panel.center
     solver.panel_collocation_points[global_panel_position, :] = panel.collocation_point
     solver.panel_back_right_vortex_vertices[
         global_panel_position, :
     ] = panel.ring_vortex.right_leg.origin
     solver.panel_front_right_vortex_vertices[
         global_panel_position, :
     ] = panel.ring_vortex.right_leg.termination
```

### Comparing `PteraSoftware-2.2.1/pterasoftware/geometry.py` & `PteraSoftware-3.0.0/pterasoftware/geometry.py`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/meshing.py` & `PteraSoftware-3.0.0/pterasoftware/meshing.py`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/movement.py` & `PteraSoftware-3.0.0/pterasoftware/movement.py`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/operating_point.py` & `PteraSoftware-3.0.0/pterasoftware/operating_point.py`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/output.py` & `PteraSoftware-3.0.0/pterasoftware/output.py`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/panel.py` & `PteraSoftware-3.0.0/pterasoftware/panel.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,17 +7,16 @@
     None
 
 This module contains the following functions:
     None
 """
 import numpy as np
 
-from . import functions
-
 
+# ToDo: Update the list of methods for this class.
 class Panel:
     """This class is used to contain the panels of a wing.
 
     This class contains the following public methods:
         calculate_collocation_point_location: This method calculates the location of
         the collocation point.
 
@@ -81,113 +80,132 @@
         # Initialize variables to hold attributes that describe the panel's position
         # in its wing's panel matrix. They will be populated by the meshing function.
         self.is_right_edge = None
         self.is_left_edge = None
         self.local_chordwise_position = None
         self.local_spanwise_position = None
 
-        # Initialize a variable to hold the position of the wing (who this panel
-        # belongs to) in the airplane's wing list. This will be populated by the
-        # airplane object.
-        self.wing_position = None
-
         # Initialize variables to hold the panel's ring and horseshoe vortices. These
         # will be populated by the solver.
         self.ring_vortex = None
         self.horseshoe_vortex = None
 
-        # Initialize a variable to hold the collocation point location and then
-        # populate it.
-        self.collocation_point = None
-        self.calculate_collocation_point_location()
-
-        # Initialize variables to hold the panel area and the panel normal vector at
-        # the collocation point. Then populate them.
-        self.area = None
-        self.normal_direction = None
-        self.calculate_area_and_normal()
-
-        # Calculate the center of the panel.
-        self.center = functions.numba_centroid_of_quadrilateral(
-            front_right_vertex, front_left_vertex, back_left_vertex, back_right_vertex
-        )
-
-        # Calculate the front and back leg lengths, then use them to find and
-        # populate the average panel width.
-        front_leg_length = np.linalg.norm(front_left_vertex - front_right_vertex)
-        back_leg_length = np.linalg.norm(back_right_vertex - back_left_vertex)
-        self.width = (front_leg_length + back_leg_length) / 2
-
-        # Initialize two variables that are along the panel's left and right legs at
-        # the quarter chord. These points are used for all types of solvers,
-        # so we will define them here.
-        self.front_right_vortex_vertex = self.front_right_vertex + 0.25 * (
-            self.back_right_vertex - self.front_right_vertex
-        )
-        self.front_left_vortex_vertex = self.front_left_vertex + 0.25 * (
-            self.back_left_vertex - self.front_left_vertex
-        )
-
         # Initialize variables to hold attributes of the panel that will be defined
         # after the solver finds a solution.
         self.near_field_force_geometry_axes = None
         self.near_field_moment_geometry_axes = None
         self.near_field_force_wind_axes = None
         self.near_field_moment_wind_axes = None
         self.induced_drag_coefficient = None
         self.side_force_coefficient = None
         self.lift_coefficient = None
 
-    def calculate_collocation_point_location(self):
-        """This method calculates the location of the collocation point.
-
-        The collocation point is at the panel's three-quarter chord point.
-
-        :return: None
-        """
-
+    # ToDo: Update this method's documentation.
+    @property
+    def right_leg(self):
+        return self.front_right_vertex - self.back_right_vertex
+
+    # ToDo: Update this method's documentation.
+    @property
+    def front_leg(self):
+        return self.front_left_vertex - self.front_right_vertex
+
+    # ToDo: Update this method's documentation.
+    @property
+    def left_leg(self):
+        return self.back_left_vertex - self.front_left_vertex
+
+    # ToDo: Update this method's documentation.
+    @property
+    def back_leg(self):
+        return self.back_right_vertex - self.back_left_vertex
+
+    # ToDo: Update this method's documentation.
+    @property
+    def front_right_vortex_vertex(self):
+        return self.back_right_vertex + 0.75 * self.right_leg
+
+    # ToDo: Update this method's documentation.
+    @property
+    def front_left_vortex_vertex(self):
+        return self.front_left_vertex + 0.25 * self.left_leg
+
+    # ToDo: Update this method's documentation.
+    @property
+    def collocation_point(self):
         # Find the location of points three quarters of the way down the left and
         # right legs of the panel.
-        right_three_quarter_chord_mark = self.front_right_vertex + 0.75 * (
-            self.back_right_vertex - self.front_right_vertex
-        )
-        left_three_quarter_chord_mark = self.front_left_vertex + 0.75 * (
-            self.back_left_vertex - self.front_left_vertex
-        )
+        right_three_quarter_chord_mark = self.back_right_vertex + 0.25 * self.right_leg
+        left_three_quarter_chord_mark = self.front_left_vertex + 0.75 * self.left_leg
 
         # Find the vector between the points three quarters of the way down the left
         # and right legs of the panel.
         three_quarter_chord_vector = (
             left_three_quarter_chord_mark - right_three_quarter_chord_mark
         )
 
         # Find the collocation point, which is halfway between the points three
         # quarters of the way down the left and right legs of the panel. Then
         # populate the class attribute.
-        self.collocation_point = (
-            right_three_quarter_chord_mark + 0.5 * three_quarter_chord_vector
-        )
-
-    def calculate_area_and_normal(self):
-        """This method calculates the panel's area and the panel's normal unit vector.
-
-        This method makes the assumption that the panel is planar. This is
-        technically incorrect for wing's with twist but is a good approximation for
-        small panels.
-
-        :return: None
-        """
+        return right_three_quarter_chord_mark + 0.5 * three_quarter_chord_vector
 
-        # Calculate panel's normal unit vector and its area via its diagonals.
-        first_diagonal = self.front_right_vertex - self.back_left_vertex
-        second_diagonal = self.front_left_vertex - self.back_right_vertex
-        cross_product = np.cross(first_diagonal, second_diagonal)
-        cross_product_magnitude = np.linalg.norm(cross_product)
-        self.normal_direction = cross_product / cross_product_magnitude
-        self.area = cross_product_magnitude / 2
+    # ToDo: Update this method's documentation.
+    @property
+    def area(self):
+        return np.linalg.norm(self._cross) / 2
+
+    # ToDo: Update this method's documentation.
+    @property
+    def unit_normal(self):
+        return self._cross / np.linalg.norm(self._cross)
+
+    # ToDo: Update this method's documentation.
+    @property
+    def unit_spanwise(self):
+        front_spanwise = -self.front_leg
+        back_spanwise = self.back_leg
+        spanwise = (front_spanwise + back_spanwise) / 2
+        return spanwise / np.linalg.norm(spanwise)
+
+    # ToDo: Update this method's documentation.
+    @property
+    def average_span(self):
+        front_leg_length = np.linalg.norm(self.front_leg)
+        back_leg_length = np.linalg.norm(self.back_leg)
+        return (front_leg_length + back_leg_length) / 2
+
+    # ToDo: Update this method's documentation.
+    @property
+    def unit_chordwise(self):
+        right_chordwise = -self.right_leg
+        left_chordwise = self.left_leg
+        chordwise = (right_chordwise + left_chordwise) / 2
+        return chordwise / np.linalg.norm(chordwise)
+
+    # ToDo: Update this method's documentation.
+    @property
+    def average_chord(self):
+        right_leg_length = np.linalg.norm(self.right_leg)
+        left_leg_length = np.linalg.norm(self.left_leg)
+        return (right_leg_length + left_leg_length) / 2
+
+    # ToDo: Update this method's documentation.
+    @property
+    def _first_diagonal(self):
+        return self.front_right_vertex - self.back_left_vertex
+
+    # ToDo: Update this method's documentation.
+    @property
+    def _second_diagonal(self):
+        return self.front_left_vertex - self.back_right_vertex
+
+    # ToDo: Update this method's documentation.
+    @property
+    def _cross(self):
+        return np.cross(self._first_diagonal, self._second_diagonal)
 
     def calculate_normalized_induced_velocity(self, point):
         """This method calculates the velocity induced at a point by this panel's
         vortices, assuming a unit vortex strength.
 
         This method does not include the effect of the panel's wake vortices.
```

### Comparing `PteraSoftware-2.2.1/pterasoftware/problems.py` & `PteraSoftware-3.0.0/pterasoftware/problems.py`

 * *Files 10% similar despite different names*

```diff
@@ -90,20 +90,37 @@
         # the first step to calculate results to the first averaging step. Otherwise,
         # set it to the zero, which is the first time step.
         if self.only_final_results:
             self.first_results_step = self.first_averaging_step
         else:
             self.first_results_step = 0
 
-        # Initialize empty lists to hold the final force, moment, force coefficients,
-        # and moment coefficients this each airplane object experiences.
-        self.final_total_near_field_forces_wind_axes = []
-        self.final_total_near_field_force_coefficients_wind_axes = []
-        self.final_total_near_field_moments_wind_axes = []
-        self.final_total_near_field_moment_coefficients_wind_axes = []
+        # Initialize empty lists to hold the final loads and load coefficients each
+        # airplane object experiences. These will only be populated for static
+        # geometry problems.
+        self.final_near_field_forces_wind_axes = []
+        self.final_near_field_force_coefficients_wind_axes = []
+        self.final_near_field_moments_wind_axes = []
+        self.final_near_field_moment_coefficients_wind_axes = []
+
+        # Initialize empty lists to hold the final cycle-averaged loads and load
+        # coefficients each airplane object experiences. These will only be populated
+        # for variable geometry problems.
+        self.final_mean_near_field_forces_wind_axes = []
+        self.final_mean_near_field_force_coefficients_wind_axes = []
+        self.final_mean_near_field_moments_wind_axes = []
+        self.final_mean_near_field_moment_coefficients_wind_axes = []
+
+        # Initialize empty lists to hold the final cycle-root-mean-squared loads and
+        # load coefficients each airplane object experiences. These will only be
+        # populated for variable geometry problems.
+        self.final_rms_near_field_forces_wind_axes = []
+        self.final_rms_near_field_force_coefficients_wind_axes = []
+        self.final_rms_near_field_moments_wind_axes = []
+        self.final_rms_near_field_moment_coefficients_wind_axes = []
 
         # Initialize an empty list to hold the steady problems.
         self.steady_problems = []
 
         # Iterate through the problem's time steps.
         for step_id in range(self.num_steps):
```

### Comparing `PteraSoftware-2.2.1/pterasoftware/steady_horseshoe_vortex_lattice_method.py` & `PteraSoftware-3.0.0/pterasoftware/steady_horseshoe_vortex_lattice_method.py`

 * *Files 0% similar despite different names*

```diff
@@ -210,15 +210,15 @@
                 for panel in panels:
 
                     # Update the solver's list of attributes with this panel's
                     # attributes.
                     self.panels[global_panel_position] = panel
                     self.panel_normal_directions[
                         global_panel_position, :
-                    ] = panel.normal_direction
+                    ] = panel.unit_normal
                     self.panel_areas[global_panel_position] = panel.area
                     self.panel_collocation_points[
                         global_panel_position, :
                     ] = panel.collocation_point
                     self.panel_back_right_vortex_vertices[
                         global_panel_position, :
                     ] = panel.horseshoe_vortex.right_leg.origin
```

### Comparing `PteraSoftware-2.2.1/pterasoftware/steady_ring_vortex_lattice_method.py` & `PteraSoftware-3.0.0/pterasoftware/steady_ring_vortex_lattice_method.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,14 @@
         self.freestream_velocity = (
             self.operating_point.calculate_freestream_velocity_geometry_axes()
         )
         self.freestream_wing_influences = np.zeros(self.num_panels)
         self.vortex_strengths = np.ones(self.num_panels)
         self.panel_normal_directions = np.zeros((self.num_panels, 3))
         self.panel_areas = np.zeros(self.num_panels)
-        self.panel_centers = np.zeros((self.num_panels, 3))
         self.panel_collocation_points = np.zeros((self.num_panels, 3))
         self.panel_back_right_vortex_vertices = np.zeros((self.num_panels, 3))
         self.panel_front_right_vortex_vertices = np.zeros((self.num_panels, 3))
         self.panel_front_left_vortex_vertices = np.zeros((self.num_panels, 3))
         self.panel_back_left_vortex_vertices = np.zeros((self.num_panels, 3))
         self.panels = np.empty(self.num_panels, dtype=object)
         self.panel_right_vortex_centers = np.zeros((self.num_panels, 3))
```

### Comparing `PteraSoftware-2.2.1/pterasoftware/trim.py` & `PteraSoftware-3.0.0/pterasoftware/trim.py`

 * *Files identical despite different names*

### Comparing `PteraSoftware-2.2.1/pterasoftware/unsteady_ring_vortex_lattice_method.py` & `PteraSoftware-3.0.0/pterasoftware/unsteady_ring_vortex_lattice_method.py`

 * *Files 6% similar despite different names*

```diff
@@ -73,17 +73,18 @@
         the apparent flow velocity due to flapping at the centers of the current
         airplanes' bound ring vortices' front legs.
 
         calculate_current_flapping_velocities_at_left_leg_centers: This method finds
         the apparent flow velocity due to flapping at the centers of the current
         airplanes' bound ring vortices' left legs.
 
-        finalize_near_field_forces_and_moments: This function finds the final
-        cycle-averaged force, moments, force coefficients, and moment coefficients
-        for each of this problem's airplanes.
+        finalize_near_field_forces_and_moments: For cases with static geometry,
+        this function finds the final loads and load coefficients for each of the
+        problem's airplanes. For cases with variable geometry, it finds the final
+        cycle-averaged and cycle-root-mean-squared loads and load coefficients.
 
     This class contains the following class attributes:
         None
 
     Subclassing:
         This class is not meant to be subclassed.
     """
@@ -114,15 +115,14 @@
         self.current_vortex_strengths = None
         self.streamline_points = None
 
         # Initialize attributes to hold geometric data that pertains to this problem.
         self.panels = None
         self.panel_normal_directions = None
         self.panel_areas = None
-        self.panel_centers = None
         self.panel_collocation_points = None
         self.panel_back_right_vortex_vertices = None
         self.panel_front_right_vortex_vertices = None
         self.panel_front_left_vortex_vertices = None
         self.panel_back_left_vortex_vertices = None
         self.panel_right_vortex_centers = None
         self.panel_right_vortex_vectors = None
@@ -360,15 +360,14 @@
                 self.current_vortex_strengths = np.ones(self.num_panels)
 
                 # Initialize attributes to hold geometric data that pertains to this
                 # problem.
                 self.panels = np.empty(self.num_panels, dtype=object)
                 self.panel_normal_directions = np.zeros((self.num_panels, 3))
                 self.panel_areas = np.zeros(self.num_panels)
-                self.panel_centers = np.zeros((self.num_panels, 3))
                 self.panel_collocation_points = np.zeros((self.num_panels, 3))
                 self.panel_back_right_vortex_vertices = np.zeros((self.num_panels, 3))
                 self.panel_front_right_vortex_vertices = np.zeros((self.num_panels, 3))
                 self.panel_front_left_vortex_vertices = np.zeros((self.num_panels, 3))
                 self.panel_back_left_vortex_vertices = np.zeros((self.num_panels, 3))
                 self.panel_right_vortex_centers = np.zeros((self.num_panels, 3))
                 self.panel_right_vortex_vectors = np.zeros((self.num_panels, 3))
@@ -1589,24 +1588,28 @@
         these_left_leg_centers = self.panel_left_vortex_centers
         last_left_leg_centers = self.last_panel_left_vortex_centers
 
         # Calculate and return the flapping velocities.
         return -(these_left_leg_centers - last_left_leg_centers) / self.delta_time
 
     def finalize_near_field_forces_and_moments(self):
-        """This function finds the final cycle-averaged force, moments,
-        force coefficients, and moment coefficients for each of this problem's
-        airplanes.
+        """For cases with static geometry, this function finds the final loads and
+        load coefficients for each of the problem's airplanes. For cases with
+        variable geometry, it finds the final cycle-averaged and
+        cycle-root-mean-squared loads and load coefficients.
 
         :return: None
         """
         # Get this solver's time step characteristics. Note that the first time step (
         # time step 0), occurs at 0 seconds.
         num_steps_to_average = self.num_steps - self.first_averaging_step
 
+        # Determine if this problem's geometry is static or variable.
+        is_static = self.unsteady_problem.max_period == 0
+
         # Initialize matrices to hold the forces, moments, and coefficients at each of
         # the time steps that has results.
         total_near_field_forces_wind_axes = np.zeros(
             (self.num_airplanes, 3, num_steps_to_average)
         )
         total_near_field_force_coefficients_wind_axes = np.zeros(
             (self.num_airplanes, 3, num_steps_to_average)
@@ -1644,85 +1647,89 @@
                 ] = airplane.total_near_field_moment_coefficients_wind_axes
 
             results_step += 1
 
         # For each airplane object, calculate and then save the final or
         # cycle-averaged forces, moments, force coefficients, and moment coefficients.
         for airplane_id, airplane in enumerate(self.steady_problems[0].airplanes):
-            these_mean_induced_drags = np.mean(
-                total_near_field_forces_wind_axes[airplane_id, 0, :]
-            )
-            these_mean_side_forces = np.mean(
-                total_near_field_forces_wind_axes[airplane_id, 1, :]
-            )
-            these_mean_lifts = np.mean(
-                total_near_field_forces_wind_axes[airplane_id, 2, :]
-            )
-            these_mean_rolling_moments = np.mean(
-                total_near_field_moments_wind_axes[airplane_id, 0, :]
-            )
-            these_mean_pitching_moments = np.mean(
-                total_near_field_moments_wind_axes[airplane_id, 1, :]
-            )
-            these_mean_yawing_moments = np.mean(
-                total_near_field_moments_wind_axes[airplane_id, 2, :]
-            )
-            these_mean_induced_drag_coefficients = np.mean(
-                total_near_field_force_coefficients_wind_axes[airplane_id, 0, :]
-            )
-            these_mean_side_force_coefficients = np.mean(
-                total_near_field_force_coefficients_wind_axes[airplane_id, 1, :]
-            )
-            these_mean_lift_coefficients = np.mean(
-                total_near_field_force_coefficients_wind_axes[airplane_id, 2, :]
-            )
-            these_mean_rolling_moment_coefficients = np.mean(
-                total_near_field_moment_coefficients_wind_axes[airplane_id, 0, :]
-            )
-            these_mean_pitching_moment_coefficients = np.mean(
-                total_near_field_moment_coefficients_wind_axes[airplane_id, 1, :]
-            )
-            these_mean_yawing_moment_coefficients = np.mean(
-                total_near_field_moment_coefficients_wind_axes[airplane_id, 2, :]
-            )
 
-            these_mean_forces = np.array(
-                [
-                    these_mean_induced_drags,
-                    these_mean_side_forces,
-                    these_mean_lifts,
-                ]
-            )
-            these_mean_force_coefficients = np.array(
-                [
-                    these_mean_induced_drag_coefficients,
-                    these_mean_side_force_coefficients,
-                    these_mean_lift_coefficients,
-                ]
-            )
-            these_mean_moments = np.array(
-                [
-                    these_mean_rolling_moments,
-                    these_mean_pitching_moments,
-                    these_mean_yawing_moments,
-                ]
-            )
-            these_mean_moment_coefficients = np.array(
-                [
-                    these_mean_rolling_moment_coefficients,
-                    these_mean_pitching_moment_coefficients,
-                    these_mean_yawing_moment_coefficients,
-                ]
-            )
+            if is_static:
+                self.unsteady_problem.final_near_field_forces_wind_axes.append(
+                    total_near_field_forces_wind_axes[airplane_id, :, -1]
+                )
+                self.unsteady_problem.final_near_field_force_coefficients_wind_axes.append(
+                    total_near_field_force_coefficients_wind_axes[airplane_id, :, -1]
+                )
+                self.unsteady_problem.final_near_field_moments_wind_axes.append(
+                    total_near_field_moments_wind_axes[airplane_id, :, -1]
+                )
+                self.unsteady_problem.final_near_field_moment_coefficients_wind_axes.append(
+                    total_near_field_moment_coefficients_wind_axes[airplane_id, :, -1]
+                )
+            else:
+                mean_forces = np.mean(
+                    total_near_field_forces_wind_axes[airplane_id], axis=-1
+                )
+                mean_force_coefficients = np.mean(
+                    total_near_field_force_coefficients_wind_axes[airplane_id], axis=-1
+                )
+                mean_moments = np.mean(
+                    total_near_field_moments_wind_axes[airplane_id], axis=-1
+                )
+                mean_moment_coefficients = np.mean(
+                    total_near_field_moment_coefficients_wind_axes[airplane_id], axis=-1
+                )
 
-            self.unsteady_problem.final_total_near_field_forces_wind_axes.append(
-                these_mean_forces
-            )
-            self.unsteady_problem.final_total_near_field_moments_wind_axes.append(
-                these_mean_moments
-            )
-            self.unsteady_problem.final_total_near_field_force_coefficients_wind_axes.append(
-                these_mean_force_coefficients
-            )
-            self.unsteady_problem.final_total_near_field_moment_coefficients_wind_axes.append(
-                these_mean_moment_coefficients
-            )
+                rms_forces = np.sqrt(
+                    np.mean(
+                        np.square(total_near_field_forces_wind_axes[airplane_id]),
+                        axis=-1,
+                    )
+                )
+                rms_force_coefficients = np.sqrt(
+                    np.mean(
+                        np.square(
+                            total_near_field_force_coefficients_wind_axes[airplane_id]
+                        ),
+                        axis=-1,
+                    )
+                )
+                rms_moments = np.sqrt(
+                    np.mean(
+                        np.square(total_near_field_moments_wind_axes[airplane_id]),
+                        axis=-1,
+                    )
+                )
+                rms_moment_coefficients = np.sqrt(
+                    np.mean(
+                        np.square(
+                            total_near_field_moment_coefficients_wind_axes[airplane_id]
+                        ),
+                        axis=-1,
+                    )
+                )
+
+                self.unsteady_problem.final_mean_near_field_forces_wind_axes.append(
+                    mean_forces
+                )
+                self.unsteady_problem.final_mean_near_field_force_coefficients_wind_axes.append(
+                    mean_force_coefficients
+                )
+                self.unsteady_problem.final_mean_near_field_moments_wind_axes.append(
+                    mean_moments
+                )
+                self.unsteady_problem.final_mean_near_field_moment_coefficients_wind_axes.append(
+                    mean_moment_coefficients
+                )
+
+                self.unsteady_problem.final_rms_near_field_forces_wind_axes.append(
+                    rms_forces
+                )
+                self.unsteady_problem.final_rms_near_field_force_coefficients_wind_axes.append(
+                    rms_force_coefficients
+                )
+                self.unsteady_problem.final_rms_near_field_moments_wind_axes.append(
+                    rms_moments
+                )
+                self.unsteady_problem.final_rms_near_field_moment_coefficients_wind_axes.append(
+                    rms_moment_coefficients
+                )
```

### Comparing `PteraSoftware-2.2.1/setup.cfg` & `PteraSoftware-3.0.0/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2050 7465 7261 536f 6674 7761 7265   = PteraSoftware
-00000020: 0d0a 7665 7273 696f 6e20 3d20 322e 322e  ..version = 2.2.
-00000030: 310d 0a61 7574 686f 7220 3d20 4361 6d65  1..author = Came
+00000020: 0d0a 7665 7273 696f 6e20 3d20 332e 302e  ..version = 3.0.
+00000030: 300d 0a61 7574 686f 7220 3d20 4361 6d65  0..author = Came
 00000040: 726f 6e20 5572 6261 6e0d 0a61 7574 686f  ron Urban..autho
 00000050: 725f 656d 6169 6c20 3d20 6361 6d65 726f  r_email = camero
 00000060: 6e67 7572 6261 6e40 676d 6169 6c2e 636f  ngurban@gmail.co
 00000070: 6d0d 0a6c 6963 656e 7365 203d 204d 4954  m..license = MIT
 00000080: 0d0a 6465 7363 7269 7074 696f 6e20 3d20  ..description = 
 00000090: 5468 6973 2069 7320 616e 206f 7065 6e2d  This is an open-
 000000a0: 736f 7572 6365 2c20 756e 7374 6561 6479  source, unsteady
@@ -71,23 +71,25 @@
 00000460: 7265 2e61 6972 666f 696c 730d 0a69 6e63  re.airfoils..inc
 00000470: 6c75 6465 5f70 6163 6b61 6765 5f64 6174  lude_package_dat
 00000480: 6120 3d20 5472 7565 0d0a 7079 7468 6f6e  a = True..python
 00000490: 5f72 6571 7569 7265 7320 3d20 3e3d 2033  _requires = >= 3
 000004a0: 2e38 2e30 2c20 3c20 332e 392e 300d 0a69  .8.0, < 3.9.0..i
 000004b0: 6e73 7461 6c6c 5f72 6571 7569 7265 7320  nstall_requires 
 000004c0: 3d20 0d0a 096d 6174 706c 6f74 6c69 6220  = ...matplotlib 
-000004d0: 3e3d 2033 2e35 2e32 2c20 3c20 342e 302e  >= 3.5.2, < 4.0.
+000004d0: 3e3d 2033 2e37 2e31 2c20 3c20 342e 302e  >= 3.7.1, < 4.0.
 000004e0: 300d 0a09 6e75 6d70 7920 3e3d 2031 2e32  0...numpy >= 1.2
-000004f0: 322e 342c 203c 2031 2e32 342e 300d 0a09  2.4, < 1.24.0...
-00000500: 7079 7669 7374 6120 3e3d 2030 2e33 342e  pyvista >= 0.34.
+000004f0: 342e 332c 203c 2031 2e32 352e 300d 0a09  4.3, < 1.25.0...
+00000500: 7079 7669 7374 6120 3e3d 2030 2e33 392e  pyvista >= 0.39.
 00000510: 312c 203c 2031 2e30 2e30 0d0a 0973 6369  1, < 1.0.0...sci
-00000520: 7079 203e 3d20 312e 382e 312c 203c 2032  py >= 1.8.1, < 2
-00000530: 2e30 2e30 0d0a 096e 756d 6261 203e 3d20  .0.0...numba >= 
-00000540: 302e 3535 2e32 2c20 3c20 312e 302e 300d  0.55.2, < 1.0.0.
-00000550: 0a09 636d 6f63 6561 6e20 3e3d 2032 2e30  ..cmocean >= 2.0
-00000560: 2e30 2c20 3c20 332e 302e 300d 0a09 7471  .0, < 3.0.0...tq
-00000570: 646d 203e 3d20 342e 3634 2e30 2c20 3c20  dm >= 4.64.0, < 
-00000580: 352e 302e 300d 0a09 7765 6270 203e 3d20  5.0.0...webp >= 
-00000590: 302e 312e 342c 203c 2031 2e30 2e30 0d0a  0.1.4, < 1.0.0..
-000005a0: 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a 7461  ..[egg_info]..ta
-000005b0: 675f 6275 696c 6420 3d20 0d0a 7461 675f  g_build = ..tag_
-000005c0: 6461 7465 203d 2030 0d0a 0d0a            date = 0....
+00000520: 7079 203e 3d20 312e 3130 2e31 2c20 3c20  py >= 1.10.1, < 
+00000530: 322e 302e 300d 0a09 6e75 6d62 6120 3e3d  2.0.0...numba >=
+00000540: 2030 2e35 372e 312c 203c 2031 2e30 2e30   0.57.1, < 1.0.0
+00000550: 0d0a 0963 6d6f 6365 616e 203e 3d20 332e  ...cmocean >= 3.
+00000560: 302e 332c 203c 2034 2e30 2e30 0d0a 0974  0.3, < 4.0.0...t
+00000570: 7164 6d20 3e3d 2034 2e36 352e 302c 203c  qdm >= 4.65.0, <
+00000580: 2035 2e30 2e30 0d0a 0977 6562 7020 3e3d   5.0.0...webp >=
+00000590: 2030 2e31 2e36 2c20 3c20 312e 302e 300d   0.1.6, < 1.0.0.
+000005a0: 0a09 5079 5369 6465 3220 3e3d 2035 2e31  ..PySide2 >= 5.1
+000005b0: 352e 322e 312c 203c 2036 2e30 2e30 2e30  5.2.1, < 6.0.0.0
+000005c0: 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a  ....[egg_info]..
+000005d0: 7461 675f 6275 696c 6420 3d20 0d0a 7461  tag_build = ..ta
+000005e0: 675f 6461 7465 203d 2030 0d0a 0d0a       g_date = 0....
```

