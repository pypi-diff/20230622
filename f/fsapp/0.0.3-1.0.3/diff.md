# Comparing `tmp/fsapp-0.0.3.tar.gz` & `tmp/fsapp-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fsapp-0.0.3.tar", last modified: Thu May 11 12:33:50 2023, max compression
+gzip compressed data, was "fsapp-1.0.3.tar", last modified: Thu Jun 22 13:57:51 2023, max compression
```

## Comparing `fsapp-0.0.3.tar` & `fsapp-1.0.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 12:33:50.542307 fsapp-0.0.3/
--rw-rw-rw-   0        0        0     1091 2023-03-29 11:26:53.000000 fsapp-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      329 2023-05-11 12:33:50.542307 fsapp-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0    12293 2023-05-11 06:34:33.000000 fsapp-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-11 12:33:50.388839 fsapp-0.0.3/fsapp/
--rw-rw-rw-   0        0        0      234 2023-03-29 08:18:14.000000 fsapp-0.0.3/fsapp/__init__.py
--rw-rw-rw-   0        0        0     1891 2023-05-11 12:33:20.000000 fsapp-0.0.3/fsapp/__main__.py
-drwxrwxrwx   0        0        0        0 2023-05-11 12:33:50.426632 fsapp-0.0.3/fsapp/api/
--rw-rw-rw-   0        0        0        0 2023-03-11 15:02:46.000000 fsapp-0.0.3/fsapp/api/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-11 12:33:50.473522 fsapp-0.0.3/fsapp/api/endpoints/
--rw-rw-rw-   0        0        0        0 2023-03-11 15:20:14.000000 fsapp-0.0.3/fsapp/api/endpoints/__init__.py
--rw-rw-rw-   0        0        0     1327 2023-03-29 07:55:56.000000 fsapp-0.0.3/fsapp/api/endpoints/auth.py
--rw-rw-rw-   0        0        0     1955 2023-05-03 14:11:55.000000 fsapp-0.0.3/fsapp/api/endpoints/search.py
--rw-rw-rw-   0        0        0      442 2023-04-01 07:48:00.000000 fsapp-0.0.3/fsapp/api/endpoints/utils.py
--rw-rw-rw-   0        0        0      310 2023-03-29 07:55:56.000000 fsapp-0.0.3/fsapp/api/routers.py
-drwxrwxrwx   0        0        0        0 2023-05-11 12:33:50.504814 fsapp-0.0.3/fsapp/api/schemas/
--rw-rw-rw-   0        0        0        0 2023-03-11 15:03:17.000000 fsapp-0.0.3/fsapp/api/schemas/__init__.py
--rw-rw-rw-   0        0        0      755 2023-03-15 13:08:09.000000 fsapp-0.0.3/fsapp/api/schemas/requests.py
--rw-rw-rw-   0        0        0      628 2023-03-15 13:12:47.000000 fsapp-0.0.3/fsapp/api/schemas/responses.py
--rw-rw-rw-   0        0        0      703 2023-05-03 13:11:19.000000 fsapp-0.0.3/fsapp/base.py
--rw-rw-rw-   0        0        0      929 2023-05-03 14:22:38.000000 fsapp-0.0.3/fsapp/classes.py
-drwxrwxrwx   0        0        0        0 2023-05-11 12:33:50.526666 fsapp-0.0.3/fsapp/core/
--rw-rw-rw-   0        0        0        0 2023-03-11 15:19:31.000000 fsapp-0.0.3/fsapp/core/__init__.py
--rw-rw-rw-   0        0        0     1220 2023-03-31 11:05:16.000000 fsapp-0.0.3/fsapp/core/config.py
--rw-rw-rw-   0        0        0      418 2023-05-03 14:11:55.000000 fsapp-0.0.3/fsapp/core/handlers.py
-drwxrwxrwx   0        0        0        0 2023-05-11 12:33:50.426632 fsapp-0.0.3/fsapp.egg-info/
--rw-rw-rw-   0        0        0      329 2023-05-11 12:33:50.000000 fsapp-0.0.3/fsapp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      587 2023-05-11 12:33:50.000000 fsapp-0.0.3/fsapp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 12:33:50.000000 fsapp-0.0.3/fsapp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      360 2023-05-11 12:33:50.000000 fsapp-0.0.3/fsapp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-11 12:33:50.000000 fsapp-0.0.3/fsapp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1057 2023-05-11 12:28:36.000000 fsapp-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-11 12:33:50.542307 fsapp-0.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-11 12:33:50.542307 fsapp-0.0.3/tests/
--rw-rw-rw-   0        0        0      320 2023-03-29 12:55:11.000000 fsapp-0.0.3/tests/test_endpoints.py
+drwxrwxrwx   0        0        0        0 2023-06-22 13:57:51.390213 fsapp-1.0.3/
+-rw-rw-rw-   0        0        0     1091 2023-03-29 11:26:53.000000 fsapp-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0      329 2023-06-22 13:57:51.390213 fsapp-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0    12282 2023-05-11 13:29:45.000000 fsapp-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-22 13:57:51.338297 fsapp-1.0.3/fsapp/
+-rw-rw-rw-   0        0        0      234 2023-03-29 08:18:14.000000 fsapp-1.0.3/fsapp/__init__.py
+-rw-rw-rw-   0        0        0     1891 2023-05-11 12:33:20.000000 fsapp-1.0.3/fsapp/__main__.py
+drwxrwxrwx   0        0        0        0 2023-06-22 13:57:51.353922 fsapp-1.0.3/fsapp/api/
+-rw-rw-rw-   0        0        0        0 2023-03-11 15:02:46.000000 fsapp-1.0.3/fsapp/api/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-22 13:57:51.369569 fsapp-1.0.3/fsapp/api/endpoints/
+-rw-rw-rw-   0        0        0        0 2023-03-11 15:20:14.000000 fsapp-1.0.3/fsapp/api/endpoints/__init__.py
+-rw-rw-rw-   0        0        0     1327 2023-03-29 07:55:56.000000 fsapp-1.0.3/fsapp/api/endpoints/auth.py
+-rw-rw-rw-   0        0        0     1875 2023-06-22 13:30:32.000000 fsapp-1.0.3/fsapp/api/endpoints/search.py
+-rw-rw-rw-   0        0        0      442 2023-04-01 07:48:00.000000 fsapp-1.0.3/fsapp/api/endpoints/utils.py
+-rw-rw-rw-   0        0        0      310 2023-03-29 07:55:56.000000 fsapp-1.0.3/fsapp/api/routers.py
+drwxrwxrwx   0        0        0        0 2023-06-22 13:57:51.374578 fsapp-1.0.3/fsapp/api/schemas/
+-rw-rw-rw-   0        0        0        0 2023-03-11 15:03:17.000000 fsapp-1.0.3/fsapp/api/schemas/__init__.py
+-rw-rw-rw-   0        0        0      253 2023-06-22 13:06:35.000000 fsapp-1.0.3/fsapp/api/schemas/requests.py
+-rw-rw-rw-   0        0        0      628 2023-03-15 13:12:47.000000 fsapp-1.0.3/fsapp/api/schemas/responses.py
+-rw-rw-rw-   0        0        0      615 2023-06-22 13:55:05.000000 fsapp-1.0.3/fsapp/base.py
+-rw-rw-rw-   0        0        0      929 2023-05-03 14:22:38.000000 fsapp-1.0.3/fsapp/classes.py
+drwxrwxrwx   0        0        0        0 2023-06-22 13:57:51.374578 fsapp-1.0.3/fsapp/core/
+-rw-rw-rw-   0        0        0        0 2023-03-11 15:19:31.000000 fsapp-1.0.3/fsapp/core/__init__.py
+-rw-rw-rw-   0        0        0     1173 2023-06-22 13:55:05.000000 fsapp-1.0.3/fsapp/core/config.py
+-rw-rw-rw-   0        0        0      418 2023-05-03 14:11:55.000000 fsapp-1.0.3/fsapp/core/handlers.py
+drwxrwxrwx   0        0        0        0 2023-06-22 13:57:51.353922 fsapp-1.0.3/fsapp.egg-info/
+-rw-rw-rw-   0        0        0      329 2023-06-22 13:57:51.000000 fsapp-1.0.3/fsapp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      587 2023-06-22 13:57:51.000000 fsapp-1.0.3/fsapp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 13:57:51.000000 fsapp-1.0.3/fsapp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      360 2023-06-22 13:57:51.000000 fsapp-1.0.3/fsapp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-22 13:57:51.000000 fsapp-1.0.3/fsapp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1057 2023-06-22 13:06:55.000000 fsapp-1.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-22 13:57:51.390213 fsapp-1.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-22 13:57:51.374578 fsapp-1.0.3/tests/
+-rw-rw-rw-   0        0        0      340 2023-06-22 13:56:28.000000 fsapp-1.0.3/tests/test_endpoints.py
```

### Comparing `fsapp-0.0.3/LICENSE` & `fsapp-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fsapp-0.0.3/README.md` & `fsapp-1.0.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 возможность не писать код для маршрутизирования, моделей и обработки запросов. Достаточно написать свой класс-обработчик,
 при этом соблюдая некторые требования, и ваш REST-API **узел** готов.
 
 Под узлом подразумевается то, что Ваш веб-сервис одна из точек обработки, соединенных с помощью шлюзового API. Схемка 
 для наглядности.
 
 ```mermaid
-graph TD;
-    A(Client) -->|Request| B(GateApi) -->|Response| A;
-    B --> D[ApiNode1] --> B;
-    B --> E[ApiNode2] --> B;
-    B --> F[Ваш ApiNode] --> B;
+graph TD
+    A(Client) -->|Request| B(GateApi) -->|Response| A
+    B --> D[ApiNode1] --> B
+    B --> E[ApiNode2] --> B
+    B --> F[Ваш ApiNode]
 ```
 
 ### Обобщение
 
 ---
 Для развертывания вашего собственного web-сервиса с REST API архитектурой:
