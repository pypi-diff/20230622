# Comparing `tmp/remotivelabs_cli-0.0.1a5.tar.gz` & `tmp/remotivelabs_cli-0.0.1a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remotivelabs_cli-0.0.1a5.tar", max compression
+gzip compressed data, was "remotivelabs_cli-0.0.1a6.tar", max compression
```

## Comparing `remotivelabs_cli-0.0.1a5.tar` & `remotivelabs_cli-0.0.1a6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      608 2023-06-19 13:55:54.232642 remotivelabs_cli-0.0.1a5/LICENSE
--rw-r--r--   0        0        0     2092 2023-06-18 17:01:10.908056 remotivelabs_cli-0.0.1a5/README.md
--rw-r--r--   0        0        0      122 2022-10-26 14:05:47.581000 remotivelabs_cli-0.0.1a5/cli/__about__.py
--rw-r--r--   0        0        0       26 2022-10-26 11:41:55.030088 remotivelabs_cli-0.0.1a5/cli/__init__.py
--rw-r--r--   0        0        0     4011 2023-06-21 12:52:00.336557 remotivelabs_cli-0.0.1a5/cli/brokers.py
--rw-r--r--   0        0        0        1 2022-10-24 12:45:02.134227 remotivelabs_cli-0.0.1a5/cli/cloud/__init__.py
--rw-r--r--   0        0        0     4568 2023-06-21 14:05:59.199099 remotivelabs_cli-0.0.1a5/cli/cloud/auth.py
--rw-r--r--   0        0        0     1391 2023-06-21 11:01:07.131368 remotivelabs_cli-0.0.1a5/cli/cloud/auth_keys.py
--rw-r--r--   0        0        0     2321 2023-06-21 11:04:28.728967 remotivelabs_cli-0.0.1a5/cli/cloud/brokers.py
--rw-r--r--   0        0        0     1580 2023-06-21 13:16:22.379502 remotivelabs_cli-0.0.1a5/cli/cloud/cloud_cli.py
--rw-r--r--   0        0        0     3132 2023-06-19 13:52:07.776885 remotivelabs_cli-0.0.1a5/cli/cloud/configs.py
--rw-r--r--   0        0        0     1366 2023-06-20 19:11:51.341364 remotivelabs_cli-0.0.1a5/cli/cloud/projects.py
--rw-r--r--   0        0        0     6887 2023-06-19 12:26:04.278978 remotivelabs_cli-0.0.1a5/cli/cloud/recordings.py
--rw-r--r--   0        0        0     3486 2023-06-21 12:56:24.052615 remotivelabs_cli-0.0.1a5/cli/cloud/rest_helper.py
--rw-r--r--   0        0        0     1990 2023-06-20 13:21:18.023240 remotivelabs_cli-0.0.1a5/cli/cloud/service_account_keys.py
--rw-r--r--   0        0        0     1615 2023-06-21 14:06:01.150934 remotivelabs_cli-0.0.1a5/cli/cloud/service_accounts.py
--rw-r--r--   0        0        0      141 2022-10-25 14:33:01.608000 remotivelabs_cli-0.0.1a5/cli/lib/__about__.py
--rw-r--r--   0        0        0     4938 2023-06-21 12:13:16.823623 remotivelabs_cli-0.0.1a5/cli/lib/broker.py
--rw-r--r--   0        0        0      315 2023-06-20 11:51:00.031101 remotivelabs_cli-0.0.1a5/cli/remotive.py
--rw-r--r--   0        0        0       77 2023-06-08 06:07:23.995982 remotivelabs_cli-0.0.1a5/cli/requirements.txt
--rw-r--r--   0        0        0       63 2023-03-21 06:24:07.422989 remotivelabs_cli-0.0.1a5/cli/test/test_simple.py
--rw-r--r--   0        0        0      498 2023-06-21 14:07:53.672220 remotivelabs_cli-0.0.1a5/pyproject.toml
--rw-r--r--   0        0        0     2744 1970-01-01 00:00:00.000000 remotivelabs_cli-0.0.1a5/PKG-INFO
+-rw-r--r--   0        0        0      608 2023-06-19 13:55:54.232642 remotivelabs_cli-0.0.1a6/LICENSE
+-rw-r--r--   0        0        0     2095 2023-06-22 08:12:57.643193 remotivelabs_cli-0.0.1a6/README.md
+-rw-r--r--   0        0        0      122 2022-10-26 14:05:47.581000 remotivelabs_cli-0.0.1a6/cli/__about__.py
+-rw-r--r--   0        0        0       26 2022-10-26 11:41:55.030088 remotivelabs_cli-0.0.1a6/cli/__init__.py
+-rw-r--r--   0        0        0     4011 2023-06-21 12:52:00.336557 remotivelabs_cli-0.0.1a6/cli/brokers.py
+-rw-r--r--   0        0        0        1 2022-10-24 12:45:02.134227 remotivelabs_cli-0.0.1a6/cli/cloud/__init__.py
+-rw-r--r--   0        0        0     3538 2023-06-22 08:03:29.813439 remotivelabs_cli-0.0.1a6/cli/cloud/auth.py
+-rw-r--r--   0        0        0     2940 2023-06-22 08:03:46.314372 remotivelabs_cli-0.0.1a6/cli/cloud/auth_keys.py
+-rw-r--r--   0        0        0     2323 2023-06-22 08:07:25.218764 remotivelabs_cli-0.0.1a6/cli/cloud/brokers.py
+-rw-r--r--   0        0        0     1580 2023-06-21 13:16:22.379502 remotivelabs_cli-0.0.1a6/cli/cloud/cloud_cli.py
+-rw-r--r--   0        0        0     3132 2023-06-19 13:52:07.776885 remotivelabs_cli-0.0.1a6/cli/cloud/configs.py
+-rw-r--r--   0        0        0     1366 2023-06-20 19:11:51.341364 remotivelabs_cli-0.0.1a6/cli/cloud/projects.py
+-rw-r--r--   0        0        0     6887 2023-06-19 12:26:04.278978 remotivelabs_cli-0.0.1a6/cli/cloud/recordings.py
+-rw-r--r--   0        0        0     3486 2023-06-21 12:56:24.052615 remotivelabs_cli-0.0.1a6/cli/cloud/rest_helper.py
+-rw-r--r--   0        0        0     1990 2023-06-20 13:21:18.023240 remotivelabs_cli-0.0.1a6/cli/cloud/service_account_keys.py
+-rw-r--r--   0        0        0     1615 2023-06-21 14:06:01.150934 remotivelabs_cli-0.0.1a6/cli/cloud/service_accounts.py
+-rw-r--r--   0        0        0      141 2022-10-25 14:33:01.608000 remotivelabs_cli-0.0.1a6/cli/lib/__about__.py
+-rw-r--r--   0        0        0     4938 2023-06-21 12:13:16.823623 remotivelabs_cli-0.0.1a6/cli/lib/broker.py
+-rw-r--r--   0        0        0      432 2023-06-22 08:58:34.023633 remotivelabs_cli-0.0.1a6/cli/remotive.py
+-rw-r--r--   0        0        0       77 2023-06-08 06:07:23.995982 remotivelabs_cli-0.0.1a6/cli/requirements.txt
+-rw-r--r--   0        0        0       63 2023-03-21 06:24:07.422989 remotivelabs_cli-0.0.1a6/cli/test/test_simple.py
+-rw-r--r--   0        0        0      498 2023-06-22 09:00:33.296453 remotivelabs_cli-0.0.1a6/pyproject.toml
+-rw-r--r--   0        0        0     2747 1970-01-01 00:00:00.000000 remotivelabs_cli-0.0.1a6/PKG-INFO
```

### Comparing `remotivelabs_cli-0.0.1a5/LICENSE` & `remotivelabs_cli-0.0.1a6/LICENSE`

 * *Files identical despite different names*

### Comparing `remotivelabs_cli-0.0.1a5/README.md` & `remotivelabs_cli-0.0.1a6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 *NOTE: This is currently an experimental version*
 
 ## Install
 
 Requires python 3
 
 ```
-pip install remotivelabs-cli
+pip install -U remotivelabs-cli
 remotive --help
 
 Usage: remotive [OPTIONS] COMMAND [ARGS]...
 
 ╭─ Options ───────────────────────────────────────────────────────────────────────────────────────────────╮
 │ --install-completion          Install completion for the current shell.                                 │
 │ --show-completion             Show completion for the current shell, to copy it or customize the        │
```

