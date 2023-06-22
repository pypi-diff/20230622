# Comparing `tmp/fair_cli-0.7.0.tar.gz` & `tmp/fair_cli-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fair_cli-0.7.0.tar", max compression
+gzip compressed data, was "fair_cli-0.7.1.tar", max compression
```

## Comparing `fair_cli-0.7.0.tar` & `fair_cli-0.7.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1855 2023-06-12 13:03:22.463189 fair_cli-0.7.0/CHANGELOG.md
--rw-r--r--   0        0        0     1358 2023-06-12 13:03:22.463239 fair_cli-0.7.0/CITATION.cff
--rw-r--r--   0        0        0     1314 2023-06-12 13:03:22.463351 fair_cli-0.7.0/LICENSE
--rw-r--r--   0        0        0    11363 2023-06-21 16:01:16.540375 fair_cli-0.7.0/README.md
--rw-r--r--   0        0        0     1976 2023-06-12 13:03:22.464552 fair_cli-0.7.0/fair/__init__.py
--rw-r--r--   0        0        0    22289 2023-06-21 17:23:03.900038 fair_cli-0.7.0/fair/cli.py
--rw-r--r--   0        0        0     9190 2023-06-21 16:01:16.540403 fair_cli-0.7.0/fair/common.py
--rw-r--r--   0        0        0    28212 2023-06-21 17:07:31.416628 fair_cli-0.7.0/fair/configuration/__init__.py
--rw-r--r--   0        0        0     3311 2023-06-12 13:03:22.464979 fair_cli-0.7.0/fair/configuration/validation.py
--rw-r--r--   0        0        0     5358 2023-06-12 13:03:22.465044 fair_cli-0.7.0/fair/exceptions.py
--rw-r--r--   0        0        0    10127 2023-06-12 13:03:22.465098 fair_cli-0.7.0/fair/files.txt
--rw-r--r--   0        0        0     4619 2023-06-12 13:03:22.465161 fair_cli-0.7.0/fair/history.py
--rw-r--r--   0        0        0     3958 2023-06-12 13:03:22.465230 fair_cli-0.7.0/fair/identifiers.py
--rw-r--r--   0        0        0     3010 2023-06-14 13:29:24.954224 fair_cli-0.7.0/fair/logging.py
--rw-r--r--   0        0        0     8206 2023-06-14 13:29:24.954405 fair_cli-0.7.0/fair/register.py
--rw-r--r--   0        0        0      161 2023-06-12 13:03:22.465449 fair_cli-0.7.0/fair/registry/__init__.py
--rw-r--r--   0        0        0     1249 2023-06-12 13:03:22.465501 fair_cli-0.7.0/fair/registry/file_formats.json
--rw-r--r--   0        0        0      120 2023-06-12 13:03:22.465547 fair_cli-0.7.0/fair/registry/file_types.py
--rw-r--r--   0        0        0    17278 2023-06-14 13:29:24.954679 fair_cli-0.7.0/fair/registry/requests.py
--rw-r--r--   0        0        0    14756 2023-06-12 13:03:22.465732 fair_cli-0.7.0/fair/registry/server.py
--rw-r--r--   0        0        0    23693 2023-06-21 16:05:36.970594 fair_cli-0.7.0/fair/registry/storage.py
--rw-r--r--   0        0        0    38433 2023-06-14 13:29:24.955335 fair_cli-0.7.0/fair/registry/sync.py
--rw-r--r--   0        0        0     4752 2023-06-12 13:03:22.466011 fair_cli-0.7.0/fair/registry/versioning.py
--rw-r--r--   0        0        0     2302 2023-06-12 13:03:22.466108 fair_cli-0.7.0/fair/run.py
--rw-r--r--   0        0        0    49608 2023-06-21 16:41:58.205044 fair_cli-0.7.0/fair/session.py
--rw-r--r--   0        0        0    16133 2023-06-14 13:29:24.955867 fair_cli-0.7.0/fair/staging.py
--rw-r--r--   0        0        0      490 2023-06-12 13:03:22.466460 fair_cli-0.7.0/fair/templates/__init__.py
--rw-r--r--   0        0        0      296 2023-06-12 13:03:22.466514 fair_cli-0.7.0/fair/templates/config.jinja
--rw-r--r--   0        0        0      136 2023-06-12 13:03:22.466556 fair_cli-0.7.0/fair/templates/hist.jinja
--rw-r--r--   0        0        0     3181 2023-06-12 13:03:22.466610 fair_cli-0.7.0/fair/testing.py
--rw-r--r--   0        0        0    53662 2023-06-12 13:03:22.466847 fair_cli-0.7.0/fair/user_config/__init__.py
--rw-r--r--   0        0        0     4830 2023-06-12 13:03:22.466916 fair_cli-0.7.0/fair/user_config/globbing.py
--rw-r--r--   0        0        0     9187 2023-06-12 13:03:22.466981 fair_cli-0.7.0/fair/user_config/validation.py
--rw-r--r--   0        0        0     5087 2023-06-14 13:29:24.956007 fair_cli-0.7.0/fair/utilities.py
--rw-r--r--   0        0        0     1465 2023-06-12 13:03:22.467103 fair_cli-0.7.0/fair/virtualenv.py
--rw-r--r--   0        0        0     2563 2023-06-21 18:06:06.014133 fair_cli-0.7.0/pyproject.toml
--rw-r--r--   0        0        0    13498 1970-01-01 00:00:00.000000 fair_cli-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1855 2023-06-21 19:13:33.324048 fair_cli-0.7.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1358 2023-06-21 19:13:33.324149 fair_cli-0.7.1/CITATION.cff
+-rw-r--r--   0        0        0     1314 2023-06-12 13:03:22.463351 fair_cli-0.7.1/LICENSE
+-rw-r--r--   0        0        0    11363 2023-06-21 19:13:33.324484 fair_cli-0.7.1/README.md
+-rw-r--r--   0        0        0     1976 2023-06-12 13:03:22.464552 fair_cli-0.7.1/fair/__init__.py
+-rw-r--r--   0        0        0    21339 2023-06-22 16:57:58.009966 fair_cli-0.7.1/fair/cli.py
+-rw-r--r--   0        0        0     9190 2023-06-21 19:13:33.326523 fair_cli-0.7.1/fair/common.py
+-rw-r--r--   0        0        0    28212 2023-06-21 19:13:33.326880 fair_cli-0.7.1/fair/configuration/__init__.py
+-rw-r--r--   0        0        0     3311 2023-06-21 19:13:33.326964 fair_cli-0.7.1/fair/configuration/validation.py
+-rw-r--r--   0        0        0     5358 2023-06-21 19:13:33.327099 fair_cli-0.7.1/fair/exceptions.py
+-rw-r--r--   0        0        0    10127 2023-06-21 19:13:33.327168 fair_cli-0.7.1/fair/files.txt
+-rw-r--r--   0        0        0     4619 2023-06-21 19:13:33.327283 fair_cli-0.7.1/fair/history.py
+-rw-r--r--   0        0        0     3958 2023-06-21 19:13:33.327397 fair_cli-0.7.1/fair/identifiers.py
+-rw-r--r--   0        0        0     3010 2023-06-21 19:13:33.327463 fair_cli-0.7.1/fair/logging.py
+-rw-r--r--   0        0        0     8206 2023-06-21 19:13:33.327581 fair_cli-0.7.1/fair/register.py
+-rw-r--r--   0        0        0      161 2023-06-21 19:13:33.327663 fair_cli-0.7.1/fair/registry/__init__.py
+-rw-r--r--   0        0        0     1249 2023-06-12 13:03:22.465501 fair_cli-0.7.1/fair/registry/file_formats.json
+-rw-r--r--   0        0        0      120 2023-06-12 13:03:22.465547 fair_cli-0.7.1/fair/registry/file_types.py
+-rw-r--r--   0        0        0    17292 2023-06-22 15:55:58.649339 fair_cli-0.7.1/fair/registry/requests.py
+-rw-r--r--   0        0        0    14756 2023-06-21 19:13:33.328007 fair_cli-0.7.1/fair/registry/server.py
+-rw-r--r--   0        0        0    23733 2023-06-22 15:55:58.649688 fair_cli-0.7.1/fair/registry/storage.py
+-rw-r--r--   0        0        0    38515 2023-06-22 15:55:58.650104 fair_cli-0.7.1/fair/registry/sync.py
+-rw-r--r--   0        0        0     4752 2023-06-21 19:13:33.329007 fair_cli-0.7.1/fair/registry/versioning.py
+-rw-r--r--   0        0        0     2302 2023-06-21 19:13:33.329217 fair_cli-0.7.1/fair/run.py
+-rw-r--r--   0        0        0    49608 2023-06-21 19:13:33.329700 fair_cli-0.7.1/fair/session.py
+-rw-r--r--   0        0        0    16133 2023-06-21 19:13:33.329852 fair_cli-0.7.1/fair/staging.py
+-rw-r--r--   0        0        0      490 2023-06-12 13:03:22.466460 fair_cli-0.7.1/fair/templates/__init__.py
+-rw-r--r--   0        0        0      296 2023-06-12 13:03:22.466514 fair_cli-0.7.1/fair/templates/config.jinja
+-rw-r--r--   0        0        0      136 2023-06-12 13:03:22.466556 fair_cli-0.7.1/fair/templates/hist.jinja
+-rw-r--r--   0        0        0     3181 2023-06-21 19:13:33.329963 fair_cli-0.7.1/fair/testing.py
+-rw-r--r--   0        0        0    53662 2023-06-22 16:29:13.604131 fair_cli-0.7.1/fair/user_config/__init__.py
+-rw-r--r--   0        0        0     4830 2023-06-21 19:13:33.330469 fair_cli-0.7.1/fair/user_config/globbing.py
+-rw-r--r--   0        0        0     9187 2023-06-21 19:13:33.330549 fair_cli-0.7.1/fair/user_config/validation.py
+-rw-r--r--   0        0        0     5087 2023-06-21 19:13:33.330678 fair_cli-0.7.1/fair/utilities.py
+-rw-r--r--   0        0        0     1465 2023-06-21 19:13:33.330742 fair_cli-0.7.1/fair/virtualenv.py
+-rw-r--r--   0        0        0     2563 2023-06-22 16:57:58.010274 fair_cli-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0    13296 1970-01-01 00:00:00.000000 fair_cli-0.7.1/PKG-INFO
```

### Comparing `fair_cli-0.7.0/CHANGELOG.md` & `fair_cli-0.7.1/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `fair_cli-0.7.0/CITATION.cff` & `fair_cli-0.7.1/CITATION.cff`

 * *Files identical despite different names*

