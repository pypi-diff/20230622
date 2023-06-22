# Comparing `tmp/fair_cli-0.7.2.tar.gz` & `tmp/fair_cli-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fair_cli-0.7.2.tar", max compression
+gzip compressed data, was "fair_cli-0.7.3.tar", max compression
```

## Comparing `fair_cli-0.7.2.tar` & `fair_cli-0.7.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1855 2023-06-21 19:13:33.324048 fair_cli-0.7.2/CHANGELOG.md
--rw-r--r--   0        0        0     1358 2023-06-22 17:26:01.247450 fair_cli-0.7.2/CITATION.cff
--rw-r--r--   0        0        0     1314 2023-06-12 13:03:22.463351 fair_cli-0.7.2/LICENSE
--rw-r--r--   0        0        0    11363 2023-06-21 19:13:33.324484 fair_cli-0.7.2/README.md
--rw-r--r--   0        0        0     1976 2023-06-12 13:03:22.464552 fair_cli-0.7.2/fair/__init__.py
--rw-r--r--   0        0        0    20495 2023-06-22 17:24:07.662164 fair_cli-0.7.2/fair/cli.py
--rw-r--r--   0        0        0     9190 2023-06-21 19:13:33.326523 fair_cli-0.7.2/fair/common.py
--rw-r--r--   0        0        0    28212 2023-06-21 19:13:33.326880 fair_cli-0.7.2/fair/configuration/__init__.py
--rw-r--r--   0        0        0     3311 2023-06-21 19:13:33.326964 fair_cli-0.7.2/fair/configuration/validation.py
--rw-r--r--   0        0        0     5358 2023-06-21 19:13:33.327099 fair_cli-0.7.2/fair/exceptions.py
--rw-r--r--   0        0        0    10127 2023-06-21 19:13:33.327168 fair_cli-0.7.2/fair/files.txt
--rw-r--r--   0        0        0     4619 2023-06-21 19:13:33.327283 fair_cli-0.7.2/fair/history.py
--rw-r--r--   0        0        0     3958 2023-06-21 19:13:33.327397 fair_cli-0.7.2/fair/identifiers.py
--rw-r--r--   0        0        0     3010 2023-06-21 19:13:33.327463 fair_cli-0.7.2/fair/logging.py
--rw-r--r--   0        0        0     8206 2023-06-21 19:13:33.327581 fair_cli-0.7.2/fair/register.py
--rw-r--r--   0        0        0      161 2023-06-21 19:13:33.327663 fair_cli-0.7.2/fair/registry/__init__.py
--rw-r--r--   0        0        0     1249 2023-06-12 13:03:22.465501 fair_cli-0.7.2/fair/registry/file_formats.json
--rw-r--r--   0        0        0      120 2023-06-12 13:03:22.465547 fair_cli-0.7.2/fair/registry/file_types.py
--rw-r--r--   0        0        0    17292 2023-06-22 15:55:58.649339 fair_cli-0.7.2/fair/registry/requests.py
--rw-r--r--   0        0        0    14756 2023-06-21 19:13:33.328007 fair_cli-0.7.2/fair/registry/server.py
--rw-r--r--   0        0        0    23733 2023-06-22 15:55:58.649688 fair_cli-0.7.2/fair/registry/storage.py
--rw-r--r--   0        0        0    38515 2023-06-22 15:55:58.650104 fair_cli-0.7.2/fair/registry/sync.py
--rw-r--r--   0        0        0     4752 2023-06-21 19:13:33.329007 fair_cli-0.7.2/fair/registry/versioning.py
--rw-r--r--   0        0        0     2302 2023-06-21 19:13:33.329217 fair_cli-0.7.2/fair/run.py
--rw-r--r--   0        0        0    49608 2023-06-21 19:13:33.329700 fair_cli-0.7.2/fair/session.py
--rw-r--r--   0        0        0    16133 2023-06-21 19:13:33.329852 fair_cli-0.7.2/fair/staging.py
--rw-r--r--   0        0        0      490 2023-06-12 13:03:22.466460 fair_cli-0.7.2/fair/templates/__init__.py
--rw-r--r--   0        0        0      296 2023-06-12 13:03:22.466514 fair_cli-0.7.2/fair/templates/config.jinja
--rw-r--r--   0        0        0      136 2023-06-12 13:03:22.466556 fair_cli-0.7.2/fair/templates/hist.jinja
--rw-r--r--   0        0        0     3181 2023-06-21 19:13:33.329963 fair_cli-0.7.2/fair/testing.py
--rw-r--r--   0        0        0    53662 2023-06-22 16:29:13.604131 fair_cli-0.7.2/fair/user_config/__init__.py
--rw-r--r--   0        0        0     4830 2023-06-21 19:13:33.330469 fair_cli-0.7.2/fair/user_config/globbing.py
--rw-r--r--   0        0        0     9187 2023-06-21 19:13:33.330549 fair_cli-0.7.2/fair/user_config/validation.py
--rw-r--r--   0        0        0     5087 2023-06-21 19:13:33.330678 fair_cli-0.7.2/fair/utilities.py
--rw-r--r--   0        0        0     1465 2023-06-21 19:13:33.330742 fair_cli-0.7.2/fair/virtualenv.py
--rw-r--r--   0        0        0     2563 2023-06-22 17:26:09.794823 fair_cli-0.7.2/pyproject.toml
--rw-r--r--   0        0        0    13296 1970-01-01 00:00:00.000000 fair_cli-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0     1855 2023-06-21 19:13:33.324048 fair_cli-0.7.3/CHANGELOG.md
+-rw-r--r--   0        0        0     1358 2023-06-22 21:33:37.591898 fair_cli-0.7.3/CITATION.cff
+-rw-r--r--   0        0        0     1314 2023-06-12 13:03:22.463351 fair_cli-0.7.3/LICENSE
+-rw-r--r--   0        0        0    11363 2023-06-21 19:13:33.324484 fair_cli-0.7.3/README.md
+-rw-r--r--   0        0        0     1976 2023-06-12 13:03:22.464552 fair_cli-0.7.3/fair/__init__.py
+-rw-r--r--   0        0        0    21491 2023-06-22 21:28:17.110682 fair_cli-0.7.3/fair/cli.py
+-rw-r--r--   0        0        0     9190 2023-06-21 19:13:33.326523 fair_cli-0.7.3/fair/common.py
+-rw-r--r--   0        0        0    28212 2023-06-21 19:13:33.326880 fair_cli-0.7.3/fair/configuration/__init__.py
+-rw-r--r--   0        0        0     3311 2023-06-21 19:13:33.326964 fair_cli-0.7.3/fair/configuration/validation.py
+-rw-r--r--   0        0        0     5358 2023-06-21 19:13:33.327099 fair_cli-0.7.3/fair/exceptions.py
+-rw-r--r--   0        0        0    10127 2023-06-21 19:13:33.327168 fair_cli-0.7.3/fair/files.txt
+-rw-r--r--   0        0        0     4619 2023-06-21 19:13:33.327283 fair_cli-0.7.3/fair/history.py
+-rw-r--r--   0        0        0     3958 2023-06-21 19:13:33.327397 fair_cli-0.7.3/fair/identifiers.py
+-rw-r--r--   0        0        0     3010 2023-06-21 19:13:33.327463 fair_cli-0.7.3/fair/logging.py
+-rw-r--r--   0        0        0     8206 2023-06-21 19:13:33.327581 fair_cli-0.7.3/fair/register.py
+-rw-r--r--   0        0        0      161 2023-06-21 19:13:33.327663 fair_cli-0.7.3/fair/registry/__init__.py
+-rw-r--r--   0        0        0     1249 2023-06-12 13:03:22.465501 fair_cli-0.7.3/fair/registry/file_formats.json
+-rw-r--r--   0        0        0      120 2023-06-12 13:03:22.465547 fair_cli-0.7.3/fair/registry/file_types.py
+-rw-r--r--   0        0        0    17292 2023-06-22 15:55:58.649339 fair_cli-0.7.3/fair/registry/requests.py
+-rw-r--r--   0        0        0    14756 2023-06-21 19:13:33.328007 fair_cli-0.7.3/fair/registry/server.py
+-rw-r--r--   0        0        0    23733 2023-06-22 15:55:58.649688 fair_cli-0.7.3/fair/registry/storage.py
+-rw-r--r--   0        0        0    38515 2023-06-22 15:55:58.650104 fair_cli-0.7.3/fair/registry/sync.py
+-rw-r--r--   0        0        0     4752 2023-06-21 19:13:33.329007 fair_cli-0.7.3/fair/registry/versioning.py
+-rw-r--r--   0        0        0     2302 2023-06-21 19:13:33.329217 fair_cli-0.7.3/fair/run.py
+-rw-r--r--   0        0        0    49608 2023-06-21 19:13:33.329700 fair_cli-0.7.3/fair/session.py
+-rw-r--r--   0        0        0    16133 2023-06-21 19:13:33.329852 fair_cli-0.7.3/fair/staging.py
+-rw-r--r--   0        0        0      490 2023-06-12 13:03:22.466460 fair_cli-0.7.3/fair/templates/__init__.py
+-rw-r--r--   0        0        0      296 2023-06-12 13:03:22.466514 fair_cli-0.7.3/fair/templates/config.jinja
+-rw-r--r--   0        0        0      136 2023-06-12 13:03:22.466556 fair_cli-0.7.3/fair/templates/hist.jinja
+-rw-r--r--   0        0        0     3181 2023-06-21 19:13:33.329963 fair_cli-0.7.3/fair/testing.py
+-rw-r--r--   0        0        0    53662 2023-06-22 16:29:13.604131 fair_cli-0.7.3/fair/user_config/__init__.py
+-rw-r--r--   0        0        0     4830 2023-06-21 19:13:33.330469 fair_cli-0.7.3/fair/user_config/globbing.py
+-rw-r--r--   0        0        0     9187 2023-06-21 19:13:33.330549 fair_cli-0.7.3/fair/user_config/validation.py
+-rw-r--r--   0        0        0     5087 2023-06-21 19:13:33.330678 fair_cli-0.7.3/fair/utilities.py
+-rw-r--r--   0        0        0     1465 2023-06-21 19:13:33.330742 fair_cli-0.7.3/fair/virtualenv.py
+-rw-r--r--   0        0        0     2563 2023-06-22 21:33:27.711998 fair_cli-0.7.3/pyproject.toml
+-rw-r--r--   0        0        0    13296 1970-01-01 00:00:00.000000 fair_cli-0.7.3/PKG-INFO
```

### Comparing `fair_cli-0.7.2/CHANGELOG.md` & `fair_cli-0.7.3/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `fair_cli-0.7.2/CITATION.cff` & `fair_cli-0.7.3/CITATION.cff`

 * *Files 0% similar despite different names*

