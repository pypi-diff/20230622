# Comparing `tmp/bye_wiki-0.0.3.tar.gz` & `tmp/bye_wiki-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bye_wiki-0.0.3.tar", last modified: Thu Jun 22 14:38:34 2023, max compression
+gzip compressed data, was "bye_wiki-0.1.0.tar", last modified: Thu Jun 22 14:42:44 2023, max compression
```

## Comparing `bye_wiki-0.0.3.tar` & `bye_wiki-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 jflory   (4211080) jflory   (4211080)        0 2023-06-22 14:38:34.317362 bye_wiki-0.0.3/
--rw-rw-r--   0 jflory   (4211080) jflory   (4211080)     1528 2020-05-24 17:53:54.000000 bye_wiki-0.0.3/LICENSE.txt
--rw-rw-r--   0 jflory   (4211080) jflory   (4211080)      293 2020-05-24 17:53:54.000000 bye_wiki-0.0.3/MANIFEST.in
--rw-r--r--   0 jflory   (4211080) jflory   (4211080)     2794 2023-06-22 14:38:34.317362 bye_wiki-0.0.3/PKG-INFO
--rw-r--r--   0 jflory   (4211080) jflory   (4211080)     2143 2023-06-22 14:36:04.000000 bye_wiki-0.0.3/README.md
-drwxr-xr-x   0 jflory   (4211080) jflory   (4211080)        0 2023-06-22 14:38:34.317362 bye_wiki-0.0.3/bye_wiki/
--rw-r--r--   0 jflory   (4211080) jflory   (4211080)       22 2023-06-22 14:36:04.000000 bye_wiki-0.0.3/bye_wiki/__init__.py
--rw-r--r--   0 jflory   (4211080) jflory   (4211080)     3101 2023-06-22 14:36:04.000000 bye_wiki-0.0.3/bye_wiki/cli.py
-drwxr-xr-x   0 jflory   (4211080) jflory   (4211080)        0 2023-06-22 14:38:34.317362 bye_wiki-0.0.3/bye_wiki.egg-info/
--rw-rw-r--   0 jflory   (4211080) jflory   (4211080)     2794 2023-06-22 14:38:34.000000 bye_wiki-0.0.3/bye_wiki.egg-info/PKG-INFO
--rw-rw-r--   0 jflory   (4211080) jflory   (4211080)      283 2023-06-22 14:38:34.000000 bye_wiki-0.0.3/bye_wiki.egg-info/SOURCES.txt
--rw-rw-r--   0 jflory   (4211080) jflory   (4211080)        1 2023-06-22 14:38:34.000000 bye_wiki-0.0.3/bye_wiki.egg-info/dependency_links.txt
--rw-rw-r--   0 jflory   (4211080) jflory   (4211080)       41 2023-06-22 14:38:34.000000 bye_wiki-0.0.3/bye_wiki.egg-info/entry_points.txt
--rw-rw-r--   0 jflory   (4211080) jflory   (4211080)        1 2020-05-24 19:29:27.000000 bye_wiki-0.0.3/bye_wiki.egg-info/not-zip-safe
--rw-rw-r--   0 jflory   (4211080) jflory   (4211080)        9 2023-06-22 14:38:34.000000 bye_wiki-0.0.3/bye_wiki.egg-info/top_level.txt
--rw-r--r--   0 jflory   (4211080) jflory   (4211080)      863 2023-06-22 14:38:34.318362 bye_wiki-0.0.3/setup.cfg
--rw-rw-r--   0 jflory   (4211080) jflory   (4211080)       38 2020-05-24 17:53:54.000000 bye_wiki-0.0.3/setup.py
+drwxr-xr-x   0 jflory   (4211080) jflory   (4211080)        0 2023-06-22 14:42:44.073625 bye_wiki-0.1.0/
+-rw-rw-r--   0 jflory   (4211080) jflory   (4211080)     1528 2020-05-24 17:53:54.000000 bye_wiki-0.1.0/LICENSE.txt
+-rw-rw-r--   0 jflory   (4211080) jflory   (4211080)      293 2020-05-24 17:53:54.000000 bye_wiki-0.1.0/MANIFEST.in
+-rw-r--r--   0 jflory   (4211080) jflory   (4211080)     2966 2023-06-22 14:42:44.073625 bye_wiki-0.1.0/PKG-INFO
+-rw-r--r--   0 jflory   (4211080) jflory   (4211080)     2315 2023-06-22 14:41:59.000000 bye_wiki-0.1.0/README.md
+drwxr-xr-x   0 jflory   (4211080) jflory   (4211080)        0 2023-06-22 14:42:44.073625 bye_wiki-0.1.0/bye_wiki/
+-rw-r--r--   0 jflory   (4211080) jflory   (4211080)       22 2023-06-22 14:41:59.000000 bye_wiki-0.1.0/bye_wiki/__init__.py
+-rw-r--r--   0 jflory   (4211080) jflory   (4211080)     4024 2023-06-22 14:41:59.000000 bye_wiki-0.1.0/bye_wiki/cli.py
+drwxr-xr-x   0 jflory   (4211080) jflory   (4211080)        0 2023-06-22 14:42:44.073625 bye_wiki-0.1.0/bye_wiki.egg-info/
+-rw-r--r--   0 jflory   (4211080) jflory   (4211080)     2966 2023-06-22 14:42:44.000000 bye_wiki-0.1.0/bye_wiki.egg-info/PKG-INFO
+-rw-r--r--   0 jflory   (4211080) jflory   (4211080)      283 2023-06-22 14:42:44.000000 bye_wiki-0.1.0/bye_wiki.egg-info/SOURCES.txt
+-rw-r--r--   0 jflory   (4211080) jflory   (4211080)        1 2023-06-22 14:42:44.000000 bye_wiki-0.1.0/bye_wiki.egg-info/dependency_links.txt
+-rw-r--r--   0 jflory   (4211080) jflory   (4211080)       41 2023-06-22 14:42:44.000000 bye_wiki-0.1.0/bye_wiki.egg-info/entry_points.txt
+-rw-r--r--   0 jflory   (4211080) jflory   (4211080)        1 2023-06-22 14:42:43.000000 bye_wiki-0.1.0/bye_wiki.egg-info/not-zip-safe
+-rw-r--r--   0 jflory   (4211080) jflory   (4211080)        9 2023-06-22 14:42:44.000000 bye_wiki-0.1.0/bye_wiki.egg-info/top_level.txt
+-rw-r--r--   0 jflory   (4211080) jflory   (4211080)      863 2023-06-22 14:42:44.074625 bye_wiki-0.1.0/setup.cfg
+-rw-rw-r--   0 jflory   (4211080) jflory   (4211080)       38 2020-05-24 17:53:54.000000 bye_wiki-0.1.0/setup.py
```

### Comparing `bye_wiki-0.0.3/LICENSE.txt` & `bye_wiki-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bye_wiki-0.0.3/PKG-INFO` & `bye_wiki-0.1.0/bye_wiki.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: bye_wiki
-Version: 0.0.3
+Name: bye-wiki
+Version: 0.1.0
 Summary: Say goodbye to your wikis! Python command-line script to convert MediaWiki pages to other formats with pandoc
 Home-page: https://github.com/jwflory/bw
 Author: Justin W. Flory
 Author-email: contact@jwf.io
 License: BSD-3-Clause
 Keywords: asciidoc,data,wiki,mediawiki,markdown,documentation,migration,pandoc
 Classifier: License :: OSI Approved :: BSD License
