# Comparing `tmp/geovisio_cli-0.2.0.tar.gz` & `tmp/geovisio_cli-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geovisio_cli-0.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "geovisio_cli-0.2.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `geovisio_cli-0.2.0.tar` & `geovisio_cli-0.2.1.tar`

### file list

```diff
@@ -1,34 +1,35 @@
--rw-r--r--   0        0        0       47 2023-03-24 13:15:13.689899 geovisio_cli-0.2.0/.gitignore
--rw-r--r--   0        0        0     1371 2023-05-22 08:59:23.607560 geovisio_cli-0.2.0/.gitlab-ci.yml
--rw-r--r--   0        0        0     3132 2023-05-24 13:20:49.654423 geovisio_cli-0.2.0/CHANGELOG.md
--rw-r--r--   0        0        0     5468 2023-03-24 13:15:13.689899 geovisio_cli-0.2.0/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1070 2023-03-14 15:26:20.137987 geovisio_cli-0.2.0/LICENSE
--rw-r--r--   0        0        0      590 2023-05-24 13:17:27.558420 geovisio_cli-0.2.0/Makefile
--rw-r--r--   0        0        0     7516 2023-05-24 13:17:27.558420 geovisio_cli-0.2.0/README.md
--rw-r--r--   0        0        0     2792 2023-05-24 13:17:27.558420 geovisio_cli-0.2.0/USAGE.md
--rw-r--r--   0        0        0       53 2023-05-24 13:20:49.654423 geovisio_cli-0.2.0/geovisio_cli/__init__.py
--rw-r--r--   0        0        0     6173 2023-05-24 13:17:27.558420 geovisio_cli-0.2.0/geovisio_cli/auth.py
--rw-r--r--   0        0        0      284 2023-04-14 11:12:54.559203 geovisio_cli-0.2.0/geovisio_cli/exception.py
--rw-r--r--   0        0        0     5455 2023-05-24 13:17:27.558420 geovisio_cli-0.2.0/geovisio_cli/main.py
--rw-r--r--   0        0        0      136 2023-05-24 13:17:27.558420 geovisio_cli-0.2.0/geovisio_cli/model.py
--rw-r--r--   0        0        0    18222 2023-05-24 13:17:27.558420 geovisio_cli-0.2.0/geovisio_cli/sequence.py
--rw-r--r--   0        0        0     1457 2023-05-24 13:17:27.558420 geovisio_cli-0.2.0/geovisio_cli/utils.py
--rw-r--r--   0        0        0      971 2023-05-24 13:17:27.558420 geovisio_cli-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-14 15:26:20.137987 geovisio_cli-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0      191 2023-03-14 15:26:20.137987 geovisio_cli-0.2.0/tests/conftest.py
--rw-r--r--   0        0        0   523332 2023-03-14 15:26:20.137987 geovisio_cli-0.2.0/tests/fixtures/e1.jpg
--rw-r--r--   0        0        0   483454 2023-03-14 15:26:20.141986 geovisio_cli-0.2.0/tests/fixtures/e2.jpg
--rw-r--r--   0        0        0   529344 2023-03-14 15:26:20.141986 geovisio_cli-0.2.0/tests/fixtures/e3.jpg
--rw-r--r--   0        0        0       16 2023-03-14 15:26:20.141986 geovisio_cli-0.2.0/tests/fixtures/invalid_pic.jpg
--rw-r--r--   0        0        0       27 2023-03-14 15:26:20.141986 geovisio_cli-0.2.0/tests/fixtures/not_a_pic.md
--rw-r--r--   0        0        0        0 2023-03-14 15:26:20.141986 geovisio_cli-0.2.0/tests/integration/__init__.py
--rw-r--r--   0        0        0     3327 2023-05-24 13:17:27.558420 geovisio_cli-0.2.0/tests/integration/conftest.py
--rw-r--r--   0        0        0     2189 2023-05-22 08:59:23.607560 geovisio_cli-0.2.0/tests/integration/docker-compose-geovisio.yml
--rw-r--r--   0        0        0      584 2023-05-22 08:59:23.607560 geovisio_cli-0.2.0/tests/integration/docker-compose-gitlab-override.yml
--rw-r--r--   0        0        0    76457 2023-05-22 08:59:23.611560 geovisio_cli-0.2.0/tests/integration/keycloak-realm.json
--rw-r--r--   0        0        0     3222 2023-05-24 13:17:27.558420 geovisio_cli-0.2.0/tests/integration/test_auth.py
--rw-r--r--   0        0        0      369 2023-05-24 13:17:27.558420 geovisio_cli-0.2.0/tests/integration/test_status.py
--rw-r--r--   0        0        0     8178 2023-05-24 13:17:27.558420 geovisio_cli-0.2.0/tests/integration/test_upload.py
--rw-r--r--   0        0        0      583 2023-05-10 11:47:16.328656 geovisio_cli-0.2.0/tests/test_process.py
--rw-r--r--   0        0        0     2579 2023-05-15 17:51:20.171581 geovisio_cli-0.2.0/tests/test_sequence.py
--rw-r--r--   0        0        0     8491 1970-01-01 00:00:00.000000 geovisio_cli-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       47 2023-03-24 13:15:13.689899 geovisio_cli-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1413 2023-06-22 09:18:10.500879 geovisio_cli-0.2.1/.gitlab-ci.yml
+-rw-r--r--   0        0        0     3716 2023-06-22 10:32:13.532461 geovisio_cli-0.2.1/CHANGELOG.md
+-rw-r--r--   0        0        0     5468 2023-03-24 13:15:13.689899 geovisio_cli-0.2.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1070 2023-03-14 15:26:20.137987 geovisio_cli-0.2.1/LICENSE
+-rw-r--r--   0        0        0      590 2023-05-24 13:17:27.558420 geovisio_cli-0.2.1/Makefile
+-rw-r--r--   0        0        0     7516 2023-05-24 13:17:27.558420 geovisio_cli-0.2.1/README.md
+-rw-r--r--   0        0        0     3250 2023-06-22 09:18:10.500879 geovisio_cli-0.2.1/USAGE.md
+-rw-r--r--   0        0        0       53 2023-06-22 10:32:13.532461 geovisio_cli-0.2.1/geovisio_cli/__init__.py
+-rw-r--r--   0        0        0     6173 2023-05-24 13:17:27.558420 geovisio_cli-0.2.1/geovisio_cli/auth.py
+-rw-r--r--   0        0        0      284 2023-04-14 11:12:54.559203 geovisio_cli-0.2.1/geovisio_cli/exception.py
+-rw-r--r--   0        0        0     6180 2023-06-22 09:18:10.500879 geovisio_cli-0.2.1/geovisio_cli/main.py
+-rw-r--r--   0        0        0      136 2023-05-24 13:17:27.558420 geovisio_cli-0.2.1/geovisio_cli/model.py
+-rw-r--r--   0        0        0    21407 2023-06-20 08:50:48.042695 geovisio_cli-0.2.1/geovisio_cli/sequence.py
+-rw-r--r--   0        0        0     2107 2023-06-22 09:18:10.500879 geovisio_cli-0.2.1/geovisio_cli/utils.py
+-rw-r--r--   0        0        0     1196 2023-06-22 09:18:10.500879 geovisio_cli-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-14 15:26:20.137987 geovisio_cli-0.2.1/tests/__init__.py
+-rw-r--r--   0        0        0      234 2023-06-19 17:19:08.702865 geovisio_cli-0.2.1/tests/conftest.py
+-rw-r--r--   0        0        0   523332 2023-03-14 15:26:20.137987 geovisio_cli-0.2.1/tests/fixtures/e1.jpg
+-rw-r--r--   0        0        0   483454 2023-03-14 15:26:20.141986 geovisio_cli-0.2.1/tests/fixtures/e2.jpg
+-rw-r--r--   0        0        0   529344 2023-03-14 15:26:20.141986 geovisio_cli-0.2.1/tests/fixtures/e3.jpg
+-rw-r--r--   0        0        0       16 2023-03-14 15:26:20.141986 geovisio_cli-0.2.1/tests/fixtures/invalid_pic.jpg
+-rw-r--r--   0        0        0       27 2023-03-14 15:26:20.141986 geovisio_cli-0.2.1/tests/fixtures/not_a_pic.md
+-rw-r--r--   0        0        0        0 2023-03-14 15:26:20.141986 geovisio_cli-0.2.1/tests/integration/__init__.py
+-rw-r--r--   0        0        0     3327 2023-05-24 13:17:27.558420 geovisio_cli-0.2.1/tests/integration/conftest.py
+-rw-r--r--   0        0        0     2189 2023-05-22 08:59:23.607560 geovisio_cli-0.2.1/tests/integration/docker-compose-geovisio.yml
+-rw-r--r--   0        0        0      584 2023-05-22 08:59:23.607560 geovisio_cli-0.2.1/tests/integration/docker-compose-gitlab-override.yml
+-rw-r--r--   0        0        0    76457 2023-05-22 08:59:23.611560 geovisio_cli-0.2.1/tests/integration/keycloak-realm.json
+-rw-r--r--   0        0        0     3210 2023-06-22 08:20:49.394297 geovisio_cli-0.2.1/tests/integration/test_auth.py
+-rw-r--r--   0        0        0      369 2023-05-24 13:17:27.558420 geovisio_cli-0.2.1/tests/integration/test_status.py
+-rw-r--r--   0        0        0     7087 2023-06-22 08:20:49.394297 geovisio_cli-0.2.1/tests/integration/test_upload.py
+-rw-r--r--   0        0        0      583 2023-05-10 11:47:16.328656 geovisio_cli-0.2.1/tests/test_process.py
+-rw-r--r--   0        0        0    10801 2023-06-22 08:20:49.394297 geovisio_cli-0.2.1/tests/test_sequence.py
+-rw-r--r--   0        0        0      682 2023-06-22 09:18:10.500879 geovisio_cli-0.2.1/tests/test_utils.py
+-rw-r--r--   0        0        0     8652 1970-01-01 00:00:00.000000 geovisio_cli-0.2.1/PKG-INFO
```