```diff
@@ -32,8 +32,8 @@
 - FAIR
 - Data Management
 - Provenance
 license: BSD-2-Clause
 message: If you use this software, please cite it using these metadata.
 repository-code: https://github.com/FAIRDataPipeline/FAIR-CLI/
 title: "The FAIR Data Pipeline command line tool"
-version: 0.7.2
+version: 0.7.3
```

### Comparing `fair_cli-0.7.2/LICENSE` & `fair_cli-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fair_cli-0.7.2/README.md` & `fair_cli-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `fair_cli-0.7.2/fair/__init__.py` & `fair_cli-0.7.3/fair/__init__.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.7.2/fair/cli.py` & `fair_cli-0.7.3/fair/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -100,15 +100,17 @@
         with fdp_session.FAIR(
             os.getcwd(), debug=debug, server_mode=fdp_svr.SwitchMode.CLI
         ) as fair_session:
             fair_session.status_data_products()
             fair_session.status_code_runs()
     except fdp_exc.FAIRCLIException as e:
         e.err_print()
-        sys.exit(e.exit_code)
+        if e.level.lower() == "error":
+            if e.level.lower() == "error":
+                sys.exit(e.exit_code)
 
 @cli.group(invoke_without_command=True)
 @click.option("--debug/--no-debug", help="Run in debug mode", default=False)
 @click.option("--remote", help="Show Remote Code Runs", default= "")
 @click.pass_context
 def list(ctx, debug, remote) -> None:
     """Commands to list data_product(s) and code_run(s)"""
