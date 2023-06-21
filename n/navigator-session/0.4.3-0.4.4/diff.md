# Comparing `tmp/navigator_session-0.4.3-py3-none-any.whl.zip` & `tmp/navigator_session-0.4.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 17580 bytes, number of entries: 15
--rw-r--r--  2.0 unx     3038 b- defN 23-Apr-17 17:00 navigator_session/__init__.py
--rw-r--r--  2.0 unx     1466 b- defN 23-Apr-17 17:00 navigator_session/conf.py
--rw-r--r--  2.0 unx     5812 b- defN 23-Apr-17 17:00 navigator_session/data.py
--rw-r--r--  2.0 unx     1954 b- defN 23-Apr-17 17:00 navigator_session/middleware.py
--rw-r--r--  2.0 unx     2186 b- defN 23-Apr-17 17:00 navigator_session/session.py
--rw-r--r--  2.0 unx      394 b- defN 23-Apr-17 17:00 navigator_session/version.py
--rw-r--r--  2.0 unx      132 b- defN 23-Apr-17 17:00 navigator_session/storages/__init__.py
--rw-r--r--  2.0 unx     6069 b- defN 23-Apr-17 17:00 navigator_session/storages/abstract.py
--rw-r--r--  2.0 unx     2463 b- defN 23-Apr-17 17:00 navigator_session/storages/cookie.py
--rw-r--r--  2.0 unx     9242 b- defN 23-Apr-17 17:00 navigator_session/storages/redis.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Apr-17 17:01 navigator_session-0.4.3.dist-info/LICENSE
--rw-r--r--  2.0 unx     2372 b- defN 23-Apr-17 17:01 navigator_session-0.4.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-17 17:01 navigator_session-0.4.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       18 b- defN 23-Apr-17 17:01 navigator_session-0.4.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1318 b- defN 23-Apr-17 17:01 navigator_session-0.4.3.dist-info/RECORD
-15 files, 47913 bytes uncompressed, 15374 bytes compressed:  67.9%
+Zip file size: 17600 bytes, number of entries: 15
+-rw-r--r--  2.0 unx     3038 b- defN 23-Jun-21 23:56 navigator_session/__init__.py
+-rw-r--r--  2.0 unx     1466 b- defN 23-Jun-21 23:56 navigator_session/conf.py
+-rw-r--r--  2.0 unx     5815 b- defN 23-Jun-21 23:56 navigator_session/data.py
+-rw-r--r--  2.0 unx     1959 b- defN 23-Jun-21 23:56 navigator_session/middleware.py
+-rw-r--r--  2.0 unx     2188 b- defN 23-Jun-21 23:56 navigator_session/session.py
+-rw-r--r--  2.0 unx      394 b- defN 23-Jun-21 23:56 navigator_session/version.py
+-rw-r--r--  2.0 unx      132 b- defN 23-Jun-21 23:56 navigator_session/storages/__init__.py
+-rw-r--r--  2.0 unx     6074 b- defN 23-Jun-21 23:56 navigator_session/storages/abstract.py
+-rw-r--r--  2.0 unx     2468 b- defN 23-Jun-21 23:56 navigator_session/storages/cookie.py
+-rw-r--r--  2.0 unx     9361 b- defN 23-Jun-21 23:56 navigator_session/storages/redis.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Jun-21 23:57 navigator_session-0.4.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2403 b- defN 23-Jun-21 23:57 navigator_session-0.4.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-21 23:57 navigator_session-0.4.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       18 b- defN 23-Jun-21 23:57 navigator_session-0.4.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1318 b- defN 23-Jun-21 23:57 navigator_session-0.4.4.dist-info/RECORD
+15 files, 48083 bytes uncompressed, 15394 bytes compressed:  68.0%
```

## zipnote {}

```diff
@@ -24,23 +24,23 @@
 
 Filename: navigator_session/storages/cookie.py
 Comment: 
 
 Filename: navigator_session/storages/redis.py
 Comment: 
 
