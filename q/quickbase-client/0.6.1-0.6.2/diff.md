# Comparing `tmp/quickbase-client-0.6.1.tar.gz` & `tmp/quickbase-client-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickbase-client-0.6.1.tar", max compression
+gzip compressed data, was "quickbase-client-0.6.2.tar", max compression
```

## Comparing `quickbase-client-0.6.1.tar` & `quickbase-client-0.6.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     1084 2022-04-09 23:52:19.129891 quickbase-client-0.6.1/LICENSE.md
--rw-r--r--   0        0        0     6690 2022-04-14 20:18:06.991241 quickbase-client-0.6.1/README.rst
--rw-r--r--   0        0        0     1624 2022-12-20 18:36:57.377144 quickbase-client-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     1805 2022-04-14 20:04:35.434682 quickbase-client-0.6.1/src/quickbase_client/__init__.py
--rw-r--r--   0        0        0      326 2022-04-09 23:52:19.134446 quickbase-client-0.6.1/src/quickbase_client/__version__.py
--rw-r--r--   0        0        0      154 2022-04-14 17:25:06.605131 quickbase-client-0.6.1/src/quickbase_client/client/__init__.py
--rw-r--r--   0        0        0     3402 2022-12-20 18:13:08.866655 quickbase-client-0.6.1/src/quickbase_client/client/api.py
--rw-r--r--   0        0        0     3381 2022-04-14 20:02:04.141835 quickbase-client-0.6.1/src/quickbase_client/client/legacy_client.py
--rw-r--r--   0        0        0      954 2022-04-14 17:25:06.589401 quickbase-client-0.6.1/src/quickbase_client/client/pager.py
--rw-r--r--   0        0        0     2541 2022-04-14 19:18:51.502194 quickbase-client-0.6.1/src/quickbase_client/client/request_factory.py
--rw-r--r--   0        0        0     8488 2022-05-03 01:09:54.121609 quickbase-client-0.6.1/src/quickbase_client/client/table_client.py
--rw-r--r--   0        0        0       85 2022-04-09 23:52:19.135017 quickbase-client-0.6.1/src/quickbase_client/orm/__init__.py
--rw-r--r--   0        0        0      226 2022-04-14 17:30:36.825281 quickbase-client-0.6.1/src/quickbase_client/orm/app.py
--rw-r--r--   0        0        0     3197 2022-12-20 18:00:26.198250 quickbase-client-0.6.1/src/quickbase_client/orm/field.py
--rw-r--r--   0        0        0      221 2022-04-14 17:34:59.222278 quickbase-client-0.6.1/src/quickbase_client/orm/report.py
--rw-r--r--   0        0        0     2738 2022-04-14 17:52:08.782336 quickbase-client-0.6.1/src/quickbase_client/orm/serialize.py
--rw-r--r--   0        0        0     3819 2022-05-03 01:09:54.121836 quickbase-client-0.6.1/src/quickbase_client/orm/table.py
--rw-r--r--   0        0        0     1334 2022-04-09 23:52:19.135570 quickbase-client-0.6.1/src/quickbase_client/query/__init__.py
--rw-r--r--   0        0        0     3678 2022-04-14 17:49:43.227190 quickbase-client-0.6.1/src/quickbase_client/query/ast.py
--rw-r--r--   0        0        0     1015 2022-05-03 01:09:54.122047 quickbase-client-0.6.1/src/quickbase_client/query/query_base.py
--rw-r--r--   0        0        0     1054 2022-04-14 17:32:52.537723 quickbase-client-0.6.1/src/quickbase_client/query/query_utils.py
--rw-r--r--   0        0        0      102 2022-04-09 23:52:19.135975 quickbase-client-0.6.1/src/quickbase_client/tools/__init__.py
--rw-r--r--   0        0        0     2693 2022-04-14 20:28:09.492932 quickbase-client-0.6.1/src/quickbase_client/tools/log_handler.py
--rw-r--r--   0        0        0     9684 2022-04-14 17:35:55.709809 quickbase-client-0.6.1/src/quickbase_client/tools/model_generate.py
--rw-r--r--   0        0        0     1480 2022-04-09 23:52:19.136280 quickbase-client-0.6.1/src/quickbase_client/tools/qbc.py
--rw-r--r--   0        0        0      314 2022-04-09 23:52:19.136349 quickbase-client-0.6.1/src/quickbase_client/tools/script.py
--rw-r--r--   0        0        0      883 2022-04-09 23:52:19.136438 quickbase-client-0.6.1/src/quickbase_client/tools/script_loader.py
--rw-r--r--   0        0        0        0 2022-04-09 23:52:19.136532 quickbase-client-0.6.1/src/quickbase_client/utils/__init__.py
--rw-r--r--   0        0        0     2725 2022-04-09 23:52:19.136632 quickbase-client-0.6.1/src/quickbase_client/utils/pywriting_utils.py
--rw-r--r--   0        0        0     2402 2022-04-14 19:40:36.510211 quickbase-client-0.6.1/src/quickbase_client/utils/string_utils.py
--rw-r--r--   0        0        0     8000 2022-12-20 18:37:07.173596 quickbase-client-0.6.1/setup.py
--rw-r--r--   0        0        0     7955 2022-12-20 18:37:07.173978 quickbase-client-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1084 2022-04-09 23:52:19.129891 quickbase-client-0.6.2/LICENSE.md
+-rw-r--r--   0        0        0     6690 2023-06-06 17:43:13.601663 quickbase-client-0.6.2/README.rst
+-rw-r--r--   0        0        0     1624 2023-06-22 15:38:15.284114 quickbase-client-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0     1805 2023-06-06 17:43:13.606541 quickbase-client-0.6.2/src/quickbase_client/__init__.py
+-rw-r--r--   0        0        0      326 2022-04-09 23:52:19.134446 quickbase-client-0.6.2/src/quickbase_client/__version__.py
+-rw-r--r--   0        0        0      154 2023-06-06 17:43:13.606831 quickbase-client-0.6.2/src/quickbase_client/client/__init__.py
+-rw-r--r--   0        0        0     3402 2023-06-06 17:43:13.607099 quickbase-client-0.6.2/src/quickbase_client/client/api.py
+-rw-r--r--   0        0        0     3381 2023-06-06 17:43:13.607412 quickbase-client-0.6.2/src/quickbase_client/client/legacy_client.py
+-rw-r--r--   0        0        0      954 2023-06-06 17:43:13.607675 quickbase-client-0.6.2/src/quickbase_client/client/pager.py
+-rw-r--r--   0        0        0     2541 2023-06-06 17:43:13.608053 quickbase-client-0.6.2/src/quickbase_client/client/request_factory.py
+-rw-r--r--   0        0        0     8488 2023-06-06 17:43:13.608349 quickbase-client-0.6.2/src/quickbase_client/client/table_client.py
+-rw-r--r--   0        0        0       85 2023-01-10 13:22:49.818758 quickbase-client-0.6.2/src/quickbase_client/orm/__init__.py
+-rw-r--r--   0        0        0      226 2023-06-06 17:43:13.608591 quickbase-client-0.6.2/src/quickbase_client/orm/app.py
+-rw-r--r--   0        0        0     3197 2023-06-06 17:43:13.608834 quickbase-client-0.6.2/src/quickbase_client/orm/field.py
+-rw-r--r--   0        0        0      221 2023-06-06 17:43:13.609088 quickbase-client-0.6.2/src/quickbase_client/orm/report.py
+-rw-r--r--   0        0        0     2738 2023-06-06 17:43:13.609366 quickbase-client-0.6.2/src/quickbase_client/orm/serialize.py
+-rw-r--r--   0        0        0     3819 2023-06-06 17:43:13.609682 quickbase-client-0.6.2/src/quickbase_client/orm/table.py
+-rw-r--r--   0        0        0     1334 2022-04-09 23:52:19.135570 quickbase-client-0.6.2/src/quickbase_client/query/__init__.py
+-rw-r--r--   0        0        0     3678 2023-06-06 17:43:13.609996 quickbase-client-0.6.2/src/quickbase_client/query/ast.py
+-rw-r--r--   0        0        0     1015 2023-06-06 17:43:13.610281 quickbase-client-0.6.2/src/quickbase_client/query/query_base.py
+-rw-r--r--   0        0        0     1054 2023-06-06 17:43:13.610590 quickbase-client-0.6.2/src/quickbase_client/query/query_utils.py
+-rw-r--r--   0        0        0      102 2022-04-09 23:52:19.135975 quickbase-client-0.6.2/src/quickbase_client/tools/__init__.py
+-rw-r--r--   0        0        0     2693 2023-06-06 17:43:13.610985 quickbase-client-0.6.2/src/quickbase_client/tools/log_handler.py
+-rw-r--r--   0        0        0     9684 2023-06-06 17:43:13.611315 quickbase-client-0.6.2/src/quickbase_client/tools/model_generate.py
+-rw-r--r--   0        0        0     1480 2022-04-09 23:52:19.136280 quickbase-client-0.6.2/src/quickbase_client/tools/qbc.py
+-rw-r--r--   0        0        0      314 2022-04-09 23:52:19.136349 quickbase-client-0.6.2/src/quickbase_client/tools/script.py
+-rw-r--r--   0        0        0      883 2022-04-09 23:52:19.136438 quickbase-client-0.6.2/src/quickbase_client/tools/script_loader.py
+-rw-r--r--   0        0        0        0 2022-04-09 23:52:19.136532 quickbase-client-0.6.2/src/quickbase_client/utils/__init__.py
+-rw-r--r--   0        0        0     2725 2022-04-09 23:52:19.136632 quickbase-client-0.6.2/src/quickbase_client/utils/pywriting_utils.py
+-rw-r--r--   0        0        0     2521 2023-06-22 15:40:21.740870 quickbase-client-0.6.2/src/quickbase_client/utils/string_utils.py
+-rw-r--r--   0        0        0     8000 2023-06-22 15:41:27.159476 quickbase-client-0.6.2/setup.py
+-rw-r--r--   0        0        0     7955 2023-06-22 15:41:27.159855 quickbase-client-0.6.2/PKG-INFO
```

### Comparing `quickbase-client-0.6.1/LICENSE.md` & `quickbase-client-0.6.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `quickbase-client-0.6.1/README.rst` & `quickbase-client-0.6.2/README.rst`

 * *Files identical despite different names*

