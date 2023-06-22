# Comparing `tmp/LeoX-0.6.0.tar.gz` & `tmp/LeoX-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LeoX-0.6.0.tar", last modified: Tue Jun 20 15:10:34 2023, max compression
+gzip compressed data, was "LeoX-0.6.1.tar", last modified: Thu Jun 22 14:25:29 2023, max compression
```

## Comparing `LeoX-0.6.0.tar` & `LeoX-0.6.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:10:34.761839 LeoX-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-20 15:10:24.000000 LeoX-0.6.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:10:34.761839 LeoX-0.6.0/LeoX.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8697 2023-06-20 15:10:34.000000 LeoX-0.6.0/LeoX.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-06-20 15:10:34.000000 LeoX-0.6.0/LeoX.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 15:10:34.000000 LeoX-0.6.0/LeoX.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-20 15:10:34.000000 LeoX-0.6.0/LeoX.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-20 15:10:34.000000 LeoX-0.6.0/LeoX.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-20 15:10:34.000000 LeoX-0.6.0/LeoX.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-20 15:10:24.000000 LeoX-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8697 2023-06-20 15:10:34.761839 LeoX-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8347 2023-06-20 15:10:24.000000 LeoX-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:10:34.761839 LeoX-0.6.0/lx/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 15:10:24.000000 LeoX-0.6.0/lx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7688 2023-06-20 15:10:24.000000 LeoX-0.6.0/lx/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-20 15:10:24.000000 LeoX-0.6.0/lx/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-06-20 15:10:24.000000 LeoX-0.6.0/lx/batch_lx.py
--rw-r--r--   0 runner    (1001) docker     (123)    11444 2023-06-20 15:10:24.000000 LeoX-0.6.0/lx/conf_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     8053 2023-06-20 15:10:24.000000 LeoX-0.6.0/lx/ld.py
--rw-r--r--   0 runner    (1001) docker     (123)     7217 2023-06-20 15:10:24.000000 LeoX-0.6.0/lx/omega.py
--rw-r--r--   0 runner    (1001) docker     (123)    34404 2023-06-20 15:10:24.000000 LeoX-0.6.0/lx/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 15:10:34.761839 LeoX-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-06-20 15:10:24.000000 LeoX-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:25:29.903132 LeoX-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-22 14:25:12.000000 LeoX-0.6.1/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:25:29.903132 LeoX-0.6.1/LeoX.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8697 2023-06-22 14:25:29.000000 LeoX-0.6.1/LeoX.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-06-22 14:25:29.000000 LeoX-0.6.1/LeoX.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 14:25:29.000000 LeoX-0.6.1/LeoX.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-22 14:25:29.000000 LeoX-0.6.1/LeoX.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-22 14:25:29.000000 LeoX-0.6.1/LeoX.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-22 14:25:29.000000 LeoX-0.6.1/LeoX.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-22 14:25:12.000000 LeoX-0.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8697 2023-06-22 14:25:29.903132 LeoX-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8347 2023-06-22 14:25:12.000000 LeoX-0.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:25:29.903132 LeoX-0.6.1/lx/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 14:25:12.000000 LeoX-0.6.1/lx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7688 2023-06-22 14:25:12.000000 LeoX-0.6.1/lx/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-22 14:25:12.000000 LeoX-0.6.1/lx/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-06-22 14:25:12.000000 LeoX-0.6.1/lx/batch_lx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11458 2023-06-22 14:25:12.000000 LeoX-0.6.1/lx/conf_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8053 2023-06-22 14:25:12.000000 LeoX-0.6.1/lx/ld.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7217 2023-06-22 14:25:12.000000 LeoX-0.6.1/lx/omega.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36155 2023-06-22 14:25:12.000000 LeoX-0.6.1/lx/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 14:25:29.903132 LeoX-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-06-22 14:25:12.000000 LeoX-0.6.1/setup.py
```

### Comparing `LeoX-0.6.0/LICENSE` & `LeoX-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `LeoX-0.6.0/LeoX.egg-info/PKG-INFO` & `LeoX-0.6.1/LeoX.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LeoX
-Version: 0.6.0
+Version: 0.6.1
 Summary: Spectrum simulations with TD(A)-DFT
 Home-page: https://github.com/LeonardoESousa/LeoX
 Author: Leonardo Evaristo de Sousa
 Author-email: leonardo.sousa137@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `LeoX-0.6.0/PKG-INFO` & `LeoX-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LeoX