-Filename: navigator_session-0.4.3.dist-info/LICENSE
+Filename: navigator_session-0.4.4.dist-info/LICENSE
 Comment: 
 
-Filename: navigator_session-0.4.3.dist-info/METADATA
+Filename: navigator_session-0.4.4.dist-info/METADATA
 Comment: 
 
-Filename: navigator_session-0.4.3.dist-info/WHEEL
+Filename: navigator_session-0.4.4.dist-info/WHEEL
 Comment: 
 
-Filename: navigator_session-0.4.3.dist-info/top_level.txt
+Filename: navigator_session-0.4.4.dist-info/top_level.txt
 Comment: 
 
-Filename: navigator_session-0.4.3.dist-info/RECORD
+Filename: navigator_session-0.4.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## navigator_session/data.py

```diff
@@ -50,18 +50,18 @@
         self._data = {}
         self._identity = data.get(SESSION_KEY, None) if data else identity
         if not self._identity:
             self._identity = uuid.uuid4().hex
         self._new = new if data != {} else True
         self._max_age = max_age if max_age else None
         created = data.get('created', None) if data else None
-        self._now = pendulum.now('UTC') # time for this instance creation
+        self._now = pendulum.now('UTC')  # time for this instance creation
         self.__created__ = self._now
         now = int(self._now.int_timestamp)
-        self._now = now # time for this instance creation
+        self._now = now  # time for this instance creation
         age = now - created if created else now
         if max_age is not None and age > max_age:
             data = None
         if self._new or created is None:
             self._created = now
         else:
             self._created = created
@@ -71,15 +71,15 @@
         # Other mark timestamp for this session:
         dt = pendulum.now('UTC')
         self._dow = dt.day_of_week
         self._time = dt.time()
         self.args = args
 
     def __repr__(self) -> str:
-        return '<{} [new:{}, created:{}] {!r}>'.format( # pylint: disable=C0209
+        return '<{} [new:{}, created:{}] {!r}>'.format(  # pylint: disable=C0209
             'NAV-Session ', self.new, self.created, self._data
         )
 
     @property
     def new(self) -> bool:
         return self._new
```

## navigator_session/middleware.py

```diff
@@ -10,22 +10,22 @@
 from .storages.abstract import AbstractStorage
 from .data import SessionData
 
 Middleware = Callable[[web.Request, Handler], Awaitable[web.StreamResponse]]
 
 ### Basic Middleware for Session System
 def session_middleware(
-        app: web.Application, # pylint: disable=W0613
+        app: web.Application,  # pylint: disable=W0613
         storage: AbstractStorage
 ) -> Middleware:
     """Middleware to attach Session Storage to every Request."""
     if not isinstance(storage, AbstractStorage):
         raise RuntimeError(
             f"Expected an AbstractStorage got {storage!s}"
-    )
+        )
 
     @web.middleware
     async def middleware(
             request: web.Request,
             handler: Handler
     ) -> web.StreamResponse:
```

## navigator_session/session.py

```diff
@@ -4,28 +4,28 @@
 from .storages.redis import RedisStorage
 from .middleware import session_middleware
 
 class SessionHandler:
     """Authentication Backend for Navigator."""
     storage: Callable = None
 
-    def __init__(self,storage: str = 'redis', **kwargs) -> None:
+    def __init__(self, storage: str = 'redis', **kwargs) -> None:
         # TODO: Session Support with parametrization (other storages):
         if storage == 'redis':
             self.storage = RedisStorage(**kwargs)
         else:
             raise NotImplementedError(
                 f"Cannot load a Session Storage {storage}"
             )
 
     def setup(self, app: web.Application) -> None:
         if isinstance(app, web.Application):
-            self.app = app # register the app into the Extension
+            self.app = app  # register the app into the Extension
         else:
-            self.app = app.get_app() # Nav Application
+            self.app = app.get_app()  # Nav Application
         ## Configure the Middleware for NAV Session.
         self.app.middlewares.append(
             session_middleware(app, self.storage)
         )
         # startup operations over extension backend
         self.app.on_startup.append(
             self.session_startup
@@ -34,15 +34,14 @@
         self.app.on_cleanup.append(
             self.session_cleanup
         )
         logging.debug(':::: Session Handler Loaded ::::')
         # register the Auth extension into the app
         self.app['nav_session'] = self
 
-
     async def session_startup(self, app: web.Application):
         """
         Calling Session (and Storage) Startup.
         """
         try:
             await self.storage.on_startup(app)
         except Exception as ex:
```

