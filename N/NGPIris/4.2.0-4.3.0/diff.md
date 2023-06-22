# Comparing `tmp/NGPIris-4.2.0.tar.gz` & `tmp/NGPIris-4.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NGPIris-4.2.0.tar", last modified: Thu Dec 22 13:38:50 2022, max compression
+gzip compressed data, was "NGPIris-4.3.0.tar", last modified: Thu Jun 22 14:22:47 2023, max compression
```

## Comparing `NGPIris-4.2.0.tar` & `NGPIris-4.3.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxr-x   0 xsylis    (1223) unix       (110)        0 2022-12-22 13:38:50.165717 NGPIris-4.2.0/
--rw-rw-r--   0 xsylis    (1223) unix       (110)    18093 2022-12-22 13:38:02.000000 NGPIris-4.2.0/LICENSE
--rw-rw-r--   0 xsylis    (1223) unix       (110)      247 2022-12-22 13:38:02.000000 NGPIris-4.2.0/MANIFEST.in
-drwxrwxr-x   0 xsylis    (1223) unix       (110)        0 2022-12-22 13:38:47.902714 NGPIris-4.2.0/NGPIris/
--rw-rw-r--   0 xsylis    (1223) unix       (110)      588 2022-12-22 13:38:02.000000 NGPIris-4.2.0/NGPIris/__init__.py
-drwxrwxr-x   0 xsylis    (1223) unix       (110)        0 2022-12-22 13:38:48.004703 NGPIris-4.2.0/NGPIris/cli/
--rw-rw-r--   0 xsylis    (1223) unix       (110)        0 2022-12-22 13:38:02.000000 NGPIris-4.2.0/NGPIris/cli/__init__.py
--rw-rw-r--   0 xsylis    (1223) unix       (110)     2122 2022-12-22 13:38:02.000000 NGPIris-4.2.0/NGPIris/cli/base.py
--rwxrwxr-x   0 xsylis    (1223) unix       (110)     5857 2022-12-22 13:38:02.000000 NGPIris-4.2.0/NGPIris/cli/functions.py
--rwxrwxr-x   0 xsylis    (1223) unix       (110)     1474 2022-12-22 13:38:02.000000 NGPIris-4.2.0/NGPIris/cli/utils.py
-drwxrwxr-x   0 xsylis    (1223) unix       (110)        0 2022-12-22 13:38:48.144732 NGPIris-4.2.0/NGPIris/hci/
--rwxrwxr-x   0 xsylis    (1223) unix       (110)       28 2022-12-22 13:38:02.000000 NGPIris-4.2.0/NGPIris/hci/__init__.py
--rwxrwxr-x   0 xsylis    (1223) unix       (110)     3245 2022-12-22 13:38:02.000000 NGPIris-4.2.0/NGPIris/hci/hci.py
--rwxrwxr-x   0 xsylis    (1223) unix       (110)      305 2022-12-22 13:38:02.000000 NGPIris-4.2.0/NGPIris/hci/template_query.json
-drwxrwxr-x   0 xsylis    (1223) unix       (110)        0 2022-12-22 13:38:48.219701 NGPIris-4.2.0/NGPIris/hcp/
--rw-rw-r--   0 xsylis    (1223) unix       (110)       28 2022-12-22 13:38:02.000000 NGPIris-4.2.0/NGPIris/hcp/__init__.py
--rw-rw-r--   0 xsylis    (1223) unix       (110)      443 2022-12-22 13:38:02.000000 NGPIris-4.2.0/NGPIris/hcp/config.py
--rw-rw-r--   0 xsylis    (1223) unix       (110)      735 2022-12-22 13:38:02.000000 NGPIris-4.2.0/NGPIris/hcp/errors.py
--rw-rw-r--   0 xsylis    (1223) unix       (110)    11052 2022-12-22 13:38:02.000000 NGPIris-4.2.0/NGPIris/hcp/hcp.py
--rw-rw-r--   0 xsylis    (1223) unix       (110)     1109 2022-12-22 13:38:02.000000 NGPIris-4.2.0/NGPIris/hcp/helpers.py
--rw-rw-r--   0 xsylis    (1223) unix       (110)     5322 2022-12-22 13:38:02.000000 NGPIris-4.2.0/NGPIris/hcp/interactive.py
-drwxrwxr-x   0 xsylis    (1223) unix       (110)        0 2022-12-22 13:38:48.314740 NGPIris-4.2.0/NGPIris/preproc/
--rw-rw-r--   0 xsylis    (1223) unix       (110)        0 2022-12-22 13:38:02.000000 NGPIris-4.2.0/NGPIris/preproc/__init__.py
--rwxrwxr-x   0 xsylis    (1223) unix       (110)     4856 2022-12-22 13:38:02.000000 NGPIris-4.2.0/NGPIris/preproc/preproc.py
-drwxrwxr-x   0 xsylis    (1223) unix       (110)        0 2022-12-22 13:38:47.946705 NGPIris-4.2.0/NGPIris.egg-info/
--rw-rw-r--   0 xsylis    (1223) unix       (110)     5935 2022-12-22 13:38:43.000000 NGPIris-4.2.0/NGPIris.egg-info/PKG-INFO
--rw-rw-r--   0 xsylis    (1223) unix       (110)      922 2022-12-22 13:38:43.000000 NGPIris-4.2.0/NGPIris.egg-info/SOURCES.txt
--rw-rw-r--   0 xsylis    (1223) unix       (110)        1 2022-12-22 13:38:43.000000 NGPIris-4.2.0/NGPIris.egg-info/dependency_links.txt
--rw-rw-r--   0 xsylis    (1223) unix       (110)       47 2022-12-22 13:38:43.000000 NGPIris-4.2.0/NGPIris.egg-info/entry_points.txt
--rw-rw-r--   0 xsylis    (1223) unix       (110)        1 2022-12-22 13:38:43.000000 NGPIris-4.2.0/NGPIris.egg-info/not-zip-safe
--rw-rw-r--   0 xsylis    (1223) unix       (110)       45 2022-12-22 13:38:43.000000 NGPIris-4.2.0/NGPIris.egg-info/requires.txt
--rw-rw-r--   0 xsylis    (1223) unix       (110)       14 2022-12-22 13:38:43.000000 NGPIris-4.2.0/NGPIris.egg-info/top_level.txt
--rw-rw-r--   0 xsylis    (1223) unix       (110)     5935 2022-12-22 13:38:50.166707 NGPIris-4.2.0/PKG-INFO
--rw-rw-r--   0 xsylis    (1223) unix       (110)     5314 2022-12-22 13:38:03.000000 NGPIris-4.2.0/README.md
--rw-rw-r--   0 xsylis    (1223) unix       (110)       76 2022-12-22 13:38:03.000000 NGPIris-4.2.0/config.ini
-drwxrwxr-x   0 xsylis    (1223) unix       (110)        0 2022-12-22 13:38:48.432731 NGPIris-4.2.0/docs/
--rw-rw-r--   0 xsylis    (1223) unix       (110)     2436 2022-12-22 13:38:03.000000 NGPIris-4.2.0/docs/package.md
--rw-rw-r--   0 xsylis    (1223) unix       (110)      268 2022-12-22 13:38:03.000000 NGPIris-4.2.0/pyproject.toml
-drwxrwxr-x   0 xsylis    (1223) unix       (110)        0 2022-12-22 13:38:48.680711 NGPIris-4.2.0/reference/
--rw-rw-r--   0 xsylis    (1223) unix       (110)     1577 2022-12-22 13:38:03.000000 NGPIris-4.2.0/reference/covidMetadataAllowedValues.csv
--rw-rw-r--   0 xsylis    (1223) unix       (110)      422 2022-12-22 13:38:03.000000 NGPIris-4.2.0/reference/covidMetadataTemplate.csv
--rw-rw-r--   0 xsylis    (1223) unix       (110)       45 2022-12-22 13:38:03.000000 NGPIris-4.2.0/requirements.txt
--rw-rw-r--   0 xsylis    (1223) unix       (110)      621 2022-12-22 13:38:50.168713 NGPIris-4.2.0/setup.cfg
--rw-rw-r--   0 xsylis    (1223) unix       (110)      788 2022-12-22 13:38:03.000000 NGPIris-4.2.0/setup.py
-drwxrwxr-x   0 xsylis    (1223) unix       (110)        0 2022-12-22 13:38:49.695719 NGPIris-4.2.0/tests/
--rw-rw-r--   0 xsylis    (1223) unix       (110)        0 2022-12-22 13:38:05.000000 NGPIris-4.2.0/tests/__init__.py
-drwxrwxr-x   0 xsylis    (1223) unix       (110)        0 2022-12-22 13:38:50.163729 NGPIris-4.2.0/tests/data/
--rw-rw-r--   0 xsylis    (1223) unix       (110)      137 2022-12-22 13:38:05.000000 NGPIris-4.2.0/tests/data/test.json
--rw-rw-r--   0 xsylis    (1223) unix       (110)    45392 2022-12-22 13:38:05.000000 NGPIris-4.2.0/tests/data/test_reads_R1.fasterq
--rw-rw-r--   0 xsylis    (1223) unix       (110)      134 2022-12-22 13:38:05.000000 NGPIris-4.2.0/tests/data/test_reads_R1.fastq.gz
--rw-rw-r--   0 xsylis    (1223) unix       (110)     3242 2022-12-22 13:38:05.000000 NGPIris-4.2.0/tests/test_cmds.py
--rwxrwxr-x   0 xsylis    (1223) unix       (110)     2061 2022-12-22 13:38:05.000000 NGPIris-4.2.0/tests/test_hcp.py
+drwxrwxr-x   0 xsylis    (1223) unix       (110)        0 2023-06-22 14:22:47.119092 NGPIris-4.3.0/
+-rw-rw-r--   0 xsylis    (1223) unix       (110)    18093 2023-06-21 07:42:22.000000 NGPIris-4.3.0/LICENSE
+-rw-rw-r--   0 xsylis    (1223) unix       (110)      247 2023-06-21 07:42:22.000000 NGPIris-4.3.0/MANIFEST.in
+drwxrwxr-x   0 xsylis    (1223) unix       (110)        0 2023-06-22 14:22:46.950092 NGPIris-4.3.0/NGPIris/
+-rw-rw-r--   0 xsylis    (1223) unix       (110)      588 2023-06-22 13:22:42.000000 NGPIris-4.3.0/NGPIris/__init__.py
+drwxrwxr-x   0 xsylis    (1223) unix       (110)        0 2023-06-22 14:22:47.012097 NGPIris-4.3.0/NGPIris/cli/
+-rw-rw-r--   0 xsylis    (1223) unix       (110)        0 2023-06-21 07:42:22.000000 NGPIris-4.3.0/NGPIris/cli/__init__.py
+-rw-rw-r--   0 xsylis    (1223) unix       (110)     2298 2023-06-22 13:49:17.000000 NGPIris-4.3.0/NGPIris/cli/base.py
+-rwxrwxr-x   0 xsylis    (1223) unix       (110)     5853 2023-06-22 14:21:11.000000 NGPIris-4.3.0/NGPIris/cli/functions.py
+-rwxrwxr-x   0 xsylis    (1223) unix       (110)     6433 2023-06-22 13:51:29.000000 NGPIris-4.3.0/NGPIris/cli/utils.py
+drwxrwxr-x   0 xsylis    (1223) unix       (110)        0 2023-06-22 14:22:47.030093 NGPIris-4.3.0/NGPIris/hci/
+-rwxrwxr-x   0 xsylis    (1223) unix       (110)       28 2023-06-21 07:42:22.000000 NGPIris-4.3.0/NGPIris/hci/__init__.py
+-rwxrwxr-x   0 xsylis    (1223) unix       (110)     3339 2023-06-21 07:42:22.000000 NGPIris-4.3.0/NGPIris/hci/hci.py
+-rwxrwxr-x   0 xsylis    (1223) unix       (110)      305 2023-06-21 07:42:22.000000 NGPIris-4.3.0/NGPIris/hci/template_query.json
+drwxrwxr-x   0 xsylis    (1223) unix       (110)        0 2023-06-22 14:22:47.066094 NGPIris-4.3.0/NGPIris/hcp/
+-rw-rw-r--   0 xsylis    (1223) unix       (110)       28 2023-06-21 07:42:22.000000 NGPIris-4.3.0/NGPIris/hcp/__init__.py
+-rw-rw-r--   0 xsylis    (1223) unix       (110)      443 2023-06-21 07:42:22.000000 NGPIris-4.3.0/NGPIris/hcp/config.py
+-rw-rw-r--   0 xsylis    (1223) unix       (110)      735 2023-06-21 07:42:22.000000 NGPIris-4.3.0/NGPIris/hcp/errors.py
+-rw-rw-r--   0 xsylis    (1223) unix       (110)    11190 2023-06-21 07:42:22.000000 NGPIris-4.3.0/NGPIris/hcp/hcp.py
+-rw-rw-r--   0 xsylis    (1223) unix       (110)     1109 2023-06-21 07:42:22.000000 NGPIris-4.3.0/NGPIris/hcp/helpers.py
+-rw-rw-r--   0 xsylis    (1223) unix       (110)     5603 2023-06-22 13:34:47.000000 NGPIris-4.3.0/NGPIris/hcp/interactive.py
+drwxrwxr-x   0 xsylis    (1223) unix       (110)        0 2023-06-22 14:22:47.074093 NGPIris-4.3.0/NGPIris/preproc/
+-rw-rw-r--   0 xsylis    (1223) unix       (110)        0 2023-06-21 07:42:22.000000 NGPIris-4.3.0/NGPIris/preproc/__init__.py
+-rwxrwxr-x   0 xsylis    (1223) unix       (110)     5451 2023-06-22 13:44:18.000000 NGPIris-4.3.0/NGPIris/preproc/preproc.py
+drwxrwxr-x   0 xsylis    (1223) unix       (110)        0 2023-06-22 14:22:46.988093 NGPIris-4.3.0/NGPIris.egg-info/
+-rw-rw-r--   0 xsylis    (1223) unix       (110)     6796 2023-06-22 14:22:46.000000 NGPIris-4.3.0/NGPIris.egg-info/PKG-INFO
+-rw-rw-r--   0 xsylis    (1223) unix       (110)      922 2023-06-22 14:22:46.000000 NGPIris-4.3.0/NGPIris.egg-info/SOURCES.txt
+-rw-rw-r--   0 xsylis    (1223) unix       (110)        1 2023-06-22 14:22:46.000000 NGPIris-4.3.0/NGPIris.egg-info/dependency_links.txt
+-rw-rw-r--   0 xsylis    (1223) unix       (110)       47 2023-06-22 14:22:46.000000 NGPIris-4.3.0/NGPIris.egg-info/entry_points.txt
+-rw-rw-r--   0 xsylis    (1223) unix       (110)        1 2023-06-21 07:42:53.000000 NGPIris-4.3.0/NGPIris.egg-info/not-zip-safe
+-rw-rw-r--   0 xsylis    (1223) unix       (110)       45 2023-06-22 14:22:46.000000 NGPIris-4.3.0/NGPIris.egg-info/requires.txt
+-rw-rw-r--   0 xsylis    (1223) unix       (110)       14 2023-06-22 14:22:46.000000 NGPIris-4.3.0/NGPIris.egg-info/top_level.txt
+-rw-rw-r--   0 xsylis    (1223) unix       (110)     6796 2023-06-22 14:22:47.120093 NGPIris-4.3.0/PKG-INFO
+-rw-rw-r--   0 xsylis    (1223) unix       (110)     6175 2023-06-22 14:21:11.000000 NGPIris-4.3.0/README.md
+-rw-rw-r--   0 xsylis    (1223) unix       (110)       76 2023-06-21 07:42:22.000000 NGPIris-4.3.0/config.ini
+drwxrwxr-x   0 xsylis    (1223) unix       (110)        0 2023-06-22 14:22:47.079093 NGPIris-4.3.0/docs/
+-rw-rw-r--   0 xsylis    (1223) unix       (110)     2436 2023-06-21 07:42:22.000000 NGPIris-4.3.0/docs/package.md
+-rw-rw-r--   0 xsylis    (1223) unix       (110)      268 2023-06-21 07:42:22.000000 NGPIris-4.3.0/pyproject.toml
+drwxrwxr-x   0 xsylis    (1223) unix       (110)        0 2023-06-22 14:22:47.090092 NGPIris-4.3.0/reference/
+-rw-rw-r--   0 xsylis    (1223) unix       (110)     1577 2023-06-21 07:42:22.000000 NGPIris-4.3.0/reference/covidMetadataAllowedValues.csv
+-rw-rw-r--   0 xsylis    (1223) unix       (110)      422 2023-06-21 07:42:22.000000 NGPIris-4.3.0/reference/covidMetadataTemplate.csv
+-rw-rw-r--   0 xsylis    (1223) unix       (110)       45 2023-06-21 07:42:22.000000 NGPIris-4.3.0/requirements.txt
+-rw-rw-r--   0 xsylis    (1223) unix       (110)      621 2023-06-22 14:22:47.123098 NGPIris-4.3.0/setup.cfg
+-rw-rw-r--   0 xsylis    (1223) unix       (110)      788 2023-06-21 07:42:22.000000 NGPIris-4.3.0/setup.py
+drwxrwxr-x   0 xsylis    (1223) unix       (110)        0 2023-06-22 14:22:47.102093 NGPIris-4.3.0/tests/
+-rw-rw-r--   0 xsylis    (1223) unix       (110)        0 2023-06-21 07:42:22.000000 NGPIris-4.3.0/tests/__init__.py
+drwxrwxr-x   0 xsylis    (1223) unix       (110)        0 2023-06-22 14:22:47.115093 NGPIris-4.3.0/tests/data/
+-rw-rw-r--   0 xsylis    (1223) unix       (110)      137 2023-06-21 07:42:22.000000 NGPIris-4.3.0/tests/data/test.json
+-rw-rw-r--   0 xsylis    (1223) unix       (110)    45392 2023-06-21 07:42:22.000000 NGPIris-4.3.0/tests/data/test_reads_R1.fasterq
+-rw-rw-r--   0 xsylis    (1223) unix       (110)      134 2023-06-21 07:42:22.000000 NGPIris-4.3.0/tests/data/test_reads_R1.fastq.gz
+-rw-rw-r--   0 xsylis    (1223) unix       (110)     3242 2023-06-21 07:42:22.000000 NGPIris-4.3.0/tests/test_cmds.py
+-rwxrwxr-x   0 xsylis    (1223) unix       (110)     2061 2023-06-21 07:42:22.000000 NGPIris-4.3.0/tests/test_hcp.py
```

### Comparing `NGPIris-4.2.0/LICENSE` & `NGPIris-4.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `NGPIris-4.2.0/NGPIris/__init__.py` & `NGPIris-4.3.0/NGPIris/__init__.py`

 * *Files identical despite different names*

