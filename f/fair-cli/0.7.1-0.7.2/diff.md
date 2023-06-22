# Comparing `tmp/fair_cli-0.7.1.tar.gz` & `tmp/fair_cli-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fair_cli-0.7.1.tar", max compression
+gzip compressed data, was "fair_cli-0.7.2.tar", max compression
```

## Comparing `fair_cli-0.7.1.tar` & `fair_cli-0.7.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1855 2023-06-21 19:13:33.324048 fair_cli-0.7.1/CHANGELOG.md
--rw-r--r--   0        0        0     1358 2023-06-21 19:13:33.324149 fair_cli-0.7.1/CITATION.cff
--rw-r--r--   0        0        0     1314 2023-06-12 13:03:22.463351 fair_cli-0.7.1/LICENSE
--rw-r--r--   0        0        0    11363 2023-06-21 19:13:33.324484 fair_cli-0.7.1/README.md
--rw-r--r--   0        0        0     1976 2023-06-12 13:03:22.464552 fair_cli-0.7.1/fair/__init__.py
--rw-r--r--   0        0        0    21339 2023-06-22 16:57:58.009966 fair_cli-0.7.1/fair/cli.py
--rw-r--r--   0        0        0     9190 2023-06-21 19:13:33.326523 fair_cli-0.7.1/fair/common.py
--rw-r--r--   0        0        0    28212 2023-06-21 19:13:33.326880 fair_cli-0.7.1/fair/configuration/__init__.py
--rw-r--r--   0        0        0     3311 2023-06-21 19:13:33.326964 fair_cli-0.7.1/fair/configuration/validation.py
--rw-r--r--   0        0        0     5358 2023-06-21 19:13:33.327099 fair_cli-0.7.1/fair/exceptions.py
--rw-r--r--   0        0        0    10127 2023-06-21 19:13:33.327168 fair_cli-0.7.1/fair/files.txt
--rw-r--r--   0        0        0     4619 2023-06-21 19:13:33.327283 fair_cli-0.7.1/fair/history.py
--rw-r--r--   0        0        0     3958 2023-06-21 19:13:33.327397 fair_cli-0.7.1/fair/identifiers.py
--rw-r--r--   0        0        0     3010 2023-06-21 19:13:33.327463 fair_cli-0.7.1/fair/logging.py
--rw-r--r--   0        0        0     8206 2023-06-21 19:13:33.327581 fair_cli-0.7.1/fair/register.py
--rw-r--r--   0        0        0      161 2023-06-21 19:13:33.327663 fair_cli-0.7.1/fair/registry/__init__.py
--rw-r--r--   0        0        0     1249 2023-06-12 13:03:22.465501 fair_cli-0.7.1/fair/registry/file_formats.json
--rw-r--r--   0        0        0      120 2023-06-12 13:03:22.465547 fair_cli-0.7.1/fair/registry/file_types.py
--rw-r--r--   0        0        0    17292 2023-06-22 15:55:58.649339 fair_cli-0.7.1/fair/registry/requests.py
--rw-r--r--   0        0        0    14756 2023-06-21 19:13:33.328007 fair_cli-0.7.1/fair/registry/server.py
--rw-r--r--   0        0        0    23733 2023-06-22 15:55:58.649688 fair_cli-0.7.1/fair/registry/storage.py
--rw-r--r--   0        0        0    38515 2023-06-22 15:55:58.650104 fair_cli-0.7.1/fair/registry/sync.py
--rw-r--r--   0        0        0     4752 2023-06-21 19:13:33.329007 fair_cli-0.7.1/fair/registry/versioning.py
--rw-r--r--   0        0        0     2302 2023-06-21 19:13:33.329217 fair_cli-0.7.1/fair/run.py
--rw-r--r--   0        0        0    49608 2023-06-21 19:13:33.329700 fair_cli-0.7.1/fair/session.py
--rw-r--r--   0        0        0    16133 2023-06-21 19:13:33.329852 fair_cli-0.7.1/fair/staging.py
--rw-r--r--   0        0        0      490 2023-06-12 13:03:22.466460 fair_cli-0.7.1/fair/templates/__init__.py
--rw-r--r--   0        0        0      296 2023-06-12 13:03:22.466514 fair_cli-0.7.1/fair/templates/config.jinja
--rw-r--r--   0        0        0      136 2023-06-12 13:03:22.466556 fair_cli-0.7.1/fair/templates/hist.jinja
--rw-r--r--   0        0        0     3181 2023-06-21 19:13:33.329963 fair_cli-0.7.1/fair/testing.py
--rw-r--r--   0        0        0    53662 2023-06-22 16:29:13.604131 fair_cli-0.7.1/fair/user_config/__init__.py
--rw-r--r--   0        0        0     4830 2023-06-21 19:13:33.330469 fair_cli-0.7.1/fair/user_config/globbing.py
--rw-r--r--   0        0        0     9187 2023-06-21 19:13:33.330549 fair_cli-0.7.1/fair/user_config/validation.py
--rw-r--r--   0        0        0     5087 2023-06-21 19:13:33.330678 fair_cli-0.7.1/fair/utilities.py
--rw-r--r--   0        0        0     1465 2023-06-21 19:13:33.330742 fair_cli-0.7.1/fair/virtualenv.py
--rw-r--r--   0        0        0     2563 2023-06-22 16:57:58.010274 fair_cli-0.7.1/pyproject.toml
--rw-r--r--   0        0        0    13296 1970-01-01 00:00:00.000000 fair_cli-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1855 2023-06-21 19:13:33.324048 fair_cli-0.7.2/CHANGELOG.md
+-rw-r--r--   0        0        0     1358 2023-06-22 17:26:01.247450 fair_cli-0.7.2/CITATION.cff
+-rw-r--r--   0        0        0     1314 2023-06-12 13:03:22.463351 fair_cli-0.7.2/LICENSE
+-rw-r--r--   0        0        0    11363 2023-06-21 19:13:33.324484 fair_cli-0.7.2/README.md
+-rw-r--r--   0        0        0     1976 2023-06-12 13:03:22.464552 fair_cli-0.7.2/fair/__init__.py
+-rw-r--r--   0        0        0    20495 2023-06-22 17:24:07.662164 fair_cli-0.7.2/fair/cli.py
+-rw-r--r--   0        0        0     9190 2023-06-21 19:13:33.326523 fair_cli-0.7.2/fair/common.py
+-rw-r--r--   0        0        0    28212 2023-06-21 19:13:33.326880 fair_cli-0.7.2/fair/configuration/__init__.py
+-rw-r--r--   0        0        0     3311 2023-06-21 19:13:33.326964 fair_cli-0.7.2/fair/configuration/validation.py
+-rw-r--r--   0        0        0     5358 2023-06-21 19:13:33.327099 fair_cli-0.7.2/fair/exceptions.py
+-rw-r--r--   0        0        0    10127 2023-06-21 19:13:33.327168 fair_cli-0.7.2/fair/files.txt
+-rw-r--r--   0        0        0     4619 2023-06-21 19:13:33.327283 fair_cli-0.7.2/fair/history.py
+-rw-r--r--   0        0        0     3958 2023-06-21 19:13:33.327397 fair_cli-0.7.2/fair/identifiers.py
+-rw-r--r--   0        0        0     3010 2023-06-21 19:13:33.327463 fair_cli-0.7.2/fair/logging.py
+-rw-r--r--   0        0        0     8206 2023-06-21 19:13:33.327581 fair_cli-0.7.2/fair/register.py
+-rw-r--r--   0        0        0      161 2023-06-21 19:13:33.327663 fair_cli-0.7.2/fair/registry/__init__.py
+-rw-r--r--   0        0        0     1249 2023-06-12 13:03:22.465501 fair_cli-0.7.2/fair/registry/file_formats.json
+-rw-r--r--   0        0        0      120 2023-06-12 13:03:22.465547 fair_cli-0.7.2/fair/registry/file_types.py
+-rw-r--r--   0        0        0    17292 2023-06-22 15:55:58.649339 fair_cli-0.7.2/fair/registry/requests.py
+-rw-r--r--   0        0        0    14756 2023-06-21 19:13:33.328007 fair_cli-0.7.2/fair/registry/server.py
+-rw-r--r--   0        0        0    23733 2023-06-22 15:55:58.649688 fair_cli-0.7.2/fair/registry/storage.py
+-rw-r--r--   0        0        0    38515 2023-06-22 15:55:58.650104 fair_cli-0.7.2/fair/registry/sync.py
+-rw-r--r--   0        0        0     4752 2023-06-21 19:13:33.329007 fair_cli-0.7.2/fair/registry/versioning.py
+-rw-r--r--   0        0        0     2302 2023-06-21 19:13:33.329217 fair_cli-0.7.2/fair/run.py
+-rw-r--r--   0        0        0    49608 2023-06-21 19:13:33.329700 fair_cli-0.7.2/fair/session.py
+-rw-r--r--   0        0        0    16133 2023-06-21 19:13:33.329852 fair_cli-0.7.2/fair/staging.py
+-rw-r--r--   0        0        0      490 2023-06-12 13:03:22.466460 fair_cli-0.7.2/fair/templates/__init__.py
+-rw-r--r--   0        0        0      296 2023-06-12 13:03:22.466514 fair_cli-0.7.2/fair/templates/config.jinja
+-rw-r--r--   0        0        0      136 2023-06-12 13:03:22.466556 fair_cli-0.7.2/fair/templates/hist.jinja
+-rw-r--r--   0        0        0     3181 2023-06-21 19:13:33.329963 fair_cli-0.7.2/fair/testing.py
+-rw-r--r--   0        0        0    53662 2023-06-22 16:29:13.604131 fair_cli-0.7.2/fair/user_config/__init__.py
+-rw-r--r--   0        0        0     4830 2023-06-21 19:13:33.330469 fair_cli-0.7.2/fair/user_config/globbing.py
+-rw-r--r--   0        0        0     9187 2023-06-21 19:13:33.330549 fair_cli-0.7.2/fair/user_config/validation.py
+-rw-r--r--   0        0        0     5087 2023-06-21 19:13:33.330678 fair_cli-0.7.2/fair/utilities.py
+-rw-r--r--   0        0        0     1465 2023-06-21 19:13:33.330742 fair_cli-0.7.2/fair/virtualenv.py
+-rw-r--r--   0        0        0     2563 2023-06-22 17:26:09.794823 fair_cli-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0    13296 1970-01-01 00:00:00.000000 fair_cli-0.7.2/PKG-INFO
```

### Comparing `fair_cli-0.7.1/CHANGELOG.md` & `fair_cli-0.7.2/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `fair_cli-0.7.1/CITATION.cff` & `fair_cli-0.7.2/CITATION.cff`

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
-version: 0.4.0
+version: 0.7.2
```

### Comparing `fair_cli-0.7.1/LICENSE` & `fair_cli-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fair_cli-0.7.1/README.md` & `fair_cli-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `fair_cli-0.7.1/fair/__init__.py` & `fair_cli-0.7.2/fair/__init__.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.7.1/fair/cli.py` & `fair_cli-0.7.2/fair/cli.py`

 * *Files 13% similar despite different names*

