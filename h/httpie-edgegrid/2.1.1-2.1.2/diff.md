# Comparing `tmp/httpie_edgegrid-2.1.1-py3-none-any.whl.zip` & `tmp/httpie_edgegrid-2.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 9074 bytes, number of entries: 7
--rw-r--r--  2.0 unx     5737 b- defN 22-Sep-26 14:39 httpie_edgegrid.py
--rw-r--r--  2.0 unx    11324 b- defN 22-Sep-27 08:11 httpie_edgegrid-2.1.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     3509 b- defN 22-Sep-27 08:11 httpie_edgegrid-2.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Sep-27 08:11 httpie_edgegrid-2.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       72 b- defN 22-Sep-27 08:11 httpie_edgegrid-2.1.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       16 b- defN 22-Sep-27 08:11 httpie_edgegrid-2.1.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      605 b- defN 22-Sep-27 08:11 httpie_edgegrid-2.1.1.dist-info/RECORD
-7 files, 21355 bytes uncompressed, 7990 bytes compressed:  62.6%
+Zip file size: 9176 bytes, number of entries: 7
+-rw-r--r--  2.0 unx     6019 b- defN 23-Jun-22 07:03 httpie_edgegrid.py
+-rw-r--r--  2.0 unx    11324 b- defN 23-Jun-22 07:10 httpie_edgegrid-2.1.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3530 b- defN 23-Jun-22 07:10 httpie_edgegrid-2.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-22 07:10 httpie_edgegrid-2.1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       72 b- defN 23-Jun-22 07:10 httpie_edgegrid-2.1.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       16 b- defN 23-Jun-22 07:10 httpie_edgegrid-2.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      605 b- defN 23-Jun-22 07:10 httpie_edgegrid-2.1.2.dist-info/RECORD
+7 files, 21658 bytes uncompressed, 8092 bytes compressed:  62.6%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: httpie_edgegrid.py
 Comment: 
 
-Filename: httpie_edgegrid-2.1.1.dist-info/LICENSE
+Filename: httpie_edgegrid-2.1.2.dist-info/LICENSE
 Comment: 
 
-Filename: httpie_edgegrid-2.1.1.dist-info/METADATA
+Filename: httpie_edgegrid-2.1.2.dist-info/METADATA
 Comment: 
 
-Filename: httpie_edgegrid-2.1.1.dist-info/WHEEL
+Filename: httpie_edgegrid-2.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: httpie_edgegrid-2.1.1.dist-info/entry_points.txt
+Filename: httpie_edgegrid-2.1.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: httpie_edgegrid-2.1.1.dist-info/top_level.txt
+Filename: httpie_edgegrid-2.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: httpie_edgegrid-2.1.1.dist-info/RECORD
+Filename: httpie_edgegrid-2.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## httpie_edgegrid.py

