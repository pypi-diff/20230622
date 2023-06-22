# Comparing `tmp/karton_classifier-1.4.0-py3-none-any.whl.zip` & `tmp/karton_classifier-2.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 9435 bytes, number of entries: 12
--rw-r--r--  2.0 unx      539 b- defN 22-Jul-27 14:08 karton_classifier-1.4.0-nspkg.pth
--rw-r--r--  2.0 unx       61 b- defN 22-Jul-27 14:08 karton/classifier/__init__.py
--rw-r--r--  2.0 unx       54 b- defN 22-Jul-27 14:08 karton/classifier/__main__.py
--rw-r--r--  2.0 unx       22 b- defN 22-Jul-27 14:08 karton/classifier/__version__.py
--rw-r--r--  2.0 unx    21772 b- defN 22-Jul-27 14:08 karton/classifier/classifier.py
--rw-r--r--  2.0 unx     1519 b- defN 22-Jul-27 14:08 karton_classifier-1.4.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     1952 b- defN 22-Jul-27 14:08 karton_classifier-1.4.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Jul-27 14:08 karton_classifier-1.4.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       73 b- defN 22-Jul-27 14:08 karton_classifier-1.4.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        7 b- defN 22-Jul-27 14:08 karton_classifier-1.4.0.dist-info/namespace_packages.txt
--rw-r--r--  2.0 unx        7 b- defN 22-Jul-27 14:08 karton_classifier-1.4.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1083 b- defN 22-Jul-27 14:08 karton_classifier-1.4.0.dist-info/RECORD
-12 files, 27181 bytes uncompressed, 7563 bytes compressed:  72.2%
+Zip file size: 10138 bytes, number of entries: 12
+-rw-r--r--  2.0 unx      539 b- defN 23-Jun-22 10:26 karton_classifier-2.0.0-nspkg.pth
+-rw-r--r--  2.0 unx       61 b- defN 23-Jun-22 10:26 karton/classifier/__init__.py
+-rw-r--r--  2.0 unx       54 b- defN 23-Jun-22 10:26 karton/classifier/__main__.py
+-rw-r--r--  2.0 unx       22 b- defN 23-Jun-22 10:26 karton/classifier/__version__.py
+-rw-r--r--  2.0 unx    24099 b- defN 23-Jun-22 10:26 karton/classifier/classifier.py
+-rw-r--r--  2.0 unx     1519 b- defN 23-Jun-22 10:26 karton_classifier-2.0.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2393 b- defN 23-Jun-22 10:26 karton_classifier-2.0.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-22 10:26 karton_classifier-2.0.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       73 b- defN 23-Jun-22 10:26 karton_classifier-2.0.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        7 b- defN 23-Jun-22 10:26 karton_classifier-2.0.0.dist-info/namespace_packages.txt
+-rw-r--r--  2.0 unx        7 b- defN 23-Jun-22 10:26 karton_classifier-2.0.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1083 b- defN 23-Jun-22 10:26 karton_classifier-2.0.0.dist-info/RECORD
+12 files, 29949 bytes uncompressed, 8266 bytes compressed:  72.4%
```

## zipnote {}

```diff
@@ -1,37 +1,37 @@
-Filename: karton_classifier-1.4.0-nspkg.pth
+Filename: karton_classifier-2.0.0-nspkg.pth
 Comment: 
 
 Filename: karton/classifier/__init__.py
 Comment: 
 
 Filename: karton/classifier/__main__.py
 Comment: 
 
 Filename: karton/classifier/__version__.py
 Comment: 
 
 Filename: karton/classifier/classifier.py
 Comment: 
 
-Filename: karton_classifier-1.4.0.dist-info/LICENSE
+Filename: karton_classifier-2.0.0.dist-info/LICENSE
 Comment: 
 
-Filename: karton_classifier-1.4.0.dist-info/METADATA
+Filename: karton_classifier-2.0.0.dist-info/METADATA
 Comment: 
 
-Filename: karton_classifier-1.4.0.dist-info/WHEEL
+Filename: karton_classifier-2.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: karton_classifier-1.4.0.dist-info/entry_points.txt
+Filename: karton_classifier-2.0.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: karton_classifier-1.4.0.dist-info/namespace_packages.txt
+Filename: karton_classifier-2.0.0.dist-info/namespace_packages.txt
 Comment: 
 
