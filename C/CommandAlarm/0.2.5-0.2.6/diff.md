# Comparing `tmp/CommandAlarm-0.2.5.tar.gz` & `tmp/CommandAlarm-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CommandAlarm-0.2.5.tar", last modified: Tue Jun 20 20:44:36 2023, max compression
+gzip compressed data, was "CommandAlarm-0.2.6.tar", last modified: Tue Jun 20 23:40:10 2023, max compression
```

## Comparing `CommandAlarm-0.2.5.tar` & `CommandAlarm-0.2.6.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 testuser  (1002) testuser  (1003)        0 2023-06-20 20:44:36.729932 CommandAlarm-0.2.5/
-drwxr-xr-x   0 testuser  (1002) testuser  (1003)        0 2023-06-20 20:44:36.709932 CommandAlarm-0.2.5/CommandAlarm.egg-info/
--rw-r--r--   0 testuser  (1002) testuser  (1003)     3239 2023-06-20 20:44:36.000000 CommandAlarm-0.2.5/CommandAlarm.egg-info/PKG-INFO
--rw-r--r--   0 testuser  (1002) testuser  (1003)      263 2023-06-20 20:44:36.000000 CommandAlarm-0.2.5/CommandAlarm.egg-info/SOURCES.txt
--rw-r--r--   0 testuser  (1002) testuser  (1003)        1 2023-06-20 20:44:36.000000 CommandAlarm-0.2.5/CommandAlarm.egg-info/dependency_links.txt
--rw-r--r--   0 testuser  (1002) testuser  (1003)       64 2023-06-20 20:44:36.000000 CommandAlarm-0.2.5/CommandAlarm.egg-info/entry_points.txt
--rw-r--r--   0 testuser  (1002) testuser  (1003)       13 2023-06-20 20:44:36.000000 CommandAlarm-0.2.5/CommandAlarm.egg-info/top_level.txt
--rw-r--r--   0 testuser  (1002) testuser  (1003)    35149 2023-06-15 23:25:58.000000 CommandAlarm-0.2.5/LICENSE
--rw-r--r--   0 testuser  (1002) testuser  (1003)     3239 2023-06-20 20:44:36.729932 CommandAlarm-0.2.5/PKG-INFO
--rw-r--r--   0 testuser  (1002) testuser  (1003)     2347 2023-06-20 07:40:35.000000 CommandAlarm-0.2.5/README.md
-drwxr-xr-x   0 testuser  (1002) testuser  (1003)        0 2023-06-20 20:44:36.721932 CommandAlarm-0.2.5/commandalarm/
--rw-r--r--   0 testuser  (1002) testuser  (1003)      767 2023-06-20 19:16:56.000000 CommandAlarm-0.2.5/commandalarm/__init__.py
--rw-r--r--   0 testuser  (1002) testuser  (1003)     7352 2023-06-20 19:17:37.000000 CommandAlarm-0.2.5/commandalarm/commandalarm.py
--rw-r--r--   0 testuser  (1002) testuser  (1003)       38 2023-06-20 20:44:36.729932 CommandAlarm-0.2.5/setup.cfg
--rw-r--r--   0 testuser  (1002) testuser  (1003)     1308 2023-06-20 19:59:54.000000 CommandAlarm-0.2.5/setup.py
+drwxr-xr-x   0 testuser  (1002) testuser  (1003)        0 2023-06-20 23:40:10.425159 CommandAlarm-0.2.6/
+-rw-r--r--   0 testuser  (1002) testuser  (1003)      967 2023-06-20 23:21:14.000000 CommandAlarm-0.2.6/CHANGELOG.md
+drwxr-xr-x   0 testuser  (1002) testuser  (1003)        0 2023-06-20 23:40:10.425159 CommandAlarm-0.2.6/CommandAlarm.egg-info/
+-rw-r--r--   0 testuser  (1002) testuser  (1003)     3293 2023-06-20 23:40:10.000000 CommandAlarm-0.2.6/CommandAlarm.egg-info/PKG-INFO
+-rw-r--r--   0 testuser  (1002) testuser  (1003)      288 2023-06-20 23:40:10.000000 CommandAlarm-0.2.6/CommandAlarm.egg-info/SOURCES.txt
+-rw-r--r--   0 testuser  (1002) testuser  (1003)        1 2023-06-20 23:40:10.000000 CommandAlarm-0.2.6/CommandAlarm.egg-info/dependency_links.txt
+-rw-r--r--   0 testuser  (1002) testuser  (1003)       64 2023-06-20 23:40:10.000000 CommandAlarm-0.2.6/CommandAlarm.egg-info/entry_points.txt
+-rw-r--r--   0 testuser  (1002) testuser  (1003)       13 2023-06-20 23:40:10.000000 CommandAlarm-0.2.6/CommandAlarm.egg-info/top_level.txt
+-rw-r--r--   0 testuser  (1002) testuser  (1003)    35149 2023-06-15 23:25:58.000000 CommandAlarm-0.2.6/LICENSE
+-rw-r--r--   0 testuser  (1002) testuser  (1003)       29 2023-06-20 23:36:04.000000 CommandAlarm-0.2.6/MANIFEST.in
+-rw-r--r--   0 testuser  (1002) testuser  (1003)     3293 2023-06-20 23:40:10.425159 CommandAlarm-0.2.6/PKG-INFO
+-rw-r--r--   0 testuser  (1002) testuser  (1003)     2401 2023-06-20 23:12:03.000000 CommandAlarm-0.2.6/README.md
+drwxr-xr-x   0 testuser  (1002) testuser  (1003)        0 2023-06-20 23:40:10.425159 CommandAlarm-0.2.6/commandalarm/
+-rw-r--r--   0 testuser  (1002) testuser  (1003)      767 2023-06-20 23:23:58.000000 CommandAlarm-0.2.6/commandalarm/__init__.py
+-rw-r--r--   0 testuser  (1002) testuser  (1003)     7641 2023-06-20 23:02:25.000000 CommandAlarm-0.2.6/commandalarm/commandalarm.py
+-rw-r--r--   0 testuser  (1002) testuser  (1003)       38 2023-06-20 23:40:10.425159 CommandAlarm-0.2.6/setup.cfg
+-rw-r--r--   0 testuser  (1002) testuser  (1003)     1308 2023-06-20 23:29:04.000000 CommandAlarm-0.2.6/setup.py
```

### Comparing `CommandAlarm-0.2.5/CommandAlarm.egg-info/PKG-INFO` & `CommandAlarm-0.2.6/CommandAlarm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CommandAlarm
-Version: 0.2.5
+Version: 0.2.6
 Summary: A simple command line program that allows users to set an alarm with a custom command.
 Home-page: https://github.com/alofgren/commandalarm
 Author: alofgren
 Author-email: drelofren@outlook.com
 License: GPLv3
 Project-URL: Bug Reports, https://github.com/alofgren/commandalarm/issues
 Project-URL: Source, https://github.com/alofgren/commandalarm