@@ -17,35 +17,35 @@
 
 bye_wiki (bw)
 =============
 
 [![License: BSD 3-Clause License][1]][2]
 
 Say goodbye to your wikis!
-Python command-line tool to convert MediaWiki pages to Markdown with pandoc
+Python command-line wrapper to convert MediaWiki pages to other formats with `pandoc`
 
 
 ## About
 
-bye_wiki (`bw`) is a Python command-line script to convert MediaWiki pages into Markdown.
+bye_wiki (`bw`) is a Python command-line script to convert MediaWiki pages into other formats like AsciiDoc and Markdown.
 
-This makes migrating documentation and pages from a MediaWiki server to somewhere else.
-Regardless of whatever "somewhere else" means for you, this tool provides a basic Markdown conversion for you to work with in a new platform.
+This makes it easier to migrate documentation and wiki pages from a MediaWiki server to somewhere else.
+Regardless of whatever "somewhere else" means for you, this tool provides a basic conversion for you to work with the information from a new format.
 bye_wiki is more or less a fancy wrapper for `requests` and `pandoc`.
 
 
 ## How to use
 
 **NOTE**:
 You must already have [pandoc][3] installed on your system for this script to work!
 
 Once you have `pandoc`, the easiest way to get started with bye_wiki is to install from PyPI:
 
 ```sh
-pip3 install --user bye-wiki
+pip install --user bye-wiki
 ```
 
 The CLI `--help` menu provides more detailed information about how to use bye_wiki.
 Some examples are below:
 
 ### Example 1
 
