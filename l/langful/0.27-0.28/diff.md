# Comparing `tmp/langful-0.27-py2.py3-none-any.whl.zip` & `tmp/langful-0.28-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 4643 bytes, number of entries: 7
+Zip file size: 4655 bytes, number of entries: 7
 -rw-rw-rw-  2.0 fat      224 b- defN 23-Jun-20 12:20 langful/__init__.py
--rw-rw-rw-  2.0 fat     6853 b- defN 23-Jun-20 15:46 langful/lang.py
--rw-rw-rw-  2.0 fat     1066 b- defN 23-Jun-20 15:50 langful-0.27.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2650 b- defN 23-Jun-20 15:50 langful-0.27.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 23-Jun-20 15:50 langful-0.27.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-Jun-20 15:50 langful-0.27.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      528 b- defN 23-Jun-20 15:50 langful-0.27.dist-info/RECORD
-7 files, 11439 bytes uncompressed, 3713 bytes compressed:  67.5%
+-rw-rw-rw-  2.0 fat     6933 b- defN 23-Jun-22 10:19 langful/lang.py
+-rw-rw-rw-  2.0 fat     1066 b- defN 23-Jun-22 10:20 langful-0.28.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     2650 b- defN 23-Jun-22 10:20 langful-0.28.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 23-Jun-22 10:20 langful-0.28.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Jun-22 10:20 langful-0.28.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      528 b- defN 23-Jun-22 10:20 langful-0.28.dist-info/RECORD
+7 files, 11519 bytes uncompressed, 3725 bytes compressed:  67.7%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: langful/__init__.py
 Comment: 
 
 Filename: langful/lang.py
 Comment: 
 
-Filename: langful-0.27.dist-info/LICENSE
+Filename: langful-0.28.dist-info/LICENSE
 Comment: 
 
-Filename: langful-0.27.dist-info/METADATA
+Filename: langful-0.28.dist-info/METADATA
 Comment: 
 
-Filename: langful-0.27.dist-info/WHEEL
+Filename: langful-0.28.dist-info/WHEEL
 Comment: 
 
-Filename: langful-0.27.dist-info/top_level.txt
+Filename: langful-0.28.dist-info/top_level.txt
 Comment: 
 
-Filename: langful-0.27.dist-info/RECORD
+Filename: langful-0.28.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## langful/lang.py

```diff
@@ -64,16 +64,18 @@
         for i in os.listdir( path ) :
             name , suffix = os.path.splitext( i )
             if ( suffix == ".json" ) or ( name + ".json" not in files ) :
                 files.append( i )
                 with open( os.path.join( path , i ) , encoding = "utf-8" ) as file :
                     if suffix == ".json" :
                         data = json.load( file )
-                    else :
+                    elif suffix == ".lang" :
                         data = lang_to_json( file.read() )
+                    else :
+                        continue
                 self.locales.append( name )
                 self.languages[ name ] = data
                 self.types[ name ] = suffix
 
     def init_dict( self , language : dict ) -> None :
         """
         init by a dictionary, but cant't to save
```

## Comparing `langful-0.27.dist-info/LICENSE` & `langful-0.28.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `langful-0.27.dist-info/METADATA` & `langful-0.28.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langful
-Version: 0.27
+Version: 0.28
 Home-page: https://github.com/cueavyqwp/langful
 Author: cueavyqwp
 Author-email: cueavyqwp@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: > 3.6
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: langful Version: 0.27 Home-page: https://
+Metadata-Version: 2.1 Name: langful Version: 0.28 Home-page: https://
 github.com/cueavyqwp/langful Author: cueavyqwp Author-email:
 cueavyqwp@outlook.com Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: > 3.6 Description-Content-Type: text/
 markdown License-File: LICENSE # langful
    [PyPI_version] [Python_version] [license] [Github_stars] [Github_issues]
 # install Use `pip` to install `pip install langful` or `pip3 install langful`
```

## Comparing `langful-0.27.dist-info/RECORD` & `langful-0.28.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 langful/__init__.py,sha256=81IWJcsG-rF5MEPRQOPJcbnRgs3n1KvcLUeWUiHp8nI,224
-langful/lang.py,sha256=TVe8KritBgdKat8CTZoyOBOjxhZj_wv0K6FqjRcpxFI,6853
-langful-0.27.dist-info/LICENSE,sha256=JrQca6fL66RGTmf-hkJU9UEX64JB0yE9gKNsOhpmZVE,1066
-langful-0.27.dist-info/METADATA,sha256=dHl-gQmKwwoqYT68RdNoDMn8fEahPZR71GJjd2Rjm4E,2650
-langful-0.27.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
-langful-0.27.dist-info/top_level.txt,sha256=EkKV_WnIZfE3A6EhWwDIt2uwZhMVHWXTUueKJL6K15w,8
-langful-0.27.dist-info/RECORD,,
+langful/lang.py,sha256=gRg4xhmKtP20495HdwVI_A9TEop51T3GXQsCIF1hIVI,6933
+langful-0.28.dist-info/LICENSE,sha256=JrQca6fL66RGTmf-hkJU9UEX64JB0yE9gKNsOhpmZVE,1066
+langful-0.28.dist-info/METADATA,sha256=p8TLIzr4Je022Zjt1VcVBOURgaoIVppGPYFrWPdTqjQ,2650
+langful-0.28.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
+langful-0.28.dist-info/top_level.txt,sha256=EkKV_WnIZfE3A6EhWwDIt2uwZhMVHWXTUueKJL6K15w,8
+langful-0.28.dist-info/RECORD,,
```

