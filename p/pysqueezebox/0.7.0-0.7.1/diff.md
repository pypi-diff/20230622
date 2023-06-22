# Comparing `tmp/pysqueezebox-0.7.0.tar.gz` & `tmp/pysqueezebox-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysqueezebox-0.7.0.tar", last modified: Fri May 26 18:37:32 2023, max compression
+gzip compressed data, was "pysqueezebox-0.7.1.tar", last modified: Thu Jun 22 20:41:10 2023, max compression
```

## Comparing `pysqueezebox-0.7.0.tar` & `pysqueezebox-0.7.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 rajlaud    (501) staff       (20)        0 2023-05-26 18:37:32.057189 pysqueezebox-0.7.0/
--rw-r--r--   0 rajlaud    (501) staff       (20)    11338 2023-05-25 20:54:54.000000 pysqueezebox-0.7.0/LICENSE
--rw-r--r--   0 rajlaud    (501) staff       (20)     2552 2023-05-26 18:37:32.057454 pysqueezebox-0.7.0/PKG-INFO
--rw-r--r--   0 rajlaud    (501) staff       (20)     2226 2023-05-25 20:54:54.000000 pysqueezebox-0.7.0/README.md
-drwxr-xr-x   0 rajlaud    (501) staff       (20)        0 2023-05-26 18:37:32.046707 pysqueezebox-0.7.0/pysqueezebox/
--rw-r--r--   0 rajlaud    (501) staff       (20)      981 2023-05-25 20:54:54.000000 pysqueezebox-0.7.0/pysqueezebox/__init__.py
--rw-r--r--   0 rajlaud    (501) staff       (20)      151 2023-05-25 20:54:54.000000 pysqueezebox-0.7.0/pysqueezebox/const.py
--rw-r--r--   0 rajlaud    (501) staff       (20)     3652 2023-05-25 20:54:54.000000 pysqueezebox-0.7.0/pysqueezebox/discovery.py
--rw-r--r--   0 rajlaud    (501) staff       (20)    23556 2023-05-26 15:26:42.000000 pysqueezebox-0.7.0/pysqueezebox/player.py
--rw-r--r--   0 rajlaud    (501) staff       (20)    13244 2023-05-26 15:27:06.000000 pysqueezebox-0.7.0/pysqueezebox/server.py
-drwxr-xr-x   0 rajlaud    (501) staff       (20)        0 2023-05-26 18:37:32.050874 pysqueezebox-0.7.0/pysqueezebox.egg-info/
--rw-r--r--   0 rajlaud    (501) staff       (20)     2552 2023-05-26 18:37:31.000000 pysqueezebox-0.7.0/pysqueezebox.egg-info/PKG-INFO
--rw-r--r--   0 rajlaud    (501) staff       (20)      462 2023-05-26 18:37:32.000000 pysqueezebox-0.7.0/pysqueezebox.egg-info/SOURCES.txt
--rw-r--r--   0 rajlaud    (501) staff       (20)        1 2023-05-26 18:37:31.000000 pysqueezebox-0.7.0/pysqueezebox.egg-info/dependency_links.txt
--rw-r--r--   0 rajlaud    (501) staff       (20)       22 2023-05-26 18:37:31.000000 pysqueezebox-0.7.0/pysqueezebox.egg-info/requires.txt
--rw-r--r--   0 rajlaud    (501) staff       (20)       19 2023-05-26 18:37:31.000000 pysqueezebox-0.7.0/pysqueezebox.egg-info/top_level.txt
--rw-r--r--   0 rajlaud    (501) staff       (20)      131 2023-05-26 18:37:32.058441 pysqueezebox-0.7.0/setup.cfg
--rw-r--r--   0 rajlaud    (501) staff       (20)      572 2023-05-26 18:34:14.000000 pysqueezebox-0.7.0/setup.py
-drwxr-xr-x   0 rajlaud    (501) staff       (20)        0 2023-05-26 18:37:32.056281 pysqueezebox-0.7.0/tests/
--rw-r--r--   0 rajlaud    (501) staff       (20)        0 2023-05-25 21:31:11.000000 pysqueezebox-0.7.0/tests/__init__.py
--rw-r--r--   0 rajlaud    (501) staff       (20)     1686 2023-05-26 18:32:29.000000 pysqueezebox-0.7.0/tests/conftest.py
--rw-r--r--   0 rajlaud    (501) staff       (20)     1693 2023-05-25 21:37:01.000000 pysqueezebox-0.7.0/tests/test_discovery.py
--rw-r--r--   0 rajlaud    (501) staff       (20)    18376 2023-05-26 18:32:50.000000 pysqueezebox-0.7.0/tests/test_integration.py
--rw-r--r--   0 rajlaud    (501) staff       (20)     1987 2023-05-25 20:54:54.000000 pysqueezebox-0.7.0/tests/test_player.py
--rw-r--r--   0 rajlaud    (501) staff       (20)     1639 2023-05-25 20:54:54.000000 pysqueezebox-0.7.0/tests/test_server.py
+drwxr-xr-x   0 rajlaud    (501) staff       (20)        0 2023-06-22 20:41:10.904865 pysqueezebox-0.7.1/
+-rw-r--r--   0 rajlaud    (501) staff       (20)    11338 2023-05-25 20:54:54.000000 pysqueezebox-0.7.1/LICENSE
+-rw-r--r--   0 rajlaud    (501) staff       (20)     2552 2023-06-22 20:41:10.905028 pysqueezebox-0.7.1/PKG-INFO
+-rw-r--r--   0 rajlaud    (501) staff       (20)     2226 2023-05-25 20:54:54.000000 pysqueezebox-0.7.1/README.md
+drwxr-xr-x   0 rajlaud    (501) staff       (20)        0 2023-06-22 20:41:10.899487 pysqueezebox-0.7.1/pysqueezebox/
+-rw-r--r--   0 rajlaud    (501) staff       (20)      981 2023-05-25 20:54:54.000000 pysqueezebox-0.7.1/pysqueezebox/__init__.py
+-rw-r--r--   0 rajlaud    (501) staff       (20)      151 2023-05-25 20:54:54.000000 pysqueezebox-0.7.1/pysqueezebox/const.py
+-rw-r--r--   0 rajlaud    (501) staff       (20)     3652 2023-05-25 20:54:54.000000 pysqueezebox-0.7.1/pysqueezebox/discovery.py
+-rw-r--r--   0 rajlaud    (501) staff       (20)    23569 2023-05-26 18:41:27.000000 pysqueezebox-0.7.1/pysqueezebox/player.py
+-rw-r--r--   0 rajlaud    (501) staff       (20)    13374 2023-06-22 19:03:47.000000 pysqueezebox-0.7.1/pysqueezebox/server.py
+drwxr-xr-x   0 rajlaud    (501) staff       (20)        0 2023-06-22 20:41:10.901842 pysqueezebox-0.7.1/pysqueezebox.egg-info/
+-rw-r--r--   0 rajlaud    (501) staff       (20)     2552 2023-06-22 20:41:10.000000 pysqueezebox-0.7.1/pysqueezebox.egg-info/PKG-INFO
+-rw-r--r--   0 rajlaud    (501) staff       (20)      462 2023-06-22 20:41:10.000000 pysqueezebox-0.7.1/pysqueezebox.egg-info/SOURCES.txt
+-rw-r--r--   0 rajlaud    (501) staff       (20)        1 2023-06-22 20:41:10.000000 pysqueezebox-0.7.1/pysqueezebox.egg-info/dependency_links.txt
+-rw-r--r--   0 rajlaud    (501) staff       (20)       22 2023-06-22 20:41:10.000000 pysqueezebox-0.7.1/pysqueezebox.egg-info/requires.txt
+-rw-r--r--   0 rajlaud    (501) staff       (20)       19 2023-06-22 20:41:10.000000 pysqueezebox-0.7.1/pysqueezebox.egg-info/top_level.txt
+-rw-r--r--   0 rajlaud    (501) staff       (20)      131 2023-06-22 20:41:10.905580 pysqueezebox-0.7.1/setup.cfg
+-rw-r--r--   0 rajlaud    (501) staff       (20)      572 2023-06-22 19:06:48.000000 pysqueezebox-0.7.1/setup.py
+drwxr-xr-x   0 rajlaud    (501) staff       (20)        0 2023-06-22 20:41:10.904483 pysqueezebox-0.7.1/tests/
+-rw-r--r--   0 rajlaud    (501) staff       (20)        0 2023-05-25 21:31:11.000000 pysqueezebox-0.7.1/tests/__init__.py
+-rw-r--r--   0 rajlaud    (501) staff       (20)     1686 2023-05-26 18:41:37.000000 pysqueezebox-0.7.1/tests/conftest.py
+-rw-r--r--   0 rajlaud    (501) staff       (20)     1693 2023-05-25 21:37:01.000000 pysqueezebox-0.7.1/tests/test_discovery.py
+-rw-r--r--   0 rajlaud    (501) staff       (20)    18376 2023-05-26 18:41:37.000000 pysqueezebox-0.7.1/tests/test_integration.py
+-rw-r--r--   0 rajlaud    (501) staff       (20)     2003 2023-06-22 19:03:47.000000 pysqueezebox-0.7.1/tests/test_player.py
+-rw-r--r--   0 rajlaud    (501) staff       (20)     1639 2023-05-25 20:54:54.000000 pysqueezebox-0.7.1/tests/test_server.py
```

### Comparing `pysqueezebox-0.7.0/LICENSE` & `pysqueezebox-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pysqueezebox-0.7.0/PKG-INFO` & `pysqueezebox-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysqueezebox
-Version: 0.7.0
+Version: 0.7.1
 Summary: Asynchronous library to control Logitech Media Server
 Home-page: https://github.com/rajlaud/pysqueezebox
 Author: Raj Laud
 Author-email: raj.laud@gmail.com
 License: apache-2.0
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `pysqueezebox-0.7.0/README.md` & `pysqueezebox-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `pysqueezebox-0.7.0/pysqueezebox/__init__.py` & `pysqueezebox-0.7.1/pysqueezebox/__init__.py`

 * *Files identical despite different names*

### Comparing `pysqueezebox-0.7.0/pysqueezebox/discovery.py` & `pysqueezebox-0.7.1/pysqueezebox/discovery.py`

 * *Files identical despite different names*

### Comparing `pysqueezebox-0.7.0/pysqueezebox/player.py` & `pysqueezebox-0.7.1/pysqueezebox/player.py`

 * *Files 0% similar despite different names*

```diff
@@ -365,27 +365,27 @@
                 self._playlist_timestamp = response["playlist_timestamp"]
                 self._playlist_tags = set(tags)
                 # poll server again for full playlist, which has either changed
                 # or about which we are seeking new tags
                 response = await self.async_query(
                     "status", "0", response["playlist_tracks"], f"tags:{tags}"
                 )