@@ -40,21 +40,22 @@
 cd commandalarm
 pip install .
 ```
 
 ## Usage Output
 
 ```
-usage: commandalarm [-h] [-v] [-d {1,2,3,4,5,6,7}] [-r] [-s] [-n] [-t TIMEOUT] time command [command ...]
+usage: commandalarm [-h] [-v] [-d {1,2,3,4,5,6,7}] [-r] [-s] [-n] [-t TIMEOUT] time command [argument ...]
 
 Set an alarm with a custom command.
 
 positional arguments:
   time                  the time in the format HH:MM:SS
   command               the command to run
+  argument              the arguments to the command
 
 optional arguments:
   -h, --help            show this help message and exit
   -v, --version         show program's version number and exit
   -d {1,2,3,4,5,6,7}, --day {1,2,3,4,5,6,7}
                         the day of the week as an integer from 1 to 7, where 1 represents Monday
   -r, --repeat          repeat indefinitely
```

### Comparing `CommandAlarm-0.2.5/LICENSE` & `CommandAlarm-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `CommandAlarm-0.2.5/PKG-INFO` & `CommandAlarm-0.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CommandAlarm
-Version: 0.2.5
+Version: 0.2.6
 Summary: A simple command line program that allows users to set an alarm with a custom command.
 Home-page: https://github.com/alofgren/commandalarm
 Author: alofgren
 Author-email: drelofren@outlook.com
 License: GPLv3
 Project-URL: Bug Reports, https://github.com/alofgren/commandalarm/issues
 Project-URL: Source, https://github.com/alofgren/commandalarm
@@ -40,21 +40,22 @@
 cd commandalarm
 pip install .
 ```
 
 ## Usage Output
 
 ```
-usage: commandalarm [-h] [-v] [-d {1,2,3,4,5,6,7}] [-r] [-s] [-n] [-t TIMEOUT] time command [command ...]
+usage: commandalarm [-h] [-v] [-d {1,2,3,4,5,6,7}] [-r] [-s] [-n] [-t TIMEOUT] time command [argument ...]
 
 Set an alarm with a custom command.
 
 positional arguments:
   time                  the time in the format HH:MM:SS
   command               the command to run
+  argument              the arguments to the command
 
 optional arguments:
   -h, --help            show this help message and exit
   -v, --version         show program's version number and exit
   -d {1,2,3,4,5,6,7}, --day {1,2,3,4,5,6,7}
                         the day of the week as an integer from 1 to 7, where 1 represents Monday
   -r, --repeat          repeat indefinitely
```