### Comparing `geovisio_cli-0.2.0/.gitlab-ci.yml` & `geovisio_cli-0.2.1/.gitlab-ci.yml`

 * *Files 4% similar despite different names*

```diff
@@ -17,23 +17,24 @@
   script:
     - pip install .[dev]
     - mypy geovisio_cli/
 
 lint:
   image: python:3.8-alpine
   script:
+    - apk add --update --no-cache git
     - pip install .[dev]
     - black --fast --check .
 
 tests:
   image: python:3.8-alpine
   services:
     - docker:dind
   script:
-    - apk add --update --no-cache docker-cli docker-cli-compose
+    - apk add --update --no-cache docker-cli docker-cli-compose git
     - PROJECT_DIR=$PWD docker compose -f tests/integration/docker-compose-geovisio.yml -f tests/integration/docker-compose-gitlab-override.yml run --rm integration-test-runner
 
   after_script:
     - PROJECT_DIR=$PWD docker compose -f tests/integration/docker-compose-geovisio.yml -f tests/integration/docker-compose-gitlab-override.yml logs || true
     - PROJECT_DIR=$PWD docker compose -f tests/integration/docker-compose-geovisio.yml -f tests/integration/docker-compose-gitlab-override.yml down || true
 
 deploy_pypi:
```