### Comparing `fair_cli-0.7.0/LICENSE` & `fair_cli-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fair_cli-0.7.0/README.md` & `fair_cli-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `fair_cli-0.7.0/fair/__init__.py` & `fair_cli-0.7.1/fair/__init__.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.7.0/fair/cli.py` & `fair_cli-0.7.1/fair/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -102,16 +102,15 @@
         ) as fair_session:
             fair_session.status_data_products()
             fair_session.status_code_runs()
     except fdp_exc.FAIRCLIException as e:
         if debug:
             raise e
         e.err_print()
-        if e.level.lower() == "error":
-            sys.exit(e.exit_code)
+        sys.exit(e.exit_code)
 
 @cli.group(invoke_without_command=True)
 @click.option("--debug/--no-debug", help="Run in debug mode", default=False)
 @click.option("--remote", help="Show Remote Code Runs", default= "")
 @click.pass_context
 def list(ctx, debug, remote) -> None:
     """Commands to list data_product(s) and code_run(s)"""
@@ -132,16 +131,15 @@
             os.getcwd(), debug=debug, server_mode=fdp_svr.SwitchMode.CLI
         ) as fair_session:
             fair_session.show_all_data_products(remote = remote)
     except fdp_exc.FAIRCLIException as e:
         if debug:
             raise e
         e.err_print()