### Comparing `remotivelabs_cli-0.0.1a5/cli/brokers.py` & `remotivelabs_cli-0.0.1a6/cli/brokers.py`

 * *Files identical despite different names*

### Comparing `remotivelabs_cli-0.0.1a5/cli/cloud/auth.py` & `remotivelabs_cli-0.0.1a6/cli/cloud/auth.py`

 * *Files 13% similar despite different names*

```diff
@@ -82,52 +82,18 @@
 def print_access_token():
     """
     Print current active access token
     """
     print(read_token())
 
 
-@app.command()
-def list():
-    """
-    List available key files in remotivelabs config directory
-    """
-    for file in os.listdir(config_dir_name):
-        print(file)
-
-
-@app.command()
-def describe(
-        file: str = typer.Option(..., help="File name")):
-    """
-    Show contents of specified key file
-    """
-    print(read_file(file))
 
 
-@app.command()
-def activate(
-        file: str = typer.Option(..., help="File name")):
-    """
-    Activate a key file to be used for authentication.
 
-    --file
 
-    This will be used as the current access token in all subsequent requests. This would
-    be the same as login with a browser.
-    """
-    # Best effort to read file
-    if os.path.exists(file):
-        token_file = json.loads(read_file_with_path(file))
-        write_token(token_file['token'])
-    elif os.path.exists(str(Path.home()) + f"/.config/.remotive/{file}"):
-        token_file = json.loads(read_file(file))
-        write_token(token_file['token'])
-    else:
-        sys.stderr.write("File could not be found \n")
 
 
 #@app.command(help="Clear access token")
 #def logout():
 #    write_token("")
 #    print("Access token removed")
```

