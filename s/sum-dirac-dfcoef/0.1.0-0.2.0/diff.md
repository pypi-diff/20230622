# Comparing `tmp/sum_dirac_dfcoef-0.1.0.tar.gz` & `tmp/sum_dirac_dfcoef-0.2.0.tar.gz`

## Comparing `sum_dirac_dfcoef-0.1.0.tar` & `sum_dirac_dfcoef-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,20 @@
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.1.0/requirements.txt
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.1.0/.github/scripts/versionup.py
--rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.1.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.1.0/.github/workflows/release-pr.yml
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.1.0/.github/workflows/reusable_test.yml
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.1.0/.github/workflows/test.yml
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.1.0/.vscode/settings.json
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.1.0/src/sum_dirac_dfcoef/__about__.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.1.0/src/sum_dirac_dfcoef/__init__.py
--rwxr-xr-x   0        0        0    20749 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.1.0/src/sum_dirac_dfcoef/sum_dirac_dfcoef.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.1.0/test/.gitignore
--rw-r--r--   0        0        0     9074 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.1.0/test/integration_test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.1.0/test/results/.gitkeep
--rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.1.0/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.1.0/LICENSE
--rw-r--r--   0        0        0     4866 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.1.0/README.md
--rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     6070 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.2.0/requirements.txt
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.2.0/.github/release-drafter.yml
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.2.0/.github/scripts/versionup.py
+-rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.2.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     2584 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.2.0/.github/workflows/release-pr.yml
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.2.0/.github/workflows/reusable_test.yml
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.2.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.2.0/.vscode/settings.json
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.2.0/src/sum_dirac_dfcoef/__about__.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.2.0/src/sum_dirac_dfcoef/__init__.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.2.0/src/sum_dirac_dfcoef/__main__.py
+-rwxr-xr-x   0        0        0    20749 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.2.0/src/sum_dirac_dfcoef/sum_dirac_dfcoef.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.2.0/test/.gitignore
+-rw-r--r--   0        0        0     9074 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.2.0/test/integration_test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.2.0/test/results/.gitkeep
+-rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.2.0/LICENSE
+-rw-r--r--   0        0        0     5065 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.2.0/README.md
+-rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6269 2020-02-02 00:00:00.000000 sum_dirac_dfcoef-0.2.0/PKG-INFO
```

### Comparing `sum_dirac_dfcoef-0.1.0/.github/scripts/versionup.py` & `sum_dirac_dfcoef-0.2.0/.github/scripts/versionup.py`

 * *Files identical despite different names*

### Comparing `sum_dirac_dfcoef-0.1.0/.github/workflows/release-pr.yml` & `sum_dirac_dfcoef-0.2.0/.github/workflows/release-pr.yml`

 * *Files 10% similar despite different names*

```diff
@@ -19,14 +19,15 @@
         required: false
         default: true
 
 env:
   NEW_VERSION: ""
   BRANCH_NAME: ""
   TAG_NAME: ""
+  VERSION_UP_TYPE: ""
   PACKAGE_NAME: sum_dirac_dfcoef
 jobs:
   test:
     uses: ./.github/workflows/reusable_test.yml
   release-pr:
     needs: test
     runs-on: ubuntu-22.04
@@ -41,18 +42,21 @@
         run: |
           python -m pip install --upgrade pip
           python -m pip install hatch twine
       - name: Update version
         run: |
           if ${{ github.event.inputs.major_versionup }}; then
             python .github/scripts/versionup.py --major
+            echo "VERSION_UP_TYPE=major" >> $GITHUB_ENV
           elif ${{ github.event.inputs.minor_versionup }}; then
             python .github/scripts/versionup.py --minor
+            echo "VERSION_UP_TYPE=minor" >> $GITHUB_ENV
           elif ${{ github.event.inputs.patch_versionup }}; then
             python .github/scripts/versionup.py --patch
+            echo "VERSION_UP_TYPE=patch" >> $GITHUB_ENV
           fi
       - name: Get the NEW_VERSION
         run: |
           NEW_VERSION=$(hatch version)
           echo "NEW_VERSION=$NEW_VERSION" >> $GITHUB_ENV
           echo "BRANCH_NAME=release-v$NEW_VERSION" >> $GITHUB_ENV
           echo "TAG_NAME=v$NEW_VERSION" >> $GITHUB_ENV