-        if e.level.lower() == "error":
-            sys.exit(e.exit_code)
+        sys.exit(e.exit_code)
 
 @list.command()
 @click.pass_context
 def code_runs(ctx) -> None:
     debug = ctx.obj['DEBUG']
     remote = ctx.obj['REMOTE']
     try:
@@ -149,16 +147,15 @@
             os.getcwd(), debug=debug, server_mode=fdp_svr.SwitchMode.CLI
         ) as fair_session:
             fair_session.show_all_code_runs(remote = remote)
     except fdp_exc.FAIRCLIException as e:
         if debug:
             raise e
         e.err_print()
-        if e.level.lower() == "error":
-            sys.exit(e.exit_code)
+        sys.exit(e.exit_code)
 
 @cli.command()
 @click.option("--debug/--no-debug", help="Run in debug mode", default=False)
 @click.argument("output", nargs=-1)
 def create(debug, output: str) -> None:
     """Generate a new FAIR repository user YAML config file"""
     output = (
@@ -180,16 +177,15 @@
             os.getcwd(), debug=debug, server_mode=fdp_svr.SwitchMode.CLI
         ) as fair_session:
             fair_session.reset_staging()
     except fdp_exc.FAIRCLIException as e:
         if debug:
             raise e
         e.err_print()