### Comparing `NGPIris-4.2.0/NGPIris/cli/base.py` & `NGPIris-4.3.0/NGPIris/cli/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,32 +7,38 @@
 from NGPIris.hci import HCIManager
 from NGPIris.hcp.interactive import HCPInteracter
 from NGPIris.preproc import preproc
 from NGPIris.cli.functions import delete, search, upload, download
 from NGPIris.cli.utils import utils
 
 @click.group()
-@click.option('-c',"--credentials", help="File containing ep, id & key",type=click.Path(),required=True)
+@click.option('-c',"--credentials", help="File containing ep, id & key",type=click.Path())
 @click.option("-b","--bucket",help="Bucket name",type=str,required=True)
 @click.option("-ep","--endpoint",help="Endpoint URL override",type=str,default="")
 @click.option("-id","--access_key_id",help="Amazon key identifier override",type=str,default="")
 @click.option("-key","--access_key",help="Amazon secret access key override",type=str,default="")
 @click.option("-p","--password",help="NGPintelligence password", type=str, default="")
 @click.option("-l","--logfile",type=click.Path(),help="Logs activity to provided file",default="")
 @click.version_option()
 @click.pass_context
 def root(ctx, endpoint, access_key_id, access_key, bucket, credentials, password, logfile):
     """NGP intelligence and repository interface software"""
