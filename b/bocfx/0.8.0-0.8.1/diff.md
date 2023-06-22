# Comparing `tmp/bocfx-0.8.0.tar.gz` & `tmp/bocfx-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bocfx-0.8.0.tar", last modified: Tue May 23 16:27:57 2023, max compression
+gzip compressed data, was "bocfx-0.8.1.tar", last modified: Thu Jun 22 06:03:43 2023, max compression
```

## Comparing `bocfx-0.8.0.tar` & `bocfx-0.8.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-23 16:27:57.561104 bocfx-0.8.0/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1073 2023-05-23 16:00:18.000000 bocfx-0.8.0/LICENSE
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    17323 2023-05-23 16:27:57.557104 bocfx-0.8.0/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    16903 2023-05-23 16:11:35.000000 bocfx-0.8.0/README.md
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-23 16:27:57.557104 bocfx-0.8.0/bocfx/
--rwxrwxrwx   0 codespace  (1000) codespace  (1000)      417 2023-05-23 16:00:18.000000 bocfx-0.8.0/bocfx/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11484 2023-05-23 16:25:11.000000 bocfx-0.8.0/bocfx/__main__.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-23 16:27:57.557104 bocfx-0.8.0/bocfx.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    17323 2023-05-23 16:27:57.000000 bocfx-0.8.0/bocfx.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      238 2023-05-23 16:27:57.000000 bocfx-0.8.0/bocfx.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-05-23 16:27:57.000000 bocfx-0.8.0/bocfx.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       39 2023-05-23 16:27:57.000000 bocfx-0.8.0/bocfx.egg-info/entry_points.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       50 2023-05-23 16:27:57.000000 bocfx-0.8.0/bocfx.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        6 2023-05-23 16:27:57.000000 bocfx-0.8.0/bocfx.egg-info/top_level.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-05-23 16:27:57.561104 bocfx-0.8.0/setup.cfg
--rwxrwxrwx   0 codespace  (1000) codespace  (1000)      880 2023-05-23 16:26:11.000000 bocfx-0.8.0/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-22 06:03:43.586890 bocfx-0.8.1/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1073 2023-05-23 16:00:18.000000 bocfx-0.8.1/LICENSE
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    17323 2023-06-22 06:03:43.582890 bocfx-0.8.1/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    16903 2023-06-22 05:56:33.000000 bocfx-0.8.1/README.md
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-22 06:03:43.582890 bocfx-0.8.1/bocfx/
+-rwxrwxrwx   0 codespace  (1000) codespace  (1000)      379 2023-06-22 05:55:23.000000 bocfx-0.8.1/bocfx/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12425 2023-06-22 05:55:14.000000 bocfx-0.8.1/bocfx/__main__.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-22 06:03:43.582890 bocfx-0.8.1/bocfx.egg-info/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    17323 2023-06-22 06:03:43.000000 bocfx-0.8.1/bocfx.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      238 2023-06-22 06:03:43.000000 bocfx-0.8.1/bocfx.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-06-22 06:03:43.000000 bocfx-0.8.1/bocfx.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       39 2023-06-22 06:03:43.000000 bocfx-0.8.1/bocfx.egg-info/entry_points.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       50 2023-06-22 06:03:43.000000 bocfx-0.8.1/bocfx.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        6 2023-06-22 06:03:43.000000 bocfx-0.8.1/bocfx.egg-info/top_level.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-06-22 06:03:43.586890 bocfx-0.8.1/setup.cfg
+-rwxrwxrwx   0 codespace  (1000) codespace  (1000)      880 2023-06-22 05:56:08.000000 bocfx-0.8.1/setup.py
```

### Comparing `bocfx-0.8.0/LICENSE` & `bocfx-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bocfx-0.8.0/PKG-INFO` & `bocfx-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: bocfx
-Version: 0.8.0
+Version: 0.8.1
 Summary: Easy API to get foreign exchange rate from Bank of China.
 Home-page: https://github.com/bobleer/bocfx
 Author: bobleer
 Author-email: liwenbo628@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# bocfx ![](https://img.shields.io/badge/License-MIT-green.svg) ![](https://img.shields.io/badge/Python-3-3776ab.svg) ![](https://img.shields.io/badge/PyPI-0.8.0-ffd242.svg)