@@ -60,10 +64,10 @@
         run: |
           git config --global user.name "github-actions[bot]"
           git config --global user.email "github-actions[bot]@users.noreply.github.com"
           git checkout -b "${{ env.BRANCH_NAME }}"
           git add .
           git commit -m "Release ${{ env.PACKAGE_NAME }} ${{ env.NEW_VERSION }}"
           git push origin "${{ env.BRANCH_NAME }}"
-          gh pr create --title "Release ${{ env.PACKAGE_NAME }} ${{ env.NEW_VERSION }}" --body "Release ${{ env.PACKAGE_NAME }} ${{ env.NEW_VERSION }}"
+          gh pr create --title "Release ${{ env.PACKAGE_NAME }} ${{ env.NEW_VERSION }}" --body "Release ${{ env.PACKAGE_NAME }} ${{ env.NEW_VERSION }}" --label ${{ env.VERSION_UP_TYPE }} --label "release"
         env:
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
```

### Comparing `sum_dirac_dfcoef-0.1.0/.github/workflows/reusable_test.yml` & `sum_dirac_dfcoef-0.2.0/.github/workflows/reusable_test.yml`

 * *Files identical despite different names*

### Comparing `sum_dirac_dfcoef-0.1.0/src/sum_dirac_dfcoef/sum_dirac_dfcoef.py` & `sum_dirac_dfcoef-0.2.0/src/sum_dirac_dfcoef/sum_dirac_dfcoef.py`

 * *Files identical despite different names*

### Comparing `sum_dirac_dfcoef-0.1.0/test/integration_test.py` & `sum_dirac_dfcoef-0.2.0/test/integration_test.py`

 * *Files identical despite different names*

### Comparing `sum_dirac_dfcoef-0.1.0/.gitignore` & `sum_dirac_dfcoef-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `sum_dirac_dfcoef-0.1.0/LICENSE` & `sum_dirac_dfcoef-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sum_dirac_dfcoef-0.1.0/README.md` & `sum_dirac_dfcoef-0.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 
 ```sh
 pip install sum_dirac_dfcoef
 ```
 
 ## Usage
 
+### Linux, macOS
+
 You can use this program with the following command!
 
 ```sh
 # Output to MOLECULE_NAME.out
 sum_dirac_dfcoef -i DIRAC_OUPUT_FILE_PATH -m MOLECULE_NAME
 # Specify output file name with -o option
 sum_dirac_dfcoef -i DIRAC_OUPUT_FILE_PATH -m MOLECULE_NAME -o OUTPUT_FILE_NAME
@@ -28,14 +30,22 @@
 
 (e.g.)
 
 ```sh
 sum_dirac_dfcoef -i x2c_uo2_238.out -m UO2
 ```
 
+### Windows
+
+If you want to use this program on Windows, you can use it with the following command.
+
+```sh
+python -m sum_dirac_dfcoef -i DIRAC_OUPUT_FILE_PATH -m MOLECULE_NAME
+```
+
 A part of x2c_uo2_238.out (DIRAC output file, ... represents an omission)
 
 ```out
 ...
     **************************************************************************
     ****************************** Vector print ******************************
     **************************************************************************
@@ -95,14 +105,15 @@
 
 ```out
 E1u 19 -8.8824415703374 B3uUpx 49.999172476298732 B2uUpy 49.999172476298732
 E1u 20 -8.8607510987047 B1uUpz 66.766609997188567 B3uUpx 16.052352691541234 B2uUpy 16.052352691541234 B1uOs 0.547408583853977 B1uOs 0.547408583853977
 E1g 17 -5.1175267254674 B2gUdxz 35.987808727554935 B3gUdyz 35.987808727554935 AgUdzz 18.548678611340048 AgUdxx 4.637169653126273 AgUdyy 4.637169653126273 AgUs 0.137285121776232
 ...
 ```
+
 This options is useful when you want to use the result in a spreadsheet like Microsoft Excel.
 
 ## Options
 
 optional arguments (--input and --mol are required)
 
 - -h, --help
@@ -114,15 +125,15 @@
   (required) file name of DIRAC output
 
 - -m MOL, --mol MOL
 
   (required) molecule specification. Write the molecular formula (e.g. Cu2O).  
   **DON'T write the rational formula (e.g. CH3OH)**
 
--  -o OUTPUT, --output OUTPUT
+- -o OUTPUT, --output OUTPUT
   Output file name. Default: (-m or --mol option value).out (e.g) --m H2O => print to H2O.out
 
 - -c, --compress
 
   Compress output. Display all coefficients on one line for each MO.  
   This options is useful when you want to use the result in a spreadsheet like Microsoft Excel.
```

