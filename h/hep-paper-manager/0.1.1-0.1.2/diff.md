# Comparing `tmp/hep_paper_manager-0.1.1.tar.gz` & `tmp/hep_paper_manager-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hep_paper_manager-0.1.1.tar", max compression
+gzip compressed data, was "hep_paper_manager-0.1.2.tar", max compression
```

## Comparing `hep_paper_manager-0.1.1.tar` & `hep_paper_manager-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     3413 2023-06-18 14:30:01.910184 hep_paper_manager-0.1.1/README.md
--rw-r--r--   0        0        0      366 2023-06-14 06:58:09.956795 hep_paper_manager-0.1.1/hpm/__init__.py
--rw-r--r--   0        0        0     5212 2023-06-18 11:14:15.458279 hep_paper_manager-0.1.1/hpm/cli.py
--rw-r--r--   0        0        0       29 2023-06-13 04:12:40.062240 hep_paper_manager-0.1.1/hpm/engines/__init__.py
--rw-r--r--   0        0        0     3298 2023-06-13 13:22:03.054110 hep_paper_manager-0.1.1/hpm/engines/inspire.py
--rw-r--r--   0        0        0       27 2023-06-13 04:13:59.907266 hep_paper_manager-0.1.1/hpm/notion/__init__.py
--rw-r--r--   0        0        0     3427 2023-06-18 11:18:06.400535 hep_paper_manager-0.1.1/hpm/notion/client.py
--rw-r--r--   0        0        0       54 2023-06-13 04:13:42.598101 hep_paper_manager-0.1.1/hpm/notion/objects/__init__.py
--rw-r--r--   0        0        0      962 2023-06-13 04:13:47.941688 hep_paper_manager-0.1.1/hpm/notion/objects/database.py
--rw-r--r--   0        0        0     3682 2023-06-13 04:13:54.692063 hep_paper_manager-0.1.1/hpm/notion/objects/page.py
--rw-r--r--   0        0        0     5166 2023-06-18 11:18:06.402552 hep_paper_manager-0.1.1/hpm/notion/properties.py
--rw-r--r--   0        0        0      170 2023-06-14 06:27:04.634648 hep_paper_manager-0.1.1/hpm/templates/paper.yml
--rw-r--r--   0        0        0      698 2023-06-18 14:30:01.910522 hep_paper_manager-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     4062 1970-01-01 00:00:00.000000 hep_paper_manager-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     3614 2023-06-22 06:48:46.781243 hep_paper_manager-0.1.2/README.md
+-rw-r--r--   0        0        0      366 2023-06-22 06:43:44.212689 hep_paper_manager-0.1.2/hpm/__init__.py
+-rw-r--r--   0        0        0     5434 2023-06-22 06:34:34.711658 hep_paper_manager-0.1.2/hpm/cli.py
+-rw-r--r--   0        0        0       29 2023-06-13 04:12:40.062240 hep_paper_manager-0.1.2/hpm/engines/__init__.py
+-rw-r--r--   0        0        0     3648 2023-06-22 06:02:12.027147 hep_paper_manager-0.1.2/hpm/engines/inspire.py
+-rw-r--r--   0        0        0       27 2023-06-13 04:13:59.907266 hep_paper_manager-0.1.2/hpm/notion/__init__.py
+-rw-r--r--   0        0        0     3427 2023-06-18 11:18:06.400535 hep_paper_manager-0.1.2/hpm/notion/client.py
+-rw-r--r--   0        0        0       54 2023-06-13 04:13:42.598101 hep_paper_manager-0.1.2/hpm/notion/objects/__init__.py
+-rw-r--r--   0        0        0      962 2023-06-13 04:13:47.941688 hep_paper_manager-0.1.2/hpm/notion/objects/database.py
+-rw-r--r--   0        0        0     3682 2023-06-13 04:13:54.692063 hep_paper_manager-0.1.2/hpm/notion/objects/page.py
+-rw-r--r--   0        0        0     5166 2023-06-18 11:18:06.402552 hep_paper_manager-0.1.2/hpm/notion/properties.py
+-rw-r--r--   0        0        0      215 2023-06-22 06:12:46.868533 hep_paper_manager-0.1.2/hpm/templates/paper.yml
+-rw-r--r--   0        0        0      698 2023-06-22 06:43:54.226477 hep_paper_manager-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4263 1970-01-01 00:00:00.000000 hep_paper_manager-0.1.2/PKG-INFO
```

### Comparing `hep_paper_manager-0.1.1/README.md` & `hep_paper_manager-0.1.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -31,14 +31,17 @@
    ```
    Arxiv ID: Text
    Citations: Number
    Title: Title
    Journal: Select
    Authors: Multi-select
    Abstract: Text
+   URL: URL
+   Bibtex: Text
+   Source: Select
    ```
    ![database](https://imgur.com/L3pJk1h.png)
    Tip: Consider adding Authors as a Relation property. This allows you to concentrate on specific authors or professors of interest. Just add the integration to the related professors' database. hpm will locate authors based on the page Title property in the related database and fetched names.
 
 2. Then set up `hpm` with `hpm init`:
    ![hpm init](https://imgur.com/282SiHF.png)
 
@@ -52,29 +55,34 @@
   ![hpm add](https://imgur.com/ycWCn3Y.png)
    The database in Notion should now look like the following:
   ![database](https://imgur.com/9U2jdSi.png)
 
 ## Engines
 - `Inspire`: It fetches papers from the [Inspire HEP](https://inspirehep.net/). It serves the default engine for `hpm`.
   - Parameters: `arxiv_id`
-  - Returns: `Paper(title, authors, abstract, journal, citations)`
+  - Returns: `Paper(title, authors, abstract, journal, citations, url, bibtex, source)`
 
 ## Templates
 You can adjust the properties within the template. On the left is the returned value from the engine and on the right is the property name in the Notion database.
 - `paper.yml`
   ```yaml
   engine: Inspire
   database: <database_id>
   properties:
     arxiv_id: Arxiv ID
     citations: Citations
     title: Title
     journal: Journal
     authors: Authors
     abstract: Abstract
+    url: URL
+    bibtex: Bibtex
+    source: Source
   ```
 
 ## Updates
+### v0.1.2
+- Update paper from Inspire engine to include url, bibtex, and source. 
 ### v0.1.1
 - Add `hpm init` for interactive setup.
 - Add `hpm add` for adding a paper to a Notion database.
 - Introduce the default `Inspire` engine and `paper.yml` template.
```

### Comparing `hep_paper_manager-0.1.1/hpm/cli.py` & `hep_paper_manager-0.1.2/hpm/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,34 +20,33 @@
     context_settings={"help_option_names": ["-h", "--help"]},
     add_completion=False,
 )
 
 
 @app.command(help="Initialize hpm with the Notion API token")
 def init():
-    print("=== Default directories ===")
-    print(f"App directory: {APP_DIR}")
-    print(f"Template directory: {TEMPLATE_DIR}")
-    print(f"Cache directory: {CACHE_DIR}")
-
-    print()
-    print(f"Welcome to {__app_name__}! Before we start, we need to set up some things.")
-    token = typer.prompt("- token", hide_input=True)
+    print("Welcome to the HEP Paper Manager!\n")
+    print("Before we start, let's set up a few necessary configurations.\n")
+    token = typer.prompt("Enter your Notion API token", hide_input=True)
     token_file = APP_DIR / "auth.yml"
     with open(token_file, "w") as f:
         yaml.dump({"token": token}, f)
-    print(f"Token saved in {token_file}")
+    print(f"[green]Your token has been saved in {token_file}\n")
 
-    use_template = typer.confirm("- Use the default paper template?")
+    use_template = typer.confirm("Would you like to use the default paper template?", default=True)
     if use_template:
         paper_template = Path(__file__).parent / "templates/paper.yml"
         shutil.copy(paper_template, TEMPLATE_DIR)
-        print("Remember to add a database id to the template before using hpm!")
+        print(f"[green]The default template has been saved in {TEMPLATE_DIR}/paper.yml")
+        print("[yellow]Remember to add a database id to the template before using hpm!\n")
 
-    print("Done!")
+    print("Configuration complete! Here are directories that hpm will use:")
+    print(f"1. App directory: {APP_DIR}")
+    print(f"2. Template directory: {TEMPLATE_DIR}")
+    print(f"3. Cache directory: {CACHE_DIR}")
 
 
 @app.command(help="Add a new page to a database")
 def add(template: str, parameters: str):
     token_file = APP_DIR / "auth.yml"
     with open(token_file, "r") as f:
         token = yaml.safe_load(f)["token"]
```

### Comparing `hep_paper_manager-0.1.1/hpm/engines/inspire.py` & `hep_paper_manager-0.1.2/hpm/engines/inspire.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,17 @@
 class Paper:
     arxiv_id: str
     title: str
     authors: list[str]
     journal: str
     citations: int
     abstract: str
+    url: str
+    bibtex: str
+    source: str
 
     @classmethod
     def from_dict(cls, contents: dict):
         metadata = contents["metadata"]
         title = metadata["titles"][-1]["title"]
 
         authors = []
@@ -49,21 +52,30 @@
                             journal = conf_metadata["acronyms"][0]
                         else:
                             journal = conf_metadata["titles"][0]["title"]
                         break
 
         citations = metadata["citation_count"]
         abstract = metadata["abstracts"][-1]["value"]
+        url = f"https://inspirehep.net/literature/{metadata['control_number']}"
+
+        bibtex_link = contents["links"]["bibtex"]
+        bibtex_response = requests.get(bibtex_link)
+        bibtex = bibtex_response.text[:-1]
+
         return Paper(
             arxiv_id=contents["id"],
             title=title,
             authors=authors,
             journal=journal,
             citations=citations,
             abstract=abstract,
+            url=url,
+            bibtex=bibtex,
+            source="Inspire",
         )
 
 
 class Inspire:
     def __init__(self):
         self.api = "https://inspirehep.net/api/arxiv/"
```

### Comparing `hep_paper_manager-0.1.1/hpm/notion/client.py` & `hep_paper_manager-0.1.2/hpm/notion/client.py`

 * *Files identical despite different names*

### Comparing `hep_paper_manager-0.1.1/hpm/notion/objects/database.py` & `hep_paper_manager-0.1.2/hpm/notion/objects/database.py`

 * *Files identical despite different names*

### Comparing `hep_paper_manager-0.1.1/hpm/notion/objects/page.py` & `hep_paper_manager-0.1.2/hpm/notion/objects/page.py`

 * *Files identical despite different names*

### Comparing `hep_paper_manager-0.1.1/hpm/notion/properties.py` & `hep_paper_manager-0.1.2/hpm/notion/properties.py`

 * *Files identical despite different names*

### Comparing `hep_paper_manager-0.1.1/pyproject.toml` & `hep_paper_manager-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hep-paper-manager"
-version = "0.1.1"
+version = "0.1.2"
 description = "HPM is a command-line tool that adds High Energy Physics (HEP) papers to a Notion database."
 authors = ["Star9daisy <star9daisy@outlook.com>"]
 readme = "README.md"
 packages = [
     { include = "hpm" },
 ]
```

### Comparing `hep_paper_manager-0.1.1/PKG-INFO` & `hep_paper_manager-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hep-paper-manager
-Version: 0.1.1
+Version: 0.1.2
 Summary: HPM is a command-line tool that adds High Energy Physics (HEP) papers to a Notion database.
 Author: Star9daisy
 Author-email: star9daisy@outlook.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -48,14 +48,17 @@
    ```
    Arxiv ID: Text
    Citations: Number
    Title: Title
    Journal: Select
    Authors: Multi-select
    Abstract: Text
+   URL: URL
+   Bibtex: Text
+   Source: Select
    ```
    ![database](https://imgur.com/L3pJk1h.png)
    Tip: Consider adding Authors as a Relation property. This allows you to concentrate on specific authors or professors of interest. Just add the integration to the related professors' database. hpm will locate authors based on the page Title property in the related database and fetched names.
 
 2. Then set up `hpm` with `hpm init`:
    ![hpm init](https://imgur.com/282SiHF.png)
 
@@ -69,29 +72,34 @@
   ![hpm add](https://imgur.com/ycWCn3Y.png)
    The database in Notion should now look like the following:
   ![database](https://imgur.com/9U2jdSi.png)
 
 ## Engines
 - `Inspire`: It fetches papers from the [Inspire HEP](https://inspirehep.net/). It serves the default engine for `hpm`.
   - Parameters: `arxiv_id`
-  - Returns: `Paper(title, authors, abstract, journal, citations)`
+  - Returns: `Paper(title, authors, abstract, journal, citations, url, bibtex, source)`
 
 ## Templates
 You can adjust the properties within the template. On the left is the returned value from the engine and on the right is the property name in the Notion database.
 - `paper.yml`
   ```yaml
   engine: Inspire
   database: <database_id>
   properties:
     arxiv_id: Arxiv ID
     citations: Citations
     title: Title
     journal: Journal
     authors: Authors
     abstract: Abstract
+    url: URL
+    bibtex: Bibtex
+    source: Source
   ```
 
 ## Updates
+### v0.1.2
+- Update paper from Inspire engine to include url, bibtex, and source. 
 ### v0.1.1
 - Add `hpm init` for interactive setup.
 - Add `hpm add` for adding a paper to a Notion database.
 - Introduce the default `Inspire` engine and `paper.yml` template.
```