### Comparing `geovisio_cli-0.2.0/CHANGELOG.md` & `geovisio_cli-0.2.1/CHANGELOG.md`

 * *Files 13% similar despite different names*

```diff
@@ -2,14 +2,26 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.2.1] - 2023-06-22
+
+### Added
+- A new parameter `--sort-method` allows user to choose how pictures should be sorted, either by their date/time or file name, in ascending or descending order. Default is now by date/time ascending (was previously by filename ascending).
+- A new `--version` parameter to get the geovisio_cli version
+
+### Changed
+- A new warning is displayed on every command if the package version is not the latest
+
+### Fixes
+- Uploading twice the same sequence do not print any misleading errors
+
 ## [0.2.0] - 2023-05-24
 
 ### Added
 - A new `--token` parameter to `geovisio upload` to provide a custom geovisio token for authentication.
 - A new `geovisio login` command to login on a geovisio instance
 
 ### Changed
@@ -57,15 +69,16 @@
 
 ## [0.0.1] - 2023-03-14
 
 ### Added
 - Basic scripts for uploading pictures to a GeoVisio API
 
 
-[Unreleased]: https://gitlab.com/geovisio/cli/-/compare/0.2.0...main
+[Unreleased]: https://gitlab.com/geovisio/cli/-/compare/0.2.1...main
+[0.2.1]: https://gitlab.com/geovisio/cli/-/compare/0.2.0...0.2.1
 [0.2.0]: https://gitlab.com/geovisio/cli/-/compare/0.1.0...0.2.0
 [0.1.0]: https://gitlab.com/geovisio/cli/-/compare/0.0.5...0.1.0
 [0.0.5]: https://gitlab.com/geovisio/cli/-/compare/0.0.4...0.0.5
 [0.0.4]: https://gitlab.com/geovisio/cli/-/compare/0.0.3...0.0.4
 [0.0.3]: https://gitlab.com/geovisio/cli/-/compare/0.0.2...0.0.3
 [0.0.2]: https://gitlab.com/geovisio/cli/-/compare/0.0.1...0.0.2
 [0.0.1]: https://gitlab.com/PanierAvide/geovisio/-/commits/0.0.1
```

### Comparing `geovisio_cli-0.2.0/CODE_OF_CONDUCT.md` & `geovisio_cli-0.2.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.2.0/LICENSE` & `geovisio_cli-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.2.0/Makefile` & `geovisio_cli-0.2.1/Makefile`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.2.0/README.md` & `geovisio_cli-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.2.0/USAGE.md` & `geovisio_cli-0.2.1/USAGE.md`

 * *Files 20% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 ```console
 $ geovisio [OPTIONS] COMMAND [ARGS]...
 ```
 
 **Options**:
 
+* `--version`: Show GeoVisio command-line client version and exit
 * `--install-completion`: Install completion for the current shell.
 * `--show-completion`: Show completion for the current shell, to copy it or customize the installation.
 * `--help`: Show this message and exit.
 
 **Commands**:
 
 * `collection-status`: Print the status of a collection.
@@ -74,14 +75,15 @@
 **Arguments**:
 
 * `PATH`: Local path to your sequence folder  [required]
 
 **Options**:
 
 * `--title TEXT`: Collection title. If not provided, the title will be the directory name.