-        if e.level.lower() == "error":
-            sys.exit(e.exit_code)
+        sys.exit(e.exit_code)
 
 
 @cli.command()
 @click.option(
     "--config",
     help="Create a starter user config.yaml file during initialisation",
     default=None,
@@ -251,16 +247,15 @@
             )
             if config:
                 fair_session.make_starter_config(config)
     except fdp_exc.FAIRCLIException as e:
         if debug:
             raise e
         e.err_print()
-        if e.level.lower() == "error":
-            sys.exit(e.exit_code)
+        sys.exit(e.exit_code)
 
 
 @cli.command()
 @click.option(
     "glob",
     "--global/--no-global",
     help="Also delete global FAIR-CLI directories",
@@ -308,16 +303,15 @@
     try:
         with fdp_session.FAIR(os.getcwd()) as fair_session:
             fair_session.purge(global_cfg=glob, clear_data=data, clear_all=all)
     except fdp_exc.FAIRCLIException as e:
         if debug:
             raise e
         e.err_print()
-        if e.level.lower() == "error":
-            sys.exit(e.exit_code)
+        sys.exit(e.exit_code)
 
 
 @cli.group()
 def registry() -> None:
     """Commands relating to control of the local registry server"""
     pass
 
@@ -336,16 +330,15 @@
         if debug:
             logging.getLogger("FAIRDataPipeline").setLevel(logging.DEBUG)
         fdp_svr.uninstall_registry()
     except fdp_exc.FAIRCLIException as e:
         if debug:
             raise e
         e.err_print()
-        if e.level.lower() == "error":
-            sys.exit(e.exit_code)
+        sys.exit(e.exit_code)
 
 
 @registry.command()
 @click.option("--force/--no-force", help="Force a reinstall", default=False)
 @click.option("--debug/--no-debug", help="Run in debug mode", default=False)
 @click.option("--directory", help="Installation location", default=None)
 @click.option(
@@ -362,16 +355,15 @@
             install_dir=directory, reference=version, force=force
         )
         click.echo(f"Installed registry version '{_version}'")
     except fdp_exc.FAIRCLIException as e:
         if debug:
             raise e
         e.err_print()
-        if e.level.lower() == "error":
-            sys.exit(e.exit_code)
+        sys.exit(e.exit_code)
 
 
 @registry.command()
 @click.option("--debug/--no-debug", help="Run in debug mode", default=False)
 @click.option("--port", help="port on which to run registry", default=8000)
 @click.option("--address", help="Address on which to run registry", default="127.0.0.1")
 def start(debug: bool, port: int, address: str) -> None:
@@ -384,16 +376,15 @@
             server_port=port,
             server_address=address
         )
     except fdp_exc.FAIRCLIException as e:
         if debug:
             raise e
         e.err_print()
-        if e.level.lower() == "error":
-            sys.exit(e.exit_code)
+        sys.exit(e.exit_code)
 
 
 @registry.command()
 @click.option("--force/--no-force", help="Force server stop", default=False)
 @click.option("--debug/--no-debug", help="Run in debug mode", default=False)
 def stop(force: bool, debug: bool) -> None:
     """Stop the local registry server"""
@@ -404,61 +395,57 @@
     )
     try:
         fdp_session.FAIR(os.getcwd(), server_mode=_mode, debug=debug)
     except fdp_exc.FAIRCLIException as e:
         if debug:
             raise e
         e.err_print()