```diff
@@ -38,30 +38,31 @@
         concrete_parser: argparse.ArgumentParser
 ) -> None:
     """Add a new group to the existing parser"""
     concrete_group = concrete_parser.add_argument_group(
         title=abstract_group.name, description=abstract_group.description
     )
     if abstract_group.is_mutually_exclusive:
-        concrete_group = concrete_group.add_mutually_exclusive_group(required=False)
+        concrete_group = concrete_group.add_mutually_exclusive_group(
+            required=False)
 
     for abstract_argument in abstract_group.arguments:
         concrete_group.add_argument(
             *abstract_argument.aliases,
             **map_qualifiers(
                 abstract_argument.configuration, ARGPARSE_QUALIFIER_MAP
             )
         )
 
-    return
-
 
 class EdgeGridSetterAction(argparse.Action):
-
-    def __init__(self,
+    """
+    Action used to set RC_PATH variable
+    """
+    def __init__(self, #pylint: disable-msg=too-many-arguments
                  option_strings,
                  dest,
                  nargs=None,
                  const=None,
                  default=None,
                  type=None,
                  choices=None,
@@ -69,75 +70,84 @@
                  help=None,
                  metavar=None):
         if nargs == 0:
             raise ValueError('nargs for store actions must be != 0; if you '
                              'have nothing to store, actions such as store '
                              'true or store const may be more appropriate')
         if const is not None and nargs != argparse.OPTIONAL:
-            raise ValueError('nargs must be %r to supply const' % argparse.OPTIONAL)
-        super(EdgeGridSetterAction, self).__init__(
+            raise ValueError(
+                f'nargs must be {argparse.OPTIONAL} to supply const')
+        super().__init__(
             option_strings=option_strings,
             dest=dest,
             nargs=nargs,
             const=const,
             default=default,
             type=type,
             choices=choices,
             required=required,
             help=help,
             metavar=metavar)
 
     def __call__(self, _, namespace, values, option_string=None):
         # Set the global RC_PATH
-        global RC_PATH
+        global RC_PATH #pylint: disable-msg=global-statement
         RC_PATH = values
 
 
 class HTTPieEdgeGridAuth(EdgeGridAuth):
-
+    """
+    A wrapper over the EdgeGridAuth
+    """
     def __init__(self, hostname, *args, **kwargs):
         self.__hostname = hostname
-        super(HTTPieEdgeGridAuth, self).__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)
 
     def __call__(self, r):
         # Here we can decorate with Agent Header (or sth)
-        r = super(HTTPieEdgeGridAuth, self).__call__(r)
+        r = super().__call__(r)
         r.url = r.url.replace("http:", "https:")
         r.url = r.url.replace("localhost/", self.__hostname)
-        return super(HTTPieEdgeGridAuth, self).__call__(r)
+        return super().__call__(r)
 
 
-class EdgeGridPlugin(AuthPlugin):
+class EdgeGridPlugin(AuthPlugin): #pylint: disable-msg=too-few-public-methods
+    """
+    The EdgeGridPlugin builds HTTPieEdgeGridAuth based on the EdgeRC credentials
+    """
     name = 'EdgeGrid auth'
     auth_type = 'edgegrid'
     description = ''
 
     def get_auth(self, username: str = None, password: str = None):
-        rc_path = os.path.expanduser(RC_PATH or os.getenv("RC_PATH") or '~/.edgerc')
+        rc_path = os.path.expanduser(
+            RC_PATH or os.getenv("RC_PATH") or '~/.edgerc')
 
         if not os.path.exists(rc_path):
-            err_msg = "\nERROR: The provided %s file does not exist\n" % rc_path
+            err_msg = f"\nERROR: The provided {rc_path} file does not exist\n"
             err_msg += "ERROR: Please generate credentials for the script functionality\n"
             err_msg += "ERROR: and run 'python gen_edgerc.py %s' to generate the credential file\n"
             sys.stderr.write(err_msg)
             sys.exit(1)
 
         try:
             rc = EdgeRc(rc_path)
-        except (configparser.DuplicateSectionError, configparser.MissingSectionHeaderError, UnicodeDecodeError):
-            err_msg = '''
-ERROR: {0} is not a valid .edgerc file
+        except (configparser.DuplicateSectionError,
+                configparser.MissingSectionHeaderError,
+                UnicodeDecodeError):
+            err_msg = f'''
+ERROR: {rc_path} is not a valid .edgerc file
 ERROR: Please generate credentials for the script functionality
-ERROR: and run 'python gen_edgerc.py %s' to generate the credential file
-'''.format(rc_path)
+ERROR: and run 'python gen_edgerc.py {rc_path}' to generate the credential file
+'''
             sys.stderr.write(err_msg)
             sys.exit(2)
 
         if not rc.has_section(username):
-            err_msg = "\nERROR: No section named '%s' was found in your .edgerc file\n" % username
+            err_msg = f"\nERROR: No section named '{username}' was found in your .edgerc file\n"
             err_msg += "ERROR: Please generate credentials for the script functionality\n"
             err_msg += "ERROR: and run 'python gen_edgerc.py %s' to generate the credential file\n"
             sys.stderr.write(err_msg)
             sys.exit(3)
 
         host = rc.get(username, 'host')
         host = host.replace("https://", "")
```