+* `--sort-method [filename-asc|filename-desc|time-asc|time-desc]`: Strategy used for sorting your pictures. Either by filename or EXIF time, in ascending or descending order.  [default: time-asc]
 * `--help`: Show this message and exit.
 
 ## `geovisio upload`
 
 Processes and sends a given sequence on your GeoVisio API
 
 **Usage**:
@@ -100,8 +102,9 @@
 * `--wait / --no-wait`: Wait for all pictures to be ready  [default: no-wait]
 * `--is-blurred / --is-not-blurred`: Define if sequence is already blurred or not  [default: is-not-blurred]
 * `--title TEXT`: Collection title. If not provided, the title will be the directory name.
 * `--token TEXT`: GeoVisio token if the geovisio instance needs it.
 
 If none is provided and the geovisio instance requires it, the token will be asked during run.
 Note: is is advised to wait for prompt without using this variable.
+* `--sort-method [filename-asc|filename-desc|time-asc|time-desc]`: Strategy used for sorting your pictures. Either by filename or EXIF time, in ascending or descending order.  [default: time-asc]
 * `--help`: Show this message and exit.
```

### Comparing `geovisio_cli-0.2.0/geovisio_cli/auth.py` & `geovisio_cli-0.2.1/geovisio_cli/auth.py`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.2.0/geovisio_cli/sequence.py` & `geovisio_cli-0.2.1/geovisio_cli/sequence.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,35 +16,48 @@
 from rich.panel import Panel
 from rich.console import Group
 from rich.live import Live
 from geovisio_cli.exception import CliException, raise_for_status
 from geovisio_cli.auth import login
 from geovisio_cli.model import Geovisio
 from geovisio_cli import utils
+from geopic_tag_reader import reader
+from PIL import Image
 from time import sleep
 from datetime import timedelta
 import os
 import toml
+from . import exception
+from enum import Enum
+import logging
 
 SEQUENCE_TOML_FILE = "_geovisio.toml"
 
 
+class SortMethod(str, Enum):
+    filename_asc = "filename-asc"
+    filename_desc = "filename-desc"
+    time_asc = "time-asc"
+    time_desc = "time-desc"
+
+
 @dataclass
 class InteriorOrientation:
     make: str
     model: str
     field_of_view: Optional[int]
 
 
 @dataclass
 class Picture:
     path: Optional[str] = None
     id: Optional[str] = None
     location: Optional[str] = None
     status: Optional[str] = None
+    metadata: Optional[reader.GeoPicTags] = None
 
     def toml(self):
         return {
             "path": self.path,
             "id": self.id,
             "location": self.location,
             "status": self.status,
@@ -65,23 +78,27 @@
     title: str = ""
     path: str = ""
     id: Optional[str] = None
     location: Optional[str] = None
     producer: Optional[str] = None
     interior_orientation: List[InteriorOrientation] = field(default_factory=lambda: [])
     pictures: List[Picture] = field(default_factory=lambda: [])
+    sort_method: Optional[SortMethod] = None
 
     def toml(self):
         res = {
             "sequence": {
                 "title": self.title,
                 "path": self.path,
                 "id": self.id,
                 "location": self.location,
                 "producer": self.producer,
+                "sort_method": self.sort_method.value
+                if self.sort_method is not None
+                else None,
             },
             "pictures": {},
         }
 
         for pos, pic in enumerate(self.pictures, start=1):
             pict = pic.toml()
             pict["position"] = pos
@@ -92,14 +109,19 @@
     def from_toml(self, data):
         if data.get("sequence"):
             self.title = data["sequence"].get("title", "")
             self.path = data["sequence"].get("path", "")
             self.id = data["sequence"].get("id")
             self.location = data["sequence"].get("location")
             self.producer = data["sequence"].get("producer")
+            self.sort_method = (
+                SortMethod(data["sequence"]["sort_method"])
+                if "sort_method" in data["sequence"]
+                else None
+            )
 
         if data.get("pictures"):
             self.pictures = [
                 Picture.from_toml(picData)
                 for picId, picData in sorted(
                     data["pictures"].items(), key=lambda item: int(item[1]["position"])
                 )
@@ -132,38 +154,41 @@
 @dataclass
 class UploadReport:
     location: str
     uploaded_pictures: List[Picture] = field(default_factory=lambda: [])
     errors: List[UploadError] = field(default_factory=lambda: [])
 
 
-def process(path: Path, title: Optional[str]) -> Sequence:
-    sequence = _read_sequence(path, title)
+def process(
+    path: Path, title: Optional[str], sortMethod: Optional[SortMethod] = None
+) -> Sequence:
+    sequence = _read_sequence(path, title, sortMethod)
     _check_sequence(sequence)
     _write_sequence_toml(sequence)
     return sequence
 
 
 def upload(
     path: Path,
     geovisio: Geovisio,
     title: Optional[str],
     wait: bool = False,
     alreadyBlurred: bool = False,
+    sortMethod: Optional[SortMethod] = None,
 ) -> UploadReport:
     # early test that the given url is correct
     utils.test_geovisio_url(geovisio.url)
     with requests.session() as s:
         # early test login
         if not _login_if_needed(s, geovisio):
             raise CliException(
                 "🔁 Computer not authenticated yet, impossible to upload pictures, but you can try again the same upload command after finalizing the login"
             )
 
-        sequence = process(path, title)
+        sequence = process(path, title, sortMethod)
 
         return _publish(s, sequence, geovisio, wait, alreadyBlurred)
 
 
 def _publish(
     session: requests.Session,
     sequence: Sequence,
@@ -200,14 +225,20 @@
         sequence.id = seq.json()["id"]
         sequence.location = seq.headers["Location"]
         _write_sequence_toml(sequence)
 
         print(f"✅ Created collection {sequence.location}")
 
     else:
+        if len(picturesToUpload) == 0:
+            print(
+                f"✅ Everything ({len(sequence.pictures)} picture{'s' if len(sequence.pictures) != 1 else ''}) have already been uploaded, nothing to do"
+            )
+            assert sequence.location
+            return UploadReport(location=sequence.location)
         print(
             f"⏭️ Skipping {len(sequence.pictures) - len(picturesToUpload)} already published pictures"
         )
 
     if not sequence.location:
         raise CliException("Sequence has no API location defined")
 
@@ -341,64 +372,116 @@
 
 
 def _check_sequence(sequence: Sequence):
     if not sequence.pictures:
         raise CliException(f"No pictures to upload for sequence {sequence.title}")
 
 
-def _sort_files(pictures: List[Picture]) -> List[Picture]:
+def _sort_files(
+    pictures: List[Picture], method: Optional[SortMethod] = SortMethod.time_asc
+) -> List[Picture]:
     """Sorts pictures according to their file name
 
     Parameters
     ----------
     pictures : Picture[]
         List of pictures to sort
+    method : SortMethod
+        Sort logic to adopt (time-asc, time-desc, filename-asc, filename-desc)
 
     Returns
     -------
     Picture[]
         List of pictures, sorted
     """
 
-    # Try to sort based on numeric notation
-    try:
-        pictures.sort(key=lambda p: int(PurePath(p.path or "").stem))
-    # Otherwise, sort as strings
-    except:
-        pictures.sort(key=lambda p: PurePath(p.path or "").stem)
+    if method is None:
+        method = SortMethod.time_asc
+
+    if method not in [item.value for item in SortMethod]:
+        raise exception.CliException("Invalid sort strategy: " + str(method))
+
+    # Get the sort logic
+    strat, order = method.split("-")
+
+    # Sort based on filename
+    if strat == "filename":
+
+        def sort_fct(p):
+            try:  # Try to sort based on numeric notation
+                return int(PurePath(p.path or "").stem)
+            except:  # Otherwise, sort as strings
+                return PurePath(p.path or "").stem
+
+        pictures.sort(key=sort_fct)
+
+    # Sort based on picture ts
+    elif strat == "time":
+        pictures.sort(key=lambda p: p.metadata.ts if p.metadata is not None else 0)
+
+    if order == "desc":
+        pictures.reverse()
 
     return pictures
 
 
-def _read_sequence(path: Path, title: Optional[str] = None) -> Sequence:
+def _read_sequence(
+    path: Path, title: Optional[str] = None, sortMethod: Optional[SortMethod] = None
+) -> Sequence:
     if not path.is_dir():
         raise CliException(f"{path} is not a directory, cannot read pictures")
 
     if title is None:
         title = path.name
 
-    s = Sequence(title=title, path=str(path.absolute()))
+    s = Sequence(title=title, path=str(path.absolute()), sort_method=sortMethod)
 
     # Check if a TOML file exists, then use it instead of generating one
     stoml = os.path.join(s.path, SEQUENCE_TOML_FILE)
     if os.path.isfile(stoml):
         print(f"📄 Using metadata from existing config file: {stoml}")
         _update_sequence_from_toml(s)
 
+        # Check sort method
+        if (
+            sortMethod is not None
+            and s.sort_method is not None
+            and sortMethod != s.sort_method
+        ):
+            raise CliException(
+                f'Sort method passed as argument ({sortMethod.value}) is different from the one defined in your metadata file ({s.sort_method.value}).\nYou may either change --sort-method argument from command-line, or change "sort_method" in your metadata file.'
+            )
+
     # Create sequence from pictures files
     else:
         print(f"🔍 Listing available pictures")
         for f in path.iterdir():
             if not f.is_file():
                 continue
             if f.suffix.lower() not in [".jpg", ".jpeg"]:
                 continue
-            s.pictures.append(Picture(path=str(f)))
 
-        s.pictures = _sort_files(s.pictures)
+            # Read metadata
+            try:
+                meta = reader.readPictureMetadata(Image.open(str(f)))
+                s.pictures.append(Picture(path=str(f), metadata=meta))
+            except Exception as e:
+                logging.warning(f"Picture {str(f)} has invalid metadata: {str(e)}")
+                s.pictures.append(Picture(path=str(f), status="broken-metadata"))
+
+        s.pictures = _sort_files(s.pictures, sortMethod)
+
+    # Check if at least one picture is valid
+    if (
+        len(s.pictures) > 0
+        and len([p for p in s.pictures if p.status != "broken-metadata"]) == 0
+    ):
+        raise CliException(
+            "❌ All read pictures have invalid metadata.\nPlease check if your pictures are geolocated and have a date defined.\nFor more information: https://gitlab.com/geovisio/api/-/blob/develop/docs/15_Pictures_requirements.md"
+        )
 
     return s
 
 
 def _write_sequence_toml(sequence: Sequence):
     """Writes TOML sequence metadata file"""
```