### Comparing `CommandAlarm-0.2.5/README.md` & `CommandAlarm-0.2.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -17,21 +17,22 @@
 cd commandalarm
 pip install .
 ```
 
 ## Usage Output
 
 ```
-usage: commandalarm [-h] [-v] [-d {1,2,3,4,5,6,7}] [-r] [-s] [-n] [-t TIMEOUT] time command [command ...]
+usage: commandalarm [-h] [-v] [-d {1,2,3,4,5,6,7}] [-r] [-s] [-n] [-t TIMEOUT] time command [argument ...]
 
 Set an alarm with a custom command.
 
 positional arguments:
   time                  the time in the format HH:MM:SS
   command               the command to run
+  argument              the arguments to the command
 
 optional arguments:
   -h, --help            show this help message and exit
   -v, --version         show program's version number and exit
   -d {1,2,3,4,5,6,7}, --day {1,2,3,4,5,6,7}
                         the day of the week as an integer from 1 to 7, where 1 represents Monday
   -r, --repeat          repeat indefinitely
```

### Comparing `CommandAlarm-0.2.5/commandalarm/__init__.py` & `CommandAlarm-0.2.6/commandalarm/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
 # FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 """ Set an alarm with a custom command. """
 
-__version__ = "0.2.5"
+__version__ = "0.2.6"
```

### Comparing `CommandAlarm-0.2.5/commandalarm/commandalarm.py` & `CommandAlarm-0.2.6/commandalarm/commandalarm.py`

 * *Files 8% similar despite different names*

```diff
@@ -108,45 +108,40 @@
     argparse.Namespace: A namespace containing the parsed arguments.
 
     Raises:
     ValueError: If the time argument is not a valid time string.
     ValueError: If the day argument is not a valid integer between 1 and 7.
     """
     parser = argparse.ArgumentParser(
-        description="Set an alarm with a custom command.")
-    parser.add_argument(
-        "time",
-        type=valid_time_string,
-        help="the time in the format HH:MM:SS",
-    )
-    parser.add_argument(
-        "command",
-        type=str,
-        nargs="+",
-        help="the command to run",
-    )
+        prog="commandalarm", description="Set an alarm with a custom command.")
+    parser.add_argument("time",
+                        type=valid_time_string,
+                        help="the time in the format HH:MM:SS")
+    parser.add_argument("command", type=str, help="the command to run")
+    parser.add_argument("argument",
+                        default=None,
+                        type=str,
+                        nargs="*",
+                        help="the arguments to the command")
     parser.add_argument("-v",
                         "--version",
                         action="version",
                         version="%(prog)s " + __version__)
     parser.add_argument(
         "-d",
         "--day",
-        type=int,
         default=datetime.date.today().isoweekday(),
+        type=int,
         help=
         "the day of the week as an integer from 1 to 7, where 1 represents Monday",
-        choices=range(1, 8),
-    )
-    parser.add_argument(
-        "-r",
-        "--repeat",
-        action="store_true",
-        help="repeat indefinitely",
-    )
+        choices=range(1, 8))
+    parser.add_argument("-r",
+                        "--repeat",
+                        action="store_true",
+                        help="repeat indefinitely")
     parser.add_argument("-s",
                         "--shell",
                         action="store_true",
                         default=False,
                         help="run command in a shell")
     parser.add_argument("-n",
                         "--no-check",
@@ -172,16 +167,17 @@
         set_alarm(args.time, args.day)
         while True:
             while not ALARM_FIRED:
                 if platform.system() == 'Windows':
                     time.sleep(1)
                 else:
                     signal.pause()
-            command_str = " ".join(args.command)
-            command = command_str if args.shell else args.command
+            command_str = f"{args.command} {' '.join(args.argument)}"
+            command = command_str if args.shell else [args.command
+                                                      ] + args.argument
             print("Time is up!")
             print("Running command:", command_str)
             try:
                 result = subprocess.run(command,
                                         capture_output=True,
                                         shell=args.shell,
                                         timeout=args.timeout,
@@ -209,13 +205,12 @@
                 ALARM_FIRED = False
                 time.sleep(1)
                 set_alarm(args.time, args.day)
             else:
                 break
     except KeyboardInterrupt:
         print("Alarm stopped manually.", file=sys.stderr)
-        signal.alarm(0)
         sys.exit(1)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `CommandAlarm-0.2.5/setup.py` & `CommandAlarm-0.2.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup (
     name = "CommandAlarm",
-    version = "0.2.5",
+    version = "0.2.6",
     author = "alofgren",
     author_email = "drelofren@outlook.com",
     description = "A simple command line program that allows users to set an alarm with a custom command.",
     license = "GPLv3",
     keywords = ["alarm","command","command-line","tool","timer","commandalarm"],
     url = "https://github.com/alofgren/commandalarm",
     long_description = long_description,
```