-Filename: karton_classifier-1.4.0.dist-info/top_level.txt
+Filename: karton_classifier-2.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: karton_classifier-1.4.0.dist-info/RECORD
+Filename: karton_classifier-2.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## karton/classifier/__version__.py

```diff
@@ -1 +1 @@
-__version__ = "1.4.0"
+__version__ = "2.0.0"
```

## karton/classifier/classifier.py

```diff
@@ -34,15 +34,15 @@
 
     if classification.get("extension") is not None:
         # Add extension (if not empty)
         extension = classification["extension"]
         if extension:
             sample_type += f":{classification['extension']}"
 
-    # Add misc: if headers doesn't have platform nor extension
+    # Add misc: when header doesn't have platform nor extension
     if ":" not in sample_type:
         sample_type = f"misc:{sample_type}"
 
     return sample_type
 
 
 class Classifier(Karton):
@@ -180,14 +180,26 @@
             )
             if magic.startswith("PE32+"):
                 sample_class["platform"] = "win64"  # 64-bit only executable
             if "(DLL)" in magic:
                 sample_class["extension"] = "dll"
             return sample_class
 
+        # Is COM file?
+        if magic.startswith("COM executable for DOS"):
+            sample_class.update(
+                {"kind": "runnable", "platform": "win32", "extension": "com"}
+            )
+            return sample_class
+
+        # Is PC MBR?
+        if magic.startswith("DOS/MBR boot sector"):
+            sample_class.update({"kind": "runnable", "extension": "mbr"})
+            return sample_class
+
         # ZIP-contained files?
         def zip_has_file(path: str) -> bool:
             try:
                 ZipFile(BytesIO(content)).getinfo(path)
                 return True
             except Exception:
                 return False
@@ -228,17 +240,45 @@
         # Windows LNK?
         if magic.startswith("MS Windows shortcut") or extension == "lnk":
             sample_class.update(
                 {"kind": "runnable", "platform": "win32", "extension": "lnk"}
             )
             return sample_class
 
+        # Windows CHM?
+        if magic.startswith("MS Windows HtmlHelp Data") or extension == "chm":
+            sample_class.update(
+                {"kind": "runnable", "platform": "win32", "extension": "chm"}
+            )
+            return sample_class
+
         # Is ELF file?
+        elf_assoc = {
+            "linux": "(GNU/Linux)",
+            "freebsd": "(FreeBSD)",
+            "netbsd": "(NetBSD)",
+            "openbsd": "(SYSV)",
+            "solaris": "(Solaris)",
+        }
         if magic.startswith("ELF"):
-            sample_class.update({"kind": "runnable", "platform": "linux"})
+            for platform, platform_full in elf_assoc.items():
+                if platform_full in magic:
+                    sample_class.update(
+                        {"kind": "runnable", "platform": platform, "extension": "elf"}
+                    )
+                    return sample_class
+
+            sample_class.update({"kind": "runnable", "extension": "elf"})
+            return sample_class
+
+        # Is XCOFF64 file (for AIX)?
+        if magic.startswith("64-bit XCOFF"):
+            sample_class.update(
+                {"kind": "runnable", "platform": "aix", "extension": "xcoff"}
+            )
             return sample_class
 
         # Is PKG file?
         if magic.startswith("xar archive") or extension == "pkg":
             sample_class.update(
                 {"kind": "runnable", "platform": "macos", "extension": "pkg"}
             )
@@ -253,15 +293,15 @@
             ]
         ):
             sample_class.update(
                 {"kind": "runnable", "platform": "macos", "extension": "dmg"}
             )
             return sample_class
 
-        # Is mach-o file?
+        # Is Mach-O file?
         if magic.startswith("Mach-O"):
             sample_class.update({"kind": "runnable", "platform": "macos"})
             return sample_class
 
         def zip_has_mac_app() -> bool:
             try:
                 zipfile = ZipFile(BytesIO(content))
@@ -275,14 +315,35 @@
         # macos app within zip
         if magic.startswith("Zip archive data") and zip_has_mac_app():
             sample_class.update(
                 {"kind": "runnable", "platform": "macos", "extension": "app"}
             )
             return sample_class
 
+        # Various graphics/image file formats
+        image_assoc = {
+            "gif": ["GIF image data"],
+            "jpg": ["JPEG image data"],
+            "png": ["PNG image data"],
+        }
+
+        for ext, patterns in image_assoc.items():
+            if any(pattern in magic for pattern in patterns):
+                sample_class.update({"kind": "misc", "extension": ext})
+                return sample_class
+
+        if extension in image_assoc.keys():
+            sample_class.update({"kind": "misc", "extension": ext})
+            return sample_class
+
+        # Is Disk image?
+        if magic.startswith("Microsoft Disk Image") or extension == "vhd":
+            sample_class.update({"kind": "archive", "extension": "vhd"})
+            return sample_class
+
         # Windows scripts (per extension)
         script_extensions = [
             "vbs",
             "vbe",
             "js",
             "jse",
             "wsh",
@@ -385,48 +446,56 @@
         # PDF files
         if magic.startswith("PDF document") or extension == "pdf":
             sample_class.update(
                 {"kind": "document", "platform": "win32", "extension": "pdf"}
             )
             return sample_class
 
+        # JSON files
+        if magic == "JSON data" or magic_mime == "application/json":
+            sample_class.update({"kind": "json"})
+            return sample_class
+
         # Archives
         archive_assoc = {
             "7z": ["7-zip archive data"],
             "ace": ["ACE archive data"],
             "bz2": ["bzip2 compressed data"],
             "cab": ["Microsoft Cabinet archive data"],
+            "cpio": ["cpio archive"],
             "gz": ["gzip compressed"],
             "iso": ["ISO 9660 CD-ROM"],
             "lz": ["lzip compressed data"],
             "tar": ["tar archive", "POSIX tar archive"],
             "rar": ["RAR archive data"],
             "udf": ["UDF filesystem data"],
             "xz": ["XZ compressed data"],
             "zip": ["Zip archive data"],
             "zlib": ["zlib compressed data"],
-            "lzh": ["  LHa (2.x) archive data"],
+            "lzh": ["  LHa (2.x) archive data", "  LHa 2.x? archive data"],
         }
         archive_extensions = [
+            "7z",
             "ace",
-            "zip",
-            "rar",
-            "tar",
+            "arc",
+            "arj",
+            "bz2",
+            "cab",
             "cab",
+            "cpio",
             "gz",
-            "7z",
-            "bz2",
-            "arj",
             "iso",
-            "xz",
             "lz",
+            "lzh",
+            "rar",
+            "tar",
             "udf",
-            "cab",
+            "xz",
+            "zip",
             "zlib",
-            "lzh",
         ]
 
         def apply_archive_headers(extension):
             headers = {"kind": "archive", "extension": extension}
             if extension == "xz":
                 # libmagic >= 5.40 generates correct MIME type for XZ archives
                 headers["mime"] = "application/x-xz"
@@ -455,19 +524,30 @@
             return sample_class
 
         # HTML
         if magic.startswith("HTML document"):
             sample_class.update({"kind": "html"})
             return sample_class
 
-        # Linux scripts
-        if ("script" in magic and "executable" in magic) or extension == "sh":
-            sample_class.update(
-                {"kind": "script", "platform": "linux", "extension": extension}
-            )
+        # Various scripting languages
+        script_assoc = {
+            "php": ["PHP script"],
+            "pl": ["Perl script", "Perl5 module"],
+            "py": ["Python script"],
+            "rb": ["Ruby script"],
+            "scpt": ["AppleScript compiled"],
+            "sh": ["Bourne-Again shell", "POSIX shell"],
+        }
+        for ext, patterns in script_assoc.items():
+            if any(pattern in magic for pattern in patterns):
+                sample_class.update({"kind": "script", "extension": ext})
+                return sample_class
+
+        if extension in script_assoc.keys():
+            sample_class.update({"kind": "script", "extension": ext})
             return sample_class
 
         # Content heuristics
         partial = content[:2048] + content[-2048:]
 
         # Dumped PE file heuristics (PE not recognized by libmagic)
         if b".text" in partial and b"This program cannot be run" in partial:
@@ -488,134 +568,129 @@
             sample_class.update(
                 {"kind": "dump", "platform": "win32", "extension": "exe"}
             )
             return sample_class
 
         # Heuristics for scripts
         try:
-            try:
-                partial_str = partial.decode(
-                    chardet.detect(partial)["encoding"]
-                ).lower()
-            except Exception:
-                self.log.warning("Heuristics disabled - unknown encoding")
-            else:
-                vbs_keywords = [
-                    "end function",
-                    "end if",
-                    "array(",
-                    "sub ",
-                    "on error ",
-                    "createobject",
-                    "execute",
-                ]
-                js_keywords = [
-                    "function ",
-                    "function(",
-                    "this.",
-                    "this[",
-                    "new ",
-                    "createobject",
-                    "activexobject",
-                    "var ",
-                    "catch",
-                ]
-                html_keywords = ["<!doctype", "<html", "<script"]
-                ps_keywords = [
-                    "powershell",
-                    "-nop",
-                    "bypass",
-                    "new-object",
-                    "invoke-expression",
-                    "frombase64string(",
-                    "| iex",
-                    "|iex",
-                ]
-                if (
-                    len([True for keyword in html_keywords if keyword in partial_str])
-                    >= 2
-                ):
-                    sample_class.update({"kind": "html"})
-                    return sample_class
+            partial_str = partial.decode(chardet.detect(partial)["encoding"]).lower()
+        except Exception:
+            self.log.warning("Heuristics disabled - unknown encoding")
+            partial_str = None
+
+        if partial_str:
+            vbs_keywords = [
+                "end function",
+                "end if",
+                "array(",
+                "sub ",
+                "on error ",
+                "createobject",
+                "execute",
+            ]
+            js_keywords = [
+                "function ",
+                "function(",
+                "this.",
+                "this[",
+                "new ",
+                "createobject",
+                "activexobject",
+                "var ",
+                "catch",
+            ]
+            html_keywords = ["<!doctype", "<html", "<script"]
+            ps_keywords = [
+                "powershell",
+                "-nop",
+                "bypass",
+                "new-object",
+                "invoke-expression",
+                "frombase64string(",
+                "| iex",
+                "|iex",
+            ]
+            if len([True for keyword in html_keywords if keyword in partial_str]) >= 2:
+                sample_class.update({"kind": "html"})
+                return sample_class
 
-                if (
-                    len([True for keyword in vbs_keywords if keyword in partial_str])
-                    >= 2
-                ):
-                    sample_class.update(
-                        {"kind": "script", "platform": "win32", "extension": "vbs"}
-                    )
-                    return sample_class
-                # Powershell heuristics
-                if len(
-                    [True for keyword in ps_keywords if keyword.lower() in partial_str]
-                ):
-                    sample_class.update(
-                        {"kind": "script", "platform": "win32", "extension": "ps1"}
-                    )
-                    return sample_class
-                # JS heuristics
-                if (
-                    len([True for keyword in js_keywords if keyword in partial_str])
-                    >= 2
-                ):
-                    sample_class.update(
-                        {"kind": "script", "platform": "win32", "extension": "js"}
-                    )
-                    return sample_class
-                # JSE heuristics
-                if re.match("#@~\\^[a-zA-Z0-9+/]{6}==", partial_str):
-                    sample_class.update(
-                        {
-                            "kind": "script",
-                            "platform": "win32",
-                            "extension": "jse",  # jse is more possible than vbe
-                        }
-                    )
-                    return sample_class
-                if magic.startswith("ASCII"):
-                    sample_class.update(
-                        {
-                            "kind": "ascii",
-                        }
-                    )
-                    return sample_class
-                if magic.startswith("ISO-8859"):
-                    sample_class.update(
-                        {
-                            "kind": "iso-8859-1",
-                        }
-                    )
-                    return sample_class
-                if magic.startswith("UTF-8"):
-                    sample_class.update(
-                        {
-                            "kind": "utf-8",
-                        }
-                    )
-                    return sample_class
-                if magic.startswith("PGP"):
-                    sample_class.update(
-                        {
-                            "kind": "pgp",
-                        }
-                    )
-                    return sample_class
-                if magic.startswith("pcap capture file"):
-                    sample_class.update(
-                        {
-                            "kind": "pcap",
-                        }
-                    )
-                    return sample_class
-                if magic.startswith("pcap") and "ng capture file" in magic:
-                    sample_class.update(
-                        {
-                            "kind": "pcapng",
-                        }
-                    )
-                    return sample_class
-        except Exception as e:
-            self.log.exception(e)
+            if len([True for keyword in vbs_keywords if keyword in partial_str]) >= 2:
+                sample_class.update(
+                    {"kind": "script", "platform": "win32", "extension": "vbs"}
+                )
+                return sample_class
+            # Powershell heuristics
+            if len([True for keyword in ps_keywords if keyword.lower() in partial_str]):
+                sample_class.update(
+                    {"kind": "script", "platform": "win32", "extension": "ps1"}
+                )
+                return sample_class
+            # JS heuristics
+            if len([True for keyword in js_keywords if keyword in partial_str]) >= 2:
+                sample_class.update(
+                    {"kind": "script", "platform": "win32", "extension": "js"}
+                )
+                return sample_class
+            # JSE heuristics
+            if re.match("#@~\\^[a-zA-Z0-9+/]{6}==", partial_str):
+                sample_class.update(
+                    {
+                        "kind": "script",
+                        "platform": "win32",
+                        "extension": "jse",  # jse is more possible than vbe
+                    }
+                )
+                return sample_class
+
+        # magic of XML files: XML 1.0 document, ASCII text
+        if magic.startswith("ASCII") or magic.endswith("ASCII text"):
+            sample_class.update(
+                {
+                    "kind": "ascii",
+                }
+            )
+            return sample_class
+        if magic.startswith("CSV text"):
+            sample_class.update(
+                {
+                    "kind": "csv",
+                }
+            )
+            return sample_class
+        if magic.startswith("ISO-8859"):
+            sample_class.update(
+                {
+                    "kind": "iso-8859-1",
+                }
+            )
+            return sample_class
+        if magic.startswith("UTF-8"):
+            sample_class.update(
+                {
+                    "kind": "utf-8",
+                }
+            )
+            return sample_class
+        if magic.startswith("PGP"):
+            sample_class.update(
+                {
+                    "kind": "pgp",
+                }
+            )
+            return sample_class
+        if magic.startswith(("pcap capture file", "tcpdump capture file")):
+            sample_class.update(
+                {
+                    "kind": "pcap",
+                }
+            )
+            return sample_class
+        if magic.startswith("pcap") and "ng capture file" in magic:
+            sample_class.update(
+                {
+                    "kind": "pcapng",
+                }
+            )
+            return sample_class
 
         # If not recognized then unsupported
         return None
```