```

### Comparing `fsapp-0.0.3/fsapp/__main__.py` & `fsapp-1.0.3/fsapp/__main__.py`

 * *Files identical despite different names*

### Comparing `fsapp-0.0.3/fsapp/api/endpoints/auth.py` & `fsapp-1.0.3/fsapp/api/endpoints/auth.py`

 * *Files identical despite different names*

### Comparing `fsapp-0.0.3/fsapp/api/endpoints/search.py` & `fsapp-1.0.3/fsapp/api/endpoints/search.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """Марштруты для запроса данных и вспомогательных действий"""
 
 from fastapi import APIRouter, Depends, HTTPException
-from typing import Tuple, Union
 
 from .utils import make_response
 from .auth import oauth2_scheme
 
 from ...core.config import settings
 from ...api.schemas.requests import RequestBody
 from ...api.schemas.responses import ResponseBody
@@ -18,21 +17,20 @@
 async def hello():
     return {"message": f'Hello {settings.required.instance}'}
 
 
 # todo try\exept
 @router.post("/api/v1/search", response_model=ResponseBody)
 async def get_search_data(request: RequestBody, token=Depends(oauth2_scheme)):
-    print(handlers.instances)
     if token != settings.token:
-        return HTTPException(status_code=503, )
+        return HTTPException(status_code=503, detail="Auth depends")
     # Получаем тип передаваемых данных
