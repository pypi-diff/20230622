# Comparing `tmp/images_upload_cli-1.1.3a0.tar.gz` & `tmp/images_upload_cli-2.0.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "images_upload_cli-1.1.3a0.tar", max compression
+gzip compressed data, was "images_upload_cli-2.0.0a0.tar", max compression
```

## Comparing `images_upload_cli-1.1.3a0.tar` & `images_upload_cli-2.0.0a0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1065 2023-05-08 18:36:04.824719 images_upload_cli-1.1.3a0/LICENSE
--rw-r--r--   0        0        0     5248 2023-05-08 18:36:04.824719 images_upload_cli-1.1.3a0/README.md
--rw-r--r--   0        0        0     2514 2023-05-08 18:36:18.724625 images_upload_cli-1.1.3a0/pyproject.toml
--rwxr-xr-x   0        0        0      188 2023-05-08 18:36:04.824719 images_upload_cli-1.1.3a0/src/images_upload_cli/__init__.py
--rwxr-xr-x   0        0        0      178 2023-05-08 18:36:04.824719 images_upload_cli-1.1.3a0/src/images_upload_cli/__main__.py
--rwxr-xr-x   0        0        0     1710 2023-05-08 18:36:04.824719 images_upload_cli-1.1.3a0/src/images_upload_cli/cli.py
--rwxr-xr-x   0        0        0    11016 2023-05-08 18:36:04.824719 images_upload_cli-1.1.3a0/src/images_upload_cli/upload.py
--rwxr-xr-x   0        0        0     3057 2023-05-08 18:36:04.824719 images_upload_cli-1.1.3a0/src/images_upload_cli/util.py
--rw-r--r--   0        0        0     6215 1970-01-01 00:00:00.000000 images_upload_cli-1.1.3a0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-06-21 20:13:21.051465 images_upload_cli-2.0.0a0/LICENSE
+-rw-r--r--   0        0        0     5236 2023-06-21 20:13:21.051465 images_upload_cli-2.0.0a0/README.md
+-rw-r--r--   0        0        0     2557 2023-06-21 20:13:37.943695 images_upload_cli-2.0.0a0/pyproject.toml
+-rwxr-xr-x   0        0        0      175 2023-06-21 20:13:21.051465 images_upload_cli-2.0.0a0/src/images_upload_cli/__init__.py
+-rwxr-xr-x   0        0        0      178 2023-06-21 20:13:21.051465 images_upload_cli-2.0.0a0/src/images_upload_cli/__main__.py
+-rwxr-xr-x   0        0        0     2453 2023-06-21 20:13:21.051465 images_upload_cli-2.0.0a0/src/images_upload_cli/cli.py
+-rwxr-xr-x   0        0        0    10781 2023-06-21 20:13:21.051465 images_upload_cli-2.0.0a0/src/images_upload_cli/upload.py
+-rwxr-xr-x   0        0        0     3090 2023-06-21 20:13:21.051465 images_upload_cli-2.0.0a0/src/images_upload_cli/util.py
+-rw-r--r--   0        0        0     6197 1970-01-01 00:00:00.000000 images_upload_cli-2.0.0a0/PKG-INFO
```

### Comparing `images_upload_cli-1.1.3a0/LICENSE` & `images_upload_cli-2.0.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `images_upload_cli-1.1.3a0/README.md` & `images_upload_cli-2.0.0a0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # images-upload-cli
 
 > Upload images via APIs
 
 [![PyPI version](https://img.shields.io/pypi/v/images-upload-cli)](https://pypi.org/project/images-upload-cli)
 [![AUR version](https://img.shields.io/aur/version/python-images-upload-cli)](https://aur.archlinux.org/packages/python-images-upload-cli)
-[![CI/CD](https://github.com/DeadNews/images-upload-cli/actions/workflows/python-app.yml/badge.svg)](https://github.com/DeadNews/images-upload-cli/actions/workflows/python-app.yml)
+[![Main](https://github.com/DeadNews/images-upload-cli/actions/workflows/main.yml/badge.svg)](https://github.com/DeadNews/images-upload-cli/actions/workflows/main.yml)
 [![pre-commit.ci](https://results.pre-commit.ci/badge/github/DeadNews/images-upload-cli/main.svg)](https://results.pre-commit.ci/latest/github/DeadNews/images-upload-cli/main)
 [![codecov](https://codecov.io/gh/DeadNews/images-upload-cli/branch/main/graph/badge.svg?token=OCZDZIYPMC)](https://codecov.io/gh/DeadNews/images-upload-cli)
 
 ## Installation
 
 PyPI
 
@@ -36,15 +36,14 @@
 | [gyazo](https://gyazo.com/)           |      +       | `https://i.gyazo.com/{id}.png`                       |
 | [imageban](https://imageban.ru/)      |      +       | `https://i2.imageban.ru/out/2022/07/30/{id}.png`     |
 | [imagebin](https://imagebin.ca/)      |      -       | `https://ibin.co/{id}.png`                           |
 | [imgbb](https://imgbb.com/)           |      +       | `https://i.ibb.co/{id}/image.png`                    |
 | [imgchest](https://imgchest.com/)     |      +       | `https://cdn.imgchest.com/files/{id}.png`            |
 | [imgur](https://imgur.com/)           |      -       | `https://i.imgur.com/{id}.png`                       |
 | [lensdump](https://lensdump.com/)     |      +       | `https://i.lensdump.com/i/{id}.png`                  |
-| [pictshare](https://pictshare.net/)   |      -       | `https://pictshare.net/{id}.png`                     |
 | [pixeldrain](https://pixeldrain.com/) |      -       | `https://pixeldrain.com/api/file/{id}`               |
 | [pixhost](https://pixhost.to/)        |      -       | `https://img75.pixhost.to/images/69/{id}_img.png`    |
 | [ptpimg](https://ptpimg.me/)          |      +       | `https://ptpimg.me/{id}.png`                         |
 | [smms](https://sm.ms/)                |      +       | `https://s2.loli.net/2022/07/30/{id}.png`            |
 | [sxcu](https://sxcu.net/)             |      -       | `https://sxcu.net/{id}.png`                          |
 | [telegraph](https://telegra.ph/)      |      -       | `https://telegra.ph/file/{id}.png`                   |
 | [thumbsnap](https://thumbsnap.com/)   |      +       | `https://thumbsnap.com/i/{id}.png`                   |
@@ -58,18 +57,20 @@
 
 ```sh
 Usage: images-upload-cli [OPTIONS] IMAGES...
 
   Upload images via APIs.
 
 Options:
-  -h, --hosting [beeimg|catbox|fastpic|filecoffee|freeimage|gyazo|imageban|imagebin|imgbb|imgchest|imgur|lensdump|pictshare|pixeldrain|pixhost|ptpimg|smms|sxcu|telegraph|thumbsnap|tixte|up2sha|uplio|uploadcare|vgy]
+  -h, --hosting [beeimg|catbox|fastpic|filecoffee|freeimage|gyazo|imageban|imagebin|imgbb|imgchest|imgur|lensdump|pixeldrain|pixhost|ptpimg|smms|sxcu|telegraph|thumbsnap|tixte|up2sha|uplio|uploadcare|vgy]
                                   [default: imgur]
   -b, --bbcode                    Add bbcode tags.
   -t, --thumbnail                 Add caption thumbnail and bbcode tags.
+  -n, --notify / -N, --no-notify  Send desktop notifications via libnotify.
+                                  [default: N]
   -c, --clipboard / -C, --no-clipboard
                                   Copy result to clipboard.  [default: c]
   --version                       Show the version and exit.
   --help                          Show this message and exit.
 ```
 
 ## Env variables
```

### Comparing `images_upload_cli-1.1.3a0/pyproject.toml` & `images_upload_cli-2.0.0a0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,50 +1,51 @@
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry]
 name = "images-upload-cli"
-version = "1.1.3-alpha.0"
+version = "2.0.0-alpha.0"
 description = "Upload images via APIs"
 authors = ["DeadNews <aurczpbgr@mozmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/DeadNews/images-upload-cli"
 repository = "https://github.com/DeadNews/images-upload-cli"
 keywords = ["cli", "imgur", "image-upload", "upload-images", "upload-pictures"]
 classifiers = ["Environment :: Console", "Operating System :: OS Independent"]
 
 [tool.poetry.scripts]
 images-upload-cli = "images_upload_cli.cli:cli"
 
 [tool.poetry.dependencies]
-python = "^3.8.1"
+python = "^3.9"
 click = "^8.1.3"
+httpx = "^0.24.1"
 pillow = "^9.5.0"
 pyperclip = "^1.8.2"
 python-dotenv = "^1.0.0"
-requests = "^2.30.0"
 
-[tool.poetry.group.ci.dependencies]
+[tool.poetry.group.lint.dependencies]
 black = "^23.3.0"
-mypy = "^1.2.0"
+mypy = "^1.4.0"
 poethepoet = "^0.20.0"
-ruff = "^0.0.265"
-types-requests = "^2.29.0.0"
+ruff = "^0.0.274"
 
 [tool.poetry.group.test.dependencies]
-pytest = "^7.3.1"
-pytest-cov = "^4.0.0"
+pytest = "^7.3.2"
+pytest-cov = "^4.1.0"
+pytest-asyncio = "^0.21.0"
+pytest-httpx = "^0.22.0"
 
 [tool.poe.tasks]
 ruff = "ruff check ."
 black = "black --check ."
 mypy = "mypy ."
-ci.sequence = ["ruff", "black", "mypy"]
+lint.sequence = ["ruff", "black", "mypy"]
 
 [tool.poetry-dynamic-versioning]
 enable = false
 vcs = "git"
 style = "semver"
 
 [tool.black]
@@ -70,23 +71,23 @@
 [tool.coverage.report]
 exclude_lines = ["if TYPE_CHECKING:", "if __name__ == .__main__.:"]
 
 [tool.ruff]
 line-length = 99
 select = ["ALL"]
 ignore = [
-  "COM812", # Trailing comma missing
-  "D203",   # 1 blank line required before class docstring
-  "D212",   # Multi-line docstring summary should start at the first line
-  "E501",   # Line too long
-  "EXE001", # Shebang is present but file is not executable
-  "FBT001", # Boolean positional arg in function definition
-  "FBT002", # Boolean default value in function definition
+  "COM812",  # Trailing comma missing
+  "D203",    # 1 blank line required before class docstring
+  "D212",    # Multi-line docstring summary should start at the first line
+  "E501",    # Line too long
+  "EXE001",  # Shebang is present but file is not executable
+  "FBT001",  # Boolean positional arg in function definition
+  "FBT002",  # Boolean default value in function definition
+  "PLR0913", # Too many arguments to function call
   #
-  "S113", # Missing requests timeout
   "S603", # Calling subprocess.Popen with shell=False
 ]
 
 [tool.ruff.per-file-ignores]
 "__init__.py" = ["F401"]
 "tests/*" = ["ANN", "D", "PLC1901", "PLR2004", "S"]
```

### Comparing `images_upload_cli-1.1.3a0/src/images_upload_cli/cli.py` & `images_upload_cli-2.0.0a0/src/images_upload_cli/cli.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,65 +1,96 @@
 #!/usr/bin/env python
 """Entrypoint for cli."""
-from __future__ import annotations
 
+import asyncio
+from collections.abc import Callable
 from pathlib import Path
 
 import click
 from dotenv import load_dotenv
+from httpx import AsyncClient
 from pyperclip import copy
 
 from images_upload_cli.upload import HOSTINGS, UPLOAD
-from images_upload_cli.util import get_config_path, kdialog, make_thumbnail
+from images_upload_cli.util import get_config_path, make_thumbnail, notify_send
 
 
 @click.command(context_settings={"show_default": True})
 @click.argument(
     "images",
     nargs=-1,
     required=True,
     type=click.Path(exists=True, dir_okay=False, path_type=Path),
 )
 @click.option("-h", "--hosting", type=click.Choice(HOSTINGS), default="imgur")
 @click.option("-b", "--bbcode", is_flag=True, help="Add bbcode tags.")
 @click.option("-t", "--thumbnail", is_flag=True, help="Add caption thumbnail and bbcode tags.")
 @click.option(
+    "-n/-N",
+    "--notify/--no-notify",
+    is_flag=True,
+    default=False,
+    help="Send desktop notifications via libnotify.",
+)
+@click.option(
     "-c/-C",
     "--clipboard/--no-clipboard",
     is_flag=True,
     default=True,
     help="Copy result to clipboard.",
 )
 @click.version_option()
 def cli(
     images: tuple[Path],
     hosting: str,
     bbcode: bool,
     thumbnail: bool,
+    notify: bool,
     clipboard: bool,
 ) -> None:
     """Upload images via APIs."""
     # loading .env variables
     load_dotenv(dotenv_path=get_config_path())
 
-    # get upload func
-    upload_func = UPLOAD[hosting]
-
-    # image upload
-    links = []
-    for img_path in images:
-        img = img_path.read_bytes()
-
-        if not thumbnail:
-            link = f"[img]{upload_func(img)}[/img]" if bbcode else upload_func(img)
-        else:
-            thumb = make_thumbnail(img)
-            link = f"[url={upload_func(img)}][img]{upload_func(thumb)}[/img][/url]"
-
-        links.append(link)
+    # images upload
+    links = asyncio.run(
+        upload_images(
+            upload_func=UPLOAD[hosting],
+            images=images,
+            bbcode=bbcode,
+            thumbnail=thumbnail,
+        )
+    )
 
     # out
     links_str = " ".join(links)
     click.echo(links_str)
     if clipboard:
         copy(links_str)
-    kdialog(links_str)
+    if notify:
+        notify_send(links_str)
+
+
+async def upload_images(
+    upload_func: Callable,
+    images: tuple[Path],
+    bbcode: bool,
+    thumbnail: bool,
+) -> list[str]:
+    """Upload images."""
+    links = []
+
+    async with AsyncClient() as client:
+        for img_path in images:
+            img = img_path.read_bytes()
+
+            if not thumbnail:
+                img_link = await upload_func(client, img)
+                link = f"[img]{img_link}[/img]" if bbcode else img_link
+            else:
+                img_link = await upload_func(client, img)
+                thumb_link = await upload_func(client, make_thumbnail(img))
+                link = f"[url={img_link}][img]{thumb_link}[/img][/url]"
+
+            links.append(link)
+
+    return links
```

### Comparing `images_upload_cli-1.1.3a0/src/images_upload_cli/upload.py` & `images_upload_cli-2.0.0a0/src/images_upload_cli/upload.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,423 +1,384 @@
 #!/usr/bin/env python
 """Upload callables."""
-from __future__ import annotations
 
-from collections.abc import Callable  # noqa: TCH003
+from collections.abc import Callable
 from os import getenv
-from re import DOTALL, search, sub
+from re import search
 from urllib.parse import urlparse
 
-from requests import get, post
+from httpx import AsyncClient, HTTPError
 
-from images_upload_cli.util import get_env_val, get_img_ext
+from images_upload_cli.util import get_env, get_img_ext
 
 
-class UploadError(Exception):
-    """Exception raised for upload errors."""
-
-
-def beeimg_upload(img: bytes) -> str:
+async def beeimg_upload(client: AsyncClient, img: bytes) -> str:
     """Upload to beeimg.com."""
     ext = f"img.{get_img_ext(img)}"
 
-    response = post(
+    response = await client.post(
         url="https://beeimg.com/api/upload/file/json/",
         files={"file": (f"img.{ext}", img, f"image/{ext}")},
     )
-    if not response.ok:
-        raise UploadError(response.json())
+    response.raise_for_status()
 
     return f"https:{response.json()['files']['url']}"
 
 
-def catbox_upload(img: bytes) -> str:
+async def catbox_upload(client: AsyncClient, img: bytes) -> str:
     """Upload to catbox.moe."""
-    response = post(
+    response = await client.post(
         url="https://catbox.moe/user/api.php",
         data={"reqtype": "fileupload"},
         files={"fileToUpload": img},
     )
-    if not response.ok:
-        raise UploadError(response.text)
+    response.raise_for_status()
 
     return f"{response.text}"
 
 
-def fastpic_upload(img: bytes) -> str:
+async def fastpic_upload(client: AsyncClient, img: bytes) -> str:
     """Upload to fastpic.org."""
-    response = post(
+    response = await client.post(
         url="https://fastpic.org/upload?api=1",
         data={
             "method": "file",
             "check_thumb": "no",
             "uploading": "1",
         },
         files={"file1": img},
     )
+    response.raise_for_status()
 
-    image_link = (
-        None
-        if (match := search(r"<imagepath>(.+?)</imagepath>", response.text)) is None
-        else match.group(1).strip()
-    )
-    if image_link is None:
-        raise UploadError(response.text)
+    match = search(r"<imagepath>(.+?)</imagepath>", response.text)
+    if match is None:
+        msg = "Image link not found in response."
+        raise HTTPError(msg)
 
-    return image_link
+    return match.group(1).strip()
 
 
-def filecoffee_upload(img: bytes) -> str:
+async def filecoffee_upload(client: AsyncClient, img: bytes) -> str:
     """Upload to file.coffee."""
-    response = post(
+    response = await client.post(
         url="https://file.coffee/api/file/upload",
         files={"file": img},
     )
-    if not response.ok:
-        raise UploadError(response.json())
+    response.raise_for_status()
 
     return response.json()["url"]
 
 
-def freeimage_upload(img: bytes) -> str:
+async def freeimage_upload(client: AsyncClient, img: bytes) -> str:
     """Upload to freeimage.host."""
-    key = get_env_val("FREEIMAGE_KEY")
+    key = get_env("FREEIMAGE_KEY")
 
-    response = post(
+    response = await client.post(
         url="https://freeimage.host/api/1/upload",
         data={"key": key},
         files={"source": img},
     )
-    if not response.ok:
-        raise UploadError(response.json())
+    response.raise_for_status()
 
     return response.json()["image"]["url"]
 
 
-def gyazo_upload(img: bytes) -> str:
+async def gyazo_upload(client: AsyncClient, img: bytes) -> str:
     """Upload to gyazo.com."""
-    key = get_env_val("GYAZO_TOKEN")
+    key = get_env("GYAZO_TOKEN")
 
-    response = post(
+    response = await client.post(
         url=f"https://upload.gyazo.com/api/upload?access_token={key}",
         files={"imagedata": img},
     )
-    if not response.ok:
-        raise UploadError(response.json())
+    response.raise_for_status()
 
     return response.json()["url"]
 
 
-def imageban_upload(img: bytes) -> str:
+async def imageban_upload(client: AsyncClient, img: bytes) -> str:
     """Upload to imageban.ru."""
-    token = get_env_val("IMAGEBAN_TOKEN")
+    token = get_env("IMAGEBAN_TOKEN")
 
-    response = post(
+    response = await client.post(
         url="https://api.imageban.ru/v1",
         headers={"Authorization": f"TOKEN {token}"},
         files={"image": img},
     )
-    if not response.ok:
-        raise UploadError(response.json())
+    response.raise_for_status()
 
     return response.json()["data"]["link"]
 
 
-def imagebin_upload(img: bytes) -> str:
+async def imagebin_upload(client: AsyncClient, img: bytes) -> str:
     """Upload to imagebin.ca."""
-    response = post(
+    response = await client.post(
         url="https://imagebin.ca/upload.php",
         files={"file": img},
     )
-    if not response.ok:
-        raise UploadError(response.text)
+    response.raise_for_status()
 
-    return sub(r".*url:", "", response.text, flags=DOTALL)
+    match = search(r"url:(.+?)$", response.text)
+    if match is None:
+        msg = "Image link not found in response."
+        raise HTTPError(msg)
 
+    return match.group(1).strip()
 
-def imgbb_upload(img: bytes) -> str:
+
+async def imgbb_upload(client: AsyncClient, img: bytes) -> str:
     """Upload to imgbb.com."""
-    key = get_env_val("IMGBB_KEY")
+    key = get_env("IMGBB_KEY")
 
-    response = post(
+    response = await client.post(
         url="https://api.imgbb.com/1/upload",
         data={"key": key},
         files={"image": img},
     )
-    if not response.ok:
-        raise UploadError(response.json())
+    response.raise_for_status()
 
     return response.json()["data"]["url"]
 
 
-def imgchest_upload(img: bytes) -> str:
+async def imgchest_upload(client: AsyncClient, img: bytes) -> str:
     """Upload to imgchest.com."""
-    key = get_env_val("IMGCHEST_KEY")
+    key = get_env("IMGCHEST_KEY")
     ext = get_img_ext(img)
 
-    response = post(
+    response = await client.post(
         url="https://api.imgchest.com/v1/post",
         headers={"Authorization": f"Bearer {key}"},
         files={"images[]": (f"img.{ext}", img)},
     )
-    if not response.ok:
-        raise UploadError(response.json())
+    response.raise_for_status()
 
-    return response.json()["data"]["images"][0]["link"].replace("comfiles", "com/files")
+    return response.json()["data"]["images"][0]["link"]
 
 
-def imgur_upload(img: bytes) -> str:
+async def imgur_upload(client: AsyncClient, img: bytes) -> str:
     """Upload to imgur.com."""
     client_id = getenv("IMGUR_CLIENT_ID", "dd32dd3c6aaa9a0")
 
-    response = post(
+    response = await client.post(
         url="https://api.imgur.com/3/image",
         headers={"Authorization": f"Client-ID {client_id}"},
         files={"image": img},
     )
-    if not response.ok:
-        raise UploadError(response.json())
+    response.raise_for_status()
 
     return response.json()["data"]["link"]
 
 
-def lensdump_upload(img: bytes) -> str:
+async def lensdump_upload(client: AsyncClient, img: bytes) -> str:
     """Upload to lensdump.com."""
-    key = get_env_val("LENSDUMP_KEY")
+    key = get_env("LENSDUMP_KEY")
 
-    response = post(
+    response = await client.post(
         url="https://lensdump.com/api/1/upload",
         data={"key": key},
         files={"source": img},
     )
-    if not response.ok:
-        raise UploadError(response.json())
+    response.raise_for_status()
 
     return response.json()["image"]["url"]
 
 
-def pictshare_upload(img: bytes) -> str:
-    """Upload to pictshare.net."""
-    response = post(
-        url="https://pictshare.net/api/upload.php",
-        files={"file": img},
-    )
-    if not response.ok:
-        raise UploadError(response.json())
-
-    return response.json()["url"]
-
-
-def pixeldrain_upload(img: bytes) -> str:
+async def pixeldrain_upload(client: AsyncClient, img: bytes) -> str:
     """Upload to pixeldrain.com."""
-    response = post(
+    response = await client.post(
         url="https://pixeldrain.com/api/file",
         files={"file": img},
     )
-    if not response.ok:
-        raise UploadError(response.json())
+    response.raise_for_status()
 
     return f"https://pixeldrain.com/api/file/{response.json()['id']}"
 
 
-def pixhost_upload(img: bytes) -> str:
+async def pixhost_upload(client: AsyncClient, img: bytes) -> str:
     """Upload to pixhost.to."""
-    response = post(
+    response = await client.post(
         url="https://api.pixhost.to/images",
         data={"content_type": 0},
         files={"img": img},
     )
-    if not response.ok:
-        raise UploadError(response.json())
+    response.raise_for_status()
 
     show_url = response.json()["show_url"]
 
     # get direct link
+    get_resp = await client.get(show_url)
     u = urlparse(show_url)
     match = search(
         rf"({u.scheme}://(.+?){u.netloc}/images/{u.path.removeprefix('/show/')})",
-        get(show_url).text,
+        get_resp.text,
     )
     image_link = None if match is None else match.group(0).strip()
 
     return show_url if image_link is None else image_link
 
 
-def ptpimg_upload(img: bytes) -> str:
+async def ptpimg_upload(client: AsyncClient, img: bytes) -> str:
     """Upload to ptpimg.me."""
-    key = get_env_val("PTPIMG_KEY")
+    key = get_env("PTPIMG_KEY")
 
-    response = post(
+    response = await client.post(
         url="https://ptpimg.me/upload.php",
         data={"api_key": key},
         files={"file-upload[0]": img},
     )
-    if not response.ok:
-        raise UploadError(response.json())
+    response.raise_for_status()
 
     return f"https://ptpimg.me/{response.json()[0]['code']}.{response.json()[0]['ext']}"
 
 
-def smms_upload(img: bytes) -> str:
+async def smms_upload(client: AsyncClient, img: bytes) -> str:
     """Upload to sm.ms."""
-    key = get_env_val("SMMS_KEY")
+    key = get_env("SMMS_KEY")
 
-    response = post(
+    response = await client.post(
         url="https://sm.ms/api/v2/upload",
         headers={"Authorization": key},
         files={"smfile": img},
     )
-    if not response.ok:
-        raise UploadError(response.json())
+    response.raise_for_status()
+    json = response.json()
 
-    return (
-        response.json()["images"]
-        if response.json()["code"] == "image_repeated"
-        else response.json()["data"]["url"]
-    )
+    return json["images"] if json["code"] == "image_repeated" else json["data"]["url"]
 
 
-def sxcu_upload(img: bytes) -> str:
+async def sxcu_upload(client: AsyncClient, img: bytes) -> str:
     """Upload to sxcu.net."""
-    response = post(
+    response = await client.post(
         url="https://sxcu.net/api/files/create",
+        headers={"user-agent": "python-https/1.0.0"},
         files={"file": img},
     )
-    if not response.ok:
-        raise UploadError(response.text)
+    response.raise_for_status()
 
     return f"{response.json()['url']}.{get_img_ext(img)}"
 
 
-def telegraph_upload(img: bytes) -> str:
+async def telegraph_upload(client: AsyncClient, img: bytes) -> str:
     """Upload to telegra.ph."""
-    response = post(
+    response = await client.post(
         url="https://telegra.ph/upload",
         files={"file": img},
     )
-    if not response.ok:
-        raise UploadError(response.json())
+    response.raise_for_status()
 
     return f"https://telegra.ph{response.json()[0]['src']}"
 
 
-def thumbsnap_upload(img: bytes) -> str:
+async def thumbsnap_upload(client: AsyncClient, img: bytes) -> str:
     """Upload to thumbsnap.com."""
-    key = get_env_val("THUMBSNAP_KEY")
+    key = get_env("THUMBSNAP_KEY")
 
-    response = post(
+    response = await client.post(
         url="https://thumbsnap.com/api/upload",
         data={"key": key},
         files={"media": img},
     )
-    if not response.ok:
-        raise UploadError(response.json())
+    response.raise_for_status()
 
     return response.json()["data"]["media"]
 
 
-def tixte_upload(img: bytes) -> str:
+async def tixte_upload(client: AsyncClient, img: bytes) -> str:
     """Upload to tixte.com."""
-    key = get_env_val("TIXTE_KEY")
+    key = get_env("TIXTE_KEY")
     ext = get_img_ext(img)
 
-    response = post(
+    response = await client.post(
         url="https://api.tixte.com/v1/upload",
         headers={"Authorization": key},
         data={"payload_json": '{"random":true}'},
         files={"file": (f"img.{ext}", img)},
     )
-    if not response.ok:
-        raise UploadError(response.json())
+    response.raise_for_status()
 
     return response.json()["data"]["direct_url"]
 
 
-def up2sha_upload(img: bytes) -> str:
+async def up2sha_upload(client: AsyncClient, img: bytes) -> str:
     """Upload to up2sha.re."""
-    key = get_env_val("UP2SHA_KEY")
+    key = get_env("UP2SHA_KEY")
     ext = get_img_ext(img)
 
-    response = post(
+    response = await client.post(
         url="https://api.up2sha.re/files",
         headers={"X-Api-Key": key},
         files={"file": (f"img.{ext}", img)},
     )
-    if not response.ok:
-        raise UploadError(response.json())
+    response.raise_for_status()
 
     return f"{response.json()['public_url'].replace('file?f=', 'media/raw/')}.{ext}"
 
 
-def uplio_upload(img: bytes) -> str:
+async def uplio_upload(client: AsyncClient, img: bytes) -> str:
     """Upload to upl.io."""
-    key = get_env_val("UPLIO_KEY")
+    key = get_env("UPLIO_KEY")
     ext = get_img_ext(img)
 
-    response = post(
+    response = await client.post(
         url="https://upl.io",
         data={"key": key},
         files={"file": (f"img.{ext}", img)},
     )
-    if not response.ok:
-        raise UploadError(response.text)
+    response.raise_for_status()
 
     host, uid = response.text.rsplit("/", 1)
     return f"{host}/i/{uid}.{ext}"
 
 
-def uploadcare_upload(img: bytes) -> str:
+async def uploadcare_upload(client: AsyncClient, img: bytes) -> str:
     """Upload to uploadcare.com."""
-    key = get_env_val("UPLOADCARE_KEY")
+    key = get_env("UPLOADCARE_KEY")
     name = f"img.{get_img_ext(img)}"
 
-    response = post(
+    response = await client.post(
         url="https://upload.uploadcare.com/base/",
         data={
             "UPLOADCARE_PUB_KEY": key,
             "UPLOADCARE_STORE": "1",
         },
         files={"filename": (name, img)},
     )
-    if not response.ok:
-        raise UploadError(response.json())
+    response.raise_for_status()
 
     return f"https://ucarecdn.com/{response.json()['filename']}/{name}"
 
 
-def vgy_upload(img: bytes) -> str:
+async def vgy_upload(client: AsyncClient, img: bytes) -> str:
     """Upload to vgy.me."""
-    key = get_env_val("VGY_KEY")
+    key = get_env("VGY_KEY")
     ext = get_img_ext(img)
 
-    response = post(
+    response = await client.post(
         url="https://vgy.me/upload",
         data={"userkey": key},
         files={"file[]": (f"img.{ext}", img)},
     )
-    if not response.ok:
-        raise UploadError(response.json())
+    response.raise_for_status()
 
     return response.json()["image"]
 
 
-UPLOAD: dict[str, Callable[[bytes], str]] = {
+UPLOAD: dict[str, Callable] = {
     "beeimg": beeimg_upload,
     "catbox": catbox_upload,
     "fastpic": fastpic_upload,
     "filecoffee": filecoffee_upload,
     "freeimage": freeimage_upload,
     "gyazo": gyazo_upload,
     "imageban": imageban_upload,
     "imagebin": imagebin_upload,
     "imgbb": imgbb_upload,
     "imgchest": imgchest_upload,
     "imgur": imgur_upload,
     "lensdump": lensdump_upload,
-    "pictshare": pictshare_upload,
     "pixeldrain": pixeldrain_upload,
     "pixhost": pixhost_upload,
     "ptpimg": ptpimg_upload,
     "smms": smms_upload,
     "sxcu": sxcu_upload,
     "telegraph": telegraph_upload,
     "thumbsnap": thumbsnap_upload,
```

### Comparing `images_upload_cli-1.1.3a0/src/images_upload_cli/util.py` & `images_upload_cli-2.0.0a0/src/images_upload_cli/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 #!/usr/bin/env python
 """Utils."""
-from __future__ import annotations
 
 from io import BytesIO
 from os import getenv
 from pathlib import Path
 from shutil import which
 from subprocess import Popen
 
@@ -17,16 +16,16 @@
 
 
 def get_config_path() -> Path:
     """Get app config path."""
     return Path(f"{click.get_app_dir('images-upload-cli')}/.env")
 
 
-def get_env_val(key: str) -> str:
-    """Get value from env."""
+def get_env(key: str) -> str:
+    """Get environment variable or raise an error."""
     if value := getenv(key):
         return value
 
     msg = f"Please setup {key} in environment variables or in '{get_config_path()}'."
     raise GetEnvError(msg)
 
 
@@ -111,11 +110,11 @@
         optimize=True,
         progressive=True,
     )
 
     return buffer.getvalue()
 
 
-def kdialog(text_to_print: str) -> None:
-    """Kde notifications."""
-    if kdialog := which("kdialog"):
-        Popen([kdialog, "--passivepopup", text_to_print])
+def notify_send(text_to_print: str) -> None:
+    """Send desktop notifications via libnotify."""
+    if notify_send := which("notify-send"):
+        Popen([notify_send, "-a", "images-upload-cli", text_to_print])
```

### Comparing `images_upload_cli-1.1.3a0/PKG-INFO` & `images_upload_cli-2.0.0a0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 Metadata-Version: 2.1
 Name: images-upload-cli
-Version: 1.1.3a0
+Version: 2.0.0a0
 Summary: Upload images via APIs
 Home-page: https://github.com/DeadNews/images-upload-cli
 License: MIT
 Keywords: cli,imgur,image-upload,upload-images,upload-pictures
 Author: DeadNews
 Author-email: aurczpbgr@mozmail.com
-Requires-Python: >=3.8.1,<4.0.0
+Requires-Python: >=3.9,<4.0
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
+Requires-Dist: httpx (>=0.24.1,<0.25.0)
 Requires-Dist: pillow (>=9.5.0,<10.0.0)
 Requires-Dist: pyperclip (>=1.8.2,<2.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
-Requires-Dist: requests (>=2.30.0,<3.0.0)
 Project-URL: Repository, https://github.com/DeadNews/images-upload-cli
 Description-Content-Type: text/markdown
 
 # images-upload-cli
 
 > Upload images via APIs
 
 [![PyPI version](https://img.shields.io/pypi/v/images-upload-cli)](https://pypi.org/project/images-upload-cli)
 [![AUR version](https://img.shields.io/aur/version/python-images-upload-cli)](https://aur.archlinux.org/packages/python-images-upload-cli)
-[![CI/CD](https://github.com/DeadNews/images-upload-cli/actions/workflows/python-app.yml/badge.svg)](https://github.com/DeadNews/images-upload-cli/actions/workflows/python-app.yml)
+[![Main](https://github.com/DeadNews/images-upload-cli/actions/workflows/main.yml/badge.svg)](https://github.com/DeadNews/images-upload-cli/actions/workflows/main.yml)
 [![pre-commit.ci](https://results.pre-commit.ci/badge/github/DeadNews/images-upload-cli/main.svg)](https://results.pre-commit.ci/latest/github/DeadNews/images-upload-cli/main)
 [![codecov](https://codecov.io/gh/DeadNews/images-upload-cli/branch/main/graph/badge.svg?token=OCZDZIYPMC)](https://codecov.io/gh/DeadNews/images-upload-cli)
 
 ## Installation
 
 PyPI
 
@@ -61,15 +61,14 @@
 | [gyazo](https://gyazo.com/)           |      +       | `https://i.gyazo.com/{id}.png`                       |
 | [imageban](https://imageban.ru/)      |      +       | `https://i2.imageban.ru/out/2022/07/30/{id}.png`     |
 | [imagebin](https://imagebin.ca/)      |      -       | `https://ibin.co/{id}.png`                           |
 | [imgbb](https://imgbb.com/)           |      +       | `https://i.ibb.co/{id}/image.png`                    |
 | [imgchest](https://imgchest.com/)     |      +       | `https://cdn.imgchest.com/files/{id}.png`            |
 | [imgur](https://imgur.com/)           |      -       | `https://i.imgur.com/{id}.png`                       |
 | [lensdump](https://lensdump.com/)     |      +       | `https://i.lensdump.com/i/{id}.png`                  |
-| [pictshare](https://pictshare.net/)   |      -       | `https://pictshare.net/{id}.png`                     |
 | [pixeldrain](https://pixeldrain.com/) |      -       | `https://pixeldrain.com/api/file/{id}`               |
 | [pixhost](https://pixhost.to/)        |      -       | `https://img75.pixhost.to/images/69/{id}_img.png`    |
 | [ptpimg](https://ptpimg.me/)          |      +       | `https://ptpimg.me/{id}.png`                         |
 | [smms](https://sm.ms/)                |      +       | `https://s2.loli.net/2022/07/30/{id}.png`            |
 | [sxcu](https://sxcu.net/)             |      -       | `https://sxcu.net/{id}.png`                          |
 | [telegraph](https://telegra.ph/)      |      -       | `https://telegra.ph/file/{id}.png`                   |
 | [thumbsnap](https://thumbsnap.com/)   |      +       | `https://thumbsnap.com/i/{id}.png`                   |
@@ -83,18 +82,20 @@
 
 ```sh
 Usage: images-upload-cli [OPTIONS] IMAGES...
 
   Upload images via APIs.
 
 Options:
-  -h, --hosting [beeimg|catbox|fastpic|filecoffee|freeimage|gyazo|imageban|imagebin|imgbb|imgchest|imgur|lensdump|pictshare|pixeldrain|pixhost|ptpimg|smms|sxcu|telegraph|thumbsnap|tixte|up2sha|uplio|uploadcare|vgy]
+  -h, --hosting [beeimg|catbox|fastpic|filecoffee|freeimage|gyazo|imageban|imagebin|imgbb|imgchest|imgur|lensdump|pixeldrain|pixhost|ptpimg|smms|sxcu|telegraph|thumbsnap|tixte|up2sha|uplio|uploadcare|vgy]
                                   [default: imgur]
   -b, --bbcode                    Add bbcode tags.
   -t, --thumbnail                 Add caption thumbnail and bbcode tags.
+  -n, --notify / -N, --no-notify  Send desktop notifications via libnotify.
+                                  [default: N]
   -c, --clipboard / -C, --no-clipboard
                                   Copy result to clipboard.  [default: c]
   --version                       Show the version and exit.
   --help                          Show this message and exit.
 ```
 
 ## Env variables
```