## navigator_session/version.py

```diff
@@ -1,11 +1,11 @@
 """Navigator Session Meta information.
    Navigator Session allows us to store user-specific data into session object.
 """
 
 __title__ = 'navigator_session'
 __description__ = ('Navigator Session allows us to store user-specific data '
                    'into session object.')
-__version__ = '0.4.3'
+__version__ = '0.4.4'
 __author__ = 'Jesus Lara'
 __author_email__ = 'jesuslarag@gmail.com'
 __license__ = 'Apache-2.0'
```

## navigator_session/storages/abstract.py

```diff
@@ -39,15 +39,15 @@
             max_age: int = None,
             secure: bool = True,
             domain: Optional[str] = None,
             path: str = "/",
             httponly: bool = True,
             samesite: Optional[str] = 'Lax',
             **kwargs
-        ) -> None:
+    ) -> None:
         if not max_age:
             self.max_age = SESSION_TIMEOUT
         else:
             self.max_age = max_age
         if 'use_cookie' in kwargs:
             self.use_cookie = kwargs['use_cookie']
             del kwargs['use_cookie']
@@ -101,15 +101,16 @@
     async def get_session(self, request: web.Request) -> SessionData:
         pass
 
     def empty_session(self) -> SessionData:
         return SessionData(None, data=None, new=True, max_age=self.max_age)
 
     @abc.abstractmethod
-    async def save_session(self,
+    async def save_session(
+        self,
         request: web.Request,
         response: web.StreamResponse,
         session: SessionData
     ) -> None:
         pass
 
     @abc.abstractmethod
@@ -124,15 +125,15 @@
         """Delete a User Session."""
         session = await self.get_session(request)
         await self.invalidate(request, session)
         request["session"] = None
         try:
             del request[SESSION_KEY]
             del request[SESSION_OBJECT]
-        except Exception as err: # pylint: disable=W0703
+        except Exception as err:  # pylint: disable=W0703
             logging.warning(
                 f'Session: Error on Forgot Method: {err}'
             )
         if response is not None:
             # also, forgot the secure Cookie:
             self.forgot_cooke(response)
 
@@ -176,15 +177,14 @@
             if not cookie_data:
                 response.del_cookie(
                     self.__name__, domain=self._domain, path=self._path
                 )
             else:
                 response.set_cookie(self.__name__, cookie_data, **params)
 
-
     def session_info(self, session: SessionData, request: web.Request) -> SessionData:
         """session_info.
             Session Helper for adding more information extracted from Request.
         Args:
             session (SessionData): Session Object.
             request (web.Request): aiohttp Web Request.
```

## navigator_session/storages/cookie.py

```diff
@@ -20,15 +20,15 @@
             http_only: bool = True,
             max_age: int = None,
             secure: bool = None,
             domain: Optional[str] = None,
             path: str = "/",
             secret_key: Union[str, bytes, bytearray, fernet.Fernet] = None,
             **kwargs
-        ) -> None:
+    ) -> None:
         super(
             CookieStorage, self
         ).__init__(
             max_age=max_age,
             secure=secure,
             domain=domain,
             path=path,
@@ -71,15 +71,16 @@
         ignore_cookie: bool = True
     ) -> SessionData:
         pass
 
     async def get_session(self, request: web.Request) -> SessionData:
         pass
 
-    async def save_session(self,
+    async def save_session(
+        self,
         request: web.Request,
         response: web.StreamResponse,
         session: SessionData
     ) -> None:
         pass
 
     async def invalidate(
```