-        if e.level.lower() == "error":
-            sys.exit(e.exit_code)
+        sys.exit(e.exit_code)
 
 
 @registry.command()
 @click.option("--debug/--no-debug", help="Run in debug mode", default=False)
 def status(debug) -> None:
     try:
         with fdp_session.FAIR(
             os.getcwd(), debug=debug, server_mode=fdp_svr.SwitchMode.NO_SERVER
         ) as fair_session:
             fair_session.registry_status()
     except fdp_exc.FAIRCLIException as e:
         if debug:
             raise e
         e.err_print()
-        if e.level.lower() == "error":
-            sys.exit(e.exit_code)
+        sys.exit(e.exit_code)
 
 
 @cli.command()
 @click.option("--debug/--no-debug", help="Run in debug mode", default=False)
 def log(debug: bool) -> None:
     """Show a full job history"""
     try:
         fdp_hist.show_history(os.getcwd())
     except fdp_exc.FAIRCLIException as e:
         if debug:
             raise e
         e.err_print()
-        if e.level.lower() == "error":
-            sys.exit(e.exit_code)
+        sys.exit(e.exit_code)
 
 
 @cli.command()
 @click.option("--debug/--no-debug", help="Run in debug mode", default=False)
 @click.argument("job_id", shell_complete=complete_jobs)
 def view(job_id: str, debug: bool) -> None:
     """View log for a given job"""
     try:
         fdp_hist.show_job_log(os.getcwd(), job_id)
     except fdp_exc.FAIRCLIException as e:
         if debug:
             raise e
         e.err_print()
-        if e.level.lower() == "error":
-            sys.exit(e.exit_code)
+        sys.exit(e.exit_code)
 
 
 @cli.command()
 @click.argument("identifier")
 @click.option("--debug/--no-debug", help="Run in debug mode", default=False)
 @click.option("-j", "--job/--no-job", help="Stage entire job", default=False)
 def unstage(identifier: str, debug: bool, job: bool) -> None:
@@ -473,16 +460,15 @@
                 job,
                 stage=False,
             )
     except fdp_exc.FAIRCLIException as e:
         if debug:
             raise e
         e.err_print()
-        if e.level.lower() == "error":
-            sys.exit(e.exit_code)
+        sys.exit(e.exit_code)
 
 
 @cli.command()
 @click.argument("identifier", shell_complete=complete_data_products)
 @click.option("--debug/--no-debug", help="Run in debug mode", default=False)
 def add(identifier: str, debug: bool) -> None:
     """
@@ -506,16 +492,15 @@
             fair_session.add_to_staging(
                 identifier
             )
     except fdp_exc.FAIRCLIException as e:
         if debug:
             raise e
         e.err_print()
-        if e.level.lower() == "error":
-            sys.exit(e.exit_code)
+        sys.exit(e.exit_code)
 
 
 @cli.command()
 @click.argument("job_ids", nargs=-1)
 @click.option("--debug/--no-debug", help="Run in debug mode", default=False)
 @click.option(
     "--cached/--not-cached",
@@ -572,16 +557,15 @@
             )
             if ci:
                 click.echo(fdp_run.get_job_dir(_hash))
     except fdp_exc.FAIRCLIException as e:
         if debug:
             raise e
         e.err_print()
-        if e.level.lower() == "error":
-            sys.exit(e.exit_code)
+        sys.exit(e.exit_code)
 
 
 @cli.group(invoke_without_command=True)
 @click.option("--verbose/--no-verbose", "-v/")
 @click.option("--debug/--no-debug", help="Run in debug mode", default=False)
 @click.pass_context
 def remote(ctx, verbose: bool = False, debug: bool = False):
@@ -590,16 +574,15 @@
         try:
             with fdp_session.FAIR(os.getcwd(), debug=debug) as fair_session:
                 fair_session.list_remotes(verbose)
         except fdp_exc.FAIRCLIException as e:
             if debug:
                 raise e
             e.err_print()
-            if e.level.lower() == "error":
-                sys.exit(e.exit_code)
+            sys.exit(e.exit_code)
 
 
 @remote.command()
 @click.argument("options", nargs=-1)
 @click.option("--debug/--no-debug", help="Run in debug mode", default=False)
 def add(options: typing.List[str], debug: bool) -> None:
     """Add a remote registry URL with option to give it a label if multiple
@@ -618,16 +601,15 @@
     try:
         with fdp_session.FAIR(os.getcwd(), debug=debug) as fair_session:
             fair_session.add_remote(_url, _label)
     except fdp_exc.FAIRCLIException as e:
         if debug:
             raise e
         e.err_print()
