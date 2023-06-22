# Comparing `tmp/sum_dirac_dfcoef-0.2.0.tar.gz` & `tmp/sum_dirac_dfcoef-0.2.1.tar.gz`

## Comparing `sum_dirac_dfcoef-0.2.0.tar` & `sum_dirac_dfcoef-0.2.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.2.0/requirements.txt
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.2.0/.github/release-drafter.yml
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.2.0/.github/scripts/versionup.py
--rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.2.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0     2584 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.2.0/.github/workflows/release-pr.yml
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.2.0/.github/workflows/reusable_test.yml
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.2.0/.github/workflows/test.yml
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.2.0/.vscode/settings.json
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.2.0/src/sum_dirac_dfcoef/__about__.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.2.0/src/sum_dirac_dfcoef/__init__.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.2.0/src/sum_dirac_dfcoef/__main__.py
--rwxr-xr-x   0        0        0    20749 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.2.0/src/sum_dirac_dfcoef/sum_dirac_dfcoef.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.2.0/test/.gitignore
--rw-r--r--   0        0        0     9074 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.2.0/test/integration_test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.2.0/test/results/.gitkeep
--rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.2.0/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.2.0/LICENSE
--rw-r--r--   0        0        0     5065 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.2.0/README.md
--rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     6269 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.2.1/requirements.txt
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.2.1/.github/release-drafter.yml
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.2.1/.github/scripts/versionup.py
+-rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.2.1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     2584 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.2.1/.github/workflows/release-pr.yml
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.2.1/.github/workflows/reusable_test.yml
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.2.1/.github/workflows/test.yml
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.2.1/.vscode/settings.json
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.2.1/src/sum_dirac_dfcoef/__about__.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.2.1/src/sum_dirac_dfcoef/__init__.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.2.1/src/sum_dirac_dfcoef/__main__.py
+-rwxr-xr-x   0        0        0    21422 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.2.1/src/sum_dirac_dfcoef/sum_dirac_dfcoef.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.2.1/test/.gitignore
+-rw-r--r--   0        0        0     9074 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.2.1/test/integration_test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.2.1/test/results/.gitkeep
+-rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.2.1/LICENSE
+-rw-r--r--   0        0        0     5110 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.2.1/README.md
+-rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     6314 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.2.1/PKG-INFO
```

### Comparing `sum_dirac_dfcoef-0.2.0/.github/release-drafter.yml` & `sum_dirac_dfcoef-0.2.1/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `sum_dirac_dfcoef-0.2.0/.github/scripts/versionup.py` & `sum_dirac_dfcoef-0.2.1/.github/scripts/versionup.py`

 * *Files identical despite different names*

### Comparing `sum_dirac_dfcoef-0.2.0/.github/workflows/publish.yml` & `sum_dirac_dfcoef-0.2.1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `sum_dirac_dfcoef-0.2.0/.github/workflows/release-pr.yml` & `sum_dirac_dfcoef-0.2.1/.github/workflows/release-pr.yml`

 * *Files identical despite different names*

### Comparing `sum_dirac_dfcoef-0.2.0/.github/workflows/reusable_test.yml` & `sum_dirac_dfcoef-0.2.1/.github/workflows/reusable_test.yml`

 * *Files identical despite different names*

### Comparing `sum_dirac_dfcoef-0.2.0/src/sum_dirac_dfcoef/sum_dirac_dfcoef.py` & `sum_dirac_dfcoef-0.2.1/src/sum_dirac_dfcoef/sum_dirac_dfcoef.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,26 +79,44 @@
         self.norm_constant = norm_constant
         self.sum_coefficients = sum_coefficients
 
     def __repr__(self) -> str:
         return f"mo_info: {self.mo_info}, mo_energy: {self.mo_energy}, coefficients: {self.data_per_orbital_types}"
 
 