```diff
@@ -99,16 +99,14 @@
     try:
         with fdp_session.FAIR(
             os.getcwd(), debug=debug, server_mode=fdp_svr.SwitchMode.CLI
         ) as fair_session:
             fair_session.status_data_products()
             fair_session.status_code_runs()
     except fdp_exc.FAIRCLIException as e:
-        if debug:
-            raise e
         e.err_print()
         sys.exit(e.exit_code)
 
 @cli.group(invoke_without_command=True)
 @click.option("--debug/--no-debug", help="Run in debug mode", default=False)
 @click.option("--remote", help="Show Remote Code Runs", default= "")
 @click.pass_context
@@ -128,32 +126,28 @@
     remote = ctx.obj['REMOTE']
     try:
         with fdp_session.FAIR(
             os.getcwd(), debug=debug, server_mode=fdp_svr.SwitchMode.CLI
         ) as fair_session:
             fair_session.show_all_data_products(remote = remote)
     except fdp_exc.FAIRCLIException as e:
-        if debug:
-            raise e
         e.err_print()
         sys.exit(e.exit_code)
 
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
-        if debug:
-            raise e
         e.err_print()
         sys.exit(e.exit_code)
 
 @cli.command()
 @click.option("--debug/--no-debug", help="Run in debug mode", default=False)
 @click.argument("output", nargs=-1)
 def create(debug, output: str) -> None:
@@ -174,16 +168,14 @@
     """Unstage all items marked for staging"""
     try:
         with fdp_session.FAIR(
             os.getcwd(), debug=debug, server_mode=fdp_svr.SwitchMode.CLI
         ) as fair_session:
             fair_session.reset_staging()
     except fdp_exc.FAIRCLIException as e:
-        if debug:
-            raise e
         e.err_print()
         sys.exit(e.exit_code)
 
 
 @cli.command()
 @click.option(
     "--config",
@@ -244,16 +236,14 @@
                 registry=registry,
                 export_as=export,
                 local=local,
             )
             if config:
                 fair_session.make_starter_config(config)
     except fdp_exc.FAIRCLIException as e:
-        if debug:
-            raise e
         e.err_print()
         sys.exit(e.exit_code)
 
 
 @cli.command()
 @click.option(
     "glob",
@@ -300,16 +290,14 @@
         if not _purge:
             return
 
     try:
         with fdp_session.FAIR(os.getcwd()) as fair_session:
             fair_session.purge(global_cfg=glob, clear_data=data, clear_all=all)
     except fdp_exc.FAIRCLIException as e:
-        if debug:
-            raise e
         e.err_print()
         sys.exit(e.exit_code)
 
 
 @cli.group()
 def registry() -> None:
     """Commands relating to control of the local registry server"""
@@ -327,16 +315,14 @@
     if not _confirm:
         return
     try:
         if debug:
             logging.getLogger("FAIRDataPipeline").setLevel(logging.DEBUG)
         fdp_svr.uninstall_registry()
     except fdp_exc.FAIRCLIException as e:
-        if debug:
-            raise e
         e.err_print()
         sys.exit(e.exit_code)
 
 
 @registry.command()
 @click.option("--force/--no-force", help="Force a reinstall", default=False)
 @click.option("--debug/--no-debug", help="Run in debug mode", default=False)
@@ -352,16 +338,14 @@
         if debug:
             logging.getLogger("FAIRDataPipeline").setLevel(logging.DEBUG)
         _version = fdp_svr.install_registry(
             install_dir=directory, reference=version, force=force
         )
         click.echo(f"Installed registry version '{_version}'")
     except fdp_exc.FAIRCLIException as e:
-        if debug:
-            raise e
         e.err_print()
         sys.exit(e.exit_code)
 
 
 @registry.command()
 @click.option("--debug/--no-debug", help="Run in debug mode", default=False)
 @click.option("--port", help="port on which to run registry", default=8000)
@@ -373,16 +357,14 @@
             os.getcwd(),
             server_mode=fdp_svr.SwitchMode.USER_START,
             debug=debug,
             server_port=port,
             server_address=address
         )
     except fdp_exc.FAIRCLIException as e:
-        if debug:
-            raise e
         e.err_print()
         sys.exit(e.exit_code)
 
 
 @registry.command()
 @click.option("--force/--no-force", help="Force server stop", default=False)
 @click.option("--debug/--no-debug", help="Run in debug mode", default=False)
@@ -392,58 +374,50 @@
         fdp_svr.SwitchMode.FORCE_STOP
         if force
         else fdp_svr.SwitchMode.USER_STOP
     )
     try:
         fdp_session.FAIR(os.getcwd(), server_mode=_mode, debug=debug)
     except fdp_exc.FAIRCLIException as e:
-        if debug:
-            raise e
         e.err_print()
         sys.exit(e.exit_code)
 
 
 @registry.command()
 @click.option("--debug/--no-debug", help="Run in debug mode", default=False)
 def status(debug) -> None:
     try:
         with fdp_session.FAIR(
             os.getcwd(), debug=debug, server_mode=fdp_svr.SwitchMode.NO_SERVER
         ) as fair_session:
             fair_session.registry_status()
     except fdp_exc.FAIRCLIException as e:
-        if debug:
-            raise e
         e.err_print()
         sys.exit(e.exit_code)
 
 
 @cli.command()
 @click.option("--debug/--no-debug", help="Run in debug mode", default=False)
 def log(debug: bool) -> None:
     """Show a full job history"""
     try:
         fdp_hist.show_history(os.getcwd())
     except fdp_exc.FAIRCLIException as e:
-        if debug:
-            raise e
         e.err_print()
         sys.exit(e.exit_code)
 
 
 @cli.command()
 @click.option("--debug/--no-debug", help="Run in debug mode", default=False)
 @click.argument("job_id", shell_complete=complete_jobs)
 def view(job_id: str, debug: bool) -> None:
     """View log for a given job"""
     try:
         fdp_hist.show_job_log(os.getcwd(), job_id)
     except fdp_exc.FAIRCLIException as e:
-        if debug:
-            raise e
         e.err_print()
         sys.exit(e.exit_code)
 
 
 @cli.command()
 @click.argument("identifier")
 @click.option("--debug/--no-debug", help="Run in debug mode", default=False)
@@ -457,16 +431,14 @@
         ) as fair_session:
             fair_session.change_staging_state(
                 identifier,
                 job,
                 stage=False,
             )
     except fdp_exc.FAIRCLIException as e:
-        if debug:
-            raise e
         e.err_print()
         sys.exit(e.exit_code)
 
 
 @cli.command()
 @click.argument("identifier", shell_complete=complete_data_products)
 @click.option("--debug/--no-debug", help="Run in debug mode", default=False)
@@ -489,16 +461,14 @@
             os.getcwd(),
             debug=debug,
         ) as fair_session:
             fair_session.add_to_staging(
                 identifier
             )
     except fdp_exc.FAIRCLIException as e:
-        if debug:
-            raise e
         e.err_print()
         sys.exit(e.exit_code)
 
 
 @cli.command()
 @click.argument("job_ids", nargs=-1)
 @click.option("--debug/--no-debug", help="Run in debug mode", default=False)
@@ -554,16 +524,14 @@
         ) as fair_session:
             _hash = fair_session.run(
                 script, passive=ci, allow_dirty=dirty, local=local
             )
             if ci:
                 click.echo(fdp_run.get_job_dir(_hash))
     except fdp_exc.FAIRCLIException as e:
-        if debug:
-            raise e
         e.err_print()
         sys.exit(e.exit_code)
 
 
 @cli.group(invoke_without_command=True)
 @click.option("--verbose/--no-verbose", "-v/")
 @click.option("--debug/--no-debug", help="Run in debug mode", default=False)
@@ -571,16 +539,14 @@
 def remote(ctx, verbose: bool = False, debug: bool = False):
     """List remotes if no additional command is provided"""
     if not ctx.invoked_subcommand:
         try:
             with fdp_session.FAIR(os.getcwd(), debug=debug) as fair_session:
                 fair_session.list_remotes(verbose)
         except fdp_exc.FAIRCLIException as e:
-            if debug:
-                raise e
             e.err_print()
             sys.exit(e.exit_code)
 
 
 @remote.command()
 @click.argument("options", nargs=-1)
 @click.option("--debug/--no-debug", help="Run in debug mode", default=False)
@@ -598,16 +564,14 @@
     _url = options[1] if len(options) > 1 else options[0]
     _label = options[0] if len(options) > 1 else "origin"
 
     try:
         with fdp_session.FAIR(os.getcwd(), debug=debug) as fair_session:
             fair_session.add_remote(_url, _label)
     except fdp_exc.FAIRCLIException as e:
-        if debug:
-            raise e
         e.err_print()
         sys.exit(e.exit_code)
 
 
 @remote.command()
 @click.argument("label")
 @click.option("--debug/--no-debug", help="Run in debug mode", default=False)
@@ -619,16 +583,14 @@
     label : str
         label of remote to remove
     """
     try:
         with fdp_session.FAIR(os.getcwd(), debug=debug) as fair_session:
             fair_session.remove_remove(label)
     except fdp_exc.FAIRCLIException as e:
-        if debug:
-            raise e
         e.err_print()
         sys.exit(e.exit_code)
 
 
 @remote.command()
 @click.argument("label")
 @click.argument("url")
@@ -636,16 +598,14 @@
 @click.option("--debug/--no-debug", help="Run in debug mode", default=False)
 def modify(ctx, label: str, url: str, debug: bool) -> None:
     """Modify a remote address"""
     try:
         with fdp_session.FAIR(os.getcwd(), debug=debug) as fair_session:
             fair_session.modify_remote(label, url)
     except fdp_exc.FAIRCLIException as e:
-        if debug:
-            raise e
         e.err_print()
         sys.exit(e.exit_code)
 
 
 @cli.command()
 @click.argument("remote", nargs=-1)
 @click.option("--debug/--no-debug", help="Run in debug mode", default=False)
@@ -662,16 +622,14 @@
             os.getcwd(),
             debug=debug,
             server_mode=fdp_svr.SwitchMode.CLI,
             allow_dirty=dirty,
         ) as fair_session:
             fair_session.push(remote)
     except fdp_exc.FAIRCLIException as e:
-        if debug:
-            raise e
         e.err_print()
         sys.exit(e.exit_code)
 
 
 @cli.group()
 def config():
     """Configure user information"""
@@ -708,15 +666,13 @@
             server_mode=fdp_svr.SwitchMode.CLI,
             debug=debug,
             local=local,
             allow_dirty=True,
         ) as fair:
             fair.pull()
     except fdp_exc.FAIRCLIException as e:
-        if debug:
-            raise e
         e.err_print()
         sys.exit(e.exit_code)
 
 
 if __name__ in "__main__":
     cli(obj={})
```

