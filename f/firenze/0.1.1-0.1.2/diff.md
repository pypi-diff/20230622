# Comparing `tmp/firenze-0.1.1.tar.gz` & `tmp/firenze-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "firenze-0.1.1.tar", max compression
+gzip compressed data, was "firenze-0.1.2.tar", max compression
```

## Comparing `firenze-0.1.1.tar` & `firenze-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1089 2023-06-20 22:32:23.212365 firenze-0.1.1/LICENSE.md
--rw-r--r--   0        0        0     1362 2023-06-20 23:51:36.311324 firenze-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-04-30 17:30:18.195622 firenze-0.1.1/firenze/__init__.py
--rw-r--r--   0        0        0     1148 2023-06-20 22:31:35.520481 firenze-0.1.1/firenze/cli.py
--rw-r--r--   0        0        0       51 2023-06-18 00:25:42.769340 firenze-0.1.1/firenze/exceptions.py
--rw-r--r--   0        0        0     3935 2023-06-20 23:15:00.821191 firenze-0.1.1/firenze/notebook.py
--rw-r--r--   0        0        0      812 2023-06-20 23:53:14.787071 firenze-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2278 1970-01-01 00:00:00.000000 firenze-0.1.1/setup.py
--rw-r--r--   0        0        0     2098 1970-01-01 00:00:00.000000 firenze-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1089 2023-06-21 14:33:40.045938 firenze-0.1.2/LICENSE.md
+-rw-r--r--   0        0        0     1362 2023-06-21 14:33:40.045938 firenze-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-06-21 14:33:40.045938 firenze-0.1.2/firenze/__init__.py
+-rw-r--r--   0        0        0     1343 2023-06-21 14:57:04.808324 firenze-0.1.2/firenze/cli.py
+-rw-r--r--   0        0        0       51 2023-06-21 14:33:40.045938 firenze-0.1.2/firenze/exceptions.py
+-rw-r--r--   0        0        0     4151 2023-06-21 15:41:47.999876 firenze-0.1.2/firenze/notebook.py
+-rw-r--r--   0        0        0      923 2023-06-22 18:08:10.471934 firenze-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2312 1970-01-01 00:00:00.000000 firenze-0.1.2/setup.py
+-rw-r--r--   0        0        0     2239 1970-01-01 00:00:00.000000 firenze-0.1.2/PKG-INFO
```

### Comparing `firenze-0.1.1/LICENSE.md` & `firenze-0.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `firenze-0.1.1/README.md` & `firenze-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `firenze-0.1.1/firenze/cli.py` & `firenze-0.1.2/firenze/cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,17 +2,23 @@
 import json
 
 import click
 
 from firenze.exceptions import VariableAssignmentError
 from firenze.notebook import Notebook
 
+# a bit hacky
+class PathOrS3(click.Path):
+    def convert(self, value, param, ctx):
+        if value.startswith('s3://'):
+            return value
+        return super().convert(value, param, ctx)
 
 @click.command()
-@click.argument("notebook-path", type=click.Path(exists=True))
+@click.argument("notebook-path", type=PathOrS3(exists=True))
 @click.option("--output-html-path", type=click.Path(), default="output.html")
 @click.argument("parameters", nargs=-1)
 def execute_notebook(notebook_path, output_html_path, parameters):
     parsed_options = parse_options(parameters)
     notebook = Notebook.from_path(notebook_path)
     notebook.clean()
     should_print = True
```

### Comparing `firenze-0.1.1/firenze/notebook.py` & `firenze-0.1.2/firenze/notebook.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,14 +49,20 @@
             try:
                 del cell["execution_count"]
             except KeyError:
                 pass
 
     @classmethod
     def from_path(cls, notebook_path, client: Optional[NotebookClient] = None):
+        if str(notebook_path).startswith("s3://"):
+            return cls.from_s3(notebook_path)
+        return cls.from_local(client, notebook_path)
+
+    @classmethod
+    def from_local(cls, client, notebook_path):
         with open(notebook_path) as f:
             jupyter_notebook = nbformat.read(f, as_version=4)
         return cls(jupyter_notebook, client)
 
     def get_first_assignment_of_variable(self, variable_name: str):
         for cell in self.code_cells:
             tree = ast.parse(cell["source"])
```

### Comparing `firenze-0.1.1/setup.py` & `firenze-0.1.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,22 +16,22 @@
  'nbformat>=5.8.0,<6.0.0']
 
 entry_points = \
 {'console_scripts': ['firenze = firenze.cli:execute_notebook']}
 
 setup_kwargs = {
     'name': 'firenze',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': 'A lean executor for jupyter notebooks.',
     'long_description': '# Firenze\n\nFirenze is a lean jupyter notebook executor, that generates the notebook output in a single HTML\nfile. You can also parameterize the notebooks without any modification to the notebook itself.\nIt supports local files and `s3` paths, both for the notebook and for the output.\n\n## As a Library\nYou can use `firenze` as a library in your own project. Install it through `pip`\n\n```bash\npip install firenze\n```\n\nSuppose you have a very simple notebook that runs a "Hello, World!"\n\n![A notebook in jupyter](https://github.com/pabloalcain/firenze/blob/main/docs/img/hello_world_in_jupyter.png?raw=true)\n\nYou can execute it right away with `firenze` through\n```bash\nfirenze docs/notebooks/hello_world.ipynb\n```\nand the output html will be, as expected:\n\n![Hello, World! output](https://github.com/pabloalcain/firenze/blob/main/docs/img/hello_world_output.png?raw=true)\n\nYou can also send parameters and `firenze` will automatically modify the variable:\n\n```bash\nfirenze docs/notebooks/hello_world.ipynb name=Firenze\n```\n\n![Hello, Firenze! output](https://github.com/pabloalcain/firenze/blob/main/docs/img/hello_world_with_parameters.png?raw=true)\n\n## As a Docker Image\nThis is still in the making, but one idea is to call `firenze` as a docker image with a notebook\nand a `requirements.txt`, so the notebook execution can be easily deployed to remote servers.\n',
     'author': 'Pablo Alcain',
     'author_email': 'pabloalcain@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
-    'url': 'None',
+    'url': 'https://github.com/pabloalcain/firenze',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
     'python_requires': '>=3.9,<4.0',
 }
```

### Comparing `firenze-0.1.1/PKG-INFO` & `firenze-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 Metadata-Version: 2.1
 Name: firenze
-Version: 0.1.1
+Version: 0.1.2
 Summary: A lean executor for jupyter notebooks.
+Home-page: https://github.com/pabloalcain/firenze
 License: MIT
+Keywords: jupyter,notebook
 Author: Pablo Alcain
 Author-email: pabloalcain@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: boto3 (>=1.26.156,<2.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: ipykernel (>=6.22.0,<7.0.0)
 Requires-Dist: nbclient (>=0.7.4,<0.8.0)
 Requires-Dist: nbconvert (>=7.3.1,<8.0.0)
 Requires-Dist: nbformat (>=5.8.0,<6.0.0)
+Project-URL: Repository, https://github.com/pabloalcain/firenze
 Description-Content-Type: text/markdown
 
 # Firenze
 
 Firenze is a lean jupyter notebook executor, that generates the notebook output in a single HTML
 file. You can also parameterize the notebooks without any modification to the notebook itself.
 It supports local files and `s3` paths, both for the notebook and for the output.
```