+class PrintVersionExitAction(argparse.Action):
+    def __init__(self, option_strings, dest=argparse.SUPPRESS, default=argparse.SUPPRESS, help=None):
+        super().__init__(
+            option_strings=option_strings,
+            dest=dest,
+            default=default,
+            nargs=0,
+            help=help,
+        )
+
+    def __call__(self, parser, namespace, values, option_string=None):
+        from .__about__ import __version__
+        print(f"{__version__}")
+        exit()
+
+
 def parse_args() -> "argparse.Namespace":
     parser = argparse.ArgumentParser(description="Summarize the coefficients from DIRAC output file that *PRIVEC option is used. (c.f. http://www.diracprogram.org/doc/master/manual/analyze/privec.html)")
     parser.add_argument("-i", "--input", type=str, required=True, help="(required) file name of DIRAC output", dest="file")
     parser.add_argument("-m", "--mol", type=str, required=True, help="(required) molecule specification. Write the molecular formula (e.g. Cu2O). ** DON'T write the rational formula (e.g. CH3OH) **")
     parser.add_argument("-o", "--output", type=str, help="Output file name. Default: (-m or --mol option value).out (e.g) --m H2O => print to H2O.out", dest="output")
     parser.add_argument("-c", "--compress", action="store_true", help="Compress output. Display all coefficients on one line for each MO. This options is useful when you want to use the result in a spreadsheet like Microsoft Excel.", dest="compress")
     parser.add_argument("-t", "--threshold", type=float, default=0.1, help="threshold. Default: 0.1 %% (e.g) --threshold=0.1 => print orbital with more than 0.1 %% contribution", dest="threshold")
     parser.add_argument("-d", "--decimal", type=int, default=5, choices=range(1, 16), help="Set the decimal places. Default: 5 (e.g) --decimal=3 => print orbital with 3 decimal places (0.123, 2.456, ...). range: 1-15", dest="decimal")
     parser.add_argument("-a", "--all-write", action="store_true", help="Print all MOs(Positronic and Electronic).", dest="all_write")
     parser.add_argument("-p", "--positronic-write", action="store_true", help="Print only Positronic MOs.", dest="positronic_write")
+    parser.add_argument("-v", "--version", action=PrintVersionExitAction, help="Print version and exit", dest="version")
     parser.add_argument("--debug", action="store_true", help="print debug output (Normalization constant, Sum of MO coefficient)", dest="debug")
     parser.add_argument("--no-sort", action="store_true", help="Don't sort the output by MO energy")
+    # If -v or --version option is used, print version and exit
     return parser.parse_args()
 
 
 def debug_print_wrapper(args: "argparse.Namespace", str: str):
     # print debug message if --debug option is used
     if args.debug:
         print(str)
```

### Comparing `sum_dirac_dfcoef-0.2.0/test/integration_test.py` & `sum_dirac_dfcoef-0.2.1/test/integration_test.py`

 * *Files identical despite different names*

### Comparing `sum_dirac_dfcoef-0.2.0/.gitignore` & `sum_dirac_dfcoef-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `sum_dirac_dfcoef-0.2.0/LICENSE` & `sum_dirac_dfcoef-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sum_dirac_dfcoef-0.2.0/README.md` & `sum_dirac_dfcoef-0.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -144,19 +144,25 @@
 
 - -d DECIMAL, --decimal DECIMAL
 
   Set the decimal places. Default: 5  
   (e.g) --decimal=3 => print orbital with 3 decimal places (0.123, 2.456, ...). range: 1-15
 
 - -a, --all-write
+
   Print all MOs(Positronic and Electronic).
 
 - -p, --positronic-write
+
   Print only Positronic MOs.
 
+- -v, --version
+
+  Print version and exit
+
 - --debug
 
   print debug output (Normalization constant, Sum of MO coefficient)
 
 - --no-sort
 
   Don't sort the output by MO energy
```

### Comparing `sum_dirac_dfcoef-0.2.0/pyproject.toml` & `sum_dirac_dfcoef-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sum_dirac_dfcoef-0.2.0/PKG-INFO` & `sum_dirac_dfcoef-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sum_dirac_dfcoef
-Version: 0.2.0
+Version: 0.2.1
 Summary: This is a utility to summarize the contribution of each atomic orbital per molecular orbital from the DIRAC output file that the *PRIVEC and .VECPRI options are used.
 Project-URL: Documentation, https://github.com/kohei-noda-qcrg/sum_dirac_dfcoef#readme
 Project-URL: Issues, https://github.com/kohei-noda-qcrg/sum_dirac_dfcoef/issues
 Project-URL: Source, https://github.com/kohei-noda-qcrg/sum_dirac_dfcoef
 Author-email: Kohei Noda <kohei-noda@hiroshima-u.ac.jp>
 License-Expression: MIT
 License-File: LICENSE
@@ -168,19 +168,25 @@
 
 - -d DECIMAL, --decimal DECIMAL
 
   Set the decimal places. Default: 5  
   (e.g) --decimal=3 => print orbital with 3 decimal places (0.123, 2.456, ...). range: 1-15
 
 - -a, --all-write
+
   Print all MOs(Positronic and Electronic).
 
 - -p, --positronic-write
+
   Print only Positronic MOs.
 
+- -v, --version
+
+  Print version and exit
+
 - --debug
 
   print debug output (Normalization constant, Sum of MO coefficient)
 
 - --no-sort
 
   Don't sort the output by MO energy
```