@@ -127,29 +129,31 @@
     try:
         with fdp_session.FAIR(
             os.getcwd(), debug=debug, server_mode=fdp_svr.SwitchMode.CLI
         ) as fair_session:
             fair_session.show_all_data_products(remote = remote)
     except fdp_exc.FAIRCLIException as e:
         e.err_print()
-        sys.exit(e.exit_code)
+        if e.level.lower() == "error":
+            sys.exit(e.exit_code)
 
 @list.command()
 @click.pass_context
 def code_runs(ctx) -> None:
     debug = ctx.obj['DEBUG']
     remote = ctx.obj['REMOTE']
     try:
         with fdp_session.FAIR(
             os.getcwd(), debug=debug, server_mode=fdp_svr.SwitchMode.CLI
         ) as fair_session:
             fair_session.show_all_code_runs(remote = remote)
     except fdp_exc.FAIRCLIException as e:
         e.err_print()
-        sys.exit(e.exit_code)
+        if e.level.lower() == "error":
+            sys.exit(e.exit_code)
 
 @cli.command()
 @click.option("--debug/--no-debug", help="Run in debug mode", default=False)
 @click.argument("output", nargs=-1)
 def create(debug, output: str) -> None:
     """Generate a new FAIR repository user YAML config file"""
     output = (
@@ -169,15 +173,16 @@
     try:
         with fdp_session.FAIR(
             os.getcwd(), debug=debug, server_mode=fdp_svr.SwitchMode.CLI
         ) as fair_session:
             fair_session.reset_staging()
     except fdp_exc.FAIRCLIException as e:
         e.err_print()
-        sys.exit(e.exit_code)
+        if e.level.lower() == "error":
+            sys.exit(e.exit_code)
 
 
 @cli.command()
 @click.option(
     "--config",
     help="Create a starter user config.yaml file during initialisation",
     default=None,
@@ -237,16 +242,16 @@
                 export_as=export,
                 local=local,
             )
             if config:
                 fair_session.make_starter_config(config)
     except fdp_exc.FAIRCLIException as e:
         e.err_print()
-        sys.exit(e.exit_code)
-
+        if e.level.lower() == "error":
+            sys.exit(e.exit_code)
 
 @cli.command()
 @click.option(
     "glob",
     "--global/--no-global",
     help="Also delete global FAIR-CLI directories",
     default=False,
@@ -291,15 +296,16 @@
             return
 
     try:
         with fdp_session.FAIR(os.getcwd()) as fair_session:
             fair_session.purge(global_cfg=glob, clear_data=data, clear_all=all)
     except fdp_exc.FAIRCLIException as e:
         e.err_print()
-        sys.exit(e.exit_code)
+        if e.level.lower() == "error":
+            sys.exit(e.exit_code)
 
 
 @cli.group()
 def registry() -> None:
     """Commands relating to control of the local registry server"""
     pass
 
@@ -316,15 +322,16 @@
         return
     try:
         if debug:
             logging.getLogger("FAIRDataPipeline").setLevel(logging.DEBUG)
         fdp_svr.uninstall_registry()
     except fdp_exc.FAIRCLIException as e:
         e.err_print()
-        sys.exit(e.exit_code)
+        if e.level.lower() == "error":
+            sys.exit(e.exit_code)
 
 
 @registry.command()
 @click.option("--force/--no-force", help="Force a reinstall", default=False)
 @click.option("--debug/--no-debug", help="Run in debug mode", default=False)
 @click.option("--directory", help="Installation location", default=None)
 @click.option(
@@ -339,15 +346,16 @@
             logging.getLogger("FAIRDataPipeline").setLevel(logging.DEBUG)
         _version = fdp_svr.install_registry(
             install_dir=directory, reference=version, force=force
         )
         click.echo(f"Installed registry version '{_version}'")
     except fdp_exc.FAIRCLIException as e:
         e.err_print()
-        sys.exit(e.exit_code)
+        if e.level.lower() == "error":
+            sys.exit(e.exit_code)
 
 
 @registry.command()
 @click.option("--debug/--no-debug", help="Run in debug mode", default=False)
 @click.option("--port", help="port on which to run registry", default=8000)
 @click.option("--address", help="Address on which to run registry", default="127.0.0.1")
 def start(debug: bool, port: int, address: str) -> None:
@@ -358,15 +366,16 @@
             server_mode=fdp_svr.SwitchMode.USER_START,
             debug=debug,
             server_port=port,
             server_address=address
         )
     except fdp_exc.FAIRCLIException as e:
         e.err_print()
-        sys.exit(e.exit_code)
+        if e.level.lower() == "error":
+            sys.exit(e.exit_code)
 
 
 @registry.command()
 @click.option("--force/--no-force", help="Force server stop", default=False)
 @click.option("--debug/--no-debug", help="Run in debug mode", default=False)
 def stop(force: bool, debug: bool) -> None:
     """Stop the local registry server"""
@@ -375,51 +384,55 @@
         if force
         else fdp_svr.SwitchMode.USER_STOP
     )
     try:
         fdp_session.FAIR(os.getcwd(), server_mode=_mode, debug=debug)
     except fdp_exc.FAIRCLIException as e:
         e.err_print()
-        sys.exit(e.exit_code)
+        if e.level.lower() == "error":
+            sys.exit(e.exit_code)
 
 
 @registry.command()
 @click.option("--debug/--no-debug", help="Run in debug mode", default=False)
 def status(debug) -> None:
     try:
         with fdp_session.FAIR(
             os.getcwd(), debug=debug, server_mode=fdp_svr.SwitchMode.NO_SERVER
         ) as fair_session:
             fair_session.registry_status()
     except fdp_exc.FAIRCLIException as e:
         e.err_print()
-        sys.exit(e.exit_code)
+        if e.level.lower() == "error":
+            sys.exit(e.exit_code)
 
 
 @cli.command()
 @click.option("--debug/--no-debug", help="Run in debug mode", default=False)
 def log(debug: bool) -> None:
     """Show a full job history"""
     try:
         fdp_hist.show_history(os.getcwd())
     except fdp_exc.FAIRCLIException as e:
         e.err_print()
-        sys.exit(e.exit_code)
+        if e.level.lower() == "error":
+            sys.exit(e.exit_code)
 
 
 @cli.command()
 @click.option("--debug/--no-debug", help="Run in debug mode", default=False)
 @click.argument("job_id", shell_complete=complete_jobs)
 def view(job_id: str, debug: bool) -> None:
     """View log for a given job"""
     try:
         fdp_hist.show_job_log(os.getcwd(), job_id)
     except fdp_exc.FAIRCLIException as e:
         e.err_print()
-        sys.exit(e.exit_code)
+        if e.level.lower() == "error":
+            sys.exit(e.exit_code)
 
 
 @cli.command()
 @click.argument("identifier")
 @click.option("--debug/--no-debug", help="Run in debug mode", default=False)
 @click.option("-j", "--job/--no-job", help="Stage entire job", default=False)
 def unstage(identifier: str, debug: bool, job: bool) -> None:
@@ -432,15 +445,16 @@
             fair_session.change_staging_state(
                 identifier,
                 job,
                 stage=False,
             )
     except fdp_exc.FAIRCLIException as e:
         e.err_print()
-        sys.exit(e.exit_code)
+        if e.level.lower() == "error":
+            sys.exit(e.exit_code)
 
 
 @cli.command()
 @click.argument("identifier", shell_complete=complete_data_products)
 @click.option("--debug/--no-debug", help="Run in debug mode", default=False)
 def add(identifier: str, debug: bool) -> None:
     """
@@ -462,15 +476,16 @@
             debug=debug,
         ) as fair_session:
             fair_session.add_to_staging(
                 identifier
             )
     except fdp_exc.FAIRCLIException as e:
         e.err_print()
-        sys.exit(e.exit_code)
+        if e.level.lower() == "error":
+            sys.exit(e.exit_code)
 
 
 @cli.command()
 @click.argument("job_ids", nargs=-1)
 @click.option("--debug/--no-debug", help="Run in debug mode", default=False)
 @click.option(
     "--cached/--not-cached",
@@ -525,30 +540,32 @@
             _hash = fair_session.run(
                 script, passive=ci, allow_dirty=dirty, local=local
             )
             if ci:
                 click.echo(fdp_run.get_job_dir(_hash))
     except fdp_exc.FAIRCLIException as e:
         e.err_print()
-        sys.exit(e.exit_code)
+        if e.level.lower() == "error":
+            sys.exit(e.exit_code)
 
 
 @cli.group(invoke_without_command=True)
 @click.option("--verbose/--no-verbose", "-v/")
 @click.option("--debug/--no-debug", help="Run in debug mode", default=False)
 @click.pass_context
 def remote(ctx, verbose: bool = False, debug: bool = False):
     """List remotes if no additional command is provided"""
     if not ctx.invoked_subcommand:
         try:
             with fdp_session.FAIR(os.getcwd(), debug=debug) as fair_session:
                 fair_session.list_remotes(verbose)
         except fdp_exc.FAIRCLIException as e:
             e.err_print()
-            sys.exit(e.exit_code)
+            if e.level.lower() == "error":
+                sys.exit(e.exit_code)
 
 
 @remote.command()
 @click.argument("options", nargs=-1)
 @click.option("--debug/--no-debug", help="Run in debug mode", default=False)
 def add(options: typing.List[str], debug: bool) -> None:
     """Add a remote registry URL with option to give it a label if multiple
@@ -565,15 +582,16 @@
     _label = options[0] if len(options) > 1 else "origin"
 
     try:
         with fdp_session.FAIR(os.getcwd(), debug=debug) as fair_session:
             fair_session.add_remote(_url, _label)
     except fdp_exc.FAIRCLIException as e:
         e.err_print()
-        sys.exit(e.exit_code)
+        if e.level.lower() == "error":
+            sys.exit(e.exit_code)
 
 
 @remote.command()
 @click.argument("label")
 @click.option("--debug/--no-debug", help="Run in debug mode", default=False)
 def remove(label: str, debug: bool) -> None:
     """Removes the specified remote from the remotes list
@@ -584,30 +602,32 @@
         label of remote to remove
     """
     try:
         with fdp_session.FAIR(os.getcwd(), debug=debug) as fair_session:
             fair_session.remove_remove(label)
     except fdp_exc.FAIRCLIException as e:
         e.err_print()
-        sys.exit(e.exit_code)
+        if e.level.lower() == "error":
+            sys.exit(e.exit_code)
 
 
 @remote.command()
 @click.argument("label")
 @click.argument("url")
 @click.pass_context
 @click.option("--debug/--no-debug", help="Run in debug mode", default=False)
 def modify(ctx, label: str, url: str, debug: bool) -> None:
     """Modify a remote address"""
     try:
         with fdp_session.FAIR(os.getcwd(), debug=debug) as fair_session:
             fair_session.modify_remote(label, url)
     except fdp_exc.FAIRCLIException as e:
         e.err_print()
-        sys.exit(e.exit_code)
+        if e.level.lower() == "error":
+            sys.exit(e.exit_code)
 
 
 @cli.command()
 @click.argument("remote", nargs=-1)
 @click.option("--debug/--no-debug", help="Run in debug mode", default=False)
 @click.option(
     "--dirty/--clean",
@@ -623,15 +643,16 @@
             debug=debug,
             server_mode=fdp_svr.SwitchMode.CLI,
             allow_dirty=dirty,
         ) as fair_session:
             fair_session.push(remote)
     except fdp_exc.FAIRCLIException as e:
         e.err_print()
-        sys.exit(e.exit_code)
+        if e.level.lower() == "error":
+            sys.exit(e.exit_code)
 
 
 @cli.group()
 def config():
     """Configure user information"""
     pass
 
@@ -667,12 +688,13 @@
             debug=debug,
             local=local,
             allow_dirty=True,
         ) as fair:
             fair.pull()
     except fdp_exc.FAIRCLIException as e:
         e.err_print()