-        if e.level.lower() == "error":
-            sys.exit(e.exit_code)
+        sys.exit(e.exit_code)
 
 
 @remote.command()
 @click.argument("label")
 @click.option("--debug/--no-debug", help="Run in debug mode", default=False)
 def remove(label: str, debug: bool) -> None:
     """Removes the specified remote from the remotes list
@@ -640,16 +622,15 @@
     try:
         with fdp_session.FAIR(os.getcwd(), debug=debug) as fair_session:
             fair_session.remove_remove(label)
     except fdp_exc.FAIRCLIException as e:
         if debug:
             raise e
         e.err_print()
-        if e.level.lower() == "error":
-            sys.exit(e.exit_code)
+        sys.exit(e.exit_code)
 
 
 @remote.command()
 @click.argument("label")
 @click.argument("url")
 @click.pass_context
 @click.option("--debug/--no-debug", help="Run in debug mode", default=False)
@@ -658,16 +639,15 @@
     try:
         with fdp_session.FAIR(os.getcwd(), debug=debug) as fair_session:
             fair_session.modify_remote(label, url)
     except fdp_exc.FAIRCLIException as e:
         if debug:
             raise e
         e.err_print()
-        if e.level.lower() == "error":
-            sys.exit(e.exit_code)
+        sys.exit(e.exit_code)
 
 
 @cli.command()
 @click.argument("remote", nargs=-1)
 @click.option("--debug/--no-debug", help="Run in debug mode", default=False)
 @click.option(
     "--dirty/--clean",
@@ -685,16 +665,15 @@
             allow_dirty=dirty,
         ) as fair_session:
             fair_session.push(remote)
     except fdp_exc.FAIRCLIException as e:
         if debug:
             raise e
         e.err_print()
-        if e.level.lower() == "error":
-            sys.exit(e.exit_code)
+        sys.exit(e.exit_code)
 
 
 @cli.group()
 def config():
     """Configure user information"""
     pass
 
@@ -732,13 +711,12 @@
             allow_dirty=True,
         ) as fair:
             fair.pull()
     except fdp_exc.FAIRCLIException as e:
         if debug:
             raise e
         e.err_print()
-        if e.level.lower() == "error":
-            sys.exit(e.exit_code)
+        sys.exit(e.exit_code)
 
 
 if __name__ in "__main__":
     cli(obj={})
```

### Comparing `fair_cli-0.7.0/fair/common.py` & `fair_cli-0.7.1/fair/common.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.7.0/fair/configuration/__init__.py` & `fair_cli-0.7.1/fair/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.7.0/fair/configuration/validation.py` & `fair_cli-0.7.1/fair/configuration/validation.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.7.0/fair/exceptions.py` & `fair_cli-0.7.1/fair/exceptions.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.7.0/fair/files.txt` & `fair_cli-0.7.1/fair/files.txt`

 * *Files identical despite different names*

### Comparing `fair_cli-0.7.0/fair/history.py` & `fair_cli-0.7.1/fair/history.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.7.0/fair/identifiers.py` & `fair_cli-0.7.1/fair/identifiers.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.7.0/fair/logging.py` & `fair_cli-0.7.1/fair/logging.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.7.0/fair/register.py` & `fair_cli-0.7.1/fair/register.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.7.0/fair/registry/file_formats.json` & `fair_cli-0.7.1/fair/registry/file_formats.json`

 * *Files identical despite different names*

### Comparing `fair_cli-0.7.0/fair/registry/requests.py` & `fair_cli-0.7.1/fair/registry/requests.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,16 +86,16 @@
         )
 
     return _file_lines[0].strip()
 
 
 def _access(
     uri: str,
-    method: str,
-    token: str,
+    method: str = None,
+    token: str = None,
     obj_path: str = None,
     response_codes: typing.List[int] = None,
     headers: typing.Dict[str, typing.Any] = None,
     params: typing.Dict = None,
     data: typing.Dict = None,
     files: typing.Dict = None,
     trailing_slash = True,
```

### Comparing `fair_cli-0.7.0/fair/registry/server.py` & `fair_cli-0.7.1/fair/registry/server.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.7.0/fair/registry/storage.py` & `fair_cli-0.7.1/fair/registry/storage.py`

 * *Files 0% similar despite different names*

```diff
@@ -831,17 +831,17 @@
         remote_token (str, optional): Remote Registry Token. Defaults to None.
 
     Returns:
         str: Ad upload url for object storage
     """
     file_hash = calculate_file_hash(file_loc)
     if not remote_uri: 