+
+                if response is False:
+                    _LOGGER.debug("Error updating status - unable to retrieve playlist")
+                    return False
             else:
                 response.pop("playlist_loop", None)
         else:
             # no current playlist
             self._status.update({"playlist_loop": None})
 
         # preserve the playlist between updates
         self._status = {"playlist_loop": self._status.get("playlist_loop")}
-        try:
-            self._status.update(response)
-        except TypeError:
-            _LOGGER.debug("Error updating status - empty response from server")
-            return False
+        self._status.update(response)
 
         # check if any property futures have been satisfied
         property_futures = []
         interval = None
         for property_future in self._property_futures:
             if not property_future["future"].done():
                 if property_future["test"](getattr(self, property_future["prop"])):
```

### Comparing `pysqueezebox-0.7.0/pysqueezebox/server.py` & `pysqueezebox-0.7.1/pysqueezebox/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -341,12 +341,15 @@
         """Generate an image url using a track id."""
         return self.generate_image_url(f"/music/{track_id}/cover.jpg")
 
     def generate_image_url(self, image_url):
         """Add the appropriate base_url to a relative image_url."""
         base_url = f"{self._prefix}://"
         if self._username:
-            base_url += f"{self._username}:{self._password}@"
+            base_url += urllib.parse.quote(self._username, safe="")
+            base_url += ":"
+            base_url += urllib.parse.quote(self._password, safe="")
+            base_url += "@"
 
         base_url += f"{self.host}:{self.port}/"
 
         return urllib.parse.urljoin(base_url, image_url)