-        sys.exit(e.exit_code)
+        if e.level.lower() == "error":
+            sys.exit(e.exit_code)
 
 
 if __name__ in "__main__":
     cli(obj={})
```

### Comparing `fair_cli-0.7.2/fair/common.py` & `fair_cli-0.7.3/fair/common.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.7.2/fair/configuration/__init__.py` & `fair_cli-0.7.3/fair/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.7.2/fair/configuration/validation.py` & `fair_cli-0.7.3/fair/configuration/validation.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.7.2/fair/exceptions.py` & `fair_cli-0.7.3/fair/exceptions.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.7.2/fair/files.txt` & `fair_cli-0.7.3/fair/files.txt`

 * *Files identical despite different names*

### Comparing `fair_cli-0.7.2/fair/history.py` & `fair_cli-0.7.3/fair/history.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.7.2/fair/identifiers.py` & `fair_cli-0.7.3/fair/identifiers.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.7.2/fair/logging.py` & `fair_cli-0.7.3/fair/logging.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.7.2/fair/register.py` & `fair_cli-0.7.3/fair/register.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.7.2/fair/registry/file_formats.json` & `fair_cli-0.7.3/fair/registry/file_formats.json`

 * *Files identical despite different names*

### Comparing `fair_cli-0.7.2/fair/registry/requests.py` & `fair_cli-0.7.3/fair/registry/requests.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.7.2/fair/registry/server.py` & `fair_cli-0.7.3/fair/registry/server.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.7.2/fair/registry/storage.py` & `fair_cli-0.7.3/fair/registry/storage.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.7.2/fair/registry/sync.py` & `fair_cli-0.7.3/fair/registry/sync.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.7.2/fair/registry/versioning.py` & `fair_cli-0.7.3/fair/registry/versioning.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.7.2/fair/run.py` & `fair_cli-0.7.3/fair/run.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.7.2/fair/session.py` & `fair_cli-0.7.3/fair/session.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.7.2/fair/staging.py` & `fair_cli-0.7.3/fair/staging.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.7.2/fair/testing.py` & `fair_cli-0.7.3/fair/testing.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.7.2/fair/user_config/__init__.py` & `fair_cli-0.7.3/fair/user_config/__init__.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.7.2/fair/user_config/globbing.py` & `fair_cli-0.7.3/fair/user_config/globbing.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.7.2/fair/user_config/validation.py` & `fair_cli-0.7.3/fair/user_config/validation.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.7.2/fair/utilities.py` & `fair_cli-0.7.3/fair/utilities.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.7.2/fair/virtualenv.py` & `fair_cli-0.7.3/fair/virtualenv.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.7.2/pyproject.toml` & `fair_cli-0.7.3/pyproject.toml`

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
-version = "0.7.2"
+version = "0.7.3"
 
 homepage = "https://www.fairdatapipeline.org/"
 
 repository = "https://github.com/FAIRDataPipeline/FAIR-CLI"
 
 documentation = "https://www.fairdatapipeline.org/docs/interface/fdp/"
```

### Comparing `fair_cli-0.7.2/PKG-INFO` & `fair_cli-0.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fair-cli
-Version: 0.7.2
+Version: 0.7.3
 Summary: Synchronization interface for the SCRC FAIR Data Pipeline registry
 Home-page: https://www.fairdatapipeline.org/
 License: BSD-2-Clause
 Keywords: FAIR Data Pipeline,FAIR,Data Management,Provenance
 Author: Richard Reeve
 Author-email: richard.reeve@glasgow.ac.uk
 Requires-Python: >=3.8.0,<4.0.0
```