### Comparing `sum_dirac_dfcoef-0.1.0/pyproject.toml` & `sum_dirac_dfcoef-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sum_dirac_dfcoef-0.1.0/PKG-INFO` & `sum_dirac_dfcoef-0.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sum_dirac_dfcoef
-Version: 0.1.0
+Version: 0.2.0
 Summary: This is a utility to summarize the contribution of each atomic orbital per molecular orbital from the DIRAC output file that the *PRIVEC and .VECPRI options are used.
 Project-URL: Documentation, https://github.com/kohei-noda-qcrg/sum_dirac_dfcoef#readme
 Project-URL: Issues, https://github.com/kohei-noda-qcrg/sum_dirac_dfcoef/issues
 Project-URL: Source, https://github.com/kohei-noda-qcrg/sum_dirac_dfcoef
 Author-email: Kohei Noda <kohei-noda@hiroshima-u.ac.jp>
 License-Expression: MIT
 License-File: LICENSE
@@ -37,14 +37,16 @@
 
 ```sh
 pip install sum_dirac_dfcoef
 ```
 
 ## Usage
 
+### Linux, macOS
+
 You can use this program with the following command!
 
 ```sh
 # Output to MOLECULE_NAME.out
 sum_dirac_dfcoef -i DIRAC_OUPUT_FILE_PATH -m MOLECULE_NAME
 # Specify output file name with -o option
 sum_dirac_dfcoef -i DIRAC_OUPUT_FILE_PATH -m MOLECULE_NAME -o OUTPUT_FILE_NAME
@@ -52,14 +54,22 @@
 
 (e.g.)
 
 ```sh
 sum_dirac_dfcoef -i x2c_uo2_238.out -m UO2
 ```
 
+### Windows
+
+If you want to use this program on Windows, you can use it with the following command.
+
+```sh
+python -m sum_dirac_dfcoef -i DIRAC_OUPUT_FILE_PATH -m MOLECULE_NAME
+```
+
 A part of x2c_uo2_238.out (DIRAC output file, ... represents an omission)
 
 ```out
 ...
     **************************************************************************
     ****************************** Vector print ******************************
     **************************************************************************
@@ -119,14 +129,15 @@
 
 ```out
 E1u 19 -8.8824415703374 B3uUpx 49.999172476298732 B2uUpy 49.999172476298732
 E1u 20 -8.8607510987047 B1uUpz 66.766609997188567 B3uUpx 16.052352691541234 B2uUpy 16.052352691541234 B1uOs 0.547408583853977 B1uOs 0.547408583853977
 E1g 17 -5.1175267254674 B2gUdxz 35.987808727554935 B3gUdyz 35.987808727554935 AgUdzz 18.548678611340048 AgUdxx 4.637169653126273 AgUdyy 4.637169653126273 AgUs 0.137285121776232
 ...
 ```
+
 This options is useful when you want to use the result in a spreadsheet like Microsoft Excel.
 
 ## Options
 
 optional arguments (--input and --mol are required)
 
 - -h, --help
@@ -138,15 +149,15 @@
   (required) file name of DIRAC output
 
 - -m MOL, --mol MOL
 
   (required) molecule specification. Write the molecular formula (e.g. Cu2O).  
   **DON'T write the rational formula (e.g. CH3OH)**
 
--  -o OUTPUT, --output OUTPUT
+- -o OUTPUT, --output OUTPUT
   Output file name. Default: (-m or --mol option value).out (e.g) --m H2O => print to H2O.out
 
 - -c, --compress
 
   Compress output. Display all coefficients on one line for each MO.  
   This options is useful when you want to use the result in a spreadsheet like Microsoft Excel.
```