-    data_type = request.search.parameters[0].type
+    data_type = request.data_type
     # Значения, переданные для поиска
-    values: list = request.search.parameters[0].value
+    values: list = request.value
     # Смотрим, есть ли обработчик именно этого класса
     if (search_class := handlers.get(data_type)) is not None:
         try:
             # Создание экземляра Вашего класса и передача ему параметров
             searcher = handlers.get_instance(search_class)
             # Передаем результат в функцию подготовки ответа и возвращаем ResponseBody
             success, data = await searcher.execute_search(data_type, values)
```

### Comparing `fsapp-0.0.3/fsapp/api/schemas/responses.py` & `fsapp-1.0.3/fsapp/api/schemas/responses.py`

 * *Files identical despite different names*

### Comparing `fsapp-0.0.3/fsapp/base.py` & `fsapp-1.0.3/fsapp/base.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 from fastapi import FastAPI
 
 from fsapp.core.config import settings
 from fsapp.api.routers import api_router
 from fsapp.classes import BaseExecutor
 from fsapp.core.config import create_settings_files
-from fsapp.core.handlers import handlers
 
 create_settings_files()
 
 # Основной объект приложения
 # todo argument comments
 app = FastAPI(
-    # todo required -> main
     title=settings.required.instance,
-    # todo openapi_url -> ope_napi_url
     docs_url="/docs",
 )
 
+settings.token = None
 # Подключение всех эндпоинтов
 app.include_router(api_router)
 # Добавляем базовый класс обработчиков
 app.base_class = BaseExecutor
```

### Comparing `fsapp-0.0.3/fsapp/classes.py` & `fsapp-1.0.3/fsapp/classes.py`

 * *Files identical despite different names*

### Comparing `fsapp-0.0.3/fsapp/core/config.py` & `fsapp-1.0.3/fsapp/core/config.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,19 +2,17 @@
 import toml
 
 from dynaconf import Dynaconf
 from pathlib import Path
 
 SETTINGS = {
     "required": {
-        "instance": 'Default_Project',
-        "acces_token_expire_minutes": 1440
+        "instance": 'Default_Project'
     },
     "optional": {
-
     }
 }
 
 SECRETS = {
     "auth": {
         "username": "user",
         "password": "202cb962ac59075b964b07152d234b70",
```

### Comparing `fsapp-0.0.3/fsapp.egg-info/SOURCES.txt` & `fsapp-1.0.3/fsapp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fsapp-0.0.3/pyproject.toml` & `fsapp-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fsapp"
-version = "0.0.3"
+version = "1.0.3"
 authors = [
     { name = "Scrandi Coulson", email = "scrandi.coulson@ro.ru" },
 ]
 description = "Fastapi web-app"
 #readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