### Comparing `geovisio_cli-0.2.0/geovisio_cli/utils.py` & `geovisio_cli-0.2.1/geovisio_cli/utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from geovisio_cli.exception import CliException
+from rich import print
 import requests
 
 REQUESTS_TIMEOUT = 30
 
 
 def test_geovisio_url(geovisio: str):
-    full_url = f"{geovisio}/api/collections"
+    full_url = f"{geovisio}/api"
     try:
         r = requests.get(full_url, timeout=REQUESTS_TIMEOUT)
     except (
         requests.Timeout,
         requests.ConnectionError,
         requests.ConnectTimeout,
         requests.TooManyRedirects,
@@ -44,7 +45,23 @@
     if r.status_code > 404:
         raise CliException(
             f"""The API is unavailable for now. Please check given error and retry later.
 [bold]Used URL:[/bold] {full_url}
 [bold]Error[/bold] (code [cyan]{r.status_code}[/cyan]):
 {r.text}"""
         )
+
+
+def check_if_lastest_version():
+    from packaging import version
+    import geovisio_cli
+
+    pypi_url = "https://pypi.org/pypi/geovisio_cli"
+    response = requests.get(f"{pypi_url}/json")
+    latest_version = response.json()["info"]["version"]
+
+    if version.parse(latest_version) > version.parse(geovisio_cli.__version__):
+        print(
+            f"⚠️ A newer geovisio_cli version {latest_version} is available on PyPI (available on {pypi_url}).\nWe highly recommend updating as this tool is still in beta version, and new versions ensure good compatibility with GeoVisio API."
+        )
+        return False
+    return True
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `geovisio_cli-0.2.0/pyproject.toml` & `geovisio_cli-0.2.1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -9,18 +9,19 @@
 ]
 readme = "README.md"
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: MIT License"]
 dynamic = ["version", "description"]
 dependencies = [
     "requests ~= 2.28.0",
-    "typer ~= 0.7.0",
+    "typer ~= 0.9.0",
     "rich[all] ~= 13.3.0",
     "toml ~= 0.10.2",
     "qrcode ~= 7.4.2",
+    "geopic-tag-reader ~= 0.1.3",
 ]
 
 [project.urls]
 Home = "https://gitlab.com/geovisio/cli"
 
 [project.scripts]
 geovisio="geovisio_cli.main:app"
@@ -29,16 +30,20 @@
 dev = [
     "black ~= 22.8.0",
     "mypy ~= 1.0.0",
     "types-requests ~= 2.28.0",
     "pytest ~= 7.2.0",
     "testcontainers-compose ~= 0.0.1rc1",
     "pytest-datafiles ~= 2.0.1",
-    "typer-cli ~= 0.0.13",
+    
+    "typer-cli-forked ~= 0.0.14", # fork dependency needed until https://github.com/tiangolo/typer-cli/pull/120 is merged.
+    #"typer-cli ~= 0.0.13",
     "types-toml ~= 0.10.8.6",
+    "types-Pillow ~= 9.5.0.4",
+    "requests_mock ~= 1.10.0",
 ]
 build = ["flit ~= 3.8.0"]
 
 [tool.pytest.ini_options]
 addopts = [
     "--import-mode=importlib",
 ]
```

### Comparing `geovisio_cli-0.2.0/tests/fixtures/e1.jpg` & `geovisio_cli-0.2.1/tests/fixtures/e1.jpg`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.2.0/tests/fixtures/e2.jpg` & `geovisio_cli-0.2.1/tests/fixtures/e2.jpg`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.2.0/tests/fixtures/e3.jpg` & `geovisio_cli-0.2.1/tests/fixtures/e3.jpg`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.2.0/tests/integration/conftest.py` & `geovisio_cli-0.2.1/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.2.0/tests/integration/docker-compose-geovisio.yml` & `geovisio_cli-0.2.1/tests/integration/docker-compose-geovisio.yml`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.2.0/tests/integration/docker-compose-gitlab-override.yml` & `geovisio_cli-0.2.1/tests/integration/docker-compose-gitlab-override.yml`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.2.0/tests/integration/keycloak-realm.json` & `geovisio_cli-0.2.1/tests/integration/keycloak-realm.json`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.2.0/tests/integration/test_auth.py` & `geovisio_cli-0.2.1/tests/integration/test_auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,10 +81,10 @@
     msg = str(e.value)
     assert msg.startswith(
         f"""The API URL is not valid.
 
 Note that your URL should be the API root (something like https://geovisio.fr, https://panoramax.ign.fr or any other geovisio instance).
 Please make sure you gave the correct URL and retry.
 
-[bold]Used URL:[/bold] {geovisio_with_token.url}/some_additional_path/api/collections
+[bold]Used URL:[/bold] {geovisio_with_token.url}/some_additional_path/api
 [bold]Error:[/bold]"""
     )
```

### Comparing `geovisio_cli-0.2.0/tests/integration/test_upload.py` & `geovisio_cli-0.2.1/tests/integration/test_upload.py`

 * *Files 12% similar despite different names*

```diff
@@ -67,15 +67,18 @@
     os.rename(picE2, picE2bak)
     with open(picE2, "w") as picE2file:
         picE2file.write("")
         picE2file.close()
 
     # Start upload -> 2 uploaded pics + 1 failure
     uploadReport = sequence.upload(
-        path=Path(datafiles), geovisio=geovisio_with_token, title="some title"
+        path=Path(datafiles),
+        geovisio=geovisio_with_token,
+        title="some title",
+        sortMethod=sequence.SortMethod.filename_asc,
     )
     assert len(uploadReport.uploaded_pictures) == 2
     assert len(uploadReport.errors) == 1
     assert uploadReport.errors[0].position == 2
 
     # Check TOML file -> e2 has no ID but broken status
     tomlFile = datafiles / sequence.SEQUENCE_TOML_FILE
@@ -88,15 +91,18 @@
 
     # Make e2 valid
     os.remove(picE2)
     os.rename(picE2bak, picE2)
 
     # Launch again upload : 1 uploaded pic + 0 failure
     uploadReport2 = sequence.upload(
-        path=Path(datafiles), geovisio=geovisio_with_token, title="some title"
+        path=Path(datafiles),
+        geovisio=geovisio_with_token,
+        title="some title",
+        sortMethod=sequence.SortMethod.filename_asc,
     )
     assert uploadReport2.location == uploadReport.location
     assert len(uploadReport2.uploaded_pictures) == 1
     assert len(uploadReport2.errors) == 0
 
     # Check TOML file -> everything has ID and looks like a charm
     with open(tomlFile, "r") as f:
@@ -114,65 +120,31 @@
         )
 
 
 @pytest.mark.datafiles(
     os.path.join(FIXTURE_DIR, "e1.jpg"),
     os.path.join(FIXTURE_DIR, "e2.jpg"),
     os.path.join(FIXTURE_DIR, "e3.jpg"),
-    os.path.join(FIXTURE_DIR, "invalid_pic.jpg"),
 )
