# Comparing `tmp/msmanager-0.2.1.tar.gz` & `tmp/msmanager-0.2.1.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msmanager-0.2.1.tar", max compression
+gzip compressed data, was "msmanager-0.2.1.dev1.tar", max compression
```

## Comparing `msmanager-0.2.1.tar` & `msmanager-0.2.1.dev1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1111 2023-05-14 16:04:08.180554 msmanager-0.2.1/LICENSE
--rw-r--r--   0        0        0      267 2023-05-15 20:57:42.797028 msmanager-0.2.1/msmanager/__init__.py
--rw-r--r--   0        0        0       67 2023-05-15 21:27:48.138274 msmanager-0.2.1/msmanager/__main__.py
--rw-r--r--   0        0        0     6762 2023-06-21 22:40:41.481806 msmanager-0.2.1/msmanager/cli.py
--rw-r--r--   0        0        0     2488 2023-05-15 19:04:10.101041 msmanager-0.2.1/msmanager/config.py
--rw-r--r--   0        0        0     2793 2023-05-15 20:31:27.149266 msmanager-0.2.1/msmanager/exceptions.py
--rw-r--r--   0        0        0     3580 2023-06-21 22:42:09.045846 msmanager-0.2.1/msmanager/functions.py
--rw-r--r--   0        0        0      384 2023-05-16 16:36:36.800666 msmanager-0.2.1/msmanager/models.py
--rw-r--r--   0        0        0     2983 2023-06-13 10:18:25.381658 msmanager-0.2.1/msmanager/msm.py
--rw-r--r--   0        0        0      143 2023-05-15 19:04:10.113824 msmanager-0.2.1/msmanager/types.py
--rw-r--r--   0        0        0      586 2023-06-21 22:41:02.896155 msmanager-0.2.1/msmanager/units.py
--rw-r--r--   0        0        0      547 2023-06-21 22:41:17.815023 msmanager-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      565 2023-06-21 13:10:25.437469 msmanager-0.2.1/README.md
--rw-r--r--   0        0        0     1364 1970-01-01 00:00:00.000000 msmanager-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1111 2023-05-14 16:04:08.180554 msmanager-0.2.1.dev1/LICENSE
+-rw-r--r--   0        0        0      267 2023-05-15 20:57:42.797028 msmanager-0.2.1.dev1/msmanager/__init__.py
+-rw-r--r--   0        0        0       67 2023-05-15 21:27:48.138274 msmanager-0.2.1.dev1/msmanager/__main__.py
+-rw-r--r--   0        0        0     5968 2023-06-21 13:00:00.586899 msmanager-0.2.1.dev1/msmanager/cli.py
+-rw-r--r--   0        0        0     2488 2023-05-15 19:04:10.101041 msmanager-0.2.1.dev1/msmanager/config.py
+-rw-r--r--   0        0        0     2793 2023-05-15 20:31:27.149266 msmanager-0.2.1.dev1/msmanager/exceptions.py
+-rw-r--r--   0        0        0     3570 2023-06-21 12:56:23.279871 msmanager-0.2.1.dev1/msmanager/functions.py
+-rw-r--r--   0        0        0      384 2023-05-16 16:36:36.800666 msmanager-0.2.1.dev1/msmanager/models.py
+-rw-r--r--   0        0        0     2983 2023-06-13 10:18:25.381658 msmanager-0.2.1.dev1/msmanager/msm.py
+-rw-r--r--   0        0        0      143 2023-05-15 19:04:10.113824 msmanager-0.2.1.dev1/msmanager/types.py
+-rw-r--r--   0        0        0      533 2023-05-17 21:01:49.385592 msmanager-0.2.1.dev1/msmanager/units.py
+-rw-r--r--   0        0        0      552 2023-06-21 13:03:32.126797 msmanager-0.2.1.dev1/pyproject.toml
+-rw-r--r--   0        0        0      565 2023-05-16 18:14:53.984547 msmanager-0.2.1.dev1/README.md
+-rw-r--r--   0        0        0     1369 1970-01-01 00:00:00.000000 msmanager-0.2.1.dev1/PKG-INFO
```

### Comparing `msmanager-0.2.1/LICENSE` & `msmanager-0.2.1.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `msmanager-0.2.1/msmanager/cli.py` & `msmanager-0.2.1.dev1/msmanager/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,12 @@
 import os
 import click
 from rich.console import Console
 from typing import Iterable, Optional
 # > Local Imports
-from .units import (
-    __version__ as prog_version,
-    __title__ as prog_name
-)
 from .msm import MSManager
 from .models import MindustryServerConfig
 from .functions import (
     rich_exception,
     is_server_connect_correct,
     wait_start_server,
     ping, endicext
@@ -77,19 +73,15 @@
         console.print("[green]>[/] Server [bold yellow]removed[/]!")
     except Exception as e:
         console.print(rich_exception(e))
 
 # ? Start Command
 @click.command("start", help="Run the server.")
 @click.argument("screen_name", type=str)
-@click.option(
-    "-w", "--wait", "wait",
-    help="Waiting for the server to start up.",
-    is_flag=True
-)
+@click.option("-w", "--wait", "wait", is_flag=True, help="Waiting for the server to start up.")
 def starter(screen_name: str, wait: bool):
     try:
         msmanager.start_server(screen_name)
         if (server_config:=msmanager.get_server_config(screen_name)) is not None:
             if is_server_connect_correct(server_config.host, server_config.port, server_config.input_port) and wait:
                 wait_start_server(server_config.host, server_config.port, server_config.input_port)
         console.print("[green]>[/] Server [bold yellow]started[/]!")
@@ -104,44 +96,28 @@
         msmanager.stop_server(screen_name)
         console.print("[green]>[/] Server [bold yellow]stoped[/]!")
     except Exception as e:
         console.print(rich_exception(e))
 
 # ? List Command
 @click.command("list", help="List of servers in the config.")
-@click.option(
-    "--pinging", "pinging",
-    help="Whether to do a ping to check.",
-    is_flag=True, default=False
-)
-@click.option(
-    "-t", "--timeout", "timeout",
-    help="Maximum response waiting time (in seconds).",
-    type=int, default=10, show_default=True
-)
-def lister(pinging: bool, timeout: int):
+def lister():
     try:
         if len(msmanager.config.config.servers) != 0:
             for idx, server in enumerate(msmanager.config.config.servers):
-                lines = [
-                    f"({idx}) Server {repr(server.screen_name)}:",
-                    f"[magenta]Executable Filepath[/] : {repr(server.executable_filepath)}",
-                    f"[magenta]Arguments[/]           : {repr(server.arguments)}",
-                    f"[magenta]Host[/]                : [green]{server.host}[/]",
-                    f"[magenta]Port[/]                : [cyan]{server.port}[/]",
-                    f"[magenta]Input Port[/]          : [cyan]{server.input_port}[/]"
-                ]
-                if pinging:
-                    try:
-                        ping(server.host, server.port, timeout)
-                        started = True
-                    except:
-                        started = False
-                    lines.append(f"[magenta]Started[/]             : {repr(started)}")
-                console.print("\n\t".join(lines))
+                console.print(
+                    "\n\t".join(
+                        [
+                            f"({idx}) Server [green]{server.screen_name}[/]:",
+                            f"[yellow]EXECUTABLE_FILEPATH[/]  : {repr(server.executable_filepath)}",
+                            f"[yellow]ARGUMENTS[/]            : {repr(' '.join(server.arguments))}",
+                            f"[yellow]HOST:PORT:INPUT_PORT[/] : [green]{server.host}[/]:{server.port}:{server.input_port}"
+                        ]
+                    )
+                )
         else:
             console.print("[green]>[/] The list of servers is [bold yellow]empty[/]!")
     except Exception as e:
         console.print(rich_exception(e))
 
 @click.command("ping", help="Server status check.")
 @click.argument("host", type=str)
@@ -153,41 +129,39 @@
 )
 def pinger(host: str, port: int, timeout: int):
     try:
         status = ping(host, port, timeout)
         console.print(
             "\n\t".join(
                 [
-                    f"[green]>[/] Server '{endicext(status.name)}':",
-                    f"- [magenta]Players[/] : {status.players} players",
-                    f"- [magenta]Map[/]     : {repr(status.map)}",
-                    f"- [magenta]Wave[/]    : {status.wave} wave",
-                    f"- [magenta]Ping[/]    : {round(status.ping)} ms",
-                    f"- [magenta]Version[/] : {repr(status.version)}",
-                    f"- [magenta]Vertype[/] : {repr(status.vertype)}"
+                    f"[green]>[/] Server {endicext(status.name)}:",
+                    f"- [yellow]Players[/] : {status.players} players",
+                    f"- [yellow]Map[/]     : [green]{status.map}[/]",
+                    f"- [yellow]Wave[/]    : {status.wave} wave",
+                    f"- [yellow]Ping[/]    : {round(status.ping)} ms",
+                    f"- [yellow]Version[/] : [green]v{status.version}[/]",
+                    f"- [yellow]Vertype[/] : [green]{status.vertype}[/]"                    
                 ]
             )
         )
     except Exception as e:
         console.print(rich_exception(e))
 
 # ! Main Group
 @click.group()
 @click.option(
     "-nce", "--not-check-environment", "not_check_environment",
     is_flag=True,
     help="Disables checks for GNU Screen, Java and system support."
 )
-@click.version_option(
-    version=prog_version,
-    prog_name=prog_name
-)
 def main(not_check_environment: bool):
     global msmanager
-    msmanager = MSManager(check_environment=(not not_check_environment))
+    msmanager = MSManager(
+        check_environment=(not not_check_environment)
+    )
 
 # ! Add in Group
 main.add_command(adder)
 main.add_command(remover)
 main.add_command(starter)
 main.add_command(stoper)
 main.add_command(lister)
```