-    c = preproc.read_credentials(credentials)
+    if credentials:
+        c = preproc.read_credentials(credentials)
+    else:
+        c = {}
 
     ep = endpoint if endpoint else c.get('endpoint','')
     aid = access_key_id if access_key_id else c.get('aws_access_key_id','') 
     key = access_key if access_key else c.get('aws_secret_access_key','')
     pw = password if password else c.get('ngpi_password', '')
 
+    if not all([ep, aid, key]):
+        print("Missing essential HCP credentials. Please provide them manually or via a credentials file.")
+
     ctx.obj = {}
     hcpm = HCPManager(ep, aid, key, bucket=bucket)
     hcpm.attach_bucket(bucket)
     hcpm.test_connection()
     ctx.obj["hcpm"] = hcpm
     interact = HCPInteracter(hcpm)
     ctx.obj['interactive'] = interact
```

### Comparing `NGPIris-4.2.0/NGPIris/cli/functions.py` & `NGPIris-4.3.0/NGPIris/cli/functions.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,25 +26,25 @@
         if not (found_objs is None) and len(found_objs) > 0:
             for obj in found_objs:
                 log.info(obj.key)
         else:
             log.info(f'No results found for: {query}')
 
     elif mode == "ngpi":
-        hcim = ctx['hcim']
+        hcpi = ctx['hcpi']
 
