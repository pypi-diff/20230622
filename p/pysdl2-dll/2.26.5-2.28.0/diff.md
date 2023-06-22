# Comparing `tmp/pysdl2-dll-2.26.5.tar.gz` & `tmp/pysdl2-dll-2.28.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysdl2-dll-2.26.5.tar", last modified: Tue May  2 14:17:28 2023, max compression
+gzip compressed data, was "pysdl2-dll-2.28.0.tar", last modified: Thu Jun 22 19:51:07 2023, max compression
```

## Comparing `pysdl2-dll-2.26.5.tar` & `pysdl2-dll-2.28.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:17:28.111384 pysdl2-dll-2.26.5/
--rw-r--r--   0 root         (0) root         (0)    16725 2023-05-02 14:17:26.000000 pysdl2-dll-2.26.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)       34 2023-05-02 14:17:26.000000 pysdl2-dll-2.26.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4322 2023-05-02 14:17:28.111384 pysdl2-dll-2.26.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3529 2023-05-02 14:17:26.000000 pysdl2-dll-2.26.5/README.md
--rw-r--r--   0 root         (0) root         (0)    19001 2023-05-02 14:17:26.000000 pysdl2-dll-2.26.5/getdlls.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:17:28.110384 pysdl2-dll-2.26.5/pysdl2_dll.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4322 2023-05-02 14:17:28.000000 pysdl2-dll-2.26.5/pysdl2_dll.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      236 2023-05-02 14:17:28.000000 pysdl2-dll-2.26.5/pysdl2_dll.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-02 14:17:28.000000 pysdl2-dll-2.26.5/pysdl2_dll.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-02 14:17:28.000000 pysdl2-dll-2.26.5/pysdl2_dll.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:17:28.111384 pysdl2-dll-2.26.5/sdl2dll/
--rw-r--r--   0 root         (0) root         (0)      419 2023-05-02 14:17:26.000000 pysdl2-dll-2.26.5/sdl2dll/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2567 2023-05-02 14:17:26.000000 pysdl2-dll-2.26.5/sdl2dll/initcheck.py
--rw-r--r--   0 root         (0) root         (0)      116 2023-05-02 14:17:28.111384 pysdl2-dll-2.26.5/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     2534 2023-05-02 14:17:26.000000 pysdl2-dll-2.26.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 19:51:07.452593 pysdl2-dll-2.28.0/
+-rw-r--r--   0 root         (0) root         (0)    16725 2023-06-22 19:51:06.000000 pysdl2-dll-2.28.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       34 2023-06-22 19:51:06.000000 pysdl2-dll-2.28.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4110 2023-06-22 19:51:07.452593 pysdl2-dll-2.28.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3317 2023-06-22 19:51:06.000000 pysdl2-dll-2.28.0/README.md
+-rw-r--r--   0 root         (0) root         (0)    19066 2023-06-22 19:51:06.000000 pysdl2-dll-2.28.0/getdlls.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 19:51:07.452593 pysdl2-dll-2.28.0/pysdl2_dll.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4110 2023-06-22 19:51:07.000000 pysdl2-dll-2.28.0/pysdl2_dll.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      236 2023-06-22 19:51:07.000000 pysdl2-dll-2.28.0/pysdl2_dll.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 19:51:07.000000 pysdl2-dll-2.28.0/pysdl2_dll.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-22 19:51:07.000000 pysdl2-dll-2.28.0/pysdl2_dll.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 19:51:07.452593 pysdl2-dll-2.28.0/sdl2dll/
+-rw-r--r--   0 root         (0) root         (0)      419 2023-06-22 19:51:06.000000 pysdl2-dll-2.28.0/sdl2dll/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2567 2023-06-22 19:51:06.000000 pysdl2-dll-2.28.0/sdl2dll/initcheck.py
+-rw-r--r--   0 root         (0) root         (0)      116 2023-06-22 19:51:07.453593 pysdl2-dll-2.28.0/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     2534 2023-06-22 19:51:06.000000 pysdl2-dll-2.28.0/setup.py
```

### Comparing `pysdl2-dll-2.26.5/LICENSE` & `pysdl2-dll-2.28.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pysdl2-dll-2.26.5/PKG-INFO` & `pysdl2-dll-2.28.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysdl2-dll
-Version: 2.26.5
+Version: 2.28.0
 Summary: Pre-built SDL2 binaries for PySDL2
 Home-page: https://github.com/a-hurst/pysdl2-dll
 Author: Austin Hurst
 Author-email: mynameisaustinhurst@gmail.com
 License: Mozilla Public License Version 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