@@ -53,31 +53,31 @@
 
 ```sh
 bw --title "El Ten Eleven" --out ~/ete.md
 ```
 
 ### Example 2
 
-Convert _Licensing:Main_ from the [Fedora Project][4] MediaWiki to a Markdown document.
+Convert _Fedora_Linux_38_Release_Party_Schedule_ from the [Fedora Project][4] MediaWiki to an AsciiDoc document.
 
 ```sh
-bw --url fedoraproject.org/w --title "Licensing:Main" --out licensing.md
+bw --url fedoraproject.org/w --format asciidoc --title "Fedora_Linux_38_Release_Party_Schedule" --out licensing.adoc
 ```
 
 ### Example 3
 
-Convert _MusicBrainz Principles_ from the [MusicBrainz][5] MediaWiki to a Markdown document, with the `--atx` flag removed from `pandoc`:
+Convert _MusicBrainz Principles_ from the [MusicBrainz][5] MediaWiki to a Markdown document, with the `--markdown-headings=atx` flag excluded from the `pandoc` command:
 
 ```sh
 bw --url wiki.musicbrainz.org --title MusicBrainz_Principles --out mb-principles.md --atx-off
 ```
 
-Hint:
-If you aren't sure if you want `--atx-off` or not, you do not.
-It is an opinionated format for converting documents but some writers may prefer to not have ATX-style headers.
+_Hint_:
+If you are not sure whether you want `--atx-off` or not, you do not.
+ATX is the more popular format for Markdown documents, but some writers may prefer to not have ATX-style headers.
 
 
 ## How to contribute
 
 See [CONTRIBUTING.md][6].
 
 
@@ -86,8 +86,8 @@
 Licensed under [BSD 3-Clause License][2].
 
 [1]: https://img.shields.io/badge/License-BSD%203--Clause-blue.svg
 [2]: https://opensource.org/licenses/BSD-3-Clause "BSD-3-Clause License - opensource.org"
 [3]: https://pandoc.org/
 [4]: https://getfedora.org
 [5]: https://musicbrainz.org
-[6]: https://github.com/jwflory/bw/blob/master/.github/CONTRIBUTING.md "How to contribute to the project"
+[6]: https://github.com/jwflory/bw/blob/main/.github/CONTRIBUTING.md "How to contribute to the project"
```

### Comparing `bye_wiki-0.0.3/bye_wiki/cli.py` & `bye_wiki-0.1.0/bye_wiki/cli.py`

 * *Files 17% similar despite different names*

```diff
@@ -25,14 +25,28 @@
 
 def clean_request_data(payload) -> str:
     """Clean up request made to MediaWiki API to return raw MediaWiki text."""
     page_id = list(payload.keys())[0]
     return payload[page_id]["revisions"][0]["*"]
 
 