## navigator_session/storages/redis.py

```diff
@@ -1,14 +1,14 @@
 """Using Redis for Saving Session Storage."""
 import time
 import logging
 from typing import Optional
 from collections.abc import Callable
 from aiohttp import web
-import aioredis
+from redis import asyncio as aioredis
 from navigator_session.conf import (
     SESSION_URL,
     SESSION_KEY,
     SESSION_OBJECT,
     SESSION_STORAGE
 )
 from .abstract import AbstractStorage, SessionData
@@ -20,15 +20,15 @@
             self,
             *,
             max_age: int = None,
             secure: bool = None,
             domain: Optional[str] = None,
             path: str = "/",
             **kwargs
-        ) -> None:
+    ) -> None:
         self._redis: Callable = None
         super(
             RedisStorage, self
         ).__init__(
             max_age=max_age,
             secure=secure,
             domain=domain,
@@ -39,28 +39,32 @@
     async def on_startup(self, app: web.Application):
         try:
             self._redis = aioredis.ConnectionPool.from_url(
                 SESSION_URL,
                 decode_responses=True,
                 encoding='utf-8'
             )
-        except Exception as err: # pylint: disable=W0703
+        except Exception as err:  # pylint: disable=W0703
             logging.exception(err, stack_info=True)
             return False
 
     async def on_cleanup(self, app: web.Application):
         try:
-            await self._redis.disconnect(inuse_connections = True)
-        except Exception as ex: # pylint: disable=W0703
+            await self._redis.disconnect(inuse_connections=True)
+        except Exception as ex:  # pylint: disable=W0703
             logging.warning(ex)
 
-    async def get_session(self, request: web.Request, userdata: dict = None) -> SessionData:
+    async def get_session(
+        self,
+        request: web.Request,
+        userdata: dict = None
+    ) -> SessionData:
         try:
             session = request.get(SESSION_OBJECT)
-        except Exception as err: # pylint: disable=W0703
+        except Exception as err:  # pylint: disable=W0703
             logging.debug(f'Redis Storage: Error on get Session: {err!s}')
             session = None
         if session is None:
             storage = request.get(SESSION_STORAGE)
             if storage is None:
                 raise RuntimeError(
                     "Missing Configuration for Session Middleware."
@@ -79,16 +83,16 @@
                 data = await conn.get(session_id)
             if data is None:
                 # nothing to forgot
                 return True
         try:
             # delete the ID of the session
             await conn.delete(session.identity)
-            session.invalidate() # invalidate this session object
-        except Exception as err: # pylint: disable=W0703
+            session.invalidate()  # invalidate this session object
+        except Exception as err:  # pylint: disable=W0703
             logging.error(err)
             return False
         return True
 
     async def load_session(
         self,
         request: web.Request,
@@ -104,15 +108,15 @@
         doesnt exists.
 
         ---
         new: if False, new session is not created.
         """
         # TODO: first: for security, check if cookie csrf_secure exists
         session_id = None
-        if ignore_cookie is False and  self.use_cookie is True:
+        if ignore_cookie is False and self.use_cookie is True:
             cookie = self.load_cookie(request)
             try:
                 session_id = cookie['session_id']
             except (TypeError, KeyError):
                 session_id = None
         # if not, session is missed, expired, bad session, etc
         try:
@@ -131,15 +135,15 @@
             # TODO: getting from cookie
         if session_id is None and new is False:
             return False
         # we need to load session data from redis
         logging.debug(f':::::: LOAD SESSION FOR {session_id} ::::: ')
         try:
             data = await conn.get(session_id)
-        except Exception as err: # pylint: disable=W0703
+        except Exception as err:  # pylint: disable=W0703
             logging.error(
                 f'Redis Storage: Error Getting Session data: {err!s}'
             )
             data = None
         if data is None:
             if new is True:
                 # create a new session if not exists:
@@ -150,15 +154,15 @@
             data = self._decoder(data)
             session = SessionData(
                 identity=session_id,
                 data=data,
                 new=False,
                 max_age=self.max_age
             )
-        except Exception as err: # pylint: disable=W0703
+        except Exception as err:  # pylint: disable=W0703
             logging.warning(err)
             session = SessionData(
                 identity=None,
                 data=None,
                 new=True,
                 max_age=self.max_age
             )
@@ -172,15 +176,16 @@
             cookie_data = {
                 "session_id": session_id
             }
             cookie_data = self._encoder(cookie_data)
             self.save_cookie(response, cookie_data=cookie_data, max_age=self.max_age)
         return session
 
-    async def save_session(self,
+    async def save_session(
+        self,
         request: web.Request,
         response: web.StreamResponse,
         session: SessionData
     ) -> None:
         """Save the whole session in the backend Storage."""
         session_id = session.identity
         if not session_id:
@@ -194,15 +199,15 @@
         expire = max_age if max_age is not None else 0
         # TODO: add expiration on redis to value
         try:
             conn = aioredis.Redis(connection_pool=self._redis)
             result = await conn.set(
                 session_id, data, expire
             )
-        except Exception as err: # pylint: disable=W0703
+        except Exception as err:  # pylint: disable=W0703
             print('Error Saving Session: ', err)
             logging.exception(err, stack_info=True)
             return False
 
     async def new_session(
         self,
         request: web.Request,
@@ -228,15 +233,15 @@
             data["last_visited"] = f"Last visited: {t!s}"
             data[SESSION_KEY] = session_id
             dt = self._encoder(data)
             result = await conn.set(
                 session_id, dt, self.max_age
             )
             logging.info(f'Creation of New Session: {result}')
-        except Exception as err: # pylint: disable=W0703
+        except Exception as err:  # pylint: disable=W0703
             logging.exception(err)
             return False
         try:
             session = SessionData(
                 identity=session_id,
                 data=data,
                 new=True,
@@ -244,17 +249,20 @@
             )
             if self.use_cookie is True and response is not None:
                 cookie_data = {
                     "last_visit": t,
                     "session_id": session_id
                 }
                 cookie_data = self._encoder(cookie_data)
-                self.save_cookie(response, cookie_data=cookie_data, max_age=self.max_age)
-        except Exception as err: # pylint: disable=W0703
-            print(err)
+                self.save_cookie(
+                    response,
+                    cookie_data=cookie_data,
+                    max_age=self.max_age
+                )
+        except Exception as err:  # pylint: disable=W0703
             logging.exception(f'Error creating Session Data: {err!s}')
         # Saving Session Object:
         ## add other options to session:
         self.session_info(session, request)
         session[SESSION_KEY] = session_id
         request[SESSION_OBJECT] = session
         request[SESSION_KEY] = session_id
```