@@ -28,15 +28,15 @@
 
 It uses the official SDL2, SDL2\_mixer, SDL2\_ttf, and SDL2\_image binaries for macOS and Windows, as well as [unofficial SDL2\_gfx binaries](https://github.com/a-hurst/sdl2gfx-builds) for the same platforms. For Linux, the SDL2 binaries and their dependencies are all built from source using the official Python [manylinux](https://github.com/pypa/manylinux) images for maximum compatibility.
 
 The latest release includes the following versions of the SDL2 binaries:
 
 SDL2 | SDL2\_ttf | SDL2\_mixer | SDL2\_image | SDL2\_gfx
 --- | --- | --- | --- | ---
-2.26.5 | 2.20.0 | 2.6.0 | 2.6.0 | 1.0.4
+2.28.0 | 2.20.0 | 2.6.0 | 2.6.0 | 1.0.4
 
 Note that the mixer and image libraries are pinned at their current versions until their next major release due to a regression in the macOS binaries.
 
 
 ## Installation
 
 You can install the latest version of pysdl2-dll via pip:
@@ -56,15 +56,15 @@
 * Windows (64-bit x86)
 * Linux (32-bit x86)
 * Linux (64-bit x86)
 * Linux (64-bit ARM)
 
 The pysdl2-dll package can be *installed* on platforms other than the ones listed above, but it won't have any effect.
 
-pysdl2-dll requires PySDL2 0.9.7 or later in order to work correctly on macOS, and for PySDL2 to load the binaries automatically when available. To update to the latest PySDL2, you can run:
+pysdl2-dll requires PySDL2 0.9.7 or later in order to work correctly. To update to the latest PySDL2, you can run:
 
 ```bash
 pip install -U pysdl2
 ```
 
 Because the wheels are not built against any specfic version of Python, pysdl2-dll supports all versions and implementations of Python that are supported by PySDL2.
 
@@ -74,12 +74,12 @@
 There are currently two versions the Linux wheels: "legacy" wheels based on the `manylinux2014` standard (for 32-bit and 64-bit x86), and "modern" wheels based on the `manylinux_2_28` standard (for 64-bit x86 and 64-bit ARM only). The `manylinux_2_28` SDL2 binaries require a more recent version of Linux, but offer dynamic support for additional features such as native Wayland windowing, Pipewire audio, and Vulkan rendering.
 
 You must have pip 19.3 or newer to install the `manylinux2014` wheels, and pip 20.3 or newer to install the `manylinux_2_28` wheels. Distributions that use musl C instead of glibc (e.g. Alpine Linux) are not supported.
 
 
 ## Usage
 
-If you are using PySDL2 0.9.7 or later, you don't need to do anything special to use the pysdl2-dll binaries in your project: PySDL2 will load them automatically (and print a message indicating such) if they are available. For older versions of PySDL2, you will need to import this module manually in your scripts (`import sdl2dll`) before PySDL2 is imported.
+If you are using PySDL2 0.9.7 or later, you don't need to do anything special to use the pysdl2-dll binaries in your project: PySDL2 will load them automatically (and print a message indicating such) if they are available.
 
 To override pysdl2-dll and use a different set of binaries, you can set the `PYSDL2_DLL_PATH` environment variable to the path of the folder containing the binaries you want to use instead, or alternatively set it to "system" to force PySDL2 to use the system install of SDL2 if available (e.g. SDL2 installed with `brew` on macOS).
```

### Comparing `pysdl2-dll-2.26.5/README.md` & `pysdl2-dll-2.28.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 It uses the official SDL2, SDL2\_mixer, SDL2\_ttf, and SDL2\_image binaries for macOS and Windows, as well as [unofficial SDL2\_gfx binaries](https://github.com/a-hurst/sdl2gfx-builds) for the same platforms. For Linux, the SDL2 binaries and their dependencies are all built from source using the official Python [manylinux](https://github.com/pypa/manylinux) images for maximum compatibility.
 
 The latest release includes the following versions of the SDL2 binaries:
 
 SDL2 | SDL2\_ttf | SDL2\_mixer | SDL2\_image | SDL2\_gfx
 --- | --- | --- | --- | ---
-2.26.5 | 2.20.0 | 2.6.0 | 2.6.0 | 1.0.4
+2.28.0 | 2.20.0 | 2.6.0 | 2.6.0 | 1.0.4
 
 Note that the mixer and image libraries are pinned at their current versions until their next major release due to a regression in the macOS binaries.
 
 
 ## Installation
 
 You can install the latest version of pysdl2-dll via pip:
@@ -35,15 +35,15 @@
 * Windows (64-bit x86)
 * Linux (32-bit x86)
 * Linux (64-bit x86)
 * Linux (64-bit ARM)
 
 The pysdl2-dll package can be *installed* on platforms other than the ones listed above, but it won't have any effect.
 
-pysdl2-dll requires PySDL2 0.9.7 or later in order to work correctly on macOS, and for PySDL2 to load the binaries automatically when available. To update to the latest PySDL2, you can run:
+pysdl2-dll requires PySDL2 0.9.7 or later in order to work correctly. To update to the latest PySDL2, you can run:
 
 ```bash
 pip install -U pysdl2
 ```
 
 Because the wheels are not built against any specfic version of Python, pysdl2-dll supports all versions and implementations of Python that are supported by PySDL2.
 
@@ -53,10 +53,10 @@
 There are currently two versions the Linux wheels: "legacy" wheels based on the `manylinux2014` standard (for 32-bit and 64-bit x86), and "modern" wheels based on the `manylinux_2_28` standard (for 64-bit x86 and 64-bit ARM only). The `manylinux_2_28` SDL2 binaries require a more recent version of Linux, but offer dynamic support for additional features such as native Wayland windowing, Pipewire audio, and Vulkan rendering.
 
 You must have pip 19.3 or newer to install the `manylinux2014` wheels, and pip 20.3 or newer to install the `manylinux_2_28` wheels. Distributions that use musl C instead of glibc (e.g. Alpine Linux) are not supported.
 
 
 ## Usage
 
-If you are using PySDL2 0.9.7 or later, you don't need to do anything special to use the pysdl2-dll binaries in your project: PySDL2 will load them automatically (and print a message indicating such) if they are available. For older versions of PySDL2, you will need to import this module manually in your scripts (`import sdl2dll`) before PySDL2 is imported.
+If you are using PySDL2 0.9.7 or later, you don't need to do anything special to use the pysdl2-dll binaries in your project: PySDL2 will load them automatically (and print a message indicating such) if they are available.
 
 To override pysdl2-dll and use a different set of binaries, you can set the `PYSDL2_DLL_PATH` environment variable to the path of the folder containing the binaries you want to use instead, or alternatively set it to "system" to force PySDL2 to use the system install of SDL2 if available (e.g. SDL2 installed with `brew` on macOS).
```

### Comparing `pysdl2-dll-2.26.5/getdlls.py` & `pysdl2-dll-2.28.0/getdlls.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 import os
 import sys
+import time
 import shutil
 import tarfile
 import subprocess as sub
 from zipfile import ZipFile
 from distutils.util import get_platform
 
 try:
+    import urllib.request
     from urllib.request import urlopen # Python 3.x
 except ImportError:
     from urllib2 import urlopen # Python 2
 
 
 libraries = ['SDL2', 'SDL2_mixer', 'SDL2_ttf', 'SDL2_image', 'SDL2_gfx']
 
 libversions = {
-    'SDL2': '2.26.5',
+    'SDL2': '2.28.0',
     'SDL2_mixer': '2.6.0',
     'SDL2_ttf': '2.20.0',
     'SDL2_image': '2.6.0',
     'SDL2_gfx': '1.0.4'
 }
 
 url_fmt = 'https://github.com/libsdl-org/SDL{LIB}/releases/download/release-{0}/SDL2{LIB}-{0}{1}'
@@ -77,23 +79,21 @@
             dllname = lib + '.framework'
             dllpath = os.path.join(mountpoint, dllname)
             dlloutpath = os.path.join(dlldir, dllname)
             optpath = os.path.join(mountpoint, 'optional')
             extraframeworkpath = os.path.join(dlloutpath, 'Versions', 'A', 'Frameworks')
             
             # Download disk image containing library
+            outpath = os.path.join('temp', lib + '.dmg')
             if lib in ['SDL2_image', 'SDL2_mixer']:
                 # NOTE: Temporary workaround for optional frameworks until 2.8.0
-                dmg = urlopen('https://www.libsdl.org/tmp/{0}-2.7.0.dmg'.format(lib))
+                download('https://www.libsdl.org/tmp/{0}-2.7.0.dmg'.format(lib), outpath)
             else:
                 libversion = libversions[lib]
-                dmg = urlopen(sdl2_urls[lib].format(libversion, '.dmg'))
-            outpath = os.path.join('temp', lib + '.dmg')
-            with open(outpath, 'wb') as out:
-                out.write(dmg.read())
+                download(sdl2_urls[lib].format(libversion, '.dmg'), outpath)
             
             # Mount image, extract framework (and any optional frameworks), then unmount
             sub.check_call(['hdiutil', 'attach', outpath, '-mountpoint', mountpoint])
             shutil.copytree(dllpath, dlloutpath, symlinks=True, ignore=find_symlinks)
             if os.path.isdir(optpath):
                 shutil.copytree(
                     optpath, extraframeworkpath, symlinks=True, ignore=find_symlinks
@@ -123,18 +123,16 @@
         
         suffix = '-win32-x64.zip' if platform_name == 'win-amd64' else '-win32-x86.zip'
         
         for lib in libraries:
             
             # Download zip archive containing library
             libversion = libversions[lib]
-            dllzip = urlopen(sdl2_urls[lib].format(libversion, suffix))
             outpath = os.path.join('temp', lib + '.zip')
-            with open(outpath, 'wb') as out:
-                out.write(dllzip.read())
+            download(sdl2_urls[lib].format(libversion, suffix), outpath)
             
             # Extract dlls and license files from archive
             with ZipFile(outpath, 'r') as z:
                 for name in z.namelist():
                     if name[-4:] == '.dll':
                         z.extract(name, dlldir)
                     elif 'LICENSE' in name:
@@ -156,18 +154,16 @@
             shutil.rmtree(libdir)
         os.mkdir(libdir)
 
         # Download and use license files from official Windows binaries
         for lib in libraries:
             # Download zip archive containing library
             libversion = libversions[lib]
-            dllzip = urlopen(sdl2_urls[lib].format(libversion, '-win32-x64.zip'))
             outpath = os.path.join('temp', lib + '.zip')
-            with open(outpath, 'wb') as out:
-                out.write(dllzip.read())
+            download(sdl2_urls[lib].format(libversion, '-win32-x64.zip'), outpath)
 
             # Extract license files from archive
             with ZipFile(outpath, 'r') as z:
                 for name in z.namelist():
                     if 'LICENSE' in name:
                         z.extract(name, licensedir)
 
@@ -317,26 +313,40 @@
     return links
 
 
 def fetch_source(libfolder, liburl, outdir):
     """Downloads and decompresses the source code for a given library.
     """
     # Download tarfile to temporary folder
-    srctar = urlopen(liburl)
     outpath = os.path.join(outdir, libfolder + '.tar.gz')
-    with open(outpath, 'wb') as out:
-        out.write(srctar.read())
+    download(liburl, outpath)
 
     # Extract source from archive
     with tarfile.open(outpath, 'r:gz') as z:
         z.extractall(path=outdir)
 
     return os.path.join(outdir, libfolder)
 
 
+def download(url, outpath):
+    """Downloads a file from a URL to a given path.
+    """
+    attempts = 0
+    while attempts < 3:
+        try:
+            data = urlopen(url)
+            break
+        except OSError:
+            time.sleep(0.2)
+            attempts += 1
+
+    with open(outpath, 'wb') as out:
+        out.write(data.read())
+
+
 def download_external(ext_path):
     """Downloads the available optional dependencies for a library.
     """
     orig_path = os.getcwd()
     os.chdir(ext_path)
     
     p = sub.Popen("./download.sh", stdout=sys.stdout, stderr=sys.stderr)
```

### Comparing `pysdl2-dll-2.26.5/pysdl2_dll.egg-info/PKG-INFO` & `pysdl2-dll-2.28.0/pysdl2_dll.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysdl2-dll
-Version: 2.26.5
+Version: 2.28.0
 Summary: Pre-built SDL2 binaries for PySDL2
 Home-page: https://github.com/a-hurst/pysdl2-dll
 Author: Austin Hurst
 Author-email: mynameisaustinhurst@gmail.com
 License: Mozilla Public License Version 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
@@ -28,15 +28,15 @@
 
 It uses the official SDL2, SDL2\_mixer, SDL2\_ttf, and SDL2\_image binaries for macOS and Windows, as well as [unofficial SDL2\_gfx binaries](https://github.com/a-hurst/sdl2gfx-builds) for the same platforms. For Linux, the SDL2 binaries and their dependencies are all built from source using the official Python [manylinux](https://github.com/pypa/manylinux) images for maximum compatibility.
 
 The latest release includes the following versions of the SDL2 binaries:
 
 SDL2 | SDL2\_ttf | SDL2\_mixer | SDL2\_image | SDL2\_gfx
 --- | --- | --- | --- | ---
-2.26.5 | 2.20.0 | 2.6.0 | 2.6.0 | 1.0.4
+2.28.0 | 2.20.0 | 2.6.0 | 2.6.0 | 1.0.4
 
 Note that the mixer and image libraries are pinned at their current versions until their next major release due to a regression in the macOS binaries.
 
 
 ## Installation
 
 You can install the latest version of pysdl2-dll via pip:
@@ -56,15 +56,15 @@
 * Windows (64-bit x86)
 * Linux (32-bit x86)
 * Linux (64-bit x86)
 * Linux (64-bit ARM)
 
 The pysdl2-dll package can be *installed* on platforms other than the ones listed above, but it won't have any effect.
 
-pysdl2-dll requires PySDL2 0.9.7 or later in order to work correctly on macOS, and for PySDL2 to load the binaries automatically when available. To update to the latest PySDL2, you can run:
+pysdl2-dll requires PySDL2 0.9.7 or later in order to work correctly. To update to the latest PySDL2, you can run:
 
 ```bash
 pip install -U pysdl2
 ```
 
 Because the wheels are not built against any specfic version of Python, pysdl2-dll supports all versions and implementations of Python that are supported by PySDL2.
 
@@ -74,12 +74,12 @@
 There are currently two versions the Linux wheels: "legacy" wheels based on the `manylinux2014` standard (for 32-bit and 64-bit x86), and "modern" wheels based on the `manylinux_2_28` standard (for 64-bit x86 and 64-bit ARM only). The `manylinux_2_28` SDL2 binaries require a more recent version of Linux, but offer dynamic support for additional features such as native Wayland windowing, Pipewire audio, and Vulkan rendering.
 
 You must have pip 19.3 or newer to install the `manylinux2014` wheels, and pip 20.3 or newer to install the `manylinux_2_28` wheels. Distributions that use musl C instead of glibc (e.g. Alpine Linux) are not supported.
 
 
 ## Usage
 
-If you are using PySDL2 0.9.7 or later, you don't need to do anything special to use the pysdl2-dll binaries in your project: PySDL2 will load them automatically (and print a message indicating such) if they are available. For older versions of PySDL2, you will need to import this module manually in your scripts (`import sdl2dll`) before PySDL2 is imported.
+If you are using PySDL2 0.9.7 or later, you don't need to do anything special to use the pysdl2-dll binaries in your project: PySDL2 will load them automatically (and print a message indicating such) if they are available.
 
 To override pysdl2-dll and use a different set of binaries, you can set the `PYSDL2_DLL_PATH` environment variable to the path of the folder containing the binaries you want to use instead, or alternatively set it to "system" to force PySDL2 to use the system install of SDL2 if available (e.g. SDL2 installed with `brew` on macOS).
```

### Comparing `pysdl2-dll-2.26.5/sdl2dll/initcheck.py` & `pysdl2-dll-2.28.0/sdl2dll/initcheck.py`

 * *Files identical despite different names*

### Comparing `pysdl2-dll-2.26.5/setup.py` & `pysdl2-dll-2.28.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 # Install the package
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
 	name='pysdl2-dll',
-	version='2.26.5',
+	version='2.28.0',
 	author='Austin Hurst',
 	author_email='mynameisaustinhurst@gmail.com',
     license='Mozilla Public License Version 2.0',
     description='Pre-built SDL2 binaries for PySDL2',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/a-hurst/pysdl2-dll',
```