### Comparing `quickbase-client-0.6.1/pyproject.toml` & `quickbase-client-0.6.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "quickbase-client"
-version = "0.6.1"
+version = "0.6.2"
 description = "A Quickbase Python API Client Generator"
 authors = ["Tim Kutcher <tim@tkutcher.com>"]
 maintainers = ["Tim Kutcher <tim@tkutcher.com>"]
 readme = "README.rst"
 license = "LICENSE.md"
 homepage = "https://github.com/tkutcher/quickbase-client"
 repository = "https://github.com/tkutcher/quickbase-client"
```

### Comparing `quickbase-client-0.6.1/src/quickbase_client/__init__.py` & `quickbase-client-0.6.2/src/quickbase_client/__init__.py`

 * *Files identical despite different names*

### Comparing `quickbase-client-0.6.1/src/quickbase_client/client/api.py` & `quickbase-client-0.6.2/src/quickbase_client/client/api.py`

 * *Files identical despite different names*

### Comparing `quickbase-client-0.6.1/src/quickbase_client/client/legacy_client.py` & `quickbase-client-0.6.2/src/quickbase_client/client/legacy_client.py`

 * *Files identical despite different names*

### Comparing `quickbase-client-0.6.1/src/quickbase_client/client/pager.py` & `quickbase-client-0.6.2/src/quickbase_client/client/pager.py`

 * *Files identical despite different names*

### Comparing `quickbase-client-0.6.1/src/quickbase_client/client/request_factory.py` & `quickbase-client-0.6.2/src/quickbase_client/client/request_factory.py`

 * *Files identical despite different names*

### Comparing `quickbase-client-0.6.1/src/quickbase_client/client/table_client.py` & `quickbase-client-0.6.2/src/quickbase_client/client/table_client.py`

 * *Files identical despite different names*

### Comparing `quickbase-client-0.6.1/src/quickbase_client/orm/field.py` & `quickbase-client-0.6.2/src/quickbase_client/orm/field.py`

 * *Files identical despite different names*

### Comparing `quickbase-client-0.6.1/src/quickbase_client/orm/serialize.py` & `quickbase-client-0.6.2/src/quickbase_client/orm/serialize.py`

 * *Files identical despite different names*

### Comparing `quickbase-client-0.6.1/src/quickbase_client/orm/table.py` & `quickbase-client-0.6.2/src/quickbase_client/orm/table.py`

 * *Files identical despite different names*

### Comparing `quickbase-client-0.6.1/src/quickbase_client/query/__init__.py` & `quickbase-client-0.6.2/src/quickbase_client/query/__init__.py`

 * *Files identical despite different names*

### Comparing `quickbase-client-0.6.1/src/quickbase_client/query/ast.py` & `quickbase-client-0.6.2/src/quickbase_client/query/ast.py`

 * *Files identical despite different names*

### Comparing `quickbase-client-0.6.1/src/quickbase_client/query/query_base.py` & `quickbase-client-0.6.2/src/quickbase_client/query/query_base.py`

 * *Files identical despite different names*

### Comparing `quickbase-client-0.6.1/src/quickbase_client/query/query_utils.py` & `quickbase-client-0.6.2/src/quickbase_client/query/query_utils.py`

 * *Files identical despite different names*

### Comparing `quickbase-client-0.6.1/src/quickbase_client/tools/log_handler.py` & `quickbase-client-0.6.2/src/quickbase_client/tools/log_handler.py`

 * *Files identical despite different names*

### Comparing `quickbase-client-0.6.1/src/quickbase_client/tools/model_generate.py` & `quickbase-client-0.6.2/src/quickbase_client/tools/model_generate.py`

 * *Files identical despite different names*

### Comparing `quickbase-client-0.6.1/src/quickbase_client/tools/qbc.py` & `quickbase-client-0.6.2/src/quickbase_client/tools/qbc.py`

 * *Files identical despite different names*

### Comparing `quickbase-client-0.6.1/src/quickbase_client/tools/script_loader.py` & `quickbase-client-0.6.2/src/quickbase_client/tools/script_loader.py`

 * *Files identical despite different names*

### Comparing `quickbase-client-0.6.1/src/quickbase_client/utils/pywriting_utils.py` & `quickbase-client-0.6.2/src/quickbase_client/utils/pywriting_utils.py`

 * *Files identical despite different names*

### Comparing `quickbase-client-0.6.1/src/quickbase_client/utils/string_utils.py` & `quickbase-client-0.6.2/src/quickbase_client/utils/string_utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,16 +12,22 @@
 
 _case_map = {
     "snake": VarMakerStrategy(stringcase.snakecase, "_"),
     "pascal": VarMakerStrategy(stringcase.pascalcase, ""),
     "camel": VarMakerStrategy(stringcase.camelcase, ""),  # :(
 }
 