-Version: 0.6.0
+Version: 0.6.1
 Summary: Spectrum simulations with TD(A)-DFT
 Home-page: https://github.com/LeonardoESousa/LeoX
 Author: Leonardo Evaristo de Sousa
 Author-email: leonardo.sousa137@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `LeoX-0.6.0/README.md` & `LeoX-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `LeoX-0.6.0/lx/__main__.py` & `LeoX-0.6.1/lx/__main__.py`

 * *Files identical despite different names*

### Comparing `LeoX-0.6.0/lx/batch_lx.py` & `LeoX-0.6.1/lx/batch_lx.py`

 * *Files identical despite different names*

### Comparing `LeoX-0.6.0/lx/conf_search.py` & `LeoX-0.6.1/lx/conf_search.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         cm = np.zeros((5,5))
     return cm              
 
 ##SAMPLES GEOMETRIES###########################################
 def make_geoms(freqlog, num_geoms, T, header, bottom):
     lista = []
     counter = lx.tools.start_counter()
-    _, atomos, A = lx.tools.sample_geometries(freqlog,num_geoms,T,3000)
+    _, atomos, A = lx.tools.sample_geometries(freqlog,num_geoms,T,3000,warning=False)
     for n in range(0,np.shape(A)[1],3):
         Gfinal = A[:,n:n+3]
         lx.tools.write_input(atomos,Gfinal,header.replace("UUUUU",str((n+3)//3)),bottom.replace("UUUUU",str((n+3)//3)),"Geometry-"+str((n+3)//3+counter)+"-.com")
         lista.append("Geometry-"+str((n+3)//3+counter)+"-.com") 
     return lista      
 ###############################################################
```

### Comparing `LeoX-0.6.0/lx/ld.py` & `LeoX-0.6.1/lx/ld.py`

 * *Files identical despite different names*

### Comparing `LeoX-0.6.0/lx/omega.py` & `LeoX-0.6.1/lx/omega.py`

 * *Files identical despite different names*

### Comparing `LeoX-0.6.0/lx/tools.py` & `LeoX-0.6.1/lx/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -210,15 +210,15 @@
 
 ##CHECKS FOR EXISTING GEOMETRIES###############################
 def start_counter():
     files = [file for file in os.listdir('Geometries') if ".com" in file and "Geometr" in file]
     return len(files)
 ###############################################################
 
-##SAMPLES GEOMETRIES###########################################
+##DISTORTS GEOMETRIES IN DIRECTION OF IMAG FREQ################
 def distort(freqlog):
     num_geoms = 1
     T = 300
     G, atomos = pega_geom(freqlog)
     F, M      = pega_freq(freqlog)
     NNC       = pega_modos(G,freqlog)
     num_atom  = np.shape(G)[0]
@@ -244,26 +244,53 @@
     bottom = '\n'
     for n in range(0,np.shape(A)[1],3):
         Gfinal = Gfinal[:,n:n+3]
         write_input(atomos,Gfinal,header,bottom,"distorted.com")
     print("New input file written to distorted.com")    
 ###############################################################
 
+##CHECKS FREQ FILES############################################
+def double_check(freqlog):
+    nproc, mem, header = get_input_params(freqlog)
+    header = header.lower()
+    if "opt" in header and 'freq' in header and 'iop(' in header:
+        optfreqissue = True
+    with open(freqlog, 'r') as f:
+        for line in f:
+            if "Non-Optimized Parameters" in line:
+                print('*'*50)
+                print("WARNING: Non-optimized parameters detected in your frequency file.")
+                print('Even though the frequencies may be all real, your structure is still not fully optimized.')
+                print('This may lead to inaccurate results.')
+                if optfreqissue:
+                    print('In your case, this may be due to running an opt freq calculation using a single input file and IOP options.')
+                    print('Gaussian does not carry the IOP options to the frequency calculation when using a single input file.')
+                    print('To avoid this issue, run the optimization and frequency calculations separately.')
+                else:
+                    print('To learn more about this issue, check https://gaussian.com/faq3/ .')        
+                print('Proceed at your own risk.')
+                print('*'*50)
+                print('\n')
+###############################################################              
+
 ##SAMPLES GEOMETRIES###########################################
 def sample_geometries(freqlog,num_geoms,T, limit=np.inf, warning=True):
     G, atomos = pega_geom(freqlog)
     F, M      = pega_freq(freqlog)
-    # check for negative frequencies
-    if warning and np.any(F < 0):
-        fatal_error("Negative frequencies detected. Check your frequency file. Goodbye.")
-    F[F < 0] *= -1
     NNC       = pega_modos(G,freqlog)
-    mask = F < limit*(c*100*2*pi)
-    F = F[mask]
-    NNC = NNC[:,mask]
+    # check for negative frequencies
+    if warning:
+        if np.any(F < 0):
+            fatal_error("Imaginary frequencies detected. Check your frequency file. Goodbye.")
+        double_check(freqlog)
+    else:
+        F[F < 0] *= -1
+        mask = F < limit*(c*100*2*pi)
+        F = F[mask]
+        NNC = NNC[:,mask]
     num_atom  = np.shape(G)[0]
     A = np.zeros((3*num_atom,num_geoms))
     for i in range(0,len(F)):
         scale = np.sqrt(hbar2/(2*M[i]*F[i]*np.tanh(hbar*F[i]/(2*kb*T))))
         normal = norm(scale=scale,loc=0)
         #Displacements in  Å
         q = normal.rvs(size=num_geoms)*1e10
@@ -461,22 +488,17 @@
         f.write(segunda)
         for i in range(0,len(x)):
             text = "{:.6f} {:.6e} {:.6e}\n".format(x[i],mean_y[i], sigma[i])
             f.write(text)
     print('Spectrum printed in the {} file'.format(arquivo))                
 ############################################################### 
 
-##CHECKS THE FREQUENCY LOG'S LEVEL OF THEORY###################
-def busca_input(freqlog):
-    base = 'lalala'
-    exc = ''
-    header = ''
-    nproc = '4'
-    mem   = '1GB'
-    scrf  = ''
+##GETS INPUT PARAMS FROM LOG FILES#############################
+def get_input_params(freqlog):
+    nproc, mem, header = '', '', ''
     with open(freqlog, 'r') as f:
         search = False
         for line in f:
             if '%nproc' in line.lower():
                 line = line.split('=')
                 nproc = line[-1].replace('\n','')
             elif '%mem' in line.lower():
@@ -486,15 +508,27 @@
                 search = True
                 header += line.lstrip().replace('\n','')
             elif search and '----------' not in line:
                 header += line.lstrip().replace('\n','')
             elif search and '----------' in line:
                 search = False
                 break
-  
+    return nproc, mem, header        
+###############################################################
+
+##CHECKS THE FREQUENCY LOG'S LEVEL OF THEORY###################
+def busca_input(freqlog):
+    base = 'lalala'
+    exc = ''
+    header = ''
+    nproc = '4'
+    mem   = '1GB'
+    scrf  = ''
+    nproc, mem, header = get_input_params(freqlog)
+    
     if 'TDA' in header.upper():
         exc = 'tda'
         spec = 'EMISPCT'
     elif 'TD' in header.upper():
         exc = 'td'
         spec = 'EMISPCT'
     else:
```

### Comparing `LeoX-0.6.0/setup.py` & `LeoX-0.6.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'LeoX'
 DESCRIPTION = 'Spectrum simulations with TD(A)-DFT'
 URL = 'https://github.com/LeonardoESousa/LeoX'
 EMAIL = 'leonardo.sousa137@gmail.com'
 AUTHOR = 'Leonardo Evaristo de Sousa'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.6.0'
+VERSION = '0.6.1'
 
 # What packages are required for this module to be executed?
 REQUIRED = ['numpy', 'scipy', 'pandas']
 
 # What packages are optional?
 EXTRAS = {
     # 'fancy feature': ['django'],
```