-        remote_uri = fdp_conf.get_remote_token()
+        remote_uri = fdp_conf.get_remote_uri(fdp_conf._session_loc)
     if not remote_token:
-        remote_token = fdp_conf.get_remote_token()
+        remote_token = fdp_conf.get_remote_token(fdp_conf._session_loc)
     return fdp_req.post_upload_url(remote_uri, remote_token, file_hash)['url']
 
 def upload_remote_file(
     file_loc: str,
     remote_uri = None,
     remote_token = None,
 ):
```

### Comparing `fair_cli-0.7.0/fair/registry/sync.py` & `fair_cli-0.7.1/fair/registry/sync.py`

 * *Files 0% similar despite different names*

```diff
@@ -814,14 +814,16 @@
     Args:
         data_product_url (str): data_product url
         token (str): token to the relevent regisrty
 
     Returns:
         str: formatted data_product as string in the format: {namespace_name}:{data_product_name}@v{data_product_version}
     """
+    if not format_data_product_list([data_product_url], token):
+        return ""
     return(format_data_product_list([data_product_url], token)[0])
 
 def get_dest_inputs(origin_inputs: typing.List, 
     origin_uri: str,
     dest_uri: str,
     dest_token: str,
     origin_token: str,
```

### Comparing `fair_cli-0.7.0/fair/registry/versioning.py` & `fair_cli-0.7.1/fair/registry/versioning.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.7.0/fair/run.py` & `fair_cli-0.7.1/fair/run.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.7.0/fair/session.py` & `fair_cli-0.7.1/fair/session.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.7.0/fair/staging.py` & `fair_cli-0.7.1/fair/staging.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.7.0/fair/testing.py` & `fair_cli-0.7.1/fair/testing.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.7.0/fair/user_config/__init__.py` & `fair_cli-0.7.1/fair/user_config/__init__.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.7.0/fair/user_config/globbing.py` & `fair_cli-0.7.1/fair/user_config/globbing.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.7.0/fair/user_config/validation.py` & `fair_cli-0.7.1/fair/user_config/validation.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.7.0/fair/utilities.py` & `fair_cli-0.7.1/fair/utilities.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.7.0/fair/virtualenv.py` & `fair_cli-0.7.1/fair/virtualenv.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.7.0/pyproject.toml` & `fair_cli-0.7.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
   "Environment :: Console",
   "Operating System :: POSIX :: Linux",
   "Operating System :: MacOS",
   "Operating System :: OS Independent",
 ]
 description = "Synchronization interface for the SCRC FAIR Data Pipeline registry"
 name = "fair-cli"
-version = "0.7.0"
+version = "0.7.1"
 
 homepage = "https://www.fairdatapipeline.org/"
 
 repository = "https://github.com/FAIRDataPipeline/FAIR-CLI"
 
 documentation = "https://www.fairdatapipeline.org/docs/interface/fdp/"
```

### Comparing `fair_cli-0.7.0/PKG-INFO` & `fair_cli-0.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fair-cli
-Version: 0.7.0
+Version: 0.7.1
 Summary: Synchronization interface for the SCRC FAIR Data Pipeline registry
 Home-page: https://www.fairdatapipeline.org/
 License: BSD-2-Clause
 Keywords: FAIR Data Pipeline,FAIR,Data Management,Provenance
 Author: Richard Reeve
 Author-email: richard.reeve@glasgow.ac.uk
 Requires-Python: >=3.8.0,<4.0.0
@@ -16,19 +16,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Database :: Front-Ends
 Classifier: Topic :: Scientific/Engineering
 Provides-Extra: all
 Requires-Dist: GitPython (>=3.1.18,<4.0.0)
 Requires-Dist: Jinja2 (>=3.0.1,<4.0.0)
 Requires-Dist: PyYAML (>=5.4.1,<7.0.0)
 Requires-Dist: click (>=8.0.0,<9.0.0)
```