+
+def _drop_numbers_strategy(v: str):
+    dropped = v.lstrip(string.digits)
+    return f"x{v}" if len(dropped) == 0 else dropped
+
+
 _number_map = {
-    "drop": lambda v: v.lstrip(string.digits),
+    "drop": _drop_numbers_strategy,
     "underscore": lambda v: f"_{v}",
 }
 
 
 def make_var_name(s: str, case="snake", number_strategy="drop"):
     case_func, special_replacer = _case_map[case]
```

### Comparing `quickbase-client-0.6.1/setup.py` & `quickbase-client-0.6.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 ['attrs>=21.4.0,<22.0.0', 'requests>=2.27.1,<3.0.0', 'stringcase>=1.2.0,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['qbc = quickbase_client.tools.qbc:main']}
 
 setup_kwargs = {
     'name': 'quickbase-client',
-    'version': '0.6.1',
+    'version': '0.6.2',
     'description': 'A Quickbase Python API Client Generator',
     'long_description': '#####################\nQuickbase-Client\n#####################\n\nA High-Level Quickbase Python API Client & Model Generator\n\n\n.. image:: https://gitlab.com/tkutcher/quickbase-client/badges/dev/pipeline.svg\n    :target: https://gitlab.com/tkutcher/quickbase-client/-/commits/dev\n    :alt: Pipeline Status\n\n.. image:: https://gitlab.com/tkutcher/quickbase-client/badges/dev/coverage.svg\n    :target: https://gitlab.com/tkutcher/quickbase-client/-/commits/dev\n    :alt: Coverage Report\n\n.. image:: https://readthedocs.org/projects/quickbase-client/badge/?version=latest\n    :target: https://quickbase-client.readthedocs.io/en/latest/?badge=latest\n    :alt: Documentation Status\n\n.. image:: https://badge.fury.io/py/quickbase-client.svg\n    :target: https://badge.fury.io/py/quickbase-client\n    :alt: PyPI\n\n.. image:: https://img.shields.io/badge/code%20style-black-000000.svg\n    :target: https://github.com/psf/black\n    :alt: Black Code Style\n\n|\n\n\n*Quickbase-Client is a library for interacting with Quickbase applications through their\nRESTful JSON API (https://developer.quickbase.com/). It has features to generate model classes\nfor tables in your Quickbase app, and provides high level classes to interface between Python\nobjects and the Quickbase tables.*\n\n|\n\n\n.. inclusion-marker-do-not-remove\n\nQuick Start\n============\n\n\nInstallation\n____________\n\nInstallation can be done through pip:\n\n.. code-block:: bash\n\n    pip install quickbase-client\n\nThis will install both the library ``quickbase_client``, and a command line tool ``qbc`` for\nrunning some handy scripts.\n\n\nGenerating your Models\n----------------------\n\nTo interact and authenticate with your Quickbase applications you need a User Token. You can read\nthe Quickbase documentation `here <https://developer.quickbase.com/auth>`_ on how to create one.\nIt is recommended to set an environment variable ``QB_USER_TOKEN`` with this value:\n\n.. code-block:: bash\n\n    export QB_USER_TOKEN=mytokenfromquickbase;\n\n\nNext, say you have a hypothetical Quickbase Application named MyApp at\n``https://foo.quickbase.com/db/abcdef`` that has tables for tracking things\nagainst a repository like Issues & Pipelines.\n\n\n.. image:: /images/example_table.png\n    :width: 500\n    :alt: Example Table\n\n|\n\nRunning the following:\n\n.. code-block:: bash\n\n    qbc run model-generate -a https://foo.quickbase.com/db/abcdef\n\nWould generate a directory structure like\n\n::\n\n    models\n    ├── __init__.py\n    └── my_app\n        ├── __init__.py\n     \xa0\xa0 ├── app.py\n    \xa0\xa0  ├── github_issue.py\n    \xa0\xa0  └── gitlab_pipeline.py\n\nAnd classes like ``GitHubIssue`` where you can interact with the data model through a Python object.\n\n\nWriting Records to Quickbase\n----------------------------\n\nClasses like ``GitHubIssue`` that subclass ``QuickbaseTable`` also get a factory class-method\n``client(user_tok)`` which creates an instance of the higher-level ``QuickbaseTableClient`` to\nmake API requests for things related to that table:\n\n.. code-block:: python\n\n    client = GitHubIssue.client(user_tok=os.environ[\'QB_USER_TOKEN\'])\n    new_issue = GitHubIssue(\n        title=\'Something broke\',   # you get friendly-kwargs for fields without worrying about ID\'s\n        description=\'Please fix!\',\n        date_opened=date.today()   # things like Python date objects will be serialized\n    )\n    response = client.add_record(new_issue)\n    print(response.json())  # all methods (except for query) return the requests Response object\n\n\nQuerying Records from Quickbase\n-------------------------------\n\nYou can also use the client object to send queries to the Quickbase API through the ``query``\nmethod. This method will serialize the data back in to a Python object. The `query` method on the\ntable class takes a ``QuickbaseQuery`` object which is high level wrapper around the parameters\nneeded to make a query.\n\nNotably, the ``where`` parameter for specifying the query string. There is one (and in the future\nthere will be more) implementation of this which allows you to build query-strings through\nhigher-level python functions.\n\nYou can use the methods exposed in the ``quickbase_client.query`` module like so:\n\n.. code-block:: python\n\n    # convention to append an underscore to these methods to avoid clashing\n    # with any python keywords\n    from quickbase_client.query import on_or_before_\n    from quickbase_client.query import eq_\n    from quickbase_client.query import and_\n\n    schema = GitHubIssue.schema\n    q = and_(\n        eq_(schema.date_opened, schema.date_created),\n        on_or_before_(schema.date_closed, date(2020, 11, 16))\n    )\n    print(q.where)  # ({\'9\'.EX.\'_FID_1\'}AND{\'10\'.OBF.\'11-16-2020\'})\n    recs = client.query(q)  # recs will be GitHubIssue objects unless passing raw=True\n    print([str(r) for r in recs])  # [\'<GitHubIssue title="Made And Closed Today" id="10000">\']\n\n\n\nControlling Lower-Level API Calls\n---------------------------------\n\nLastly, say you want to deal with just posting the specific json/data Quickbase is looking for.\nThe ``QuickbaseTableClient`` object wraps the lower-level ``QuickbaseApiClient`` object which has\nmethods for just sending the actual data (with an even lower-level utility\n``QuickbaseRequestFactory`` you could also use). These classes manage hanging on to the user token,\nand the realm hostname, etc. for each request that is made.\n\nFor example, note the signature of ``query`` in ``QuickbaseApiClient``:\n\n.. code-block:: python\n\n    def query(self, table_id, fields_to_select=None, where_str=None,\n              sort_by=None, group_by=None, options=None):\n\n\nYou can get to this class by going through the table client: ``api = client.api``, or from\ninstantiating it directly ``api = QuickbaseApiClient(my_user_token, my_realm)``\n\nWith this, we could make the exact same request as before:\n\n.. code-block:: python\n\n    api = QuickbaseApiClient(user_token=\'my_token\', realm_hostname=\'foo.quickbase.com\')\n    response = api.query(\n        table_id=\'abcdef\',\n        where_str="({\'9\'.EX.\'_FID_1\'}AND{\'10\'.OBF.\'11-16-2020\'})")\n    data = response.json()\n\n\n.. exclusion-marker-do-not-remove\n\nMore Resources\n==============\n- `examples </examples>`_ directory.\n- `CONTRIBUTING </CONTRIBUTING.md>`_\n- `LICENSE </LICENSE.md>`_\n\n\nOther Notes\n====================\n\n\nCurrently a bunch of duplicate aliases for ``QuickBase`` to ``Quickbase`` since this\nwas originally released with everything prefixed as ``QuickBase-``. But since Quickbase\nis branding more to "Quickbase", this will eventually be the main naming for\nversion 1.0 in an effort to keep more consistent. So prefer to use `Quickbase-` prefixed classes\nas in the future the other aliases will be dropped.\n',
     'author': 'Tim Kutcher',
     'author_email': 'tim@tkutcher.com',
     'maintainer': 'Tim Kutcher',
     'maintainer_email': 'tim@tkutcher.com',
     'url': 'https://github.com/tkutcher/quickbase-client',
```

### Comparing `quickbase-client-0.6.1/PKG-INFO` & `quickbase-client-0.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickbase-client
-Version: 0.6.1
+Version: 0.6.2
 Summary: A Quickbase Python API Client Generator
 Home-page: https://github.com/tkutcher/quickbase-client
 License: LICENSE.md
 Keywords: quickbase,client,quickbase-api,orm,generator
 Author: Tim Kutcher
 Author-email: tim@tkutcher.com
 Maintainer: Tim Kutcher
```