-def test_upload_with_invalid_file(geovisio_with_token, datafiles):
+def test_upload_twice(geovisio_with_token, datafiles):
+    """Uploading twice the same sequence, should result of nothing done in the second upload"""
+    # Start upload -> 2 uploaded pics + 1 failure
     uploadReport = sequence.upload(
-        path=Path(datafiles), geovisio=geovisio_with_token, title=None
+        path=Path(datafiles), geovisio=geovisio_with_token, title="some title"
     )
-
-    # Only 3 pictures should have been uploaded, 1 is in error
     assert len(uploadReport.uploaded_pictures) == 3
-    assert len(uploadReport.errors) == 1
-
-    # But the collection status should have 3 items (and be valid)
-    collection = sequence.Sequence(location=uploadReport.location)
-    sequence.wait_for_sequence(collection, timeout=timedelta(minutes=1))
-    status = sequence.status(collection)
-    # 3 pictures should have been uploaded
-    assert len(status.pictures) == 3
-
-    assert all([i.status == "ready" for i in status.pictures])
-
-    # the collection should also have 3 items
-    items = requests.get(f"{collection.location}/items")
-    items.raise_for_status()
-    features = items.json()["features"]
-    assert len(features) == 3
-    collection = requests.get(f"{collection.location}")
-    assert (
-        collection.json()["title"] == Path(datafiles).name
-    )  # since no title has been set, the directory name has been choosen
-
+    assert len(uploadReport.errors) == 0
 