### Comparing `fair_cli-0.7.1/fair/common.py` & `fair_cli-0.7.2/fair/common.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.7.1/fair/configuration/__init__.py` & `fair_cli-0.7.2/fair/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.7.1/fair/configuration/validation.py` & `fair_cli-0.7.2/fair/configuration/validation.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.7.1/fair/exceptions.py` & `fair_cli-0.7.2/fair/exceptions.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.7.1/fair/files.txt` & `fair_cli-0.7.2/fair/files.txt`

 * *Files identical despite different names*

### Comparing `fair_cli-0.7.1/fair/history.py` & `fair_cli-0.7.2/fair/history.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.7.1/fair/identifiers.py` & `fair_cli-0.7.2/fair/identifiers.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.7.1/fair/logging.py` & `fair_cli-0.7.2/fair/logging.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.7.1/fair/register.py` & `fair_cli-0.7.2/fair/register.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.7.1/fair/registry/file_formats.json` & `fair_cli-0.7.2/fair/registry/file_formats.json`

 * *Files identical despite different names*

### Comparing `fair_cli-0.7.1/fair/registry/requests.py` & `fair_cli-0.7.2/fair/registry/requests.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.7.1/fair/registry/server.py` & `fair_cli-0.7.2/fair/registry/server.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.7.1/fair/registry/storage.py` & `fair_cli-0.7.2/fair/registry/storage.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.7.1/fair/registry/sync.py` & `fair_cli-0.7.2/fair/registry/sync.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.7.1/fair/registry/versioning.py` & `fair_cli-0.7.2/fair/registry/versioning.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.7.1/fair/run.py` & `fair_cli-0.7.2/fair/run.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.7.1/fair/session.py` & `fair_cli-0.7.2/fair/session.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.7.1/fair/staging.py` & `fair_cli-0.7.2/fair/staging.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.7.1/fair/testing.py` & `fair_cli-0.7.2/fair/testing.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.7.1/fair/user_config/__init__.py` & `fair_cli-0.7.2/fair/user_config/__init__.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.7.1/fair/user_config/globbing.py` & `fair_cli-0.7.2/fair/user_config/globbing.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.7.1/fair/user_config/validation.py` & `fair_cli-0.7.2/fair/user_config/validation.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.7.1/fair/utilities.py` & `fair_cli-0.7.2/fair/utilities.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.7.1/fair/virtualenv.py` & `fair_cli-0.7.2/fair/virtualenv.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.7.1/pyproject.toml` & `fair_cli-0.7.2/pyproject.toml`

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
-version = "0.7.1"
+version = "0.7.2"
 
 homepage = "https://www.fairdatapipeline.org/"
 
 repository = "https://github.com/FAIRDataPipeline/FAIR-CLI"
 
 documentation = "https://www.fairdatapipeline.org/docs/interface/fdp/"
```

### Comparing `fair_cli-0.7.1/PKG-INFO` & `fair_cli-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fair-cli
-Version: 0.7.1
+Version: 0.7.2
 Summary: Synchronization interface for the SCRC FAIR Data Pipeline registry
 Home-page: https://www.fairdatapipeline.org/
 License: BSD-2-Clause
 Keywords: FAIR Data Pipeline,FAIR,Data Management,Provenance
 Author: Richard Reeve
 Author-email: richard.reeve@glasgow.ac.uk
 Requires-Python: >=3.8.0,<4.0.0
```