## Comparing `navigator_session-0.4.3.dist-info/LICENSE` & `navigator_session-0.4.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `navigator_session-0.4.3.dist-info/METADATA` & `navigator_session-0.4.4.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: navigator-session
-Version: 0.4.3
+Version: 0.4.4
 Summary: Navigator Session allows us to store user-specific data into session object.
 Home-page: https://github.com/phenobarbital/navigator-session
 Author: Jesus Lara
 Author-email: jesuslarag@gmail.com
 License: Apache-2.0
 Project-URL: Source, https://github.com/phenobarbital/navigator-session
 Project-URL: Funding, https://paypal.me/phenobarbital
@@ -29,14 +29,15 @@
 Requires-Dist: PyNaCl (==1.5.0)
 Requires-Dist: aiohttp (==3.8.4)
 Requires-Dist: uvloop (==0.17.0)
 Requires-Dist: asyncio (==3.4.3)
 Requires-Dist: navconfig[default] (>=1.0.15)
 Requires-Dist: jsonpickle (==3.0.1)
 Requires-Dist: aioredis (==2.0.1)
+Requires-Dist: redis (==4.5.5)
 Requires-Dist: pendulum (==2.1.2)
 Requires-Dist: python-datamodel (>=0.2.1)
 
 # Navigator_Session #
 
 Navigator_Session Allows us to store User-based data into a session Object, this session object exposes an dict-like interface and uses cookies or redis as persistent backend.