+def convert_mediawiki_to_asciidoc(mw_content: str) -> str:
+    """Use pandoc via subprocess to convert temp. file to AsciiDoc raw text."""
+    pandoc_str = ["pandoc", "--from", "mediawiki", "--to", "asciidoc"]
+
+    mediawiki_doc = subprocess.Popen(
+        ("echo", mw_content),
+        stdout=subprocess.PIPE,
+    )
+    return str(
+        subprocess.check_output(pandoc_str, stdin=mediawiki_doc.stdout),
+        "utf-8",
+    )
+
+
 def convert_mediawiki_to_markdown(mw_content: str, atx_off: bool) -> str:
     """Use pandoc via subprocess to convert temp. file to Markdown raw text."""
     pandoc_str = ["pandoc", "--from", "mediawiki", "--to", "markdown"]
     if atx_off is False:
         pandoc_str.append("--markdown-headings=atx")
 
     mediawiki_doc = subprocess.Popen(
@@ -41,33 +55,41 @@
     )
     return str(
         subprocess.check_output(pandoc_str, stdin=mediawiki_doc.stdout),
         "utf-8",
     )
 
 
-def save_file(out_path: str, markdown_doc: str):
-    """Save Markdown text to specified file path."""
+def save_file(out_path: str, converted_doc: str):
+    """Save converted text file to the specified file path."""
     with open(out_path, "w") as file:
-        file.write(str(markdown_doc))
+        file.write(str(converted_doc))
 
 
 def main():
     # Create main parser and subparser
     parser = argparse.ArgumentParser(
-        description="Convert MediaWiki pages to Markdown."
+        description="Convert MediaWiki pages to other formats."
     )
 
     parser.add_argument(
         "--atx-off",
         default=False,
         help="(Markdown only) Do not convert with Pandoc --markdown-headings=atx flag",
         action="store_true",
     )
     parser.add_argument(
+        "-f",
+        "--format",
+        default="markdown",
+        help="Format of saved text file: asciidoc, markdown (default: markdown)",
+        metavar="FORMAT",
+        type=str,
+    )
+    parser.add_argument(
         "-i",
         "--insecure",
         default=False,
         help="Use for http:// MediaWiki sites only (defaults to https://)",
         action="store_true",
     )
     parser.add_argument(
@@ -97,13 +119,20 @@
     parser.add_argument(
         "--version", action="version", version="%(prog)s " + __version__
     )
     args = parser.parse_args()
 
     raw_mw_content = get_mediawiki_content(args.insecure, args.url, args.title)
     mw_content = clean_request_data(raw_mw_content)
-    md_doc = convert_mediawiki_to_markdown(mw_content, args.atx_off)
-    save_file(args.out, md_doc)
+
+    if args.format == "asciidoc":
+        adoc_file = convert_mediawiki_to_asciidoc(mw_content)
+        save_file(args.out, adoc_file)
+    elif args.format == "markdown":
+        md_doc = convert_mediawiki_to_markdown(mw_content, args.atx_off)
+        save_file(args.out, md_doc)
+    else:
+        raise RuntimeError("An invalid export format was given.")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `bye_wiki-0.0.3/bye_wiki.egg-info/PKG-INFO` & `bye_wiki-0.1.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: bye-wiki
-Version: 0.0.3
+Name: bye_wiki
+Version: 0.1.0
 Summary: Say goodbye to your wikis! Python command-line script to convert MediaWiki pages to other formats with pandoc
 Home-page: https://github.com/jwflory/bw
 Author: Justin W. Flory
 Author-email: contact@jwf.io
 License: BSD-3-Clause
 Keywords: asciidoc,data,wiki,mediawiki,markdown,documentation,migration,pandoc
 Classifier: License :: OSI Approved :: BSD License
@@ -17,35 +17,35 @@
 
 bye_wiki (bw)
 =============
 
 [![License: BSD 3-Clause License][1]][2]
 
 Say goodbye to your wikis!
-Python command-line tool to convert MediaWiki pages to Markdown with pandoc
+Python command-line wrapper to convert MediaWiki pages to other formats with `pandoc`
 
 
 ## About
 
-bye_wiki (`bw`) is a Python command-line script to convert MediaWiki pages into Markdown.
+bye_wiki (`bw`) is a Python command-line script to convert MediaWiki pages into other formats like AsciiDoc and Markdown.
 
-This makes migrating documentation and pages from a MediaWiki server to somewhere else.
-Regardless of whatever "somewhere else" means for you, this tool provides a basic Markdown conversion for you to work with in a new platform.
+This makes it easier to migrate documentation and wiki pages from a MediaWiki server to somewhere else.
+Regardless of whatever "somewhere else" means for you, this tool provides a basic conversion for you to work with the information from a new format.
 bye_wiki is more or less a fancy wrapper for `requests` and `pandoc`.
 
 
 ## How to use
 
 **NOTE**:
 You must already have [pandoc][3] installed on your system for this script to work!
 
 Once you have `pandoc`, the easiest way to get started with bye_wiki is to install from PyPI:
 
 ```sh
-pip3 install --user bye-wiki
+pip install --user bye-wiki
 ```
 
 The CLI `--help` menu provides more detailed information about how to use bye_wiki.
 Some examples are below:
 
 ### Example 1
 
@@ -53,31 +53,31 @@
 
 ```sh
 bw --title "El Ten Eleven" --out ~/ete.md
 ```
 
 ### Example 2
 
-Convert _Licensing:Main_ from the [Fedora Project][4] MediaWiki to a Markdown document.
+Convert _Fedora_Linux_38_Release_Party_Schedule_ from the [Fedora Project][4] MediaWiki to an AsciiDoc document.
 
 ```sh
-bw --url fedoraproject.org/w --title "Licensing:Main" --out licensing.md
+bw --url fedoraproject.org/w --format asciidoc --title "Fedora_Linux_38_Release_Party_Schedule" --out licensing.adoc
 ```
 
 ### Example 3
 
-Convert _MusicBrainz Principles_ from the [MusicBrainz][5] MediaWiki to a Markdown document, with the `--atx` flag removed from `pandoc`:
+Convert _MusicBrainz Principles_ from the [MusicBrainz][5] MediaWiki to a Markdown document, with the `--markdown-headings=atx` flag excluded from the `pandoc` command:
 
 ```sh
 bw --url wiki.musicbrainz.org --title MusicBrainz_Principles --out mb-principles.md --atx-off
 ```
 
-Hint:
-If you aren't sure if you want `--atx-off` or not, you do not.
-It is an opinionated format for converting documents but some writers may prefer to not have ATX-style headers.
+_Hint_:
+If you are not sure whether you want `--atx-off` or not, you do not.
+ATX is the more popular format for Markdown documents, but some writers may prefer to not have ATX-style headers.
 
 
 ## How to contribute
 
 See [CONTRIBUTING.md][6].
 
 
@@ -86,8 +86,8 @@
 Licensed under [BSD 3-Clause License][2].
 
 [1]: https://img.shields.io/badge/License-BSD%203--Clause-blue.svg
 [2]: https://opensource.org/licenses/BSD-3-Clause "BSD-3-Clause License - opensource.org"
 [3]: https://pandoc.org/
 [4]: https://getfedora.org
 [5]: https://musicbrainz.org
-[6]: https://github.com/jwflory/bw/blob/master/.github/CONTRIBUTING.md "How to contribute to the project"
+[6]: https://github.com/jwflory/bw/blob/main/.github/CONTRIBUTING.md "How to contribute to the project"
```

### Comparing `bye_wiki-0.0.3/setup.cfg` & `bye_wiki-0.1.0/setup.cfg`

 * *Files identical despite different names*