### Comparing `msmanager-0.2.1/msmanager/config.py` & `msmanager-0.2.1.dev1/msmanager/config.py`

 * *Files identical despite different names*

### Comparing `msmanager-0.2.1/msmanager/exceptions.py` & `msmanager-0.2.1.dev1/msmanager/exceptions.py`

 * *Files identical despite different names*

### Comparing `msmanager-0.2.1/msmanager/functions.py` & `msmanager-0.2.1.dev1/msmanager/functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pydustry
 import platform
 from versioner import Version
 from vbml import Pattern, Patcher
 from subprocess import getstatusoutput
-from typing import Tuple, Dict, Any, Iterable, Optional
+from typing import Tuple, Dict, Any, Iterable
 # * Local Imports
 from .types import DefaultVersioner, DefaultVBMLPacther
 from .units import SUPPORT_PLATFORMS, COLORS_STRINGS_REPLACEBLE
 from .exceptions import (
     VBMLParseError, 
     PlatformSupportError,
     ScreenNotWorkingError,
@@ -37,19 +37,19 @@
     while True:
         try:
             server.get_status(per_second)
             break
         except:
             pass
 
-def is_server_connect_correct(server_host: str, port: int, input_port: Optional[int]) -> bool:
+def is_server_connect_correct(server_host: str, port: int, input_port: int) -> bool:
     return \
         isinstance(server_host, str) and \
         isinstance(port, int) and \
-        (isinstance(input_port, int) or (input_port is not None))
+        (isinstance(input_port, int) if (input_port is not None) else True)
 
 def ping(host: str, port: int, timeout: int=10) -> pydustry.Status:
     return pydustry.Server(host, port).get_status(timeout)
 
 # ! Subproccess Functions
 def runner(*args: str) -> Tuple[int, str]:
     return getstatusoutput(" ".join([*args]))
```

### Comparing `msmanager-0.2.1/msmanager/msm.py` & `msmanager-0.2.1.dev1/msmanager/msm.py`

 * *Files identical despite different names*

### Comparing `msmanager-0.2.1/pyproject.toml` & `msmanager-0.2.1.dev1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "msmanager"
-version = "0.2.1"
-description = "Manager for managing Mindustry servers."
+version = "0.2.1.dev1"
+description = "Manager for managing Mindusrty servers."
 authors = ["Romanin <semina054@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "msmanager"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `msmanager-0.2.1/README.md` & `msmanager-0.2.1.dev1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MSManager
 ## Description
-Manager for managing Mindustry servers.
+Manager for managing Mindusrty servers.
 ## Install
 ```shell
 python3 -m pip install --upgrade msmanager
 ```
 ## Usage
 ```
 Usage: python -m msmanager [OPTIONS] COMMAND [ARGS]...
```

### Comparing `msmanager-0.2.1/PKG-INFO` & `msmanager-0.2.1.dev1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: msmanager
-Version: 0.2.1
-Summary: Manager for managing Mindustry servers.
+Version: 0.2.1.dev1
+Summary: Manager for managing Mindusrty servers.
 License: MIT
 Author: Romanin
 Author-email: semina054@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -19,15 +19,15 @@
 Requires-Dist: screens-py (>=0.5.0,<0.6.0)
 Requires-Dist: vbml (>=1.1.post1,<2.0)
 Requires-Dist: versioner.py (>=1.1.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # MSManager
 ## Description
-Manager for managing Mindustry servers.
+Manager for managing Mindusrty servers.
 ## Install
 ```shell
 python3 -m pip install --upgrade msmanager
 ```
 ## Usage
 ```
 Usage: python -m msmanager [OPTIONS] COMMAND [ARGS]...
```