-        hcim.create_template(index, query)
-        token = hcim.generate_token()
+        hcpi.create_template(index, query)
+        token = hcpi.generate_token()
 
         #if verbose:
-        #    resp = hcim.query(token)
+        #    resp = hcpi.query(token)
         #    pretty = json.loads(resp)
         #    click.secho(json.dumps(pretty, indent=4))
 
-        results = hcim.pretty_query(token)
+        results = hcpi.pretty_query(token)
         for item in results:
             md = item["metadata"]
             hci_name = md["HCI_displayName"]
             path = md["samples_Fastq_paths"]
             string = "".join(path).strip("[]").strip("{]}'")
             lst = string.replace('"','').replace("\\","").replace("[","").replace("]","").replace(";",",").split(",")
             log.info(f"Metadata file: {hci_name}")
@@ -64,19 +64,20 @@
 @click.command()
 @click.argument("input")
 @click.option('-o',"--output",help="Destination file name on HCP", default="")
 @click.option('-t',"--tag", default="None", help="Tag for downstream pipeline execution")
 @click.option('-m',"--meta",help="Local path for metadata file",default=f"")
 @click.option('-f',"--force",help="Overwrites any remote file with same name if present",is_flag=True, default=False)
 @click.option('-s',"--silent",help="Suppresses file progress output",is_flag=True,default=False)
-@click.option('-a',"--atypical",help="Allows upload of non-fastq file", is_flag=True,default=False)
+@click.option('-q',"--fastq",help="Verifies that files exclusively contain valid fastq", is_flag=True,default=False)
 @click.pass_obj
-def upload(ctx, input, output, tag, meta, force, silent,atypical):
-    """Upload fastq files / fastq folder structure"""
-    ctx['interactive'].upload_interactive(input, output, fastq_only=(not atypical), force=force, metadata=meta, silent=silent)
+def upload(ctx, input, output, tag, meta, force, silent,fastq):
+    """Upload a file or folder structure"""
+    ctx['interactive'].upload_interactive(input, output, fastq_only=fastq, force=force, metadata=meta, silent=silent)
+
 
 @click.command()
 @click.argument("query")
 @click.option('-o',"--output",help="Specify output file to write to",default="")
 @click.option("-m", "--mode",help="Search mode", type=click.Choice(['ngpi','ngpr','none','legacy-ngpi'], case_sensitive=False),default='ngpr')
 @click.option('-s',"--silent",help="Suppresses file progress output",is_flag=True,default=False)
 @click.option('-f',"--force",help="Overwrites any local file with same name if present",is_flag=True, default=False)
@@ -88,18 +89,18 @@
     if output == "":
         output = os.path.basename(query)
     #If output is folder. Default file name to input name
     elif output[-1] in ["/","\\"]:
         output = os.path.join(output, os.path.basename(query))
 
     if mode == "ngpi" or mode == "ngpi-legacy":
-        hcim = ctx['hcim']
-        hcim.create_template(index, query)
-        token = hcim.generate_token()
-        results = hcim.pretty_query(token)
+        hcpi = ctx['hcpi']
+        hcpi.create_template(index, query)
+        token = hcpi.generate_token()
+        results = hcpi.pretty_query(token)
 
         if mode == "ngpi-legacy":
             for item in results:
                 md = item["metadata"]
                 path = md["samples_Fastq_paths"]
             for i in path:
                 obj = ctx["hcpm"].get_object(i) # Get object with json.
```

### Comparing `NGPIris-4.2.0/NGPIris/hci/hci.py` & `NGPIris-4.3.0/NGPIris/hci/hci.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,26 +8,26 @@
 import requests
 import ast
 import json
 import os
 import sys
 import urllib3
 