```

### Comparing `pysqueezebox-0.7.0/pysqueezebox.egg-info/PKG-INFO` & `pysqueezebox-0.7.1/pysqueezebox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysqueezebox
-Version: 0.7.0
+Version: 0.7.1
 Summary: Asynchronous library to control Logitech Media Server
 Home-page: https://github.com/rajlaud/pysqueezebox
 Author: Raj Laud
 Author-email: raj.laud@gmail.com
 License: apache-2.0
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `pysqueezebox-0.7.0/setup.py` & `pysqueezebox-0.7.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pysqueezebox",
-    version="0.7.0",
+    version="0.7.1",
     license="apache-2.0",
     author="Raj Laud",
     author_email="raj.laud@gmail.com",
     description="Asynchronous library to control Logitech Media Server",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/rajlaud/pysqueezebox",
```

### Comparing `pysqueezebox-0.7.0/tests/conftest.py` & `pysqueezebox-0.7.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pysqueezebox-0.7.0/tests/test_discovery.py` & `pysqueezebox-0.7.1/tests/test_discovery.py`

 * *Files identical despite different names*

### Comparing `pysqueezebox-0.7.0/tests/test_integration.py` & `pysqueezebox-0.7.1/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `pysqueezebox-0.7.0/tests/test_player.py` & `pysqueezebox-0.7.1/tests/test_player.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,19 +19,19 @@
     # pylint: disable=eval-used
     test_player2 = eval(repr(test_player))
     assert repr(test_player) == repr(test_player2)
 
 
 async def test_image_url():
     """Test creating image urls."""
-    lms = Server(None, "192.168.1.1", username="test", password="password")
+    lms = Server(None, "192.168.1.1", username="test#", password="~/.$password")
     player = Player(lms, "00:11:22:33:44:55", "Test Player")
     assert (
         player.image_url
-        == "http://test:password@192.168.1.1:9000/music/unknown/cover.jpg"
+        == "http://test%23:~%2F.%24password@192.168.1.1:9000/music/unknown/cover.jpg"
     )
 
 
 async def test_wait():
     """Test player._wait_for_property()."""
     with patch.object(Player, "async_update", AsyncMock()):
         mock_player = Player(None, "00:11:22:33:44:55", "Test Player")
```

### Comparing `pysqueezebox-0.7.0/tests/test_server.py` & `pysqueezebox-0.7.1/tests/test_server.py`

 * *Files identical despite different names*