+# bocfx ![](https://img.shields.io/badge/License-MIT-green.svg) ![](https://img.shields.io/badge/Python-3-3776ab.svg) ![](https://img.shields.io/badge/PyPI-0.8.1-ffd242.svg)
 An easy-to-use python package for getting foreign exchange rate from Bank of China (BOC).  
 一个帮你快速获取中国银行外汇牌价的 Python 爬虫（也可作外汇牌价实时查询API)。  
 Author: [**Bob Lee**](https://boblee.cn)
 
 <br>
 
 # Features
```

### Comparing `bocfx-0.8.0/README.md` & `bocfx-0.8.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# bocfx ![](https://img.shields.io/badge/License-MIT-green.svg) ![](https://img.shields.io/badge/Python-3-3776ab.svg) ![](https://img.shields.io/badge/PyPI-0.8.0-ffd242.svg)
+# bocfx ![](https://img.shields.io/badge/License-MIT-green.svg) ![](https://img.shields.io/badge/Python-3-3776ab.svg) ![](https://img.shields.io/badge/PyPI-0.8.1-ffd242.svg)
 An easy-to-use python package for getting foreign exchange rate from Bank of China (BOC).  
 一个帮你快速获取中国银行外汇牌价的 Python 爬虫（也可作外汇牌价实时查询API)。  
 Author: [**Bob Lee**](https://boblee.cn)
 
 <br>
 
 # Features
```

### Comparing `bocfx-0.8.0/bocfx/__main__.py` & `bocfx-0.8.1/bocfx/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,53 @@
 #!/usr/bin/env python
 # coding: utf-8
 # Author: Bob Lee
-# Blog: https://boblee.cn
-# Version: 0.8.0
-# Date: 2023-05-24 00:12:05
 
-import getopt
+from getopt import getopt
 import sys
 import time as tm
 import os
 import requests
 
 from scrapy.selector import Selector
 from concurrent.futures import ThreadPoolExecutor
 from tqdm import tqdm
 import datetime
 import re
 
+VERSION = "0.8.1"
+LAST_MODIFY_TIME = "2023-06-22 13:52:05"
+
 def asexec():
     FX = 0
     sort = 0
     time = -1
     plot = 0
     csv = 0
     pt = 1
-    op = '~/bocfx_output'
+    op = os.path.join('~', 'bocfx_output')
     bar = 0
-    opts, args = getopt.getopt(sys.argv[1:],'hf:s:t:pco:b',['help','FX=','sort=','time=','plot','csv','op=', 'bar'])
+    try:
+        opts, args = getopt(sys.argv[1:], 'hf:s:t:pco:bv', ['help','FX=','sort=','time=','plot','csv','op=', 'bar', 'version'])
+    except:
+        print("option", sys.argv[1:], "not recognized!")
+        sys.exit()
 
     for opt, arg in opts:
         if opt in ('-h','--help'):
-            print("A python package for getting foreign exchange rate from Bank of China (BOC).\n\nbocfx [-f|--fx] [-s|--sort] [-t|--time] (-p|--plot) (-c|--csv) {-o|--op} (-b|--bar)\n\nExample:\nbocfx -f USD,EUR,GBP -s ASK,SE -t 7 -p -c -o '/User/root/newDir'\n\nFind detailed help: https://github.com/bobleer/bocfx")
+            print("A python package for getting foreign exchange rate from Bank of China(BOC).")
+            print("Version:", VERSION)
+            print("Last modify:", LAST_MODIFY_TIME)
+            print("")
+            print("Usage:\n    bocfx [-f|--fx] [-s|--sort] [-t|--time] (-p|--plot) (-c|--csv) {-o|--op} (-b|--bar)")
+            print("")
+            print("Example:\n    bocfx -f USD,EUR,GBP -s ASK,SE -t 7 -p -c -o '/User/root/newDir'")
+            print("")
+            print("Find detailed help: https://github.com/bobleer/bocfx")
+            print("")
             sys.exit()
 
         elif opt in ('-f','--FX'):
             FX = arg.replace(" ","")
 
         elif opt in ('-s','--sort'):
             sort = arg.replace(" ","")
@@ -50,47 +63,52 @@
 
         elif opt in ('-o','--op'):
             op = arg
         
         elif opt in ('-b','--bar'):
             bar = 1
 
+        elif opt in ('-v','--version'):
+            print("Version:", VERSION)
+            print("Last modify:", LAST_MODIFY_TIME)
+            sys.exit()
+
     output = main(FX, sort, time, plot, csv, pt, op, bar)
     sys.exit() 
 
 
-def bocfx(FX=0, sort=0, time=-1, plot=0, csv=0, pt=0, op='~/bocfx_output', bar=0):
+def bocfx(FX=0, sort=0, time=-1, plot=0, csv=0, pt=0, op=os.path.join('~', 'bocfx_output'), bar=0):
     if FX in [None,""]: FX = 0
     if sort in [None,""]: sort = 0
     if time in [None,""]: time = -1
     if plot in [None,""]: plot = 0
     if csv in [None,""]: csv = 0
     if pt in [None,""]: pt = 0
-    if op in [None,""]: op = '~/bocfx_output'
+    if op in [None,""]: op = os.path.join('~', 'bocfx_output')
     if bar in [None,""]: bar = 0
     output = main(FX, sort, time, plot, csv, pt, op, bar)
     return output
 
 
 def page_get(output, sort, FX_or, erectDate, nothing, FX, i, page, end):
     error_times = 0
     try:
         r = requests.post('https://srh.bankofchina.com/search/whpj/search_cn.jsp', data = {'erectDate':erectDate, 'nothing':nothing, 'pjname':str(FX[i]), 'page':str(page)})
     except:
-        print("Internet Error, waiting 2s.\n")
+        print("Internet Error, waiting 60s.\n")
         error_times += 1
-        tm.sleep(2)
+        tm.sleep(60)
         while error_times <= 3:
             r = requests.post('https://srh.bankofchina.com/search/whpj/search_cn.jsp', data = {'erectDate':erectDate, 'nothing':nothing, 'pjname':str(FX[i]), 'page':str(page)})
         else:
             print("Retry 3 times, break!")
             exit()
 
     html = r.text
-    for row in range(2,end):
+    for row in range(2,end+2):
         try:
             SE_B = Selector(text=html).xpath('//tr[%i]/td[2]/text()' % (row)).extract()[0].strip('\r\n\t ')
             BN_B = Selector(text=html).xpath('//tr[%i]/td[3]/text()' % (row)).extract()[0].strip('\r\n\t ')
             SE_A = Selector(text=html).xpath('//tr[%i]/td[4]/text()' % (row)).extract()[0].strip('\r\n\t ')
             BN_A = Selector(text=html).xpath('//tr[%i]/td[5]/text()' % (row)).extract()[0].strip('\r\n\t ')
             BOC_C = Selector(text=html).xpath('//tr[%i]/td[6]/text()' % (row)).extract()[0].strip('\r\n\t ')
             time = Selector(text=html).xpath('//tr[%i]/td[7]/text()' % (row)).extract()[0].replace('.','-').strip('\r\n\t ')
@@ -185,30 +203,34 @@
         else:
             print("Incorrect time input!")
 
         all_task = []
         for i in range(len(FX)):
             r = requests.post('https://srh.bankofchina.com/search/whpj/search_cn.jsp', data = {'erectDate':erectDate, 'nothing':nothing, 'pjname':FX[i], 'page':'1'})
             r = r.text
+            while "您的查询操作太频繁，请一分钟后再试。" in r:
+                tm.sleep(60)
+                r = requests.post('https://srh.bankofchina.com/search/whpj/search_cn.jsp', data = {'erectDate':erectDate, 'nothing':nothing, 'pjname':FX[i], 'page':'1'})
+                r = r.text
             searchOBJ = re.search(r'var m_nRecordCount = (.*);',r)
             pages = (int(searchOBJ.group(1))//20)+1
 
-            ex = ThreadPoolExecutor(max_workers=20)
+            ex = ThreadPoolExecutor(max_workers=1) # BOC 设置了查询频率，不建议放开多线程了
             for page in range(1,(pages+1)):
-                all_task.append(ex.submit(page_get, output, sort, FX_or, erectDate, nothing, FX, i, page, 22))
+                all_task.append(ex.submit(page_get, output, sort, FX_or, erectDate, nothing, FX, i, page, 20))
 
         [i.result() for i in show_prog(all_task, ifbar=bar)]
         ex.shutdown(wait=True)
         output = list(set(output))
         output.sort(reverse=True,key=lambda ele:ele[-1])
         filename = '['+'+'.join(FX_or)+']'+'+'.join(output[0][1:-1])+'_'+erectDate+'_'+nothing
 
     else:
-        ex = ThreadPoolExecutor(max_workers=20)
-        all_task = [ex.submit(page_get, output, sort, FX_or, '', '', FX, i, '1', 3) for i in range(len(FX))]
+        ex = ThreadPoolExecutor(max_workers=1)
+        all_task = [ex.submit(page_get, output, sort, FX_or, '', '', FX, i, '1', 1) for i in range(len(FX))]
         [i.result() for i in show_prog(all_task, ifbar=bar)]
         ex.shutdown(wait=True)
         
         t=[output[0]]
         for i in range(len(FX_or)):
             for f in range(len(output)):
                 if output[f][0] == FX_or[i]:
@@ -233,20 +255,20 @@
         #print(output)
 
 
     if csv != 0:
         op = os.path.expanduser(op)
         if not os.path.exists(op):
             os.makedirs(op)
-        csvpath = os.path.join(op,filename)+'.csv'
+        csvpath = os.path.join(op, filename)+'.csv'
 
         with open(csvpath, 'w')  as f:
             for i in output:
                 f.write(','.join(map(str,i))+'\n')
-        print('\n.csv has already saved to '+csvpath)
+        print('\ncsv file has already saved to '+csvpath)
 
 
     if plot != 0:
         import numpy as np
         import matplotlib.pyplot as plt
 
         p = np.array(output)
@@ -262,18 +284,18 @@
                 plt.plot(x,sd[:,i][:].astype(float),label='['+FX_or[f]+']'+str(p[:,i][0])+': '+str(sd[:,i][0]))
 
             plt.legend(loc=2)
 
         op = os.path.expanduser(op)
         if not os.path.exists(op):
             os.makedirs(op)
-        plotpath = os.path.join(op,filename)+'.png'
+        plotpath = os.path.join(op, filename)+'.png'
         
         plt.savefig(plotpath, dpi=150)
-        print('\nPlot has already saved to '+plotpath)
+        print('\nPlot file has already saved to '+plotpath)
         plt.show()
 
 
     if len(output[1])==3 and time==-1 and plot==0 and csv==0 and pt==0:
         simple_output = [i[1] for i in output[1:]]
         output = simple_output
```

### Comparing `bocfx-0.8.0/bocfx.egg-info/PKG-INFO` & `bocfx-0.8.1/bocfx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: bocfx
-Version: 0.8.0
+Version: 0.8.1
 Summary: Easy API to get foreign exchange rate from Bank of China.
 Home-page: https://github.com/bobleer/bocfx
 Author: bobleer
 Author-email: liwenbo628@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# bocfx ![](https://img.shields.io/badge/License-MIT-green.svg) ![](https://img.shields.io/badge/Python-3-3776ab.svg) ![](https://img.shields.io/badge/PyPI-0.8.0-ffd242.svg)
+# bocfx ![](https://img.shields.io/badge/License-MIT-green.svg) ![](https://img.shields.io/badge/Python-3-3776ab.svg) ![](https://img.shields.io/badge/PyPI-0.8.1-ffd242.svg)
 An easy-to-use python package for getting foreign exchange rate from Bank of China (BOC).  
 一个帮你快速获取中国银行外汇牌价的 Python 爬虫（也可作外汇牌价实时查询API)。  
 Author: [**Bob Lee**](https://boblee.cn)
 
 <br>
 
 # Features
```

### Comparing `bocfx-0.8.0/setup.py` & `bocfx-0.8.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="bocfx",
-    version="0.8.0",
+    version="0.8.1",
     author="bobleer",
     author_email="liwenbo628@gmail.com",
     description="Easy API to get foreign exchange rate from Bank of China.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/bobleer/bocfx",
     packages=setuptools.find_packages(),
```