-from NGPIris import WD
+from NGPIris import WD, log
 
 from NGPIris.preproc import preproc
 
 class HCIManager:
     
     def __init__(self,password="", credentials_path=""):
         if credentials_path:
             c = preproc.read_credentials(credentials_path)
 
         self.password = password if password else c('password','')
-        self.address = "10.248.192.3"
+        self.address = "10.81.222.13"
         self.authport = "8000"
         self.apiport = "8888"
 
     def get_password(self):
         return self.password
 
     def create_template(self, index, query):
@@ -42,15 +42,16 @@
 
 
     def generate_token(self):
         """Generate a security token from a password"""
         my_key = requests.post(f"https://{self.address}:{self.authport}/auth/oauth/", 
                  data={"grant_type": "password", "username": "admin", "password": f"{self.password}", "scope": "*",  
                  "client_secret": "hci-client", "client_id": "hci-client", "realm": "LOCAL"}, verify=False)
-            
+        if my_key.status_code == 401:
+            raise Exception("Invalid index password specified")
         return ast.literal_eval(my_key.text)["access_token"].lstrip()
 
 
     def query(self, token):
         """Queries the HCI using a token"""
         with open ("{}/hci/package.json".format(WD), "r") as signal:
             json_data = json.load(signal)
```

### Comparing `NGPIris-4.2.0/NGPIris/hcp/errors.py` & `NGPIris-4.3.0/NGPIris/hcp/errors.py`

 * *Files identical despite different names*

### Comparing `NGPIris-4.2.0/NGPIris/hcp/hcp.py` & `NGPIris-4.3.0/NGPIris/hcp/hcp.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,16 @@
         self._interval = 0.1
         self._speed = 0
         self._creation_time = time.time()
 
     def _calculate_speed(self):
         curr_time = time.time()
         if curr_time - self._interval > self._previous_time:
-            speed = (self._seen_so_far - self._previous_bytesize) / (curr_time - self._previous_time)
+            delta_time = curr_time - self._previous_time or 0.0001  # Avoid division by zero
+            speed = (self._seen_so_far - self._previous_bytesize) / delta_time
             self._speed = round(speed / (1024 ** 2), 2)
             self._previous_time = curr_time
             self._previous_bytesize = self._seen_so_far
 
         return self._speed
 
     def _trim_text(self, text):
@@ -93,15 +94,16 @@
             sys.stdout.flush()
 
     def __enter__(self):
         return self
 
     def __exit__(self, *args, **kwargs):
         print('')
-        avg_transfer_speed = self._size/(self._previous_time - self._creation_time)
+        delta_time = (self._previous_time - self._creation_time) or 0.0001  # Avoid division by zero
+        avg_transfer_speed = self._size/delta_time
         avg_transfer_speed_mb = avg_transfer_speed / 1_000_000
         rounded_speed = abs(round(avg_transfer_speed_mb, 2))
         if rounded_speed == 0.0:
             rounded_speed = "Inf."
         print(f'Average transfer speed {rounded_speed} MB/s')
```

### Comparing `NGPIris-4.2.0/NGPIris/hcp/helpers.py` & `NGPIris-4.3.0/NGPIris/hcp/helpers.py`

 * *Files identical despite different names*

### Comparing `NGPIris-4.2.0/NGPIris/hcp/interactive.py` & `NGPIris-4.3.0/NGPIris/hcp/interactive.py`

 * *Files 4% similar despite different names*

```diff
@@ -81,39 +81,46 @@
                         destination = os.path.join(destination, obj.key)
 
                     self.hcpm.download_file(obj, destination, force=force, callback=(not silent)) # Downloads file.
                     #log.info(f"Downloaded {obj.key}"
 
     def upload_interactive(self, source, destination="", fastq_only=False, metadata="", force=False, silent=False):
         """ Uploads a file/folder-of-files and verifies its content """
+
         file_lst = []
-        ###Sets destinations
-        #Defaults destination to source name
-        if destination == "":
-            destination = os.path.basename(source)
-        #If destination is folder. Default file name to source name
-        elif destination[-1] in ["/","\\"]:
-            destination = os.path.join(destination, os.path.basename(source))
+        if not os.path.isdir(source):
+            ###Sets destinations
+            #Defaults destination to source name
+            if destination == "":
+                destination = os.path.basename(source)
+            #If destination is folder. Default file name to source name
+            elif destination[-1] in ["/","\\"]:
+                destination = os.path.join(destination, os.path.basename(source))
+            #Run fastq verification
+            if fastq_only:
+                [file_lst, mdfile]=preproc.verify_upload_file(source, metadata=metadata)
 
         ###Verify fastq contents and metadata existence
-        if os.path.isdir(source) and fastq_only:
-            [file_lst, mdfile]=preproc.verify_upload_folder(source, metadata=metadata)
-        elif os.path.isdir(source):
-            [file_lst, mdfile]=preproc.folder_to_list(source, metadata=metadata)
-        elif fastq_only:
-            [file_lst, mdfile]=preproc.verify_upload_file(source, metadata=metadata)
+        elif os.path.isdir(source) and fastq_only:
+            [file_lst, out_lst, mdfile]=preproc.verify_upload_folder(source, metadata=metadata)
+        else:
+            [file_lst, out_lst, mdfile]=preproc.folder_to_list(source, metadata=metadata)
+
+        #Error if no valid fastq in valid fastq only mode
         if fastq_only and file_lst == []:
-            log.error(f"{source} could not be uploaded to NGPr. Try using an atypical (-a) upload")
+            log.error(f"{source} could not be uploaded to NGPr. Try disabling fastq (-q) upload")
 
+        #Upload folder
         if os.path.isdir(source):
-            pass
-            #for file_pg in file_lst:
-            #    self.hcpm.upload_file(file_pg, destination, force=force, callback=(not silent))
-            #    #time.sleep(2)
-            #    log.info(f"Uploaded: {file_pg}")
+            for file_pg in file_lst:
+                out_pg = out_lst[file_lst.index(file_pg)] #Find destination counterpart to file_pg
+                self.hcpm.upload_file(file_pg, out_pg, force=force, callback=(not silent))
+                #time.sleep(2)
+                log.info(f"Uploaded: {file_pg}")
+        #Upload file
         else:
             self.hcpm.upload_file(source, destination, force=force, callback=(not silent))
             #time.sleep(2)
             log.info(f"Uploaded: {destination}")
 
         #Upload metadata
         #dstfld = Path(destination)