```

## Comparing `navigator_session-0.4.3.dist-info/RECORD` & `navigator_session-0.4.4.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 navigator_session/__init__.py,sha256=xsmc90K04EgQEtYidPN7bsXn0WIqw6GucNwy138Mmno,3038
 navigator_session/conf.py,sha256=PwCGoYpg_2MEq5_zObvbx4yXKf7AIKObO-lzTh2AvxM,1466
-navigator_session/data.py,sha256=CwvOqi0ZfJU4wsppMQ-m-he0PEgim3xdhBhTEYgPucs,5812
-navigator_session/middleware.py,sha256=EE2efxSzcCmh13tDu7_-qGROk6xlD174Fo3j3vCVcx4,1954
-navigator_session/session.py,sha256=k0RuyWix41rmlcTsSHRg5ZDxsU20n4igrRYCwTT6L8M,2186
-navigator_session/version.py,sha256=D8Lt03n0mQ6PxA0E4eMd8aYOcZoWkG0PRzqz5r2JxHw,394
+navigator_session/data.py,sha256=9XEaLDRIs3qrIVmeouN2Tx_mTPa2QbLZlB6s4ewelG8,5815
+navigator_session/middleware.py,sha256=kbTFWwY-NrFE-yen7DyOEyWjy8Pfol-5qiXCnm0vGa8,1959
+navigator_session/session.py,sha256=I6qWkMbqIpVX1RjxmccGsk1sCcqWZ_ZBVGwLXjV8wjw,2188
+navigator_session/version.py,sha256=0dtA2J4VlV6Gd58dmBTMcc3e3RWakzapNI5wVw6Gxg0,394
 navigator_session/storages/__init__.py,sha256=ln0Xli0lppUopDMrvQGt69BFtUAe1Grmy2DGkEpANNU,132
-navigator_session/storages/abstract.py,sha256=ceVOCPV7SOEfTq5iKFdjvP9139qQBvvXPFwJsXc9Nis,6069
-navigator_session/storages/cookie.py,sha256=2jmpC4asep_qPH-Lte2aGXLEHi2v4P1U5dpkziP0foY,2463
-navigator_session/storages/redis.py,sha256=CUa05CmMJDLV5lsGqvySrReqUcUD-ylJkuSV2rU838Y,9242
-navigator_session-0.4.3.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-navigator_session-0.4.3.dist-info/METADATA,sha256=c_9CBvtXkqWAxwpt8672etLbF3z0hrLulf__gs2BiA4,2372
-navigator_session-0.4.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-navigator_session-0.4.3.dist-info/top_level.txt,sha256=ZpOEy3wLKGsxG2rc0nHqcqJCV3HIOG_XCfE6mtsYYYY,18
-navigator_session-0.4.3.dist-info/RECORD,,
+navigator_session/storages/abstract.py,sha256=mgtCvUD5KKlkWa-xOUBAoZbtZyPG_R7MbxIDOKGANYU,6074
+navigator_session/storages/cookie.py,sha256=_qL5kIGbT4rtCMze4yj1h4J7Zauz_e7HnorPnFbi90w,2468
+navigator_session/storages/redis.py,sha256=XSNEJ_xuyM-8y6xrraDyF6w_BT_JR4eGyclfa8ZvODo,9361
+navigator_session-0.4.4.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+navigator_session-0.4.4.dist-info/METADATA,sha256=3oDu055agOp9EhWoDzUDwd-x5nl7q593MTs7dwNvCz8,2403
+navigator_session-0.4.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+navigator_session-0.4.4.dist-info/top_level.txt,sha256=ZpOEy3wLKGsxG2rc0nHqcqJCV3HIOG_XCfE6mtsYYYY,18
+navigator_session-0.4.4.dist-info/RECORD,,
```