-@pytest.mark.datafiles(
-    os.path.join(FIXTURE_DIR, "invalid_pic.jpg"),
-)
-def test_upload_with_no_valid_file(geovisio_with_token, datafiles):
-    uploadReport = sequence.upload(
-        path=Path(datafiles), geovisio=geovisio_with_token, title="a title"
+    # Launch again upload : 1 uploaded pic + 0 failure
+    uploadReport2 = sequence.upload(
+        path=Path(datafiles), geovisio=geovisio_with_token, title="some title"
     )
-
-    assert len(uploadReport.uploaded_pictures) == 0
-    assert len(uploadReport.errors) == 1
-
-    status = requests.get(f"{uploadReport.location}/geovisio_status")
-    assert (
-        status.status_code == 404
-    )  # TODO: For the moment geovisio return a 404, we it should return a valid status response with the sequence status
-
-    items = requests.get(f"{uploadReport.location}/items")
-    items.raise_for_status()
-    features = items.json()["features"]
-    assert len(features) == 0
+    assert uploadReport2.location == uploadReport.location
+    assert len(uploadReport2.uploaded_pictures) == 0
+    assert len(uploadReport2.errors) == 0
 
 
 @pytest.mark.datafiles(
     os.path.join(FIXTURE_DIR, "e1.jpg"),
 )
 def test_upload_on_invalid_url_host(datafiles):
     with pytest.raises(exception.CliException) as e:
@@ -181,15 +153,15 @@
             geovisio=model.Geovisio(url="http://some_invalid_url"),
             title="some title",
         )
     msg = str(e.value)
     assert msg.startswith(
         """The API is not reachable. Please check error and used URL below, and retry later if the URL is correct.
 
-[bold]Used URL:[/bold] http://some_invalid_url/api/collections
+[bold]Used URL:[/bold] http://some_invalid_url/api
 [bold]Error:[/bold]"""
     )
     assert "Failed to establish a new connection:" in msg
 
 
 @pytest.mark.datafiles(
     os.path.join(FIXTURE_DIR, "e1.jpg"),
@@ -206,15 +178,15 @@
     msg = str(e.value)
     assert msg.startswith(
         f"""The API URL is not valid.
 
 Note that your URL should be the API root (something like https://geovisio.fr, https://panoramax.ign.fr or any other geovisio instance).
 Please make sure you gave the correct URL and retry.
 
-[bold]Used URL:[/bold] {geovisio_with_token.url}/some_additional_path/api/collections
+[bold]Used URL:[/bold] {geovisio_with_token.url}/some_additional_path/api
 [bold]Error:[/bold]"""
     )
 
 
 @pytest.mark.datafiles(
     os.path.join(FIXTURE_DIR, "e1.jpg"),
 )
@@ -224,10 +196,10 @@
             path=Path(datafiles),
             geovisio=model.Geovisio(url="a non valid url at all"),
             title=None,
         )
     assert str(e.value).startswith(
         """Error while connecting to the API. Please check error and used URL below
 
-[bold]Used URL:[/bold] a non valid url at all/api/collections
+[bold]Used URL:[/bold] a non valid url at all/api
 [bold]Error:[/bold]"""
     )