```

### Comparing `NGPIris-4.2.0/NGPIris/preproc/preproc.py` & `NGPIris-4.3.0/NGPIris/preproc/preproc.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 """
 
 import csv
 import gzip
 import json
 import os
 import re
+import pathlib
 
 from NGPIris import log, WD, TIMESTAMP
 
 from NGPIris.hcp.errors import (UnattachedBucketError, LocalFileExistsError,
                                      UnknownSourceTypeError, MismatchChecksumError,
                                      ConnectionError, MissingCredentialsError)
 
@@ -91,49 +92,59 @@
 
     if c.get('endpoint') is None or c.get('aws_access_key_id') is None or c.get('aws_secret_access_key') is None:
         raise MissingCredentialsError('One or more values missing from provided json.')
         log.error('One or more critical values missing from provided json.')
         sys.exit(-1)
 
     if c.get('ngpi_password') is None:
-        log.warning('Credentials file lack NGPi credentials')
+        log.debug('Credentials file lack NGPi credentials')
 
     return c
 
 def folder_to_list(folder, metadata=""):
+    folder = pathlib.Path(os.path.abspath(os.path.normpath(folder))) #Input folder is now super-safe
     file_lst = []
+    out_lst = []
     md_lst= []
     #Recursively loop over all folders
     for root, dirs, files in os.walk(folder):
+        rshort = os.path.relpath(root, folder.parent)
         for f in files:
             try:
                 #Auto-generate metadata
                 #if metadata == "":
                 #    metadata = preproc.generate_tagmap(os.path.join(root,f), tag,"meta-{}.json".format(TIMESTAMP))
+                #log.debug(f"Dirs {dirs} Files {files}")
+                out_lst.append(os.path.join(rshort,f))
                 file_lst.append(os.path.join(root,f))
+                log.debug(f"Root {rshort} File {f}")
             except Exception as e:
                 log.warning(f"{f} is not a valid upload file: {e}")
-    return [file_lst, metadata]
+    return [file_lst, out_lst, metadata]
 
 def verify_upload_folder(folder, metadata=""):
+    folder = pathlib.Path(os.path.abspath(os.path.normpath(folder))) #Input folder is now super-safe
     file_lst = []
     md_lst= []
+    out_lst = []
     #Recursively loop over all folders
     for root, dirs, files in os.walk(folder):
+        rshort = os.path.relpath(root, folder.parent)
         for f in files:
             try:
                 verify_fq_suffix(os.path.join(root,f))
                 verify_fq_content(os.path.join(root,f))
                 #Auto-generate metadata
                 #if metadata == "":
                 #    metadata = preproc.generate_tagmap(os.path.join(root,f), tag,"meta-{}.json".format(TIMESTAMP))
                 file_lst.append(os.path.join(root,f))
+                out_lst.append(os.path.join(rshort,f))
             except Exception as e:
                 log.warning(f"{f} is not a valid upload file: {e}")
-    return [file_lst, metadata]
+    return [file_lst, out_lst, metadata]
 
 def verify_upload_file(source, metadata=""):
     source = os.path.abspath(source)
     dst = []
     try:
         verify_fq_suffix(source)
         verify_fq_content(source)
```

### Comparing `NGPIris-4.2.0/NGPIris.egg-info/PKG-INFO` & `NGPIris-4.3.0/NGPIris.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NGPIris
-Version: 4.2.0
+Version: 4.3.0
 Summary: "Iris is a light-weight tool for interacting with a Boto3 backed Hitachi Content Platform"
 Home-page: https://github.com/genomic-medicine-sweden/NGPIris
 Author: Isak Sylvin
 Author-email: Isak Sylvin <isak.sylvin@gu.se>
 Project-URL: Bug Tracker, https://github.com/genomic-medicine-sweden/NGPIris/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
@@ -83,55 +83,77 @@
   download  Download files using a given query
   search    List all file hits for a given query by directly calling HCP
   upload    Upload fastq files / fastq folder structure
   utils     Advanced commands for specific purposes
 ```
 
 #### Search for a file
-`iris -b BUCKETNAME -c CREDENTIALS_FILE search MYDU*TESTFILE --mode ngpr`
+`iris -b BUCKETNAME -c CREDENTIALS_FILE search "MYDU*TESTFILE" --mode ngpr`
 
 This command will search the bucket BUCKETNAME for the object `MYDU*TESTFILE`.  
 The search command supports both asterix (*) completion and most regex.  
 
 `--mode ngpr` uses the NGPr search mode to find this file. This is the slowest mode, but also the one that has existed the longest.  
 
+To list the contents the entire bucket, use the command `iris -b BUCKETNAME -c CREDENTIALS_FILE search "*" --mode ngpr`
+The ngpr mode will take long while to complete this process, which is why other modes are in development.
+
 #### Download a file
 `iris -b BUCKETNAME -c CREDENTIALS_FILE download /tmp/MYDUMBTESTFILE -o ./MYLOCALTESTFILE --silent --mode ngpr -f`
 
 This command will download your previously uploaded testfile, and put it in your current directory.  
 `--mode ngpr` uses the NGPr search mode to find this file. This is the slowest mode, but also the one that has existed the longest. 
 Alternatively use `--mode None` to skip searching for the file altogether. This is lightening fast. But requires the file name to be exactly correct.   
 `-f` will overwrite any locally stored file with the same name  
 `--silent` will remove the download progress bar. Which is sometimes useful when scripting  
 
 #### Upload a file
-`iris -b BUCKETNAME -c CREDENTIALS_FILE upload FILE2UPLOAD -o /tmp/MYDUMBTESTFILE -a -s`
+`iris -b BUCKETNAME -c CREDENTIALS_FILE upload FILE2UPLOAD -o /tmp/MYDUMBTESTFILE -s`
 
 This command will upload your test file as `MYDUMBTESTFILE` on the bucket BUCKETNAME.  
-`-a` allows non-fastq file formats.  
+`-q` verifies that only fastq files are uploaded
 `-s` removes the transfer speed info. Which can get very spammy in scripts.  
 
+`iris -b BUCKETNAME -c CREDENTIALS_FILE upload FOLDER2UPLOAD/`
+
+This command will upload your entire folder, its contents and the substructure.
+
 #### Delete a file
 `iris -b BUCKETNAME -c CREDENTIALS_FILE delete MYDUMBTESTFILE`
 
 This command will delete the file MYDUMBTESTFILE.  
 By default you will be prompted that you are certain that you wish to remove your file.  
 
 
 #### Additional commands
-`iris` contains more commands and flags for additional operations. Such as search, deleting, or doing things in a more nuanced way. The help menu packaged with the program is always kept up to date, so refer to that to easily discover more.
+
+`iris -c CREDENTIALS_FILE -b BUCKETNAME utils test-connection`
+
+This command tests if you can successfully connect to NGPRepository.  
+
+If it doesn't crash, it means you have correct credentials and an uninterrupted path to NGPRepository.
+
+`iris -c CREDENTIALS_FILE -b anything utils list-buckets`
+
+This command lists all the buckets of a tenent, that you at some point had admin access to. 
+Note that you do not need to provide a _valid_ bucketname for this command to successfully execute.
+
+
+`iris` contains more commands and flags for additional operations. The help menu packaged with the program is always kept up to date, so refer to that to easily discover more.
 
 For more use cases, check out [the CLI file](https://github.com/genomic-medicine-sweden/NGPIris/blob/master/NGPIris/cli/functions.py)
 
 ## As a package
 For usage of Iris as a package see the [package documentation](https://github.com/genomic-medicine-sweden/NGPIris/blob/master/docs/package.md)
 
 For an index of all HCPManager functionality, check out the [source file](https://github.com/genomic-medicine-sweden/NGPIris/blob/master/NGPIris/hcp/hcp.py)
 
 
-## Development build
+## Development installation
 ``` 
 git clone git@github.com:genomic-medicine-sweden/NGPIris.git
 cd NGPIris
-bash setup.sh iris
-source activate iris
+bash setup.sh ENVNAME
+source activate ENVNAME
+Edit credentials.json
+pytest tests/
 ```
```

### Comparing `NGPIris-4.2.0/NGPIris.egg-info/SOURCES.txt` & `NGPIris-4.3.0/NGPIris.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `NGPIris-4.2.0/PKG-INFO` & `NGPIris-4.3.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NGPIris
-Version: 4.2.0
+Version: 4.3.0
 Summary: "Iris is a light-weight tool for interacting with a Boto3 backed Hitachi Content Platform"
 Home-page: https://github.com/genomic-medicine-sweden/NGPIris
 Author: Isak Sylvin
 Author-email: Isak Sylvin <isak.sylvin@gu.se>
 Project-URL: Bug Tracker, https://github.com/genomic-medicine-sweden/NGPIris/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
@@ -83,55 +83,77 @@
   download  Download files using a given query
   search    List all file hits for a given query by directly calling HCP
   upload    Upload fastq files / fastq folder structure
   utils     Advanced commands for specific purposes
 ```
 
 #### Search for a file
-`iris -b BUCKETNAME -c CREDENTIALS_FILE search MYDU*TESTFILE --mode ngpr`
+`iris -b BUCKETNAME -c CREDENTIALS_FILE search "MYDU*TESTFILE" --mode ngpr`
 
 This command will search the bucket BUCKETNAME for the object `MYDU*TESTFILE`.  
 The search command supports both asterix (*) completion and most regex.  
 
 `--mode ngpr` uses the NGPr search mode to find this file. This is the slowest mode, but also the one that has existed the longest.  
 
+To list the contents the entire bucket, use the command `iris -b BUCKETNAME -c CREDENTIALS_FILE search "*" --mode ngpr`
+The ngpr mode will take long while to complete this process, which is why other modes are in development.
+
 #### Download a file
 `iris -b BUCKETNAME -c CREDENTIALS_FILE download /tmp/MYDUMBTESTFILE -o ./MYLOCALTESTFILE --silent --mode ngpr -f`
 
 This command will download your previously uploaded testfile, and put it in your current directory.  
 `--mode ngpr` uses the NGPr search mode to find this file. This is the slowest mode, but also the one that has existed the longest. 
 Alternatively use `--mode None` to skip searching for the file altogether. This is lightening fast. But requires the file name to be exactly correct.   
 `-f` will overwrite any locally stored file with the same name  
 `--silent` will remove the download progress bar. Which is sometimes useful when scripting  
 
 #### Upload a file
-`iris -b BUCKETNAME -c CREDENTIALS_FILE upload FILE2UPLOAD -o /tmp/MYDUMBTESTFILE -a -s`
+`iris -b BUCKETNAME -c CREDENTIALS_FILE upload FILE2UPLOAD -o /tmp/MYDUMBTESTFILE -s`
 
 This command will upload your test file as `MYDUMBTESTFILE` on the bucket BUCKETNAME.  
-`-a` allows non-fastq file formats.  
+`-q` verifies that only fastq files are uploaded
 `-s` removes the transfer speed info. Which can get very spammy in scripts.  
 
+`iris -b BUCKETNAME -c CREDENTIALS_FILE upload FOLDER2UPLOAD/`
+
+This command will upload your entire folder, its contents and the substructure.
+
 #### Delete a file
 `iris -b BUCKETNAME -c CREDENTIALS_FILE delete MYDUMBTESTFILE`
 
 This command will delete the file MYDUMBTESTFILE.  
 By default you will be prompted that you are certain that you wish to remove your file.  
 
 
 #### Additional commands
-`iris` contains more commands and flags for additional operations. Such as search, deleting, or doing things in a more nuanced way. The help menu packaged with the program is always kept up to date, so refer to that to easily discover more.
+
+`iris -c CREDENTIALS_FILE -b BUCKETNAME utils test-connection`
+
+This command tests if you can successfully connect to NGPRepository.  
+
+If it doesn't crash, it means you have correct credentials and an uninterrupted path to NGPRepository.
+
+`iris -c CREDENTIALS_FILE -b anything utils list-buckets`
+
+This command lists all the buckets of a tenent, that you at some point had admin access to. 
+Note that you do not need to provide a _valid_ bucketname for this command to successfully execute.
+
+
+`iris` contains more commands and flags for additional operations. The help menu packaged with the program is always kept up to date, so refer to that to easily discover more.
 
 For more use cases, check out [the CLI file](https://github.com/genomic-medicine-sweden/NGPIris/blob/master/NGPIris/cli/functions.py)
 
 ## As a package
 For usage of Iris as a package see the [package documentation](https://github.com/genomic-medicine-sweden/NGPIris/blob/master/docs/package.md)
 
 For an index of all HCPManager functionality, check out the [source file](https://github.com/genomic-medicine-sweden/NGPIris/blob/master/NGPIris/hcp/hcp.py)
 
 
-## Development build
+## Development installation
 ``` 
 git clone git@github.com:genomic-medicine-sweden/NGPIris.git
 cd NGPIris
-bash setup.sh iris
-source activate iris
+bash setup.sh ENVNAME
+source activate ENVNAME
+Edit credentials.json
+pytest tests/
 ```
```

### Comparing `NGPIris-4.2.0/README.md` & `NGPIris-4.3.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -68,55 +68,77 @@
   download  Download files using a given query
   search    List all file hits for a given query by directly calling HCP
   upload    Upload fastq files / fastq folder structure
   utils     Advanced commands for specific purposes
 ```
 
 #### Search for a file
-`iris -b BUCKETNAME -c CREDENTIALS_FILE search MYDU*TESTFILE --mode ngpr`
+`iris -b BUCKETNAME -c CREDENTIALS_FILE search "MYDU*TESTFILE" --mode ngpr`
 
 This command will search the bucket BUCKETNAME for the object `MYDU*TESTFILE`.  
 The search command supports both asterix (*) completion and most regex.  
 
 `--mode ngpr` uses the NGPr search mode to find this file. This is the slowest mode, but also the one that has existed the longest.  
 
+To list the contents the entire bucket, use the command `iris -b BUCKETNAME -c CREDENTIALS_FILE search "*" --mode ngpr`
+The ngpr mode will take long while to complete this process, which is why other modes are in development.
+
 #### Download a file
 `iris -b BUCKETNAME -c CREDENTIALS_FILE download /tmp/MYDUMBTESTFILE -o ./MYLOCALTESTFILE --silent --mode ngpr -f`
 
 This command will download your previously uploaded testfile, and put it in your current directory.  
 `--mode ngpr` uses the NGPr search mode to find this file. This is the slowest mode, but also the one that has existed the longest. 
 Alternatively use `--mode None` to skip searching for the file altogether. This is lightening fast. But requires the file name to be exactly correct.   
 `-f` will overwrite any locally stored file with the same name  
 `--silent` will remove the download progress bar. Which is sometimes useful when scripting  
 
 #### Upload a file
-`iris -b BUCKETNAME -c CREDENTIALS_FILE upload FILE2UPLOAD -o /tmp/MYDUMBTESTFILE -a -s`
+`iris -b BUCKETNAME -c CREDENTIALS_FILE upload FILE2UPLOAD -o /tmp/MYDUMBTESTFILE -s`
 
 This command will upload your test file as `MYDUMBTESTFILE` on the bucket BUCKETNAME.  
-`-a` allows non-fastq file formats.  
+`-q` verifies that only fastq files are uploaded
 `-s` removes the transfer speed info. Which can get very spammy in scripts.  
 
+`iris -b BUCKETNAME -c CREDENTIALS_FILE upload FOLDER2UPLOAD/`
+
+This command will upload your entire folder, its contents and the substructure.
+
 #### Delete a file
 `iris -b BUCKETNAME -c CREDENTIALS_FILE delete MYDUMBTESTFILE`
 
 This command will delete the file MYDUMBTESTFILE.  
 By default you will be prompted that you are certain that you wish to remove your file.  
 
 
 #### Additional commands
-`iris` contains more commands and flags for additional operations. Such as search, deleting, or doing things in a more nuanced way. The help menu packaged with the program is always kept up to date, so refer to that to easily discover more.
+
+`iris -c CREDENTIALS_FILE -b BUCKETNAME utils test-connection`
+
+This command tests if you can successfully connect to NGPRepository.  
+
+If it doesn't crash, it means you have correct credentials and an uninterrupted path to NGPRepository.
+
+`iris -c CREDENTIALS_FILE -b anything utils list-buckets`
+
+This command lists all the buckets of a tenent, that you at some point had admin access to. 
+Note that you do not need to provide a _valid_ bucketname for this command to successfully execute.
+
+
+`iris` contains more commands and flags for additional operations. The help menu packaged with the program is always kept up to date, so refer to that to easily discover more.
 
 For more use cases, check out [the CLI file](https://github.com/genomic-medicine-sweden/NGPIris/blob/master/NGPIris/cli/functions.py)
 
 ## As a package
 For usage of Iris as a package see the [package documentation](https://github.com/genomic-medicine-sweden/NGPIris/blob/master/docs/package.md)
 
 For an index of all HCPManager functionality, check out the [source file](https://github.com/genomic-medicine-sweden/NGPIris/blob/master/NGPIris/hcp/hcp.py)
 
 
-## Development build
+## Development installation
 ``` 
 git clone git@github.com:genomic-medicine-sweden/NGPIris.git
 cd NGPIris
-bash setup.sh iris
-source activate iris
+bash setup.sh ENVNAME
+source activate ENVNAME
+Edit credentials.json
+pytest tests/
 ```
```

### Comparing `NGPIris-4.2.0/docs/package.md` & `NGPIris-4.3.0/docs/package.md`

 * *Files identical despite different names*

### Comparing `NGPIris-4.2.0/reference/covidMetadataAllowedValues.csv` & `NGPIris-4.3.0/reference/covidMetadataAllowedValues.csv`

 * *Files identical despite different names*

### Comparing `NGPIris-4.2.0/setup.cfg` & `NGPIris-4.3.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = NGPIris
-version = 4.2.0
+version = 4.3.0
 description = "Iris is a light-weight tool for interacting with a Boto3 backed Hitachi Content Platform"
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/genomic-medicine-sweden/NGPIris
 author = Isak Sylvin
 author_email = isak.sylvin@gu.se
 project_urls =
```

### Comparing `NGPIris-4.2.0/setup.py` & `NGPIris-4.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `NGPIris-4.2.0/tests/data/test_reads_R1.fasterq` & `NGPIris-4.3.0/tests/data/test_reads_R1.fasterq`

 * *Files identical despite different names*

### Comparing `NGPIris-4.2.0/tests/test_cmds.py` & `NGPIris-4.3.0/tests/test_cmds.py`

 * *Files identical despite different names*

### Comparing `NGPIris-4.2.0/tests/test_hcp.py` & `NGPIris-4.3.0/tests/test_hcp.py`

 * *Files identical despite different names*