## Comparing `httpie_edgegrid-2.1.1.dist-info/LICENSE` & `httpie_edgegrid-2.1.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `httpie_edgegrid-2.1.1.dist-info/METADATA` & `httpie_edgegrid-2.1.2.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: httpie-edgegrid
-Version: 2.1.1
+Version: 2.1.2
 Summary: Edgegrid plugin for HTTPie.
 Home-page: https://github.com/akamai/httpie-edgegrid
 Download-URL: https://github.com/akamai/httpie-edgegrid
 Author: Developer Experience Akamai
 Author-email: devrel@akamai.com
 License: Apache 2.0
 Requires-Python: >=3.7
 License-File: LICENSE
-Requires-Dist: httpie (==3.2.1)
+Requires-Dist: httpie (==3.2.2)
 Requires-Dist: edgegrid-python (==1.3.1)
-Requires-Dist: pyOpenSSL (==22.0.0)
+Requires-Dist: pyOpenSSL (==23.2.0)
+Requires-Dist: urllib3 (<2.0.0)
 
 # httpie-edgegrid
 
 EdgeGrid plugin for [HTTPie](https://github.com/jkbr/httpie).
 
 ## Installation
 
@@ -76,15 +77,15 @@
 ```
 
 ### Example
 
 Making the diagnostic-tools API [locations]{.title-ref} call:
 
 ``` bash
-% http --auth-type edgegrid -a default: :/diagnostic-tools/v2/ghost-locations/available
+% http --auth-type edgegrid -a default: :/edge-diagnostics/v1/edge-locations
 ```
 
 ## Parameters
 
 `--edgegrid-config`
 
     Path to `.edgerc` credentials file (optional, defaults to `~/.edgerc`)
```

## Comparing `httpie_edgegrid-2.1.1.dist-info/RECORD` & `httpie_edgegrid-2.1.2.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-httpie_edgegrid.py,sha256=189ikueeipXlV1ooUEvVz3Rt-TuclrqvdViB7ZsNFKE,5737
-httpie_edgegrid-2.1.1.dist-info/LICENSE,sha256=qK0xscP0DcpahBGTUbj6jdyGjt13-tio6_bY8tFvpK4,11324
-httpie_edgegrid-2.1.1.dist-info/METADATA,sha256=0H2I4cKn_RJSm5oStPWdfjdOk7gC5IQZJmL9sC1EaHY,3509
-httpie_edgegrid-2.1.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-httpie_edgegrid-2.1.1.dist-info/entry_points.txt,sha256=FCPyBV3NFc86RR_oZp0LBBIK6e_C6oQt60zJBzaaDGs,72
-httpie_edgegrid-2.1.1.dist-info/top_level.txt,sha256=T0Z54T_2oi03IuwFcm7mverCF-Ymhbif-Z77tNB-l88,16
-httpie_edgegrid-2.1.1.dist-info/RECORD,,
+httpie_edgegrid.py,sha256=XkNY6PUCqe1jNNp167xZ6deJA597_5wBg9gHSR2sIfY,6019
+httpie_edgegrid-2.1.2.dist-info/LICENSE,sha256=qK0xscP0DcpahBGTUbj6jdyGjt13-tio6_bY8tFvpK4,11324
+httpie_edgegrid-2.1.2.dist-info/METADATA,sha256=yN7u4-ts1WppdRXU6ETSQ-l2Mtt7Yj8l3veg0Ga2nwU,3530
+httpie_edgegrid-2.1.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+httpie_edgegrid-2.1.2.dist-info/entry_points.txt,sha256=FCPyBV3NFc86RR_oZp0LBBIK6e_C6oQt60zJBzaaDGs,72
+httpie_edgegrid-2.1.2.dist-info/top_level.txt,sha256=T0Z54T_2oi03IuwFcm7mverCF-Ymhbif-Z77tNB-l88,16
+httpie_edgegrid-2.1.2.dist-info/RECORD,,
```