```

### Comparing `geovisio_cli-0.2.0/tests/test_process.py` & `geovisio_cli-0.2.1/tests/test_process.py`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.2.0/PKG-INFO` & `geovisio_cli-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 Metadata-Version: 2.1
 Name: geovisio_cli
-Version: 0.2.0
+Version: 0.2.1
 Summary: Geovio client cli tool
 Author-email: Antoine Desbordes <antoine.desbordes@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: requests ~= 2.28.0
-Requires-Dist: typer ~= 0.7.0
+Requires-Dist: typer ~= 0.9.0
 Requires-Dist: rich[all] ~= 13.3.0
 Requires-Dist: toml ~= 0.10.2
 Requires-Dist: qrcode ~= 7.4.2
+Requires-Dist: geopic-tag-reader ~= 0.1.3
 Requires-Dist: flit ~= 3.8.0 ; extra == "build"
 Requires-Dist: black ~= 22.8.0 ; extra == "dev"
 Requires-Dist: mypy ~= 1.0.0 ; extra == "dev"
 Requires-Dist: types-requests ~= 2.28.0 ; extra == "dev"
 Requires-Dist: pytest ~= 7.2.0 ; extra == "dev"
 Requires-Dist: testcontainers-compose ~= 0.0.1rc1 ; extra == "dev"
 Requires-Dist: pytest-datafiles ~= 2.0.1 ; extra == "dev"
-Requires-Dist: typer-cli ~= 0.0.13 ; extra == "dev"
+Requires-Dist: typer-cli-forked ~= 0.0.14 ; extra == "dev"
 Requires-Dist: types-toml ~= 0.10.8.6 ; extra == "dev"
+Requires-Dist: types-Pillow ~= 9.5.0.4 ; extra == "dev"
+Requires-Dist: requests_mock ~= 1.10.0 ; extra == "dev"
 Project-URL: Home, https://gitlab.com/geovisio/cli
 Provides-Extra: build
 Provides-Extra: dev
 
 # ![GeoVisio](https://gitlab.com/geovisio/api/-/raw/develop/images/logo_full.png)
 
 __GeoVisio__ is a complete solution for storing and __serving your own 📍📷 geolocated pictures__ (like [StreetView](https://www.google.com/streetview/) / [Mapillary](https://mapillary.com/)).
```