## Comparing `karton_classifier-1.4.0-nspkg.pth` & `karton_classifier-2.0.0-nspkg.pth`

 * *Files identical despite different names*

## Comparing `karton_classifier-1.4.0.dist-info/LICENSE` & `karton_classifier-2.0.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `karton_classifier-1.4.0.dist-info/METADATA` & `karton_classifier-2.0.0.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: karton-classifier
-Version: 1.4.0
+Version: 2.0.0
 Summary: File type classifier for Karton framework
 Home-page: https://github.com/CERT-Polska/karton-classifier/
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: chardet (==3.0.4)
 Requires-Dist: karton-core (<6.0.0,>=5.0.0)
 Requires-Dist: python-magic (==0.4.18)
 
 # Classifier karton service
 
 File type classifier for the Karton framework.
@@ -42,24 +43,32 @@
     "type":      "sample",
     "stage":     "recognized",
     "kind":      "runnable"  # Executable format default for OS platform
               || "document"  # Office document
               || "archive"   # Archive containing samples (zip, e-mails)
               || "dump"      # Dump from sandbox
               || "script",   # Script (js/vbs/bat...)
+              || "misc",     # No platform or extension
     "platform":  "win32" 
               || "win64" 
               || "linux" 
               || "android",
               || "macos",
+              || "freebsd",
+              || "netbsd",
+              || "openbsd",
+              || "solaris",
     "extension": "*",        # Expected file extension
+    "mime": "*",        # Expected file mimetype
     ... (other fields are derived from incoming task)
 }
 ```
 
+**Warning** the output `mime` field is not deterministic across libmagic versions and can change depending on the version you're using. We don't recommend creating consumers that listen on it directly.
+
 ## Usage
 
 First of all, make sure you have setup the core system: https://github.com/CERT-Polska/karton
 
 Then install karton-classifier from PyPi:
 
 ```shell
```

