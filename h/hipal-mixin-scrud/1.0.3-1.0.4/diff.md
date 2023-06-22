# Comparing `tmp/hipal_mixin_scrud-1.0.3.tar.gz` & `tmp/hipal_mixin_scrud-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\hipal_mixin_scrud-1.0.3.tar", last modified: Thu Jun 22 18:20:27 2023, max compression
+gzip compressed data, was "dist\hipal_mixin_scrud-1.0.4.tar", last modified: Thu Jun 22 18:36:34 2023, max compression
```

## Comparing `hipal_mixin_scrud-1.0.3.tar` & `hipal_mixin_scrud-1.0.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 18:20:27.075886 hipal_mixin_scrud-1.0.3/
--rw-rw-rw-   0        0        0     4613 2023-06-22 18:20:27.074885 hipal_mixin_scrud-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     3264 2023-06-22 18:16:36.000000 hipal_mixin_scrud-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-22 18:20:27.041888 hipal_mixin_scrud-1.0.3/hipal_mixin_scrud/
--rw-rw-rw-   0        0        0        0 2023-06-20 21:27:42.000000 hipal_mixin_scrud-1.0.3/hipal_mixin_scrud/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-22 18:20:27.060886 hipal_mixin_scrud-1.0.3/hipal_mixin_scrud/crud/
--rw-rw-rw-   0        0        0        0 2023-06-20 21:28:13.000000 hipal_mixin_scrud-1.0.3/hipal_mixin_scrud/crud/__init__.py
--rw-rw-rw-   0        0        0     5808 2023-06-22 17:44:55.000000 hipal_mixin_scrud-1.0.3/hipal_mixin_scrud/crud/generator.py
--rw-rw-rw-   0        0        0     3366 2023-06-22 17:45:00.000000 hipal_mixin_scrud-1.0.3/hipal_mixin_scrud/crud/mixin_list.py
-drwxrwxrwx   0        0        0        0 2023-06-22 18:20:27.067886 hipal_mixin_scrud-1.0.3/hipal_mixin_scrud/enums/
--rw-rw-rw-   0        0        0        0 2023-06-20 21:28:13.000000 hipal_mixin_scrud-1.0.3/hipal_mixin_scrud/enums/__init__.py
--rw-rw-rw-   0        0        0      255 2023-06-22 17:45:04.000000 hipal_mixin_scrud-1.0.3/hipal_mixin_scrud/enums/operators.py
--rw-rw-rw-   0        0        0       82 2023-06-22 17:45:06.000000 hipal_mixin_scrud-1.0.3/hipal_mixin_scrud/enums/sorts.py
--rw-rw-rw-   0        0        0     4691 2023-06-22 17:44:49.000000 hipal_mixin_scrud-1.0.3/hipal_mixin_scrud/mixin.py
-drwxrwxrwx   0        0        0        0 2023-06-22 18:20:27.072887 hipal_mixin_scrud-1.0.3/hipal_mixin_scrud/schemas/
--rw-rw-rw-   0        0        0        0 2023-06-20 21:28:13.000000 hipal_mixin_scrud-1.0.3/hipal_mixin_scrud/schemas/__init__.py
--rw-rw-rw-   0        0        0      352 2023-06-22 17:45:08.000000 hipal_mixin_scrud-1.0.3/hipal_mixin_scrud/schemas/paginate_params.py
--rw-rw-rw-   0        0        0      364 2023-06-22 17:45:13.000000 hipal_mixin_scrud-1.0.3/hipal_mixin_scrud/schemas/pagination_base.py
-drwxrwxrwx   0        0        0        0 2023-06-22 18:20:27.055889 hipal_mixin_scrud-1.0.3/hipal_mixin_scrud.egg-info/
--rw-rw-rw-   0        0        0     4613 2023-06-22 18:20:26.000000 hipal_mixin_scrud-1.0.3/hipal_mixin_scrud.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      621 2023-06-22 18:20:26.000000 hipal_mixin_scrud-1.0.3/hipal_mixin_scrud.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 18:20:26.000000 hipal_mixin_scrud-1.0.3/hipal_mixin_scrud.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-06-22 18:20:26.000000 hipal_mixin_scrud-1.0.3/hipal_mixin_scrud.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-06-22 18:20:26.000000 hipal_mixin_scrud-1.0.3/hipal_mixin_scrud.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-22 18:20:27.077886 hipal_mixin_scrud-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      788 2023-06-22 18:18:21.000000 hipal_mixin_scrud-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-22 18:36:34.691867 hipal_mixin_scrud-1.0.4/
+-rw-rw-rw-   0        0        0     5283 2023-06-22 18:36:34.690866 hipal_mixin_scrud-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3835 2023-06-22 18:34:44.000000 hipal_mixin_scrud-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-22 18:36:34.655990 hipal_mixin_scrud-1.0.4/hipal_mixin_scrud/
+-rw-rw-rw-   0        0        0        0 2023-06-20 21:27:42.000000 hipal_mixin_scrud-1.0.4/hipal_mixin_scrud/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-22 18:36:34.676867 hipal_mixin_scrud-1.0.4/hipal_mixin_scrud/crud/
+-rw-rw-rw-   0        0        0        0 2023-06-20 21:28:13.000000 hipal_mixin_scrud-1.0.4/hipal_mixin_scrud/crud/__init__.py
+-rw-rw-rw-   0        0        0     5808 2023-06-22 17:44:55.000000 hipal_mixin_scrud-1.0.4/hipal_mixin_scrud/crud/generator.py
+-rw-rw-rw-   0        0        0     3366 2023-06-22 17:45:00.000000 hipal_mixin_scrud-1.0.4/hipal_mixin_scrud/crud/mixin_list.py
+drwxrwxrwx   0        0        0        0 2023-06-22 18:36:34.682866 hipal_mixin_scrud-1.0.4/hipal_mixin_scrud/enums/
+-rw-rw-rw-   0        0        0        0 2023-06-20 21:28:13.000000 hipal_mixin_scrud-1.0.4/hipal_mixin_scrud/enums/__init__.py
+-rw-rw-rw-   0        0        0      255 2023-06-22 17:45:04.000000 hipal_mixin_scrud-1.0.4/hipal_mixin_scrud/enums/operators.py
+-rw-rw-rw-   0        0        0       82 2023-06-22 17:45:06.000000 hipal_mixin_scrud-1.0.4/hipal_mixin_scrud/enums/sorts.py
+-rw-rw-rw-   0        0        0     4691 2023-06-22 17:44:49.000000 hipal_mixin_scrud-1.0.4/hipal_mixin_scrud/mixin.py
+drwxrwxrwx   0        0        0        0 2023-06-22 18:36:34.688867 hipal_mixin_scrud-1.0.4/hipal_mixin_scrud/schemas/
+-rw-rw-rw-   0        0        0        0 2023-06-20 21:28:13.000000 hipal_mixin_scrud-1.0.4/hipal_mixin_scrud/schemas/__init__.py
+-rw-rw-rw-   0        0        0      352 2023-06-22 17:45:08.000000 hipal_mixin_scrud-1.0.4/hipal_mixin_scrud/schemas/paginate_params.py
+-rw-rw-rw-   0        0        0      364 2023-06-22 17:45:13.000000 hipal_mixin_scrud-1.0.4/hipal_mixin_scrud/schemas/pagination_base.py
+drwxrwxrwx   0        0        0        0 2023-06-22 18:36:34.671866 hipal_mixin_scrud-1.0.4/hipal_mixin_scrud.egg-info/
+-rw-rw-rw-   0        0        0     5283 2023-06-22 18:36:34.000000 hipal_mixin_scrud-1.0.4/hipal_mixin_scrud.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      621 2023-06-22 18:36:34.000000 hipal_mixin_scrud-1.0.4/hipal_mixin_scrud.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 18:36:34.000000 hipal_mixin_scrud-1.0.4/hipal_mixin_scrud.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-06-22 18:36:34.000000 hipal_mixin_scrud-1.0.4/hipal_mixin_scrud.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-06-22 18:36:34.000000 hipal_mixin_scrud-1.0.4/hipal_mixin_scrud.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-22 18:36:34.692866 hipal_mixin_scrud-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      788 2023-06-22 18:36:14.000000 hipal_mixin_scrud-1.0.4/setup.py
```

### Comparing `hipal_mixin_scrud-1.0.3/PKG-INFO` & `hipal_mixin_scrud-1.0.4/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hipal_mixin_scrud
-Version: 1.0.3
+Version: 1.0.4
 Summary: Libreria para crud basica.
 Home-page: http://git.hipal.com.co/libraries/ms-mixins/-/tree/feature/mixins
 Author: Hipal
 Author-email: desarrollo@hipal.com.co
 License: UNKNOWN
 Description: 
         # Hipal Mixin Scrud