### Comparing `remotivelabs_cli-0.0.1a5/cli/cloud/brokers.py` & `remotivelabs_cli-0.0.1a6/cli/cloud/brokers.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 
 @app.command("describe", help="Shows details about a specific broker")
 def describe(name: str, project: str = typer.Option(..., help="Project ID", envvar='REMOTIVE_CLOUD_PROJECT')):
     rest.handle_get(f"/api/project/{project}/brokers/{name}")
 
 
-@app.command("stop", help="Stops and removes a broker from project")
+@app.command("remove", help="Stops and removes a broker from project")
 def stop(name: str, project: str = typer.Option(..., help="Project ID", envvar='REMOTIVE_CLOUD_PROJECT')):
     with Progress(
             SpinnerColumn(),
             TextColumn("[progress.description]{task.description}"),
             transient=True,
     ) as progress:
         progress.add_task(description=f"Stopping broker {name}...", total=None)
```

### Comparing `remotivelabs_cli-0.0.1a5/cli/cloud/cloud_cli.py` & `remotivelabs_cli-0.0.1a6/cli/cloud/cloud_cli.py`

 * *Files identical despite different names*

### Comparing `remotivelabs_cli-0.0.1a5/cli/cloud/configs.py` & `remotivelabs_cli-0.0.1a6/cli/cloud/configs.py`

 * *Files identical despite different names*

### Comparing `remotivelabs_cli-0.0.1a5/cli/cloud/projects.py` & `remotivelabs_cli-0.0.1a6/cli/cloud/projects.py`

 * *Files identical despite different names*

### Comparing `remotivelabs_cli-0.0.1a5/cli/cloud/recordings.py` & `remotivelabs_cli-0.0.1a6/cli/cloud/recordings.py`

 * *Files identical despite different names*

### Comparing `remotivelabs_cli-0.0.1a5/cli/cloud/rest_helper.py` & `remotivelabs_cli-0.0.1a6/cli/cloud/rest_helper.py`

 * *Files identical despite different names*

### Comparing `remotivelabs_cli-0.0.1a5/cli/cloud/service_account_keys.py` & `remotivelabs_cli-0.0.1a6/cli/cloud/service_account_keys.py`

 * *Files identical despite different names*

### Comparing `remotivelabs_cli-0.0.1a5/cli/cloud/service_accounts.py` & `remotivelabs_cli-0.0.1a6/cli/cloud/service_accounts.py`

 * *Files identical despite different names*

### Comparing `remotivelabs_cli-0.0.1a5/cli/lib/broker.py` & `remotivelabs_cli-0.0.1a6/cli/lib/broker.py`

 * *Files identical despite different names*

### Comparing `remotivelabs_cli-0.0.1a5/PKG-INFO` & `remotivelabs_cli-0.0.1a6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remotivelabs-cli
-Version: 0.0.1a5
+Version: 0.0.1a6
 Summary: 
 Author: Johan Rask
 Author-email: johan.rask@remotivelabs.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -24,15 +24,15 @@
 *NOTE: This is currently an experimental version*
 
 ## Install
 
 Requires python 3
 
 ```
-pip install remotivelabs-cli
+pip install -U remotivelabs-cli
 remotive --help
 
 Usage: remotive [OPTIONS] COMMAND [ARGS]...
 
 ╭─ Options ───────────────────────────────────────────────────────────────────────────────────────────────╮
 │ --install-completion          Install completion for the current shell.                                 │
 │ --show-completion             Show completion for the current shell, to copy it or customize the        │
```