@@ -107,14 +107,25 @@
             update_schema=UpdateUserSchema,
             query=default_query
         )
         ```
         
         El parametro query es opcional, y en caso de que se requiera recibira una funcion que como obligacion debera recibir por argument "request" y tendra que devolver la query que se requiera.
         
+        Paginación
+        ---------
+        
+        Para generar una paginacion es exactamente igual a lo dicho anteriormente, Sin embargo, recibe algunos parametros opcionales los cuales sirven para:
+        
+        - **offset**: Recibe el numero de la posicion del registro donde se requiere empezar a ver 
+        - **limit**: Limite de registros a visualizar
+        - **search**: Lista de campos con su valor a buscar separados por ; ejemplo: name=alan;company=Gooogle
+        - **sort**: ASC o DESC para especificar si se requiere el orden descendente o ascendente
+        - **sort_field**: Nombre del campo por el cual se requiere ordenar
+        
         Adicionalmente se podra user "users_router" para generar las rutas como generalmente las conocemos:
         
         ```
         @users_router.get("/me", response_model=UserSchema)
         def endpoint() -> UserSchema:
             return {"msg":"prueba"}
         ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `hipal_mixin_scrud-1.0.3/README.md` & `hipal_mixin_scrud-1.0.4/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -99,14 +99,25 @@
     update_schema=UpdateUserSchema,
     query=default_query
 )
 ```
 
 El parametro query es opcional, y en caso de que se requiera recibira una funcion que como obligacion debera recibir por argument "request" y tendra que devolver la query que se requiera.
 
+Paginación
+---------
+
+Para generar una paginacion es exactamente igual a lo dicho anteriormente, Sin embargo, recibe algunos parametros opcionales los cuales sirven para:
+
+- **offset**: Recibe el numero de la posicion del registro donde se requiere empezar a ver 
+- **limit**: Limite de registros a visualizar
+- **search**: Lista de campos con su valor a buscar separados por ; ejemplo: name=alan;company=Gooogle
+- **sort**: ASC o DESC para especificar si se requiere el orden descendente o ascendente
+- **sort_field**: Nombre del campo por el cual se requiere ordenar
+
 Adicionalmente se podra user "users_router" para generar las rutas como generalmente las conocemos:
 
 ```
 @users_router.get("/me", response_model=UserSchema)
 def endpoint() -> UserSchema:
     return {"msg":"prueba"}
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `hipal_mixin_scrud-1.0.3/hipal_mixin_scrud/crud/generator.py` & `hipal_mixin_scrud-1.0.4/hipal_mixin_scrud/crud/generator.py`

 * *Files identical despite different names*

### Comparing `hipal_mixin_scrud-1.0.3/hipal_mixin_scrud/crud/mixin_list.py` & `hipal_mixin_scrud-1.0.4/hipal_mixin_scrud/crud/mixin_list.py`

 * *Files identical despite different names*

### Comparing `hipal_mixin_scrud-1.0.3/hipal_mixin_scrud/mixin.py` & `hipal_mixin_scrud-1.0.4/hipal_mixin_scrud/mixin.py`

 * *Files identical despite different names*

### Comparing `hipal_mixin_scrud-1.0.3/hipal_mixin_scrud.egg-info/PKG-INFO` & `hipal_mixin_scrud-1.0.4/hipal_mixin_scrud.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hipal-mixin-scrud
-Version: 1.0.3
+Version: 1.0.4
 Summary: Libreria para crud basica.
 Home-page: http://git.hipal.com.co/libraries/ms-mixins/-/tree/feature/mixins
 Author: Hipal
 Author-email: desarrollo@hipal.com.co
 License: UNKNOWN
 Description: 
         # Hipal Mixin Scrud
@@ -107,14 +107,25 @@
             update_schema=UpdateUserSchema,
             query=default_query
         )
         ```
         
         El parametro query es opcional, y en caso de que se requiera recibira una funcion que como obligacion debera recibir por argument "request" y tendra que devolver la query que se requiera.
         
+        Paginación
+        ---------
+        
+        Para generar una paginacion es exactamente igual a lo dicho anteriormente, Sin embargo, recibe algunos parametros opcionales los cuales sirven para:
+        
+        - **offset**: Recibe el numero de la posicion del registro donde se requiere empezar a ver 
+        - **limit**: Limite de registros a visualizar
+        - **search**: Lista de campos con su valor a buscar separados por ; ejemplo: name=alan;company=Gooogle
+        - **sort**: ASC o DESC para especificar si se requiere el orden descendente o ascendente
+        - **sort_field**: Nombre del campo por el cual se requiere ordenar
+        
         Adicionalmente se podra user "users_router" para generar las rutas como generalmente las conocemos:
         
         ```
         @users_router.get("/me", response_model=UserSchema)
         def endpoint() -> UserSchema:
             return {"msg":"prueba"}
         ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `hipal_mixin_scrud-1.0.3/hipal_mixin_scrud.egg-info/SOURCES.txt` & `hipal_mixin_scrud-1.0.4/hipal_mixin_scrud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hipal_mixin_scrud-1.0.3/setup.py` & `hipal_mixin_scrud-1.0.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # Lee el contenido del archivo README.md
 readme_path = Path(__file__).parent / "README.md"
 with open(readme_path, "r", encoding="utf-8") as f:
     long_description = f.read()
     
 setup(
     name="hipal_mixin_scrud",
-    version="1.0.3",
+    version="1.0.4",
     description="Libreria para crud basica.",
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
     python_requires=">=3.9",
     install_requires=[
         "pydantic==1.10.7",
```

